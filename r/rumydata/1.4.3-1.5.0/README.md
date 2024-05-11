# Comparing `tmp/rumydata-1.4.3.tar.gz` & `tmp/rumydata-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rumydata-1.4.3.tar", last modified: Thu Jan 25 19:55:00 2024, max compression
+gzip compressed data, was "rumydata-1.5.0.tar", last modified: Sat May 11 03:08:49 2024, max compression
```

## Comparing `rumydata-1.4.3.tar` & `rumydata-1.5.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 19:55:00.821053 rumydata-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-01-25 19:54:48.000000 rumydata-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-01-25 19:55:00.821053 rumydata-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-01-25 19:54:48.000000 rumydata-1.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 19:55:00.817053 rumydata-1.4.3/rumydata/
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-01-25 19:54:48.000000 rumydata-1.4.3/rumydata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10180 2024-01-25 19:54:48.000000 rumydata-1.4.3/rumydata/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-01-25 19:54:48.000000 rumydata-1.4.3/rumydata/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-01-25 19:54:48.000000 rumydata-1.4.3/rumydata/field.py
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-01-25 19:54:48.000000 rumydata-1.4.3/rumydata/menu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 19:55:00.817053 rumydata-1.4.3/rumydata/rules/
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-01-25 19:54:48.000000 rumydata-1.4.3/rumydata/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18981 2024-01-25 19:54:48.000000 rumydata-1.4.3/rumydata/rules/cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-01-25 19:54:48.000000 rumydata-1.4.3/rumydata/rules/column.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-01-25 19:54:48.000000 rumydata-1.4.3/rumydata/rules/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-01-25 19:54:48.000000 rumydata-1.4.3/rumydata/rules/row.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-01-25 19:54:48.000000 rumydata-1.4.3/rumydata/rules/table.py
--rw-r--r--   0 runner    (1001) docker     (127)    20934 2024-01-25 19:54:48.000000 rumydata-1.4.3/rumydata/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 19:55:00.821053 rumydata-1.4.3/rumydata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-01-25 19:55:00.000000 rumydata-1.4.3/rumydata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-01-25 19:55:00.000000 rumydata-1.4.3/rumydata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 19:55:00.000000 rumydata-1.4.3/rumydata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-01-25 19:55:00.000000 rumydata-1.4.3/rumydata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-25 19:55:00.000000 rumydata-1.4.3/rumydata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-25 19:55:00.821053 rumydata-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-01-25 19:54:48.000000 rumydata-1.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 19:55:00.821053 rumydata-1.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 19:54:48.000000 rumydata-1.4.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-01-25 19:54:48.000000 rumydata-1.4.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-01-25 19:54:48.000000 rumydata-1.4.3/tests/test_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-01-25 19:54:48.000000 rumydata-1.4.3/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-01-25 19:54:48.000000 rumydata-1.4.3/tests/test_menu.py
--rw-r--r--   0 runner    (1001) docker     (127)    11886 2024-01-25 19:54:48.000000 rumydata-1.4.3/tests/test_other.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-01-25 19:54:48.000000 rumydata-1.4.3/tests/test_parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-01-25 19:54:48.000000 rumydata-1.4.3/tests/test_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-01-25 19:54:48.000000 rumydata-1.4.3/tests/test_rules_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    14261 2024-01-25 19:54:48.000000 rumydata-1.4.3/tests/test_rules_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-01-25 19:54:48.000000 rumydata-1.4.3/tests/test_rules_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-01-25 19:54:48.000000 rumydata-1.4.3/tests/test_rules_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     8984 2024-01-25 19:54:48.000000 rumydata-1.4.3/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-01-25 19:54:48.000000 rumydata-1.4.3/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:08:49.171013 rumydata-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-11 03:08:41.000000 rumydata-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-05-11 03:08:49.171013 rumydata-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-11 03:08:41.000000 rumydata-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:08:49.167013 rumydata-1.5.0/rumydata/
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-11 03:08:41.000000 rumydata-1.5.0/rumydata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10180 2024-05-11 03:08:41.000000 rumydata-1.5.0/rumydata/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-05-11 03:08:41.000000 rumydata-1.5.0/rumydata/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12992 2024-05-11 03:08:41.000000 rumydata-1.5.0/rumydata/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-11 03:08:41.000000 rumydata-1.5.0/rumydata/menu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:08:49.167013 rumydata-1.5.0/rumydata/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-11 03:08:41.000000 rumydata-1.5.0/rumydata/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19363 2024-05-11 03:08:41.000000 rumydata-1.5.0/rumydata/rules/cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-11 03:08:41.000000 rumydata-1.5.0/rumydata/rules/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-11 03:08:41.000000 rumydata-1.5.0/rumydata/rules/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-11 03:08:41.000000 rumydata-1.5.0/rumydata/rules/row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-11 03:08:41.000000 rumydata-1.5.0/rumydata/rules/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20934 2024-05-11 03:08:41.000000 rumydata-1.5.0/rumydata/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:08:49.171013 rumydata-1.5.0/rumydata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-05-11 03:08:49.000000 rumydata-1.5.0/rumydata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-11 03:08:49.000000 rumydata-1.5.0/rumydata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 03:08:49.000000 rumydata-1.5.0/rumydata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-11 03:08:49.000000 rumydata-1.5.0/rumydata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-11 03:08:49.000000 rumydata-1.5.0/rumydata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 03:08:49.171013 rumydata-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-11 03:08:41.000000 rumydata-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:08:49.171013 rumydata-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:08:41.000000 rumydata-1.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-11 03:08:41.000000 rumydata-1.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-11 03:08:41.000000 rumydata-1.5.0/tests/test_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-05-11 03:08:41.000000 rumydata-1.5.0/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-05-11 03:08:41.000000 rumydata-1.5.0/tests/test_menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11886 2024-05-11 03:08:41.000000 rumydata-1.5.0/tests/test_other.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-11 03:08:41.000000 rumydata-1.5.0/tests/test_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-11 03:08:41.000000 rumydata-1.5.0/tests/test_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-11 03:08:41.000000 rumydata-1.5.0/tests/test_rules_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14762 2024-05-11 03:08:41.000000 rumydata-1.5.0/tests/test_rules_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-11 03:08:41.000000 rumydata-1.5.0/tests/test_rules_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-11 03:08:41.000000 rumydata-1.5.0/tests/test_rules_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8984 2024-05-11 03:08:41.000000 rumydata-1.5.0/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-11 03:08:41.000000 rumydata-1.5.0/tests/utils.py
```

### Comparing `rumydata-1.4.3/LICENSE` & `rumydata-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rumydata-1.4.3/PKG-INFO` & `rumydata-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rumydata
-Version: 1.4.3
+Version: 1.5.0
 Summary: A python package for validating expectations of text data, and safely reporting exceptions
 Home-page: https://github.com/Mikuana/rumydata
 Author: Christopher Boyd
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `rumydata-1.4.3/README.md` & `rumydata-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `rumydata-1.4.3/rumydata/__init__.py` & `rumydata-1.5.0/rumydata/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,8 +31,8 @@
 
 from rumydata import exception
 from rumydata import field
 from rumydata import rules
 from rumydata.menu import menu
 from rumydata.table import *
 
