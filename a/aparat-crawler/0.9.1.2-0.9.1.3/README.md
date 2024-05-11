# Comparing `tmp/aparat_crawler-0.9.1.2.tar.gz` & `tmp/aparat_crawler-0.9.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aparat_crawler-0.9.1.2.tar", last modified: Sat May 11 12:00:49 2024, max compression
+gzip compressed data, was "aparat_crawler-0.9.1.3.tar", last modified: Sat May 11 12:03:07 2024, max compression
```

## Comparing `aparat_crawler-0.9.1.2.tar` & `aparat_crawler-0.9.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 12:00:49.407030 aparat_crawler-0.9.1.2/
--rw-rw-rw-   0        0        0        0 2024-02-10 08:06:39.000000 aparat_crawler-0.9.1.2/LICENSE
--rw-rw-rw-   0        0        0      517 2024-05-11 12:00:49.407030 aparat_crawler-0.9.1.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-02-10 08:06:33.000000 aparat_crawler-0.9.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 12:00:49.379087 aparat_crawler-0.9.1.2/aparatCrawler/
--rw-rw-rw-   0        0        0        0 2024-02-10 08:06:03.000000 aparat_crawler-0.9.1.2/aparatCrawler/__init__.py
--rw-rw-rw-   0        0        0     1230 2024-03-01 09:13:38.000000 aparat_crawler-0.9.1.2/aparatCrawler/firstPageFetcher.py
--rw-rw-rw-   0        0        0     2867 2024-03-09 09:08:39.000000 aparat_crawler-0.9.1.2/aparatCrawler/getChanneldetails.py
--rw-rw-rw-   0        0        0      613 2024-03-01 09:15:04.000000 aparat_crawler-0.9.1.2/aparatCrawler/getOfficialChannels.py
--rw-rw-rw-   0        0        0      755 2024-03-01 09:15:27.000000 aparat_crawler-0.9.1.2/aparatCrawler/getVideoRecommndedChannles.py
--rw-rw-rw-   0        0        0     6153 2024-05-11 12:00:37.000000 aparat_crawler-0.9.1.2/aparatCrawler/getVideodetails.py
--rw-rw-rw-   0        0        0     7532 2024-05-11 10:46:18.000000 aparat_crawler-0.9.1.2/aparatCrawler/getchaneelVideosDetail.py
--rw-rw-rw-   0        0        0     2922 2024-03-01 09:14:44.000000 aparat_crawler-0.9.1.2/aparatCrawler/getchaneelVideosuid.py
--rw-rw-rw-   0        0        0     1894 2024-03-01 09:15:41.000000 aparat_crawler-0.9.1.2/aparatCrawler/search.py
-drwxrwxrwx   0        0        0        0 2024-05-11 12:00:49.405665 aparat_crawler-0.9.1.2/aparat_crawler.egg-info/
--rw-rw-rw-   0        0        0      517 2024-05-11 12:00:49.000000 aparat_crawler-0.9.1.2/aparat_crawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      535 2024-05-11 12:00:49.000000 aparat_crawler-0.9.1.2/aparat_crawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 12:00:49.000000 aparat_crawler-0.9.1.2/aparat_crawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2024-05-11 12:00:49.000000 aparat_crawler-0.9.1.2/aparat_crawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-11 12:00:49.000000 aparat_crawler-0.9.1.2/aparat_crawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-11 12:00:49.409694 aparat_crawler-0.9.1.2/setup.cfg
--rw-rw-rw-   0        0        0      669 2024-05-11 12:00:41.000000 aparat_crawler-0.9.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 12:03:07.035318 aparat_crawler-0.9.1.3/
+-rw-rw-rw-   0        0        0        0 2024-02-10 08:06:39.000000 aparat_crawler-0.9.1.3/LICENSE
+-rw-rw-rw-   0        0        0      517 2024-05-11 12:03:07.029290 aparat_crawler-0.9.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-02-10 08:06:33.000000 aparat_crawler-0.9.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 12:03:06.945007 aparat_crawler-0.9.1.3/aparatCrawler/
+-rw-rw-rw-   0        0        0        0 2024-02-10 08:06:03.000000 aparat_crawler-0.9.1.3/aparatCrawler/__init__.py
+-rw-rw-rw-   0        0        0     1230 2024-03-01 09:13:38.000000 aparat_crawler-0.9.1.3/aparatCrawler/firstPageFetcher.py
+-rw-rw-rw-   0        0        0     2867 2024-03-09 09:08:39.000000 aparat_crawler-0.9.1.3/aparatCrawler/getChanneldetails.py
+-rw-rw-rw-   0        0        0      613 2024-03-01 09:15:04.000000 aparat_crawler-0.9.1.3/aparatCrawler/getOfficialChannels.py
+-rw-rw-rw-   0        0        0      755 2024-03-01 09:15:27.000000 aparat_crawler-0.9.1.3/aparatCrawler/getVideoRecommndedChannles.py
+-rw-rw-rw-   0        0        0     6155 2024-05-11 12:02:58.000000 aparat_crawler-0.9.1.3/aparatCrawler/getVideodetails.py
+-rw-rw-rw-   0        0        0     7532 2024-05-11 10:46:18.000000 aparat_crawler-0.9.1.3/aparatCrawler/getchaneelVideosDetail.py
+-rw-rw-rw-   0        0        0     2922 2024-03-01 09:14:44.000000 aparat_crawler-0.9.1.3/aparatCrawler/getchaneelVideosuid.py
+-rw-rw-rw-   0        0        0     1894 2024-03-01 09:15:41.000000 aparat_crawler-0.9.1.3/aparatCrawler/search.py
+drwxrwxrwx   0        0        0        0 2024-05-11 12:03:07.026552 aparat_crawler-0.9.1.3/aparat_crawler.egg-info/
+-rw-rw-rw-   0        0        0      517 2024-05-11 12:03:06.000000 aparat_crawler-0.9.1.3/aparat_crawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      535 2024-05-11 12:03:06.000000 aparat_crawler-0.9.1.3/aparat_crawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 12:03:06.000000 aparat_crawler-0.9.1.3/aparat_crawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2024-05-11 12:03:06.000000 aparat_crawler-0.9.1.3/aparat_crawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-11 12:03:06.000000 aparat_crawler-0.9.1.3/aparat_crawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-11 12:03:07.040830 aparat_crawler-0.9.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      669 2024-05-11 12:03:02.000000 aparat_crawler-0.9.1.3/setup.py
```

### Comparing `aparat_crawler-0.9.1.2/PKG-INFO` & `aparat_crawler-0.9.1.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aparat_crawler
-Version: 0.9.1.2
+Version: 0.9.1.3
 Summary: this is an aparat crawler library
 Home-page: https://github.com/maorojloo/aparat_crawler
 Author: Mohammad Amin Orojloo
 Author-email: ma.orojloo@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aparat_crawler-0.9.1.2/aparatCrawler/firstPageFetcher.py` & `aparat_crawler-0.9.1.3/aparatCrawler/firstPageFetcher.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1.2/aparatCrawler/getChanneldetails.py` & `aparat_crawler-0.9.1.3/aparatCrawler/getChanneldetails.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1.2/aparatCrawler/getOfficialChannels.py` & `aparat_crawler-0.9.1.3/aparatCrawler/getOfficialChannels.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1.2/aparatCrawler/getVideoRecommndedChannles.py` & `aparat_crawler-0.9.1.3/aparatCrawler/getVideoRecommndedChannles.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1.2/aparatCrawler/getVideodetails.py` & `aparat_crawler-0.9.1.3/aparatCrawler/getVideodetails.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,18 +98,18 @@
         "owner_name":data["included"][0]["attributes"]["name"] ,
         
         "poster":included["attributes"]["big_poster"] if "big_poster" in included["attributes"] else None,
         "owner_avatar":data["included"][0]["attributes"]["avatar"],
         "duration":int(included["attributes"]["duration"]) if "duration" in included["attributes"] else 0,
         "posted_date":included["attributes"]["sdate_real"] if "sdate_real" in included["attributes"] else included["attributes"]["sdate_rss"],
 
