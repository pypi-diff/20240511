# Comparing `tmp/runner_v1-0.0.0.tar.gz` & `tmp/runner_v1-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runner_v1-0.0.0.tar", max compression
+gzip compressed data, was "runner_v1-0.1.0.tar", max compression
```

## Comparing `runner_v1-0.0.0.tar` & `runner_v1-0.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      278 2024-05-10 08:33:30.321158 runner_v1-0.0.0/README.md
--rw-r--r--   0        0        0      513 2024-05-10 10:02:49.085023 runner_v1-0.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-10 07:15:40.540219 runner_v1-0.0.0/runner/__init__.py
--rw-r--r--   0        0        0     3193 2024-05-10 10:11:50.875934 runner_v1-0.0.0/runner/__main__.py
--rw-r--r--   0        0        0      133 2024-05-10 07:53:50.737020 runner_v1-0.0.0/runner/runner.toml
--rw-r--r--   0        0        0      871 1970-01-01 00:00:00.000000 runner_v1-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0      497 2024-05-10 14:39:05.572920 runner_v1-0.1.0/README.md
+-rw-r--r--   0        0        0      513 2024-05-10 14:39:14.551262 runner_v1-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-10 07:15:40.540219 runner_v1-0.1.0/runner/__init__.py
+-rw-r--r--   0        0        0     3193 2024-05-10 10:11:50.875934 runner_v1-0.1.0/runner/__main__.py
+-rw-r--r--   0        0        0      133 2024-05-10 07:53:50.737020 runner_v1-0.1.0/runner/runner.toml
+-rw-r--r--   0        0        0     1090 1970-01-01 00:00:00.000000 runner_v1-0.1.0/PKG-INFO
```

### Comparing `runner_v1-0.0.0/pyproject.toml` & `runner_v1-0.1.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "runner-v1"
-version = "0.0.0"
+version = "0.1.0"
 description = "script runner"
 authors = ["kagemeka <kagemeka1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 package-mode = true
 packages = [{ include = "runner" }]
 include = ["runner.toml"]
```

### Comparing `runner_v1-0.0.0/runner/__main__.py` & `runner_v1-0.1.0/runner/__main__.py`

 * *Files identical despite different names*

### Comparing `runner_v1-0.0.0/PKG-INFO` & `runner_v1-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runner-v1
-Version: 0.0.0
+Version: 0.1.0
 Summary: script runner
 License: MIT
 Author: kagemeka
 Author-email: kagemeka1@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,27 +16,46 @@
 Requires-Dist: toml (==0.10.2)
 Description-Content-Type: text/markdown
 
 # runner
 
 ## usage
 
+### configuratioins
+
+```sh
+pip install runner-v1
+```
+
+make `runner.toml` in your project directory.
+
 required
 profile.name, profile.run, from_ext.ext, from_ext.profile
 
 optional
 profile.pre_run, profile.post_run
 
 ```toml
 [[profile]]
 name = 'c++'
 pre_run = 'g++ -O2 <file>'
 run = './a.out'
 post_run = 'rm a.out'
 
+[[profile]]
+name = 'python'
+run = 'python <file>'
 
 [[from_ext]]
 ext = 'cpp'
 profile = 'c++'
 
+[[from_ext]]
+ext = 'py'
+profile = 'python'
+
+```
+
+```sh
+run main.cpp
 ```
```

