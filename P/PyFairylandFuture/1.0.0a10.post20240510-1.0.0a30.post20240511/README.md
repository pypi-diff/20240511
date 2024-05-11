# Comparing `tmp/pyfairylandfuture-1.0.0a10.post20240510.tar.gz` & `tmp/pyfairylandfuture-1.0.0a30.post20240511.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfairylandfuture-1.0.0a10.post20240510.tar", last modified: Fri May 10 07:26:00 2024, max compression
+gzip compressed data, was "pyfairylandfuture-1.0.0a30.post20240511.tar", last modified: Sat May 11 10:53:17 2024, max compression
```

## Comparing `pyfairylandfuture-1.0.0a10.post20240510.tar` & `pyfairylandfuture-1.0.0a30.post20240511.tar`

### file list

```diff
@@ -1,41 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 07:26:00.170214 pyfairylandfuture-1.0.0a10.post20240510/
--rw-rw-rw-   0        0        0    34523 2024-05-09 08:14:38.000000 pyfairylandfuture-1.0.0a10.post20240510/LICENSE.txt
--rw-rw-rw-   0        0        0     7747 2024-05-10 07:26:00.169217 pyfairylandfuture-1.0.0a10.post20240510/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-10 07:26:00.167249 pyfairylandfuture-1.0.0a10.post20240510/PyFairylandFuture.egg-info/
--rw-rw-rw-   0        0        0     7747 2024-05-10 07:26:00.000000 pyfairylandfuture-1.0.0a10.post20240510/PyFairylandFuture.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      937 2024-05-10 07:26:00.000000 pyfairylandfuture-1.0.0a10.post20240510/PyFairylandFuture.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 07:26:00.000000 pyfairylandfuture-1.0.0a10.post20240510/PyFairylandFuture.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-05-10 07:26:00.000000 pyfairylandfuture-1.0.0a10.post20240510/PyFairylandFuture.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-10 07:26:00.000000 pyfairylandfuture-1.0.0a10.post20240510/PyFairylandFuture.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5696 2024-05-10 06:14:21.000000 pyfairylandfuture-1.0.0a10.post20240510/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 07:26:00.143284 pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/
--rw-rw-rw-   0        0        0      180 2024-05-09 08:15:49.000000 pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 07:26:00.144281 pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/api/
--rw-rw-rw-   0        0        0      180 2024-05-09 10:43:16.000000 pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 07:26:00.145278 pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/common/
--rw-rw-rw-   0        0        0      180 2024-05-09 10:44:07.000000 pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 07:26:00.149270 pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/constants/
--rw-rw-rw-   0        0        0      180 2024-05-09 10:44:31.000000 pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/constants/__init__.py
--rw-rw-rw-   0        0        0     1530 2024-05-10 04:40:06.000000 pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/constants/enums.py
--rw-rw-rw-   0        0        0      313 2024-05-10 03:32:06.000000 pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/constants/typed.py
-drwxrwxrwx   0        0        0        0 2024-05-10 07:26:00.150266 pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/core/
--rw-rw-rw-   0        0        0      180 2024-05-09 10:43:29.000000 pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 07:26:00.153259 pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/core/abstracts/
--rw-rw-rw-   0        0        0      180 2024-05-10 02:45:56.000000 pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/core/abstracts/__init__.py
--rw-rw-rw-   0        0        0     3363 2024-05-10 04:38:50.000000 pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/core/abstracts/enumerate.py
--rw-rw-rw-   0        0        0     1149 2024-05-10 04:39:23.000000 pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/core/abstracts/metaclass.py
-drwxrwxrwx   0        0        0        0 2024-05-10 07:26:00.159242 pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/modules/
--rw-rw-rw-   0        0        0      180 2024-05-09 10:46:13.000000 pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/modules/__init__.py
--rw-rw-rw-   0        0        0    13614 2024-05-10 06:10:06.000000 pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/modules/datetimes.py
--rw-rw-rw-   0        0        0     5715 2024-05-10 02:54:57.000000 pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/modules/decorators.py
--rw-rw-rw-   0        0        0     1249 2024-05-10 03:40:57.000000 pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/modules/exceptions.py
--rw-rw-rw-   0        0        0     6326 2024-05-10 04:37:27.000000 pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/modules/journal.py
-drwxrwxrwx   0        0        0        0 2024-05-10 07:26:00.161237 pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/test/
--rw-rw-rw-   0        0        0      180 2024-05-09 10:32:02.000000 pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 07:26:00.162235 pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/utils/
--rw-rw-rw-   0        0        0      180 2024-05-09 10:43:16.000000 pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 07:26:00.166224 pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/utils/general/
--rw-rw-rw-   0        0        0      180 2024-05-10 02:26:32.000000 pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/utils/general/__init__.py
--rw-rw-rw-   0        0        0     6140 2024-05-10 04:38:37.000000 pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/utils/general/constants.py
--rw-rw-rw-   0        0        0       42 2024-05-10 07:26:00.170214 pyfairylandfuture-1.0.0a10.post20240510/setup.cfg
--rw-rw-rw-   0        0        0     7398 2024-05-10 07:24:51.000000 pyfairylandfuture-1.0.0a10.post20240510/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 10:53:17.013385 pyfairylandfuture-1.0.0a30.post20240511/
+-rw-rw-rw-   0        0        0    34523 2024-05-09 08:14:38.000000 pyfairylandfuture-1.0.0a30.post20240511/LICENSE.txt
+-rw-rw-rw-   0        0        0     7883 2024-05-11 10:53:17.011391 pyfairylandfuture-1.0.0a30.post20240511/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-11 10:53:17.010393 pyfairylandfuture-1.0.0a30.post20240511/PyFairylandFuture.egg-info/
+-rw-rw-rw-   0        0        0     7883 2024-05-11 10:53:16.000000 pyfairylandfuture-1.0.0a30.post20240511/PyFairylandFuture.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1054 2024-05-11 10:53:16.000000 pyfairylandfuture-1.0.0a30.post20240511/PyFairylandFuture.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 10:53:16.000000 pyfairylandfuture-1.0.0a30.post20240511/PyFairylandFuture.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-11 10:53:16.000000 pyfairylandfuture-1.0.0a30.post20240511/PyFairylandFuture.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-11 10:53:16.000000 pyfairylandfuture-1.0.0a30.post20240511/PyFairylandFuture.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5860 2024-05-11 08:08:29.000000 pyfairylandfuture-1.0.0a30.post20240511/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 10:53:16.982468 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/
+-rw-rw-rw-   0        0        0      180 2024-05-09 08:15:49.000000 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 10:53:16.983465 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/api/
+-rw-rw-rw-   0        0        0      180 2024-05-09 10:43:16.000000 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 10:53:16.984462 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/common/
+-rw-rw-rw-   0        0        0      180 2024-05-09 10:44:07.000000 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 10:53:16.988478 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/constants/
+-rw-rw-rw-   0        0        0      180 2024-05-09 10:44:31.000000 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/constants/__init__.py
+-rw-rw-rw-   0        0        0     1530 2024-05-10 08:51:05.000000 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/constants/enums.py
+-rw-rw-rw-   0        0        0      313 2024-05-10 03:32:06.000000 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/constants/typed.py
+drwxrwxrwx   0        0        0        0 2024-05-11 10:53:16.989449 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/core/
+-rw-rw-rw-   0        0        0      180 2024-05-09 10:43:29.000000 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 10:53:16.993439 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/core/abstracts/
+-rw-rw-rw-   0        0        0      180 2024-05-10 02:45:56.000000 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/core/abstracts/__init__.py
+-rw-rw-rw-   0        0        0     3365 2024-05-10 10:12:39.000000 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/core/abstracts/enumerate.py
+-rw-rw-rw-   0        0        0     1158 2024-05-10 08:53:34.000000 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/core/abstracts/metaclass.py
+drwxrwxrwx   0        0        0        0 2024-05-11 10:53:17.000419 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/modules/
+-rw-rw-rw-   0        0        0      180 2024-05-09 10:46:13.000000 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/modules/__init__.py
+-rw-rw-rw-   0        0        0     3975 2024-05-11 06:41:11.000000 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/modules/datetimes.py
+-rw-rw-rw-   0        0        0     5723 2024-05-10 10:32:26.000000 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/modules/decorators.py
+-rw-rw-rw-   0        0        0     1249 2024-05-10 03:40:57.000000 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/modules/exceptions.py
+-rw-rw-rw-   0        0        0     6334 2024-05-10 08:52:14.000000 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/modules/journal.py
+drwxrwxrwx   0        0        0        0 2024-05-11 10:53:17.001416 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/scripts/
+-rw-rw-rw-   0        0        0      180 2024-05-11 09:20:11.000000 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/scripts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 10:53:17.003411 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/test/
+-rw-rw-rw-   0        0        0      180 2024-05-09 10:32:02.000000 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 10:53:17.004409 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/util/
+-rw-rw-rw-   0        0        0      180 2024-05-09 10:43:16.000000 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/util/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 10:53:17.006403 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/util/general/
+-rw-rw-rw-   0        0        0      180 2024-05-10 02:26:32.000000 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/util/general/__init__.py
+-rw-rw-rw-   0        0        0     6140 2024-05-10 04:38:37.000000 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/util/general/constants.py
+drwxrwxrwx   0        0        0        0 2024-05-11 10:53:17.008398 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/util/verifies/
+-rw-rw-rw-   0        0        0      180 2024-05-10 10:55:57.000000 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/util/verifies/__init__.py
+-rw-rw-rw-   0        0        0     1596 2024-05-10 11:12:45.000000 pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/util/verifies/validate.py
+-rw-rw-rw-   0        0        0       42 2024-05-11 10:53:17.013385 pyfairylandfuture-1.0.0a30.post20240511/setup.cfg
+-rw-rw-rw-   0        0        0     7812 2024-05-11 10:42:33.000000 pyfairylandfuture-1.0.0a30.post20240511/setup.py
```

### Comparing `pyfairylandfuture-1.0.0a10.post20240510/LICENSE.txt` & `pyfairylandfuture-1.0.0a30.post20240511/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyfairylandfuture-1.0.0a10.post20240510/PKG-INFO` & `pyfairylandfuture-1.0.0a30.post20240511/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFairylandFuture
-Version: 1.0.0a10.post20240510
+Version: 1.0.0a30.post20240511
 Summary: personally developed Python library.
 Home-page: https://github.com/PrettiestFairy/pypi-fairylandfuture
 Author: Lionel Johnson
 Author-email: fairylandfuture@outlook.com
 Keywords: fairyland,Fairyland,pyfairyland,PyFairyland,fairy,Fairy
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -35,86 +35,84 @@
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: Topic :: System :: Operating System Kernels :: Linux
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: loguru
-Requires-Dist: pip-review
 
 # PyPI - FairylandFuture
 
 > @software: PyCharm  
 > @author: [Lionel Johnson](https://fairy.host)  
 > @contact: [Blog](https://blog.fairy.host/) | [Github](https://github.com/PrettiestFairy) | [Telegram](https://t.me/FairylandFuture)  
 > @organization: [Github·FairylandFuture](https://github.com/FairylandFuture)  
 > @since: 2024-05-09 16:15:43 UTC+8
 
-[![Author](https://img.shields.io/badge/Author-Lionel_Johnson-orange)](https://t.me/FairylandFuture) [![github](https://img.shields.io/badge/Github-PrettiestFairy-green)](https://github.com/PrettiestFairy) [![GitBook](https://img.shields.io/badge/Gitbook-Interesting_book-green)](https://interestingbooks.gitbook.io/) [![Editor](https://img.shields.io/badge/Editor-Jetbrains_PyCharm-yellow)](https://www.jetbrains.com/pycharm) [![Language](https://img.shields.io/badge/Language-Markdown-orange)](https://en.wikipedia.org/wiki/Markdown) [![Version](https://img.shields.io/badge/Version-Release-blue)]() [![Docs](https://img.shields.io/badge/Docs-Passing-brightgreen)]() [![Type](https://img.shields.io/badge/Type-Document-blue)]() [![Wakatime](https://wakatime.com/badge/user/fa851759-c657-4b1e-8bcb-3ec3a693a2cd.svg)](https://wakatime.com/@fa851759-c657-4b1e-8bcb-3ec3a693a2cd) [![Sign](https://img.shields.io/badge/%E7%AD%89%E6%88%91%E4%BB%A3%E7%A0%81%E7%BC%96%E6%88%90-%E5%A8%B6%E4%BD%A0%E4%B8%BA%E5%A6%BB%E5%8F%AF%E5%A5%BD-red)](https://fairy.host)
+[![Author](https://img.shields.io/badge/Author-Lionel_Johnson-orange)](https://fairy.host) [![github](https://img.shields.io/badge/Github-Lionel_Johnson-green)](https://github.com/PrettiestFairy) [![GitBook](https://img.shields.io/badge/GitBook-Interesting-green)](https://interestingbooks.gitbook.io/) [![Editor](https://img.shields.io/badge/Editor-Typora-yellow)](https://github.com/PrettiestFairy) [![Language](https://img.shields.io/badge/Language-Markdown-orange)](https://github.com/PrettiestFairy) [![Version](https://img.shields.io/badge/Version-Release-blue)](https://github.com/PrettiestFairy) [![Docs](https://img.shields.io/badge/Docs-Passing-brightgreen)](https://github.com/PrettiestFairy) [![Type](https://img.shields.io/badge/Type-Document-blue)](https://github.com/PrettiestFairy) [![Wakatime](https://wakatime.com/badge/user/fa851759-c657-4b1e-8bcb-3ec3a693a2cd.svg)](https://wakatime.com/@fa851759-c657-4b1e-8bcb-3ec3a693a2cd) [![Sign](https://img.shields.io/badge/%E7%AD%89%E6%88%91%E4%BB%A3%E7%A0%81%E7%BC%96%E6%88%90-%E5%A8%B6%E4%BD%A0%E4%B8%BA%E5%A6%BB%E5%8F%AF%E5%A5%BD-red)](https://fairy.host)
 
 ---
 
-Development Environment
+Development Environment  
+**Please Higher than the version below**
 
-[![DevelopmentSystem](https://img.shields.io/badge/Development%20System-Win11%20Pro%20Workstations%2023H2%20Canary%20Channel-%230078D4?logo=windows11&logoColor=%230078D4)](https://www.microsoft.com/software-download/windows11) [![VCS](https://img.shields.io/badge/VCS-GitHub-%23181717?logo=github&logoColor=%23181717)](https://github.com/AustinFairyland) [![Anaconda](https://img.shields.io/badge/Anaconda-latest-%2344A833?logo=anaconda&logoColor=%2344A833)](https://www.anaconda.com/download#downloads) [![Python](https://img.shields.io/badge/Python-3.9.13-%233776AB?logo=python&logoColor=%233776AB)](https://www.python.org/downloads/release/python-3913/) [![Pip](https://img.shields.io/badge/PIP-23.2.1-%233775A9?logo=pypi&logoColor=%233775A9)](https://pypi.org/) ![MySQL](https://img.shields.io/badge/MySQL-8.0.33-%234479A1?logo=mysql&logoColor=%234479A1) [![GO](https://img.shields.io/badge/Go-1.20.6-%2300ADD8?logo=go&logoColor=%2300ADD8)](https://go.dev/dl/) ![NodeJS](https://img.shields.io/badge/Node-18.18.0-%23339933?logo=nodedotjs&logoColor=%23339933) ![Npm](https://img.shields.io/badge/Npm-10.1.0-%23CB3837?logo=npm&logoColor=%23CB3837) ![Pnpm](https://img.shields.io/badge/Pnpm-8.7.6-%23F69220?logo=pnpm&logoColor=%23F69220) ![Yarn](https://img.shields.io/badge/Yarn-1.22.19-%232C8EBB?logo=yarn&logoColor=%232C8EBB) ![Maven](https://img.shields.io/badge/Maven-3.9.1-%23C71A36?logo=apachemaven&logoColor=%23C71A36) ![Perl](https://img.shields.io/badge/Perl-8.3.0-%2339457E?logo=perl&logoColor=%2339457E) [![jetbrains](https://img.shields.io/badge/Jetbrains-2024-%2347f38a?logo=jetbrains&logoColor=%2347f38a)](https://www.jetbrains.com/) ![Git](https://img.shields.io/badge/Git-2.42.0-%23F05032?logo=git&logoColor=%23F05032) ![Chrome](https://img.shields.io/badge/Chrome-119_dev-%234285F4?logo=googlechrome&logoColor=%234285F4) ![AdaptingWindows](https://img.shields.io/badge/Adapting%20OS-Windows-%230078D4?logo=windows&logoColor=%230078D4) ![AdaptingLinux](https://img.shields.io/badge/Adapting%20OS-Linux-%23FCC624?logo=linux&logoColor=%23FCC624) ![AdaptingMac](https://img.shields.io/badge/Adapting%20OS-Mac-%23ffffff?logo=apple&logoColor=%23ffffff) ![Deployment](https://img.shields.io/badge/Deployment-Local-%2351BB7B?logo=local&logoColor=%2351BB7B) [![Deployment](https://img.shields.io/badge/Deployment-Docker-%232496ED?logo=docker&logoColor=%232496ED)](https://www.docker.com/) [![Deployment](https://img.shields.io/badge/Deployment-Kubernetes-%23326CE5?logo=kubernetes&logoColor=%23326CE5)](https://kubernetes.io/) [![Package](https://img.shields.io/badge/Package-requirements.txt-%2302A8EF?logo=packer&logoColor=%2302A8EF)](requirements.txt)
+[![DevelopmentSystem](https://img.shields.io/badge/Development%20System-Win11%20Pro%2023H2-%230078D4?logo=windows11&logoColor=%230078D4)](https://www.microsoft.com/software-download/windows11) [![VCS](https://img.shields.io/badge/VCS-GitHub-%23181717?logo=github&logoColor=%23181717)](https://github.com/PrettiestFairy) [![Anaconda](https://img.shields.io/badge/Anaconda-latest-%2344A833?logo=anaconda&logoColor=%2344A833)](https://www.anaconda.com/download#downloads) [![Python](https://img.shields.io/badge/Python-3.9.x~3.11.x-%233776AB?logo=python&logoColor=%233776AB)](https://www.python.org/downloads/release/python-3913/) [![Pip](https://img.shields.io/badge/PIP-latest-%233775A9?logo=pypi&logoColor=%233775A9)](https://pypi.org/) ![MySQL](https://img.shields.io/badge/MySQL-8.0.35-%234479A1?logo=mysql&logoColor=%234479A1) [![GO](https://img.shields.io/badge/Go-1.18-%2300ADD8?logo=go&logoColor=%2300ADD8)](https://go.dev/dl/) ![NodeJS](https://img.shields.io/badge/Node-18.19+-%23339933?logo=nodedotjs&logoColor=%23339933) ![Npm](https://img.shields.io/badge/Npm-10.x.x-%23CB3837?logo=npm&logoColor=%23CB3837) ![Pnpm](https://img.shields.io/badge/Pnpm-8.7.6-%23F69220?logo=pnpm&logoColor=%23F69220) ![Yarn](https://img.shields.io/badge/Yarn-1.22.19-%232C8EBB?logo=yarn&logoColor=%232C8EBB) ![Maven](https://img.shields.io/badge/Maven-3.9.1-%23C71A36?logo=apachemaven&logoColor=%23C71A36) ![Perl](https://img.shields.io/badge/Perl-8.3.0-%2339457E?logo=perl&logoColor=%2339457E) [![jetbrains](https://img.shields.io/badge/Jetbrains-2024-%2347f38a?logo=jetbrains&logoColor=%2347f38a)](https://www.jetbrains.com/) ![Git](https://img.shields.io/badge/Git-Release-%23F05032?logo=git&logoColor=%23F05032) ![Chrome](https://img.shields.io/badge/Chrome-Release_Release-%234285F4?logo=googlechrome&logoColor=%234285F4) ![AdaptingWindows](https://img.shields.io/badge/Adapting%20OS-Windows-%230078D4?logo=windows&logoColor=%230078D4) ![AdaptingLinux](https://img.shields.io/badge/Adapting%20OS-Linux-%23FCC624?logo=linux&logoColor=%23FCC624) ![AdaptingMac](https://img.shields.io/badge/Adapting%20OS-Mac-%23ffffff?logo=apple&logoColor=%23ffffff) ![Deployment](https://img.shields.io/badge/Deployment-Local-%2351BB7B?logo=local&logoColor=%2351BB7B) [![Deployment](https://img.shields.io/badge/Deployment-Docker-%232496ED?logo=docker&logoColor=%232496ED)](https://www.docker.com/) [![Deployment](https://img.shields.io/badge/Deployment-Kubernetes-%23326CE5?logo=kubernetes&logoColor=%23326CE5)](https://kubernetes.io/) [![Package](https://img.shields.io/badge/Python_Package-requirements.txt-%2302A8EF?logo=packer&logoColor=%2302A8EF)]()
 
 ---
 
 [**English** ✔️](README.md) | [简体中文 ✔️](docs/zh-CN/README-zh-CN.md) | [繁體中文 ❌]() | [日本語 ❌]() | [한국어 ❌]()
 
 ```text
  _____       _               _                    _  _____        _                      
 |  ___|__ _ (_) _ __  _   _ | |  __ _  _ __    __| ||  ___|_   _ | |_  _   _  _ __  ___  
 | |_  / _` || || '__|| | | || | / _` || '_ \  / _` || |_  | | | || __|| | | || '__|/ _ \ 
 |  _|| (_| || || |   | |_| || || (_| || | | || (_| ||  _| | |_| || |_ | |_| || |  |  __/ 
 |_|   \__,_||_||_|    \__, ||_| \__,_||_| |_| \__,_||_|    \__,_| \__| \__,_||_|   \___| 
                       |___/
 ```
 
-# Quick Start
+# 🚀 Quick Start
 
 ## Installation
 
 To install `PyFairylandFuture`, use the following command:
 
 ```shell
 pip install PyFairylandFuture
 ```
 
-# Document
+# ✍ Document
 
 ## Using PyFairyland Library
 
 Tips: Wait fill up
 
-# Further Information
+# 🎉 Further Information
 
 Tips: Wait fill up
 
-# Getting Support
+# 💚 Getting Support
 
 Tips: Wait fill up
 
-# Contributors
+# 🧑 Contributors
 
-Tips: Wait fill up
-
-![https://github.com/AustinFairyland/AustinFairylandRepository/graphs/contributors](https://contrib.rocks/image?repo=AustinFairyland/AustinFairylandRepository)
+![https://github.com/AustinFairyland/AustinFairylandRepository/graphs/contributors](https://contrib.rocks/image?repo=PrettiestFairy/pypi-fairylandfuture)
 
-[PrettiestFairy](https://github.com/PrettiestFairy) · [AustinEngineer](https://github.com/AustinEngineer) · []()
+[PrettiestFairy-Lionel Johnson(Admin)](https://github.com/PrettiestFairy) · [PrettiestFairy-Lionel Johnson(work)](https://github.com/AustinEngineer) · [duhuanzhuo](https://github.com/duhuanzhuo)
 
 Gitee:
 
 [maplethefox](https://gitee.com/maplethefox)
 
-# License
+# 📖 License
 
-The `PyFairylandGuture` module was written by Lionel Johnson. Personal maintained.
+The `PyFairylandFuture` module was written by Lionel Johnson. Personal maintained.
 
-`PyFairylandGuture` is released under the AGPLv3+ license.
+`PyFairylandFuture` is released under the AGPLv3+ license.
 
 See the file LICENSE for more details.
 
 ---
 
 [@HomePage](https://fairy.host) · [@Github](https://github.com/PrettiestFairy) · [@TelegramGroup]()
```

### Comparing `pyfairylandfuture-1.0.0a10.post20240510/PyFairylandFuture.egg-info/PKG-INFO` & `pyfairylandfuture-1.0.0a30.post20240511/PyFairylandFuture.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFairylandFuture
-Version: 1.0.0a10.post20240510
+Version: 1.0.0a30.post20240511
 Summary: personally developed Python library.
 Home-page: https://github.com/PrettiestFairy/pypi-fairylandfuture
 Author: Lionel Johnson
 Author-email: fairylandfuture@outlook.com
 Keywords: fairyland,Fairyland,pyfairyland,PyFairyland,fairy,Fairy
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -35,86 +35,84 @@
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: Topic :: System :: Operating System Kernels :: Linux
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: loguru
-Requires-Dist: pip-review
 
 # PyPI - FairylandFuture
 
 > @software: PyCharm  
 > @author: [Lionel Johnson](https://fairy.host)  
 > @contact: [Blog](https://blog.fairy.host/) | [Github](https://github.com/PrettiestFairy) | [Telegram](https://t.me/FairylandFuture)  
 > @organization: [Github·FairylandFuture](https://github.com/FairylandFuture)  
 > @since: 2024-05-09 16:15:43 UTC+8
 
-[![Author](https://img.shields.io/badge/Author-Lionel_Johnson-orange)](https://t.me/FairylandFuture) [![github](https://img.shields.io/badge/Github-PrettiestFairy-green)](https://github.com/PrettiestFairy) [![GitBook](https://img.shields.io/badge/Gitbook-Interesting_book-green)](https://interestingbooks.gitbook.io/) [![Editor](https://img.shields.io/badge/Editor-Jetbrains_PyCharm-yellow)](https://www.jetbrains.com/pycharm) [![Language](https://img.shields.io/badge/Language-Markdown-orange)](https://en.wikipedia.org/wiki/Markdown) [![Version](https://img.shields.io/badge/Version-Release-blue)]() [![Docs](https://img.shields.io/badge/Docs-Passing-brightgreen)]() [![Type](https://img.shields.io/badge/Type-Document-blue)]() [![Wakatime](https://wakatime.com/badge/user/fa851759-c657-4b1e-8bcb-3ec3a693a2cd.svg)](https://wakatime.com/@fa851759-c657-4b1e-8bcb-3ec3a693a2cd) [![Sign](https://img.shields.io/badge/%E7%AD%89%E6%88%91%E4%BB%A3%E7%A0%81%E7%BC%96%E6%88%90-%E5%A8%B6%E4%BD%A0%E4%B8%BA%E5%A6%BB%E5%8F%AF%E5%A5%BD-red)](https://fairy.host)
+[![Author](https://img.shields.io/badge/Author-Lionel_Johnson-orange)](https://fairy.host) [![github](https://img.shields.io/badge/Github-Lionel_Johnson-green)](https://github.com/PrettiestFairy) [![GitBook](https://img.shields.io/badge/GitBook-Interesting-green)](https://interestingbooks.gitbook.io/) [![Editor](https://img.shields.io/badge/Editor-Typora-yellow)](https://github.com/PrettiestFairy) [![Language](https://img.shields.io/badge/Language-Markdown-orange)](https://github.com/PrettiestFairy) [![Version](https://img.shields.io/badge/Version-Release-blue)](https://github.com/PrettiestFairy) [![Docs](https://img.shields.io/badge/Docs-Passing-brightgreen)](https://github.com/PrettiestFairy) [![Type](https://img.shields.io/badge/Type-Document-blue)](https://github.com/PrettiestFairy) [![Wakatime](https://wakatime.com/badge/user/fa851759-c657-4b1e-8bcb-3ec3a693a2cd.svg)](https://wakatime.com/@fa851759-c657-4b1e-8bcb-3ec3a693a2cd) [![Sign](https://img.shields.io/badge/%E7%AD%89%E6%88%91%E4%BB%A3%E7%A0%81%E7%BC%96%E6%88%90-%E5%A8%B6%E4%BD%A0%E4%B8%BA%E5%A6%BB%E5%8F%AF%E5%A5%BD-red)](https://fairy.host)
 
 ---
 
-Development Environment
+Development Environment  
+**Please Higher than the version below**
 
-[![DevelopmentSystem](https://img.shields.io/badge/Development%20System-Win11%20Pro%20Workstations%2023H2%20Canary%20Channel-%230078D4?logo=windows11&logoColor=%230078D4)](https://www.microsoft.com/software-download/windows11) [![VCS](https://img.shields.io/badge/VCS-GitHub-%23181717?logo=github&logoColor=%23181717)](https://github.com/AustinFairyland) [![Anaconda](https://img.shields.io/badge/Anaconda-latest-%2344A833?logo=anaconda&logoColor=%2344A833)](https://www.anaconda.com/download#downloads) [![Python](https://img.shields.io/badge/Python-3.9.13-%233776AB?logo=python&logoColor=%233776AB)](https://www.python.org/downloads/release/python-3913/) [![Pip](https://img.shields.io/badge/PIP-23.2.1-%233775A9?logo=pypi&logoColor=%233775A9)](https://pypi.org/) ![MySQL](https://img.shields.io/badge/MySQL-8.0.33-%234479A1?logo=mysql&logoColor=%234479A1) [![GO](https://img.shields.io/badge/Go-1.20.6-%2300ADD8?logo=go&logoColor=%2300ADD8)](https://go.dev/dl/) ![NodeJS](https://img.shields.io/badge/Node-18.18.0-%23339933?logo=nodedotjs&logoColor=%23339933) ![Npm](https://img.shields.io/badge/Npm-10.1.0-%23CB3837?logo=npm&logoColor=%23CB3837) ![Pnpm](https://img.shields.io/badge/Pnpm-8.7.6-%23F69220?logo=pnpm&logoColor=%23F69220) ![Yarn](https://img.shields.io/badge/Yarn-1.22.19-%232C8EBB?logo=yarn&logoColor=%232C8EBB) ![Maven](https://img.shields.io/badge/Maven-3.9.1-%23C71A36?logo=apachemaven&logoColor=%23C71A36) ![Perl](https://img.shields.io/badge/Perl-8.3.0-%2339457E?logo=perl&logoColor=%2339457E) [![jetbrains](https://img.shields.io/badge/Jetbrains-2024-%2347f38a?logo=jetbrains&logoColor=%2347f38a)](https://www.jetbrains.com/) ![Git](https://img.shields.io/badge/Git-2.42.0-%23F05032?logo=git&logoColor=%23F05032) ![Chrome](https://img.shields.io/badge/Chrome-119_dev-%234285F4?logo=googlechrome&logoColor=%234285F4) ![AdaptingWindows](https://img.shields.io/badge/Adapting%20OS-Windows-%230078D4?logo=windows&logoColor=%230078D4) ![AdaptingLinux](https://img.shields.io/badge/Adapting%20OS-Linux-%23FCC624?logo=linux&logoColor=%23FCC624) ![AdaptingMac](https://img.shields.io/badge/Adapting%20OS-Mac-%23ffffff?logo=apple&logoColor=%23ffffff) ![Deployment](https://img.shields.io/badge/Deployment-Local-%2351BB7B?logo=local&logoColor=%2351BB7B) [![Deployment](https://img.shields.io/badge/Deployment-Docker-%232496ED?logo=docker&logoColor=%232496ED)](https://www.docker.com/) [![Deployment](https://img.shields.io/badge/Deployment-Kubernetes-%23326CE5?logo=kubernetes&logoColor=%23326CE5)](https://kubernetes.io/) [![Package](https://img.shields.io/badge/Package-requirements.txt-%2302A8EF?logo=packer&logoColor=%2302A8EF)](requirements.txt)
+[![DevelopmentSystem](https://img.shields.io/badge/Development%20System-Win11%20Pro%2023H2-%230078D4?logo=windows11&logoColor=%230078D4)](https://www.microsoft.com/software-download/windows11) [![VCS](https://img.shields.io/badge/VCS-GitHub-%23181717?logo=github&logoColor=%23181717)](https://github.com/PrettiestFairy) [![Anaconda](https://img.shields.io/badge/Anaconda-latest-%2344A833?logo=anaconda&logoColor=%2344A833)](https://www.anaconda.com/download#downloads) [![Python](https://img.shields.io/badge/Python-3.9.x~3.11.x-%233776AB?logo=python&logoColor=%233776AB)](https://www.python.org/downloads/release/python-3913/) [![Pip](https://img.shields.io/badge/PIP-latest-%233775A9?logo=pypi&logoColor=%233775A9)](https://pypi.org/) ![MySQL](https://img.shields.io/badge/MySQL-8.0.35-%234479A1?logo=mysql&logoColor=%234479A1) [![GO](https://img.shields.io/badge/Go-1.18-%2300ADD8?logo=go&logoColor=%2300ADD8)](https://go.dev/dl/) ![NodeJS](https://img.shields.io/badge/Node-18.19+-%23339933?logo=nodedotjs&logoColor=%23339933) ![Npm](https://img.shields.io/badge/Npm-10.x.x-%23CB3837?logo=npm&logoColor=%23CB3837) ![Pnpm](https://img.shields.io/badge/Pnpm-8.7.6-%23F69220?logo=pnpm&logoColor=%23F69220) ![Yarn](https://img.shields.io/badge/Yarn-1.22.19-%232C8EBB?logo=yarn&logoColor=%232C8EBB) ![Maven](https://img.shields.io/badge/Maven-3.9.1-%23C71A36?logo=apachemaven&logoColor=%23C71A36) ![Perl](https://img.shields.io/badge/Perl-8.3.0-%2339457E?logo=perl&logoColor=%2339457E) [![jetbrains](https://img.shields.io/badge/Jetbrains-2024-%2347f38a?logo=jetbrains&logoColor=%2347f38a)](https://www.jetbrains.com/) ![Git](https://img.shields.io/badge/Git-Release-%23F05032?logo=git&logoColor=%23F05032) ![Chrome](https://img.shields.io/badge/Chrome-Release_Release-%234285F4?logo=googlechrome&logoColor=%234285F4) ![AdaptingWindows](https://img.shields.io/badge/Adapting%20OS-Windows-%230078D4?logo=windows&logoColor=%230078D4) ![AdaptingLinux](https://img.shields.io/badge/Adapting%20OS-Linux-%23FCC624?logo=linux&logoColor=%23FCC624) ![AdaptingMac](https://img.shields.io/badge/Adapting%20OS-Mac-%23ffffff?logo=apple&logoColor=%23ffffff) ![Deployment](https://img.shields.io/badge/Deployment-Local-%2351BB7B?logo=local&logoColor=%2351BB7B) [![Deployment](https://img.shields.io/badge/Deployment-Docker-%232496ED?logo=docker&logoColor=%232496ED)](https://www.docker.com/) [![Deployment](https://img.shields.io/badge/Deployment-Kubernetes-%23326CE5?logo=kubernetes&logoColor=%23326CE5)](https://kubernetes.io/) [![Package](https://img.shields.io/badge/Python_Package-requirements.txt-%2302A8EF?logo=packer&logoColor=%2302A8EF)]()
 
 ---
 
 [**English** ✔️](README.md) | [简体中文 ✔️](docs/zh-CN/README-zh-CN.md) | [繁體中文 ❌]() | [日本語 ❌]() | [한국어 ❌]()
 
 ```text
  _____       _               _                    _  _____        _                      
 |  ___|__ _ (_) _ __  _   _ | |  __ _  _ __    __| ||  ___|_   _ | |_  _   _  _ __  ___  
 | |_  / _` || || '__|| | | || | / _` || '_ \  / _` || |_  | | | || __|| | | || '__|/ _ \ 
 |  _|| (_| || || |   | |_| || || (_| || | | || (_| ||  _| | |_| || |_ | |_| || |  |  __/ 
 |_|   \__,_||_||_|    \__, ||_| \__,_||_| |_| \__,_||_|    \__,_| \__| \__,_||_|   \___| 
                       |___/
 ```
 
-# Quick Start
+# 🚀 Quick Start
 
 ## Installation
 
 To install `PyFairylandFuture`, use the following command:
 
 ```shell
 pip install PyFairylandFuture
 ```
 
-# Document
+# ✍ Document
 
 ## Using PyFairyland Library
 
 Tips: Wait fill up
 
-# Further Information
+# 🎉 Further Information
 
 Tips: Wait fill up
 
-# Getting Support
+# 💚 Getting Support
 
 Tips: Wait fill up
 
-# Contributors
+# 🧑 Contributors
 
-Tips: Wait fill up
-
-![https://github.com/AustinFairyland/AustinFairylandRepository/graphs/contributors](https://contrib.rocks/image?repo=AustinFairyland/AustinFairylandRepository)
+![https://github.com/AustinFairyland/AustinFairylandRepository/graphs/contributors](https://contrib.rocks/image?repo=PrettiestFairy/pypi-fairylandfuture)
 
-[PrettiestFairy](https://github.com/PrettiestFairy) · [AustinEngineer](https://github.com/AustinEngineer) · []()
+[PrettiestFairy-Lionel Johnson(Admin)](https://github.com/PrettiestFairy) · [PrettiestFairy-Lionel Johnson(work)](https://github.com/AustinEngineer) · [duhuanzhuo](https://github.com/duhuanzhuo)
 
 Gitee:
 
 [maplethefox](https://gitee.com/maplethefox)
 
-# License
+# 📖 License
 
-The `PyFairylandGuture` module was written by Lionel Johnson. Personal maintained.
+The `PyFairylandFuture` module was written by Lionel Johnson. Personal maintained.
 
-`PyFairylandGuture` is released under the AGPLv3+ license.
+`PyFairylandFuture` is released under the AGPLv3+ license.
 
 See the file LICENSE for more details.
 
 ---
 
 [@HomePage](https://fairy.host) · [@Github](https://github.com/PrettiestFairy) · [@TelegramGroup]()
```

### Comparing `pyfairylandfuture-1.0.0a10.post20240510/PyFairylandFuture.egg-info/SOURCES.txt` & `pyfairylandfuture-1.0.0a30.post20240511/PyFairylandFuture.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -17,11 +17,14 @@
 fairylandfuture/core/abstracts/enumerate.py
 fairylandfuture/core/abstracts/metaclass.py
 fairylandfuture/modules/__init__.py
 fairylandfuture/modules/datetimes.py
 fairylandfuture/modules/decorators.py
 fairylandfuture/modules/exceptions.py
 fairylandfuture/modules/journal.py
+fairylandfuture/scripts/__init__.py
 fairylandfuture/test/__init__.py
-fairylandfuture/utils/__init__.py
-fairylandfuture/utils/general/__init__.py
-fairylandfuture/utils/general/constants.py
+fairylandfuture/util/__init__.py
+fairylandfuture/util/general/__init__.py
+fairylandfuture/util/general/constants.py
+fairylandfuture/util/verifies/__init__.py
+fairylandfuture/util/verifies/validate.py
```

### Comparing `pyfairylandfuture-1.0.0a10.post20240510/README.md` & `pyfairylandfuture-1.0.0a30.post20240511/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,76 +2,75 @@
 
 > @software: PyCharm  
 > @author: [Lionel Johnson](https://fairy.host)  
 > @contact: [Blog](https://blog.fairy.host/) | [Github](https://github.com/PrettiestFairy) | [Telegram](https://t.me/FairylandFuture)  
 > @organization: [Github·FairylandFuture](https://github.com/FairylandFuture)  
 > @since: 2024-05-09 16:15:43 UTC+8
 
-[![Author](https://img.shields.io/badge/Author-Lionel_Johnson-orange)](https://t.me/FairylandFuture) [![github](https://img.shields.io/badge/Github-PrettiestFairy-green)](https://github.com/PrettiestFairy) [![GitBook](https://img.shields.io/badge/Gitbook-Interesting_book-green)](https://interestingbooks.gitbook.io/) [![Editor](https://img.shields.io/badge/Editor-Jetbrains_PyCharm-yellow)](https://www.jetbrains.com/pycharm) [![Language](https://img.shields.io/badge/Language-Markdown-orange)](https://en.wikipedia.org/wiki/Markdown) [![Version](https://img.shields.io/badge/Version-Release-blue)]() [![Docs](https://img.shields.io/badge/Docs-Passing-brightgreen)]() [![Type](https://img.shields.io/badge/Type-Document-blue)]() [![Wakatime](https://wakatime.com/badge/user/fa851759-c657-4b1e-8bcb-3ec3a693a2cd.svg)](https://wakatime.com/@fa851759-c657-4b1e-8bcb-3ec3a693a2cd) [![Sign](https://img.shields.io/badge/%E7%AD%89%E6%88%91%E4%BB%A3%E7%A0%81%E7%BC%96%E6%88%90-%E5%A8%B6%E4%BD%A0%E4%B8%BA%E5%A6%BB%E5%8F%AF%E5%A5%BD-red)](https://fairy.host)
+[![Author](https://img.shields.io/badge/Author-Lionel_Johnson-orange)](https://fairy.host) [![github](https://img.shields.io/badge/Github-Lionel_Johnson-green)](https://github.com/PrettiestFairy) [![GitBook](https://img.shields.io/badge/GitBook-Interesting-green)](https://interestingbooks.gitbook.io/) [![Editor](https://img.shields.io/badge/Editor-Typora-yellow)](https://github.com/PrettiestFairy) [![Language](https://img.shields.io/badge/Language-Markdown-orange)](https://github.com/PrettiestFairy) [![Version](https://img.shields.io/badge/Version-Release-blue)](https://github.com/PrettiestFairy) [![Docs](https://img.shields.io/badge/Docs-Passing-brightgreen)](https://github.com/PrettiestFairy) [![Type](https://img.shields.io/badge/Type-Document-blue)](https://github.com/PrettiestFairy) [![Wakatime](https://wakatime.com/badge/user/fa851759-c657-4b1e-8bcb-3ec3a693a2cd.svg)](https://wakatime.com/@fa851759-c657-4b1e-8bcb-3ec3a693a2cd) [![Sign](https://img.shields.io/badge/%E7%AD%89%E6%88%91%E4%BB%A3%E7%A0%81%E7%BC%96%E6%88%90-%E5%A8%B6%E4%BD%A0%E4%B8%BA%E5%A6%BB%E5%8F%AF%E5%A5%BD-red)](https://fairy.host)
 
 ---
 
-Development Environment
+Development Environment  
+**Please Higher than the version below**
 
-[![DevelopmentSystem](https://img.shields.io/badge/Development%20System-Win11%20Pro%20Workstations%2023H2%20Canary%20Channel-%230078D4?logo=windows11&logoColor=%230078D4)](https://www.microsoft.com/software-download/windows11) [![VCS](https://img.shields.io/badge/VCS-GitHub-%23181717?logo=github&logoColor=%23181717)](https://github.com/AustinFairyland) [![Anaconda](https://img.shields.io/badge/Anaconda-latest-%2344A833?logo=anaconda&logoColor=%2344A833)](https://www.anaconda.com/download#downloads) [![Python](https://img.shields.io/badge/Python-3.9.13-%233776AB?logo=python&logoColor=%233776AB)](https://www.python.org/downloads/release/python-3913/) [![Pip](https://img.shields.io/badge/PIP-23.2.1-%233775A9?logo=pypi&logoColor=%233775A9)](https://pypi.org/) ![MySQL](https://img.shields.io/badge/MySQL-8.0.33-%234479A1?logo=mysql&logoColor=%234479A1) [![GO](https://img.shields.io/badge/Go-1.20.6-%2300ADD8?logo=go&logoColor=%2300ADD8)](https://go.dev/dl/) ![NodeJS](https://img.shields.io/badge/Node-18.18.0-%23339933?logo=nodedotjs&logoColor=%23339933) ![Npm](https://img.shields.io/badge/Npm-10.1.0-%23CB3837?logo=npm&logoColor=%23CB3837) ![Pnpm](https://img.shields.io/badge/Pnpm-8.7.6-%23F69220?logo=pnpm&logoColor=%23F69220) ![Yarn](https://img.shields.io/badge/Yarn-1.22.19-%232C8EBB?logo=yarn&logoColor=%232C8EBB) ![Maven](https://img.shields.io/badge/Maven-3.9.1-%23C71A36?logo=apachemaven&logoColor=%23C71A36) ![Perl](https://img.shields.io/badge/Perl-8.3.0-%2339457E?logo=perl&logoColor=%2339457E) [![jetbrains](https://img.shields.io/badge/Jetbrains-2024-%2347f38a?logo=jetbrains&logoColor=%2347f38a)](https://www.jetbrains.com/) ![Git](https://img.shields.io/badge/Git-2.42.0-%23F05032?logo=git&logoColor=%23F05032) ![Chrome](https://img.shields.io/badge/Chrome-119_dev-%234285F4?logo=googlechrome&logoColor=%234285F4) ![AdaptingWindows](https://img.shields.io/badge/Adapting%20OS-Windows-%230078D4?logo=windows&logoColor=%230078D4) ![AdaptingLinux](https://img.shields.io/badge/Adapting%20OS-Linux-%23FCC624?logo=linux&logoColor=%23FCC624) ![AdaptingMac](https://img.shields.io/badge/Adapting%20OS-Mac-%23ffffff?logo=apple&logoColor=%23ffffff) ![Deployment](https://img.shields.io/badge/Deployment-Local-%2351BB7B?logo=local&logoColor=%2351BB7B) [![Deployment](https://img.shields.io/badge/Deployment-Docker-%232496ED?logo=docker&logoColor=%232496ED)](https://www.docker.com/) [![Deployment](https://img.shields.io/badge/Deployment-Kubernetes-%23326CE5?logo=kubernetes&logoColor=%23326CE5)](https://kubernetes.io/) [![Package](https://img.shields.io/badge/Package-requirements.txt-%2302A8EF?logo=packer&logoColor=%2302A8EF)](requirements.txt)
+[![DevelopmentSystem](https://img.shields.io/badge/Development%20System-Win11%20Pro%2023H2-%230078D4?logo=windows11&logoColor=%230078D4)](https://www.microsoft.com/software-download/windows11) [![VCS](https://img.shields.io/badge/VCS-GitHub-%23181717?logo=github&logoColor=%23181717)](https://github.com/PrettiestFairy) [![Anaconda](https://img.shields.io/badge/Anaconda-latest-%2344A833?logo=anaconda&logoColor=%2344A833)](https://www.anaconda.com/download#downloads) [![Python](https://img.shields.io/badge/Python-3.9.x~3.11.x-%233776AB?logo=python&logoColor=%233776AB)](https://www.python.org/downloads/release/python-3913/) [![Pip](https://img.shields.io/badge/PIP-latest-%233775A9?logo=pypi&logoColor=%233775A9)](https://pypi.org/) ![MySQL](https://img.shields.io/badge/MySQL-8.0.35-%234479A1?logo=mysql&logoColor=%234479A1) [![GO](https://img.shields.io/badge/Go-1.18-%2300ADD8?logo=go&logoColor=%2300ADD8)](https://go.dev/dl/) ![NodeJS](https://img.shields.io/badge/Node-18.19+-%23339933?logo=nodedotjs&logoColor=%23339933) ![Npm](https://img.shields.io/badge/Npm-10.x.x-%23CB3837?logo=npm&logoColor=%23CB3837) ![Pnpm](https://img.shields.io/badge/Pnpm-8.7.6-%23F69220?logo=pnpm&logoColor=%23F69220) ![Yarn](https://img.shields.io/badge/Yarn-1.22.19-%232C8EBB?logo=yarn&logoColor=%232C8EBB) ![Maven](https://img.shields.io/badge/Maven-3.9.1-%23C71A36?logo=apachemaven&logoColor=%23C71A36) ![Perl](https://img.shields.io/badge/Perl-8.3.0-%2339457E?logo=perl&logoColor=%2339457E) [![jetbrains](https://img.shields.io/badge/Jetbrains-2024-%2347f38a?logo=jetbrains&logoColor=%2347f38a)](https://www.jetbrains.com/) ![Git](https://img.shields.io/badge/Git-Release-%23F05032?logo=git&logoColor=%23F05032) ![Chrome](https://img.shields.io/badge/Chrome-Release_Release-%234285F4?logo=googlechrome&logoColor=%234285F4) ![AdaptingWindows](https://img.shields.io/badge/Adapting%20OS-Windows-%230078D4?logo=windows&logoColor=%230078D4) ![AdaptingLinux](https://img.shields.io/badge/Adapting%20OS-Linux-%23FCC624?logo=linux&logoColor=%23FCC624) ![AdaptingMac](https://img.shields.io/badge/Adapting%20OS-Mac-%23ffffff?logo=apple&logoColor=%23ffffff) ![Deployment](https://img.shields.io/badge/Deployment-Local-%2351BB7B?logo=local&logoColor=%2351BB7B) [![Deployment](https://img.shields.io/badge/Deployment-Docker-%232496ED?logo=docker&logoColor=%232496ED)](https://www.docker.com/) [![Deployment](https://img.shields.io/badge/Deployment-Kubernetes-%23326CE5?logo=kubernetes&logoColor=%23326CE5)](https://kubernetes.io/) [![Package](https://img.shields.io/badge/Python_Package-requirements.txt-%2302A8EF?logo=packer&logoColor=%2302A8EF)]()
 
 ---
 
 [**English** ✔️](README.md) | [简体中文 ✔️](docs/zh-CN/README-zh-CN.md) | [繁體中文 ❌]() | [日本語 ❌]() | [한국어 ❌]()
 
 ```text
  _____       _               _                    _  _____        _                      
 |  ___|__ _ (_) _ __  _   _ | |  __ _  _ __    __| ||  ___|_   _ | |_  _   _  _ __  ___  
 | |_  / _` || || '__|| | | || | / _` || '_ \  / _` || |_  | | | || __|| | | || '__|/ _ \ 
 |  _|| (_| || || |   | |_| || || (_| || | | || (_| ||  _| | |_| || |_ | |_| || |  |  __/ 
 |_|   \__,_||_||_|    \__, ||_| \__,_||_| |_| \__,_||_|    \__,_| \__| \__,_||_|   \___| 
                       |___/
 ```
 
-# Quick Start
+# 🚀 Quick Start
 
 ## Installation
 
 To install `PyFairylandFuture`, use the following command:
 
 ```shell
 pip install PyFairylandFuture
 ```
 
-# Document
+# ✍ Document
 
 ## Using PyFairyland Library
 
 Tips: Wait fill up
 
-# Further Information
+# 🎉 Further Information
 
 Tips: Wait fill up
 
-# Getting Support
+# 💚 Getting Support
 
 Tips: Wait fill up
 
-# Contributors
+# 🧑 Contributors
 
-Tips: Wait fill up
-
-![https://github.com/AustinFairyland/AustinFairylandRepository/graphs/contributors](https://contrib.rocks/image?repo=AustinFairyland/AustinFairylandRepository)
+![https://github.com/AustinFairyland/AustinFairylandRepository/graphs/contributors](https://contrib.rocks/image?repo=PrettiestFairy/pypi-fairylandfuture)
 
-[PrettiestFairy](https://github.com/PrettiestFairy) · [AustinEngineer](https://github.com/AustinEngineer) · []()
+[PrettiestFairy-Lionel Johnson(Admin)](https://github.com/PrettiestFairy) · [PrettiestFairy-Lionel Johnson(work)](https://github.com/AustinEngineer) · [duhuanzhuo](https://github.com/duhuanzhuo)
 
 Gitee:
 
 [maplethefox](https://gitee.com/maplethefox)
 
-# License
+# 📖 License
 
-The `PyFairylandGuture` module was written by Lionel Johnson. Personal maintained.
+The `PyFairylandFuture` module was written by Lionel Johnson. Personal maintained.
 
-`PyFairylandGuture` is released under the AGPLv3+ license.
+`PyFairylandFuture` is released under the AGPLv3+ license.
 
 See the file LICENSE for more details.
 
 ---
 
 [@HomePage](https://fairy.host) · [@Github](https://github.com/PrettiestFairy) · [@TelegramGroup]()
```

### Comparing `pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/constants/enums.py` & `pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/constants/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,30 +31,30 @@
         return cls.DATETIME.value
 
     @classmethod
     def default_cn(cls) -> str:
         return cls.DATETIME_CN.value
 
 
-class EncodingEnum(BaseEnum):
+class EncodingEnum(EnumBase):
     """
     Encoding enum.
     """
 
     UTF_8 = utf_8 = "UTF-8"
     GBK = gbk = "GBK"
     GB2312 = gb2312 = "GB2312"
     GB18030 = gb18030 = "GB18030"
 
     @classmethod
     def default(cls) -> str:
         return cls.UTF_8.value
 
 
-class LogLevelEnum(BaseEnum):
+class LogLevelEnum(EnumBase):
     """
     Log level Enum.
     """
 
     TRACE = trace = "TRACE"
     DEBUG = debug = "DEBUG"
     INFO = info = "INFO"
```

### Comparing `pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/core/abstracts/enumerate.py` & `pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/core/abstracts/enumerate.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,49 +30,49 @@
         raise NotImplementedError("Implement it in a subclass.")
 
     @classmethod
     def get(cls, value: str) -> Any:
         """
         Get the Enum value by member.
 
-        :param value: Attribute name
+        :param value: Attribute action
         :type value: str
         :return: Attribute value
         :rtype: ...
         """
         if not isinstance(value, str):
             raise TypeError("The value must be a string.")
 
-        value_object: _TypeBaseEnum = getattr(cls, value)
+        value_object: _TypeEnumBase = getattr(cls, value)
 
         return value_object.value
 
     @classmethod
     def members(
         cls,
         exclude_enums: Union[List[str], Tuple[str, ...], Set[str]] = None,
         only_value: bool = False,
-    ) -> Union[Tuple[_TypeBaseEnum, ...], Tuple[Any, ...]]:
+    ) -> Union[Tuple[_TypeEnumBase, ...], Tuple[Any, ...]]:
         """
         Returns a tuple with all members of the Enum.
 
         :param exclude_enums: List of members to exclude from the result.
         :type exclude_enums: list or tuple or set
         :param only_value: If True, returns only the values of the members.
         :type only_value: bool
         :return: Tuple with all members of the Enum.
         :rtype: tuple
         """
         if exclude_enums and not isinstance(exclude_enums, (list, tuple, set)):
             raise TypeError("The exclude_enums must be a list, tuple or set.")
 
-        member_list: List[_TypeBaseEnum] = list(cls)
+        member_list: List[_TypeEnumBase] = list(cls)
 
         if exclude_enums:
-            member_list: List[_TypeBaseEnum] = [member for member in member_list if member not in exclude_enums]
+            member_list: List[_TypeEnumBase] = [member for member in member_list if member not in exclude_enums]
 
         if only_value:
             return tuple(member.value for member in member_list)
         else:
             return tuple(member_list)
 
     @classmethod
```

### Comparing `pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/core/abstracts/metaclass.py` & `pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/core/abstracts/metaclass.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 @author: Lionel Johnson
 @contact: https://fairy.host
 @organization: https://github.com/FairylandFuture
 @since: 2024-05-10 10:58:14 UTC+8
 """
 
 import functools
+import abc
 
 from typing import Any, Dict
 
 
 class SingletonMeta(type):
     """
     Singleton pattern metaclass
@@ -32,17 +33,18 @@
         if not hasattr(cls, "__instance"):
             setattr(cls, "__instance", super().__call__(*args, **kwargs))
             return getattr(cls, "__instance")
         else:
             return getattr(cls, "__instance")
 
 
-class SingletonABCMeta(ABCMeta):
+class SingletonABCMeta(abc.ABCMeta):
     """
     Singleton meta
     """
+
     _instances: Dict[type, object] = dict()
 
-    def __call__(self, *args, **kwargs):
-        if self not in self._instances:
-            self._instances.update({self: super().__call__(*args, **kwargs)})
-        return self._instances.get(self)
+    def __call__(cls, *args, **kwargs):
+        if cls not in cls._instances:
+            cls._instances.update({cls: super().__call__(*args, **kwargs)})
+        return cls._instances.get(cls)
```

### Comparing `pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/modules/decorators.py` & `pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/modules/decorators.py`

 * *Files 9% similar despite different names*

```diff
@@ -86,27 +86,27 @@
         return results
 
 
 class ActionDecorator:
     """
     Decorator to log method execution tips (start, success, failure).
 
-    :param name: The name of the method for logging purposes. Defaults to "A Method".
-    :type name: str
+    :param action: The name of the method for logging purposes. Defaults to "A Method".
+    :type action: str
     """
 
-    def __init__(self, name: str = "A Method"):
-        self.__name = name
+    def __init__(self, action: str = "A Method"):
+        self.__action = action
 
-    def __call__(self, __method: Union[FunctionType, MethodType], *args: Any, **kwargs: Any) -> Callable[..., Any]:
+    def __call__(self, method: Union[FunctionType, MethodType], *args: Any, **kwargs: Any) -> Callable[..., Any]:
         """
         The decorator's logic to wrap around the given method.
 
-        :param __method: The function or method to be decorated.
-        :type __method: FunctionType or MethodType
+        :param method: The function or method to be decorated.
+        :type method: FunctionType or MethodType
         :param args: args
         :type args: Any
         :param kwargs: kwargs
         :type kwargs: Any
         :return: The wrapper function around the original method.
         :rtype: Callable
         """
@@ -119,20 +119,20 @@
             :type args: Any
             :param kwargs: Keyword arguments for the decorated method.
             :type kwargs: Any
             :return: The return value of the decorated method.
             :rtype: ...
             """
             try:
-                journal.info(f"Action Running {self.__name}")
-                results = __method(*args, **kwargs)
-                journal.success(f"Success Running {self.__name}")
+                journal.info(f"Action Running {self.__action}")
+                results = method(*args, **kwargs)
+                journal.success(f"Success Running {self.__action}")
             except Exception as error:
                 journal.exception(error)
-                journal.error(f"Failure Running {self.__name}")
+                journal.error(f"Failure Running {self.__action}")
                 journal.error(error.args.__getitem__(0))
                 raise error
 
             return results
 
         return wrapper
```

### Comparing `pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/modules/exceptions.py` & `pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/modules/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/modules/journal.py` & `pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/modules/journal.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,19 @@
 @since: 02 29, 2024
 """
 
 import sys
 from loguru import logger
 
 from fairylandfuture.constants.typed import TypeLogLevel
-from fairylandfuture.modules.decorators import SingletonDecorator
 from fairylandfuture.constants.enums import EncodingEnum, LogLevelEnum
+from fairylandfuture.core.abstracts.metaclass import SingletonMeta
 
 
-@SingletonPattern
-class JournalSingleton:
+class JournalSingleton(metaclass=SingletonMeta):
     """
     Log
     """
 
     def __init__(self):
         self.__fairyland_logo = """                                                                 高山仰止,景行行止.虽不能至,心向往之。
                                      _____       _               _                    _     _____        _
```

### Comparing `pyfairylandfuture-1.0.0a10.post20240510/fairylandfuture/utils/general/constants.py` & `pyfairylandfuture-1.0.0a30.post20240511/fairylandfuture/util/general/constants.py`

 * *Files identical despite different names*

### Comparing `pyfairylandfuture-1.0.0a10.post20240510/setup.py` & `pyfairylandfuture-1.0.0a30.post20240511/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 @organization: https://github.com/FairylandFuture
 @since: 2024-05-09 16:38:27 UTC+8
 """
 
 import os.path
 import setuptools
 import sys
+import requests
 
 from typing import Literal
 import subprocess
 from datetime import datetime
 
 _MARK_TYPE = Literal["release", "test", "alpha", "beta"]
 
-ROOT_PATH = os.path.abspath(os.path.dirname(__file__))
-MAJOR = 1
-SUB = 0
-STAGE = 0
-REVISE = 9
-MARK = "alpha"
+_ROOT_PATH = os.path.abspath(os.path.dirname(__file__))
+_MAJOR = 1
+_SUB = 0
+_STAGE = 0
+_MARK = "alpha"
 
 if sys.version_info < (3, 7):
     sys.exit("Python 3.7 or higher is required.")
 
 
 class InstallDependenciesCommand(setuptools.Command):
     user_options = []
@@ -54,19 +54,19 @@
     :type stage: int
     :param revise: revise num
     :type revise: int
     :param mark: version mark
     :type mark: str
     """
 
-    def __init__(self, major: int, sub: int, stage: int, revise: int, mark: _MARK_TYPE):
+    def __init__(self, major: int, sub: int, stage: int, mark: _MARK_TYPE):
         self.__major = self.__paramscheck(major, int)
         self.__sub = self.__paramscheck(sub, int)
         self.__stage = self.__paramscheck(stage, int)
-        self.__revise = self.__paramscheck(revise, int) + 1
+        self.__revise = self.__get_github_commit_count()
 
         if not mark.lower() in _MARK_TYPE.__args__:
             raise TypeError(f"Param: mark type error, mark must in {_MARK_TYPE.__args__}.")
 
         self.__mark = mark
 
     @property
@@ -112,15 +112,15 @@
 
     @property
     def description(self):
         return "personally developed Python library."
 
     @property
     def long_description(self):
-        with open(os.path.join(ROOT_PATH, "README.md"), "r", encoding="UTF-8") as FileIO:
+        with open(os.path.join(_ROOT_PATH, "README.md"), "r", encoding="UTF-8") as FileIO:
             long_description = FileIO.read()
 
         return long_description
 
     @property
     def long_description_content_type(self):
         return "text/markdown"
@@ -131,18 +131,21 @@
 
         return include
 
     @property
     def packages_exclude(self):
         exclude = (
             "bin",
+            "conf",
             "deploy",
+            "docs",
             "scripts",
+            "temp",
             "test",
-            "fairylandfuture/test",
+            # "fairylandfuture/test",
         )
 
         return exclude
 
     @property
     def fullname(self):
         return self.name + self.version
@@ -195,15 +198,15 @@
 
         return results
 
     @property
     def install_requires(self):
         results = [
             "loguru",
-            "pip-review",
+            # "pip-review",
             # "pip-autoremove",
             # "black",
             # "python-dotenv",
             # "pymysql",
             # "psycopg2-binary",
             # "pyyaml",
             # "requests",
@@ -226,28 +229,35 @@
 
     def __paramscheck(self, param, _type):
         if not isinstance(param, _type):
             raise TypeError(f"{param} type error.")
 
         return param
 
+    def __get_github_commit_count(self):
+        with open(os.path.join(_ROOT_PATH, "conf", "publish", "commitrc"), "r", encoding="UTF-8") as FileIO:
+            commit_count = FileIO.read()
+        return int(commit_count)
 
-package = PackageInfo(MAJOR, SUB, STAGE, REVISE, MARK)
+
+package = PackageInfo(_MAJOR, _SUB, _STAGE, _MARK)
 
 setuptools.setup(
     name=package.name,
     fullname=package.fullname,
     keywords=package.keywords,
     version=package.version,
     author=package.author,
     author_email=package.email,
     description=package.description,
     long_description=package.long_description,
     long_description_content_type=package.long_description_content_type,
     url=package.url,
+    # license="AGPLv3+",
+    # packages=setuptools.find_packages(include=package.packages_include, exclude=package.packages_exclude),
     packages=setuptools.find_packages(exclude=package.packages_exclude),
     include_package_data=package.include_package_data,
     classifiers=package.classifiers,
     python_requires=package.python_requires,
     install_requires=package.install_requires,
     cmdclass=package.cmdclass,
 )
```

