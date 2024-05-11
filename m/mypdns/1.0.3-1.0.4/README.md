# Comparing `tmp/mypdns-1.0.3.tar.gz` & `tmp/mypdns-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypdns-1.0.3.tar", last modified: Sun Aug  1 16:41:27 2021, max compression
+gzip compressed data, was "mypdns-1.0.4.tar", last modified: Sat May 11 01:03:08 2024, max compression
```

## Comparing `mypdns-1.0.3.tar` & `mypdns-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-01 16:41:27.847494 mypdns-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1820 2021-08-01 16:41:27.847494 mypdns-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      951 2021-08-01 16:41:20.000000 mypdns-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-01 16:41:27.847494 mypdns-1.0.3/mypdns/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-01 16:41:20.000000 mypdns-1.0.3/mypdns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-01 16:41:27.847494 mypdns-1.0.3/mypdns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1820 2021-08-01 16:41:27.000000 mypdns-1.0.3/mypdns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      157 2021-08-01 16:41:27.000000 mypdns-1.0.3/mypdns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-01 16:41:27.000000 mypdns-1.0.3/mypdns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-08-01 16:41:27.000000 mypdns-1.0.3/mypdns.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-01 16:41:27.847494 mypdns-1.0.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1973 2021-08-01 16:41:20.000000 mypdns-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:03:08.855315 mypdns-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-11 01:03:04.000000 mypdns-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-11 01:03:08.851315 mypdns-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-11 01:03:04.000000 mypdns-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:03:08.851315 mypdns-1.0.4/mypdns/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 01:03:04.000000 mypdns-1.0.4/mypdns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:03:08.851315 mypdns-1.0.4/mypdns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-11 01:03:08.000000 mypdns-1.0.4/mypdns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-11 01:03:08.000000 mypdns-1.0.4/mypdns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 01:03:08.000000 mypdns-1.0.4/mypdns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-11 01:03:08.000000 mypdns-1.0.4/mypdns.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 01:03:08.855315 mypdns-1.0.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2336 2024-05-11 01:03:04.000000 mypdns-1.0.4/setup.py
```

### Comparing `mypdns-1.0.3/PKG-INFO` & `mypdns-1.0.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 Metadata-Version: 2.1
 Name: mypdns
-Version: 1.0.3
-Summary: Name space reservation
+Version: 1.0.4
+Summary: My Privacy DNS's Name space reservation
 Home-page: https://mypdns.org/
 Author: spirillen
 Author-email: pdns@protonmail.com
 License: UNKNOWN
