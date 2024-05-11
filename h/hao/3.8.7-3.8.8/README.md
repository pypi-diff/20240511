# Comparing `tmp/hao-3.8.7.tar.gz` & `tmp/hao-3.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hao-3.8.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "hao-3.8.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `hao-3.8.7.tar` & `hao-3.8.8.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0    11357 2020-08-14 05:40:38.118171 hao-3.8.7/LICENSE
--rw-r--r--   0        0        0     4550 2024-01-24 03:43:53.608275 hao-3.8.7/README.md
--rw-r--r--   0        0        0      371 2024-04-17 09:52:45.530290 hao-3.8.7/hao/__init__.py
--rw-r--r--   0        0        0     5202 2024-02-08 23:32:22.070927 hao-3.8.7/hao/arango.py
--rw-r--r--   0        0        0     1752 2024-03-21 02:42:14.902996 hao-3.8.7/hao/args.py
--rw-r--r--   0        0        0      456 2021-10-13 03:48:38.248130 hao-3.8.7/hao/asyncs.py
--rw-r--r--   0        0        0     4287 2023-12-12 10:48:58.766747 hao-3.8.7/hao/charsets.py
--rw-r--r--   0        0        0     1886 2024-01-04 06:05:25.811022 hao-3.8.7/hao/cli.py
--rw-r--r--   0        0        0     5539 2024-01-22 09:11:37.678170 hao-3.8.7/hao/config.py
--rw-r--r--   0        0        0     1465 2021-10-13 03:48:38.248130 hao-3.8.7/hao/currencies.py
--rw-r--r--   0        0        0     9092 2024-03-21 01:47:17.438178 hao-3.8.7/hao/dates.py
--rw-r--r--   0        0        0     2450 2023-12-07 02:22:50.584468 hao-3.8.7/hao/db.py
--rw-r--r--   0        0        0     5452 2023-11-21 08:14:53.909683 hao-3.8.7/hao/decorators.py
--rw-r--r--   0        0        0     1513 2023-06-13 10:11:01.543543 hao-3.8.7/hao/dicts.py
--rw-r--r--   0        0        0    55769 2021-10-13 03:48:38.248130 hao-3.8.7/hao/english.py
--rw-r--r--   0        0        0      662 2023-03-27 03:43:21.995697 hao-3.8.7/hao/enums.py
--rw-r--r--   0        0        0     2067 2024-01-19 03:23:22.550873 hao-3.8.7/hao/envs.py
--rw-r--r--   0        0        0    11233 2024-04-17 09:43:38.646299 hao-3.8.7/hao/es.py
--rw-r--r--   0        0        0      190 2021-10-13 03:48:38.248130 hao-3.8.7/hao/exceptions.py
--rw-r--r--   0        0        0      775 2024-03-07 06:56:26.246672 hao-3.8.7/hao/exits.py
--rw-r--r--   0        0        0     3289 2023-04-04 08:33:34.689439 hao-3.8.7/hao/files.py
--rw-r--r--   0        0        0     3557 2024-01-04 07:46:49.520797 hao-3.8.7/hao/hf.py
--rw-r--r--   0        0        0      379 2023-06-29 02:10:36.407201 hao-3.8.7/hao/invoker.py
--rw-r--r--   0        0        0     1782 2023-06-13 10:11:01.543543 hao-3.8.7/hao/jsons.py
--rw-r--r--   0        0        0     4611 2023-12-07 02:22:50.584468 hao-3.8.7/hao/kafka.py
--rw-r--r--   0        0        0     3719 2023-03-27 03:43:21.995697 hao-3.8.7/hao/lists.py
--rw-r--r--   0        0        0     9040 2024-03-20 10:39:59.305419 hao-3.8.7/hao/logs.py
--rw-r--r--   0        0        0     3893 2024-02-09 02:44:21.683818 hao-3.8.7/hao/meters.py
--rw-r--r--   0        0        0     1278 2023-04-25 17:21:24.642589 hao-3.8.7/hao/modules.py
--rw-r--r--   0        0        0     9237 2023-12-07 02:22:50.584468 hao-3.8.7/hao/mongo.py
--rw-r--r--   0        0        0     5466 2024-04-03 14:27:23.635069 hao-3.8.7/hao/mysql.py
--rw-r--r--   0        0        0    10862 2024-03-06 10:18:35.715088 hao-3.8.7/hao/namespaces.py
--rw-r--r--   0        0        0     9785 2021-10-13 03:48:38.248130 hao-3.8.7/hao/nations.py
--rw-r--r--   0        0        0      295 2021-10-13 03:48:38.248130 hao-3.8.7/hao/networks.py
--rw-r--r--   0        0        0    14779 2023-04-04 08:18:53.973078 hao-3.8.7/hao/oss.py
--rw-r--r--   0        0        0     3713 2024-03-06 06:20:59.128480 hao-3.8.7/hao/paths.py
--rw-r--r--   0        0        0     5238 2024-04-03 14:27:23.635069 hao-3.8.7/hao/pg.py
--rw-r--r--   0        0        0   211235 2023-12-13 08:25:09.409744 hao-3.8.7/hao/places.py
--rw-r--r--   0        0        0     8705 2023-12-07 02:22:50.584468 hao-3.8.7/hao/rabbit.py
--rw-r--r--   0        0        0     2441 2023-12-07 02:22:50.584468 hao-3.8.7/hao/redis.py
--rw-r--r--   0        0        0     1383 2023-06-29 05:50:26.598477 hao-3.8.7/hao/regexes.py
--rw-r--r--   0        0        0     6273 2023-06-29 02:10:36.411201 hao-3.8.7/hao/s3.py
--rw-r--r--   0        0        0     1152 2022-06-03 16:02:48.521000 hao-3.8.7/hao/singleton.py
--rw-r--r--   0        0        0     1839 2023-06-13 10:11:01.543543 hao-3.8.7/hao/slacks.py
--rw-r--r--   0        0        0     1914 2024-03-21 01:47:17.438178 hao-3.8.7/hao/spinner.py
--rw-r--r--   0        0        0     3676 2024-03-20 11:19:02.953658 hao-3.8.7/hao/sqlite.py
--rw-r--r--   0        0        0     3079 2024-03-21 01:47:26.214112 hao-3.8.7/hao/stopwatch.py
--rw-r--r--   0        0        0    12052 2024-02-08 23:39:08.139407 hao-3.8.7/hao/strings.py
--rw-r--r--   0        0        0      906 2024-02-09 01:58:02.438476 hao-3.8.7/hao/threads.py
--rw-r--r--   0        0        0     1375 2023-08-03 03:04:54.324235 hao-3.8.7/hao/uuid.py
--rw-r--r--   0        0        0     1441 2023-12-10 10:14:12.527924 hao-3.8.7/hao/versions.py
--rw-r--r--   0        0        0     1095 2024-04-09 10:18:22.444119 hao-3.8.7/hao/vs.py
--rw-r--r--   0        0        0     2243 2024-03-20 08:27:31.296321 hao-3.8.7/pyproject.toml
--rw-r--r--   0        0        0     6293 1970-01-01 00:00:00.000000 hao-3.8.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2020-08-14 05:40:38.118171 hao-3.8.8/LICENSE
+-rw-r--r--   0        0        0     4550 2024-01-24 03:43:53.608275 hao-3.8.8/README.md
+-rw-r--r--   0        0        0      371 2024-05-11 10:40:15.616066 hao-3.8.8/hao/__init__.py
+-rw-r--r--   0        0        0     5202 2024-02-08 23:32:22.070927 hao-3.8.8/hao/arango.py
+-rw-r--r--   0        0        0     1752 2024-03-21 02:42:14.902996 hao-3.8.8/hao/args.py
+-rw-r--r--   0        0        0      456 2021-10-13 03:48:38.248130 hao-3.8.8/hao/asyncs.py
+-rw-r--r--   0        0        0     4287 2023-12-12 10:48:58.766747 hao-3.8.8/hao/charsets.py
+-rw-r--r--   0        0        0     1886 2024-01-04 06:05:25.811022 hao-3.8.8/hao/cli.py
+-rw-r--r--   0        0        0     5539 2024-01-22 09:11:37.678170 hao-3.8.8/hao/config.py
+-rw-r--r--   0        0        0     1465 2021-10-13 03:48:38.248130 hao-3.8.8/hao/currencies.py
+-rw-r--r--   0        0        0     9092 2024-03-21 01:47:17.438178 hao-3.8.8/hao/dates.py
+-rw-r--r--   0        0        0     2450 2023-12-07 02:22:50.584468 hao-3.8.8/hao/db.py
+-rw-r--r--   0        0        0     5452 2023-11-21 08:14:53.909683 hao-3.8.8/hao/decorators.py
+-rw-r--r--   0        0        0     1513 2023-06-13 10:11:01.543543 hao-3.8.8/hao/dicts.py
+-rw-r--r--   0        0        0    55769 2021-10-13 03:48:38.248130 hao-3.8.8/hao/english.py
+-rw-r--r--   0        0        0      662 2023-03-27 03:43:21.995697 hao-3.8.8/hao/enums.py
+-rw-r--r--   0        0        0     2067 2024-01-19 03:23:22.550873 hao-3.8.8/hao/envs.py
+-rw-r--r--   0        0        0    11233 2024-04-17 09:43:38.646299 hao-3.8.8/hao/es.py
+-rw-r--r--   0        0        0      190 2021-10-13 03:48:38.248130 hao-3.8.8/hao/exceptions.py
+-rw-r--r--   0        0        0      775 2024-03-07 06:56:26.246672 hao-3.8.8/hao/exits.py
+-rw-r--r--   0        0        0     3289 2023-04-04 08:33:34.689439 hao-3.8.8/hao/files.py
+-rw-r--r--   0        0        0     3557 2024-01-04 07:46:49.520797 hao-3.8.8/hao/hf.py
+-rw-r--r--   0        0        0      379 2023-06-29 02:10:36.407201 hao-3.8.8/hao/invoker.py
+-rw-r--r--   0        0        0     1782 2023-06-13 10:11:01.543543 hao-3.8.8/hao/jsons.py
+-rw-r--r--   0        0        0     4611 2023-12-07 02:22:50.584468 hao-3.8.8/hao/kafka.py
+-rw-r--r--   0        0        0     3719 2023-03-27 03:43:21.995697 hao-3.8.8/hao/lists.py
+-rw-r--r--   0        0        0     9040 2024-03-20 10:39:59.305419 hao-3.8.8/hao/logs.py
+-rw-r--r--   0        0        0     3896 2024-05-11 10:37:59.737523 hao-3.8.8/hao/meters.py
+-rw-r--r--   0        0        0     1278 2023-04-25 17:21:24.642589 hao-3.8.8/hao/modules.py
+-rw-r--r--   0        0        0     9237 2023-12-07 02:22:50.584468 hao-3.8.8/hao/mongo.py
+-rw-r--r--   0        0        0     5466 2024-04-03 14:27:23.635069 hao-3.8.8/hao/mysql.py
+-rw-r--r--   0        0        0    10862 2024-03-06 10:18:35.715088 hao-3.8.8/hao/namespaces.py
+-rw-r--r--   0        0        0     9785 2021-10-13 03:48:38.248130 hao-3.8.8/hao/nations.py
+-rw-r--r--   0        0        0      295 2024-05-09 06:37:26.761310 hao-3.8.8/hao/networks.py
+-rw-r--r--   0        0        0    14779 2023-04-04 08:18:53.973078 hao-3.8.8/hao/oss.py
+-rw-r--r--   0        0        0     3713 2024-03-06 06:20:59.128480 hao-3.8.8/hao/paths.py
+-rw-r--r--   0        0        0     5238 2024-04-03 14:27:23.635069 hao-3.8.8/hao/pg.py
+-rw-r--r--   0        0        0   211235 2023-12-13 08:25:09.409744 hao-3.8.8/hao/places.py
+-rw-r--r--   0        0        0     8705 2023-12-07 02:22:50.584468 hao-3.8.8/hao/rabbit.py
+-rw-r--r--   0        0        0     2441 2023-12-07 02:22:50.584468 hao-3.8.8/hao/redis.py
+-rw-r--r--   0        0        0     1383 2023-06-29 05:50:26.598477 hao-3.8.8/hao/regexes.py
+-rw-r--r--   0        0        0     6273 2023-06-29 02:10:36.411201 hao-3.8.8/hao/s3.py
+-rw-r--r--   0        0        0     1152 2022-06-03 16:02:48.521000 hao-3.8.8/hao/singleton.py
+-rw-r--r--   0        0        0     1839 2023-06-13 10:11:01.543543 hao-3.8.8/hao/slacks.py
+-rw-r--r--   0        0        0     2736 2024-04-24 04:12:38.869239 hao-3.8.8/hao/spinner.py
+-rw-r--r--   0        0        0     3676 2024-03-20 11:19:02.953658 hao-3.8.8/hao/sqlite.py
+-rw-r--r--   0        0        0     3079 2024-03-21 01:47:26.214112 hao-3.8.8/hao/stopwatch.py
+-rw-r--r--   0        0        0    12052 2024-02-08 23:39:08.139407 hao-3.8.8/hao/strings.py
+-rw-r--r--   0        0        0      906 2024-02-09 01:58:02.438476 hao-3.8.8/hao/threads.py
+-rw-r--r--   0        0        0     1375 2023-08-03 03:04:54.324235 hao-3.8.8/hao/uuid.py
+-rw-r--r--   0        0        0     1441 2023-12-10 10:14:12.527924 hao-3.8.8/hao/versions.py
+-rw-r--r--   0        0        0     1236 2024-05-07 07:39:24.455128 hao-3.8.8/hao/vs.py
+-rw-r--r--   0        0        0     2243 2024-03-20 08:27:31.296321 hao-3.8.8/pyproject.toml
+-rw-r--r--   0        0        0     6293 1970-01-01 00:00:00.000000 hao-3.8.8/PKG-INFO
```

### Comparing `hao-3.8.7/LICENSE` & `hao-3.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/README.md` & `hao-3.8.8/README.md`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/arango.py` & `hao-3.8.8/hao/arango.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/args.py` & `hao-3.8.8/hao/args.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/charsets.py` & `hao-3.8.8/hao/charsets.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/cli.py` & `hao-3.8.8/hao/cli.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/config.py` & `hao-3.8.8/hao/config.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/currencies.py` & `hao-3.8.8/hao/currencies.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/dates.py` & `hao-3.8.8/hao/dates.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/db.py` & `hao-3.8.8/hao/db.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/decorators.py` & `hao-3.8.8/hao/decorators.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/dicts.py` & `hao-3.8.8/hao/dicts.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/english.py` & `hao-3.8.8/hao/english.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/enums.py` & `hao-3.8.8/hao/enums.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/envs.py` & `hao-3.8.8/hao/envs.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/es.py` & `hao-3.8.8/hao/es.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/exits.py` & `hao-3.8.8/hao/exits.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/files.py` & `hao-3.8.8/hao/files.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/hf.py` & `hao-3.8.8/hao/hf.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/jsons.py` & `hao-3.8.8/hao/jsons.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/kafka.py` & `hao-3.8.8/hao/kafka.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/lists.py` & `hao-3.8.8/hao/lists.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/logs.py` & `hao-3.8.8/hao/logs.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/meters.py` & `hao-3.8.8/hao/meters.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,28 +54,27 @@
         self.prometheus_gateway = config.get('prometheus.gateway')
         self.prometheus_key = config.get('prometheus.key')
 
     def start(self):
         if self._reporter.is_alive():
             return self
         self.reset()
-        # self._reporter.start()
+        self._reporter.start()
         return self
 
     def stop(self):
         if self._reporter.is_alive():
             self._reporter.stop()
 
     def reset(self):
         self._meters: DefaultDict[str, SimpleCounter] = collections.defaultdict(SimpleCounter)
         self._n_cycle = 0
 
     def on_exit(self):
         for key in self._meters:
-            self._logger.info(f"[meter-{key}] removing from prometheus")
             self._remove_from_prometheus(key)
 
     def mark(self, key):
         self._meters[key].increment()
 
     def register_gauge(self, key, gauge: Callable, overwrite=True):
         if not overwrite and key in self._gauges:
@@ -114,12 +113,13 @@
             try:
                 requests.put(url, data=data, timeout=5)
             except Exception as e:
                 LOGGER.info(e)
 
     def _remove_from_prometheus(self, job_name):
         if self.prometheus_gateway and self.prometheus_key:
+            self._logger.info(f"[meter-{job_name}] removing from prometheus")
             url = f"{self.prometheus_gateway}/metrics/job/{job_name}/instance/{config.HOSTNAME}"
             try:
                 requests.delete(url, timeout=5)
             except Exception as e:
                 LOGGER.info(e)
```

