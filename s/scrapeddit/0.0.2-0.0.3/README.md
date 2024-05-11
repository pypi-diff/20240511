# Comparing `tmp/scrapeddit-0.0.2.tar.gz` & `tmp/scrapeddit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapeddit-0.0.2.tar", last modified: Sat May 11 10:05:59 2024, max compression
+gzip compressed data, was "scrapeddit-0.0.3.tar", last modified: Sat May 11 10:21:19 2024, max compression
```

## Comparing `scrapeddit-0.0.2.tar` & `scrapeddit-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 10:05:59.379099 scrapeddit-0.0.2/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1063 2024-05-11 09:03:02.000000 scrapeddit-0.0.2/LICENSE.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 10:05:59.378789 scrapeddit-0.0.2/PKG-INFO
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2735 2024-05-11 09:30:19.000000 scrapeddit-0.0.2/README.md
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 10:05:59.377185 scrapeddit-0.0.2/scrapeddit/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1516 2024-05-11 08:43:10.000000 scrapeddit-0.0.2/scrapeddit/Dataset.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       56 2024-05-11 10:04:07.000000 scrapeddit-0.0.2/scrapeddit/__init__.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2816 2024-05-11 08:43:10.000000 scrapeddit-0.0.2/scrapeddit/redditdl.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1158 2024-05-11 09:32:09.000000 scrapeddit-0.0.2/scrapeddit/scrapedit.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2396 2024-05-11 08:43:10.000000 scrapeddit-0.0.2/scrapeddit/showit.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      576 2024-05-11 08:43:10.000000 scrapeddit-0.0.2/scrapeddit/transforms.py
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 10:05:59.378519 scrapeddit-0.0.2/scrapeddit.egg-info/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 10:05:59.000000 scrapeddit-0.0.2/scrapeddit.egg-info/PKG-INFO
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      337 2024-05-11 10:05:59.000000 scrapeddit-0.0.2/scrapeddit.egg-info/SOURCES.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:05:59.000000 scrapeddit-0.0.2/scrapeddit.egg-info/dependency_links.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       15 2024-05-11 10:05:59.000000 scrapeddit-0.0.2/scrapeddit.egg-info/requires.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       11 2024-05-11 10:05:59.000000 scrapeddit-0.0.2/scrapeddit.egg-info/top_level.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       38 2024-05-11 10:05:59.379153 scrapeddit-0.0.2/setup.cfg
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      662 2024-05-11 10:04:53.000000 scrapeddit-0.0.2/setup.py
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 10:21:19.826354 scrapeddit-0.0.3/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1063 2024-05-11 09:03:02.000000 scrapeddit-0.0.3/LICENSE.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 10:21:19.826020 scrapeddit-0.0.3/PKG-INFO
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2735 2024-05-11 09:30:19.000000 scrapeddit-0.0.3/README.md
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 10:21:19.824416 scrapeddit-0.0.3/scrapeddit/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1516 2024-05-11 08:43:10.000000 scrapeddit-0.0.3/scrapeddit/Dataset.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       56 2024-05-11 10:04:07.000000 scrapeddit-0.0.3/scrapeddit/__init__.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3602 2024-05-11 10:19:06.000000 scrapeddit-0.0.3/scrapeddit/redditdl.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1233 2024-05-11 10:18:03.000000 scrapeddit-0.0.3/scrapeddit/scrapedit.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2396 2024-05-11 08:43:10.000000 scrapeddit-0.0.3/scrapeddit/showit.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      576 2024-05-11 08:43:10.000000 scrapeddit-0.0.3/scrapeddit/transforms.py
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 10:21:19.825648 scrapeddit-0.0.3/scrapeddit.egg-info/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 10:21:19.000000 scrapeddit-0.0.3/scrapeddit.egg-info/PKG-INFO
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      337 2024-05-11 10:21:19.000000 scrapeddit-0.0.3/scrapeddit.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:21:19.000000 scrapeddit-0.0.3/scrapeddit.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       15 2024-05-11 10:21:19.000000 scrapeddit-0.0.3/scrapeddit.egg-info/requires.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       11 2024-05-11 10:21:19.000000 scrapeddit-0.0.3/scrapeddit.egg-info/top_level.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       38 2024-05-11 10:21:19.826437 scrapeddit-0.0.3/setup.cfg
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      662 2024-05-11 10:21:17.000000 scrapeddit-0.0.3/setup.py
```

### Comparing `scrapeddit-0.0.2/LICENSE.txt` & `scrapeddit-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.0.2/PKG-INFO` & `scrapeddit-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapeddit
-Version: 0.0.2
+Version: 0.0.3
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
-Metadata-Version: 2.1 Name: scrapeddit Version: 0.0.2 Summary: Simple test
+Metadata-Version: 2.1 Name: scrapeddit Version: 0.0.3 Summary: Simple test
 package Home-page: https://github.com/Mafaz03/ReditScraper Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE.txt Requires-Dist: praw Requires-Dist: torchinfo
 ************ SSccrraappeeddddiitt ************
 ********** OOvveerrvviieeww **********
 Scrapeddit is a Python class designed for scraping images from Reddit
 subreddits and creating PyTorch datasets. It facilitates the collection of
```

### Comparing `scrapeddit-0.0.2/README.md` & `scrapeddit-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.0.2/scrapeddit/Dataset.py` & `scrapeddit-0.0.3/scrapeddit/Dataset.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.0.2/scrapeddit/redditdl.py` & `scrapeddit-0.0.3/scrapeddit/redditdl.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,41 @@
+
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
+
+reddit = praw.Reddit(client_id = "",
+            client_secret = "",
+            username = '',
+            password = '',
+            redirect_uri = "",
+            user_agent = "",
+            check_for_async=False)
+
 from PIL import UnidentifiedImageError
 
 class InvalidSubreddit(Exception):
     pass
 class RestrictedSubreddit(Exception):
     pass
```

### Comparing `scrapeddit-0.0.2/scrapeddit/scrapedit.py` & `scrapeddit-0.0.3/scrapeddit/scrapedit.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+import tqdm
+import praw
+from datetime import datetime
+import pandas as pd
+
 reddit = praw.Reddit(client_id = "",
             client_secret = "",
             username = '',
             password = '',
             redirect_uri = "",
             user_agent = "",
             check_for_async=False)
```

### Comparing `scrapeddit-0.0.2/scrapeddit/showit.py` & `scrapeddit-0.0.3/scrapeddit/showit.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.0.2/scrapeddit/transforms.py` & `scrapeddit-0.0.3/scrapeddit/transforms.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.0.2/scrapeddit.egg-info/PKG-INFO` & `scrapeddit-0.0.3/scrapeddit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapeddit
-Version: 0.0.2
+Version: 0.0.3
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
-Metadata-Version: 2.1 Name: scrapeddit Version: 0.0.2 Summary: Simple test
+Metadata-Version: 2.1 Name: scrapeddit Version: 0.0.3 Summary: Simple test
 package Home-page: https://github.com/Mafaz03/ReditScraper Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE.txt Requires-Dist: praw Requires-Dist: torchinfo
 ************ SSccrraappeeddddiitt ************
 ********** OOvveerrvviieeww **********
 Scrapeddit is a Python class designed for scraping images from Reddit
 subreddits and creating PyTorch datasets. It facilitates the collection of
```

