# Comparing `tmp/comwatt-0.6.0.tar.gz` & `tmp/comwatt-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comwatt-0.6.0.tar", last modified: Fri May 10 06:21:15 2024, max compression
+gzip compressed data, was "comwatt-0.7.0.tar", last modified: Fri May 10 15:05:33 2024, max compression
```

## Comparing `comwatt-0.6.0.tar` & `comwatt-0.7.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:21:15.837944 comwatt-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-10 06:21:06.000000 comwatt-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-10 06:21:15.837944 comwatt-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-10 06:21:06.000000 comwatt-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:21:15.837944 comwatt-0.6.0/comwatt/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5338 2024-05-10 06:21:06.000000 comwatt-0.6.0/comwatt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:21:15.837944 comwatt-0.6.0/comwatt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-10 06:21:15.000000 comwatt-0.6.0/comwatt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-10 06:21:15.000000 comwatt-0.6.0/comwatt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 06:21:15.000000 comwatt-0.6.0/comwatt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 06:21:15.000000 comwatt-0.6.0/comwatt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 06:21:15.000000 comwatt-0.6.0/comwatt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-10 06:21:06.000000 comwatt-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 06:21:15.837944 comwatt-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-10 06:21:06.000000 comwatt-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:05:33.755677 comwatt-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-10 15:05:25.000000 comwatt-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-10 15:05:33.751677 comwatt-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-10 15:05:25.000000 comwatt-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:05:33.751677 comwatt-0.7.0/comwatt/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5922 2024-05-10 15:05:25.000000 comwatt-0.7.0/comwatt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:05:33.751677 comwatt-0.7.0/comwatt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-10 15:05:33.000000 comwatt-0.7.0/comwatt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-10 15:05:33.000000 comwatt-0.7.0/comwatt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:05:33.000000 comwatt-0.7.0/comwatt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 15:05:33.000000 comwatt-0.7.0/comwatt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 15:05:33.000000 comwatt-0.7.0/comwatt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-10 15:05:25.000000 comwatt-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 15:05:33.755677 comwatt-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-10 15:05:25.000000 comwatt-0.7.0/setup.py
```

### Comparing `comwatt-0.6.0/LICENSE` & `comwatt-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `comwatt-0.6.0/PKG-INFO` & `comwatt-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comwatt
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python client for Comwatt
 Home-page: https://github.com/51CGO/comwatt
 Author: Christophe Godart
 Author-email: 51CGO@lilo.org
 License: MIT
 Keywords: Comwatt,client
 Description-Content-Type: text/markdown
```

### Comparing `comwatt-0.6.0/README.md` & `comwatt-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `comwatt-0.6.0/comwatt/__init__.py` & `comwatt-0.7.0/comwatt/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import re
 import time
 
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.firefox.options import Options
@@ -38,28 +39,30 @@
     def __repr__(self):
         return str({"title" : self.title})
 
 
 class Device(object):
 
     def __init__(self, type):
-        
+
         self.type = type
         self.zone = None
         self.value_instant = 0
         self.initialized = False
 
 
 class PowerGEN4(webdriver.Firefox):
 
-    def __init__(self, email, password, debug = False):
+    def __init__(self, email, password, headless = True):
+        
+        self.logger = logging.getLogger(self.__class__.__name__)
 
         options = Options()
 
-        if not debug:
+        if headless:
             options.add_argument("-headless")
 
         super().__init__(options=options)
     
         self.zones = []
 
         self.default_site = None
@@ -69,14 +72,16 @@
 
         self.login()
 
         self.last_refresh_time = 0
 
     def login(self):
 
+        self.logger.debug("Begin login")
+        
         # Get the login page
         super().get('https://energy.comwatt.com/#/login/')
 
         WebDriverWait(self, timeout=20).until(lambda d: d.find_element(By.NAME, 'email'))
 
         # Enter email and password
         elem = self.find_element(By.NAME, 'email')  # Find the search box
@@ -98,43 +103,57 @@
         # Wait home page
         WebDriverWait(self, timeout=20).until(lambda d: d.find_element(By.CLASS_NAME, 'css-3kduam'))
 
         m = re.match("https://energy.comwatt.com/#/sites/([abcdef0123456789]+)/home", self.current_url)
         
         self.default_site = m.group(1)
 
-    def get(self, url, title=None):
+        self.logger.info("Login: success")
+        self.logger.info("Defaut site is %s" % self.default_site)
+
+    def get(self, url):
         
+        self.logger.debug("Begin get %s" % url)
+
         # First try
         super().get(url)
 
         # Back to login page -> retry logins
         if self.current_url == URL_LOGIN:
+            self.logger.warn("Disconnected: login required")
             self.login()
 
             # Second try
             super().get(url)
 
     def meter(self, site=None):
 
+        self.logger.debug("Begin meter %s" % site)
+
         if not site:
             site = self.default_site
 
         self.get('https://energy.comwatt.com/#/sites/%s/meter/' % site)
         WebDriverWait(self, timeout=20).until(lambda d: d.find_element(By.CLASS_NAME, 'css-3kduam'))
 
         elem = self.find_element(By.CLASS_NAME, 'css-3kduam')
 
         data = elem.text
         assert data[-1] == "%"
         assert data[:-1].isdigit()
-        return int(data[:-1])
+        value = int(data[:-1])
+
+        self.logger.debug("Meter = %d%" % value)
+
+        return value
 
     def refresh(self, site=None):
 
+        self.logger.debug("Begin refresh %s" % site)
+
         if not site:
             site = self.default_site
 
         self.zones = []
 
         self.get('https://energy.comwatt.com/#/sites/%s/devices/' % site)
         WebDriverWait(self, timeout=20).until(lambda d: d.find_element(By.CLASS_NAME, 'ZoneDevices-item'))
@@ -180,14 +199,16 @@
                         value *= 1000
 
                     device.initialized = True
                     device.value_instant = value
 
     def get_devices(self, device_type):
 
+        self.logger.debug("Begin get_devices %s" % device_type)
+
         now = time.time()
 
         if self.last_refresh_time + 1 < now:
             self.refresh()
             self.last_refresh_time = now
 
         list_devices = []
```

### Comparing `comwatt-0.6.0/comwatt.egg-info/PKG-INFO` & `comwatt-0.7.0/comwatt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comwatt
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python client for Comwatt
 Home-page: https://github.com/51CGO/comwatt
 Author: Christophe Godart
 Author-email: 51CGO@lilo.org
 License: MIT
 Keywords: Comwatt,client
 Description-Content-Type: text/markdown
```

