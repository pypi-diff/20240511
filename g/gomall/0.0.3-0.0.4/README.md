# Comparing `tmp/gomall-0.0.3.tar.gz` & `tmp/gomall-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gomall-0.0.3.tar", last modified: Thu Jun  1 12:57:52 2023, max compression
+gzip compressed data, was "gomall-0.0.4.tar", last modified: Sat May 11 11:12:36 2024, max compression
```

## Comparing `gomall-0.0.3.tar` & `gomall-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 12:57:52.473168 gomall-0.0.3/
--rw-rw-rw-   0        0        0     1086 2023-05-26 11:23:18.000000 gomall-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      561 2023-06-01 12:57:52.471701 gomall-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      105 2023-05-26 11:26:17.000000 gomall-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 12:57:52.448982 gomall-0.0.3/gomall/
--rw-rw-rw-   0        0        0       46 2023-05-26 11:41:00.000000 gomall-0.0.3/gomall/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 12:57:52.469491 gomall-0.0.3/gomall/autolog/
--rw-rw-rw-   0        0        0       90 2023-05-26 11:38:51.000000 gomall-0.0.3/gomall/autolog/__init__.py
--rw-rw-rw-   0        0        0     5537 2023-06-01 12:27:11.000000 gomall-0.0.3/gomall/autolog/log.py
--rw-rw-rw-   0        0        0      880 2023-05-26 11:38:51.000000 gomall-0.0.3/gomall/autolog/model.py
-drwxrwxrwx   0        0        0        0 2023-06-01 12:57:52.462298 gomall-0.0.3/gomall.egg-info/
--rw-rw-rw-   0        0        0      561 2023-06-01 12:57:52.000000 gomall-0.0.3/gomall.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-06-01 12:57:52.000000 gomall-0.0.3/gomall.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 12:57:52.000000 gomall-0.0.3/gomall.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-01 12:57:52.000000 gomall-0.0.3/gomall.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-01 12:57:52.000000 gomall-0.0.3/gomall.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 12:57:52.473168 gomall-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      730 2023-06-01 12:57:47.000000 gomall-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 11:12:36.550000 gomall-0.0.4/
+-rw-rw-rw-   0        0        0     1086 2023-05-26 11:23:18.000000 gomall-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      620 2024-05-11 11:12:38.000000 gomall-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      105 2023-05-26 11:26:18.000000 gomall-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 11:12:36.560000 gomall-0.0.4/gomall/
+-rw-rw-rw-   0        0        0       46 2023-05-26 11:41:00.000000 gomall-0.0.4/gomall/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 11:12:36.580000 gomall-0.0.4/gomall/autolog/
+-rw-rw-rw-   0        0        0       90 2023-05-26 11:38:52.000000 gomall-0.0.4/gomall/autolog/__init__.py
+-rw-rw-rw-   0        0        0     5537 2023-06-01 12:27:12.000000 gomall-0.0.4/gomall/autolog/log.py
+-rw-rw-rw-   0        0        0      880 2023-05-26 11:38:52.000000 gomall-0.0.4/gomall/autolog/model.py
+drwxrwxrwx   0        0        0        0 2024-05-11 11:12:36.570000 gomall-0.0.4/gomall.egg-info/
+-rw-rw-rw-   0        0        0      620 2024-05-11 11:12:38.000000 gomall-0.0.4/gomall.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-11 11:12:38.000000 gomall-0.0.4/gomall.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 11:12:38.000000 gomall-0.0.4/gomall.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-11 11:12:38.000000 gomall-0.0.4/gomall.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-11 11:12:38.000000 gomall-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      672 2024-05-11 11:10:16.000000 gomall-0.0.4/setup.py
```

### Comparing `gomall-0.0.3/LICENSE` & `gomall-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gomall-0.0.3/PKG-INFO` & `gomall-0.0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 Metadata-Version: 2.1
 Name: gomall
-Version: 0.0.3
+Version: 0.0.4
 Summary: 和gomall平台配合使用的python依赖包，包括实验追踪、指令构造、模型评估等工具
+Home-page: UNKNOWN
 Author: GoMall Development Team
 Author-email: wangwenshan@ict.ac.cn
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 和gomall平台配合使用的python依赖包，包括实验追踪、指令构造、模型评估等工具
+
```

### Comparing `gomall-0.0.3/gomall/autolog/log.py` & `gomall-0.0.4/gomall/autolog/log.py`

 * *Files identical despite different names*

### Comparing `gomall-0.0.3/gomall/autolog/model.py` & `gomall-0.0.4/gomall/autolog/model.py`

 * *Files identical despite different names*

### Comparing `gomall-0.0.3/gomall.egg-info/PKG-INFO` & `gomall-0.0.4/gomall.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 Metadata-Version: 2.1
 Name: gomall
-Version: 0.0.3
+Version: 0.0.4
 Summary: 和gomall平台配合使用的python依赖包，包括实验追踪、指令构造、模型评估等工具
+Home-page: UNKNOWN
 Author: GoMall Development Team
 Author-email: wangwenshan@ict.ac.cn
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 和gomall平台配合使用的python依赖包，包括实验追踪、指令构造、模型评估等工具
+
```

