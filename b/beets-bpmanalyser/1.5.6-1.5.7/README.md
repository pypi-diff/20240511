# Comparing `tmp/beets-bpmanalyser-1.5.6.tar.gz` & `tmp/beets-bpmanalyser-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/BeetsPluginBpmAnalyser/BeetsPluginBpmAnalyser/dist/.tmp-5rynycxh/beets-bpmanalyser-1.5.6.tar", last modified: Mon May  6 20:06:20 2024, max compression
+gzip compressed data, was "/home/runner/work/BeetsPluginBpmAnalyser/BeetsPluginBpmAnalyser/dist/.tmp-t2eeseoh/beets-bpmanalyser-1.5.7.tar", last modified: Sat May 11 16:20:51 2024, max compression
```

## Comparing `beets-bpmanalyser-1.5.6.tar` & `beets-bpmanalyser-1.5.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:06:20.000000 beets-bpmanalyser-1.5.6/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1067 2024-05-06 20:06:08.000000 beets-bpmanalyser-1.5.6/LICENSE.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-05-06 20:06:08.000000 beets-bpmanalyser-1.5.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-05-06 20:06:20.000000 beets-bpmanalyser-1.5.6/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     5747 2024-05-06 20:06:08.000000 beets-bpmanalyser-1.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:06:20.000000 beets-bpmanalyser-1.5.6/beets_bpmanalyser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-05-06 20:06:20.000000 beets-bpmanalyser-1.5.6/beets_bpmanalyser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-06 20:06:20.000000 beets-bpmanalyser-1.5.6/beets_bpmanalyser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 20:06:20.000000 beets-bpmanalyser-1.5.6/beets_bpmanalyser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-06 20:06:20.000000 beets-bpmanalyser-1.5.6/beets_bpmanalyser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-06 20:06:20.000000 beets-bpmanalyser-1.5.6/beets_bpmanalyser.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:06:20.000000 beets-bpmanalyser-1.5.6/beetsplug/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:06:20.000000 beets-bpmanalyser-1.5.6/beetsplug/bpmanalyser/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1256 2024-05-06 20:06:08.000000 beets-bpmanalyser-1.5.6/beetsplug/bpmanalyser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-06 20:06:08.000000 beets-bpmanalyser-1.5.6/beetsplug/bpmanalyser/analyser.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7357 2024-05-06 20:06:08.000000 beets-bpmanalyser-1.5.6/beetsplug/bpmanalyser/command.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      175 2024-05-06 20:06:08.000000 beets-bpmanalyser-1.5.6/beetsplug/bpmanalyser/version.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      193 2024-05-06 20:06:20.000000 beets-bpmanalyser-1.5.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1492 2024-05-06 20:06:08.000000 beets-bpmanalyser-1.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:20:51.000000 beets-bpmanalyser-1.5.7/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1067 2024-05-11 16:20:35.000000 beets-bpmanalyser-1.5.7/LICENSE.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-05-11 16:20:35.000000 beets-bpmanalyser-1.5.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-05-11 16:20:51.000000 beets-bpmanalyser-1.5.7/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5760 2024-05-11 16:20:35.000000 beets-bpmanalyser-1.5.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:20:51.000000 beets-bpmanalyser-1.5.7/beets_bpmanalyser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-05-11 16:20:51.000000 beets-bpmanalyser-1.5.7/beets_bpmanalyser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-11 16:20:51.000000 beets-bpmanalyser-1.5.7/beets_bpmanalyser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 16:20:51.000000 beets-bpmanalyser-1.5.7/beets_bpmanalyser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-11 16:20:51.000000 beets-bpmanalyser-1.5.7/beets_bpmanalyser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-11 16:20:51.000000 beets-bpmanalyser-1.5.7/beets_bpmanalyser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:20:51.000000 beets-bpmanalyser-1.5.7/beetsplug/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:20:51.000000 beets-bpmanalyser-1.5.7/beetsplug/bpmanalyser/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1293 2024-05-11 16:20:35.000000 beets-bpmanalyser-1.5.7/beetsplug/bpmanalyser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-11 16:20:35.000000 beets-bpmanalyser-1.5.7/beetsplug/bpmanalyser/analyser.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7425 2024-05-11 16:20:35.000000 beets-bpmanalyser-1.5.7/beetsplug/bpmanalyser/command.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      175 2024-05-11 16:20:35.000000 beets-bpmanalyser-1.5.7/beetsplug/bpmanalyser/version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      193 2024-05-11 16:20:51.000000 beets-bpmanalyser-1.5.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1492 2024-05-11 16:20:35.000000 beets-bpmanalyser-1.5.7/setup.py
```

### Comparing `beets-bpmanalyser-1.5.6/LICENSE.txt` & `beets-bpmanalyser-1.5.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `beets-bpmanalyser-1.5.6/PKG-INFO` & `beets-bpmanalyser-1.5.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,8 @@
-Metadata-Version: 2.1
-Name: beets-bpmanalyser
-Version: 1.5.6
-Summary: A beets plugin for analysing tempo of songs and storing it in the bpm tag.
-Home-page: https://github.com/adamjakab/BeetsPluginBpmAnalyser
-Author: Adam Jakab
-Author-email: adam@jakab.pro
-License: MIT
-Platform: ALL
-Classifier: Topic :: Multimedia :: Sound/Audio
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-[![Test and Release](https://github.com/adamjakab/BeetsPluginBpmAnalyser/actions/workflows/test_and_release.yml/badge.svg)](https://github.com/adamjakab/BeetsPluginBpmAnalyser/actions/workflows/test_and_release.yml)
+[![Test & Release & Deploy](https://github.com/adamjakab/BeetsPluginBpmAnalyser/actions/workflows/test_release_deploy.yml/badge.svg)](https://github.com/adamjakab/BeetsPluginBpmAnalyser/actions/workflows/test_release_deploy.yml)
 [![PyPi](https://img.shields.io/pypi/v/beets-bpmanalyser.svg)](https://pypi.org/project/beets-bpmanalyser/)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE.txt)
 
 # BPM Analyser (Beets Plugin)
 
 The _beets-bpmanalyser_ plugin lets you analyse the tempo of the songs you have in your library and write the bpm information on the bpm tag of your media files.
```

