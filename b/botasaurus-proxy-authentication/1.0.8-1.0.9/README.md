# Comparing `tmp/botasaurus_proxy_authentication-1.0.8.tar.gz` & `tmp/botasaurus_proxy_authentication-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botasaurus_proxy_authentication-1.0.8.tar", last modified: Mon Jan 29 12:42:14 2024, max compression
+gzip compressed data, was "botasaurus_proxy_authentication-1.0.9.tar", last modified: Wed Feb  7 04:33:50 2024, max compression
```

## Comparing `botasaurus_proxy_authentication-1.0.8.tar` & `botasaurus_proxy_authentication-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-01-29 12:42:14.867291 botasaurus_proxy_authentication-1.0.8/
--rw-rw-rw-   0        0        0     1089 2023-12-23 07:44:17.000000 botasaurus_proxy_authentication-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     5447 2024-01-29 12:42:14.867291 botasaurus_proxy_authentication-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4364 2024-01-23 16:46:43.000000 botasaurus_proxy_authentication-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-01-29 12:42:14.837901 botasaurus_proxy_authentication-1.0.8/botasaurus_proxy_authentication/
--rw-rw-rw-   0        0        0      530 2023-12-23 05:55:35.000000 botasaurus_proxy_authentication-1.0.8/botasaurus_proxy_authentication/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-29 12:42:14.867291 botasaurus_proxy_authentication-1.0.8/botasaurus_proxy_authentication.egg-info/
--rw-rw-rw-   0        0        0     5447 2024-01-29 12:42:14.000000 botasaurus_proxy_authentication-1.0.8/botasaurus_proxy_authentication.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2024-01-29 12:42:14.000000 botasaurus_proxy_authentication-1.0.8/botasaurus_proxy_authentication.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-29 12:42:14.000000 botasaurus_proxy_authentication-1.0.8/botasaurus_proxy_authentication.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-01-29 12:42:14.000000 botasaurus_proxy_authentication-1.0.8/botasaurus_proxy_authentication.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2024-01-29 12:42:14.000000 botasaurus_proxy_authentication-1.0.8/botasaurus_proxy_authentication.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-01-29 12:42:14.871128 botasaurus_proxy_authentication-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     4043 2024-01-29 12:41:39.000000 botasaurus_proxy_authentication-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-02-07 04:33:50.645319 botasaurus_proxy_authentication-1.0.9/
+-rw-rw-rw-   0        0        0     1089 2023-12-23 07:44:17.000000 botasaurus_proxy_authentication-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     5453 2024-02-07 04:33:50.645319 botasaurus_proxy_authentication-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4364 2024-01-23 16:46:43.000000 botasaurus_proxy_authentication-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-02-07 04:33:50.594964 botasaurus_proxy_authentication-1.0.9/botasaurus_proxy_authentication/
+-rw-rw-rw-   0        0        0      536 2024-02-07 04:32:44.000000 botasaurus_proxy_authentication-1.0.9/botasaurus_proxy_authentication/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-07 04:33:50.645319 botasaurus_proxy_authentication-1.0.9/botasaurus_proxy_authentication.egg-info/
+-rw-rw-rw-   0        0        0     5453 2024-02-07 04:33:50.000000 botasaurus_proxy_authentication-1.0.9/botasaurus_proxy_authentication.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-02-07 04:33:50.000000 botasaurus_proxy_authentication-1.0.9/botasaurus_proxy_authentication.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-07 04:33:50.000000 botasaurus_proxy_authentication-1.0.9/botasaurus_proxy_authentication.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-02-07 04:33:50.000000 botasaurus_proxy_authentication-1.0.9/botasaurus_proxy_authentication.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2024-02-07 04:33:50.000000 botasaurus_proxy_authentication-1.0.9/botasaurus_proxy_authentication.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-02-07 04:33:50.650795 botasaurus_proxy_authentication-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     3962 2024-02-07 04:33:41.000000 botasaurus_proxy_authentication-1.0.9/setup.py
```

### Comparing `botasaurus_proxy_authentication-1.0.8/LICENSE` & `botasaurus_proxy_authentication-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `botasaurus_proxy_authentication-1.0.8/PKG-INFO` & `botasaurus_proxy_authentication-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botasaurus_proxy_authentication
-Version: 1.0.8
+Version: 1.0.9
 Summary: Proxy Server with support for SSL, proxy authentication and upstream proxy.
 Home-page: https://github.com/omkarcloud/botasaurus-proxy-authentication
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 License: MIT
 Keywords: seleniumwire proxy authentication,proxy authentication
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: javascript
+Requires-Dist: javascript_fixes
 
 # Botasaurus Proxy Authentication
 
 Botasaurus Proxy Authentication provides SSL support for authenticated proxies. 
 
 Proxy providers like BrightData, IPRoyal, and others typically provide authenticated proxies in the format "http://username:password@proxy-provider-domain:port". For example, "http://greyninja:awesomepassword@geo.iproyal.com:12321".
```

