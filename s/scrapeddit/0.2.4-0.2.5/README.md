# Comparing `tmp/scrapeddit-0.2.4.tar.gz` & `tmp/scrapeddit-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapeddit-0.2.4.tar", last modified: Sat May 11 12:47:40 2024, max compression
+gzip compressed data, was "scrapeddit-0.2.5.tar", last modified: Sat May 11 12:54:01 2024, max compression
```

## Comparing `scrapeddit-0.2.4.tar` & `scrapeddit-0.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 12:47:40.417836 scrapeddit-0.2.4/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1063 2024-05-11 09:03:02.000000 scrapeddit-0.2.4/LICENSE.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 12:47:40.417479 scrapeddit-0.2.4/PKG-INFO
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2735 2024-05-11 09:30:19.000000 scrapeddit-0.2.4/README.md
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 12:47:40.415748 scrapeddit-0.2.4/scrapeddit/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:24:22.000000 scrapeddit-0.2.4/scrapeddit/__init__.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      838 2024-05-11 12:43:33.000000 scrapeddit-0.2.4/scrapeddit/authentication.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3526 2024-05-11 12:10:46.000000 scrapeddit-0.2.4/scrapeddit/redditdl.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1550 2024-05-11 12:41:22.000000 scrapeddit-0.2.4/scrapeddit/scrapeonce.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2974 2024-05-11 12:47:14.000000 scrapeddit-0.2.4/scrapeddit/showit.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      576 2024-05-11 08:43:10.000000 scrapeddit-0.2.4/scrapeddit/transforms.py
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 12:47:40.417105 scrapeddit-0.2.4/scrapeddit.egg-info/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 12:47:40.000000 scrapeddit-0.2.4/scrapeddit.egg-info/PKG-INFO
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      345 2024-05-11 12:47:40.000000 scrapeddit-0.2.4/scrapeddit.egg-info/SOURCES.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 12:47:40.000000 scrapeddit-0.2.4/scrapeddit.egg-info/dependency_links.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       15 2024-05-11 12:47:40.000000 scrapeddit-0.2.4/scrapeddit.egg-info/requires.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       11 2024-05-11 12:47:40.000000 scrapeddit-0.2.4/scrapeddit.egg-info/top_level.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       38 2024-05-11 12:47:40.417911 scrapeddit-0.2.4/setup.cfg
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      662 2024-05-11 12:43:39.000000 scrapeddit-0.2.4/setup.py
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 12:54:01.943896 scrapeddit-0.2.5/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1063 2024-05-11 09:03:02.000000 scrapeddit-0.2.5/LICENSE.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 12:54:01.943569 scrapeddit-0.2.5/PKG-INFO
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2735 2024-05-11 09:30:19.000000 scrapeddit-0.2.5/README.md
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 12:54:01.942060 scrapeddit-0.2.5/scrapeddit/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:24:22.000000 scrapeddit-0.2.5/scrapeddit/__init__.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      827 2024-05-11 12:48:27.000000 scrapeddit-0.2.5/scrapeddit/authentication.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3526 2024-05-11 12:10:46.000000 scrapeddit-0.2.5/scrapeddit/redditdl.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1550 2024-05-11 12:41:22.000000 scrapeddit-0.2.5/scrapeddit/scrapeonce.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2989 2024-05-11 12:53:35.000000 scrapeddit-0.2.5/scrapeddit/showit.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      576 2024-05-11 08:43:10.000000 scrapeddit-0.2.5/scrapeddit/transforms.py
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 12:54:01.943252 scrapeddit-0.2.5/scrapeddit.egg-info/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 12:54:01.000000 scrapeddit-0.2.5/scrapeddit.egg-info/PKG-INFO
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      345 2024-05-11 12:54:01.000000 scrapeddit-0.2.5/scrapeddit.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 12:54:01.000000 scrapeddit-0.2.5/scrapeddit.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       15 2024-05-11 12:54:01.000000 scrapeddit-0.2.5/scrapeddit.egg-info/requires.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       11 2024-05-11 12:54:01.000000 scrapeddit-0.2.5/scrapeddit.egg-info/top_level.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       38 2024-05-11 12:54:01.943964 scrapeddit-0.2.5/setup.cfg
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      662 2024-05-11 12:54:00.000000 scrapeddit-0.2.5/setup.py
```

### Comparing `scrapeddit-0.2.4/LICENSE.txt` & `scrapeddit-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.2.4/PKG-INFO` & `scrapeddit-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapeddit
-Version: 0.2.4
+Version: 0.2.5
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
-Metadata-Version: 2.1 Name: scrapeddit Version: 0.2.4 Summary: Simple test
+Metadata-Version: 2.1 Name: scrapeddit Version: 0.2.5 Summary: Simple test
 package Home-page: https://github.com/Mafaz03/ReditScraper Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE.txt Requires-Dist: praw Requires-Dist: torchinfo
 ************ SSccrraappeeddddiitt ************
 ********** OOvveerrvviieeww **********
 Scrapeddit is a Python class designed for scraping images from Reddit
 subreddits and creating PyTorch datasets. It facilitates the collection of
