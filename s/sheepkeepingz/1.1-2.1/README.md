# Comparing `tmp/sheepkeepingz-1.1.tar.gz` & `tmp/sheepkeepingz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sheepkeepingz-1.1.tar", last modified: Thu May  9 16:24:53 2024, max compression
+gzip compressed data, was "sheepkeepingz-2.1.tar", last modified: Sat May 11 15:02:22 2024, max compression
```

## Comparing `sheepkeepingz-1.1.tar` & `sheepkeepingz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 16:24:53.361227 sheepkeepingz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1668 2024-05-09 16:24:53.361227 sheepkeepingz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 16:24:50.553175 sheepkeepingz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-09 16:24:51.125186 sheepkeepingz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 16:24:53.361227 sheepkeepingz-1.1/sheepkeepingz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 16:24:50.553175 sheepkeepingz-1.1/sheepkeepingz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 16:24:50.761179 sheepkeepingz-1.1/sheepkeepingz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 15:02:22.600276 sheepkeepingz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 16:24:50.000000 sheepkeepingz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-11 15:02:22.600276 sheepkeepingz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 16:24:50.000000 sheepkeepingz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 15:02:22.600276 sheepkeepingz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-11 15:02:22.000000 sheepkeepingz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 15:02:22.600276 sheepkeepingz-2.1/sheepkeepingz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 16:24:50.000000 sheepkeepingz-2.1/sheepkeepingz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 16:24:50.000000 sheepkeepingz-2.1/sheepkeepingz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 15:02:22.600276 sheepkeepingz-2.1/sheepkeepingz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-11 15:02:22.000000 sheepkeepingz-2.1/sheepkeepingz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      268 2024-05-11 15:02:22.000000 sheepkeepingz-2.1/sheepkeepingz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 15:02:22.000000 sheepkeepingz-2.1/sheepkeepingz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 15:02:22.000000 sheepkeepingz-2.1/sheepkeepingz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       14 2024-05-11 15:02:22.000000 sheepkeepingz-2.1/sheepkeepingz.egg-info/top_level.txt
```

### Comparing `sheepkeepingz-1.1/PKG-INFO` & `sheepkeepingz-2.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,51 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: sheepkeepingz
-Version: 1.1
+Version: 2.1
 Summary: sheepkeepingz
 Home-page: https://github.com/mirukutea/sheepkeepingz
+Download-URL: https://github.com/mirukutea/sheepkeepingz/archive/v_01.tar.gz
 Author: Mirukutea
 Author-email: tea@masrizky.com
 License: MIT
-Download-URL: https://github.com/mirukutea/sheepkeepingz/archive/v_01.tar.gz
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
+Project-URL: Documentation, https://github.com/mirukutea/sheepkeepingz
+Project-URL: Funding, https://donate.pypi.org
+Project-URL: Say Thanks!, http://saythanks.io/to/example
+Project-URL: Source, https://github.com/mirukutea/sheepkeepingz/
+Project-URL: Tracker, https://github.com/mirukutea/sheepkeepingz/issues
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

### Comparing `sheepkeepingz-1.1/setup.py` & `sheepkeepingz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'sheepkeepingz',
     packages = ['sheepkeepingz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'sheepkeepingz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/sheepkeepingz',
```

