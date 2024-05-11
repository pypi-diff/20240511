# Comparing `tmp/scrapeddit-0.1.3.tar.gz` & `tmp/scrapeddit-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapeddit-0.1.3.tar", last modified: Sat May 11 11:19:04 2024, max compression
+gzip compressed data, was "scrapeddit-0.1.4.tar", last modified: Sat May 11 11:24:23 2024, max compression
```

## Comparing `scrapeddit-0.1.3.tar` & `scrapeddit-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 11:19:04.488691 scrapeddit-0.1.3/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1063 2024-05-11 09:03:02.000000 scrapeddit-0.1.3/LICENSE.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 11:19:04.488335 scrapeddit-0.1.3/PKG-INFO
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2735 2024-05-11 09:30:19.000000 scrapeddit-0.1.3/README.md
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 11:19:04.486677 scrapeddit-0.1.3/scrapeddit/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1516 2024-05-11 08:43:10.000000 scrapeddit-0.1.3/scrapeddit/Dataset.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:24:22.000000 scrapeddit-0.1.3/scrapeddit/__init__.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3602 2024-05-11 10:19:06.000000 scrapeddit-0.1.3/scrapeddit/redditdl.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2214 2024-05-11 11:18:16.000000 scrapeddit-0.1.3/scrapeddit/scrapedit.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2396 2024-05-11 08:43:10.000000 scrapeddit-0.1.3/scrapeddit/showit.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      576 2024-05-11 08:43:10.000000 scrapeddit-0.1.3/scrapeddit/transforms.py
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 11:19:04.487955 scrapeddit-0.1.3/scrapeddit.egg-info/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 11:19:04.000000 scrapeddit-0.1.3/scrapeddit.egg-info/PKG-INFO
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      337 2024-05-11 11:19:04.000000 scrapeddit-0.1.3/scrapeddit.egg-info/SOURCES.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 11:19:04.000000 scrapeddit-0.1.3/scrapeddit.egg-info/dependency_links.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       15 2024-05-11 11:19:04.000000 scrapeddit-0.1.3/scrapeddit.egg-info/requires.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       11 2024-05-11 11:19:04.000000 scrapeddit-0.1.3/scrapeddit.egg-info/top_level.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       38 2024-05-11 11:19:04.488772 scrapeddit-0.1.3/setup.cfg
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      662 2024-05-11 11:18:55.000000 scrapeddit-0.1.3/setup.py
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 11:24:23.023756 scrapeddit-0.1.4/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1063 2024-05-11 09:03:02.000000 scrapeddit-0.1.4/LICENSE.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 11:24:23.023473 scrapeddit-0.1.4/PKG-INFO
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2735 2024-05-11 09:30:19.000000 scrapeddit-0.1.4/README.md
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 11:24:23.021920 scrapeddit-0.1.4/scrapeddit/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1516 2024-05-11 08:43:10.000000 scrapeddit-0.1.4/scrapeddit/Dataset.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:24:22.000000 scrapeddit-0.1.4/scrapeddit/__init__.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3602 2024-05-11 10:19:06.000000 scrapeddit-0.1.4/scrapeddit/redditdl.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2210 2024-05-11 11:24:10.000000 scrapeddit-0.1.4/scrapeddit/scrapedit.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2396 2024-05-11 08:43:10.000000 scrapeddit-0.1.4/scrapeddit/showit.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      576 2024-05-11 08:43:10.000000 scrapeddit-0.1.4/scrapeddit/transforms.py
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 11:24:23.023130 scrapeddit-0.1.4/scrapeddit.egg-info/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 11:24:22.000000 scrapeddit-0.1.4/scrapeddit.egg-info/PKG-INFO
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      337 2024-05-11 11:24:22.000000 scrapeddit-0.1.4/scrapeddit.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 11:24:22.000000 scrapeddit-0.1.4/scrapeddit.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       15 2024-05-11 11:24:22.000000 scrapeddit-0.1.4/scrapeddit.egg-info/requires.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       11 2024-05-11 11:24:22.000000 scrapeddit-0.1.4/scrapeddit.egg-info/top_level.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       38 2024-05-11 11:24:23.023835 scrapeddit-0.1.4/setup.cfg
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      662 2024-05-11 11:24:21.000000 scrapeddit-0.1.4/setup.py
```

### Comparing `scrapeddit-0.1.3/LICENSE.txt` & `scrapeddit-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.1.3/PKG-INFO` & `scrapeddit-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapeddit
-Version: 0.1.3
+Version: 0.1.4
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
-Metadata-Version: 2.1 Name: scrapeddit Version: 0.1.3 Summary: Simple test
+Metadata-Version: 2.1 Name: scrapeddit Version: 0.1.4 Summary: Simple test
 package Home-page: https://github.com/Mafaz03/ReditScraper Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE.txt Requires-Dist: praw Requires-Dist: torchinfo
 ************ SSccrraappeeddddiitt ************
 ********** OOvveerrvviieeww **********
 Scrapeddit is a Python class designed for scraping images from Reddit
 subreddits and creating PyTorch datasets. It facilitates the collection of
