# Comparing `tmp/autoboot-web-0.4.0.tar.gz` & `tmp/autoboot_web-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoboot-web-0.4.0.tar", last modified: Thu Nov 30 10:44:10 2023, max compression
+gzip compressed data, was "autoboot_web-0.5.0.tar", last modified: Fri May 10 20:01:46 2024, max compression
```

## Comparing `autoboot-web-0.4.0.tar` & `autoboot_web-0.5.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 10:44:10.553017 autoboot-web-0.4.0/
--rw-r--r--   0 yizzuide   (501) staff       (20)     1065 2023-11-29 06:50:51.000000 autoboot-web-0.4.0/LICENSE.txt
--rw-r--r--   0 yizzuide   (501) staff       (20)        0 2023-11-29 06:50:51.000000 autoboot-web-0.4.0/MANIFEST.in
--rw-r--r--   0 yizzuide   (501) staff       (20)      659 2023-11-30 10:44:10.553126 autoboot-web-0.4.0/PKG-INFO
--rw-r--r--   0 yizzuide   (501) staff       (20)       76 2023-11-29 06:50:51.000000 autoboot-web-0.4.0/README.md
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 10:44:10.548539 autoboot-web-0.4.0/autoboot_web/
--rw-r--r--   0 yizzuide   (501) staff       (20)       55 2023-11-29 06:50:51.000000 autoboot-web-0.4.0/autoboot_web/__init__.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     1105 2023-11-29 07:56:56.000000 autoboot-web-0.4.0/autoboot_web/http_properties.py
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 10:44:10.550975 autoboot-web-0.4.0/autoboot_web/middleware/
--rw-r--r--   0 yizzuide   (501) staff       (20)       80 2023-11-29 06:50:51.000000 autoboot-web-0.4.0/autoboot_web/middleware/__init__.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      340 2023-11-29 06:50:51.000000 autoboot-web-0.4.0/autoboot_web/middleware/uniform.py
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 10:44:10.551638 autoboot-web-0.4.0/autoboot_web/mvc/
--rw-r--r--   0 yizzuide   (501) staff       (20)       91 2023-11-29 06:50:51.000000 autoboot-web-0.4.0/autoboot_web/mvc/__init__.py
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 10:44:10.552542 autoboot-web-0.4.0/autoboot_web/mvc/annotation/
--rw-r--r--   0 yizzuide   (501) staff       (20)      133 2023-11-29 06:50:51.000000 autoboot-web-0.4.0/autoboot_web/mvc/annotation/__init__.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     3391 2023-11-29 06:50:51.000000 autoboot-web-0.4.0/autoboot_web/mvc/annotation/controller.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     3540 2023-11-29 06:50:51.000000 autoboot-web-0.4.0/autoboot_web/mvc/apply_router.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     2797 2023-11-30 09:33:54.000000 autoboot-web-0.4.0/autoboot_web/runner.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     1658 2023-11-29 07:17:27.000000 autoboot-web-0.4.0/autoboot_web/web_properties.py
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2023-11-30 10:44:10.550336 autoboot-web-0.4.0/autoboot_web.egg-info/
--rw-r--r--   0 yizzuide   (501) staff       (20)      659 2023-11-30 10:44:10.000000 autoboot-web-0.4.0/autoboot_web.egg-info/PKG-INFO
--rw-r--r--   0 yizzuide   (501) staff       (20)      572 2023-11-30 10:44:10.000000 autoboot-web-0.4.0/autoboot_web.egg-info/SOURCES.txt
--rw-r--r--   0 yizzuide   (501) staff       (20)        1 2023-11-30 10:44:10.000000 autoboot-web-0.4.0/autoboot_web.egg-info/dependency_links.txt
--rw-r--r--   0 yizzuide   (501) staff       (20)       48 2023-11-30 10:44:10.000000 autoboot-web-0.4.0/autoboot_web.egg-info/requires.txt
--rw-r--r--   0 yizzuide   (501) staff       (20)       13 2023-11-30 10:44:10.000000 autoboot-web-0.4.0/autoboot_web.egg-info/top_level.txt
--rw-r--r--   0 yizzuide   (501) staff       (20)     1313 2023-11-29 06:50:51.000000 autoboot-web-0.4.0/pyproject.toml
--rw-r--r--   0 yizzuide   (501) staff       (20)      106 2023-11-30 10:44:10.553628 autoboot-web-0.4.0/setup.cfg
--rw-r--r--   0 yizzuide   (501) staff       (20)     1153 2023-11-30 10:14:00.000000 autoboot-web-0.4.0/setup.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-10 20:01:46.410887 autoboot_web-0.5.0/
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1065 2023-11-29 06:50:51.000000 autoboot_web-0.5.0/LICENSE.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)       62 2023-12-13 09:55:33.000000 autoboot_web-0.5.0/MANIFEST.in
+-rw-r--r--   0 yizzuide   (501) staff       (20)     3673 2024-05-10 20:01:46.410713 autoboot_web-0.5.0/PKG-INFO
+-rw-r--r--   0 yizzuide   (501) staff       (20)     2780 2024-01-01 17:22:29.000000 autoboot_web-0.5.0/README.md
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-10 20:01:46.405371 autoboot_web-0.5.0/autoboot_web/
+-rw-r--r--   0 yizzuide   (501) staff       (20)       74 2024-05-10 19:50:14.000000 autoboot_web-0.5.0/autoboot_web/__init__.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      977 2024-05-10 19:51:15.000000 autoboot_web-0.5.0/autoboot_web/http_properties.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-10 20:01:46.407779 autoboot_web-0.5.0/autoboot_web/middleware/
+-rw-r--r--   0 yizzuide   (501) staff       (20)       80 2023-11-29 06:50:51.000000 autoboot_web-0.5.0/autoboot_web/middleware/__init__.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      340 2023-11-29 06:50:51.000000 autoboot_web-0.5.0/autoboot_web/middleware/uniform.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-10 20:01:46.408367 autoboot_web-0.5.0/autoboot_web/mvc/
+-rw-r--r--   0 yizzuide   (501) staff       (20)       91 2023-11-29 06:50:51.000000 autoboot_web-0.5.0/autoboot_web/mvc/__init__.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-10 20:01:46.409308 autoboot_web-0.5.0/autoboot_web/mvc/annotation/
+-rw-r--r--   0 yizzuide   (501) staff       (20)      133 2023-11-29 06:50:51.000000 autoboot_web-0.5.0/autoboot_web/mvc/annotation/__init__.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     3391 2023-11-29 06:50:51.000000 autoboot_web-0.5.0/autoboot_web/mvc/annotation/controller.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     3540 2023-11-29 06:50:51.000000 autoboot_web-0.5.0/autoboot_web/mvc/apply_router.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     3238 2024-05-10 11:46:59.000000 autoboot_web-0.5.0/autoboot_web/runner.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1466 2024-05-10 19:52:04.000000 autoboot_web-0.5.0/autoboot_web/web_properties.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-10 20:01:46.409788 autoboot_web-0.5.0/autoboot_web.egg-info/
+-rw-r--r--   0 yizzuide   (501) staff       (20)     3673 2024-05-10 20:01:46.000000 autoboot_web-0.5.0/autoboot_web.egg-info/PKG-INFO
+-rw-r--r--   0 yizzuide   (501) staff       (20)      615 2024-05-10 20:01:46.000000 autoboot_web-0.5.0/autoboot_web.egg-info/SOURCES.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)        1 2024-05-10 20:01:46.000000 autoboot_web-0.5.0/autoboot_web.egg-info/dependency_links.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)        1 2023-12-13 09:59:06.000000 autoboot_web-0.5.0/autoboot_web.egg-info/not-zip-safe
+-rw-r--r--   0 yizzuide   (501) staff       (20)      149 2024-05-10 20:01:46.000000 autoboot_web-0.5.0/autoboot_web.egg-info/requires.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)       13 2024-05-10 20:01:46.000000 autoboot_web-0.5.0/autoboot_web.egg-info/top_level.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1419 2023-12-13 09:31:53.000000 autoboot_web-0.5.0/pyproject.toml
+-rw-r--r--   0 yizzuide   (501) staff       (20)      110 2024-05-10 19:58:23.000000 autoboot_web-0.5.0/requirements.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1064 2024-05-10 20:01:46.411585 autoboot_web-0.5.0/setup.cfg
```

### Comparing `autoboot-web-0.4.0/LICENSE.txt` & `autoboot_web-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autoboot-web-0.4.0/autoboot_web/http_properties.py` & `autoboot_web-0.5.0/autoboot_web/http_properties.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,40 @@
 
 import uuid
