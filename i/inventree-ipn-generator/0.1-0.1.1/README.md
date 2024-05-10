# Comparing `tmp/inventree-ipn-generator-0.1.tar.gz` & `tmp/inventree_ipn_generator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inventree-ipn-generator-0.1.tar", last modified: Thu Mar 21 20:08:52 2024, max compression
+gzip compressed data, was "inventree_ipn_generator-0.1.1.tar", last modified: Fri May 10 23:23:42 2024, max compression
```

## Comparing `inventree-ipn-generator-0.1.tar` & `inventree_ipn_generator-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 20:08:52.547988 inventree-ipn-generator-0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-21 20:08:47.000000 inventree-ipn-generator-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-03-21 20:08:52.547988 inventree-ipn-generator-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-03-21 20:08:47.000000 inventree-ipn-generator-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 20:08:52.547988 inventree-ipn-generator-0.1/inventree_ipn_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-03-21 20:08:52.000000 inventree-ipn-generator-0.1/inventree_ipn_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-21 20:08:52.000000 inventree-ipn-generator-0.1/inventree_ipn_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 20:08:52.000000 inventree-ipn-generator-0.1/inventree_ipn_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-21 20:08:52.000000 inventree-ipn-generator-0.1/inventree_ipn_generator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-21 20:08:52.000000 inventree-ipn-generator-0.1/inventree_ipn_generator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 20:08:52.547988 inventree-ipn-generator-0.1/ipn_generator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 20:08:47.000000 inventree-ipn-generator-0.1/ipn_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-03-21 20:08:47.000000 inventree-ipn-generator-0.1/ipn_generator/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 20:08:52.547988 inventree-ipn-generator-0.1/ipn_generator/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 20:08:47.000000 inventree-ipn-generator-0.1/ipn_generator/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13247 2024-03-21 20:08:47.000000 inventree-ipn-generator-0.1/ipn_generator/tests/test_IPNGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-21 20:08:47.000000 inventree-ipn-generator-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 20:08:52.547988 inventree-ipn-generator-0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:23:42.554019 inventree_ipn_generator-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-10 23:23:36.000000 inventree_ipn_generator-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-05-10 23:23:42.550019 inventree_ipn_generator-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-10 23:23:36.000000 inventree_ipn_generator-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:23:42.550019 inventree_ipn_generator-0.1.1/inventree_ipn_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-05-10 23:23:42.000000 inventree_ipn_generator-0.1.1/inventree_ipn_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-10 23:23:42.000000 inventree_ipn_generator-0.1.1/inventree_ipn_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 23:23:42.000000 inventree_ipn_generator-0.1.1/inventree_ipn_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-10 23:23:42.000000 inventree_ipn_generator-0.1.1/inventree_ipn_generator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 23:23:42.000000 inventree_ipn_generator-0.1.1/inventree_ipn_generator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:23:42.550019 inventree_ipn_generator-0.1.1/ipn_generator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 23:23:36.000000 inventree_ipn_generator-0.1.1/ipn_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8754 2024-05-10 23:23:36.000000 inventree_ipn_generator-0.1.1/ipn_generator/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:23:42.550019 inventree_ipn_generator-0.1.1/ipn_generator/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 23:23:36.000000 inventree_ipn_generator-0.1.1/ipn_generator/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13247 2024-05-10 23:23:36.000000 inventree_ipn_generator-0.1.1/ipn_generator/tests/test_IPNGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-10 23:23:36.000000 inventree_ipn_generator-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 23:23:42.554019 inventree_ipn_generator-0.1.1/setup.cfg
```

### Comparing `inventree-ipn-generator-0.1/LICENSE` & `inventree_ipn_generator-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inventree-ipn-generator-0.1/PKG-INFO` & `inventree_ipn_generator-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventree-ipn-generator
-Version: 0.1
+Version: 0.1.1
 Summary: InvenTree plugin to automatically generate and assign Internal Part Numbers to parts
 Author-email: Nichlas Walsøe <lavissawow@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Nichlas Walsøe
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -62,25 +62,35 @@
 ## Pattern
 Part Number patterns follow three basic groups. Literals, Numerics, and characters.
 When incrementing a part number, the rightmost group that is mutable will be incremented.
 All groups can be combined in any order.
 
 A pattern cannot consist of _only_ Literals.
 
