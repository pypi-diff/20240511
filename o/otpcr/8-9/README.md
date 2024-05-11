# Comparing `tmp/otpcr-8.tar.gz` & `tmp/otpcr-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otpcr-8.tar", last modified: Sat Apr 27 14:21:51 2024, max compression
+gzip compressed data, was "otpcr-9.tar", last modified: Mon Apr 29 19:56:54 2024, max compression
```

## Comparing `otpcr-8.tar` & `otpcr-9.tar`

### file list

```diff
@@ -1,58 +1,43 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-27 14:21:51.433202 otpcr-8/
--rw-r--r--   0 bart      (1000) bart      (1000)     2496 2024-04-27 14:21:51.433202 otpcr-8/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     1868 2024-04-26 20:04:47.000000 otpcr-8/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-27 14:21:51.425202 otpcr-8/docs/
--rw-r--r--   0 bart      (1000) bart      (1000)     3722 2024-04-27 11:24:31.000000 otpcr-8/docs/MANUAL.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-27 14:21:51.425202 otpcr-8/files/
--rw-r--r--   0 bart      (1000) bart      (1000)   225470 2024-04-26 20:04:47.000000 otpcr-8/files/EM_Ack_OTP-CR-117_19.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)   238330 2024-04-26 20:04:47.000000 otpcr-8/files/EM_T04_OTP-CR-117_19.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)   236671 2024-04-26 20:04:47.000000 otpcr-8/files/EM_T07_OTP-CR-117_19_001.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)  1685507 2024-04-26 20:04:47.000000 otpcr-8/files/bevestigd.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)    50044 2024-04-26 20:04:47.000000 otpcr-8/files/bevestigd.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)    69979 2024-04-26 20:04:47.000000 otpcr-8/files/informed.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)   242205 2024-04-26 20:04:47.000000 otpcr-8/files/verbatim5.png
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-27 14:21:51.429202 otpcr-8/otpcr/
--rw-r--r--   0 bart      (1000) bart      (1000)       53 2024-04-26 20:04:47.000000 otpcr-8/otpcr/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)     4795 2024-04-27 14:14:13.000000 otpcr-8/otpcr/__main__.py
--rw-r--r--   0 bart      (1000) bart      (1000)      704 2024-04-26 22:47:25.000000 otpcr-8/otpcr/broker.py
--rw-r--r--   0 bart      (1000) bart      (1000)     4002 2024-04-26 20:04:47.000000 otpcr-8/otpcr/client.py
--rw-r--r--   0 bart      (1000) bart      (1000)      581 2024-04-27 14:13:19.000000 otpcr-8/otpcr/command.py
--rw-r--r--   0 bart      (1000) bart      (1000)      285 2024-04-26 20:04:47.000000 otpcr-8/otpcr/default.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1397 2024-04-27 12:24:03.000000 otpcr-8/otpcr/errors.py
--rw-r--r--   0 bart      (1000) bart      (1000)      813 2024-04-26 20:04:47.000000 otpcr-8/otpcr/event.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2008 2024-04-26 20:04:47.000000 otpcr-8/otpcr/find.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1405 2024-04-26 20:04:47.000000 otpcr-8/otpcr/handler.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-27 14:21:51.429202 otpcr-8/otpcr/modules/
--rw-r--r--   0 bart      (1000) bart      (1000)      311 2024-04-27 14:15:12.000000 otpcr-8/otpcr/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)      216 2024-04-27 14:12:24.000000 otpcr-8/otpcr/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1000)      344 2024-04-27 12:21:57.000000 otpcr-8/otpcr/modules/err.py
--rw-r--r--   0 bart      (1000) bart      (1000)      372 2024-04-27 11:40:49.000000 otpcr-8/otpcr/modules/flt.py
--rw-r--r--   0 bart      (1000) bart      (1000)      764 2024-04-27 11:41:03.000000 otpcr-8/otpcr/modules/fnd.py
--rw-r--r--   0 bart      (1000) bart      (1000)    18837 2024-04-27 12:41:01.000000 otpcr-8/otpcr/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1000)      706 2024-04-27 11:41:44.000000 otpcr-8/otpcr/modules/log.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3577 2024-04-27 11:42:03.000000 otpcr-8/otpcr/modules/mbx.py
--rw-r--r--   0 bart      (1000) bart      (1000)      183 2024-04-27 11:42:13.000000 otpcr-8/otpcr/modules/mod.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2354 2024-04-27 11:42:25.000000 otpcr-8/otpcr/modules/req.py
--rw-r--r--   0 bart      (1000) bart      (1000)    10834 2024-04-27 14:11:08.000000 otpcr-8/otpcr/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3169 2024-04-26 20:04:47.000000 otpcr-8/otpcr/modules/rst.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1159 2024-04-27 14:11:44.000000 otpcr-8/otpcr/modules/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1000)      988 2024-04-27 11:43:30.000000 otpcr-8/otpcr/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5200 2024-04-27 11:44:01.000000 otpcr-8/otpcr/modules/tmr.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3062 2024-04-27 14:10:56.000000 otpcr-8/otpcr/modules/udp.py
--rw-r--r--   0 bart      (1000) bart      (1000)     6085 2024-04-27 12:21:16.000000 otpcr-8/otpcr/object.py
--rw-r--r--   0 bart      (1000) bart      (1000)      278 2024-04-26 20:04:47.000000 otpcr-8/otpcr/repeater.py
--rw-r--r--   0 bart      (1000) bart      (1000)      161 2024-04-27 12:54:45.000000 otpcr-8/otpcr/runtime.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1956 2024-04-26 20:04:47.000000 otpcr-8/otpcr/thread.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1085 2024-04-26 20:04:47.000000 otpcr-8/otpcr/timer.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1120 2024-04-27 11:55:38.000000 otpcr-8/otpcr/whitelist.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1266 2024-04-27 10:40:11.000000 otpcr-8/otpcr/workdir.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-27 14:21:51.429202 otpcr-8/otpcr.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)     2496 2024-04-27 14:21:51.000000 otpcr-8/otpcr.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     1021 2024-04-27 14:21:51.000000 otpcr-8/otpcr.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-27 14:21:51.000000 otpcr-8/otpcr.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)       49 2024-04-27 14:21:51.000000 otpcr-8/otpcr.egg-info/entry_points.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        6 2024-04-27 14:21:51.000000 otpcr-8/otpcr.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-27 14:21:51.000000 otpcr-8/otpcr.egg-info/zip-safe
--rw-r--r--   0 bart      (1000) bart      (1000)     1197 2024-04-27 14:04:29.000000 otpcr-8/pyproject.toml
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-04-27 14:21:51.433202 otpcr-8/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1000)      148 2024-04-26 20:04:47.000000 otpcr-8/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-04-29 19:56:54.747650 otpcr-9/
+-rw-r--r--   0 bart      (1000) bart      (1001)     2691 2024-04-29 19:56:54.747650 otpcr-9/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)     2026 2024-04-29 19:49:58.000000 otpcr-9/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-04-29 19:56:54.739650 otpcr-9/bin/
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     3715 2024-04-29 19:43:52.000000 otpcr-9/bin/otpcr
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-04-29 19:56:54.743650 otpcr-9/files/
+-rw-r--r--   0 bart      (1000) bart      (1001)   225470 2024-04-29 11:30:06.000000 otpcr-9/files/EM_Ack_OTP-CR-117_19.pdf
+-rw-r--r--   0 bart      (1000) bart      (1001)   238330 2024-04-29 11:30:06.000000 otpcr-9/files/EM_T04_OTP-CR-117_19.pdf
+-rw-r--r--   0 bart      (1000) bart      (1001)   236671 2024-04-29 11:30:06.000000 otpcr-9/files/EM_T07_OTP-CR-117_19_001.pdf
+-rw-r--r--   0 bart      (1000) bart      (1001)  1685507 2024-04-29 11:30:06.000000 otpcr-9/files/bevestigd.jpg
+-rw-r--r--   0 bart      (1000) bart      (1001)    50044 2024-04-29 11:30:06.000000 otpcr-9/files/bevestigd.pdf
+-rw-r--r--   0 bart      (1000) bart      (1001)    69979 2024-04-29 11:30:06.000000 otpcr-9/files/informed.jpg
+-rw-r--r--   0 bart      (1000) bart      (1001)   242205 2024-04-29 11:30:06.000000 otpcr-9/files/verbatim5.png
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-04-29 19:56:54.747650 otpcr-9/otpcr/
+-rw-r--r--   0 bart      (1000) bart      (1001)      200 2024-04-29 19:19:07.000000 otpcr-9/otpcr/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      704 2024-04-29 12:15:10.000000 otpcr-9/otpcr/broker.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4002 2024-04-29 19:33:49.000000 otpcr-9/otpcr/client.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      581 2024-04-29 12:15:10.000000 otpcr-9/otpcr/command.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      285 2024-04-29 12:15:10.000000 otpcr-9/otpcr/default.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1397 2024-04-29 12:15:10.000000 otpcr-9/otpcr/errors.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      813 2024-04-29 12:15:10.000000 otpcr-9/otpcr/event.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2008 2024-04-29 12:15:10.000000 otpcr-9/otpcr/find.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1405 2024-04-29 12:15:10.000000 otpcr-9/otpcr/handler.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-04-29 19:56:54.747650 otpcr-9/otpcr/modules/
+-rw-r--r--   0 bart      (1000) bart      (1001)      166 2024-04-29 19:42:16.000000 otpcr-9/otpcr/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      216 2024-04-29 12:15:21.000000 otpcr-9/otpcr/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2354 2024-04-29 11:30:06.000000 otpcr-9/otpcr/modules/req.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     6109 2024-04-29 18:47:13.000000 otpcr-9/otpcr/object.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      278 2024-04-29 12:15:10.000000 otpcr-9/otpcr/repeater.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1340 2024-04-29 19:13:14.000000 otpcr-9/otpcr/runtime.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1956 2024-04-29 12:15:10.000000 otpcr-9/otpcr/thread.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1085 2024-04-29 12:15:10.000000 otpcr-9/otpcr/timer.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1120 2024-04-29 12:15:10.000000 otpcr-9/otpcr/whitelist.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1266 2024-04-29 12:15:10.000000 otpcr-9/otpcr/workdir.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-04-29 19:56:54.747650 otpcr-9/otpcr.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1001)     2691 2024-04-29 19:56:54.000000 otpcr-9/otpcr.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)      692 2024-04-29 19:56:54.000000 otpcr-9/otpcr.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        1 2024-04-29 19:56:54.000000 otpcr-9/otpcr.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        6 2024-04-29 19:56:54.000000 otpcr-9/otpcr.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        1 2024-04-29 19:56:54.000000 otpcr-9/otpcr.egg-info/zip-safe
+-rw-r--r--   0 bart      (1000) bart      (1001)     1217 2024-04-29 19:19:18.000000 otpcr-9/pyproject.toml
+-rw-r--r--   0 bart      (1000) bart      (1001)       38 2024-04-29 19:56:54.747650 otpcr-9/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1001)      169 2024-04-29 19:05:41.000000 otpcr-9/setup.py
```

### Comparing `otpcr-8/PKG-INFO` & `otpcr-9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: otpcr
-Version: 8
-Summary: The 117 communication record of the year 2019 to the Office of the Prosecutor of the International Criminal Court.
+Version: 9
+Summary: OTP-CR-117/19 - Communication Record (CR) 117 of the year 2019 (117/19) to the Office of the Prosecutor (OTP) of the International Criminal Court (ICC)
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/otpcr
 Project-URL: bugs, https://github.com/xobjectz/otpcr/issues
 Project-URL: source, https://github.com/xobjectz/otpcr
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: Public Domain
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Topic :: Utilities
 Description-Content-Type: text/x-rst
 
