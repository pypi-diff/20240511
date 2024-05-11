# Comparing `tmp/bibla-2.0.1.tar.gz` & `tmp/bibla-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibla-2.0.1.tar", last modified: Sat May 11 13:26:10 2024, max compression
+gzip compressed data, was "bibla-2.0.2.tar", last modified: Sat May 11 21:24:20 2024, max compression
```

## Comparing `bibla-2.0.1.tar` & `bibla-2.0.2.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 tristan    (501) staff       (20)        0 2024-05-11 13:26:10.645169 bibla-2.0.1/
--rw-r--r--   0 tristan    (501) staff       (20)      139 2024-04-19 08:23:33.000000 bibla-2.0.1/.flake8
-drwxr-xr-x   0 tristan    (501) staff       (20)        0 2024-05-11 13:26:10.636070 bibla-2.0.1/.idea/
--rw-r--r--   0 tristan    (501) staff       (20)      572 2024-04-21 10:12:56.000000 bibla-2.0.1/.idea/biblint.iml
-drwxr-xr-x   0 tristan    (501) staff       (20)        0 2024-05-11 13:26:10.636312 bibla-2.0.1/.idea/inspectionProfiles/
--rw-r--r--   0 tristan    (501) staff       (20)      174 2024-04-19 08:23:33.000000 bibla-2.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 tristan    (501) staff       (20)      195 2024-04-19 08:23:33.000000 bibla-2.0.1/.idea/misc.xml
--rw-r--r--   0 tristan    (501) staff       (20)      266 2024-04-19 08:23:33.000000 bibla-2.0.1/.idea/modules.xml
--rw-r--r--   0 tristan    (501) staff       (20)      180 2024-04-19 08:23:33.000000 bibla-2.0.1/.idea/vcs.xml
--rw-r--r--   0 tristan    (501) staff       (20)     1541 2024-05-11 12:03:28.000000 bibla-2.0.1/LICENSE
--rw-r--r--   0 tristan    (501) staff       (20)      324 2024-04-21 10:12:56.000000 bibla-2.0.1/MANIFEST.in
--rw-r--r--   0 tristan    (501) staff       (20)     5930 2024-05-11 13:26:10.644908 bibla-2.0.1/PKG-INFO
--rw-r--r--   0 tristan    (501) staff       (20)     4836 2024-04-21 10:12:56.000000 bibla-2.0.1/README.md
-drwxr-xr-x   0 tristan    (501) staff       (20)        0 2024-05-11 13:26:10.637453 bibla-2.0.1/bibla/
--rw-r--r--   0 tristan    (501) staff       (20)      226 2024-05-11 13:25:49.000000 bibla-2.0.1/bibla/__init__.py
--rw-r--r--   0 tristan    (501) staff       (20)     3760 2024-04-21 10:12:56.000000 bibla-2.0.1/bibla/__main__.py
--rw-r--r--   0 tristan    (501) staff       (20)     3096 2024-05-01 14:48:41.000000 bibla-2.0.1/bibla/bibla.yml
--rw-r--r--   0 tristan    (501) staff       (20)     1884 2024-04-21 10:12:56.000000 bibla-2.0.1/bibla/config.py
--rw-r--r--   0 tristan    (501) staff       (20)     4467 2024-04-26 13:55:23.000000 bibla-2.0.1/bibla/lint.py
--rw-r--r--   0 tristan    (501) staff       (20)     5259 2024-04-21 10:12:56.000000 bibla-2.0.1/bibla/rule.py
-drwxr-xr-x   0 tristan    (501) staff       (20)        0 2024-05-11 13:26:10.639191 bibla-2.0.1/bibla/rules/
--rw-r--r--   0 tristan    (501) staff       (20)      253 2024-04-21 10:12:56.000000 bibla-2.0.1/bibla/rules/__init__.py
--rw-r--r--   0 tristan    (501) staff       (20)     2386 2024-04-21 10:12:56.000000 bibla-2.0.1/bibla/rules/database_rules.py
--rw-r--r--   0 tristan    (501) staff       (20)    13175 2024-05-11 12:08:54.000000 bibla-2.0.1/bibla/rules/entry_rules.py
--rw-r--r--   0 tristan    (501) staff       (20)     4244 2024-05-03 07:38:40.000000 bibla-2.0.1/bibla/rules/field_rules.py
--rw-r--r--   0 tristan    (501) staff       (20)     2428 2024-04-21 10:12:56.000000 bibla-2.0.1/bibla/rules/specification_rules.py
--rw-r--r--   0 tristan    (501) staff       (20)     3101 2024-04-21 10:12:56.000000 bibla-2.0.1/bibla/rules/text_rules.py
--rw-r--r--   0 tristan    (501) staff       (20)     2466 2024-04-26 13:59:35.000000 bibla-2.0.1/bibla/text_utils.py
-drwxr-xr-x   0 tristan    (501) staff       (20)        0 2024-05-11 13:26:10.644225 bibla-2.0.1/bibla.egg-info/
--rw-r--r--   0 tristan    (501) staff       (20)     5930 2024-05-11 13:26:10.000000 bibla-2.0.1/bibla.egg-info/PKG-INFO
--rw-r--r--   0 tristan    (501) staff       (20)     1079 2024-05-11 13:26:10.000000 bibla-2.0.1/bibla.egg-info/SOURCES.txt
--rw-r--r--   0 tristan    (501) staff       (20)        1 2024-05-11 13:26:10.000000 bibla-2.0.1/bibla.egg-info/dependency_links.txt
--rw-r--r--   0 tristan    (501) staff       (20)       45 2024-05-11 13:26:10.000000 bibla-2.0.1/bibla.egg-info/entry_points.txt
--rw-r--r--   0 tristan    (501) staff       (20)      171 2024-05-11 13:26:10.000000 bibla-2.0.1/bibla.egg-info/requires.txt
--rw-r--r--   0 tristan    (501) staff       (20)        6 2024-05-11 13:26:10.000000 bibla-2.0.1/bibla.egg-info/top_level.txt
--rw-r--r--   0 tristan    (501) staff       (20)       38 2024-05-11 13:26:10.645226 bibla-2.0.1/setup.cfg
--rwxr-xr-x   0 tristan    (501) staff       (20)     1669 2024-05-11 13:24:32.000000 bibla-2.0.1/setup.py
-drwxr-xr-x   0 tristan    (501) staff       (20)        0 2024-05-11 13:26:10.639444 bibla-2.0.1/test/
--rw-r--r--   0 tristan    (501) staff       (20)        0 2024-04-19 08:23:33.000000 bibla-2.0.1/test/__init__.py
--rw-r--r--   0 tristan    (501) staff       (20)      472 2024-04-21 10:12:56.000000 bibla-2.0.1/test/test_base.py
-drwxr-xr-x   0 tristan    (501) staff       (20)        0 2024-05-11 13:26:10.643898 bibla-2.0.1/test_data/
--rw-r--r--   0 tristan    (501) staff       (20)       87 2024-04-26 13:44:15.000000 bibla-2.0.1/test_data/.bibla.yml
--rw-r--r--   0 tristan    (501) staff       (20)    13625 2024-05-03 07:47:06.000000 bibla-2.0.1/test_data/Valid_bibLaTeX.bib
--rw-r--r--   0 tristan    (501) staff       (20)      346 2024-05-01 19:55:39.000000 bibla-2.0.1/test_data/authorNameFormat.bib
--rw-r--r--   0 tristan    (501) staff       (20)       33 2024-04-26 13:52:19.000000 bibla-2.0.1/test_data/emptyEntries.bib
--rw-r--r--   0 tristan    (501) staff       (20)     2577 2024-05-01 15:24:57.000000 bibla-2.0.1/test_data/mit.bib
--rw-r--r--   0 tristan    (501) staff       (20)      279 2024-05-01 21:03:36.000000 bibla-2.0.1/test_data/noHomepages.bib
--rw-r--r--   0 tristan    (501) staff       (20)     1275 2024-05-01 21:18:36.000000 bibla-2.0.1/test_data/nodirectives.bib
--rw-r--r--   0 tristan    (501) staff       (20)       21 2024-05-03 07:52:51.000000 bibla-2.0.1/test_data/nokeys.bib
--rw-r--r--   0 tristan    (501) staff       (20)      781 2024-04-27 19:22:01.000000 bibla-2.0.1/test_data/originalOverAlias.bib
--rw-r--r--   0 tristan    (501) staff       (20)      161 2024-05-01 14:50:50.000000 bibla-2.0.1/test_data/pages.bib
--rw-r--r--   0 tristan    (501) staff       (20)      408 2024-04-26 13:53:03.000000 bibla-2.0.1/test_data/required.bib
--rw-r--r--   0 tristan    (501) staff       (20)      192 2024-04-27 16:08:08.000000 bibla-2.0.1/test_data/shouldUseDateInsteadOfYearMonthDay.bib
--rw-r--r--   0 tristan    (501) staff       (20)      297 2024-04-20 19:44:58.000000 bibla-2.0.1/test_data/syntax.bib
--rw-r--r--   0 tristan    (501) staff       (20)      216 2024-04-22 19:15:10.000000 bibla-2.0.1/test_data/unique.bib
--rw-r--r--   0 tristan    (501) staff       (20)      697 2024-05-01 18:56:32.000000 bibla-2.0.1/test_data/wrongDateFormat.bib
--rw-r--r--   0 tristan    (501) staff       (20)       99 2024-05-03 07:54:52.000000 bibla-2.0.1/test_data/wrongFormatKey.bib
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:24:20.892944 bibla-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-11 21:24:12.000000 bibla-2.0.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:24:20.884945 bibla-2.0.2/.idea/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-11 21:24:12.000000 bibla-2.0.2/.idea/biblint.iml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:24:20.884945 bibla-2.0.2/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-11 21:24:12.000000 bibla-2.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-11 21:24:12.000000 bibla-2.0.2/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-11 21:24:12.000000 bibla-2.0.2/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-11 21:24:12.000000 bibla-2.0.2/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-11 21:24:12.000000 bibla-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-11 21:24:12.000000 bibla-2.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-05-11 21:24:20.892944 bibla-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-05-11 21:24:12.000000 bibla-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:24:20.888944 bibla-2.0.2/bibla/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-11 21:24:12.000000 bibla-2.0.2/bibla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-11 21:24:12.000000 bibla-2.0.2/bibla/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-11 21:24:12.000000 bibla-2.0.2/bibla/bibla.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-11 21:24:12.000000 bibla-2.0.2/bibla/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-11 21:24:12.000000 bibla-2.0.2/bibla/lint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-05-11 21:24:12.000000 bibla-2.0.2/bibla/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:24:20.888944 bibla-2.0.2/bibla/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-11 21:24:12.000000 bibla-2.0.2/bibla/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-11 21:24:12.000000 bibla-2.0.2/bibla/rules/database_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13128 2024-05-11 21:24:12.000000 bibla-2.0.2/bibla/rules/entry_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-11 21:24:12.000000 bibla-2.0.2/bibla/rules/field_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-11 21:24:12.000000 bibla-2.0.2/bibla/rules/specification_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-11 21:24:12.000000 bibla-2.0.2/bibla/rules/text_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-11 21:24:12.000000 bibla-2.0.2/bibla/text_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:24:20.892944 bibla-2.0.2/bibla.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-05-11 21:24:20.000000 bibla-2.0.2/bibla.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-11 21:24:20.000000 bibla-2.0.2/bibla.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 21:24:20.000000 bibla-2.0.2/bibla.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-11 21:24:20.000000 bibla-2.0.2/bibla.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-11 21:24:20.000000 bibla-2.0.2/bibla.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-11 21:24:20.000000 bibla-2.0.2/bibla.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 21:24:20.892944 bibla-2.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1581 2024-05-11 21:24:12.000000 bibla-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:24:20.888944 bibla-2.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 21:24:12.000000 bibla-2.0.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-11 21:24:12.000000 bibla-2.0.2/test/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:24:20.892944 bibla-2.0.2/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/.bibla.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/authorNameFormatting.bib
+-rw-r--r--   0 runner    (1001) docker     (127)    13625 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/bibLaTeX.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/dateFormat.bib
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/emptyEntries.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/mit.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/noHomepages.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/nodirectives.bib
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/nokeys.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/originalOverAlias.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/pages.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/required.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/shouldUseDateInsteadOfYearMonthDay.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/syntax.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/unique.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/wrongDateFormat.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/wrongFormatKey.bib
```

### Comparing `bibla-2.0.1/.idea/biblint.iml` & `bibla-2.0.2/.idea/biblint.iml`

 * *Files identical despite different names*

### Comparing `bibla-2.0.1/LICENSE` & `bibla-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bibla-2.0.1/PKG-INFO` & `bibla-2.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 Metadata-Version: 2.1
 Name: bibla