-__version__ = '1.4.3'
+__version__ = '1.5.0'
```

### Comparing `rumydata-1.4.3/rumydata/_base.py` & `rumydata-1.5.0/rumydata/_base.py`

 * *Files identical despite different names*

### Comparing `rumydata-1.4.3/rumydata/exception.py` & `rumydata-1.5.0/rumydata/exception.py`

 * *Files identical despite different names*

### Comparing `rumydata-1.4.3/rumydata/field.py` & `rumydata-1.5.0/rumydata/field.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 """
 from typing import Union, Tuple, Dict, List
 
 from rumydata import exception as ex
 from rumydata._base import _BaseSubject
 from rumydata.rules import cell as clr, column as cr
 
-__all__ = ['Text', 'Date', 'Currency', 'Digit', 'Integer', 'Choice', 'Ignore', 'Empty']
+__all__ = ['Text', 'Date', 'Currency', 'Digit', 'Integer', 'Choice', 'Ignore',
+           'Empty', 'Number']
 
 
 class Field(_BaseSubject):
     """
     Base Field class
 
     This class provides the framework for the definition of field types in this
@@ -313,14 +314,43 @@
         self.rules.append(clr.MaxDigit(max_length))
 
         if min_length:
             self.descriptors['Min Length'] = f'{str(max_length)} digits'
             self.rules.append(clr.MinDigit(min_length))
 
 
