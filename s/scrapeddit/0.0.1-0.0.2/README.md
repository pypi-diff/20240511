# Comparing `tmp/scrapeddit-0.0.1.tar.gz` & `tmp/scrapeddit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapeddit-0.0.1.tar", last modified: Sat May 11 09:37:55 2024, max compression
+gzip compressed data, was "scrapeddit-0.0.2.tar", last modified: Sat May 11 10:05:59 2024, max compression
```

## Comparing `scrapeddit-0.0.1.tar` & `scrapeddit-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 09:37:55.878161 scrapeddit-0.0.1/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1063 2024-05-11 09:03:02.000000 scrapeddit-0.0.1/LICENSE.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 09:37:55.877894 scrapeddit-0.0.1/PKG-INFO
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2735 2024-05-11 09:30:19.000000 scrapeddit-0.0.1/README.md
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 09:37:55.876289 scrapeddit-0.0.1/scrapeddit/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1516 2024-05-11 08:43:10.000000 scrapeddit-0.0.1/scrapeddit/Dataset.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       67 2024-05-11 08:50:08.000000 scrapeddit-0.0.1/scrapeddit/__init__.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2816 2024-05-11 08:43:10.000000 scrapeddit-0.0.1/scrapeddit/redditdl.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1158 2024-05-11 09:32:09.000000 scrapeddit-0.0.1/scrapeddit/scrapedit.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2396 2024-05-11 08:43:10.000000 scrapeddit-0.0.1/scrapeddit/showit.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      576 2024-05-11 08:43:10.000000 scrapeddit-0.0.1/scrapeddit/transforms.py
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 09:37:55.877567 scrapeddit-0.0.1/scrapeddit.egg-info/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 09:37:55.000000 scrapeddit-0.0.1/scrapeddit.egg-info/PKG-INFO
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      337 2024-05-11 09:37:55.000000 scrapeddit-0.0.1/scrapeddit.egg-info/SOURCES.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 09:37:55.000000 scrapeddit-0.0.1/scrapeddit.egg-info/dependency_links.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       15 2024-05-11 09:37:55.000000 scrapeddit-0.0.1/scrapeddit.egg-info/requires.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       11 2024-05-11 09:37:55.000000 scrapeddit-0.0.1/scrapeddit.egg-info/top_level.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       38 2024-05-11 09:37:55.878232 scrapeddit-0.0.1/setup.cfg
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      662 2024-05-11 09:37:54.000000 scrapeddit-0.0.1/setup.py
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 10:05:59.379099 scrapeddit-0.0.2/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1063 2024-05-11 09:03:02.000000 scrapeddit-0.0.2/LICENSE.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 10:05:59.378789 scrapeddit-0.0.2/PKG-INFO
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2735 2024-05-11 09:30:19.000000 scrapeddit-0.0.2/README.md
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 10:05:59.377185 scrapeddit-0.0.2/scrapeddit/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1516 2024-05-11 08:43:10.000000 scrapeddit-0.0.2/scrapeddit/Dataset.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       56 2024-05-11 10:04:07.000000 scrapeddit-0.0.2/scrapeddit/__init__.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2816 2024-05-11 08:43:10.000000 scrapeddit-0.0.2/scrapeddit/redditdl.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1158 2024-05-11 09:32:09.000000 scrapeddit-0.0.2/scrapeddit/scrapedit.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2396 2024-05-11 08:43:10.000000 scrapeddit-0.0.2/scrapeddit/showit.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      576 2024-05-11 08:43:10.000000 scrapeddit-0.0.2/scrapeddit/transforms.py
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 10:05:59.378519 scrapeddit-0.0.2/scrapeddit.egg-info/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 10:05:59.000000 scrapeddit-0.0.2/scrapeddit.egg-info/PKG-INFO
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      337 2024-05-11 10:05:59.000000 scrapeddit-0.0.2/scrapeddit.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:05:59.000000 scrapeddit-0.0.2/scrapeddit.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       15 2024-05-11 10:05:59.000000 scrapeddit-0.0.2/scrapeddit.egg-info/requires.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       11 2024-05-11 10:05:59.000000 scrapeddit-0.0.2/scrapeddit.egg-info/top_level.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       38 2024-05-11 10:05:59.379153 scrapeddit-0.0.2/setup.cfg
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      662 2024-05-11 10:04:53.000000 scrapeddit-0.0.2/setup.py
```

### Comparing `scrapeddit-0.0.1/LICENSE.txt` & `scrapeddit-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.0.1/PKG-INFO` & `scrapeddit-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapeddit
-Version: 0.0.1
+Version: 0.0.2
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
-Metadata-Version: 2.1 Name: scrapeddit Version: 0.0.1 Summary: Simple test
+Metadata-Version: 2.1 Name: scrapeddit Version: 0.0.2 Summary: Simple test
 package Home-page: https://github.com/Mafaz03/ReditScraper Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE.txt Requires-Dist: praw Requires-Dist: torchinfo
 ************ SSccrraappeeddddiitt ************
 ********** OOvveerrvviieeww **********
 Scrapeddit is a Python class designed for scraping images from Reddit
 subreddits and creating PyTorch datasets. It facilitates the collection of
```

### Comparing `scrapeddit-0.0.1/README.md` & `scrapeddit-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.0.1/scrapeddit/Dataset.py` & `scrapeddit-0.0.2/scrapeddit/Dataset.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.0.1/scrapeddit/redditdl.py` & `scrapeddit-0.0.2/scrapeddit/redditdl.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.0.1/scrapeddit/scrapedit.py` & `scrapeddit-0.0.2/scrapeddit/scrapedit.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.0.1/scrapeddit/showit.py` & `scrapeddit-0.0.2/scrapeddit/showit.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.0.1/scrapeddit/transforms.py` & `scrapeddit-0.0.2/scrapeddit/transforms.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.0.1/scrapeddit.egg-info/PKG-INFO` & `scrapeddit-0.0.2/scrapeddit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapeddit
-Version: 0.0.1
+Version: 0.0.2
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
-Metadata-Version: 2.1 Name: scrapeddit Version: 0.0.1 Summary: Simple test
+Metadata-Version: 2.1 Name: scrapeddit Version: 0.0.2 Summary: Simple test
 package Home-page: https://github.com/Mafaz03/ReditScraper Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE.txt Requires-Dist: praw Requires-Dist: torchinfo
 ************ SSccrraappeeddddiitt ************
 ********** OOvveerrvviieeww **********
 Scrapeddit is a Python class designed for scraping images from Reddit
 subreddits and creating PyTorch datasets. It facilitates the collection of
```

