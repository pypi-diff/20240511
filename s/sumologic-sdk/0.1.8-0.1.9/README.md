# Comparing `tmp/sumologic-sdk-0.1.8.tar.gz` & `tmp/sumologic-sdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sumologic-sdk-0.1.8.tar", last modified: Sat Sep 15 07:12:08 2018, max compression
+gzip compressed data, was "dist/sumologic-sdk-0.1.9.tar", last modified: Thu Feb 20 16:55:18 2020, max compression
```

## Comparing `sumologic-sdk-0.1.8.tar` & `sumologic-sdk-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 duc        (501) staff       (20)        0 2018-09-15 07:12:08.000000 sumologic-sdk-0.1.8/
--rw-r--r--   0 duc        (501) staff       (20)      408 2018-09-15 07:12:08.000000 sumologic-sdk-0.1.8/PKG-INFO
--rw-r--r--   0 duc        (501) staff       (20)     1385 2018-09-15 07:01:14.000000 sumologic-sdk-0.1.8/README.md
--rw-r--r--   0 duc        (501) staff       (20)       38 2018-09-15 07:12:08.000000 sumologic-sdk-0.1.8/setup.cfg
--rw-r--r--   0 duc        (501) staff       (20)      557 2018-09-15 07:11:45.000000 sumologic-sdk-0.1.8/setup.py
-drwxr-xr-x   0 duc        (501) staff       (20)        0 2018-09-15 07:12:08.000000 sumologic-sdk-0.1.8/sumologic/
--rw-r--r--   0 duc        (501) staff       (20)      114 2018-09-15 07:01:14.000000 sumologic-sdk-0.1.8/sumologic/__init__.py
--rw-r--r--   0 duc        (501) staff       (20)     6869 2018-09-15 07:01:14.000000 sumologic-sdk-0.1.8/sumologic/sumologic.py
-drwxr-xr-x   0 duc        (501) staff       (20)        0 2018-09-15 07:12:08.000000 sumologic-sdk-0.1.8/sumologic_sdk.egg-info/
--rw-r--r--   0 duc        (501) staff       (20)        1 2018-09-15 07:12:08.000000 sumologic-sdk-0.1.8/sumologic_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 duc        (501) staff       (20)      408 2018-09-15 07:12:08.000000 sumologic-sdk-0.1.8/sumologic_sdk.egg-info/PKG-INFO
--rw-r--r--   0 duc        (501) staff       (20)       16 2018-09-15 07:12:08.000000 sumologic-sdk-0.1.8/sumologic_sdk.egg-info/requires.txt
--rw-r--r--   0 duc        (501) staff       (20)      279 2018-09-15 07:12:08.000000 sumologic-sdk-0.1.8/sumologic_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 duc        (501) staff       (20)       10 2018-09-15 07:12:08.000000 sumologic-sdk-0.1.8/sumologic_sdk.egg-info/top_level.txt
--rw-r--r--   0 duc        (501) staff       (20)        1 2018-09-15 07:12:08.000000 sumologic-sdk-0.1.8/sumologic_sdk.egg-info/zip-safe
+drwxr-xr-x   0 hpal       (501) staff       (20)        0 2020-02-20 16:55:18.000000 sumologic-sdk-0.1.9/
+-rw-r--r--   0 hpal       (501) staff       (20)    11323 2019-05-06 06:08:33.000000 sumologic-sdk-0.1.9/LICENSE
+-rw-r--r--   0 hpal       (501) staff       (20)      124 2020-02-20 16:18:14.000000 sumologic-sdk-0.1.9/MANIFEST.in
+-rw-r--r--   0 hpal       (501) staff       (20)     2348 2020-02-20 16:55:18.000000 sumologic-sdk-0.1.9/PKG-INFO
+-rw-r--r--   0 hpal       (501) staff       (20)     1470 2020-02-20 15:49:53.000000 sumologic-sdk-0.1.9/README.md
+-rw-r--r--   0 hpal       (501) staff       (20)        6 2020-02-20 16:53:44.000000 sumologic-sdk-0.1.9/VERSION
+-rw-r--r--   0 hpal       (501) staff       (20)       16 2020-02-20 15:53:06.000000 sumologic-sdk-0.1.9/requirements.txt
+-rw-r--r--   0 hpal       (501) staff       (20)       38 2020-02-20 16:55:18.000000 sumologic-sdk-0.1.9/setup.cfg
+-rw-r--r--   0 hpal       (501) staff       (20)     1080 2020-02-20 15:55:23.000000 sumologic-sdk-0.1.9/setup.py
+drwxr-xr-x   0 hpal       (501) staff       (20)        0 2020-02-20 16:55:18.000000 sumologic-sdk-0.1.9/sumologic/
+-rw-r--r--   0 hpal       (501) staff       (20)      114 2019-05-06 06:08:33.000000 sumologic-sdk-0.1.9/sumologic/__init__.py
+-rw-r--r--   0 hpal       (501) staff       (20)     7222 2020-02-20 15:49:53.000000 sumologic-sdk-0.1.9/sumologic/sumologic.py
+drwxr-xr-x   0 hpal       (501) staff       (20)        0 2020-02-20 16:55:18.000000 sumologic-sdk-0.1.9/sumologic_sdk.egg-info/
+-rw-r--r--   0 hpal       (501) staff       (20)     2348 2020-02-20 16:55:18.000000 sumologic-sdk-0.1.9/sumologic_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 hpal       (501) staff       (20)      324 2020-02-20 16:55:18.000000 sumologic-sdk-0.1.9/sumologic_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 hpal       (501) staff       (20)        1 2020-02-20 16:55:18.000000 sumologic-sdk-0.1.9/sumologic_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 hpal       (501) staff       (20)       16 2020-02-20 16:55:18.000000 sumologic-sdk-0.1.9/sumologic_sdk.egg-info/requires.txt
+-rw-r--r--   0 hpal       (501) staff       (20)       10 2020-02-20 16:55:18.000000 sumologic-sdk-0.1.9/sumologic_sdk.egg-info/top_level.txt
+-rw-r--r--   0 hpal       (501) staff       (20)        1 2020-02-20 15:59:18.000000 sumologic-sdk-0.1.9/sumologic_sdk.egg-info/zip-safe
```

### Comparing `sumologic-sdk-0.1.8/sumologic/sumologic.py` & `sumologic-sdk-0.1.9/sumologic/sumologic.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,28 @@
 try:
     import cookielib
 except ImportError:
     import http.cookiejar as cookielib
 
 class SumoLogic(object):
 
