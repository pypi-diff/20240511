# Comparing `tmp/brazilfiscalreport-0.3.3.tar.gz` & `tmp/brazilfiscalreport-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brazilfiscalreport-0.3.3.tar", last modified: Thu May  9 02:21:30 2024, max compression
+gzip compressed data, was "brazilfiscalreport-0.3.4.tar", last modified: Sat May 11 01:51:21 2024, max compression
```

## Comparing `brazilfiscalreport-0.3.3.tar` & `brazilfiscalreport-0.3.4.tar`

### file list

```diff
@@ -1,39 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:21:30.384814 brazilfiscalreport-0.3.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:21:30.384814 brazilfiscalreport-0.3.3/BrazilFiscalReport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-09 02:21:30.000000 brazilfiscalreport-0.3.3/BrazilFiscalReport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-09 02:21:30.000000 brazilfiscalreport-0.3.3/BrazilFiscalReport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 02:21:30.000000 brazilfiscalreport-0.3.3/BrazilFiscalReport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-09 02:21:30.000000 brazilfiscalreport-0.3.3/BrazilFiscalReport.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-09 02:21:30.000000 brazilfiscalreport-0.3.3/BrazilFiscalReport.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-05-09 02:21:26.000000 brazilfiscalreport-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-09 02:21:30.384814 brazilfiscalreport-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-05-09 02:21:26.000000 brazilfiscalreport-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:21:30.380814 brazilfiscalreport-0.3.3/brazilfiscalreport/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 02:21:26.000000 brazilfiscalreport-0.3.3/brazilfiscalreport/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:21:30.380814 brazilfiscalreport-0.3.3/brazilfiscalreport/dacce/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-09 02:21:26.000000 brazilfiscalreport-0.3.3/brazilfiscalreport/dacce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-05-09 02:21:26.000000 brazilfiscalreport-0.3.3/brazilfiscalreport/dacce/dacce.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:21:30.384814 brazilfiscalreport-0.3.3/brazilfiscalreport/danfe/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-09 02:21:26.000000 brazilfiscalreport-0.3.3/brazilfiscalreport/danfe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-09 02:21:26.000000 brazilfiscalreport-0.3.3/brazilfiscalreport/danfe/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    51511 2024-05-09 02:21:26.000000 brazilfiscalreport-0.3.3/brazilfiscalreport/danfe/danfe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-09 02:21:26.000000 brazilfiscalreport-0.3.3/brazilfiscalreport/danfe/danfe_basic_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-09 02:21:26.000000 brazilfiscalreport-0.3.3/brazilfiscalreport/danfe/danfe_block.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-09 02:21:26.000000 brazilfiscalreport-0.3.3/brazilfiscalreport/danfe/danfe_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-09 02:21:26.000000 brazilfiscalreport-0.3.3/brazilfiscalreport/danfe/danfe_conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-09 02:21:26.000000 brazilfiscalreport-0.3.3/brazilfiscalreport/danfe/danfe_emit_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-09 02:21:26.000000 brazilfiscalreport-0.3.3/brazilfiscalreport/danfe/danfe_ident_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-09 02:21:26.000000 brazilfiscalreport-0.3.3/brazilfiscalreport/danfe/danfe_verification_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-09 02:21:26.000000 brazilfiscalreport-0.3.3/brazilfiscalreport/danfe/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-09 02:21:26.000000 brazilfiscalreport-0.3.3/brazilfiscalreport/pdf_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-09 02:21:26.000000 brazilfiscalreport-0.3.3/brazilfiscalreport/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-09 02:21:26.000000 brazilfiscalreport-0.3.3/brazilfiscalreport/xfpdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-09 02:21:26.000000 brazilfiscalreport-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 02:21:30.384814 brazilfiscalreport-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-09 02:21:26.000000 brazilfiscalreport-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:21:30.384814 brazilfiscalreport-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 02:21:26.000000 brazilfiscalreport-0.3.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-05-09 02:21:26.000000 brazilfiscalreport-0.3.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-09 02:21:26.000000 brazilfiscalreport-0.3.3/tests/test_dacce.py
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-09 02:21:26.000000 brazilfiscalreport-0.3.3/tests/test_danfe.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-09 02:21:26.000000 brazilfiscalreport-0.3.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:51:21.779507 brazilfiscalreport-0.3.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:51:21.779507 brazilfiscalreport-0.3.4/BrazilFiscalReport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16983 2024-05-11 01:51:21.000000 brazilfiscalreport-0.3.4/BrazilFiscalReport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-11 01:51:21.000000 brazilfiscalreport-0.3.4/BrazilFiscalReport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 01:51:21.000000 brazilfiscalreport-0.3.4/BrazilFiscalReport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-11 01:51:21.000000 brazilfiscalreport-0.3.4/BrazilFiscalReport.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-11 01:51:21.000000 brazilfiscalreport-0.3.4/BrazilFiscalReport.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-05-11 01:51:17.000000 brazilfiscalreport-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16983 2024-05-11 01:51:21.779507 brazilfiscalreport-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-05-11 01:51:17.000000 brazilfiscalreport-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:51:21.775507 brazilfiscalreport-0.3.4/brazilfiscalreport/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-11 01:51:17.000000 brazilfiscalreport-0.3.4/brazilfiscalreport/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:51:21.775507 brazilfiscalreport-0.3.4/brazilfiscalreport/dacce/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-11 01:51:17.000000 brazilfiscalreport-0.3.4/brazilfiscalreport/dacce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-05-11 01:51:17.000000 brazilfiscalreport-0.3.4/brazilfiscalreport/dacce/dacce.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:51:21.779507 brazilfiscalreport-0.3.4/brazilfiscalreport/danfe/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-11 01:51:17.000000 brazilfiscalreport-0.3.4/brazilfiscalreport/danfe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-11 01:51:17.000000 brazilfiscalreport-0.3.4/brazilfiscalreport/danfe/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51511 2024-05-11 01:51:17.000000 brazilfiscalreport-0.3.4/brazilfiscalreport/danfe/danfe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-11 01:51:17.000000 brazilfiscalreport-0.3.4/brazilfiscalreport/danfe/danfe_basic_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-11 01:51:17.000000 brazilfiscalreport-0.3.4/brazilfiscalreport/danfe/danfe_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-11 01:51:17.000000 brazilfiscalreport-0.3.4/brazilfiscalreport/danfe/danfe_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-11 01:51:17.000000 brazilfiscalreport-0.3.4/brazilfiscalreport/danfe/danfe_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-11 01:51:17.000000 brazilfiscalreport-0.3.4/brazilfiscalreport/danfe/danfe_emit_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-11 01:51:17.000000 brazilfiscalreport-0.3.4/brazilfiscalreport/danfe/danfe_ident_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-11 01:51:17.000000 brazilfiscalreport-0.3.4/brazilfiscalreport/danfe/danfe_verification_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-11 01:51:17.000000 brazilfiscalreport-0.3.4/brazilfiscalreport/danfe/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-11 01:51:17.000000 brazilfiscalreport-0.3.4/brazilfiscalreport/pdf_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-11 01:51:17.000000 brazilfiscalreport-0.3.4/brazilfiscalreport/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-11 01:51:17.000000 brazilfiscalreport-0.3.4/brazilfiscalreport/xfpdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-11 01:51:17.000000 brazilfiscalreport-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 01:51:21.779507 brazilfiscalreport-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:51:21.779507 brazilfiscalreport-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-11 01:51:17.000000 brazilfiscalreport-0.3.4/tests/test_dacce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-11 01:51:17.000000 brazilfiscalreport-0.3.4/tests/test_danfe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-11 01:51:17.000000 brazilfiscalreport-0.3.4/tests/test_utils.py
```

### Comparing `brazilfiscalreport-0.3.3/BrazilFiscalReport.egg-info/SOURCES.txt` & `brazilfiscalreport-0.3.4/BrazilFiscalReport.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 pyproject.toml
-setup.py
 BrazilFiscalReport.egg-info/PKG-INFO
 BrazilFiscalReport.egg-info/SOURCES.txt
 BrazilFiscalReport.egg-info/dependency_links.txt
 BrazilFiscalReport.egg-info/requires.txt
 BrazilFiscalReport.egg-info/top_level.txt
 brazilfiscalreport/__init__.py
 brazilfiscalreport/pdf_element.py
