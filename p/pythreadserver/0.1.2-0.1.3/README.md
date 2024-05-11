# Comparing `tmp/pythreadserver-0.1.2.tar.gz` & `tmp/pythreadserver-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythreadserver-0.1.2.tar", last modified: Fri Apr  5 22:06:48 2024, max compression
+gzip compressed data, was "pythreadserver-0.1.3.tar", last modified: Sat May 11 10:58:44 2024, max compression
```

## Comparing `pythreadserver-0.1.2.tar` & `pythreadserver-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 22:06:48.848094 pythreadserver-0.1.2/
--rw-rw-rw-   0        0        0      524 2024-04-05 22:06:48.848094 pythreadserver-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      186 2024-04-05 13:30:40.000000 pythreadserver-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 22:06:48.836091 pythreadserver-0.1.2/pythreadserver/
--rw-rw-rw-   0        0        0       58 2024-04-05 22:06:46.000000 pythreadserver-0.1.2/pythreadserver/__init__.py
--rw-rw-rw-   0        0        0     3407 2024-04-05 20:40:27.000000 pythreadserver-0.1.2/pythreadserver/client.py
--rw-rw-rw-   0        0        0      141 2024-04-05 20:52:10.000000 pythreadserver-0.1.2/pythreadserver/constants.py
--rw-rw-rw-   0        0        0     5035 2024-04-05 21:06:34.000000 pythreadserver-0.1.2/pythreadserver/server.py
--rw-rw-rw-   0        0        0      465 2024-04-05 13:30:40.000000 pythreadserver-0.1.2/pythreadserver/textlog.py
-drwxrwxrwx   0        0        0        0 2024-04-05 22:06:48.846093 pythreadserver-0.1.2/pythreadserver.egg-info/
--rw-rw-rw-   0        0        0      524 2024-04-05 22:06:48.000000 pythreadserver-0.1.2/pythreadserver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      301 2024-04-05 22:06:48.000000 pythreadserver-0.1.2/pythreadserver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 22:06:48.000000 pythreadserver-0.1.2/pythreadserver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-05 22:06:48.000000 pythreadserver-0.1.2/pythreadserver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 22:06:48.848094 pythreadserver-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      996 2024-04-05 22:06:46.000000 pythreadserver-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 10:58:44.634315 pythreadserver-0.1.3/
+-rw-rw-rw-   0        0        0      512 2024-05-11 10:58:44.634315 pythreadserver-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2024-05-11 10:23:05.000000 pythreadserver-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 10:58:44.618297 pythreadserver-0.1.3/pythreadserver/
+-rw-rw-rw-   0        0        0       60 2024-05-11 10:43:35.000000 pythreadserver-0.1.3/pythreadserver/__init__.py
+-rw-rw-rw-   0        0        0     3371 2024-05-11 10:43:35.000000 pythreadserver-0.1.3/pythreadserver/client.py
+-rw-rw-rw-   0        0        0      115 2024-05-11 10:43:35.000000 pythreadserver-0.1.3/pythreadserver/constants.py
+-rw-rw-rw-   0        0        0     4995 2024-05-11 10:43:35.000000 pythreadserver-0.1.3/pythreadserver/server.py
+-rw-rw-rw-   0        0        0      561 2024-05-11 10:43:35.000000 pythreadserver-0.1.3/pythreadserver/textlog.py
+drwxrwxrwx   0        0        0        0 2024-05-11 10:58:44.633315 pythreadserver-0.1.3/pythreadserver.egg-info/
+-rw-rw-rw-   0        0        0      512 2024-05-11 10:58:44.000000 pythreadserver-0.1.3/pythreadserver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2024-05-11 10:58:44.000000 pythreadserver-0.1.3/pythreadserver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 10:58:44.000000 pythreadserver-0.1.3/pythreadserver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-11 10:58:44.000000 pythreadserver-0.1.3/pythreadserver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-11 10:58:44.634315 pythreadserver-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      781 2024-05-11 10:57:35.000000 pythreadserver-0.1.3/setup.py
```

### Comparing `pythreadserver-0.1.2/pythreadserver/client.py` & `pythreadserver-0.1.3/pythreadserver/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,29 +2,36 @@
 import threading
 import time
 from .textlog import Log
 from .constants import *
 
 
 class Client:
-    def __init__(self, ip, output_to_console=False):
+    def __init__(self, ip, **kwargs):
+        output_to_console = True
+        log_path = ""
+        if "console" in kwargs:
+            output_to_console = kwargs["console"]
+        if "log_path" in kwargs:
+            log_path = kwargs["log_path"]
+
         self.ip = ip
         if self.ip == "" or self.ip == "localhost":
             self.ip = socket.gethostname()
-        self.runtime = time.time()
         self.__listeners = []
         self.packets = []
-        self.tick_rate = DEFAULT_TICK_RATE
-        self.log = Log(output_to_console, "pyserver/log/clientlog.txt")
+        self.log = Log(output_to_console, log_path)
         self.socket_out = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.socket_in = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.send_loop_thread = None
         self.recv_loop_thread = None
         self.connected = False
 
