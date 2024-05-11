# Comparing `tmp/relic_engine-0.2.8.tar.gz` & `tmp/relic_engine-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relic_engine-0.2.8.tar", last modified: Mon Nov  6 20:56:07 2023, max compression
+gzip compressed data, was "relic_engine-0.2.9.tar", last modified: Mon Apr 29 04:57:42 2024, max compression
```

## Comparing `relic_engine-0.2.8.tar` & `relic_engine-0.2.9.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-11-06 20:56:07.497249 relic_engine-0.2.8/
--rw-rw-rw-   0        0        0      454 2023-11-06 20:56:07.497249 relic_engine-0.2.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-11-06 20:56:07.472455 relic_engine-0.2.8/relic_engine/
--rw-rw-rw-   0        0        0     5861 2023-11-06 20:55:35.000000 relic_engine-0.2.8/relic_engine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-06 20:56:07.495249 relic_engine-0.2.8/relic_engine.egg-info/
--rw-rw-rw-   0        0        0      454 2023-11-06 20:56:07.000000 relic_engine-0.2.8/relic_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-11-06 20:56:07.000000 relic_engine-0.2.8/relic_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-06 20:56:07.000000 relic_engine-0.2.8/relic_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-11-06 20:56:07.000000 relic_engine-0.2.8/relic_engine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-11-06 20:56:07.000000 relic_engine-0.2.8/relic_engine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-06 20:56:07.497249 relic_engine-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0      800 2023-11-06 20:55:59.000000 relic_engine-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 04:57:42.514308 relic_engine-0.2.9/
+-rw-rw-rw-   0        0        0      520 2024-04-29 04:57:42.513311 relic_engine-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      129 2024-02-04 15:46:30.000000 relic_engine-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 04:57:42.492302 relic_engine-0.2.9/relic_engine/
+-rw-rw-rw-   0        0        0     5838 2024-04-29 04:56:05.000000 relic_engine-0.2.9/relic_engine/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 04:57:42.512302 relic_engine-0.2.9/relic_engine.egg-info/
+-rw-rw-rw-   0        0        0      520 2024-04-29 04:57:42.000000 relic_engine-0.2.9/relic_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2024-04-29 04:57:42.000000 relic_engine-0.2.9/relic_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 04:57:42.000000 relic_engine-0.2.9/relic_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-29 04:57:42.000000 relic_engine-0.2.9/relic_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-29 04:57:42.000000 relic_engine-0.2.9/relic_engine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 04:57:42.514308 relic_engine-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      800 2024-04-29 04:57:37.000000 relic_engine-0.2.9/setup.py
```

### Comparing `relic_engine-0.2.8/relic_engine/__init__.py` & `relic_engine-0.2.9/relic_engine/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def __decode_and_decompress(url):
     file = requests.get(url).content
     file = gzip.decompress(file)
     return json.loads(file.decode("utf-8"))
 
 
 def __get_index_file():
-    index = __decode_and_decompress("https://github.com/JCalMcBride/RelicEngine/raw/master/index.json.gz")
+    index = __decode_and_decompress("http://mercuriusapp.com/index/index.json.gz")
 
     return index
 
 
 __index = __get_index_file()
 __relic_dict = __index['relics']
 __price_dict = __index['prices']
@@ -53,21 +53,22 @@
     if "Kavasa" in set_name:
         set_name += " Kubrow Collar"
 
     return set_name
 
 
 def get_drop_chance(refinement: str, rarity_id: int):
+    ref = refinement.lower()[0]
     try:
-        return __rarity_dict[refinement[0]][rarity_id]
+        return __rarity_dict[ref][rarity_id]
     except KeyError:
         drop_chances = []
         for digit in str(rarity_id):
-            if int(digit) in __rarity_dict[refinement[0]]:
-                drop_chances.append(get_drop_chance(refinement[0], int(digit)))
+            if int(digit) in __rarity_dict[ref]:
+                drop_chances.append(get_drop_chance(ref, int(digit)))
             else:
                 return 'N/A'
 
         return drop_chances
 
 
 def get_relic_drops(relic, refinement):
@@ -255,8 +256,7 @@
 
 def get_set_required(set_name):
     required_amount = {}
     for item in get_set_parts(set_name):
         required_amount[item] = get_required_amount(item)
 
     return required_amount
-
```

