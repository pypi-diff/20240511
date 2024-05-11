# Comparing `tmp/scrapeddit-0.2.2.tar.gz` & `tmp/scrapeddit-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapeddit-0.2.2.tar", last modified: Sat May 11 12:40:17 2024, max compression
+gzip compressed data, was "scrapeddit-0.2.3.tar", last modified: Sat May 11 12:41:34 2024, max compression
```

## Comparing `scrapeddit-0.2.2.tar` & `scrapeddit-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 12:40:17.643395 scrapeddit-0.2.2/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1063 2024-05-11 09:03:02.000000 scrapeddit-0.2.2/LICENSE.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 12:40:17.643058 scrapeddit-0.2.2/PKG-INFO
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2735 2024-05-11 09:30:19.000000 scrapeddit-0.2.2/README.md
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 12:40:17.641362 scrapeddit-0.2.2/scrapeddit/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:24:22.000000 scrapeddit-0.2.2/scrapeddit/__init__.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      835 2024-05-11 12:34:40.000000 scrapeddit-0.2.2/scrapeddit/authentication.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3526 2024-05-11 12:10:46.000000 scrapeddit-0.2.2/scrapeddit/redditdl.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1553 2024-05-11 12:40:07.000000 scrapeddit-0.2.2/scrapeddit/scrapeonce.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2396 2024-05-11 08:43:10.000000 scrapeddit-0.2.2/scrapeddit/showit.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      576 2024-05-11 08:43:10.000000 scrapeddit-0.2.2/scrapeddit/transforms.py
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 12:40:17.642699 scrapeddit-0.2.2/scrapeddit.egg-info/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 12:40:17.000000 scrapeddit-0.2.2/scrapeddit.egg-info/PKG-INFO
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      345 2024-05-11 12:40:17.000000 scrapeddit-0.2.2/scrapeddit.egg-info/SOURCES.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 12:40:17.000000 scrapeddit-0.2.2/scrapeddit.egg-info/dependency_links.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       15 2024-05-11 12:40:17.000000 scrapeddit-0.2.2/scrapeddit.egg-info/requires.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       11 2024-05-11 12:40:17.000000 scrapeddit-0.2.2/scrapeddit.egg-info/top_level.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       38 2024-05-11 12:40:17.643471 scrapeddit-0.2.2/setup.cfg
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      662 2024-05-11 12:40:15.000000 scrapeddit-0.2.2/setup.py
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 12:41:34.953348 scrapeddit-0.2.3/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1063 2024-05-11 09:03:02.000000 scrapeddit-0.2.3/LICENSE.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 12:41:34.953038 scrapeddit-0.2.3/PKG-INFO
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2735 2024-05-11 09:30:19.000000 scrapeddit-0.2.3/README.md
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 12:41:34.951187 scrapeddit-0.2.3/scrapeddit/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:24:22.000000 scrapeddit-0.2.3/scrapeddit/__init__.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      835 2024-05-11 12:34:40.000000 scrapeddit-0.2.3/scrapeddit/authentication.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3526 2024-05-11 12:10:46.000000 scrapeddit-0.2.3/scrapeddit/redditdl.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1550 2024-05-11 12:41:22.000000 scrapeddit-0.2.3/scrapeddit/scrapeonce.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2396 2024-05-11 08:43:10.000000 scrapeddit-0.2.3/scrapeddit/showit.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      576 2024-05-11 08:43:10.000000 scrapeddit-0.2.3/scrapeddit/transforms.py
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 12:41:34.952569 scrapeddit-0.2.3/scrapeddit.egg-info/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 12:41:34.000000 scrapeddit-0.2.3/scrapeddit.egg-info/PKG-INFO
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      345 2024-05-11 12:41:34.000000 scrapeddit-0.2.3/scrapeddit.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 12:41:34.000000 scrapeddit-0.2.3/scrapeddit.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       15 2024-05-11 12:41:34.000000 scrapeddit-0.2.3/scrapeddit.egg-info/requires.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       11 2024-05-11 12:41:34.000000 scrapeddit-0.2.3/scrapeddit.egg-info/top_level.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       38 2024-05-11 12:41:34.953418 scrapeddit-0.2.3/setup.cfg
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      662 2024-05-11 12:41:33.000000 scrapeddit-0.2.3/setup.py
```

### Comparing `scrapeddit-0.2.2/LICENSE.txt` & `scrapeddit-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.2.2/PKG-INFO` & `scrapeddit-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapeddit
-Version: 0.2.2
+Version: 0.2.3
 Summary: Simple test package
 Home-page: https://github.com/Mafaz03/ReditScraper
 Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: praw
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scrapeddit Version: 0.2.2 Summary: Simple test
+Metadata-Version: 2.1 Name: scrapeddit Version: 0.2.3 Summary: Simple test
 package Home-page: https://github.com/Mafaz03/ReditScraper Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE.txt Requires-Dist: praw Requires-Dist: torchinfo
 ************ SSccrraappeeddddiitt ************
 ********** OOvveerrvviieeww **********
 Scrapeddit is a Python class designed for scraping images from Reddit
 subreddits and creating PyTorch datasets. It facilitates the collection of
