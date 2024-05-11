# Comparing `tmp/soundtools-0.2.2.0.tar.gz` & `tmp/soundtools-0.2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soundtools-0.2.2.0.tar", last modified: Sun May  5 01:33:55 2024, max compression
+gzip compressed data, was "soundtools-0.2.2.1.tar", last modified: Sat May 11 05:10:22 2024, max compression
```

## Comparing `soundtools-0.2.2.0.tar` & `soundtools-0.2.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 01:33:55.540721 soundtools-0.2.2.0/
--rw-rw-rw-   0        0        0      701 2024-05-05 01:33:55.540721 soundtools-0.2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      224 2024-04-10 02:26:25.000000 soundtools-0.2.2.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-05 01:33:55.540721 soundtools-0.2.2.0/setup.cfg
--rw-rw-rw-   0        0        0      789 2024-05-05 01:33:25.000000 soundtools-0.2.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 01:33:55.536722 soundtools-0.2.2.0/soundtools/
--rw-rw-rw-   0        0        0      399 2024-05-05 01:33:20.000000 soundtools-0.2.2.0/soundtools/__init__.py
--rw-rw-rw-   0        0        0    33899 2024-05-05 01:31:59.000000 soundtools-0.2.2.0/soundtools/soundtools.py
-drwxrwxrwx   0        0        0        0 2024-05-05 01:33:55.539722 soundtools-0.2.2.0/soundtools.egg-info/
--rw-rw-rw-   0        0        0      701 2024-05-05 01:33:55.000000 soundtools-0.2.2.0/soundtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-05-05 01:33:55.000000 soundtools-0.2.2.0/soundtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 01:33:55.000000 soundtools-0.2.2.0/soundtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-05 01:33:55.000000 soundtools-0.2.2.0/soundtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-11 05:10:22.605748 soundtools-0.2.2.1/
+-rw-rw-rw-   0        0        0      701 2024-05-11 05:10:22.604749 soundtools-0.2.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2024-04-10 02:26:25.000000 soundtools-0.2.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-11 05:10:22.605748 soundtools-0.2.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      789 2024-05-11 05:10:00.000000 soundtools-0.2.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 05:10:22.602569 soundtools-0.2.2.1/soundtools/
+-rw-rw-rw-   0        0        0      399 2024-05-11 05:09:46.000000 soundtools-0.2.2.1/soundtools/__init__.py
+-rw-rw-rw-   0        0        0    34887 2024-05-11 05:09:43.000000 soundtools-0.2.2.1/soundtools/soundtools.py
+drwxrwxrwx   0        0        0        0 2024-05-11 05:10:22.604749 soundtools-0.2.2.1/soundtools.egg-info/
+-rw-rw-rw-   0        0        0      701 2024-05-11 05:10:22.000000 soundtools-0.2.2.1/soundtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-05-11 05:10:22.000000 soundtools-0.2.2.1/soundtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 05:10:22.000000 soundtools-0.2.2.1/soundtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-11 05:10:22.000000 soundtools-0.2.2.1/soundtools.egg-info/top_level.txt
```

### Comparing `soundtools-0.2.2.0/PKG-INFO` & `soundtools-0.2.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: soundtools
-Version: 0.2.2.0
+Version: 0.2.2.1
 Summary: used to work with sounds waves
 Author: Mohammad Erfan Karami
 Author-email: erfan012amir016@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 
 made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
-version: 0.2.2.0
+version: 0.2.2.1
 
 this package is used to create, play and save sound files
 it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
 and uses matplotlib to visualize the waves
