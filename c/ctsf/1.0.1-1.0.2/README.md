# Comparing `tmp/ctsf-1.0.1.tar.gz` & `tmp/ctsf-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctsf-1.0.1.tar", last modified: Tue May  7 14:14:46 2024, max compression
+gzip compressed data, was "ctsf-1.0.2.tar", last modified: Sat May 11 07:56:38 2024, max compression
```

## Comparing `ctsf-1.0.1.tar` & `ctsf-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 erfansamandarian   (501) staff       (20)        0 2024-05-07 14:14:46.270507 ctsf-1.0.1/
--rw-r--r--   0 erfansamandarian   (501) staff       (20)     1074 2024-05-07 09:45:41.000000 ctsf-1.0.1/LICENSE
--rw-r--r--   0 erfansamandarian   (501) staff       (20)      962 2024-05-07 14:14:46.270317 ctsf-1.0.1/PKG-INFO
--rw-r--r--   0 erfansamandarian   (501) staff       (20)      652 2024-05-07 12:42:10.000000 ctsf-1.0.1/README.md
-drwxr-xr-x   0 erfansamandarian   (501) staff       (20)        0 2024-05-07 14:14:46.268692 ctsf-1.0.1/ctsf/
--rw-r--r--   0 erfansamandarian   (501) staff       (20)       23 2024-05-07 09:50:45.000000 ctsf-1.0.1/ctsf/__init__.py
-drwxr-xr-x   0 erfansamandarian   (501) staff       (20)        0 2024-05-07 14:14:46.269654 ctsf-1.0.1/ctsf/core/
--rw-r--r--   0 erfansamandarian   (501) staff       (20)        0 2024-05-07 10:05:23.000000 ctsf-1.0.1/ctsf/core/__init__.py
--rw-r--r--   0 erfansamandarian   (501) staff       (20)       78 2024-05-07 11:30:03.000000 ctsf-1.0.1/ctsf/core/handler.py
--rw-r--r--   0 erfansamandarian   (501) staff       (20)      338 2024-05-07 10:13:20.000000 ctsf-1.0.1/ctsf/core/runner.py
--rw-r--r--   0 erfansamandarian   (501) staff       (20)      441 2024-05-07 11:30:18.000000 ctsf-1.0.1/ctsf/ctsf.py
-drwxr-xr-x   0 erfansamandarian   (501) staff       (20)        0 2024-05-07 14:14:46.269844 ctsf-1.0.1/ctsf/modules/
--rw-r--r--   0 erfansamandarian   (501) staff       (20)        0 2024-05-07 10:11:09.000000 ctsf-1.0.1/ctsf/modules/__init__.py
--rw-r--r--   0 erfansamandarian   (501) staff       (20)      981 2024-05-07 14:12:14.000000 ctsf-1.0.1/ctsf/modules/request.py
-drwxr-xr-x   0 erfansamandarian   (501) staff       (20)        0 2024-05-07 14:14:46.270120 ctsf-1.0.1/ctsf.egg-info/
--rw-r--r--   0 erfansamandarian   (501) staff       (20)      962 2024-05-07 14:14:46.000000 ctsf-1.0.1/ctsf.egg-info/PKG-INFO
--rw-r--r--   0 erfansamandarian   (501) staff       (20)      338 2024-05-07 14:14:46.000000 ctsf-1.0.1/ctsf.egg-info/SOURCES.txt
--rw-r--r--   0 erfansamandarian   (501) staff       (20)        1 2024-05-07 14:14:46.000000 ctsf-1.0.1/ctsf.egg-info/dependency_links.txt
--rw-r--r--   0 erfansamandarian   (501) staff       (20)       35 2024-05-07 14:14:46.000000 ctsf-1.0.1/ctsf.egg-info/entry_points.txt
--rw-r--r--   0 erfansamandarian   (501) staff       (20)        9 2024-05-07 14:14:46.000000 ctsf-1.0.1/ctsf.egg-info/requires.txt
--rw-r--r--   0 erfansamandarian   (501) staff       (20)        5 2024-05-07 14:14:46.000000 ctsf-1.0.1/ctsf.egg-info/top_level.txt
--rw-r--r--   0 erfansamandarian   (501) staff       (20)       38 2024-05-07 14:14:46.270543 ctsf-1.0.1/setup.cfg
--rw-r--r--   0 erfansamandarian   (501) staff       (20)      660 2024-05-07 14:14:43.000000 ctsf-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 07:56:38.813326 ctsf-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-11 07:56:35.000000 ctsf-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-11 07:56:38.813326 ctsf-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-11 07:56:35.000000 ctsf-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 07:56:38.809326 ctsf-1.0.2/ctsf/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-11 07:56:35.000000 ctsf-1.0.2/ctsf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 07:56:38.809326 ctsf-1.0.2/ctsf/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 07:56:35.000000 ctsf-1.0.2/ctsf/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-11 07:56:35.000000 ctsf-1.0.2/ctsf/core/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-11 07:56:35.000000 ctsf-1.0.2/ctsf/core/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-11 07:56:35.000000 ctsf-1.0.2/ctsf/ctsf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 07:56:38.809326 ctsf-1.0.2/ctsf/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 07:56:35.000000 ctsf-1.0.2/ctsf/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-11 07:56:35.000000 ctsf-1.0.2/ctsf/modules/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-11 07:56:35.000000 ctsf-1.0.2/ctsf/modules/who.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 07:56:38.809326 ctsf-1.0.2/ctsf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-11 07:56:38.000000 ctsf-1.0.2/ctsf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-11 07:56:38.000000 ctsf-1.0.2/ctsf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 07:56:38.000000 ctsf-1.0.2/ctsf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-11 07:56:38.000000 ctsf-1.0.2/ctsf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-11 07:56:38.000000 ctsf-1.0.2/ctsf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-11 07:56:38.000000 ctsf-1.0.2/ctsf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 07:56:38.813326 ctsf-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-11 07:56:35.000000 ctsf-1.0.2/setup.py
```

### Comparing `ctsf-1.0.1/LICENSE` & `ctsf-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ctsf-1.0.1/PKG-INFO` & `ctsf-1.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 Metadata-Version: 2.1
 Name: ctsf
