# Comparing `tmp/types-regex-2024.4.28.20240506.tar.gz` & `tmp/types-regex-2024.5.10.20240511.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-regex-2024.4.28.20240506.tar", last modified: Mon May  6 02:22:04 2024, max compression
+gzip compressed data, was "types-regex-2024.5.10.20240511.tar", last modified: Sat May 11 02:17:51 2024, max compression
```

## Comparing `types-regex-2024.4.28.20240506.tar` & `types-regex-2024.5.10.20240511.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:22:04.848860 types-regex-2024.4.28.20240506/
--rw-r--r--   0 runner    (1001) docker     (127)     7033 2024-05-06 02:22:02.000000 types-regex-2024.4.28.20240506/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-06 02:22:02.000000 types-regex-2024.4.28.20240506/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-06 02:22:04.848860 types-regex-2024.4.28.20240506/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:22:04.844860 types-regex-2024.4.28.20240506/regex-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-06 02:22:02.000000 types-regex-2024.4.28.20240506/regex-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-06 02:21:48.000000 types-regex-2024.4.28.20240506/regex-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-06 02:21:48.000000 types-regex-2024.4.28.20240506/regex-stubs/_regex.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-06 02:21:48.000000 types-regex-2024.4.28.20240506/regex-stubs/_regex_core.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 02:22:02.000000 types-regex-2024.4.28.20240506/regex-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-05-06 02:21:48.000000 types-regex-2024.4.28.20240506/regex-stubs/regex.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 02:22:04.848860 types-regex-2024.4.28.20240506/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-06 02:22:02.000000 types-regex-2024.4.28.20240506/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:22:04.848860 types-regex-2024.4.28.20240506/types_regex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-06 02:22:04.000000 types-regex-2024.4.28.20240506/types_regex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-06 02:22:04.000000 types-regex-2024.4.28.20240506/types_regex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 02:22:04.000000 types-regex-2024.4.28.20240506/types_regex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 02:22:04.000000 types-regex-2024.4.28.20240506/types_regex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:17:51.062107 types-regex-2024.5.10.20240511/
+-rw-r--r--   0 runner    (1001) docker     (127)     7557 2024-05-11 02:17:50.000000 types-regex-2024.5.10.20240511/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-11 02:17:50.000000 types-regex-2024.5.10.20240511/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-11 02:17:51.062107 types-regex-2024.5.10.20240511/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:17:51.058107 types-regex-2024.5.10.20240511/regex-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-11 02:17:50.000000 types-regex-2024.5.10.20240511/regex-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-11 02:17:34.000000 types-regex-2024.5.10.20240511/regex-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-11 02:17:34.000000 types-regex-2024.5.10.20240511/regex-stubs/_regex.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-11 02:17:34.000000 types-regex-2024.5.10.20240511/regex-stubs/_regex_core.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:17:50.000000 types-regex-2024.5.10.20240511/regex-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-05-11 02:17:34.000000 types-regex-2024.5.10.20240511/regex-stubs/regex.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 02:17:51.062107 types-regex-2024.5.10.20240511/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-11 02:17:50.000000 types-regex-2024.5.10.20240511/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:17:51.062107 types-regex-2024.5.10.20240511/types_regex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-11 02:17:51.000000 types-regex-2024.5.10.20240511/types_regex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-11 02:17:51.000000 types-regex-2024.5.10.20240511/types_regex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 02:17:51.000000 types-regex-2024.5.10.20240511/types_regex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-11 02:17:51.000000 types-regex-2024.5.10.20240511/types_regex.egg-info/top_level.txt
```

### Comparing `types-regex-2024.4.28.20240506/CHANGELOG.md` & `types-regex-2024.5.10.20240511/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+## 2024.5.10.20240511 (2024-05-11)
+
+[stubsabot] Bump regex to 2024.5.10 (#11894)
+
+Release: https://pypi.org/pypi/regex/2024.5.10
+Homepage: https://github.com/mrabarnett/mrab-regex
+Repository: https://github.com/mrabarnett/mrab-regex
+Typeshed stubs: https://github.com/python/typeshed/tree/main/stubs/regex
+Diff: https://github.com/mrabarnett/mrab-regex/compare/2024.4.28...2024.5.10
+
+Stubsabot analysis of the diff between the two releases:
+ - Total lines of Python code added: 6.
+ - Total lines of Python code deleted: 4.
+
 ## 2024.4.28.20240506 (2024-05-06)
 
 regex: improve Pattern annotations (#11862)
 
 - Corrected types for `pos` and `endpos` arguments to `int | None = None`
 - Corrected type for `timeout` argument to `float | None = None`
 - Added default value `None` for `concurrent` and `timeout` parameters
```

### Comparing `types-regex-2024.4.28.20240506/PKG-INFO` & `types-regex-2024.5.10.20240511/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-regex
-Version: 2024.4.28.20240506
+Version: 2024.5.10.20240511
 Summary: Typing stubs for regex
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/regex.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,16 +22,16 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `regex`.
 
 This version of `types-regex` aims to provide accurate annotations
-for `regex==2024.4.28`.
+for `regex==2024.5.10`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/regex. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `8ff50fbea2f607380c23d9b120fccfb1926284e5` and was tested
-with mypy 1.10.0, pyright 1.1.361, and
+This package was generated from typeshed commit `7bfde5b676a19080f4496c618117b748e2a02628` and was tested
+with mypy 1.10.0, pyright 1.1.362, and
 pytype 2024.4.11.
```

### Comparing `types-regex-2024.4.28.20240506/regex-stubs/_regex.pyi` & `types-regex-2024.5.10.20240511/regex-stubs/_regex.pyi`

 * *Files identical despite different names*

### Comparing `types-regex-2024.4.28.20240506/regex-stubs/_regex_core.pyi` & `types-regex-2024.5.10.20240511/regex-stubs/_regex_core.pyi`

 * *Files identical despite different names*

### Comparing `types-regex-2024.4.28.20240506/regex-stubs/regex.pyi` & `types-regex-2024.5.10.20240511/regex-stubs/regex.pyi`

 * *Files identical despite different names*

### Comparing `types-regex-2024.4.28.20240506/setup.py` & `types-regex-2024.5.10.20240511/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `regex`.
 
 This version of `types-regex` aims to provide accurate annotations
-for `regex==2024.4.28`.
+for `regex==2024.5.10`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/regex. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `8ff50fbea2f607380c23d9b120fccfb1926284e5` and was tested
-with mypy 1.10.0, pyright 1.1.361, and
+This package was generated from typeshed commit `7bfde5b676a19080f4496c618117b748e2a02628` and was tested
+with mypy 1.10.0, pyright 1.1.362, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="2024.4.28.20240506",
+      version="2024.5.10.20240511",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/regex.md",
```

### Comparing `types-regex-2024.4.28.20240506/types_regex.egg-info/PKG-INFO` & `types-regex-2024.5.10.20240511/types_regex.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-regex
-Version: 2024.4.28.20240506
+Version: 2024.5.10.20240511
 Summary: Typing stubs for regex
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/regex.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,16 +22,16 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `regex`.
 
 This version of `types-regex` aims to provide accurate annotations
-for `regex==2024.4.28`.
+for `regex==2024.5.10`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/regex. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `8ff50fbea2f607380c23d9b120fccfb1926284e5` and was tested
-with mypy 1.10.0, pyright 1.1.361, and
+This package was generated from typeshed commit `7bfde5b676a19080f4496c618117b748e2a02628` and was tested
+with mypy 1.10.0, pyright 1.1.362, and
 pytype 2024.4.11.
```

