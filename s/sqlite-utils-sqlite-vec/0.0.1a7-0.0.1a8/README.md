# Comparing `tmp/sqlite_utils_sqlite_vec-0.0.1a7-py3-none-any.whl.zip` & `tmp/sqlite_utils_sqlite_vec-0.0.1a8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
 Zip file size: 1953 bytes, number of entries: 5
--rw-r--r--  4.6 unx      289 b- stor 24-May-11 04:34 sqlite_utils_sqlite_vec/__init__.py
--rw-r--r--  4.6 unx      212 b- stor 24-May-11 04:34 sqlite_utils_sqlite_vec-0.0.1a7.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- stor 24-May-11 04:34 sqlite_utils_sqlite_vec-0.0.1a7.dist-info/WHEEL
--rw-r--r--  4.6 unx       24 b- stor 24-May-11 04:34 sqlite_utils_sqlite_vec-0.0.1a7.dist-info/top_level.txt
--rw-r--r--  4.6 unx      460 b- stor 24-May-11 04:34 sqlite_utils_sqlite_vec-0.0.1a7.dist-info/RECORD
+-rw-r--r--  4.6 unx      289 b- stor 24-May-11 05:53 sqlite_utils_sqlite_vec/__init__.py
+-rw-r--r--  4.6 unx      212 b- stor 24-May-11 05:53 sqlite_utils_sqlite_vec-0.0.1a8.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- stor 24-May-11 05:53 sqlite_utils_sqlite_vec-0.0.1a8.dist-info/WHEEL
+-rw-r--r--  4.6 unx       24 b- stor 24-May-11 05:53 sqlite_utils_sqlite_vec-0.0.1a8.dist-info/top_level.txt
+-rw-r--r--  4.6 unx      460 b- stor 24-May-11 05:53 sqlite_utils_sqlite_vec-0.0.1a8.dist-info/RECORD
 5 files, 1081 bytes uncompressed, 1081 bytes compressed:  0.0%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: sqlite_utils_sqlite_vec/__init__.py
 Comment: 
 
-Filename: sqlite_utils_sqlite_vec-0.0.1a7.dist-info/METADATA
+Filename: sqlite_utils_sqlite_vec-0.0.1a8.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_utils_sqlite_vec-0.0.1a7.dist-info/WHEEL
+Filename: sqlite_utils_sqlite_vec-0.0.1a8.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_utils_sqlite_vec-0.0.1a7.dist-info/top_level.txt
+Filename: sqlite_utils_sqlite_vec-0.0.1a8.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_utils_sqlite_vec-0.0.1a7.dist-info/RECORD
+Filename: sqlite_utils_sqlite_vec-0.0.1a8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_utils_sqlite_vec/__init__.py

```diff
@@ -1,12 +1,12 @@
 
 from sqlite_utils import hookimpl
 import sqlite_utils_sqlite_vec
 
-__version__ = "0.0.1a7"
+__version__ = "0.0.1a8"
 __version_info__ = tuple(__version__.split("."))
 
 @hookimpl
 def prepare_connection(conn):
   conn.enable_load_extension(True)
   sqlite_utils_sqlite_vec.load(conn)
   conn.enable_load_extension(False)
```

