# Comparing `tmp/packaged-0.0.2.tar.gz` & `tmp/packaged-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packaged-0.0.2.tar", last modified: Wed May  8 23:11:05 2024, max compression
+gzip compressed data, was "packaged-0.1.0.tar", last modified: Fri May 10 11:08:21 2024, max compression
```

## Comparing `packaged-0.0.2.tar` & `packaged-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-08 23:11:05.971979 packaged-0.0.2/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1072 2024-05-04 21:39:47.000000 packaged-0.0.2/LICENSE
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1949 2024-05-08 23:11:05.971903 packaged-0.0.2/PKG-INFO
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      834 2024-05-08 23:07:10.000000 packaged-0.0.2/README.md
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1233 2024-05-08 23:11:05.972310 packaged-0.0.2/setup.cfg
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       37 2024-05-04 21:39:47.000000 packaged-0.0.2/setup.py
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-08 23:11:05.968805 packaged-0.0.2/src/
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-08 23:11:05.970142 packaged-0.0.2/src/packaged/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3431 2024-05-08 23:07:56.000000 packaged-0.0.2/src/packaged/__init__.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      184 2024-05-04 21:39:47.000000 packaged-0.0.2/src/packaged/__main__.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1308 2024-05-08 23:09:57.000000 packaged-0.0.2/src/packaged/cli.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       59 2024-05-04 21:39:47.000000 packaged-0.0.2/src/packaged/py.typed
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)        0 2024-05-08 21:00:51.000000 packaged-0.0.2/src/packaged/startup.template.sh
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-08 23:11:05.971344 packaged-0.0.2/src/packaged.egg-info/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1949 2024-05-08 23:11:05.000000 packaged-0.0.2/src/packaged.egg-info/PKG-INFO
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      379 2024-05-08 23:11:05.000000 packaged-0.0.2/src/packaged.egg-info/SOURCES.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)        1 2024-05-08 23:11:05.000000 packaged-0.0.2/src/packaged.egg-info/dependency_links.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       46 2024-05-08 23:11:05.000000 packaged-0.0.2/src/packaged.egg-info/entry_points.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       51 2024-05-08 23:11:05.000000 packaged-0.0.2/src/packaged.egg-info/requires.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)        9 2024-05-08 23:11:05.000000 packaged-0.0.2/src/packaged.egg-info/top_level.txt
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-10 11:08:21.354122 packaged-0.1.0/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1072 2024-05-04 21:39:47.000000 packaged-0.1.0/LICENSE
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2385 2024-05-10 11:08:21.354053 packaged-0.1.0/PKG-INFO
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1270 2024-05-09 19:03:38.000000 packaged-0.1.0/README.md
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1233 2024-05-10 11:08:21.354421 packaged-0.1.0/setup.cfg
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       37 2024-05-09 19:00:34.000000 packaged-0.1.0/setup.py
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-10 11:08:21.351313 packaged-0.1.0/src/
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-10 11:08:21.352647 packaged-0.1.0/src/packaged/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3778 2024-05-10 11:05:33.000000 packaged-0.1.0/src/packaged/__init__.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      184 2024-05-04 21:39:47.000000 packaged-0.1.0/src/packaged/__main__.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1308 2024-05-08 23:09:57.000000 packaged-0.1.0/src/packaged/cli.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       59 2024-05-04 21:39:47.000000 packaged-0.1.0/src/packaged/py.typed
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        0 2024-05-08 21:00:51.000000 packaged-0.1.0/src/packaged/startup.template.sh
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-10 11:08:21.353575 packaged-0.1.0/src/packaged.egg-info/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2385 2024-05-10 11:08:21.000000 packaged-0.1.0/src/packaged.egg-info/PKG-INFO
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      379 2024-05-10 11:08:21.000000 packaged-0.1.0/src/packaged.egg-info/SOURCES.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        1 2024-05-10 11:08:21.000000 packaged-0.1.0/src/packaged.egg-info/dependency_links.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       46 2024-05-10 11:08:21.000000 packaged-0.1.0/src/packaged.egg-info/entry_points.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       51 2024-05-10 11:08:21.000000 packaged-0.1.0/src/packaged.egg-info/requires.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        9 2024-05-10 11:08:21.000000 packaged-0.1.0/src/packaged.egg-info/top_level.txt
```

### Comparing `packaged-0.0.2/LICENSE` & `packaged-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `packaged-0.0.2/PKG-INFO` & `packaged-0.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packaged
-Version: 0.0.2
+Version: 0.1.0
 Summary: The easiest way to ship python applications.
 Home-page: https://github.com/tusharsadhwani/packaged
 Author: Tushar Sadhwani
 Author-email: tushar.sadhwani000@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -40,20 +40,41 @@
 
 ## Usage
 
 ```bash
 packaged <source_directory> <output_file> <build_command> <startup_command>
 ```
 
-For example:
+Such as:
 
 ```bash
 packaged path/to/project my_project.bin 'pip install .' 'python -m your_package'
 ```
 
+### Example
+
+There's an `example` folder where you can test this:
+
+```bash
+pip install packaged
+cd example
+packaged . curve 'pip install -r requirements.txt' 'python bubble_sort_curve.py'
+```
+
+This produces a `./curve` binary with:
+
+- Python 3.11
+- `matplotlib`
+- `numba`
+- `llvmlite`
+- `pillow`
+
+... and is directly executable. You can send this binary file to another machine
+with the same OS and architecture, and it will run the same.
+
 ## Local Development / Testing
 
 - Create and activate a virtual environment
 - Run `pip install -r requirements-dev.txt` to do an editable install
 - Run `pytest` to run tests
 
 ## Type Checking
```

