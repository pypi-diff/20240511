# Comparing `tmp/apt_mirror-6a1.tar.gz` & `tmp/apt_mirror-6a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apt_mirror-6a1.tar", last modified: Fri May 10 13:35:17 2024, max compression
+gzip compressed data, was "apt_mirror-6a2.tar", last modified: Sat May 11 12:11:09 2024, max compression
```

## Comparing `apt_mirror-6a1.tar` & `apt_mirror-6a2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:35:17.329154 apt_mirror-6a1/
--rw-rw-rw-   0 root         (0) root         (0)    35149 2024-05-10 13:35:04.000000 apt_mirror-6a1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    45768 2024-05-10 13:35:17.329154 apt_mirror-6a1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3684 2024-05-10 13:35:04.000000 apt_mirror-6a1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:35:17.322154 apt_mirror-6a1/apt_mirror/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:35:04.000000 apt_mirror-6a1/apt_mirror/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2844 2024-05-10 13:35:04.000000 apt_mirror-6a1/apt_mirror/aiofile.py
--rw-rw-rw-   0 root         (0) root         (0)    25895 2024-05-10 13:35:04.000000 apt_mirror-6a1/apt_mirror/apt_mirror.py
--rw-rw-rw-   0 root         (0) root         (0)    18578 2024-05-10 13:35:04.000000 apt_mirror-6a1/apt_mirror/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:35:17.325154 apt_mirror-6a1/apt_mirror/download/
--rw-rw-rw-   0 root         (0) root         (0)      491 2024-05-10 13:35:04.000000 apt_mirror-6a1/apt_mirror/download/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5120 2024-05-10 13:35:04.000000 apt_mirror-6a1/apt_mirror/download/download_file.py
--rw-rw-rw-   0 root         (0) root         (0)    15146 2024-05-10 13:35:04.000000 apt_mirror-6a1/apt_mirror/download/downloader.py
--rw-rw-rw-   0 root         (0) root         (0)     1401 2024-05-10 13:35:04.000000 apt_mirror-6a1/apt_mirror/download/factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:35:17.326154 apt_mirror-6a1/apt_mirror/download/protocols/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:35:04.000000 apt_mirror-6a1/apt_mirror/download/protocols/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5040 2024-05-10 13:35:04.000000 apt_mirror-6a1/apt_mirror/download/protocols/ftp.py
--rw-rw-rw-   0 root         (0) root         (0)     4204 2024-05-10 13:35:04.000000 apt_mirror-6a1/apt_mirror/download/protocols/http.py
--rw-rw-rw-   0 root         (0) root         (0)     1041 2024-05-10 13:35:04.000000 apt_mirror-6a1/apt_mirror/download/proxy.py
--rw-rw-rw-   0 root         (0) root         (0)      563 2024-05-10 13:35:04.000000 apt_mirror-6a1/apt_mirror/download/response.py
--rw-rw-rw-   0 root         (0) root         (0)     2312 2024-05-10 13:35:04.000000 apt_mirror-6a1/apt_mirror/download/url.py
--rw-rw-rw-   0 root         (0) root         (0)     2488 2024-05-10 13:35:04.000000 apt_mirror-6a1/apt_mirror/logs.py
--rw-rw-rw-   0 root         (0) root         (0)     2728 2024-05-10 13:35:04.000000 apt_mirror-6a1/apt_mirror/prometheus.py
--rw-rw-rw-   0 root         (0) root         (0)    28952 2024-05-10 13:35:04.000000 apt_mirror-6a1/apt_mirror/repository.py
--rw-rw-rw-   0 root         (0) root         (0)      207 2024-05-10 13:35:04.000000 apt_mirror-6a1/apt_mirror/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:35:17.327154 apt_mirror-6a1/apt_mirror.egg-info/
--rw-r--r--   0 root         (0) root         (0)    45768 2024-05-10 13:35:17.000000 apt_mirror-6a1/apt_mirror.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      867 2024-05-10 13:35:17.000000 apt_mirror-6a1/apt_mirror.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 13:35:17.000000 apt_mirror-6a1/apt_mirror.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2024-05-10 13:35:17.000000 apt_mirror-6a1/apt_mirror.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      279 2024-05-10 13:35:17.000000 apt_mirror-6a1/apt_mirror.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-05-10 13:35:17.000000 apt_mirror-6a1/apt_mirror.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     2167 2024-05-10 13:35:04.000000 apt_mirror-6a1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      129 2024-05-10 13:35:17.329154 apt_mirror-6a1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      104 2024-05-10 13:35:04.000000 apt_mirror-6a1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:35:17.327154 apt_mirror-6a1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1141 2024-05-10 13:35:04.000000 apt_mirror-6a1/tests/test_clean.py
--rw-rw-rw-   0 root         (0) root         (0)     8286 2024-05-10 13:35:04.000000 apt_mirror-6a1/tests/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)      630 2024-05-10 13:35:04.000000 apt_mirror-6a1/tests/test_download.py
--rw-rw-rw-   0 root         (0) root         (0)     7768 2024-05-10 13:35:04.000000 apt_mirror-6a1/tests/test_repository.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 12:11:09.798311 apt_mirror-6a2/
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2024-05-11 12:10:54.000000 apt_mirror-6a2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    45768 2024-05-11 12:11:09.798311 apt_mirror-6a2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3684 2024-05-11 12:10:54.000000 apt_mirror-6a2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 12:11:09.792311 apt_mirror-6a2/apt_mirror/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 12:10:54.000000 apt_mirror-6a2/apt_mirror/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2844 2024-05-11 12:10:54.000000 apt_mirror-6a2/apt_mirror/aiofile.py
+-rw-rw-rw-   0 root         (0) root         (0)    25895 2024-05-11 12:10:54.000000 apt_mirror-6a2/apt_mirror/apt_mirror.py
+-rw-rw-rw-   0 root         (0) root         (0)    18578 2024-05-11 12:10:54.000000 apt_mirror-6a2/apt_mirror/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 12:11:09.795311 apt_mirror-6a2/apt_mirror/download/
+-rw-rw-rw-   0 root         (0) root         (0)      491 2024-05-11 12:10:54.000000 apt_mirror-6a2/apt_mirror/download/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5120 2024-05-11 12:10:54.000000 apt_mirror-6a2/apt_mirror/download/download_file.py
+-rw-rw-rw-   0 root         (0) root         (0)    15146 2024-05-11 12:10:54.000000 apt_mirror-6a2/apt_mirror/download/downloader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1401 2024-05-11 12:10:54.000000 apt_mirror-6a2/apt_mirror/download/factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 12:11:09.795311 apt_mirror-6a2/apt_mirror/download/protocols/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 12:10:54.000000 apt_mirror-6a2/apt_mirror/download/protocols/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5040 2024-05-11 12:10:54.000000 apt_mirror-6a2/apt_mirror/download/protocols/ftp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4204 2024-05-11 12:10:54.000000 apt_mirror-6a2/apt_mirror/download/protocols/http.py
+-rw-rw-rw-   0 root         (0) root         (0)     1041 2024-05-11 12:10:54.000000 apt_mirror-6a2/apt_mirror/download/proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)      563 2024-05-11 12:10:54.000000 apt_mirror-6a2/apt_mirror/download/response.py
+-rw-rw-rw-   0 root         (0) root         (0)     2312 2024-05-11 12:10:54.000000 apt_mirror-6a2/apt_mirror/download/url.py
+-rw-rw-rw-   0 root         (0) root         (0)     2488 2024-05-11 12:10:54.000000 apt_mirror-6a2/apt_mirror/logs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2728 2024-05-11 12:10:54.000000 apt_mirror-6a2/apt_mirror/prometheus.py
+-rw-rw-rw-   0 root         (0) root         (0)    28952 2024-05-11 12:10:54.000000 apt_mirror-6a2/apt_mirror/repository.py
+-rw-rw-rw-   0 root         (0) root         (0)      207 2024-05-11 12:10:54.000000 apt_mirror-6a2/apt_mirror/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 12:11:09.796311 apt_mirror-6a2/apt_mirror.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    45768 2024-05-11 12:11:09.000000 apt_mirror-6a2/apt_mirror.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      867 2024-05-11 12:11:09.000000 apt_mirror-6a2/apt_mirror.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 12:11:09.000000 apt_mirror-6a2/apt_mirror.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2024-05-11 12:11:09.000000 apt_mirror-6a2/apt_mirror.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      279 2024-05-11 12:11:09.000000 apt_mirror-6a2/apt_mirror.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-11 12:11:09.000000 apt_mirror-6a2/apt_mirror.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2167 2024-05-11 12:10:54.000000 apt_mirror-6a2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      129 2024-05-11 12:11:09.798311 apt_mirror-6a2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      104 2024-05-11 12:10:54.000000 apt_mirror-6a2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 12:11:09.796311 apt_mirror-6a2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1141 2024-05-11 12:10:54.000000 apt_mirror-6a2/tests/test_clean.py
+-rw-rw-rw-   0 root         (0) root         (0)     8286 2024-05-11 12:10:54.000000 apt_mirror-6a2/tests/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      630 2024-05-11 12:10:54.000000 apt_mirror-6a2/tests/test_download.py
+-rw-rw-rw-   0 root         (0) root         (0)     7768 2024-05-11 12:10:54.000000 apt_mirror-6a2/tests/test_repository.py
```

### Comparing `apt_mirror-6a1/LICENSE` & `apt_mirror-6a2/LICENSE`

 * *Files identical despite different names*

### Comparing `apt_mirror-6a1/PKG-INFO` & `apt_mirror-6a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apt-mirror
-Version: 6a1
+Version: 6a2
 Summary: apt-mirror Python reimplementation
 Author-email: Yuri Konotopov <ykonotopov@gnome.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `apt_mirror-6a1/README.md` & `apt_mirror-6a2/README.md`

 * *Files identical despite different names*

