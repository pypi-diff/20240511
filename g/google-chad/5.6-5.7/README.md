# Comparing `tmp/google-chad-5.6.tar.gz` & `tmp/google_chad-5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-chad-5.6.tar", last modified: Sat Dec 30 15:26:00 2023, max compression
+gzip compressed data, was "google_chad-5.7.tar", last modified: Sat May 11 10:53:57 2024, max compression
```

## Comparing `google-chad-5.6.tar` & `google_chad-5.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-30 15:26:00.069801 google-chad-5.6/
--rw-r--r--   0 root         (0) root         (0)     1069 2023-12-30 15:15:02.000000 google-chad-5.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      107 2023-12-30 15:15:02.000000 google-chad-5.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    13236 2023-12-30 15:26:00.069801 google-chad-5.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12544 2023-12-30 15:24:33.000000 google-chad-5.6/README.md
--rw-r--r--   0 root         (0) root         (0)      888 2023-12-30 15:24:35.000000 google-chad-5.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-12-30 15:26:00.069801 google-chad-5.6/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-30 15:26:00.065799 google-chad-5.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-30 15:26:00.069801 google-chad-5.6/src/chad/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-30 15:15:02.000000 google-chad-5.6/src/chad/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22568 2023-12-30 15:24:02.000000 google-chad-5.6/src/chad/chad.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-30 15:26:00.069801 google-chad-5.6/src/chad_extractor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-30 15:15:02.000000 google-chad-5.6/src/chad_extractor/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31531 2023-12-30 15:24:05.000000 google-chad-5.6/src/chad_extractor/chad_extractor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-30 15:26:00.069801 google-chad-5.6/src/dorks/
--rw-r--r--   0 root         (0) root         (0)      282 2023-12-30 15:15:02.000000 google-chad-5.6/src/dorks/social_media_dorks.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-30 15:26:00.069801 google-chad-5.6/src/google_chad.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13236 2023-12-30 15:26:00.000000 google-chad-5.6/src/google_chad.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2023-12-30 15:26:00.000000 google-chad-5.6/src/google_chad.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-30 15:26:00.000000 google-chad-5.6/src/google_chad.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       92 2023-12-30 15:26:00.000000 google-chad-5.6/src/google_chad.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      151 2023-12-30 15:26:00.000000 google-chad-5.6/src/google_chad.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-12-30 15:26:00.000000 google-chad-5.6/src/google_chad.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-30 15:26:00.069801 google-chad-5.6/src/templates/
--rw-r--r--   0 root         (0) root         (0)     2057 2023-12-30 15:15:02.000000 google-chad-5.6/src/templates/social_media_template.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 10:53:57.001403 google_chad-5.7/
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-05-11 10:50:58.000000 google_chad-5.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      107 2024-05-11 10:50:58.000000 google_chad-5.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    13517 2024-05-11 10:53:57.001403 google_chad-5.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12856 2024-05-11 10:51:32.000000 google_chad-5.7/README.md
+-rw-r--r--   0 root         (0) root         (0)      869 2024-05-11 10:51:12.000000 google_chad-5.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-11 10:53:57.001403 google_chad-5.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 10:53:57.001403 google_chad-5.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 10:53:57.001403 google_chad-5.7/src/chad/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 10:50:58.000000 google_chad-5.7/src/chad/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22568 2024-05-11 10:51:48.000000 google_chad-5.7/src/chad/chad.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 10:53:57.001403 google_chad-5.7/src/chad_extractor/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 10:50:58.000000 google_chad-5.7/src/chad_extractor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31531 2024-05-11 10:52:02.000000 google_chad-5.7/src/chad_extractor/chad_extractor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 10:53:57.001403 google_chad-5.7/src/dorks/
+-rw-r--r--   0 root         (0) root         (0)      282 2024-05-11 10:50:58.000000 google_chad-5.7/src/dorks/social_media_dorks.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 10:53:57.001403 google_chad-5.7/src/google_chad.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13517 2024-05-11 10:53:56.000000 google_chad-5.7/src/google_chad.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2024-05-11 10:53:57.000000 google_chad-5.7/src/google_chad.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 10:53:56.000000 google_chad-5.7/src/google_chad.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2024-05-11 10:53:56.000000 google_chad-5.7/src/google_chad.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      135 2024-05-11 10:53:56.000000 google_chad-5.7/src/google_chad.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2024-05-11 10:53:56.000000 google_chad-5.7/src/google_chad.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 10:53:57.001403 google_chad-5.7/src/templates/
+-rw-r--r--   0 root         (0) root         (0)     2057 2024-05-11 10:50:58.000000 google_chad-5.7/src/templates/social_media_template.json
```

### Comparing `google-chad-5.6/LICENSE` & `google_chad-5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `google-chad-5.6/PKG-INFO` & `google_chad-5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: google-chad
-Version: 5.6
+Version: 5.7
 Summary: Not another Google Dorking tool.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/chad
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: argparse>=1.4.0
 Requires-Dist: asyncio>=3.4.3
 Requires-Dist: colorama>=0.4.6
 Requires-Dist: datetime>=5.0
 Requires-Dist: nagooglesearch>=6.9
 Requires-Dist: playwright>=1.40.0
 Requires-Dist: regex>=2022.4.24
 Requires-Dist: requests>=2.27.1
@@ -27,48 +26,56 @@
 Tested on Kali Linux v2023.4 (64-bit).
 
 Made for educational purposes. I hope it will help!
 
 ## Table of Contents
 
 * [How to Install](#how-to-install)
-* [How to Build and Install Manually](#how-to-build-and-install-manually)
+	* [Install Playwright and Chromium](#install-playwright-and-chromium)
+	* [Standard Install](#standard-install)
+	* [Build and Install From the Source](#build-and-install-from-the-source)
 * [Shortest Possible](#shortest-possible)
 * [Basic Example: File Download](#basic-example-file-download)
 * [Chad Extractor](#chad-extractor)
-    * [Extracting and Validating Data)](#extracting-and-validating-data)
+    * [Extracting and Validating Data](#extracting-and-validating-data)
 * [Advanced Example: Social Media Takover](#advanced-example-social-media-takover)
     * [Basic Use (Single Domain)](#basic-use-single-domain)
     * [Advanced Use (Multiple Domains)](#advanced-use-multiple-domains)
 * [Rate Limiting](#rate-limiting)
 * [Usage](#usage)
 * [Images](#images)
 
 ## How to Install
 
+### Install Playwright and Chromium
+
 ```bash
