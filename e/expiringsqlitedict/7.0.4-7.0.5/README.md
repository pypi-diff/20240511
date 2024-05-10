# Comparing `tmp/expiringsqlitedict-7.0.4.tar.gz` & `tmp/expiringsqlitedict-7.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expiringsqlitedict-7.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "expiringsqlitedict-7.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `expiringsqlitedict-7.0.4.tar` & `expiringsqlitedict-7.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      249 2023-01-17 17:32:50.440949 expiringsqlitedict-7.0.4/.gitignore
--rw-r--r--   0        0        0     1034 2024-05-07 15:05:36.603482 expiringsqlitedict-7.0.4/.readthedocs.yaml
--rw-r--r--   0        0        0      271 2018-06-07 21:48:55.951133 expiringsqlitedict-7.0.4/.travis.yml
--rw-r--r--   0        0        0     1900 2022-07-01 21:27:31.727826 expiringsqlitedict-7.0.4/CHANGELOG.txt
--rw-r--r--   0        0        0    16727 2023-07-18 23:00:00.257716 expiringsqlitedict-7.0.4/LICENSE
--rw-r--r--   0        0        0       52 2021-10-13 21:06:48.260857 expiringsqlitedict-7.0.4/Makefile
--rw-r--r--   0        0        0     3702 2023-07-18 21:30:52.504076 expiringsqlitedict-7.0.4/README.md
--rwxr-xr-x   0        0        0      988 2023-04-29 13:08:50.374197 expiringsqlitedict-7.0.4/bench.py
--rw-r--r--   0        0        0      634 2023-01-17 00:40:43.681234 expiringsqlitedict-7.0.4/docs/Makefile
--rw-r--r--   0        0        0     2302 2023-01-17 00:42:16.953463 expiringsqlitedict-7.0.4/docs/conf.py
--rw-r--r--   0        0        0       87 2023-01-17 00:44:05.124729 expiringsqlitedict-7.0.4/docs/expiringsqlitedict.rst
--rw-r--r--   0        0        0      520 2023-01-17 00:47:24.429206 expiringsqlitedict-7.0.4/docs/index.rst
--rw-r--r--   0        0        0      800 2023-01-17 00:40:43.682233 expiringsqlitedict-7.0.4/docs/make.bat
--rw-r--r--   0        0        0       40 2023-01-17 00:43:04.237580 expiringsqlitedict-7.0.4/docs/requirements.txt
--rwxr-xr-x   0        0        0     2874 2023-11-03 15:15:57.363150 expiringsqlitedict-7.0.4/justfile
--rw-r--r--   0        0        0     1300 2024-05-07 15:08:27.287081 expiringsqlitedict-7.0.4/pyproject.toml
--rwxr-xr-x   0        0        0    23434 2023-11-03 15:14:21.875453 expiringsqlitedict-7.0.4/src/expiringsqlitedict/__init__.py
--rw-r--r--   0        0        0        0 2023-01-17 00:39:05.082991 expiringsqlitedict-7.0.4/src/expiringsqlitedict/py.typed
--rwxr-xr-x   0        0        0    17983 2023-07-19 02:02:15.553877 expiringsqlitedict-7.0.4/test.py
--rw-r--r--   0        0        0     4928 1970-01-01 00:00:00.000000 expiringsqlitedict-7.0.4/PKG-INFO
+-rw-r--r--   0        0        0      249 2023-01-17 17:32:50.440949 expiringsqlitedict-7.0.5/.gitignore
+-rw-r--r--   0        0        0     1034 2024-05-10 23:24:53.048432 expiringsqlitedict-7.0.5/.readthedocs.yaml
+-rw-r--r--   0        0        0      271 2018-06-07 21:48:55.951133 expiringsqlitedict-7.0.5/.travis.yml
+-rw-r--r--   0        0        0     1900 2022-07-01 21:27:31.727826 expiringsqlitedict-7.0.5/CHANGELOG.txt
+-rw-r--r--   0        0        0    16727 2023-07-18 23:00:00.257716 expiringsqlitedict-7.0.5/LICENSE
+-rw-r--r--   0        0        0       52 2021-10-13 21:06:48.260857 expiringsqlitedict-7.0.5/Makefile
+-rw-r--r--   0        0        0     3724 2024-05-10 23:24:53.048432 expiringsqlitedict-7.0.5/README.md
+-rwxr-xr-x   0        0        0      988 2023-04-29 13:08:50.374197 expiringsqlitedict-7.0.5/bench.py
+-rw-r--r--   0        0        0      634 2023-01-17 00:40:43.681234 expiringsqlitedict-7.0.5/docs/Makefile
+-rw-r--r--   0        0        0     2302 2023-01-17 00:42:16.953463 expiringsqlitedict-7.0.5/docs/conf.py
+-rw-r--r--   0        0        0       87 2023-01-17 00:44:05.124729 expiringsqlitedict-7.0.5/docs/expiringsqlitedict.rst
+-rw-r--r--   0        0        0      520 2023-01-17 00:47:24.429206 expiringsqlitedict-7.0.5/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-01-17 00:40:43.682233 expiringsqlitedict-7.0.5/docs/make.bat
+-rw-r--r--   0        0        0       40 2023-01-17 00:43:04.237580 expiringsqlitedict-7.0.5/docs/requirements.txt
+-rwxr-xr-x   0        0        0     2855 2024-05-10 23:24:53.048432 expiringsqlitedict-7.0.5/justfile
+-rw-r--r--   0        0        0     1300 2024-05-10 23:24:53.048432 expiringsqlitedict-7.0.5/pyproject.toml
+-rwxr-xr-x   0        0        0    25836 2024-05-10 23:24:53.048432 expiringsqlitedict-7.0.5/src/expiringsqlitedict/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-17 00:39:05.082991 expiringsqlitedict-7.0.5/src/expiringsqlitedict/py.typed
+-rwxr-xr-x   0        0        0    17983 2023-07-19 02:02:15.553877 expiringsqlitedict-7.0.5/test.py
+-rw-r--r--   0        0        0     4950 1970-01-01 00:00:00.000000 expiringsqlitedict-7.0.5/PKG-INFO
```

### Comparing `expiringsqlitedict-7.0.4/.readthedocs.yaml` & `expiringsqlitedict-7.0.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-7.0.4/CHANGELOG.txt` & `expiringsqlitedict-7.0.5/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-7.0.4/LICENSE` & `expiringsqlitedict-7.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-7.0.4/README.md` & `expiringsqlitedict-7.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -74,17 +74,17 @@
 working directory.  There is a convenience justfile to do this for you when you
 run:
 
 ```sh
 just test
 ```
 
