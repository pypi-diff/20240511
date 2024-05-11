# Comparing `tmp/ezfs-1.0.2.tar.gz` & `tmp/ezfs-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezfs-1.0.2.tar", last modified: Sat May  4 14:12:43 2024, max compression
+gzip compressed data, was "ezfs-1.1.0.tar", last modified: Sat May 11 14:51:50 2024, max compression
```

## Comparing `ezfs-1.0.2.tar` & `ezfs-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2024-05-04 14:12:43.418589 ezfs-1.0.2/
--rw-r--r--   0 dfritz     (502) staff       (20)     1068 2024-04-27 18:07:45.000000 ezfs-1.0.2/LICENSE
--rw-r--r--   0 dfritz     (502) staff       (20)       34 2024-04-19 22:50:42.000000 ezfs-1.0.2/MANIFEST.in
--rw-r--r--   0 dfritz     (502) staff       (20)    14932 2024-05-04 14:12:43.418218 ezfs-1.0.2/PKG-INFO
--rw-r--r--   0 dfritz     (502) staff       (20)    13355 2024-05-04 14:06:50.000000 ezfs-1.0.2/README.md
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2024-05-04 14:12:43.417560 ezfs-1.0.2/ezfs.egg-info/
--rw-r--r--   0 dfritz     (502) staff       (20)    14932 2024-05-04 14:12:43.000000 ezfs-1.0.2/ezfs.egg-info/PKG-INFO
--rw-r--r--   0 dfritz     (502) staff       (20)      191 2024-05-04 14:12:43.000000 ezfs-1.0.2/ezfs.egg-info/SOURCES.txt
--rw-r--r--   0 dfritz     (502) staff       (20)        1 2024-05-04 14:12:43.000000 ezfs-1.0.2/ezfs.egg-info/dependency_links.txt
--rw-r--r--   0 dfritz     (502) staff       (20)       97 2024-05-04 14:12:43.000000 ezfs-1.0.2/ezfs.egg-info/requires.txt
--rw-r--r--   0 dfritz     (502) staff       (20)        5 2024-05-04 14:12:43.000000 ezfs-1.0.2/ezfs.egg-info/top_level.txt
--rw-r--r--   0 dfritz     (502) staff       (20)    34425 2024-05-04 14:12:39.000000 ezfs-1.0.2/ezfs.py
--rw-r--r--   0 dfritz     (502) staff       (20)     5343 2024-04-27 18:07:45.000000 ezfs-1.0.2/pyproject.toml
--rw-r--r--   0 dfritz     (502) staff       (20)       38 2024-05-04 14:12:43.418638 ezfs-1.0.2/setup.cfg
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2024-05-11 14:51:50.176410 ezfs-1.1.0/
+-rw-r--r--   0 dfritz     (502) staff       (20)     1068 2024-04-27 18:07:45.000000 ezfs-1.1.0/LICENSE
+-rw-r--r--   0 dfritz     (502) staff       (20)       34 2024-04-19 22:50:42.000000 ezfs-1.1.0/MANIFEST.in
+-rw-r--r--   0 dfritz     (502) staff       (20)    16137 2024-05-11 14:51:50.176014 ezfs-1.1.0/PKG-INFO
+-rw-r--r--   0 dfritz     (502) staff       (20)    14560 2024-05-11 14:43:15.000000 ezfs-1.1.0/README.md
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2024-05-11 14:51:50.175370 ezfs-1.1.0/ezfs.egg-info/
+-rw-r--r--   0 dfritz     (502) staff       (20)    16137 2024-05-11 14:51:50.000000 ezfs-1.1.0/ezfs.egg-info/PKG-INFO
+-rw-r--r--   0 dfritz     (502) staff       (20)      209 2024-05-11 14:51:50.000000 ezfs-1.1.0/ezfs.egg-info/SOURCES.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)        1 2024-05-11 14:51:50.000000 ezfs-1.1.0/ezfs.egg-info/dependency_links.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)       97 2024-05-11 14:51:50.000000 ezfs-1.1.0/ezfs.egg-info/requires.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)        5 2024-05-11 14:51:50.000000 ezfs-1.1.0/ezfs.egg-info/top_level.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)    36527 2024-05-11 14:51:45.000000 ezfs-1.1.0/ezfs.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     5372 2024-05-05 19:07:12.000000 ezfs-1.1.0/pyproject.toml
+-rw-r--r--   0 dfritz     (502) staff       (20)       38 2024-05-11 14:51:50.176450 ezfs-1.1.0/setup.cfg
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2024-05-11 14:51:50.174621 ezfs-1.1.0/test/
+-rw-r--r--   0 dfritz     (502) staff       (20)    26178 2024-05-11 13:51:41.000000 ezfs-1.1.0/test/test_ezfs.py
```

### Comparing `ezfs-1.0.2/LICENSE` & `ezfs-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ezfs-1.0.2/PKG-INFO` & `ezfs-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,7 @@
-Metadata-Version: 2.1
-Name: ezfs
-Version: 1.0.2
-Summary: Minimalistic virtual filesystem adapters for Python
-Author: David Fritz
-License: MIT
-Project-URL: Home, https://github.com/pyranha-labs/ezfs
-Project-URL: Changelog, https://github.com/pyranha-labs/ezfs/releases
-Project-URL: Issues, https://github.com/pyranha-labs/ezfs/issues
-Keywords: filesystem,s3,compression
-Platform: MacOS
-Platform: Linux
-Platform: Windows
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Software Development
-Classifier: Topic :: System :: Filesystems
-Classifier: Typing :: Typed
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Provides-Extra: blosc
-Requires-Dist: blosc; extra == "blosc"
-Provides-Extra: brotli
-Requires-Dist: brotli; extra == "brotli"
-Provides-Extra: s3
-Requires-Dist: boto3; extra == "s3"
-Provides-Extra: lz4
-Requires-Dist: lz4; extra == "lz4"
-Provides-Extra: snappy
-Requires-Dist: python-snappy; extra == "snappy"
-Provides-Extra: zstd
-Requires-Dist: zstandard; extra == "zstd"
-
 
 [![os: windows mac linux](https://img.shields.io/badge/os-linux_|_macos_|_windows-blue)](https://docs.python.org/3.10/)
 [![python: 3.10+](https://img.shields.io/badge/python-3.10_|_3.11_|_3.12-blue)](https://devguide.python.org/versions)
 [![python style: google](https://img.shields.io/badge/python%20style-google-blue)](https://google.github.io/styleguide/pyguide.html)
 [![imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://github.com/PyCQA/isort)
 [![code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![code style: pycodestyle](https://img.shields.io/badge/code%20style-pycodestyle-green)](https://github.com/PyCQA/pycodestyle)
@@ -68,44 +24,50 @@
 In order to provide a streamlined UX and DX, EZFS leverages existing native Python designs and patterns,
 such as open/read/write operations, and applies them all backend storage types. The learning curve is minimal:
 if you know how to read/write a local file in Python, you also know how to read/write to any location in EZFS.
 
 Reading and writing is supported for both text and binary files across local, remote, and memory "filesystems".
 Additional compression types and storage types can be supported by extending the primary `File`, `Filesystem`,
 and `Compressor` adapters. EZFS can also be faster than "native" open/read/write operations in some scenarios,
-due to having a specialized focus. Refer to the compatibility guides, and "Why EZFS", for more information.
+due to having a specialized focus. Refer to the [Compatibility](#compatibility) guide, and [Why EZFS?](#why-ezfs),
+for more information.
 
 
 ## Table Of Contents
 
   * [Compatibility](#compatibility)
   * [Getting Started](#getting-started)
     * [Installation](#installation)
   * [How Tos](#how-tos)
-    * [Write a file with compression](#write-a-file-with-compression)
-    * [Read a file with compression](#read-a-file-with-compression)
+    * [Read or write a file](#read-or-write-a-file)
     * [Swap between filesystem types](#swap-between-filesystem-types-local-file-to-local-db)
     * [Access a file in an S3 bucket](#access-a-file-object-in-an-s3-bucket-and-use-compression)
+    * [Transform file data](#transform-file-data-such-as-base64)
   * [Why EZFS?](#why-ezfs)
     * [What does EZFS provide? What does EZFS not provide?](#what-does-ezfs-provide-what-does-ezfs-not-provide)
     * [Dependency Simplicity Example](#dependency-simplicity-example)
     * [Optimized Remote Filesystem Example](#optimized-remote-filesystem-example)
   * [Contributing](#contributing)
 
 
 ## Compatibility
 
 - Supports Python 3.10+
-- Supports multiple compression types
-  - `bz2`, `gzip`, `lzma` (when built into Python)
-  - `blosc`, `brotli`, `lz4`, `snappy`, and `zstd` (when installed separately)
 - Supports multiple storage types
-  - `sqlite3` (when built into Python)
+  - Local filesystem
+  - Temporary in-memory storage
+  - `sqlite3`, local or in-memory (when built with Python)
   - `S3` (when installed separately)
-- Theoretically any compression type, or backend storage type, by extending `Compressor`, `File`, and `Filesystem` 
+  - Any storage by extending `File` and `Filesystem`
+- Supports multiple compression types
+  - `bz2`, `gzip`, `lzma` (when built with Python)
+  - `blosc`, `brotli`, `lz4`, `snappy`, and `zstd` (when installed separately)
+  - Any compression by extending `Compressor` or `Transform`
+- Custom transformations, such as encryption/decryption, Base64 encoding/decoding, obfuscation, etc.
+  - Any data transformation by extending `Transform`
 
 
 ## Getting Started
 
 ### Installation
 
 Install EZFS via pip:
@@ -142,73 +104,97 @@
 
 EZFS filesystems and file objects are designed to work nearly identical to native `open()` file handles.
 Basic read and write operations can be directly swapped out after creating a filesystem adapter, and calling `open()`
 against the filesystem instead of Python built-ins, or 3rd party compression libraries. Here are a few examples
 of how to use the more advanced features, such as compression and remote storage. Refer to the supported operations
 table in [Why EZFS?](#why-ezfs) for information on additional features.
 
-### Write a file with compression
+### Read or write a file
 ```python
 import ezfs
 
-filesystem = ezfs.LocalFilesystem('/tmp')
-with filesystem.open('test-file.txt.gz', 'w+', compression='gzip') as out_file:
-    out_file.write('test message')
+# No default compression/decompression:
+fs = ezfs.LocalFilesystem('/tmp')
 
-# Or automatically compress all files on the "filesystem" on write:
-filesystem = ezfs.LocalFilesystem('/tmp', compression='gzip')
-with filesystem.open('test-file.txt.gz', 'w+') as out_file:
+# With default compression/decompression for all files:
+fs = ezfs.LocalFilesystem('/tmp', compression='gzip')
+
+# Use default compression from filesystem during write:
+with fs.open('test.txt.gz', 'w+') as out_file:
     out_file.write('test message')
-```
 
-### Read a file with compression
-```python
-import ezfs
+# Manually specify compression during write:
+with fs.open('test.txt.gz', 'w+', compression='gzip') as out_file:
+    out_file.write('test message')
 
-filesystem = ezfs.LocalFilesystem('/tmp')
-with filesystem.open('test-file.txt.gz', compression='gzip') as in_file:
+# Use default decompression from filesystem during read:
+with fs.open('test.txt.gz') as in_file:
     print(in_file.read())
 
-# Or automatically decompress all files on the "filesystem" on read:
-filesystem = ezfs.LocalFilesystem('/tmp', compression='gzip')
-with filesystem.open('test-file.txt.gz') as in_file:
+# Manually specify decompression during read:
+with fs.open('test.txt.gz', compression='gzip') as in_file:
     print(in_file.read())
 ```
 
 ### Swap between filesystem types (local file to local db)
 ```python
 import ezfs
 
 # Only a single change is needed, such as from a local folder:
-filesystem = ezfs.LocalFilesystem('/tmp')
+fs = ezfs.LocalFilesystem('/tmp')
 # To a local database file:
-filesystem = ezfs.SQLiteFilesystem('/tmp/tmp.db')
+fs = ezfs.SQLiteFilesystem('/tmp/tmp.db')
 
 # No change is needed to open/read/write operations:
-with filesystem.open('test-file.txt.gz', 'w+', compression='gzip') as out_file:
+with fs.open('test.txt.gz', 'w+', compression='gzip') as out_file:
     out_file.write('test message')
 ```
 
 ### Access a file (object) in an S3 bucket, and use compression
 ```python
 import ezfs
 
 # To use advanced compression types, they must be installed separately.
-filesystem = ezfs.S3BotoFilesystem(
+fs = ezfs.S3BotoFilesystem(
     'my-bucket-1234',
     access_key_id='ABC123',
     secret_access_key='abcdefg1234567',
     compression='zstd',
 )
-with filesystem.open('test-file.txt.zst', 'w+') as out_file:
+with fs.open('test.txt.zst', 'w+') as out_file:
     out_file.write('test message')
-with filesystem.open('test-file.txt.zst') as in_file:
+with fs.open('test.txt.zst') as in_file:
     print(in_file.read())
 ```
 
+### Transform file data, such as Base64
+```python
+import base64
+import ezfs
+
+b64_transform = ezfs.Transform(
+    apply=lambda data: base64.b64encode(data),  # Used on write.
+    remove=lambda data: base64.b64decode(data),  # Used on read.
+)
+
+# Transforms can be applied at the Filesystem level, or File level,
+# similar to compression, with "transform=...":
+fs = ezfs.LocalFilesystem('/tmp', transform=b64_transform)
+with fs.open('test.txt', 'w+') as out_file:
+    out_file.write('test message')
+with fs.open('test.txt', transform=b64_transform) as in_file:
+    print(in_file.read())
+
+# Transforms can be combined to create complex transformations:
+transform = ezfs.Transform.chain(
+    b64_transform,
+    ...
+)
+```
+
 
 ## Why EZFS?
 
 To simplify simple use cases.
 
 EZFS is a very lightweight library (one file!), used to optimize "simple" use cases, or provide a starting point
 for more complex use cases. What make a use case "simple? Reliance on core file/filesystem functionality, such as
@@ -241,17 +227,21 @@
 | read()                | ✅   | -      | ✅         | ✅          |
 | write()               | ✅   | -      | ✅         | ✅          |
 | close()               | ✅   | -      | ✅ ²       | ✅          |
 | exists()              | ✅   | -      | ✅ ³       | ✅          |
 | isfile()              | ✅   | -      | ✅ ³       | ✅          |
 | remove()              | ✅   | -      | ✅ ³       | ✅          |
 | rename()              | ✅   | -      | ✅ ³       | ✅          |
-| Memory file storage   | ✅   | ✅      | ✅         | ✅          |
+| Text files            | ✅   | -      | ✅ ² ³     | ✅          |
+| Binary files          | ✅   | -      | ✅ ² ³     | ✅          |
+| Local file storage    | ✅   | -      | ✅         | ✅          |
+| Memory file storage   | ✅   | -      | ✅         | ✅          |
 | S3 file storage       | ❌   | ✅      | ✅         | ✅          |
 | SQLite file storage   | ✅ ¹ | -      | ✅         | ✅          |
+| Custom data transform | ✅   | -      | ✅         | ✅          |
 | bz2 compression       | ✅ ¹ | -      | ✅         | ✅          |
 | gzip compression      | ✅ ¹ | -      | ✅         | ✅          |
 | lzma compression      | ✅ ¹ | -      | ✅         | ✅          |
 | blosc compression     | ❌   | ✅      | ✅         | ✅          |
 | brotli compression    | ❌   | ✅      | ✅         | ✅          |
 | lz4 compression       | ❌   | ✅      | ✅         | ✅          |
 | snappy compression    | ❌   | ✅      | ✅         | ✅          |
@@ -306,26 +296,30 @@
 
 Here is a basic performance example, using S3 + `pandas` to store DataFrames. EZFS can optimize the S3 client used
 to reduce networking overhead, leading to improved performance. The optimization benefit is greater with small files,
 but even larger files benefit, and the simplicity to use stays the same.
 - Small file: 100K
 - Large file: 1M
 - 100 iterations per test
+- s3fs 2024.2.0
+- ezfs 1.0.0
 
 | Scenario               | Write    | Read     |
 |------------------------|----------|----------|
 | pandas s3fs small raw  | 25.0 sec | 15.6 sec |
 | pandas ezfs small raw  | 16.9 sec |  8.3 sec |
 | pandas s3fs large raw  | 47.3 sec | 17.9 sec |
 | pandas ezfs large raw  | 28.7 sec | 11.2 sec |
 | pandas s3fs small zstd | 20.2 sec | 12.0 sec |
 | pandas ezfs small zstd | 12.6 sec |  6.8 sec |
 | pandas s3fs large zstd | 37.4 sec | 18.1 sec |
 | pandas ezfs large zstd | 21.5 sec | 11.1 sec |
 
+> Additional comparisons can be found in [Benchmarks](docs/benchmarks.md)
+
 
 ### Contributing
 
 EZFS is not currently accepting new features. Minor features may be added to improve the native use cases,
 but outside minor changes it will only receive bug fixes and dependency updates. This decision is to ensure
 EZFS remains focused on its primary goal: stay simple and efficient, by focusing on simple use cases.
 Feel free to import, fork, copy, etc., to other projects to expand the scope of its ecosystem. Refer to the
```

### Comparing `ezfs-1.0.2/README.md` & `ezfs-1.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,51 @@
+Metadata-Version: 2.1
+Name: ezfs
+Version: 1.1.0
+Summary: Minimalistic virtual filesystem adapters for Python
+Author: David Fritz
+License: MIT
+Project-URL: Home, https://github.com/pyranha-labs/ezfs
+Project-URL: Changelog, https://github.com/pyranha-labs/ezfs/releases
+Project-URL: Issues, https://github.com/pyranha-labs/ezfs/issues
+Keywords: filesystem,s3,compression
+Platform: MacOS
+Platform: Linux
+Platform: Windows
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development
+Classifier: Topic :: System :: Filesystems
+Classifier: Typing :: Typed
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Provides-Extra: blosc
+Requires-Dist: blosc; extra == "blosc"
+Provides-Extra: brotli
+Requires-Dist: brotli; extra == "brotli"
+Provides-Extra: s3
+Requires-Dist: boto3; extra == "s3"
+Provides-Extra: lz4
+Requires-Dist: lz4; extra == "lz4"
+Provides-Extra: snappy
+Requires-Dist: python-snappy; extra == "snappy"
+Provides-Extra: zstd
+Requires-Dist: zstandard; extra == "zstd"
+
 
 [![os: windows mac linux](https://img.shields.io/badge/os-linux_|_macos_|_windows-blue)](https://docs.python.org/3.10/)
 [![python: 3.10+](https://img.shields.io/badge/python-3.10_|_3.11_|_3.12-blue)](https://devguide.python.org/versions)
 [![python style: google](https://img.shields.io/badge/python%20style-google-blue)](https://google.github.io/styleguide/pyguide.html)
 [![imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://github.com/PyCQA/isort)
 [![code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![code style: pycodestyle](https://img.shields.io/badge/code%20style-pycodestyle-green)](https://github.com/PyCQA/pycodestyle)
@@ -24,44 +68,50 @@
 In order to provide a streamlined UX and DX, EZFS leverages existing native Python designs and patterns,
 such as open/read/write operations, and applies them all backend storage types. The learning curve is minimal:
 if you know how to read/write a local file in Python, you also know how to read/write to any location in EZFS.
 
 Reading and writing is supported for both text and binary files across local, remote, and memory "filesystems".
 Additional compression types and storage types can be supported by extending the primary `File`, `Filesystem`,
 and `Compressor` adapters. EZFS can also be faster than "native" open/read/write operations in some scenarios,
-due to having a specialized focus. Refer to the compatibility guides, and "Why EZFS", for more information.
+due to having a specialized focus. Refer to the [Compatibility](#compatibility) guide, and [Why EZFS?](#why-ezfs),
+for more information.
 
 
 ## Table Of Contents
 
   * [Compatibility](#compatibility)
   * [Getting Started](#getting-started)
     * [Installation](#installation)
   * [How Tos](#how-tos)
-    * [Write a file with compression](#write-a-file-with-compression)
-    * [Read a file with compression](#read-a-file-with-compression)
+    * [Read or write a file](#read-or-write-a-file)
     * [Swap between filesystem types](#swap-between-filesystem-types-local-file-to-local-db)
     * [Access a file in an S3 bucket](#access-a-file-object-in-an-s3-bucket-and-use-compression)
+    * [Transform file data](#transform-file-data-such-as-base64)
   * [Why EZFS?](#why-ezfs)
     * [What does EZFS provide? What does EZFS not provide?](#what-does-ezfs-provide-what-does-ezfs-not-provide)
     * [Dependency Simplicity Example](#dependency-simplicity-example)
     * [Optimized Remote Filesystem Example](#optimized-remote-filesystem-example)
   * [Contributing](#contributing)
 
 
 ## Compatibility
 
 - Supports Python 3.10+
-- Supports multiple compression types
-  - `bz2`, `gzip`, `lzma` (when built into Python)
-  - `blosc`, `brotli`, `lz4`, `snappy`, and `zstd` (when installed separately)
 - Supports multiple storage types
-  - `sqlite3` (when built into Python)
+  - Local filesystem
+  - Temporary in-memory storage
+  - `sqlite3`, local or in-memory (when built with Python)
   - `S3` (when installed separately)
-- Theoretically any compression type, or backend storage type, by extending `Compressor`, `File`, and `Filesystem` 
+  - Any storage by extending `File` and `Filesystem`
+- Supports multiple compression types
+  - `bz2`, `gzip`, `lzma` (when built with Python)
+  - `blosc`, `brotli`, `lz4`, `snappy`, and `zstd` (when installed separately)
+  - Any compression by extending `Compressor` or `Transform`
+- Custom transformations, such as encryption/decryption, Base64 encoding/decoding, obfuscation, etc.
+  - Any data transformation by extending `Transform`
 
 
 ## Getting Started
 
 ### Installation
 
 Install EZFS via pip:
@@ -98,73 +148,97 @@
 
 EZFS filesystems and file objects are designed to work nearly identical to native `open()` file handles.
 Basic read and write operations can be directly swapped out after creating a filesystem adapter, and calling `open()`
 against the filesystem instead of Python built-ins, or 3rd party compression libraries. Here are a few examples
 of how to use the more advanced features, such as compression and remote storage. Refer to the supported operations
 table in [Why EZFS?](#why-ezfs) for information on additional features.
 
-### Write a file with compression
+### Read or write a file
 ```python
 import ezfs
 
-filesystem = ezfs.LocalFilesystem('/tmp')
-with filesystem.open('test-file.txt.gz', 'w+', compression='gzip') as out_file:
-    out_file.write('test message')
+# No default compression/decompression:
+fs = ezfs.LocalFilesystem('/tmp')
 
-# Or automatically compress all files on the "filesystem" on write:
-filesystem = ezfs.LocalFilesystem('/tmp', compression='gzip')
-with filesystem.open('test-file.txt.gz', 'w+') as out_file:
+# With default compression/decompression for all files:
+fs = ezfs.LocalFilesystem('/tmp', compression='gzip')
+
+# Use default compression from filesystem during write:
+with fs.open('test.txt.gz', 'w+') as out_file:
     out_file.write('test message')
-```
 
-### Read a file with compression
-```python
-import ezfs
+# Manually specify compression during write:
+with fs.open('test.txt.gz', 'w+', compression='gzip') as out_file:
+    out_file.write('test message')
 
-filesystem = ezfs.LocalFilesystem('/tmp')
-with filesystem.open('test-file.txt.gz', compression='gzip') as in_file:
+# Use default decompression from filesystem during read:
+with fs.open('test.txt.gz') as in_file:
     print(in_file.read())
 
-# Or automatically decompress all files on the "filesystem" on read:
-filesystem = ezfs.LocalFilesystem('/tmp', compression='gzip')
-with filesystem.open('test-file.txt.gz') as in_file:
+# Manually specify decompression during read:
+with fs.open('test.txt.gz', compression='gzip') as in_file:
     print(in_file.read())
 ```
 
 ### Swap between filesystem types (local file to local db)
 ```python
 import ezfs
 
 # Only a single change is needed, such as from a local folder:
-filesystem = ezfs.LocalFilesystem('/tmp')
+fs = ezfs.LocalFilesystem('/tmp')
 # To a local database file:
-filesystem = ezfs.SQLiteFilesystem('/tmp/tmp.db')
+fs = ezfs.SQLiteFilesystem('/tmp/tmp.db')
 
 # No change is needed to open/read/write operations:
-with filesystem.open('test-file.txt.gz', 'w+', compression='gzip') as out_file:
+with fs.open('test.txt.gz', 'w+', compression='gzip') as out_file:
     out_file.write('test message')
 ```
 
 ### Access a file (object) in an S3 bucket, and use compression
 ```python
 import ezfs
 
 # To use advanced compression types, they must be installed separately.
-filesystem = ezfs.S3BotoFilesystem(
+fs = ezfs.S3BotoFilesystem(
     'my-bucket-1234',
     access_key_id='ABC123',
     secret_access_key='abcdefg1234567',
     compression='zstd',
 )
-with filesystem.open('test-file.txt.zst', 'w+') as out_file:
+with fs.open('test.txt.zst', 'w+') as out_file:
     out_file.write('test message')
-with filesystem.open('test-file.txt.zst') as in_file:
+with fs.open('test.txt.zst') as in_file:
     print(in_file.read())
 ```
 
+### Transform file data, such as Base64
+```python
+import base64
+import ezfs
+
+b64_transform = ezfs.Transform(
+    apply=lambda data: base64.b64encode(data),  # Used on write.
+    remove=lambda data: base64.b64decode(data),  # Used on read.
+)
+
+# Transforms can be applied at the Filesystem level, or File level,
+# similar to compression, with "transform=...":
+fs = ezfs.LocalFilesystem('/tmp', transform=b64_transform)
+with fs.open('test.txt', 'w+') as out_file:
+    out_file.write('test message')
+with fs.open('test.txt', transform=b64_transform) as in_file:
+    print(in_file.read())
+
+# Transforms can be combined to create complex transformations:
+transform = ezfs.Transform.chain(
+    b64_transform,
+    ...
+)
+```
+
 
 ## Why EZFS?
 
 To simplify simple use cases.
 
 EZFS is a very lightweight library (one file!), used to optimize "simple" use cases, or provide a starting point
 for more complex use cases. What make a use case "simple? Reliance on core file/filesystem functionality, such as
@@ -197,17 +271,21 @@
 | read()                | ✅   | -      | ✅         | ✅          |
 | write()               | ✅   | -      | ✅         | ✅          |
 | close()               | ✅   | -      | ✅ ²       | ✅          |
 | exists()              | ✅   | -      | ✅ ³       | ✅          |
 | isfile()              | ✅   | -      | ✅ ³       | ✅          |
 | remove()              | ✅   | -      | ✅ ³       | ✅          |
 | rename()              | ✅   | -      | ✅ ³       | ✅          |
-| Memory file storage   | ✅   | ✅      | ✅         | ✅          |
+| Text files            | ✅   | -      | ✅ ² ³     | ✅          |
+| Binary files          | ✅   | -      | ✅ ² ³     | ✅          |
+| Local file storage    | ✅   | -      | ✅         | ✅          |
+| Memory file storage   | ✅   | -      | ✅         | ✅          |
 | S3 file storage       | ❌   | ✅      | ✅         | ✅          |
 | SQLite file storage   | ✅ ¹ | -      | ✅         | ✅          |
+| Custom data transform | ✅   | -      | ✅         | ✅          |
 | bz2 compression       | ✅ ¹ | -      | ✅         | ✅          |
 | gzip compression      | ✅ ¹ | -      | ✅         | ✅          |
 | lzma compression      | ✅ ¹ | -      | ✅         | ✅          |
 | blosc compression     | ❌   | ✅      | ✅         | ✅          |
 | brotli compression    | ❌   | ✅      | ✅         | ✅          |
 | lz4 compression       | ❌   | ✅      | ✅         | ✅          |
 | snappy compression    | ❌   | ✅      | ✅         | ✅          |
@@ -262,26 +340,30 @@
 
 Here is a basic performance example, using S3 + `pandas` to store DataFrames. EZFS can optimize the S3 client used
 to reduce networking overhead, leading to improved performance. The optimization benefit is greater with small files,
 but even larger files benefit, and the simplicity to use stays the same.
 - Small file: 100K
 - Large file: 1M
 - 100 iterations per test
+- s3fs 2024.2.0
+- ezfs 1.0.0
 
 | Scenario               | Write    | Read     |
 |------------------------|----------|----------|
 | pandas s3fs small raw  | 25.0 sec | 15.6 sec |
 | pandas ezfs small raw  | 16.9 sec |  8.3 sec |
 | pandas s3fs large raw  | 47.3 sec | 17.9 sec |
 | pandas ezfs large raw  | 28.7 sec | 11.2 sec |
 | pandas s3fs small zstd | 20.2 sec | 12.0 sec |
 | pandas ezfs small zstd | 12.6 sec |  6.8 sec |
 | pandas s3fs large zstd | 37.4 sec | 18.1 sec |
 | pandas ezfs large zstd | 21.5 sec | 11.1 sec |
 
+> Additional comparisons can be found in [Benchmarks](docs/benchmarks.md)
+
 
 ### Contributing
 
 EZFS is not currently accepting new features. Minor features may be added to improve the native use cases,
 but outside minor changes it will only receive bug fixes and dependency updates. This decision is to ensure
 EZFS remains focused on its primary goal: stay simple and efficient, by focusing on simple use cases.
 Feel free to import, fork, copy, etc., to other projects to expand the scope of its ecosystem. Refer to the
```

### Comparing `ezfs-1.0.2/ezfs.egg-info/PKG-INFO` & `ezfs-1.1.0/ezfs.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezfs
-Version: 1.0.2
+Version: 1.1.0
 Summary: Minimalistic virtual filesystem adapters for Python
 Author: David Fritz
 License: MIT
 Project-URL: Home, https://github.com/pyranha-labs/ezfs
 Project-URL: Changelog, https://github.com/pyranha-labs/ezfs/releases
 Project-URL: Issues, https://github.com/pyranha-labs/ezfs/issues
 Keywords: filesystem,s3,compression
@@ -68,44 +68,50 @@
 In order to provide a streamlined UX and DX, EZFS leverages existing native Python designs and patterns,
 such as open/read/write operations, and applies them all backend storage types. The learning curve is minimal:
 if you know how to read/write a local file in Python, you also know how to read/write to any location in EZFS.
 
 Reading and writing is supported for both text and binary files across local, remote, and memory "filesystems".
 Additional compression types and storage types can be supported by extending the primary `File`, `Filesystem`,
 and `Compressor` adapters. EZFS can also be faster than "native" open/read/write operations in some scenarios,
-due to having a specialized focus. Refer to the compatibility guides, and "Why EZFS", for more information.
+due to having a specialized focus. Refer to the [Compatibility](#compatibility) guide, and [Why EZFS?](#why-ezfs),
+for more information.
 
 
 ## Table Of Contents
 
   * [Compatibility](#compatibility)
   * [Getting Started](#getting-started)
     * [Installation](#installation)
   * [How Tos](#how-tos)
-    * [Write a file with compression](#write-a-file-with-compression)
-    * [Read a file with compression](#read-a-file-with-compression)
+    * [Read or write a file](#read-or-write-a-file)
     * [Swap between filesystem types](#swap-between-filesystem-types-local-file-to-local-db)
     * [Access a file in an S3 bucket](#access-a-file-object-in-an-s3-bucket-and-use-compression)
+    * [Transform file data](#transform-file-data-such-as-base64)
   * [Why EZFS?](#why-ezfs)
     * [What does EZFS provide? What does EZFS not provide?](#what-does-ezfs-provide-what-does-ezfs-not-provide)
     * [Dependency Simplicity Example](#dependency-simplicity-example)
     * [Optimized Remote Filesystem Example](#optimized-remote-filesystem-example)
   * [Contributing](#contributing)
 
 
 ## Compatibility
 
 - Supports Python 3.10+
-- Supports multiple compression types
-  - `bz2`, `gzip`, `lzma` (when built into Python)
-  - `blosc`, `brotli`, `lz4`, `snappy`, and `zstd` (when installed separately)
 - Supports multiple storage types
-  - `sqlite3` (when built into Python)
+  - Local filesystem
+  - Temporary in-memory storage
+  - `sqlite3`, local or in-memory (when built with Python)
   - `S3` (when installed separately)
-- Theoretically any compression type, or backend storage type, by extending `Compressor`, `File`, and `Filesystem` 
+  - Any storage by extending `File` and `Filesystem`
+- Supports multiple compression types
+  - `bz2`, `gzip`, `lzma` (when built with Python)
+  - `blosc`, `brotli`, `lz4`, `snappy`, and `zstd` (when installed separately)
+  - Any compression by extending `Compressor` or `Transform`
+- Custom transformations, such as encryption/decryption, Base64 encoding/decoding, obfuscation, etc.
+  - Any data transformation by extending `Transform`
 
 
 ## Getting Started
 
 ### Installation
 
 Install EZFS via pip:
@@ -142,71 +148,95 @@
 
 EZFS filesystems and file objects are designed to work nearly identical to native `open()` file handles.
 Basic read and write operations can be directly swapped out after creating a filesystem adapter, and calling `open()`
 against the filesystem instead of Python built-ins, or 3rd party compression libraries. Here are a few examples
 of how to use the more advanced features, such as compression and remote storage. Refer to the supported operations
 table in [Why EZFS?](#why-ezfs) for information on additional features.
 
-### Write a file with compression
+### Read or write a file
 ```python
 import ezfs
 
-filesystem = ezfs.LocalFilesystem('/tmp')
-with filesystem.open('test-file.txt.gz', 'w+', compression='gzip') as out_file:
-    out_file.write('test message')
+# No default compression/decompression:
+fs = ezfs.LocalFilesystem('/tmp')
+
+# With default compression/decompression for all files:
+fs = ezfs.LocalFilesystem('/tmp', compression='gzip')
 
-# Or automatically compress all files on the "filesystem" on write:
-filesystem = ezfs.LocalFilesystem('/tmp', compression='gzip')
-with filesystem.open('test-file.txt.gz', 'w+') as out_file:
+# Use default compression from filesystem during write:
+with fs.open('test.txt.gz', 'w+') as out_file:
     out_file.write('test message')
-```
 
-### Read a file with compression
-```python
-import ezfs
+# Manually specify compression during write:
+with fs.open('test.txt.gz', 'w+', compression='gzip') as out_file:
+    out_file.write('test message')
 
-filesystem = ezfs.LocalFilesystem('/tmp')
-with filesystem.open('test-file.txt.gz', compression='gzip') as in_file:
+# Use default decompression from filesystem during read:
+with fs.open('test.txt.gz') as in_file:
     print(in_file.read())
 
-# Or automatically decompress all files on the "filesystem" on read:
-filesystem = ezfs.LocalFilesystem('/tmp', compression='gzip')
-with filesystem.open('test-file.txt.gz') as in_file:
+# Manually specify decompression during read:
+with fs.open('test.txt.gz', compression='gzip') as in_file:
     print(in_file.read())
 ```
 
 ### Swap between filesystem types (local file to local db)
 ```python
 import ezfs
 
 # Only a single change is needed, such as from a local folder:
-filesystem = ezfs.LocalFilesystem('/tmp')
+fs = ezfs.LocalFilesystem('/tmp')
 # To a local database file:
-filesystem = ezfs.SQLiteFilesystem('/tmp/tmp.db')
+fs = ezfs.SQLiteFilesystem('/tmp/tmp.db')
 
 # No change is needed to open/read/write operations:
-with filesystem.open('test-file.txt.gz', 'w+', compression='gzip') as out_file:
+with fs.open('test.txt.gz', 'w+', compression='gzip') as out_file:
     out_file.write('test message')
 ```
 
 ### Access a file (object) in an S3 bucket, and use compression
 ```python
 import ezfs
 
 # To use advanced compression types, they must be installed separately.
-filesystem = ezfs.S3BotoFilesystem(
+fs = ezfs.S3BotoFilesystem(
     'my-bucket-1234',
     access_key_id='ABC123',
     secret_access_key='abcdefg1234567',
     compression='zstd',
 )
-with filesystem.open('test-file.txt.zst', 'w+') as out_file:
+with fs.open('test.txt.zst', 'w+') as out_file:
+    out_file.write('test message')
+with fs.open('test.txt.zst') as in_file:
+    print(in_file.read())
+```
+
+### Transform file data, such as Base64
+```python
+import base64
+import ezfs
+
+b64_transform = ezfs.Transform(
+    apply=lambda data: base64.b64encode(data),  # Used on write.
+    remove=lambda data: base64.b64decode(data),  # Used on read.
+)
+
+# Transforms can be applied at the Filesystem level, or File level,
+# similar to compression, with "transform=...":
+fs = ezfs.LocalFilesystem('/tmp', transform=b64_transform)
+with fs.open('test.txt', 'w+') as out_file:
     out_file.write('test message')
-with filesystem.open('test-file.txt.zst') as in_file:
+with fs.open('test.txt', transform=b64_transform) as in_file:
     print(in_file.read())
+
+# Transforms can be combined to create complex transformations:
+transform = ezfs.Transform.chain(
+    b64_transform,
+    ...
+)
 ```
 
 
 ## Why EZFS?
 
 To simplify simple use cases.
 
@@ -241,17 +271,21 @@
 | read()                | ✅   | -      | ✅         | ✅          |
 | write()               | ✅   | -      | ✅         | ✅          |
 | close()               | ✅   | -      | ✅ ²       | ✅          |
 | exists()              | ✅   | -      | ✅ ³       | ✅          |
 | isfile()              | ✅   | -      | ✅ ³       | ✅          |
 | remove()              | ✅   | -      | ✅ ³       | ✅          |
 | rename()              | ✅   | -      | ✅ ³       | ✅          |
-| Memory file storage   | ✅   | ✅      | ✅         | ✅          |
+| Text files            | ✅   | -      | ✅ ² ³     | ✅          |
+| Binary files          | ✅   | -      | ✅ ² ³     | ✅          |
+| Local file storage    | ✅   | -      | ✅         | ✅          |
+| Memory file storage   | ✅   | -      | ✅         | ✅          |
 | S3 file storage       | ❌   | ✅      | ✅         | ✅          |
 | SQLite file storage   | ✅ ¹ | -      | ✅         | ✅          |
+| Custom data transform | ✅   | -      | ✅         | ✅          |
 | bz2 compression       | ✅ ¹ | -      | ✅         | ✅          |
 | gzip compression      | ✅ ¹ | -      | ✅         | ✅          |
 | lzma compression      | ✅ ¹ | -      | ✅         | ✅          |
 | blosc compression     | ❌   | ✅      | ✅         | ✅          |
 | brotli compression    | ❌   | ✅      | ✅         | ✅          |
 | lz4 compression       | ❌   | ✅      | ✅         | ✅          |
 | snappy compression    | ❌   | ✅      | ✅         | ✅          |
@@ -306,26 +340,30 @@
 
 Here is a basic performance example, using S3 + `pandas` to store DataFrames. EZFS can optimize the S3 client used
 to reduce networking overhead, leading to improved performance. The optimization benefit is greater with small files,
 but even larger files benefit, and the simplicity to use stays the same.
 - Small file: 100K
 - Large file: 1M
 - 100 iterations per test
+- s3fs 2024.2.0
+- ezfs 1.0.0
 
 | Scenario               | Write    | Read     |
 |------------------------|----------|----------|
 | pandas s3fs small raw  | 25.0 sec | 15.6 sec |
 | pandas ezfs small raw  | 16.9 sec |  8.3 sec |
 | pandas s3fs large raw  | 47.3 sec | 17.9 sec |
 | pandas ezfs large raw  | 28.7 sec | 11.2 sec |
 | pandas s3fs small zstd | 20.2 sec | 12.0 sec |
 | pandas ezfs small zstd | 12.6 sec |  6.8 sec |
 | pandas s3fs large zstd | 37.4 sec | 18.1 sec |
 | pandas ezfs large zstd | 21.5 sec | 11.1 sec |
 
+> Additional comparisons can be found in [Benchmarks](docs/benchmarks.md)
+
 
 ### Contributing
 
 EZFS is not currently accepting new features. Minor features may be added to improve the native use cases,
 but outside minor changes it will only receive bug fixes and dependency updates. This decision is to ensure
 EZFS remains focused on its primary goal: stay simple and efficient, by focusing on simple use cases.
 Feel free to import, fork, copy, etc., to other projects to expand the scope of its ecosystem. Refer to the
```

### Comparing `ezfs-1.0.2/ezfs.py` & `ezfs-1.1.0/ezfs.py`

 * *Files 19% similar despite different names*

```diff
@@ -32,16 +32,19 @@
 import re
 import typing
 from contextlib import contextmanager
 from io import UnsupportedOperation
 from os import PathLike
 from types import ModuleType
 from types import TracebackType
+from typing import Any
 from typing import Callable
+from typing import Generic
 from typing import Iterable
+from typing import TypeVar
 
 try:
     from typing import override  # pylint: disable=ungrouped-imports
 except ImportError:
     try:
         from typing_extensions import override
     except ModuleNotFoundError:
@@ -58,234 +61,177 @@
 
         class sqlite3:  # pylint: disable=invalid-name
             """Placeholder module for typing."""
 
             Cursor = None
 
 
-__version__ = "1.0.2"
-# Compressors may either be a module, or subclass of Compressor,
-# with `compress()` and `decompress()` functions.
-__COMPRESSORS__: dict[str, Compressor | ModuleType | None] = {}
-NO_COMPRESSION = "none"
+__version__ = "1.1.0"
+__COMPRESSORS__: dict[str, Transform | None] = {}
+NO_TRANSFORM = "none"
+NO_COMPRESSION = NO_TRANSFORM
 Path = str | bytes | PathLike[str] | PathLike[bytes]
 
 
-class Compressor(metaclass=abc.ABCMeta):
-    """Custom compressor to control compress/decompress logic."""
+class Transform(metaclass=abc.ABCMeta):
+    """Transformation to apply to raw bytes before writing to, or after reading from, raw storage.
 
-    @abc.abstractmethod
-    def compress(self, data: bytes) -> bytes:
-        """Shrink the data using a compression algorithm.
+    Common transformations include compression/decompression, encoding/decoding, and encrypting/decrypting.
+    Transforms may perform any operations against raw bytes, as long as they output raw bytes, and are reversible.
 
-        Args:
-            data: The original bytes to compress.
+    Transforms should be stateless, and allow reuse across multiple files after instantiation.
+    """
 
-        Returns:
-            The compressed bytes.
+    def __init__(self, apply: Callable[[bytes], bytes], remove: Callable[[bytes], bytes]) -> None:
+        """Initialize the transformation with byte modification operations.
+
+        Args:
+            apply: The function to call to modify the data before writing.
+            remove: The function to call to undo the operation when reading.
         """
-        # Example: gzip.compress(data, compresslevel=1)
+        self._dependent = None
+        self._apply = apply
+        self._remove = remove
 
-    @abc.abstractmethod
-    def decompress(self, data: bytes) -> bytes:
-        """Expand the data using a decompression algorithm.
+    def apply(self, data: bytes) -> bytes:
+        """Run the transformation against raw data.
 
         Args:
-            data: The original bytes to decompress.
+            data: The original bytes to transform.
 
         Returns:
-            The decompressed bytes.
+            The transformed bytes.
         """
-        # Example: gzip.decompress(data)
-
-
-class File(metaclass=abc.ABCMeta):
-    """Representation of a file-like object used for storage and retrival of data."""
-
-    __slots__ = (
-        "filesystem",
-        "file",
-        "mode",
-        "encoding",
-        "compression",
-    )
-    valid_modes = ("r", "w", "b", "t", "+")
+        data = self._apply(data)
+        if self._dependent:
+            data = self._dependent.apply(data)
+        return data
 
-    def __init__(
-        self,
-        filesystem: Filesystem,
-        file: str,
-        mode: str = "rt",
-        encoding: str = "utf-8",
-        compression: str | Compressor | ModuleType | None = NO_COMPRESSION,
-    ) -> None:
-        """Initialize the base attributes of the file for read and write operations.
+    @staticmethod
+    def chain(*transforms: Transform) -> Transform:
+        """Combine multiple transformations together to modify data on read and write.
 
         Args:
-            filesystem: Original filesystem used to create the File.
-            file: Location of the file in the filesystem.
-            mode: Options used to open the file. See `File.valid_modes` and `builtins.open()` for details.
-            encoding: Name of the encoding used to decode or encode the file when in text mode.
-            compression: Compressor type to use when reading or writing the file contents.
-                Use basic string name to load from default compressor cache.
-        """
-        self.filesystem = filesystem
-        self.file = file
-        self.mode = mode
-        self.encoding = encoding
-        self.compression = __COMPRESSORS__[compression] if isinstance(compression, str) else compression
-
-    def __repr__(self) -> str:
-        """Internal string representation of the file."""
-        return f"{self.__class__.__name__.lower()}:{self.file}"
-
-    def __str__(self) -> str:
-        """External string representation of the file."""
-        return self.file
+            transforms: All transformations to apply to the data.
+                Transformations applied in ascending order on write, and descending order on read.
 
-    def __enter__(self) -> File:
-        """Open a file for read and write operations.
-
-        Return:
-            This File in an open state as a context manager to handle read and write operations.
+        Returns:
+            The primary transformation to use to start applications and removals.
         """
-        self._open()
-        return self
-
-    def __exit__(
-        self,
-        exc_type: type[BaseException],
-        exc_value: BaseException,
-        traceback: TracebackType,  # Preserve the original python name. pylint: disable=redefined-outer-name
-    ) -> None:
-        """Cleanup anc close the File when read and write operations are complete."""
-        self._close()
-
-    def _close(self) -> None:
-        """Close any open resources used by the file."""
-        # No actions required by default. Subclasses must inherit and override if they need to close resources.
+        transforms = [transform._copy() for transform in transforms]  # pylint: disable=protected-access
+        for index, transform in enumerate(transforms):
+            if transform != transforms[-1]:
+                transform._dependent = transforms[index + 1]  # pylint: disable=protected-access
+        return transforms[0]
 
-    def _open(self) -> None:
-        """Open file for read and write operations."""
-        self._open_checks()
-
-    def _open_checks(self) -> None:
-        """Perform pre-checks before opening a file and raise exceptions matching local files."""
-        mode = self.mode
-        for char in mode:
-            if char not in self.valid_modes:
-                raise ValueError(f"Invalid mode: '{mode}'")
-        if "t" not in mode and "b" not in mode:
-            mode = f"{mode}t"
-            self.mode = mode
-        if "r" in mode and "w" in mode:
-            raise ValueError("must have exactly one of read/write mode")
-        if "t" in mode and "b" in mode:
-            raise ValueError("can't have text and binary mode at once")
+    def _copy(self) -> Transform:
+        """Create a copy of this transformation to allow use in chained operations without modifying original."""
+        return type(self)(self._apply, self._remove)
 
-    @abc.abstractmethod
-    def _read(self) -> bytes | str:
-        """Read the contents of the file."""
+    def remove(self, data: bytes) -> bytes:
+        """Reverse the transformation on previously transformed data.
 
-    def read(self) -> bytes | str:
-        """Read the contents of the file.
+        Args:
+            data: The bytes with the transformation applied.
 
-        Raises:
-            UnsupportedOperation if the file is not writeable.
+        Returns:
+            The original bytes without the transformation applied.
         """
-        self._read_checks()
-        data = self._read()
-        if self.compression:
-            data = self.compression.decompress(data)
-        if isinstance(data, bytes) and "t" in self.mode:
-            data = data.decode(self.encoding)
+        if self._dependent:
+            data = self._dependent.remove(data)
+        data = self._remove(data)
         return data
 
-    def _read_checks(self) -> None:
-        """Perform pre-checks before reading a file and raise exceptions matching local files."""
-        if "r" not in self.mode:
-            raise UnsupportedOperation("not readable")
 
-    @abc.abstractmethod
-    def _write(self, data: bytes | str) -> int:
-        """Write the contents to the file."""
+class Compressor(Transform):
+    """Transform data using a compression/decompression module."""
 
-    def write(self, content: bytes | str) -> int:
-        """Write the contents to the file.
+    def __init__(
+        self,
+        compressor: ModuleType,
+        compress_kwargs: Any | None = None,
+        decompress_kwargs: Any | None = None,
+    ) -> None:
+        """Initialize the compressor with a specific compression module.
 
         Args:
-            content: The contents to write out to the file.
+            compressor: The module, or object, with `compress()` and `decompress()` functions.
+            compress_kwargs: Keyword arguments to use during compression. Support varies by compressor.
+            decompress_kwargs: Keyword arguments to use during decompression. Support varies by compressor.
+        """
+        super().__init__(self._compress, self._decompress)
+        self.compressor = compressor
+        self.compression_kwargs = dict(compress_kwargs or {})
+        self.decompression_kwargs = dict(decompress_kwargs or {})
 
-        Returns:
-            Number of bytes written.
+    @override
+    def _copy(self) -> Transform:
+        return type(self)(self.compressor, self.compression_kwargs.copy(), self.decompression_kwargs.copy())
 
-        Raises:
-            UnsupportedOperation if the file is not writeable.
-            TypeError if the contents are invalid.
-        """
-        self._write_checks(content)
-        if self.compression:
-            if isinstance(content, str):
-                content = content.encode(self.encoding)
-            content = self.compression.compress(content)
-        return self._write(content)
+    def _compress(self, data: bytes) -> bytes:
+        """Compress the data using the provided module."""
+        return self.compressor.compress(data, **self.compression_kwargs)
 
-    def _write_checks(self, content: bytes | str) -> None:
-        """Perform pre-checks before writing a file and raise exceptions matching local filesystem behavior."""
-        if "w" not in self.mode:
-            raise UnsupportedOperation("not writeable")
-        if not isinstance(content, (bytes, str)):
-            raise TypeError("write() argument must be bytes or str")
-        if isinstance(content, bytes) and "b" not in self.mode:
-            raise TypeError("write() argument must be str, not bytes")
-        if isinstance(content, str) and "t" not in self.mode:
-            raise TypeError("write() argument must be bytes, not str")
-        if not isinstance(content, (bytes, str)):
-            raise TypeError("write() argument must be bytes, not str")
+    def _decompress(self, data: bytes) -> bytes:
+        """Decompress the data using the provided module."""
+        return self.compressor.decompress(data, **self.decompression_kwargs)
 
 
 class Filesystem(metaclass=abc.ABCMeta):
     """Collection of file-like objects used for storage and retrival of data."""
 
     def __init__(
         self,
         file_type: type[File],
-        compression: str | Compressor | ModuleType | None = NO_COMPRESSION,
+        compression: str | Transform | None = NO_COMPRESSION,
+        transform: Transform | None = None,
     ) -> None:
         """Initialize the base attributes of the filesystem for read and write operations.
 
         Args:
             file_type: File adapter type to use when opening files for read and write operations.
             compression: Default compression type to use when reading or writing file contents.
                 Use basic string name to load from default compressor cache.
+            transform: Default transformation used when reading or writing the file contents.
+                Transformations are applied before compression when writing, and after decompression when reading.
         """
-        self.ftype = file_type
-        self.compression = compression
         if not __COMPRESSORS__:
             init_compressors()
+        self.ftype = file_type
+        self.compression = compression
+        self.transform = transform
 
     @contextmanager
     def open(
         self,
         file: str,
         mode: str = "rt",
         encoding: str = "utf-8",
-        compression: str | None = None,
+        compression: str | Transform | None = None,
+        transform: Transform | None = None,
     ) -> File:
         """Open file for read and write operations, and perform automatic cleanup.
 
         Args:
             file: Location of the file in the filesystem.
             mode: Options used to open the file. See "open()" for details.
             encoding: Name of the encoding used to decode or encode the file when in text mode.
             compression: Type of compression used when reading or writing the file contents.
                 Use `None` to default to the Filesystem compression type.
-                Default Filesystem compression is no compression.
+            transform: Type of transformation used when reading or writing the file contents.
+                Use `None` to default to the Filesystem transformation type.
         """
-        with self.ftype(self, file, mode=mode, encoding=encoding, compression=compression or self.compression) as _file:
+        with self.ftype(
+            self,
+            file,
+            mode=mode,
+            encoding=encoding,
+            compression=compression or self.compression,
+            transform=transform or self.transform,
+        ) as _file:
             yield _file
 
     def exists(self, path: str | bytes | PathLike[str] | PathLike[bytes]) -> bool:
         """Check whether path refers to an existing location in the filesystem.
 
         Behavior mirrors `os.path.exists()` as closely as possible if supported by the filesystem.
 
@@ -330,15 +276,15 @@
         """
         if dir_fd is not None:
             # Non-local filesystems do not support dir_fd. Default to not allowed.
             raise NotImplementedError(f"dir_fd is not supported by {self.__class__.__name__}")
         if not self.exists(path):
             raise FileNotFoundError(errno.ENOENT, f"No such file or directory: {path}")
         if not self.isfile(path):
-            raise OSError(1, f"Operation not permitted: {path}")
+            raise OSError(errno.EPERM, f"Operation not permitted: {path}")
         self._remove(path, dir_fd=dir_fd)
 
     @abc.abstractmethod
     def _rename(self, src: Path, dst: Path, *, src_dir_fd: int | None = None, dst_dir_fd: int | None = None) -> None:
         """Rename (move) the file from source to destination."""
 
     def rename(self, src: Path, dst: Path, *, src_dir_fd: int | None = None, dst_dir_fd: int | None = None) -> None:
@@ -360,129 +306,226 @@
         """
         if src_dir_fd is not None or dst_dir_fd is not None:
             # Non-local filesystems do not support dir_fd(s). Default to not allowed.
             raise NotImplementedError(f"src_dir_fd and dst_dir_fd are not supported by {self.__class__.__name__}")
         if not self.exists(src):
             raise FileNotFoundError(errno.ENOENT, f"No such file or directory: {src}")
         if not self.isfile(src):
-            raise OSError(1, f"Operation not permitted: {src}")
+            raise OSError(errno.EPERM, f"Operation not permitted: {src}")
         if self.exists(dst):
             raise FileExistsError(errno.EEXIST, f"File exists: {dst}")
         self._rename(src, dst, src_dir_fd=src_dir_fd, dst_dir_fd=dst_dir_fd)
 
 
-class LocalFile(File):
-    """File-like object on a local filesystem."""
+FilesystemType = TypeVar("FilesystemType", bound=Filesystem)  # pylint: disable=invalid-name
 
-    __slots__ = ("_file",)
+
+class File(Generic[FilesystemType], metaclass=abc.ABCMeta):
+    """Representation of a file-like object used for storage and retrival of data."""
+
+    __slots__ = (
+        "filesystem",
+        "file",
+        "mode",
+        "encoding",
+        "compression",
+        "transform",
+    )
+    valid_modes = ("r", "w", "b", "t", "+")
+    skip_write_encode = False
 
     def __init__(  # pylint: disable=too-many-arguments
         self,
-        filesystem: LocalFilesystem,
+        filesystem: FilesystemType,
         file: str,
         mode: str = "rt",
         encoding: str = "utf-8",
-        compression: str = NO_COMPRESSION,
+        compression: str | Transform | None = NO_COMPRESSION,
+        transform: Transform | None = None,
     ) -> None:
-        """Initialize the base attributes of the local file for read and write operations.
+        """Initialize the base attributes of the file for read and write operations.
 
         Args:
             filesystem: Original filesystem used to create the File.
-            file: Location of the file on the local filesystem.
-            mode: Options used to open the file.
+            file: Location of the file in the filesystem.
+            mode: Options used to open the file. See `File.valid_modes` and `builtins.open()` for details.
             encoding: Name of the encoding used to decode or encode the file when in text mode.
-            compression: Type of compression used when reading or writing the file contents.
+            compression: Compressor type to use when reading or writing the file contents.
+                Use basic string name to load from default compressor cache.
+            transform: Data transformation used when reading or writing the file contents.
+                Transformations are applied before compression when writing, and after decompression when reading.
         """
-        # Left strip to ensure that absolute paths are treated as relative, so that the filesystem directory is root.
-        super().__init__(filesystem, file, mode=mode, encoding=encoding, compression=compression)
-        self.filesystem: LocalFilesystem = filesystem  # Set again with typehint to avoid lint warnings.
-        self._file = None
+        self.filesystem = filesystem
+        self.file = file
+        self.mode = mode
+        self.encoding = encoding
+        self.compression = __COMPRESSORS__[compression] if isinstance(compression, str) else compression
+        self.transform = transform if transform != NO_TRANSFORM else None
+
+    def __repr__(self) -> str:
+        """Internal string representation of the file."""
+        return f"{self.__class__.__name__.lower()}:{self.file}"
 
-    @override
     def __str__(self) -> str:
-        # Use relative path within filesystem to avoid exposing full path in case it contains sensitive information.
-        return self.file.replace(self.filesystem.directory, "")
+        """External string representation of the file."""
+        return self.file
+
+    def __enter__(self) -> File:
+        """Open a file for read and write operations.
+
+        Return:
+            This File in an open state as a context manager to handle read and write operations.
+        """
+        self._open()
+        return self
+
+    def __exit__(
+        self,
+        exc_type: type[BaseException],
+        exc_value: BaseException,
+        traceback: TracebackType,  # Preserve the original python name. pylint: disable=redefined-outer-name
+    ) -> None:
+        """Cleanup anc close the File when read and write operations are complete."""
+        self._close()
 
-    @override
     def _close(self) -> None:
-        self._file.close()
-        self._file = None
+        """Close any open resources used by the file."""
+        # No actions required by default. Subclasses must inherit and override if they need to close resources.
 
-    @override
     def _open(self) -> None:
-        # Do not call super full open checks, they will be performed by the native file open operation with local files.
+        """Open file for read and write operations."""
+        self._open_checks()
+
+    def _open_checks(self) -> None:
+        """Perform pre-checks before opening a file and raise exceptions matching local files."""
         mode = self.mode
+        for char in mode:
+            if char not in self.valid_modes:
+                raise ValueError(f"Invalid mode: '{mode}'")
         if "t" not in mode and "b" not in mode:
             mode = f"{mode}t"
+            self.mode = mode
+        if "r" in mode and "w" in mode:
+            raise ValueError("must have exactly one of read/write mode")
+        if "t" in mode and "b" in mode:
+            raise ValueError("can't have text and binary mode at once")
 
-        encoding = self.encoding
-        if self.compression:
-            # Force the mode to binary to allow utilizing native open operation to read/write compressed data.
-            mode = mode.replace("t", "b")
-            encoding = None
-        self._file = open(self.file, mode, encoding=encoding)  # pylint: disable=consider-using-with
+    @abc.abstractmethod
+    def _read(self) -> bytes:
+        """Read the raw contents of the file."""
 
-    @override
-    def _read(self) -> bytes | str:
-        return self._file.read()
+    def read(self) -> bytes | str:
+        """Read the contents of the file.
+
+        Raises:
+            UnsupportedOperation if the file is not writeable.
+        """
+        self._read_checks()
+        data = self._read()
+        if self.compression:
+            data = self.compression.remove(data)
+        if self.transform:
+            data = self.transform.remove(data)
+        if isinstance(data, bytes) and "t" in self.mode:
+            data = data.decode(self.encoding)
+        return data
 
-    @override
     def _read_checks(self) -> None:
-        # No checks are needed for local files, they will raise directly from native code.
-        pass
+        """Perform pre-checks before reading a file and raise exceptions matching local files."""
+        if "r" not in self.mode:
+            raise UnsupportedOperation("not readable")
 
-    @override
-    def _write(self, data: bytes | str) -> int:
-        return self._file.write(data)
+    @abc.abstractmethod
+    def _write(self, data: bytes) -> int:
+        """Write the raw contents to the file."""
+
+    def write(self, content: bytes | str) -> int:
+        """Write the contents to the file.
+
+        Args:
+            content: The contents to write out to the file.
+
+        Returns:
+            Number of bytes written.
+
+        Raises:
+            UnsupportedOperation if the file is not writeable.
+            TypeError if the contents are invalid.
+        """
+        self._write_checks(content)
+        if (self.compression or self.transform) and isinstance(content, str):
+            content = content.encode(self.encoding)
+        if self.transform:
+            content = self.transform.apply(content)
+        if self.compression:
+            content = self.compression.apply(content)
+        if not self.skip_write_encode and isinstance(content, str):
+            content = content.encode(self.encoding)
+        return self._write(content)
 
-    @override
     def _write_checks(self, content: bytes | str) -> None:
-        # No checks are needed for local files, they will raise directly from native code.
-        pass
+        """Perform pre-checks before writing a file and raise exceptions matching local filesystem behavior."""
+        if "w" not in self.mode:
+            raise UnsupportedOperation("not writeable")
+        if not isinstance(content, (bytes, str)):
+            raise TypeError("write() argument must be bytes or str")
+        if isinstance(content, bytes) and "b" not in self.mode:
+            raise TypeError("write() argument must be str, not bytes")
+        if isinstance(content, str) and "t" not in self.mode:
+            raise TypeError("write() argument must be bytes, not str")
 
 
 class LocalFilesystem(Filesystem):
     """Collection of file-like objects available on a local filesystem."""
 
     def __init__(
         self,
         directory: str,
-        compression: str = NO_COMPRESSION,
+        compression: str | Transform | None = NO_COMPRESSION,
+        transform: Transform | None = None,
         safe_paths: bool = True,
     ) -> None:
         """Initialize the base attributes of the local filesystem for read and write operations.
 
         Args:
             directory: Root directory for all files available in the filesystem.
             compression: Default compression type to use when reading or writing file contents.
-                Use basic string name to load from default compressor cache.
+            transform: Default transformation used when reading or writing file contents.
             safe_paths: Whether safety checks are performed to prevent path escape attempts from filesystem directory.
                 If paths are guaranteed to be safe, disable to maximize performance.
         """
-        super().__init__(LocalFile, compression=compression)
+        super().__init__(LocalFile, compression=compression, transform=transform)
         self.ftype = LocalFile  # Set again to avoid lint errors.
         self.directory = os.path.abspath(directory)
         self.safe_paths = safe_paths
 
     @override
     @contextmanager
     def open(
         self,
         file: str,
         mode: str = "rt",
         encoding: str = "utf-8",
-        compression: str | None = None,
-    ) -> File:
+        compression: str | Transform | None = None,
+        transform: Transform | None = None,
+    ) -> LocalFile:
         path = os.path.abspath(os.path.join(self.directory, file.lstrip(os.path.sep)))
         if self.safe_paths:
             # Validate final path to file, and treat as not found if attempting to escape the root.
             if not path.startswith(self.directory):
                 raise FileNotFoundError(errno.ENOENT, f"No such file or directory: {file}")
 
-        with self.ftype(self, path, mode=mode, encoding=encoding, compression=compression or self.compression) as _file:
+        with self.ftype(
+            self,
+            path,
+            mode=mode,
+            encoding=encoding,
+            compression=compression or self.compression,
+            transform=transform or self.transform,
+        ) as _file:
             yield _file
 
     @override
     def exists(self, path: str | bytes | PathLike[str] | PathLike[bytes]) -> bool:
         return os.path.exists(path)
 
     @override
@@ -491,82 +534,108 @@
 
     @override
     def _remove(self, path: str | bytes | PathLike[str] | PathLike[bytes], *, dir_fd: int | None = None) -> None:
         pass
 
     @override
     def remove(self, path: str | bytes | PathLike[str] | PathLike[bytes], *, dir_fd: int | None = None) -> None:
+        if self.safe_paths:
+            # Validate final path to file, and treat as not found if attempting to escape the root.
+            path = self._validate(path)
         # Bypass base remove() checks to allow support for dir_fd, and 1-to-1 match with native behavior.
         os.remove(path, dir_fd=dir_fd)
 
     @override
     def _rename(self, src: Path, dst: Path, *, src_dir_fd: int | None = None, dst_dir_fd: int | None = None) -> None:
         pass
 
     @override
     def rename(self, src: Path, dst: Path, *, src_dir_fd: int | None = None, dst_dir_fd: int | None = None) -> None:
+        if self.safe_paths:
+            # Validate final path to files, and treat as not found if attempting to escape the root.
+            src = self._validate(src)
+            dst = self._validate(dst)
         # Bypass base rename() checks to allow support for dir_fd arguments, and 1-to-1 match with native behavior.
         os.rename(src, dst, src_dir_fd=src_dir_fd, dst_dir_fd=dst_dir_fd)
 
+    def _validate(self, path: str) -> str:
+        """Ensure a path is within the directory boundary for this filesystem."""
+        final_path = os.path.abspath(os.path.join(self.directory, path.lstrip(os.path.sep)))
+        if not final_path.startswith(self.directory):
+            raise FileNotFoundError(errno.ENOENT, f"No such file or directory: {path}")
+        return final_path
 
-class MemFile(File):
-    """File-like object stored in memory."""
 
-    def __init__(
-        self,
-        filesystem: MemFilesystem,
-        file: str,
-        mode: str = "rt",
-        encoding: str = "utf-8",
-        compression: str = NO_COMPRESSION,
-    ) -> None:
-        """Initialize the base attributes of the in-memory file for read and write operations.
+class LocalFile(File[LocalFilesystem]):
+    """File-like object on a local filesystem."""
 
-        Args:
-            filesystem: Original filesystem used to create the File.
-            file: Location of the file in the in-memory filesystem.
-            mode: Options used to open the file.
-            encoding: Name of the encoding used to decode or encode the file when in text mode.
-            compression: Type of compression used when reading or writing the file contents.
-        """
-        super().__init__(filesystem, file, mode=mode, encoding=encoding, compression=compression)
-        self.filesystem: MemFilesystem = filesystem  # Set again with typehint to avoid lint warnings.
+    __slots__ = ("_file",)
+    skip_write_encode = True
+
+    @override
+    def __str__(self) -> str:
+        # Use relative path within filesystem to avoid exposing full path in case it contains sensitive information.
+        return self.file.replace(self.filesystem.directory, "")
+
+    @override
+    def _close(self) -> None:
+        self._file.close()
+
+    @override
+    def _open(self) -> None:
+        # Do not call super full open checks, they will be performed by the native file open operation with local files.
+        mode = self.mode
+        if "t" not in mode and "b" not in mode:
+            mode = f"{mode}t"
+
+        encoding = self.encoding
+        if self.compression or self.transform:
+            # Force the mode to binary to allow utilizing native open operation to read/write compressed data.
+            mode = mode.replace("t", "b")
+            encoding = None
+        if "b" in mode:
+            encoding = None
+        self._file = open(self.file, mode, encoding=encoding)  # pylint: disable=attribute-defined-outside-init,consider-using-with
 
     @override
     def _read(self) -> bytes | str:
-        return self.filesystem.tree.get(self.file)
+        return self._file.read()
 
     @override
     def _read_checks(self) -> None:
-        if "r" in self.mode and self.file not in self.filesystem.tree:
-            raise FileNotFoundError(errno.ENOENT, f"No such file: '{self.file}'")
-        super()._read_checks()
+        # No checks are needed for local files, they will raise directly from native code.
+        pass
 
     @override
     def _write(self, data: bytes | str) -> int:
-        self.filesystem.tree[self.file] = data
-        return len(data)
+        return self._file.write(data)
+
+    @override
+    def _write_checks(self, content: bytes | str) -> None:
+        # No checks are needed for local files, they will raise directly from native code.
+        pass
 
 
 class MemFilesystem(Filesystem):
     """Collection of file-like objects available in an in-memory filesystem."""
 
     def __init__(
         self,
         tree: dict[str, bytes | str] | None = None,
-        compression: str = NO_COMPRESSION,
+        compression: str | Transform | None = NO_COMPRESSION,
+        transform: Transform | None = None,
     ) -> None:
         """Initialize the base attributes of the in-memory filesystem for read and write operations.
 
         Args:
             tree: Initial virtual filesystem tree contents.
             compression: Default compression type to use when reading or writing file contents.
-                Use basic string name to load from default compressor cache.
+            transform: Default transformation used when reading or writing file contents.
         """
-        super().__init__(MemFile, compression=compression)
+        super().__init__(MemFile, compression=compression, transform=transform)
         self.tree = tree or {}
 
     @override
     def isfile(self, path: str | bytes | PathLike[str] | PathLike[bytes]) -> bool:
         return str(path) in self.tree
 
     @override
@@ -574,104 +643,60 @@
         self.tree.pop(str(path))
 
     @override
     def _rename(self, src: Path, dst: Path, *, src_dir_fd: int | None = None, dst_dir_fd: int | None = None) -> None:
         self.tree[str(dst)] = self.tree.pop(str(src))
 
 
-class S3BotoFile(File):
-    """File-like object in a remote S3 bucket."""
-
-    __slots__ = (
-        "_read_response",
-        "_write_response",
-    )
-
-    def __init__(
-        self,
-        filesystem: S3BotoFilesystem,
-        file: str,
-        mode: str = "rt",
-        encoding: str = "utf-8",
-        compression: str = NO_COMPRESSION,
-    ) -> None:
-        """Initialize the base attributes of the file-like S3 object for read and write operations.
+class MemFile(File[MemFilesystem]):
+    """File-like object stored in memory."""
 
-        Args:
-            filesystem: Original filesystem used to create the File.
-            file: Location of the object in the S3 bucket.
-            mode: Options used to open the file.
-            encoding: Name of the encoding used to decode or encode the file when in text mode.
-            compression: Type of compression used when reading or writing the file contents.
-        """
-        super().__init__(filesystem, file, mode=mode, encoding=encoding, compression=compression)
-        self.filesystem: S3BotoFilesystem = filesystem  # Set again with typehint to avoid lint warnings.
-        self._read_response = None
-        self._write_response = None
+    __slots__ = ()
 
     @override
-    def __repr__(self) -> str:
-        return f"{self.filesystem.bucket_name}:{self.file}"
+    def _read(self) -> bytes:
+        return self.filesystem.tree.get(self.file)
 
     @override
-    def _read(self) -> bytes | str:
-        try:
-            self._read_response = self.filesystem.client.get_object(Bucket=self.filesystem.bucket_name, Key=self.file)
-            content = self._read_response["Body"].read()
-        except self.filesystem.ClientError as client_error:
-            # For consistency across File types, change missing objects errors to standard FileNotFoundErrors.
-            if client_error.response["Error"]["Code"] == "NoSuchKey":
-                raise FileNotFoundError(errno.ENOENT, f"No such file: {self}") from client_error
-            raise client_error
-        return content
-
-    @property
-    def read_response(self) -> dict | None:
-        """The raw S3 response after a read operation is performed."""
-        return self._read_response
+    def _read_checks(self) -> None:
+        if "r" in self.mode and self.file not in self.filesystem.tree:
+            raise FileNotFoundError(errno.ENOENT, f"No such file: '{self.file}'")
+        super()._read_checks()
 
     @override
-    def _write(self, data: bytes | str) -> int:
-        self._write_response = self.filesystem.client.put_object(
-            Body=data,
-            Bucket=self.filesystem.bucket_name,
-            Key=self.file,
-        )
+    def _write(self, data: bytes) -> int:
+        self.filesystem.tree[self.file] = data
         return len(data)
 
-    @property
-    def write_response(self) -> dict | None:
-        """The raw S3 response after a write operation is performed."""
-        return self._write_response
-
 
 class S3BotoFilesystem(Filesystem):
     """Collection of file-like objects available in a remote S3 bucket."""
 
     def __init__(  # pylint: disable=too-many-arguments
         self,
         bucket_name: str,
         access_key_id: str = None,
         secret_access_key: str = None,
         region_name: str = None,
         profile_name: str = None,
-        compression: str = NO_COMPRESSION,
+        compression: str | Transform | None = NO_COMPRESSION,
+        transform: Transform | None = None,
     ) -> None:
         """Initialize the base attributes of the S3 filesystem for read and write operations.
 
         Args:
             bucket_name: Name of the bucket with all objects available as files in the filesystem.
             access_key_id: Access key ID with permission to read/write to the bucket.
             secret_access_key: AWS secret access key with permission to read/write to the bucket.
             region_name: Default region when creating bucket connection.
             profile_name: Name of a custom profile to use, instead of default.
             compression: Default compression type to use when reading or writing file contents.
-                Use basic string name to load from default compressor cache.
+            transform: Default transformation used when reading or writing file contents.
         """
-        super().__init__(S3BotoFile, compression=compression)
+        super().__init__(S3BotoFile, compression=compression, transform=transform)
         try:
             # pylint: disable=import-outside-toplevel,invalid-name
             import boto3
             from botocore.exceptions import ClientError
 
             self.ClientError = ClientError
         except ModuleNotFoundError as error:
@@ -704,85 +729,71 @@
     @override
     def _rename(self, src: Path, dst: Path, *, src_dir_fd: int | None = None, dst_dir_fd: int | None = None) -> None:
         cp_src = {"Bucket": self.bucket_name, "Key": src}
         self.client.copy_object(Bucket=self.bucket_name, Key=str(dst), CopySource=cp_src)
         self._remove(src)
 
 
-class SQLiteFile(File):
-    """File-like object in a SQLite database."""
-
-    def __init__(
-        self,
-        filesystem: SQLiteFilesystem,
-        file: str,
-        mode: str = "rt",
-        encoding: str = "utf-8",
-        compression: str = NO_COMPRESSION,
-    ) -> None:
-        """Initialize the base attributes of the file-like database object for read and write operations.
+class S3BotoFile(File[S3BotoFilesystem]):
+    """File-like object in a remote S3 bucket."""
 
-        Args:
-            filesystem: Original filesystem used to create the File.
-            file: Location of the object in the database table.
-            mode: Options used to open the file.
-            encoding: Name of the encoding used to decode or encode the file when in text mode.
-            compression: Type of compression used when reading or writing the file contents.
-        """
-        super().__init__(filesystem, file, mode=mode, encoding=encoding, compression=compression)
-        self.filesystem: SQLiteFilesystem = filesystem  # Set again with typehint to avoid lint warnings.
+    __slots__ = ()
 
     @override
     def __repr__(self) -> str:
-        return f"sqlite3://{self.filesystem.database}?table_name={self.filesystem.table_name}&file={self.file}"
+        return f"{self.filesystem.bucket_name}:{self.file}"
 
     @override
-    def _read(self) -> bytes | str:
-        res = self.filesystem.execute(self.filesystem.read_query, (self.file,)).fetchone()
-        if res is None:
-            raise FileNotFoundError(errno.ENOENT, f"No such file: '{self.file}'")
-        content = res[0]
+    def _read(self) -> bytes:
+        try:
+            read_response = self.filesystem.client.get_object(Bucket=self.filesystem.bucket_name, Key=self.file)
+            content = read_response["Body"].read()
+        except self.filesystem.ClientError as client_error:
+            # For consistency across File types, change missing objects errors to standard FileNotFoundErrors.
+            if client_error.response["Error"]["Code"] == "NoSuchKey":
+                raise FileNotFoundError(errno.ENOENT, f"No such file: {self}") from client_error
+            raise client_error
         return content
 
     @override
-    def _write(self, data: bytes | str) -> int:
-        self.filesystem.execute(self.filesystem.write_query, (self.file, data, data))
-        self.filesystem.commit()
+    def _write(self, data: bytes) -> int:
+        self.filesystem.client.put_object(Body=data, Bucket=self.filesystem.bucket_name, Key=self.file)
         return len(data)
 
 
 class SQLiteFilesystem(Filesystem):
     """Collection of file-like objects available in a database using SQLite."""
 
-    def __init__(
+    def __init__(  # pylint: disable=too-many-arguments
         self,
-        database: str,
+        database: str = ":memory:",
         table_name: str = "files",
         file_col: str = "file",
         content_col: str = "content",
-        compression: str = NO_COMPRESSION,
+        compression: str | Transform | None = NO_COMPRESSION,
+        transform: Transform | None = None,
     ) -> None:
         """Initialize the base attributes of the database filesystem for read and write operations.
 
         Args:
             database: The path to the database file to be opened. e.g., "example.db", ":memory:", etc.
             table_name: Name of the table with data available as files in the filesystem.
             file_col: Name of the column in the table that contains the path to the files.
             content_col: Name of the column in the table that contains the raw contents for the files.
             compression: Default compression type to use when reading or writing file contents.
-                Use basic string name to load from default compressor cache.
+            transform: Default transformation used when reading or writing file contents.
         """
         for name, value in (
             ("table_name", table_name),
             ("file_col", file_col),
             ("content_col", content_col),
         ):
             if not re.match(r"^[A-za-z0-9_]+$", value):
                 raise ValueError(f"{name} may only contain letters, numbers, and underscores.")
-        super().__init__(SQLiteFile, compression=compression)
+        super().__init__(SQLiteFile, compression=compression, transform=transform)
         try:
             # pylint: disable=import-outside-toplevel,redefined-outer-name,reimported
             import sqlite3
 
         except ModuleNotFoundError as error:
             raise ModuleNotFoundError(f"sqlite3 is required to use {self.__class__.__name__}") from error
 
@@ -801,14 +812,17 @@
             f"INSERT INTO {table_name}({file_col}, {content_col}) VALUES(?, ?) "  # nosec
             f"ON CONFLICT({file_col}) DO UPDATE SET {content_col}=?;"
         )
         self.exists_query = f"SELECT {file_col} FROM {table_name} WHERE {file_col}=(?) LIMIT 1;"  # nosec
         self.remove_query = f"DELETE FROM {table_name} WHERE {file_col}=(?);"  # nosec
         self.rename_query = f"UPDATE {table_name} SET {file_col}=(?) WHERE {file_col}=(?);"  # nosec
 
+        if self.database == ":memory:":
+            self.create_table()
+
     def commit(self) -> None:
         """Commit any pending transactions to the database backend."""
         self._connection.commit()
 
     def create_table(self) -> None:
         """Create a basic table to use for storage."""
         self.execute(self._create_query)
@@ -840,14 +854,38 @@
 
     @override
     def _rename(self, src: Path, dst: Path, *, src_dir_fd: int | None = None, dst_dir_fd: int | None = None) -> None:
         self.execute(self.rename_query, (str(dst), str(src)))
         self.commit()
 
 
+class SQLiteFile(File[SQLiteFilesystem]):
+    """File-like object in a SQLite database."""
+
+    __slots__ = ()
+
+    @override
+    def __repr__(self) -> str:
+        return f"sqlite3://{self.filesystem.database}?table_name={self.filesystem.table_name}&file={self.file}"
+
+    @override
+    def _read(self) -> bytes:
+        res = self.filesystem.execute(self.filesystem.read_query, (self.file,)).fetchone()
+        if res is None:
+            raise FileNotFoundError(errno.ENOENT, f"No such file: '{self.file}'")
+        content = res[0]
+        return content
+
+    @override
+    def _write(self, data: bytes) -> int:
+        self.filesystem.execute(self.filesystem.write_query, (self.file, data, data))
+        self.filesystem.commit()
+        return len(data)
+
+
 def init_compressors() -> list[str]:
     """Search the system for available compression algorithms.
 
     Returns:
         List of the available compression types for reading and writing files.
     """
     __COMPRESSORS__.update({None: None, NO_COMPRESSION: None})
@@ -862,11 +900,15 @@
         ("lz4", "lz4.frame"),
         ("snappy",),
         ("zstd", "zstandard"),
     )
     for lib in libs:
         name, module_name = lib if len(lib) == 2 else (lib[0], lib[0])  # pylint: disable=unbalanced-tuple-unpacking
         try:
-            __COMPRESSORS__[name] = importlib.import_module(module_name)
+            mod = importlib.import_module(module_name)
+            if name == "zstd":
+                __COMPRESSORS__[name] = Transform(mod.ZstdCompressor().compress, mod.ZstdDecompressor().decompress)
+            else:
+                __COMPRESSORS__[name] = Compressor(mod)
         except ImportError:
             pass
     return sorted(set(str(key).lower() for key in __COMPRESSORS__))
```

### Comparing `ezfs-1.0.2/pyproject.toml` & `ezfs-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,17 @@
 ]
 
 [tool.coverage.report]
 fail_under = 90
 
 [tool.coverage.run]
 branch = true
+omit = [
+    "conftest.py"
+]
 
 [tool.pylint]
 # Pylint requires a full list of disables, or a full list of includes, and cannot be partially overridden.
 # The following list starts with the pylint defaults, followed by project specifics.
 # Do not modify the pylint defaults without adding a comment as to why, and only comment out instead of remove.
 disable = [
     "raw-checker-failed",
```

