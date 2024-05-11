# Comparing `tmp/revolutioneeringz-1.1.tar.gz` & `tmp/revolutioneeringz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revolutioneeringz-1.1.tar", last modified: Thu May  9 04:33:13 2024, max compression
+gzip compressed data, was "revolutioneeringz-2.1.tar", last modified: Sat May 11 13:54:56 2024, max compression
```

## Comparing `revolutioneeringz-1.1.tar` & `revolutioneeringz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 04:33:13.479225 revolutioneeringz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1684 2024-05-09 04:33:13.479225 revolutioneeringz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 04:33:13.475225 revolutioneeringz-1.1/revolutioneeringz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 04:33:11.827194 revolutioneeringz-1.1/revolutioneeringz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 04:33:12.031198 revolutioneeringz-1.1/revolutioneeringz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 04:33:11.827194 revolutioneeringz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1654 2024-05-09 04:33:12.387205 revolutioneeringz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 13:54:56.401275 revolutioneeringz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 04:33:11.000000 revolutioneeringz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1982 2024-05-11 13:54:56.401275 revolutioneeringz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 04:33:11.000000 revolutioneeringz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 13:54:56.401275 revolutioneeringz-2.1/revolutioneeringz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 04:33:11.000000 revolutioneeringz-2.1/revolutioneeringz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 04:33:12.000000 revolutioneeringz-2.1/revolutioneeringz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 13:54:56.401275 revolutioneeringz-2.1/revolutioneeringz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1982 2024-05-11 13:54:56.000000 revolutioneeringz-2.1/revolutioneeringz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      296 2024-05-11 13:54:56.000000 revolutioneeringz-2.1/revolutioneeringz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 13:54:56.000000 revolutioneeringz-2.1/revolutioneeringz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 13:54:56.000000 revolutioneeringz-2.1/revolutioneeringz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       18 2024-05-11 13:54:56.000000 revolutioneeringz-2.1/revolutioneeringz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 13:54:56.405275 revolutioneeringz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1654 2024-05-11 13:54:55.000000 revolutioneeringz-2.1/setup.py
```

### Comparing `revolutioneeringz-1.1/PKG-INFO` & `revolutioneeringz-2.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,51 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: revolutioneeringz
-Version: 1.1
+Version: 2.1
 Summary: revolutioneeringz
 Home-page: https://github.com/mirukutea/revolutioneeringz
+Download-URL: https://github.com/mirukutea/revolutioneeringz/archive/v_01.tar.gz
 Author: Mirukutea
 Author-email: tea@masrizky.com
 License: MIT
-Download-URL: https://github.com/mirukutea/revolutioneeringz/archive/v_01.tar.gz
-Description: # Python library quick start
-        This is a minimal template for uploading your python packages to pypi.org.
-        
-        ## To Use
-        * First clone this project.
-        ```bash
-        # Clone this repository
-        git clone https://github.com/defartsa23/python-library-quick-start.git
-        # Go into the repository
-        cd python-library-quick-start
-        ```
-        * Rename the folder `your-package` to the package name you want. then place all your files into a folder. Open the `__init__.py` file with a text editor of your choice. In this file, you write nothing but the import statement which has the following schema:
-        ```python
-        from .Filename import Classname
-        ```
-        * Replace the information in the `setup.py` file with the matching content.
-        * Upload your package to PyPi
-        ```sh
-        python setup.py sdist
-        twine upload dist/*
-        ```
-        
+Project-URL: Documentation, https://github.com/mirukutea/revolutioneeringz
+Project-URL: Funding, https://donate.pypi.org
+Project-URL: Say Thanks!, http://saythanks.io/to/example
+Project-URL: Source, https://github.com/mirukutea/revolutioneeringz/
+Project-URL: Tracker, https://github.com/mirukutea/revolutioneeringz/issues
 Keywords: SOME,MEANINGFULL,KEYWORDS
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: validators
+Requires-Dist: beautifulsoup4
+Requires-Dist: discordautochat
+Requires-Dist: discorudo
+
+# Python library quick start
+This is a minimal template for uploading your python packages to pypi.org.
+
+## To Use
+* First clone this project.
+```bash
+# Clone this repository
+git clone https://github.com/defartsa23/python-library-quick-start.git
+# Go into the repository
+cd python-library-quick-start
+```
+* Rename the folder `your-package` to the package name you want. then place all your files into a folder. Open the `__init__.py` file with a text editor of your choice. In this file, you write nothing but the import statement which has the following schema:
+```python
+from .Filename import Classname
+```
+* Replace the information in the `setup.py` file with the matching content.
+* Upload your package to PyPi
+```sh
+python setup.py sdist
+twine upload dist/*
+```
```

### Comparing `revolutioneeringz-1.1/setup.py` & `revolutioneeringz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'revolutioneeringz',
     packages = ['revolutioneeringz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'revolutioneeringz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/revolutioneeringz',
```

