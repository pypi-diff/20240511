# Comparing `tmp/lambkid-0.1.9.tar.gz` & `tmp/lambkid-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambkid-0.1.9.tar", last modified: Tue Apr  9 07:47:44 2024, max compression
+gzip compressed data, was "lambkid-0.2.0.tar", last modified: Sat May 11 14:14:15 2024, max compression
```

## Comparing `lambkid-0.1.9.tar` & `lambkid-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 07:47:44.224520 lambkid-0.1.9/
--rw-rw-rw-   0        0        0     1089 2024-03-27 01:13:02.000000 lambkid-0.1.9/LICENSE
--rw-rw-rw-   0        0        0       27 2024-04-01 08:22:25.000000 lambkid-0.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0     2005 2024-04-09 07:47:44.223548 lambkid-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0      628 2024-04-09 07:16:28.000000 lambkid-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 07:47:44.169695 lambkid-0.1.9/docs/
--rw-rw-rw-   0        0        0      371 2024-04-08 03:30:43.000000 lambkid-0.1.9/docs/cli.md
--rw-rw-rw-   0        0        0       54 2024-03-31 06:58:42.000000 lambkid-0.1.9/docs/install.md
--rw-rw-rw-   0        0        0      778 2024-04-07 15:20:10.000000 lambkid-0.1.9/docs/log.md
--rw-rw-rw-   0        0        0     1878 2024-04-01 07:39:19.000000 lambkid-0.1.9/docs/sshclient.md
-drwxrwxrwx   0        0        0        0 2024-04-09 07:47:44.177646 lambkid-0.1.9/lambkid/
--rw-rw-rw-   0        0        0      113 2024-04-01 07:23:01.000000 lambkid-0.1.9/lambkid/__init__.py
--rw-rw-rw-   0        0        0      969 2024-04-08 15:55:58.000000 lambkid-0.1.9/lambkid/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-09 07:47:44.220531 lambkid-0.1.9/lambkid/libs/
--rw-rw-rw-   0        0        0        0 2024-03-31 06:59:08.000000 lambkid-0.1.9/lambkid/libs/__init__.py
--rw-rw-rw-   0        0        0     1406 2024-04-07 15:19:33.000000 lambkid-0.1.9/lambkid/libs/log.py
--rw-rw-rw-   0        0        0      825 2024-04-08 02:45:19.000000 lambkid-0.1.9/lambkid/libs/minio_client.py
--rw-rw-rw-   0        0        0     6889 2024-04-09 07:46:29.000000 lambkid-0.1.9/lambkid/libs/ssh.py
-drwxrwxrwx   0        0        0        0 2024-04-09 07:47:44.222526 lambkid-0.1.9/lambkid.egg-info/
--rw-rw-rw-   0        0        0     2005 2024-04-09 07:47:44.000000 lambkid-0.1.9/lambkid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-04-09 07:47:44.000000 lambkid-0.1.9/lambkid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 07:47:44.000000 lambkid-0.1.9/lambkid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-04-09 07:47:44.000000 lambkid-0.1.9/lambkid.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2024-04-09 07:47:44.000000 lambkid-0.1.9/lambkid.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-09 07:47:44.000000 lambkid-0.1.9/lambkid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 07:47:44.225518 lambkid-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1845 2024-04-09 07:46:55.000000 lambkid-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 14:14:15.076256 lambkid-0.2.0/
+-rw-rw-rw-   0        0        0     1089 2024-03-27 01:13:02.000000 lambkid-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0       27 2024-04-01 08:22:25.000000 lambkid-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2094 2024-05-11 14:14:15.075258 lambkid-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      717 2024-04-24 02:44:24.000000 lambkid-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 14:14:14.971051 lambkid-0.2.0/docs/
+-rw-rw-rw-   0        0        0      371 2024-04-08 03:30:43.000000 lambkid-0.2.0/docs/cli.md
+-rw-rw-rw-   0        0        0      221 2024-04-24 02:42:57.000000 lambkid-0.2.0/docs/csv.md
+-rw-rw-rw-   0        0        0       54 2024-03-31 06:58:42.000000 lambkid-0.2.0/docs/install.md
+-rw-rw-rw-   0        0        0      778 2024-04-07 15:20:10.000000 lambkid-0.2.0/docs/log.md
+-rw-rw-rw-   0        0        0     1878 2024-04-01 07:39:19.000000 lambkid-0.2.0/docs/sshclient.md
+-rw-rw-rw-   0        0        0       36 2024-04-25 02:05:46.000000 lambkid-0.2.0/docs/utils.md
+drwxrwxrwx   0        0        0        0 2024-05-11 14:14:14.973017 lambkid-0.2.0/lambkid/
+-rw-rw-rw-   0        0        0      188 2024-04-25 02:53:27.000000 lambkid-0.2.0/lambkid/__init__.py
+-rw-rw-rw-   0        0        0      969 2024-04-08 15:55:58.000000 lambkid-0.2.0/lambkid/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-11 14:14:15.054339 lambkid-0.2.0/lambkid/libs/
+-rw-rw-rw-   0        0        0        0 2024-03-31 06:59:08.000000 lambkid-0.2.0/lambkid/libs/__init__.py
+-rw-rw-rw-   0        0        0     1514 2024-04-29 07:44:19.000000 lambkid-0.2.0/lambkid/libs/log.py
+-rw-rw-rw-   0        0        0      825 2024-04-08 02:45:19.000000 lambkid-0.2.0/lambkid/libs/minio_client.py
+-rw-rw-rw-   0        0        0     7344 2024-05-11 14:13:31.000000 lambkid-0.2.0/lambkid/libs/ssh.py
+-rw-rw-rw-   0        0        0     2259 2024-04-28 05:47:19.000000 lambkid-0.2.0/lambkid/libs/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-11 14:14:15.074261 lambkid-0.2.0/lambkid.egg-info/
+-rw-rw-rw-   0        0        0     2094 2024-05-11 14:14:14.000000 lambkid-0.2.0/lambkid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      461 2024-05-11 14:14:14.000000 lambkid-0.2.0/lambkid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 14:14:14.000000 lambkid-0.2.0/lambkid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-11 14:14:14.000000 lambkid-0.2.0/lambkid.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       43 2024-05-11 14:14:14.000000 lambkid-0.2.0/lambkid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-11 14:14:14.000000 lambkid-0.2.0/lambkid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-11 14:14:15.076256 lambkid-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1834 2024-05-11 14:13:43.000000 lambkid-0.2.0/setup.py
```

### Comparing `lambkid-0.1.9/LICENSE` & `lambkid-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.9/PKG-INFO` & `lambkid-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambkid
-Version: 0.1.9
+Version: 0.2.0
 Summary: lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.
 Home-page: https://github.com/redrose2100/lambkid
 Author: redrose2100
 Author-email: hitredrose@163.com
 Maintainer: redrose2100
 Maintainer-email: hitredrose@163.com
 License: MIT
