# Comparing `tmp/SocietyEvolutionNetwork-0.1.2.tar.gz` & `tmp/SocietyEvolutionNetwork-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SocietyEvolutionNetwork-0.1.2.tar", last modified: Thu May  9 03:12:57 2024, max compression
+gzip compressed data, was "dist\SocietyEvolutionNetwork-0.1.3.tar", last modified: Sat May 11 07:39:30 2024, max compression
```

## Comparing `SocietyEvolutionNetwork-0.1.2.tar` & `SocietyEvolutionNetwork-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 03:12:57.000000 SocietyEvolutionNetwork-0.1.2/
--rw-rw-rw-   0        0        0     1067 2024-05-09 02:03:55.000000 SocietyEvolutionNetwork-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       27 2024-05-09 02:03:55.000000 SocietyEvolutionNetwork-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3069 2024-05-09 03:12:57.000000 SocietyEvolutionNetwork-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2403 2024-05-09 02:03:55.000000 SocietyEvolutionNetwork-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-09 03:12:57.000000 SocietyEvolutionNetwork-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     3901 2024-05-09 03:12:43.000000 SocietyEvolutionNetwork-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-09 03:12:57.000000 SocietyEvolutionNetwork-0.1.2/SocietyEvolutionNetwork/
--rw-rw-rw-   0        0        0    10703 2024-05-09 03:12:09.000000 SocietyEvolutionNetwork-0.1.2/SocietyEvolutionNetwork/core.py
--rw-rw-rw-   0        0        0       21 2024-05-09 03:09:16.000000 SocietyEvolutionNetwork-0.1.2/SocietyEvolutionNetwork/__init__.py
--rw-rw-rw-   0        0        0      360 2024-05-09 03:12:21.000000 SocietyEvolutionNetwork-0.1.2/SocietyEvolutionNetwork/__version__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 03:12:57.000000 SocietyEvolutionNetwork-0.1.2/SocietyEvolutionNetwork.egg-info/
--rw-rw-rw-   0        0        0        1 2024-05-09 03:12:57.000000 SocietyEvolutionNetwork-0.1.2/SocietyEvolutionNetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     3069 2024-05-09 03:12:57.000000 SocietyEvolutionNetwork-0.1.2/SocietyEvolutionNetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2024-05-09 03:12:57.000000 SocietyEvolutionNetwork-0.1.2/SocietyEvolutionNetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       24 2024-05-09 03:12:57.000000 SocietyEvolutionNetwork-0.1.2/SocietyEvolutionNetwork.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-11 07:39:30.000000 SocietyEvolutionNetwork-0.1.3/
+-rw-rw-rw-   0        0        0     1067 2024-05-09 02:03:55.000000 SocietyEvolutionNetwork-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0       27 2024-05-09 02:03:55.000000 SocietyEvolutionNetwork-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3249 2024-05-11 07:39:30.000000 SocietyEvolutionNetwork-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2583 2024-05-09 05:54:22.000000 SocietyEvolutionNetwork-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-11 07:39:30.000000 SocietyEvolutionNetwork-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     3901 2024-05-11 07:39:03.000000 SocietyEvolutionNetwork-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 07:39:30.000000 SocietyEvolutionNetwork-0.1.3/SocietyEvolutionNetwork/
+-rw-rw-rw-   0        0        0     2710 2024-05-11 07:36:04.000000 SocietyEvolutionNetwork-0.1.3/SocietyEvolutionNetwork/logger.py
+-rw-rw-rw-   0        0        0    10703 2024-05-09 03:12:09.000000 SocietyEvolutionNetwork-0.1.3/SocietyEvolutionNetwork/network.py
+-rw-rw-rw-   0        0        0       45 2024-05-11 07:36:27.000000 SocietyEvolutionNetwork-0.1.3/SocietyEvolutionNetwork/__init__.py
+-rw-rw-rw-   0        0        0      360 2024-05-11 07:39:11.000000 SocietyEvolutionNetwork-0.1.3/SocietyEvolutionNetwork/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 07:39:30.000000 SocietyEvolutionNetwork-0.1.3/SocietyEvolutionNetwork.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-05-11 07:39:29.000000 SocietyEvolutionNetwork-0.1.3/SocietyEvolutionNetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     3249 2024-05-11 07:39:29.000000 SocietyEvolutionNetwork-0.1.3/SocietyEvolutionNetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      370 2024-05-11 07:39:29.000000 SocietyEvolutionNetwork-0.1.3/SocietyEvolutionNetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       24 2024-05-11 07:39:29.000000 SocietyEvolutionNetwork-0.1.3/SocietyEvolutionNetwork.egg-info/top_level.txt
```

### Comparing `SocietyEvolutionNetwork-0.1.2/LICENSE` & `SocietyEvolutionNetwork-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SocietyEvolutionNetwork-0.1.2/PKG-INFO` & `SocietyEvolutionNetwork-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SocietyEvolutionNetwork
-Version: 0.1.2
+Version: 0.1.3
 Summary: demo of society evolution network.
 Home-page: UNKNOWN
 Author: HaiLong Zheng
 Author-email: SkinChange06@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,22 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