-This will run all tests against all supported versions of Python (and 3.6), as
-well as all supported versions of Alpine, CentOS, Debian, Fedora, and Ubuntu
-Linux.
+This will run all tests against all supported versions of Python (and 3.6, for
+CentOS 7 support), as well as all supported versions of Alpine, CentOS, Debian,
+Fedora, and Ubuntu Linux.
 
 ## Documentation
 
 [Documentation is available on readthedocs](https://expiringsqlitedict.readthedocs.io/)
 
 Standard Python document strings are inside the module
```

### Comparing `expiringsqlitedict-7.0.4/bench.py` & `expiringsqlitedict-7.0.5/bench.py`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-7.0.4/docs/Makefile` & `expiringsqlitedict-7.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-7.0.4/docs/conf.py` & `expiringsqlitedict-7.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-7.0.4/docs/index.rst` & `expiringsqlitedict-7.0.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-7.0.4/docs/make.bat` & `expiringsqlitedict-7.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-7.0.4/justfile` & `expiringsqlitedict-7.0.5/justfile`

 * *Files 4% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 # Test all supported centos versions
 centos-tests: (test-centos "7")
 
 # Test a particular alpine version
 test-alpine version="latest": (_run-test ("alpine:" + version) apk-setup)
 
 # Test all supported alpine versions
-alpine-tests: (test-alpine "3.15") (test-alpine "3.16") (test-alpine "3.17") (test-alpine "3.18")
+alpine-tests: (test-alpine "3.16") (test-alpine "3.17") (test-alpine "3.18") (test-alpine "3.19")
 
 _test-apt image="debian:latest": (_run-test image apt-setup)
 
 # Test a particular debian version
 test-debian version="latest": (_test-apt ("debian:" + version))
 
 # Test a particular ubuntu version
@@ -88,14 +88,14 @@
 
 _test-dnf image="fedora:latest": (_run-test image dnf-setup)
 
 # Test a particular fedora version
 test-fedora version="latest": (_test-dnf ("fedora:" + version))
 
 # Test all supported fedora versions
-fedora-tests: (test-fedora "36") (test-fedora "37") (test-fedora "38") (test-fedora "39")
+fedora-tests: (test-fedora "38") (test-fedora "39") (test-fedora "40")
 
 # Test a particular RHEL version
 test-rhel version="ubi9": (_test-dnf ("redhat/" + version))
 
 # Test all supported RHEL versions
 rhel-tests: (test-rhel "ubi8") (test-rhel "ubi9")
```

### Comparing `expiringsqlitedict-7.0.4/pyproject.toml` & `expiringsqlitedict-7.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = 'expiringsqlitedict'
 description = 'Persistent compressed expiring dict in Python, backed up by sqlite3 and json'
-version = '7.0.4'
+version = '7.0.5'
 readme = 'README.md'
 requires-python = '>= 3.6, < 4'
 license = { text = 'MPL 2.0' }
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `expiringsqlitedict-7.0.4/src/expiringsqlitedict/__init__.py` & `expiringsqlitedict-7.0.5/src/expiringsqlitedict/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import json
 import sqlite3
 from sqlite3 import sqlite_version_info
 from contextlib import ExitStack, closing, contextmanager
 from datetime import timedelta
 from types import TracebackType
-from typing import Any, Generator, Iterable, Iterator, Optional, Reversible, Tuple, Type, Union, MutableMapping
+from typing import Any, Generator, ItemsView, Iterator, KeysView, Optional, Reversible, Tuple, Type, Union, MutableMapping, ValuesView
 from weakref import finalize
 from enum import unique, Enum
 
 class Identifier:
     '''An auto-escaping identifier similar to a string.
     '''
     __slots__ = (
@@ -85,15 +85,15 @@
         with closing(connection.cursor()) as cursor:
             cursor.execute('ROLLBACK')
         raise
     else:
         with closing(connection.cursor()) as cursor:
             cursor.execute('COMMIT')
 
-class _Keys(Reversible, Iterable[str]):
+class _Keys(Reversible, KeysView[str]):
     __slots__ = (
         '_connection',
         '_table',
         '_order',
     )
 
     def __init__(
@@ -110,21 +110,38 @@
     def _iterator(self, order: str) -> Iterator[str]:
         with closing(self._connection.cursor()) as cursor:
             for row in cursor.execute(
                 f'SELECT key FROM {self._table} ORDER BY {self._order} {order}',
             ):
                 yield row[0]
 
+    def __contains__(self, obj: object) -> bool:
+        if isinstance(obj, str):
+            with closing(self._connection.cursor()) as cursor:
+                for row in cursor.execute(
+                    f'SELECT 1 FROM {self._table} WHERE key = ?',
+                    (obj,),
+                ):
+                    return True
+
+        return False
+
+    def __len__(self) -> int:
+        with closing(self._connection.cursor()) as cursor:
+            return cursor.execute(f'SELECT COUNT(*) FROM {self._table}').fetchone()[0]
+
+        assert False
+
     def __iter__(self) -> Iterator[str]:
         return self._iterator('ASC')
 
     def __reversed__(self) -> Iterator[str]:
         return self._iterator('DESC')
 
-class _Values(Reversible, Iterable[Any]):
+class _Values(Reversible, ValuesView[Any]):
     __slots__ = (
         '_connection',
         '_table',
         '_serializer',
         '_order',
     )
 
@@ -144,21 +161,40 @@
     def _iterator(self, order: str) -> Iterator[Any]:
         with closing(self._connection.cursor()) as cursor:
             for row in cursor.execute(
                 f'SELECT value FROM {self._table} ORDER BY {self._order} {order}',
             ):
                 yield self._serializer.loads(row[0])
 
+    def __contains__(self, obj: object) -> bool:
+        try:
+            serialized = self._serializer.dumps(obj)
+        except Exception:
+            return False
+        if isinstance(obj, str):
+            with closing(self._connection.cursor()) as cursor:
+                for row in cursor.execute(
+                    f'SELECT 1 FROM {self._table} WHERE value = ?',
+                    (serialized,),
+                ):
+                    return True
+
+        return False
+
+    def __len__(self) -> int:
+        with closing(self._connection.cursor()) as cursor:
+            return cursor.execute(f'SELECT COUNT(*) FROM {self._table}').fetchone()[0]
+
     def __iter__(self) -> Iterator[Any]:
         return self._iterator('ASC')
 
     def __reversed__(self) -> Iterator[Any]:
         return self._iterator('DESC')
 
-class _Items(Reversible, Iterable[Tuple[str, Any]]):
+class _Items(Reversible, ItemsView[str, Any]):
     __slots__ = (
         '_connection',
         '_table',
         '_serializer',
         '_order',
     )
 
@@ -178,14 +214,37 @@
         with closing(self._connection.cursor()) as cursor:
             for row in cursor.execute(f'''
                 SELECT key, value FROM {self._table}
                     ORDER BY {self._order} {order}
             '''):
                 yield row[0], self._serializer.loads(row[1])
 
+    def __len__(self) -> int:
+        with closing(self._connection.cursor()) as cursor:
+            return cursor.execute(f'SELECT COUNT(*) FROM {self._table}').fetchone()[0]
+
+    def __contains__(self, obj: object) -> bool:
+        key: Any
+        value: Any
+        try:
+            key, value = obj # type: ignore
+            if not isinstance(key, str):
+                return False
+            serialized = self._serializer.dumps(value)
+        except Exception:
+            return False
+
+        if isinstance(obj, str):
+            with closing(self._connection.cursor()) as cursor:
+                for row in cursor.execute(
+                    f'SELECT 1 FROM {self._table} WHERE key = ? AND value = ?',
+                    (key, serialized),
+                ):
+                    return True
+        return False
     def __iter__(self) -> Iterator[Tuple[str, Any]]:
         return self._iterator('ASC')
 
     def __reversed__(self) -> Iterator[Tuple[str, Any]]:
         return self._iterator('DESC')
 
 
@@ -275,15 +334,15 @@
         assert False, 'UNREACHABLE'
 
     def __exit__(
         self,
         type: Optional[Type[BaseException]],
         value: Optional[BaseException],
         traceback: Optional[TracebackType],
-    ) -> bool:
+    ) -> Optional[bool]:
         try:
             return self._exit_stack.__exit__(type, value, traceback)
         finally:
             del self._exit_stack
 
 class TransactionManager:
     """
@@ -349,15 +408,15 @@
         assert False, 'UNREACHABLE'
 
     def __exit__(
         self,
         type: Optional[Type[BaseException]],
         value: Optional[BaseException],
         traceback: Optional[TracebackType],
-    ) -> bool:
+    ) -> Optional[bool]:
         try:
             return self._exit_stack.__exit__(type, value, traceback)
         finally:
             del self._exit_stack
 
 class Manager:
     """
@@ -415,15 +474,15 @@
         assert False, 'UNREACHABLE'
 
     def __exit__(
         self,
         type: Optional[Type[BaseException]],
         value: Optional[BaseException],
         traceback: Optional[TracebackType],
-    ) -> bool:
+    ) -> Optional[bool]:
         try:
             return self._exit_stack.__exit__(type, value, traceback)
         finally:
             del self._exit_stack
 
 def Simple(
     *args,
@@ -436,14 +495,16 @@
     """
     Set up the sqlite dictionary manager as a non-contextmanager with a finalizer.
 
     If you set the isolation_level, you will be responsible for calling
     d.connection.commit() and d.connection.rollback() appropriately.
     """
 
+    # Needed until we drop Python 3.6 and 3.7 support so we have access to Literal.  This will happen in July.
+    assert isolation_level is None or isolation_level == 'DEFERRED' or isolation_level == 'EXCLUSIVE' or isolation_level == 'IMMEDIATE'
     db = sqlite3.connect(*args, isolation_level=isolation_level, **kwargs)
     with closing(db.cursor()) as cursor:
         cursor.execute('PRAGMA journal_mode=WAL')
         cursor.execute('PRAGMA synchronous=NORMAL')
 
     if isinstance(table, str):
         table = Identifier(table)
@@ -665,18 +726,21 @@
         return _Items(
             connection=self._connection,
             table=self._table,
             serializer=self._serializer,
             order=order,
         )
 
-    def __contains__(self, key: str) -> bool:
+    def __contains__(self, key: object) -> bool:
         '''Check if the table contains the given key.
         '''
 
+        if not isinstance(key, str):
+            return False
+
         with closing(self._connection.cursor()) as cursor:
             for _ in cursor.execute(
                 f'SELECT 1 FROM {self._table} WHERE key = ?',
                 (key,),
             ):
                 return True
         return False
```

### Comparing `expiringsqlitedict-7.0.4/test.py` & `expiringsqlitedict-7.0.5/test.py`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-7.0.4/PKG-INFO` & `expiringsqlitedict-7.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expiringsqlitedict
-Version: 7.0.4
+Version: 7.0.5
 Summary: Persistent compressed expiring dict in Python, backed up by sqlite3 and json
 Author-email: "Taylor C. Richberger" <taylor.richberger@procern.com>
 Requires-Python: >= 3.6, < 4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -100,17 +100,17 @@
 working directory.  There is a convenience justfile to do this for you when you
 run:
 
 ```sh
 just test
 ```
 
-This will run all tests against all supported versions of Python (and 3.6), as
-well as all supported versions of Alpine, CentOS, Debian, Fedora, and Ubuntu
-Linux.
+This will run all tests against all supported versions of Python (and 3.6, for
+CentOS 7 support), as well as all supported versions of Alpine, CentOS, Debian,
+Fedora, and Ubuntu Linux.
 
 ## Documentation
 
 [Documentation is available on readthedocs](https://expiringsqlitedict.readthedocs.io/)
 
 Standard Python document strings are inside the module
```

