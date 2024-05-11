# Comparing `tmp/rtorrent_rpc-0.6.1.tar.gz` & `tmp/rtorrent_rpc-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtorrent_rpc-0.6.1.tar", max compression
+gzip compressed data, was "rtorrent_rpc-0.6.2.tar", max compression
```

## Comparing `rtorrent_rpc-0.6.1.tar` & `rtorrent_rpc-0.6.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1084 2024-04-27 16:18:58.033188 rtorrent_rpc-0.6.1/LICENSE
--rw-r--r--   0        0        0     2456 2024-04-27 16:18:58.033188 rtorrent_rpc-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     1436 2024-04-27 16:18:58.033188 rtorrent_rpc-0.6.1/readme.md
--rw-r--r--   0        0        0    29525 2024-04-27 16:18:58.033188 rtorrent_rpc-0.6.1/rtorrent_rpc/__init__.py
--rw-r--r--   0        0        0     2458 2024-04-27 16:18:58.033188 rtorrent_rpc-0.6.1/rtorrent_rpc/_jsonrpc/__init__.py
--rw-r--r--   0        0        0     3050 2024-04-27 16:18:58.033188 rtorrent_rpc-0.6.1/rtorrent_rpc/_jsonrpc/transport.py
--rw-r--r--   0        0        0     1235 2024-04-27 16:18:58.033188 rtorrent_rpc-0.6.1/rtorrent_rpc/_scgi.py
--rw-r--r--   0        0        0      803 2024-04-27 16:18:58.033188 rtorrent_rpc-0.6.1/rtorrent_rpc/_transport.py
--rw-r--r--   0        0        0     3920 2024-04-27 16:18:58.033188 rtorrent_rpc-0.6.1/rtorrent_rpc/helper.py
--rw-r--r--   0        0        0        0 2024-04-27 16:18:58.037188 rtorrent_rpc-0.6.1/rtorrent_rpc/py.typed
--rw-r--r--   0        0        0     2403 1970-01-01 00:00:00.000000 rtorrent_rpc-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-05-11 00:46:47.770881 rtorrent_rpc-0.6.2/LICENSE
+-rw-r--r--   0        0        0     2515 2024-05-11 00:46:47.770881 rtorrent_rpc-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     1669 2024-05-11 00:46:47.770881 rtorrent_rpc-0.6.2/readme.md
+-rw-r--r--   0        0        0    29769 2024-05-11 00:46:47.774881 rtorrent_rpc-0.6.2/rtorrent_rpc/__init__.py
+-rw-r--r--   0        0        0     2458 2024-05-11 00:46:47.774881 rtorrent_rpc-0.6.2/rtorrent_rpc/_jsonrpc/__init__.py
+-rw-r--r--   0        0        0     3050 2024-05-11 00:46:47.774881 rtorrent_rpc-0.6.2/rtorrent_rpc/_jsonrpc/transport.py
+-rw-r--r--   0        0        0     1235 2024-05-11 00:46:47.774881 rtorrent_rpc-0.6.2/rtorrent_rpc/_scgi.py
+-rw-r--r--   0        0        0      803 2024-05-11 00:46:47.774881 rtorrent_rpc-0.6.2/rtorrent_rpc/_transport.py
+-rw-r--r--   0        0        0     3920 2024-05-11 00:46:47.774881 rtorrent_rpc-0.6.2/rtorrent_rpc/helper.py
+-rw-r--r--   0        0        0        0 2024-05-11 00:46:47.774881 rtorrent_rpc-0.6.2/rtorrent_rpc/py.typed
+-rw-r--r--   0        0        0     2636 1970-01-01 00:00:00.000000 rtorrent_rpc-0.6.2/PKG-INFO
```

### Comparing `rtorrent_rpc-0.6.1/LICENSE` & `rtorrent_rpc-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.6.1/pyproject.toml` & `rtorrent_rpc-0.6.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "rtorrent-rpc"
-version = "0.6.1"
+version = "0.6.2"
 description = "Typed rtorrent rpc client"
 authors = ["Trim21 <i@trim21.me>"]
 readme = 'readme.md'
 repository = 'https://github.com/trim21/rtorrent-rpc'
 license = 'MIT'
 packages = [{ include = 'rtorrent_rpc' }]
 keywords = ['rtorrent', 'rpc']
@@ -22,30 +22,33 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 # dependencies
 typing-extensions = ">=4.7.1"
 bencode2 = ">=0.0.6,<1"
 urllib3 = "^2.2.1"
 
+[tool.poetry.group.orjson.dependencies]
+orjson = ">3.9.0"
+
 [tool.poetry.group.docs.dependencies]
 sphinx = { version = "^7.0.0", python = "^3.9" }
 furo = { version = "^2024.0.0", python = "^3.9" }
 
 [tool.poetry.group.dev.dependencies]
 # tests
-pytest = "==8.1.1"
+pytest = "==8.2.0"
 pytest-github-actions-annotate-failures = "==0.2.0"
 coverage = "==7.5.0"
 
 # linter and formatter
 pre-commit = { version = "==3.7.0", markers = "implementation_name != 'pypy'", python = "^3.9" }
 #mypy = { version = "==1.4.1", markers = "implementation_name != 'pypy'", python = "^3.9" }
 sphinx-autobuild = { version = "2024.4.16", python = "^3.9" }
 mypy = { version = "1.10.0", python = "^3.9" }