-Version: 2.0.1
+Version: 2.0.2
 Summary: A minimalistic bibLaTeX linter based by Tristan Cuvelier.
 Home-page: https://github.com/MrClassicT/bibla
 Author: Tristan Cuvelier
 Author-email: tristan.cuvelier@student.hogent.be
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click>=7
-Requires-Dist: fuzzywuzzy<1,>=0.10
+Requires-Dist: fuzzywuzzy>=0.10
 Requires-Dist: markdown-table
 Requires-Dist: pybtex==0.23.0
-Requires-Dist: pyyaml<6,>=5
+Requires-Dist: pyyaml>=5
 Requires-Dist: unidecode<2,>=1
 Provides-Extra: dev
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: pep8-naming; extra == "dev"
-Requires-Dist: flake8-docstrings; extra == "dev"
 Requires-Dist: anybadge; extra == "dev"
 Requires-Dist: markdown; extra == "dev"
 Requires-Dist: check-manifest; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # bibla
```

### Comparing `bibla-2.0.1/README.md` & `bibla-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `bibla-2.0.1/bibla/__main__.py` & `bibla-2.0.2/bibla/__main__.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.1/bibla/bibla.yml` & `bibla-2.0.2/bibla/bibla.yml`

 * *Files identical despite different names*

### Comparing `bibla-2.0.1/bibla/config.py` & `bibla-2.0.2/bibla/config.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.1/bibla/lint.py` & `bibla-2.0.2/bibla/lint.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,18 +58,18 @@
             print(f"{bibliography} D03: Duplicate entry with key '{duplicate_key}'")
         else:
             print(f"Warning: {e}")
         return []
     except pybtex.scanner.TokenRequired as e:
         print(f"E00: {e}")
         return []
