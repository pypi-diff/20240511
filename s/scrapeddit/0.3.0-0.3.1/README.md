# Comparing `tmp/scrapeddit-0.3.0.tar.gz` & `tmp/scrapeddit-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapeddit-0.3.0.tar", last modified: Sat May 11 13:12:28 2024, max compression
+gzip compressed data, was "scrapeddit-0.3.1.tar", last modified: Sat May 11 13:31:55 2024, max compression
```

## Comparing `scrapeddit-0.3.0.tar` & `scrapeddit-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 13:12:28.995592 scrapeddit-0.3.0/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1063 2024-05-11 09:03:02.000000 scrapeddit-0.3.0/LICENSE.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3035 2024-05-11 13:12:28.995278 scrapeddit-0.3.0/PKG-INFO
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2735 2024-05-11 09:30:19.000000 scrapeddit-0.3.0/README.md
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 13:12:28.993541 scrapeddit-0.3.0/scrapeddit/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:24:22.000000 scrapeddit-0.3.0/scrapeddit/__init__.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      827 2024-05-11 12:48:27.000000 scrapeddit-0.3.0/scrapeddit/authentication.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3549 2024-05-11 13:08:02.000000 scrapeddit-0.3.0/scrapeddit/redditdl.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1550 2024-05-11 12:41:22.000000 scrapeddit-0.3.0/scrapeddit/scrapeonce.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3014 2024-05-11 13:11:08.000000 scrapeddit-0.3.0/scrapeddit/showit.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      599 2024-05-11 12:59:46.000000 scrapeddit-0.3.0/scrapeddit/transforms.py
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 13:12:28.994943 scrapeddit-0.3.0/scrapeddit.egg-info/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3035 2024-05-11 13:12:28.000000 scrapeddit-0.3.0/scrapeddit.egg-info/PKG-INFO
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      345 2024-05-11 13:12:28.000000 scrapeddit-0.3.0/scrapeddit.egg-info/SOURCES.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 13:12:28.000000 scrapeddit-0.3.0/scrapeddit.egg-info/dependency_links.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       15 2024-05-11 13:12:28.000000 scrapeddit-0.3.0/scrapeddit.egg-info/requires.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       11 2024-05-11 13:12:28.000000 scrapeddit-0.3.0/scrapeddit.egg-info/top_level.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       38 2024-05-11 13:12:28.995669 scrapeddit-0.3.0/setup.cfg
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      660 2024-05-11 13:12:26.000000 scrapeddit-0.3.0/setup.py
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 13:31:55.451481 scrapeddit-0.3.1/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1063 2024-05-11 09:03:02.000000 scrapeddit-0.3.1/LICENSE.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3035 2024-05-11 13:31:55.451164 scrapeddit-0.3.1/PKG-INFO
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2735 2024-05-11 09:30:19.000000 scrapeddit-0.3.1/README.md
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 13:31:55.449491 scrapeddit-0.3.1/scrapeddit/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:24:22.000000 scrapeddit-0.3.1/scrapeddit/__init__.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      827 2024-05-11 12:48:27.000000 scrapeddit-0.3.1/scrapeddit/authentication.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3549 2024-05-11 13:08:02.000000 scrapeddit-0.3.1/scrapeddit/redditdl.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1550 2024-05-11 12:41:22.000000 scrapeddit-0.3.1/scrapeddit/scrapeonce.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3014 2024-05-11 13:11:08.000000 scrapeddit-0.3.1/scrapeddit/showit.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      599 2024-05-11 12:59:46.000000 scrapeddit-0.3.1/scrapeddit/transforms.py
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 13:31:55.450775 scrapeddit-0.3.1/scrapeddit.egg-info/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3035 2024-05-11 13:31:55.000000 scrapeddit-0.3.1/scrapeddit.egg-info/PKG-INFO
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      345 2024-05-11 13:31:55.000000 scrapeddit-0.3.1/scrapeddit.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 13:31:55.000000 scrapeddit-0.3.1/scrapeddit.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       15 2024-05-11 13:31:55.000000 scrapeddit-0.3.1/scrapeddit.egg-info/requires.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       11 2024-05-11 13:31:55.000000 scrapeddit-0.3.1/scrapeddit.egg-info/top_level.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       38 2024-05-11 13:31:55.451560 scrapeddit-0.3.1/setup.cfg
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      660 2024-05-11 13:31:51.000000 scrapeddit-0.3.1/setup.py
```

### Comparing `scrapeddit-0.3.0/LICENSE.txt` & `scrapeddit-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.3.0/PKG-INFO` & `scrapeddit-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapeddit
-Version: 0.3.0
+Version: 0.3.1
 Summary: Simple test package
 Home-page: https://github.com/Mafaz03/scrapeddit
 Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: praw
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scrapeddit Version: 0.3.0 Summary: Simple test
+Metadata-Version: 2.1 Name: scrapeddit Version: 0.3.1 Summary: Simple test
 package Home-page: https://github.com/Mafaz03/scrapeddit Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE.txt Requires-Dist: praw Requires-Dist: torchinfo
 ************ SSccrraappeeddddiitt ************
 ********** OOvveerrvviieeww **********
 Scrapeddit is a Python class designed for scraping images from Reddit
 subreddits and creating PyTorch datasets. It facilitates the collection of
```

### Comparing `scrapeddit-0.3.0/README.md` & `scrapeddit-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.3.0/scrapeddit/authentication.py` & `scrapeddit-0.3.1/scrapeddit/authentication.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.3.0/scrapeddit/redditdl.py` & `scrapeddit-0.3.1/scrapeddit/redditdl.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.3.0/scrapeddit/scrapeonce.py` & `scrapeddit-0.3.1/scrapeddit/scrapeonce.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.3.0/scrapeddit/showit.py` & `scrapeddit-0.3.1/scrapeddit/showit.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.3.0/scrapeddit/transforms.py` & `scrapeddit-0.3.1/scrapeddit/transforms.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.3.0/scrapeddit.egg-info/PKG-INFO` & `scrapeddit-0.3.1/scrapeddit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapeddit
-Version: 0.3.0
+Version: 0.3.1
 Summary: Simple test package
 Home-page: https://github.com/Mafaz03/scrapeddit
 Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: praw
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scrapeddit Version: 0.3.0 Summary: Simple test
+Metadata-Version: 2.1 Name: scrapeddit Version: 0.3.1 Summary: Simple test
 package Home-page: https://github.com/Mafaz03/scrapeddit Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE.txt Requires-Dist: praw Requires-Dist: torchinfo
 ************ SSccrraappeeddddiitt ************
 ********** OOvveerrvviieeww **********
 Scrapeddit is a Python class designed for scraping images from Reddit
 subreddits and creating PyTorch datasets. It facilitates the collection of
```

### Comparing `scrapeddit-0.3.0/setup.py` & `scrapeddit-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 working_directory = path.abspath(path.dirname(__file__))
 
 with open(path.join(working_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='scrapeddit', # name of packe which will be package dir below project
-    version='0.3.0',
+    version='0.3.1',
     url='https://github.com/Mafaz03/scrapeddit',
     author='Mafaz03',
     author_email='mohdmafaz200303@gmail.com',
     description='Simple test package',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