### Comparing `beets-bpmanalyser-1.5.6/README.md` & `beets-bpmanalyser-1.5.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,25 @@
-[![Test and Release](https://github.com/adamjakab/BeetsPluginBpmAnalyser/actions/workflows/test_and_release.yml/badge.svg)](https://github.com/adamjakab/BeetsPluginBpmAnalyser/actions/workflows/test_and_release.yml)
+Metadata-Version: 2.1
+Name: beets-bpmanalyser
+Version: 1.5.7
+Summary: A beets plugin for analysing tempo of songs and storing it in the bpm tag.
+Home-page: https://github.com/adamjakab/BeetsPluginBpmAnalyser
+Author: Adam Jakab
+Author-email: adam@jakab.pro
+License: MIT
+Platform: ALL
+Classifier: Topic :: Multimedia :: Sound/Audio
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Environment :: Console
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+[![Test & Release & Deploy](https://github.com/adamjakab/BeetsPluginBpmAnalyser/actions/workflows/test_release_deploy.yml/badge.svg)](https://github.com/adamjakab/BeetsPluginBpmAnalyser/actions/workflows/test_release_deploy.yml)
 [![PyPi](https://img.shields.io/pypi/v/beets-bpmanalyser.svg)](https://pypi.org/project/beets-bpmanalyser/)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE.txt)
 
 # BPM Analyser (Beets Plugin)
 
 The _beets-bpmanalyser_ plugin lets you analyse the tempo of the songs you have in your library and write the bpm information on the bpm tag of your media files.
```

### Comparing `beets-bpmanalyser-1.5.6/beets_bpmanalyser.egg-info/PKG-INFO` & `beets-bpmanalyser-1.5.7/beets_bpmanalyser.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: beets-bpmanalyser
-Version: 1.5.6
+Version: 1.5.7
 Summary: A beets plugin for analysing tempo of songs and storing it in the bpm tag.
 Home-page: https://github.com/adamjakab/BeetsPluginBpmAnalyser
 Author: Adam Jakab
 Author-email: adam@jakab.pro
 License: MIT
 Platform: ALL
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-[![Test and Release](https://github.com/adamjakab/BeetsPluginBpmAnalyser/actions/workflows/test_and_release.yml/badge.svg)](https://github.com/adamjakab/BeetsPluginBpmAnalyser/actions/workflows/test_and_release.yml)
+[![Test & Release & Deploy](https://github.com/adamjakab/BeetsPluginBpmAnalyser/actions/workflows/test_release_deploy.yml/badge.svg)](https://github.com/adamjakab/BeetsPluginBpmAnalyser/actions/workflows/test_release_deploy.yml)
 [![PyPi](https://img.shields.io/pypi/v/beets-bpmanalyser.svg)](https://pypi.org/project/beets-bpmanalyser/)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE.txt)
 
 # BPM Analyser (Beets Plugin)
 
 The _beets-bpmanalyser_ plugin lets you analyse the tempo of the songs you have in your library and write the bpm information on the bpm tag of your media files.
```

### Comparing `beets-bpmanalyser-1.5.6/beetsplug/bpmanalyser/__init__.py` & `beets-bpmanalyser-1.5.7/beetsplug/bpmanalyser/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,15 +29,16 @@
         if self.config['auto']:
             self.import_stages = [self.imported]
 
     def commands(self):
         return [BpmAnalyserCommand(self.config)]
 
     def imported(self, session, task):
+        cmd = BpmAnalyserCommand(self.config)
         # Add BPM for imported items.
         for item in task.imported_items():
             if not self.config['force'] and item['bpm'] != 0:
                 item_path = item.get("path").decode("utf-8")
-                log.debug("Skipping item with existing BPM[{0}]...".format(item_path))
+                log.debug("Skipped. Item({}) has already got BPM: {}".format(item_path, item['bpm']))
                 return
             else:
-                BpmAnalyserCommand(self.config).analyse(item)
+                cmd.runAnalyser(item)
```

### Comparing `beets-bpmanalyser-1.5.6/beetsplug/bpmanalyser/analyser.py` & `beets-bpmanalyser-1.5.7/beetsplug/bpmanalyser/analyser.py`

 * *Files identical despite different names*

### Comparing `beets-bpmanalyser-1.5.6/beetsplug/bpmanalyser/command.py` & `beets-bpmanalyser-1.5.7/beetsplug/bpmanalyser/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,14 +174,17 @@
         # @TODO: create and show a progress bar (--progress-only option)
         with cf.ThreadPoolExecutor(max_workers) as executor:
             for result in executor.map(taskRef, items):
                 finished += 1
             
         self._say("Done.")
     
+    #
+    # Run the external analyser script on a single item
+    #
     def runAnalyser(self, item: Item):
         item_path = item.get("path").decode("utf-8")
         log.debug("Analysing[{0}]...".format(item_path))
         
         proc = Popen([sys.executable, self.analyser_script_path, item_path],
                      stdout=PIPE, stderr=PIPE)
         stdout, stderr = proc.communicate()
```

### Comparing `beets-bpmanalyser-1.5.6/setup.py` & `beets-bpmanalyser-1.5.7/setup.py`

 * *Files identical despite different names*

