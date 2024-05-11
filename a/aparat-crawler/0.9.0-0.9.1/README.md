# Comparing `tmp/aparat_crawler-0.9.0.tar.gz` & `tmp/aparat_crawler-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aparat_crawler-0.9.0.tar", last modified: Sat May 11 11:17:34 2024, max compression
+gzip compressed data, was "aparat_crawler-0.9.1.tar", last modified: Sat May 11 11:41:44 2024, max compression
```

## Comparing `aparat_crawler-0.9.0.tar` & `aparat_crawler-0.9.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 11:17:34.069132 aparat_crawler-0.9.0/
--rw-rw-rw-   0        0        0        0 2024-02-10 08:06:39.000000 aparat_crawler-0.9.0/LICENSE
--rw-rw-rw-   0        0        0      515 2024-05-11 11:17:34.069132 aparat_crawler-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-02-10 08:06:33.000000 aparat_crawler-0.9.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 11:17:34.040523 aparat_crawler-0.9.0/aparatCrawler/
--rw-rw-rw-   0        0        0        0 2024-02-10 08:06:03.000000 aparat_crawler-0.9.0/aparatCrawler/__init__.py
--rw-rw-rw-   0        0        0     1230 2024-03-01 09:13:38.000000 aparat_crawler-0.9.0/aparatCrawler/firstPageFetcher.py
--rw-rw-rw-   0        0        0     2867 2024-03-09 09:08:39.000000 aparat_crawler-0.9.0/aparatCrawler/getChanneldetails.py
--rw-rw-rw-   0        0        0      613 2024-03-01 09:15:04.000000 aparat_crawler-0.9.0/aparatCrawler/getOfficialChannels.py
--rw-rw-rw-   0        0        0      755 2024-03-01 09:15:27.000000 aparat_crawler-0.9.0/aparatCrawler/getVideoRecommndedChannles.py
--rw-rw-rw-   0        0        0     5753 2024-03-09 09:07:54.000000 aparat_crawler-0.9.0/aparatCrawler/getVideodetails.py
--rw-rw-rw-   0        0        0     7532 2024-05-11 10:46:18.000000 aparat_crawler-0.9.0/aparatCrawler/getchaneelVideosDetail.py
--rw-rw-rw-   0        0        0     2922 2024-03-01 09:14:44.000000 aparat_crawler-0.9.0/aparatCrawler/getchaneelVideosuid.py
--rw-rw-rw-   0        0        0     1894 2024-03-01 09:15:41.000000 aparat_crawler-0.9.0/aparatCrawler/search.py
-drwxrwxrwx   0        0        0        0 2024-05-11 11:17:34.066398 aparat_crawler-0.9.0/aparat_crawler.egg-info/
--rw-rw-rw-   0        0        0      515 2024-05-11 11:17:33.000000 aparat_crawler-0.9.0/aparat_crawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      535 2024-05-11 11:17:33.000000 aparat_crawler-0.9.0/aparat_crawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 11:17:33.000000 aparat_crawler-0.9.0/aparat_crawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2024-05-11 11:17:33.000000 aparat_crawler-0.9.0/aparat_crawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-11 11:17:33.000000 aparat_crawler-0.9.0/aparat_crawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-11 11:17:34.071642 aparat_crawler-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0      667 2024-05-11 10:46:30.000000 aparat_crawler-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 11:41:44.886324 aparat_crawler-0.9.1/
+-rw-rw-rw-   0        0        0        0 2024-02-10 08:06:39.000000 aparat_crawler-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0      515 2024-05-11 11:41:44.885283 aparat_crawler-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-02-10 08:06:33.000000 aparat_crawler-0.9.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 11:41:44.840759 aparat_crawler-0.9.1/aparatCrawler/
+-rw-rw-rw-   0        0        0        0 2024-02-10 08:06:03.000000 aparat_crawler-0.9.1/aparatCrawler/__init__.py
+-rw-rw-rw-   0        0        0     1230 2024-03-01 09:13:38.000000 aparat_crawler-0.9.1/aparatCrawler/firstPageFetcher.py
+-rw-rw-rw-   0        0        0     2867 2024-03-09 09:08:39.000000 aparat_crawler-0.9.1/aparatCrawler/getChanneldetails.py
+-rw-rw-rw-   0        0        0      613 2024-03-01 09:15:04.000000 aparat_crawler-0.9.1/aparatCrawler/getOfficialChannels.py
+-rw-rw-rw-   0        0        0      755 2024-03-01 09:15:27.000000 aparat_crawler-0.9.1/aparatCrawler/getVideoRecommndedChannles.py
+-rw-rw-rw-   0        0        0     5858 2024-05-11 11:39:51.000000 aparat_crawler-0.9.1/aparatCrawler/getVideodetails.py
+-rw-rw-rw-   0        0        0     7532 2024-05-11 10:46:18.000000 aparat_crawler-0.9.1/aparatCrawler/getchaneelVideosDetail.py
+-rw-rw-rw-   0        0        0     2922 2024-03-01 09:14:44.000000 aparat_crawler-0.9.1/aparatCrawler/getchaneelVideosuid.py
+-rw-rw-rw-   0        0        0     1894 2024-03-01 09:15:41.000000 aparat_crawler-0.9.1/aparatCrawler/search.py
+drwxrwxrwx   0        0        0        0 2024-05-11 11:41:44.879007 aparat_crawler-0.9.1/aparat_crawler.egg-info/
+-rw-rw-rw-   0        0        0      515 2024-05-11 11:41:44.000000 aparat_crawler-0.9.1/aparat_crawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      535 2024-05-11 11:41:44.000000 aparat_crawler-0.9.1/aparat_crawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 11:41:44.000000 aparat_crawler-0.9.1/aparat_crawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2024-05-11 11:41:44.000000 aparat_crawler-0.9.1/aparat_crawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-11 11:41:44.000000 aparat_crawler-0.9.1/aparat_crawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-11 11:41:44.890357 aparat_crawler-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      667 2024-05-11 11:41:36.000000 aparat_crawler-0.9.1/setup.py
```

### Comparing `aparat_crawler-0.9.0/PKG-INFO` & `aparat_crawler-0.9.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aparat_crawler
-Version: 0.9.0
+Version: 0.9.1
 Summary: this is an aparat crawler library
 Home-page: https://github.com/maorojloo/aparat_crawler
 Author: Mohammad Amin Orojloo
 Author-email: ma.orojloo@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aparat_crawler-0.9.0/aparatCrawler/firstPageFetcher.py` & `aparat_crawler-0.9.1/aparatCrawler/firstPageFetcher.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.0/aparatCrawler/getChanneldetails.py` & `aparat_crawler-0.9.1/aparatCrawler/getChanneldetails.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.0/aparatCrawler/getOfficialChannels.py` & `aparat_crawler-0.9.1/aparatCrawler/getOfficialChannels.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.0/aparatCrawler/getVideoRecommndedChannles.py` & `aparat_crawler-0.9.1/aparatCrawler/getVideoRecommndedChannles.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.0/aparatCrawler/getVideodetails.py` & `aparat_crawler-0.9.1/aparatCrawler/getVideodetails.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,16 +67,21 @@
         async with session.get(url) as response:
             if response.status != 200:
                 raise Exception(f"Aparat api error {response.status}")
             data = await response.json()
 
 
 
