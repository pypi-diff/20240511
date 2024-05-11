# Comparing `tmp/ShellUtilities-2.1.8.tar.gz` & `tmp/ShellUtilities-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ShellUtilities-2.1.8.tar", last modified: Thu Aug 10 00:16:53 2023, max compression
+gzip compressed data, was "ShellUtilities-2.1.9.tar", last modified: Mon Aug 21 18:59:30 2023, max compression
```

## Comparing `ShellUtilities-2.1.8.tar` & `ShellUtilities-2.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-10 00:16:53.979361 ShellUtilities-2.1.8/
--rw-r--r--   0 root         (0) root         (0)     3166 2023-08-10 00:16:53.979361 ShellUtilities-2.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2689 2023-08-10 00:12:41.000000 ShellUtilities-2.1.8/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-10 00:16:53.979361 ShellUtilities-2.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      965 2023-08-10 00:16:48.000000 ShellUtilities-2.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-10 00:16:53.977361 ShellUtilities-2.1.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-10 00:16:53.978361 ShellUtilities-2.1.8/src/ShellUtilities/
--rw-r--r--   0 root         (0) root         (0)     3770 2023-08-10 00:12:41.000000 ShellUtilities-2.1.8/src/ShellUtilities/Shell.py
--rw-r--r--   0 root         (0) root         (0)     1173 2023-08-09 20:33:01.000000 ShellUtilities-2.1.8/src/ShellUtilities/ShellCommandException.py
--rw-r--r--   0 root         (0) root         (0)     6158 2023-08-10 00:12:41.000000 ShellUtilities-2.1.8/src/ShellUtilities/ShellCommandResults.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-09 20:33:01.000000 ShellUtilities-2.1.8/src/ShellUtilities/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-10 00:16:53.978361 ShellUtilities-2.1.8/src/ShellUtilities.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3166 2023-08-10 00:16:53.000000 ShellUtilities-2.1.8/src/ShellUtilities.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      351 2023-08-10 00:16:53.000000 ShellUtilities-2.1.8/src/ShellUtilities.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-10 00:16:53.000000 ShellUtilities-2.1.8/src/ShellUtilities.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-08-10 00:16:53.000000 ShellUtilities-2.1.8/src/ShellUtilities.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-10 00:16:53.978361 ShellUtilities-2.1.8/tests/
--rw-r--r--   0 root         (0) root         (0)    10846 2023-08-10 00:12:41.000000 ShellUtilities-2.1.8/tests/test_Shell.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-21 18:59:30.138589 ShellUtilities-2.1.9/
+-rw-r--r--   0 root         (0) root         (0)     3166 2023-08-21 18:59:30.138589 ShellUtilities-2.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2689 2023-08-21 18:39:49.000000 ShellUtilities-2.1.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-21 18:59:30.138589 ShellUtilities-2.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      965 2023-08-21 18:58:38.000000 ShellUtilities-2.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-21 18:59:30.137589 ShellUtilities-2.1.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-21 18:59:30.137589 ShellUtilities-2.1.9/src/ShellUtilities/
+-rw-r--r--   0 root         (0) root         (0)     4129 2023-08-21 18:52:17.000000 ShellUtilities-2.1.9/src/ShellUtilities/Shell.py
+-rw-r--r--   0 root         (0) root         (0)     1173 2023-08-21 18:39:49.000000 ShellUtilities-2.1.9/src/ShellUtilities/ShellCommandException.py
+-rw-r--r--   0 root         (0) root         (0)     6158 2023-08-21 18:39:49.000000 ShellUtilities-2.1.9/src/ShellUtilities/ShellCommandResults.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-21 18:39:49.000000 ShellUtilities-2.1.9/src/ShellUtilities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-21 18:59:30.138589 ShellUtilities-2.1.9/src/ShellUtilities.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3166 2023-08-21 18:59:30.000000 ShellUtilities-2.1.9/src/ShellUtilities.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      351 2023-08-21 18:59:30.000000 ShellUtilities-2.1.9/src/ShellUtilities.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-21 18:59:30.000000 ShellUtilities-2.1.9/src/ShellUtilities.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-08-21 18:59:30.000000 ShellUtilities-2.1.9/src/ShellUtilities.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-21 18:59:30.138589 ShellUtilities-2.1.9/tests/
+-rw-r--r--   0 root         (0) root         (0)    10846 2023-08-21 18:39:49.000000 ShellUtilities-2.1.9/tests/test_Shell.py
```

### Comparing `ShellUtilities-2.1.8/PKG-INFO` & `ShellUtilities-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ShellUtilities
-Version: 2.1.8
+Version: 2.1.9
 Summary: A library for executing shell commands in either a blocking or non-blocking way.
 Home-page: https://github.com/taylor-schneider/ShellUtilities
 Author: tschneider
 Author-email: tschneider@live.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `ShellUtilities-2.1.8/README.md` & `ShellUtilities-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ShellUtilities-2.1.8/setup.py` & `ShellUtilities-2.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 with open('README.md', "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="ShellUtilities",
-    version="2.1.8",
+    version="2.1.9",
     author="tschneider",
     author_email="tschneider@live.com",
     description="A library for executing shell commands in either a blocking or non-blocking way.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(source_code_dir),
     package_dir={
```

### Comparing `ShellUtilities-2.1.8/src/ShellUtilities/Shell.py` & `ShellUtilities-2.1.9/src/ShellUtilities/Shell.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,16 +71,24 @@
             # Run the shell command
             if blocking:
                 exitcode, stdout_string, stderr_string = __execute_shell_command(command, env, cwd, executable)
             else:
                 process = __execute_shell_command_async(command, env, cwd, executable)
                 return AsynchronousShellCommandResults(command, process, async_buffer_funcs)
 
-            # Set the exit code and return
+            # If successful, return the results
             if exitcode == 0:
+                logging.debug("Command STDOUT:")
+                for line in stdout_string.split("\n"):
+                    if line:
+                        logging.debug(line)
+                logging.debug("Command STDERR:")
+                for line in stderr_string.split("\n"):
+                    if line:
+                        logging.error(line)
                 return ShellCommandResults(command, stdout_string, stderr_string, exitcode)
 
             # If an error occured we need to determine if this is the last retry attempt
             last_retry = i == max_retries - 1
 
             # If it is not the last retry we must determine whether or not we can ignore the error
             # To do this we must see if our retry conditions have been satisfied
```

### Comparing `ShellUtilities-2.1.8/src/ShellUtilities/ShellCommandException.py` & `ShellUtilities-2.1.9/src/ShellUtilities/ShellCommandException.py`

 * *Files identical despite different names*

### Comparing `ShellUtilities-2.1.8/src/ShellUtilities/ShellCommandResults.py` & `ShellUtilities-2.1.9/src/ShellUtilities/ShellCommandResults.py`

 * *Files identical despite different names*

### Comparing `ShellUtilities-2.1.8/src/ShellUtilities.egg-info/PKG-INFO` & `ShellUtilities-2.1.9/src/ShellUtilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ShellUtilities
-Version: 2.1.8
+Version: 2.1.9
 Summary: A library for executing shell commands in either a blocking or non-blocking way.
 Home-page: https://github.com/taylor-schneider/ShellUtilities
 Author: tschneider
 Author-email: tschneider@live.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `ShellUtilities-2.1.8/tests/test_Shell.py` & `ShellUtilities-2.1.9/tests/test_Shell.py`

 * *Files identical despite different names*