```

### Comparing `soundtools-0.2.2.0/setup.py` & `soundtools-0.2.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 setup(
 name='soundtools',
-version='0.2.2.0',
+version='0.2.2.1',
 description="used to work with sounds waves",
 long_description="""made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
-version: 0.2.2.0
+version: 0.2.2.1
 
 this package is used to create, play and save sound files
 it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
 and uses matplotlib to visualize the waves""",
 author='Mohammad Erfan Karami',
```

### Comparing `soundtools-0.2.2.0/soundtools/soundtools.py` & `soundtools-0.2.2.1/soundtools/soundtools.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """### made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
-### version: 0.2.2.0
+### version: 0.2.2.1
 
 this package is used to create, play and save sound files
 it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
 and uses matplotlib to visualize the waves"""
 
@@ -222,39 +222,64 @@
     
     def _fix_amp(self, wave: SoundBuffer) -> SoundBuffer:
         wave[wave > self.max_amp] = self.max_amp
         wave[wave < self.min_amp] = self.min_amp
         return wave
     
     
-    def _generate_fade_buffer(self, fade_len:int = 1500, dtype: Dtype|None=None) -> SoundBuffer:
+    def _generate_fade_buffer(self, fade_len:int, dtype: Dtype|None=None) -> SoundBuffer:
         dtype = self.dtype if not dtype else dtype
         return ((1 - np.cos(np.linspace(0, np.pi, fade_len))) * 0.5).astype(dtype)
     
     
-    def fade_in(self, buffer: SoundBuffer, fadein_len:int = 1500) -> SoundBuffer:
+    def fade_in(self, buffer: SoundBuffer, fadein_len:int) -> SoundBuffer:
         fadein = self._generate_fade_buffer(fadein_len, buffer.dtype)
         buffer[:fadein_len] *= fadein
         return buffer
     
     
-    def fade_out(self, buffer: SoundBuffer, fadeout_len:int = 1500) -> SoundBuffer:
+    def fade_in_secs(self, buffer: SoundBuffer, secs: float, sample_rate:int|None=None) -> SoundBuffer:
+        if not sample_rate:
+            sample_rate = self.default_sample_rate
+        
+        fadein_nsamples = secs * sample_rate
+        return self.fade_in(buffer, fadein_nsamples)
+    
+    
+    def fade_out(self, buffer: SoundBuffer, fadeout_len:int) -> SoundBuffer:
         fadein = self._generate_fade_buffer(fadeout_len, buffer.dtype)
         fadeout = np.flip(fadein)
         buffer[-fadeout_len:] *= fadeout
         
         return buffer
     
     
-    def fade_in_out(self, buffer: SoundBuffer, fadein_len:int = 1500, fadeout_len:int = 1500) -> SoundBuffer:
+    def fade_out_secs(self, buffer: SoundBuffer, secs: float, sample_rate:int|None=None) -> SoundBuffer:
+        if not sample_rate:
+            sample_rate = self.default_sample_rate
+        
+        fadein_nsamples = secs * sample_rate
+        return self.fade_out(buffer, fadein_nsamples)
+    
+    
+    def fade_in_out(self, buffer: SoundBuffer, fadein_len:int, fadeout_len:int) -> SoundBuffer:
         buffer = self.fade_in(buffer, fadein_len)
         buffer = self.fade_out(buffer, fadeout_len)
         return buffer
     
     
+    def fade_in_out_secs(self, buffer: SoundBuffer, fadein_secs: float, fadeout_secs: float, sample_rate:int|None=None) -> SoundBuffer:
+        if not sample_rate:
+            sample_rate = self.default_sample_rate
+        
+        buffer = self.fade_in_secs(buffer, fadein_secs, sample_rate)
+        buffer = self.fade_out_secs(buffer, fadeout_secs, sample_rate)
+        return buffer
+    
+    
     def staccato(self, wave: SoundBuffer, play_time: float=0.75) -> SoundBuffer:
         playing = len(wave)*play_time
         resting = (1-play_time) * (wave.size/self.default_sample_rate)
         return np.append(wave[0:int(playing)], self.generate_note_buffer(0, self.sine_wave, resting))
     
     
     def array_to_tuple(self, np_array: SoundBuffer) -> tuple:
```

### Comparing `soundtools-0.2.2.0/soundtools.egg-info/PKG-INFO` & `soundtools-0.2.2.1/soundtools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: soundtools
-Version: 0.2.2.0
+Version: 0.2.2.1
 Summary: used to work with sounds waves
 Author: Mohammad Erfan Karami
 Author-email: erfan012amir016@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 
 made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
-version: 0.2.2.0
+version: 0.2.2.1
 
 this package is used to create, play and save sound files
 it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
 and uses matplotlib to visualize the waves
```