+For any pattern, only the rightmost non-literal group will be incremented.
+When this group rolls over its max, the next non-literal group to the left will be incremented.
+Example: Given the groups (named for demo): L1C1N1C2L2
+Incrementing follows this order: C2, N1, C1.
+
+> **_NOTE:_** When C1 in the above example rolls over, the plugin will loop back to the first IPN.
+> This will cause duplicate IPNs if your InvenTree allows duplicate IPNs.
+> If your InvenTree does not allow duplicate IPNs, this will cause an error at the moment!
+> This will be addressed in an upcoming update.
+
 ### Literals (Immutable)
 Anything encased in `()` will be rendered as-is. no change will be made to anything within.
 
 Example: `(A6C)` will _always_ render as "A6C", regardless of other groups
 
 ### Numeric
 Numbers that should change over time should be encased in `{}`
 - `{5}` respresents a number with max 5 digits
 - `{25+}` represents a number 25-99
 
-Example: `{5+}{3}` will result in this range: 5000-5999
+Example: `{5+}{3}` will result in this range: 5000-9999
 
 ### Characters
 Characters that change should be encased in `[]`
 - `[abc]` represents looping through the letters `a`, `b`, `c` in order.
 - `[a-f]` represents looping through the letters from `a` to `f` alphabetaically
 
 These two directives can be combined.
```

### Comparing `inventree-ipn-generator-0.1/README.md` & `inventree_ipn_generator-0.1.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -27,25 +27,35 @@
 ## Pattern
 Part Number patterns follow three basic groups. Literals, Numerics, and characters.
 When incrementing a part number, the rightmost group that is mutable will be incremented.
 All groups can be combined in any order.
 
 A pattern cannot consist of _only_ Literals.
 
+For any pattern, only the rightmost non-literal group will be incremented.
+When this group rolls over its max, the next non-literal group to the left will be incremented.
+Example: Given the groups (named for demo): L1C1N1C2L2
+Incrementing follows this order: C2, N1, C1.
+
+> **_NOTE:_** When C1 in the above example rolls over, the plugin will loop back to the first IPN.
+> This will cause duplicate IPNs if your InvenTree allows duplicate IPNs.
+> If your InvenTree does not allow duplicate IPNs, this will cause an error at the moment!
+> This will be addressed in an upcoming update.
+
 ### Literals (Immutable)
 Anything encased in `()` will be rendered as-is. no change will be made to anything within.
 
 Example: `(A6C)` will _always_ render as "A6C", regardless of other groups
 
 ### Numeric
 Numbers that should change over time should be encased in `{}`
 - `{5}` respresents a number with max 5 digits
 - `{25+}` represents a number 25-99
 
-Example: `{5+}{3}` will result in this range: 5000-5999
+Example: `{5+}{3}` will result in this range: 5000-9999
 
 ### Characters
 Characters that change should be encased in `[]`
 - `[abc]` represents looping through the letters `a`, `b`, `c` in order.
 - `[a-f]` represents looping through the letters from `a` to `f` alphabetaically
 
 These two directives can be combined.
```

### Comparing `inventree-ipn-generator-0.1/inventree_ipn_generator.egg-info/PKG-INFO` & `inventree_ipn_generator-0.1.1/inventree_ipn_generator.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventree-ipn-generator
-Version: 0.1
+Version: 0.1.1
 Summary: InvenTree plugin to automatically generate and assign Internal Part Numbers to parts
 Author-email: Nichlas Walsøe <lavissawow@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Nichlas Walsøe
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -62,25 +62,35 @@
 ## Pattern
 Part Number patterns follow three basic groups. Literals, Numerics, and characters.
 When incrementing a part number, the rightmost group that is mutable will be incremented.
 All groups can be combined in any order.
 
 A pattern cannot consist of _only_ Literals.
 
