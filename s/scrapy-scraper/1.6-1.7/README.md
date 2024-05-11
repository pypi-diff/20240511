# Comparing `tmp/scrapy-scraper-1.6.tar.gz` & `tmp/scrapy_scraper-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy-scraper-1.6.tar", last modified: Sun Mar 31 01:32:41 2024, max compression
+gzip compressed data, was "scrapy_scraper-1.7.tar", last modified: Sat May 11 10:35:13 2024, max compression
```

## Comparing `scrapy-scraper-1.6.tar` & `scrapy_scraper-1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 01:32:41.191949 scrapy-scraper-1.6/
--rw-r--r--   0 root         (0) root         (0)     1069 2024-03-30 23:47:44.000000 scrapy-scraper-1.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       65 2024-03-30 23:47:44.000000 scrapy-scraper-1.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4729 2024-03-31 01:32:41.187950 scrapy-scraper-1.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3981 2024-03-31 00:50:49.000000 scrapy-scraper-1.6/README.md
--rw-r--r--   0 root         (0) root         (0)      904 2024-03-30 23:51:21.000000 scrapy-scraper-1.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-31 01:32:41.191949 scrapy-scraper-1.6/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 01:32:41.187950 scrapy-scraper-1.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 01:32:41.187950 scrapy-scraper-1.6/src/scrapy_scraper/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-30 23:47:44.000000 scrapy-scraper-1.6/src/scrapy_scraper/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23949 2024-03-31 01:13:23.000000 scrapy-scraper-1.6/src/scrapy_scraper/scrapy_scraper.py
--rw-r--r--   0 root         (0) root         (0)    11174 2024-03-31 01:13:42.000000 scrapy-scraper-1.6/src/scrapy_scraper/user_agents.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 01:32:41.187950 scrapy-scraper-1.6/src/scrapy_scraper.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4729 2024-03-31 01:32:41.000000 scrapy-scraper-1.6/src/scrapy_scraper.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      401 2024-03-31 01:32:41.000000 scrapy-scraper-1.6/src/scrapy_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-31 01:32:41.000000 scrapy-scraper-1.6/src/scrapy_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2024-03-31 01:32:41.000000 scrapy-scraper-1.6/src/scrapy_scraper.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      152 2024-03-31 01:32:41.000000 scrapy-scraper-1.6/src/scrapy_scraper.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-03-31 01:32:41.000000 scrapy-scraper-1.6/src/scrapy_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 10:35:13.661183 scrapy_scraper-1.7/
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-05-11 10:33:15.000000 scrapy_scraper-1.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-11 10:33:15.000000 scrapy_scraper-1.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4698 2024-05-11 10:35:13.661183 scrapy_scraper-1.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3981 2024-05-11 10:34:14.000000 scrapy_scraper-1.7/README.md
+-rw-r--r--   0 root         (0) root         (0)      885 2024-05-11 10:33:57.000000 scrapy_scraper-1.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-11 10:35:13.661183 scrapy_scraper-1.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 10:35:13.657181 scrapy_scraper-1.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 10:35:13.661183 scrapy_scraper-1.7/src/scrapy_scraper/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 10:33:15.000000 scrapy_scraper-1.7/src/scrapy_scraper/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23949 2024-05-11 10:34:46.000000 scrapy_scraper-1.7/src/scrapy_scraper/scrapy_scraper.py
+-rw-r--r--   0 root         (0) root         (0)    11174 2024-05-11 09:59:35.000000 scrapy_scraper-1.7/src/scrapy_scraper/user_agents.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 10:35:13.661183 scrapy_scraper-1.7/src/scrapy_scraper.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4698 2024-05-11 10:35:13.000000 scrapy_scraper-1.7/src/scrapy_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      401 2024-05-11 10:35:13.000000 scrapy_scraper-1.7/src/scrapy_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 10:35:13.000000 scrapy_scraper-1.7/src/scrapy_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2024-05-11 10:35:13.000000 scrapy_scraper-1.7/src/scrapy_scraper.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      136 2024-05-11 10:35:13.000000 scrapy_scraper-1.7/src/scrapy_scraper.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-11 10:35:13.000000 scrapy_scraper-1.7/src/scrapy_scraper.egg-info/top_level.txt
```

### Comparing `scrapy-scraper-1.6/LICENSE` & `scrapy_scraper-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapy-scraper-1.6/PKG-INFO` & `scrapy_scraper-1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: scrapy-scraper
-Version: 1.6
+Version: 1.7
 Summary: Web crawler and scraper based on Scrapy and Playwright's headless browser.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/scrapy-scraper
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: argparse>=1.4.0
 Requires-Dist: beautifulsoup4>=4.11.1
 Requires-Dist: bs4>=0.0.1
 Requires-Dist: colorama>=0.4.6
 Requires-Dist: datetime>=5.2
 Requires-Dist: jsbeautifier>=1.14.11
 Requires-Dist: scrapy>=2.11.0
 Requires-Dist: termcolor>=1.1.0