+| OTP-CR-117/19 - Communication Record (CR) 117 of the year 2019 (117/19) to the Office of the Prosecutor (OTP) of the International Criminal Court (ICC)
+|
+|
 | **Information and Evidence Unit**
 | **Office of the Prosecutor**
 | **Post Office Box 19519**
 | **2500 CM The Hague**
 | **The Netherlands**
 |
 |
```

### Comparing `otpcr-8/README.rst` & `otpcr-9/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+| OTP-CR-117/19 - Communication Record (CR) 117 of the year 2019 (117/19) to the Office of the Prosecutor (OTP) of the International Criminal Court (ICC)
+|
+|
 | **Information and Evidence Unit**
 | **Office of the Prosecutor**
 | **Post Office Box 19519**
 | **2500 CM The Hague**
 | **The Netherlands**
 |
 |
```

### Comparing `otpcr-8/files/EM_Ack_OTP-CR-117_19.pdf` & `otpcr-9/files/EM_Ack_OTP-CR-117_19.pdf`

 * *Files identical despite different names*

### Comparing `otpcr-8/files/EM_T04_OTP-CR-117_19.pdf` & `otpcr-9/files/EM_T04_OTP-CR-117_19.pdf`

 * *Files identical despite different names*

### Comparing `otpcr-8/files/EM_T07_OTP-CR-117_19_001.pdf` & `otpcr-9/files/EM_T07_OTP-CR-117_19_001.pdf`

 * *Files identical despite different names*

### Comparing `otpcr-8/files/bevestigd.jpg` & `otpcr-9/files/bevestigd.jpg`

 * *Files identical despite different names*

### Comparing `otpcr-8/files/bevestigd.pdf` & `otpcr-9/files/bevestigd.pdf`

 * *Files identical despite different names*

### Comparing `otpcr-8/files/informed.jpg` & `otpcr-9/files/informed.jpg`

 * *Files identical despite different names*

### Comparing `otpcr-8/files/verbatim5.png` & `otpcr-9/files/verbatim5.png`

 * *Files identical despite different names*

### Comparing `otpcr-8/otpcr/__main__.py` & `otpcr-9/bin/otpcr`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#!/usr/bin/env python3
 # This file is placed in the Public Domain.
 
 
 "main"
 
 
 import getpass
@@ -9,46 +10,40 @@
 import pwd
 import readline
 import sys
 import termios
 import time
 
 
-from .client  import Client, cmnd, parse_cmd, spl
-from .default import Default
-from .errors  import debug, enable, errors, later
-from .event   import Event
-from .object  import cdir
-from .runtime import broker
-from .workdir import Workdir, skel
+sys.path.insert(0, os.getcwd())
 
 
-from .command   import scan as scancmd
-from .whitelist import scan as scancls
+from otpcr.client  import Client, cmnd, parse_cmd
+from otpcr.default import Default
+from otpcr.errors  import debug, enable, errors
+from otpcr.event   import Event
+from otpcr.object  import cdir
+from otpcr.runtime import broker, dte, init, scan
+from otpcr.workdir import Workdir, skel
 
 
-from . import modules
+from otpcr import modules
 
 
 Cfg             = Default()
 Cfg.dis         = ""
-Cfg.mod         = ""
+Cfg.mod         = "cmd,req"
 Cfg.opts        = ""
-Cfg.name        = __file__.split(os.sep)[-2]
+Cfg.name        = __file__.split(os.sep)[-1]
 Cfg.version     = "8"
 Cfg.wdr         = os.path.expanduser(f"~/.{Cfg.name}")
 Cfg.pidfile     = os.path.join(Cfg.wdr, f"{Cfg.name}.pid")
-
-
 Workdir.workdir = Cfg.wdr
 
 
-dte = time.ctime(time.time()).replace("  ", " ")
-
-
 class Console(Client):
 
     "Console"
 
     def __init__(self):
         Client.__init__(self)
         broker.add(self)
@@ -97,61 +92,21 @@
     if os.path.exists(pidfile):
         os.unlink(pidfile)
     cdir(os.path.dirname(pidfile))
     with open(pidfile, "w", encoding="utf-8") as fds:
         fds.write(str(os.getpid()))
 
 
-def init(pkg, modstr, disable=""):
-    "init"
-    mds = []
-    for modname in spl(modstr):
-        if skip(modname, disable):
-            continue
-        module = getattr(pkg, modname, None)
-        if not module:
-            continue
-        if "init" in dir(module):
-            try:
-                module.init()
-                mds.append(module)
-            except Exception as ex: # pylint: disable=W0718
-                later(ex)
-    return mds
-
-
-def scan(pkg, modstr, disable=""):
-    "scan modules for commands and classes"
-    mds = []
-    for modname in spl(modstr):
-        if skip(modname, disable):
-            continue
-        module = getattr(pkg, modname, None)
-        if not module:
-            continue
-        scancmd(module)
-        scancls(module)
-    return mds
-
-
 def privileges(username):
     "drop privileges."
     pwnam = pwd.getpwnam(username)
     os.setgid(pwnam.pw_gid)
     os.setuid(pwnam.pw_uid)
 
 
-def skip(name, skipped):
-    "check for skipping"
-    for skp in spl(skipped):
-        if skp in name:
-            return True
-    return False
-
-
 def wrap(func):
     "restore console."
     old2 = None
     try:
         old2 = termios.tcgetattr(sys.stdin.fileno())
     except termios.error:
         pass
@@ -160,27 +115,23 @@
     except (KeyboardInterrupt, EOFError):
         print("")
     finally:
         if old2:
             termios.tcsetattr(sys.stdin.fileno(), termios.TCSADRAIN, old2)
 
 
-def ver(event):
-    "show version."
-    event.reply(f"{Cfg.name.upper()} {Cfg.version}")
-
-
 def main():
     "main"
     enable(print)
     skel()
     parse_cmd(Cfg, " ".join(sys.argv[1:]))
     if Cfg.sets.dis:
         Cfg.dis += "," + Cfg.sets.dis
-    Cfg.mod = ",".join(modules.__dir__())
+    if "a" in Cfg.opts:
+        Cfg.mod = ",".join(modules.__dir__())
     if "v" in Cfg.opts:
         debug(f"{Cfg.name.upper()} {Cfg.opts.upper()} started {dte}")
     scan(modules, Cfg.mod, Cfg.dis)
     if "h" in Cfg.opts:
         print(__doc__)
     elif "d" in Cfg.opts:
         Cfg.mod = ",".join(modules.__dir__())
@@ -196,16 +147,11 @@
         csl.start()
         while 1:
             time.sleep(1.0)
     elif Cfg.otxt:
         cmnd(Cfg.otxt, print)
 
 
-def wrapped():
-    "wrap main function."
-    wrap(main)
-
-
 if __name__ == "__main__":
     readline.redisplay()
-    wrapped()
+    wrap(main)
     errors()
```

