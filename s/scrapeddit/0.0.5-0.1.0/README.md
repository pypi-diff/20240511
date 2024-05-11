# Comparing `tmp/scrapeddit-0.0.5.tar.gz` & `tmp/scrapeddit-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapeddit-0.0.5.tar", last modified: Sat May 11 10:25:44 2024, max compression
+gzip compressed data, was "scrapeddit-0.1.0.tar", last modified: Sat May 11 10:35:02 2024, max compression
```

## Comparing `scrapeddit-0.0.5.tar` & `scrapeddit-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 10:25:44.752231 scrapeddit-0.0.5/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1063 2024-05-11 09:03:02.000000 scrapeddit-0.0.5/LICENSE.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 10:25:44.751839 scrapeddit-0.0.5/PKG-INFO
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2735 2024-05-11 09:30:19.000000 scrapeddit-0.0.5/README.md
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 10:25:44.749976 scrapeddit-0.0.5/scrapeddit/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1516 2024-05-11 08:43:10.000000 scrapeddit-0.0.5/scrapeddit/Dataset.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:24:22.000000 scrapeddit-0.0.5/scrapeddit/__init__.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3602 2024-05-11 10:19:06.000000 scrapeddit-0.0.5/scrapeddit/redditdl.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1233 2024-05-11 10:18:03.000000 scrapeddit-0.0.5/scrapeddit/scrapedit.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2396 2024-05-11 08:43:10.000000 scrapeddit-0.0.5/scrapeddit/showit.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      576 2024-05-11 08:43:10.000000 scrapeddit-0.0.5/scrapeddit/transforms.py
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 10:25:44.751448 scrapeddit-0.0.5/scrapeddit.egg-info/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 10:25:44.000000 scrapeddit-0.0.5/scrapeddit.egg-info/PKG-INFO
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      337 2024-05-11 10:25:44.000000 scrapeddit-0.0.5/scrapeddit.egg-info/SOURCES.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:25:44.000000 scrapeddit-0.0.5/scrapeddit.egg-info/dependency_links.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       15 2024-05-11 10:25:44.000000 scrapeddit-0.0.5/scrapeddit.egg-info/requires.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       11 2024-05-11 10:25:44.000000 scrapeddit-0.0.5/scrapeddit.egg-info/top_level.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       38 2024-05-11 10:25:44.752323 scrapeddit-0.0.5/setup.cfg
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      662 2024-05-11 10:25:35.000000 scrapeddit-0.0.5/setup.py
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 10:35:02.489970 scrapeddit-0.1.0/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1063 2024-05-11 09:03:02.000000 scrapeddit-0.1.0/LICENSE.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 10:35:02.489675 scrapeddit-0.1.0/PKG-INFO
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2735 2024-05-11 09:30:19.000000 scrapeddit-0.1.0/README.md
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 10:35:02.487896 scrapeddit-0.1.0/scrapeddit/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1516 2024-05-11 08:43:10.000000 scrapeddit-0.1.0/scrapeddit/Dataset.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:24:22.000000 scrapeddit-0.1.0/scrapeddit/__init__.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3602 2024-05-11 10:19:06.000000 scrapeddit-0.1.0/scrapeddit/redditdl.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1956 2024-05-11 10:34:38.000000 scrapeddit-0.1.0/scrapeddit/scrapedit.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2396 2024-05-11 08:43:10.000000 scrapeddit-0.1.0/scrapeddit/showit.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      576 2024-05-11 08:43:10.000000 scrapeddit-0.1.0/scrapeddit/transforms.py
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 10:35:02.489288 scrapeddit-0.1.0/scrapeddit.egg-info/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 10:35:02.000000 scrapeddit-0.1.0/scrapeddit.egg-info/PKG-INFO
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      337 2024-05-11 10:35:02.000000 scrapeddit-0.1.0/scrapeddit.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:35:02.000000 scrapeddit-0.1.0/scrapeddit.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       15 2024-05-11 10:35:02.000000 scrapeddit-0.1.0/scrapeddit.egg-info/requires.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       11 2024-05-11 10:35:02.000000 scrapeddit-0.1.0/scrapeddit.egg-info/top_level.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       38 2024-05-11 10:35:02.490050 scrapeddit-0.1.0/setup.cfg
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      662 2024-05-11 10:34:59.000000 scrapeddit-0.1.0/setup.py
```

### Comparing `scrapeddit-0.0.5/LICENSE.txt` & `scrapeddit-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.0.5/PKG-INFO` & `scrapeddit-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapeddit
-Version: 0.0.5
+Version: 0.1.0
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
-Metadata-Version: 2.1 Name: scrapeddit Version: 0.0.5 Summary: Simple test
+Metadata-Version: 2.1 Name: scrapeddit Version: 0.1.0 Summary: Simple test
 package Home-page: https://github.com/Mafaz03/ReditScraper Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE.txt Requires-Dist: praw Requires-Dist: torchinfo
 ************ SSccrraappeeddddiitt ************
 ********** OOvveerrvviieeww **********
 Scrapeddit is a Python class designed for scraping images from Reddit
 subreddits and creating PyTorch datasets. It facilitates the collection of
