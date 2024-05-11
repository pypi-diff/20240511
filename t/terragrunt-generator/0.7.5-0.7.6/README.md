# Comparing `tmp/terragrunt-generator-0.7.5.tar.gz` & `tmp/terragrunt_generator-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terragrunt-generator-0.7.5.tar", last modified: Sat Jan 20 20:17:38 2024, max compression
+gzip compressed data, was "terragrunt_generator-0.7.6.tar", last modified: Sat May 11 14:46:58 2024, max compression
```

## Comparing `terragrunt-generator-0.7.5.tar` & `terragrunt_generator-0.7.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:17:38.023511 terragrunt-generator-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-20 20:17:24.000000 terragrunt-generator-0.7.5/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)    21692 2024-01-20 20:17:38.023511 terragrunt-generator-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21046 2024-01-20 20:17:24.000000 terragrunt-generator-0.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:17:38.019511 terragrunt-generator-0.7.5/generator/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-01-20 20:17:29.000000 terragrunt-generator-0.7.5/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-20 20:17:24.000000 terragrunt-generator-0.7.5/generator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-01-20 20:17:24.000000 terragrunt-generator-0.7.5/generator/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-01-20 20:17:24.000000 terragrunt-generator-0.7.5/generator/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-01-20 20:17:24.000000 terragrunt-generator-0.7.5/generator/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-01-20 20:17:24.000000 terragrunt-generator-0.7.5/generator/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-01-20 20:17:24.000000 terragrunt-generator-0.7.5/generator/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-01-20 20:17:24.000000 terragrunt-generator-0.7.5/generator/yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-01-20 20:17:29.000000 terragrunt-generator-0.7.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-20 20:17:38.023511 terragrunt-generator-0.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-01-20 20:17:24.000000 terragrunt-generator-0.7.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:17:38.023511 terragrunt-generator-0.7.5/terragrunt_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21692 2024-01-20 20:17:38.000000 terragrunt-generator-0.7.5/terragrunt_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-01-20 20:17:38.000000 terragrunt-generator-0.7.5/terragrunt_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-20 20:17:38.000000 terragrunt-generator-0.7.5/terragrunt_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-20 20:17:38.000000 terragrunt-generator-0.7.5/terragrunt_generator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-01-20 20:17:38.000000 terragrunt-generator-0.7.5/terragrunt_generator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-20 20:17:38.000000 terragrunt-generator-0.7.5/terragrunt_generator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:17:38.023511 terragrunt-generator-0.7.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 20:17:24.000000 terragrunt-generator-0.7.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-01-20 20:17:24.000000 terragrunt-generator-0.7.5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    15916 2024-01-20 20:17:24.000000 terragrunt-generator-0.7.5/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-01-20 20:17:24.000000 terragrunt-generator-0.7.5/tests/test_get_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-01-20 20:17:24.000000 terragrunt-generator-0.7.5/tests/test_git.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-01-20 20:17:24.000000 terragrunt-generator-0.7.5/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-01-20 20:17:24.000000 terragrunt-generator-0.7.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:46:58.162025 terragrunt_generator-0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-11 14:46:49.000000 terragrunt_generator-0.7.6/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)    21692 2024-05-11 14:46:58.162025 terragrunt_generator-0.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21046 2024-05-11 14:46:49.000000 terragrunt_generator-0.7.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:46:58.158025 terragrunt_generator-0.7.6/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-11 14:46:53.000000 terragrunt_generator-0.7.6/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-11 14:46:49.000000 terragrunt_generator-0.7.6/generator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-05-11 14:46:49.000000 terragrunt_generator-0.7.6/generator/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-11 14:46:49.000000 terragrunt_generator-0.7.6/generator/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-11 14:46:49.000000 terragrunt_generator-0.7.6/generator/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-11 14:46:49.000000 terragrunt_generator-0.7.6/generator/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-11 14:46:49.000000 terragrunt_generator-0.7.6/generator/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-11 14:46:49.000000 terragrunt_generator-0.7.6/generator/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-11 14:46:53.000000 terragrunt_generator-0.7.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 14:46:58.162025 terragrunt_generator-0.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-11 14:46:49.000000 terragrunt_generator-0.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:46:58.162025 terragrunt_generator-0.7.6/terragrunt_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21692 2024-05-11 14:46:58.000000 terragrunt_generator-0.7.6/terragrunt_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-11 14:46:58.000000 terragrunt_generator-0.7.6/terragrunt_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 14:46:58.000000 terragrunt_generator-0.7.6/terragrunt_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-11 14:46:58.000000 terragrunt_generator-0.7.6/terragrunt_generator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-11 14:46:58.000000 terragrunt_generator-0.7.6/terragrunt_generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-11 14:46:58.000000 terragrunt_generator-0.7.6/terragrunt_generator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:46:58.162025 terragrunt_generator-0.7.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 14:46:49.000000 terragrunt_generator-0.7.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-11 14:46:49.000000 terragrunt_generator-0.7.6/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15916 2024-05-11 14:46:49.000000 terragrunt_generator-0.7.6/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-11 14:46:49.000000 terragrunt_generator-0.7.6/tests/test_get_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-11 14:46:49.000000 terragrunt_generator-0.7.6/tests/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-11 14:46:49.000000 terragrunt_generator-0.7.6/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-11 14:46:49.000000 terragrunt_generator-0.7.6/tests/test_utils.py
```

### Comparing `terragrunt-generator-0.7.5/COPYING` & `terragrunt_generator-0.7.6/COPYING`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.7.5/PKG-INFO` & `terragrunt_generator-0.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terragrunt-generator
-Version: 0.7.5
+Version: 0.7.6
 Summary: generate terragrunt manifest from terraform module.
 Author: Chris
 Author-email: goabonga@pm.me
 Description-Content-Type: text/markdown
 License-File: COPYING
 Requires-Dist: python-hcl2==3.0.5
 Requires-Dist: GitPython==3.1.41
```

