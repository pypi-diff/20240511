# Comparing `tmp/matplotloom-0.3.0.tar.gz` & `tmp/matplotloom-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matplotloom-0.3.0.tar", max compression
+gzip compressed data, was "matplotloom-0.4.0.tar", max compression
```

## Comparing `matplotloom-0.3.0.tar` & `matplotloom-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2024-04-05 12:53:08.255332 matplotloom-0.3.0/LICENSE
--rw-r--r--   0        0        0       66 2024-04-05 12:53:08.255332 matplotloom-0.3.0/README.md
--rw-r--r--   0        0        0       23 2024-04-05 12:53:08.255332 matplotloom-0.3.0/matplotloom/__init__.py
--rw-r--r--   0        0        0     3393 2024-04-05 12:53:08.255332 matplotloom-0.3.0/matplotloom/loom.py
--rw-r--r--   0        0        0      439 2024-04-05 12:53:08.255332 matplotloom-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      760 1970-01-01 00:00:00.000000 matplotloom-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-11 15:42:31.805999 matplotloom-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4262 2024-05-11 15:42:31.805999 matplotloom-0.4.0/README.md
+-rw-r--r--   0        0        0       23 2024-05-11 15:42:31.809999 matplotloom-0.4.0/matplotloom/__init__.py
+-rw-r--r--   0        0        0     4111 2024-05-11 15:42:31.809999 matplotloom-0.4.0/matplotloom/loom.py
+-rw-r--r--   0        0        0      514 2024-05-11 15:42:31.809999 matplotloom-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4901 1970-01-01 00:00:00.000000 matplotloom-0.4.0/PKG-INFO
```

### Comparing `matplotloom-0.3.0/LICENSE` & `matplotloom-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `matplotloom-0.3.0/matplotloom/loom.py` & `matplotloom-0.4.0/matplotloom/loom.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,51 +13,67 @@
         self,
         output_filepath: Union[Path, str],
         frames_directory: Union[Path, str] = Path(TemporaryDirectory().name),
         fps: int = 30,
         keep_frames: bool = False,
         overwrite: bool = False,
         verbose: bool = False,
+        parallel: bool = False,
         savefig_kwargs: dict = {}
     ) -> None:
         self.output_filepath = Path(output_filepath)
         self.frames_directory = Path(frames_directory)
         self.fps = fps
         self.keep_frames = keep_frames
         self.overwrite = overwrite
         self.verbose = verbose
+        self.parallel = parallel
         self.savefig_kwargs = savefig_kwargs
         
+        if not self.parallel:
+            self.frame_counter = 0
+        else:
+            # We don't use the frame counter in parallel mode.
+            self.frame_counter = None
+
         self.frame_filepaths = []
-        self.frame_counter = 0
         self.file_format = self.output_filepath.suffix[1:]
 
         self.output_directory = self.output_filepath.parent
         self.output_directory.mkdir(parents=True, exist_ok=True)
         self.frames_directory.mkdir(parents=True, exist_ok=True)
 
         if self.verbose:
             print(f"output_filepath: {self.output_filepath}")
             print(f"frames_directory: {self.frames_directory}")
+        
+        if self.output_filepath.exists() and not self.overwrite:
+            raise FileExistsError(f"Output file '{self.output_filepath}' already exists. Set `overwrite=True` to overwrite the file.")
     
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.save_video()
         return
     
-    def save_frame(self, fig):
-        frame_filepath = self.frames_directory / f"frame_{self.frame_counter:06d}.png"
-
-        self.frame_counter += 1
+    def save_frame(self, fig, frame_number=None):
+        if not self.parallel:
+            frame_filepath = self.frames_directory / f"frame_{self.frame_counter:06d}.png"
+            self.frame_counter += 1
+        else:
+            frame_filepath = self.frames_directory / f"frame_{frame_number:06d}.png"
+        
         self.frame_filepaths.append(frame_filepath)
         
         if self.verbose:
-            print(f"Saving frame {self.frame_counter} to {frame_filepath}")
+            if not self.parallel:
+                print(f"Saving frame {self.frame_counter} to {frame_filepath}")
+            else:
+                print(f"Saving frame {frame_number} to {frame_filepath}")
         
         fig.savefig(frame_filepath, **self.savefig_kwargs)
         plt.close(fig)
 
     def save_video(self):
         if self.file_format == "mp4":
             command = [
```

