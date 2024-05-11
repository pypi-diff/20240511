# Comparing `tmp/mtg_card_api-0.1.1.tar.gz` & `tmp/mtg_card_api-0.1.2.tar.gz`

## Comparing `mtg_card_api-0.1.1.tar` & `mtg_card_api-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0      155 2020-02-02 00:00:00.000000 mtg_card_api-0.1.1/main.py
--rwxr-xr-x   0        0        0      121 2020-02-02 00:00:00.000000 mtg_card_api-0.1.1/src/mtg_card_api/__init__.py
--rwxr-xr-x   0        0        0      149 2020-02-02 00:00:00.000000 mtg_card_api-0.1.1/src/mtg_card_api/_utils.py
--rwxr-xr-x   0        0        0     3754 2020-02-02 00:00:00.000000 mtg_card_api-0.1.1/src/mtg_card_api/mtg_scryfall_api.py
--rwxr-xr-x   0        0        0     3078 2020-02-02 00:00:00.000000 mtg_card_api-0.1.1/.gitignore
--rwxr-xr-x   0        0        0     1069 2020-02-02 00:00:00.000000 mtg_card_api-0.1.1/LICENSE
--rwxr-xr-x   0        0        0      912 2020-02-02 00:00:00.000000 mtg_card_api-0.1.1/README.md
--rwxr-xr-x   0        0        0      649 2020-02-02 00:00:00.000000 mtg_card_api-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 mtg_card_api-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0      155 2020-02-02 00:00:00.000000 mtg_card_api-0.1.2/main.py
+-rwxr-xr-x   0        0        0      121 2020-02-02 00:00:00.000000 mtg_card_api-0.1.2/src/mtg_card_api/__init__.py
+-rwxr-xr-x   0        0        0      149 2020-02-02 00:00:00.000000 mtg_card_api-0.1.2/src/mtg_card_api/_utils.py
+-rwxr-xr-x   0        0        0     4280 2020-02-02 00:00:00.000000 mtg_card_api-0.1.2/src/mtg_card_api/mtg_scryfall_api.py
+-rwxr-xr-x   0        0        0     3078 2020-02-02 00:00:00.000000 mtg_card_api-0.1.2/.gitignore
+-rwxr-xr-x   0        0        0     1069 2020-02-02 00:00:00.000000 mtg_card_api-0.1.2/LICENSE
+-rwxr-xr-x   0        0        0      912 2020-02-02 00:00:00.000000 mtg_card_api-0.1.2/README.md
+-rwxr-xr-x   0        0        0      649 2020-02-02 00:00:00.000000 mtg_card_api-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 mtg_card_api-0.1.2/PKG-INFO
```

### Comparing `mtg_card_api-0.1.1/src/mtg_card_api/mtg_scryfall_api.py` & `mtg_card_api-0.1.2/src/mtg_card_api/mtg_scryfall_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -110,9 +110,28 @@
             'cards/named',
             {
                 'exact': card_name
             },
             Utils.encodeMD5(card_name),
             'cache/cards')
 
+    def get_card_variants(self, oracle_id: str) -> R:
+        """Searches Scryfall by the oracle to find all variants of a card
+
+        Args:
+            card_name (str): Exact string oracle id of a card
+
+        Returns:
+            R: Full search result
+        """
+        return self._run_get(
+            'https://api.scryfall.com/cards/search',
+            {
+                'q': f'oracle_id={oracle_id}',
+                'unique': 'prints'
+            },
+            oracle_id,
+            'cache/variants'
+        )
+
     def run(self):
         pass
```

### Comparing `mtg_card_api-0.1.1/.gitignore` & `mtg_card_api-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mtg_card_api-0.1.1/LICENSE` & `mtg_card_api-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mtg_card_api-0.1.1/README.md` & `mtg_card_api-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mtg_card_api-0.1.1/pyproject.toml` & `mtg_card_api-0.1.2/pyproject.toml`

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
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     { name = "Samuel Shiels" },
 ]
 description = "An unofficial wrapper for the Scryfall REST API providing common queries"
 readme = "README.md"
 requires-python = ">=3.12.2"
 classifiers = [
```

### Comparing `mtg_card_api-0.1.1/PKG-INFO` & `mtg_card_api-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mtg_card_api
-Version: 0.1.1
+Version: 0.1.2
 Summary: An unofficial wrapper for the Scryfall REST API providing common queries
 Author: Samuel Shiels
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Other Environment
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