@@ -20,12 +19,10 @@
 brazilfiscalreport/danfe/danfe_block.py
 brazilfiscalreport/danfe/danfe_code.py
 brazilfiscalreport/danfe/danfe_conf.py
 brazilfiscalreport/danfe/danfe_emit_info.py
 brazilfiscalreport/danfe/danfe_ident_info.py
 brazilfiscalreport/danfe/danfe_verification_msg.py
 brazilfiscalreport/danfe/models.py
-tests/__init__.py
-tests/conftest.py
 tests/test_dacce.py
 tests/test_danfe.py
 tests/test_utils.py
```

### Comparing `brazilfiscalreport-0.3.3/LICENSE` & `brazilfiscalreport-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `brazilfiscalreport-0.3.3/README.md` & `brazilfiscalreport-0.3.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 ## Beta Stage Notice
 
 This library is currently in the beta stage of development. While it has many of the intended features implemented, it is still undergoing testing and improvements. Users should note that during this phase, functionality may change and some instability may occur. We welcome feedback on any issues or suggestions for enhancements. Use in production environments should be approached with caution.
 
 ## Dependencies:
 
 - [FPDF2](https://github.com/py-pdf/fpdf2) - PDF creation library for Python
+- phonenumbers
+- python-barcode
 
 ## To install:
 
 ```bash
 pip install brazilfiscalreport
 ```
```

