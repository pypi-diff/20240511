# Comparing `tmp/aparat_crawler-0.9.1.tar.gz` & `tmp/aparat_crawler-0.9.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aparat_crawler-0.9.1.tar", last modified: Sat May 11 11:41:44 2024, max compression
+gzip compressed data, was "aparat_crawler-0.9.1.1.tar", last modified: Sat May 11 11:48:44 2024, max compression
```

## Comparing `aparat_crawler-0.9.1.tar` & `aparat_crawler-0.9.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 11:41:44.886324 aparat_crawler-0.9.1/
--rw-rw-rw-   0        0        0        0 2024-02-10 08:06:39.000000 aparat_crawler-0.9.1/LICENSE
--rw-rw-rw-   0        0        0      515 2024-05-11 11:41:44.885283 aparat_crawler-0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-02-10 08:06:33.000000 aparat_crawler-0.9.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 11:41:44.840759 aparat_crawler-0.9.1/aparatCrawler/
--rw-rw-rw-   0        0        0        0 2024-02-10 08:06:03.000000 aparat_crawler-0.9.1/aparatCrawler/__init__.py
--rw-rw-rw-   0        0        0     1230 2024-03-01 09:13:38.000000 aparat_crawler-0.9.1/aparatCrawler/firstPageFetcher.py
--rw-rw-rw-   0        0        0     2867 2024-03-09 09:08:39.000000 aparat_crawler-0.9.1/aparatCrawler/getChanneldetails.py
--rw-rw-rw-   0        0        0      613 2024-03-01 09:15:04.000000 aparat_crawler-0.9.1/aparatCrawler/getOfficialChannels.py
--rw-rw-rw-   0        0        0      755 2024-03-01 09:15:27.000000 aparat_crawler-0.9.1/aparatCrawler/getVideoRecommndedChannles.py
--rw-rw-rw-   0        0        0     5858 2024-05-11 11:39:51.000000 aparat_crawler-0.9.1/aparatCrawler/getVideodetails.py
--rw-rw-rw-   0        0        0     7532 2024-05-11 10:46:18.000000 aparat_crawler-0.9.1/aparatCrawler/getchaneelVideosDetail.py
--rw-rw-rw-   0        0        0     2922 2024-03-01 09:14:44.000000 aparat_crawler-0.9.1/aparatCrawler/getchaneelVideosuid.py
--rw-rw-rw-   0        0        0     1894 2024-03-01 09:15:41.000000 aparat_crawler-0.9.1/aparatCrawler/search.py
-drwxrwxrwx   0        0        0        0 2024-05-11 11:41:44.879007 aparat_crawler-0.9.1/aparat_crawler.egg-info/
--rw-rw-rw-   0        0        0      515 2024-05-11 11:41:44.000000 aparat_crawler-0.9.1/aparat_crawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      535 2024-05-11 11:41:44.000000 aparat_crawler-0.9.1/aparat_crawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 11:41:44.000000 aparat_crawler-0.9.1/aparat_crawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2024-05-11 11:41:44.000000 aparat_crawler-0.9.1/aparat_crawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-11 11:41:44.000000 aparat_crawler-0.9.1/aparat_crawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-11 11:41:44.890357 aparat_crawler-0.9.1/setup.cfg
--rw-rw-rw-   0        0        0      667 2024-05-11 11:41:36.000000 aparat_crawler-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 11:48:44.699640 aparat_crawler-0.9.1.1/
+-rw-rw-rw-   0        0        0        0 2024-02-10 08:06:39.000000 aparat_crawler-0.9.1.1/LICENSE
+-rw-rw-rw-   0        0        0      517 2024-05-11 11:48:44.698638 aparat_crawler-0.9.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-02-10 08:06:33.000000 aparat_crawler-0.9.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 11:48:44.671485 aparat_crawler-0.9.1.1/aparatCrawler/
+-rw-rw-rw-   0        0        0        0 2024-02-10 08:06:03.000000 aparat_crawler-0.9.1.1/aparatCrawler/__init__.py
+-rw-rw-rw-   0        0        0     1230 2024-03-01 09:13:38.000000 aparat_crawler-0.9.1.1/aparatCrawler/firstPageFetcher.py
+-rw-rw-rw-   0        0        0     2867 2024-03-09 09:08:39.000000 aparat_crawler-0.9.1.1/aparatCrawler/getChanneldetails.py
+-rw-rw-rw-   0        0        0      613 2024-03-01 09:15:04.000000 aparat_crawler-0.9.1.1/aparatCrawler/getOfficialChannels.py
+-rw-rw-rw-   0        0        0      755 2024-03-01 09:15:27.000000 aparat_crawler-0.9.1.1/aparatCrawler/getVideoRecommndedChannles.py
+-rw-rw-rw-   0        0        0     5959 2024-05-11 11:48:28.000000 aparat_crawler-0.9.1.1/aparatCrawler/getVideodetails.py
+-rw-rw-rw-   0        0        0     7532 2024-05-11 10:46:18.000000 aparat_crawler-0.9.1.1/aparatCrawler/getchaneelVideosDetail.py
+-rw-rw-rw-   0        0        0     2922 2024-03-01 09:14:44.000000 aparat_crawler-0.9.1.1/aparatCrawler/getchaneelVideosuid.py
+-rw-rw-rw-   0        0        0     1894 2024-03-01 09:15:41.000000 aparat_crawler-0.9.1.1/aparatCrawler/search.py
+drwxrwxrwx   0        0        0        0 2024-05-11 11:48:44.697635 aparat_crawler-0.9.1.1/aparat_crawler.egg-info/
+-rw-rw-rw-   0        0        0      517 2024-05-11 11:48:44.000000 aparat_crawler-0.9.1.1/aparat_crawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      535 2024-05-11 11:48:44.000000 aparat_crawler-0.9.1.1/aparat_crawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 11:48:44.000000 aparat_crawler-0.9.1.1/aparat_crawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2024-05-11 11:48:44.000000 aparat_crawler-0.9.1.1/aparat_crawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-11 11:48:44.000000 aparat_crawler-0.9.1.1/aparat_crawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-11 11:48:44.701647 aparat_crawler-0.9.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      669 2024-05-11 11:48:32.000000 aparat_crawler-0.9.1.1/setup.py
```

### Comparing `aparat_crawler-0.9.1/PKG-INFO` & `aparat_crawler-0.9.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aparat_crawler
-Version: 0.9.1
+Version: 0.9.1.1
 Summary: this is an aparat crawler library
 Home-page: https://github.com/maorojloo/aparat_crawler
 Author: Mohammad Amin Orojloo
 Author-email: ma.orojloo@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aparat_crawler-0.9.1/aparatCrawler/firstPageFetcher.py` & `aparat_crawler-0.9.1.1/aparatCrawler/firstPageFetcher.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1/aparatCrawler/getChanneldetails.py` & `aparat_crawler-0.9.1.1/aparatCrawler/getChanneldetails.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1/aparatCrawler/getOfficialChannels.py` & `aparat_crawler-0.9.1.1/aparatCrawler/getOfficialChannels.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1/aparatCrawler/getVideoRecommndedChannles.py` & `aparat_crawler-0.9.1.1/aparatCrawler/getVideoRecommndedChannles.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1/aparatCrawler/getVideodetails.py` & `aparat_crawler-0.9.1.1/aparatCrawler/getVideodetails.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,16 @@
         "_":"video",
         "id":included["id"] if "id" in included else None,
         "owner_username":included["attributes"]["owner_username"] if "owner_username" in included["attributes"] else None,
         "owner_id":int(included["relationships"]["Channel"]["data"]["id"]) ,
         "title":included["attributes"]["title"] if "title" in included["attributes"] else None,
         "tags":included["attributes"]["tags"] if "tags" in included["attributes"] else None,
         "uid":included["attributes"]["uid"] if "uid" in included["attributes"] else None,