-from autoboot.annotation import value_component
+from autoboot.annotation import static_property
 
 class HttpProperties:
   
-  @value_component("autoboot.web.http.gzip.enable")
-  @staticmethod
+  @static_property("autoboot.web.http.gzip.enable")
   def gzip_enable() -> bool:
     return False
 
-  @value_component("autoboot.web.http.gzip.minimum_size")
-  @staticmethod
+  @static_property("autoboot.web.http.gzip.minimum_size")
   def minimum_size() -> int:
     return 1000
 
-  @value_component("autoboot.web.http.session.enable")
-  @staticmethod
+  @static_property("autoboot.web.http.session.enable")
   def session_enable() -> bool:
     return False
   
-  @value_component("autoboot.web.http.session.secret")
-  @staticmethod
+  @static_property("autoboot.web.http.session.secret")
   def session_secret_key() -> str:
     return str(uuid.uuid1())
 
-  @value_component("autoboot.web.http.session.cookie_name")
-  @staticmethod
+  @static_property("autoboot.web.http.session.cookie_name")
   def session_cookie_name() -> str:
     return "session_id"
   
-  @value_component("autoboot.web.http.session.max_age")
-  @staticmethod
+  @static_property("autoboot.web.http.session.max_age")
   def session_max_age() -> int:
     return 3600
 