### Comparing `hao-3.8.7/hao/modules.py` & `hao-3.8.8/hao/modules.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/mongo.py` & `hao-3.8.8/hao/mongo.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/mysql.py` & `hao-3.8.8/hao/mysql.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/namespaces.py` & `hao-3.8.8/hao/namespaces.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/nations.py` & `hao-3.8.8/hao/nations.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/oss.py` & `hao-3.8.8/hao/oss.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/paths.py` & `hao-3.8.8/hao/paths.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/pg.py` & `hao-3.8.8/hao/pg.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/places.py` & `hao-3.8.8/hao/places.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/rabbit.py` & `hao-3.8.8/hao/rabbit.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/redis.py` & `hao-3.8.8/hao/redis.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/regexes.py` & `hao-3.8.8/hao/regexes.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/s3.py` & `hao-3.8.8/hao/s3.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/singleton.py` & `hao-3.8.8/hao/singleton.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/slacks.py` & `hao-3.8.8/hao/slacks.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/spinner.py` & `hao-3.8.8/hao/spinner.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,45 +5,69 @@
 from .dates import pretty_time_delta
 
 
 class Spinner(threading.Thread):
 
     LINE_CLEAR = '\x1b[2K'
     FRAMES = [
-        '|\\_________',
-        '_|\\________',
-        '__|\\_______',
-        '___|\\______',
-        '____|\\_____',
-        '_____|\\____',
-        '______|\\___',
-        '_______|\\__',
-        '________|\\_',
-        '_________|\\',
-        '_________/|',
-        '________/|_',
-        '_______/|__',
-        '______/|___',
-        '_____/|____',
-        '____/|_____',
-        '___/|______',
-        '__/|_______',
-        '_/|________',
-        '/|_________',
+        '_________________',
+        '\\________________',
+        '|\\_______________',
+        '_|\\______________',
+        '__|\\_____________',
+        '___|\\____________',
+        '____|\\___________',
+        '_____|\\__________',
+        '______|\\_________',
+        '_______|\\________',
+        '________|\\_______',
+        '_________|\\______',
+        '__________|\\_____',
+        '___________|\\____',
+        '____________|\\___',
+        '_____________|\\__',
+        '______________|\\_',
+        '_______________|\\',
+        '________________|',
+        '_________________',
+        '_________________',
+        '________________/',
+        '_______________/|',
+        '______________/|_',
+        '_____________/|__',
+        '____________/|___',
+        '___________/|____',
+        '__________/|_____',
+        '_________/|______',
+        '________/|_______',
+        '_______/|________',
+        '______/|_________',
+        '_____/|__________',
+        '____/|___________',
+        '___/|____________',
+        '__/|_____________',
+        '_/|______________',
+        '/|_______________',
+        '|________________',
+        '_________________',
     ]
 
     def __init__(self, msg: str, *, ps='>', done: str = '✔️', interval=0.1, frames: Optional[List[str]] = None):
         super().__init__()
         self.msg = msg
         self.ps = ps
         self.done = done
         self.interval = interval
         self.frames = frames or self.FRAMES
         self.status = threading.Event()
         self.daemon = True
