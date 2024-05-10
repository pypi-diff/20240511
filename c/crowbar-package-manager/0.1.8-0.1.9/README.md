# Comparing `tmp/crowbar_package_manager-0.1.8.tar.gz` & `tmp/crowbar_package_manager-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crowbar_package_manager-0.1.8.tar", last modified: Sat Apr 13 00:20:41 2024, max compression
+gzip compressed data, was "crowbar_package_manager-0.1.9.tar", last modified: Fri Apr 19 20:17:39 2024, max compression
```

## Comparing `crowbar_package_manager-0.1.8.tar` & `crowbar_package_manager-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-13 00:20:41.260911 crowbar_package_manager-0.1.8/
--rw-r--r--   0 coryfitz   (501) staff       (20)     1281 2024-04-13 00:20:41.260763 crowbar_package_manager-0.1.8/PKG-INFO
--rw-r--r--   0 coryfitz   (501) staff       (20)     1102 2024-04-13 00:19:40.000000 crowbar_package_manager-0.1.8/README.md
-drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-13 00:20:41.259486 crowbar_package_manager-0.1.8/crowbar/
--rw-r--r--   0 coryfitz   (501) staff       (20)       25 2024-04-07 23:29:44.000000 crowbar_package_manager-0.1.8/crowbar/__init__.py
--rw-r--r--   0 coryfitz   (501) staff       (20)     8976 2024-04-13 00:14:00.000000 crowbar_package_manager-0.1.8/crowbar/crowbar.py
-drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-13 00:20:41.260520 crowbar_package_manager-0.1.8/crowbar_package_manager.egg-info/
--rw-r--r--   0 coryfitz   (501) staff       (20)     1281 2024-04-13 00:20:41.000000 crowbar_package_manager-0.1.8/crowbar_package_manager.egg-info/PKG-INFO
--rw-r--r--   0 coryfitz   (501) staff       (20)      295 2024-04-13 00:20:41.000000 crowbar_package_manager-0.1.8/crowbar_package_manager.egg-info/SOURCES.txt
--rw-r--r--   0 coryfitz   (501) staff       (20)        1 2024-04-13 00:20:41.000000 crowbar_package_manager-0.1.8/crowbar_package_manager.egg-info/dependency_links.txt
--rw-r--r--   0 coryfitz   (501) staff       (20)       59 2024-04-13 00:20:41.000000 crowbar_package_manager-0.1.8/crowbar_package_manager.egg-info/entry_points.txt
--rw-r--r--   0 coryfitz   (501) staff       (20)        8 2024-04-13 00:20:41.000000 crowbar_package_manager-0.1.8/crowbar_package_manager.egg-info/top_level.txt
--rw-r--r--   0 coryfitz   (501) staff       (20)       38 2024-04-13 00:20:41.260979 crowbar_package_manager-0.1.8/setup.cfg
--rw-r--r--   0 coryfitz   (501) staff       (20)      653 2024-04-13 00:20:26.000000 crowbar_package_manager-0.1.8/setup.py
+drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-19 20:17:39.972956 crowbar_package_manager-0.1.9/
+-rw-r--r--   0 coryfitz   (501) staff       (20)     1643 2024-04-19 20:17:39.972822 crowbar_package_manager-0.1.9/PKG-INFO
+-rw-r--r--   0 coryfitz   (501) staff       (20)     1464 2024-04-19 20:13:24.000000 crowbar_package_manager-0.1.9/README.md
+drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-19 20:17:39.971835 crowbar_package_manager-0.1.9/crowbar/
+-rw-r--r--   0 coryfitz   (501) staff       (20)       25 2024-04-07 23:29:44.000000 crowbar_package_manager-0.1.9/crowbar/__init__.py
+-rw-r--r--   0 coryfitz   (501) staff       (20)     3463 2024-04-19 20:01:18.000000 crowbar_package_manager-0.1.9/crowbar/crowbar.py
+drwxr-xr-x   0 coryfitz   (501) staff       (20)        0 2024-04-19 20:17:39.972630 crowbar_package_manager-0.1.9/crowbar_package_manager.egg-info/
+-rw-r--r--   0 coryfitz   (501) staff       (20)     1643 2024-04-19 20:17:39.000000 crowbar_package_manager-0.1.9/crowbar_package_manager.egg-info/PKG-INFO
+-rw-r--r--   0 coryfitz   (501) staff       (20)      295 2024-04-19 20:17:39.000000 crowbar_package_manager-0.1.9/crowbar_package_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 coryfitz   (501) staff       (20)        1 2024-04-19 20:17:39.000000 crowbar_package_manager-0.1.9/crowbar_package_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 coryfitz   (501) staff       (20)       59 2024-04-19 20:17:39.000000 crowbar_package_manager-0.1.9/crowbar_package_manager.egg-info/entry_points.txt
+-rw-r--r--   0 coryfitz   (501) staff       (20)        8 2024-04-19 20:17:39.000000 crowbar_package_manager-0.1.9/crowbar_package_manager.egg-info/top_level.txt
+-rw-r--r--   0 coryfitz   (501) staff       (20)       38 2024-04-19 20:17:39.973006 crowbar_package_manager-0.1.9/setup.cfg
+-rw-r--r--   0 coryfitz   (501) staff       (20)      653 2024-04-19 20:17:29.000000 crowbar_package_manager-0.1.9/setup.py
```

### Comparing `crowbar_package_manager-0.1.8/PKG-INFO` & `crowbar_package_manager-0.1.9/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-Metadata-Version: 2.1
-Name: crowbar_package_manager
-Version: 0.1.8
-Summary: a local-first tool for managing python dependencies with pip
-Description-Content-Type: text/markdown
-
 ## crowbar
 
 Note: any instance of ```crowbar``` can be replaced with ```cb```
 
 
 ```
 crowbar install <package_name> <package_name>
@@ -30,20 +24,44 @@
 ```
 crowbar run <file_name>.py
 ```
 -Runs a python file using the contents of the local venv
 
 Warning – you may have pip muscle memory which may cause you to accidentally install globally. Use crowbar/cb and not pip if you are not in an active virtual environment.
 
+<br>
+
 ### global flag
 
 ```
 crowbar --global install <package_name>
 ```
 ```
 cb -g uninstall <package_name>
 ```
 -installs or uninstalls a package globally
 
-### conda support
+<br>
+
+### running package commands
+
+With the crowbar command you can run any commands installed in the virtual environment.
+
+Example - starting a new Django project:
+
+```
+cb django-admin startproject django_project .
+```
+
+Use ```crowbar run``` to run any commands surfaced by files within your Python program.
+
+Example - running the Django development server:
+
+```
+cb run manage.py runserver
+```
+
+<br>
+
+### package managers other than pip
 
-Crowbar supports python and will create an environment called conda_env instead of venv if it detects that it is within a conda environment.
+Crowbar does not support Conda. Crowbar has plans to support UV eventually.
```

