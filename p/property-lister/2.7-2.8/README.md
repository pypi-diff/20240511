# Comparing `tmp/property-lister-2.7.tar.gz` & `tmp/property_lister-2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "property-lister-2.7.tar", last modified: Fri Mar  8 14:15:50 2024, max compression
+gzip compressed data, was "property_lister-2.8.tar", last modified: Sat May 11 10:46:16 2024, max compression
```

## Comparing `property-lister-2.7.tar` & `property_lister-2.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 14:15:50.989372 property-lister-2.7/
--rwxrwx---   0 root         (0) root         (0)     1090 2024-03-08 14:12:50.000000 property-lister-2.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3293 2024-03-08 14:15:50.989372 property-lister-2.7/PKG-INFO
--rwxrwx---   0 root         (0) root         (0)     2821 2024-03-08 14:14:57.000000 property-lister-2.7/README.md
--rwxrwx---   0 root         (0) root         (0)      780 2024-03-08 14:15:02.000000 property-lister-2.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-08 14:15:50.989372 property-lister-2.7/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 14:15:50.985374 property-lister-2.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 14:15:50.985374 property-lister-2.7/src/property_lister/
--rwxrwx---   0 root         (0) root         (0)        0 2024-03-08 14:12:50.000000 property-lister-2.7/src/property_lister/__init__.py
--rwxrwx---   0 root         (0) root         (0)     9104 2024-03-08 14:15:15.000000 property-lister-2.7/src/property_lister/property_lister.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 14:15:50.989372 property-lister-2.7/src/property_lister.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3293 2024-03-08 14:15:50.000000 property-lister-2.7/src/property_lister.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      363 2024-03-08 14:15:50.000000 property-lister-2.7/src/property_lister.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 14:15:50.000000 property-lister-2.7/src/property_lister.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-08 14:15:50.000000 property-lister-2.7/src/property_lister.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       45 2024-03-08 14:15:50.000000 property-lister-2.7/src/property_lister.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-03-08 14:15:50.000000 property-lister-2.7/src/property_lister.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 10:46:16.366362 property_lister-2.8/
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-05-11 10:45:15.000000 property_lister-2.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3233 2024-05-11 10:46:16.366362 property_lister-2.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2683 2024-05-11 10:45:48.000000 property_lister-2.8/README.md
+-rw-r--r--   0 root         (0) root         (0)      735 2024-05-11 10:45:25.000000 property_lister-2.8/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-11 10:46:16.366362 property_lister-2.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 10:46:16.362360 property_lister-2.8/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 10:46:16.362360 property_lister-2.8/src/property_lister/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 10:45:15.000000 property_lister-2.8/src/property_lister/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8839 2024-05-11 10:46:05.000000 property_lister-2.8/src/property_lister/property_lister.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 10:46:16.362360 property_lister-2.8/src/property_lister.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3233 2024-05-11 10:46:16.000000 property_lister-2.8/src/property_lister.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      363 2024-05-11 10:46:16.000000 property_lister-2.8/src/property_lister.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 10:46:16.000000 property_lister-2.8/src/property_lister.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-11 10:46:16.000000 property_lister-2.8/src/property_lister.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-11 10:46:16.000000 property_lister-2.8/src/property_lister.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-11 10:46:16.000000 property_lister-2.8/src/property_lister.egg-info/top_level.txt
```

### Comparing `property-lister-2.7/PKG-INFO` & `property_lister-2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: property-lister
-Version: 2.7
+Version: 2.8
 Summary: Extract and convert property list files from SQLite database files and from other property list files.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/property-lister
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: argparse>=1.4.0
 Requires-Dist: biplist>=1.0.3
 Requires-Dist: datetime>=5.0
 
 # Property Lister
 
 Extract and convert property list files from SQLite database files and from other property list files.
 
@@ -57,24 +56,22 @@
 
 ```bash
 pip3 install --upgrade property-lister
 ```
 
 ## Build and Install From the Source
 
