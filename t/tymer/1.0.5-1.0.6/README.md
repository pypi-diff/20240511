# Comparing `tmp/tymer-1.0.5.tar.gz` & `tmp/tymer-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tymer-1.0.5.tar", last modified: Sat Apr 20 10:21:08 2024, max compression
+gzip compressed data, was "tymer-1.0.6.tar", last modified: Sat May 11 17:36:37 2024, max compression
```

## Comparing `tymer-1.0.5.tar` & `tymer-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 10:21:08.083924 tymer-1.0.5/
--rw-rw-rw-   0        0        0      667 2024-04-20 10:20:32.000000 tymer-1.0.5/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1060 2023-02-17 15:12:04.000000 tymer-1.0.5/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2022-07-06 14:59:00.000000 tymer-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      166 2024-04-20 10:21:08.082551 tymer-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-02-17 15:13:38.000000 tymer-1.0.5/README.txt
-drwxrwxrwx   0        0        0        0 2024-04-20 10:21:08.063624 tymer-1.0.5/Tymer/
--rw-rw-rw-   0        0        0     2061 2024-04-20 10:19:37.000000 tymer-1.0.5/Tymer/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-20 10:21:08.083924 tymer-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      343 2024-04-20 10:19:54.000000 tymer-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-20 10:21:08.081128 tymer-1.0.5/tymer.egg-info/
--rw-rw-rw-   0        0        0      166 2024-04-20 10:21:07.000000 tymer-1.0.5/tymer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2024-04-20 10:21:07.000000 tymer-1.0.5/tymer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 10:21:07.000000 tymer-1.0.5/tymer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-20 10:21:07.000000 tymer-1.0.5/tymer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-11 17:36:37.409858 tymer-1.0.6/
+-rw-rw-rw-   0        0        0      777 2024-05-11 17:35:45.000000 tymer-1.0.6/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1060 2023-02-17 15:12:04.000000 tymer-1.0.6/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2022-07-06 14:59:00.000000 tymer-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      166 2024-05-11 17:36:37.409858 tymer-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-02-17 15:13:38.000000 tymer-1.0.6/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-11 17:36:37.400180 tymer-1.0.6/Tymer/
+-rw-rw-rw-   0        0        0     2247 2024-05-11 17:34:45.000000 tymer-1.0.6/Tymer/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-11 17:36:37.410858 tymer-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      343 2024-05-11 17:36:15.000000 tymer-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 17:36:37.408854 tymer-1.0.6/tymer.egg-info/
+-rw-rw-rw-   0        0        0      166 2024-05-11 17:36:37.000000 tymer-1.0.6/tymer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2024-05-11 17:36:37.000000 tymer-1.0.6/tymer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 17:36:37.000000 tymer-1.0.6/tymer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-11 17:36:37.000000 tymer-1.0.6/tymer.egg-info/top_level.txt
```

### Comparing `tymer-1.0.5/CHANGELOG.txt` & `tymer-1.0.6/CHANGELOG.txt`

 * *Files 11% similar despite different names*

```diff
@@ -21,8 +21,12 @@
 -------------------
 - Added Countdown option
 - Added option to display time as integer rather than float
 - whenever you instance .restart() without inputing a value, it restarts the timer with the same time as the previous instance
 
 1.0.5 (4/20/2024)
 -------------------
-- Set the default value when instancing .time() to show as an integer
+- Set the default value when instancing .time() to show as an integer
+
+1.0.6 (5/11/2024)
+-------------------
+- when running .start() you can set the amount of seconds in start
```

### Comparing `tymer-1.0.5/LICENCE.txt` & `tymer-1.0.6/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `tymer-1.0.5/Tymer/__init__.py` & `tymer-1.0.6/Tymer/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,20 @@
         self.sec = seconds
         self.start_time = None
         self.run_timer = True
         self.timer = 0
         self.start_timer = True
         self.countdown = countdown
         self.integer = integer
-    def start(self):
+        self.run_once = True
+    def start(self, seconds='default'):
+        if self.run_once:
+            if seconds != 'default':
+                self.sec = seconds
+            self.run_once = False
         if self.start_timer:
             self.start_time = t.time()
             self.start_timer = False
         self.current_time = t.time()
         if self.run_timer:
             if self.start_time != None:
                 if not self.countdown:
@@ -33,15 +38,15 @@
         else:
             if self.timer <= 0:
                 self.run_timer = False
                 self.timer = 0
     def stop(self):
         self.run_timer = False
         pass
-    def restart(self,seconds='default'):
+    def restart(self, seconds='default'):
         self.new_time = seconds
         self.start_time = None
         self.run_timer = True
         if self.new_time != 'default':
             self.sec = self.new_time
         self.start_timer = True
         pass
```

