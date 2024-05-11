# Comparing `tmp/hyperdrivepy-0.9.0.tar.gz` & `tmp/hyperdrivepy-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperdrivepy-0.9.0.tar", last modified: Sat Mar 16 04:18:42 2024, max compression
+gzip compressed data, was "hyperdrivepy-0.9.2.tar", last modified: Mon Mar 18 17:18:26 2024, max compression
```

## Comparing `hyperdrivepy-0.9.0.tar` & `hyperdrivepy-0.9.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 04:18:42.373575 hyperdrivepy-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-03-16 04:18:37.000000 hyperdrivepy-0.9.0/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-16 04:18:37.000000 hyperdrivepy-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-16 04:18:37.000000 hyperdrivepy-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-16 04:18:42.373575 hyperdrivepy-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-16 04:18:37.000000 hyperdrivepy-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-16 04:18:37.000000 hyperdrivepy-0.9.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 04:18:42.369575 hyperdrivepy-0.9.0/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 04:18:42.369575 hyperdrivepy-0.9.0/python/hyperdrivepy/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-16 04:18:37.000000 hyperdrivepy-0.9.0/python/hyperdrivepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15974 2024-03-16 04:18:37.000000 hyperdrivepy-0.9.0/python/hyperdrivepy/hyperdrive_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-03-16 04:18:37.000000 hyperdrivepy-0.9.0/python/hyperdrivepy/hyperdrive_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 04:18:42.373575 hyperdrivepy-0.9.0/python/hyperdrivepy/pypechain_types/
--rw-r--r--   0 runner    (1001) docker     (127)   245208 2024-03-16 04:18:37.000000 hyperdrivepy-0.9.0/python/hyperdrivepy/pypechain_types/IERC4626HyperdriveContract.py
--rw-r--r--   0 runner    (1001) docker     (127)    14272 2024-03-16 04:18:37.000000 hyperdrivepy-0.9.0/python/hyperdrivepy/pypechain_types/IERC4626HyperdriveTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-03-16 04:18:37.000000 hyperdrivepy-0.9.0/python/hyperdrivepy/pypechain_types/IHyperdriveTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-16 04:18:37.000000 hyperdrivepy-0.9.0/python/hyperdrivepy/pypechain_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-03-16 04:18:37.000000 hyperdrivepy-0.9.0/python/hyperdrivepy/pypechain_types/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-03-16 04:18:37.000000 hyperdrivepy-0.9.0/python/hyperdrivepy/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-03-16 04:18:37.000000 hyperdrivepy-0.9.0/python/hyperdrivepy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 04:18:42.373575 hyperdrivepy-0.9.0/python/hyperdrivepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-16 04:18:42.000000 hyperdrivepy-0.9.0/python/hyperdrivepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-16 04:18:42.000000 hyperdrivepy-0.9.0/python/hyperdrivepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 04:18:42.000000 hyperdrivepy-0.9.0/python/hyperdrivepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 04:18:42.000000 hyperdrivepy-0.9.0/python/hyperdrivepy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-16 04:18:42.000000 hyperdrivepy-0.9.0/python/hyperdrivepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-16 04:18:42.373575 hyperdrivepy-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-16 04:18:37.000000 hyperdrivepy-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 04:18:42.373575 hyperdrivepy-0.9.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-03-16 04:18:37.000000 hyperdrivepy-0.9.0/src/hyperdrive_state.rs
--rw-r--r--   0 runner    (1001) docker     (127)    11261 2024-03-16 04:18:37.000000 hyperdrivepy-0.9.0/src/hyperdrive_state_methods.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-03-16 04:18:37.000000 hyperdrivepy-0.9.0/src/hyperdrive_utils.rs
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-03-16 04:18:37.000000 hyperdrivepy-0.9.0/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-03-16 04:18:37.000000 hyperdrivepy-0.9.0/src/pool_config.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-03-16 04:18:37.000000 hyperdrivepy-0.9.0/src/pool_info.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-03-16 04:18:37.000000 hyperdrivepy-0.9.0/src/utils.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:18:26.381579 hyperdrivepy-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-18 17:18:26.381579 hyperdrivepy-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:18:26.373579 hyperdrivepy-0.9.2/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:18:26.377579 hyperdrivepy-0.9.2/python/hyperdrivepy/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/python/hyperdrivepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15974 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/python/hyperdrivepy/hyperdrive_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/python/hyperdrivepy/hyperdrive_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:18:26.381579 hyperdrivepy-0.9.2/python/hyperdrivepy/pypechain_types/
+-rw-r--r--   0 runner    (1001) docker     (127)   245208 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/python/hyperdrivepy/pypechain_types/IERC4626HyperdriveContract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14272 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/python/hyperdrivepy/pypechain_types/IERC4626HyperdriveTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/python/hyperdrivepy/pypechain_types/IHyperdriveTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/python/hyperdrivepy/pypechain_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/python/hyperdrivepy/pypechain_types/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/python/hyperdrivepy/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/python/hyperdrivepy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:18:26.381579 hyperdrivepy-0.9.2/python/hyperdrivepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-18 17:18:26.000000 hyperdrivepy-0.9.2/python/hyperdrivepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-18 17:18:26.000000 hyperdrivepy-0.9.2/python/hyperdrivepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 17:18:26.000000 hyperdrivepy-0.9.2/python/hyperdrivepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 17:18:26.000000 hyperdrivepy-0.9.2/python/hyperdrivepy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-18 17:18:26.000000 hyperdrivepy-0.9.2/python/hyperdrivepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 17:18:26.381579 hyperdrivepy-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:18:26.381579 hyperdrivepy-0.9.2/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/src/hyperdrive_state.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    11261 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/src/hyperdrive_state_methods.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/src/hyperdrive_utils.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/src/pool_config.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/src/pool_info.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/src/utils.rs
```

### Comparing `hyperdrivepy-0.9.0/Cargo.toml` & `hyperdrivepy-0.9.2/Cargo.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "hyperdrivepy"
 edition = "2021"
