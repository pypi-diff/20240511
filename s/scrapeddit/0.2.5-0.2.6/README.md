# Comparing `tmp/scrapeddit-0.2.5.tar.gz` & `tmp/scrapeddit-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapeddit-0.2.5.tar", last modified: Sat May 11 12:54:01 2024, max compression
+gzip compressed data, was "scrapeddit-0.2.6.tar", last modified: Sat May 11 12:56:32 2024, max compression
```

## Comparing `scrapeddit-0.2.5.tar` & `scrapeddit-0.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 12:54:01.943896 scrapeddit-0.2.5/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1063 2024-05-11 09:03:02.000000 scrapeddit-0.2.5/LICENSE.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 12:54:01.943569 scrapeddit-0.2.5/PKG-INFO
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2735 2024-05-11 09:30:19.000000 scrapeddit-0.2.5/README.md
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 12:54:01.942060 scrapeddit-0.2.5/scrapeddit/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:24:22.000000 scrapeddit-0.2.5/scrapeddit/__init__.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      827 2024-05-11 12:48:27.000000 scrapeddit-0.2.5/scrapeddit/authentication.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3526 2024-05-11 12:10:46.000000 scrapeddit-0.2.5/scrapeddit/redditdl.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1550 2024-05-11 12:41:22.000000 scrapeddit-0.2.5/scrapeddit/scrapeonce.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2989 2024-05-11 12:53:35.000000 scrapeddit-0.2.5/scrapeddit/showit.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      576 2024-05-11 08:43:10.000000 scrapeddit-0.2.5/scrapeddit/transforms.py
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 12:54:01.943252 scrapeddit-0.2.5/scrapeddit.egg-info/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 12:54:01.000000 scrapeddit-0.2.5/scrapeddit.egg-info/PKG-INFO
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      345 2024-05-11 12:54:01.000000 scrapeddit-0.2.5/scrapeddit.egg-info/SOURCES.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 12:54:01.000000 scrapeddit-0.2.5/scrapeddit.egg-info/dependency_links.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       15 2024-05-11 12:54:01.000000 scrapeddit-0.2.5/scrapeddit.egg-info/requires.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       11 2024-05-11 12:54:01.000000 scrapeddit-0.2.5/scrapeddit.egg-info/top_level.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       38 2024-05-11 12:54:01.943964 scrapeddit-0.2.5/setup.cfg
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      662 2024-05-11 12:54:00.000000 scrapeddit-0.2.5/setup.py
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 12:56:32.152995 scrapeddit-0.2.6/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1063 2024-05-11 09:03:02.000000 scrapeddit-0.2.6/LICENSE.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 12:56:32.152696 scrapeddit-0.2.6/PKG-INFO
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2735 2024-05-11 09:30:19.000000 scrapeddit-0.2.6/README.md
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 12:56:32.151155 scrapeddit-0.2.6/scrapeddit/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:24:22.000000 scrapeddit-0.2.6/scrapeddit/__init__.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      827 2024-05-11 12:48:27.000000 scrapeddit-0.2.6/scrapeddit/authentication.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3550 2024-05-11 12:56:00.000000 scrapeddit-0.2.6/scrapeddit/redditdl.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1550 2024-05-11 12:41:22.000000 scrapeddit-0.2.6/scrapeddit/scrapeonce.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2989 2024-05-11 12:53:35.000000 scrapeddit-0.2.6/scrapeddit/showit.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      576 2024-05-11 08:43:10.000000 scrapeddit-0.2.6/scrapeddit/transforms.py
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 12:56:32.152357 scrapeddit-0.2.6/scrapeddit.egg-info/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 12:56:32.000000 scrapeddit-0.2.6/scrapeddit.egg-info/PKG-INFO
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      345 2024-05-11 12:56:32.000000 scrapeddit-0.2.6/scrapeddit.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 12:56:32.000000 scrapeddit-0.2.6/scrapeddit.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       15 2024-05-11 12:56:32.000000 scrapeddit-0.2.6/scrapeddit.egg-info/requires.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       11 2024-05-11 12:56:32.000000 scrapeddit-0.2.6/scrapeddit.egg-info/top_level.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       38 2024-05-11 12:56:32.153065 scrapeddit-0.2.6/setup.cfg
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      662 2024-05-11 12:56:25.000000 scrapeddit-0.2.6/setup.py
```

### Comparing `scrapeddit-0.2.5/LICENSE.txt` & `scrapeddit-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.2.5/PKG-INFO` & `scrapeddit-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapeddit
-Version: 0.2.5
+Version: 0.2.6
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
-Metadata-Version: 2.1 Name: scrapeddit Version: 0.2.5 Summary: Simple test
+Metadata-Version: 2.1 Name: scrapeddit Version: 0.2.6 Summary: Simple test
 package Home-page: https://github.com/Mafaz03/ReditScraper Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE.txt Requires-Dist: praw Requires-Dist: torchinfo
 ************ SSccrraappeeddddiitt ************
 ********** OOvveerrvviieeww **********
 Scrapeddit is a Python class designed for scraping images from Reddit
 subreddits and creating PyTorch datasets. It facilitates the collection of