@@ -36,10 +36,11 @@
 lambkid is an advance lib abstract from some common use python lib. it aim to supply a more easily and more fewer code for python developer.
 it will practise for life is short and I will choose python.
 
 ## install lambkid
 refer to [install lambkid](https://github.com/redrose2100/lambkid/blob/master/docs/install.md)
 
 ## function of lambkid
+* [csv usage](https://github.com/redrose2100/lambkid/blob/master/docs/csv.md)(>=0.1.18)
 * [sshclient](https://github.com/redrose2100/lambkid/blob/master/docs/sshclient.md)(>=0.0.6)
 * [log](https://github.com/redrose2100/lambkid/blob/master/docs/log.md) (>=0.0.4)
 * [cli command](https://github.com/redrose2100/lambkid/blob/master/docs/cli.md)(>=0.1.8)
```

### Comparing `lambkid-0.1.9/README.md` & `lambkid-0.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -3,10 +3,11 @@
 lambkid is an advance lib abstract from some common use python lib. it aim to supply a more easily and more fewer code for python developer.
 it will practise for life is short and I will choose python.
 
 ## install lambkid
 refer to [install lambkid](https://github.com/redrose2100/lambkid/blob/master/docs/install.md)
 
 ## function of lambkid
+* [csv usage](https://github.com/redrose2100/lambkid/blob/master/docs/csv.md)(>=0.1.18)
 * [sshclient](https://github.com/redrose2100/lambkid/blob/master/docs/sshclient.md)(>=0.0.6)
 * [log](https://github.com/redrose2100/lambkid/blob/master/docs/log.md) (>=0.0.4)
 * [cli command](https://github.com/redrose2100/lambkid/blob/master/docs/cli.md)(>=0.1.8)
```

### Comparing `lambkid-0.1.9/docs/log.md` & `lambkid-0.2.0/docs/log.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.9/docs/sshclient.md` & `lambkid-0.2.0/docs/sshclient.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.9/lambkid/cli.py` & `lambkid-0.2.0/lambkid/cli.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.9/lambkid/libs/log.py` & `lambkid-0.2.0/lambkid/libs/log.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,32 +2,34 @@
 import logging
 import platform
 from pathlib import Path
 from datetime import datetime
 from concurrent_log_handler import ConcurrentRotatingFileHandler
 
 
-def get_logger(name, level=logging.INFO, log_path=None):
+def get_logger(name, level=logging.INFO, log_path=None,open_console=True):
     sys_name = platform.system()
     timestamp = datetime.now().strftime("%Y%m%d")
     if not log_path:
         if sys_name == "Linux":
             os.system(f"mkdir -p /var/log/{name}")
             log_path = f"/var/log/{name}/lambkid_{timestamp}.log"
         else:
             log_path = Path(__file__).parent / f"lambkid_{timestamp}.log"
-    handler = ConcurrentRotatingFileHandler(log_path, "a", 512 * 1024, 30)
+    handler = ConcurrentRotatingFileHandler(log_path, "a", 1024 * 1024 * 1024, 200)
     handler.setFormatter(logging.Formatter('%(asctime)s | %(levelname)s | %(filename)s:%(lineno)s | %(message)s'))
-    console_handler = logging.StreamHandler()
-    console_handler.setLevel(logging.INFO)
-    console_handler.setFormatter(logging.Formatter('%(asctime)s | %(levelname)s | %(filename)s:%(lineno)s | %(message)s'))
+    handler.setLevel(logging.INFO)
     logger = logging.getLogger(name)
-    logger.addHandler(console_handler)
+    if open_console:
+        console_handler = logging.StreamHandler()
+        console_handler.setLevel(logging.INFO)
+        console_handler.setFormatter(logging.Formatter('%(asctime)s | %(levelname)s | %(filename)s:%(lineno)s | %(message)s'))
+        logger.addHandler(console_handler)
     logger.addHandler(handler)
-    logger.setLevel(level)
+    logger.setLevel(logging.INFO)
     logger.propagate = False
     return logger
 
 
 log = get_logger("lambkid")
 
 if __name__ == "__main__":
```

### Comparing `lambkid-0.1.9/lambkid/libs/minio_client.py` & `lambkid-0.2.0/lambkid/libs/minio_client.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.9/lambkid/libs/ssh.py` & `lambkid-0.2.0/lambkid/libs/ssh.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import re
 import time
 import paramiko
 from lambkid import log
+import concurrent.futures
 
 
 class ExecResult(object):
     def __init__(self, output, exit_status_code):
         self.__stdout = output
         self.__exit_status_code = exit_status_code
 
@@ -41,33 +42,45 @@
         return self.__ip
 
     @property
     def port(self):
         return self.__port
 
     def wait_for_sshable(self, timeout=600):
-        count = 0
+        count=0
         while True:
-            count += 1
-            if count > (int(timeout / 10)):
-                log.error(f" {self.__ip}:{self.__port} | server {self.__ip} ssh timeout {timeout}s: Error.")
+            count+=1
+            if count>(timeout/10):
+                log.error(
+                    f" {self.__ip}:{self.__port} | server {self.__ip} can not ssh: Error. err msg is in time {timeout} server cannot ssh.")
                 return False
             try:
                 if self.__connect():
                     log.info(f" {self.__ip}:{self.__port} | server {self.__ip} can ssh: OK.")
                     return True
             except Exception as e:
-                log.warning(f" {self.__ip}:{self.__port} | server {self.__ip} can not ssh: Error. err msg is {str(e)}")
-                time.sleep(10)
+                log.warning(
+                    f" {self.__ip}:{self.__port} | server {self.__ip} can not ssh: Error. err msg is {str(e)}")
+            time.sleep(10)
+
 
-    def exec(self, cmd, timeout=600):
+    def exec(self, cmd, timeout=600,max_attempts=1):
         log.info(f" {self.__ip}:{self.__port} | begin to run cmd {cmd}, timeout is {timeout}...")
         try:
-            if not self.__is_active():
-                self.__reconnect()
+            try_times=0
+            while True:
+                try_times+=1
+                if try_times>(timeout/10):
+                    raise RuntimeError(f"after {timeout} seconds try, ssh is still not sshable.")
+                if not self.__is_active():
+                    self.__reconnect()
+                    time.sleep(10)
+                    continue
+                else:
+                    break
             stdin, stdout, stderr = self.__ssh.exec_command(cmd, timeout=timeout)
             exit_status_code = stdout.channel.recv_exit_status()
             output = stdout.read().decode("utf-8")
             if exit_status_code == 0:
                 log.info(f" {self.__ip}:{self.__port} | successful to run cmd {cmd}, output is {output}")
             else:
                 log.warning(
```

### Comparing `lambkid-0.1.9/lambkid.egg-info/PKG-INFO` & `lambkid-0.2.0/lambkid.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambkid
-Version: 0.1.9
+Version: 0.2.0
 Summary: lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.
 Home-page: https://github.com/redrose2100/lambkid
 Author: redrose2100
 Author-email: hitredrose@163.com
 Maintainer: redrose2100
 Maintainer-email: hitredrose@163.com
 License: MIT
@@ -36,10 +36,11 @@
 lambkid is an advance lib abstract from some common use python lib. it aim to supply a more easily and more fewer code for python developer.
 it will practise for life is short and I will choose python.
 
 ## install lambkid
 refer to [install lambkid](https://github.com/redrose2100/lambkid/blob/master/docs/install.md)
 
 ## function of lambkid
+* [csv usage](https://github.com/redrose2100/lambkid/blob/master/docs/csv.md)(>=0.1.18)
 * [sshclient](https://github.com/redrose2100/lambkid/blob/master/docs/sshclient.md)(>=0.0.6)
 * [log](https://github.com/redrose2100/lambkid/blob/master/docs/log.md) (>=0.0.4)
 * [cli command](https://github.com/redrose2100/lambkid/blob/master/docs/cli.md)(>=0.1.8)
```

### Comparing `lambkid-0.1.9/setup.py` & `lambkid-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-import os
 from setuptools import setup, find_packages
 
 
 try:
     with open("README.md",encoding="utf-8",mode="r") as f:
         long_desc=f.read()
 except:
     long_desc=""
 
 
 setup(
     name="lambkid",
-    version="0.1.9",
+    version="0.2.0",
     description="lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.",
     long_description=long_desc,
     long_description_content_type="text/markdown",
     author="redrose2100",
     author_email="hitredrose@163.com",
     maintainer="redrose2100",
     maintainer_email="hitredrose@163.com",
```

