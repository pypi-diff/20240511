# Comparing `tmp/packaged-0.1.0.tar.gz` & `tmp/packaged-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packaged-0.1.0.tar", last modified: Fri May 10 11:08:21 2024, max compression
+gzip compressed data, was "packaged-0.1.1.tar", last modified: Sat May 11 01:07:12 2024, max compression
```

## Comparing `packaged-0.1.0.tar` & `packaged-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-10 11:08:21.354122 packaged-0.1.0/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1072 2024-05-04 21:39:47.000000 packaged-0.1.0/LICENSE
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2385 2024-05-10 11:08:21.354053 packaged-0.1.0/PKG-INFO
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1270 2024-05-09 19:03:38.000000 packaged-0.1.0/README.md
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1233 2024-05-10 11:08:21.354421 packaged-0.1.0/setup.cfg
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       37 2024-05-09 19:00:34.000000 packaged-0.1.0/setup.py
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-10 11:08:21.351313 packaged-0.1.0/src/
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-10 11:08:21.352647 packaged-0.1.0/src/packaged/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3778 2024-05-10 11:05:33.000000 packaged-0.1.0/src/packaged/__init__.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      184 2024-05-04 21:39:47.000000 packaged-0.1.0/src/packaged/__main__.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1308 2024-05-08 23:09:57.000000 packaged-0.1.0/src/packaged/cli.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       59 2024-05-04 21:39:47.000000 packaged-0.1.0/src/packaged/py.typed
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)        0 2024-05-08 21:00:51.000000 packaged-0.1.0/src/packaged/startup.template.sh
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-10 11:08:21.353575 packaged-0.1.0/src/packaged.egg-info/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2385 2024-05-10 11:08:21.000000 packaged-0.1.0/src/packaged.egg-info/PKG-INFO
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      379 2024-05-10 11:08:21.000000 packaged-0.1.0/src/packaged.egg-info/SOURCES.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)        1 2024-05-10 11:08:21.000000 packaged-0.1.0/src/packaged.egg-info/dependency_links.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       46 2024-05-10 11:08:21.000000 packaged-0.1.0/src/packaged.egg-info/entry_points.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       51 2024-05-10 11:08:21.000000 packaged-0.1.0/src/packaged.egg-info/requires.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)        9 2024-05-10 11:08:21.000000 packaged-0.1.0/src/packaged.egg-info/top_level.txt
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-11 01:07:12.427004 packaged-0.1.1/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1072 2024-05-04 21:39:47.000000 packaged-0.1.1/LICENSE
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2426 2024-05-11 01:07:12.426928 packaged-0.1.1/PKG-INFO
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1267 2024-05-11 01:01:30.000000 packaged-0.1.1/README.md
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1254 2024-05-11 01:07:12.427318 packaged-0.1.1/setup.cfg
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       37 2024-05-09 19:00:34.000000 packaged-0.1.1/setup.py
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-11 01:07:12.424192 packaged-0.1.1/src/
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-11 01:07:12.425291 packaged-0.1.1/src/packaged/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     4038 2024-05-10 23:59:49.000000 packaged-0.1.1/src/packaged/__init__.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      184 2024-05-04 21:39:47.000000 packaged-0.1.1/src/packaged/__main__.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1308 2024-05-10 23:59:49.000000 packaged-0.1.1/src/packaged/cli.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       59 2024-05-04 21:39:47.000000 packaged-0.1.1/src/packaged/py.typed
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-11 01:07:12.426372 packaged-0.1.1/src/packaged.egg-info/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2426 2024-05-11 01:07:12.000000 packaged-0.1.1/src/packaged.egg-info/PKG-INFO
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      346 2024-05-11 01:07:12.000000 packaged-0.1.1/src/packaged.egg-info/SOURCES.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        1 2024-05-11 01:07:12.000000 packaged-0.1.1/src/packaged.egg-info/dependency_links.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       46 2024-05-11 01:07:12.000000 packaged-0.1.1/src/packaged.egg-info/entry_points.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       64 2024-05-11 01:07:12.000000 packaged-0.1.1/src/packaged.egg-info/requires.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        9 2024-05-11 01:07:12.000000 packaged-0.1.1/src/packaged.egg-info/top_level.txt
```

### Comparing `packaged-0.1.0/LICENSE` & `packaged-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `packaged-0.1.0/PKG-INFO` & `packaged-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packaged
-Version: 0.1.0
+Version: 0.1.1
 Summary: The easiest way to ship python applications.
 Home-page: https://github.com/tusharsadhwani/packaged
 Author: Tushar Sadhwani
 Author-email: tushar.sadhwani000@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,14 +22,15 @@
 License-File: LICENSE
 Requires-Dist: yen>=0.4.2
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 
 # packaged
 
 The easiest way to ship python applications.
 
 ## Installation
@@ -37,34 +38,32 @@
 ```bash
 pip install packaged
 ```
 
 ## Usage
 
 ```bash
