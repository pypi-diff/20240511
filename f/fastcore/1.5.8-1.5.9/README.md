# Comparing `tmp/fastcore-1.5.8.tar.gz` & `tmp/fastcore-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastcore-1.5.8.tar", last modified: Mon Jul 25 04:40:20 2022, max compression
+gzip compressed data, was "fastcore-1.5.9.tar", last modified: Mon Jul 25 18:21:04 2022, max compression
```

## Comparing `fastcore-1.5.8.tar` & `fastcore-1.5.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 jhoward   (1000) jhoward   (1000)        0 2022-07-25 04:40:20.802720 fastcore-1.5.8/
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     2348 2022-07-25 01:01:04.000000 fastcore-1.5.8/CONTRIBUTING.md
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    11357 2021-12-01 06:28:35.000000 fastcore-1.5.8/LICENSE
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)      111 2022-07-25 01:01:04.000000 fastcore-1.5.8/MANIFEST.in
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    16723 2022-07-25 04:40:20.802720 fastcore-1.5.8/PKG-INFO
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    15850 2022-07-25 04:21:03.000000 fastcore-1.5.8/README.md
-drwxrwxr-x   0 jhoward   (1000) jhoward   (1000)        0 2022-07-25 04:40:20.802720 fastcore-1.5.8/fastcore/
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)       22 2022-07-25 04:39:29.000000 fastcore-1.5.8/fastcore/__init__.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    47612 2022-07-25 04:39:29.000000 fastcore-1.5.8/fastcore/_modidx.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    12257 2022-07-25 04:09:00.000000 fastcore-1.5.8/fastcore/_nbdev.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)      247 2022-07-25 04:09:00.000000 fastcore-1.5.8/fastcore/all.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    38333 2022-07-25 04:39:29.000000 fastcore-1.5.8/fastcore/basics.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     7917 2022-07-25 04:39:29.000000 fastcore-1.5.8/fastcore/dispatch.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     6360 2022-07-25 04:39:29.000000 fastcore-1.5.8/fastcore/docments.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     8687 2022-07-25 04:09:00.000000 fastcore-1.5.8/fastcore/docscrape.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    12626 2022-07-25 04:39:29.000000 fastcore-1.5.8/fastcore/foundation.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     3748 2022-07-25 04:09:00.000000 fastcore-1.5.8/fastcore/imports.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     5816 2022-07-25 04:39:29.000000 fastcore-1.5.8/fastcore/meta.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)      204 2022-07-25 04:09:00.000000 fastcore-1.5.8/fastcore/nb_imports.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    11758 2022-07-25 04:39:29.000000 fastcore-1.5.8/fastcore/net.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     5886 2022-07-25 04:39:29.000000 fastcore-1.5.8/fastcore/parallel.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     5004 2022-07-25 04:39:29.000000 fastcore-1.5.8/fastcore/script.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)      666 2022-07-25 04:09:00.000000 fastcore-1.5.8/fastcore/shutil.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     3838 2022-07-25 04:39:29.000000 fastcore-1.5.8/fastcore/test.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     9737 2022-07-25 04:39:29.000000 fastcore-1.5.8/fastcore/transform.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)      117 2022-07-25 04:09:00.000000 fastcore-1.5.8/fastcore/utils.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    20793 2022-07-25 04:39:29.000000 fastcore-1.5.8/fastcore/xtras.py
-drwxrwxr-x   0 jhoward   (1000) jhoward   (1000)        0 2022-07-25 04:40:20.802720 fastcore-1.5.8/fastcore.egg-info/
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    16723 2022-07-25 04:40:20.000000 fastcore-1.5.8/fastcore.egg-info/PKG-INFO
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)      649 2022-07-25 04:40:20.000000 fastcore-1.5.8/fastcore.egg-info/SOURCES.txt
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)        1 2022-07-25 04:40:20.000000 fastcore-1.5.8/fastcore.egg-info/dependency_links.txt
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)        1 2021-12-01 18:23:34.000000 fastcore-1.5.8/fastcore.egg-info/not-zip-safe
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)       72 2022-07-25 04:40:20.000000 fastcore-1.5.8/fastcore.egg-info/requires.txt
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)        9 2022-07-25 04:40:20.000000 fastcore-1.5.8/fastcore.egg-info/top_level.txt
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)      639 2022-07-25 04:39:25.000000 fastcore-1.5.8/settings.ini
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)       38 2022-07-25 04:40:20.802720 fastcore-1.5.8/setup.cfg
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     2719 2022-07-25 04:09:00.000000 fastcore-1.5.8/setup.py
+drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2022-07-25 18:21:04.225325 fastcore-1.5.9/
+-rw-r--r--   0 jhoward    (501) staff       (20)     2348 2022-07-23 05:42:57.000000 fastcore-1.5.9/CONTRIBUTING.md
+-rw-r--r--   0 jhoward    (501) staff       (20)    11357 2022-07-23 05:42:57.000000 fastcore-1.5.9/LICENSE
+-rw-r--r--   0 jhoward    (501) staff       (20)      111 2022-07-23 05:42:57.000000 fastcore-1.5.9/MANIFEST.in
+-rw-r--r--   0 jhoward    (501) staff       (20)    16703 2022-07-25 18:21:04.225179 fastcore-1.5.9/PKG-INFO
+-rw-r--r--   0 jhoward    (501) staff       (20)    15850 2022-07-25 17:16:34.000000 fastcore-1.5.9/README.md
+drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2022-07-25 18:21:04.224349 fastcore-1.5.9/fastcore/
+-rw-r--r--   0 jhoward    (501) staff       (20)       22 2022-07-25 18:12:22.000000 fastcore-1.5.9/fastcore/__init__.py
+-rw-r--r--   0 jhoward    (501) staff       (20)    47722 2022-07-25 18:12:22.000000 fastcore-1.5.9/fastcore/_modidx.py
+-rw-r--r--   0 jhoward    (501) staff       (20)    12257 2022-07-23 05:42:57.000000 fastcore-1.5.9/fastcore/_nbdev.py
+-rw-r--r--   0 jhoward    (501) staff       (20)      247 2022-07-23 05:42:57.000000 fastcore-1.5.9/fastcore/all.py
+-rw-r--r--   0 jhoward    (501) staff       (20)    38333 2022-07-25 18:12:22.000000 fastcore-1.5.9/fastcore/basics.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     7917 2022-07-25 18:12:22.000000 fastcore-1.5.9/fastcore/dispatch.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     6360 2022-07-25 18:12:22.000000 fastcore-1.5.9/fastcore/docments.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     8687 2022-07-23 05:42:57.000000 fastcore-1.5.9/fastcore/docscrape.py
+-rw-r--r--   0 jhoward    (501) staff       (20)    12626 2022-07-25 18:12:22.000000 fastcore-1.5.9/fastcore/foundation.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     3748 2022-07-23 05:42:57.000000 fastcore-1.5.9/fastcore/imports.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     6058 2022-07-25 18:12:22.000000 fastcore-1.5.9/fastcore/meta.py
+-rw-r--r--   0 jhoward    (501) staff       (20)      204 2022-07-23 05:42:57.000000 fastcore-1.5.9/fastcore/nb_imports.py
+-rw-r--r--   0 jhoward    (501) staff       (20)    11758 2022-07-25 18:12:22.000000 fastcore-1.5.9/fastcore/net.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     6111 2022-07-25 18:12:22.000000 fastcore-1.5.9/fastcore/parallel.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     5004 2022-07-25 18:12:22.000000 fastcore-1.5.9/fastcore/script.py
+-rw-r--r--   0 jhoward    (501) staff       (20)      666 2022-07-23 05:42:57.000000 fastcore-1.5.9/fastcore/shutil.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     3838 2022-07-25 18:12:22.000000 fastcore-1.5.9/fastcore/test.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     9737 2022-07-25 18:12:22.000000 fastcore-1.5.9/fastcore/transform.py
+-rw-r--r--   0 jhoward    (501) staff       (20)      117 2022-07-23 05:42:57.000000 fastcore-1.5.9/fastcore/utils.py
+-rw-r--r--   0 jhoward    (501) staff       (20)    20793 2022-07-25 18:12:22.000000 fastcore-1.5.9/fastcore/xtras.py
+drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2022-07-25 18:21:04.225037 fastcore-1.5.9/fastcore.egg-info/
+-rw-r--r--   0 jhoward    (501) staff       (20)    16703 2022-07-25 18:21:03.000000 fastcore-1.5.9/fastcore.egg-info/PKG-INFO
+-rw-r--r--   0 jhoward    (501) staff       (20)      649 2022-07-25 18:21:04.000000 fastcore-1.5.9/fastcore.egg-info/SOURCES.txt
+-rw-r--r--   0 jhoward    (501) staff       (20)        1 2022-07-25 18:21:04.000000 fastcore-1.5.9/fastcore.egg-info/dependency_links.txt
+-rw-r--r--   0 jhoward    (501) staff       (20)        1 2022-07-23 05:43:11.000000 fastcore-1.5.9/fastcore.egg-info/not-zip-safe
+-rw-r--r--   0 jhoward    (501) staff       (20)       83 2022-07-25 18:21:04.000000 fastcore-1.5.9/fastcore.egg-info/requires.txt
+-rw-r--r--   0 jhoward    (501) staff       (20)        9 2022-07-25 18:21:04.000000 fastcore-1.5.9/fastcore.egg-info/top_level.txt
+-rw-r--r--   0 jhoward    (501) staff       (20)      650 2022-07-25 17:16:34.000000 fastcore-1.5.9/settings.ini
+-rw-r--r--   0 jhoward    (501) staff       (20)       38 2022-07-25 18:21:04.225358 fastcore-1.5.9/setup.cfg
+-rw-r--r--   0 jhoward    (501) staff       (20)     2736 2022-07-25 17:16:34.000000 fastcore-1.5.9/setup.py
```

### Comparing `fastcore-1.5.8/CONTRIBUTING.md` & `fastcore-1.5.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fastcore-1.5.8/LICENSE` & `fastcore-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fastcore-1.5.8/PKG-INFO` & `fastcore-1.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: fastcore
-Version: 1.5.8
+Version: 1.5.9
 Summary: Python supercharged for fastai development
 Home-page: https://github.com/fastai/fastcore/tree/master/
 Author: Jeremy Howard and Sylvain Gugger
 Author-email: infos@fast.ai
 License: Apache Software License 2.0
 Keywords: python
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -479,9 +478,7 @@
 Before submitting a PR, check that the local library and notebooks
 match. The script `nbdev_diff_nbs` can let you know if there is a
 difference between the local library and the notebooks. \* If you made a
 change to the notebooks in one of the exported cells, you can export it
 to the library with `nbdev_build_lib` or `make fastcore`. \* If you made
 a change to the library, you can export it back to the notebooks with
 `nbdev_update_lib`.
