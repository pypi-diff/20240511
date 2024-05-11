# Comparing `tmp/types-psutil-5.9.5.8.tar.gz` & `tmp/types-psutil-5.9.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-psutil-5.9.5.8.tar", last modified: Tue Feb 21 01:32:05 2023, max compression
+gzip compressed data, was "types-psutil-5.9.5.9.tar", last modified: Sun Feb 26 01:39:31 2023, max compression
```

## Comparing `types-psutil-5.9.5.8.tar` & `types-psutil-5.9.5.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:32:05.554412 types-psutil-5.9.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-02-21 01:32:04.000000 types-psutil-5.9.5.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-21 01:32:04.000000 types-psutil-5.9.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-02-21 01:32:05.554412 types-psutil-5.9.5.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:32:05.554412 types-psutil-5.9.5.8/psutil-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-02-21 01:32:04.000000 types-psutil-5.9.5.8/psutil-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-02-21 01:26:21.000000 types-psutil-5.9.5.8/psutil-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-02-21 01:26:21.000000 types-psutil-5.9.5.8/psutil-stubs/_common.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-02-21 01:26:21.000000 types-psutil-5.9.5.8/psutil-stubs/_compat.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-02-21 01:26:21.000000 types-psutil-5.9.5.8/psutil-stubs/_psaix.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-02-21 01:26:21.000000 types-psutil-5.9.5.8/psutil-stubs/_psbsd.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-02-21 01:26:21.000000 types-psutil-5.9.5.8/psutil-stubs/_pslinux.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-02-21 01:26:21.000000 types-psutil-5.9.5.8/psutil-stubs/_psosx.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-02-21 01:26:21.000000 types-psutil-5.9.5.8/psutil-stubs/_psposix.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-02-21 01:26:21.000000 types-psutil-5.9.5.8/psutil-stubs/_pssunos.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-02-21 01:26:21.000000 types-psutil-5.9.5.8/psutil-stubs/_psutil_linux.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-02-21 01:26:21.000000 types-psutil-5.9.5.8/psutil-stubs/_psutil_osx.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-02-21 01:26:21.000000 types-psutil-5.9.5.8/psutil-stubs/_psutil_posix.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-02-21 01:26:21.000000 types-psutil-5.9.5.8/psutil-stubs/_psutil_windows.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-02-21 01:26:21.000000 types-psutil-5.9.5.8/psutil-stubs/_pswindows.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 01:32:05.554412 types-psutil-5.9.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-02-21 01:32:04.000000 types-psutil-5.9.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:32:05.554412 types-psutil-5.9.5.8/types_psutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-02-21 01:32:05.000000 types-psutil-5.9.5.8/types_psutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-02-21 01:32:05.000000 types-psutil-5.9.5.8/types_psutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 01:32:05.000000 types-psutil-5.9.5.8/types_psutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-21 01:32:05.000000 types-psutil-5.9.5.8/types_psutil.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 01:39:31.086529 types-psutil-5.9.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-02-26 01:39:30.000000 types-psutil-5.9.5.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-26 01:39:30.000000 types-psutil-5.9.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-02-26 01:39:31.086529 types-psutil-5.9.5.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 01:39:31.082528 types-psutil-5.9.5.9/psutil-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-02-26 01:39:30.000000 types-psutil-5.9.5.9/psutil-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-02-26 01:38:11.000000 types-psutil-5.9.5.9/psutil-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-02-26 01:38:11.000000 types-psutil-5.9.5.9/psutil-stubs/_common.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-02-26 01:38:11.000000 types-psutil-5.9.5.9/psutil-stubs/_compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-02-26 01:38:11.000000 types-psutil-5.9.5.9/psutil-stubs/_psaix.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-02-26 01:38:11.000000 types-psutil-5.9.5.9/psutil-stubs/_psbsd.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-02-26 01:38:11.000000 types-psutil-5.9.5.9/psutil-stubs/_pslinux.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-02-26 01:38:11.000000 types-psutil-5.9.5.9/psutil-stubs/_psosx.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-02-26 01:38:11.000000 types-psutil-5.9.5.9/psutil-stubs/_psposix.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-02-26 01:38:11.000000 types-psutil-5.9.5.9/psutil-stubs/_pssunos.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-02-26 01:38:11.000000 types-psutil-5.9.5.9/psutil-stubs/_psutil_linux.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-02-26 01:38:11.000000 types-psutil-5.9.5.9/psutil-stubs/_psutil_osx.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-02-26 01:38:11.000000 types-psutil-5.9.5.9/psutil-stubs/_psutil_posix.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-02-26 01:38:11.000000 types-psutil-5.9.5.9/psutil-stubs/_psutil_windows.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-02-26 01:38:11.000000 types-psutil-5.9.5.9/psutil-stubs/_pswindows.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-26 01:39:31.086529 types-psutil-5.9.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-02-26 01:39:30.000000 types-psutil-5.9.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 01:39:31.086529 types-psutil-5.9.5.9/types_psutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-02-26 01:39:31.000000 types-psutil-5.9.5.9/types_psutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-02-26 01:39:31.000000 types-psutil-5.9.5.9/types_psutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-26 01:39:31.000000 types-psutil-5.9.5.9/types_psutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-26 01:39:31.000000 types-psutil-5.9.5.9/types_psutil.egg-info/top_level.txt
```

### Comparing `types-psutil-5.9.5.8/CHANGELOG.md` & `types-psutil-5.9.5.9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 5.9.5.9 (2023-02-26)
+
+Improve many `__(a)exit__` annotations (#9696)
+
 ## 5.9.5.8 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
 
 If you're reading about this commit from an autogenerated changelog entry, this should have no user-visible impact on how the stubs are interpreted by a type checker; it's just an internal change to how typeshed's tests work.
 
 ## 5.9.5.7 (2023-02-15)
```

### Comparing `types-psutil-5.9.5.8/PKG-INFO` & `types-psutil-5.9.5.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-psutil
-Version: 5.9.5.8
+Version: 5.9.5.9
 Summary: Typing stubs for psutil
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/psutil.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `psutil`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/psutil. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `880c0da4045cd5ff2c29b73429629adf27e49d50`.
+This package was generated from typeshed commit `2daa07ddf099750acf08a004b74efafafa11cf67`.
```

### Comparing `types-psutil-5.9.5.8/psutil-stubs/__init__.pyi` & `types-psutil-5.9.5.9/psutil-stubs/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -214,15 +214,15 @@
     def terminate(self) -> None: ...
     def kill(self) -> None: ...
     def wait(self, timeout: int | None = ...) -> int: ...
 
 class Popen(Process):
     def __init__(self, *args, **kwargs) -> None: ...
     def __enter__(self) -> Self: ...
-    def __exit__(self, *args, **kwargs) -> None: ...
+    def __exit__(self, *args: object, **kwargs: object) -> None: ...
     def __getattribute__(self, name: str) -> Any: ...
 
 def pids() -> list[int]: ...
 def pid_exists(pid: int) -> bool: ...
 def process_iter(
     attrs: list[str] | tuple[str, ...] | set[str] | frozenset[str] | None = ..., ad_value: Incomplete | None = ...
 ) -> Iterator[Process]: ...
```

### Comparing `types-psutil-5.9.5.8/psutil-stubs/_common.pyi` & `types-psutil-5.9.5.9/psutil-stubs/_common.pyi`

 * *Files identical despite different names*

### Comparing `types-psutil-5.9.5.8/psutil-stubs/_compat.pyi` & `types-psutil-5.9.5.9/psutil-stubs/_compat.pyi`

 * *Files identical despite different names*

### Comparing `types-psutil-5.9.5.8/psutil-stubs/_psaix.pyi` & `types-psutil-5.9.5.9/psutil-stubs/_psaix.pyi`

 * *Files identical despite different names*

### Comparing `types-psutil-5.9.5.8/psutil-stubs/_psbsd.pyi` & `types-psutil-5.9.5.9/psutil-stubs/_psbsd.pyi`

 * *Files identical despite different names*

### Comparing `types-psutil-5.9.5.8/psutil-stubs/_pslinux.pyi` & `types-psutil-5.9.5.9/psutil-stubs/_pslinux.pyi`

 * *Files identical despite different names*

### Comparing `types-psutil-5.9.5.8/psutil-stubs/_psosx.pyi` & `types-psutil-5.9.5.9/psutil-stubs/_psosx.pyi`

 * *Files identical despite different names*

### Comparing `types-psutil-5.9.5.8/psutil-stubs/_pssunos.pyi` & `types-psutil-5.9.5.9/psutil-stubs/_pssunos.pyi`

 * *Files identical despite different names*

### Comparing `types-psutil-5.9.5.8/psutil-stubs/_psutil_linux.pyi` & `types-psutil-5.9.5.9/psutil-stubs/_psutil_linux.pyi`

 * *Files identical despite different names*

### Comparing `types-psutil-5.9.5.8/psutil-stubs/_psutil_osx.pyi` & `types-psutil-5.9.5.9/psutil-stubs/_psutil_osx.pyi`

 * *Files identical despite different names*

### Comparing `types-psutil-5.9.5.8/psutil-stubs/_psutil_posix.pyi` & `types-psutil-5.9.5.9/psutil-stubs/_psutil_posix.pyi`

 * *Files identical despite different names*

### Comparing `types-psutil-5.9.5.8/psutil-stubs/_psutil_windows.pyi` & `types-psutil-5.9.5.9/psutil-stubs/_psutil_windows.pyi`

 * *Files identical despite different names*

### Comparing `types-psutil-5.9.5.8/psutil-stubs/_pswindows.pyi` & `types-psutil-5.9.5.9/psutil-stubs/_pswindows.pyi`

 * *Files identical despite different names*

### Comparing `types-psutil-5.9.5.8/setup.py` & `types-psutil-5.9.5.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `psutil`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/psutil. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `880c0da4045cd5ff2c29b73429629adf27e49d50`.
+This package was generated from typeshed commit `2daa07ddf099750acf08a004b74efafafa11cf67`.
 '''.lstrip()
 
 setup(name=name,
-      version="5.9.5.8",
+      version="5.9.5.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/psutil.md",
```

### Comparing `types-psutil-5.9.5.8/types_psutil.egg-info/PKG-INFO` & `types-psutil-5.9.5.9/types_psutil.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-psutil
-Version: 5.9.5.8
+Version: 5.9.5.9
 Summary: Typing stubs for psutil
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/psutil.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `psutil`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/psutil. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `880c0da4045cd5ff2c29b73429629adf27e49d50`.
+This package was generated from typeshed commit `2daa07ddf099750acf08a004b74efafafa11cf67`.
```

### Comparing `types-psutil-5.9.5.8/types_psutil.egg-info/SOURCES.txt` & `types-psutil-5.9.5.9/types_psutil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

