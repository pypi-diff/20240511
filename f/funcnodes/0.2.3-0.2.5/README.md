# Comparing `tmp/funcnodes-0.2.3.tar.gz` & `tmp/funcnodes-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcnodes-0.2.3.tar", max compression
+gzip compressed data, was "funcnodes-0.2.5.tar", max compression
```

## Comparing `funcnodes-0.2.3.tar` & `funcnodes-0.2.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1725 2024-05-08 14:21:45.953180 funcnodes-0.2.3/funcnodes/__init__.py
--rw-r--r--   0        0        0     6499 2024-05-07 08:28:48.305494 funcnodes-0.2.3/funcnodes/__main__.py
--rw-r--r--   0        0        0     2032 2024-05-06 20:07:59.075924 funcnodes-0.2.3/funcnodes/_logging.py
--rw-r--r--   0        0        0      313 2024-04-11 20:53:13.157950 funcnodes-0.2.3/funcnodes/basic_nodes/__init__.py
--rw-r--r--   0        0        0     4391 2024-05-07 07:50:51.041520 funcnodes-0.2.3/funcnodes/basic_nodes/files.py
--rw-r--r--   0        0        0     3474 2024-05-07 07:39:01.326392 funcnodes-0.2.3/funcnodes/basic_nodes/logic.py
--rw-r--r--   0        0        0    11280 2024-05-05 22:02:37.701451 funcnodes-0.2.3/funcnodes/basic_nodes/math.py
--rw-r--r--   0        0        0     3593 2024-05-06 20:07:58.990311 funcnodes-0.2.3/funcnodes/config.py
--rw-r--r--   0        0        0     1594 2024-05-08 14:21:29.102094 funcnodes-0.2.3/funcnodes/data.py
--rw-r--r--   0        0        0    22123 2024-05-07 08:27:31.506589 funcnodes-0.2.3/funcnodes/eventmanager.py
--rw-r--r--   0        0        0      125 2024-05-06 20:08:00.654935 funcnodes-0.2.3/funcnodes/exceptions.py
--rw-r--r--   0        0        0        0 2024-02-26 12:43:49.198582 funcnodes-0.2.3/funcnodes/frontends/__init__.py
--rw-r--r--   0        0        0       28 2024-02-26 12:44:57.877828 funcnodes-0.2.3/funcnodes/frontends/funcnodes_react/__init__.py
--rw-r--r--   0        0        0      965 2024-04-25 08:06:56.551013 funcnodes-0.2.3/funcnodes/frontends/funcnodes_react/asset-manifest.json
--rw-r--r--   0        0        0    28362 2024-04-25 08:34:16.885037 funcnodes-0.2.3/funcnodes/frontends/funcnodes_react/css/style.css
--rw-r--r--   0        0        0     3870 2024-01-19 12:49:44.602000 funcnodes-0.2.3/funcnodes/frontends/funcnodes_react/favicon.ico
--rw-r--r--   0        0        0      658 2024-04-25 08:27:16.808142 funcnodes-0.2.3/funcnodes/frontends/funcnodes_react/index.html
--rw-r--r--   0        0        0  4138461 2024-04-25 08:27:16.808142 funcnodes-0.2.3/funcnodes/frontends/funcnodes_react/js/424.js
--rw-r--r--   0        0        0     3258 2024-04-25 08:27:16.808142 funcnodes-0.2.3/funcnodes/frontends/funcnodes_react/js/424.js.LICENSE.txt
--rw-r--r--   0        0        0   246139 2024-04-25 08:34:16.885037 funcnodes-0.2.3/funcnodes/frontends/funcnodes_react/js/main.js
--rw-r--r--   0        0        0    11348 2024-04-25 08:27:16.808142 funcnodes-0.2.3/funcnodes/frontends/funcnodes_react/js/main.js.LICENSE.txt
--rw-r--r--   0        0        0     5347 2024-01-19 12:49:44.602000 funcnodes-0.2.3/funcnodes/frontends/funcnodes_react/logo192.png
--rw-r--r--   0        0        0     9664 2024-01-19 12:49:44.602000 funcnodes-0.2.3/funcnodes/frontends/funcnodes_react/logo512.png
--rw-r--r--   0        0        0      492 2024-01-19 12:49:44.602000 funcnodes-0.2.3/funcnodes/frontends/funcnodes_react/manifest.json
--rw-r--r--   0        0        0       67 2024-01-19 12:49:44.602000 funcnodes-0.2.3/funcnodes/frontends/funcnodes_react/robots.txt
--rw-r--r--   0        0        0     2952 2024-04-25 08:14:13.637341 funcnodes-0.2.3/funcnodes/frontends/funcnodes_react/run.py
--rw-r--r--   0        0        0    27882 2024-05-06 04:17:35.134204 funcnodes-0.2.3/funcnodes/io.py
--rw-r--r--   0        0        0      421 2024-04-12 04:01:45.484336 funcnodes-0.2.3/funcnodes/lib/__init__.py
--rw-r--r--   0        0        0     6807 2024-03-19 15:11:29.279085 funcnodes-0.2.3/funcnodes/lib/lib.py
--rw-r--r--   0        0        0     7107 2024-05-08 11:06:44.923372 funcnodes-0.2.3/funcnodes/lib/libfinder.py
--rw-r--r--   0        0        0     1792 2024-04-16 04:49:07.183174 funcnodes-0.2.3/funcnodes/lib/libparser.py
--rw-r--r--   0        0        0    31452 2024-05-07 15:29:57.471965 funcnodes-0.2.3/funcnodes/node.py
--rw-r--r--   0        0        0    19738 2024-05-07 08:39:11.933956 funcnodes-0.2.3/funcnodes/nodemaker.py
--rw-r--r--   0        0        0    11850 2024-05-07 03:17:09.186518 funcnodes-0.2.3/funcnodes/nodespace.py
--rw-r--r--   0        0        0     3043 2024-02-23 07:11:27.809136 funcnodes-0.2.3/funcnodes/triggerstack.py
--rw-r--r--   0        0        0      362 2024-02-23 07:11:27.812331 funcnodes-0.2.3/funcnodes/utils/__init__.py
--rw-r--r--   0        0        0     3189 2024-04-11 08:37:44.578407 funcnodes-0.2.3/funcnodes/utils/data.py
--rw-r--r--   0        0        0     2744 2024-02-23 07:11:27.812331 funcnodes-0.2.3/funcnodes/utils/nodeutils.py
--rw-r--r--   0        0        0     5271 2024-05-07 08:22:20.139829 funcnodes-0.2.3/funcnodes/utils/serialization.py
--rw-r--r--   0        0        0      444 2024-05-07 13:05:54.019733 funcnodes-0.2.3/funcnodes/worker/__init__.py
--rw-r--r--   0        0        0     1808 2024-05-07 08:35:08.888378 funcnodes-0.2.3/funcnodes/worker/external_worker.py
--rw-r--r--   0        0        0     3736 2024-03-26 07:43:19.651903 funcnodes-0.2.3/funcnodes/worker/loop.py
--rw-r--r--   0        0        0     3293 2024-05-07 08:43:41.552734 funcnodes-0.2.3/funcnodes/worker/remote_worker.py
--rw-r--r--   0        0        0     8270 2024-05-07 08:43:38.346889 funcnodes-0.2.3/funcnodes/worker/websocket.py
--rw-r--r--   0        0        0    37914 2024-05-07 08:42:49.613686 funcnodes-0.2.3/funcnodes/worker/worker.py
--rw-r--r--   0        0        0    30152 2024-05-06 20:08:11.694569 funcnodes-0.2.3/funcnodes/worker/worker_manager.py
--rw-r--r--   0        0        0     1091 2023-10-26 07:00:17.799913 funcnodes-0.2.3/LICENSE
--rw-r--r--   0        0        0      666 2024-05-08 14:21:54.183390 funcnodes-0.2.3/pyproject.toml
--rw-r--r--   0        0        0    13174 2024-05-07 11:03:57.250582 funcnodes-0.2.3/README.md
--rw-r--r--   0        0        0    13528 1970-01-01 00:00:00.000000 funcnodes-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1725 2024-05-10 14:36:07.580636 funcnodes-0.2.5/funcnodes/__init__.py
+-rw-r--r--   0        0        0     6499 2024-05-07 08:28:48.305494 funcnodes-0.2.5/funcnodes/__main__.py
+-rw-r--r--   0        0        0     2032 2024-05-06 20:07:59.075924 funcnodes-0.2.5/funcnodes/_logging.py
+-rw-r--r--   0        0        0      313 2024-04-11 20:53:13.157950 funcnodes-0.2.5/funcnodes/basic_nodes/__init__.py
+-rw-r--r--   0        0        0     4654 2024-05-09 04:31:49.230279 funcnodes-0.2.5/funcnodes/basic_nodes/files.py
+-rw-r--r--   0        0        0     3474 2024-05-07 07:39:01.326392 funcnodes-0.2.5/funcnodes/basic_nodes/logic.py
+-rw-r--r--   0        0        0    11280 2024-05-05 22:02:37.701451 funcnodes-0.2.5/funcnodes/basic_nodes/math.py
+-rw-r--r--   0        0        0     3593 2024-05-06 20:07:58.990311 funcnodes-0.2.5/funcnodes/config.py
+-rw-r--r--   0        0        0     1911 2024-05-08 18:44:35.771663 funcnodes-0.2.5/funcnodes/data.py
+-rw-r--r--   0        0        0    22123 2024-05-07 08:27:31.506589 funcnodes-0.2.5/funcnodes/eventmanager.py
+-rw-r--r--   0        0        0      125 2024-05-06 20:08:00.654935 funcnodes-0.2.5/funcnodes/exceptions.py
+-rw-r--r--   0        0        0        0 2024-02-26 12:43:49.198582 funcnodes-0.2.5/funcnodes/frontends/__init__.py
+-rw-r--r--   0        0        0       28 2024-02-26 12:44:57.877828 funcnodes-0.2.5/funcnodes/frontends/funcnodes_react/__init__.py
+-rw-r--r--   0        0        0      965 2024-04-25 08:06:56.551013 funcnodes-0.2.5/funcnodes/frontends/funcnodes_react/asset-manifest.json
+-rw-r--r--   0        0        0    28362 2024-04-25 08:34:16.885037 funcnodes-0.2.5/funcnodes/frontends/funcnodes_react/css/style.css
+-rw-r--r--   0        0        0     3870 2024-01-19 12:49:44.602000 funcnodes-0.2.5/funcnodes/frontends/funcnodes_react/favicon.ico
+-rw-r--r--   0        0        0      658 2024-04-25 08:27:16.808142 funcnodes-0.2.5/funcnodes/frontends/funcnodes_react/index.html
+-rw-r--r--   0        0        0  4138461 2024-04-25 08:27:16.808142 funcnodes-0.2.5/funcnodes/frontends/funcnodes_react/js/424.js
+-rw-r--r--   0        0        0     3258 2024-04-25 08:27:16.808142 funcnodes-0.2.5/funcnodes/frontends/funcnodes_react/js/424.js.LICENSE.txt
+-rw-r--r--   0        0        0   246139 2024-04-25 08:34:16.885037 funcnodes-0.2.5/funcnodes/frontends/funcnodes_react/js/main.js
+-rw-r--r--   0        0        0    11348 2024-04-25 08:27:16.808142 funcnodes-0.2.5/funcnodes/frontends/funcnodes_react/js/main.js.LICENSE.txt
+-rw-r--r--   0        0        0     5347 2024-01-19 12:49:44.602000 funcnodes-0.2.5/funcnodes/frontends/funcnodes_react/logo192.png
+-rw-r--r--   0        0        0     9664 2024-01-19 12:49:44.602000 funcnodes-0.2.5/funcnodes/frontends/funcnodes_react/logo512.png
+-rw-r--r--   0        0        0      492 2024-01-19 12:49:44.602000 funcnodes-0.2.5/funcnodes/frontends/funcnodes_react/manifest.json
+-rw-r--r--   0        0        0       67 2024-01-19 12:49:44.602000 funcnodes-0.2.5/funcnodes/frontends/funcnodes_react/robots.txt
+-rw-r--r--   0        0        0     2952 2024-04-25 08:14:13.637341 funcnodes-0.2.5/funcnodes/frontends/funcnodes_react/run.py
+-rw-r--r--   0        0        0    27882 2024-05-06 04:17:35.134204 funcnodes-0.2.5/funcnodes/io.py
+-rw-r--r--   0        0        0      421 2024-04-12 04:01:45.484336 funcnodes-0.2.5/funcnodes/lib/__init__.py
+-rw-r--r--   0        0        0     6807 2024-03-19 15:11:29.279085 funcnodes-0.2.5/funcnodes/lib/lib.py
+-rw-r--r--   0        0        0     7175 2024-05-09 08:39:29.434373 funcnodes-0.2.5/funcnodes/lib/libfinder.py
+-rw-r--r--   0        0        0     1792 2024-04-16 04:49:07.183174 funcnodes-0.2.5/funcnodes/lib/libparser.py
+-rw-r--r--   0        0        0    31937 2024-05-10 08:51:13.309814 funcnodes-0.2.5/funcnodes/node.py
+-rw-r--r--   0        0        0    20423 2024-05-10 06:00:55.728776 funcnodes-0.2.5/funcnodes/nodemaker.py
+-rw-r--r--   0        0        0    11850 2024-05-07 03:17:09.186518 funcnodes-0.2.5/funcnodes/nodespace.py
+-rw-r--r--   0        0        0     3043 2024-02-23 07:11:27.809136 funcnodes-0.2.5/funcnodes/triggerstack.py
+-rw-r--r--   0        0        0      362 2024-02-23 07:11:27.812331 funcnodes-0.2.5/funcnodes/utils/__init__.py
+-rw-r--r--   0        0        0     3189 2024-04-11 08:37:44.578407 funcnodes-0.2.5/funcnodes/utils/data.py
+-rw-r--r--   0        0        0     2744 2024-02-23 07:11:27.812331 funcnodes-0.2.5/funcnodes/utils/nodeutils.py
+-rw-r--r--   0        0        0     5271 2024-05-07 08:22:20.139829 funcnodes-0.2.5/funcnodes/utils/serialization.py
+-rw-r--r--   0        0        0      444 2024-05-07 13:05:54.019733 funcnodes-0.2.5/funcnodes/worker/__init__.py
+-rw-r--r--   0        0        0     1808 2024-05-07 08:35:08.888378 funcnodes-0.2.5/funcnodes/worker/external_worker.py
+-rw-r--r--   0        0        0     3736 2024-03-26 07:43:19.651903 funcnodes-0.2.5/funcnodes/worker/loop.py
+-rw-r--r--   0        0        0     3293 2024-05-07 08:43:41.552734 funcnodes-0.2.5/funcnodes/worker/remote_worker.py
+-rw-r--r--   0        0        0     8270 2024-05-07 08:43:38.346889 funcnodes-0.2.5/funcnodes/worker/websocket.py
+-rw-r--r--   0        0        0    37914 2024-05-07 08:42:49.613686 funcnodes-0.2.5/funcnodes/worker/worker.py
+-rw-r--r--   0        0        0    30152 2024-05-06 20:08:11.694569 funcnodes-0.2.5/funcnodes/worker/worker_manager.py
+-rw-r--r--   0        0        0     1091 2023-10-26 07:00:17.799913 funcnodes-0.2.5/LICENSE
+-rw-r--r--   0        0        0      652 2024-05-10 14:36:56.954892 funcnodes-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0    13174 2024-05-07 11:03:57.250582 funcnodes-0.2.5/README.md
+-rw-r--r--   0        0        0    13505 1970-01-01 00:00:00.000000 funcnodes-0.2.5/PKG-INFO
```

### Comparing `funcnodes-0.2.3/funcnodes/__init__.py` & `funcnodes-0.2.5/funcnodes/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,10 +62,10 @@
     "assert_worker_manager_running",
     "config",
     "RenderOptions",
     "NoValue",
     "DataEnum",
 ]
 