-
-
```

### Comparing `fastcore-1.5.8/README.md` & `fastcore-1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `fastcore-1.5.8/fastcore/_modidx.py` & `fastcore-1.5.9/fastcore/_modidx.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 d = { 'settings': { 'audience': 'Developers',
                 'author': 'Jeremy Howard and Sylvain Gugger',
                 'author_email': 'infos@fast.ai',
                 'branch': 'master',
                 'copyright': 'fast.ai',
                 'custom_sidebar': 'False',
                 'description': 'Python supercharged for fastai development',
-                'dev_requirements': 'numpy nbdev>=0.2.39 matplotlib pillow torch pandas',
+                'dev_requirements': 'numpy nbdev>=0.2.39 matplotlib pillow torch pandas jupyterlab',
                 'doc_baseurl': '/',
                 'doc_host': 'https://fastcore.fast.ai',
                 'doc_path': 'docs',
                 'doc_src_path': 'docs_src',
                 'git_url': 'https://github.com/fastai/fastcore/tree/master/',
                 'host': 'github',
                 'keywords': 'python',
@@ -20,15 +20,15 @@
                 'lib_path': 'fastcore',
                 'license': 'apache2',
                 'min_python': '3.7',
                 'nbs_path': 'nbs',
                 'status': '4',
                 'title': 'fastcore',
                 'user': 'fastai',
-                'version': '1.5.8'},
+                'version': '1.5.9'},
   'syms': { 'fastcore.all': {},
             'fastcore.basics': { 'fastcore.basics.AttrDict': 'https://fastcore.fast.ai/basics#AttrDict',
                                  'fastcore.basics.Float': 'https://fastcore.fast.ai/basics#Float',
                                  'fastcore.basics.GetAttr': 'https://fastcore.fast.ai/basics#GetAttr',
                                  'fastcore.basics.GetAttrBase': 'https://fastcore.fast.ai/basics#GetAttrBase',
                                  'fastcore.basics.ImportEnum': 'https://fastcore.fast.ai/basics#ImportEnum',
                                  'fastcore.basics.ImportEnum.imports': 'https://fastcore.fast.ai/basics#ImportEnum.imports',
@@ -249,15 +249,16 @@
                                   'fastcore.imports.is_iter': 'https://fastcore.fast.ai/imports#is_iter',
                                   'fastcore.imports.isinstance_str': 'https://fastcore.fast.ai/imports#isinstance_str',
                                   'fastcore.imports.noop': 'https://fastcore.fast.ai/imports#noop',
                                   'fastcore.imports.noops': 'https://fastcore.fast.ai/imports#noops',
                                   'fastcore.imports.remove_prefix': 'https://fastcore.fast.ai/imports#remove_prefix',
                                   'fastcore.imports.remove_suffix': 'https://fastcore.fast.ai/imports#remove_suffix',
                                   'fastcore.imports.string_classes': 'https://fastcore.fast.ai/imports#string_classes'},
-            'fastcore.meta': { 'fastcore.meta.BypassNewMeta': 'https://fastcore.fast.ai/meta#BypassNewMeta',
+            'fastcore.meta': { 'fastcore.meta.AutoInit': 'https://fastcore.fast.ai/meta#AutoInit',
+                               'fastcore.meta.BypassNewMeta': 'https://fastcore.fast.ai/meta#BypassNewMeta',
                                'fastcore.meta.FixSigMeta': 'https://fastcore.fast.ai/meta#FixSigMeta',
                                'fastcore.meta.NewChkMeta': 'https://fastcore.fast.ai/meta#NewChkMeta',
                                'fastcore.meta.PrePostInitMeta': 'https://fastcore.fast.ai/meta#PrePostInitMeta',
                                'fastcore.meta.anno_dict': 'https://fastcore.fast.ai/meta#anno_dict',
                                'fastcore.meta.delegates': 'https://fastcore.fast.ai/meta#delegates',
                                'fastcore.meta.empty2none': 'https://fastcore.fast.ai/meta#empty2none',
                                'fastcore.meta.funcs_kwargs': 'https://fastcore.fast.ai/meta#funcs_kwargs',
```