### Comparing `apt_mirror-6a1/apt_mirror/aiofile.py` & `apt_mirror-6a2/apt_mirror/aiofile.py`

 * *Files identical despite different names*

### Comparing `apt_mirror-6a1/apt_mirror/apt_mirror.py` & `apt_mirror-6a2/apt_mirror/apt_mirror.py`

 * *Files identical despite different names*

### Comparing `apt_mirror-6a1/apt_mirror/config.py` & `apt_mirror-6a2/apt_mirror/config.py`

 * *Files identical despite different names*

### Comparing `apt_mirror-6a1/apt_mirror/download/download_file.py` & `apt_mirror-6a2/apt_mirror/download/download_file.py`

 * *Files identical despite different names*

### Comparing `apt_mirror-6a1/apt_mirror/download/downloader.py` & `apt_mirror-6a2/apt_mirror/download/downloader.py`

 * *Files identical despite different names*

### Comparing `apt_mirror-6a1/apt_mirror/download/factory.py` & `apt_mirror-6a2/apt_mirror/download/factory.py`

 * *Files identical despite different names*

### Comparing `apt_mirror-6a1/apt_mirror/download/protocols/ftp.py` & `apt_mirror-6a2/apt_mirror/download/protocols/ftp.py`

 * *Files identical despite different names*

