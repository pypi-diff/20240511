# Comparing `tmp/statute_utils-0.6.8.tar.gz` & `tmp/statute-utils-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statute_utils-0.6.8.tar", max compression
+gzip compressed data, was "statute-utils-0.6.9.tar", last modified: Sun Feb 18 09:56:42 2024, max compression
```

## Comparing `statute_utils-0.6.8.tar` & `statute-utils-0.6.9.tar`

### file list

```diff
@@ -1,29 +1,41 @@
--rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.6.8/LICENSE
--rw-r--r--   0        0        0     2825 2023-07-31 16:21:33.481263 statute_utils-0.6.8/README.md
--rw-r--r--   0        0        0     1461 2023-08-08 02:44:55.650236 statute_utils-0.6.8/pyproject.toml
--rw-r--r--   0        0        0      897 2023-07-29 18:29:16.464915 statute_utils-0.6.8/statute_utils/__init__.py
--rw-r--r--   0        0        0     3506 2023-08-08 02:43:41.966962 statute_utils-0.6.8/statute_utils/codification.py
--rw-r--r--   0        0        0      588 2023-07-16 08:01:39.314430 statute_utils-0.6.8/statute_utils/components/__init__.py
--rw-r--r--   0        0        0     6011 2023-07-29 18:29:59.938432 statute_utils-0.6.8/statute_utils/components/branch.py
--rw-r--r--   0        0        0     9721 2023-07-30 10:35:07.925035 statute_utils-0.6.8/statute_utils/components/builder.py
--rw-r--r--   0        0        0    15560 2023-08-07 10:54:20.469809 statute_utils-0.6.8/statute_utils/components/category.py
--rw-r--r--   0        0        0     2015 2023-07-01 04:37:03.664929 statute_utils-0.6.8/statute_utils/components/short.py
--rw-r--r--   0        0        0     3717 2023-07-16 05:41:42.450594 statute_utils-0.6.8/statute_utils/components/utils.py
--rw-r--r--   0        0        0     1288 2023-07-17 01:57:30.575440 statute_utils-0.6.8/statute_utils/config.py
--rw-r--r--   0        0        0     9858 2023-07-17 02:00:05.382207 statute_utils-0.6.8/statute_utils/main.py
--rw-r--r--   0        0        0     4170 2023-07-17 01:57:45.971391 statute_utils-0.6.8/statute_utils/models.py
--rw-r--r--   0        0        0     9892 2023-07-02 03:43:37.827535 statute_utils-0.6.8/statute_utils/models_names.py
--rw-r--r--   0        0        0     6699 2023-07-02 03:43:23.216281 statute_utils-0.6.8/statute_utils/models_serials.py
--rw-r--r--   0        0        0      249 2023-07-01 04:12:57.597987 statute_utils-0.6.8/statute_utils/recipes/__init__.py
--rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.6.8/statute_utils/recipes/const.py
--rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.6.8/statute_utils/recipes/digits.py
--rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.6.8/statute_utils/recipes/roc.py
--rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.6.8/statute_utils/recipes/spain.py
--rw-r--r--   0        0        0     7519 2023-08-08 02:41:49.319929 statute_utils-0.6.8/statute_utils/statute.py
--rw-r--r--   0        0        0     1851 2023-07-16 08:51:22.676004 statute_utils-0.6.8/statute_utils/templater.py
--rw-r--r--   0        0        0      208 2023-07-16 07:34:21.108245 statute_utils-0.6.8/statute_utils/templates/crumbs.html
--rw-r--r--   0        0        0      164 2023-07-16 07:29:47.336036 statute_utils-0.6.8/statute_utils/templates/paragraph.html
--rw-r--r--   0        0        0      200 2023-07-16 07:34:28.065021 statute_utils-0.6.8/statute_utils/templates/subtree.html
--rw-r--r--   0        0        0     1117 2023-07-16 09:00:07.666662 statute_utils-0.6.8/statute_utils/templates/tree.css
--rw-r--r--   0        0        0     3043 2023-07-31 18:24:05.729977 statute_utils-0.6.8/statute_utils/templates/tree.html
--rw-r--r--   0        0        0     3752 1970-01-01 00:00:00.000000 statute_utils-0.6.8/PKG-INFO
+drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-02-18 09:56:42.034749 statute-utils-0.6.9/
+-rw-r--r--   0 mv         (501) staff       (20)     1491 2023-06-21 15:08:07.000000 statute-utils-0.6.9/LICENSE
+-rw-r--r--   0 mv         (501) staff       (20)      886 2024-02-18 09:56:42.034339 statute-utils-0.6.9/PKG-INFO
+-rw-r--r--   0 mv         (501) staff       (20)     2824 2024-02-18 09:51:33.000000 statute-utils-0.6.9/README.md
+-rw-r--r--   0 mv         (501) staff       (20)     1009 2024-02-18 09:53:52.000000 statute-utils-0.6.9/pyproject.toml
+-rw-r--r--   0 mv         (501) staff       (20)       38 2024-02-18 09:56:42.034826 statute-utils-0.6.9/setup.cfg
+drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-02-18 09:56:42.011119 statute-utils-0.6.9/src/
+drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-02-18 09:56:42.019366 statute-utils-0.6.9/src/statute_utils/
+-rw-r--r--   0 mv         (501) staff       (20)      897 2023-07-29 18:29:16.000000 statute-utils-0.6.9/src/statute_utils/__init__.py
+-rw-r--r--   0 mv         (501) staff       (20)     3830 2024-02-18 09:49:29.000000 statute-utils-0.6.9/src/statute_utils/codification.py
+drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-02-18 09:56:42.028750 statute-utils-0.6.9/src/statute_utils/components/
+-rw-r--r--   0 mv         (501) staff       (20)      636 2024-02-18 09:39:58.000000 statute-utils-0.6.9/src/statute_utils/components/__init__.py
+-rw-r--r--   0 mv         (501) staff       (20)     7261 2024-02-18 09:39:51.000000 statute-utils-0.6.9/src/statute_utils/components/branch.py
+-rw-r--r--   0 mv         (501) staff       (20)     9721 2023-07-30 10:35:07.000000 statute-utils-0.6.9/src/statute_utils/components/builder.py
+-rw-r--r--   0 mv         (501) staff       (20)    15560 2023-08-07 10:54:20.000000 statute-utils-0.6.9/src/statute_utils/components/category.py
+-rw-r--r--   0 mv         (501) staff       (20)     2015 2023-07-01 04:37:03.000000 statute-utils-0.6.9/src/statute_utils/components/short.py
+-rw-r--r--   0 mv         (501) staff       (20)     3717 2023-07-16 05:41:42.000000 statute-utils-0.6.9/src/statute_utils/components/utils.py
+-rw-r--r--   0 mv         (501) staff       (20)     1288 2023-07-17 01:57:30.000000 statute-utils-0.6.9/src/statute_utils/config.py
+-rw-r--r--   0 mv         (501) staff       (20)     9858 2023-07-17 02:00:05.000000 statute-utils-0.6.9/src/statute_utils/main.py
+-rw-r--r--   0 mv         (501) staff       (20)     4136 2023-09-22 08:06:03.000000 statute-utils-0.6.9/src/statute_utils/models.py
+-rw-r--r--   0 mv         (501) staff       (20)     9904 2024-02-18 09:51:05.000000 statute-utils-0.6.9/src/statute_utils/models_names.py
+-rw-r--r--   0 mv         (501) staff       (20)     6699 2023-07-02 03:43:23.000000 statute-utils-0.6.9/src/statute_utils/models_serials.py
+drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-02-18 09:56:42.030922 statute-utils-0.6.9/src/statute_utils/recipes/
+-rw-r--r--   0 mv         (501) staff       (20)      249 2023-07-01 04:12:57.000000 statute-utils-0.6.9/src/statute_utils/recipes/__init__.py
+-rw-r--r--   0 mv         (501) staff       (20)      380 2023-06-22 05:28:27.000000 statute-utils-0.6.9/src/statute_utils/recipes/const.py
+-rw-r--r--   0 mv         (501) staff       (20)     2649 2023-06-22 05:28:27.000000 statute-utils-0.6.9/src/statute_utils/recipes/digits.py
+-rw-r--r--   0 mv         (501) staff       (20)      311 2023-06-22 05:28:27.000000 statute-utils-0.6.9/src/statute_utils/recipes/roc.py
+-rw-r--r--   0 mv         (501) staff       (20)      667 2023-06-22 05:28:27.000000 statute-utils-0.6.9/src/statute_utils/recipes/spain.py
+-rw-r--r--   0 mv         (501) staff       (20)     7519 2023-08-08 02:41:49.000000 statute-utils-0.6.9/src/statute_utils/statute.py
+-rw-r--r--   0 mv         (501) staff       (20)     1851 2023-07-16 08:51:22.000000 statute-utils-0.6.9/src/statute_utils/templater.py
+drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-02-18 09:56:42.032780 statute-utils-0.6.9/src/statute_utils.egg-info/
+-rw-r--r--   0 mv         (501) staff       (20)      886 2024-02-18 09:56:42.000000 statute-utils-0.6.9/src/statute_utils.egg-info/PKG-INFO
+-rw-r--r--   0 mv         (501) staff       (20)     1012 2024-02-18 09:56:42.000000 statute-utils-0.6.9/src/statute_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 mv         (501) staff       (20)        1 2024-02-18 09:56:42.000000 statute-utils-0.6.9/src/statute_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 mv         (501) staff       (20)      299 2024-02-18 09:56:42.000000 statute-utils-0.6.9/src/statute_utils.egg-info/requires.txt
+-rw-r--r--   0 mv         (501) staff       (20)       14 2024-02-18 09:56:42.000000 statute-utils-0.6.9/src/statute_utils.egg-info/top_level.txt
+drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-02-18 09:56:42.032373 statute-utils-0.6.9/tests/
+-rw-r--r--   0 mv         (501) staff       (20)     1610 2024-02-18 09:30:22.000000 statute-utils-0.6.9/tests/test_history.py
+-rw-r--r--   0 mv         (501) staff       (20)     5014 2024-02-18 09:30:22.000000 statute-utils-0.6.9/tests/test_html.py
+-rw-r--r--   0 mv         (501) staff       (20)     3833 2024-02-18 09:30:22.000000 statute-utils-0.6.9/tests/test_main.py
+-rw-r--r--   0 mv         (501) staff       (20)      671 2023-07-17 02:01:54.000000 statute-utils-0.6.9/tests/test_validations.py
```

### Comparing `statute_utils-0.6.8/LICENSE` & `statute-utils-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.8/README.md` & `statute-utils-0.6.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,21 +6,19 @@
 
 ## Documentation
 
 See [documentation](https://justmars.github.io/statute-utils).
 
 ## Development
 
-Checkout code, create a new virtual environment:
+## Todo
 
-```sh
-poetry add statute-utils # python -m pip install statute-utils
-poetry update # install dependencies
-poetry shell
-```
+- [ ] Detect Family Code, see gr/227728/2022-09-28/main-193.md
+- [ ] Detect Penal Code with `REV. PEN. CODE, Art. 308:`, gr/224316/2021-11-10/main-180.md
+- [ ] Provision matching
 
 ## Some unit patterns
 
 ```json title="Convention used when desiring to exclude appropriation laws."
 {
   "units": [
     {
@@ -43,19 +41,20 @@
 ## Use in Datasette
 
 ### Add units to a database from a pre-made file
 
 Consider an example `db.sqlite`:
 
 ```py title="Assumes path-to-file.yml exists"
->>> from sqlite_utils import Database
->>> from statute_utils import Statute
->>> f = Path().joinpath(path-to-file.yml)
->>> db = Database('db.sqlite')
->>> db["statutes"].insert(Statute.from_file(f).make_row())
+from sqlite_utils import Database
+from statute_utils import Statute
+
+f = Path().joinpath(path - to - file.yml)
+db = Database("db.sqlite")
+db["statutes"].insert(Statute.from_file(f).make_row())
 # this will contain an 'html' column containing a semantic tree structure that can be styled via css
 ```
 
 ### Copy html/css files
 
 1. `tree.html` - Tree-building macros (which can be used for creating an html tree to represent the statute)
 2. `tree.css` - Sample css rulesets to use for the tree generated with the macros
@@ -106,14 +105,13 @@
 
 ```jinja
 datasette serve db.sqlite --plugins-dir=app/plugins/ {# plus the other arguments #}...
 ```
 
 It becomes possible to use custom functions and filters found in `tree.py`.
 
-
 ## Changes
 
 1. em / strong no longer with label
 2. Need to add href on <a.label/>
 3. `span.par-branch` converted to `a.par-branch`
 4. <li#id> and <span#id> changed to <a[data-slug]/>
```

### Comparing `statute_utils-0.6.8/statute_utils/__init__.py` & `statute-utils-0.6.9/src/statute_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.8/statute_utils/codification.py` & `statute-utils-0.6.9/src/statute_utils/codification.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import yaml  # type: ignore
 from dateutil.parser import parse  # type: ignore
 
 from .components import (
     create_fts_snippet_column,
     create_unit_heading,
+    fetch_values_from_key,
     set_node_ids,
     walk,
 )
 from .main import extract_rule
 from .models import Rule
 from .templater import html_tree_from_hierarchy
 
@@ -111,7 +112,15 @@
                 "item": unit.get("item"),
                 "caption": unit.get("caption"),
                 "content": unit.get("content"),
                 "snippetable": create_fts_snippet_column(unit),  # enable searchability
             }
             if subunits := unit.get("units"):
                 yield from cls.flatten_units(codification_id, subunits, present_heading)
+
+    def extract_events(self):
+        """Each unit in a codification may contain a history."""
+        data = {"units": self.units}
+        histories = fetch_values_from_key(data=data, key="history")
+        for history in histories:
+            for event in history:
+                yield event
```

### Comparing `statute_utils-0.6.8/statute_utils/components/__init__.py` & `statute-utils-0.6.9/src/statute_utils/components/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,14 @@
-from .branch import make_branch, make_branch_json_array, set_node_ids, walk
+from .branch import (
+    fetch_values_from_key,
+    make_branch,
+    make_branch_json_array,
+    set_node_ids,
+    walk,
+)
 from .builder import (
     TREE_FILTERS,
     crumb,
     from_json,
     from_mp,
     is_excluded,
     is_first_par,
```

### Comparing `statute_utils-0.6.8/statute_utils/components/branch.py` & `statute-utils-0.6.9/src/statute_utils/components/branch.py`

 * *Files 22% similar despite different names*

```diff
@@ -174,7 +174,45 @@
                 data.append(("content", formatted_content))
 
             if node.get("units", None):
                 walked_units = walk(node["units"])
                 data.append(("units", walked_units))
             revised_nodes.append(dict(data))
     return revised_nodes
+
+
+def fetch_values_from_key(data: dict, key: str):
+    """Stack based function applicable to nested dictionaries to yield values
+    that match the key; e.g. `fetch_values_from_key(data, "history")` will go
+    through the nested dictionary searching for the "history" key.
+
+    Args:
+        data (dict): The nested dictionary
+        key (str): The key of the nested dictionary
+
+    Yields:
+        Iterator: [description]
+    """
+    stack = [data]
+
+    while stack:
+        # remove from stack
+        evaluate_data = stack.pop()
+
+        # yield if the key value pair is found
+        if (
+            not isinstance(evaluate_data, str)
+            and key in evaluate_data
+            and evaluate_data[key] is not None
+        ):
+            yield evaluate_data[key]
+
+        # continue if the data being evaluated is a string;
+        # if not, determine whether a list or a dict
+        # if a dict, add the dictionary to the stacked list to evaluate later
+        # if a list, extend the stacked list
+        if not isinstance(evaluate_data, str):
+            for v in evaluate_data.values():
+                if isinstance(v, dict):
+                    stack.append(v)
+                if isinstance(v, list):
+                    stack += v
```

### Comparing `statute_utils-0.6.8/statute_utils/components/builder.py` & `statute-utils-0.6.9/src/statute_utils/components/builder.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.8/statute_utils/components/category.py` & `statute-utils-0.6.9/src/statute_utils/components/category.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.8/statute_utils/components/short.py` & `statute-utils-0.6.9/src/statute_utils/components/short.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.8/statute_utils/components/utils.py` & `statute-utils-0.6.9/src/statute_utils/components/utils.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.8/statute_utils/config.py` & `statute-utils-0.6.9/src/statute_utils/config.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.8/statute_utils/main.py` & `statute-utils-0.6.9/src/statute_utils/main.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.8/statute_utils/models.py` & `statute-utils-0.6.9/src/statute_utils/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from collections.abc import Iterator
 from dataclasses import dataclass
 from functools import cached_property
 from re import Pattern
 from typing import NamedTuple
 
 from slugify import slugify
-from sqlite_utils import Database
 
 from .components import StatuteSerialCategory, make_regex_readable
 from .config import get_local_statute_db
 
 
 @dataclass(frozen=True)
 class Rule:
```

### Comparing `statute_utils-0.6.8/statute_utils/models_names.py` & `statute-utils-0.6.9/src/statute_utils/models_names.py`

 * *Files 0% similar despite different names*

```diff
@@ -395,14 +395,15 @@
                 Accountability|ACCOUNTABILITY
             )?
 """
 
 STYLES_NAMED: list[NamedPattern] = [
     admin,
     civ,
+    family,
     rpc,
     corp,
     labor,
     locgov,
     prof_responsibility,
     const,
     roc,
```

### Comparing `statute_utils-0.6.8/statute_utils/models_serials.py` & `statute-utils-0.6.9/src/statute_utils/models_serials.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.8/statute_utils/recipes/digits.py` & `statute-utils-0.6.9/src/statute_utils/recipes/digits.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.8/statute_utils/recipes/spain.py` & `statute-utils-0.6.9/src/statute_utils/recipes/spain.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.8/statute_utils/statute.py` & `statute-utils-0.6.9/src/statute_utils/statute.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.8/statute_utils/templater.py` & `statute-utils-0.6.9/src/statute_utils/templater.py`

 * *Files identical despite different names*

