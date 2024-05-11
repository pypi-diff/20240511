# Comparing `tmp/mtg_card_api-0.1.3.tar.gz` & `tmp/mtg_card_api-0.1.4.tar.gz`

## Comparing `mtg_card_api-0.1.3.tar` & `mtg_card_api-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0      155 2020-02-02 00:00:00.000000 mtg_card_api-0.1.3/main.py
--rwxr-xr-x   0        0        0      121 2020-02-02 00:00:00.000000 mtg_card_api-0.1.3/src/mtg_card_api/__init__.py
--rwxr-xr-x   0        0        0      149 2020-02-02 00:00:00.000000 mtg_card_api-0.1.3/src/mtg_card_api/_utils.py
--rwxr-xr-x   0        0        0     4278 2020-02-02 00:00:00.000000 mtg_card_api-0.1.3/src/mtg_card_api/mtg_scryfall_api.py
--rwxr-xr-x   0        0        0     3078 2020-02-02 00:00:00.000000 mtg_card_api-0.1.3/.gitignore
--rwxr-xr-x   0        0        0     1069 2020-02-02 00:00:00.000000 mtg_card_api-0.1.3/LICENSE
--rwxr-xr-x   0        0        0      912 2020-02-02 00:00:00.000000 mtg_card_api-0.1.3/README.md
--rwxr-xr-x   0        0        0      649 2020-02-02 00:00:00.000000 mtg_card_api-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 mtg_card_api-0.1.3/PKG-INFO
+-rwxr-xr-x   0        0        0      155 2020-02-02 00:00:00.000000 mtg_card_api-0.1.4/main.py
+-rwxr-xr-x   0        0        0      121 2020-02-02 00:00:00.000000 mtg_card_api-0.1.4/src/mtg_card_api/__init__.py
+-rwxr-xr-x   0        0        0      149 2020-02-02 00:00:00.000000 mtg_card_api-0.1.4/src/mtg_card_api/_utils.py
+-rwxr-xr-x   0        0        0     4253 2020-02-02 00:00:00.000000 mtg_card_api-0.1.4/src/mtg_card_api/mtg_scryfall_api.py
+-rwxr-xr-x   0        0        0     3078 2020-02-02 00:00:00.000000 mtg_card_api-0.1.4/.gitignore
+-rwxr-xr-x   0        0        0     1069 2020-02-02 00:00:00.000000 mtg_card_api-0.1.4/LICENSE
+-rwxr-xr-x   0        0        0      912 2020-02-02 00:00:00.000000 mtg_card_api-0.1.4/README.md
+-rwxr-xr-x   0        0        0      649 2020-02-02 00:00:00.000000 mtg_card_api-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 mtg_card_api-0.1.4/PKG-INFO
```

### Comparing `mtg_card_api-0.1.3/src/mtg_card_api/mtg_scryfall_api.py` & `mtg_card_api-0.1.4/src/mtg_card_api/mtg_scryfall_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         Args:
             card_name (str): Exact string oracle id of a card
 
         Returns:
             R: Full search result
         """
         return self._run_get(
-            'https://api.scryfall.com/cards/search',
+            'cards/search',
             {
                 'q': f'oracle_id={oracle_id}',
                 'unique': 'prints'
             },
             oracle_id,
             'cache/variants'
         )
```

### Comparing `mtg_card_api-0.1.3/.gitignore` & `mtg_card_api-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `mtg_card_api-0.1.3/LICENSE` & `mtg_card_api-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mtg_card_api-0.1.3/README.md` & `mtg_card_api-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mtg_card_api-0.1.3/pyproject.toml` & `mtg_card_api-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "hatchling",
 ]
 build-backend = "hatchling.build"
 [project]
 name = "mtg_card_api"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
     { name = "Samuel Shiels" },
 ]
 description = "An unofficial wrapper for the Scryfall REST API providing common queries"
 readme = "README.md"
 requires-python = ">=3.12.2"
 classifiers = [
```

### Comparing `mtg_card_api-0.1.3/PKG-INFO` & `mtg_card_api-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mtg_card_api
-Version: 0.1.3
+Version: 0.1.4
 Summary: An unofficial wrapper for the Scryfall REST API providing common queries
 Author: Samuel Shiels
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Other Environment
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

