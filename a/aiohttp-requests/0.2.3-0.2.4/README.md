# Comparing `tmp/aiohttp-requests-0.2.3.tar.gz` & `tmp/aiohttp-requests-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohttp-requests-0.2.3.tar", last modified: Sat Sep 30 01:54:35 2023, max compression
+gzip compressed data, was "aiohttp-requests-0.2.4.tar", last modified: Sat May 11 19:48:51 2024, max compression
```

## Comparing `aiohttp-requests-0.2.3.tar` & `aiohttp-requests-0.2.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-09-30 01:54:35.458948 aiohttp-requests-0.2.3/
--rw-r--r--   0 max        (501) staff       (20)       82 2023-04-11 16:12:04.000000 aiohttp-requests-0.2.3/.coveragerc
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-09-30 01:54:35.456730 aiohttp-requests-0.2.3/.github/
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-09-30 01:54:35.457760 aiohttp-requests-0.2.3/.github/workflows/
--rw-r--r--   0 max        (501) staff       (20)      850 2023-09-23 22:50:32.000000 aiohttp-requests-0.2.3/.github/workflows/python-package.yml
--rw-r--r--   0 max        (501) staff       (20)     1212 2023-04-11 16:12:04.000000 aiohttp-requests-0.2.3/.gitignore
--rw-r--r--   0 max        (501) staff       (20)     1066 2023-04-11 16:12:04.000000 aiohttp-requests-0.2.3/LICENSE
--rw-r--r--   0 max        (501) staff       (20)     2935 2023-09-30 01:54:35.458838 aiohttp-requests-0.2.3/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)     2318 2023-09-30 01:53:34.000000 aiohttp-requests-0.2.3/README.rst
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-09-30 01:54:35.457981 aiohttp-requests-0.2.3/aiohttp_requests/
--rw-r--r--   0 max        (501) staff       (20)     3324 2023-09-30 01:49:43.000000 aiohttp-requests-0.2.3/aiohttp_requests/__init__.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-09-30 01:54:35.458471 aiohttp-requests-0.2.3/aiohttp_requests.egg-info/
--rw-r--r--   0 max        (501) staff       (20)     2935 2023-09-30 01:54:35.000000 aiohttp-requests-0.2.3/aiohttp_requests.egg-info/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)      390 2023-09-30 01:54:35.000000 aiohttp-requests-0.2.3/aiohttp_requests.egg-info/SOURCES.txt
--rw-r--r--   0 max        (501) staff       (20)        1 2023-09-30 01:54:35.000000 aiohttp-requests-0.2.3/aiohttp_requests.egg-info/dependency_links.txt
--rw-r--r--   0 max        (501) staff       (20)       32 2023-09-30 01:54:35.000000 aiohttp-requests-0.2.3/aiohttp_requests.egg-info/requires.txt
--rw-r--r--   0 max        (501) staff       (20)       17 2023-09-30 01:54:35.000000 aiohttp-requests-0.2.3/aiohttp_requests.egg-info/top_level.txt
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-09-30 01:54:35.458571 aiohttp-requests-0.2.3/docs/
--rw-r--r--   0 max        (501) staff       (20)     3200 2023-09-30 01:54:35.000000 aiohttp-requests-0.2.3/docs/CHANGELOG.rst
--rw-r--r--   0 max        (501) staff       (20)       32 2023-09-30 01:35:47.000000 aiohttp-requests-0.2.3/requirements.txt
--rw-r--r--   0 max        (501) staff       (20)       38 2023-09-30 01:54:35.458980 aiohttp-requests-0.2.3/setup.cfg
--rw-r--r--   0 max        (501) staff       (20)      908 2023-09-24 02:28:09.000000 aiohttp-requests-0.2.3/setup.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-09-30 01:54:35.458672 aiohttp-requests-0.2.3/tests/
--rw-r--r--   0 max        (501) staff       (20)     1551 2023-09-30 01:26:24.000000 aiohttp-requests-0.2.3/tests/test_aiohttp_requests.py
--rw-r--r--   0 max        (501) staff       (20)     1174 2023-09-23 22:39:38.000000 aiohttp-requests-0.2.3/tox.ini
+drwxr-xr-x   0 max        (501) staff       (20)        0 2024-05-11 19:48:51.640044 aiohttp-requests-0.2.4/
+-rw-r--r--   0 max        (501) staff       (20)       82 2023-04-11 16:12:04.000000 aiohttp-requests-0.2.4/.coveragerc
+drwxr-xr-x   0 max        (501) staff       (20)        0 2024-05-11 19:48:51.637246 aiohttp-requests-0.2.4/.github/
+drwxr-xr-x   0 max        (501) staff       (20)        0 2024-05-11 19:48:51.638651 aiohttp-requests-0.2.4/.github/workflows/
+-rw-r--r--   0 max        (501) staff       (20)      850 2023-09-23 22:50:32.000000 aiohttp-requests-0.2.4/.github/workflows/python-package.yml
+-rw-r--r--   0 max        (501) staff       (20)     1212 2023-04-11 16:12:04.000000 aiohttp-requests-0.2.4/.gitignore
+-rw-r--r--   0 max        (501) staff       (20)     1066 2023-04-11 16:12:04.000000 aiohttp-requests-0.2.4/LICENSE
+-rw-r--r--   0 max        (501) staff       (20)     2943 2024-05-11 19:48:51.639922 aiohttp-requests-0.2.4/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)     2326 2024-05-11 19:33:11.000000 aiohttp-requests-0.2.4/README.rst
+drwxr-xr-x   0 max        (501) staff       (20)        0 2024-05-11 19:48:51.638900 aiohttp-requests-0.2.4/aiohttp_requests/
+-rw-r--r--   0 max        (501) staff       (20)     3442 2024-05-11 19:41:52.000000 aiohttp-requests-0.2.4/aiohttp_requests/__init__.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2024-05-11 19:48:51.639508 aiohttp-requests-0.2.4/aiohttp_requests.egg-info/
+-rw-r--r--   0 max        (501) staff       (20)     2943 2024-05-11 19:48:51.000000 aiohttp-requests-0.2.4/aiohttp_requests.egg-info/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)      390 2024-05-11 19:48:51.000000 aiohttp-requests-0.2.4/aiohttp_requests.egg-info/SOURCES.txt
+-rw-r--r--   0 max        (501) staff       (20)        1 2024-05-11 19:48:51.000000 aiohttp-requests-0.2.4/aiohttp_requests.egg-info/dependency_links.txt
+-rw-r--r--   0 max        (501) staff       (20)       32 2024-05-11 19:48:51.000000 aiohttp-requests-0.2.4/aiohttp_requests.egg-info/requires.txt
+-rw-r--r--   0 max        (501) staff       (20)       17 2024-05-11 19:48:51.000000 aiohttp-requests-0.2.4/aiohttp_requests.egg-info/top_level.txt
+drwxr-xr-x   0 max        (501) staff       (20)        0 2024-05-11 19:48:51.639614 aiohttp-requests-0.2.4/docs/
+-rw-r--r--   0 max        (501) staff       (20)     3340 2024-05-11 19:48:51.000000 aiohttp-requests-0.2.4/docs/CHANGELOG.rst
+-rw-r--r--   0 max        (501) staff       (20)       32 2023-09-30 01:35:47.000000 aiohttp-requests-0.2.4/requirements.txt
+-rw-r--r--   0 max        (501) staff       (20)       38 2024-05-11 19:48:51.640080 aiohttp-requests-0.2.4/setup.cfg
+-rw-r--r--   0 max        (501) staff       (20)      908 2023-09-30 01:54:39.000000 aiohttp-requests-0.2.4/setup.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2024-05-11 19:48:51.639746 aiohttp-requests-0.2.4/tests/
+-rw-r--r--   0 max        (501) staff       (20)     1682 2024-05-11 19:47:12.000000 aiohttp-requests-0.2.4/tests/test_aiohttp_requests.py
+-rw-r--r--   0 max        (501) staff       (20)     1174 2023-09-23 22:39:38.000000 aiohttp-requests-0.2.4/tox.ini
```

### Comparing `aiohttp-requests-0.2.3/.github/workflows/python-package.yml` & `aiohttp-requests-0.2.4/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `aiohttp-requests-0.2.3/.gitignore` & `aiohttp-requests-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `aiohttp-requests-0.2.3/LICENSE` & `aiohttp-requests-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aiohttp-requests-0.2.3/PKG-INFO` & `aiohttp-requests-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohttp-requests
-Version: 0.2.3
+Version: 0.2.4
 Summary: A thin wrapper for aiohttp client with Requests simplicity
 Home-page: https://github.com/maxzheng/aiohttp-requests
 Author: Max Zheng
 Author-email: maxzheng.os @t gmail.com
 License: MIT
 Keywords: aiohttp HTTP client async requests
 Classifier: Development Status :: 5 - Production/Stable