### Comparing `packaged-0.0.2/setup.cfg` & `packaged-0.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = packaged
-version = 0.0.2
+version = 0.1.0
 description = The easiest way to ship python applications.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tusharsadhwani/packaged
 author = Tushar Sadhwani
 author_email = tushar.sadhwani000@gmail.com
 license = MIT
```

### Comparing `packaged-0.0.2/src/packaged/__init__.py` & `packaged-0.1.0/src/packaged/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,61 +38,70 @@
         [makeself_run_path, "--nox11"],
         stdout=subprocess.DEVNULL,
         stderr=subprocess.DEVNULL,
         cwd=MAKESELF_DOWNLOAD_PATH,
     )
 
 
-def create_package(source_directory, output_file, build_command, startup_command):
+def create_package(
+    source_directory: str, output_file: str, build_command: str, startup_command: str
+) -> None:
     """Create the makeself executable, with the startup script in it."""
-    package_name = os.path.basename(source_directory)
+    startup_script_name = "_packaged_startup.sh"
 
     packaged_python_path = os.path.join(source_directory, ".packaged_python")
     if os.path.exists(packaged_python_path):
         shutil.rmtree(packaged_python_path)
 
-    python_version, python_bin_path = yen.ensure_python("3.11")
-    python_path = os.path.join(yen.PYTHON_INSTALLS_PATH, python_version)
-    python_bin_relpath = os.path.relpath(python_bin_path, python_path)
-
-    # Copy python to the source directory
-    shutil.copytree(python_path, packaged_python_path)
-    # Get the bin folder path relative to source directory
-    python_bin_folder = os.path.join(
-        packaged_python_path, os.path.dirname(python_bin_relpath)
-    )
-    python_bin_folder_relpath = os.path.relpath(python_bin_folder, source_directory)
-
-    # Run the build command in the source directory, while making sure
-    # that `python` and related binaries point to the installed python
-    subprocess.check_call(
-        [build_command],
-        shell=True,
-        env={"PATH": os.pathsep.join([python_bin_folder, os.environ.get("PATH", "")])},
-    )
-
-    # copy the startup script to the source directory
-    startup_script_name = "_packaged_startup.sh"
-    startup_script_path = shutil.copyfile(
-        STARTUP_TEMPLATE_PATH, os.path.join(source_directory, startup_script_name)
-    )
-    # Add the startup command right at the end of the startup script
-    with open(startup_script_path, "a") as startup_file:
-        startup_file.write(f"PATH={python_bin_folder_relpath}:$PATH\n")
-        startup_file.write(startup_command)
-
-    os.chmod(startup_script_path, 0o777)
-
-    subprocess.check_call(
-        [
-            MAKESELF_PATH,
-            source_directory,
-            output_file,
-            output_file,
-            # makeself wants the startup script path to be a relative path
-            os.path.join(".", startup_script_name),
-        ],
-    )
-
-    # Cleanup the packaged python and startup script
-    os.remove(startup_script_path)
-    shutil.rmtree(packaged_python_path)
+    try:
+        python_version, python_bin_path = yen.ensure_python("3.11")
+        python_path = os.path.join(yen.PYTHON_INSTALLS_PATH, python_version)
+        python_bin_relpath = os.path.relpath(python_bin_path, python_path)
+
+        # Copy the startup script to the source directory
+        startup_script_path = shutil.copyfile(
+            STARTUP_TEMPLATE_PATH, os.path.join(source_directory, startup_script_name)
+        )
+
+        # Put a standalone python interpreter inside the package
+        shutil.copytree(python_path, packaged_python_path)
+
+        # Get the bin folder path relative to source directory
+        python_bin_folder = os.path.join(
+            packaged_python_path, os.path.dirname(python_bin_relpath)
+        )
+        python_bin_folder_relpath = os.path.relpath(python_bin_folder, source_directory)
+
+        # Run the build command in the source directory, while making sure
+        # that `python` and related binaries point to the installed python
+        subprocess.check_call(
+            [build_command],
+            shell=True,
+            env={
+                "PATH": os.pathsep.join([python_bin_folder, os.environ.get("PATH", "")])
+            },
+            cwd=source_directory,
+        )
+
+        # Add the startup command right at the end of the startup script
+        with open(startup_script_path, "a") as startup_file:
+            startup_file.write(f"PATH={python_bin_folder_relpath}:$PATH\n")
+            startup_file.write(startup_command)
+
+        os.chmod(startup_script_path, 0o777)
+
+        subprocess.check_call(
+            [
+                MAKESELF_PATH,
+                source_directory,
+                output_file,
+                output_file,
+                # makeself wants the startup script path to be a relative path
+                os.path.join(".", startup_script_name),
+            ],
+        )
+    finally:
+        # Cleanup the packaged python and startup script
+        if os.path.exists(startup_script_path):
+            os.remove(startup_script_path)
+        if os.path.exists(packaged_python_path):
+            shutil.rmtree(packaged_python_path)
```

### Comparing `packaged-0.0.2/src/packaged/cli.py` & `packaged-0.1.0/src/packaged/cli.py`

 * *Files identical despite different names*

### Comparing `packaged-0.0.2/src/packaged.egg-info/PKG-INFO` & `packaged-0.1.0/src/packaged.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packaged
-Version: 0.0.2
+Version: 0.1.0
 Summary: The easiest way to ship python applications.
 Home-page: https://github.com/tusharsadhwani/packaged
 Author: Tushar Sadhwani
 Author-email: tushar.sadhwani000@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -40,20 +40,41 @@
 
 ## Usage
 
 ```bash
 packaged <source_directory> <output_file> <build_command> <startup_command>
 ```
 
-For example:
+Such as:
 
 ```bash
 packaged path/to/project my_project.bin 'pip install .' 'python -m your_package'
 ```
 
+### Example
+
+There's an `example` folder where you can test this:
+
+```bash
+pip install packaged
+cd example
+packaged . curve 'pip install -r requirements.txt' 'python bubble_sort_curve.py'
+```
+
+This produces a `./curve` binary with:
+
+- Python 3.11
+- `matplotlib`
+- `numba`
+- `llvmlite`
+- `pillow`
+
+... and is directly executable. You can send this binary file to another machine
+with the same OS and architecture, and it will run the same.
+
 ## Local Development / Testing
 
 - Create and activate a virtual environment
 - Run `pip install -r requirements-dev.txt` to do an editable install
 - Run `pytest` to run tests
 
 ## Type Checking
```

