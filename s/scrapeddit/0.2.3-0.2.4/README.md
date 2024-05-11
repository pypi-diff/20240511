# Comparing `tmp/scrapeddit-0.2.3.tar.gz` & `tmp/scrapeddit-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapeddit-0.2.3.tar", last modified: Sat May 11 12:41:34 2024, max compression
+gzip compressed data, was "scrapeddit-0.2.4.tar", last modified: Sat May 11 12:47:40 2024, max compression
```

## Comparing `scrapeddit-0.2.3.tar` & `scrapeddit-0.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 12:41:34.953348 scrapeddit-0.2.3/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1063 2024-05-11 09:03:02.000000 scrapeddit-0.2.3/LICENSE.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 12:41:34.953038 scrapeddit-0.2.3/PKG-INFO
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2735 2024-05-11 09:30:19.000000 scrapeddit-0.2.3/README.md
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 12:41:34.951187 scrapeddit-0.2.3/scrapeddit/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:24:22.000000 scrapeddit-0.2.3/scrapeddit/__init__.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      835 2024-05-11 12:34:40.000000 scrapeddit-0.2.3/scrapeddit/authentication.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3526 2024-05-11 12:10:46.000000 scrapeddit-0.2.3/scrapeddit/redditdl.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1550 2024-05-11 12:41:22.000000 scrapeddit-0.2.3/scrapeddit/scrapeonce.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2396 2024-05-11 08:43:10.000000 scrapeddit-0.2.3/scrapeddit/showit.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      576 2024-05-11 08:43:10.000000 scrapeddit-0.2.3/scrapeddit/transforms.py
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 12:41:34.952569 scrapeddit-0.2.3/scrapeddit.egg-info/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 12:41:34.000000 scrapeddit-0.2.3/scrapeddit.egg-info/PKG-INFO
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      345 2024-05-11 12:41:34.000000 scrapeddit-0.2.3/scrapeddit.egg-info/SOURCES.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 12:41:34.000000 scrapeddit-0.2.3/scrapeddit.egg-info/dependency_links.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       15 2024-05-11 12:41:34.000000 scrapeddit-0.2.3/scrapeddit.egg-info/requires.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       11 2024-05-11 12:41:34.000000 scrapeddit-0.2.3/scrapeddit.egg-info/top_level.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       38 2024-05-11 12:41:34.953418 scrapeddit-0.2.3/setup.cfg
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      662 2024-05-11 12:41:33.000000 scrapeddit-0.2.3/setup.py
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 12:47:40.417836 scrapeddit-0.2.4/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1063 2024-05-11 09:03:02.000000 scrapeddit-0.2.4/LICENSE.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 12:47:40.417479 scrapeddit-0.2.4/PKG-INFO
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2735 2024-05-11 09:30:19.000000 scrapeddit-0.2.4/README.md
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 12:47:40.415748 scrapeddit-0.2.4/scrapeddit/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:24:22.000000 scrapeddit-0.2.4/scrapeddit/__init__.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      838 2024-05-11 12:43:33.000000 scrapeddit-0.2.4/scrapeddit/authentication.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3526 2024-05-11 12:10:46.000000 scrapeddit-0.2.4/scrapeddit/redditdl.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1550 2024-05-11 12:41:22.000000 scrapeddit-0.2.4/scrapeddit/scrapeonce.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2974 2024-05-11 12:47:14.000000 scrapeddit-0.2.4/scrapeddit/showit.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      576 2024-05-11 08:43:10.000000 scrapeddit-0.2.4/scrapeddit/transforms.py
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 12:47:40.417105 scrapeddit-0.2.4/scrapeddit.egg-info/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 12:47:40.000000 scrapeddit-0.2.4/scrapeddit.egg-info/PKG-INFO
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      345 2024-05-11 12:47:40.000000 scrapeddit-0.2.4/scrapeddit.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 12:47:40.000000 scrapeddit-0.2.4/scrapeddit.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       15 2024-05-11 12:47:40.000000 scrapeddit-0.2.4/scrapeddit.egg-info/requires.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       11 2024-05-11 12:47:40.000000 scrapeddit-0.2.4/scrapeddit.egg-info/top_level.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       38 2024-05-11 12:47:40.417911 scrapeddit-0.2.4/setup.cfg
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      662 2024-05-11 12:43:39.000000 scrapeddit-0.2.4/setup.py
```

### Comparing `scrapeddit-0.2.3/LICENSE.txt` & `scrapeddit-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.2.3/PKG-INFO` & `scrapeddit-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapeddit
-Version: 0.2.3
+Version: 0.2.4
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
-Metadata-Version: 2.1 Name: scrapeddit Version: 0.2.3 Summary: Simple test
+Metadata-Version: 2.1 Name: scrapeddit Version: 0.2.4 Summary: Simple test
 package Home-page: https://github.com/Mafaz03/ReditScraper Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE.txt Requires-Dist: praw Requires-Dist: torchinfo
 ************ SSccrraappeeddddiitt ************
 ********** OOvveerrvviieeww **********
 Scrapeddit is a Python class designed for scraping images from Reddit
 subreddits and creating PyTorch datasets. It facilitates the collection of