+<!--
+ * @Author: ZhengHaiLong
+ * @Date: 2024-05-09 13:51:57
+ * @LastEditors: SkinChange06 1581065016@qq.com
+ * @LastEditTime: 2024-05-09 13:53:11
+ * @Description: 
+ * 
+-->
 📦 setup.py (for humans)
 =======================
 
 This repo exists to provide [an example setup.py] file, that can be used
 to bootstrap your next Python project. It includes some advanced
 patterns and best practices for `setup.py`, as well as some
 commented–out nice–to–haves.
```

### Comparing `SocietyEvolutionNetwork-0.1.2/README.md` & `SocietyEvolutionNetwork-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+<!--
+ * @Author: ZhengHaiLong
+ * @Date: 2024-05-09 13:51:57
+ * @LastEditors: SkinChange06 1581065016@qq.com
+ * @LastEditTime: 2024-05-09 13:53:11
+ * @Description: 
+ * 
+-->
 📦 setup.py (for humans)
 =======================
 
 This repo exists to provide [an example setup.py] file, that can be used
 to bootstrap your next Python project. It includes some advanced
 patterns and best practices for `setup.py`, as well as some
 commented–out nice–to–haves.
```

### Comparing `SocietyEvolutionNetwork-0.1.2/setup.py` & `SocietyEvolutionNetwork-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'SocietyEvolutionNetwork'
 DESCRIPTION = 'demo of society evolution network.'
 URL = ''
 EMAIL = 'SkinChange06@gmail.com'
 AUTHOR = 'HaiLong Zheng'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

### Comparing `SocietyEvolutionNetwork-0.1.2/SocietyEvolutionNetwork/core.py` & `SocietyEvolutionNetwork-0.1.3/SocietyEvolutionNetwork/network.py`

 * *Files identical despite different names*

### Comparing `SocietyEvolutionNetwork-0.1.2/SocietyEvolutionNetwork.egg-info/PKG-INFO` & `SocietyEvolutionNetwork-0.1.3/SocietyEvolutionNetwork.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SocietyEvolutionNetwork
-Version: 0.1.2
+Version: 0.1.3
 Summary: demo of society evolution network.
 Home-page: UNKNOWN
 Author: HaiLong Zheng
 Author-email: SkinChange06@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,22 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
+<!--
+ * @Author: ZhengHaiLong
+ * @Date: 2024-05-09 13:51:57
+ * @LastEditors: SkinChange06 1581065016@qq.com
+ * @LastEditTime: 2024-05-09 13:53:11
+ * @Description: 
+ * 
+-->
 📦 setup.py (for humans)
 =======================
 
 This repo exists to provide [an example setup.py] file, that can be used
 to bootstrap your next Python project. It includes some advanced
 patterns and best practices for `setup.py`, as well as some
 commented–out nice–to–haves.
```