+For any pattern, only the rightmost non-literal group will be incremented.
+When this group rolls over its max, the next non-literal group to the left will be incremented.
+Example: Given the groups (named for demo): L1C1N1C2L2
+Incrementing follows this order: C2, N1, C1.
+
+> **_NOTE:_** When C1 in the above example rolls over, the plugin will loop back to the first IPN.
+> This will cause duplicate IPNs if your InvenTree allows duplicate IPNs.
+> If your InvenTree does not allow duplicate IPNs, this will cause an error at the moment!
+> This will be addressed in an upcoming update.
+
 ### Literals (Immutable)
 Anything encased in `()` will be rendered as-is. no change will be made to anything within.
 
 Example: `(A6C)` will _always_ render as "A6C", regardless of other groups
 
 ### Numeric
 Numbers that should change over time should be encased in `{}`
 - `{5}` respresents a number with max 5 digits
 - `{25+}` represents a number 25-99
 
-Example: `{5+}{3}` will result in this range: 5000-5999
+Example: `{5+}{3}` will result in this range: 5000-9999
 
 ### Characters
 Characters that change should be encased in `[]`
 - `[abc]` represents looping through the letters `a`, `b`, `c` in order.
 - `[a-f]` represents looping through the letters from `a` to `f` alphabetaically
 
 These two directives can be combined.
```

### Comparing `inventree-ipn-generator-0.1/ipn_generator/generator.py` & `inventree_ipn_generator-0.1.1/ipn_generator/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from django.core.exceptions import ValidationError
 
 import logging
 import re
 
 logger = logging.getLogger("inventree")
 
+PERMITTED_SPECIAL_LITERALS = "\-.:/\\"
+
 
 def validate_pattern(pattern):
     """Validates pattern groups"""
     regex = re.compile(r"(\{\d+\+?\})|(\[(?!\w\])(?:\w+|(?:\w-\w)+)+\])")
     if not regex.search(pattern):
         raise ValidationError("Pattern must include more than Literals")
 
@@ -114,15 +116,15 @@
     def construct_regex(self, disable_groups=False):
         """Constructs a valid regex from provided IPN pattern.
         This regex is used to find the latest assigned IPN
         """
         regex = "^"
 
         m = re.findall(
-            r"(\{\d+\+?\})|(\([\w\(\)]+\))|(\[(?:\w+|\w-\w)+\])",
+            r"(\{\d+\+?\})|(\([\w\(\)\-.:/\\]+\))|(\[(?:\w+|\w-\w)+\])",
             self.get_setting("PATTERN"),
         )
 
         for idx, group in enumerate(m):
             numeric, literal, character = group
             # Numeric, increment
             if numeric:
@@ -244,15 +246,15 @@
 
         ipn_list.reverse()
         return "".join(ipn_list)
 
     def construct_first_ipn(self):
         """No IPNs matching the pattern were found. Constructing the first IPN."""
         m = re.findall(
-            r"(\{\d+\+?\})|(\([\w\(\)]+\))|(\[(?:\w+|(?:\w-\w)+)\])",
+            r"(\{\d+\+?\})|(\([\w\(\)\-.:/\\]+\))|(\[(?:\w+|(?:\w-\w)+)\])",
             self.get_setting("PATTERN"),
         )
 
         ipn = ""
 
         for group in m:
             numeric, literal, character = group
```

### Comparing `inventree-ipn-generator-0.1/ipn_generator/tests/test_IPNGenerator.py` & `inventree_ipn_generator-0.1.1/ipn_generator/tests/test_IPNGenerator.py`

 * *Files identical despite different names*

### Comparing `inventree-ipn-generator-0.1/pyproject.toml` & `inventree_ipn_generator-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "inventree-ipn-generator"
-version = "0.1"
+version = "0.1.1"
 description = "InvenTree plugin to automatically generate and assign Internal Part Numbers to parts"
 authors = [
     {name = "Nichlas Walsøe", email = "lavissawow@gmail.com"}
 ]
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 classifiers = [
```

