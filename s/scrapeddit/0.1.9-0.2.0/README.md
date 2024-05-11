# Comparing `tmp/scrapeddit-0.1.9.tar.gz` & `tmp/scrapeddit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapeddit-0.1.9.tar", last modified: Sat May 11 11:59:24 2024, max compression
+gzip compressed data, was "scrapeddit-0.2.0.tar", last modified: Sat May 11 12:13:20 2024, max compression
```

## Comparing `scrapeddit-0.1.9.tar` & `scrapeddit-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 11:59:24.270129 scrapeddit-0.1.9/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1063 2024-05-11 09:03:02.000000 scrapeddit-0.1.9/LICENSE.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 11:59:24.269760 scrapeddit-0.1.9/PKG-INFO
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2735 2024-05-11 09:30:19.000000 scrapeddit-0.1.9/README.md
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 11:59:24.268132 scrapeddit-0.1.9/scrapeddit/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1516 2024-05-11 08:43:10.000000 scrapeddit-0.1.9/scrapeddit/Dataset.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:24:22.000000 scrapeddit-0.1.9/scrapeddit/__init__.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3602 2024-05-11 10:19:06.000000 scrapeddit-0.1.9/scrapeddit/redditdl.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2235 2024-05-11 11:58:56.000000 scrapeddit-0.1.9/scrapeddit/scrapedit.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2396 2024-05-11 08:43:10.000000 scrapeddit-0.1.9/scrapeddit/showit.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      576 2024-05-11 08:43:10.000000 scrapeddit-0.1.9/scrapeddit/transforms.py
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 11:59:24.269362 scrapeddit-0.1.9/scrapeddit.egg-info/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 11:59:24.000000 scrapeddit-0.1.9/scrapeddit.egg-info/PKG-INFO
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      337 2024-05-11 11:59:24.000000 scrapeddit-0.1.9/scrapeddit.egg-info/SOURCES.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 11:59:24.000000 scrapeddit-0.1.9/scrapeddit.egg-info/dependency_links.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       15 2024-05-11 11:59:24.000000 scrapeddit-0.1.9/scrapeddit.egg-info/requires.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       11 2024-05-11 11:59:24.000000 scrapeddit-0.1.9/scrapeddit.egg-info/top_level.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       38 2024-05-11 11:59:24.270217 scrapeddit-0.1.9/setup.cfg
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      662 2024-05-11 11:59:18.000000 scrapeddit-0.1.9/setup.py
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 12:13:20.955929 scrapeddit-0.2.0/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1063 2024-05-11 09:03:02.000000 scrapeddit-0.2.0/LICENSE.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 12:13:20.955646 scrapeddit-0.2.0/PKG-INFO
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2735 2024-05-11 09:30:19.000000 scrapeddit-0.2.0/README.md
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 12:13:20.953773 scrapeddit-0.2.0/scrapeddit/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:24:22.000000 scrapeddit-0.2.0/scrapeddit/__init__.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      808 2024-05-11 12:06:22.000000 scrapeddit-0.2.0/scrapeddit/authentication.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3526 2024-05-11 12:10:46.000000 scrapeddit-0.2.0/scrapeddit/redditdl.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1527 2024-05-11 12:08:20.000000 scrapeddit-0.2.0/scrapeddit/scrapeonce.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2396 2024-05-11 08:43:10.000000 scrapeddit-0.2.0/scrapeddit/showit.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      576 2024-05-11 08:43:10.000000 scrapeddit-0.2.0/scrapeddit/transforms.py
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 12:13:20.955341 scrapeddit-0.2.0/scrapeddit.egg-info/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 12:13:20.000000 scrapeddit-0.2.0/scrapeddit.egg-info/PKG-INFO
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      345 2024-05-11 12:13:20.000000 scrapeddit-0.2.0/scrapeddit.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 12:13:20.000000 scrapeddit-0.2.0/scrapeddit.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       15 2024-05-11 12:13:20.000000 scrapeddit-0.2.0/scrapeddit.egg-info/requires.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       11 2024-05-11 12:13:20.000000 scrapeddit-0.2.0/scrapeddit.egg-info/top_level.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       38 2024-05-11 12:13:20.955999 scrapeddit-0.2.0/setup.cfg
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      662 2024-05-11 12:13:19.000000 scrapeddit-0.2.0/setup.py
```

### Comparing `scrapeddit-0.1.9/LICENSE.txt` & `scrapeddit-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.1.9/PKG-INFO` & `scrapeddit-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapeddit
-Version: 0.1.9
+Version: 0.2.0
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
-Metadata-Version: 2.1 Name: scrapeddit Version: 0.1.9 Summary: Simple test
+Metadata-Version: 2.1 Name: scrapeddit Version: 0.2.0 Summary: Simple test
 package Home-page: https://github.com/Mafaz03/ReditScraper Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE.txt Requires-Dist: praw Requires-Dist: torchinfo
 ************ SSccrraappeeddddiitt ************
 ********** OOvveerrvviieeww **********
 Scrapeddit is a Python class designed for scraping images from Reddit
 subreddits and creating PyTorch datasets. It facilitates the collection of