-packaged <source_directory> <output_file> <build_command> <startup_command>
+packaged <source_directory> <output_path> <build_command> <startup_command>
 ```
 
 Such as:
 
 ```bash
 packaged path/to/project my_project.bin 'pip install .' 'python -m your_package'
 ```
 
 ### Example
 
 There's an `example` folder where you can test this:
 
 ```bash
-pip install packaged
-cd example
-packaged . curve 'pip install -r requirements.txt' 'python bubble_sort_curve.py'
+packaged ./example/matplotlib ./curve.bin 'pip install -r requirements.txt' 'python bubble_sort_curve.py'
 ```
 
-This produces a `./curve` binary with:
+This produces a `./curve.bin` binary with:
 
 - Python 3.11
 - `matplotlib`
 - `numba`
 - `llvmlite`
 - `pillow`
```

### Comparing `packaged-0.1.0/README.md` & `packaged-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -7,34 +7,32 @@
 ```bash
 pip install packaged
 ```
 
 ## Usage
 
 ```bash
-packaged <source_directory> <output_file> <build_command> <startup_command>
+packaged <source_directory> <output_path> <build_command> <startup_command>
 ```
 
 Such as:
 
 ```bash
 packaged path/to/project my_project.bin 'pip install .' 'python -m your_package'
 ```
 
 ### Example
 
 There's an `example` folder where you can test this:
 
 ```bash
-pip install packaged
-cd example
-packaged . curve 'pip install -r requirements.txt' 'python bubble_sort_curve.py'
+packaged ./example/matplotlib ./curve.bin 'pip install -r requirements.txt' 'python bubble_sort_curve.py'
 ```
 
-This produces a `./curve` binary with:
+This produces a `./curve.bin` binary with:
 
 - Python 3.11
 - `matplotlib`
 - `numba`
 - `llvmlite`
 - `pillow`
```

### Comparing `packaged-0.1.0/setup.cfg` & `packaged-0.1.1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = packaged
-version = 0.1.0
+version = 0.1.1
 description = The easiest way to ship python applications.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tusharsadhwani/packaged
 author = Tushar Sadhwani
 author_email = tushar.sadhwani000@gmail.com
 license = MIT
@@ -38,21 +38,22 @@
 
 [options.extras_require]
 dev = 
 	black
 	mypy
 	pytest
 	pytest-cov
+	pytest-xdist
 	tox
 
 [options.package_data]
 packaged = 
 	py.typed
 	startup.template.sh
 
 [tool:pytest]
-addopts = --cov --cov-report=term-missing
+addopts = --cov --cov-report=term-missing -nauto
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `packaged-0.1.0/src/packaged/__init__.py` & `packaged-0.1.1/src/packaged/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import os.path
 import shutil
 import subprocess
 import urllib.request
 
 import yen
 
-STARTUP_TEMPLATE_PATH = os.path.join(os.path.dirname(__file__), "startup.template.sh")
 
 MAKESELF_VERSION = "2.5.0"
 MAKESELF_DOWNLOAD_URL = (
     "https://github.com/megastep/makeself/releases/download/"
     f"release-{MAKESELF_VERSION}/makeself-{MAKESELF_VERSION}.run"
 )
 MAKESELF_DOWNLOAD_PATH = os.path.join(os.path.dirname(__file__), ".build_deps")
@@ -39,69 +38,72 @@
         stdout=subprocess.DEVNULL,
         stderr=subprocess.DEVNULL,
         cwd=MAKESELF_DOWNLOAD_PATH,
     )
 
 
 def create_package(
-    source_directory: str, output_file: str, build_command: str, startup_command: str
+    source_directory: str, output_path: str, build_command: str, startup_command: str
 ) -> None:
     """Create the makeself executable, with the startup script in it."""
     startup_script_name = "_packaged_startup.sh"
+    startup_script_path = os.path.join(source_directory, startup_script_name)
 
     packaged_python_path = os.path.join(source_directory, ".packaged_python")
     if os.path.exists(packaged_python_path):
         shutil.rmtree(packaged_python_path)
 
     try:
-        python_version, python_bin_path = yen.ensure_python("3.11")
-        python_path = os.path.join(yen.PYTHON_INSTALLS_PATH, python_version)
-        python_bin_relpath = os.path.relpath(python_bin_path, python_path)
-
-        # Copy the startup script to the source directory
-        startup_script_path = shutil.copyfile(
-            STARTUP_TEMPLATE_PATH, os.path.join(source_directory, startup_script_name)
-        )
+        # Use `yen` to ensure a portable Python is present on the system
+        python_version, yen_python_bin_path = yen.ensure_python("3.11")
+        yen_python_path = os.path.join(yen.PYTHON_INSTALLS_PATH, python_version)
+        yen_python_bin_relpath = os.path.relpath(yen_python_bin_path, yen_python_path)
 
         # Put a standalone python interpreter inside the package
-        shutil.copytree(python_path, packaged_python_path)
+        shutil.copytree(yen_python_path, packaged_python_path)
 
-        # Get the bin folder path relative to source directory
+        # Get the `python/bin` folder path relative to source directory
         python_bin_folder = os.path.join(
-            packaged_python_path, os.path.dirname(python_bin_relpath)
+            packaged_python_path, os.path.dirname(yen_python_bin_relpath)
         )
         python_bin_folder_relpath = os.path.relpath(python_bin_folder, source_directory)
 
         # Run the build command in the source directory, while making sure
         # that `python` and related binaries point to the installed python
         subprocess.check_call(
             [build_command],
             shell=True,
             env={
                 "PATH": os.pathsep.join([python_bin_folder, os.environ.get("PATH", "")])
             },
             cwd=source_directory,
         )
 
-        # Add the startup command right at the end of the startup script
-        with open(startup_script_path, "a") as startup_file:
+        # The startup script is simply the startup command, prepended with a PATH
+        # change to ensure that `python` refers to the bundled python.
+        with open(startup_script_path, "w") as startup_file:
             startup_file.write(f"PATH={python_bin_folder_relpath}:$PATH\n")
             startup_file.write(startup_command)
 
         os.chmod(startup_script_path, 0o777)
 
+        # This uses `makeself` to build the binary
         subprocess.check_call(
             [
                 MAKESELF_PATH,
+                # Path to package
                 source_directory,
-                output_file,
-                output_file,
-                # makeself wants the startup script path to be a relative path
+                # Filename to output
+                output_path,
+                # Label for the package, for now it's just the filename
+                output_path,
+                # The command to run when starting the package.
+                # `makeself` wants the startup script path to be a relative path
                 os.path.join(".", startup_script_name),
             ],
         )
     finally:
-        # Cleanup the packaged python and startup script
+        # Cleanup the packaged python and startup script from source directory
         if os.path.exists(startup_script_path):
             os.remove(startup_script_path)
         if os.path.exists(packaged_python_path):
             shutil.rmtree(packaged_python_path)
```