```

### Comparing `scrapeddit-0.2.4/README.md` & `scrapeddit-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.2.4/scrapeddit/authentication.py` & `scrapeddit-0.2.5/scrapeddit/authentication.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 import praw
 
-class InvalidSubreddit(Exception):
-    pass
-class RestrictedSubreddit(Exception):
-    pass
-class AuthFailed(Exception):
-   pass
+class InvalidSubreddit(Exception): pass
+class RestrictedSubreddit(Exception): pass
+class AuthFailed(Exception): pass
 class IncompleteAuth(Exception): pass
    
 auths = []
 
 def auth_reddit(client_id, client_secret, username, password, redirect_uri, user_agent, check_for_async = False):
   reddit = praw.Reddit(client_id = client_id,
             client_secret = client_secret,
```

### Comparing `scrapeddit-0.2.4/scrapeddit/redditdl.py` & `scrapeddit-0.2.5/scrapeddit/redditdl.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.2.4/scrapeddit/scrapeonce.py` & `scrapeddit-0.2.5/scrapeddit/scrapeonce.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.2.4/scrapeddit/showit.py` & `scrapeddit-0.2.5/scrapeddit/showit.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,15 @@
       image = Image.open(BytesIO(response.content))
       image.thumbnail((max_size, max_size), Image.LANCZOS)
       if image.mode != 'RGB': image = image.convert('RGB')
       img_tensor = transform(image)
       if img_tensor.shape[0] == 3: img_tensor = img_tensor.permute(1, 2, 0)
       np_image = np.array(img_tensor)
       if sub_title:
-        word = sub_title[i] if len(sub_title[i]) <= 45 else ""
+        word = sub_title[i] if len(sub_title[i]) <= 45 else sub_title[i][:30]
         axes[i].set_title(word, fontsize = fontsize)
       axes[i].imshow(np_image, **kwargs)
     except: pass
     if noframe: axes[i].axis('off')
   for j in range(i + 1, num_rows * max_col):
       axes[j].axis('off')
   if title: plt.suptitle(title)
```

### Comparing `scrapeddit-0.2.4/scrapeddit/transforms.py` & `scrapeddit-0.2.5/scrapeddit/transforms.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.2.4/scrapeddit.egg-info/PKG-INFO` & `scrapeddit-0.2.5/scrapeddit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapeddit
-Version: 0.2.4
+Version: 0.2.5
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
-Metadata-Version: 2.1 Name: scrapeddit Version: 0.2.4 Summary: Simple test
+Metadata-Version: 2.1 Name: scrapeddit Version: 0.2.5 Summary: Simple test
 package Home-page: https://github.com/Mafaz03/ReditScraper Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE.txt Requires-Dist: praw Requires-Dist: torchinfo
 ************ SSccrraappeeddddiitt ************
 ********** OOvveerrvviieeww **********
 Scrapeddit is a Python class designed for scraping images from Reddit
 subreddits and creating PyTorch datasets. It facilitates the collection of
```

### Comparing `scrapeddit-0.2.4/setup.py` & `scrapeddit-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 working_directory = path.abspath(path.dirname(__file__))
 
 with open(path.join(working_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='scrapeddit', # name of packe which will be package dir below project
-    version='0.2.4',
+    version='0.2.5',
     url='https://github.com/Mafaz03/ReditScraper',
     author='Mafaz03',
     author_email='mohdmafaz200303@gmail.com',
     description='Simple test package',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