### Comparing `fastcore-1.5.8/fastcore/_nbdev.py` & `fastcore-1.5.9/fastcore/_nbdev.py`

 * *Files identical despite different names*

### Comparing `fastcore-1.5.8/fastcore/basics.py` & `fastcore-1.5.9/fastcore/basics.py`

 * *Files identical despite different names*

### Comparing `fastcore-1.5.8/fastcore/dispatch.py` & `fastcore-1.5.9/fastcore/dispatch.py`

 * *Files identical despite different names*

### Comparing `fastcore-1.5.8/fastcore/docments.py` & `fastcore-1.5.9/fastcore/docments.py`

 * *Files identical despite different names*

### Comparing `fastcore-1.5.8/fastcore/docscrape.py` & `fastcore-1.5.9/fastcore/docscrape.py`

 * *Files identical despite different names*

### Comparing `fastcore-1.5.8/fastcore/foundation.py` & `fastcore-1.5.9/fastcore/foundation.py`

 * *Files identical despite different names*

### Comparing `fastcore-1.5.8/fastcore/imports.py` & `fastcore-1.5.9/fastcore/imports.py`

 * *Files identical despite different names*

### Comparing `fastcore-1.5.8/fastcore/meta.py` & `fastcore-1.5.9/fastcore/meta.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/07_meta.ipynb.
 
 # %% auto 0
