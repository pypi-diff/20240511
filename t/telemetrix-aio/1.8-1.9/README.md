# Comparing `tmp/telemetrix-aio-1.8.tar.gz` & `tmp/telemetrix-aio-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telemetrix-aio-1.8.tar", last modified: Sun Oct 24 13:54:27 2021, max compression
+gzip compressed data, was "telemetrix-aio-1.9.tar", last modified: Mon Nov 29 16:31:34 2021, max compression
```

## Comparing `telemetrix-aio-1.8.tar` & `telemetrix-aio-1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2021-10-24 13:54:27.214129 telemetrix-aio-1.8/
--rw-rw-r--   0 afy       (1000) afy       (1000)       21 2020-11-09 15:43:28.000000 telemetrix-aio-1.8/MANIFEST.in
--rw-rw-r--   0 afy       (1000) afy       (1000)     2380 2021-10-24 13:54:27.214129 telemetrix-aio-1.8/PKG-INFO
--rw-rw-r--   0 afy       (1000) afy       (1000)     1473 2021-08-14 20:25:58.000000 telemetrix-aio-1.8/README.md
--rw-rw-r--   0 afy       (1000) afy       (1000)      964 2020-11-09 15:58:02.000000 telemetrix-aio-1.8/pypi_desc.md
--rw-rw-r--   0 afy       (1000) afy       (1000)       38 2021-10-24 13:54:27.214129 telemetrix-aio-1.8/setup.cfg
--rw-rw-r--   0 afy       (1000) afy       (1000)     1165 2021-10-20 19:32:18.000000 telemetrix-aio-1.8/setup.py
-drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2021-10-24 13:54:27.214129 telemetrix-aio-1.8/telemetrix_aio/
--rw-rw-r--   0 afy       (1000) afy       (1000)        0 2020-10-21 20:12:31.000000 telemetrix-aio-1.8/telemetrix_aio/__init__.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     3042 2021-10-20 19:32:18.000000 telemetrix-aio-1.8/telemetrix_aio/private_constants.py
--rw-rw-r--   0 afy       (1000) afy       (1000)    54686 2021-10-23 22:44:43.000000 telemetrix-aio-1.8/telemetrix_aio/telemetrix_aio.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     2480 2021-05-12 14:25:03.000000 telemetrix-aio-1.8/telemetrix_aio/telemetrix_aio_socket.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     7424 2020-10-23 23:11:33.000000 telemetrix-aio-1.8/telemetrix_aio/telemtrix_aio_serial.py
-drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2021-10-24 13:54:27.214129 telemetrix-aio-1.8/telemetrix_aio.egg-info/
--rw-rw-r--   0 afy       (1000) afy       (1000)     2380 2021-10-24 13:54:27.000000 telemetrix-aio-1.8/telemetrix_aio.egg-info/PKG-INFO
--rw-rw-r--   0 afy       (1000) afy       (1000)      407 2021-10-24 13:54:27.000000 telemetrix-aio-1.8/telemetrix_aio.egg-info/SOURCES.txt
--rw-rw-r--   0 afy       (1000) afy       (1000)        1 2021-10-24 13:54:27.000000 telemetrix-aio-1.8/telemetrix_aio.egg-info/dependency_links.txt
--rw-rw-r--   0 afy       (1000) afy       (1000)        9 2021-10-24 13:54:27.000000 telemetrix-aio-1.8/telemetrix_aio.egg-info/requires.txt
--rw-rw-r--   0 afy       (1000) afy       (1000)       15 2021-10-24 13:54:27.000000 telemetrix-aio-1.8/telemetrix_aio.egg-info/top_level.txt
+drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2021-11-29 16:31:34.973179 telemetrix-aio-1.9/
+-rw-rw-r--   0 afy       (1000) afy       (1000)       21 2020-11-09 15:43:28.000000 telemetrix-aio-1.9/MANIFEST.in
+-rw-rw-r--   0 afy       (1000) afy       (1000)     3018 2021-11-29 16:31:34.973179 telemetrix-aio-1.9/PKG-INFO
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2111 2021-11-29 16:23:33.000000 telemetrix-aio-1.9/README.md
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2111 2021-11-29 16:24:12.000000 telemetrix-aio-1.9/pypi_desc.md
+-rw-rw-r--   0 afy       (1000) afy       (1000)       38 2021-11-29 16:31:34.973179 telemetrix-aio-1.9/setup.cfg
+-rw-rw-r--   0 afy       (1000) afy       (1000)     1165 2021-11-29 16:15:32.000000 telemetrix-aio-1.9/setup.py
+drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2021-11-29 16:31:34.973179 telemetrix-aio-1.9/telemetrix_aio/
+-rw-rw-r--   0 afy       (1000) afy       (1000)        0 2020-10-21 20:12:31.000000 telemetrix-aio-1.9/telemetrix_aio/__init__.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     4084 2021-11-29 16:15:32.000000 telemetrix-aio-1.9/telemetrix_aio/private_constants.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)    87489 2021-11-17 15:20:01.000000 telemetrix-aio-1.9/telemetrix_aio/telemetrix_aio.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2480 2021-05-12 14:25:03.000000 telemetrix-aio-1.9/telemetrix_aio/telemetrix_aio_socket.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     7424 2020-10-23 23:11:33.000000 telemetrix-aio-1.9/telemetrix_aio/telemtrix_aio_serial.py
+drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2021-11-29 16:31:34.973179 telemetrix-aio-1.9/telemetrix_aio.egg-info/
+-rw-rw-r--   0 afy       (1000) afy       (1000)     3018 2021-11-29 16:31:34.000000 telemetrix-aio-1.9/telemetrix_aio.egg-info/PKG-INFO
+-rw-rw-r--   0 afy       (1000) afy       (1000)      407 2021-11-29 16:31:34.000000 telemetrix-aio-1.9/telemetrix_aio.egg-info/SOURCES.txt
+-rw-rw-r--   0 afy       (1000) afy       (1000)        1 2021-11-29 16:31:34.000000 telemetrix-aio-1.9/telemetrix_aio.egg-info/dependency_links.txt
+-rw-rw-r--   0 afy       (1000) afy       (1000)        9 2021-11-29 16:31:34.000000 telemetrix-aio-1.9/telemetrix_aio.egg-info/requires.txt
+-rw-rw-r--   0 afy       (1000) afy       (1000)       15 2021-11-29 16:31:34.000000 telemetrix-aio-1.9/telemetrix_aio.egg-info/top_level.txt
```

### Comparing `telemetrix-aio-1.8/setup.py` & `telemetrix-aio-1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = f.read()
 
 setup(
     name='telemetrix-aio',
     packages=['telemetrix_aio'],
     install_requires=['pyserial'],
 
-    version='1.8',
+    version='1.9',
     description="Remotely Control And Monitor Arduino-Core devices",
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     author='Alan Yorinks',
     author_email='MisterYsLab@gmail.com',
     url='https://github.com/MrYsLab/telemetrix-aio',
```

### Comparing `telemetrix-aio-1.8/telemetrix_aio/telemetrix_aio_socket.py` & `telemetrix-aio-1.9/telemetrix_aio/telemetrix_aio_socket.py`

 * *Files identical despite different names*

### Comparing `telemetrix-aio-1.8/telemetrix_aio/telemtrix_aio_serial.py` & `telemetrix-aio-1.9/telemetrix_aio/telemtrix_aio_serial.py`

 * *Files identical despite different names*

