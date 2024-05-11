# Comparing `tmp/proxies-taster-1.2.1.tar.gz` & `tmp/proxies-taster-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxies-taster-1.2.1.tar", last modified: Thu Nov  9 18:47:30 2023, max compression
+gzip compressed data, was "proxies_taster-1.2.2.tar", last modified: Sat May 11 05:18:04 2024, max compression
```

## Comparing `proxies-taster-1.2.1.tar` & `proxies-taster-1.2.2.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 whatis    (1000) whatis    (1000)        0 2023-11-09 18:47:30.486484 proxies-taster-1.2.1/
--rw-r--r--   0 whatis    (1000) whatis    (1000)     1084 2023-11-08 12:32:08.000000 proxies-taster-1.2.1/LICENSE
--rw-r--r--   0 whatis    (1000) whatis    (1000)      169 2023-10-19 12:55:04.000000 proxies-taster-1.2.1/MANIFEST.in
--rw-r--r--   0 whatis    (1000) whatis    (1000)      733 2023-11-09 18:47:30.486484 proxies-taster-1.2.1/PKG-INFO
--rw-r--r--   0 whatis    (1000) whatis    (1000)      333 2023-10-19 12:55:04.000000 proxies-taster-1.2.1/README.md
-drwxr-xr-x   0 whatis    (1000) whatis    (1000)        0 2023-11-09 18:47:30.483150 proxies-taster-1.2.1/proxies_taster/
--rw-r--r--   0 whatis    (1000) whatis    (1000)      166 2023-10-19 12:55:04.000000 proxies-taster-1.2.1/proxies_taster/__init__.py
--rw-r--r--   0 whatis    (1000) whatis    (1000)     6395 2023-11-08 16:30:56.000000 proxies-taster-1.2.1/proxies_taster/events_data.py
--rw-r--r--   0 whatis    (1000) whatis    (1000)      232 2023-11-09 07:31:54.000000 proxies-taster-1.2.1/proxies_taster/exceptions.py
--rw-r--r--   0 whatis    (1000) whatis    (1000)    20955 2023-11-09 17:39:32.000000 proxies-taster-1.2.1/proxies_taster/taster.py
--rw-r--r--   0 whatis    (1000) whatis    (1000)     1869 2023-11-09 18:45:17.000000 proxies-taster-1.2.1/proxies_taster/types.py
-drwxr-xr-x   0 whatis    (1000) whatis    (1000)        0 2023-11-09 18:47:30.486484 proxies-taster-1.2.1/proxies_taster.egg-info/
--rw-r--r--   0 whatis    (1000) whatis    (1000)      733 2023-11-09 18:47:30.000000 proxies-taster-1.2.1/proxies_taster.egg-info/PKG-INFO
--rw-r--r--   0 whatis    (1000) whatis    (1000)      362 2023-11-09 18:47:30.000000 proxies-taster-1.2.1/proxies_taster.egg-info/SOURCES.txt
--rw-r--r--   0 whatis    (1000) whatis    (1000)        1 2023-11-09 18:47:30.000000 proxies-taster-1.2.1/proxies_taster.egg-info/dependency_links.txt
--rw-r--r--   0 whatis    (1000) whatis    (1000)       52 2023-11-09 18:47:30.000000 proxies-taster-1.2.1/proxies_taster.egg-info/requires.txt
--rw-r--r--   0 whatis    (1000) whatis    (1000)       15 2023-11-09 18:47:30.000000 proxies-taster-1.2.1/proxies_taster.egg-info/top_level.txt
--rw-r--r--   0 whatis    (1000) whatis    (1000)       38 2023-11-09 18:47:30.486484 proxies-taster-1.2.1/setup.cfg
--rw-r--r--   0 whatis    (1000) whatis    (1000)      962 2023-11-09 18:47:21.000000 proxies-taster-1.2.1/setup.py
+drwxr-xr-x   0 whatis    (1000) whatis    (1000)        0 2024-05-11 05:18:04.011603 proxies_taster-1.2.2/
+-rw-r--r--   0 whatis    (1000) whatis    (1000)     1084 2023-11-08 12:32:08.000000 proxies_taster-1.2.2/LICENSE
+-rw-r--r--   0 whatis    (1000) whatis    (1000)      169 2023-10-19 12:55:04.000000 proxies_taster-1.2.2/MANIFEST.in
+-rw-r--r--   0 whatis    (1000) whatis    (1000)      845 2024-05-11 05:18:04.011603 proxies_taster-1.2.2/PKG-INFO
+-rw-r--r--   0 whatis    (1000) whatis    (1000)      333 2023-10-19 12:55:04.000000 proxies_taster-1.2.2/README.md
+drwxr-xr-x   0 whatis    (1000) whatis    (1000)        0 2024-05-11 05:18:04.011603 proxies_taster-1.2.2/proxies_taster/
+-rw-r--r--   0 whatis    (1000) whatis    (1000)      166 2023-10-19 12:55:04.000000 proxies_taster-1.2.2/proxies_taster/__init__.py
+-rw-r--r--   0 whatis    (1000) whatis    (1000)    13881 2024-05-11 04:45:38.000000 proxies_taster-1.2.2/proxies_taster/__main__.py
+-rw-r--r--   0 whatis    (1000) whatis    (1000)     6395 2023-11-08 16:30:56.000000 proxies_taster-1.2.2/proxies_taster/events_data.py
+-rw-r--r--   0 whatis    (1000) whatis    (1000)      232 2023-11-09 07:31:54.000000 proxies_taster-1.2.2/proxies_taster/exceptions.py
+-rw-r--r--   0 whatis    (1000) whatis    (1000)     7746 2024-05-11 04:24:35.000000 proxies_taster-1.2.2/proxies_taster/proxies_parser_logger.py
+-rw-r--r--   0 whatis    (1000) whatis    (1000)    20956 2024-05-11 04:50:03.000000 proxies_taster-1.2.2/proxies_taster/taster.py
+-rw-r--r--   0 whatis    (1000) whatis    (1000)     1842 2023-11-12 06:26:57.000000 proxies_taster-1.2.2/proxies_taster/types.py
+drwxr-xr-x   0 whatis    (1000) whatis    (1000)        0 2024-05-11 05:18:04.011603 proxies_taster-1.2.2/proxies_taster.egg-info/
+-rw-r--r--   0 whatis    (1000) whatis    (1000)      845 2024-05-11 05:18:03.000000 proxies_taster-1.2.2/proxies_taster.egg-info/PKG-INFO
+-rw-r--r--   0 whatis    (1000) whatis    (1000)      429 2024-05-11 05:18:03.000000 proxies_taster-1.2.2/proxies_taster.egg-info/SOURCES.txt
+-rw-r--r--   0 whatis    (1000) whatis    (1000)        1 2024-05-11 05:18:03.000000 proxies_taster-1.2.2/proxies_taster.egg-info/dependency_links.txt
+-rw-r--r--   0 whatis    (1000) whatis    (1000)       52 2024-05-11 05:18:03.000000 proxies_taster-1.2.2/proxies_taster.egg-info/requires.txt
+-rw-r--r--   0 whatis    (1000) whatis    (1000)       15 2024-05-11 05:18:03.000000 proxies_taster-1.2.2/proxies_taster.egg-info/top_level.txt
+-rw-r--r--   0 whatis    (1000) whatis    (1000)       38 2024-05-11 05:18:04.011603 proxies_taster-1.2.2/setup.cfg
+-rw-r--r--   0 whatis    (1000) whatis    (1000)      962 2024-05-11 04:51:51.000000 proxies_taster-1.2.2/setup.py
```

### Comparing `proxies-taster-1.2.1/LICENSE` & `proxies_taster-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `proxies-taster-1.2.1/PKG-INFO` & `proxies_taster-1.2.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: proxies-taster
-Version: 1.2.1
+Version: 1.2.2
 Summary: Пакет для проверки прокси
 Home-page: https://github.com/TheWhatis/ProxiesTaster
-Download-URL: https://github.com/TheWhatis/ProxiesTaster/dist/proxies-taster-1.2.1.zip
+Download-URL: https://github.com/TheWhatis/ProxiesTaster/dist/proxies-taster-1.2.2.zip
 Author: Whatis
 Author-email: asdwdagwahwabe@gmail.com
 License: GPL
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp
+Requires-Dist: aiohttp-proxy
+Requires-Dist: fake-useragent
+Requires-Dist: PyEventEmitter
 
 # ProxiesTaster
 
   * [Wiki](https://github.com/TheWhatis/ProxiesTaster/tree/master/docs/_build/markdown/index.md "Wiki")
   * [App](https://github.com/TheWhatis/ProxiesTaster/tree/master/docs/_build/markdown/app.md "App")
   * [Package](https://github.com/TheWhatis/ProxiesTaster/tree/master/docs/_build/markdown/package.md "Package")
```