@@ -71,15 +70,15 @@
 ```bash
 git clone https://github.com/ivan-sincek/scrapy-scraper && cd scrapy-scraper
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/scrapy-scraper-1.6-py3-none-any.whl
+python3 -m pip install dist/scrapy-scraper-1.7-py3-none-any.whl
 ```
 
 ## How to Run
 
 Restricted (domain whitelisting is on):
 
 ```fundamental
@@ -91,15 +90,15 @@
 ```fundamental
 scrapy-scraper -u https://example.com/home -o results.txt -a random -s random -dir js -l -w off
 ```
 
 ## Usage
 
 ```fundamental
-Scrapy Scraper v1.6 ( github.com/ivan-sincek/scrapy-scraper )
+Scrapy Scraper v1.7 ( github.com/ivan-sincek/scrapy-scraper )
 
 Usage:   scrapy-scraper -u urls                     -o out         [-dir directory]
 Example: scrapy-scraper -u https://example.com/home -o results.txt [-dir downloads]
 
 DESCRIPTION
     Crawl and scrape websites
 URLS
@@ -135,15 +134,15 @@
 RECURSION
     Recursion depth limit
     Specify '0' for no limit
     Default: 1
     -r, --recursion = 0 | 2 | 4 | etc.
 USER AGENT
     User agent to use
-    Default: Scrapy Scraper/1.6
+    Default: Scrapy Scraper/1.7
     -a, --user-agent = curl/3.30.1 | random | etc.
 PROXY
     Web proxy to use
     -x, --proxy = http://127.0.0.1:8080 | etc.
 DIRECTORY
     Output directory
     All extracted JavaScript files will be saved in this directory
```

### Comparing `scrapy-scraper-1.6/README.md` & `scrapy_scraper-1.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 ```bash
 git clone https://github.com/ivan-sincek/scrapy-scraper && cd scrapy-scraper
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/scrapy-scraper-1.6-py3-none-any.whl
+python3 -m pip install dist/scrapy-scraper-1.7-py3-none-any.whl
 ```
 
 ## How to Run
 
 Restricted (domain whitelisting is on):
 
 ```fundamental
@@ -69,15 +69,15 @@
 ```fundamental
 scrapy-scraper -u https://example.com/home -o results.txt -a random -s random -dir js -l -w off
 ```
 
 ## Usage
 
 ```fundamental
-Scrapy Scraper v1.6 ( github.com/ivan-sincek/scrapy-scraper )
+Scrapy Scraper v1.7 ( github.com/ivan-sincek/scrapy-scraper )
 
 Usage:   scrapy-scraper -u urls                     -o out         [-dir directory]
 Example: scrapy-scraper -u https://example.com/home -o results.txt [-dir downloads]
 
 DESCRIPTION
     Crawl and scrape websites
 URLS
@@ -113,15 +113,15 @@
 RECURSION
     Recursion depth limit
     Specify '0' for no limit
     Default: 1
     -r, --recursion = 0 | 2 | 4 | etc.
 USER AGENT
     User agent to use
-    Default: Scrapy Scraper/1.6
+    Default: Scrapy Scraper/1.7
     -a, --user-agent = curl/3.30.1 | random | etc.
 PROXY
     Web proxy to use
     -x, --proxy = http://127.0.0.1:8080 | etc.
 DIRECTORY
     Output directory
     All extracted JavaScript files will be saved in this directory
