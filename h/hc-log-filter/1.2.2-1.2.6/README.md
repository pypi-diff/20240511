# Comparing `tmp/hc_log_filter-1.2.2.tar.gz` & `tmp/hc_log_filter-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hc_log_filter-1.2.2.tar", last modified: Sat May 11 03:43:03 2024, max compression
+gzip compressed data, was "hc_log_filter-1.2.6.tar", last modified: Sat May 11 06:50:00 2024, max compression
```

## Comparing `hc_log_filter-1.2.2.tar` & `hc_log_filter-1.2.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 os         (501) staff       (20)        0 2024-05-11 03:43:03.785721 hc_log_filter-1.2.2/
--rw-r--r--   0 os         (501) staff       (20)     1074 2024-04-28 07:49:30.000000 hc_log_filter-1.2.2/LICENSE
--rw-r--r--   0 os         (501) staff       (20)       24 2024-04-28 07:49:30.000000 hc_log_filter-1.2.2/MANIFEST.in
--rw-r--r--   0 os         (501) staff       (20)     1673 2024-05-11 03:43:03.784622 hc_log_filter-1.2.2/PKG-INFO
--rw-r--r--   0 os         (501) staff       (20)     1272 2024-04-28 07:49:30.000000 hc_log_filter-1.2.2/README.md
-drwxr-xr-x   0 os         (501) staff       (20)        0 2024-05-11 03:43:03.783903 hc_log_filter-1.2.2/hc_log_filter.egg-info/
--rw-r--r--   0 os         (501) staff       (20)     1673 2024-05-11 03:43:03.000000 hc_log_filter-1.2.2/hc_log_filter.egg-info/PKG-INFO
--rw-r--r--   0 os         (501) staff       (20)      530 2024-05-11 03:43:03.000000 hc_log_filter-1.2.2/hc_log_filter.egg-info/SOURCES.txt
--rw-r--r--   0 os         (501) staff       (20)        1 2024-05-11 03:43:03.000000 hc_log_filter-1.2.2/hc_log_filter.egg-info/dependency_links.txt
--rw-r--r--   0 os         (501) staff       (20)       94 2024-05-11 03:43:03.000000 hc_log_filter-1.2.2/hc_log_filter.egg-info/requires.txt
--rw-r--r--   0 os         (501) staff       (20)        9 2024-05-11 03:43:03.000000 hc_log_filter-1.2.2/hc_log_filter.egg-info/top_level.txt
--rw-r--r--   0 os         (501) staff       (20)      380 2024-05-11 03:42:57.000000 hc_log_filter-1.2.2/pyproject.toml
--rw-r--r--   0 os         (501) staff       (20)       94 2024-04-28 07:49:30.000000 hc_log_filter-1.2.2/requirements.txt
--rw-r--r--   0 os         (501) staff       (20)       38 2024-05-11 03:43:03.785885 hc_log_filter-1.2.2/setup.cfg
--rw-r--r--   0 os         (501) staff       (20)      749 2024-04-28 07:49:30.000000 hc_log_filter-1.2.2/setup.py
-drwxr-xr-x   0 os         (501) staff       (20)        0 2024-05-11 03:43:03.779725 hc_log_filter-1.2.2/src/
--rw-r--r--   0 os         (501) staff       (20)        0 2024-04-28 07:49:30.000000 hc_log_filter-1.2.2/src/__init__.py
--rw-r--r--   0 os         (501) staff       (20)     1318 2024-04-30 07:46:05.000000 hc_log_filter-1.2.2/src/entry.py
--rw-r--r--   0 os         (501) staff       (20)    18729 2024-04-30 08:11:09.000000 hc_log_filter-1.2.2/src/log_utility.py
--rw-r--r--   0 os         (501) staff       (20)     6125 2024-05-10 05:47:31.000000 hc_log_filter-1.2.2/src/pack_log.py
--rw-r--r--   0 os         (501) staff       (20)       39 2024-04-30 03:52:15.000000 hc_log_filter-1.2.2/src/public.py
--rw-r--r--   0 os         (501) staff       (20)     3986 2024-04-28 07:49:30.000000 hc_log_filter-1.2.2/src/v_t_chart.py
-drwxr-xr-x   0 os         (501) staff       (20)        0 2024-05-11 03:43:03.783220 hc_log_filter-1.2.2/test/
--rw-r--r--   0 os         (501) staff       (20)        0 2024-04-28 07:49:30.000000 hc_log_filter-1.2.2/test/__init__.py
--rw-r--r--   0 os         (501) staff       (20)     3537 2024-04-28 07:49:30.000000 hc_log_filter-1.2.2/test/test_log_download.py
--rw-r--r--   0 os         (501) staff       (20)     1093 2024-04-28 07:49:30.000000 hc_log_filter-1.2.2/test/test_log_file_name_match.py
--rw-r--r--   0 os         (501) staff       (20)     1946 2024-04-28 07:49:30.000000 hc_log_filter-1.2.2/test/test_log_utility.py
--rw-r--r--   0 os         (501) staff       (20)      595 2024-04-28 07:49:30.000000 hc_log_filter-1.2.2/test/test_read_pick_data.py
--rw-r--r--   0 os         (501) staff       (20)     2601 2024-04-28 07:49:30.000000 hc_log_filter-1.2.2/test/test_read_sort_data.py
--rw-r--r--   0 os         (501) staff       (20)     3784 2024-04-28 07:49:30.000000 hc_log_filter-1.2.2/test/test_tiem_range.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 06:50:00.981078 hc_log_filter-1.2.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2024-05-11 04:32:33.000000 hc_log_filter-1.2.6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-11 04:32:33.000000 hc_log_filter-1.2.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1673 2024-05-11 06:50:00.981078 hc_log_filter-1.2.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1272 2024-05-11 04:32:33.000000 hc_log_filter-1.2.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 06:50:00.977078 hc_log_filter-1.2.6/hc_log_filter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1673 2024-05-11 06:50:00.000000 hc_log_filter-1.2.6/hc_log_filter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      530 2024-05-11 06:50:00.000000 hc_log_filter-1.2.6/hc_log_filter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 06:50:00.000000 hc_log_filter-1.2.6/hc_log_filter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       94 2024-05-11 06:50:00.000000 hc_log_filter-1.2.6/hc_log_filter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-11 06:50:00.000000 hc_log_filter-1.2.6/hc_log_filter.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      396 2024-05-11 06:49:53.000000 hc_log_filter-1.2.6/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       94 2024-05-11 04:32:33.000000 hc_log_filter-1.2.6/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-11 06:50:00.981078 hc_log_filter-1.2.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      749 2024-05-11 04:32:33.000000 hc_log_filter-1.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 06:50:00.977078 hc_log_filter-1.2.6/src/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 06:48:03.000000 hc_log_filter-1.2.6/src/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1318 2024-05-11 04:32:33.000000 hc_log_filter-1.2.6/src/entry.py
+-rw-rw-rw-   0 root         (0) root         (0)    18729 2024-05-11 04:32:33.000000 hc_log_filter-1.2.6/src/log_utility.py
+-rw-rw-rw-   0 root         (0) root         (0)     6125 2024-05-11 04:32:33.000000 hc_log_filter-1.2.6/src/pack_log.py
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-11 04:32:33.000000 hc_log_filter-1.2.6/src/public.py
+-rw-rw-rw-   0 root         (0) root         (0)     3986 2024-05-11 04:32:33.000000 hc_log_filter-1.2.6/src/v_t_chart.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 06:50:00.977078 hc_log_filter-1.2.6/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 06:48:03.000000 hc_log_filter-1.2.6/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3537 2024-05-11 04:32:33.000000 hc_log_filter-1.2.6/test/test_log_download.py
+-rw-rw-rw-   0 root         (0) root         (0)     1093 2024-05-11 04:32:33.000000 hc_log_filter-1.2.6/test/test_log_file_name_match.py
+-rw-rw-rw-   0 root         (0) root         (0)     1946 2024-05-11 04:32:33.000000 hc_log_filter-1.2.6/test/test_log_utility.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2024-05-11 04:32:33.000000 hc_log_filter-1.2.6/test/test_read_pick_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2601 2024-05-11 04:32:33.000000 hc_log_filter-1.2.6/test/test_read_sort_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3784 2024-05-11 04:32:33.000000 hc_log_filter-1.2.6/test/test_tiem_range.py
```

### Comparing `hc_log_filter-1.2.2/LICENSE` & `hc_log_filter-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hc_log_filter-1.2.2/PKG-INFO` & `hc_log_filter-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hc_log_filter
-Version: 1.2.2
+Version: 1.2.6
 Author-email: "xukai.shi" <xukai.shi@hcrobots.com>, "xukai.shi" <xukai.shi@hcrobots.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: alive_progress==2.4.1
 Requires-Dist: matplotlib==3.5.3
 Requires-Dist: pip>=20.0.2
