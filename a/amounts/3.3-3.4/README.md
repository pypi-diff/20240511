# Comparing `tmp/amounts-3.3.tar.gz` & `tmp/amounts-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amounts-3.3.tar", last modified: Sat Dec 30 01:23:24 2023, max compression
+gzip compressed data, was "amounts-3.4.tar", last modified: Sat May 11 10:57:42 2024, max compression
```

## Comparing `amounts-3.3.tar` & `amounts-3.4.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxrwx---   0 root         (0) vboxsf     (141)        0 2023-12-30 01:23:26.749534 amounts-3.3/
--rwxrwx---   0 root         (0) vboxsf     (141)     1069 2023-12-25 22:42:18.000000 amounts-3.3/LICENSE
--rwxrwx---   0 root         (0) vboxsf     (141)       28 2023-12-25 22:42:18.000000 amounts-3.3/MANIFEST.in
--rwxrwx---   0 root         (0) vboxsf     (141)     6115 2023-12-30 01:23:26.742857 amounts-3.3/PKG-INFO
--rwxrwx---   0 root         (0) vboxsf     (141)     5645 2023-12-30 01:14:20.000000 amounts-3.3/README.md
--rwxrwx---   0 root         (0) vboxsf     (141)      701 2023-12-29 21:46:29.000000 amounts-3.3/pyproject.toml
--rwxrwx---   0 root         (0) vboxsf     (141)       38 2023-12-30 01:23:26.750046 amounts-3.3/setup.cfg
-drwxrwx---   0 root         (0) vboxsf     (141)        0 2023-12-30 01:23:26.507948 amounts-3.3/src/
-drwxrwx---   0 root         (0) vboxsf     (141)        0 2023-12-30 01:23:26.566223 amounts-3.3/src/amounts/
--rwxrwx---   0 root         (0) vboxsf     (141)        0 2023-12-25 22:42:18.000000 amounts-3.3/src/amounts/__init__.py
--rwxrwx---   0 root         (0) vboxsf     (141)    13245 2023-12-30 01:14:00.000000 amounts-3.3/src/amounts/amounts.py
-drwxrwx---   0 root         (0) vboxsf     (141)        0 2023-12-30 01:23:26.737742 amounts-3.3/src/amounts.egg-info/
--rwxrwx---   0 root         (0) vboxsf     (141)     6115 2023-12-30 01:23:26.000000 amounts-3.3/src/amounts.egg-info/PKG-INFO
--rwxrwx---   0 root         (0) vboxsf     (141)      569 2023-12-30 01:23:26.000000 amounts-3.3/src/amounts.egg-info/SOURCES.txt
--rwxrwx---   0 root         (0) vboxsf     (141)        1 2023-12-30 01:23:26.000000 amounts-3.3/src/amounts.egg-info/dependency_links.txt
--rwxrwx---   0 root         (0) vboxsf     (141)       49 2023-12-30 01:23:26.000000 amounts-3.3/src/amounts.egg-info/entry_points.txt
--rwxrwx---   0 root         (0) vboxsf     (141)       16 2023-12-30 01:23:26.000000 amounts-3.3/src/amounts.egg-info/requires.txt
--rwxrwx---   0 root         (0) vboxsf     (141)       18 2023-12-30 01:23:26.000000 amounts-3.3/src/amounts.egg-info/top_level.txt
-drwxrwx---   0 root         (0) vboxsf     (141)        0 2023-12-30 01:23:26.724370 amounts-3.3/src/wordlists/
--rwxrwx---   0 root         (0) vboxsf     (141)     5080 2023-12-25 22:42:18.000000 amounts-3.3/src/wordlists/all.txt
--rwxrwx---   0 root         (0) vboxsf     (141)     2120 2023-12-25 22:42:18.000000 amounts-3.3/src/wordlists/hundred.txt
--rwxrwx---   0 root         (0) vboxsf     (141)     2322 2023-12-25 22:42:18.000000 amounts-3.3/src/wordlists/hundred_thousand.txt
--rwxrwx---   0 root         (0) vboxsf     (141)     2386 2023-12-25 22:42:18.000000 amounts-3.3/src/wordlists/milion.txt
--rwxrwx---   0 root         (0) vboxsf     (141)     1992 2023-12-25 22:42:18.000000 amounts-3.3/src/wordlists/one.txt
--rwxrwx---   0 root         (0) vboxsf     (141)     2061 2023-12-25 22:42:18.000000 amounts-3.3/src/wordlists/ten.txt
--rwxrwx---   0 root         (0) vboxsf     (141)     2260 2023-12-25 22:42:18.000000 amounts-3.3/src/wordlists/ten_thousand.txt
--rwxrwx---   0 root         (0) vboxsf     (141)     2197 2023-12-25 22:42:18.000000 amounts-3.3/src/wordlists/thousand.txt
--rwxrwx---   0 root         (0) vboxsf     (141)     1981 2023-12-25 22:42:18.000000 amounts-3.3/src/wordlists/zero.txt
--rwxrwx---   0 root         (0) vboxsf     (141)     2145 2023-12-25 22:42:18.000000 amounts-3.3/src/wordlists/zero_point_one.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 10:57:42.521397 amounts-3.4/
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-05-11 10:56:04.000000 amounts-3.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-05-11 10:56:04.000000 amounts-3.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6119 2024-05-11 10:57:42.521397 amounts-3.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5680 2024-05-11 10:57:09.000000 amounts-3.4/README.md
+-rw-r--r--   0 root         (0) root         (0)      684 2024-05-11 10:57:13.000000 amounts-3.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-11 10:57:42.521397 amounts-3.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 10:57:42.521397 amounts-3.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 10:57:42.521397 amounts-3.4/src/amounts/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 10:56:04.000000 amounts-3.4/src/amounts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13222 2024-05-11 10:57:25.000000 amounts-3.4/src/amounts/amounts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 10:57:42.521397 amounts-3.4/src/amounts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6119 2024-05-11 10:57:42.000000 amounts-3.4/src/amounts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      535 2024-05-11 10:57:42.000000 amounts-3.4/src/amounts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 10:57:42.000000 amounts-3.4/src/amounts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2024-05-11 10:57:42.000000 amounts-3.4/src/amounts.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-05-11 10:57:42.000000 amounts-3.4/src/amounts.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 10:57:42.521397 amounts-3.4/src/wordlists/
+-rw-r--r--   0 root         (0) root         (0)     5080 2024-05-11 10:56:04.000000 amounts-3.4/src/wordlists/all.txt
+-rw-r--r--   0 root         (0) root         (0)     2120 2024-05-11 10:56:04.000000 amounts-3.4/src/wordlists/hundred.txt
+-rw-r--r--   0 root         (0) root         (0)     2322 2024-05-11 10:56:04.000000 amounts-3.4/src/wordlists/hundred_thousand.txt
+-rw-r--r--   0 root         (0) root         (0)     2386 2024-05-11 10:56:04.000000 amounts-3.4/src/wordlists/milion.txt
+-rw-r--r--   0 root         (0) root         (0)     1992 2024-05-11 10:56:04.000000 amounts-3.4/src/wordlists/one.txt
+-rw-r--r--   0 root         (0) root         (0)     2061 2024-05-11 10:56:04.000000 amounts-3.4/src/wordlists/ten.txt
+-rw-r--r--   0 root         (0) root         (0)     2260 2024-05-11 10:56:04.000000 amounts-3.4/src/wordlists/ten_thousand.txt
+-rw-r--r--   0 root         (0) root         (0)     2197 2024-05-11 10:56:04.000000 amounts-3.4/src/wordlists/thousand.txt
+-rw-r--r--   0 root         (0) root         (0)     1981 2024-05-11 10:56:04.000000 amounts-3.4/src/wordlists/zero.txt
+-rw-r--r--   0 root         (0) root         (0)     2145 2024-05-11 10:56:04.000000 amounts-3.4/src/wordlists/zero_point_one.txt
```

### Comparing `amounts-3.3/LICENSE` & `amounts-3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `amounts-3.3/PKG-INFO` & `amounts-3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: amounts
-Version: 3.3
+Version: 3.4
 Summary: Generate a wordlist to fuzz amounts or any other numerical values.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/amounts
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: argparse>=1.4.0
 
 # Amounts
 
 Generate a wordlist to fuzz amounts or any other numerical values. Based on [Common Security Issues in Financially-Oriented Web Applications](https://research.nccgroup.com/wp-content/uploads/2020/07/common_security_issues_in_financially-orientated_web.pdf).
 
 Bypass minimum and maximum restrictions, cause an unintended behavior and errors, etc.
 
@@ -43,36 +42,37 @@
 Tested on Kali Linux v2023.4 (64-bit).
 
 Made for educational purposes. I hope it will help!
 
 ## Table of Contents
 
 * [How to Install](#how-to-install)
-* [How to Build and Install Manually](#how-to-build-and-install-manually)
+	* [Standard Install](#standard-install)
+	* [Build and Install From the Source](#build-and-install-from-the-source)
 * [Generated Amounts](#generated-amounts)
 * [Usage](#usage)
 
 ## How to Install
 
+### Standard Install
+
 ```fundamental
 pip3 install --upgrade amounts
 ```
 
-## How to Build and Install Manually
-
-Run the following commands:
+## Build and Install From the Source
 
 ```fundamental
 git clone https://github.com/ivan-sincek/amounts && cd amounts
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/amounts-3.3-py3-none-any.whl
+python3 -m pip install dist/amounts-3.4-py3-none-any.whl
 ```
 
 ## Generated Amounts
 
 ```fundamental
 amounts -min 1 -max 10000 -mid 2200 -o amounts.txt
 ```
@@ -167,15 +167,15 @@
 -999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999
 -99999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999
 ```
 
 ## Usage
 
 ```fundamental
-Amounts v3.3 ( github.com/ivan-sincek/amounts )
+Amounts v3.4 ( github.com/ivan-sincek/amounts )
 
 --- Generate a wordlist from an amount range ---
 Usage:   python3 amounts.py -min minimum -max maximum -mid middle -o out         [-q quotes]
 Example: python3 amounts.py -min 1       -max 1000    -mid 20     -o amounts.txt [-q double]
 
 --- Generate a wordlist from a single amount ---
 Usage:   python3 amounts.py -mid middle -o out         [-q quotes]
```