-    except Error as e:
+    except Exception as e:
         print(f"Error: {e}")
         return []
-    
+
     bib_data.file = bibliography
     with open(bibliography, 'r') as bib_file:
         bib_text = bib_file.read()
 
     rules = load_rules()
 
     text_warnings = _apply_text_rules(bibliography, bib_text,
```

### Comparing `bibla-2.0.1/bibla/rule.py` & `bibla-2.0.2/bibla/rule.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.1/bibla/rules/database_rules.py` & `bibla-2.0.2/bibla/rules/database_rules.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.1/bibla/rules/entry_rules.py` & `bibla-2.0.2/bibla/rules/entry_rules.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import itertools
 import os
 import re
 from unidecode import unidecode
 
 from bibla.config import get_config
 from bibla.rule import register_entry_rule
-from bibla.text_utils import MONTH_NAMES
 
-@register_entry_rule('E00','Keys of published works should have format `AuthorYEARa`')
+
+@register_entry_rule('E00', 'Keys of published works should have format `AuthorYEARa`')
 def key_format(key, entry, database):
     """Raise a linter warning when entry key is not of format `AuthorYEARa`.
 
     E.g. an entry with values
     ```
     author = {Arthur B Cummings and David Eftekhary and Frank G House},
     date   = {2003-02-02}
@@ -24,15 +24,15 @@
     This rule only applies when `date` and at least one author are set.
 
     :param key: The key of the current bibliography entry
     :param entry: The current bibliography entry
     :param database: All bibliography entries
     :return: True if the current entry's key has the specified format or
     year or author are not specified, False otherwise.
-    """   
+    """
     if 'date' not in entry.fields or list(
             itertools.chain(*entry.persons.values())).count == 0:
         return True
     author = entry.persons['author'][0]
     names = author.rich_prelast_names + author.rich_last_names
     date = entry.fields['date']
     year = re.search(r'\d{4}', date).group()
@@ -288,19 +288,21 @@
         :return: False if the alias entry type is used, True otherwise
         """
         if entry.type == alt_entry_type:
             return False
         else:
             return True
 
+
 alias_entry_types = get_config().get('alias_entry_types', {})
 for entry_type, alt_entry_types in alias_entry_types.items():
     for alt_entry_type in alt_entry_types:
         register_alternate_entry_type_rule(entry_type, alt_entry_type)
-        
+
+
 @register_entry_rule('E12', 'Homepages should not be used as a source')
 def check_homepage_in_url(key, entry, database):
     """Raise a linter warning when a URL field contains a homepage.
 
     :param key: The key of the current bibliography entry
     :param entry: The current bibliography entry
     :param database: All bibliography entries
@@ -310,14 +312,15 @@
         return True
     url = entry.fields['url']
     regex = re.compile(r'^(https?://)?[^/]+/?$')
     if regex.match(url):
         return False
     return True
 
+
 @register_entry_rule('E13', 'URLs should only include the critical parts and nothing more')
 def check_url_directive_parts(key, entry, database):
     """Raise a linter warning when a URL field contains text highlighting directive parts.
 
     :param key: The key of the current bibliography entry
     :param entry: The current bibliography entry
     :param database: All bibliography entries
```

### Comparing `bibla-2.0.1/bibla/rules/field_rules.py` & `bibla-2.0.2/bibla/rules/field_rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         :return: False if the specific field is used instead of its variant, True otherwise
         """
         if entry.type == entry_type and field in entry.fields:
             return False
         else:
             return True
 
+
 for entry_type, spec in get_config()['type_spec'].items():
     for req_field in spec['required']:
         rule_id = 'M01{}{}'.format(entry_type.capitalize(), req_field.capitalize())
         message = 'Missing required field `{}` for entry type `{}`'.format(req_field, entry_type)
 
         @register_entry_rule(rule_id, message)
         def check_required_field_present(key, entry, database, entry_type=entry_type, req_field=req_field):
@@ -67,24 +68,26 @@
             else:
                 return True
 
         alternate_fields = get_config()['alternate_fields']
         if req_field in alternate_fields:
             for alt_field in alternate_fields[req_field]:
                 register_variant_rule(entry_type, alt_field, req_field)
-                
-                
-@register_entry_rule('M02', 'Special characters should be replaced by the command to generate them: %, &, $, #, _, \, {, }, \, ~, ^, |')
+
+
+@register_entry_rule('M02', 'Special characters should be replaced by the command to generate them: %, &, $, #, _, \\, ~, ^, |')
 def check_special_characters(key, entry, database):
     """Raise a linter warning when a field contains special characters that should be replaced.
 
     :param key: The key of the current bibliography entry
     :param entry: The current bibliography entry
     :param database: All bibliography entries
     :return: True if no field contains special characters, False otherwise.
     """
-    special_chars = ['%', '&', '$','#','_','\\','~','^','|']
-    
+    special_chars = ['%', '&', '$', '#', '_', '\\', '~', '^', '|']
+
     for field in entry.fields.values():
         if any(char in field for char in special_chars):
-            return False
-    return True
+            for char in special_chars:
+                if char in field and field[field.index(char) - 1] != '\\':
+                    return False
+    return True
```

### Comparing `bibla-2.0.1/bibla/rules/specification_rules.py` & `bibla-2.0.2/bibla/rules/specification_rules.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.1/bibla/rules/text_rules.py` & `bibla-2.0.2/bibla/rules/text_rules.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.1/bibla/text_utils.py` & `bibla-2.0.2/bibla/text_utils.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.1/bibla.egg-info/PKG-INFO` & `bibla-2.0.2/bibla.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 Metadata-Version: 2.1
 Name: bibla
-Version: 2.0.1
+Version: 2.0.2
 Summary: A minimalistic bibLaTeX linter based by Tristan Cuvelier.
 Home-page: https://github.com/MrClassicT/bibla
 Author: Tristan Cuvelier
 Author-email: tristan.cuvelier@student.hogent.be
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click>=7
-Requires-Dist: fuzzywuzzy<1,>=0.10
+Requires-Dist: fuzzywuzzy>=0.10
 Requires-Dist: markdown-table
 Requires-Dist: pybtex==0.23.0
-Requires-Dist: pyyaml<6,>=5
+Requires-Dist: pyyaml>=5
 Requires-Dist: unidecode<2,>=1
 Provides-Extra: dev
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: pep8-naming; extra == "dev"
-Requires-Dist: flake8-docstrings; extra == "dev"
 Requires-Dist: anybadge; extra == "dev"
 Requires-Dist: markdown; extra == "dev"
 Requires-Dist: check-manifest; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # bibla
```

### Comparing `bibla-2.0.1/bibla.egg-info/SOURCES.txt` & `bibla-2.0.2/bibla.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,17 @@
 bibla/rules/entry_rules.py
 bibla/rules/field_rules.py
 bibla/rules/specification_rules.py
 bibla/rules/text_rules.py
 test/__init__.py
 test/test_base.py
 test_data/.bibla.yml
-test_data/Valid_bibLaTeX.bib
-test_data/authorNameFormat.bib
+test_data/authorNameFormatting.bib
+test_data/bibLaTeX.bib
+test_data/dateFormat.bib
 test_data/emptyEntries.bib
 test_data/mit.bib
 test_data/noHomepages.bib
 test_data/nodirectives.bib
 test_data/nokeys.bib
 test_data/originalOverAlias.bib
 test_data/pages.bib
```

### Comparing `bibla-2.0.1/setup.py` & `bibla-2.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,25 +27,22 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.12",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         'click>=7',
-        'fuzzywuzzy>=0.10,<1',
+        'fuzzywuzzy>=0.10',
         'markdown-table',
         'pybtex==0.23.0',
-        'pyyaml>=5,<6',
+        'pyyaml>=5',
         'unidecode>=1,<2',
     ],
     extras_require={
         'dev': [
-            'flake8',
-            'pep8-naming',
-            'flake8-docstrings',
             'anybadge',
             'markdown',
             'check-manifest',
             'twine',
         ]
     },
     entry_points={
```

### Comparing `bibla-2.0.1/test_data/Valid_bibLaTeX.bib` & `bibla-2.0.2/test_data/bibLaTeX.bib`

 * *Files identical despite different names*

### Comparing `bibla-2.0.1/test_data/mit.bib` & `bibla-2.0.2/test_data/mit.bib`

 * *Files identical despite different names*

### Comparing `bibla-2.0.1/test_data/nodirectives.bib` & `bibla-2.0.2/test_data/nodirectives.bib`

 * *Files identical despite different names*

### Comparing `bibla-2.0.1/test_data/originalOverAlias.bib` & `bibla-2.0.2/test_data/originalOverAlias.bib`

 * *Files identical despite different names*

### Comparing `bibla-2.0.1/test_data/wrongDateFormat.bib` & `bibla-2.0.2/test_data/wrongDateFormat.bib`

 * *Files identical despite different names*