### Comparing `otpcr-8/otpcr/broker.py` & `otpcr-9/otpcr/broker.py`

 * *Files identical despite different names*

### Comparing `otpcr-8/otpcr/client.py` & `otpcr-9/otpcr/client.py`

 * *Files identical despite different names*

### Comparing `otpcr-8/otpcr/command.py` & `otpcr-9/otpcr/command.py`

 * *Files identical despite different names*

### Comparing `otpcr-8/otpcr/errors.py` & `otpcr-9/otpcr/errors.py`

 * *Files identical despite different names*

### Comparing `otpcr-8/otpcr/event.py` & `otpcr-9/otpcr/event.py`

 * *Files identical despite different names*

### Comparing `otpcr-8/otpcr/find.py` & `otpcr-9/otpcr/find.py`

 * *Files identical despite different names*

### Comparing `otpcr-8/otpcr/handler.py` & `otpcr-9/otpcr/handler.py`

 * *Files identical despite different names*

### Comparing `otpcr-8/otpcr/modules/req.py` & `otpcr-9/otpcr/modules/req.py`

 * *Files identical despite different names*

### Comparing `otpcr-8/otpcr/modules/tmr.py` & `otpcr-9/otpcr/object.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,229 +1,272 @@
 # This file is placed in the Public Domain.
 
 