```

### Comparing `scrapeddit-0.0.5/README.md` & `scrapeddit-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.0.5/scrapeddit/Dataset.py` & `scrapeddit-0.1.0/scrapeddit/Dataset.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.0.5/scrapeddit/redditdl.py` & `scrapeddit-0.1.0/scrapeddit/redditdl.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.0.5/scrapeddit/scrapedit.py` & `scrapeddit-0.1.0/scrapeddit/scrapedit.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,40 @@
 import tqdm
 import praw
 from datetime import datetime
 import pandas as pd
 
-reddit = praw.Reddit(client_id = "",
-            client_secret = "",
-            username = '',
-            password = '',
-            redirect_uri = "",
-            user_agent = "",
-            check_for_async=False)
+class InvalidSubreddit(Exception):
+    pass
+class RestrictedSubreddit(Exception):
+    pass
+class AuthFailed(Exception):
+   pass
+   
+def auth_reddit(client_id, client_secret, username, password, redirect_uri, user_agent, check_for_async = False):
+  global reddit
+  reddit = praw.Reddit(client_id = client_id,
+            client_secret = client_secret,
+            username = username,
+            password = password,
+            redirect_uri = redirect_uri,
+            user_agent = user_agent,
+            check_for_async=check_for_async)
+  sub = reddit.subreddit('cars')
+  try: sub_type = sub.subreddit_type
+  except: raise InvalidSubreddit("Invalid Authentication, please recheck and try again")
+
 
 def scrape_reddit(subreddit: str, limit = 10, sortby = 'year', show_safe = None):
   sub = reddit.subreddit(subreddit)
+  try:
+    sub_type = sub.subreddit_type
+    if sub_type != 'public':
+      raise RestrictedSubreddit(f"r/{r} is restricted to public access")
+  except: raise InvalidSubreddit(f"r/{r} is invalid Subreddit, make sure the subreddit is valid")
   result = []
   sub_itter = sub.top(sortby,limit = limit)
   for submission in tqdm(sub_itter):
     d = {}
     d['id'] = submission.id
     d['title'] = submission.title
     d['num_comments'] = submission.num_comments
```

### Comparing `scrapeddit-0.0.5/scrapeddit/showit.py` & `scrapeddit-0.1.0/scrapeddit/showit.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.0.5/scrapeddit/transforms.py` & `scrapeddit-0.1.0/scrapeddit/transforms.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.0.5/scrapeddit.egg-info/PKG-INFO` & `scrapeddit-0.1.0/scrapeddit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapeddit
-Version: 0.0.5
+Version: 0.1.0
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
-Metadata-Version: 2.1 Name: scrapeddit Version: 0.0.5 Summary: Simple test
+Metadata-Version: 2.1 Name: scrapeddit Version: 0.1.0 Summary: Simple test
 package Home-page: https://github.com/Mafaz03/ReditScraper Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE.txt Requires-Dist: praw Requires-Dist: torchinfo
 ************ SSccrraappeeddddiitt ************
 ********** OOvveerrvviieeww **********
 Scrapeddit is a Python class designed for scraping images from Reddit
 subreddits and creating PyTorch datasets. It facilitates the collection of
```

### Comparing `scrapeddit-0.0.5/setup.py` & `scrapeddit-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 working_directory = path.abspath(path.dirname(__file__))
 
 with open(path.join(working_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='scrapeddit', # name of packe which will be package dir below project
-    version='0.0.5',
+    version='0.1.0',
     url='https://github.com/Mafaz03/ReditScraper',
     author='Mafaz03',
     author_email='mohdmafaz200303@gmail.com',
     description='Simple test package',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

