# Comparing `tmp/scrapeddit-0.1.7.tar.gz` & `tmp/scrapeddit-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapeddit-0.1.7.tar", last modified: Sat May 11 11:54:48 2024, max compression
+gzip compressed data, was "scrapeddit-0.1.8.tar", last modified: Sat May 11 11:56:04 2024, max compression
```

## Comparing `scrapeddit-0.1.7.tar` & `scrapeddit-0.1.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 11:54:48.031366 scrapeddit-0.1.7/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1063 2024-05-11 09:03:02.000000 scrapeddit-0.1.7/LICENSE.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 11:54:48.031061 scrapeddit-0.1.7/PKG-INFO
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2735 2024-05-11 09:30:19.000000 scrapeddit-0.1.7/README.md
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 11:54:48.028681 scrapeddit-0.1.7/scrapeddit/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1516 2024-05-11 08:43:10.000000 scrapeddit-0.1.7/scrapeddit/Dataset.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:24:22.000000 scrapeddit-0.1.7/scrapeddit/__init__.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3602 2024-05-11 10:19:06.000000 scrapeddit-0.1.7/scrapeddit/redditdl.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2055 2024-05-11 11:54:34.000000 scrapeddit-0.1.7/scrapeddit/scrapedit.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2396 2024-05-11 08:43:10.000000 scrapeddit-0.1.7/scrapeddit/showit.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      576 2024-05-11 08:43:10.000000 scrapeddit-0.1.7/scrapeddit/transforms.py
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 11:54:48.030563 scrapeddit-0.1.7/scrapeddit.egg-info/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 11:54:47.000000 scrapeddit-0.1.7/scrapeddit.egg-info/PKG-INFO
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      337 2024-05-11 11:54:47.000000 scrapeddit-0.1.7/scrapeddit.egg-info/SOURCES.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 11:54:47.000000 scrapeddit-0.1.7/scrapeddit.egg-info/dependency_links.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       15 2024-05-11 11:54:47.000000 scrapeddit-0.1.7/scrapeddit.egg-info/requires.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       11 2024-05-11 11:54:47.000000 scrapeddit-0.1.7/scrapeddit.egg-info/top_level.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       38 2024-05-11 11:54:48.031439 scrapeddit-0.1.7/setup.cfg
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      662 2024-05-11 11:54:45.000000 scrapeddit-0.1.7/setup.py
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 11:56:04.313699 scrapeddit-0.1.8/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1063 2024-05-11 09:03:02.000000 scrapeddit-0.1.8/LICENSE.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 11:56:04.313384 scrapeddit-0.1.8/PKG-INFO
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2735 2024-05-11 09:30:19.000000 scrapeddit-0.1.8/README.md
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 11:56:04.311778 scrapeddit-0.1.8/scrapeddit/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1516 2024-05-11 08:43:10.000000 scrapeddit-0.1.8/scrapeddit/Dataset.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:24:22.000000 scrapeddit-0.1.8/scrapeddit/__init__.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3602 2024-05-11 10:19:06.000000 scrapeddit-0.1.8/scrapeddit/redditdl.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2236 2024-05-11 11:55:43.000000 scrapeddit-0.1.8/scrapeddit/scrapedit.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2396 2024-05-11 08:43:10.000000 scrapeddit-0.1.8/scrapeddit/showit.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      576 2024-05-11 08:43:10.000000 scrapeddit-0.1.8/scrapeddit/transforms.py
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 11:56:04.313061 scrapeddit-0.1.8/scrapeddit.egg-info/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 11:56:04.000000 scrapeddit-0.1.8/scrapeddit.egg-info/PKG-INFO
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      337 2024-05-11 11:56:04.000000 scrapeddit-0.1.8/scrapeddit.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 11:56:04.000000 scrapeddit-0.1.8/scrapeddit.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       15 2024-05-11 11:56:04.000000 scrapeddit-0.1.8/scrapeddit.egg-info/requires.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       11 2024-05-11 11:56:04.000000 scrapeddit-0.1.8/scrapeddit.egg-info/top_level.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       38 2024-05-11 11:56:04.313784 scrapeddit-0.1.8/setup.cfg
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      662 2024-05-11 11:56:02.000000 scrapeddit-0.1.8/setup.py
```

### Comparing `scrapeddit-0.1.7/LICENSE.txt` & `scrapeddit-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.1.7/PKG-INFO` & `scrapeddit-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapeddit
-Version: 0.1.7
+Version: 0.1.8
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
-Metadata-Version: 2.1 Name: scrapeddit Version: 0.1.7 Summary: Simple test
+Metadata-Version: 2.1 Name: scrapeddit Version: 0.1.8 Summary: Simple test
 package Home-page: https://github.com/Mafaz03/ReditScraper Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE.txt Requires-Dist: praw Requires-Dist: torchinfo
 ************ SSccrraappeeddddiitt ************
 ********** OOvveerrvviieeww **********
 Scrapeddit is a Python class designed for scraping images from Reddit
 subreddits and creating PyTorch datasets. It facilitates the collection of