### Comparing `apt_mirror-6a1/apt_mirror/download/protocols/http.py` & `apt_mirror-6a2/apt_mirror/download/protocols/http.py`

 * *Files identical despite different names*

### Comparing `apt_mirror-6a1/apt_mirror/download/proxy.py` & `apt_mirror-6a2/apt_mirror/download/proxy.py`

 * *Files identical despite different names*

### Comparing `apt_mirror-6a1/apt_mirror/download/response.py` & `apt_mirror-6a2/apt_mirror/download/response.py`

 * *Files identical despite different names*

### Comparing `apt_mirror-6a1/apt_mirror/download/url.py` & `apt_mirror-6a2/apt_mirror/download/url.py`

 * *Files identical despite different names*

### Comparing `apt_mirror-6a1/apt_mirror/logs.py` & `apt_mirror-6a2/apt_mirror/logs.py`

 * *Files identical despite different names*

### Comparing `apt_mirror-6a1/apt_mirror/prometheus.py` & `apt_mirror-6a2/apt_mirror/prometheus.py`

 * *Files identical despite different names*

### Comparing `apt_mirror-6a1/apt_mirror/repository.py` & `apt_mirror-6a2/apt_mirror/repository.py`

 * *Files identical despite different names*

### Comparing `apt_mirror-6a1/apt_mirror.egg-info/PKG-INFO` & `apt_mirror-6a2/apt_mirror.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apt-mirror
-Version: 6a1
+Version: 6a2
 Summary: apt-mirror Python reimplementation
 Author-email: Yuri Konotopov <ykonotopov@gnome.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `apt_mirror-6a1/apt_mirror.egg-info/SOURCES.txt` & `apt_mirror-6a2/apt_mirror.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apt_mirror-6a1/pyproject.toml` & `apt_mirror-6a2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apt-mirror"
-version = "6a1"
+version = "6a2"
 authors = [
     {name = "Yuri Konotopov", email = "ykonotopov@gnome.org"},
 ]
 description = "apt-mirror Python reimplementation"
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["apt", "debian"]
```

### Comparing `apt_mirror-6a1/tests/test_clean.py` & `apt_mirror-6a2/tests/test_clean.py`

 * *Files identical despite different names*

### Comparing `apt_mirror-6a1/tests/test_config.py` & `apt_mirror-6a2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `apt_mirror-6a1/tests/test_download.py` & `apt_mirror-6a2/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `apt_mirror-6a1/tests/test_repository.py` & `apt_mirror-6a2/tests/test_repository.py`

 * *Files identical despite different names*