```

### Comparing `scrapy-scraper-1.6/pyproject.toml` & `scrapy_scraper-1.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scrapy-scraper"
-version = "1.6"
+version = "1.7"
 authors = [{ name = "Ivan Sincek" }]
 description = "Web crawler and scraper based on Scrapy and Playwright's headless browser."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
 	"Operating System :: OS Independent"
 ]
-dependencies = ["argparse>=1.4.0", "beautifulsoup4>=4.11.1", "bs4>=0.0.1", "colorama>=0.4.6", "datetime>=5.2", "jsbeautifier>=1.14.11", "scrapy>=2.11.0", "termcolor>=1.1.0", "tldextract>=3.6.0"]
+dependencies = ["beautifulsoup4>=4.11.1", "bs4>=0.0.1", "colorama>=0.4.6", "datetime>=5.2", "jsbeautifier>=1.14.11", "scrapy>=2.11.0", "termcolor>=1.1.0", "tldextract>=3.6.0"]
 
 [project.urls]
 "Homepage" = "https://github.com/ivan-sincek/scrapy-scraper"
 
 [project.scripts]
 scrapy-scraper = "scrapy_scraper.scrapy_scraper:main"
```

### Comparing `scrapy-scraper-1.6/src/scrapy_scraper/scrapy_scraper.py` & `scrapy_scraper-1.7/src/scrapy_scraper/scrapy_scraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 			with open(out, "w") as stream:
 				for line in data:
 					stream.write(str(line).strip() + "\n")
 			print(("Results have been saved to '{0}'").format(out))
 		except FileNotFoundError:
 			print(("Cannot save results to '{0}'").format(out))
 
-default_user_agent = "Scrapy Scraper/1.6"
+default_user_agent = "Scrapy Scraper/1.7"
 
 def get_all_user_agents():
 	array = []
 	file = os.path.join(os.path.abspath(os.path.split(__file__)[0]), "user_agents.txt")
 	if os.path.isfile(file) and os.access(file, os.R_OK) and os.stat(file).st_size > 0:
 		with open(file, "r", encoding = default_encoding) as stream:
 			for line in stream:
@@ -319,15 +319,15 @@
 		return request.resource_type in ["fetch", "stylesheet", "image", "ping", "font", "media", "imageset", "beacon", "csp_report", "object", "texttrack", "manifest"]
 
 # ----------------------------------------
 
 class MyArgParser(argparse.ArgumentParser):
 	
 	def print_help(self):
-		print("Scrapy Scraper v1.6 ( github.com/ivan-sincek/scrapy-scraper )")
+		print("Scrapy Scraper v1.7 ( github.com/ivan-sincek/scrapy-scraper )")
 		print("")
 		print("Usage:   scrapy-scraper -u urls                     -o out         [-dir directory]")
 		print("Example: scrapy-scraper -u https://example.com/home -o results.txt [-dir downloads]")
 		print("")
 		print("DESCRIPTION")
 		print("    Crawl and scrape websites")
 		print("URLS")
@@ -566,15 +566,15 @@
 # ----------------------------------------
 
 def main():
 	validate = Validate()
 	if validate.run():
 		print("###########################################################################")
 		print("#                                                                         #")
-		print("#                           Scrapy Scraper v1.6                           #")
+		print("#                           Scrapy Scraper v1.7                           #")
 		print("#                                     by Ivan Sincek                      #")
 		print("#                                                                         #")
 		print("# Crawl and scrape websites.                                              #")
 		print("# GitHub repository at github.com/ivan-sincek/scrapy-scraper.             #")
 		print("# Feel free to donate ETH at 0xbc00e800f29524AD8b0968CEBEAD4cD5C5c1f105.  #")
 		print("#                                                                         #")
 		print("###########################################################################")