-        "visit_count":int(included["attributes"]["visit_cnt_non_formatted"]),
+
+        "visit_count":int(included["attributes"]["visit_cnt_non_formatted"]) if "visit_cnt_non_formatted" in included["attributes"] else included["attributes"]["visit_cnt_int"],
         
         "owner_name":data["included"][0]["attributes"]["name"] ,
         
         "poster":included["attributes"]["big_poster"] if "big_poster" in included["attributes"] else None,
         "owner_avatar":data["included"][0]["attributes"]["avatar"],
         "duration":int(included["attributes"]["duration"]) if "duration" in included["attributes"] else 0,
         "posted_date":included["attributes"]["sdate_real"] ,
```

### Comparing `aparat_crawler-0.9.1/aparatCrawler/getchaneelVideosDetail.py` & `aparat_crawler-0.9.1.1/aparatCrawler/getchaneelVideosDetail.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1/aparatCrawler/getchaneelVideosuid.py` & `aparat_crawler-0.9.1.1/aparatCrawler/getchaneelVideosuid.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1/aparatCrawler/search.py` & `aparat_crawler-0.9.1.1/aparatCrawler/search.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1/aparat_crawler.egg-info/PKG-INFO` & `aparat_crawler-0.9.1.1/aparat_crawler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aparat_crawler
-Version: 0.9.1
+Version: 0.9.1.1
 Summary: this is an aparat crawler library
 Home-page: https://github.com/maorojloo/aparat_crawler
 Author: Mohammad Amin Orojloo
 Author-email: ma.orojloo@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aparat_crawler-0.9.1/aparat_crawler.egg-info/SOURCES.txt` & `aparat_crawler-0.9.1.1/aparat_crawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1/setup.py` & `aparat_crawler-0.9.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aparat_crawler',
-    version='0.9.1',
+    version='0.9.1.1',
     packages=find_packages(),
     author='Mohammad Amin Orojloo',
     author_email='ma.orojloo@gmail.com',
     description='this is an aparat crawler library',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/maorojloo/aparat_crawler',
```