```

### Comparing `scrapeddit-0.2.3/README.md` & `scrapeddit-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.2.3/scrapeddit/authentication.py` & `scrapeddit-0.2.4/scrapeddit/authentication.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,9 +17,10 @@
             password = password,
             redirect_uri = redirect_uri,
             user_agent = user_agent,
             check_for_async=check_for_async)
   sub = reddit.subreddit('aww')
   try: sub_type = sub.subreddit_type
   except: raise InvalidSubreddit("Invalid Authentication, please recheck and try again")
+  auths.append(reddit)
   print(f"Authentication was successful, auth stack: {len(auths)}")
-  auths.append(reddit)
+
```

### Comparing `scrapeddit-0.2.3/scrapeddit/redditdl.py` & `scrapeddit-0.2.4/scrapeddit/redditdl.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.2.3/scrapeddit/scrapeonce.py` & `scrapeddit-0.2.4/scrapeddit/scrapeonce.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.2.3/scrapeddit/showit.py` & `scrapeddit-0.2.4/scrapeddit/showit.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+from datetime import datetime
+import pandas as pd
+import matplotlib.pyplot as plt
+import seaborn as sb
+import praw
+import pandas as pd
+from tqdm import tqdm
+import requests
+from PIL import Image
+from torchvision import transforms
+from io import BytesIO
+import numpy as np
+import seaborn as sns
+from collections import Counter
+
+import torch
+from torch.utils.data import Dataset, DataLoader
+import requests
+from PIL import Image
+from io import BytesIO
+import numpy as np
+from tqdm import tqdm
+import torchvision.transforms as transforms
+from torchinfo import summary
+import math
+
 def show_images(links_, title = None, figsize=(15,15), sub_title=None, noframe=True, max_col = 6, max_size=500, max_images = None, fontsize = 10, **kwargs):
   transform = transforms.ToTensor()
   if isinstance(links_, str): links = [links_]
   if max_images: num_images = min(len(links_), max_images)
   else: num_images = len(links_)
   num_rows = (num_images - 1) // max_col + 1
   fig, axes = plt.subplots(num_rows, max_col, figsize=figsize)
```

### Comparing `scrapeddit-0.2.3/scrapeddit/transforms.py` & `scrapeddit-0.2.4/scrapeddit/transforms.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.2.3/scrapeddit.egg-info/PKG-INFO` & `scrapeddit-0.2.4/scrapeddit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapeddit
-Version: 0.2.3
+Version: 0.2.4
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
-Metadata-Version: 2.1 Name: scrapeddit Version: 0.2.3 Summary: Simple test
+Metadata-Version: 2.1 Name: scrapeddit Version: 0.2.4 Summary: Simple test
 package Home-page: https://github.com/Mafaz03/ReditScraper Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE.txt Requires-Dist: praw Requires-Dist: torchinfo
 ************ SSccrraappeeddddiitt ************
 ********** OOvveerrvviieeww **********
 Scrapeddit is a Python class designed for scraping images from Reddit
 subreddits and creating PyTorch datasets. It facilitates the collection of
```

### Comparing `scrapeddit-0.2.3/setup.py` & `scrapeddit-0.2.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 working_directory = path.abspath(path.dirname(__file__))
 
 with open(path.join(working_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='scrapeddit', # name of packe which will be package dir below project
-    version='0.2.3',
+    version='0.2.4',
     url='https://github.com/Mafaz03/ReditScraper',
     author='Mafaz03',
     author_email='mohdmafaz200303@gmail.com',
     description='Simple test package',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