@@ -53,15 +53,15 @@
 .. code-block:: python
 
     async def main():
         # Pass in a list of urls instead of just one. Optionally pass in as_iterator=True to iterate the responses.
         responses = await requests.get(['https://api.github.com'] * 2, auth=aiohttp.BasicAuth('user', 'password'))
         print(responses)    # [<ClientResponse(https://...) [200 OK]>, , <ClientResponse(https://...) [200 OK]>]
 
-        # It defaults to 10 concurrent requests. If you can handle more, then set it higher:
+        # It defaults to 10 concurrent requests maximum. If you can handle more, then set it higher:
         requests.max_concurrency = 100
 
     asyncio.run(main())
 
 The `requests` object is just proxying `get` and other HTTP verb methods to `aiohttp.ClientSession`_, which returns `aiohttp.ClientResponse`_. To do anything else, read the aiohttp_ doc.
 
 .. _`aiohttp.ClientSession`: https://docs.aiohttp.org/en/stable/client_reference.html?#aiohttp.ClientSession
```

### Comparing `aiohttp-requests-0.2.3/README.rst` & `aiohttp-requests-0.2.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 .. code-block:: python
 
     async def main():
         # Pass in a list of urls instead of just one. Optionally pass in as_iterator=True to iterate the responses.
         responses = await requests.get(['https://api.github.com'] * 2, auth=aiohttp.BasicAuth('user', 'password'))
         print(responses)    # [<ClientResponse(https://...) [200 OK]>, , <ClientResponse(https://...) [200 OK]>]
 