```

### Comparing `scrapeddit-0.2.2/README.md` & `scrapeddit-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.2.2/scrapeddit/authentication.py` & `scrapeddit-0.2.3/scrapeddit/authentication.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.2.2/scrapeddit/redditdl.py` & `scrapeddit-0.2.3/scrapeddit/redditdl.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.2.2/scrapeddit/scrapeonce.py` & `scrapeddit-0.2.3/scrapeddit/scrapeonce.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from tqdm import tqdm
 import praw
 from datetime import datetime
 import pandas as pd
 from scrapeddit import authentication
 from scrapeddit.authentication import *
-auths = authentication.auths[0]
+auths = authentication.auths
 
 def scrape_reddit(subreddit: str, limit = 10, sortby = 'year', show_safe = None):
   if len(auths) == 0: raise IncompleteAuth("Complete Authentication by calling `authentication.auth_reddit` before proceeding")
   reddit = auths[0]
   sub = reddit.subreddit(subreddit)
   try:
     sub_type = sub.subreddit_type
```

### Comparing `scrapeddit-0.2.2/scrapeddit/showit.py` & `scrapeddit-0.2.3/scrapeddit/showit.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.2.2/scrapeddit/transforms.py` & `scrapeddit-0.2.3/scrapeddit/transforms.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.2.2/scrapeddit.egg-info/PKG-INFO` & `scrapeddit-0.2.3/scrapeddit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapeddit
-Version: 0.2.2
+Version: 0.2.3
 Summary: Simple test package
 Home-page: https://github.com/Mafaz03/ReditScraper
 Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: praw
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scrapeddit Version: 0.2.2 Summary: Simple test
+Metadata-Version: 2.1 Name: scrapeddit Version: 0.2.3 Summary: Simple test
 package Home-page: https://github.com/Mafaz03/ReditScraper Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE.txt Requires-Dist: praw Requires-Dist: torchinfo
 ************ SSccrraappeeddddiitt ************
 ********** OOvveerrvviieeww **********
 Scrapeddit is a Python class designed for scraping images from Reddit
 subreddits and creating PyTorch datasets. It facilitates the collection of
```

### Comparing `scrapeddit-0.2.2/setup.py` & `scrapeddit-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 working_directory = path.abspath(path.dirname(__file__))
 
 with open(path.join(working_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='scrapeddit', # name of packe which will be package dir below project
-    version='0.2.2',
+    version='0.2.3',
     url='https://github.com/Mafaz03/ReditScraper',
     author='Mafaz03',
     author_email='mohdmafaz200303@gmail.com',
     description='Simple test package',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