+        self.runtime = time.time()
+
     def connect(self):
         self.log.log("Connecting to server...")
         try:
             self.socket_in.connect((self.ip, PORT_S_TO_C))
             self.socket_out.connect((self.ip, PORT_C_TO_S))
         except ConnectionRefusedError:
             self.log.log("Error: Connection refused")
@@ -37,23 +44,19 @@
         self.recv_loop_thread = threading.Thread(target=self.recv_loop)
         self.recv_loop_thread.start()
         self.log.log("Done.")
         return 0
 
     def send_loop(self):
         while self.connected:
-            loop_time = time.time()
             try:
                 self.send_server()
             except (ConnectionResetError, socket.SO_ERROR):
                 self.connected = False
                 break
-            dt = time.time() - loop_time
-            if (1/self.tick_rate) - dt > 0:
-                time.sleep((1 / self.tick_rate) - dt)
 
     def recv_loop(self):
         while self.connected:
             try:
                 self.recv_server()
             except (ConnectionResetError, ConnectionAbortedError):
                 self.close()
```

### Comparing `pythreadserver-0.1.2/pythreadserver/server.py` & `pythreadserver-0.1.3/pythreadserver/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,24 +20,20 @@
         self.send_loop_thread = threading.Thread(target=self.send_loop)
         self.send_loop_thread.start()
         self.recv_loop_thread = threading.Thread(target=self.recv_loop)
         self.recv_loop_thread.start()
 
     def send_loop(self,):
         while self.connected:
-            init = time.time()
             try:
                 self.server.client_send(self)
             except ConnectionResetError:
                 self.connected = False
                 self.close()
                 break
-            dt = time.time() - init
-            if (1/self.server.tick_rate) - dt > 0:
-                time.sleep((1/self.server.tick_rate) - dt)
 
     def recv_loop(self):
         while self.connected:
             try:
                 self.server.client_receive(self)
             except ConnectionResetError:
                 self.connected = False
@@ -55,22 +51,28 @@
             self.server.log.log(f"Connection from {self.addr[0]} closed.")
 
     def send(self, data):
         self.packets.append(data)
 
 
 class Server:
-    def __init__(self, output_to_console=False):
+    def __init__(self, **kwargs):
+        output_to_console = True
+        log_path = ""
+        if "console" in kwargs:
+            output_to_console = kwargs["console"]
+        if "log_path" in kwargs:
+            log_path = kwargs["log_path"]
+
         self.running = True
         self.runtime = time.time()
         self.clients = []
         self.threads = []
         self.__listeners = []
-        self.tick_rate = DEFAULT_TICK_RATE
-        self.log = Log(output_to_console, "pyserver/log/serverlog.txt")
+        self.log = Log(output_to_console, log_path)
 
         self.socket_in = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.socket_out = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         host = ""
         self.log.log("Binding sockets to ports...")
         self.socket_in.bind((host, PORT_C_TO_S))
         self.socket_out.bind((host, PORT_S_TO_C))
```

### Comparing `pythreadserver-0.1.2/setup.py` & `pythreadserver-0.1.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,27 @@
-from setuptools import setup, find_packages
-import codecs
-import os
-
-here = os.path.abspath(os.path.dirname(__file__))
-
-with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
-    long_description = "\n" + fh.read()
-
-VERSION = '0.1.2'
-DESCRIPTION = 'Simple multi-threaded server package'
-LONG_DESCRIPTION = ''
-
-# Setting up
-setup(
-    name="pythreadserver",
-    version=VERSION,
-    author="rain-1107",
-    author_email="",
-    description=DESCRIPTION,
-    long_description_content_type="text/markdown",
-    long_description=LONG_DESCRIPTION,
-    packages=find_packages(),
-    keywords=['python', 'server', 'network', 'multi-threaded', 'sockets'],
-    classifiers=[
-        "Development Status :: 1 - Planning",
-        "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3",
-        "Operating System :: Unix",
-        "Operating System :: MacOS :: MacOS X",
-        "Operating System :: Microsoft :: Windows",
-    ]
-)
+from setuptools import setup, find_packages
+
+VERSION = '0.1.3'
+DESCRIPTION = 'Socket-based server package'
+LONG_DESCRIPTION = ''
+
+# Setting up
+setup(
+    name="pythreadserver",
+    version=VERSION,
+    author="rain1107",
+    author_email="ryanbays@icloud.com",
+    description=DESCRIPTION,
+    long_description_content_type="text/markdown",
+    long_description=LONG_DESCRIPTION,
+    packages=find_packages(),
+    install_requires=[],
+    keywords=['python', 'socket', 'threading'],
+    classifiers=[
+        "Development Status :: 1 - Planning",
+        "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3",
+        "Operating System :: Unix",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: Microsoft :: Windows",
+    ]
+)
```

