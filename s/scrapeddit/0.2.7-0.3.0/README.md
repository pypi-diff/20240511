# Comparing `tmp/scrapeddit-0.2.7.tar.gz` & `tmp/scrapeddit-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapeddit-0.2.7.tar", last modified: Sat May 11 13:00:06 2024, max compression
+gzip compressed data, was "scrapeddit-0.3.0.tar", last modified: Sat May 11 13:12:28 2024, max compression
```

## Comparing `scrapeddit-0.2.7.tar` & `scrapeddit-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 13:00:06.402418 scrapeddit-0.2.7/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1063 2024-05-11 09:03:02.000000 scrapeddit-0.2.7/LICENSE.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 13:00:06.402088 scrapeddit-0.2.7/PKG-INFO
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2735 2024-05-11 09:30:19.000000 scrapeddit-0.2.7/README.md
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 13:00:06.400159 scrapeddit-0.2.7/scrapeddit/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:24:22.000000 scrapeddit-0.2.7/scrapeddit/__init__.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      827 2024-05-11 12:48:27.000000 scrapeddit-0.2.7/scrapeddit/authentication.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3550 2024-05-11 12:56:00.000000 scrapeddit-0.2.7/scrapeddit/redditdl.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1550 2024-05-11 12:41:22.000000 scrapeddit-0.2.7/scrapeddit/scrapeonce.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2989 2024-05-11 12:53:35.000000 scrapeddit-0.2.7/scrapeddit/showit.py
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      599 2024-05-11 12:59:46.000000 scrapeddit-0.2.7/scrapeddit/transforms.py
-drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 13:00:06.401739 scrapeddit-0.2.7/scrapeddit.egg-info/
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3037 2024-05-11 13:00:06.000000 scrapeddit-0.2.7/scrapeddit.egg-info/PKG-INFO
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      345 2024-05-11 13:00:06.000000 scrapeddit-0.2.7/scrapeddit.egg-info/SOURCES.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 13:00:06.000000 scrapeddit-0.2.7/scrapeddit.egg-info/dependency_links.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       15 2024-05-11 13:00:06.000000 scrapeddit-0.2.7/scrapeddit.egg-info/requires.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       11 2024-05-11 13:00:06.000000 scrapeddit-0.2.7/scrapeddit.egg-info/top_level.txt
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)       38 2024-05-11 13:00:06.402499 scrapeddit-0.2.7/setup.cfg
--rw-r--r--   0 mohamedmafaz   (501) staff       (20)      662 2024-05-11 13:00:00.000000 scrapeddit-0.2.7/setup.py
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 13:12:28.995592 scrapeddit-0.3.0/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1063 2024-05-11 09:03:02.000000 scrapeddit-0.3.0/LICENSE.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3035 2024-05-11 13:12:28.995278 scrapeddit-0.3.0/PKG-INFO
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     2735 2024-05-11 09:30:19.000000 scrapeddit-0.3.0/README.md
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 13:12:28.993541 scrapeddit-0.3.0/scrapeddit/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 10:24:22.000000 scrapeddit-0.3.0/scrapeddit/__init__.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      827 2024-05-11 12:48:27.000000 scrapeddit-0.3.0/scrapeddit/authentication.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3549 2024-05-11 13:08:02.000000 scrapeddit-0.3.0/scrapeddit/redditdl.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     1550 2024-05-11 12:41:22.000000 scrapeddit-0.3.0/scrapeddit/scrapeonce.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3014 2024-05-11 13:11:08.000000 scrapeddit-0.3.0/scrapeddit/showit.py
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      599 2024-05-11 12:59:46.000000 scrapeddit-0.3.0/scrapeddit/transforms.py
+drwxr-xr-x   0 mohamedmafaz   (501) staff       (20)        0 2024-05-11 13:12:28.994943 scrapeddit-0.3.0/scrapeddit.egg-info/
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)     3035 2024-05-11 13:12:28.000000 scrapeddit-0.3.0/scrapeddit.egg-info/PKG-INFO
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      345 2024-05-11 13:12:28.000000 scrapeddit-0.3.0/scrapeddit.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)        1 2024-05-11 13:12:28.000000 scrapeddit-0.3.0/scrapeddit.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       15 2024-05-11 13:12:28.000000 scrapeddit-0.3.0/scrapeddit.egg-info/requires.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       11 2024-05-11 13:12:28.000000 scrapeddit-0.3.0/scrapeddit.egg-info/top_level.txt
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)       38 2024-05-11 13:12:28.995669 scrapeddit-0.3.0/setup.cfg
+-rw-r--r--   0 mohamedmafaz   (501) staff       (20)      660 2024-05-11 13:12:26.000000 scrapeddit-0.3.0/setup.py
```

### Comparing `scrapeddit-0.2.7/LICENSE.txt` & `scrapeddit-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.2.7/PKG-INFO` & `scrapeddit-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: scrapeddit
-Version: 0.2.7
+Version: 0.3.0
 Summary: Simple test package
-Home-page: https://github.com/Mafaz03/ReditScraper
+Home-page: https://github.com/Mafaz03/scrapeddit
 Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: praw
 Requires-Dist: torchinfo
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: scrapeddit Version: 0.2.7 Summary: Simple test
-package Home-page: https://github.com/Mafaz03/ReditScraper Author: Mafaz03
+Metadata-Version: 2.1 Name: scrapeddit Version: 0.3.0 Summary: Simple test
+package Home-page: https://github.com/Mafaz03/scrapeddit Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE.txt Requires-Dist: praw Requires-Dist: torchinfo
 ************ SSccrraappeeddddiitt ************
 ********** OOvveerrvviieeww **********
 Scrapeddit is a Python class designed for scraping images from Reddit
 subreddits and creating PyTorch datasets. It facilitates the collection of
 image data from various subreddits, allowing for easy integration into machine