-pip3 install --upgrade google-chad
+pip3 install --upgrade playwright
 
 playwright install chromium
 ```
 
-## How to Build and Install Manually
+Make sure each time you upgrade your Playwright dependency to re-install Chromium; otherwise, you might get no results from Chad Extractor.
 
-Run the following commands:
+### Standard Install
+
+```bash
+pip3 install --upgrade google-chad
+```
+
+### Build and Install From the Source
 
 ```bash
 git clone https://github.com/ivan-sincek/chad && cd chad
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/google_chad-5.6-py3-none-any.whl
-
-playwright install chromium
+python3 -m pip install dist/google_chad-5.7-py3-none-any.whl
 ```
 
 ## Shortest Possible
 
 ```bash
 chad -q 'intitle:"index of /" intext:"parent directory"'
 ```
@@ -91,29 +98,29 @@
 
 Chad Extractor is a powerful tool based on [Playwright's](https://playwright.dev/python) Chromium headless browser created to efficiently scrape web; in other words, to compensate for Python Requests library which cannot render JavaScript encoded HTML and is easily blocked by anti-bot solutions.
 
 There is a built-in 4 seconds delay between starting each headless browser; otherwise, it would be very resources-intensive.
 
 ### Extracting and Validating Data
 
-Chad Extractor was mainly designed to extract and validate data from Chad results; but, you can also use it to extract and validate data from plaintext files by specifying `-pt` option - plaintext files will be treated like server responses and extraction logic will be immediately applied.
+Chad Extractor was mainly designed to extract and validate data from Chad results; but, you can also use it to extract and validate data from plaintext files by specifying `-pt` option - plaintext files will be treated similar to server responses and extraction logic will be immediately applied.
 
 ## Advanced Example: Social Media Takover
 
 Prepare Google Dorks as [social_media_dorks.txt](https://github.com/ivan-sincek/chad/blob/main/src/dorks/social_media_dorks.txt) file:
 
 ```fundamental
 intext:"t.me/"
 intext:"discord.com/invite/" OR intext:"discord.gg/invite/"
 intext:"youtube.com/c/" OR intext:"youtube.com/channel/"
 intext:"twitter.com/"
 intext:"facebook.com/"
 intext:"instagram.com/"
 intext:"tiktok.com/"
