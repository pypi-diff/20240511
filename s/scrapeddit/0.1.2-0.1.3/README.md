# Comparing `tmp/scrapeddit-0.1.2.tar.gz` & `tmp/scrapeddit-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapeddit-0.1.2.tar", last modified: Sat May 11 10:46:21 2024, max compression
+gzip compressed data, was "scrapeddit-0.1.3.tar", last modified: Sat May 11 11:19:04 2024, max compression
```

## Comparing `scrapeddit-0.1.2.tar` & `scrapeddit-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 10:46:21.312251 scrapeddit-0.1.2/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1063 2024-05-11 09:03:02.000000 scrapeddit-0.1.2/LICENSE.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 10:46:21.311943 scrapeddit-0.1.2/PKG-INFO
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2735 2024-05-11 09:30:19.000000 scrapeddit-0.1.2/README.md
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 10:46:21.310166 scrapeddit-0.1.2/scrapeddit/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1516 2024-05-11 08:43:10.000000 scrapeddit-0.1.2/scrapeddit/Dataset.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:24:22.000000 scrapeddit-0.1.2/scrapeddit/__init__.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3602 2024-05-11 10:19:06.000000 scrapeddit-0.1.2/scrapeddit/redditdl.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2034 2024-05-11 10:46:13.000000 scrapeddit-0.1.2/scrapeddit/scrapedit.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2396 2024-05-11 08:43:10.000000 scrapeddit-0.1.2/scrapeddit/showit.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      576 2024-05-11 08:43:10.000000 scrapeddit-0.1.2/scrapeddit/transforms.py
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 10:46:21.311579 scrapeddit-0.1.2/scrapeddit.egg-info/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 10:46:21.000000 scrapeddit-0.1.2/scrapeddit.egg-info/PKG-INFO
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      337 2024-05-11 10:46:21.000000 scrapeddit-0.1.2/scrapeddit.egg-info/SOURCES.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:46:21.000000 scrapeddit-0.1.2/scrapeddit.egg-info/dependency_links.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       15 2024-05-11 10:46:21.000000 scrapeddit-0.1.2/scrapeddit.egg-info/requires.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       11 2024-05-11 10:46:21.000000 scrapeddit-0.1.2/scrapeddit.egg-info/top_level.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       38 2024-05-11 10:46:21.312327 scrapeddit-0.1.2/setup.cfg
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      662 2024-05-11 10:46:19.000000 scrapeddit-0.1.2/setup.py
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 11:19:04.488691 scrapeddit-0.1.3/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1063 2024-05-11 09:03:02.000000 scrapeddit-0.1.3/LICENSE.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 11:19:04.488335 scrapeddit-0.1.3/PKG-INFO
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2735 2024-05-11 09:30:19.000000 scrapeddit-0.1.3/README.md
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 11:19:04.486677 scrapeddit-0.1.3/scrapeddit/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1516 2024-05-11 08:43:10.000000 scrapeddit-0.1.3/scrapeddit/Dataset.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:24:22.000000 scrapeddit-0.1.3/scrapeddit/__init__.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3602 2024-05-11 10:19:06.000000 scrapeddit-0.1.3/scrapeddit/redditdl.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2214 2024-05-11 11:18:16.000000 scrapeddit-0.1.3/scrapeddit/scrapedit.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2396 2024-05-11 08:43:10.000000 scrapeddit-0.1.3/scrapeddit/showit.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      576 2024-05-11 08:43:10.000000 scrapeddit-0.1.3/scrapeddit/transforms.py
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 11:19:04.487955 scrapeddit-0.1.3/scrapeddit.egg-info/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 11:19:04.000000 scrapeddit-0.1.3/scrapeddit.egg-info/PKG-INFO
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      337 2024-05-11 11:19:04.000000 scrapeddit-0.1.3/scrapeddit.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 11:19:04.000000 scrapeddit-0.1.3/scrapeddit.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       15 2024-05-11 11:19:04.000000 scrapeddit-0.1.3/scrapeddit.egg-info/requires.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       11 2024-05-11 11:19:04.000000 scrapeddit-0.1.3/scrapeddit.egg-info/top_level.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       38 2024-05-11 11:19:04.488772 scrapeddit-0.1.3/setup.cfg
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      662 2024-05-11 11:18:55.000000 scrapeddit-0.1.3/setup.py
```

### Comparing `scrapeddit-0.1.2/LICENSE.txt` & `scrapeddit-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.1.2/PKG-INFO` & `scrapeddit-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapeddit
-Version: 0.1.2
+Version: 0.1.3
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
-Metadata-Version: 2.1 Name: scrapeddit Version: 0.1.2 Summary: Simple test
+Metadata-Version: 2.1 Name: scrapeddit Version: 0.1.3 Summary: Simple test
 package Home-page: https://github.com/Mafaz03/ReditScraper Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE.txt Requires-Dist: praw Requires-Dist: torchinfo
 ************ SSccrraappeeddddiitt ************
 ********** OOvveerrvviieeww **********
 Scrapeddit is a Python class designed for scraping images from Reddit
 subreddits and creating PyTorch datasets. It facilitates the collection of