### Comparing `packaged-0.1.0/src/packaged/cli.py` & `packaged-0.1.1/src/packaged/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import platform
 
 from packaged import ensure_makeself, create_package
 
 
 class CLIArgs:
     source_directory: str
-    output_file: str
+    output_path: str
     build_command: str
     startup_command: str
 
 
 def error(message: str) -> None:
     """Print error message"""
     print(f"\033[1;31mError:\033[m {message}")
@@ -25,27 +25,27 @@
     """CLI interface."""
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "source_directory",
         help="folder containing your python source to package",
         type=os.path.abspath,
     )
-    parser.add_argument("output_file", help="Filename for the generated binary")
+    parser.add_argument("output_path", help="Filename for the generated binary")
     parser.add_argument(
         "build_command", help="Python command to run when building the package"
     )
     parser.add_argument("startup_command", help="Command to run when the script starts")
     args = parser.parse_args(argv, namespace=CLIArgs)
 
     if platform.system() == "Windows":
         error("Sorry, Windows is not supported yet. Ask for it on GitHub!")
         return 2
 
     ensure_makeself()
     create_package(
         args.source_directory,
-        args.output_file,
+        args.output_path,
         args.build_command,
         args.startup_command,
     )
 
     return 0
```

### Comparing `packaged-0.1.0/src/packaged.egg-info/PKG-INFO` & `packaged-0.1.1/src/packaged.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packaged
-Version: 0.1.0
+Version: 0.1.1
 Summary: The easiest way to ship python applications.
 Home-page: https://github.com/tusharsadhwani/packaged
 Author: Tushar Sadhwani
 Author-email: tushar.sadhwani000@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,14 +22,15 @@
 License-File: LICENSE
 Requires-Dist: yen>=0.4.2
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 
 # packaged
 
 The easiest way to ship python applications.
 
 ## Installation
@@ -37,34 +38,32 @@
 ```bash
 pip install packaged
 ```
 
 ## Usage
 
 ```bash
-packaged <source_directory> <output_file> <build_command> <startup_command>
+packaged <source_directory> <output_path> <build_command> <startup_command>
 ```
 
 Such as:
 
 ```bash
 packaged path/to/project my_project.bin 'pip install .' 'python -m your_package'
 ```
 
 ### Example
 
 There's an `example` folder where you can test this:
 
 ```bash
-pip install packaged
-cd example
-packaged . curve 'pip install -r requirements.txt' 'python bubble_sort_curve.py'
+packaged ./example/matplotlib ./curve.bin 'pip install -r requirements.txt' 'python bubble_sort_curve.py'
 ```
 
-This produces a `./curve` binary with:
+This produces a `./curve.bin` binary with:
 
 - Python 3.11
 - `matplotlib`
 - `numba`
 - `llvmlite`
 - `pillow`
```