### Comparing `crowbar_package_manager-0.1.8/crowbar_package_manager.egg-info/PKG-INFO` & `crowbar_package_manager-0.1.9/crowbar_package_manager.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crowbar-package-manager
-Version: 0.1.8
+Version: 0.1.9
 Summary: a local-first tool for managing python dependencies with pip
 Description-Content-Type: text/markdown
 
 ## crowbar
 
 Note: any instance of ```crowbar``` can be replaced with ```cb```
 
@@ -30,20 +30,44 @@
 ```
 crowbar run <file_name>.py
 ```
 -Runs a python file using the contents of the local venv
 
 Warning – you may have pip muscle memory which may cause you to accidentally install globally. Use crowbar/cb and not pip if you are not in an active virtual environment.
 
+<br>
+
 ### global flag
 
 ```
 crowbar --global install <package_name>
 ```
 ```
 cb -g uninstall <package_name>
 ```
 -installs or uninstalls a package globally
 
-### conda support
+<br>
+
+### running package commands
+
+With the crowbar command you can run any commands installed in the virtual environment.
+
+Example - starting a new Django project:
+
+```
+cb django-admin startproject django_project .
+```
+
+Use ```crowbar run``` to run any commands surfaced by files within your Python program.
+
+Example - running the Django development server:
+
+```
+cb run manage.py runserver
+```
+
+<br>
+
+### package managers other than pip
 
-Crowbar supports python and will create an environment called conda_env instead of venv if it detects that it is within a conda environment.
+Crowbar does not support Conda. Crowbar has plans to support UV eventually.
```

### Comparing `crowbar_package_manager-0.1.8/setup.py` & `crowbar_package_manager-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='crowbar_package_manager',
-    version='0.1.8',
+    version='0.1.9',
     packages=find_packages(),
     install_requires=[],
     entry_points={
         'console_scripts': [
             'crowbar=crowbar:main',
             'cb=crowbar:main',
         ],
```

