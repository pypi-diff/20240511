# Comparing `tmp/gmxpy-0.0.4.tar.gz` & `tmp/gmxpy-0.0.5.tar.gz`

## Comparing `gmxpy-0.0.4.tar` & `gmxpy-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 gmxpy-0.0.4/gmxpy/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gmxpy-0.0.4/gmxpy/main.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 gmxpy-0.0.4/gmxpy/analysis/__init__.py
--rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 gmxpy-0.0.4/gmxpy/analysis/functional.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gmxpy-0.0.4/gmxpy/editconf/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gmxpy-0.0.4/gmxpy/grompp/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gmxpy-0.0.4/gmxpy/grompp/functional.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gmxpy-0.0.4/gmxpy/solvate/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gmxpy-0.0.4/gmxpy/utils/__init__,py
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 gmxpy-0.0.4/gmxpy/utils/functional.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gmxpy-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gmxpy-0.0.4/tests/test_gmxpy.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 gmxpy-0.0.4/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 gmxpy-0.0.4/LICENSE
--rw-r--r--   0        0        0    10030 2020-02-02 00:00:00.000000 gmxpy-0.0.4/README.md
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 gmxpy-0.0.4/pyproject.toml
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 gmxpy-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 gmxpy-0.0.5/gmxpy/__init__.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 gmxpy-0.0.5/gmxpy/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gmxpy-0.0.5/gmxpy/main.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 gmxpy-0.0.5/gmxpy/analysis/__init__.py
+-rw-r--r--   0        0        0     5977 2020-02-02 00:00:00.000000 gmxpy-0.0.5/gmxpy/analysis/functional.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gmxpy-0.0.5/gmxpy/editconf/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gmxpy-0.0.5/gmxpy/grompp/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gmxpy-0.0.5/gmxpy/grompp/functional.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gmxpy-0.0.5/gmxpy/solvate/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gmxpy-0.0.5/gmxpy/utils/__init__,py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 gmxpy-0.0.5/gmxpy/utils/functional.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gmxpy-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gmxpy-0.0.5/tests/test_gmxpy.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 gmxpy-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 gmxpy-0.0.5/LICENSE
+-rw-r--r--   0        0        0    10030 2020-02-02 00:00:00.000000 gmxpy-0.0.5/README.md
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 gmxpy-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 gmxpy-0.0.5/PKG-INFO
```

### Comparing `gmxpy-0.0.4/gmxpy/utils/functional.py` & `gmxpy-0.0.5/gmxpy/utils/functional.py`

 * *Files identical despite different names*

### Comparing `gmxpy-0.0.4/.gitignore` & `gmxpy-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `gmxpy-0.0.4/LICENSE` & `gmxpy-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gmxpy-0.0.4/README.md` & `gmxpy-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gmxpy-0.0.4/pyproject.toml` & `gmxpy-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gmxpy-0.0.4/PKG-INFO` & `gmxpy-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: gmxpy
-Version: 0.0.4
+Version: 0.0.5
 Summary: Wrapping GROMACS by Python for me
 Project-URL: Homepage, https://github.com/Goosang-Yu/gmxpy
 Project-URL: Repository, https://github.com/Goosang-Yu/gmxpy
 Project-URL: Source, https://github.com/Goosang-Yu/gmxpy
 Project-URL: Tracker, https://github.com/Goosang-Yu/gmxpy/issues
 Author-email: Goosang Yu <gsyu93@gmail.com>
 License-Expression: MIT
```

