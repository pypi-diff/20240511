# Comparing `tmp/gnews-0.3.6.tar.gz` & `tmp/gnews-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnews-0.3.6.tar", last modified: Tue Oct 31 18:08:44 2023, max compression
+gzip compressed data, was "gnews-0.3.7.tar", last modified: Sat May 11 09:32:56 2024, max compression
```

## Comparing `gnews-0.3.6.tar` & `gnews-0.3.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 18:08:44.981491 gnews-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-10-31 18:08:32.000000 gnews-0.3.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17482 2023-10-31 18:08:44.981491 gnews-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16228 2023-10-31 18:08:32.000000 gnews-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 18:08:44.981491 gnews-0.3.6/gnews/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-10-31 18:08:32.000000 gnews-0.3.6/gnews/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13199 2023-10-31 18:08:32.000000 gnews-0.3.6/gnews/gnews.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 18:08:44.981491 gnews-0.3.6/gnews/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-31 18:08:32.000000 gnews-0.3.6/gnews/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24441 2023-10-31 18:08:32.000000 gnews-0.3.6/gnews/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2023-10-31 18:08:32.000000 gnews-0.3.6/gnews/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 18:08:44.981491 gnews-0.3.6/gnews.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17482 2023-10-31 18:08:44.000000 gnews-0.3.6/gnews.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      297 2023-10-31 18:08:44.000000 gnews-0.3.6/gnews.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-31 18:08:44.000000 gnews-0.3.6/gnews.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-10-31 18:08:44.000000 gnews-0.3.6/gnews.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-10-31 18:08:44.000000 gnews-0.3.6/gnews.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-31 18:08:44.981491 gnews-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2023-10-31 18:08:32.000000 gnews-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 18:08:44.981491 gnews-0.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2023-10-31 18:08:32.000000 gnews-0.3.6/tests/test_gnews.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 09:32:56.562312 gnews-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-11 09:32:53.000000 gnews-0.3.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17333 2024-05-11 09:32:56.562312 gnews-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16228 2024-05-11 09:32:53.000000 gnews-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 09:32:56.562312 gnews-0.3.7/gnews/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-11 09:32:53.000000 gnews-0.3.7/gnews/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12332 2024-05-11 09:32:53.000000 gnews-0.3.7/gnews/gnews.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 09:32:56.562312 gnews-0.3.7/gnews/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 09:32:53.000000 gnews-0.3.7/gnews/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24441 2024-05-11 09:32:53.000000 gnews-0.3.7/gnews/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-11 09:32:53.000000 gnews-0.3.7/gnews/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 09:32:56.562312 gnews-0.3.7/gnews.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17333 2024-05-11 09:32:56.000000 gnews-0.3.7/gnews.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-11 09:32:56.000000 gnews-0.3.7/gnews.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 09:32:56.000000 gnews-0.3.7/gnews.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-11 09:32:56.000000 gnews-0.3.7/gnews.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-11 09:32:56.000000 gnews-0.3.7/gnews.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 09:32:56.562312 gnews-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-11 09:32:53.000000 gnews-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 09:32:56.562312 gnews-0.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-11 09:32:53.000000 gnews-0.3.7/tests/test_gnews.py
```

### Comparing `gnews-0.3.6/LICENSE.txt` & `gnews-0.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gnews-0.3.6/PKG-INFO` & `gnews-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 Metadata-Version: 2.1
 Name: gnews
-Version: 0.3.6
+Version: 0.3.7
 Summary: Provide an API to search for articles on Google News and returns a usable JSON response.
 Home-page: https://github.com/ranahaani/GNews/
 Author: Muhammad Abdullah
 Author-email: ranahaani@gmail.com
 Project-URL: Documentation, https://github.com/ranahaani/GNews/blob/master/README.md
 Project-URL: Source, https://github.com/ranahaani/GNews/
 Project-URL: Tracker, https://github.com/ranahaani/GNews/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: feedparser~=6.0.2
-Requires-Dist: bs4~=0.0.1
-Requires-Dist: beautifulsoup4~=4.9.3
-Requires-Dist: pymongo~=3.12.0
+Requires-Dist: beautifulsoup4<5,>=4.9.3
 Requires-Dist: dnspython~=1.16.0
