# Comparing `tmp/notionaut-0.2.1.tar.gz` & `tmp/notionaut-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notionaut-0.2.1.tar", max compression
+gzip compressed data, was "notionaut-0.2.2.tar", max compression
```

## Comparing `notionaut-0.2.1.tar` & `notionaut-0.2.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       80 2023-08-29 01:52:58.840253 notionaut-0.2.1/README.md
--rw-r--r--   0        0        0      701 2023-08-29 02:03:01.531220 notionaut-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       67 2023-08-29 01:52:58.840764 notionaut-0.2.1/src/notionaut/__init__.py
--rw-r--r--   0        0        0     3942 2023-08-29 02:02:41.726201 notionaut-0.2.1/src/notionaut/client.py
--rw-r--r--   0        0        0      794 1970-01-01 00:00:00.000000 notionaut-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       80 2023-06-19 21:35:19.704354 notionaut-0.2.2/README.md
+-rw-r--r--   0        0        0      701 2024-05-11 01:31:34.267129 notionaut-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       67 2023-06-21 00:43:34.630935 notionaut-0.2.2/src/notionaut/__init__.py
+-rw-r--r--   0        0        0     4153 2024-05-11 01:31:12.439497 notionaut-0.2.2/src/notionaut/client.py
+-rw-r--r--   0        0        0      845 1970-01-01 00:00:00.000000 notionaut-0.2.2/PKG-INFO
```

### Comparing `notionaut-0.2.1/pyproject.toml` & `notionaut-0.2.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "notionaut"
-version = "0.2.1"
+version = "0.2.2"
 description = "A simple package for fetching Notion databases as pandas dataframes"
 authors = ["Nick Schenone <nschenone16@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
   { include = "notionaut", from = "src"}
 ]
```

### Comparing `notionaut-0.2.1/src/notionaut/client.py` & `notionaut-0.2.2/src/notionaut/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,15 +53,19 @@
     :param columns: List of columns to include, defaults to None.
 
     :return: The parsed row.
     """
     row = {}
     for name, properties in to_parse.items():
         if not columns or name in columns:
-            row[name] = parse_property(properties)
+            try:
+                row[name] = parse_property(properties)
+            except:
+                print(f"Failed parsing column {name} in record {to_parse}")
+    row["error"] = False
     return row
 
 
 class NotionautClient:
     def __init__(self, notion_token: str, notion: Client = None):
         """
         Initializes a NotionautClient instance.
@@ -86,14 +90,15 @@
     ) -> pd.DataFrame:
         df = pd.DataFrame(results["results"])
         if df.empty:
             return pd.DataFrame()
         parsed = pd.DataFrame(
             [parse_row(to_parse=d, columns=columns) for d in df["properties"]]
         )
+        parsed = parsed[parsed.error == False].drop("error", axis=1)
         parsed["id"] = df["id"]
         if columns:
             parsed = parsed[columns]
         if with_url:
             parsed["_url"] = df["url"].apply(
                 lambda x: x.replace("https://", "notion://")
             )
```

### Comparing `notionaut-0.2.1/PKG-INFO` & `notionaut-0.2.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: notionaut
-Version: 0.2.1
+Version: 0.2.2
 Summary: A simple package for fetching Notion databases as pandas dataframes
 Home-page: https://github.com/nschenone/notionaut
 License: MIT
 Author: Nick Schenone
 Author-email: nschenone16@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: notion-client (>=1.0.0,<2.0.0)
 Requires-Dist: pandas (==1.5.1)
 Project-URL: Repository, https://github.com/nschenone/notionaut
 Description-Content-Type: text/markdown
 
 # Notionaut
```