-        # It defaults to 10 concurrent requests. If you can handle more, then set it higher:
+        # It defaults to 10 concurrent requests maximum. If you can handle more, then set it higher:
         requests.max_concurrency = 100
 
     asyncio.run(main())
 
 The `requests` object is just proxying `get` and other HTTP verb methods to `aiohttp.ClientSession`_, which returns `aiohttp.ClientResponse`_. To do anything else, read the aiohttp_ doc.
 
 .. _`aiohttp.ClientSession`: https://docs.aiohttp.org/en/stable/client_reference.html?#aiohttp.ClientSession
```

### Comparing `aiohttp-requests-0.2.3/aiohttp_requests/__init__.py` & `aiohttp-requests-0.2.4/aiohttp_requests/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,40 +25,44 @@
         """ An instance of aiohttp.ClientSession """
         if not self._session or self._session.closed or self._session._loop.is_closed():
             self._session = aiohttp.ClientSession(*self._session_args[0], **self._session_args[1])
         return self._session
 
     def __getattr__(self, attr):
         if attr.upper() in aiohttp.hdrs.METH_ALL:
-            @functools.wraps(self.session._request)
-            def session_request(path, *args, **kwargs):
-                """
-                This ensures `self.session` is always called where it can check the session/loop state so can't use
-                functools.partials as monkeypatch seems to do something weird where __getattr__ is only called once
-                for each attribute after patch is undone
-                """
-                if isinstance(path, (list, tuple)):
-                    return self._concurrent_request(self.session._request, attr.upper(), path, args, kwargs,
-                                                    as_iterator=kwargs.pop('as_iterator', False))
-                else:
-                    return self.session._request(attr.upper(), path, *args, **kwargs)
-
-            return session_request
+            return functools.partial(self.request, attr.upper())
         else:
             return super().__getattribute__(attr)
 
     def __setattr__(self, attr, value):
         if attr == 'max_concurrency':
             self._worker.max_concurrency = value
         else:
             super().__setattr__(attr, value)
 
     def _concurrent_request(self, request, verb, paths, args, kwargs, as_iterator=False):
         return self._worker.do([(request, verb, path, args, kwargs) for path in paths], as_iterator=as_iterator)
 
