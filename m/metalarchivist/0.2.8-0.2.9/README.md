# Comparing `tmp/metalarchivist-0.2.8.tar.gz` & `tmp/metalarchivist-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metalarchivist-0.2.8.tar", last modified: Wed Apr 10 17:46:34 2024, max compression
+gzip compressed data, was "metalarchivist-0.2.9.tar", last modified: Fri Apr 26 14:15:07 2024, max compression
```

## Comparing `metalarchivist-0.2.8.tar` & `metalarchivist-0.2.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:46:34.268761 metalarchivist-0.2.8/
--rwxrwxrwx   0 root         (0) root         (0)      693 2024-04-10 17:46:21.000000 metalarchivist-0.2.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      702 2024-04-10 17:46:34.268761 metalarchivist-0.2.8/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      113 2024-04-10 17:46:21.000000 metalarchivist-0.2.8/README.md
--rwxrwxrwx   0 root         (0) root         (0)      677 2024-04-10 17:46:21.000000 metalarchivist-0.2.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 17:46:34.268761 metalarchivist-0.2.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:46:34.261761 metalarchivist-0.2.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:46:34.262761 metalarchivist-0.2.8/src/metalarchivist/
--rwxrwxrwx   0 root         (0) root         (0)       81 2024-04-10 17:46:21.000000 metalarchivist-0.2.8/src/metalarchivist/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:46:34.265761 metalarchivist-0.2.8/src/metalarchivist/export/
--rwxrwxrwx   0 root         (0) root         (0)      257 2024-04-10 17:46:21.000000 metalarchivist-0.2.8/src/metalarchivist/export/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4170 2024-04-10 17:46:21.000000 metalarchivist-0.2.8/src/metalarchivist/export/album.py
--rwxrwxrwx   0 root         (0) root         (0)     4193 2024-04-10 17:46:21.000000 metalarchivist-0.2.8/src/metalarchivist/export/band.py
--rw-rw-rw-   0 root         (0) root         (0)     2685 2024-04-10 17:46:21.000000 metalarchivist-0.2.8/src/metalarchivist/export/genre.py
--rw-rw-rw-   0 root         (0) root         (0)     2235 2024-04-10 17:46:21.000000 metalarchivist-0.2.8/src/metalarchivist/export/label.py
--rw-rw-rw-   0 root         (0) root         (0)     1754 2024-04-10 17:46:21.000000 metalarchivist-0.2.8/src/metalarchivist/export/user-agents.json
--rwxrwxrwx   0 root         (0) root         (0)     5625 2024-04-10 17:46:21.000000 metalarchivist-0.2.8/src/metalarchivist/export/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:46:34.266761 metalarchivist-0.2.8/src/metalarchivist/interface/
--rwxrwxrwx   0 root         (0) root         (0)      909 2024-04-10 17:46:21.000000 metalarchivist-0.2.8/src/metalarchivist/interface/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6013 2024-04-10 17:46:21.000000 metalarchivist-0.2.8/src/metalarchivist/interface/album.py
--rwxrwxrwx   0 root         (0) root         (0)     8342 2024-04-10 17:46:21.000000 metalarchivist-0.2.8/src/metalarchivist/interface/band.py
--rw-rw-rw-   0 root         (0) root         (0)     2441 2024-04-10 17:46:21.000000 metalarchivist-0.2.8/src/metalarchivist/interface/base.py
--rw-rw-rw-   0 root         (0) root         (0)     7914 2024-04-10 17:46:21.000000 metalarchivist-0.2.8/src/metalarchivist/interface/genre.py
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-10 17:46:21.000000 metalarchivist-0.2.8/src/metalarchivist/interface/label.py
--rw-rw-rw-   0 root         (0) root         (0)     4648 2024-04-10 17:46:21.000000 metalarchivist-0.2.8/src/metalarchivist/interface/page.py
--rwxrwxrwx   0 root         (0) root         (0)      372 2024-04-10 17:46:21.000000 metalarchivist-0.2.8/src/metalarchivist/interface/search.py
--rw-rw-rw-   0 root         (0) root         (0)     4494 2024-04-10 17:46:21.000000 metalarchivist-0.2.8/src/metalarchivist/interface/theme.py
--rwxrwxrwx   0 root         (0) root         (0)     3337 2024-04-10 17:46:21.000000 metalarchivist-0.2.8/src/metalarchivist/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:46:34.268761 metalarchivist-0.2.8/src/metalarchivist.egg-info/
--rw-r--r--   0 root         (0) root         (0)      702 2024-04-10 17:46:34.000000 metalarchivist-0.2.8/src/metalarchivist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      993 2024-04-10 17:46:34.000000 metalarchivist-0.2.8/src/metalarchivist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 17:46:34.000000 metalarchivist-0.2.8/src/metalarchivist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-04-10 17:46:34.000000 metalarchivist-0.2.8/src/metalarchivist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-04-10 17:46:34.000000 metalarchivist-0.2.8/src/metalarchivist.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:46:34.267761 metalarchivist-0.2.8/src/test/
--rwxrwxrwx   0 root         (0) root         (0)    10014 2024-04-10 17:46:21.000000 metalarchivist-0.2.8/src/test/test_albums.py
--rwxrwxrwx   0 root         (0) root         (0)     5079 2024-04-10 17:46:21.000000 metalarchivist-0.2.8/src/test/test_bands.py
--rwxrwxrwx   0 root         (0) root         (0)     8412 2024-04-10 17:46:21.000000 metalarchivist-0.2.8/src/test/test_genres.py
--rw-rw-rw-   0 root         (0) root         (0)     2735 2024-04-10 17:46:21.000000 metalarchivist-0.2.8/src/test/test_themes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:15:07.668043 metalarchivist-0.2.9/
+-rwxrwxrwx   0 root         (0) root         (0)      693 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      702 2024-04-26 14:15:07.667043 metalarchivist-0.2.9/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      113 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/README.md
+-rwxrwxrwx   0 root         (0) root         (0)      677 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-26 14:15:07.668043 metalarchivist-0.2.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:15:07.659043 metalarchivist-0.2.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:15:07.660043 metalarchivist-0.2.9/src/metalarchivist/
+-rwxrwxrwx   0 root         (0) root         (0)       81 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:15:07.664043 metalarchivist-0.2.9/src/metalarchivist/export/
+-rwxrwxrwx   0 root         (0) root         (0)      257 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/export/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4170 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/export/album.py
+-rwxrwxrwx   0 root         (0) root         (0)     4193 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/export/band.py
+-rw-rw-rw-   0 root         (0) root         (0)     2685 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/export/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)     2235 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/export/label.py
+-rw-rw-rw-   0 root         (0) root         (0)     1754 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/export/user-agents.json
+-rwxrwxrwx   0 root         (0) root         (0)     5625 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/export/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:15:07.666043 metalarchivist-0.2.9/src/metalarchivist/interface/
+-rwxrwxrwx   0 root         (0) root         (0)      909 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/interface/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6013 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/interface/album.py
+-rwxrwxrwx   0 root         (0) root         (0)     8342 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/interface/band.py
+-rw-rw-rw-   0 root         (0) root         (0)     2441 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/interface/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7914 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/interface/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/interface/label.py
+-rw-rw-rw-   0 root         (0) root         (0)     4648 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/interface/page.py
+-rwxrwxrwx   0 root         (0) root         (0)      372 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/interface/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     6386 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/interface/theme.py
+-rwxrwxrwx   0 root         (0) root         (0)     3337 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:15:07.667043 metalarchivist-0.2.9/src/metalarchivist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      702 2024-04-26 14:15:07.000000 metalarchivist-0.2.9/src/metalarchivist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      993 2024-04-26 14:15:07.000000 metalarchivist-0.2.9/src/metalarchivist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 14:15:07.000000 metalarchivist-0.2.9/src/metalarchivist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-26 14:15:07.000000 metalarchivist-0.2.9/src/metalarchivist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-04-26 14:15:07.000000 metalarchivist-0.2.9/src/metalarchivist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:15:07.666043 metalarchivist-0.2.9/src/test/
+-rwxrwxrwx   0 root         (0) root         (0)    10014 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/test/test_albums.py
+-rwxrwxrwx   0 root         (0) root         (0)     5079 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/test/test_bands.py
+-rwxrwxrwx   0 root         (0) root         (0)     8412 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/test/test_genres.py
+-rw-rw-rw-   0 root         (0) root         (0)     3059 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/test/test_themes.py
```

### Comparing `metalarchivist-0.2.8/LICENSE` & `metalarchivist-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.8/PKG-INFO` & `metalarchivist-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.2.8
+Version: 0.2.9
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `metalarchivist-0.2.8/pyproject.toml` & `metalarchivist-0.2.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "metalarchivist"
-version = "0.2.8"
+version = "0.2.9"
 authors = [ { name = "z3c0", email = "z3c0@21337.tech" } ]
 description = "A package for extracting data from metal-archives.com"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [ "rich", "lxml", "urllib3", "pycryptodome" ]
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `metalarchivist-0.2.8/src/metalarchivist/export/album.py` & `metalarchivist-0.2.9/src/metalarchivist/export/album.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.8/src/metalarchivist/export/band.py` & `metalarchivist-0.2.9/src/metalarchivist/export/band.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.8/src/metalarchivist/export/genre.py` & `metalarchivist-0.2.9/src/metalarchivist/export/genre.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.8/src/metalarchivist/export/label.py` & `metalarchivist-0.2.9/src/metalarchivist/export/label.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.8/src/metalarchivist/export/user-agents.json` & `metalarchivist-0.2.9/src/metalarchivist/export/user-agents.json`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.8/src/metalarchivist/export/util.py` & `metalarchivist-0.2.9/src/metalarchivist/export/util.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.8/src/metalarchivist/interface/__init__.py` & `metalarchivist-0.2.9/src/metalarchivist/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.8/src/metalarchivist/interface/album.py` & `metalarchivist-0.2.9/src/metalarchivist/interface/album.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.8/src/metalarchivist/interface/band.py` & `metalarchivist-0.2.9/src/metalarchivist/interface/band.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.8/src/metalarchivist/interface/base.py` & `metalarchivist-0.2.9/src/metalarchivist/interface/base.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.8/src/metalarchivist/interface/genre.py` & `metalarchivist-0.2.9/src/metalarchivist/interface/genre.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.8/src/metalarchivist/interface/label.py` & `metalarchivist-0.2.9/src/metalarchivist/interface/label.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.8/src/metalarchivist/interface/page.py` & `metalarchivist-0.2.9/src/metalarchivist/interface/page.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.8/src/metalarchivist/report.py` & `metalarchivist-0.2.9/src/metalarchivist/report.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.8/src/metalarchivist.egg-info/PKG-INFO` & `metalarchivist-0.2.9/src/metalarchivist.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.2.8
+Version: 0.2.9
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `metalarchivist-0.2.8/src/metalarchivist.egg-info/SOURCES.txt` & `metalarchivist-0.2.9/src/metalarchivist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.8/src/test/test_albums.py` & `metalarchivist-0.2.9/src/test/test_albums.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.8/src/test/test_bands.py` & `metalarchivist-0.2.9/src/test/test_bands.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.8/src/test/test_genres.py` & `metalarchivist-0.2.9/src/test/test_genres.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.8/src/test/test_themes.py` & `metalarchivist-0.2.9/src/test/test_themes.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,29 +49,35 @@
 class TestThemes(unittest.TestCase):
     
     metalarchivist, interface, export, config = load_module()
 
     def test_themes(self):
         themes = self.interface.Themes('National Socialism, Aryanism, Antisemitism, Anti-communism, W.A.R.')
         self.assertIsNotNone(themes)