### Comparing `amounts-3.3/README.md` & `amounts-3.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -29,36 +29,37 @@
 Tested on Kali Linux v2023.4 (64-bit).
 
 Made for educational purposes. I hope it will help!
 
 ## Table of Contents
 
 * [How to Install](#how-to-install)
-* [How to Build and Install Manually](#how-to-build-and-install-manually)
+	* [Standard Install](#standard-install)
+	* [Build and Install From the Source](#build-and-install-from-the-source)
 * [Generated Amounts](#generated-amounts)
 * [Usage](#usage)
 
 ## How to Install
 
+### Standard Install
+
 ```fundamental
 pip3 install --upgrade amounts
 ```
 
-## How to Build and Install Manually
-
-Run the following commands:
+## Build and Install From the Source
 
 ```fundamental
 git clone https://github.com/ivan-sincek/amounts && cd amounts
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/amounts-3.3-py3-none-any.whl
+python3 -m pip install dist/amounts-3.4-py3-none-any.whl
 ```
 
 ## Generated Amounts
 
 ```fundamental
 amounts -min 1 -max 10000 -mid 2200 -o amounts.txt
 ```
@@ -153,15 +154,15 @@
 -999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999
 -99999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999
 ```
 
 ## Usage
 
 ```fundamental
-Amounts v3.3 ( github.com/ivan-sincek/amounts )
+Amounts v3.4 ( github.com/ivan-sincek/amounts )
 
 --- Generate a wordlist from an amount range ---
 Usage:   python3 amounts.py -min minimum -max maximum -mid middle -o out         [-q quotes]
 Example: python3 amounts.py -min 1       -max 1000    -mid 20     -o amounts.txt [-q double]
 
 --- Generate a wordlist from a single amount ---
 Usage:   python3 amounts.py -mid middle -o out         [-q quotes]
```

### Comparing `amounts-3.3/pyproject.toml` & `amounts-3.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "amounts"
-version = "3.3"
+version = "3.4"
 authors = [{ name = "Ivan Sincek" }]
 description = "Generate a wordlist to fuzz amounts or any other numerical values."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
 	"Operating System :: OS Independent"
 ]
-dependencies = ["argparse>=1.4.0"]
+dependencies = []
 
 [project.urls]
 "Homepage" = "https://github.com/ivan-sincek/amounts"
 
 [project.scripts]
 amounts = "amounts.amounts:main"
```

### Comparing `amounts-3.3/src/amounts/amounts.py` & `amounts-3.4/src/amounts/amounts.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,15 +272,15 @@
 		return unique(self.__amounts)
 
 # ----------------------------------------
 
 class MyArgParser(argparse.ArgumentParser):
 
 	def print_help(self):
-		print("Amounts v3.3 ( github.com/ivan-sincek/amounts )")
+		print("Amounts v3.4 ( github.com/ivan-sincek/amounts )")
 		print("")
 		print("--- Generate a wordlist from an amount range ---")
 		print("Usage:   python3 amounts.py -min minimum -max maximum -mid middle -o out         [-q quotes]")
 		print("Example: python3 amounts.py -min 1       -max 1000    -mid 20     -o amounts.txt [-q double]")
 		print("")
 		print("--- Generate a wordlist from a single amount ---")
 		print("Usage:   python3 amounts.py -mid middle -o out         [-q quotes]")
@@ -327,15 +327,15 @@
 		self.__parser.add_argument("-q"  , "--quotes" , required = False, type = str.lower, default = "")
 
 	def run(self):
 		self.__args = self.__parser.parse_args()
 		self.__args.middle  = self.__parse_digit(self.__args.middle, "middle")   # required
 		self.__args.minimum = self.__parse_digit(self.__args.minimum, "minimum") if self.__args.minimum else self.__args.middle
 		self.__args.maximum = self.__parse_digit(self.__args.maximum, "maximum") if self.__args.maximum else self.__args.middle
-		self.__args.quotes  = self.__parse_qoutes(self.__args.quotes)            if self.__args.quotes else self.__get_quote("original")
+		self.__args.quotes  = self.__parse_qoutes(self.__args.quotes)            if self.__args.quotes else self.__get_quotes("original")
 		self.__args         = vars(self.__args)
 		return self.__proceed
 
 	def get_arg(self, key):
 		return self.__args[key]
 
 	def __error(self, msg):
@@ -364,22 +364,21 @@
 			entry = entry.strip()
 			if not entry:
 				continue
 			elif entry not in ["original", "single", "double", "backtick", "all"]:
 				self.__error("Supported quotes are 'original', 'single', 'double', 'backtick', or 'all'")
 				break
 			elif entry == "all":
-				tmp.clear()
-				tmp.extend(self.__get_quote(entry))
+				tmp = self.__get_quotes(entry)
 				break
 			else:
-				tmp.extend(self.__get_quote(entry))
+				tmp += self.__get_quotes(entry)
 		return unique(tmp)
 
-	def __get_quote(self, value):
+	def __get_quotes(self, value):
 		if value == "original":
 			return [""]
 		elif value == "single":
 			return ["\x27"]
 		elif value == "double":
 			return ["\x22"]
 		elif value == "backtick":
@@ -390,15 +389,15 @@
 # ----------------------------------------
 
 def main():
 	validate = Validate()
 	if validate.run():
 		print("##########################################################################")
 		print("#                                                                        #")
-		print("#                              Amounts v3.3                              #")
+		print("#                              Amounts v3.4                              #")
 		print("#                                 by Ivan Sincek                         #")
 		print("#                                                                        #")
 		print("# Generate a wordlist to fuzz amounts or any other numerical values.     #")
 		print("# GitHub repository at github.com/ivan-sincek/amounts.                   #")
 		print("# Feel free to donate ETH at 0xbc00e800f29524AD8b0968CEBEAD4cD5C5c1f105. #")
 		print("#                                                                        #")
 		print("##########################################################################")
```

### Comparing `amounts-3.3/src/amounts.egg-info/PKG-INFO` & `amounts-3.4/src/amounts.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: amounts
-Version: 3.3
+Version: 3.4
 Summary: Generate a wordlist to fuzz amounts or any other numerical values.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/amounts
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: argparse>=1.4.0
 
 # Amounts
 
 Generate a wordlist to fuzz amounts or any other numerical values. Based on [Common Security Issues in Financially-Oriented Web Applications](https://research.nccgroup.com/wp-content/uploads/2020/07/common_security_issues_in_financially-orientated_web.pdf).
 
 Bypass minimum and maximum restrictions, cause an unintended behavior and errors, etc.
 
@@ -43,36 +42,37 @@
 Tested on Kali Linux v2023.4 (64-bit).
 
 Made for educational purposes. I hope it will help!
 
 ## Table of Contents
 
 * [How to Install](#how-to-install)
-* [How to Build and Install Manually](#how-to-build-and-install-manually)
+	* [Standard Install](#standard-install)
+	* [Build and Install From the Source](#build-and-install-from-the-source)
 * [Generated Amounts](#generated-amounts)
 * [Usage](#usage)
 
 ## How to Install
 
+### Standard Install
+
 ```fundamental
 pip3 install --upgrade amounts
 ```
 
-## How to Build and Install Manually
-
-Run the following commands:
+## Build and Install From the Source
 
 ```fundamental
 git clone https://github.com/ivan-sincek/amounts && cd amounts
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/amounts-3.3-py3-none-any.whl
+python3 -m pip install dist/amounts-3.4-py3-none-any.whl
 ```
 
 ## Generated Amounts
 
 ```fundamental
 amounts -min 1 -max 10000 -mid 2200 -o amounts.txt
 ```
@@ -167,15 +167,15 @@
 -999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999
 -99999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999
 ```
 
 ## Usage
 
 ```fundamental
-Amounts v3.3 ( github.com/ivan-sincek/amounts )
+Amounts v3.4 ( github.com/ivan-sincek/amounts )
 
 --- Generate a wordlist from an amount range ---
 Usage:   python3 amounts.py -min minimum -max maximum -mid middle -o out         [-q quotes]
 Example: python3 amounts.py -min 1       -max 1000    -mid 20     -o amounts.txt [-q double]
 
 --- Generate a wordlist from a single amount ---
 Usage:   python3 amounts.py -mid middle -o out         [-q quotes]
```

### Comparing `amounts-3.3/src/amounts.egg-info/SOURCES.txt` & `amounts-3.4/src/amounts.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 pyproject.toml
 src/amounts/__init__.py
 src/amounts/amounts.py
 src/amounts.egg-info/PKG-INFO
 src/amounts.egg-info/SOURCES.txt
 src/amounts.egg-info/dependency_links.txt
 src/amounts.egg-info/entry_points.txt
-src/amounts.egg-info/requires.txt
 src/amounts.egg-info/top_level.txt
 src/wordlists/all.txt
 src/wordlists/hundred.txt
 src/wordlists/hundred_thousand.txt
 src/wordlists/milion.txt
 src/wordlists/one.txt
 src/wordlists/ten.txt
```

### Comparing `amounts-3.3/src/wordlists/all.txt` & `amounts-3.4/src/wordlists/all.txt`

 * *Files identical despite different names*

### Comparing `amounts-3.3/src/wordlists/hundred.txt` & `amounts-3.4/src/wordlists/hundred.txt`

 * *Files identical despite different names*

### Comparing `amounts-3.3/src/wordlists/hundred_thousand.txt` & `amounts-3.4/src/wordlists/hundred_thousand.txt`

 * *Files identical despite different names*

### Comparing `amounts-3.3/src/wordlists/milion.txt` & `amounts-3.4/src/wordlists/milion.txt`

 * *Files identical despite different names*

### Comparing `amounts-3.3/src/wordlists/one.txt` & `amounts-3.4/src/wordlists/one.txt`

 * *Files identical despite different names*

### Comparing `amounts-3.3/src/wordlists/ten.txt` & `amounts-3.4/src/wordlists/ten.txt`

 * *Files identical despite different names*

### Comparing `amounts-3.3/src/wordlists/ten_thousand.txt` & `amounts-3.4/src/wordlists/ten_thousand.txt`

 * *Files identical despite different names*

### Comparing `amounts-3.3/src/wordlists/thousand.txt` & `amounts-3.4/src/wordlists/thousand.txt`

 * *Files identical despite different names*

### Comparing `amounts-3.3/src/wordlists/zero.txt` & `amounts-3.4/src/wordlists/zero.txt`

 * *Files identical despite different names*

### Comparing `amounts-3.3/src/wordlists/zero_point_one.txt` & `amounts-3.4/src/wordlists/zero_point_one.txt`

 * *Files identical despite different names*

