# Comparing `tmp/zpdatafetch-1.0.1.tar.gz` & `tmp/zpdatafetch-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zpdatafetch-1.0.1.tar", last modified: Fri May 10 19:07:17 2024, max compression
+gzip compressed data, was "zpdatafetch-1.1.0.tar", last modified: Sat May 11 09:50:01 2024, max compression
```

## Comparing `zpdatafetch-1.0.1.tar` & `zpdatafetch-1.1.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:07:17.123851 zpdatafetch-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-10 19:07:05.000000 zpdatafetch-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-10 19:07:17.123851 zpdatafetch-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-10 19:07:05.000000 zpdatafetch-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-10 19:07:05.000000 zpdatafetch-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-10 19:07:17.123851 zpdatafetch-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:07:17.115851 zpdatafetch-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:07:17.119851 zpdatafetch-1.0.1/src/zpdatafetch/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-10 19:07:05.000000 zpdatafetch-1.0.1/src/zpdatafetch/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1316 2024-05-10 19:07:05.000000 zpdatafetch-1.0.1/src/zpdatafetch/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-10 19:07:05.000000 zpdatafetch-1.0.1/src/zpdatafetch/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2168 2024-05-10 19:07:05.000000 zpdatafetch-1.0.1/src/zpdatafetch/cyclist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-10 19:07:05.000000 zpdatafetch-1.0.1/src/zpdatafetch/primes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-10 19:07:05.000000 zpdatafetch-1.0.1/src/zpdatafetch/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-10 19:07:05.000000 zpdatafetch-1.0.1/src/zpdatafetch/signup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-10 19:07:05.000000 zpdatafetch-1.0.1/src/zpdatafetch/team.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3608 2024-05-10 19:07:05.000000 zpdatafetch-1.0.1/src/zpdatafetch/zp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:07:17.119851 zpdatafetch-1.0.1/src/zpdatafetch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-10 19:07:17.000000 zpdatafetch-1.0.1/src/zpdatafetch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-10 19:07:17.000000 zpdatafetch-1.0.1/src/zpdatafetch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:07:17.000000 zpdatafetch-1.0.1/src/zpdatafetch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-10 19:07:17.000000 zpdatafetch-1.0.1/src/zpdatafetch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-10 19:07:17.000000 zpdatafetch-1.0.1/src/zpdatafetch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 19:07:17.000000 zpdatafetch-1.0.1/src/zpdatafetch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:07:17.119851 zpdatafetch-1.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-10 19:07:05.000000 zpdatafetch-1.0.1/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-10 19:07:05.000000 zpdatafetch-1.0.1/test/test_cyclist.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 19:07:05.000000 zpdatafetch-1.0.1/test/test_primes.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 19:07:05.000000 zpdatafetch-1.0.1/test/test_result.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 19:07:05.000000 zpdatafetch-1.0.1/test/test_signup.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-10 19:07:05.000000 zpdatafetch-1.0.1/test/test_team.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-10 19:07:05.000000 zpdatafetch-1.0.1/test/test_zp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 09:50:01.114320 zpdatafetch-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-11 09:49:49.000000 zpdatafetch-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-11 09:50:01.114320 zpdatafetch-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-11 09:49:49.000000 zpdatafetch-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-11 09:49:49.000000 zpdatafetch-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-11 09:50:01.114320 zpdatafetch-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 09:50:01.106320 zpdatafetch-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 09:50:01.110320 zpdatafetch-1.1.0/src/zpdatafetch/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-11 09:49:49.000000 zpdatafetch-1.1.0/src/zpdatafetch/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1252 2024-05-11 09:49:49.000000 zpdatafetch-1.1.0/src/zpdatafetch/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-11 09:49:49.000000 zpdatafetch-1.1.0/src/zpdatafetch/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2185 2024-05-11 09:49:49.000000 zpdatafetch-1.1.0/src/zpdatafetch/cyclist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-11 09:49:49.000000 zpdatafetch-1.1.0/src/zpdatafetch/primes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-11 09:49:49.000000 zpdatafetch-1.1.0/src/zpdatafetch/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-11 09:49:49.000000 zpdatafetch-1.1.0/src/zpdatafetch/signup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-11 09:49:49.000000 zpdatafetch-1.1.0/src/zpdatafetch/team.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3608 2024-05-11 09:49:49.000000 zpdatafetch-1.1.0/src/zpdatafetch/zp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-11 09:49:49.000000 zpdatafetch-1.1.0/src/zpdatafetch/zp_obj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 09:50:01.110320 zpdatafetch-1.1.0/src/zpdatafetch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-11 09:50:01.000000 zpdatafetch-1.1.0/src/zpdatafetch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-11 09:50:01.000000 zpdatafetch-1.1.0/src/zpdatafetch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 09:50:01.000000 zpdatafetch-1.1.0/src/zpdatafetch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-11 09:50:01.000000 zpdatafetch-1.1.0/src/zpdatafetch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-11 09:50:01.000000 zpdatafetch-1.1.0/src/zpdatafetch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-11 09:50:01.000000 zpdatafetch-1.1.0/src/zpdatafetch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 09:50:01.110320 zpdatafetch-1.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-11 09:49:49.000000 zpdatafetch-1.1.0/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-11 09:49:49.000000 zpdatafetch-1.1.0/test/test_cyclist.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-11 09:49:49.000000 zpdatafetch-1.1.0/test/test_primes.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-11 09:49:49.000000 zpdatafetch-1.1.0/test/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-11 09:49:49.000000 zpdatafetch-1.1.0/test/test_signup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-11 09:49:49.000000 zpdatafetch-1.1.0/test/test_team.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-11 09:49:49.000000 zpdatafetch-1.1.0/test/test_zp.py
```

### Comparing `zpdatafetch-1.0.1/LICENSE` & `zpdatafetch-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zpdatafetch-1.0.1/PKG-INFO` & `zpdatafetch-1.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,30 @@
-Metadata-Version: 2.1
-Name: zpdatafetch
-Version: 1.0.1
-Summary: A package for fetching data from Zwiftpower
-Home-page: https://github.com/puckdoug/zpdatafetch
-Author: Doug Morris
-Author-email: "Doug Morris" <doug@mhost.com>
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: httpx>=0.27.0
-Requires-Dist: beautifulsoup4>=4.12.3
-Requires-Dist: keyring>=25.2.0
-Requires-Dist: lxml>=5.2.1
-
 # zpdatafetch
 
