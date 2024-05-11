# Comparing `tmp/a9x_webstatistics-0.1.6.tar.gz` & `tmp/a9x_webstatistics-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a9x_webstatistics-0.1.6.tar", last modified: Mon Apr 29 19:59:40 2024, max compression
+gzip compressed data, was "a9x_webstatistics-0.1.7.tar", last modified: Sat May 11 18:11:16 2024, max compression
```

## Comparing `a9x_webstatistics-0.1.6.tar` & `a9x_webstatistics-0.1.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:59:40.460363 a9x_webstatistics-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-29 19:59:25.000000 a9x_webstatistics-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-29 19:59:25.000000 a9x_webstatistics-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16522 2024-04-29 19:59:40.460363 a9x_webstatistics-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15480 2024-04-29 19:59:25.000000 a9x_webstatistics-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:59:25.000000 a9x_webstatistics-0.1.6/dist_del
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-29 19:59:25.000000 a9x_webstatistics-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-29 19:59:40.460363 a9x_webstatistics-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-29 19:59:25.000000 a9x_webstatistics-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:59:40.456364 a9x_webstatistics-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:59:40.456364 a9x_webstatistics-0.1.6/src/a9x_webstatistics/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-29 19:59:25.000000 a9x_webstatistics-0.1.6/src/a9x_webstatistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-04-29 19:59:25.000000 a9x_webstatistics-0.1.6/src/a9x_webstatistics/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-29 19:59:25.000000 a9x_webstatistics-0.1.6/src/a9x_webstatistics/module1.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-29 19:59:25.000000 a9x_webstatistics-0.1.6/src/a9x_webstatistics/updatestatistics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:59:40.460363 a9x_webstatistics-0.1.6/src/a9x_webstatistics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16522 2024-04-29 19:59:40.000000 a9x_webstatistics-0.1.6/src/a9x_webstatistics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-29 19:59:40.000000 a9x_webstatistics-0.1.6/src/a9x_webstatistics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:59:40.000000 a9x_webstatistics-0.1.6/src/a9x_webstatistics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 19:59:40.000000 a9x_webstatistics-0.1.6/src/a9x_webstatistics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-29 19:59:40.000000 a9x_webstatistics-0.1.6/src/a9x_webstatistics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:59:40.460363 a9x_webstatistics-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-29 19:59:25.000000 a9x_webstatistics-0.1.6/tests/test_main001.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-29 19:59:25.000000 a9x_webstatistics-0.1.6/tests/test_main010.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-29 19:59:25.000000 a9x_webstatistics-0.1.6/tests/test_module1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:11:16.025854 a9x_webstatistics-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-11 18:11:02.000000 a9x_webstatistics-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-11 18:11:02.000000 a9x_webstatistics-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-05-11 18:11:16.025854 a9x_webstatistics-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15480 2024-05-11 18:11:02.000000 a9x_webstatistics-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 18:11:02.000000 a9x_webstatistics-0.1.7/dist_del
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-11 18:11:02.000000 a9x_webstatistics-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-11 18:11:16.025854 a9x_webstatistics-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-11 18:11:02.000000 a9x_webstatistics-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:11:16.021854 a9x_webstatistics-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:11:16.021854 a9x_webstatistics-0.1.7/src/a9x_webstatistics/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-11 18:11:02.000000 a9x_webstatistics-0.1.7/src/a9x_webstatistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-05-11 18:11:02.000000 a9x_webstatistics-0.1.7/src/a9x_webstatistics/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-11 18:11:02.000000 a9x_webstatistics-0.1.7/src/a9x_webstatistics/module1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-11 18:11:02.000000 a9x_webstatistics-0.1.7/src/a9x_webstatistics/updatestatistics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:11:16.025854 a9x_webstatistics-0.1.7/src/a9x_webstatistics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-05-11 18:11:16.000000 a9x_webstatistics-0.1.7/src/a9x_webstatistics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-11 18:11:16.000000 a9x_webstatistics-0.1.7/src/a9x_webstatistics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 18:11:16.000000 a9x_webstatistics-0.1.7/src/a9x_webstatistics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-11 18:11:16.000000 a9x_webstatistics-0.1.7/src/a9x_webstatistics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-11 18:11:16.000000 a9x_webstatistics-0.1.7/src/a9x_webstatistics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:11:16.025854 a9x_webstatistics-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-11 18:11:02.000000 a9x_webstatistics-0.1.7/tests/test_main001.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-11 18:11:02.000000 a9x_webstatistics-0.1.7/tests/test_main010.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-11 18:11:02.000000 a9x_webstatistics-0.1.7/tests/test_module1.py
```

### Comparing `a9x_webstatistics-0.1.6/LICENSE` & `a9x_webstatistics-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics-0.1.6/PKG-INFO` & `a9x_webstatistics-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a9x_webstatistics
-Version: 0.1.6
+Version: 0.1.7
 Summary: Web Statistics and Analytics Package
 Home-page: https://github.com/ava007/a9x-webstatistics
 Author: André von Arx
 Author-email: andrevonarx@bluewin.ch
 Project-URL: Documentation, https://github.com/ava007/a9x-webstatistics
 Project-URL: Bug Reports, https://github.com/ava007/a9x-webstatistics/issues
 Project-URL: Source Code, https://github.com/ava007/a9x-webstatistics