-"timer"
+"clean namespace"
 
 
-import datetime
-import re
-import time as ttime
-
-
-from ..client    import laps
-from ..event     import Event
-from ..find      import find
-from ..object    import update
-from ..runtime   import broker
-from ..thread    import launch
-from ..timer     import Timer
-from ..workdir   import sync
-
-
-def init():
-    "start timers."
-    for _fn, obj in find("timer"):
-        if "time" not in obj:
-            continue
-        diff = float(obj.time) - ttime.time()
-        if diff > 0:
-            bot = broker.first()
-            evt = Event()
-            update(evt, obj)
-            evt.orig = object.__repr__(bot)
-            timer = Timer(diff, evt.show)
-            launch(timer.start)
-
-
-MONTHS = [
-    'Bo',
-    'Jan',
-    'Feb',
-    'Mar',
-    'Apr',
-    'May',
-    'Jun',
-    'Jul',
-    'Aug',
-    'Sep',
-    'Oct',
-    'Nov',
-    'Dec'
-]
-
-
-FORMATS = [
-    "%Y-%m-%d",
-    "%d-%m-%Y",
-    "%d-%m",
-    "%m-%d",
-]
-
-
-class NoDate(Exception):
-
-    "NoDate"
-
-
-def extract_date(daystr):
-    "extract date from string."
-    res = None
-    for fmt in FORMATS:
-        try:
-            res = ttime.mktime(ttime.strptime(daystr, fmt))
-            break
-        except ValueError:
-            res = None
-    return res
+import json
+import os
+import pathlib
+import _thread
 
 
-def get_day(daystr):
-    "return day from string."
-    day = None
-    month = None
-    yea = None
-    try:
-        ymdre = re.search(r'(\d+)-(\d+)-(\d+)', daystr)
-        if ymdre:
-            (day, month, yea) = ymdre.groups()
-    except ValueError:
-        try:
-            ymre = re.search(r'(\d+)-(\d+)', daystr)
-            if ymre:
-                (day, month) = ymre.groups()
-                yea = ttime.strftime("%Y", ttime.localtime())
-        except Exception as ex: # pylint: disable=W0212
-            raise NoDate(daystr) from ex
-    if day:
-        day = int(day)
-        month = int(month)
-        yea = int(yea)
-        date = f"{day} {MONTHS[month]} {yea}"
-        return ttime.mktime(ttime.strptime(date, r"%d %b %Y"))
-    raise NoDate(daystr)
-
-
-def get_hour(daystr):
-    "return hour from string."
-    try:
-        hmsre = re.search(r'(\d+):(\d+):(\d+)', str(daystr))
-        hours = 60 * 60 * (int(hmsre.group(1)))
-        hoursmin = hours  + int(hmsre.group(2)) * 60
-        hmsres = hoursmin + int(hmsre.group(3))
-    except AttributeError:
-        pass
-    except ValueError:
-        pass
-    try:
-        hmre = re.search(r'(\d+):(\d+)', str(daystr))
-        hours = 60 * 60 * (int(hmre.group(1)))
-        hmsres = hours + int(hmre.group(2)) * 60
-    except AttributeError:
-        return 0
-    except ValueError:
-        return 0
-    return hmsres
-
-
-def get_time(txt):
-    "parse full time string."
-    try:
-        target = get_day(txt)
-    except NoDate:
-        target = to_day(today())
-    hour =  get_hour(txt)
-    if hour:
-        target += hour
-    return target
-
-
-def parse_time(txt):
-    "parse time from string."
-    seconds = 0
-    target = 0
-    txt = str(txt)
-    for word in txt.split():
-        if word.startswith("+"):
-            seconds = int(word[1:])
-            return ttime.time() + seconds
-        if word.startswith("-"):
-            seconds = int(word[1:])
-            return ttime.time() - seconds
-    if not target:
+lock = _thread.allocate_lock()
+
+
+class Object: # pylint: disable=R0902
+
+    "Object"
+
+    def __contains__(self, key):
+        return key in dir(self)
+
+    def __iter__(self):
+        return iter(self.__dict__)
+
+    def __len__(self):
+        return len(self.__dict__)
+
+    def __str__(self):
+        return str(self.__dict__)
+
+
+def construct(obj, *args, **kwargs):
+    "construct an object from provided arguments."
+    if args:
+        val = args[0]
+        if isinstance(val, zip):
+            update(obj, dict(val))
+        elif isinstance(val, dict):
+            update(obj, val)
+        elif isinstance(val, Object):
+            update(obj, vars(val))
+    if kwargs:
+        update(obj, kwargs)
+
+
+def edit(obj, setter, skip=False):
+    "edit an object from provided dict/dict-like."
+    for key, val in items(setter):
+        if skip and val == "":
+            continue
         try:
-            target = get_day(txt)
-        except NoDate:
-            target = to_day(today())
-        hour =  get_hour(txt)
-        if hour:
-            target += hour
-    return target
-
-
-def to_day(daystr):
-    "parse day from string."
-    previous = ""
-    line = ""
-    daystr = str(daystr)
-    res = None
-    for word in daystr.split():
-        line = previous + " " + word
-        previous = word
+            setattr(obj, key, int(val))
+            continue
+        except ValueError:
+            pass
         try:
-            res = extract_date(line.strip())
-            break
+            setattr(obj, key, float(val))
+            continue
         except ValueError:
-            res = None
-        line = ""
-    return res
+            pass
+        if val in ["True", "true"]:
+            setattr(obj, key, True)
+        elif val in ["False", "false"]:
+            setattr(obj, key, False)
+        else:
+            setattr(obj, key, val)
 
 
-def today():
-    "return date."
-    return str(datetime.datetime.today()).split()[0]
-
-
-def tmr(event):
-    "add a timer."
-    result = ""
-    if not event.rest:
-        nmr = 0
-        for _fn, obj in find('timer'):
-            lap = float(obj.time) - ttime.time()
-            if lap > 0:
-                event.reply(f'{nmr} {obj.txt} {laps(lap)}')
-                nmr += 1
-        return result
-    seconds = 0
-    line = ""
-    for word in event.args:
-        if word.startswith("+"):
-            try:
-                seconds = int(word[1:])
-            except (ValueError, IndexError):
-                event.reply(f"{seconds} is not an integer")
-                return result
+def fmt(obj, args=None, skip=None, plain=False):
+    "format an object to a printable string."
+    if args is None:
+        args = keys(obj)
+    if skip is None:
+        skip = []
+    txt = ""
+    for key in args:
+        if key.startswith("__"):
+            continue
+        if key in skip:
+            continue
+        value = getattr(obj, key, None)
+        if value is None:
+            continue
+        if plain:
+            txt += f"{value} "
+        elif isinstance(value, str) and len(value.split()) >= 2:
+            txt += f'{key}="{value}" '
+        else:
+            txt += f"{key}={value} "
+    return txt.strip()
+
+
+def fqn(obj):
+    "return full qualified name of an object."
+    kin = str(type(obj)).split()[-1][1:-2]
+    if kin == "type":
+        kin = obj.__name__
+    return kin
+
+
+def items(obj):
+    "return the items of an object."
+    if isinstance(obj, type({})):
+        return obj.items()
+    return obj.__dict__.items()
+
+
+def keys(obj):
+    "return keys of an object."
+    if isinstance(obj, type({})):
+        return obj.keys()
+    return list(obj.__dict__.keys())
+
+
+def read(obj, pth):
+    "read an object from file path."
+    with lock:
+        with open(pth, 'r', encoding='utf-8') as ofile:
+            update(obj, load(ofile))
+
+
+def search(obj, selector):
+    "check if object matches provided values."
+    res = False
+    if not selector:
+        return True
+    for key, value in items(selector):
+        val = getattr(obj, key, None)
+        if str(value).lower() in str(val).lower():
+            res = True
         else:
-            line += word + " "
-    if seconds:
-        target = ttime.time() + seconds
+            res = False
+            break
+    return res
+
+
+def update(obj, data, empty=True):
+    "update an object."
+    for key, value in items(data):
+        if empty and not value:
+            continue
+        setattr(obj, key, value)
+
+
+def values(obj):
+    "return values of an object."
+    return obj.__dict__.values()
+
+
+def write(obj, pth):
+    "write an object to disk."
+    with lock:
+        cdir(os.path.dirname(pth))
+        with open(pth, 'w', encoding='utf-8') as ofile:
+            dump(obj, ofile, indent=4)
+
+
+class ObjectDecoder(json.JSONDecoder):
+
+    "ObjectDecoder"
+
+    def __init__(self, *args, **kwargs):
+        json.JSONDecoder.__init__(self, *args, **kwargs)
+
+    def decode(self, s, _w=None):
+        "decoding string to object."
+        val = json.JSONDecoder.decode(self, s)
+        if not val:
+            val = {}
+        return hook(val)
+
+    def raw_decode(self, s, idx=0):
+        "decode partial string to object."
+        return json.JSONDecoder.raw_decode(self, s, idx)
+
+
+def hook(objdict, typ=None):
+    "construct object from dict."
+    if typ:
+        obj = typ()
     else:
+        obj = Object()
+    construct(obj, objdict)
+    return obj
+
+
+def load(fpt, *args, **kw):
+    "load object from file."
+    kw["cls"] = ObjectDecoder
+    kw["object_hook"] = hook
+    return json.load(fpt, *args, **kw)
+
+
+def loads(string, *args, **kw):
+    "load object from string."
+    kw["cls"] = ObjectDecoder
+    kw["object_hook"] = hook
+    return json.loads(string, *args, **kw)
+
+
+class ObjectEncoder(json.JSONEncoder):
+
+    "ObjectEncoder"
+
+    def __init__(self, *args, **kwargs):
+        json.JSONEncoder.__init__(self, *args, **kwargs)
+
+    def default(self, o):
+        "return stringable value."
+        if isinstance(o, dict):
+            return o.items()
+        if isinstance(o, Object):
+            return vars(o)
+        if isinstance(o, list):
+            return iter(o)
+        if isinstance(o, (type(str), type(True), type(False), type(int), type(float))):
+            return o
         try:
-            target = get_day(event.rest)
-        except NoDate:
-            target = to_day(today())
-        hour =  get_hour(event.rest)
-        if hour:
-            target += hour
-    if not target or ttime.time() > target:
-        event.reply("already passed given time.")
-        return result
-    event.time = target
-    diff = target - ttime.time()
-    event.reply("ok " +  laps(diff))
-    event.result = []
-    event.result.append(event.rest)
-    timer = Timer(diff, event.show, thrname=event.cmd)
-    update(timer, event)
-    sync(timer)
-    launch(timer.start)
-    return result
+            return json.JSONEncoder.default(self, o)
+        except TypeError:
+            return o.__dict__
+
+    def encode(self, o) -> str:
+        "encode object to string."
+        return json.JSONEncoder.encode(self, o)
+
+    def iterencode(self, o, _one_shot=False):
+        "loop over object to encode to string."
+        return json.JSONEncoder.iterencode(self, o, _one_shot)
+
+
+def dump(*args, **kw):
+    "dump object to file."
+    kw["cls"] = ObjectEncoder
+    return json.dump(*args, **kw)
+
+
+def dumps(*args, **kw):
+    "dump object to string."
+    kw["cls"] = ObjectEncoder
+    return json.dumps(*args, **kw)
+
+
+def cdir(pth):
+    "create directory."
+    if os.path.exists(pth):
+        return
+    pth = pathlib.Path(pth)
+    os.makedirs(pth, exist_ok=True)
+
+
+def __dir__():
+    return (
+        'Object',
+        'construct',
+        'dump',
+        'dumps',
+        'edit',
+        'fmt',
+        'fqn',
+        'hook',
+        'items',
+        'keys',
+        'load',
+        'loads',
+        'read',
+        'search',
+        'update',
+        'values',
+        'write'
+    )
```

### Comparing `otpcr-8/otpcr/thread.py` & `otpcr-9/otpcr/thread.py`

 * *Files identical despite different names*

### Comparing `otpcr-8/otpcr/timer.py` & `otpcr-9/otpcr/timer.py`

 * *Files identical despite different names*

### Comparing `otpcr-8/otpcr/whitelist.py` & `otpcr-9/otpcr/whitelist.py`

 * *Files identical despite different names*

### Comparing `otpcr-8/otpcr/workdir.py` & `otpcr-9/otpcr/workdir.py`

 * *Files identical despite different names*

### Comparing `otpcr-8/otpcr.egg-info/PKG-INFO` & `otpcr-9/otpcr.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: otpcr
-Version: 8
-Summary: The 117 communication record of the year 2019 to the Office of the Prosecutor of the International Criminal Court.
+Version: 9
+Summary: OTP-CR-117/19 - Communication Record (CR) 117 of the year 2019 (117/19) to the Office of the Prosecutor (OTP) of the International Criminal Court (ICC)
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/otpcr
 Project-URL: bugs, https://github.com/xobjectz/otpcr/issues
 Project-URL: source, https://github.com/xobjectz/otpcr
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: Public Domain
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Topic :: Utilities
 Description-Content-Type: text/x-rst
 
