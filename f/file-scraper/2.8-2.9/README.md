# Comparing `tmp/file-scraper-2.8.tar.gz` & `tmp/file_scraper-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file-scraper-2.8.tar", last modified: Fri Mar  8 14:30:45 2024, max compression
+gzip compressed data, was "file_scraper-2.9.tar", last modified: Sat May 11 10:40:28 2024, max compression
```

## Comparing `file-scraper-2.8.tar` & `file_scraper-2.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 14:30:45.214049 file-scraper-2.8/
--rwxrwx---   0 root         (0) root         (0)     1090 2024-03-07 13:49:18.000000 file-scraper-2.8/LICENSE
--rwxrwx---   0 root         (0) root         (0)       96 2024-03-07 13:49:19.000000 file-scraper-2.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6376 2024-03-08 14:30:45.210051 file-scraper-2.8/PKG-INFO
--rwxrwx---   0 root         (0) root         (0)     5687 2024-03-08 14:28:30.000000 file-scraper-2.8/README.md
--rwxrwx---   0 root         (0) root         (0)      883 2024-03-08 14:28:39.000000 file-scraper-2.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-08 14:30:45.214049 file-scraper-2.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 14:30:45.210051 file-scraper-2.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 14:30:45.210051 file-scraper-2.8/src/file_scraper/
--rwxrwx---   0 root         (0) root         (0)   138800 2024-03-07 13:36:00.000000 file-scraper-2.8/src/file_scraper/FiraCode-Medium.otf
--rwxrwx---   0 root         (0) root         (0)        0 2024-03-07 13:36:00.000000 file-scraper-2.8/src/file_scraper/__init__.py
--rwxrwx---   0 root         (0) root         (0)     1489 2024-03-07 13:36:00.000000 file-scraper-2.8/src/file_scraper/default.json
--rwxrwx---   0 root         (0) root         (0)    28284 2024-03-08 14:28:53.000000 file-scraper-2.8/src/file_scraper/file_scraper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 14:30:45.210051 file-scraper-2.8/src/file_scraper.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6376 2024-03-08 14:30:45.000000 file-scraper-2.8/src/file_scraper.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      415 2024-03-08 14:30:45.000000 file-scraper-2.8/src/file_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 14:30:45.000000 file-scraper-2.8/src/file_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-03-08 14:30:45.000000 file-scraper-2.8/src/file_scraper.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      121 2024-03-08 14:30:45.000000 file-scraper-2.8/src/file_scraper.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-03-08 14:30:45.000000 file-scraper-2.8/src/file_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 10:40:28.886710 file_scraper-2.9/
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-05-11 10:38:39.000000 file_scraper-2.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       93 2024-05-11 10:38:39.000000 file_scraper-2.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6345 2024-05-11 10:40:28.886710 file_scraper-2.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5687 2024-05-11 10:39:10.000000 file_scraper-2.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      864 2024-05-11 10:38:50.000000 file_scraper-2.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-11 10:40:28.886710 file_scraper-2.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 10:40:28.886710 file_scraper-2.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 10:40:28.886710 file_scraper-2.9/src/file_scraper/
+-rw-r--r--   0 root         (0) root         (0)   138800 2024-05-11 10:38:39.000000 file_scraper-2.9/src/file_scraper/FiraCode-Medium.otf
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 10:38:39.000000 file_scraper-2.9/src/file_scraper/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2024-05-11 10:38:39.000000 file_scraper-2.9/src/file_scraper/default.json
+-rw-r--r--   0 root         (0) root         (0)    28284 2024-05-11 10:40:11.000000 file_scraper-2.9/src/file_scraper/file_scraper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 10:40:28.886710 file_scraper-2.9/src/file_scraper.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6345 2024-05-11 10:40:28.000000 file_scraper-2.9/src/file_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      415 2024-05-11 10:40:28.000000 file_scraper-2.9/src/file_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 10:40:28.000000 file_scraper-2.9/src/file_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-05-11 10:40:28.000000 file_scraper-2.9/src/file_scraper.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2024-05-11 10:40:28.000000 file_scraper-2.9/src/file_scraper.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-11 10:40:28.000000 file_scraper-2.9/src/file_scraper.egg-info/top_level.txt
```

### Comparing `file-scraper-2.8/PKG-INFO` & `file_scraper-2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: file-scraper
-Version: 2.8
+Version: 2.9
 Summary: Scrape files for sensitive information, and generate an interactive HTML report.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/file-scraper
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: argparse>=1.4.0
 Requires-Dist: beautifulsoup4>=4.11.1
 Requires-Dist: bs4>=0.0.1
 Requires-Dist: datetime>=5.0
 Requires-Dist: jsbeautifier>=1.14.11
 Requires-Dist: pyOpenSSL>=23.2.0
 Requires-Dist: regex>=2022.4.24
 