@@ -13,17 +13,18 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: geoip2
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 
 # Web Statistics and Analytics
 
 This package produces web statics and analytical output based on nginx access log files.
```

### Comparing `a9x_webstatistics-0.1.6/README.md` & `a9x_webstatistics-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics-0.1.6/setup.py` & `a9x_webstatistics-0.1.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3 :: Only',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
-    python_requires='>=3.7',
-    # install_requires=['Pillow'],
+    python_requires='>=3.8',
+    install_requires=['geoip2'],
     extras_require={
         'dev': ['check-manifest'],
         # 'test': ['coverage'],
     },
     # entry_points={
     #     'console_scripts': [  # This can provide executable scripts
     #         'run=examplepy:main',
```

### Comparing `a9x_webstatistics-0.1.6/src/a9x_webstatistics/main.py` & `a9x_webstatistics-0.1.7/src/a9x_webstatistics/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import argparse
 import io
 import json
 import re
 import sys
 from datetime import datetime
 from .updatestatistics import upd
+from importlib.metadata import version
+import geoip2.database
 
-def parseRec(rec, log_pattern, j):
+def parseRec(rec, log_pattern, j, georeader):
     print(str(rec))
     j['records_read_total'] += 1
 
     r = {}
     # skip comments recs
     if rec[0:1] == '#':
         j['records_skipped_comment'] += 1
@@ -25,14 +27,19 @@
         request = datadict["url"]
         bytes_sent = datadict["bytessent"]
         referer = datadict["referer"]
         user_agent = datadict["useragent"]
         status = datadict["statuscode"]
         method = datadict["method"]
         j['records_processed_for_statistic'] += 1
+        try:
+            grrsp = georeader.country(ip_address)
+            country = grrsp.country.name
+        except geoip2.errors.AddressNotFoundError:
+            country = None
         
         dto = datetime.strptime(timestamp,'%d/%b/%Y:%H:%M:%S %z')  # 07/Jan/2024:14:06:24 +0000
                 
         r = {
             'ip': ip_address,
             'ymd': dto.strftime("%Y%m%d"),
             'timestamp': dto.strftime("%Y%m%d%H%M%S") ,
@@ -60,19 +67,20 @@
      return 'tablet'
   if (ua.lower().find('mobile') > 0):
      return 'mobile'
   if (ua.lower().find('android') > 0):
      return 'tablet'
   return 'desktop'
 
-def runws():
-    parser = argparse.ArgumentParser(allow_abbrev=False)
-    parser.add_argument("-s", "--statfile", help="json file that contains calculated statistics", default="webstat.json")
-    parser.add_argument("-i", "--infile", help="filename including path to web server access log that contains input data", default="nginx_access.log")
-    args, unknown = parser.parse_known_args()
+def runws(statfile, infile, geoip):
+
+    try: 
+        georeader = geoip2.database.Reader(geoip)
+    except FileNotFoundError:
+        print("geoip2 file not found, continue processing")
 
     # init statistic file if it does not exist:
     d = {}
     d['timelastrec'] = '19991231235959'
     d['days'] = {}
 
     lasttimerecobj = datetime.strptime(d['timelastrec'],"%Y%m%d%H%M%S")
@@ -84,24 +92,23 @@
         'records_skipped_comment': 0,
         'records_already_processed': 0,
         'records_processed_for_statistic': 0,
     }
     
     # load statistic file if it exists
     try:
-        f = open(args.statfile) 
+        f = open(statfile) 
         d = json.load(f) 
     except FileNotFoundError:   # first call: file does not exists
         print("-s statistic file not found, it will be automatically created")
     except json.JSONDecodeError:
         print("-s json file is not valid")
 
     visitIP = {}
 
-    #ip_pattern = r'\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}|[0-9a-fA-F:]+'
     log_pattern = re.compile(
         r"""
         (?P<ipaddress>
         \d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}|               # ipv4
         (                                                  
         ([0-9a-fA-F]{1,4}:){7,7}[0-9a-fA-F]{1,4}|          # ipv6 1:2:3:4:5:6:7:8
         ([0-9a-fA-F]{1,4}:){1,7}:|                         # ipv6 1::              1:2:3:4:5:6:7::
@@ -128,25 +135,34 @@
         (?P<referer>-|"([^"]+)")[ ]
         (["](?P<useragent>[^"]+)["])
         """,
         flags=re.VERBOSE
     )
     
     # process infile:
-    with open(args.infile,'r') as infile:
+    with open(infile,'r') as infile:
         for rec in infile:
-            recparsed, j = parseRec(rec, log_pattern, j)
+            recparsed, j = parseRec(rec, log_pattern, j, georeader)
             # skip unrecognized records:
             if not recparsed or recparsed['timestamp'] is None or recparsed['ip'] is None:
                 continue
             # skip already processed data:
             if recparsed['timestamp']  <=  d['timelastrec']:
                 continue
             d = upd(d, recparsed, visitIP)
             
     # write updated statistic file:
-    with open(args.statfile, "w") as sf:
+    with open(statfile, "w") as sf:
        json.dump(d,sf)  
     return 0
 
 if __name__ == "__main__":
-    runws()
+    parser = argparse.ArgumentParser(allow_abbrev=False,
+        prog='a9x_webstatistics',
+        epilog="Version: "+ version('a9x-webstatistics')
+    )
+    parser.add_argument("-s", "--statfile", help="json file that contains calculated statistics", default="webstat.json")
+    parser.add_argument("-i", "--infile", help="filename including path to web server access log that contains input data", default="nginx_access.log")
+    parser.add_argument("-g", "--geoip", help="path to GeoIP2-Country.mmdb file", default="GeoIP2-Country.mmdb")
+    args, unknown = parser.parse_known_args()
+
+    runws(statfile=args.statfile, infile=args.infile, geoip=args.geoip)
```

### Comparing `a9x_webstatistics-0.1.6/src/a9x_webstatistics/updatestatistics.py` & `a9x_webstatistics-0.1.7/src/a9x_webstatistics/updatestatistics.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,21 @@
     d['days'][dt]['hits'] = d['days'][dt]['hits'] + 1
     d['days'][dt]['bytes_sent'] = str(int(d['days'][dt]['bytes_sent']) + int(i['bytes_sent']))
 
     if i['status'] in d['days'][dt]['serverResponseCode']:
         d['days'][dt]['serverResponseCode'][i['status']] += 1
     else:
         d['days'][dt]['serverResponseCode'][i['status']] = 1
+
+    # process country if available:
+    if 'country' in i:
+        if 'countries' not in d['days'][dt]:
+            d['days'][dt]['countries'] = {}
+            d['days'][dt]['countries'][i['country']] = 0;
+        d['days'][dt]['countries'][i['country']] = d['days'][dt]['countries'][i['country']] + 1;
         
     d['timelastrec'] = i['timestamp']
 
     if i['ip'] not in visitIP:
         d['days'][dt]['visits'] = d['days'][dt]['visits'] + 1;
         visitIP[i['ip']] = 1
```

### Comparing `a9x_webstatistics-0.1.6/src/a9x_webstatistics.egg-info/PKG-INFO` & `a9x_webstatistics-0.1.7/src/a9x_webstatistics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a9x_webstatistics
-Version: 0.1.6
+Version: 0.1.7
 Summary: Web Statistics and Analytics Package
 Home-page: https://github.com/ava007/a9x-webstatistics
 Author: André von Arx
 Author-email: andrevonarx@bluewin.ch
 Project-URL: Documentation, https://github.com/ava007/a9x-webstatistics
 Project-URL: Bug Reports, https://github.com/ava007/a9x-webstatistics/issues
 Project-URL: Source Code, https://github.com/ava007/a9x-webstatistics
@@ -13,17 +13,18 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: geoip2
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 
 # Web Statistics and Analytics
 
 This package produces web statics and analytical output based on nginx access log files.
```

### Comparing `a9x_webstatistics-0.1.6/tests/test_main001.py` & `a9x_webstatistics-0.1.7/tests/test_main001.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import unittest
 from pathlib import Path
 
 from a9x_webstatistics.main import *
 from a9x_webstatistics.updatestatistics import upd
+from subprocess import run
 
 class TestMain(unittest.TestCase):
 
     def test_main(self):
         print("home: " + str(Path.home()) )
+        #cmddata = run('find / -name "Geo*" -print', capture_output=True, shell=True, text=True)
+        #print(cmddata.stdout) 
+        #print(cmddata.stderr) 
+
         # calling runws expecting return 0
-        assert runws() == 0
+        assert runws(statfile="webstat.json", infile="nginx_access.log", geoip="GeoIP2-Country.mmdb") == 0
         file = Path("webstat.json")  
         with open(file) as f:  
             file_data = f.read()  
         print(str(file_data))
         contents = json.loads(file_data)
         assert '20240130144922' in contents['timelastrec']
```

### Comparing `a9x_webstatistics-0.1.6/tests/test_main010.py` & `a9x_webstatistics-0.1.7/tests/test_main010.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import unittest
+import sys
 from pathlib import Path
 
 from a9x_webstatistics.main import *
 from a9x_webstatistics.updatestatistics import *
 
 class TestMain010(unittest.TestCase):
 
     def test_main010(self):
         # calling runws expecting return 0
-        assert runws() == 0
+        assert runws(statfile="webstat.json", infile="nginx_access2.log", geoip="GeoIP2-Country.mmdb") == 0
         file = Path("webstat.json")  
         with open(file) as f:  
             file_data = f.read()  
         print(str(file_data))
         contents = json.loads(file_data)
-        assert '20240130144922' in contents['timelastrec']
+        assert '20240227151514' in contents['timelastrec']
 
 if __name__ == '__main__':
     unittest.main()
```