-orjson = "3.10.1"
+orjson = "3.10.2"
 
 [tool.poetry-plugin-bump]
 commit_msg = 'bump: v{version}'
 
 [tool.pytest.ini_options]
 addopts = '-rav -Werror'
```

### Comparing `rtorrent_rpc-0.6.1/readme.md` & `rtorrent_rpc-0.6.2/readme.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 # Typed rtorrent rpc client
 
 [![PyPI](https://img.shields.io/pypi/v/rtorrent-rpc)](https://pypi.org/project/rtorrent-rpc/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rtorrent-rpc)](https://pypi.org/project/rtorrent-rpc/)
+[![Documentation Status](https://readthedocs.org/projects/rtorrent-rpc/badge/)](https://rtorrent-rpc.readthedocs.io/)
 
 `rtorrent-rpc` is a python wrapper on top of rtorrent XML RPC protocol,
 hosted on GitHub at [github.com/trim21/rtorrent-rpc](https://github.com/trim21/rtorrent-rpc)
 
 Document is hosted at https://rtorrent-rpc.readthedocs.io/ by readthedocs.
 
 ## Introduction
 
 ```console
-pip install rtorrent-rpc -U
+pip install rtorrent-rpc
+```
+
+if you prefer [orjson](https://github.com/ijl/orjson) as jsonlib:
+
+```console
+pip install 'rtorrent-rpc[orjson]'
 ```
 
 ## Contributing
 
 All kinds of PRs (docs, feature, bug fixes and eta...) are most welcome.
 
 ## Quick Start
```

### Comparing `rtorrent_rpc-0.6.1/rtorrent_rpc/__init__.py` & `rtorrent_rpc-0.6.2/rtorrent_rpc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,14 +163,19 @@
         content: bytes,
         directory_base: str,
         tags: list[str] | None = None,
     ) -> None:
         """
         Add a torrent to the client by providing the torrent file content as bytes.
 
+        Note:
+            rTorrent need some time to handle your torrent,
+            there is a chance info_hash of the torrent you just added is not inoperable.
+            In that case, you need wait some time after you just add a torrent.
+
         Args:
             content: The content of the torrent file as bytes.
             directory_base: The base directory where the downloaded files will be saved.
             tags: A list of tags associated with the torrent. Defaults to None.
                 This argument is compatible with ruTorrent and flood.
         """
         params: list[str | bytes] = [
```

### Comparing `rtorrent_rpc-0.6.1/rtorrent_rpc/_jsonrpc/__init__.py` & `rtorrent_rpc-0.6.2/rtorrent_rpc/_jsonrpc/__init__.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.6.1/rtorrent_rpc/_jsonrpc/transport.py` & `rtorrent_rpc-0.6.2/rtorrent_rpc/_jsonrpc/transport.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.6.1/rtorrent_rpc/_scgi.py` & `rtorrent_rpc-0.6.2/rtorrent_rpc/_scgi.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.6.1/rtorrent_rpc/_transport.py` & `rtorrent_rpc-0.6.2/rtorrent_rpc/_transport.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.6.1/rtorrent_rpc/helper.py` & `rtorrent_rpc-0.6.2/rtorrent_rpc/helper.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.6.1/PKG-INFO` & `rtorrent_rpc-0.6.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtorrent-rpc
-Version: 0.6.1
+Version: 0.6.2
 Summary: Typed rtorrent rpc client
 Home-page: https://github.com/trim21/rtorrent-rpc
 License: MIT
 Keywords: rtorrent,rpc
 Author: Trim21
 Author-email: i@trim21.me
 Requires-Python: >=3.8,<4.0
@@ -24,24 +24,31 @@
 Project-URL: Repository, https://github.com/trim21/rtorrent-rpc
 Description-Content-Type: text/markdown
 
 # Typed rtorrent rpc client
 
 [![PyPI](https://img.shields.io/pypi/v/rtorrent-rpc)](https://pypi.org/project/rtorrent-rpc/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rtorrent-rpc)](https://pypi.org/project/rtorrent-rpc/)
+[![Documentation Status](https://readthedocs.org/projects/rtorrent-rpc/badge/)](https://rtorrent-rpc.readthedocs.io/)
 
 `rtorrent-rpc` is a python wrapper on top of rtorrent XML RPC protocol,
 hosted on GitHub at [github.com/trim21/rtorrent-rpc](https://github.com/trim21/rtorrent-rpc)
 
 Document is hosted at https://rtorrent-rpc.readthedocs.io/ by readthedocs.
 
 ## Introduction
 
 ```console
-pip install rtorrent-rpc -U
+pip install rtorrent-rpc
+```
+
+if you prefer [orjson](https://github.com/ijl/orjson) as jsonlib:
+
+```console
+pip install 'rtorrent-rpc[orjson]'
 ```
 
 ## Contributing
 
 All kinds of PRs (docs, feature, bug fixes and eta...) are most welcome.
 
 ## Quick Start
```