-  @value_component("autoboot.web.http.session.same_site")
-  @staticmethod
+  @static_property("autoboot.web.http.session.same_site")
   def session_same_site() -> str:
     return "lax"
   
-  @value_component("autoboot.web.http.session.https_only")
-  @staticmethod
+  @static_property("autoboot.web.http.session.https_only")
   def session_https_only() -> bool:
     return False
```

### Comparing `autoboot-web-0.4.0/autoboot_web/mvc/annotation/controller.py` & `autoboot_web-0.5.0/autoboot_web/mvc/annotation/controller.py`

 * *Files identical despite different names*

### Comparing `autoboot-web-0.4.0/autoboot_web/mvc/apply_router.py` & `autoboot_web-0.5.0/autoboot_web/mvc/apply_router.py`

 * *Files identical despite different names*

### Comparing `autoboot-web-0.4.0/autoboot_web/runner.py` & `autoboot_web-0.5.0/autoboot_web/runner.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,43 @@
+import asyncio
 from typing import Optional
 from importlib import import_module
 from autoboot import AutoBoot
 from autoboot.plugin import AppPlugin
 from fastapi import FastAPI
 from fastapi.middleware.gzip import GZipMiddleware
 from starlette.middleware.sessions import SessionMiddleware
 from .http_properties import HttpProperties
 from .web_properties import WebProperties
 
 class WebRunner(AppPlugin[FastAPI]):
   
+  _loop: asyncio.AbstractEventLoop
+  
   # custom context name, default is class name
   #context_name = "WebRunner"
   
   def __init__(self, scan_controllers: Optional[str | list[str]] = None) -> None:
     self._scan_controllers = scan_controllers
+    
+  def __repr__(self) -> str:
+    return f"WebRunner(scan_controllers={self.scan_controllers}"
+    
+  def get_event_loop(cls) -> asyncio.AbstractEventLoop:
+    return cls._loop
   
   def install(self) -> FastAPI:
-    return FastAPI()
+    app = FastAPI()
+    
+    @app.on_event("startup")
+    def startup_event() -> None:
+      WebRunner._loop = asyncio.get_running_loop()
+      AutoBoot.logger.info("hold event loop: {}.", WebRunner._loop)
+      
+    return app
   
   def env_prepared(self) -> None:
     self.packages: list[str] = []
     if self._scan_controllers:
       self.packages.extend([self._scan_controllers] if isinstance(self._scan_controllers, str) else self._scan_controllers)
     
     if WebProperties.scan_controller_packages():
```

### Comparing `autoboot-web-0.4.0/autoboot_web.egg-info/SOURCES.txt` & `autoboot_web-0.5.0/autoboot_web.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
+requirements.txt
 setup.cfg
-setup.py
 autoboot_web/__init__.py
 autoboot_web/http_properties.py
 autoboot_web/runner.py
 autoboot_web/web_properties.py
 autoboot_web.egg-info/PKG-INFO
 autoboot_web.egg-info/SOURCES.txt
 autoboot_web.egg-info/dependency_links.txt
+autoboot_web.egg-info/not-zip-safe
 autoboot_web.egg-info/requires.txt
 autoboot_web.egg-info/top_level.txt
 autoboot_web/middleware/__init__.py
 autoboot_web/middleware/uniform.py
 autoboot_web/mvc/__init__.py
 autoboot_web/mvc/apply_router.py
 autoboot_web/mvc/annotation/__init__.py
```

### Comparing `autoboot-web-0.4.0/pyproject.toml` & `autoboot_web-0.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+# Python package
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+
 # https://beta.ruff.rs/docs/configuration/
 [tool.ruff]
 # Enable the pycodestyle (`E`) and Pyflakes (`F`) rules by default.
 # Unlike Flake8, Ruff doesn't enable pycodestyle warnings (`W`) or
 # McCabe complexity (`C901`) by default.
 select = ["E", "F"]
```