-intext:"linkedin.com/in/" OR intext:"linkedin.com/company/"
+intext:"linkedin.com/company/" OR intext:"linkedin.com/in/"
 ```
 
 Prepare a template as [social_media_template.json](https://github.com/ivan-sincek/chad/blob/main/src/templates/social_media_template.json) file:
 
 ```json
 {
    "telegram":{
@@ -167,15 +174,15 @@
 
 **Make sure your regular expressions return only one capturing group e.g. `[1, 2, 3, 4]`; and not a touple e.g. `[(1, 2), (3, 4)]`.**
 
 Make sure to properly escape regular expression specific symbols in your template file, e.g. make sure to escape dot `.` as `\\.`, and forward slash `/` as `\\/`, etc.
 
 All regular expression searches are case-insensitive.
 
-Web content fetched from the URLs in Chad results will be matched against all the regular expressions (`extract` attributes) in the template file in order to find as much relevant data as possible.
+Web content fetched from the URLs from Chad results will be matched against all the regular expressions (`extract` attributes) from the template file in order to find as much relevant data as possible.
 
 To extract data without validating it, omit `validate` attributes from the template file as necessary.
 
 ### Basic Use (Single Domain)
 
 ```bash
 chad -q social_media_dorks.txt -s *.example.com -tr 200 -o results.json
@@ -244,28 +251,28 @@
 chad-extractor -t social_media_template.json -res chad_results -a user_agents.txt -o results_report.json -v
 ```
 
 ## Rate Limiting
 
 Google's cooling-off period can be from a few hours to a whole day.
 
-To avoid hitting Google's rate limit with Chad, increase the minimum and maximum sleep between Google queries and/or pages; or use proxies \([1](https://geonode.com/free-proxy-list)\)\([2](https://proxyscrape.com/home)\), although, free proxies are not always stable and often blocked.
+To avoid hitting Google's rate limit with Chad, increase the minimum and maximum sleep between Google queries and/or pages; or use \[free\] proxies \([1](https://geonode.com/free-proxy-list)\)\([2](https://proxyscrape.com/home)\); although, free proxies are often blocked and unstable.
 
 To download a list of free proxies, run:
 
 ```bash
 curl -s 'https://proxylist.geonode.com/api/proxy-list?limit=50&page=1&sort_by=lastChecked&sort_type=desc' -H 'Referer: https://proxylist.geonode.com/' | jq -r '.data[] | "\(.protocols[])://\(.ip):\(.port)"' > proxies.txt
 ```
 
 Additionally, to avoid hitting e.g. [Instagram's](https://www.instagram.com) rate limit with Chad Extractor, you might want to isolate it in a separate run, increase the wait time, and use only one thread.
 
 ## Usage
 
 ```fundamental
-Chad v5.6 ( github.com/ivan-sincek/chad )
+Chad v5.7 ( github.com/ivan-sincek/chad )
 
 Usage:   chad -q queries     [-s site         ] [-x proxies    ] [-o out         ]
 Example: chad -q queries.txt [-s *.example.com] [-x proxies.txt] [-o results.json]
 
 DESCRIPTION
     Search Google Dorks like Chad
 QUERIES
@@ -324,15 +331,15 @@
     -nsos, --no-sleep-on-start
 DEBUG
     Debug output
     -dbg, --debug
 ```
 
 ```fundamental
-Chad Extractor v5.6 ( github.com/ivan-sincek/chad )
+Chad Extractor v5.7 ( github.com/ivan-sincek/chad )
 
 Usage:   chad-extractor -t template      -res results      -o out                 [-th threads] [-r retries] [-w wait]
 Example: chad-extractor -t template.json -res chad_results -o results_report.json [-th 10     ] [-r 5      ] [-w 10  ]
 
 DESCRIPTION
     Extract and validate data from Chad results or plaintext files
 TEMPLATE
```

### Comparing `google-chad-5.6/README.md` & `google_chad-5.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,48 +5,56 @@
 Tested on Kali Linux v2023.4 (64-bit).
 
 Made for educational purposes. I hope it will help!
 
 ## Table of Contents
 
 * [How to Install](#how-to-install)
-* [How to Build and Install Manually](#how-to-build-and-install-manually)
+	* [Install Playwright and Chromium](#install-playwright-and-chromium)
+	* [Standard Install](#standard-install)
+	* [Build and Install From the Source](#build-and-install-from-the-source)
 * [Shortest Possible](#shortest-possible)
 * [Basic Example: File Download](#basic-example-file-download)
 * [Chad Extractor](#chad-extractor)
-    * [Extracting and Validating Data)](#extracting-and-validating-data)
+    * [Extracting and Validating Data](#extracting-and-validating-data)
 * [Advanced Example: Social Media Takover](#advanced-example-social-media-takover)
     * [Basic Use (Single Domain)](#basic-use-single-domain)
     * [Advanced Use (Multiple Domains)](#advanced-use-multiple-domains)
 * [Rate Limiting](#rate-limiting)
 * [Usage](#usage)
 * [Images](#images)
 
 ## How to Install
 
+### Install Playwright and Chromium
+
 ```bash
-pip3 install --upgrade google-chad
+pip3 install --upgrade playwright
 
 playwright install chromium
 ```
 
-## How to Build and Install Manually
+Make sure each time you upgrade your Playwright dependency to re-install Chromium; otherwise, you might get no results from Chad Extractor.
 
-Run the following commands:
+### Standard Install
+
+```bash
+pip3 install --upgrade google-chad
+```
+
+### Build and Install From the Source
 
 ```bash
 git clone https://github.com/ivan-sincek/chad && cd chad
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/google_chad-5.6-py3-none-any.whl
-
-playwright install chromium
+python3 -m pip install dist/google_chad-5.7-py3-none-any.whl
 ```
 
 ## Shortest Possible
 
 ```bash
 chad -q 'intitle:"index of /" intext:"parent directory"'
 ```
@@ -69,29 +77,29 @@
 
 Chad Extractor is a powerful tool based on [Playwright's](https://playwright.dev/python) Chromium headless browser created to efficiently scrape web; in other words, to compensate for Python Requests library which cannot render JavaScript encoded HTML and is easily blocked by anti-bot solutions.
 
 There is a built-in 4 seconds delay between starting each headless browser; otherwise, it would be very resources-intensive.
 
 ### Extracting and Validating Data
 
-Chad Extractor was mainly designed to extract and validate data from Chad results; but, you can also use it to extract and validate data from plaintext files by specifying `-pt` option - plaintext files will be treated like server responses and extraction logic will be immediately applied.
+Chad Extractor was mainly designed to extract and validate data from Chad results; but, you can also use it to extract and validate data from plaintext files by specifying `-pt` option - plaintext files will be treated similar to server responses and extraction logic will be immediately applied.
 
 ## Advanced Example: Social Media Takover
 
 Prepare Google Dorks as [social_media_dorks.txt](https://github.com/ivan-sincek/chad/blob/main/src/dorks/social_media_dorks.txt) file:
 
 ```fundamental
 intext:"t.me/"
 intext:"discord.com/invite/" OR intext:"discord.gg/invite/"
 intext:"youtube.com/c/" OR intext:"youtube.com/channel/"
 intext:"twitter.com/"
 intext:"facebook.com/"
 intext:"instagram.com/"
 intext:"tiktok.com/"
-intext:"linkedin.com/in/" OR intext:"linkedin.com/company/"
+intext:"linkedin.com/company/" OR intext:"linkedin.com/in/"
 ```
 
 Prepare a template as [social_media_template.json](https://github.com/ivan-sincek/chad/blob/main/src/templates/social_media_template.json) file:
 
 ```json
 {
    "telegram":{
@@ -145,15 +153,15 @@
 
 **Make sure your regular expressions return only one capturing group e.g. `[1, 2, 3, 4]`; and not a touple e.g. `[(1, 2), (3, 4)]`.**
 
 Make sure to properly escape regular expression specific symbols in your template file, e.g. make sure to escape dot `.` as `\\.`, and forward slash `/` as `\\/`, etc.
 
 All regular expression searches are case-insensitive.
 
-Web content fetched from the URLs in Chad results will be matched against all the regular expressions (`extract` attributes) in the template file in order to find as much relevant data as possible.
+Web content fetched from the URLs from Chad results will be matched against all the regular expressions (`extract` attributes) from the template file in order to find as much relevant data as possible.
 
 To extract data without validating it, omit `validate` attributes from the template file as necessary.
 
 ### Basic Use (Single Domain)
 
 ```bash
 chad -q social_media_dorks.txt -s *.example.com -tr 200 -o results.json
@@ -222,28 +230,28 @@
 chad-extractor -t social_media_template.json -res chad_results -a user_agents.txt -o results_report.json -v
 ```
 
 ## Rate Limiting
 
 Google's cooling-off period can be from a few hours to a whole day.
 
-To avoid hitting Google's rate limit with Chad, increase the minimum and maximum sleep between Google queries and/or pages; or use proxies \([1](https://geonode.com/free-proxy-list)\)\([2](https://proxyscrape.com/home)\), although, free proxies are not always stable and often blocked.
+To avoid hitting Google's rate limit with Chad, increase the minimum and maximum sleep between Google queries and/or pages; or use \[free\] proxies \([1](https://geonode.com/free-proxy-list)\)\([2](https://proxyscrape.com/home)\); although, free proxies are often blocked and unstable.
 
 To download a list of free proxies, run:
 
 ```bash
 curl -s 'https://proxylist.geonode.com/api/proxy-list?limit=50&page=1&sort_by=lastChecked&sort_type=desc' -H 'Referer: https://proxylist.geonode.com/' | jq -r '.data[] | "\(.protocols[])://\(.ip):\(.port)"' > proxies.txt
 ```
 
 Additionally, to avoid hitting e.g. [Instagram's](https://www.instagram.com) rate limit with Chad Extractor, you might want to isolate it in a separate run, increase the wait time, and use only one thread.
 
 ## Usage
 
 ```fundamental
-Chad v5.6 ( github.com/ivan-sincek/chad )
+Chad v5.7 ( github.com/ivan-sincek/chad )
 
 Usage:   chad -q queries     [-s site         ] [-x proxies    ] [-o out         ]
 Example: chad -q queries.txt [-s *.example.com] [-x proxies.txt] [-o results.json]
 
 DESCRIPTION
     Search Google Dorks like Chad
 QUERIES
@@ -302,15 +310,15 @@
     -nsos, --no-sleep-on-start
 DEBUG
     Debug output
     -dbg, --debug
 ```
 
 ```fundamental
-Chad Extractor v5.6 ( github.com/ivan-sincek/chad )
+Chad Extractor v5.7 ( github.com/ivan-sincek/chad )
 
 Usage:   chad-extractor -t template      -res results      -o out                 [-th threads] [-r retries] [-w wait]
 Example: chad-extractor -t template.json -res chad_results -o results_report.json [-th 10     ] [-r 5      ] [-w 10  ]
 
 DESCRIPTION
     Extract and validate data from Chad results or plaintext files
 TEMPLATE
```

### Comparing `google-chad-5.6/pyproject.toml` & `google_chad-5.7/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "google-chad"
-version = "5.6"
+version = "5.7"
 authors = [{ name = "Ivan Sincek" }]
 description = "Not another Google Dorking tool."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
 	"Operating System :: OS Independent"
 ]
-dependencies = ["argparse>=1.4.0", "asyncio>=3.4.3", "colorama>=0.4.6", "datetime>=5.0", "nagooglesearch>=6.9", "playwright>=1.40.0", "regex>=2022.4.24", "requests>=2.27.1", "termcolor>=1.1.0"]
+dependencies = ["asyncio>=3.4.3", "colorama>=0.4.6", "datetime>=5.0", "nagooglesearch>=6.9", "playwright>=1.40.0", "regex>=2022.4.24", "requests>=2.27.1", "termcolor>=1.1.0"]
 
 [project.urls]
 "Homepage" = "https://github.com/ivan-sincek/chad"
 
 [project.scripts]
 chad = "chad.chad:main"
 chad-extractor = "chad_extractor.chad_extractor:main"
```

### Comparing `google-chad-5.6/src/chad/chad.py` & `google_chad-5.7/src/chad/chad.py`

 * *Files 0% similar despite different names*

```diff
@@ -339,15 +339,15 @@
 		self.__count += 1
 
 # ----------------------------------------
 
 class MyArgParser(argparse.ArgumentParser):
 
 	def print_help(self):
-		print("Chad v5.6 ( github.com/ivan-sincek/chad )")
+		print("Chad v5.7 ( github.com/ivan-sincek/chad )")
 		print("")
 		print("Usage:   chad -q queries     [-s site         ] [-x proxies    ] [-o out         ]")
 		print("Example: chad -q queries.txt [-s *.example.com] [-x proxies.txt] [-o results.json]")
 		print("")
 		print("DESCRIPTION")
 		print("    Search Google Dorks like Chad")
 		print("QUERIES")
@@ -558,15 +558,15 @@
 # ----------------------------------------
 
 def main():
 	validate = Validate()
 	if validate.run():
 		print("###########################################################################")
 		print("#                                                                         #")
-		print("#                                Chad v5.6                                #")
+		print("#                                Chad v5.7                                #")
 		print("#                                  by Ivan Sincek                         #")
 		print("#                                                                         #")
 		print("# Search Google Dorks like Chad.                                          #")
 		print("# GitHub repository at github.com/ivan-sincek/chad.                       #")
 		print("# Feel free to donate ETH at 0xbc00e800f29524AD8b0968CEBEAD4cD5C5c1f105.  #")
 		print("#                                                                         #")
 		print("###########################################################################")
```

### Comparing `google-chad-5.6/src/chad_extractor/chad_extractor.py` & `google_chad-5.7/src/chad_extractor/chad_extractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -577,15 +577,15 @@
 		return tmp
 
 # ----------------------------------------
 
 class MyArgParser(argparse.ArgumentParser):
 
 	def print_help(self):
-		print("Chad Extractor v5.6 ( github.com/ivan-sincek/chad )")
+		print("Chad Extractor v5.7 ( github.com/ivan-sincek/chad )")
 		print("")
 		print("Usage:   chad-extractor -t template      -res results      -o out                 [-th threads] [-r retries] [-w wait]")
 		print("Example: chad-extractor -t template.json -res chad_results -o results_report.json [-th 10     ] [-r 5      ] [-w 10  ]")
 		print("")
 		print("DESCRIPTION")
 		print("    Extract and validate data from Chad results or plaintext files")
 		print("TEMPLATE")
@@ -800,15 +800,15 @@
 # ----------------------------------------
 
 def main():
 	validate = Validate()
 	if validate.run():
 		print("###########################################################################")
 		print("#                                                                         #")
-		print("#                           Chad Extractor v5.6                           #")
+		print("#                           Chad Extractor v5.7                           #")
 		print("#                                   by Ivan Sincek                        #")
 		print("#                                                                         #")
 		print("# Extract and validate data from Chad results.                            #")
 		print("# GitHub repository at github.com/ivan-sincek/chad.                       #")
 		print("# Feel free to donate ETH at 0xbc00e800f29524AD8b0968CEBEAD4cD5C5c1f105.  #")
 		print("#                                                                         #")
 		print("###########################################################################")
```

### Comparing `google-chad-5.6/src/google_chad.egg-info/PKG-INFO` & `google_chad-5.7/src/google_chad.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: google-chad
-Version: 5.6
+Version: 5.7
 Summary: Not another Google Dorking tool.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/chad
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: argparse>=1.4.0
 Requires-Dist: asyncio>=3.4.3
 Requires-Dist: colorama>=0.4.6
 Requires-Dist: datetime>=5.0
 Requires-Dist: nagooglesearch>=6.9
 Requires-Dist: playwright>=1.40.0
 Requires-Dist: regex>=2022.4.24
 Requires-Dist: requests>=2.27.1
@@ -27,48 +26,56 @@
 Tested on Kali Linux v2023.4 (64-bit).
 
 Made for educational purposes. I hope it will help!
 
 ## Table of Contents
 
 * [How to Install](#how-to-install)
-* [How to Build and Install Manually](#how-to-build-and-install-manually)
+	* [Install Playwright and Chromium](#install-playwright-and-chromium)
+	* [Standard Install](#standard-install)
+	* [Build and Install From the Source](#build-and-install-from-the-source)
 * [Shortest Possible](#shortest-possible)
 * [Basic Example: File Download](#basic-example-file-download)
 * [Chad Extractor](#chad-extractor)
-    * [Extracting and Validating Data)](#extracting-and-validating-data)
+    * [Extracting and Validating Data](#extracting-and-validating-data)
 * [Advanced Example: Social Media Takover](#advanced-example-social-media-takover)
     * [Basic Use (Single Domain)](#basic-use-single-domain)
     * [Advanced Use (Multiple Domains)](#advanced-use-multiple-domains)
 * [Rate Limiting](#rate-limiting)
 * [Usage](#usage)
 * [Images](#images)
 
 ## How to Install
 
+### Install Playwright and Chromium
+
 ```bash
-pip3 install --upgrade google-chad
+pip3 install --upgrade playwright
 
 playwright install chromium
 ```
 
-## How to Build and Install Manually
+Make sure each time you upgrade your Playwright dependency to re-install Chromium; otherwise, you might get no results from Chad Extractor.
 
-Run the following commands:
+### Standard Install
+
+```bash
+pip3 install --upgrade google-chad
+```
+
+### Build and Install From the Source
 
 ```bash
 git clone https://github.com/ivan-sincek/chad && cd chad
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/google_chad-5.6-py3-none-any.whl
-
-playwright install chromium
+python3 -m pip install dist/google_chad-5.7-py3-none-any.whl
 ```
 
 ## Shortest Possible
 
 ```bash
 chad -q 'intitle:"index of /" intext:"parent directory"'
 ```
@@ -91,29 +98,29 @@
 
 Chad Extractor is a powerful tool based on [Playwright's](https://playwright.dev/python) Chromium headless browser created to efficiently scrape web; in other words, to compensate for Python Requests library which cannot render JavaScript encoded HTML and is easily blocked by anti-bot solutions.
 
 There is a built-in 4 seconds delay between starting each headless browser; otherwise, it would be very resources-intensive.
 
 ### Extracting and Validating Data
 
-Chad Extractor was mainly designed to extract and validate data from Chad results; but, you can also use it to extract and validate data from plaintext files by specifying `-pt` option - plaintext files will be treated like server responses and extraction logic will be immediately applied.
+Chad Extractor was mainly designed to extract and validate data from Chad results; but, you can also use it to extract and validate data from plaintext files by specifying `-pt` option - plaintext files will be treated similar to server responses and extraction logic will be immediately applied.
 
 ## Advanced Example: Social Media Takover
 
 Prepare Google Dorks as [social_media_dorks.txt](https://github.com/ivan-sincek/chad/blob/main/src/dorks/social_media_dorks.txt) file:
 
 ```fundamental
 intext:"t.me/"
 intext:"discord.com/invite/" OR intext:"discord.gg/invite/"
 intext:"youtube.com/c/" OR intext:"youtube.com/channel/"
 intext:"twitter.com/"
 intext:"facebook.com/"
 intext:"instagram.com/"
 intext:"tiktok.com/"
-intext:"linkedin.com/in/" OR intext:"linkedin.com/company/"
+intext:"linkedin.com/company/" OR intext:"linkedin.com/in/"
 ```
 
 Prepare a template as [social_media_template.json](https://github.com/ivan-sincek/chad/blob/main/src/templates/social_media_template.json) file:
 
 ```json
 {
    "telegram":{
@@ -167,15 +174,15 @@
 
 **Make sure your regular expressions return only one capturing group e.g. `[1, 2, 3, 4]`; and not a touple e.g. `[(1, 2), (3, 4)]`.**
 
 Make sure to properly escape regular expression specific symbols in your template file, e.g. make sure to escape dot `.` as `\\.`, and forward slash `/` as `\\/`, etc.
 
 All regular expression searches are case-insensitive.
 
-Web content fetched from the URLs in Chad results will be matched against all the regular expressions (`extract` attributes) in the template file in order to find as much relevant data as possible.
+Web content fetched from the URLs from Chad results will be matched against all the regular expressions (`extract` attributes) from the template file in order to find as much relevant data as possible.
 
 To extract data without validating it, omit `validate` attributes from the template file as necessary.
 
 ### Basic Use (Single Domain)
 
 ```bash
 chad -q social_media_dorks.txt -s *.example.com -tr 200 -o results.json
@@ -244,28 +251,28 @@
 chad-extractor -t social_media_template.json -res chad_results -a user_agents.txt -o results_report.json -v
 ```
 
 ## Rate Limiting
 
 Google's cooling-off period can be from a few hours to a whole day.
 
-To avoid hitting Google's rate limit with Chad, increase the minimum and maximum sleep between Google queries and/or pages; or use proxies \([1](https://geonode.com/free-proxy-list)\)\([2](https://proxyscrape.com/home)\), although, free proxies are not always stable and often blocked.
+To avoid hitting Google's rate limit with Chad, increase the minimum and maximum sleep between Google queries and/or pages; or use \[free\] proxies \([1](https://geonode.com/free-proxy-list)\)\([2](https://proxyscrape.com/home)\); although, free proxies are often blocked and unstable.
 
 To download a list of free proxies, run:
 
 ```bash
 curl -s 'https://proxylist.geonode.com/api/proxy-list?limit=50&page=1&sort_by=lastChecked&sort_type=desc' -H 'Referer: https://proxylist.geonode.com/' | jq -r '.data[] | "\(.protocols[])://\(.ip):\(.port)"' > proxies.txt
 ```
 
 Additionally, to avoid hitting e.g. [Instagram's](https://www.instagram.com) rate limit with Chad Extractor, you might want to isolate it in a separate run, increase the wait time, and use only one thread.
 
 ## Usage
 
 ```fundamental
-Chad v5.6 ( github.com/ivan-sincek/chad )
+Chad v5.7 ( github.com/ivan-sincek/chad )
 
 Usage:   chad -q queries     [-s site         ] [-x proxies    ] [-o out         ]
 Example: chad -q queries.txt [-s *.example.com] [-x proxies.txt] [-o results.json]
 
 DESCRIPTION
     Search Google Dorks like Chad
 QUERIES
@@ -324,15 +331,15 @@
     -nsos, --no-sleep-on-start
 DEBUG
     Debug output
     -dbg, --debug
 ```
 
 ```fundamental
-Chad Extractor v5.6 ( github.com/ivan-sincek/chad )
+Chad Extractor v5.7 ( github.com/ivan-sincek/chad )
 
 Usage:   chad-extractor -t template      -res results      -o out                 [-th threads] [-r retries] [-w wait]
 Example: chad-extractor -t template.json -res chad_results -o results_report.json [-th 10     ] [-r 5      ] [-w 10  ]
 
 DESCRIPTION
     Extract and validate data from Chad results or plaintext files
 TEMPLATE
```

### Comparing `google-chad-5.6/src/templates/social_media_template.json` & `google_chad-5.7/src/templates/social_media_template.json`

 * *Files identical despite different names*