-__version__ = "0.2.3"
+__version__ = "0.2.5"
 
 DEBUG = True
```

### Comparing `funcnodes-0.2.3/funcnodes/__main__.py` & `funcnodes-0.2.5/funcnodes/__main__.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/funcnodes/_logging.py` & `funcnodes-0.2.5/funcnodes/_logging.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/funcnodes/basic_nodes/files.py` & `funcnodes-0.2.5/funcnodes/basic_nodes/files.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,24 @@
         """
         Downloads a file from a given URL and sets the "data" output to the file's content as bytes.
 
         Args:
           url (str): The URL of the file to download.
           timeout (float): The timeout in seconds for the download request.
         """
-        response = requests.get(url, timeout=timeout)
+        response = requests.get(
+            url,
+            timeout=timeout,
+            headers={
+                # set user agent to avoid 403 forbidden error
+                "User-Agent": "Mozilla/5.0",
+                # allow download of files
+                "Accept": "*/*",
+            },
+        )
         self.outputs["data"].value = response.content
 
 
 class BytesToStringNode(Node):
     """
     Converts bytes to a string using the specified encoding.
```

### Comparing `funcnodes-0.2.3/funcnodes/basic_nodes/logic.py` & `funcnodes-0.2.5/funcnodes/basic_nodes/logic.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/funcnodes/basic_nodes/math.py` & `funcnodes-0.2.5/funcnodes/basic_nodes/math.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/funcnodes/config.py` & `funcnodes-0.2.5/funcnodes/config.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/funcnodes/data.py` & `funcnodes-0.2.5/funcnodes/data.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,28 +29,39 @@
 
     def __init_subclass__(cls) -> None:
         add_type(
             cls,
             cls.__name__,
         )
 
+        cls._lookup = {}
+        for member in cls:
+            cls._lookup[member.name] = member
+            try:
+                if member.value not in cls._lookup:
+                    cls._lookup[member.value] = member
+            except TypeError:
+                pass
+            if str(member.value) not in cls._lookup:
+                cls._lookup[str(member.value)] = member
+
     @classmethod
     def interfere(cls: Type[ET], a: Union[ET, str, Any]) -> ET:
-        if isinstance(a, str) and a in cls.__members__:
-            return cls[a]
-        elif isinstance(a, cls):
+
+        if isinstance(a, cls):
             return a
-        else:
-            try:
-                return cls(a)
-            except ValueError as e:
-                if isinstance(a, str):
-                    if a.startswith(cls.__name__ + "."):
-                        a = a[len(cls.__name__) + 1 :]
-                        if a in cls.__members__:
-                            return cls[a]
+        if a in cls._lookup:
+            return cls._lookup[a]
+        try:
+            return cls(a)
+        except ValueError as e:
+            if isinstance(a, str):
+                if a.startswith(cls.__name__ + "."):
+                    a = a[len(cls.__name__) + 1 :]
+                    if a in cls._lookup:
+                        return cls._lookup[a]
 
-                raise e
+            raise e
 
     @classmethod
     def v(cls: Type[ET], a: Union[ET, str, Any]) -> Any:
         return cls.interfere(a).value
```

### Comparing `funcnodes-0.2.3/funcnodes/eventmanager.py` & `funcnodes-0.2.5/funcnodes/eventmanager.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/funcnodes/frontends/funcnodes_react/asset-manifest.json` & `funcnodes-0.2.5/funcnodes/frontends/funcnodes_react/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/funcnodes/frontends/funcnodes_react/css/style.css` & `funcnodes-0.2.5/funcnodes/frontends/funcnodes_react/css/style.css`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/funcnodes/frontends/funcnodes_react/favicon.ico` & `funcnodes-0.2.5/funcnodes/frontends/funcnodes_react/favicon.ico`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/funcnodes/frontends/funcnodes_react/index.html` & `funcnodes-0.2.5/funcnodes/frontends/funcnodes_react/index.html`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/funcnodes/frontends/funcnodes_react/js/424.js` & `funcnodes-0.2.5/funcnodes/frontends/funcnodes_react/js/424.js`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/funcnodes/frontends/funcnodes_react/js/424.js.LICENSE.txt` & `funcnodes-0.2.5/funcnodes/frontends/funcnodes_react/js/424.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/funcnodes/frontends/funcnodes_react/js/main.js` & `funcnodes-0.2.5/funcnodes/frontends/funcnodes_react/js/main.js`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/funcnodes/frontends/funcnodes_react/js/main.js.LICENSE.txt` & `funcnodes-0.2.5/funcnodes/frontends/funcnodes_react/js/main.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/funcnodes/frontends/funcnodes_react/logo192.png` & `funcnodes-0.2.5/funcnodes/frontends/funcnodes_react/logo192.png`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/funcnodes/frontends/funcnodes_react/logo512.png` & `funcnodes-0.2.5/funcnodes/frontends/funcnodes_react/logo512.png`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/funcnodes/frontends/funcnodes_react/run.py` & `funcnodes-0.2.5/funcnodes/frontends/funcnodes_react/run.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/funcnodes/io.py` & `funcnodes-0.2.5/funcnodes/io.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/funcnodes/lib/lib.py` & `funcnodes-0.2.5/funcnodes/lib/lib.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/funcnodes/lib/libfinder.py` & `funcnodes-0.2.5/funcnodes/lib/libfinder.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,18 @@
             strmod = mod
             dat = BaseShelfDict(module=strmod)
 
         # submodules = strmod.split(".")
 
         module = importlib.import_module(strmod)
         # reload module to get the latest version
-        importlib.reload(module)
+        try:
+            importlib.reload(module)
+        except Exception as e:
+            pass
         # for submod in submodules[1:]:
         #     mod = getattr(mod, submod)
 
         return module_to_shelf(module), dat
 
     except (ModuleNotFoundError, KeyError) as e:
         fn.FUNCNODES_LOGGER.exception(e)
```

### Comparing `funcnodes-0.2.3/funcnodes/lib/libparser.py` & `funcnodes-0.2.5/funcnodes/lib/libparser.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/funcnodes/node.py` & `funcnodes-0.2.5/funcnodes/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,15 @@
     node_id: str
     node_name: str
     default_reset_inputs_on_trigger: bool = False
     description: Optional[str] = None
 
     default_render_options: RenderOptions = {}
     default_io_options: Dict[str, NodeInputOptions | NodeOutputOptions] = {}
-    default_trigger_on_create: bool = False
+    default_trigger_on_create: bool = True
 
     triggerinput = NodeInput(
         id="_triggerinput",
         name="( )",
         description="Trigger the node",
         default=None,
         required=False,
@@ -700,14 +700,15 @@
             kwargs = {
                 ip.uuid: ip.value for ip in self._inputs if ip.value is not NoValue
             }
             err = None
             if "_triggerinput" in kwargs:
                 del kwargs["_triggerinput"]
             try:
+
                 ans = await self.func(**kwargs)
                 # reset the inputs if requested
                 if self.reset_inputs_on_trigger:
                     for ip in self._inputs:
                         ip.set_value(ip.default, does_trigger=False)
             except Exception as e:
                 err = e
@@ -889,28 +890,47 @@
     render_options: NotRequired[RenderOptions]
 
 
 # region node registry
 REGISTERED_NODES: Dict[str, Type[Node]] = {}
 
 
+def _get_node_src(node: Type[Node]) -> str:
+    try:
+        file = inspect.getfile(node)
+    except Exception:
+        file = "<unknown file>"
+    try:
+        line = inspect.getsourcelines(node)[1]
+    except Exception:
+        line = "<unknown line>"
+
+    try:
+        module = node.__module__
+    except Exception:
+        module = "<unknown module>"
+    return f"{module}({file}:{line})"
+
+
 def register_node(node_class: Type[Node]):
     """
     Registers a node class by adding it to the REGISTERED_NODES dictionary with its 'node_id' as the key.
     If the 'node_id' already exists in the dictionary, it raises a NodeIdAlreadyExistsError.
 
     Args:
         node_class (Type[Node]): The class of the node to register.
 
     Raises:
         NodeIdAlreadyExistsError: If a node with the same 'node_id' is already registered.
     """
     node_id = node_class.node_id
     if node_id in REGISTERED_NODES:
-        raise NodeIdAlreadyExistsError(f"Node with id {node_id} already exists")
+        raise NodeIdAlreadyExistsError(
+            f"Node with id '{node_id}' already exists at {_get_node_src(REGISTERED_NODES[node_id])}"
+        )
 
     REGISTERED_NODES[node_id] = node_class
 
 
 class NodeKeyError(KeyError):
     """Exception raised when a node with a given id is not registered."""
```

### Comparing `funcnodes-0.2.3/funcnodes/nodemaker.py` & `funcnodes-0.2.5/funcnodes/nodemaker.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     from typing_extensions import Unpack
 
 
 def node_class_maker(
     id: Optional[str] = None,
     func: Callable[..., ReturnType] = None,
     superclass: Type[Node] = Node,
+    seperate_thread: bool = False,
     **kwargs: Unpack[NodeClassDict],
 ) -> Type[Node]:
     """
     Creates a node class from a function.
 
     Args:
       id (str, optional): The id of the node. Defaults to None.