+    included=None
+    if isinstance(data["data"], list):
+        included=data["data"][0]
+    else:
+        included=data["data"]
     
-    included=data["data"]
+
     
     
     
 
     
     video={
         "platform": "aparat",
```

### Comparing `aparat_crawler-0.9.0/aparatCrawler/getchaneelVideosDetail.py` & `aparat_crawler-0.9.1/aparatCrawler/getchaneelVideosDetail.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.0/aparatCrawler/getchaneelVideosuid.py` & `aparat_crawler-0.9.1/aparatCrawler/getchaneelVideosuid.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.0/aparatCrawler/search.py` & `aparat_crawler-0.9.1/aparatCrawler/search.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.0/aparat_crawler.egg-info/PKG-INFO` & `aparat_crawler-0.9.1/aparat_crawler.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aparat_crawler
-Version: 0.9.0
+Version: 0.9.1
 Summary: this is an aparat crawler library
 Home-page: https://github.com/maorojloo/aparat_crawler
 Author: Mohammad Amin Orojloo
 Author-email: ma.orojloo@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aparat_crawler-0.9.0/aparat_crawler.egg-info/SOURCES.txt` & `aparat_crawler-0.9.1/aparat_crawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.0/setup.py` & `aparat_crawler-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aparat_crawler',
-    version='0.9.0',
+    version='0.9.1',
     packages=find_packages(),
     author='Mohammad Amin Orojloo',
     author_email='ma.orojloo@gmail.com',
     description='this is an aparat crawler library',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/maorojloo/aparat_crawler',
```