```

### Comparing `scrapeddit-0.2.5/README.md` & `scrapeddit-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.2.5/scrapeddit/authentication.py` & `scrapeddit-0.2.6/scrapeddit/authentication.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.2.5/scrapeddit/redditdl.py` & `scrapeddit-0.2.6/scrapeddit/redditdl.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 import requests
 from PIL import Image
 from io import BytesIO
 import numpy as np
 from tqdm import tqdm
 import torchvision.transforms as transforms
 from torchinfo import summary
-from authentication import *
-import authentication
-auths = authentication.auths[0]
+from scrapeddit import authentication
+from scrapeddit.authentication import *
+auths = authentication.auths
 
 from PIL import UnidentifiedImageError
 
 class ScrapeditDataset(Dataset):
   def __init__(self, subreddit: list, limit=10, sortby='year', show_safe=None, max_size=500, transform=None):
     if len(auths) == 0: raise IncompleteAuth("Complete Authentication by calling `authentication.auth_reddit` before proceeding")
     reddit = auths[0]
```

### Comparing `scrapeddit-0.2.5/scrapeddit/scrapeonce.py` & `scrapeddit-0.2.6/scrapeddit/scrapeonce.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.2.5/scrapeddit/showit.py` & `scrapeddit-0.2.6/scrapeddit/showit.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.2.5/scrapeddit/transforms.py` & `scrapeddit-0.2.6/scrapeddit/transforms.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.2.5/scrapeddit.egg-info/PKG-INFO` & `scrapeddit-0.2.6/scrapeddit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapeddit
-Version: 0.2.5
+Version: 0.2.6
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
-Metadata-Version: 2.1 Name: scrapeddit Version: 0.2.5 Summary: Simple test
+Metadata-Version: 2.1 Name: scrapeddit Version: 0.2.6 Summary: Simple test
 package Home-page: https://github.com/Mafaz03/ReditScraper Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE.txt Requires-Dist: praw Requires-Dist: torchinfo
 ************ SSccrraappeeddddiitt ************
 ********** OOvveerrvviieeww **********
 Scrapeddit is a Python class designed for scraping images from Reddit
 subreddits and creating PyTorch datasets. It facilitates the collection of
```

### Comparing `scrapeddit-0.2.5/setup.py` & `scrapeddit-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 working_directory = path.abspath(path.dirname(__file__))
 
 with open(path.join(working_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='scrapeddit', # name of packe which will be package dir below project
-    version='0.2.5',
+    version='0.2.6',
     url='https://github.com/Mafaz03/ReditScraper',
     author='Mafaz03',
     author_email='mohdmafaz200303@gmail.com',
     description='Simple test package',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