-        "posted_timestamp":int(included["attributes"]["sdate_real"] if "sdate_real" in included["attributes"] else included["attributes"]["sdate_rss"], "%Y-%m-%d %H:%M:%S").timestamp())-12600 ,#2015-05-17 12:12:51 ##-12600 to convert iran timezone to utc
+        "posted_timestamp":(int(included["attributes"]["sdate_real"] if "sdate_real" in included["attributes"] else included["attributes"]["sdate_rss"], "%Y-%m-%d %H:%M:%S").timestamp())-12600 ,#2015-05-17 12:12:51 ##-12600 to convert iran timezone to utc
         
         "sdate_rss":included["attributes"]["sdate_rss"] ,
-        "sdate_rss_tp":int(included["attributes"]["sdate_real"] if "sdate_real" in included["attributes"] else included["attributes"]["sdate_rss"], "%Y-%m-%d %H:%M:%S").timestamp())-12600 ,#2015-05-17 12:12:51 ##-12600 to convert iran timezone to utc
+        "sdate_rss_tp":(int(included["attributes"]["sdate_real"] if "sdate_real" in included["attributes"] else included["attributes"]["sdate_rss"], "%Y-%m-%d %H:%M:%S").timestamp())-12600 ,#2015-05-17 12:12:51 ##-12600 to convert iran timezone to utc
         "comments":None,
         "frame":included["attributes"]["frame"] if "frame" in included["attributes"] else None,
         "like_count":int(included["attributes"]["like_cnt_non_formatted"]) if "like_cnt_non_formatted" in included["attributes"] else int(included["attributes"]["like_cnt"]),
         "description":included["attributes"]["description"] if "description" in included["attributes"]  else None,
         "is_deleted": False,
 
     }
```

### Comparing `aparat_crawler-0.9.1.2/aparatCrawler/getchaneelVideosDetail.py` & `aparat_crawler-0.9.1.3/aparatCrawler/getchaneelVideosDetail.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1.2/aparatCrawler/getchaneelVideosuid.py` & `aparat_crawler-0.9.1.3/aparatCrawler/getchaneelVideosuid.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1.2/aparatCrawler/search.py` & `aparat_crawler-0.9.1.3/aparatCrawler/search.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1.2/aparat_crawler.egg-info/PKG-INFO` & `aparat_crawler-0.9.1.3/aparat_crawler.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aparat_crawler
-Version: 0.9.1.2
+Version: 0.9.1.3
 Summary: this is an aparat crawler library
 Home-page: https://github.com/maorojloo/aparat_crawler
 Author: Mohammad Amin Orojloo
 Author-email: ma.orojloo@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aparat_crawler-0.9.1.2/aparat_crawler.egg-info/SOURCES.txt` & `aparat_crawler-0.9.1.3/aparat_crawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.9.1.2/setup.py` & `aparat_crawler-0.9.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aparat_crawler',
-    version='0.9.1.2',
+    version='0.9.1.3',
     packages=find_packages(),
     author='Mohammad Amin Orojloo',
     author_email='ma.orojloo@gmail.com',
     description='this is an aparat crawler library',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/maorojloo/aparat_crawler',
```

