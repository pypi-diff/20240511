# Comparing `tmp/crepe-0.0.7.tar.gz` & `tmp/crepe-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/crepe-0.0.7.tar", last modified: Fri Jul 13 16:05:33 2018, max compression
+gzip compressed data, was "dist/crepe-0.0.9.tar", last modified: Fri Oct 18 03:39:52 2019, max compression
```

## Comparing `crepe-0.0.7.tar` & `crepe-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxrwxr-x   0 jongwook  (1000) jongwook  (1000)        0 2018-07-13 16:05:33.000000 crepe-0.0.7/
--rw-rw-r--   0 jongwook  (1000) jongwook  (1000)     9764 2018-07-13 16:05:33.000000 crepe-0.0.7/PKG-INFO
--rw-rw-r--   0 jongwook  (1000) jongwook  (1000)     7655 2018-07-13 16:03:14.000000 crepe-0.0.7/README.md
--rw-rw-r--   0 jongwook  (1000) jongwook  (1000)       38 2018-07-13 16:05:33.000000 crepe-0.0.7/setup.cfg
-drwxrwxr-x   0 jongwook  (1000) jongwook  (1000)        0 2018-07-13 16:05:33.000000 crepe-0.0.7/crepe.egg-info/
--rw-rw-r--   0 jongwook  (1000) jongwook  (1000)        6 2018-07-13 16:05:33.000000 crepe-0.0.7/crepe.egg-info/top_level.txt
--rw-rw-r--   0 jongwook  (1000) jongwook  (1000)     9764 2018-07-13 16:05:33.000000 crepe-0.0.7/crepe.egg-info/PKG-INFO
--rw-rw-r--   0 jongwook  (1000) jongwook  (1000)        1 2018-07-13 16:05:33.000000 crepe-0.0.7/crepe.egg-info/dependency_links.txt
--rw-rw-r--   0 jongwook  (1000) jongwook  (1000)      274 2018-07-13 16:05:33.000000 crepe-0.0.7/crepe.egg-info/SOURCES.txt
--rw-rw-r--   0 jongwook  (1000) jongwook  (1000)       42 2018-07-13 16:05:33.000000 crepe-0.0.7/crepe.egg-info/entry_points.txt
--rw-rw-r--   0 jongwook  (1000) jongwook  (1000)      156 2018-07-13 16:05:33.000000 crepe-0.0.7/crepe.egg-info/requires.txt
-drwxrwxr-x   0 jongwook  (1000) jongwook  (1000)        0 2018-07-13 16:05:33.000000 crepe-0.0.7/crepe/
--rw-rw-r--   0 jongwook  (1000) jongwook  (1000)    13579 2018-07-13 16:03:14.000000 crepe-0.0.7/crepe/core.py
--rw-rw-r--   0 jongwook  (1000) jongwook  (1000)      102 2018-07-13 16:03:14.000000 crepe-0.0.7/crepe/__main__.py
--rwxrwxr-x   0 jongwook  (1000) jongwook  (1000)      100 2018-07-13 16:03:14.000000 crepe-0.0.7/crepe/__init__.py
--rw-rw-r--   0 jongwook  (1000) jongwook  (1000)       18 2018-07-13 16:03:14.000000 crepe-0.0.7/crepe/version.py
--rw-rw-r--   0 jongwook  (1000) jongwook  (1000)     7872 2018-07-13 16:03:14.000000 crepe-0.0.7/crepe/cli.py
--rw-rw-r--   0 jongwook  (1000) jongwook  (1000)     2787 2018-07-13 16:03:14.000000 crepe-0.0.7/setup.py
+drwxr-xr-x   0 jongwook  (1000) jongwook  (1000)        0 2019-10-18 03:39:52.000000 crepe-0.0.9/
+-rw-r--r--   0 jongwook  (1000) jongwook  (1000)     1079 2019-10-18 02:51:46.000000 crepe-0.0.9/LICENSE
+-rw-r--r--   0 jongwook  (1000) jongwook  (1000)       88 2019-10-18 03:33:41.000000 crepe-0.0.9/MANIFEST.in
+-rw-r--r--   0 jongwook  (1000) jongwook  (1000)     9764 2019-10-18 03:39:52.000000 crepe-0.0.9/PKG-INFO
+-rw-r--r--   0 jongwook  (1000) jongwook  (1000)     7655 2019-10-18 02:51:46.000000 crepe-0.0.9/README.md
+drwxr-xr-x   0 jongwook  (1000) jongwook  (1000)        0 2019-10-18 03:39:52.000000 crepe-0.0.9/crepe/
+-rwxr-xr-x   0 jongwook  (1000) jongwook  (1000)      100 2019-10-18 02:51:46.000000 crepe-0.0.9/crepe/__init__.py
+-rw-r--r--   0 jongwook  (1000) jongwook  (1000)      102 2019-10-18 02:51:46.000000 crepe-0.0.9/crepe/__main__.py
+-rw-r--r--   0 jongwook  (1000) jongwook  (1000)     7872 2019-10-18 02:51:46.000000 crepe-0.0.9/crepe/cli.py
+-rw-r--r--   0 jongwook  (1000) jongwook  (1000)    13637 2019-10-18 03:19:30.000000 crepe-0.0.9/crepe/core.py
+-rw-r--r--   0 jongwook  (1000) jongwook  (1000)       18 2019-10-18 03:35:02.000000 crepe-0.0.9/crepe/version.py
+drwxr-xr-x   0 jongwook  (1000) jongwook  (1000)        0 2019-10-18 03:39:52.000000 crepe-0.0.9/crepe.egg-info/
+-rw-r--r--   0 jongwook  (1000) jongwook  (1000)     9764 2019-10-18 03:39:52.000000 crepe-0.0.9/crepe.egg-info/PKG-INFO
+-rw-r--r--   0 jongwook  (1000) jongwook  (1000)      311 2019-10-18 03:39:52.000000 crepe-0.0.9/crepe.egg-info/SOURCES.txt
+-rw-r--r--   0 jongwook  (1000) jongwook  (1000)        1 2019-10-18 03:39:52.000000 crepe-0.0.9/crepe.egg-info/dependency_links.txt
+-rw-r--r--   0 jongwook  (1000) jongwook  (1000)       42 2019-10-18 03:39:52.000000 crepe-0.0.9/crepe.egg-info/entry_points.txt
+-rw-r--r--   0 jongwook  (1000) jongwook  (1000)      159 2019-10-18 03:39:52.000000 crepe-0.0.9/crepe.egg-info/requires.txt
+-rw-r--r--   0 jongwook  (1000) jongwook  (1000)        6 2019-10-18 03:39:52.000000 crepe-0.0.9/crepe.egg-info/top_level.txt
+-rw-r--r--   0 jongwook  (1000) jongwook  (1000)      159 2019-10-18 03:19:30.000000 crepe-0.0.9/requirements.txt
+-rw-r--r--   0 jongwook  (1000) jongwook  (1000)       38 2019-10-18 03:39:52.000000 crepe-0.0.9/setup.cfg
+-rw-r--r--   0 jongwook  (1000) jongwook  (1000)     2729 2019-10-18 03:34:31.000000 crepe-0.0.9/setup.py
```

### Comparing `crepe-0.0.7/PKG-INFO` & `crepe-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crepe
-Version: 0.0.7
+Version: 0.0.9
 Summary: CREPE pitch tracker
 Home-page: https://github.com/marl/crepe
 Author: Jong Wook Kim and Justin Salamon
 Author-email: jongwook@nyu.edu
 License: MIT
 Project-URL: Source, https://github.com/marl/crepe
 Project-URL: Tracker, https://github.com/marl/crepe/issues