### Comparing `brazilfiscalreport-0.3.3/brazilfiscalreport/dacce/dacce.py` & `brazilfiscalreport-0.3.4/brazilfiscalreport/dacce/dacce.py`

 * *Files identical despite different names*

### Comparing `brazilfiscalreport-0.3.3/brazilfiscalreport/danfe/config.py` & `brazilfiscalreport-0.3.4/brazilfiscalreport/danfe/config.py`

 * *Files identical despite different names*

### Comparing `brazilfiscalreport-0.3.3/brazilfiscalreport/danfe/danfe.py` & `brazilfiscalreport-0.3.4/brazilfiscalreport/danfe/danfe.py`

 * *Files identical despite different names*

### Comparing `brazilfiscalreport-0.3.3/brazilfiscalreport/danfe/danfe_basic_field.py` & `brazilfiscalreport-0.3.4/brazilfiscalreport/danfe/danfe_basic_field.py`

 * *Files identical despite different names*

### Comparing `brazilfiscalreport-0.3.3/brazilfiscalreport/danfe/danfe_block.py` & `brazilfiscalreport-0.3.4/brazilfiscalreport/danfe/danfe_block.py`

 * *Files identical despite different names*

### Comparing `brazilfiscalreport-0.3.3/brazilfiscalreport/danfe/danfe_code.py` & `brazilfiscalreport-0.3.4/brazilfiscalreport/danfe/danfe_code.py`

 * *Files identical despite different names*

### Comparing `brazilfiscalreport-0.3.3/brazilfiscalreport/danfe/danfe_emit_info.py` & `brazilfiscalreport-0.3.4/brazilfiscalreport/danfe/danfe_emit_info.py`

 * *Files identical despite different names*

### Comparing `brazilfiscalreport-0.3.3/brazilfiscalreport/danfe/danfe_ident_info.py` & `brazilfiscalreport-0.3.4/brazilfiscalreport/danfe/danfe_ident_info.py`

 * *Files identical despite different names*

### Comparing `brazilfiscalreport-0.3.3/brazilfiscalreport/pdf_element.py` & `brazilfiscalreport-0.3.4/brazilfiscalreport/pdf_element.py`

 * *Files identical despite different names*

### Comparing `brazilfiscalreport-0.3.3/brazilfiscalreport/utils.py` & `brazilfiscalreport-0.3.4/brazilfiscalreport/utils.py`

 * *Files identical despite different names*

### Comparing `brazilfiscalreport-0.3.3/brazilfiscalreport/xfpdf.py` & `brazilfiscalreport-0.3.4/brazilfiscalreport/xfpdf.py`

 * *Files identical despite different names*

### Comparing `brazilfiscalreport-0.3.3/tests/test_dacce.py` & `brazilfiscalreport-0.3.4/tests/test_dacce.py`

 * *Files identical despite different names*

### Comparing `brazilfiscalreport-0.3.3/tests/test_danfe.py` & `brazilfiscalreport-0.3.4/tests/test_danfe.py`

 * *Files identical despite different names*