-    def __init__(self, accessId, accessKey, endpoint=None, cookieFile='cookies.txt'):
+    def __init__(self, accessId, accessKey, endpoint=None, caBundle=None, cookieFile='cookies.txt'):
         self.session = requests.Session()
         self.session.auth = (accessId, accessKey)
         self.session.headers = {'content-type': 'application/json', 'accept': 'application/json'}
+        if caBundle is not None:
+            self.session.verify = caBundle
         cj = cookielib.FileCookieJar(cookieFile)
         self.session.cookies = cj
         if endpoint is None:
             self.endpoint = self._get_endpoint()
         else:
             self.endpoint = endpoint
+        if self.endpoint[-1:] == "/":
+          raise Exception("Endpoint should not end with a slash character")
 
     def _get_endpoint(self):
         """
         SumoLogic REST API endpoint changes based on the geo location of the client.
         For example, If the client geolocation is Australia then the REST end point is
         https://api.au.sumologic.com/api/v1
 
@@ -107,15 +111,15 @@
         return self.post('/collectors', collector, headers)
 
     def update_collector(self, collector, etag):
         headers = {'If-Match': etag}
         return self.put('/collectors/' + str(collector['collector']['id']), collector, headers)
 
     def delete_collector(self, collector):
-        return self.delete('/collectors/' + str(collector['id']))
+        return self.delete('/collectors/' + str(collector['collector']['id']))
 
     def sources(self, collector_id, limit=None, offset=None):
         params = {'limit': limit, 'offset': offset}
         r = self.get('/collectors/' + str(collector_id) + '/sources', params)
         return json.loads(r.text)['sources']
 
     def source(self, collector_id, source_id):
@@ -158,7 +162,11 @@
         params = {'query': [{"query":query, "rowId":"A"}],
                   'startTime': millisectimestamp(fromTime),
                   'endTime': millisectimestamp(toTime),
                   'requestedDataPoints': requestedDataPoints,
                   'maxDataPoints': maxDataPoints}
         r = self.post('/metrics/results', params)
         return json.loads(r.text)
+
+    def get_available_builds(self):
+        r = self.get('/collectors/upgrades/targets')
+        return json.loads(r.text)['targets']
```