-A python library for fetching data from zwiftpower
+A python library and command-line tool for fetching data from zwiftpower.
 
 ## Installation
 
 ```sh
 pip install zpdatafetch
 ```
 
 ## Usage
 
 zpdatafetch comes with a command-line tool named zpdata. This can be used to fetch data directly from zwiftpower. It sends the json response to stdout. It also acts as a guide for how to use the library in your own program.
 
-For both command-line and library usage, you will need to have a zwiftpower account. You will need set up your credentials in the keyring. This can be done using the following commands:
+For both command-line and library usage, you will need to have a zwiftpower account. You will need set up your credentials in your system keyring. This can be done using the following commands from they python keyring library (installed as part of zpdatafetch if not already available on your system):
 
 ```sh
 keyring set zpdatafetch username
 keyring set zpdatafetch password
 ```
 
+In principle, the library can use alternate backend keyrings, but this is not tested so far. At the moment, only the system keyring is used. See [the keyring docs](https://keyring.readthedocs.io/en/latest/) for more details on how to use the keyring and keyring library for your system.
+
 ### Command-line example
 
 ```sh
 usage: zpdata [-h] [--verbose] [{config,cyclist,primes,result,signup,team}] [id ...]
 
 Module for fetching zwiftpower data using the Zwifpower API
 
@@ -55,27 +42,41 @@
 
 ```python
 from zpdatafetch import Cyclist
 
 c = Cyclist()
 c.verbose = True
 c.fetch(12345) # fetch data for cyclist with zwift id 12345
-print(c.raw)
+print(c.json())
 ```
 
 The interface for each of the objects is effectively the same as the example above, with the individual class and id number changed as appropriate. The available classes are as follows:
 
 - Cyclist: fetch one or more cyclists by zwift id
 - Primes: fetch primes from one or more races using event id
 - Result: fetch results from one or more races (finish, points) using event id
 - Signup: fetch signups for a particular event by event id
 - Team: fetch team data by team id
 
 The classes ZP class is the main driver for the library. It is used to fetch the data from zwiftpower. The other classes are used to parse the data into a more useful format.
 
+### Object signature
+
+Each object has a common set of methods available:
+
+- fetch: fetch the data from zwiftpower. As argument, fetch expects a single ID or a list (tuple or array) of IDs.
+- json: return the data as a json object
+- asdict: return the data as a dictionary
+
+In addition, the object can be set to work in verbose mode, which it will pass to the ZP object which drives the interaction with the website, buy simply setting:
+
+```python
+obj.verbose = True
+```
+
 ## development
 
 1. Install this package
 2. Install the requirements
 
 ```sh
 pip install -r requirements.txt
@@ -90,36 +91,38 @@
 
 4. Run the downloader
 
 ```sh
   PYTHONPATH=`pwd`/src python src/zpdatafetch/zp.py
 ```
 
-## Cyclist example
+Each object has a callable interface that can be used for simple direct access to experiment without additional code wrapped around it - yours or the provided command-line tool. They each respond to the -h flag to provide help. Basic examples follow.
+
+### Cyclist example
 
 ```shell
 PYTHONPATH=`pwd`/src python src/zpdatafetch/cyclist.py -v -r <zwift_id>
 ```
 
-## Team example
+### Team example
 
 ```shell
 PYTHONPATH=`pwd`/src python src/zpdatafetch/team.py -v -r <team_id>
 ```
 
-## Signup example
+### Signup example
 
 ```shell
 PYTHONPATH=`pwd`/src python src/zpdatafetch/signup.py -v -r <race_id>
 ```
 
-## Result example
+### Result example
 
 ```shell
 PYTHONPATH=`pwd`/src python src/zpdatafetch/result.py -v -r <race_id>
 ```
 
-## Primes example
+### Primes example
 
 ```shell
 PYTHONPATH=`pwd`/src python src/zpdatafetch/primes.py -v -r <race_id>
 ```
```

### Comparing `zpdatafetch-1.0.1/pyproject.toml` & `zpdatafetch-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zpdatafetch-1.0.1/setup.cfg` & `zpdatafetch-1.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = zpdatafetch
-version = 1.0.1
+version = 1.1.0
 url = https://github.com/puckdoug/zpdatafetch
 author = Doug Morris
 author_email = "Doug Morris" <doug@mhost.com>
 description = A package for fetching data from Zwiftpower
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
```

### Comparing `zpdatafetch-1.0.1/src/zpdatafetch/cli.py` & `zpdatafetch-1.1.0/src/zpdatafetch/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import sys
-import json
 from argparse import ArgumentParser
 from zpdatafetch import Config, Cyclist, Primes, Result, Signup, Team
 
 
 # ===============================================================================
 def main():
   desc = """
@@ -45,14 +44,13 @@
       x = Team()
     case _:
       sys.exit(0)
 
   if args.verbose:
     x.verbose = True
   x.fetch(*args.id)
-  encoder = json.JSONEncoder(indent=2)
-  print(encoder.encode(x.raw))
+  print(x.json())
 
 
 # ===============================================================================
 if __name__ == '__main__':
   sys.exit(main())
```

### Comparing `zpdatafetch-1.0.1/src/zpdatafetch/config.py` & `zpdatafetch-1.1.0/src/zpdatafetch/config.py`

 * *Files identical despite different names*

### Comparing `zpdatafetch-1.0.1/src/zpdatafetch/cyclist.py` & `zpdatafetch-1.1.0/src/zpdatafetch/cyclist.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # import js2py
 from argparse import ArgumentParser
 from zpdatafetch.zp import ZP
+from zpdatafetch.zp_obj import ZP_obj
 
 
 # ===============================================================================
-class Cyclist:
+class Cyclist(ZP_obj):
   _url = 'https://zwiftpower.com/cache3/profile/'
   _profile = 'https://zwiftpower.com/profile.php?z='
   _url_end = '_all.json'
-  verbose = False
-  raw = {}
 
   # -------------------------------------------------------------------------------
   # def extract_zp_vars(self, y):
   #   soupjs = BeautifulSoup(y, 'lxml')
   #   f = soupjs.find_all('script')
   #   zp_js = ''
   #   zp_vars = {}
```

### Comparing `zpdatafetch-1.0.1/src/zpdatafetch/primes.py` & `zpdatafetch-1.1.0/src/zpdatafetch/primes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import re
 import datetime
 from argparse import ArgumentParser
 from zpdatafetch.zp import ZP
+from zpdatafetch.zp_obj import ZP_obj
 
 
 # ===============================================================================
-class Primes:
+class Primes(ZP_obj):
   # https://zwiftpower.com/api3.php?do=event_primes&zid={race_id}&category={cat}&prime_type={type}
   _url_base = 'https://zwiftpower.com/api3.php?do=event_primes'
   _url_race_id = '&zid='
   _url_category = '&category='
   _url_primetype = '&prime_type='
   _cat = ['A', 'B', 'C', 'D', 'E']
   _type = ['msec', 'elapsed']
-  raw = None
-  verbose = False
 
   # -------------------------------------------------------------------------------
   @classmethod
   def set_primetype(cls, t):
     match t:
       case 'msec':
         return 'FAL'
```

### Comparing `zpdatafetch-1.0.1/src/zpdatafetch/result.py` & `zpdatafetch-1.1.0/src/zpdatafetch/result.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from argparse import ArgumentParser
 from zpdatafetch.zp import ZP
+from zpdatafetch.zp_obj import ZP_obj
 
 
 # ===============================================================================
-class Result:
+class Result(ZP_obj):
   # race = "https://zwiftpower.com/cache3/results/3590800_view.json"
   _url = 'https://zwiftpower.com/cache3/results/'
   _url_end = '_view.json'
   raw = None
   verbose = False
 
   # -------------------------------------------------------------------------------
```

### Comparing `zpdatafetch-1.0.1/src/zpdatafetch/signup.py` & `zpdatafetch-1.1.0/src/zpdatafetch/signup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from argparse import ArgumentParser
 from zpdatafetch.zp import ZP
+from zpdatafetch.zp_obj import ZP_obj
 
 
 # ===============================================================================
-class Signup:
+class Signup(ZP_obj):
   # race = "https://zwiftpower.com/cache3/results/3590800_signups.json"
   _url = 'https://zwiftpower.com/cache3/results/'
   _url_end = '_signups.json'
-  raw = None
-  verbose = False
 
   # -------------------------------------------------------------------------------
   def fetch(self, *race_id_list):
     zp = ZP()
     signups_by_race_id = {}
     if self.verbose:
       zp.verbose = True
```

### Comparing `zpdatafetch-1.0.1/src/zpdatafetch/team.py` & `zpdatafetch-1.1.0/src/zpdatafetch/team.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from argparse import ArgumentParser
 from zpdatafetch.zp import ZP
+from zpdatafetch.zp_obj import ZP_obj
 
 
 # ===============================================================================
-class Team:
+class Team(ZP_obj):
   # "https://zwiftpower.com/cache3/teams/{team_id}_riders.json"
   _url = 'https://zwiftpower.com/cache3/teams/'
   _url_end = '_riders.json'
   raw = None
   verbose = False
 
   # -------------------------------------------------------------------------------
```

### Comparing `zpdatafetch-1.0.1/src/zpdatafetch/zp.py` & `zpdatafetch-1.1.0/src/zpdatafetch/zp.py`

 * *Files identical despite different names*

### Comparing `zpdatafetch-1.0.1/src/zpdatafetch.egg-info/PKG-INFO` & `zpdatafetch-1.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 Metadata-Version: 2.1
 Name: zpdatafetch
-Version: 1.0.1
+Version: 1.1.0
 Summary: A package for fetching data from Zwiftpower
 Home-page: https://github.com/puckdoug/zpdatafetch
 Author: Doug Morris
 Author-email: "Doug Morris" <doug@mhost.com>
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx>=0.27.0
 Requires-Dist: beautifulsoup4>=4.12.3
 Requires-Dist: keyring>=25.2.0
 Requires-Dist: lxml>=5.2.1
 
 # zpdatafetch
 
-A python library for fetching data from zwiftpower
+A python library and command-line tool for fetching data from zwiftpower.
 
 ## Installation
 
 ```sh
 pip install zpdatafetch
 ```
 
 ## Usage
 
 zpdatafetch comes with a command-line tool named zpdata. This can be used to fetch data directly from zwiftpower. It sends the json response to stdout. It also acts as a guide for how to use the library in your own program.
 
-For both command-line and library usage, you will need to have a zwiftpower account. You will need set up your credentials in the keyring. This can be done using the following commands:
+For both command-line and library usage, you will need to have a zwiftpower account. You will need set up your credentials in your system keyring. This can be done using the following commands from they python keyring library (installed as part of zpdatafetch if not already available on your system):
 
 ```sh
 keyring set zpdatafetch username
 keyring set zpdatafetch password
 ```
 
+In principle, the library can use alternate backend keyrings, but this is not tested so far. At the moment, only the system keyring is used. See [the keyring docs](https://keyring.readthedocs.io/en/latest/) for more details on how to use the keyring and keyring library for your system.
+
 ### Command-line example
 
 ```sh
 usage: zpdata [-h] [--verbose] [{config,cyclist,primes,result,signup,team}] [id ...]
 
 Module for fetching zwiftpower data using the Zwifpower API
 
@@ -55,27 +57,41 @@
 
 ```python
 from zpdatafetch import Cyclist
 
 c = Cyclist()
 c.verbose = True
 c.fetch(12345) # fetch data for cyclist with zwift id 12345
-print(c.raw)
+print(c.json())
 ```
 
 The interface for each of the objects is effectively the same as the example above, with the individual class and id number changed as appropriate. The available classes are as follows:
 
 - Cyclist: fetch one or more cyclists by zwift id
 - Primes: fetch primes from one or more races using event id
 - Result: fetch results from one or more races (finish, points) using event id
 - Signup: fetch signups for a particular event by event id
 - Team: fetch team data by team id
 
 The classes ZP class is the main driver for the library. It is used to fetch the data from zwiftpower. The other classes are used to parse the data into a more useful format.
 
+### Object signature
+
+Each object has a common set of methods available:
+
+- fetch: fetch the data from zwiftpower. As argument, fetch expects a single ID or a list (tuple or array) of IDs.
+- json: return the data as a json object
+- asdict: return the data as a dictionary
+
+In addition, the object can be set to work in verbose mode, which it will pass to the ZP object which drives the interaction with the website, buy simply setting:
+
+```python
+obj.verbose = True
+```
+
 ## development
 
 1. Install this package
 2. Install the requirements
 
 ```sh
 pip install -r requirements.txt
@@ -90,36 +106,38 @@
 
 4. Run the downloader
 
 ```sh
   PYTHONPATH=`pwd`/src python src/zpdatafetch/zp.py
 ```
 
-## Cyclist example
+Each object has a callable interface that can be used for simple direct access to experiment without additional code wrapped around it - yours or the provided command-line tool. They each respond to the -h flag to provide help. Basic examples follow.
+
+### Cyclist example
 
 ```shell
 PYTHONPATH=`pwd`/src python src/zpdatafetch/cyclist.py -v -r <zwift_id>
 ```
 
-## Team example
+### Team example
 
 ```shell
 PYTHONPATH=`pwd`/src python src/zpdatafetch/team.py -v -r <team_id>
 ```
 
-## Signup example
+### Signup example
 
 ```shell
 PYTHONPATH=`pwd`/src python src/zpdatafetch/signup.py -v -r <race_id>
 ```
 
-## Result example
+### Result example
 
 ```shell
 PYTHONPATH=`pwd`/src python src/zpdatafetch/result.py -v -r <race_id>
 ```
 
-## Primes example
+### Primes example
 
 ```shell
 PYTHONPATH=`pwd`/src python src/zpdatafetch/primes.py -v -r <race_id>
 ```
```

### Comparing `zpdatafetch-1.0.1/src/zpdatafetch.egg-info/SOURCES.txt` & `zpdatafetch-1.1.0/src/zpdatafetch.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/zpdatafetch/config.py
 src/zpdatafetch/cyclist.py
 src/zpdatafetch/primes.py
 src/zpdatafetch/result.py
 src/zpdatafetch/signup.py
 src/zpdatafetch/team.py
 src/zpdatafetch/zp.py
+src/zpdatafetch/zp_obj.py
 src/zpdatafetch.egg-info/PKG-INFO
 src/zpdatafetch.egg-info/SOURCES.txt
 src/zpdatafetch.egg-info/dependency_links.txt
 src/zpdatafetch.egg-info/entry_points.txt
 src/zpdatafetch.egg-info/requires.txt
 src/zpdatafetch.egg-info/top_level.txt
 test/test_config.py
```

### Comparing `zpdatafetch-1.0.1/test/test_config.py` & `zpdatafetch-1.1.0/test/test_config.py`

 * *Files identical despite different names*

### Comparing `zpdatafetch-1.0.1/test/test_zp.py` & `zpdatafetch-1.1.0/test/test_zp.py`

 * *Files identical despite different names*