+    def request(self, verb, path, *args, **kwargs):
+        """
+        This ensures `self.session` is always called where it can check the session/loop state so can't use
+        functools.partials as monkeypatch seems to do something weird where __getattr__ is only called once
+        for each attribute after patch is undone
+
+        :param verb: HTTP verb
+        :param path: URL path
+        :param args: Additional arguments for aiohttp.ClientSession.request
+        :param kwargs: Additional keyword arguments for aiohttp.ClientSession.request
+        """
+        if isinstance(path, (list, tuple)):
+            return self._concurrent_request(self.session._request, verb.upper(), path, args, kwargs,
+                                            as_iterator=kwargs.pop('as_iterator', False))
+        else:
+            return self.session._request(verb.upper(), path, *args, **kwargs)
+
     def close(self):
         """
         Close aiohttp.ClientSession.
 
         This is useful to be called manually in tests if each test when each test uses a new loop. After close, new
         requests will automatically create a new session.
```

### Comparing `aiohttp-requests-0.2.3/aiohttp_requests.egg-info/PKG-INFO` & `aiohttp-requests-0.2.4/aiohttp_requests.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohttp-requests
-Version: 0.2.3
+Version: 0.2.4
 Summary: A thin wrapper for aiohttp client with Requests simplicity
 Home-page: https://github.com/maxzheng/aiohttp-requests
 Author: Max Zheng
 Author-email: maxzheng.os @t gmail.com
 License: MIT
 Keywords: aiohttp HTTP client async requests
 Classifier: Development Status :: 5 - Production/Stable
@@ -53,15 +53,15 @@
 .. code-block:: python
 
     async def main():
         # Pass in a list of urls instead of just one. Optionally pass in as_iterator=True to iterate the responses.
         responses = await requests.get(['https://api.github.com'] * 2, auth=aiohttp.BasicAuth('user', 'password'))
         print(responses)    # [<ClientResponse(https://...) [200 OK]>, , <ClientResponse(https://...) [200 OK]>]
 
-        # It defaults to 10 concurrent requests. If you can handle more, then set it higher:
+        # It defaults to 10 concurrent requests maximum. If you can handle more, then set it higher:
         requests.max_concurrency = 100
 
     asyncio.run(main())
 
 The `requests` object is just proxying `get` and other HTTP verb methods to `aiohttp.ClientSession`_, which returns `aiohttp.ClientResponse`_. To do anything else, read the aiohttp_ doc.
 
 .. _`aiohttp.ClientSession`: https://docs.aiohttp.org/en/stable/client_reference.html?#aiohttp.ClientSession
```

### Comparing `aiohttp-requests-0.2.3/docs/CHANGELOG.rst` & `aiohttp-requests-0.2.4/docs/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,16 @@
-Version 0.2.3
+Version 0.2.4
 ================================================================================
 
+* Add request() method
+* Update README.rst
+
+Version 0.2.3
+--------------------------------------------------------------------------------
+
 * Support concurrent requests
 
 Version 0.2.2
 --------------------------------------------------------------------------------
 
 * Update readme to use asyncio.run
```

### Comparing `aiohttp-requests-0.2.3/setup.py` & `aiohttp-requests-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 
 setuptools.setup(
     name='aiohttp-requests',
-    version='0.2.3',
+    version='0.2.4',
 
     author='Max Zheng',
     author_email='maxzheng.os @t gmail.com',
 
     description='A thin wrapper for aiohttp client with Requests simplicity',
     long_description=open('README.rst').read(),
```

### Comparing `aiohttp-requests-0.2.3/tests/test_aiohttp_requests.py` & `aiohttp-requests-0.2.4/tests/test_aiohttp_requests.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,34 +20,37 @@
 async def test_aiohttp_requests_integration():
     # One request
     response = await requests.get('https://www.google.com')
     content = await response.text()
 
     assert response.status == 200
     assert len(content) > 10000
+    assert 'Search the world' in content
 
 
 async def test_aiohttp_requests_integration_multiple():
     # Multiple requests
     responses = await requests.get(['https://www.google.com'] * 2)
     assert len(responses) == 2
     for response in responses:
         content = await response.text()
 
         assert response.status == 200
         assert len(content) > 10000
+        assert 'Search the world' in content
 
     # Multiple requests as iterator
     responses = requests.get(['https://www.google.com'] * 2, as_iterator=True)
     for response in responses:
         response = await response
         content = await response.text()
 
         assert response.status == 200
         assert len(content) > 10000
+        assert 'Search the world' in content
 
 
 async def test_aiohttp_requests_after_close():
     # Closing ourself
     requests.close()
 
     await test_aiohttp_requests_integration()
```

### Comparing `aiohttp-requests-0.2.3/tox.ini` & `aiohttp-requests-0.2.4/tox.ini`

 * *Files identical despite different names*

