# Comparing `tmp/proxies-taster-1.2.2.tar.gz` & `tmp/proxies_taster-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxies_taster-1.2.2.tar", last modified: Sat May 11 05:18:04 2024, max compression
+gzip compressed data, was "proxies_taster-1.2.3.tar", last modified: Sat May 11 05:43:49 2024, max compression
```

## Comparing `proxies-taster-1.2.2.tar` & `proxies_taster-1.2.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 whatis    (1000) whatis    (1000)        0 2024-05-11 05:18:04.011603 proxies_taster-1.2.2/
--rw-r--r--   0 whatis    (1000) whatis    (1000)     1084 2023-11-08 12:32:08.000000 proxies_taster-1.2.2/LICENSE
--rw-r--r--   0 whatis    (1000) whatis    (1000)      169 2023-10-19 12:55:04.000000 proxies_taster-1.2.2/MANIFEST.in
--rw-r--r--   0 whatis    (1000) whatis    (1000)      845 2024-05-11 05:18:04.011603 proxies_taster-1.2.2/PKG-INFO
--rw-r--r--   0 whatis    (1000) whatis    (1000)      333 2023-10-19 12:55:04.000000 proxies_taster-1.2.2/README.md
-drwxr-xr-x   0 whatis    (1000) whatis    (1000)        0 2024-05-11 05:18:04.011603 proxies_taster-1.2.2/proxies_taster/
--rw-r--r--   0 whatis    (1000) whatis    (1000)      166 2023-10-19 12:55:04.000000 proxies_taster-1.2.2/proxies_taster/__init__.py
--rw-r--r--   0 whatis    (1000) whatis    (1000)    13881 2024-05-11 04:45:38.000000 proxies_taster-1.2.2/proxies_taster/__main__.py
--rw-r--r--   0 whatis    (1000) whatis    (1000)     6395 2023-11-08 16:30:56.000000 proxies_taster-1.2.2/proxies_taster/events_data.py
--rw-r--r--   0 whatis    (1000) whatis    (1000)      232 2023-11-09 07:31:54.000000 proxies_taster-1.2.2/proxies_taster/exceptions.py
--rw-r--r--   0 whatis    (1000) whatis    (1000)     7746 2024-05-11 04:24:35.000000 proxies_taster-1.2.2/proxies_taster/proxies_parser_logger.py
--rw-r--r--   0 whatis    (1000) whatis    (1000)    20956 2024-05-11 04:50:03.000000 proxies_taster-1.2.2/proxies_taster/taster.py
--rw-r--r--   0 whatis    (1000) whatis    (1000)     1842 2023-11-12 06:26:57.000000 proxies_taster-1.2.2/proxies_taster/types.py
-drwxr-xr-x   0 whatis    (1000) whatis    (1000)        0 2024-05-11 05:18:04.011603 proxies_taster-1.2.2/proxies_taster.egg-info/
--rw-r--r--   0 whatis    (1000) whatis    (1000)      845 2024-05-11 05:18:03.000000 proxies_taster-1.2.2/proxies_taster.egg-info/PKG-INFO
--rw-r--r--   0 whatis    (1000) whatis    (1000)      429 2024-05-11 05:18:03.000000 proxies_taster-1.2.2/proxies_taster.egg-info/SOURCES.txt
--rw-r--r--   0 whatis    (1000) whatis    (1000)        1 2024-05-11 05:18:03.000000 proxies_taster-1.2.2/proxies_taster.egg-info/dependency_links.txt
--rw-r--r--   0 whatis    (1000) whatis    (1000)       52 2024-05-11 05:18:03.000000 proxies_taster-1.2.2/proxies_taster.egg-info/requires.txt
--rw-r--r--   0 whatis    (1000) whatis    (1000)       15 2024-05-11 05:18:03.000000 proxies_taster-1.2.2/proxies_taster.egg-info/top_level.txt
--rw-r--r--   0 whatis    (1000) whatis    (1000)       38 2024-05-11 05:18:04.011603 proxies_taster-1.2.2/setup.cfg
--rw-r--r--   0 whatis    (1000) whatis    (1000)      962 2024-05-11 04:51:51.000000 proxies_taster-1.2.2/setup.py
+drwxr-xr-x   0 whatis    (1000) whatis    (1000)        0 2024-05-11 05:43:49.501611 proxies_taster-1.2.3/
+-rw-r--r--   0 whatis    (1000) whatis    (1000)     1084 2023-11-08 12:32:08.000000 proxies_taster-1.2.3/LICENSE
+-rw-r--r--   0 whatis    (1000) whatis    (1000)      169 2023-10-19 12:55:04.000000 proxies_taster-1.2.3/MANIFEST.in
+-rw-r--r--   0 whatis    (1000) whatis    (1000)      845 2024-05-11 05:43:49.501611 proxies_taster-1.2.3/PKG-INFO
+-rw-r--r--   0 whatis    (1000) whatis    (1000)      333 2023-10-19 12:55:04.000000 proxies_taster-1.2.3/README.md
+drwxr-xr-x   0 whatis    (1000) whatis    (1000)        0 2024-05-11 05:43:49.501611 proxies_taster-1.2.3/proxies_taster/
+-rw-r--r--   0 whatis    (1000) whatis    (1000)      166 2023-10-19 12:55:04.000000 proxies_taster-1.2.3/proxies_taster/__init__.py
+-rw-r--r--   0 whatis    (1000) whatis    (1000)    13829 2024-05-11 05:28:30.000000 proxies_taster-1.2.3/proxies_taster/__main__.py
+-rw-r--r--   0 whatis    (1000) whatis    (1000)     6395 2023-11-08 16:30:56.000000 proxies_taster-1.2.3/proxies_taster/events_data.py
+-rw-r--r--   0 whatis    (1000) whatis    (1000)      232 2023-11-09 07:31:54.000000 proxies_taster-1.2.3/proxies_taster/exceptions.py
+-rw-r--r--   0 whatis    (1000) whatis    (1000)     7746 2024-05-11 04:24:35.000000 proxies_taster-1.2.3/proxies_taster/proxies_parser_logger.py
+-rw-r--r--   0 whatis    (1000) whatis    (1000)    20956 2024-05-11 04:50:03.000000 proxies_taster-1.2.3/proxies_taster/taster.py
+-rw-r--r--   0 whatis    (1000) whatis    (1000)     1842 2023-11-12 06:26:57.000000 proxies_taster-1.2.3/proxies_taster/types.py
+drwxr-xr-x   0 whatis    (1000) whatis    (1000)        0 2024-05-11 05:43:49.501611 proxies_taster-1.2.3/proxies_taster.egg-info/
+-rw-r--r--   0 whatis    (1000) whatis    (1000)      845 2024-05-11 05:43:49.000000 proxies_taster-1.2.3/proxies_taster.egg-info/PKG-INFO
+-rw-r--r--   0 whatis    (1000) whatis    (1000)      470 2024-05-11 05:43:49.000000 proxies_taster-1.2.3/proxies_taster.egg-info/SOURCES.txt
+-rw-r--r--   0 whatis    (1000) whatis    (1000)        1 2024-05-11 05:43:49.000000 proxies_taster-1.2.3/proxies_taster.egg-info/dependency_links.txt
+-rw-r--r--   0 whatis    (1000) whatis    (1000)       64 2024-05-11 05:43:49.000000 proxies_taster-1.2.3/proxies_taster.egg-info/entry_points.txt
+-rw-r--r--   0 whatis    (1000) whatis    (1000)       52 2024-05-11 05:43:49.000000 proxies_taster-1.2.3/proxies_taster.egg-info/requires.txt
+-rw-r--r--   0 whatis    (1000) whatis    (1000)       15 2024-05-11 05:43:49.000000 proxies_taster-1.2.3/proxies_taster.egg-info/top_level.txt
+-rw-r--r--   0 whatis    (1000) whatis    (1000)       38 2024-05-11 05:43:49.501611 proxies_taster-1.2.3/setup.cfg
+-rw-r--r--   0 whatis    (1000) whatis    (1000)     1109 2024-05-11 05:43:24.000000 proxies_taster-1.2.3/setup.py
```

### Comparing `proxies_taster-1.2.2/LICENSE` & `proxies_taster-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `proxies_taster-1.2.2/PKG-INFO` & `proxies_taster-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: proxies-taster
-Version: 1.2.2
+Version: 1.2.3
 Summary: Пакет для проверки прокси
 Home-page: https://github.com/TheWhatis/ProxiesTaster
-Download-URL: https://github.com/TheWhatis/ProxiesTaster/dist/proxies-taster-1.2.2.zip
+Download-URL: https://github.com/TheWhatis/ProxiesTaster/dist/proxies-taster-1.2.3.zip
 Author: Whatis
 Author-email: asdwdagwahwabe@gmail.com
 License: GPL
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
```