```

### Comparing `scrapeddit-0.2.7/README.md` & `scrapeddit-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.2.7/scrapeddit/authentication.py` & `scrapeddit-0.3.0/scrapeddit/authentication.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.2.7/scrapeddit/redditdl.py` & `scrapeddit-0.3.0/scrapeddit/redditdl.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
           self.colated_ds.append([pil_image, r])
         except: pass
 
     z = [i[1] for i in self.colated_ds]
     self.ds_count = dict(Counter(z))
 
   def __call__(self):
-    print(f"Out of {len(self.subreddit) * self.limit}, f{len(self.colated_ds)} were able to scrape")
+    print(f"Out of {len(self.subreddit) * self.limit}, {len(self.colated_ds)} were able to scrape")
     plt.bar(self.ds_count.keys(), self.ds_count.values())
     plt.title('Distribution of Data Sources')
     plt.xlabel('Data Sources')
     plt.ylabel('Count')
     plt.xticks(rotation=45, ha='right')
     plt.grid(axis='y', linestyle='--', alpha=0.7)
     plt.tight_layout()
```

### Comparing `scrapeddit-0.2.7/scrapeddit/scrapeonce.py` & `scrapeddit-0.3.0/scrapeddit/scrapeonce.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.2.7/scrapeddit/showit.py` & `scrapeddit-0.3.0/scrapeddit/showit.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,39 +54,39 @@
       image = Image.open(BytesIO(response.content))
       image.thumbnail((max_size, max_size), Image.LANCZOS)
       if image.mode != 'RGB': image = image.convert('RGB')
       img_tensor = transform(image)
       if img_tensor.shape[0] == 3: img_tensor = img_tensor.permute(1, 2, 0)
       np_image = np.array(img_tensor)
       if sub_title:
-        word = sub_title[i] if len(sub_title[i]) <= 45 else sub_title[i][:30]
+        word = sub_title[i] if len(sub_title[i]) <= 45 else sub_title[i][:30] + '...'
         axes[i].set_title(word, fontsize = fontsize)
       axes[i].imshow(np_image, **kwargs)
     except: pass
     if noframe: axes[i].axis('off')
   for j in range(i + 1, num_rows * max_col):
       axes[j].axis('off')
   if title: plt.suptitle(title)
   print(f"{failed} post did not have images, or failed to fetch")
   plt.tight_layout()
   plt.show()
 
 
-def show_batch(sample_batch, max = 25, X = 'image', y = 'y', cmap=None, **kwargs):
+def show_batch(sample_batch, max = 25, X = 'image', y = 'y', cmap=None, figsize = (5,5), **kwargs):
   if max:
     images = sample_batch[X][:max]
     labels = sample_batch[y][:max]
   else:
     images = sample_batch[X]
     labels = sample_batch[y]
 
   img_len = images.shape[0]
   row = int(math.sqrt(img_len))
   img_len = row ** 2
 
-  fig, axes = plt.subplots(row, row, figsize=(25,25))
+  fig, axes = plt.subplots(row, row, figsize=figsize)
   axes = axes.flatten()
 
   for i in range(img_len):
     axes[i].imshow(images[i], **kwargs)
     axes[i].set_title(labels[i])
     axes[i].axis('off')
```

### Comparing `scrapeddit-0.2.7/scrapeddit/transforms.py` & `scrapeddit-0.3.0/scrapeddit/transforms.py`

 * *Files identical despite different names*

### Comparing `scrapeddit-0.2.7/scrapeddit.egg-info/PKG-INFO` & `scrapeddit-0.3.0/scrapeddit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: scrapeddit
-Version: 0.2.7
+Version: 0.3.0
 Summary: Simple test package
-Home-page: https://github.com/Mafaz03/ReditScraper
+Home-page: https://github.com/Mafaz03/scrapeddit
 Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: praw
 Requires-Dist: torchinfo
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: scrapeddit Version: 0.2.7 Summary: Simple test
-package Home-page: https://github.com/Mafaz03/ReditScraper Author: Mafaz03
+Metadata-Version: 2.1 Name: scrapeddit Version: 0.3.0 Summary: Simple test
+package Home-page: https://github.com/Mafaz03/scrapeddit Author: Mafaz03
 Author-email: mohdmafaz200303@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE.txt Requires-Dist: praw Requires-Dist: torchinfo
 ************ SSccrraappeeddddiitt ************
 ********** OOvveerrvviieeww **********
 Scrapeddit is a Python class designed for scraping images from Reddit
 subreddits and creating PyTorch datasets. It facilitates the collection of
 image data from various subreddits, allowing for easy integration into machine
```

### Comparing `scrapeddit-0.2.7/setup.py` & `scrapeddit-0.3.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 working_directory = path.abspath(path.dirname(__file__))
 
 with open(path.join(working_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='scrapeddit', # name of packe which will be package dir below project
-    version='0.2.7',
-    url='https://github.com/Mafaz03/ReditScraper',
+    version='0.3.0',
+    url='https://github.com/Mafaz03/scrapeddit',
     author='Mafaz03',
     author_email='mohdmafaz200303@gmail.com',
     description='Simple test package',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=['praw', 'torchinfo'],
```

