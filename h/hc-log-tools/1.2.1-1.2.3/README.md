# Comparing `tmp/hc_log_tools-1.2.1.tar.gz` & `tmp/hc_log_tools-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hc_log_tools-1.2.1.tar", last modified: Wed May  8 09:27:21 2024, max compression
+gzip compressed data, was "hc_log_tools-1.2.3.tar", last modified: Sat May 11 03:29:59 2024, max compression
```

## Comparing `hc_log_tools-1.2.1.tar` & `hc_log_tools-1.2.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 shixukai   (501) staff       (20)        0 2024-05-08 09:27:21.402740 hc_log_tools-1.2.1/
--rw-r--r--   0 shixukai   (501) staff       (20)     1074 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/LICENSE
--rw-r--r--   0 shixukai   (501) staff       (20)       24 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/MANIFEST.in
--rw-r--r--   0 shixukai   (501) staff       (20)     1658 2024-05-08 09:27:21.402540 hc_log_tools-1.2.1/PKG-INFO
--rw-r--r--   0 shixukai   (501) staff       (20)     1272 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/README.md
-drwxr-xr-x   0 shixukai   (501) staff       (20)        0 2024-05-08 09:27:21.402315 hc_log_tools-1.2.1/hc_log_tools.egg-info/
--rw-r--r--   0 shixukai   (501) staff       (20)     1658 2024-05-08 09:27:21.000000 hc_log_tools-1.2.1/hc_log_tools.egg-info/PKG-INFO
--rw-r--r--   0 shixukai   (501) staff       (20)      525 2024-05-08 09:27:21.000000 hc_log_tools-1.2.1/hc_log_tools.egg-info/SOURCES.txt
--rw-r--r--   0 shixukai   (501) staff       (20)        1 2024-05-08 09:27:21.000000 hc_log_tools-1.2.1/hc_log_tools.egg-info/dependency_links.txt
--rw-r--r--   0 shixukai   (501) staff       (20)       94 2024-05-08 09:27:21.000000 hc_log_tools-1.2.1/hc_log_tools.egg-info/requires.txt
--rw-r--r--   0 shixukai   (501) staff       (20)        9 2024-05-08 09:27:21.000000 hc_log_tools-1.2.1/hc_log_tools.egg-info/top_level.txt
--rw-r--r--   0 shixukai   (501) staff       (20)      365 2024-05-08 09:27:18.000000 hc_log_tools-1.2.1/pyproject.toml
--rw-r--r--   0 shixukai   (501) staff       (20)       94 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/requirements.txt
--rw-r--r--   0 shixukai   (501) staff       (20)       38 2024-05-08 09:27:21.402786 hc_log_tools-1.2.1/setup.cfg
--rw-r--r--   0 shixukai   (501) staff       (20)      719 2024-05-08 09:24:58.000000 hc_log_tools-1.2.1/setup.py
-drwxr-xr-x   0 shixukai   (501) staff       (20)        0 2024-05-08 09:27:21.401164 hc_log_tools-1.2.1/src/
--rw-r--r--   0 shixukai   (501) staff       (20)        0 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/src/__init__.py
--rw-r--r--   0 shixukai   (501) staff       (20)     1283 2024-05-08 09:24:58.000000 hc_log_tools-1.2.1/src/entry.py
--rw-r--r--   0 shixukai   (501) staff       (20)    18729 2024-05-08 09:24:58.000000 hc_log_tools-1.2.1/src/log_utility.py
--rw-r--r--   0 shixukai   (501) staff       (20)     5306 2024-05-08 09:24:58.000000 hc_log_tools-1.2.1/src/pack_log.py
--rw-r--r--   0 shixukai   (501) staff       (20)       39 2024-05-08 09:24:58.000000 hc_log_tools-1.2.1/src/public.py
--rw-r--r--   0 shixukai   (501) staff       (20)     3986 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/src/v_t_chart.py
-drwxr-xr-x   0 shixukai   (501) staff       (20)        0 2024-05-08 09:27:21.402135 hc_log_tools-1.2.1/test/
--rw-r--r--   0 shixukai   (501) staff       (20)        0 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/test/__init__.py
--rw-r--r--   0 shixukai   (501) staff       (20)     3537 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/test/test_log_download.py
--rw-r--r--   0 shixukai   (501) staff       (20)     1093 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/test/test_log_file_name_match.py
--rw-r--r--   0 shixukai   (501) staff       (20)     1946 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/test/test_log_utility.py
--rw-r--r--   0 shixukai   (501) staff       (20)      595 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/test/test_read_pick_data.py
--rw-r--r--   0 shixukai   (501) staff       (20)     2601 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/test/test_read_sort_data.py
--rw-r--r--   0 shixukai   (501) staff       (20)     3784 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/test/test_tiem_range.py
+drwxr-xr-x   0 shixukai   (501) staff       (20)        0 2024-05-11 03:29:59.460087 hc_log_tools-1.2.3/
+-rw-r--r--   0 shixukai   (501) staff       (20)     1074 2024-04-19 01:19:58.000000 hc_log_tools-1.2.3/LICENSE
+-rw-r--r--   0 shixukai   (501) staff       (20)       24 2024-04-19 01:19:58.000000 hc_log_tools-1.2.3/MANIFEST.in
+-rw-r--r--   0 shixukai   (501) staff       (20)     1658 2024-05-11 03:29:59.459831 hc_log_tools-1.2.3/PKG-INFO
+-rw-r--r--   0 shixukai   (501) staff       (20)     1272 2024-04-19 01:19:58.000000 hc_log_tools-1.2.3/README.md
+drwxr-xr-x   0 shixukai   (501) staff       (20)        0 2024-05-11 03:29:59.459557 hc_log_tools-1.2.3/hc_log_tools.egg-info/
+-rw-r--r--   0 shixukai   (501) staff       (20)     1658 2024-05-11 03:29:59.000000 hc_log_tools-1.2.3/hc_log_tools.egg-info/PKG-INFO
+-rw-r--r--   0 shixukai   (501) staff       (20)      525 2024-05-11 03:29:59.000000 hc_log_tools-1.2.3/hc_log_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 shixukai   (501) staff       (20)        1 2024-05-11 03:29:59.000000 hc_log_tools-1.2.3/hc_log_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 shixukai   (501) staff       (20)       94 2024-05-11 03:29:59.000000 hc_log_tools-1.2.3/hc_log_tools.egg-info/requires.txt
+-rw-r--r--   0 shixukai   (501) staff       (20)        9 2024-05-11 03:29:59.000000 hc_log_tools-1.2.3/hc_log_tools.egg-info/top_level.txt
+-rw-r--r--   0 shixukai   (501) staff       (20)      365 2024-05-11 03:29:57.000000 hc_log_tools-1.2.3/pyproject.toml
+-rw-r--r--   0 shixukai   (501) staff       (20)       94 2024-04-19 01:19:58.000000 hc_log_tools-1.2.3/requirements.txt
+-rw-r--r--   0 shixukai   (501) staff       (20)       38 2024-05-11 03:29:59.460145 hc_log_tools-1.2.3/setup.cfg
+-rw-r--r--   0 shixukai   (501) staff       (20)      719 2024-05-08 09:24:58.000000 hc_log_tools-1.2.3/setup.py
+drwxr-xr-x   0 shixukai   (501) staff       (20)        0 2024-05-11 03:29:59.457166 hc_log_tools-1.2.3/src/
+-rw-r--r--   0 shixukai   (501) staff       (20)        0 2024-04-19 01:19:58.000000 hc_log_tools-1.2.3/src/__init__.py
+-rw-r--r--   0 shixukai   (501) staff       (20)     1283 2024-05-08 09:24:58.000000 hc_log_tools-1.2.3/src/entry.py
+-rw-r--r--   0 shixukai   (501) staff       (20)    18729 2024-05-08 09:24:58.000000 hc_log_tools-1.2.3/src/log_utility.py
+-rw-r--r--   0 shixukai   (501) staff       (20)     6125 2024-05-11 03:28:19.000000 hc_log_tools-1.2.3/src/pack_log.py
+-rw-r--r--   0 shixukai   (501) staff       (20)       39 2024-05-08 09:24:58.000000 hc_log_tools-1.2.3/src/public.py
+-rw-r--r--   0 shixukai   (501) staff       (20)     3986 2024-04-19 01:19:58.000000 hc_log_tools-1.2.3/src/v_t_chart.py
+drwxr-xr-x   0 shixukai   (501) staff       (20)        0 2024-05-11 03:29:59.459066 hc_log_tools-1.2.3/test/
+-rw-r--r--   0 shixukai   (501) staff       (20)        0 2024-04-19 01:19:58.000000 hc_log_tools-1.2.3/test/__init__.py
+-rw-r--r--   0 shixukai   (501) staff       (20)     3537 2024-04-19 01:19:58.000000 hc_log_tools-1.2.3/test/test_log_download.py
+-rw-r--r--   0 shixukai   (501) staff       (20)     1093 2024-04-19 01:19:58.000000 hc_log_tools-1.2.3/test/test_log_file_name_match.py
+-rw-r--r--   0 shixukai   (501) staff       (20)     1946 2024-04-19 01:19:58.000000 hc_log_tools-1.2.3/test/test_log_utility.py
+-rw-r--r--   0 shixukai   (501) staff       (20)      595 2024-04-19 01:19:58.000000 hc_log_tools-1.2.3/test/test_read_pick_data.py
+-rw-r--r--   0 shixukai   (501) staff       (20)     2601 2024-04-19 01:19:58.000000 hc_log_tools-1.2.3/test/test_read_sort_data.py
+-rw-r--r--   0 shixukai   (501) staff       (20)     3784 2024-04-19 01:19:58.000000 hc_log_tools-1.2.3/test/test_tiem_range.py
```

### Comparing `hc_log_tools-1.2.1/LICENSE` & `hc_log_tools-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.1/PKG-INFO` & `hc_log_tools-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hc_log_tools
-Version: 1.2.1
+Version: 1.2.3
 Author-email: "xukai.sh" <shixukai@163.com>, "xukai.sh" <shixukai@163.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: alive_progress==2.4.1
 Requires-Dist: matplotlib==3.5.3
 Requires-Dist: pip>=20.0.2