+| OTP-CR-117/19 - Communication Record (CR) 117 of the year 2019 (117/19) to the Office of the Prosecutor (OTP) of the International Criminal Court (ICC)
+|
+|
 | **Information and Evidence Unit**
 | **Office of the Prosecutor**
 | **Post Office Box 19519**
 | **2500 CM The Hague**
 | **The Netherlands**
 |
 |
```

### Comparing `otpcr-8/otpcr.egg-info/SOURCES.txt` & `otpcr-9/otpcr.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 README.rst
 pyproject.toml
 setup.py
-docs/MANUAL.rst
+bin/otpcr
 files/EM_Ack_OTP-CR-117_19.pdf
 files/EM_T04_OTP-CR-117_19.pdf
 files/EM_T07_OTP-CR-117_19_001.pdf
 files/bevestigd.jpg
 files/bevestigd.pdf
 files/informed.jpg
 files/verbatim5.png
 otpcr/__init__.py
-otpcr/__main__.py
 otpcr/broker.py
 otpcr/client.py
 otpcr/command.py
 otpcr/default.py
 otpcr/errors.py
 otpcr/event.py
 otpcr/find.py
@@ -25,26 +24,12 @@
 otpcr/thread.py
 otpcr/timer.py
 otpcr/whitelist.py
 otpcr/workdir.py
 otpcr.egg-info/PKG-INFO
 otpcr.egg-info/SOURCES.txt
 otpcr.egg-info/dependency_links.txt
-otpcr.egg-info/entry_points.txt
 otpcr.egg-info/top_level.txt
 otpcr.egg-info/zip-safe
 otpcr/modules/__init__.py
 otpcr/modules/cmd.py
-otpcr/modules/err.py
-otpcr/modules/flt.py
-otpcr/modules/fnd.py
-otpcr/modules/irc.py
-otpcr/modules/log.py
-otpcr/modules/mbx.py
-otpcr/modules/mod.py
-otpcr/modules/req.py
-otpcr/modules/rss.py
-otpcr/modules/rst.py
-otpcr/modules/tdo.py
-otpcr/modules/thr.py
-otpcr/modules/tmr.py
-otpcr/modules/udp.py
+otpcr/modules/req.py
```

### Comparing `otpcr-8/pyproject.toml` & `otpcr-9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,38 +3,39 @@
     "setuptools>=43.0.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "otpcr"
-description = "The 117 communication record of the year 2019 to the Office of the Prosecutor of the International Criminal Court."
-version = "8"
+description = "OTP-CR-117/19 - Communication Record (CR) 117 of the year 2019 (117/19) to the Office of the Prosecutor (OTP) of the International Criminal Court (ICC)"
+version = "9"
 authors = [
     {name = "Bart Thate", email = "bthate@dds.nl"},
 ]
 readme = "README.rst"
 license = {text="Public Domain"}
 classifiers = [ 
     'Development Status :: 3 - Alpha',
     'License :: Public Domain',
     'Operating System :: Unix',
     'Programming Language :: Python',
     'Topic :: Utilities'
 ]
 
-[project.scripts]
-"otpcr" = "otpcr.__main__:wrapped"
 
 [project.urls]
 "home" = "https://pypi.org/project/otpcr"
 "bugs" = "https://github.com/xobjectz/otpcr/issues"
 "source" = "https://github.com/xobjectz/otpcr"
 
 [tool.setuptools]
+script-files = [
+    'bin/otpcr',
+]
 packages = [
     'otpcr',
     'otpcr.modules'
 ]
 zip-safe=true
```

