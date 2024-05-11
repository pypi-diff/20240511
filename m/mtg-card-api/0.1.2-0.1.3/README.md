# Comparing `tmp/mtg_card_api-0.1.2.tar.gz` & `tmp/mtg_card_api-0.1.3.tar.gz`

## Comparing `mtg_card_api-0.1.2.tar` & `mtg_card_api-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0      155 2020-02-02 00:00:00.000000 mtg_card_api-0.1.2/main.py
--rwxr-xr-x   0        0        0      121 2020-02-02 00:00:00.000000 mtg_card_api-0.1.2/src/mtg_card_api/__init__.py
--rwxr-xr-x   0        0        0      149 2020-02-02 00:00:00.000000 mtg_card_api-0.1.2/src/mtg_card_api/_utils.py
--rwxr-xr-x   0        0        0     4280 2020-02-02 00:00:00.000000 mtg_card_api-0.1.2/src/mtg_card_api/mtg_scryfall_api.py
--rwxr-xr-x   0        0        0     3078 2020-02-02 00:00:00.000000 mtg_card_api-0.1.2/.gitignore
--rwxr-xr-x   0        0        0     1069 2020-02-02 00:00:00.000000 mtg_card_api-0.1.2/LICENSE
--rwxr-xr-x   0        0        0      912 2020-02-02 00:00:00.000000 mtg_card_api-0.1.2/README.md
--rwxr-xr-x   0        0        0      649 2020-02-02 00:00:00.000000 mtg_card_api-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 mtg_card_api-0.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0      155 2020-02-02 00:00:00.000000 mtg_card_api-0.1.3/main.py
+-rwxr-xr-x   0        0        0      121 2020-02-02 00:00:00.000000 mtg_card_api-0.1.3/src/mtg_card_api/__init__.py
+-rwxr-xr-x   0        0        0      149 2020-02-02 00:00:00.000000 mtg_card_api-0.1.3/src/mtg_card_api/_utils.py
+-rwxr-xr-x   0        0        0     4278 2020-02-02 00:00:00.000000 mtg_card_api-0.1.3/src/mtg_card_api/mtg_scryfall_api.py
+-rwxr-xr-x   0        0        0     3078 2020-02-02 00:00:00.000000 mtg_card_api-0.1.3/.gitignore
+-rwxr-xr-x   0        0        0     1069 2020-02-02 00:00:00.000000 mtg_card_api-0.1.3/LICENSE
+-rwxr-xr-x   0        0        0      912 2020-02-02 00:00:00.000000 mtg_card_api-0.1.3/README.md
+-rwxr-xr-x   0        0        0      649 2020-02-02 00:00:00.000000 mtg_card_api-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 mtg_card_api-0.1.3/PKG-INFO
```

### Comparing `mtg_card_api-0.1.2/src/mtg_card_api/mtg_scryfall_api.py` & `mtg_card_api-0.1.3/src/mtg_card_api/mtg_scryfall_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,17 +73,16 @@
         config['output'] = o + '.json'
         config['cache'] = self.cache_dir + c
         config['time'] = self.cache_time_mins
         config['sleep'] = self.sleep_ms
         config['rest'] = rest_obj
         self._debug(f"{config}")
         response = rc.execute(rest_obj)
-        if self.use_cache:
+        if response.error is not False and self.use_cache:
             self._set_cache(o, response)
-
         return response
 
     def clear_cache(self) -> None:
         """
         Clears all keys from the diskcache database
         """
         self.cache.clear()
@@ -128,10 +127,7 @@
             {
                 'q': f'oracle_id={oracle_id}',
                 'unique': 'prints'
             },
             oracle_id,
             'cache/variants'
         )
-
-    def run(self):
-        pass
```

### Comparing `mtg_card_api-0.1.2/.gitignore` & `mtg_card_api-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `mtg_card_api-0.1.2/LICENSE` & `mtg_card_api-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mtg_card_api-0.1.2/README.md` & `mtg_card_api-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `mtg_card_api-0.1.2/pyproject.toml` & `mtg_card_api-0.1.3/pyproject.toml`

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
-version = "0.1.2"
+version = "0.1.3"
 authors = [
     { name = "Samuel Shiels" },
 ]
 description = "An unofficial wrapper for the Scryfall REST API providing common queries"
 readme = "README.md"
 requires-python = ">=3.12.2"
 classifiers = [
```

### Comparing `mtg_card_api-0.1.2/PKG-INFO` & `mtg_card_api-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mtg_card_api
-Version: 0.1.2
+Version: 0.1.3
 Summary: An unofficial wrapper for the Scryfall REST API providing common queries
 Author: Samuel Shiels
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Other Environment
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