### Comparing `terragrunt-generator-0.7.5/README.md` & `terragrunt_generator-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.7.5/generator/generate.py` & `terragrunt_generator-0.7.6/generator/generate.py`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.7.5/generator/main.py` & `terragrunt_generator-0.7.6/generator/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import argparse
-from distutils.dir_util import copy_tree
+from shutil import copytree
 from tempfile import gettempdir
 from uuid import uuid4
 
 from generator import __version__
 from generator.generate import generate
 from generator.git import clone
 from generator.reader import read_directory
@@ -39,15 +39,15 @@
 def create_working_directory() -> str:
     tempdir = f'{gettempdir()}/{uuid4()}'
     return tempdir
 
 
 def copy_terraform_module(url: str, version: str, path: str):
     if is_local(url):
-        copy_tree(url, path)
+        copytree(url, path)
     else:
         clone(url, path, version)
 
 
 def main(args=None):
     args: map = parser.parse_args(args)
```

### Comparing `terragrunt-generator-0.7.5/generator/yaml.py` & `terragrunt_generator-0.7.6/generator/yaml.py`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.7.5/pyproject.toml` & `terragrunt_generator-0.7.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -19,13 +19,13 @@
   | build
   | dist
 )/
 '''
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.7.5"
+version = "0.7.6"
 tag_format = "$major.$minor.$patch$prerelease"
 version_files = [
     "pyproject.toml:version",
     "generator/__init__.py",
 ]
```

### Comparing `terragrunt-generator-0.7.5/setup.py` & `terragrunt_generator-0.7.6/setup.py`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.7.5/terragrunt_generator.egg-info/PKG-INFO` & `terragrunt_generator-0.7.6/terragrunt_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terragrunt-generator
-Version: 0.7.5
+Version: 0.7.6
 Summary: generate terragrunt manifest from terraform module.
 Author: Chris
 Author-email: goabonga@pm.me
 Description-Content-Type: text/markdown
 License-File: COPYING
 Requires-Dist: python-hcl2==3.0.5
 Requires-Dist: GitPython==3.1.41
```

### Comparing `terragrunt-generator-0.7.5/terragrunt_generator.egg-info/SOURCES.txt` & `terragrunt_generator-0.7.6/terragrunt_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.7.5/tests/test_cli.py` & `terragrunt_generator-0.7.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.7.5/tests/test_generate.py` & `terragrunt_generator-0.7.6/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.7.5/tests/test_get_yaml.py` & `terragrunt_generator-0.7.6/tests/test_get_yaml.py`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.7.5/tests/test_reader.py` & `terragrunt_generator-0.7.6/tests/test_reader.py`

 * *Files identical despite different names*

