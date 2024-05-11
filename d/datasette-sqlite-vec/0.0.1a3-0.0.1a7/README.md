# Comparing `tmp/datasette_sqlite_vec-0.0.1a3-py3-none-any.whl.zip` & `tmp/datasette_sqlite_vec-0.0.1a7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
 Zip file size: 1893 bytes, number of entries: 5
--rw-r--r--  4.6 unx      280 b- stor 24-Apr-27 19:55 datasette_sqlite_vec/__init__.py
--rw-r--r--  4.6 unx      209 b- stor 24-Apr-27 19:55 datasette_sqlite_vec-0.0.1a3.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- stor 24-Apr-27 19:55 datasette_sqlite_vec-0.0.1a3.dist-info/WHEEL
--rw-r--r--  4.6 unx       21 b- stor 24-Apr-27 19:55 datasette_sqlite_vec-0.0.1a3.dist-info/top_level.txt
--rw-r--r--  4.6 unx      445 b- stor 24-Apr-27 19:55 datasette_sqlite_vec-0.0.1a3.dist-info/RECORD
+-rw-r--r--  4.6 unx      280 b- stor 24-May-11 04:34 datasette_sqlite_vec/__init__.py
+-rw-r--r--  4.6 unx      209 b- stor 24-May-11 04:34 datasette_sqlite_vec-0.0.1a7.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- stor 24-May-11 04:34 datasette_sqlite_vec-0.0.1a7.dist-info/WHEEL
+-rw-r--r--  4.6 unx       21 b- stor 24-May-11 04:34 datasette_sqlite_vec-0.0.1a7.dist-info/top_level.txt
+-rw-r--r--  4.6 unx      445 b- stor 24-May-11 04:34 datasette_sqlite_vec-0.0.1a7.dist-info/RECORD
 5 files, 1051 bytes uncompressed, 1051 bytes compressed:  0.0%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: datasette_sqlite_vec/__init__.py
 Comment: 
 
-Filename: datasette_sqlite_vec-0.0.1a3.dist-info/METADATA
+Filename: datasette_sqlite_vec-0.0.1a7.dist-info/METADATA
 Comment: 
 
-Filename: datasette_sqlite_vec-0.0.1a3.dist-info/WHEEL
+Filename: datasette_sqlite_vec-0.0.1a7.dist-info/WHEEL
 Comment: 
 
-Filename: datasette_sqlite_vec-0.0.1a3.dist-info/top_level.txt
+Filename: datasette_sqlite_vec-0.0.1a7.dist-info/top_level.txt
 Comment: 
 
-Filename: datasette_sqlite_vec-0.0.1a3.dist-info/RECORD
+Filename: datasette_sqlite_vec-0.0.1a7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datasette_sqlite_vec/__init__.py

```diff
@@ -1,12 +1,12 @@
 
 from datasette import hookimpl
 import datasette_sqlite_vec
 
-__version__ = "0.0.1a3"
+__version__ = "0.0.1a7"
 __version_info__ = tuple(__version__.split("."))
 
 @hookimpl
 def prepare_connection(conn):
   conn.enable_load_extension(True)
   datasette_sqlite_vec.load(conn)
   conn.enable_load_extension(False)
```