```

### Comparing `scrapeddit-0.1.9/README.md` & `scrapeddit-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.1.9/scrapeddit/redditdl.py` & `scrapeddit-0.2.0/scrapeddit/redditdl.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,32 +19,24 @@
 import requests
 from PIL import Image
 from io import BytesIO
 import numpy as np
 from tqdm import tqdm
 import torchvision.transforms as transforms
 from torchinfo import summary
-
-reddit = praw.Reddit(client_id = "",
-            client_secret = "",
-            username = '',
-            password = '',
-            redirect_uri = "",
-            user_agent = "",
-            check_for_async=False)
+from authentication import *
+import authentication
+auths = authentication.auths[0]
 
 from PIL import UnidentifiedImageError
 
-class InvalidSubreddit(Exception):
-    pass
-class RestrictedSubreddit(Exception):
-    pass
-
 class ScrapeditDataset(Dataset):
   def __init__(self, subreddit: list, limit=10, sortby='year', show_safe=None, max_size=500, transform=None):
+    if len(auths) == 0: raise IncompleteAuth("Complete Authentication by calling `authentication.auth_reddit` before proceeding")
+    reddit = auths[0]
     if transform: self.transform = transform
     else: self.transform = transforms.ToTensor()
     self.subreddit = subreddit
     self.max_size = max_size
     self.results = {}
     self.limit = limit
     print(f"Collecting Data from {len(self.subreddit)} subreddits")
```

### Comparing `scrapeddit-0.1.9/scrapeddit/scrapedit.py` & `scrapeddit-0.2.0/scrapeddit/scrapeonce.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,18 @@
 from tqdm import tqdm
 import praw
 from datetime import datetime
 import pandas as pd
+from authentication import *
+import authentication
 
-class InvalidSubreddit(Exception):
-    pass
-class RestrictedSubreddit(Exception):
-    pass
-class AuthFailed(Exception):
-   pass
-class IncompleteAuth(Exception): pass
-   
-auths = []
-
-def auth_reddit(client_id, client_secret, username, password, redirect_uri, user_agent, check_for_async = False):
-  reddit = praw.Reddit(client_id = client_id,
-            client_secret = client_secret,
-            username = username,
-            password = password,
-            redirect_uri = redirect_uri,
-            user_agent = user_agent,
-            check_for_async=check_for_async)
-  sub = reddit.subreddit('aww')
-  try: sub_type = sub.subreddit_type
-  except: raise InvalidSubreddit("Invalid Authentication, please recheck and try again")
-  print("Authentication was successful")
-  auths.append(reddit)
+auths = authentication.auths[0]
 
 def scrape_reddit(subreddit: str, limit = 10, sortby = 'year', show_safe = None):
-  if len(auths) == 0: raise IncompleteAuth("Complete Authentication by calling `scrapedit.auth_reddit` before proceeding")
+  if len(auths) == 0: raise IncompleteAuth("Complete Authentication by calling `authentication.auth_reddit` before proceeding")
   reddit = auths[0]
   sub = reddit.subreddit(subreddit)
   try:
     sub_type = sub.subreddit_type
     if sub_type != 'public':
       raise RestrictedSubreddit(f"r/{subreddit} is restricted to public access")
   except: raise InvalidSubreddit(f"r/{subreddit} is invalid Subreddit, make sure the subreddit is valid")
```

### Comparing `scrapeddit-0.1.9/scrapeddit/showit.py` & `scrapeddit-0.2.0/scrapeddit/showit.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.1.9/scrapeddit/transforms.py` & `scrapeddit-0.2.0/scrapeddit/transforms.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.1.9/scrapeddit.egg-info/PKG-INFO` & `scrapeddit-0.2.0/scrapeddit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapeddit
-Version: 0.1.9
+Version: 0.2.0
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
-Metadata-Version: 2.1 Name: scrapeddit Version: 0.1.9 Summary: Simple test
+Metadata-Version: 2.1 Name: scrapeddit Version: 0.2.0 Summary: Simple test
 package Home-page: https://github.com/Mafaz03/ReditScraper Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE.txt Requires-Dist: praw Requires-Dist: torchinfo
 ************ SSccrraappeeddddiitt ************
 ********** OOvveerrvviieeww **********
 Scrapeddit is a Python class designed for scraping images from Reddit
 subreddits and creating PyTorch datasets. It facilitates the collection of
```

### Comparing `scrapeddit-0.1.9/setup.py` & `scrapeddit-0.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 working_directory = path.abspath(path.dirname(__file__))
 
 with open(path.join(working_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='scrapeddit', # name of packe which will be package dir below project
-    version='0.1.9',
+    version='0.2.0',
     url='https://github.com/Mafaz03/ReditScraper',
     author='Mafaz03',
     author_email='mohdmafaz200303@gmail.com',
     description='Simple test package',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