-Requires-Dist: python-dotenv~=0.19.0
-Requires-Dist: requests==2.26.0
+Requires-Dist: requests
 
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
 [![Download][download-sheild]][download-url]
```

#### html2text {}

```diff
@@ -1,24 +1,22 @@
-Metadata-Version: 2.1 Name: gnews Version: 0.3.6 Summary: Provide an API to
+Metadata-Version: 2.1 Name: gnews Version: 0.3.7 Summary: Provide an API to
 search for articles on Google News and returns a usable JSON response. Home-
 page: https://github.com/ranahaani/GNews/ Author: Muhammad Abdullah Author-
 email: ranahaani@gmail.com Project-URL: Documentation, https://github.com/
 ranahaani/GNews/blob/master/README.md Project-URL: Source, https://github.com/
 ranahaani/GNews/ Project-URL: Tracker, https://github.com/ranahaani/GNews/
 issues Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Description-Content-Type: text/
-markdown License-File: LICENSE.txt Requires-Dist: feedparser~=6.0.2 Requires-
-Dist: bs4~=0.0.1 Requires-Dist: beautifulsoup4~=4.9.3 Requires-Dist:
-pymongo~=3.12.0 Requires-Dist: dnspython~=1.16.0 Requires-Dist: python-
-dotenv~=0.19.0 Requires-Dist: requests==2.26.0 [![Contributors][contributors-
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown License-File: LICENSE.txt Requires-
+Dist: feedparser~=6.0.2 Requires-Dist: beautifulsoup4<5,>=4.9.3 Requires-Dist:
+dnspython~=1.16.0 Requires-Dist: requests [![Contributors][contributors-
 shield]][contributors-url] [![Forks][forks-shield]][forks-url] [![Stargazers]
 [stars-shield]][stars-url] [![Issues][issues-shield]][issues-url] [![MIT
 License][license-shield]][license-url] [![Download][download-sheild]][download-
 url] [![LinkedIn][linkedin-shield]][linkedin-url]
                                     _[_G_N_e_w_s_]
                              ******** GGNNeewwss ?ð???° ********
    A Happy and lightweight Python Package that Provides an API to search for
```

### Comparing `gnews-0.3.6/README.md` & `gnews-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `gnews-0.3.6/gnews/gnews.py` & `gnews-0.3.7/gnews/gnews.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,18 @@
 import logging
-import os
-import sys
 import urllib.request
 import datetime
 import inspect
 import warnings
 
 import feedparser
 from bs4 import BeautifulSoup as Soup
-from dotenv import load_dotenv
-
-try:
-    import newspaper  # Optional - required by GNews.get_full_article()
-except ImportError:
-    pass
 
 from gnews.utils.constants import AVAILABLE_COUNTRIES, AVAILABLE_LANGUAGES, TOPICS, BASE_URL, USER_AGENT
-from gnews.utils.utils import connect_database, post_database, process_url
+from gnews.utils.utils import process_url
 
 logging.basicConfig(format='%(asctime)s - %(message)s', level=logging.INFO,
                     datefmt='%m/%d/%Y %I:%M:%S %p')
 logger = logging.getLogger(__name__)
 
 
 class GNews:
@@ -308,26 +300,7 @@
                 feed_data = feedparser.parse(url, agent=USER_AGENT)
 
             return [item for item in
                     map(self._process, feed_data.entries[:self._max_results]) if item]
         except Exception as err:
             logger.error(err.args[0])
             return []
-
-    def store_in_mongodb(self, news):
-        """
-        - MongoDB cluster needs to be created first - https://www.mongodb.com/cloud/atlas/register
-        - Connect to the MongoDB cluster
-        - Create a new collection
-        - Insert the news into the collection
-         :param news: the news object that we created in the previous function
-        """
-
-        load_dotenv()
-
-        db_user = os.getenv("DB_USER")
-        db_pw = os.getenv("DB_PW")
-        db_name = os.getenv("DB_NAME")
-        collection_name = os.getenv("COLLECTION_NAME")
-
-        collection = connect_database(db_user, db_pw, db_name, collection_name)
-        post_database(collection, news)
```

### Comparing `gnews-0.3.6/gnews/utils/constants.py` & `gnews-0.3.7/gnews/utils/constants.py`

 * *Files identical despite different names*

### Comparing `gnews-0.3.6/gnews.egg-info/PKG-INFO` & `gnews-0.3.7/gnews.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 Metadata-Version: 2.1
 Name: gnews
-Version: 0.3.6
+Version: 0.3.7
 Summary: Provide an API to search for articles on Google News and returns a usable JSON response.
 Home-page: https://github.com/ranahaani/GNews/
 Author: Muhammad Abdullah
 Author-email: ranahaani@gmail.com
 Project-URL: Documentation, https://github.com/ranahaani/GNews/blob/master/README.md
 Project-URL: Source, https://github.com/ranahaani/GNews/
 Project-URL: Tracker, https://github.com/ranahaani/GNews/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: feedparser~=6.0.2
-Requires-Dist: bs4~=0.0.1
-Requires-Dist: beautifulsoup4~=4.9.3
-Requires-Dist: pymongo~=3.12.0
+Requires-Dist: beautifulsoup4<5,>=4.9.3
 Requires-Dist: dnspython~=1.16.0
-Requires-Dist: python-dotenv~=0.19.0
-Requires-Dist: requests==2.26.0
+Requires-Dist: requests
 
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
 [![Download][download-sheild]][download-url]
```

#### html2text {}

```diff
@@ -1,24 +1,22 @@
-Metadata-Version: 2.1 Name: gnews Version: 0.3.6 Summary: Provide an API to
+Metadata-Version: 2.1 Name: gnews Version: 0.3.7 Summary: Provide an API to
 search for articles on Google News and returns a usable JSON response. Home-
 page: https://github.com/ranahaani/GNews/ Author: Muhammad Abdullah Author-
 email: ranahaani@gmail.com Project-URL: Documentation, https://github.com/
 ranahaani/GNews/blob/master/README.md Project-URL: Source, https://github.com/
 ranahaani/GNews/ Project-URL: Tracker, https://github.com/ranahaani/GNews/
 issues Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Description-Content-Type: text/
-markdown License-File: LICENSE.txt Requires-Dist: feedparser~=6.0.2 Requires-
-Dist: bs4~=0.0.1 Requires-Dist: beautifulsoup4~=4.9.3 Requires-Dist:
-pymongo~=3.12.0 Requires-Dist: dnspython~=1.16.0 Requires-Dist: python-
-dotenv~=0.19.0 Requires-Dist: requests==2.26.0 [![Contributors][contributors-
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown License-File: LICENSE.txt Requires-
+Dist: feedparser~=6.0.2 Requires-Dist: beautifulsoup4<5,>=4.9.3 Requires-Dist:
+dnspython~=1.16.0 Requires-Dist: requests [![Contributors][contributors-
 shield]][contributors-url] [![Forks][forks-shield]][forks-url] [![Stargazers]
 [stars-shield]][stars-url] [![Issues][issues-shield]][issues-url] [![MIT
 License][license-shield]][license-url] [![Download][download-sheild]][download-
 url] [![LinkedIn][linkedin-shield]][linkedin-url]
                                     _[_G_N_e_w_s_]
                              ******** GGNNeewwss ?ð???° ********
    A Happy and lightweight Python Package that Provides an API to search for
```

### Comparing `gnews-0.3.6/setup.py` & `gnews-0.3.7/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,16 +4,16 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='gnews',
-    version='0.3.6',
-    # setup_requires=['setuptools_scm'],  
+    version='0.3.7',
+    # setup_requires=['setuptools_scm'],
     # use_scm_version={
     #     "local_scheme": "no-local-version"
     # },
 
     author="Muhammad Abdullah",
     author_email="ranahaani@gmail.com",
     description='Provide an API to search for articles on Google News and returns a usable JSON response.',
@@ -27,15 +27,14 @@
         'Source': 'https://github.com/ranahaani/GNews/',
         'Tracker': 'https://github.com/ranahaani/GNews/issues',
     },
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
```

### Comparing `gnews-0.3.6/tests/test_gnews.py` & `gnews-0.3.7/tests/test_gnews.py`

 * *Files identical despite different names*

