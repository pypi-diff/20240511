# Comparing `tmp/nondiaphanousnessz-1.1.tar.gz` & `tmp/nondiaphanousnessz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nondiaphanousnessz-1.1.tar", last modified: Fri May 10 00:12:24 2024, max compression
+gzip compressed data, was "nondiaphanousnessz-2.1.tar", last modified: Sat May 11 06:07:59 2024, max compression
```

## Comparing `nondiaphanousnessz-1.1.tar` & `nondiaphanousnessz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 00:12:24.161201 nondiaphanousnessz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1688 2024-05-10 00:12:24.161201 nondiaphanousnessz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 00:12:24.161201 nondiaphanousnessz-1.1/nondiaphanousnessz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 00:12:23.953197 nondiaphanousnessz-1.1/nondiaphanousnessz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 00:12:23.973198 nondiaphanousnessz-1.1/nondiaphanousnessz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-10 00:12:23.953197 nondiaphanousnessz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1662 2024-05-10 00:12:23.981198 nondiaphanousnessz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 06:07:59.566561 nondiaphanousnessz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-10 00:12:23.000000 nondiaphanousnessz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1989 2024-05-11 06:07:59.566561 nondiaphanousnessz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-10 00:12:23.000000 nondiaphanousnessz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 06:07:59.566561 nondiaphanousnessz-2.1/nondiaphanousnessz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 00:12:23.000000 nondiaphanousnessz-2.1/nondiaphanousnessz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 00:12:23.000000 nondiaphanousnessz-2.1/nondiaphanousnessz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 06:07:59.566561 nondiaphanousnessz-2.1/nondiaphanousnessz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1989 2024-05-11 06:07:59.000000 nondiaphanousnessz-2.1/nondiaphanousnessz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      303 2024-05-11 06:07:59.000000 nondiaphanousnessz-2.1/nondiaphanousnessz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 06:07:59.000000 nondiaphanousnessz-2.1/nondiaphanousnessz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 06:07:59.000000 nondiaphanousnessz-2.1/nondiaphanousnessz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       19 2024-05-11 06:07:59.000000 nondiaphanousnessz-2.1/nondiaphanousnessz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 06:07:59.570561 nondiaphanousnessz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1662 2024-05-11 06:07:59.000000 nondiaphanousnessz-2.1/setup.py
```

### Comparing `nondiaphanousnessz-1.1/PKG-INFO` & `nondiaphanousnessz-2.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,51 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: nondiaphanousnessz
-Version: 1.1
+Version: 2.1
 Summary: nondiaphanousnessz
 Home-page: https://github.com/mirukutea/nondiaphanousnessz
+Download-URL: https://github.com/mirukutea/nondiaphanousnessz/archive/v_01.tar.gz
 Author: Mirukutea
 Author-email: tea@masrizky.com
 License: MIT
-Download-URL: https://github.com/mirukutea/nondiaphanousnessz/archive/v_01.tar.gz
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
+Project-URL: Documentation, https://github.com/mirukutea/nondiaphanousnessz
+Project-URL: Funding, https://donate.pypi.org
+Project-URL: Say Thanks!, http://saythanks.io/to/example
+Project-URL: Source, https://github.com/mirukutea/nondiaphanousnessz/
+Project-URL: Tracker, https://github.com/mirukutea/nondiaphanousnessz/issues
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

### Comparing `nondiaphanousnessz-1.1/setup.py` & `nondiaphanousnessz-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'nondiaphanousnessz',
     packages = ['nondiaphanousnessz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'nondiaphanousnessz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/nondiaphanousnessz',
```

