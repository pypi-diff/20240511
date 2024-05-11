# Comparing `tmp/aparat_crawler-0.8.9.tar.gz` & `tmp/aparat_crawler-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aparat_crawler-0.8.9.tar", last modified: Sat Mar  9 09:09:50 2024, max compression
+gzip compressed data, was "aparat_crawler-0.9.0.tar", last modified: Sat May 11 11:17:34 2024, max compression
```

## Comparing `aparat_crawler-0.8.9.tar` & `aparat_crawler-0.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 maorojloo  (1000) maorojloo  (1000)        0 2024-03-09 09:09:50.988996 aparat_crawler-0.8.9/
--rw-rw-r--   0 maorojloo  (1000) maorojloo  (1000)        0 2024-02-10 08:06:39.000000 aparat_crawler-0.8.9/LICENSE
--rw-r--r--   0 maorojloo  (1000) maorojloo  (1000)      500 2024-03-09 09:09:50.988996 aparat_crawler-0.8.9/PKG-INFO
--rw-rw-r--   0 maorojloo  (1000) maorojloo  (1000)        0 2024-02-10 08:06:33.000000 aparat_crawler-0.8.9/README.md
-drwxrwxr-x   0 maorojloo  (1000) maorojloo  (1000)        0 2024-03-09 09:09:50.984995 aparat_crawler-0.8.9/aparatCrawler/
--rw-rw-r--   0 maorojloo  (1000) maorojloo  (1000)        0 2024-02-10 08:06:03.000000 aparat_crawler-0.8.9/aparatCrawler/__init__.py
--rw-rw-r--   0 maorojloo  (1000) maorojloo  (1000)     1230 2024-03-01 09:13:38.000000 aparat_crawler-0.8.9/aparatCrawler/firstPageFetcher.py
--rw-rw-r--   0 maorojloo  (1000) maorojloo  (1000)     2867 2024-03-09 09:08:39.000000 aparat_crawler-0.8.9/aparatCrawler/getChanneldetails.py
--rw-rw-r--   0 maorojloo  (1000) maorojloo  (1000)      613 2024-03-01 09:15:04.000000 aparat_crawler-0.8.9/aparatCrawler/getOfficialChannels.py
--rw-rw-r--   0 maorojloo  (1000) maorojloo  (1000)      755 2024-03-01 09:15:27.000000 aparat_crawler-0.8.9/aparatCrawler/getVideoRecommndedChannles.py
--rw-rw-r--   0 maorojloo  (1000) maorojloo  (1000)     5753 2024-03-09 09:07:54.000000 aparat_crawler-0.8.9/aparatCrawler/getVideodetails.py
--rw-rw-r--   0 maorojloo  (1000) maorojloo  (1000)     7535 2024-03-03 06:32:01.000000 aparat_crawler-0.8.9/aparatCrawler/getchaneelVideosDetail.py
--rw-rw-r--   0 maorojloo  (1000) maorojloo  (1000)     2922 2024-03-01 09:14:44.000000 aparat_crawler-0.8.9/aparatCrawler/getchaneelVideosuid.py
--rw-rw-r--   0 maorojloo  (1000) maorojloo  (1000)     1894 2024-03-01 09:15:41.000000 aparat_crawler-0.8.9/aparatCrawler/search.py
-drwxrwxr-x   0 maorojloo  (1000) maorojloo  (1000)        0 2024-03-09 09:09:50.988996 aparat_crawler-0.8.9/aparat_crawler.egg-info/
--rw-r--r--   0 maorojloo  (1000) maorojloo  (1000)      500 2024-03-09 09:09:50.000000 aparat_crawler-0.8.9/aparat_crawler.egg-info/PKG-INFO
--rw-rw-r--   0 maorojloo  (1000) maorojloo  (1000)      535 2024-03-09 09:09:50.000000 aparat_crawler-0.8.9/aparat_crawler.egg-info/SOURCES.txt
--rw-rw-r--   0 maorojloo  (1000) maorojloo  (1000)        1 2024-03-09 09:09:50.000000 aparat_crawler-0.8.9/aparat_crawler.egg-info/dependency_links.txt
--rw-rw-r--   0 maorojloo  (1000) maorojloo  (1000)       91 2024-03-09 09:09:50.000000 aparat_crawler-0.8.9/aparat_crawler.egg-info/requires.txt
--rw-rw-r--   0 maorojloo  (1000) maorojloo  (1000)       14 2024-03-09 09:09:50.000000 aparat_crawler-0.8.9/aparat_crawler.egg-info/top_level.txt
--rw-rw-r--   0 maorojloo  (1000) maorojloo  (1000)       38 2024-03-09 09:09:50.988996 aparat_crawler-0.8.9/setup.cfg
--rw-rw-r--   0 maorojloo  (1000) maorojloo  (1000)      667 2024-03-09 08:59:35.000000 aparat_crawler-0.8.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 11:17:34.069132 aparat_crawler-0.9.0/
+-rw-rw-rw-   0        0        0        0 2024-02-10 08:06:39.000000 aparat_crawler-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0      515 2024-05-11 11:17:34.069132 aparat_crawler-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-02-10 08:06:33.000000 aparat_crawler-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 11:17:34.040523 aparat_crawler-0.9.0/aparatCrawler/
+-rw-rw-rw-   0        0        0        0 2024-02-10 08:06:03.000000 aparat_crawler-0.9.0/aparatCrawler/__init__.py
+-rw-rw-rw-   0        0        0     1230 2024-03-01 09:13:38.000000 aparat_crawler-0.9.0/aparatCrawler/firstPageFetcher.py
+-rw-rw-rw-   0        0        0     2867 2024-03-09 09:08:39.000000 aparat_crawler-0.9.0/aparatCrawler/getChanneldetails.py
+-rw-rw-rw-   0        0        0      613 2024-03-01 09:15:04.000000 aparat_crawler-0.9.0/aparatCrawler/getOfficialChannels.py
+-rw-rw-rw-   0        0        0      755 2024-03-01 09:15:27.000000 aparat_crawler-0.9.0/aparatCrawler/getVideoRecommndedChannles.py
+-rw-rw-rw-   0        0        0     5753 2024-03-09 09:07:54.000000 aparat_crawler-0.9.0/aparatCrawler/getVideodetails.py
+-rw-rw-rw-   0        0        0     7532 2024-05-11 10:46:18.000000 aparat_crawler-0.9.0/aparatCrawler/getchaneelVideosDetail.py
+-rw-rw-rw-   0        0        0     2922 2024-03-01 09:14:44.000000 aparat_crawler-0.9.0/aparatCrawler/getchaneelVideosuid.py
+-rw-rw-rw-   0        0        0     1894 2024-03-01 09:15:41.000000 aparat_crawler-0.9.0/aparatCrawler/search.py
+drwxrwxrwx   0        0        0        0 2024-05-11 11:17:34.066398 aparat_crawler-0.9.0/aparat_crawler.egg-info/
+-rw-rw-rw-   0        0        0      515 2024-05-11 11:17:33.000000 aparat_crawler-0.9.0/aparat_crawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      535 2024-05-11 11:17:33.000000 aparat_crawler-0.9.0/aparat_crawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 11:17:33.000000 aparat_crawler-0.9.0/aparat_crawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2024-05-11 11:17:33.000000 aparat_crawler-0.9.0/aparat_crawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-11 11:17:33.000000 aparat_crawler-0.9.0/aparat_crawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-11 11:17:34.071642 aparat_crawler-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      667 2024-05-11 10:46:30.000000 aparat_crawler-0.9.0/setup.py
```

### Comparing `aparat_crawler-0.8.9/aparatCrawler/firstPageFetcher.py` & `aparat_crawler-0.9.0/aparatCrawler/firstPageFetcher.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.8.9/aparatCrawler/getChanneldetails.py` & `aparat_crawler-0.9.0/aparatCrawler/getChanneldetails.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.8.9/aparatCrawler/getOfficialChannels.py` & `aparat_crawler-0.9.0/aparatCrawler/getOfficialChannels.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.8.9/aparatCrawler/getVideoRecommndedChannles.py` & `aparat_crawler-0.9.0/aparatCrawler/getVideoRecommndedChannles.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.8.9/aparatCrawler/getVideodetails.py` & `aparat_crawler-0.9.0/aparatCrawler/getVideodetails.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.8.9/aparatCrawler/getchaneelVideosDetail.py` & `aparat_crawler-0.9.0/aparatCrawler/getchaneelVideosDetail.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,26 @@
 
 timeout_seconds=10
 
 def getchannelvideocount(username,proxy=None):
     response=None
     url = "https://www.aparat.com/api/fa/v1/user/user/information/username/" + username
     try:
-        if proxy==None:
-            response = requests.request("GET", url, proxies=proxy, timeout=10)
-        else:
-            response = requests.request("GET", url, timeout=10)
+        response = requests.request("GET", url, proxies=proxy, timeout=10)
+
     except Timeout:
         print("The request timed out after 10 seconds.")
     except requests.RequestException as e:
         print(f"An error occurred: {e}")
 
     if response.status_code == 404:
         return 404
+    if response.status_code == 429:
+        print("we have got 429 ERROR")
+        return 429        
     data = response.json()
     video_cnt=int(data["data"]["attributes"]["video_cnt"])
 
     return video_cnt
 
 
 def get_video_commnets(video_uid,proxy=None):
```

### Comparing `aparat_crawler-0.8.9/aparatCrawler/getchaneelVideosuid.py` & `aparat_crawler-0.9.0/aparatCrawler/getchaneelVideosuid.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.8.9/aparatCrawler/search.py` & `aparat_crawler-0.9.0/aparatCrawler/search.py`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.8.9/aparat_crawler.egg-info/SOURCES.txt` & `aparat_crawler-0.9.0/aparat_crawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aparat_crawler-0.8.9/setup.py` & `aparat_crawler-0.9.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aparat_crawler',
-    version='0.8.9',
+    version='0.9.0',
     packages=find_packages(),
     author='Mohammad Amin Orojloo',
     author_email='ma.orojloo@gmail.com',
     description='this is an aparat crawler library',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/maorojloo/aparat_crawler',
```