-version = "0.9.0"
+version = "0.9.2"
 authors = [
     "Dylan Paiton",
     "Matt Brown",
     "Sheng Lundquist",
 ]
 description = "Python wrappers for the Hyperdrive AMM"
```

### Comparing `hyperdrivepy-0.9.0/LICENSE` & `hyperdrivepy-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-0.9.0/PKG-INFO` & `hyperdrivepy-0.9.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: hyperdrivepy
-Version: 0.9.0
-Project-URL: Homepage, https://github.com/delvtech/hyperdrive-sdk
-Project-URL: Issues, https://github.com/delvtech/hyperdrive-sdk/issues
+Version: 0.9.2
+Project-URL: Homepage, https://github.com/delvtech/hyperdrive-bindings
+Project-URL: Issues, https://github.com/delvtech/hyperdrive-bindings/issues
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hyperdrivepy
 
-Hyperdrivepy is the Python to rust bindings of [hyperdrive-sdk](https://github.com/delvtech/hyperdrive-sdk).
+Hyperdrivepy is the Python to rust bindings of [hyperdrive-bindings](https://github.com/delvtech/hyperdrive-bindings).
 
 ## Disclaimer
 
 The language used in this codebase is for coding convenience only, and is not
 intended to, and does not, have any particular legal or regulatory significance.
```

### Comparing `hyperdrivepy-0.9.0/pyproject.toml` & `hyperdrivepy-0.9.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [project]
 name = "hyperdrivepy"
-version = "0.9.0"
+version = "0.9.2"
 requires-python = ">=3.7"
 classifiers = [
   "Programming Language :: Rust",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 readme = "README.md"
 
 [project.urls]
-Homepage = "https://github.com/delvtech/hyperdrive-sdk"
-Issues = "https://github.com/delvtech/hyperdrive-sdk/issues"
+Homepage = "https://github.com/delvtech/hyperdrive-bindings"
+Issues = "https://github.com/delvtech/hyperdrive-bindings/issues"
 
 [build-system]
 requires = ["setuptools", "wheel", "setuptools-rust"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["python", "src"]
```

### Comparing `hyperdrivepy-0.9.0/python/hyperdrivepy/hyperdrive_state.py` & `hyperdrivepy-0.9.2/python/hyperdrivepy/hyperdrive_state.py`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-0.9.0/python/hyperdrivepy/hyperdrive_utils.py` & `hyperdrivepy-0.9.2/python/hyperdrivepy/hyperdrive_utils.py`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-0.9.0/python/hyperdrivepy/pypechain_types/IERC4626HyperdriveContract.py` & `hyperdrivepy-0.9.2/python/hyperdrivepy/pypechain_types/IERC4626HyperdriveContract.py`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-0.9.0/python/hyperdrivepy/pypechain_types/IERC4626HyperdriveTypes.py` & `hyperdrivepy-0.9.2/python/hyperdrivepy/pypechain_types/IERC4626HyperdriveTypes.py`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-0.9.0/python/hyperdrivepy/pypechain_types/IHyperdriveTypes.py` & `hyperdrivepy-0.9.2/python/hyperdrivepy/pypechain_types/IHyperdriveTypes.py`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-0.9.0/python/hyperdrivepy/pypechain_types/utilities.py` & `hyperdrivepy-0.9.2/python/hyperdrivepy/pypechain_types/utilities.py`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-0.9.0/python/hyperdrivepy/types.py` & `hyperdrivepy-0.9.2/python/hyperdrivepy/types.py`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-0.9.0/python/hyperdrivepy/utils.py` & `hyperdrivepy-0.9.2/python/hyperdrivepy/utils.py`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-0.9.0/python/hyperdrivepy.egg-info/PKG-INFO` & `hyperdrivepy-0.9.2/python/hyperdrivepy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: hyperdrivepy
-Version: 0.9.0
-Project-URL: Homepage, https://github.com/delvtech/hyperdrive-sdk
-Project-URL: Issues, https://github.com/delvtech/hyperdrive-sdk/issues
+Version: 0.9.2
+Project-URL: Homepage, https://github.com/delvtech/hyperdrive-bindings
+Project-URL: Issues, https://github.com/delvtech/hyperdrive-bindings/issues
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hyperdrivepy
 
-Hyperdrivepy is the Python to rust bindings of [hyperdrive-sdk](https://github.com/delvtech/hyperdrive-sdk).
+Hyperdrivepy is the Python to rust bindings of [hyperdrive-bindings](https://github.com/delvtech/hyperdrive-bindings).
 
 ## Disclaimer
 
 The language used in this codebase is for coding convenience only, and is not
 intended to, and does not, have any particular legal or regulatory significance.
```

### Comparing `hyperdrivepy-0.9.0/python/hyperdrivepy.egg-info/SOURCES.txt` & `hyperdrivepy-0.9.2/python/hyperdrivepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-0.9.0/src/hyperdrive_state.rs` & `hyperdrivepy-0.9.2/src/hyperdrive_state.rs`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-0.9.0/src/hyperdrive_state_methods.rs` & `hyperdrivepy-0.9.2/src/hyperdrive_state_methods.rs`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-0.9.0/src/hyperdrive_utils.rs` & `hyperdrivepy-0.9.2/src/hyperdrive_utils.rs`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-0.9.0/src/lib.rs` & `hyperdrivepy-0.9.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-0.9.0/src/pool_config.rs` & `hyperdrivepy-0.9.2/src/pool_config.rs`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-0.9.0/src/pool_info.rs` & `hyperdrivepy-0.9.2/src/pool_info.rs`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-0.9.0/src/utils.rs` & `hyperdrivepy-0.9.2/src/utils.rs`

 * *Files identical despite different names*