```

### Comparing `hc_log_filter-1.2.2/README.md` & `hc_log_filter-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `hc_log_filter-1.2.2/hc_log_filter.egg-info/PKG-INFO` & `hc_log_filter-1.2.6/hc_log_filter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hc_log_filter
-Version: 1.2.2
+Version: 1.2.6
 Author-email: "xukai.shi" <xukai.shi@hcrobots.com>, "xukai.shi" <xukai.shi@hcrobots.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: alive_progress==2.4.1
 Requires-Dist: matplotlib==3.5.3
 Requires-Dist: pip>=20.0.2
```

### Comparing `hc_log_filter-1.2.2/hc_log_filter.egg-info/SOURCES.txt` & `hc_log_filter-1.2.6/hc_log_filter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hc_log_filter-1.2.2/setup.py` & `hc_log_filter-1.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `hc_log_filter-1.2.2/src/entry.py` & `hc_log_filter-1.2.6/src/entry.py`

 * *Files identical despite different names*

### Comparing `hc_log_filter-1.2.2/src/log_utility.py` & `hc_log_filter-1.2.6/src/log_utility.py`

 * *Files identical despite different names*

### Comparing `hc_log_filter-1.2.2/src/pack_log.py` & `hc_log_filter-1.2.6/src/pack_log.py`

 * *Files identical despite different names*