```

### Comparing `crepe-0.0.7/README.md` & `crepe-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `crepe-0.0.7/crepe.egg-info/PKG-INFO` & `crepe-0.0.9/crepe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crepe
-Version: 0.0.7
+Version: 0.0.9
 Summary: CREPE pitch tracker
 Home-page: https://github.com/marl/crepe
 Author: Jong Wook Kim and Justin Salamon
 Author-email: jongwook@nyu.edu
 License: MIT
 Project-URL: Source, https://github.com/marl/crepe
 Project-URL: Tracker, https://github.com/marl/crepe/issues
```

### Comparing `crepe-0.0.7/crepe/core.py` & `crepe-0.0.9/crepe/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import division
 from __future__ import print_function
 
 import os
 import re
 import sys
 
 from scipy.io import wavfile
@@ -20,33 +21,33 @@
 # the model is trained on 16kHz audio
 model_srate = 16000
 
 
 def build_and_load_model(model_capacity):
     """
     Build the CNN model and load the weights
-    
+
     Parameters
     ----------
     model_capacity : 'tiny', 'small', 'medium', 'large', or 'full'
         String specifying the model capacity, which determines the model's
         capacity multiplier to 4 (tiny), 8 (small), 16 (medium), 24 (large),
         or 32 (full). 'full' uses the model size specified in the paper,
         and the others use a reduced number of filters in each convolutional
         layer, resulting in a smaller model that is faster to evaluate at the
         cost of slightly reduced pitch estimation accuracy.
 
     Returns
     -------
-    model : keras.models.Model
+    model : tensorflow.keras.models.Model
         The pre-trained keras model loaded in memory
     """