### Comparing `proxies_taster-1.2.2/proxies_taster/__main__.py` & `proxies_taster-1.2.3/proxies_taster/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 # Colorama
 from colorama import init
 
 # Tqdm
 from tqdm import tqdm
 
 # ProxiesTaster
-from proxies_taster import Protocol
-from proxies_taster import WorkedProxy
-from proxies_taster import ProxiesTaster
-from proxies_taster.events_data import Events
-from proxies_taster.exceptions import TooManyOpenFilesError
+from .types import Protocol
+from .types import WorkedProxy
+from .types import ProxiesTaster
+from .events_data import Events
+from .exceptions import TooManyOpenFilesError
 
 # My logger
 from proxies_parser_logger import setting_logging
 
 
 args = []
 bars: dict = {}
```

### Comparing `proxies_taster-1.2.2/proxies_taster/events_data.py` & `proxies_taster-1.2.3/proxies_taster/events_data.py`

 * *Files identical despite different names*

### Comparing `proxies_taster-1.2.2/proxies_taster/proxies_parser_logger.py` & `proxies_taster-1.2.3/proxies_taster/proxies_parser_logger.py`

 * *Files identical despite different names*

### Comparing `proxies_taster-1.2.2/proxies_taster/taster.py` & `proxies_taster-1.2.3/proxies_taster/taster.py`

 * *Files identical despite different names*

### Comparing `proxies_taster-1.2.2/proxies_taster/types.py` & `proxies_taster-1.2.3/proxies_taster/types.py`

 * *Files identical despite different names*

### Comparing `proxies_taster-1.2.2/proxies_taster.egg-info/PKG-INFO` & `proxies_taster-1.2.3/proxies_taster.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: proxies-taster
-Version: 1.2.2
+Version: 1.2.3
 Summary: Пакет для проверки прокси
 Home-page: https://github.com/TheWhatis/ProxiesTaster
-Download-URL: https://github.com/TheWhatis/ProxiesTaster/dist/proxies-taster-1.2.2.zip
+Download-URL: https://github.com/TheWhatis/ProxiesTaster/dist/proxies-taster-1.2.3.zip
 Author: Whatis
 Author-email: asdwdagwahwabe@gmail.com
 License: GPL
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
```

### Comparing `proxies_taster-1.2.2/setup.py` & `proxies_taster-1.2.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Скрипт для установлки пакета"""
 from setuptools import setup
 
 
 name = 'proxies-taster'
-version = '1.2.2'
+version = '1.2.3'
+
 
 # Long description
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 url = 'https://github.com/TheWhatis/ProxiesTaster'
 
@@ -34,9 +35,15 @@
         packages=['proxies_taster'],
         include_package_data=True,
         install_requires=[
             'aiohttp',
             'aiohttp-proxy',
             'fake-useragent',
             'PyEventEmitter'
-        ]
+        ],
+
+        entry_points={
+            "console_scripts": [
+                'proxies-taster = proxies_taster.__main__:main'
+            ]
+        }
     )
```