```

### Comparing `scrapy-scraper-1.6/src/scrapy_scraper/user_agents.txt` & `scrapy_scraper-1.7/src/scrapy_scraper/user_agents.txt`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/86.0.4240.111 Safari/537.36
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/88.0.4324.182 Safari/537.36 Edg/88.0.705.74
-Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/86.0.4240.198 Safari/537.36
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.82 Safari/537.36 Edg/89.0.774.50
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/87.0.4280.88 Safari/537.36
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/85.0.4183.121 Safari/537.36 Edg/85.0.564.70
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/87.0.4280.67 Safari/537.36 Edg/87.0.664.52
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/85.0.4183.121 Safari/537.36
+Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:79.0) Gecko/20100101 Firefox/79.0
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/42.0.2311.135 Safari/537.36 Edge/12.10240
+Mozilla/5.0 (Windows NT 10.0; WOW64; rv:56.0) Gecko/20100101 Firefox/56.0
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.85 Safari/537.36
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/86.0.4240.198 Safari/537.36 Edg/86.0.622.69
 Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/86.0.4240.198 Safari/537.36
-Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.90 Safari/537.36
-Mozilla/5.0 (Windows NT 6.3; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.93 Safari/537.36
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/84.0.4147.135 Safari/537.36 Edg/84.0.522.63
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.82 Safari/537.36 Edg/89.0.774.50
+Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:88.0) Gecko/20100101 Firefox/88.0
+Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/84.0.4147.105 Safari/537.36
+Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.212 Safari/537.36
+Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.93 Safari/537.36
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/73.0.3683.75 Safari/537.36
+Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/14.0 Safari/605.1.15
+Mozilla/5.0 (Windows NT 6.3; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/88.0.4324.190 Safari/537.36
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.72 Safari/537.36 Edg/90.0.818.42
+Mozilla/5.0 (Macintosh; Intel Mac OS X 11_2_3) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.90 Safari/537.36
+Mozilla/5.0 (Macintosh; Intel Mac OS X 11_2_3) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.114 Safari/537.36
+Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:88.0) Gecko/20100101 Firefox/88.0
 Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.114 Safari/537.36 Edg/89.0.774.76
-Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/84.0.4147.125 Safari/537.36
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.85 Safari/537.36 Edg/90.0.818.46
-Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/86.0.4240.111 Safari/537.36
-Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.93 Safari/537.36
-Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.90 Safari/537.36
-Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/84.0.4147.135 Safari/537.36
-Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_6) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/14.0.3 Safari/605.1.15
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.102 Safari/537.36
-Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.116 Safari/537.36
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/81.0.4044.138 Safari/537.36
+Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/84.0.4147.105 Safari/537.36
+Mozilla/5.0 (Windows NT 6.3; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.93 Safari/537.36
+Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/14.1.1 Safari/605.1.15
+Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:79.0) Gecko/20100101 Firefox/79.0
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.93 Safari/537.36 Edg/90.0.818.56
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.82 Safari/537.36
+Mozilla/5.0 (Macintosh; Intel Mac OS X 10_12_6) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/12.1.2 Safari/605.1.15
 Mozilla/5.0 (Windows NT 6.3; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.61 Safari/537.36
-Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.114 Safari/537.36
+Mozilla/5.0 (Windows NT 6.2; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/86.0.4240.198 Safari/537.36
+Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_6) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/14.0.2 Safari/605.1.15
+Mozilla/5.0 (Windows NT 6.1; ) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.116 Safari/537.36
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/85.0.4183.121 Safari/537.36 Edg/85.0.564.70
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.93 Safari/537.36
+Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/85.0.4183.83 Safari/537.36
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/79.0.3945.136 Safari/537.36
+Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/86.0.4240.198 Safari/537.36
 Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.85 Safari/537.36 Edg/90.0.818.49
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.61 Safari/537.36 Edg/83.0.478.37
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.85 Safari/537.36
+Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.90 Safari/537.36
+Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_6) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/14.0.1 Safari/605.1.15
+Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.116 Safari/537.36
+Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/86.0.4240.111 Safari/537.36
+Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.116 Safari/537.36
+Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/88.0.4324.192 Safari/537.36
+Mozilla/5.0 (Windows NT 6.3; WOW64; Trident/7.0; rv:11.0) like Gecko
 Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.132 Safari/537.36
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/87.0.4280.67 Safari/537.36 Edg/87.0.664.47
-Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:88.0) Gecko/20100101 Firefox/88.0
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.114 Safari/537.36 Edg/89.0.774.68
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/73.0.3683.75 Safari/537.36
-Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.114 Safari/537.36
 Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/52.0.2743.116 Safari/537.36 Edge/15.15063
+Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/72.0.3626.121 Safari/537.36
 Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/55.0.2883.87 Safari/537.36
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/88.0.4324.182 Safari/537.36
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.128 Safari/537.36 Edg/89.0.774.77
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/86.0.4240.198 Safari/537.36 Edg/86.0.622.69
-Mozilla/5.0 (Windows NT 6.3; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/84.0.4147.125 Safari/537.36
-Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.93 Safari/537.36
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.90 Safari/537.36 Edg/89.0.774.54
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.114 Safari/537.36
+Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:86.0) Gecko/20100101 Firefox/86.0
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.102 Safari/537.36
 Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/87.0.4280.141 Safari/537.36 Edg/87.0.664.75
-Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.212 Safari/537.36
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/87.0.4280.67 Safari/537.36 Edg/87.0.664.52
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.82 Safari/537.36
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.72 Safari/537.36
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/84.0.4147.89 Safari/537.36
 Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.90 Safari/537.36
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/85.0.4183.121 Safari/537.36
-Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/72.0.3626.121 Safari/537.36
-Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/84.0.4147.105 Safari/537.36
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.116 Safari/537.36
-Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/85.0.4183.83 Safari/537.36
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.93 Safari/537.36 Edg/90.0.818.56
-Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/84.0.4147.105 Safari/537.36
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/84.0.4147.135 Safari/537.36 Edg/84.0.522.63
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.84 Safari/537.36
-Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_6) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/14.0.2 Safari/605.1.15
-Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:88.0) Gecko/20100101 Firefox/88.0
+Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/84.0.4147.135 Safari/537.36
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/87.0.4280.67 Safari/537.36 Edg/87.0.664.47
+Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.90 Safari/537.36
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/87.0.4280.66 Safari/537.36
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.90 Safari/537.36 Edg/89.0.774.57
+Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.106 Safari/537.36
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.72 Safari/537.36
+Mozilla/5.0 (Windows NT 6.3; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/84.0.4147.125 Safari/537.36
 Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/84.0.4147.135 Safari/537.36
-Mozilla/5.0 (Windows NT 6.3; WOW64; Trident/7.0; rv:11.0) like Gecko
-Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.106 Safari/537.36
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/88.0.4324.182 Safari/537.36 Edg/88.0.705.74
+Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.114 Safari/537.36
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/88.0.4324.182 Safari/537.36 Edg/88.0.705.81
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.85 Safari/537.36 Edg/90.0.818.46
+Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_6) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/14.0.3 Safari/605.1.15
+Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.93 Safari/537.36
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/87.0.4280.88 Safari/537.36
+Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/13.1 Safari/605.1.15
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.84 Safari/537.36
+Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.114 Safari/537.36
 Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/14.0.3 Safari/605.1.15
-Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.93 Safari/537.36
 Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/78.0.3904.70 Safari/537.36
-Mozilla/5.0 (Macintosh; Intel Mac OS X 11_2_3) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.90 Safari/537.36
+Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.114 Safari/537.36
+Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.93 Safari/537.36
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/88.0.4324.182 Safari/537.36
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.61 Safari/537.36 Edg/83.0.478.37
+Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/84.0.4147.125 Safari/537.36
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.128 Safari/537.36 Edg/89.0.774.77
 Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/88.0.4324.150 Safari/537.36
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/84.0.4147.89 Safari/537.36
-Mozilla/5.0 (Windows NT 10.0; WOW64; rv:56.0) Gecko/20100101 Firefox/56.0
-Mozilla/5.0 (Macintosh; Intel Mac OS X 11_2_3) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.114 Safari/537.36
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.72 Safari/537.36
-Mozilla/5.0 (Windows NT 6.3; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/88.0.4324.190 Safari/537.36
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.90 Safari/537.36 Edg/89.0.774.57
-Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.106 Safari/537.36
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.93 Safari/537.36
-Mozilla/5.0 (Windows NT 6.2; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/86.0.4240.198 Safari/537.36
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.90 Safari/537.36 Edg/89.0.774.54
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/79.0.3945.136 Safari/537.36
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.72 Safari/537.36
-Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/14.0 Safari/605.1.15
-Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.114 Safari/537.36
-Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:79.0) Gecko/20100101 Firefox/79.0
-Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.93 Safari/537.36
-Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/88.0.4324.192 Safari/537.36
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.114 Safari/537.36
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.72 Safari/537.36 Edg/90.0.818.42
-Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.116 Safari/537.36
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/88.0.4324.182 Safari/537.36 Edg/88.0.705.81
-Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:86.0) Gecko/20100101 Firefox/86.0
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/87.0.4280.66 Safari/537.36
-Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:85.0) Gecko/20100101 Firefox/85.0
-Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.90 Safari/537.36
-Mozilla/5.0 (Windows NT 6.1; ) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.116 Safari/537.36
-Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/42.0.2311.135 Safari/537.36 Edge/12.10240
-Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/14.1.1 Safari/605.1.15
 Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:88.0) Gecko/20100101 Firefox/88.0
-Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:79.0) Gecko/20100101 Firefox/79.0
-Mozilla/5.0 (Macintosh; Intel Mac OS X 10_12_6) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/12.1.2 Safari/605.1.15
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.114 Safari/537.36 Edg/89.0.774.68
+Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/86.0.4240.111 Safari/537.36
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.116 Safari/537.36
+Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.93 Safari/537.36
 Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_6) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/14.0 Safari/605.1.15
-Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/13.1 Safari/605.1.15
-Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_6) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/14.0.1 Safari/605.1.15
+Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.90 Safari/537.36
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/81.0.4044.138 Safari/537.36
+Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.106 Safari/537.36
+Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:85.0) Gecko/20100101 Firefox/85.0
```