-__all__ = ['test_sig', 'FixSigMeta', 'PrePostInitMeta', 'NewChkMeta', 'BypassNewMeta', 'empty2none', 'anno_dict',
+__all__ = ['test_sig', 'FixSigMeta', 'PrePostInitMeta', 'AutoInit', 'NewChkMeta', 'BypassNewMeta', 'empty2none', 'anno_dict',
            'use_kwargs_dict', 'use_kwargs', 'delegates', 'method', 'funcs_kwargs']
 
 # %% ../nbs/07_meta.ipynb 1
 from .imports import *
 from .test import *
 from contextlib import contextmanager
 from copy import copy
@@ -37,14 +37,19 @@
         res = cls.__new__(cls)
         if type(res)==cls:
             if hasattr(res,'__pre_init__'): res.__pre_init__(*args,**kwargs)
             res.__init__(*args,**kwargs)
             if hasattr(res,'__post_init__'): res.__post_init__(*args,**kwargs)
         return res
 
+# %% ../nbs/07_meta.ipynb 28
+class AutoInit(metaclass=PrePostInitMeta):
+    "Same as `object`, but no need for subclasses to call `super().__init__`"
+    def __pre_init__(self, *args, **kwargs): super().__init__(*args, **kwargs)
+
 # %% ../nbs/07_meta.ipynb 31
 class NewChkMeta(FixSigMeta):
     "Metaclass to avoid recreating object passed to constructor"
     def __call__(cls, x=None, *args, **kwargs):
         if not args and not kwargs and x is not None and isinstance(x,cls): return x
         res = super().__call__(*((x,) + args), **kwargs)
         return res
```

### Comparing `fastcore-1.5.8/fastcore/net.py` & `fastcore-1.5.9/fastcore/net.py`

 * *Files identical despite different names*

### Comparing `fastcore-1.5.8/fastcore/parallel.py` & `fastcore-1.5.9/fastcore/parallel.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 # %% auto 0
 __all__ = ['threaded', 'startthread', 'parallelable', 'ThreadPoolExecutor', 'ProcessPoolExecutor', 'parallel', 'add_one',
            'run_procs', 'parallel_gen']
 
 # %% ../nbs/03a_parallel.ipynb 1
 from .imports import *
-from .foundation import *
 from .basics import *
+from .foundation import *
+from .meta import *
 from .xtras import *
 from functools import wraps
 
-from multiprocessing import Process, Queue
 import concurrent.futures,time
-from multiprocessing import Manager, set_start_method
+from multiprocessing import Process,Queue,Manager,set_start_method,get_all_start_methods,get_context
 from threading import Thread
 try:
     if sys.platform == 'darwin' and IN_NOTEBOOK: set_start_method("fork")
 except: pass
 
 # %% ../nbs/03a_parallel.ipynb 4
 def threaded(f):
@@ -69,14 +69,15 @@
         g = partial(f, *args, **kwargs)
         if self.not_parallel: return map(g, items)
         _g = partial(_call, self.lock, self.pause, self.max_workers, g)
         try: return super().map(_g, items, timeout=timeout, chunksize=chunksize)
         except Exception as e: self.on_exc(e)
 
 # %% ../nbs/03a_parallel.ipynb 12
+@delegates()
 class ProcessPoolExecutor(concurrent.futures.ProcessPoolExecutor):
     "Same as Python's ProcessPoolExecutor, except can pass `max_workers==0` for serial execution"
     def __init__(self, max_workers=defaults.cpus, on_exc=print, pause=0, **kwargs):
         if max_workers is None: max_workers=defaults.cpus
         store_attr()
         self.not_parallel = max_workers==0
         if self.not_parallel: max_workers=1
@@ -96,18 +97,23 @@
 
 # %% ../nbs/03a_parallel.ipynb 14
 try: from fastprogress import progress_bar
 except: progress_bar = None
 
 # %% ../nbs/03a_parallel.ipynb 15
 def parallel(f, items, *args, n_workers=defaults.cpus, total=None, progress=None, pause=0,
-             threadpool=False, timeout=None, chunksize=1, **kwargs):
+             method=None, threadpool=False, timeout=None, chunksize=1, **kwargs):
     "Applies `func` in parallel to `items`, using `n_workers`"