```

### Comparing `scrapeddit-0.1.3/README.md` & `scrapeddit-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.1.3/scrapeddit/Dataset.py` & `scrapeddit-0.1.4/scrapeddit/Dataset.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.1.3/scrapeddit/redditdl.py` & `scrapeddit-0.1.4/scrapeddit/redditdl.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.1.3/scrapeddit/scrapedit.py` & `scrapeddit-0.1.4/scrapeddit/scrapedit.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   reddit = praw.Reddit(client_id = client_id,
             client_secret = client_secret,
             username = username,
             password = password,
             redirect_uri = redirect_uri,
             user_agent = user_agent,
             check_for_async=check_for_async)
-  sub = reddit.subreddit('popular')
+  sub = reddit.subreddit('aww')
   try: sub_type = sub.subreddit_type
   except: raise InvalidSubreddit("Invalid Authentication, please recheck and try again")
   print("Authentication was successful")
   auths.append(reddit)
 
 def scrape_reddit(subreddit: str, limit = 10, sortby = 'year', show_safe = None):
   if len(auths) == 0: raise IncompleteAuth("Complete Authentication by calling `scrapedit.auth_reddit` before proceeding")
```

### Comparing `scrapeddit-0.1.3/scrapeddit/showit.py` & `scrapeddit-0.1.4/scrapeddit/showit.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.1.3/scrapeddit/transforms.py` & `scrapeddit-0.1.4/scrapeddit/transforms.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.1.3/scrapeddit.egg-info/PKG-INFO` & `scrapeddit-0.1.4/scrapeddit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapeddit
-Version: 0.1.3
+Version: 0.1.4
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
-Metadata-Version: 2.1 Name: scrapeddit Version: 0.1.3 Summary: Simple test
+Metadata-Version: 2.1 Name: scrapeddit Version: 0.1.4 Summary: Simple test
 package Home-page: https://github.com/Mafaz03/ReditScraper Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE.txt Requires-Dist: praw Requires-Dist: torchinfo
 ************ SSccrraappeeddddiitt ************
 ********** OOvveerrvviieeww **********
 Scrapeddit is a Python class designed for scraping images from Reddit
 subreddits and creating PyTorch datasets. It facilitates the collection of
```

### Comparing `scrapeddit-0.1.3/setup.py` & `scrapeddit-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 working_directory = path.abspath(path.dirname(__file__))
 
 with open(path.join(working_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='scrapeddit', # name of packe which will be package dir below project
-    version='0.1.3',
+    version='0.1.4',
     url='https://github.com/Mafaz03/ReditScraper',
     author='Mafaz03',
     author_email='mohdmafaz200303@gmail.com',
     description='Simple test package',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