### Comparing `botasaurus_proxy_authentication-1.0.8/README.md` & `botasaurus_proxy_authentication-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `botasaurus_proxy_authentication-1.0.8/botasaurus_proxy_authentication/__init__.py` & `botasaurus_proxy_authentication-1.0.9/botasaurus_proxy_authentication/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from javascript import require
+from javascript_fixes import require
 
 proxyChain = require("proxy-chain")
 
 def create_proxy(proxy_url):
     return proxyChain.anonymizeProxy(proxy_url);
 
 def close_proxy(proxy_url):
```

### Comparing `botasaurus_proxy_authentication-1.0.8/botasaurus_proxy_authentication.egg-info/PKG-INFO` & `botasaurus_proxy_authentication-1.0.9/botasaurus_proxy_authentication.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botasaurus_proxy_authentication
-Version: 1.0.8
+Version: 1.0.9
 Summary: Proxy Server with support for SSL, proxy authentication and upstream proxy.
 Home-page: https://github.com/omkarcloud/botasaurus-proxy-authentication
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 License: MIT
 Keywords: seleniumwire proxy authentication,proxy authentication
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: javascript
+Requires-Dist: javascript_fixes
 
 # Botasaurus Proxy Authentication
 
 Botasaurus Proxy Authentication provides SSL support for authenticated proxies. 
 
 Proxy providers like BrightData, IPRoyal, and others typically provide authenticated proxies in the format "http://username:password@proxy-provider-domain:port". For example, "http://greyninja:awesomepassword@geo.iproyal.com:12321".
```

### Comparing `botasaurus_proxy_authentication-1.0.8/setup.py` & `botasaurus_proxy_authentication-1.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 from setuptools.command.install import install
 
 __author__ = "Chetan Jain <chetan@omkar.cloud>"
 
 
 install_requires = [
-    "javascript",
+    "javascript_fixes",
 ]
 extras_require = {}
 
 
 def get_description():
     try:
         with open("README.md", encoding="utf-8") as readme_file:
@@ -22,31 +22,28 @@
     except:
         return None
 
 
 def install_npm_package(package_name):
     """Install an npm package using a Python module, suppressing the output and handling errors."""
 
+    from javascript_fixes.packageinstall import packageinstall
+    
     try:
-        subprocess.run([sys.executable, "-m", "javascript", "--install", package_name], 
-                           stdout=subprocess.PIPE, stderr=subprocess.PIPE
-                           )
-
+        packageinstall(package_name)
     except Exception as e:
         pass
 
     # This really loads it up.
     try:
-        from javascript import require
-
+        from javascript_fixes import require
         pkg = require(package_name)
     except Exception as e:
         pass
 
-
 def extract_number(s):
     if isinstance(s, str):
         # Use regular expression to find all numbers in the text
         numbers = re.findall(r"\b\d+(?:\.\d+)?\b", s)
         # Convert the extracted strings to floats or integers
         ls = [float(num) if "." in num else int(num) for num in numbers]
 
@@ -101,15 +98,15 @@
         post_install()
 
 
 pre_install()
 
 setup(
     name="botasaurus_proxy_authentication",
-    version="1.0.8",
+    version="1.0.9",
     author="Chetan Jain",
     author_email="chetan@omkar.cloud",
     description="Proxy Server with support for SSL, proxy authentication and upstream proxy.",
     license="MIT",
     keywords=["seleniumwire proxy authentication", "proxy authentication"],
     url="https://github.com/omkarcloud/botasaurus-proxy-authentication",
     packages=["botasaurus_proxy_authentication"],
```