-    pool = ThreadPoolExecutor if threadpool else ProcessPoolExecutor
-    with pool(n_workers, pause=pause) as ex:
+    kwpool = {}
+    if threadpool: pool = ThreadPoolExecutor
+    else:
+        if not method and sys.platform == 'darwin': method='fork'
+        if method: kwpool['mp_context'] = get_context(method)
+        pool = ProcessPoolExecutor
+    with pool(n_workers, pause=pause, **kwpool) as ex:
         r = ex.map(f,items, *args, timeout=timeout, chunksize=chunksize, **kwargs)
         if progress and progress_bar:
             if total is None: total = len(items)
             r = progress_bar(r, total=total, leave=False)
         return L(r)
 
 # %% ../nbs/03a_parallel.ipynb 16
```

### Comparing `fastcore-1.5.8/fastcore/script.py` & `fastcore-1.5.9/fastcore/script.py`

 * *Files identical despite different names*

### Comparing `fastcore-1.5.8/fastcore/shutil.py` & `fastcore-1.5.9/fastcore/shutil.py`

 * *Files identical despite different names*

### Comparing `fastcore-1.5.8/fastcore/test.py` & `fastcore-1.5.9/fastcore/test.py`

 * *Files identical despite different names*

### Comparing `fastcore-1.5.8/fastcore/transform.py` & `fastcore-1.5.9/fastcore/transform.py`

 * *Files identical despite different names*

### Comparing `fastcore-1.5.8/fastcore/xtras.py` & `fastcore-1.5.9/fastcore/xtras.py`

 * *Files identical despite different names*

### Comparing `fastcore-1.5.8/fastcore.egg-info/PKG-INFO` & `fastcore-1.5.9/fastcore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: fastcore
-Version: 1.5.8
+Version: 1.5.9
 Summary: Python supercharged for fastai development
 Home-page: https://github.com/fastai/fastcore/tree/master/
 Author: Jeremy Howard and Sylvain Gugger
 Author-email: infos@fast.ai
 License: Apache Software License 2.0
 Keywords: python
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -479,9 +478,7 @@
 Before submitting a PR, check that the local library and notebooks
 match. The script `nbdev_diff_nbs` can let you know if there is a
 difference between the local library and the notebooks. \* If you made a
 change to the notebooks in one of the exported cells, you can export it
 to the library with `nbdev_build_lib` or `make fastcore`. \* If you made
 a change to the library, you can export it back to the notebooks with
 `nbdev_update_lib`.