### Comparing `hc_log_filter-1.2.2/src/v_t_chart.py` & `hc_log_filter-1.2.6/src/v_t_chart.py`

 * *Files identical despite different names*

### Comparing `hc_log_filter-1.2.2/test/test_log_download.py` & `hc_log_filter-1.2.6/test/test_log_download.py`

 * *Files identical despite different names*

### Comparing `hc_log_filter-1.2.2/test/test_log_file_name_match.py` & `hc_log_filter-1.2.6/test/test_log_file_name_match.py`

 * *Files identical despite different names*

### Comparing `hc_log_filter-1.2.2/test/test_log_utility.py` & `hc_log_filter-1.2.6/test/test_log_utility.py`

 * *Files identical despite different names*

### Comparing `hc_log_filter-1.2.2/test/test_read_pick_data.py` & `hc_log_filter-1.2.6/test/test_read_pick_data.py`

 * *Files identical despite different names*

### Comparing `hc_log_filter-1.2.2/test/test_read_sort_data.py` & `hc_log_filter-1.2.6/test/test_read_sort_data.py`

 * *Files identical despite different names*

### Comparing `hc_log_filter-1.2.2/test/test_tiem_range.py` & `hc_log_filter-1.2.6/test/test_tiem_range.py`

 * *Files identical despite different names*