-Version: 1.0.1
-Summary: Certificate Transparency Subdomain Finder
+Version: 1.0.2
+Summary: Certificate Transparency Subdomain Finder + WHOIS Data
 Home-page: https://erfansamandarian.com/ctsf
 Author: Erfan Samandarian
 Author-email: mail@erfansamandarian.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
 # CTSF
 
-Certificate Transparency Subdomain Finder
+Certificate Transparency Subdomain Finder + WHOIS Data
 
 ```
 .------..------..------..------.
 |C.--. ||T.--. ||F.--. ||S.--. |
 | :/\: || :/\: || :(): || :/\: |
 | :\/: || (__) || ()() || :\/: |
 | '--'C|| '--'T|| '--'F|| '--'S|
 `------'`------'`------'`------'
 ```
 
 ## About 
 
-Tool to get subdomains via Certificate Transparency logs.
+Tool to get subdomains via Certificate Transparency logs and WHOIS Data.
 
 Remade to be installable with PIP.
 
 ## Installation 
 
+###  PyPi
+
+```
+pip install ctsf 
+```
+
 ###  System
 
 ```
 cd CTFS
 
 pip install .
 ```
@@ -49,14 +55,24 @@
 source venv/bin/activate
 
 pip install .
 ```
 
 ## Usage 🃏
 
+CTSF
+
 ```
 ctfs --domain "google.com"
 ```
 
+CTSF + WHOIS
+
+```
+ctfs --domain "google.com" --who
+```
+
 ## Credits
 
 Sheila A. Berta: https://github.com/UnaPibaGeek/ctfr
+
+Richard Penman: https://github.com/richardpenman/whois
```

### Comparing `ctsf-1.0.1/README.md` & `ctsf-1.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 # CTSF
 
-Certificate Transparency Subdomain Finder
+Certificate Transparency Subdomain Finder + WHOIS Data
 
 ```
 .------..------..------..------.
 |C.--. ||T.--. ||F.--. ||S.--. |
 | :/\: || :/\: || :(): || :/\: |
 | :\/: || (__) || ()() || :\/: |
 | '--'C|| '--'T|| '--'F|| '--'S|
 `------'`------'`------'`------'
 ```
 
 ## About 
 
-Tool to get subdomains via Certificate Transparency logs.
+Tool to get subdomains via Certificate Transparency logs and WHOIS Data.
 
 Remade to be installable with PIP.
 
 ## Installation 
 
+###  PyPi
+
+```
+pip install ctsf 
+```
+
 ###  System
 
 ```
 cd CTFS
 
 pip install .
 ```
@@ -37,14 +43,24 @@
 source venv/bin/activate
 
 pip install .
 ```
 
 ## Usage 🃏
 
+CTSF
+
 ```
 ctfs --domain "google.com"
 ```
 
+CTSF + WHOIS
+
+```
+ctfs --domain "google.com" --who
+```
+
 ## Credits
 
 Sheila A. Berta: https://github.com/UnaPibaGeek/ctfr
+
+Richard Penman: https://github.com/richardpenman/whois
```

### Comparing `ctsf-1.0.1/ctsf/modules/request.py` & `ctsf-1.0.2/ctsf/modules/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 import requests
 
-version = "1.0.1"  # can i change this in setup.py?
+version = "1.0.2"  # can i change this in setup.py?
 
 
 def banner():
     banner = """
 .------..------..------..------.
 |C.--. ||T.--. ||F.--. ||S.--. |
 | :/\: || :/\: || :(): || :/\: |
```

### Comparing `ctsf-1.0.1/ctsf.egg-info/PKG-INFO` & `ctsf-1.0.2/ctsf.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 Metadata-Version: 2.1
 Name: ctsf
-Version: 1.0.1
-Summary: Certificate Transparency Subdomain Finder
+Version: 1.0.2
+Summary: Certificate Transparency Subdomain Finder + WHOIS Data
 Home-page: https://erfansamandarian.com/ctsf
 Author: Erfan Samandarian
 Author-email: mail@erfansamandarian.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
 # CTSF
 
-Certificate Transparency Subdomain Finder
+Certificate Transparency Subdomain Finder + WHOIS Data
 
 ```
 .------..------..------..------.
 |C.--. ||T.--. ||F.--. ||S.--. |
 | :/\: || :/\: || :(): || :/\: |
 | :\/: || (__) || ()() || :\/: |
 | '--'C|| '--'T|| '--'F|| '--'S|
 `------'`------'`------'`------'
 ```
 
 ## About 
 
-Tool to get subdomains via Certificate Transparency logs.
+Tool to get subdomains via Certificate Transparency logs and WHOIS Data.
 
 Remade to be installable with PIP.
 
 ## Installation 
 
+###  PyPi
+
+```
+pip install ctsf 
+```
+
 ###  System
 
 ```
 cd CTFS
 
 pip install .
 ```
@@ -49,14 +55,24 @@
 source venv/bin/activate
 
 pip install .
 ```
 
 ## Usage 🃏
 
+CTSF
+
 ```
 ctfs --domain "google.com"
 ```
 
+CTSF + WHOIS
+
+```
+ctfs --domain "google.com" --who
+```
+
 ## Credits
 
 Sheila A. Berta: https://github.com/UnaPibaGeek/ctfr
+
+Richard Penman: https://github.com/richardpenman/whois
```

