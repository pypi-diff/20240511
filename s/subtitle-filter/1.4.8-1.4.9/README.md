# Comparing `tmp/subtitle-filter-1.4.8.tar.gz` & `tmp/subtitle-filter-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subtitle-filter-1.4.8.tar", last modified: Sun Oct 15 19:58:06 2023, max compression
+gzip compressed data, was "subtitle-filter-1.4.9.tar", last modified: Sat Mar  9 12:36:56 2024, max compression
```

## Comparing `subtitle-filter-1.4.8.tar` & `subtitle-filter-1.4.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 19:58:06.554737 subtitle-filter-1.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2023-10-15 19:57:57.000000 subtitle-filter-1.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2023-10-15 19:58:06.554737 subtitle-filter-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2023-10-15 19:57:57.000000 subtitle-filter-1.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-15 19:58:06.554737 subtitle-filter-1.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2023-10-15 19:57:57.000000 subtitle-filter-1.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 19:58:06.554737 subtitle-filter-1.4.8/subtitle_filter/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-10-15 19:57:57.000000 subtitle-filter-1.4.8/subtitle_filter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 19:58:06.554737 subtitle-filter-1.4.8/subtitle_filter/bin/
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2023-10-15 19:57:57.000000 subtitle-filter-1.4.8/subtitle_filter/bin/filter-subtitles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 19:58:06.554737 subtitle-filter-1.4.8/subtitle_filter/libs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-15 19:57:57.000000 subtitle-filter-1.4.8/subtitle_filter/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11694 2023-10-15 19:57:57.000000 subtitle-filter-1.4.8/subtitle_filter/libs/subtitle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 19:58:06.554737 subtitle-filter-1.4.8/subtitle_filter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2023-10-15 19:58:06.000000 subtitle-filter-1.4.8/subtitle_filter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      316 2023-10-15 19:58:06.000000 subtitle-filter-1.4.8/subtitle_filter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-15 19:58:06.000000 subtitle-filter-1.4.8/subtitle_filter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-10-15 19:58:06.000000 subtitle-filter-1.4.8/subtitle_filter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 12:36:56.595740 subtitle-filter-1.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-09 12:36:49.000000 subtitle-filter-1.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-03-09 12:36:56.595740 subtitle-filter-1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-03-09 12:36:49.000000 subtitle-filter-1.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-09 12:36:56.595740 subtitle-filter-1.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-03-09 12:36:49.000000 subtitle-filter-1.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 12:36:56.591740 subtitle-filter-1.4.9/subtitle_filter/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-09 12:36:49.000000 subtitle-filter-1.4.9/subtitle_filter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 12:36:56.595740 subtitle-filter-1.4.9/subtitle_filter/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-03-09 12:36:49.000000 subtitle-filter-1.4.9/subtitle_filter/bin/filter-subtitles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 12:36:56.595740 subtitle-filter-1.4.9/subtitle_filter/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 12:36:49.000000 subtitle-filter-1.4.9/subtitle_filter/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-03-09 12:36:49.000000 subtitle-filter-1.4.9/subtitle_filter/libs/subtitle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 12:36:56.595740 subtitle-filter-1.4.9/subtitle_filter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-03-09 12:36:56.000000 subtitle-filter-1.4.9/subtitle_filter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-09 12:36:56.000000 subtitle-filter-1.4.9/subtitle_filter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-09 12:36:56.000000 subtitle-filter-1.4.9/subtitle_filter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-09 12:36:56.000000 subtitle-filter-1.4.9/subtitle_filter.egg-info/top_level.txt
```

### Comparing `subtitle-filter-1.4.8/LICENSE` & `subtitle-filter-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `subtitle-filter-1.4.8/PKG-INFO` & `subtitle-filter-1.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: subtitle-filter
-Version: 1.4.8
+Version: 1.4.9
 Summary: Filter SDH entries and more from .srt files
 Home-page: https://github.com/mattlyon93/filter-subs
-Download-URL: https://github.com/mattlyon93/filter-subs/archive/v1.4.8.tar.gz
+Download-URL: https://github.com/mattlyon93/filter-subs/archive/v1.4.9.tar.gz
 Author: Matt Lyon
 Author-email: matthewlyon18@gmail.com
 License: MIT License
 Keywords: subtitle,SDH,hard-of-hearing,filter,movie,tv
 Classifier: Programming Language :: Python
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
```

### Comparing `subtitle-filter-1.4.8/README.md` & `subtitle-filter-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `subtitle-filter-1.4.8/setup.py` & `subtitle-filter-1.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 '''setup.py, use this to install module'''
 from os import path
 from setuptools import setup
 
-version = '1.4.8'
+version = '1.4.9'
 this_dir = path.abspath(path.dirname(__file__))
 with open(path.join(this_dir, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='subtitle-filter',
     version=version,
```

### Comparing `subtitle-filter-1.4.8/subtitle_filter/bin/filter-subtitles.py` & `subtitle-filter-1.4.9/subtitle_filter/bin/filter-subtitles.py`

 * *Files identical despite different names*

### Comparing `subtitle-filter-1.4.8/subtitle_filter/libs/subtitle.py` & `subtitle-filter-1.4.9/subtitle_filter/libs/subtitle.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         # Remove multi-line brackets
         self._contents = re.sub(r'[\(\[][\S\s]*[\)\]][\s:]*', '', self._contents)
         self._filter_empty()
 
     def replace_names(self):
         '''Replace names in all caps'''
         # Care is taken here to preserve genuine sentences with a colon.
-        NAME_REGEXP = r"([A-Z0-9 ][A-Z0-9' ]*: *|[A-Z]{1}[a-z]+ *: *)"
+        NAME_REGEXP = r"([A-Z0-9 ][A-Z0-9' ]*: *|[A-Z]{1}[a-z]+ *: *|^[A-Za-z]+: *)"
 
         names = re.findall(NAME_REGEXP, self._contents)
         # dialogues from different people preceeded with -
         # TODO: does this cover the case where the names are the same?
         replacement = '- ' if len(names) > 1 else ''
 
         def replace_if_not_hour(match):
```

### Comparing `subtitle-filter-1.4.8/subtitle_filter.egg-info/PKG-INFO` & `subtitle-filter-1.4.9/subtitle_filter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: subtitle-filter
-Version: 1.4.8
+Version: 1.4.9
 Summary: Filter SDH entries and more from .srt files
 Home-page: https://github.com/mattlyon93/filter-subs
-Download-URL: https://github.com/mattlyon93/filter-subs/archive/v1.4.8.tar.gz
+Download-URL: https://github.com/mattlyon93/filter-subs/archive/v1.4.9.tar.gz
 Author: Matt Lyon
 Author-email: matthewlyon18@gmail.com
 License: MIT License
 Keywords: subtitle,SDH,hard-of-hearing,filter,movie,tv
 Classifier: Programming Language :: Python
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
```

