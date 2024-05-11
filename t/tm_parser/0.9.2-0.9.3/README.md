# Comparing `tmp/tm_parser-0.9.2.tar.gz` & `tmp/tm_parser-0.9.3.tar.gz`

## Comparing `tm_parser-0.9.2.tar` & `tm_parser-0.9.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 tm_parser-0.9.2/README.md
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tm_parser-0.9.2/VERSION
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tm_parser-0.9.2/__init__.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 tm_parser-0.9.2/__main__.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tm_parser-0.9.2/requirements.txt
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 tm_parser-0.9.2/test.py
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 tm_parser-0.9.2/data/mb_names.txt
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 tm_parser-0.9.2/tm_parser/__init__.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 tm_parser-0.9.2/tm_parser/__main__.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 tm_parser-0.9.2/tm_parser/activity.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 tm_parser-0.9.2/tm_parser/config.py
--rw-r--r--   0        0        0     4825 2020-02-02 00:00:00.000000 tm_parser-0.9.2/tm_parser/config.toml
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 tm_parser-0.9.2/tm_parser/leadership.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 tm_parser-0.9.2/tm_parser/merit_badge.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 tm_parser-0.9.2/tm_parser/oa.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 tm_parser-0.9.2/tm_parser/output.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 tm_parser-0.9.2/tm_parser/parser.py
--rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 tm_parser-0.9.2/tm_parser/partial_merit_badge.py
--rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 tm_parser-0.9.2/tm_parser/pdf.py
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 tm_parser-0.9.2/tm_parser/rank.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 tm_parser-0.9.2/tm_parser/scout.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 tm_parser-0.9.2/tm_parser/utils.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 tm_parser-0.9.2/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 tm_parser-0.9.2/LICENSE
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 tm_parser-0.9.2/pyproject.toml
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 tm_parser-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 tm_parser-0.9.3/README.md
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tm_parser-0.9.3/VERSION
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tm_parser-0.9.3/__init__.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 tm_parser-0.9.3/__main__.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tm_parser-0.9.3/requirements.txt
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 tm_parser-0.9.3/test.py
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 tm_parser-0.9.3/data/mb_names.txt
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 tm_parser-0.9.3/tm_parser/__init__.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 tm_parser-0.9.3/tm_parser/__main__.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 tm_parser-0.9.3/tm_parser/activity.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 tm_parser-0.9.3/tm_parser/config.py
+-rw-r--r--   0        0        0     4825 2020-02-02 00:00:00.000000 tm_parser-0.9.3/tm_parser/config.toml
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 tm_parser-0.9.3/tm_parser/leadership.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 tm_parser-0.9.3/tm_parser/merit_badge.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 tm_parser-0.9.3/tm_parser/oa.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 tm_parser-0.9.3/tm_parser/output.py
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 tm_parser-0.9.3/tm_parser/parser.py
+-rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 tm_parser-0.9.3/tm_parser/partial_merit_badge.py
+-rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 tm_parser-0.9.3/tm_parser/pdf.py
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 tm_parser-0.9.3/tm_parser/rank.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 tm_parser-0.9.3/tm_parser/scout.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 tm_parser-0.9.3/tm_parser/utils.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 tm_parser-0.9.3/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 tm_parser-0.9.3/LICENSE
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 tm_parser-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 tm_parser-0.9.3/PKG-INFO
```

### Comparing `tm_parser-0.9.2/README.md` & `tm_parser-0.9.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 tm_parser
 
 Michael Perkins, 2023
 
 ## Installation
 
-Recommend you use a virtual environment:
-
-    python -m venv .venv
-    source .venv/bin/activate
-
-    python -m pip install --upgrade pip
-    pip install -r requirements.txt
+python -m pip install tm_parser
 
 ## Instructions:
 
 In troopmaster, under reports -> advancement -> individual history
 - select all the scouts you want to report
 - select all the ranks you want to report
 - Do not select "Omit details on completed ranks"
@@ -22,15 +16,16 @@
 
 generate the report and save it to a PDF.
 
 by default, the output is to the console in YAML format
 
 Then run:
 
-    python -m tm_parser INPUTFILE.pdf
+
+    tmparser INPUTFILE.pdf
 
 Options:
 
     -t --output-type  [yaml], json or toml
 
     -o --outfile output filename
 
@@ -43,15 +38,15 @@
     with open('output.yaml') as f:
 
         scouts = yaml.safe_load(f)
 
 
 ## Using TmParser in code:
 
-    from tm_parser import TmParser
+    from tm_parser import Parser
 
     #initializing the parser automatically parses the file and stores
     #the information in TmParser().scouts
     parser = TmParser(infile='filename.pdf')
 
 
     # Iterating on the parser yields scouts
```

### Comparing `tm_parser-0.9.2/__main__.py` & `tm_parser-0.9.3/__main__.py`

 * *Files identical despite different names*

### Comparing `tm_parser-0.9.2/data/mb_names.txt` & `tm_parser-0.9.3/data/mb_names.txt`

 * *Files identical despite different names*

### Comparing `tm_parser-0.9.2/tm_parser/__init__.py` & `tm_parser-0.9.3/tm_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `tm_parser-0.9.2/tm_parser/__main__.py` & `tm_parser-0.9.3/tm_parser/__main__.py`

 * *Files identical despite different names*