```

### Comparing `scrapeddit-0.1.2/README.md` & `scrapeddit-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.1.2/scrapeddit/Dataset.py` & `scrapeddit-0.1.3/scrapeddit/Dataset.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.1.2/scrapeddit/redditdl.py` & `scrapeddit-0.1.3/scrapeddit/redditdl.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.1.2/scrapeddit/scrapedit.py` & `scrapeddit-0.1.3/scrapeddit/scrapedit.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,39 +5,41 @@
 
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
             password = password,
             redirect_uri = redirect_uri,
             user_agent = user_agent,
             check_for_async=check_for_async)
-  sub = reddit.subreddit('cars')
+  sub = reddit.subreddit('popular')
   try: sub_type = sub.subreddit_type
   except: raise InvalidSubreddit("Invalid Authentication, please recheck and try again")
   print("Authentication was successful")
   auths.append(reddit)
 
 def scrape_reddit(subreddit: str, limit = 10, sortby = 'year', show_safe = None):
+  if len(auths) == 0: raise IncompleteAuth("Complete Authentication by calling `scrapedit.auth_reddit` before proceeding")
   reddit = auths[0]
   sub = reddit.subreddit(subreddit)
   try:
     sub_type = sub.subreddit_type
     if sub_type != 'public':
-      raise RestrictedSubreddit(f"r/{r} is restricted to public access")
-  except: raise InvalidSubreddit(f"r/{r} is invalid Subreddit, make sure the subreddit is valid")
+      raise RestrictedSubreddit(f"r/{subreddit} is restricted to public access")
+  except: raise InvalidSubreddit(f"r/{subreddit} is invalid Subreddit, make sure the subreddit is valid")
   result = []
   sub_itter = sub.top(sortby,limit = limit)
   for submission in tqdm(sub_itter):
     d = {}
     d['id'] = submission.id
     d['title'] = submission.title
     d['num_comments'] = submission.num_comments
```

### Comparing `scrapeddit-0.1.2/scrapeddit/showit.py` & `scrapeddit-0.1.3/scrapeddit/showit.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.1.2/scrapeddit/transforms.py` & `scrapeddit-0.1.3/scrapeddit/transforms.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.1.2/scrapeddit.egg-info/PKG-INFO` & `scrapeddit-0.1.3/scrapeddit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapeddit
-Version: 0.1.2
+Version: 0.1.3
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
-Metadata-Version: 2.1 Name: scrapeddit Version: 0.1.2 Summary: Simple test
+Metadata-Version: 2.1 Name: scrapeddit Version: 0.1.3 Summary: Simple test
 package Home-page: https://github.com/Mafaz03/ReditScraper Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE.txt Requires-Dist: praw Requires-Dist: torchinfo
 ************ SSccrraappeeddddiitt ************
 ********** OOvveerrvviieeww **********
 Scrapeddit is a Python class designed for scraping images from Reddit
 subreddits and creating PyTorch datasets. It facilitates the collection of
```

