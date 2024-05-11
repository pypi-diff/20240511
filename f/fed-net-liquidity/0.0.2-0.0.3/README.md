# Comparing `tmp/fed_net_liquidity-0.0.2.tar.gz` & `tmp/fed_net_liquidity-0.0.3.tar.gz`

## Comparing `fed_net_liquidity-0.0.2.tar` & `fed_net_liquidity-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 fed_net_liquidity-0.0.2/src/fed_net_liquidity/__init__.py
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 fed_net_liquidity-0.0.2/src/fed_net_liquidity/fed_net_liquidity.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 fed_net_liquidity-0.0.2/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 fed_net_liquidity-0.0.2/LICENSE
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 fed_net_liquidity-0.0.2/README.md
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 fed_net_liquidity-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 fed_net_liquidity-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 fed_net_liquidity-0.0.3/src/fed_net_liquidity/__init__.py
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 fed_net_liquidity-0.0.3/src/fed_net_liquidity/fed_net_liquidity.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 fed_net_liquidity-0.0.3/src/fed_net_liquidity/update.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 fed_net_liquidity-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 fed_net_liquidity-0.0.3/LICENSE
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 fed_net_liquidity-0.0.3/README.md
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 fed_net_liquidity-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 fed_net_liquidity-0.0.3/PKG-INFO
```

### Comparing `fed_net_liquidity-0.0.2/src/fed_net_liquidity/fed_net_liquidity.py` & `fed_net_liquidity-0.0.3/src/fed_net_liquidity/fed_net_liquidity.py`

 * *Files identical despite different names*

### Comparing `fed_net_liquidity-0.0.2/LICENSE` & `fed_net_liquidity-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fed_net_liquidity-0.0.2/pyproject.toml` & `fed_net_liquidity-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fed_net_liquidity"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Eduardo Cavazos", email="wayo.cavazos@gmail.com" },
 ]
 description = "Library for calculating Fed Net Liquidity"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `fed_net_liquidity-0.0.2/PKG-INFO` & `fed_net_liquidity-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fed_net_liquidity
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library for calculating Fed Net Liquidity
 Project-URL: Homepage, https://github.com/dharmatech/fed_net_liquidity.py
 Project-URL: Issues, https://github.com/dharmatech/fed_net_liquidity.py/issues
 Author-email: Eduardo Cavazos <wayo.cavazos@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