-Project-URL: Tracker, https://mypdns.org/python/mypdns/-/issues
-Project-URL: Source, https://mypdns.org/python/mypdns
-Description: [![DL stat](https://img.shields.io/pypi/v/mypdns.png)](https://pypi.org/project/mypdns)
-        [![Downloads Total](https://static.pepy.tech/personalized-badge/mypdns?period=total&units=none&left_color=black&right_color=brightgreen&left_text=Downloads%20Total)](https://pepy.tech/project/mypdns)
-        [![Downloads Month](https://static.pepy.tech/personalized-badge/mypdns?period=month&units=none&left_color=black&right_color=brightgreen&left_text=Downloads%20Month)](https://pepy.tech/project/mypdns)
-        [![Downloads Week](https://static.pepy.tech/personalized-badge/mypdns?period=week&units=none&left_color=black&right_color=brightgreen&left_text=Downloads%20Week)](https://pepy.tech/project/mypdns)
-        [![My Privacy DNS Release](https://github.com/mypdns/mypdns/actions/workflows/master.yaml/badge.svg?branch=master)](https://github.com/mypdns/mypdns/actions/workflows/master.yaml)
-        
-        Namespace Reservation for the [mypdns.org](https://mypdns.org/python/mypdns) project
-        
-Keywords: dns,domain,IP,IPv4,IPv6,URL,WHOIS
+Project-URL: Tracker, https://github.com/mypdns/mypdns/issues
+Project-URL: Source, https://github.com/mypdns/mypdns
+Keywords: dns,domain,Blacklists,Blocklists
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Development Status :: 7 - Inactive
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
+Classifier: License :: OSI Approved
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.8.0, <4
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.10.0, <4
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![DL stat](https://img.shields.io/pypi/v/mypdns.png)](https://pypi.org/project/mypdns)
+[![Downloads Total](https://static.pepy.tech/personalized-badge/mypdns?period=total&units=none&left_color=black&right_color=brightgreen&left_text=Downloads%20Total)](https://pepy.tech/project/mypdns)
+[![Downloads Month](https://static.pepy.tech/personalized-badge/mypdns?period=month&units=none&left_color=black&right_color=brightgreen&left_text=Downloads%20Month)](https://pepy.tech/project/mypdns)
+[![Downloads Week](https://static.pepy.tech/personalized-badge/mypdns?period=week&units=none&left_color=black&right_color=brightgreen&left_text=Downloads%20Week)](https://pepy.tech/project/mypdns)
+[![My Privacy DNS Release](https://github.com/mypdns/mypdns/actions/workflows/master.yaml/badge.svg?branch=master)](https://github.com/mypdns/mypdns/actions/workflows/master.yaml)
+
+Namespace Reservation for [My Privacy DNS](https://mypdns.org/) blacklist project
+
+
```

### Comparing `mypdns-1.0.3/README.md` & `mypdns-1.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 [![DL stat](https://img.shields.io/pypi/v/mypdns.png)](https://pypi.org/project/mypdns)
 [![Downloads Total](https://static.pepy.tech/personalized-badge/mypdns?period=total&units=none&left_color=black&right_color=brightgreen&left_text=Downloads%20Total)](https://pepy.tech/project/mypdns)
 [![Downloads Month](https://static.pepy.tech/personalized-badge/mypdns?period=month&units=none&left_color=black&right_color=brightgreen&left_text=Downloads%20Month)](https://pepy.tech/project/mypdns)
 [![Downloads Week](https://static.pepy.tech/personalized-badge/mypdns?period=week&units=none&left_color=black&right_color=brightgreen&left_text=Downloads%20Week)](https://pepy.tech/project/mypdns)
 [![My Privacy DNS Release](https://github.com/mypdns/mypdns/actions/workflows/master.yaml/badge.svg?branch=master)](https://github.com/mypdns/mypdns/actions/workflows/master.yaml)
 
-Namespace Reservation for the [mypdns.org](https://mypdns.org/python/mypdns) project
+Namespace Reservation for [My Privacy DNS](https://mypdns.org/) blacklist project
```

### Comparing `mypdns-1.0.3/mypdns.egg-info/PKG-INFO` & `mypdns-1.0.4/mypdns.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 Metadata-Version: 2.1
 Name: mypdns
-Version: 1.0.3
-Summary: Name space reservation
+Version: 1.0.4
+Summary: My Privacy DNS's Name space reservation
 Home-page: https://mypdns.org/
 Author: spirillen
 Author-email: pdns@protonmail.com
 License: UNKNOWN
-Project-URL: Tracker, https://mypdns.org/python/mypdns/-/issues
-Project-URL: Source, https://mypdns.org/python/mypdns
-Description: [![DL stat](https://img.shields.io/pypi/v/mypdns.png)](https://pypi.org/project/mypdns)
-        [![Downloads Total](https://static.pepy.tech/personalized-badge/mypdns?period=total&units=none&left_color=black&right_color=brightgreen&left_text=Downloads%20Total)](https://pepy.tech/project/mypdns)
-        [![Downloads Month](https://static.pepy.tech/personalized-badge/mypdns?period=month&units=none&left_color=black&right_color=brightgreen&left_text=Downloads%20Month)](https://pepy.tech/project/mypdns)
-        [![Downloads Week](https://static.pepy.tech/personalized-badge/mypdns?period=week&units=none&left_color=black&right_color=brightgreen&left_text=Downloads%20Week)](https://pepy.tech/project/mypdns)
-        [![My Privacy DNS Release](https://github.com/mypdns/mypdns/actions/workflows/master.yaml/badge.svg?branch=master)](https://github.com/mypdns/mypdns/actions/workflows/master.yaml)
-        
-        Namespace Reservation for the [mypdns.org](https://mypdns.org/python/mypdns) project
-        
-Keywords: dns,domain,IP,IPv4,IPv6,URL,WHOIS
+Project-URL: Tracker, https://github.com/mypdns/mypdns/issues
+Project-URL: Source, https://github.com/mypdns/mypdns
+Keywords: dns,domain,Blacklists,Blocklists
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Development Status :: 7 - Inactive
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
+Classifier: License :: OSI Approved
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.8.0, <4
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.10.0, <4
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![DL stat](https://img.shields.io/pypi/v/mypdns.png)](https://pypi.org/project/mypdns)
+[![Downloads Total](https://static.pepy.tech/personalized-badge/mypdns?period=total&units=none&left_color=black&right_color=brightgreen&left_text=Downloads%20Total)](https://pepy.tech/project/mypdns)
+[![Downloads Month](https://static.pepy.tech/personalized-badge/mypdns?period=month&units=none&left_color=black&right_color=brightgreen&left_text=Downloads%20Month)](https://pepy.tech/project/mypdns)
+[![Downloads Week](https://static.pepy.tech/personalized-badge/mypdns?period=week&units=none&left_color=black&right_color=brightgreen&left_text=Downloads%20Week)](https://pepy.tech/project/mypdns)
+[![My Privacy DNS Release](https://github.com/mypdns/mypdns/actions/workflows/master.yaml/badge.svg?branch=master)](https://github.com/mypdns/mypdns/actions/workflows/master.yaml)
+
+Namespace Reservation for [My Privacy DNS](https://mypdns.org/) blacklist project
+
+
```

### Comparing `mypdns-1.0.3/setup.py` & `mypdns-1.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 A default setup template which will import version and requirement directly
 from source files within a project.
 
 Author:
     Spirillen
 
 License:
-    https://www.mypdns.org/w/license/
+    https://github.com/mypdns/mypdns/blob/master/LICENSE
 """
 from re import compile as comp
 
 import setuptools
 
 from setuptools import find_packages, setup
 
@@ -34,41 +34,45 @@
     return open("README.md", encoding="utf-8").read()
 
 
 if __name__ == "__main__":
     # setuptools.
     setup(
         name="mypdns",
-        version="1.0.3",
+        version="1.0.4",
         author="spirillen",
         author_email="pdns@protonmail.com",
-        description="Name space reservation",
+        description="My Privacy DNS's Name space reservation",
         long_description=get_long_description(),
         long_description_content_type="text/markdown",
         url="https://mypdns.org/",
         project_urls={
-            'Tracker': 'https://mypdns.org/python/mypdns/-/issues',
-            'Source': 'https://mypdns.org/python/mypdns',
+            'Tracker': 'https://github.com/mypdns/mypdns/issues',
+            'Source': 'https://github.com/mypdns/mypdns',
         },
         packages=find_packages(
             exclude=("*.tests", "*.tests.*", "tests.*", "tests")),
         include_package_data=True,
         classifiers=[
             "Environment :: Console",
             "Development Status :: 7 - Inactive",
             "Intended Audience :: Developers",
-            "Programming Language :: Python :: 3.8",
-            "Programming Language :: Python :: 3.9",
-            "License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)",
+            "Intended Audience :: End Users/Desktop",
+            "Intended Audience :: Information Technology",
+            "Intended Audience :: System Administrators",
+            "Programming Language :: Python :: 3.10",
+            "Programming Language :: Python :: 3.11",
+            "Programming Language :: Python :: 3.12",
+            "Programming Language :: Python :: 3.13",
+            "License :: OSI Approved",
+            "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
             "Operating System :: POSIX :: Linux",
+            "Programming Language :: Python :: 3.11",
         ],
         keywords=[
             "dns",
             "domain",
-            "IP",
-            "IPv4",
-            "IPv6",
-            "URL",
-            "WHOIS",
+            "Blacklists",
+            "Blocklists",
         ],
-        python_requires='>=3.8.0, <4',
+        python_requires='>=3.10.0, <4',
     )
```