@@ -83,14 +84,30 @@
             """
             return ofunc(*args, **kwargs)
 
     else:
         in_func: ExposedFunction[Coroutine[Any, Any, ReturnType]] = in_func
         asyncfunc = in_func
 
+    if seperate_thread:
+        oasyncfunc = asyncfunc
+
+        @wraps(oasyncfunc)
+        async def _wrapped_func(*args, **kwargs):
+            """
+            A wrapper for the exposed function that sets the output values of the node.
+            """
+            loop = asyncio.get_event_loop()
+            outs = await loop.run_in_executor(
+                None, lambda: asyncio.run(oasyncfunc(*args, **kwargs))
+            )
+            return outs
+
+        asyncfunc = _wrapped_func
+
     exfunc: ExposedFunction[Coroutine[Any, Any, ReturnType]] = asyncfunc
 
     @wraps(asyncfunc)
     async def _wrapped_func(self: Node, *args, **kwargs):
         """
         A wrapper for the exposed function that sets the output values of the node.
         """
@@ -142,14 +159,15 @@
 
 class NodeDecoratorKwargs(ExposedMethodKwargs, NodeClassDict, total=False):
     """
     Keyword arguments for the node_class_maker function.
     """
 
     superclass: Optional[Type[Node]]
+    seperate_thread: Optional[bool]
 
 
 def NodeDecorator(
     id: Optional[str] = None, **kwargs: Unpack[NodeDecoratorKwargs]
 ) -> Callable[..., Type[Node]]:
     """Decorator to create a Node class from a function."""
 
@@ -172,15 +190,19 @@
             v: kwargs[v] for v in NodeClassDictsKeys if v in kwargs  # type: ignore
         }
 
         # Assure the method is exposed for node functionality
         func = assure_exposed_method(func, **exposed_method_kwargs)
         # Create the node class
         return node_class_maker(
-            id, func, superclass=kwargs.get("superclass", Node), **node_class_kwargs
+            id,
+            func,
+            superclass=kwargs.get("superclass", Node),
+            seperate_thread=kwargs.get("seperate_thread", False),
+            **node_class_kwargs,
         )
 
     return decorator
 
 
 def instance_nodefunction(
     trigger_on_call: Optional[bool] = None, **kwargs: Unpack[NodeDecoratorKwargs]
```

### Comparing `funcnodes-0.2.3/funcnodes/nodespace.py` & `funcnodes-0.2.5/funcnodes/nodespace.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/funcnodes/triggerstack.py` & `funcnodes-0.2.5/funcnodes/triggerstack.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/funcnodes/utils/data.py` & `funcnodes-0.2.5/funcnodes/utils/data.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/funcnodes/utils/nodeutils.py` & `funcnodes-0.2.5/funcnodes/utils/nodeutils.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/funcnodes/utils/serialization.py` & `funcnodes-0.2.5/funcnodes/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/funcnodes/worker/external_worker.py` & `funcnodes-0.2.5/funcnodes/worker/external_worker.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/funcnodes/worker/loop.py` & `funcnodes-0.2.5/funcnodes/worker/loop.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/funcnodes/worker/remote_worker.py` & `funcnodes-0.2.5/funcnodes/worker/remote_worker.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/funcnodes/worker/websocket.py` & `funcnodes-0.2.5/funcnodes/worker/websocket.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/funcnodes/worker/worker.py` & `funcnodes-0.2.5/funcnodes/worker/worker.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/funcnodes/worker/worker_manager.py` & `funcnodes-0.2.5/funcnodes/worker/worker_manager.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/LICENSE` & `funcnodes-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/pyproject.toml` & `funcnodes-0.2.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tool.poetry]
 name = "funcnodes"
-version = "0.2.3"
+version = "0.2.5"
 description = "funcnodes"
 authors = ["Julian Kimmig <julian.kimmig@linkdlab.de>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-exposedfunctionality = "^0.3.6"
+exposedfunctionality = "^0.3"
 websockets = "^12.0"
-virtualenv = "^20.25.1"
-poetry-plugin-export = "^1.7.1"
-python-dotenv = "^1.0.1"
+virtualenv = "*"
+poetry-plugin-export = "^1.7"
+python-dotenv = "*"
+poetry = "*" 
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.4.2"
-coverage = "^7.3.2"
-pandas = "^2.2.0"
-pillow = "^10.2.0"
-opencv-python = "^4.9.0.80"
+pytest = "^7.4"
+coverage = "^7.3"
+pandas = "^2.2"
+pillow = "^10.2"
+opencv-python = "^4.9"
 vulture = "^2.11"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
```

### Comparing `funcnodes-0.2.3/README.md` & `funcnodes-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.3/PKG-INFO` & `funcnodes-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: funcnodes
-Version: 0.2.3
+Version: 0.2.5
 Summary: funcnodes
 Author: Julian Kimmig
 Author-email: julian.kimmig@linkdlab.de
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: exposedfunctionality (>=0.3.6,<0.4.0)
-Requires-Dist: poetry-plugin-export (>=1.7.1,<2.0.0)
-Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
-Requires-Dist: virtualenv (>=20.25.1,<21.0.0)
+Requires-Dist: exposedfunctionality (>=0.3,<0.4)
+Requires-Dist: poetry
+Requires-Dist: poetry-plugin-export (>=1.7,<2.0)
+Requires-Dist: python-dotenv
+Requires-Dist: virtualenv
 Requires-Dist: websockets (>=12.0,<13.0)
 Description-Content-Type: text/markdown
 
 # Funcnodes Project README
 
 ## Project Overview
```