@@ -71,15 +70,15 @@
 ```bash
 git clone https://github.com/ivan-sincek/file-scraper && cd file-scraper
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/file_scraper-2.8-py3-none-any.whl
+python3 -m pip install dist/file_scraper-2.9-py3-none-any.whl
 ```
 
 ## Build the Template & Run
 
 Prepare a [template](https://github.com/ivan-sincek/file-scraper/blob/main/src/file_scraper/default.json):
 
 ```json
@@ -160,15 +159,15 @@
 ```fundamental
 car, css, gif, jpeg, jpg, mp3, mp4, nib, ogg, otf, png, storyboard, strings, svg, ttf, webp, woff, woff2, xib
 ```
 
 ## Usage
 
 ```fundamental
-File Scraper v2.8 ( github.com/ivan-sincek/file-scraper )
+File Scraper v2.9 ( github.com/ivan-sincek/file-scraper )
 
 Usage:   file-scraper -dir directory -o out          [-t template     ] [-e excludes    ] [-th threads]
 Example: file-scraper -dir decoded   -o results.html [-t template.json] [-e jpeg,jpg,png] [-th 10     ]
 
 DESCRIPTION
     Scrape files for sensitive information
 DIRECTORY
```

### Comparing `file-scraper-2.8/README.md` & `file_scraper-2.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 ```bash
 git clone https://github.com/ivan-sincek/file-scraper && cd file-scraper
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/file_scraper-2.8-py3-none-any.whl
+python3 -m pip install dist/file_scraper-2.9-py3-none-any.whl
 ```
 
 ## Build the Template & Run
 
 Prepare a [template](https://github.com/ivan-sincek/file-scraper/blob/main/src/file_scraper/default.json):
 
 ```json
@@ -140,15 +140,15 @@
 ```fundamental
 car, css, gif, jpeg, jpg, mp3, mp4, nib, ogg, otf, png, storyboard, strings, svg, ttf, webp, woff, woff2, xib
 ```
 
 ## Usage
 
 ```fundamental
-File Scraper v2.8 ( github.com/ivan-sincek/file-scraper )
+File Scraper v2.9 ( github.com/ivan-sincek/file-scraper )
 
 Usage:   file-scraper -dir directory -o out          [-t template     ] [-e excludes    ] [-th threads]
 Example: file-scraper -dir decoded   -o results.html [-t template.json] [-e jpeg,jpg,png] [-th 10     ]
 
 DESCRIPTION
     Scrape files for sensitive information
 DIRECTORY
```

### Comparing `file-scraper-2.8/pyproject.toml` & `file_scraper-2.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "file-scraper"
-version = "2.8"
+version = "2.9"
 authors = [{ name = "Ivan Sincek" }]
 description = "Scrape files for sensitive information, and generate an interactive HTML report."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
 	"Operating System :: OS Independent"
 ]
-dependencies = ["argparse>=1.4.0", "beautifulsoup4>=4.11.1", "bs4>=0.0.1", "datetime>=5.0", "jsbeautifier>=1.14.11", "pyOpenSSL>=23.2.0", "regex>=2022.4.24"]
+dependencies = ["beautifulsoup4>=4.11.1", "bs4>=0.0.1", "datetime>=5.0", "jsbeautifier>=1.14.11", "pyOpenSSL>=23.2.0", "regex>=2022.4.24"]
 
 [project.urls]
 "Homepage" = "https://github.com/ivan-sincek/file-scraper"
 
 [project.scripts]
 file-scraper = "file_scraper.file_scraper:main"
```

### Comparing `file-scraper-2.8/src/file_scraper/FiraCode-Medium.otf` & `file_scraper-2.9/src/file_scraper/FiraCode-Medium.otf`

 * *Files identical despite different names*

### Comparing `file-scraper-2.8/src/file_scraper/default.json` & `file_scraper-2.9/src/file_scraper/default.json`

 * *Files identical despite different names*

### Comparing `file-scraper-2.8/src/file_scraper/file_scraper.py` & `file_scraper-2.9/src/file_scraper/file_scraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -593,15 +593,15 @@
 			print(msg)
 
 # ----------------------------------------
 
 class MyArgParser(argparse.ArgumentParser):
 
 	def print_help(self):
-		print("File Scraper v2.8 ( github.com/ivan-sincek/file-scraper )")
+		print("File Scraper v2.9 ( github.com/ivan-sincek/file-scraper )")
 		print("")
 		print("Usage:   file-scraper -dir directory -o out          [-t template     ] [-e excludes    ] [-th threads]")
 		print("Example: file-scraper -dir decoded   -o results.html [-t template.json] [-e jpeg,jpg,png] [-th 10     ]")
 		print("")
 		print("DESCRIPTION")
 		print("    Scrape files for sensitive information")
 		print("DIRECTORY")
@@ -779,15 +779,15 @@
 # ----------------------------------------
 
 def main():
 	validate = Validate()
 	if validate.run():
 		print("###########################################################################")
 		print("#                                                                         #")
-		print("#                            File Scraper v2.8                            #")
+		print("#                            File Scraper v2.9                            #")
 		print("#                                    by Ivan Sincek                       #")
 		print("#                                                                         #")
 		print("# Scrape files for sensitive information.                                 #")
 		print("# GitHub repository at github.com/ivan-sincek/file-scraper.               #")
 		print("# Feel free to donate ETH at 0xbc00e800f29524AD8b0968CEBEAD4cD5C5c1f105.  #")
 		print("#                                                                         #")
 		print("###########################################################################")
```

### Comparing `file-scraper-2.8/src/file_scraper.egg-info/PKG-INFO` & `file_scraper-2.9/src/file_scraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: file-scraper
-Version: 2.8
+Version: 2.9
 Summary: Scrape files for sensitive information, and generate an interactive HTML report.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/file-scraper
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: argparse>=1.4.0
 Requires-Dist: beautifulsoup4>=4.11.1
 Requires-Dist: bs4>=0.0.1
 Requires-Dist: datetime>=5.0
 Requires-Dist: jsbeautifier>=1.14.11
 Requires-Dist: pyOpenSSL>=23.2.0
 Requires-Dist: regex>=2022.4.24
 
@@ -71,15 +70,15 @@
 ```bash
 git clone https://github.com/ivan-sincek/file-scraper && cd file-scraper
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/file_scraper-2.8-py3-none-any.whl
+python3 -m pip install dist/file_scraper-2.9-py3-none-any.whl
 ```
 
 ## Build the Template & Run
 
 Prepare a [template](https://github.com/ivan-sincek/file-scraper/blob/main/src/file_scraper/default.json):
 
 ```json
@@ -160,15 +159,15 @@
 ```fundamental
 car, css, gif, jpeg, jpg, mp3, mp4, nib, ogg, otf, png, storyboard, strings, svg, ttf, webp, woff, woff2, xib
 ```
 
 ## Usage
 
 ```fundamental
-File Scraper v2.8 ( github.com/ivan-sincek/file-scraper )
+File Scraper v2.9 ( github.com/ivan-sincek/file-scraper )
 
 Usage:   file-scraper -dir directory -o out          [-t template     ] [-e excludes    ] [-th threads]
 Example: file-scraper -dir decoded   -o results.html [-t template.json] [-e jpeg,jpg,png] [-th 10     ]
 
 DESCRIPTION
     Scrape files for sensitive information
 DIRECTORY
```