-
-
```

### Comparing `fastcore-1.5.8/fastcore.egg-info/SOURCES.txt` & `fastcore-1.5.9/fastcore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastcore-1.5.8/settings.ini` & `fastcore-1.5.9/settings.ini`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 user = fastai
 description = Python supercharged for fastai development
 keywords = python
 author = Jeremy Howard and Sylvain Gugger
 author_email = infos@fast.ai
 copyright = fast.ai
 branch = master
-version = 1.5.8
+version = 1.5.9
 min_python = 3.7
 audience = Developers
 language = English
 custom_sidebar = False
 license = apache2
 status = 4
 nbs_path = nbs
 doc_path = docs
-dev_requirements = numpy nbdev>=0.2.39 matplotlib pillow torch pandas
+dev_requirements = numpy nbdev>=0.2.39 matplotlib pillow torch pandas jupyterlab
 git_url = https://github.com/fastai/fastcore/tree/master/
 lib_path = fastcore
 title = fastcore
 doc_host = https://fastcore.fast.ai
 doc_baseurl = /
 host = github
 doc_src_path = docs_src
```

### Comparing `fastcore-1.5.8/setup.py` & `fastcore-1.5.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 lic = licenses[cfg['license']]
 
 requirements = ['pip', 'packaging']
 if cfg.get('requirements'): requirements += cfg.get('requirements','').split()
 if cfg.get('pip_requirements'): requirements += cfg.get('pip_requirements','').split()
 dev_requirements = (cfg.get('dev_requirements') or '').split()
 
-long_description = open('README.md').read()
+long_description = open('README.md', encoding="utf8").read()
 # ![png](docs/images/output_13_0.png)
 for ext in ['png', 'svg']:
     long_description = re.sub(r'!\['+ext+'\]\((.*)\)', '!['+ext+']('+'https://raw.githubusercontent.com/{}/{}'.format(cfg['user'],cfg['lib_name'])+'/'+cfg['branch']+'/\\1)', long_description)
     long_description = re.sub(r'src=\"(.*)\.'+ext+'\"', 'src=\"https://raw.githubusercontent.com/{}/{}'.format(cfg['user'],cfg['lib_name'])+'/'+cfg['branch']+'/\\1.'+ext+'\"', long_description)
 
 setuptools.setup(
     name = 'fastcore',
```