### Comparing `proxies-taster-1.2.1/proxies_taster/events_data.py` & `proxies_taster-1.2.2/proxies_taster/events_data.py`

 * *Files identical despite different names*

### Comparing `proxies-taster-1.2.1/proxies_taster/taster.py` & `proxies_taster-1.2.2/proxies_taster/taster.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 
 from .events_data import RunStart
 from .events_data import RunEnd
 
 # Exceptions
 from .exceptions import TooManyOpenFilesError
 
+
 def events_wrap(
         event: str,
         protocol: int,
         proxy: int,
 ):
     """
     Декоратор для методов ProxiesTaster
```

### Comparing `proxies-taster-1.2.1/proxies_taster/types.py` & `proxies_taster-1.2.2/proxies_taster/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # Typing
 from typing import Union
-from typing import Literal
 
 # Enum
 from enum import Enum
 
 # Dataclass
 from dataclasses import dataclass
```

### Comparing `proxies-taster-1.2.1/proxies_taster.egg-info/PKG-INFO` & `proxies_taster-1.2.2/proxies_taster.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: proxies-taster
-Version: 1.2.1
+Version: 1.2.2
 Summary: Пакет для проверки прокси
 Home-page: https://github.com/TheWhatis/ProxiesTaster
-Download-URL: https://github.com/TheWhatis/ProxiesTaster/dist/proxies-taster-1.2.1.zip
+Download-URL: https://github.com/TheWhatis/ProxiesTaster/dist/proxies-taster-1.2.2.zip
 Author: Whatis
 Author-email: asdwdagwahwabe@gmail.com
 License: GPL
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp
+Requires-Dist: aiohttp-proxy
+Requires-Dist: fake-useragent
+Requires-Dist: PyEventEmitter
 
 # ProxiesTaster
 
   * [Wiki](https://github.com/TheWhatis/ProxiesTaster/tree/master/docs/_build/markdown/index.md "Wiki")
   * [App](https://github.com/TheWhatis/ProxiesTaster/tree/master/docs/_build/markdown/app.md "App")
   * [Package](https://github.com/TheWhatis/ProxiesTaster/tree/master/docs/_build/markdown/package.md "Package")
```

### Comparing `proxies-taster-1.2.1/setup.py` & `proxies_taster-1.2.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Скрипт для установлки пакета"""
 from setuptools import setup
 
 
 name = 'proxies-taster'
-version = '1.2.1'
+version = '1.2.2'
 
 # Long description
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 url = 'https://github.com/TheWhatis/ProxiesTaster'
```