```

### Comparing `hc_log_tools-1.2.1/README.md` & `hc_log_tools-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.1/hc_log_tools.egg-info/PKG-INFO` & `hc_log_tools-1.2.3/hc_log_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hc_log_tools
-Version: 1.2.1
+Version: 1.2.3
 Author-email: "xukai.sh" <shixukai@163.com>, "xukai.sh" <shixukai@163.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: alive_progress==2.4.1
 Requires-Dist: matplotlib==3.5.3
 Requires-Dist: pip>=20.0.2
```

### Comparing `hc_log_tools-1.2.1/hc_log_tools.egg-info/SOURCES.txt` & `hc_log_tools-1.2.3/hc_log_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.1/setup.py` & `hc_log_tools-1.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.1/src/entry.py` & `hc_log_tools-1.2.3/src/entry.py`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.1/src/log_utility.py` & `hc_log_tools-1.2.3/src/log_utility.py`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.1/src/v_t_chart.py` & `hc_log_tools-1.2.3/src/v_t_chart.py`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.1/test/test_log_download.py` & `hc_log_tools-1.2.3/test/test_log_download.py`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.1/test/test_log_file_name_match.py` & `hc_log_tools-1.2.3/test/test_log_file_name_match.py`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.1/test/test_log_utility.py` & `hc_log_tools-1.2.3/test/test_log_utility.py`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.1/test/test_read_pick_data.py` & `hc_log_tools-1.2.3/test/test_read_pick_data.py`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.1/test/test_read_sort_data.py` & `hc_log_tools-1.2.3/test/test_read_sort_data.py`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.1/test/test_tiem_range.py` & `hc_log_tools-1.2.3/test/test_tiem_range.py`

 * *Files identical despite different names*