+class Number(Field):
+    """
+    Number field
+
+    A value made up entirely of digits (numbers). A whole number.
+
+    :param max_length: the maximum number of digits
+    :param min_length: (optional) the minimum number of digits
+    :param allow_scientific: (optional) whether to allow scientific notation. Defaults to False.
+    """
+    _default_args = (1,)
+
+    def __init__(self, max_length, min_length=None, allow_scientific=False, **kwargs):
+        super().__init__(**kwargs)
+
+        self.descriptors['Type'] = 'Numeric'
+        self.descriptors['Format'] = f'{"9" * max_length}.{"0"}'
+        self.descriptors['Max Length'] = f'{str(max_length)} digits'
+
+        self.rules.append(clr.CanBeFloat())
+        if allow_scientific is False:
+            self.rules.append(clr.NoScientific())
+        self.rules.append(clr.MaxDigit(max_length))
+
+        if min_length:
+            self.descriptors['Min Length'] = f'{str(max_length)} digits'
+            self.rules.append(clr.MinDigit(min_length))
+
+
 class Choice(Field):
     """
     Choice field
 
     A field with one of a pre-defined set of values.
 
     :param valid_values: a list of values which are considered valid
```

### Comparing `rumydata-1.4.3/rumydata/menu.py` & `rumydata-1.5.0/rumydata/menu.py`

 * *Files identical despite different names*

### Comparing `rumydata-1.4.3/rumydata/rules/__init__.py` & `rumydata-1.5.0/rumydata/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `rumydata-1.4.3/rumydata/rules/cell.py` & `rumydata-1.5.0/rumydata/rules/cell.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     'MinDigit', 'MaxDigit', 'OnlyNumbers', 'NoLeadingZero', 'CanBeFloat',
     'CanBeInteger', 'NumericDecimals', 'LengthComparison', 'LengthGT',
     'LengthGTE', 'LengthET', 'LengthLTE', 'LengthLT', 'NumericComparison',
     'NumericGT', 'NumericGTE', 'NumericET', 'NumericLTE', 'NumericLT',
     'DateRule', 'CanBeDateIso', 'DateGT', 'DateGTE', 'DateET', 'DateLTE',
     'DateLT', 'GreaterThanColumn', 'NotNullIfCompare', 'GreaterThanOrEqualColumn',
     'OtherMustExist', 'OtherCantExist', 'LessThanColumn', 'LessThanOrEqualColumn',
-    'NotNullIfOtherEquals',
+    'NotNullIfOtherEquals', 'NoScientific', 'CanBeFloat',
     'make_static_cell_rule'
 ]
 
 
 class Rule(_BaseRule):
     """ Cell Rule """
 
@@ -251,14 +251,28 @@
     def _evaluator(self):
         return lambda x: bool(re.fullmatch(r'(0|([1-9]\d*))', re.sub(r'[^\d]', '', x)))
 
     def _explain(self) -> str:
         return 'cannot have a leading zero digit'
 
 
+class NoScientific(Rule):
+    """
+    Cell no scientific notation.
+
+    Ensure that there are no scientific notation characters in the cell.
+    """
+
+    def _evaluator(self):
+        return lambda x: bool(re.fullmatch(r'^([+\-\d])[0-9.]*[eE+\-]{1,2}.*$', x)) is False
+
+    def _explain(self) -> str:
+        return 'cannot have scientific notation'
+
+
 class CanBeFloat(Rule):
     """ Cell can be float Rule """
 
     def _evaluator(self):
         def fun(x):
             try:
                 return isinstance(float(x), float)
```

### Comparing `rumydata-1.4.3/rumydata/rules/column.py` & `rumydata-1.5.0/rumydata/rules/column.py`

 * *Files identical despite different names*

### Comparing `rumydata-1.4.3/rumydata/rules/header.py` & `rumydata-1.5.0/rumydata/rules/header.py`

 * *Files identical despite different names*

### Comparing `rumydata-1.4.3/rumydata/rules/row.py` & `rumydata-1.5.0/rumydata/rules/row.py`

 * *Files identical despite different names*

### Comparing `rumydata-1.4.3/rumydata/rules/table.py` & `rumydata-1.5.0/rumydata/rules/table.py`

 * *Files identical despite different names*

### Comparing `rumydata-1.4.3/rumydata/table.py` & `rumydata-1.5.0/rumydata/table.py`

 * *Files identical despite different names*

### Comparing `rumydata-1.4.3/rumydata.egg-info/PKG-INFO` & `rumydata-1.5.0/rumydata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rumydata
-Version: 1.4.3
+Version: 1.5.0
 Summary: A python package for validating expectations of text data, and safely reporting exceptions
 Home-page: https://github.com/Mikuana/rumydata
 Author: Christopher Boyd
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `rumydata-1.4.3/rumydata.egg-info/SOURCES.txt` & `rumydata-1.5.0/rumydata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rumydata-1.4.3/setup.py` & `rumydata-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `rumydata-1.4.3/tests/test_exception.py` & `rumydata-1.5.0/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `rumydata-1.4.3/tests/test_fields.py` & `rumydata-1.5.0/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `rumydata-1.4.3/tests/test_menu.py` & `rumydata-1.5.0/tests/test_menu.py`

 * *Files identical despite different names*

### Comparing `rumydata-1.4.3/tests/test_other.py` & `rumydata-1.5.0/tests/test_other.py`

 * *Files identical despite different names*

### Comparing `rumydata-1.4.3/tests/test_parquet.py` & `rumydata-1.5.0/tests/test_parquet.py`

 * *Files identical despite different names*

### Comparing `rumydata-1.4.3/tests/test_row.py` & `rumydata-1.5.0/tests/test_row.py`

 * *Files identical despite different names*

### Comparing `rumydata-1.4.3/tests/test_rules_base.py` & `rumydata-1.5.0/tests/test_rules_base.py`

 * *Files identical despite different names*

### Comparing `rumydata-1.4.3/tests/test_rules_cell.py` & `rumydata-1.5.0/tests/test_rules_cell.py`

 * *Files 7% similar despite different names*

```diff
@@ -144,15 +144,23 @@
     r = NoLeadingZero()
     assert r._evaluator()(*r._prepare(value)) is expected
 
 
 @pytest.mark.parametrize('value,expected', [
     ('1', True),
     ('0', True),
+    ('0.1', True),
     ('a', False),
+    ('+3', True),
+    ('3.2e23', True),
+    ('-4.70e+9', True),
+    ('-.2E-4', True),
+    ('-7.6603', True),
+    ('+0003 ', True),
+    ('37.e88', True)
 ])
 def test_can_be_float(value: str, expected: bool):
     r = CanBeFloat()
     assert r._evaluator()(*r._prepare(value)) is expected
 
 
 @pytest.mark.parametrize('value,expected', [
@@ -471,7 +479,21 @@
     ('1 ', False),
     (' 1 ', False),
     ('1\t', False),
 ])
 def test_non_trim(value, expected):
     r = NonTrim()
     assert r._evaluator()(*r._prepare(value)) is expected
+
+
+@pytest.mark.parametrize('value, expected', [
+    ('+3', True),
+    ('3.2e23', False),
+    ('-4.70e+9', False),
+    ('-.2E-4', False),
+    ('-7.6603', True),
+    ('+0003 ', True),
+    ('37.e88', False)
+])
+def test_non_scientific(value, expected):
+    r = NoScientific()
+    assert r._evaluator()(*r._prepare(value)) is expected
```

### Comparing `rumydata-1.4.3/tests/test_rules_column.py` & `rumydata-1.5.0/tests/test_rules_column.py`

 * *Files identical despite different names*

### Comparing `rumydata-1.4.3/tests/test_rules_header.py` & `rumydata-1.5.0/tests/test_rules_header.py`

 * *Files identical despite different names*

### Comparing `rumydata-1.4.3/tests/test_table.py` & `rumydata-1.5.0/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `rumydata-1.4.3/tests/utils.py` & `rumydata-1.5.0/tests/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import csv
 import tempfile
 from pathlib import Path
 from typing import List, Union, Tuple
 from unittest.mock import DEFAULT
 
+
 import openpyxl
 
 from rumydata import Layout, CsvFile, ExcelFile
 from rumydata.field import Field
 
 
 def mock_no_module(module: str):
@@ -21,39 +22,41 @@
 
     return func
 
 
 def file_row_harness(row: List[Union[str, int]], layout: dict):
     """ Write row to file for testing in ingest """
     lay = Layout(layout, no_header=True)
-
-    with tempfile.TemporaryDirectory() as d:
-        csv_p = Path(d, 'file_test.csv')
-
-        with csv_p.open('w', newline='') as f:
-            writer = csv.writer(f)
-            writer.writerow(row)
-
-        xl_p = Path(d, 'excel_test.xlsx')
-        wb = openpyxl.Workbook()
-        sheet = wb['Sheet']
-        for ix, value in enumerate(row, start=1):
-            sheet.cell(row=1, column=ix).value = value
-        wb.save(filename=xl_p)
-
-        to_check = [
-            ('CsvFile', CsvFile(lay), csv_p),
-            ('ExcelFile', ExcelFile(lay), xl_p)
-        ]
-        aes = {}
-        for nm, obj, p in to_check:
-            try:
-                assert not obj.check(p)
-            except AssertionError as e:
-                aes[nm] = e
-        new_line = '\n'
+    try:
+        with tempfile.TemporaryDirectory() as d:
+            csv_p = Path(d, 'file_test.csv')
+
+            with csv_p.open('w', newline='') as f:
+                writer = csv.writer(f)
+                writer.writerow(row)
+
+            xl_p = Path(d, 'excel_test.xlsx')
+            wb = openpyxl.Workbook()
+            sheet = wb['Sheet']
+            for ix, value in enumerate(row, start=1):
+                sheet.cell(row=1, column=ix).value = value
+            wb.save(filename=xl_p)
+
+            to_check = [
+                ('CsvFile', CsvFile(lay), csv_p),
+                ('ExcelFile', ExcelFile(lay), xl_p)
+            ]
+            aes = {}
+            for nm, obj, p in to_check:
+                try:
+                    assert not obj.check(p)
+                except AssertionError as e:
+                    aes[nm] = e
+            new_line = '\n'
+        assert not aes, f'Write test failed for:\n {new_line.join([f"{k}:{v}" for k, v in aes.items()])}'
+    except PermissionError:
         assert not aes, f'Write test failed for:\n {new_line.join([f"{k}:{v}" for k, v in aes.items()])}'
 
 
 def file_cell_harness(value: str, field: Field):
     """ Wrapper to convert cell to row for harness check """
     file_row_harness(row=[value], layout={'c1': field})
```