### Comparing `scrapy-scraper-1.6/src/scrapy_scraper.egg-info/PKG-INFO` & `scrapy_scraper-1.7/src/scrapy_scraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: scrapy-scraper
-Version: 1.6
+Version: 1.7
 Summary: Web crawler and scraper based on Scrapy and Playwright's headless browser.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/scrapy-scraper
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: argparse>=1.4.0
 Requires-Dist: beautifulsoup4>=4.11.1
 Requires-Dist: bs4>=0.0.1
 Requires-Dist: colorama>=0.4.6
 Requires-Dist: datetime>=5.2
 Requires-Dist: jsbeautifier>=1.14.11
 Requires-Dist: scrapy>=2.11.0
 Requires-Dist: termcolor>=1.1.0
@@ -71,15 +70,15 @@
 ```bash
 git clone https://github.com/ivan-sincek/scrapy-scraper && cd scrapy-scraper
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/scrapy-scraper-1.6-py3-none-any.whl
+python3 -m pip install dist/scrapy-scraper-1.7-py3-none-any.whl
 ```
 
 ## How to Run
 
 Restricted (domain whitelisting is on):
 
 ```fundamental
@@ -91,15 +90,15 @@
 ```fundamental
 scrapy-scraper -u https://example.com/home -o results.txt -a random -s random -dir js -l -w off
 ```
 
 ## Usage
 
 ```fundamental
-Scrapy Scraper v1.6 ( github.com/ivan-sincek/scrapy-scraper )
+Scrapy Scraper v1.7 ( github.com/ivan-sincek/scrapy-scraper )
 
 Usage:   scrapy-scraper -u urls                     -o out         [-dir directory]
 Example: scrapy-scraper -u https://example.com/home -o results.txt [-dir downloads]
 
 DESCRIPTION
     Crawl and scrape websites
 URLS
@@ -135,15 +134,15 @@
 RECURSION
     Recursion depth limit
     Specify '0' for no limit
     Default: 1
     -r, --recursion = 0 | 2 | 4 | etc.
 USER AGENT
     User agent to use
-    Default: Scrapy Scraper/1.6
+    Default: Scrapy Scraper/1.7
     -a, --user-agent = curl/3.30.1 | random | etc.
 PROXY
     Web proxy to use
     -x, --proxy = http://127.0.0.1:8080 | etc.
 DIRECTORY
     Output directory
     All extracted JavaScript files will be saved in this directory
```