-    from keras.layers import Input, Reshape, Conv2D, BatchNormalization
-    from keras.layers import MaxPool2D, Dropout, Permute, Flatten, Dense
-    from keras.models import Model
+    from tensorflow.keras.layers import Input, Reshape, Conv2D, BatchNormalization
+    from tensorflow.keras.layers import MaxPool2D, Dropout, Permute, Flatten, Dense
+    from tensorflow.keras.models import Model
 
     if models[model_capacity] is None:
         capacity_multiplier = {
             'tiny': 4, 'small': 8, 'medium': 16, 'large': 24, 'full': 32
         }[model_capacity]
 
         layers = [1, 2, 3, 4, 5, 6]
@@ -151,19 +152,19 @@
     return np.array([to_local_average_cents(salience[i, :], path[i]) for i in
                      range(len(observations))])
 
 
 def get_activation(audio, sr, model_capacity='full', center=True, step_size=10,
                    verbose=1):
     """
-    
+
     Parameters
     ----------
     audio : np.ndarray [shape=(N,) or (N, C)]
-        The audio samples. Multichannel audio will be downmixed. 
+        The audio samples. Multichannel audio will be downmixed.
     sr : int
         Sample rate of the audio samples. The audio will be resampled if
         the sample rate is not 16 kHz, which is expected by the model.
     model_capacity : 'tiny', 'small', 'medium', 'large', or 'full'
         String specifying the model capacity; see the docstring of
         :func:`~crepe.core.build_and_load_model`
     center : boolean
@@ -211,19 +212,19 @@
     return model.predict(frames, verbose=verbose)
 
 
 def predict(audio, sr, model_capacity='full',
             viterbi=False, center=True, step_size=10, verbose=1):
     """
     Perform pitch estimation on given audio
-    
+
     Parameters
     ----------
     audio : np.ndarray [shape=(N,) or (N, C)]
-        The audio samples. Multichannel audio will be downmixed. 
+        The audio samples. Multichannel audio will be downmixed.
     sr : int
         Sample rate of the audio samples. The audio will be resampled if
         the sample rate is not 16 kHz, which is expected by the model.
     model_capacity : 'tiny', 'small', 'medium', 'large', or 'full'
         String specifying the model capacity; see the docstring of
         :func:`~crepe.core.build_and_load_model`
     viterbi : bool
@@ -237,15 +238,15 @@
     verbose : int
         Set the keras verbosity mode: 1 (default) will print out a progress bar
         during prediction, 0 will suppress all non-error printouts.
 
     Returns
     -------
     A 4-tuple consisting of:
-    
+
         time: np.ndarray [shape=(T,)]
             The timestamps on which the pitch was estimated
         frequency: np.ndarray [shape=(T,)]
             The predicted pitch values in Hz
         confidence: np.ndarray [shape=(T,)]
             The confidence of voice activity, between 0 and 1
         activation: np.ndarray [shape=(T, 360)]
```

### Comparing `crepe-0.0.7/crepe/cli.py` & `crepe-0.0.9/crepe/cli.py`

 * *Files identical despite different names*

### Comparing `crepe-0.0.7/setup.py` & `crepe-0.0.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-import os
-import sys
 import bz2
 import imp
+import os
+import sys
+
+import pkg_resources
 from setuptools import setup, find_packages
 
 try:
     from urllib.request import urlretrieve
 except ImportError:
     from urllib import urlretrieve
 
@@ -63,21 +65,16 @@
     ],
     keywords='tfrecord',
     project_urls={
         'Source': 'https://github.com/marl/crepe',
         'Tracker': 'https://github.com/marl/crepe/issues'
     },
     install_requires=[
-        'keras==2.1.5',
-        'numpy>=1.14.0',
-        'scipy>=1.0.0',
-        'matplotlib>=2.1.0',
-        'resampy>=0.2.0,<0.3.0',
-        'h5py>=2.7.0,<3.0.0',
-        'hmmlearn>=0.2.0,<0.3.0',
-        'imageio>=2.3.0',
-        'scikit-learn>=0.16'
+        str(requirement)
+        for requirement in pkg_resources.parse_requirements(
+            open(os.path.join(os.path.dirname(__file__), "requirements.txt"))
+        )
     ],
     package_data={
         'crepe': weight_files
     },
 )
```