-        self.assertEqual(len(themes.phases), 5)
         self.assertEqual(themes.clean_theme, 'Anti-communism, Antisemitism, Aryanism, Nazism, White Aryan Resistance')
+        self.assertEqual(len(themes.phases), 5)
 
         themes = self.interface.Themes('Satanism, War, Hate, National Socialism, Anti-Judeo-Christianity, Racism')
         self.assertIsNotNone(themes)
-        self.assertEqual(len(themes.phases), 6)
         self.assertEqual(themes.clean_theme, 'Anti-Judeo-Christianity, Hate, Nazism, Racism, Satanism, War')
+        self.assertEqual(len(themes.phases), 6)
         
         themes = self.interface.Themes('National Socialism, War, Winter')
         self.assertIsNotNone(themes)
-        self.assertEqual(len(themes.phases), 3)
         self.assertEqual(themes.clean_theme, 'Nazism, War, Winter')
+        self.assertEqual(len(themes.phases), 3)
 
         themes = self.interface.Themes('National Socialism, Nazism')
         self.assertIsNotNone(themes)
-        self.assertEqual(len(themes.phases), 1)
         self.assertEqual(themes.clean_theme, 'Nazism')
+        self.assertEqual(len(themes.phases), 1)
 
         themes = self.interface.Themes('Satanism, Anti-Christianity, Death, Genocide, Hatred, National Socialism')
         self.assertIsNotNone(themes)
-        self.assertEqual(len(themes.phases), 6)
         self.assertEqual(themes.clean_theme, 'Anti-Christianity, Death, Genocide, Hatred, Nazism, Satanism')
+        self.assertEqual(len(themes.phases), 6)
+     
+        themes = self.interface.Themes('Anime (Lolicon, Hentai), Suicide, Racism')
+        self.assertIsNotNone(themes)
+        self.assertEqual(themes.clean_theme, 'Anime (Lolicon, Hentai), Racism, Suicide')
+        self.assertEqual(len(themes.phases), 3)
+        self.assertEqual(len(themes.phases[0].subthemes), 2)
```