### Comparing `tm_parser-0.9.2/tm_parser/activity.py` & `tm_parser-0.9.3/tm_parser/activity.py`

 * *Files identical despite different names*

### Comparing `tm_parser-0.9.2/tm_parser/config.py` & `tm_parser-0.9.3/tm_parser/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 class Config:
     # the troop directory is data/TROOP/
     LOG_DIR = TROOP_DIR = basedir / "data"
 
     OUTPUT_FORMAT = config.get("OUTPUT_FORMAT", "yaml")
     OUTPUT_TO_FILE = config.get("OUTPUT_TO_FILE", False)
 
-    #FILES = {
-        #"input_file": config.get("INPUT_FILE", os.path.join(TROOP_DIR, "tm_data.pdf")),
-        #"output_file": config.get(
-            #"OUTPUT_FILE", os.path.join(TROOP_DIR, f"output.{OUTPUT_FORMAT}")
-        #),
-    #}
+    # FILES = {
+    # "input_file": config.get("INPUT_FILE", os.path.join(TROOP_DIR, "tm_data.pdf")),
+    # "output_file": config.get(
+    # "OUTPUT_FILE", os.path.join(TROOP_DIR, f"output.{OUTPUT_FORMAT}")
+    # ),
+    # }
 
     PARTIAL_MB_HEADERS = config.get("PARTIAL_MB_HEADERS")
     OA_HEADERS = config.get("OA_HEADERS")
     ACTIVITY_HEADERS = config.get("ACTIVITY_HEADERS")
     SECTION_MARKERS = config.get("SECTION_MARKERS")
     TEXT_FIELDS = config.get("TEXT_FIELDS")
     DATE_FIELDS = config.get("DATE_FIELDS")
```

### Comparing `tm_parser-0.9.2/tm_parser/config.toml` & `tm_parser-0.9.3/tm_parser/config.toml`

 * *Files identical despite different names*

### Comparing `tm_parser-0.9.2/tm_parser/merit_badge.py` & `tm_parser-0.9.3/tm_parser/merit_badge.py`

 * *Files identical despite different names*

### Comparing `tm_parser-0.9.2/tm_parser/oa.py` & `tm_parser-0.9.3/tm_parser/oa.py`

 * *Files identical despite different names*

### Comparing `tm_parser-0.9.2/tm_parser/output.py` & `tm_parser-0.9.3/tm_parser/output.py`

 * *Files identical despite different names*

### Comparing `tm_parser-0.9.2/tm_parser/parser.py` & `tm_parser-0.9.3/tm_parser/parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,32 +31,32 @@
 
     def dump(self, outfile=None, file_format=None):
         if outfile:
             file = outfile
         elif self.output_file:
             file = self.output_file
         else:
-            raise ValueError ("no output file specified")
+            raise ValueError("no output file specified")
 
         if file_format:
             filetype = file_format
         elif self.output_format:
             filetype = file_format
-        elif file.split(".")[-1].lower() in ('yaml', 'toml', 'json'):
-            filetype = file.split(".")[-1].lower() 
+        elif file.split(".")[-1].lower() in ("yaml", "toml", "json"):
+            filetype = file.split(".")[-1].lower()
         else:
-            raise ValueError ("no output format specified")
+            raise ValueError("no output format specified")
 
         if not self.scouts:
             raise ValueError("No scout data found, run parse() first")
         with open(file, "w", encoding="utf-8") as f:
             dump_file(self.scouts, filetype, outfile=f)
 
     def dumps(self, format=None):
-        if format in ('json', 'yaml', 'toml'):
+        if format in ("json", "yaml", "toml"):
             text_format = format
         else:
             text_format = self.output_format
 
         if not self.scouts:
             raise ValueError("No scout data found, run parse() first")
         return dump_string(self.scouts, text_format)
```

### Comparing `tm_parser-0.9.2/tm_parser/partial_merit_badge.py` & `tm_parser-0.9.3/tm_parser/partial_merit_badge.py`

 * *Files identical despite different names*

### Comparing `tm_parser-0.9.2/tm_parser/pdf.py` & `tm_parser-0.9.3/tm_parser/pdf.py`

 * *Files identical despite different names*

### Comparing `tm_parser-0.9.2/tm_parser/rank.py` & `tm_parser-0.9.3/tm_parser/rank.py`

 * *Files identical despite different names*

### Comparing `tm_parser-0.9.2/tm_parser/scout.py` & `tm_parser-0.9.3/tm_parser/scout.py`

 * *Files identical despite different names*

### Comparing `tm_parser-0.9.2/tm_parser/utils.py` & `tm_parser-0.9.3/tm_parser/utils.py`

 * *Files identical despite different names*

### Comparing `tm_parser-0.9.2/LICENSE` & `tm_parser-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tm_parser-0.9.2/pyproject.toml` & `tm_parser-0.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tm_parser-0.9.2/PKG-INFO` & `tm_parser-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tm_parser
-Version: 0.9.2
+Version: 0.9.3
 Summary: Parse Troopmaster export files into TOML, YAML, or JSON
 Project-URL: Repository, https://gitlab.com/perkinsms/tm_parser
 Author-email: Michael Perkins <perkinsms@gmail.com>
 Maintainer-email: Michael Perkins <perkinsms@gmail.com>
 License: MIT License
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
```