+        self._start = None
+
+    def elapes(self):
+        return pretty_time_delta(int(time.time()) - self._start, millis=False) if self._start else '-'
 
     def stop(self):
         self.status.set()
 
     def is_stopped(self):
         return self.status.is_set()
 
@@ -52,19 +76,19 @@
             for cursor in self.frames:
                 yield cursor
 
     def write(self, text):
         print(f"{self.LINE_CLEAR}\r{self.ps} {text}", flush=True)
 
     def run(self):
-        start = int(time.time())
+        self._start = int(time.time())
         cursors = self.cursors()
         while not self.is_stopped():
             self.status.wait(self.interval)
-            took = pretty_time_delta(int(time.time()) - start, millis=False)
+            took = self.elapes()
             p = f"{self.LINE_CLEAR}\r{self.ps} {self.msg} [{took}] {next(cursors)}"
             print(p, end='', flush=True)
         print(f"{self.done} ", end='\n', flush=True)
 
     def __enter__(self):
         self.start()
         return self
```

### Comparing `hao-3.8.7/hao/sqlite.py` & `hao-3.8.8/hao/sqlite.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/stopwatch.py` & `hao-3.8.8/hao/stopwatch.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/strings.py` & `hao-3.8.8/hao/strings.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/threads.py` & `hao-3.8.8/hao/threads.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/uuid.py` & `hao-3.8.8/hao/uuid.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/versions.py` & `hao-3.8.8/hao/versions.py`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/hao/vs.py` & `hao-3.8.8/hao/vs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 # -*- coding: utf-8 -*-
-import json
+import ast
 import logging
 import os
 import sys
 
 from . import jsons, paths
 
 LOGGER = logging.getLogger(__name__)
 
 
 def run():
     argv = sys.argv
     n_args = len(argv)
     if n_args == 1:
-        print('Usage: h-code {module.name}')
+        print('Usage: h-vs {module.name}')
         return
 
     try:
         module_name = argv[-1]
         path_launch_json = paths.get('.vscode/launch.json')
         if not os.path.exists(path_launch_json):
             data = {'version': '0.2.0', 'configurations': []}
             paths.make_parent_dirs(path_launch_json)
         else:
             with open(path_launch_json) as f:
-                data = json.load(f)
+                text = f.read()
+                text = text.replace('null', 'None').replace('true', 'True').replace('false', 'False')
+                data = ast.literal_eval(text)
         data.get('configurations').append({
             "name": module_name,
             "type": "debugpy",
             "request": "launch",
             "program": "-m",
             "env": {},
             "console": "integratedTerminal",
```

### Comparing `hao-3.8.7/pyproject.toml` & `hao-3.8.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hao-3.8.7/PKG-INFO` & `hao-3.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hao
-Version: 3.8.7
+Version: 3.8.8
 Summary: conf, logs, namespace, etc
 Home-page: https://github.com/orctom/hao
 License: Apache-2.0
 Author: orctom
 Author-email: orctom <orctom@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