-Run the following commands:
-
 ```bash
 git clone https://github.com/ivan-sincek/property-lister && cd property-lister
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/property_lister-2.7-py3-none-any.whl
+python3 -m pip install dist/property_lister-2.8-py3-none-any.whl
 ```
 
 ## Extracting and Converting
 
 Extract and convert property list files inside Cache.db unencrypted SQLite database file:
 
 ```fundamental
@@ -96,15 +93,15 @@
 Repeat the same for the app specific directories.
 
 Check my other project on how to [search for files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#3-search-for-files-and-directories) and on how to [extract sensitive data from the files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#4-inspect-files).
 
 ## Usage
 
 ```fundamental
-Property Lister v2.7 ( github.com/ivan-sincek/property-lister )
+Property Lister v2.8 ( github.com/ivan-sincek/property-lister )
 
 --- Extract from an SQLite database file ---
 Usage:   property-lister -db database -o out
 Example: property-lister -db Cache.db -o results_db
 
 --- Extract from a property list file ---
 Usage:   property-lister -pl property-list -o out
```

### Comparing `property-lister-2.7/README.md` & `property_lister-2.8/src/property_lister.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,109 +1,122 @@
-# Property Lister
-
-Extract and convert property list files from SQLite database files and from other property list files.
-
-Tested on Kali Linux v2023.4 (64-bit).
-
-Made for educational purposes. I hope it will help!
-
-## Table of Contents
-
-* [How to Install](#how-to-install)
-	* [Install plistutil](#install-plistutil)
-	* [Standard Install](#standard-install)
-	* [Build and Install From the Source](#build-and-install-from-the-source)
-* [Extracting and Converting](#extracting-and-converting)
-* [Usage](#usage)
-
-## How to Install
-
-### Install plistutil
-
-On Kali Linux, run:
-
-```bash
-apt-get -y install plistutil
-```
-
----
-
-Windows OS is not supported.
-
----
-
-On macOS, run:
-
-```bash
-brew install libplist
-```
-
-### Standard Install
-
-```bash
-pip3 install --upgrade property-lister
-```
-
-## Build and Install From the Source
-
-Run the following commands:
-
-```bash
-git clone https://github.com/ivan-sincek/property-lister && cd property-lister
-
-python3 -m pip install --upgrade build
-
-python3 -m build
-
-python3 -m pip install dist/property_lister-2.7-py3-none-any.whl
-```
-
-## Extracting and Converting
-
-Extract and convert property list files inside Cache.db unencrypted SQLite database file:
-
-```fundamental
-scp root@192.168.1.10:/var/mobile/Containers/Data/Application/YYY...YYY/Library/Caches/com.someapp.dev/Cache.db ./
-
-property-lister -db Cache.db -o results_db
-```
-
-Extract and convert property list files inside an IPA:
-
-```fundamental
-unzip someapp.ipa
-
-property-lister -db Payload -o results_db
-
-property-lister -pl Payload -o results_pl
-```
-
-Repeat the same for the app specific directories.
-
-Check my other project on how to [search for files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#3-search-for-files-and-directories) and on how to [extract sensitive data from the files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#4-inspect-files).
-
-## Usage
-
-```fundamental
-Property Lister v2.7 ( github.com/ivan-sincek/property-lister )
-
---- Extract from an SQLite database file ---
-Usage:   property-lister -db database -o out
-Example: property-lister -db Cache.db -o results_db
-
---- Extract from a property list file ---
-Usage:   property-lister -pl property-list -o out
-Example: property-lister -pl Info.plist    -o results_pl
-
-DESCRIPTION
-    Extract and convert property list files
-DATABASE
-    SQLite database file, or directory containing multiple files
-    -db, --database = Cache.db | databases | etc.
-PROPERTY LIST
-    Property list file, or directory containing multiple files
-    -pl, --property-list = Info.plist | plists | etc.
-OUT
-    Output directory
-    All extracted propery list files will be saved in this directory
-    -o, --out = results | etc.
-```
+Metadata-Version: 2.1
+Name: property-lister
+Version: 2.8
+Summary: Extract and convert property list files from SQLite database files and from other property list files.
+Author: Ivan Sincek
+Project-URL: Homepage, https://github.com/ivan-sincek/property-lister
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: biplist>=1.0.3
+Requires-Dist: datetime>=5.0
+
+# Property Lister
+
+Extract and convert property list files from SQLite database files and from other property list files.
+
+Tested on Kali Linux v2023.4 (64-bit).
+
+Made for educational purposes. I hope it will help!
+
+## Table of Contents
+
+* [How to Install](#how-to-install)
+	* [Install plistutil](#install-plistutil)
+	* [Standard Install](#standard-install)
+	* [Build and Install From the Source](#build-and-install-from-the-source)
+* [Extracting and Converting](#extracting-and-converting)
+* [Usage](#usage)
+
+## How to Install
+
+### Install plistutil
+
+On Kali Linux, run:
+
+```bash
+apt-get -y install plistutil
+```
+
+---
+
+Windows OS is not supported.
+
+---
+
+On macOS, run:
+
+```bash
+brew install libplist
+```
+
+### Standard Install
+
+```bash
+pip3 install --upgrade property-lister
+```
+
+## Build and Install From the Source
+
+```bash
+git clone https://github.com/ivan-sincek/property-lister && cd property-lister
+
+python3 -m pip install --upgrade build
+
+python3 -m build
+
+python3 -m pip install dist/property_lister-2.8-py3-none-any.whl
+```
+
+## Extracting and Converting
+
+Extract and convert property list files inside Cache.db unencrypted SQLite database file:
+
+```fundamental
+scp root@192.168.1.10:/var/mobile/Containers/Data/Application/YYY...YYY/Library/Caches/com.someapp.dev/Cache.db ./
+
+property-lister -db Cache.db -o results_db
+```
+
+Extract and convert property list files inside an IPA:
+
+```fundamental
+unzip someapp.ipa
+
+property-lister -db Payload -o results_db
+
+property-lister -pl Payload -o results_pl
+```
+
+Repeat the same for the app specific directories.
+
+Check my other project on how to [search for files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#3-search-for-files-and-directories) and on how to [extract sensitive data from the files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#4-inspect-files).
+
+## Usage
+
+```fundamental
+Property Lister v2.8 ( github.com/ivan-sincek/property-lister )
+
+--- Extract from an SQLite database file ---
+Usage:   property-lister -db database -o out
+Example: property-lister -db Cache.db -o results_db
+
+--- Extract from a property list file ---
+Usage:   property-lister -pl property-list -o out
+Example: property-lister -pl Info.plist    -o results_pl
+
+DESCRIPTION
+    Extract and convert property list files
+DATABASE
+    SQLite database file, or directory containing multiple files
+    -db, --database = Cache.db | databases | etc.
+PROPERTY LIST
+    Property list file, or directory containing multiple files
+    -pl, --property-list = Info.plist | plists | etc.
+OUT
+    Output directory
+    All extracted propery list files will be saved in this directory
+    -o, --out = results | etc.
+```
```

### Comparing `property-lister-2.7/pyproject.toml` & `property_lister-2.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "property-lister"
-version = "2.7"
-authors = [{ name = "Ivan Sincek" }]
-description = "Extract and convert property list files from SQLite database files and from other property list files."
-readme = "README.md"
-requires-python = ">=3.6"
-classifiers = [
-	"Programming Language :: Python :: 3",
-	"License :: OSI Approved :: MIT License",
-	"Operating System :: POSIX :: Linux"
-]
-dependencies = ["argparse>=1.4.0", "biplist>=1.0.3", "datetime>=5.0"]
-
-[project.urls]
-"Homepage" = "https://github.com/ivan-sincek/property-lister"
-
-[project.scripts]
-property-lister = "property_lister.property_lister:main"
-
-[tool.setuptools.packages.find]
-where = ["src"]
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "property-lister"
+version = "2.8"
+authors = [{ name = "Ivan Sincek" }]
+description = "Extract and convert property list files from SQLite database files and from other property list files."
+readme = "README.md"
+requires-python = ">=3.6"
+classifiers = [
+	"Programming Language :: Python :: 3",
+	"License :: OSI Approved :: MIT License",
+	"Operating System :: POSIX :: Linux"
+]
+dependencies = ["biplist>=1.0.3", "datetime>=5.0"]
+
+[project.urls]
+"Homepage" = "https://github.com/ivan-sincek/property-lister"
+
+[project.scripts]
+property-lister = "property_lister.property_lister:main"
+
+[tool.setuptools.packages.find]
+where = ["src"]
```

### Comparing `property-lister-2.7/src/property_lister/property_lister.py` & `property_lister-2.8/src/property_lister/property_lister.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,265 +1,265 @@
-#!/usr/bin/env python3
-
-import argparse, binascii, biplist, datetime, os, re, shutil, sqlite3, subprocess, sys
-
-# ----------------------------------------
-
-class Stopwatch:
-
-	def __init__(self):
-		self.__start = datetime.datetime.now()
-
-	def stop(self):
-		self.__end = datetime.datetime.now()
-		print(("Script has finished in {0}").format(self.__end - self.__start))
-
-stopwatch = Stopwatch()
-
-# ----------------------------------------
-
-def check_duplicate(file):
-	array = os.path.splitext(file)
-	count = 0
-	filename = file
-	while os.path.exists(filename):
-		count += 1
-		filename = ("{0} ({1}){2}").format(array[0], count, array[1])
-	return filename
-
-def build(out, file, ext, replace = False, count = None):
-	if out:
-		file = os.path.join(out, os.path.basename(file))
-	if ext:
-		if replace or file.lower().endswith(ext):
-			file = os.path.splitext(file)[0] + ext # NOTE: Normalize.
-		else:
-			file = file + ext # NOTE: Normalize.
-	if count:
-		file = os.path.splitext(file)[0] + "." + str(count) + ext
-	return check_duplicate(file)
-
-def read_database(file):
-	tmp = ""
-	db = None
-	try:
-		db = sqlite3.connect(file)
-		tmp = ("\n").join(db.iterdump())
-	except sqlite3.DatabaseError:
-		pass
-	finally:
-		if db:
-			db.close()
-	return tmp
-
-ext = {"txt": ".txt", "blob": ".blob", "plist": ".plist", "xml": ".plist.xml"}
-
-# database --> full path (external)
-def dump(database, out):
-	for db in database:
-		count = 0
-		data = read_database(db)
-		if data:
-			db = build(out, db, ext["txt"])
-			open(db, "w").write(data)
-			blobs = re.findall(r"(?<=,X')[\w\d]+", data, re.MULTILINE | re.IGNORECASE)
-			if blobs:
-				for blob in blobs:
-					count += 1
-					new = build(out, db, ext["blob"], True, count)
-					open(new, "wb").write(binascii.unhexlify(blob))
-					extract(new, out, True)
-
-def run(command):
-	return subprocess.run((" ").join(command), shell = True, stdout = subprocess.PIPE, stderr = subprocess.STDOUT).stdout
-
-# file --> full path (external/internal)
-def extract(file, out, internal):
-	data = run(["plistutil", "-f", "xml", "-i", ("\"{0}\"").format(file)])
-	if re.search(rb"\<plist[\s\S]+\<\/plist\>", data, re.MULTILINE | re.IGNORECASE):
-		open(build(out, file, ext["xml"], True) if internal else build(out, build(out, file, ext["plist"]), ext["xml"], True), "wb").write(data)
-		try:
-			data = biplist.readPlist(file)
-			if isinstance(data, dict):
-				count = 0
-				for key in data:
-					if isinstance(data[key], biplist.Data):
-						string = biplist.readPlistFromString(data[key]) # NOTE: Extract a property list file from a property list file.
-						if string:
-							count += 1
-							new = build(out, file, ext["plist"], internal, count)
-							biplist.writePlist(string, new)
-							extract(new, out, True)
-		except (biplist.InvalidPlistException, biplist.NotBinaryPlistException):
-			pass
-		if internal:
-			os.remove(file)
-
-# ----------------------------------------
-
-class PropertyLister:
-
-	def __init__(self, database, property_list, out):
-		self.__database      = database
-		self.__property_list = property_list
-		self.__out           = out
-
-	def run (self):
-		print("Extracting...")
-		if self.__database:
-			dump(self.__database, self.__out)
-		elif self.__property_list:
-			for file in self.__property_list:
-				extract(file, self.__out, False)
-		return len(os.listdir(self.__out))
-
-# ----------------------------------------
-
-class MyArgParser(argparse.ArgumentParser):
-
-	def print_help(self):
-		print("Property Lister v2.7 ( github.com/ivan-sincek/property-lister )")
-		print("")
-		print("--- Extract from an SQLite database file ---")
-		print("Usage:   property-lister -db database -o out")
-		print("Example: property-lister -db Cache.db -o results_db")
-		print("")
-		print("--- Extract from a property list file ---")
-		print("Usage:   property-lister -pl property-list -o out")
-		print("Example: property-lister -pl Info.plist    -o results_pl")
-		print("")
-		print("DESCRIPTION")
-		print("    Extract and convert property list files")
-		print("DATABASE")
-		print("    SQLite database file, or directory containing multiple files")
-		print("    -db, --database = Cache.db | databases | etc.")
-		print("PROPERTY LIST")
-		print("    Property list file, or directory containing multiple files")
-		print("    -pl, --property-list = Info.plist | plists | etc.")
-		print("OUT")
-		print("    Output directory")
-		print("    All extracted propery list files will be saved in this directory")
-		print("    -o, --out = results | etc.")
-
-	def error(self, message):
-		if len(sys.argv) > 1:
-			print("Missing a mandatory option (-db, -o) or (-pl, -o)")
-		else:
-			self.print_help()
-		exit()
-
-class Validate:
-
-	def __init__(self):
-		self.__proceed = True
-		self.__parser  = MyArgParser()
-		group = self.__parser.add_mutually_exclusive_group(  required = True                           )
-		group.add_argument(        "-db", "--database"     , required = False, type = str, default = "")
-		group.add_argument(        "-pl", "--property-list", required = False, type = str, default = "")
-		self.__parser.add_argument("-o" , "--out"          , required = True , type = str, default = "")
-
-	def run(self):
-		self.__args               = self.__parser.parse_args()
-		self.__args.database      = self.__parse_directory(self.__args.database)      if self.__args.database      else []
-		self.__args.property_list = self.__parse_directory(self.__args.property_list) if self.__args.property_list else []
-		self.__args.out           = self.__parse_out(self.__args.out)                 # required
-		self.__args               = vars(self.__args)
-		return self.__proceed
-
-	def get_arg(self, key):
-		return self.__args[key]
-
-	def __error(self, msg):
-		self.__proceed = False
-		self.__print_error(msg)
-
-	def __print_error(self, msg):
-		print(("ERROR: {0}").format(msg))
-
-	def __parse_directory(self, value):
-		tmp = []
-		if not os.path.exists(value):
-			self.__error("Directory containing files, or a single file does not exists")
-		elif os.path.isdir(value):
-			tmp = self.__validate_directory_files(value)
-			if not tmp:
-				self.__error("No valid files were found")
-		else:
-			if not os.access(value, os.R_OK):
-				self.__error("File does not have read permission")
-			elif not os.stat(value).st_size > 0:
-				self.__error("File is empty")
-			else:
-				tmp = [value]
-		return tmp
-
-	def __validate_directory_files(self, directory):
-		tmp = []
-		for path, dirs, files in os.walk(directory):
-			for file in files:
-				file = os.path.join(path, file)
-				if os.path.isfile(file) and os.access(file, os.R_OK) and os.stat(file).st_size > 0:
-					tmp.append(file)
-		return tmp
-
-	def __parse_out(self, value):
-		if self.__proceed:
-			self.__proceed = False
-			overwrite = "yes"
-			if os.path.exists(value):
-				print(("'{0}' directory already exists").format(value))
-				overwrite = input("Overwrite the output directory (yes): ")
-			if overwrite.lower() == "yes" and self.remove_directory(value):
-				self.__proceed = self.__create_directory(value)
-		return value
-
-	def remove_directory(self, directory):
-		success = True
-		try:
-			if os.path.exists(directory):
-				shutil.rmtree(directory)
-		except Exception:
-			success = False
-			self.__error(("Cannot remove '{0}' related directories/subdirectories and/or files").format(directory))
-		return success
-
-	def __create_directory(self, directory):
-		success = True
-		try:
-			if not os.path.exists(directory):
-				os.mkdir(directory)
-		except Exception:
-			success = False
-			self.__error(("Cannot create '{0}' directory").format(directory))
-		return success
-
-# ----------------------------------------
-
-def main():
-	validate = Validate()
-	if validate.run():
-		print("##########################################################################")
-		print("#                                                                        #")
-		print("#                          Property Lister v2.7                          #")
-		print("#                                     by Ivan Sincek                     #")
-		print("#                                                                        #")
-		print("# Extract and convert property list files.                               #")
-		print("# GitHub repository at github.com/ivan-sincek/property-lister.           #")
-		print("# Feel free to donate ETH at 0xbc00e800f29524AD8b0968CEBEAD4cD5C5c1f105. #")
-		print("#                                                                        #")
-		print("##########################################################################")
-		out = validate.get_arg("out")
-		property_lister = PropertyLister(
-			validate.get_arg("database"),
-			validate.get_arg("property_list"),
-			validate.get_arg("out")
-		)
-		length = property_lister.run()
-		if length <= 0:
-			print("No results")
-			validate.remove_directory(out)
-		else:
-			print(("Created files: {0}").format(length))
-		stopwatch.stop()
-
-if __name__ == "__main__":
-	main()
+#!/usr/bin/env python3
+
+import argparse, binascii, biplist, datetime, os, re, shutil, sqlite3, subprocess, sys
+
+# ----------------------------------------
+
+class Stopwatch:
+
+	def __init__(self):
+		self.__start = datetime.datetime.now()
+
+	def stop(self):
+		self.__end = datetime.datetime.now()
+		print(("Script has finished in {0}").format(self.__end - self.__start))
+
+stopwatch = Stopwatch()
+
+# ----------------------------------------
+
+def check_duplicate(file):
+	array = os.path.splitext(file)
+	count = 0
+	filename = file
+	while os.path.exists(filename):
+		count += 1
+		filename = ("{0} ({1}){2}").format(array[0], count, array[1])
+	return filename
+
+def build(out, file, ext, replace = False, count = None):
+	if out:
+		file = os.path.join(out, os.path.basename(file))
+	if ext:
+		if replace or file.lower().endswith(ext):
+			file = os.path.splitext(file)[0] + ext # NOTE: Normalize.
+		else:
+			file = file + ext # NOTE: Normalize.
+	if count:
+		file = os.path.splitext(file)[0] + "." + str(count) + ext
+	return check_duplicate(file)
+
+def read_database(file):
+	tmp = ""
+	db = None
+	try:
+		db = sqlite3.connect(file)
+		tmp = ("\n").join(db.iterdump())
+	except sqlite3.DatabaseError:
+		pass
+	finally:
+		if db:
+			db.close()
+	return tmp
+
+ext = {"txt": ".txt", "blob": ".blob", "plist": ".plist", "xml": ".plist.xml"}
+
+# database --> full path (external)
+def dump(database, out):
+	for db in database:
+		count = 0
+		data = read_database(db)
+		if data:
+			db = build(out, db, ext["txt"])
+			open(db, "w").write(data)
+			blobs = re.findall(r"(?<=,X')[\w\d]+", data, re.MULTILINE | re.IGNORECASE)
+			if blobs:
+				for blob in blobs:
+					count += 1
+					new = build(out, db, ext["blob"], True, count)
+					open(new, "wb").write(binascii.unhexlify(blob))
+					extract(new, out, True)
+
+def run(command):
+	return subprocess.run((" ").join(command), shell = True, stdout = subprocess.PIPE, stderr = subprocess.STDOUT).stdout
+
+# file --> full path (external/internal)
+def extract(file, out, internal):
+	data = run(["plistutil", "-f", "xml", "-i", ("\"{0}\"").format(file)])
+	if re.search(rb"\<plist[\s\S]+\<\/plist\>", data, re.MULTILINE | re.IGNORECASE):
+		open(build(out, file, ext["xml"], True) if internal else build(out, build(out, file, ext["plist"]), ext["xml"], True), "wb").write(data)
+		try:
+			data = biplist.readPlist(file)
+			if isinstance(data, dict):
+				count = 0
+				for key in data:
+					if isinstance(data[key], biplist.Data):
+						string = biplist.readPlistFromString(data[key]) # NOTE: Extract a property list file from a property list file.
+						if string:
+							count += 1
+							new = build(out, file, ext["plist"], internal, count)
+							biplist.writePlist(string, new)
+							extract(new, out, True)
+		except (biplist.InvalidPlistException, biplist.NotBinaryPlistException):
+			pass
+		if internal:
+			os.remove(file)
+
+# ----------------------------------------
+
+class PropertyLister:
+
+	def __init__(self, database, property_list, out):
+		self.__database      = database
+		self.__property_list = property_list
+		self.__out           = out
+
+	def run (self):
+		print("Extracting...")
+		if self.__database:
+			dump(self.__database, self.__out)
+		elif self.__property_list:
+			for file in self.__property_list:
+				extract(file, self.__out, False)
+		return len(os.listdir(self.__out))
+
+# ----------------------------------------
+
+class MyArgParser(argparse.ArgumentParser):
+
+	def print_help(self):
+		print("Property Lister v2.8 ( github.com/ivan-sincek/property-lister )")
+		print("")
+		print("--- Extract from an SQLite database file ---")
+		print("Usage:   property-lister -db database -o out")
+		print("Example: property-lister -db Cache.db -o results_db")
+		print("")
+		print("--- Extract from a property list file ---")
+		print("Usage:   property-lister -pl property-list -o out")
+		print("Example: property-lister -pl Info.plist    -o results_pl")
+		print("")
+		print("DESCRIPTION")
+		print("    Extract and convert property list files")
+		print("DATABASE")
+		print("    SQLite database file, or directory containing multiple files")
+		print("    -db, --database = Cache.db | databases | etc.")
+		print("PROPERTY LIST")
+		print("    Property list file, or directory containing multiple files")
+		print("    -pl, --property-list = Info.plist | plists | etc.")
+		print("OUT")
+		print("    Output directory")
+		print("    All extracted propery list files will be saved in this directory")
+		print("    -o, --out = results | etc.")
+
+	def error(self, message):
+		if len(sys.argv) > 1:
+			print("Missing a mandatory option (-db, -o) or (-pl, -o)")
+		else:
+			self.print_help()
+		exit()
+
+class Validate:
+
+	def __init__(self):
+		self.__proceed = True
+		self.__parser  = MyArgParser()
+		group = self.__parser.add_mutually_exclusive_group(  required = True                           )
+		group.add_argument(        "-db", "--database"     , required = False, type = str, default = "")
+		group.add_argument(        "-pl", "--property-list", required = False, type = str, default = "")
+		self.__parser.add_argument("-o" , "--out"          , required = True , type = str, default = "")
+
+	def run(self):
+		self.__args               = self.__parser.parse_args()
+		self.__args.database      = self.__parse_directory(self.__args.database)      if self.__args.database      else []
+		self.__args.property_list = self.__parse_directory(self.__args.property_list) if self.__args.property_list else []
+		self.__args.out           = self.__parse_out(self.__args.out)                 # required
+		self.__args               = vars(self.__args)
+		return self.__proceed
+
+	def get_arg(self, key):
+		return self.__args[key]
+
+	def __error(self, msg):
+		self.__proceed = False
+		self.__print_error(msg)
+
+	def __print_error(self, msg):
+		print(("ERROR: {0}").format(msg))
+
+	def __parse_directory(self, value):
+		tmp = []
+		if not os.path.exists(value):
+			self.__error("Directory containing files, or a single file does not exists")
+		elif os.path.isdir(value):
+			tmp = self.__validate_directory_files(value)
+			if not tmp:
+				self.__error("No valid files were found")
+		else:
+			if not os.access(value, os.R_OK):
+				self.__error("File does not have read permission")
+			elif not os.stat(value).st_size > 0:
+				self.__error("File is empty")
+			else:
+				tmp = [value]
+		return tmp
+
+	def __validate_directory_files(self, directory):
+		tmp = []
+		for path, dirs, files in os.walk(directory):
+			for file in files:
+				file = os.path.join(path, file)
+				if os.path.isfile(file) and os.access(file, os.R_OK) and os.stat(file).st_size > 0:
+					tmp.append(file)
+		return tmp
+
+	def __parse_out(self, value):
+		if self.__proceed:
+			self.__proceed = False
+			overwrite = "yes"
+			if os.path.exists(value):
+				print(("'{0}' directory already exists").format(value))
+				overwrite = input("Overwrite the output directory (yes): ")
+			if overwrite.lower() == "yes" and self.remove_directory(value):
+				self.__proceed = self.__create_directory(value)
+		return value
+
+	def remove_directory(self, directory):
+		success = True
+		try:
+			if os.path.exists(directory):
+				shutil.rmtree(directory)
+		except Exception:
+			success = False
+			self.__error(("Cannot remove '{0}' related directories/subdirectories and/or files").format(directory))
+		return success
+
+	def __create_directory(self, directory):
+		success = True
+		try:
+			if not os.path.exists(directory):
+				os.mkdir(directory)
+		except Exception:
+			success = False
+			self.__error(("Cannot create '{0}' directory").format(directory))
+		return success
+
+# ----------------------------------------
+
+def main():
+	validate = Validate()
+	if validate.run():
+		print("##########################################################################")
+		print("#                                                                        #")
+		print("#                          Property Lister v2.8                          #")
+		print("#                                     by Ivan Sincek                     #")
+		print("#                                                                        #")
+		print("# Extract and convert property list files.                               #")
+		print("# GitHub repository at github.com/ivan-sincek/property-lister.           #")
+		print("# Feel free to donate ETH at 0xbc00e800f29524AD8b0968CEBEAD4cD5C5c1f105. #")
+		print("#                                                                        #")
+		print("##########################################################################")
+		out = validate.get_arg("out")
+		property_lister = PropertyLister(
+			validate.get_arg("database"),
+			validate.get_arg("property_list"),
+			validate.get_arg("out")
+		)
+		length = property_lister.run()
+		if length <= 0:
+			print("No results")
+			validate.remove_directory(out)
+		else:
+			print(("Created files: {0}").format(length))
+		stopwatch.stop()
+
+if __name__ == "__main__":
+	main()
```

### Comparing `property-lister-2.7/src/property_lister.egg-info/PKG-INFO` & `property_lister-2.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: property-lister
-Version: 2.7
-Summary: Extract and convert property list files from SQLite database files and from other property list files.
-Author: Ivan Sincek
-Project-URL: Homepage, https://github.com/ivan-sincek/property-lister
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: argparse>=1.4.0
-Requires-Dist: biplist>=1.0.3
-Requires-Dist: datetime>=5.0
-
 # Property Lister
 
 Extract and convert property list files from SQLite database files and from other property list files.
 
 Tested on Kali Linux v2023.4 (64-bit).
 
 Made for educational purposes. I hope it will help!
@@ -57,24 +41,22 @@
 
 ```bash
 pip3 install --upgrade property-lister
 ```
 
 ## Build and Install From the Source
 
-Run the following commands:
-
 ```bash
 git clone https://github.com/ivan-sincek/property-lister && cd property-lister
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/property_lister-2.7-py3-none-any.whl
+python3 -m pip install dist/property_lister-2.8-py3-none-any.whl
 ```
 
 ## Extracting and Converting
 
 Extract and convert property list files inside Cache.db unencrypted SQLite database file:
 
 ```fundamental
@@ -96,15 +78,15 @@
 Repeat the same for the app specific directories.
 
 Check my other project on how to [search for files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#3-search-for-files-and-directories) and on how to [extract sensitive data from the files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#4-inspect-files).
 
 ## Usage
 
 ```fundamental
-Property Lister v2.7 ( github.com/ivan-sincek/property-lister )
+Property Lister v2.8 ( github.com/ivan-sincek/property-lister )
 
 --- Extract from an SQLite database file ---
 Usage:   property-lister -db database -o out
 Example: property-lister -db Cache.db -o results_db
 
 --- Extract from a property list file ---
 Usage:   property-lister -pl property-list -o out
```