```

### Comparing `scrapeddit-0.1.7/README.md` & `scrapeddit-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.1.7/scrapeddit/Dataset.py` & `scrapeddit-0.1.8/scrapeddit/Dataset.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.1.7/scrapeddit/redditdl.py` & `scrapeddit-0.1.8/scrapeddit/redditdl.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.1.7/scrapeddit/scrapedit.py` & `scrapeddit-0.1.8/scrapeddit/scrapedit.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 class InvalidSubreddit(Exception):
     pass
 class RestrictedSubreddit(Exception):
     pass
 class AuthFailed(Exception):
    pass
+class IncompleteAuth(Exception): pass
    
 auths = []
 
 def auth_reddit(client_id, client_secret, username, password, redirect_uri, user_agent, check_for_async = False):
   reddit = praw.Reddit(client_id = client_id,
             client_secret = client_secret,
             username = username,
@@ -23,14 +24,16 @@
   sub = reddit.subreddit('aww')
   try: sub_type = sub.subreddit_type
   except: raise InvalidSubreddit("Invalid Authentication, please recheck and try again")
   print("Authentication was successful")
   return reddit
 
 def scrape_reddit(reddit, subreddit: str, limit = 10, sortby = 'year', show_safe = None):
+  if len(auths) == 0: raise IncompleteAuth("Complete Authentication by calling `scrapedit.auth_reddit` before proceeding")
+  reddit = auths[0]
   sub = reddit.subreddit(subreddit)
   try:
     sub_type = sub.subreddit_type
     if sub_type != 'public':
       raise RestrictedSubreddit(f"r/{subreddit} is restricted to public access")
   except: raise InvalidSubreddit(f"r/{subreddit} is invalid Subreddit, make sure the subreddit is valid")
   result = []
```

### Comparing `scrapeddit-0.1.7/scrapeddit/showit.py` & `scrapeddit-0.1.8/scrapeddit/showit.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.1.7/scrapeddit/transforms.py` & `scrapeddit-0.1.8/scrapeddit/transforms.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.1.7/scrapeddit.egg-info/PKG-INFO` & `scrapeddit-0.1.8/scrapeddit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapeddit
-Version: 0.1.7
+Version: 0.1.8
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
-Metadata-Version: 2.1 Name: scrapeddit Version: 0.1.7 Summary: Simple test
+Metadata-Version: 2.1 Name: scrapeddit Version: 0.1.8 Summary: Simple test
 package Home-page: https://github.com/Mafaz03/ReditScraper Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE.txt Requires-Dist: praw Requires-Dist: torchinfo
 ************ SSccrraappeeddddiitt ************
 ********** OOvveerrvviieeww **********
 Scrapeddit is a Python class designed for scraping images from Reddit
 subreddits and creating PyTorch datasets. It facilitates the collection of
```

### Comparing `scrapeddit-0.1.7/setup.py` & `scrapeddit-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 working_directory = path.abspath(path.dirname(__file__))
 
 with open(path.join(working_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='scrapeddit', # name of packe which will be package dir below project
-    version='0.1.7',
+    version='0.1.8',
     url='https://github.com/Mafaz03/ReditScraper',
     author='Mafaz03',
     author_email='mohdmafaz200303@gmail.com',
     description='Simple test package',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

