# Comparing `tmp/romt-0.6.0.tar.gz` & `tmp/romt-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "romt-0.6.0.tar", max compression
+gzip compressed data, was "romt-0.6.1.tar", max compression
```

## Comparing `romt-0.6.0.tar` & `romt-0.6.1.tar`

### file list

```diff
@@ -1,27 +1,25 @@
--rw-r--r--   0        0        0    11692 2024-04-20 17:40:16.132832 romt-0.6.0/CHANGES.rst
--rw-r--r--   0        0        0     1122 2022-03-27 00:55:58.237668 romt-0.6.0/LICENSE.rst
--rw-r--r--   0        0        0    69410 2024-04-20 17:41:12.944064 romt-0.6.0/README.rst
--rw-r--r--   0        0        0     2149 2024-02-29 08:50:17.419836 romt-0.6.0/maintainer.rst
--rwxr-xr-x   0        0        0      315 2024-02-29 08:50:17.419836 romt-0.6.0/make-exec-darwin.sh
--rwxr-xr-x   0        0        0      249 2024-04-20 13:18:31.896068 romt-0.6.0/make-exec-linux.sh
--rw-r--r--   0        0        0      246 2024-02-29 08:50:17.419836 romt-0.6.0/make-exec-windows.bat
--rw-r--r--   0        0        0    90538 2024-04-20 13:18:31.896068 romt-0.6.0/poetry.lock
--rw-r--r--   0        0        0     3815 2024-04-20 13:18:31.896068 romt-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     9162 2024-04-20 19:25:11.631664 romt-0.6.0/requirements.txt
--rwxr-xr-x   0        0        0       57 2022-03-27 00:55:58.237668 romt-0.6.0/romt-wrapper.py
--rw-r--r--   0        0        0        0 2022-03-27 00:55:58.241668 romt-0.6.0/src/romt/__init__.py
--rw-r--r--   0        0        0     1614 2024-02-29 08:50:17.423836 romt-0.6.0/src/romt/base.py
--rw-r--r--   0        0        0     5614 2024-02-29 08:50:17.423836 romt-0.6.0/src/romt/cli.py
--rw-r--r--   0        0        0     5503 2024-02-29 08:50:17.423836 romt-0.6.0/src/romt/common.py
--rw-r--r--   0        0        0    36373 2024-02-29 08:50:17.423836 romt-0.6.0/src/romt/crate.py
--rw-r--r--   0        0        0     2616 2024-02-29 08:50:17.423836 romt-0.6.0/src/romt/dist.py
--rw-r--r--   0        0        0     8216 2024-02-29 08:50:17.423836 romt-0.6.0/src/romt/download.py
--rw-r--r--   0        0        0     2314 2024-02-29 08:50:17.423836 romt-0.6.0/src/romt/error.py
--rw-r--r--   0        0        0     2049 2024-02-29 08:50:17.423836 romt-0.6.0/src/romt/integrity.py
--rw-r--r--   0        0        0     6900 2024-02-29 08:50:17.423836 romt-0.6.0/src/romt/manifest.py
--rw-r--r--   0        0        0       93 2024-02-29 08:50:17.423836 romt-0.6.0/src/romt/py.typed
--rw-r--r--   0        0        0    17677 2024-02-29 08:50:17.427836 romt-0.6.0/src/romt/rustup.py
--rw-r--r--   0        0        0     7383 2024-04-20 16:03:02.608214 romt-0.6.0/src/romt/serve.py
--rw-r--r--   0        0        0     7457 2024-02-29 08:50:17.427836 romt-0.6.0/src/romt/signature.py
--rw-r--r--   0        0        0    26142 2024-03-02 18:46:58.786858 romt-0.6.0/src/romt/toolchain.py
--rw-r--r--   0        0        0    70588 1970-01-01 00:00:00.000000 romt-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    12647 2024-05-11 10:03:42.815987 romt-0.6.1/CHANGES.rst
+-rw-r--r--   0        0        0     1122 2022-03-27 00:55:58.237668 romt-0.6.1/LICENSE.rst
+-rw-r--r--   0        0        0    70178 2024-05-11 10:03:42.815987 romt-0.6.1/README.rst
+-rw-r--r--   0        0        0     2304 2024-05-05 00:01:39.458011 romt-0.6.1/maintainer.rst
+-rw-r--r--   0        0        0     6834 2024-05-11 10:03:42.815987 romt-0.6.1/noxfile.py
+-rw-r--r--   0        0        0    90538 2024-04-20 13:18:31.896068 romt-0.6.1/poetry.lock
+-rw-r--r--   0        0        0     3701 2024-05-05 00:03:36.899110 romt-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     9162 2024-05-11 08:27:35.759328 romt-0.6.1/requirements.txt
+-rwxr-xr-x   0        0        0       57 2022-03-27 00:55:58.237668 romt-0.6.1/romt-wrapper.py
+-rw-r--r--   0        0        0        0 2022-03-27 00:55:58.241668 romt-0.6.1/src/romt/__init__.py
+-rw-r--r--   0        0        0     1614 2024-02-29 08:50:17.423836 romt-0.6.1/src/romt/base.py
+-rw-r--r--   0        0        0     5614 2024-02-29 08:50:17.423836 romt-0.6.1/src/romt/cli.py
+-rw-r--r--   0        0        0     5551 2024-05-01 21:47:00.540509 romt-0.6.1/src/romt/common.py
+-rw-r--r--   0        0        0    36541 2024-05-01 21:49:16.543980 romt-0.6.1/src/romt/crate.py
+-rw-r--r--   0        0        0     2617 2024-05-11 10:03:42.815987 romt-0.6.1/src/romt/dist.py
+-rw-r--r--   0        0        0     8216 2024-02-29 08:50:17.423836 romt-0.6.1/src/romt/download.py
+-rw-r--r--   0        0        0     2314 2024-02-29 08:50:17.423836 romt-0.6.1/src/romt/error.py
+-rw-r--r--   0        0        0     2049 2024-02-29 08:50:17.423836 romt-0.6.1/src/romt/integrity.py
+-rw-r--r--   0        0        0     7077 2024-05-01 22:11:51.212251 romt-0.6.1/src/romt/manifest.py
+-rw-r--r--   0        0        0       93 2024-02-29 08:50:17.423836 romt-0.6.1/src/romt/py.typed
+-rw-r--r--   0        0        0    17678 2024-05-11 10:03:42.819987 romt-0.6.1/src/romt/rustup.py
+-rw-r--r--   0        0        0     7383 2024-04-20 16:03:02.608214 romt-0.6.1/src/romt/serve.py
+-rw-r--r--   0        0        0     7457 2024-02-29 08:50:17.427836 romt-0.6.1/src/romt/signature.py
+-rw-r--r--   0        0        0    26143 2024-05-11 10:03:42.819987 romt-0.6.1/src/romt/toolchain.py
+-rw-r--r--   0        0        0    71356 1970-01-01 00:00:00.000000 romt-0.6.1/PKG-INFO
```

### Comparing `romt-0.6.0/CHANGES.rst` & `romt-0.6.1/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,37 @@
 *******
 History
 *******
 
+Version 0.6.1
+=============
+
+- Speed up tests.
+
+- Fix accidental reliance on backported security fixes in Python's ``tarfile``
+  module.  The "data_filter" feature was added in Python 3.12, but got
+  backported to some previous versions, making it look like it was supported
+  since Python 3.8 (our oldest supported version). Now we probe for the feature
+  directly to ensure it's available before we use it.
+
+- Move build and release steps into ``noxfile.py``.
+
+- Add GitHub workflow for testing and quality checks.
+
+- Add Docker-based build for Linux, based on Ubuntu 18.04.  This provides
+  executables that will run on older versions of Linux.
+
+- Add GitHub workflow for building Romt executables.
+
+- Change Romt's ``darwin`` alias to denote ``aarch64-apple-darwin`` now that
+  ``x86_64`` is no longer the primary macOS architecture.
+
+- Note changed URL for ``httpx`` library; add some details on proxy-related
+  environment variables for ``httpx``.
+
 Version 0.6.0
 =============
 
 - Include ``poetry.lock`` and ``requirements.txt`` in the generated
   ``romt-x.y.z.tar.gz`` source archive.  This allows explicit use of locked
   versions for all dependencies when installing from PyPI.
```

### Comparing `romt-0.6.0/LICENSE.rst` & `romt-0.6.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `romt-0.6.0/README.rst` & `romt-0.6.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -167,39 +167,23 @@
     cd romt
 
 - Run a Poetry shell (which creates and activates a virtual environment
   installed with Romt and all dependencies)::
 
     poetry shell
 
-- Optionally build an executable for your platform:
+- Optionally build an executable for your platform::
 
-  - Linux:
-
-  .. code-block:: sh
-
-    ./make-exec-linux.sh
-
-  - Windows:
-
-  .. code-block:: sh
-
-    make-exec-windows.bat
-
-  - Mac:
-
-  .. code-block:: sh
-
-    ./make-exec-darwin.sh
+    nox -s build
 
-  Find executables at::
+  Find executables in ``dist/`` tree based on your platform, e.g.::
 
-    dist/linux/romt
-    dist/windows/romt.exe
-    dist/darwin/romt
+    dist/x86_64-linux/romt
+    dist/x86_64-windows/romt.exe
+    dist/aarch64-darwin/romt
 
 Romt usage overview
 ===================
 
 Romt is a Python-based command-line tool with several commands:
 
 - ``romt toolchain``: mirror and manage Rust toolchains.
@@ -422,15 +406,15 @@
   - Linux:
     http://localhost:8000/rustup/dist/x86_64-unknown-linux-gnu/rustup-init
 
   - Windows:
     http://localhost:8000/rustup/dist/x86_64-pc-windows-msvc/rustup-init.exe
 
   - Mac:
-    http://localhost:8000/rustup/dist/x86_64-apple-darwin/rustup-init
+    http://localhost:8000/rustup/dist/aarch64-apple-darwin/rustup-init
 
 - Run the installer, accepting the defaults:
 
   .. code-block:: sh
 
     # Linux/Mac:
     chmod +x rustup-init
@@ -576,15 +560,15 @@
 The TARGET specifies the platform for executables using standard tuple values
 (e.g., ``x86_64-unknown-linux-gnu``).  Any tuples supported by Rust are valid.
 Typical values are shown below; in parentheses are aliases Romt provides for
 ease of typing these common targets:
 
 - ``x86_64-unknown-linux-gnu`` (alias ``linux``)
 - ``x86_64-pc-windows-msvc`` (alias ``windows``)
-- ``x86_64-apple-darwin`` (alias ``darwin``)
+- ``aarch64-apple-darwin`` (alias ``darwin``)
 
 TARGET values are given by the option ``--target TARGET``.  Multiple TARGET
 options may be given, and each TARGET will be split at commas and whitespace to
 produce a list of desired TARGET values, e.g.::
 
   --target linux,windows --target 'darwin i686-pc-windows-msvc'
 
@@ -2064,19 +2048,49 @@
 
 Proxy server troubleshooting
 ----------------------------
 
 The author has not tested Romt with a proxy server, but user feedback indicates
 it's possible (see https://github.com/drmikehenry/romt/issues/10).  The
 ``httpx`` library's support for proxying is documented at:
-https://www.python-httpx.org/advanced/#http-proxying
+https://www.python-httpx.org/advanced/proxies/
+
+``httpx`` understands several environment variables (documented at
+https://www.python-httpx.org/environment_variables/ in the "Proxies" section)
+that may be used to influence proxy operation.  For example:
+
+- ``HTTP_PROXY``, ``HTTPS_PROXY``, ``ALL_PROXY``:
+
+  Valid values: A URL to a proxy
+
+  ``HTTP_PROXY``, ``HTTPS_PROXY``, ``ALL_PROXY`` set the proxy to be used for
+  http, https, or all requests respectively.
+
+  Example::
+
+    export HTTP_PROXY=http://my-external-proxy.com:1234
+
+    # This request will be sent through the proxy
+    python -c "import httpx; httpx.get('http://example.com')"
+
+    # This request will be sent directly, as we set `trust_env=False`
+    python -c "import httpx; httpx.get('http://example.com', trust_env=False)"
+
+- ``NO_PROXY``
+
+  Valid values: a comma-separated list of hostnames/urls
+
+  ``NO_PROXY`` disables the proxy for specific urls
+
+  Example::
+
+    export HTTP_PROXY=http://my-external-proxy.com:1234
+    export NO_PROXY=http://127.0.0.1,python-httpx.org
 
-``httpx`` understands several environment variables (documented at the page
-above) that may be used to influence proxy operation.  In addition, ``httpx``
-has information about debugging proxy-related issues at:
+In addition, ``httpx`` has information about debugging proxy-related issues at:
 https://www.python-httpx.org/contributing/#development-proxy-setup
 
 Also, ``httpx`` can produce more debugging information by setting the
 environment variable ``HTTPX_LOG_LEVEL`` to ``trace`` (as documented at
 https://www.python-httpx.org/environment_variables/).  As a sample invocation on
 Linux::
```

### Comparing `romt-0.6.0/maintainer.rst` & `romt-0.6.1/maintainer.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 ******************
 Maintainer's notes
 ******************
 
 These notes are intended for use by the maintainer.
 
+Building an executable with PyInstaller
+=======================================
+
+- Use the Nox ``build`` session::
+
+    poetry run nox -s build
+
 Making a release
 ================
 
+Perform these steps on Linux.
+
 - Verify proper ``version = "x.y.z"`` in ``pyproject.toml``.
 
 - Verify changes are recorded in ``CHANGES.rst``.
 
 - Run a Poetry shell::
 
     poetry shell
 
 - Verify all Nox tests are passing::
 
     nox
 
-- On Linux, run:
-
-  .. code-block:: sh
+- Prepare the release::
 
-    ./prepare-release.sh
+    nox -s release
 
 - Follow on-screen instructions to complete release.
 
 Upgrading dependencies
 ======================
 
 - ``poetry upgrade``.
```

### Comparing `romt-0.6.0/poetry.lock` & `romt-0.6.1/poetry.lock`

 * *Files identical despite different names*

### Comparing `romt-0.6.0/pyproject.toml` & `romt-0.6.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 [tool.poetry]
 name = "romt"
-version = "0.6.0"
+version = "0.6.1"
 include = [
   { path = "CHANGES.rst", format="sdist" },
   { path = "LICENSE.rst", format="sdist" },
   { path = "README.rst", format="sdist" },
   { path = "maintainer.rst", format="sdist" },
-  { path = "make-exec-darwin.sh", format="sdist" },
-  { path = "make-exec-linux.sh", format="sdist" },
-  { path = "make-exec-windows.bat", format="sdist" },
+  { path = "noxfile.py", format="sdist" },
   { path = "poetry.lock", format="sdist" },
   { path = "requirements.txt", format="sdist" },
   { path = "romt-wrapper.py", format="sdist" },
 ]
 description = """\
   Romt (Rust Offline Mirror Tool) enables mirroring of Rust \
   programming language tools and crates for use in an offline context.\
```

### Comparing `romt-0.6.0/requirements.txt` & `romt-0.6.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `romt-0.6.0/src/romt/base.py` & `romt-0.6.1/src/romt/base.py`

 * *Files identical despite different names*

### Comparing `romt-0.6.0/src/romt/cli.py` & `romt-0.6.1/src/romt/cli.py`

 * *Files identical despite different names*

### Comparing `romt-0.6.0/src/romt/common.py` & `romt-0.6.1/src/romt/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,10 +206,11 @@
             if tmp_archive_path.is_file():
                 tmp_archive_path.unlink()
             raise
         tar_f.close()
         tmp_archive_path.rename(archive_path)
     else:
         tar_f = tarfile.open(str(archive_path), mode)
-        tar_f.extraction_filter = tarfile.data_filter
+        if hasattr(tarfile, "data_filter"):
+            tar_f.extraction_filter = tarfile.data_filter
         yield tar_f
         tar_f.close()
```

### Comparing `romt-0.6.0/src/romt/crate.py` & `romt-0.6.1/src/romt/crate.py`

 * *Files 0% similar despite different names*

```diff
@@ -606,21 +606,24 @@
                 common.vprint(f"Detected archive_format {archive_format} ")
 
             elif tar_info.name == INDEX_BUNDLE_PACKED_NAME:
                 found_file = True
                 found_bundle = True
                 tar_info.name = str(bundle_path)
                 common.vprint(f"[unpack] {tar_info.name}")
-                # Use the "fully_trusted" filter for this member because we're
-                # overriding the destination path to the correct value.
-                # (Otherwise, `.extract()` will not allow absolute paths for
-                # `tarinfo.name`).
-                tar_f.extract(
-                    tar_info, set_attrs=False, filter="fully_trusted"
-                )
+                if hasattr(tar_f, "extraction_filter"):
+                    # Use the "fully_trusted" filter for this member because
+                    # we're overriding the destination path to the correct
+                    # value.  (Otherwise, `.extract()` will not allow absolute
+                    # paths for `tarinfo.name`).
+                    tar_f.extract(
+                        tar_info, set_attrs=False, filter="fully_trusted"
+                    )
+                else:
+                    tar_f.extract(tar_info, set_attrs=False)
 
             elif tar_info.name.startswith(crates_prefix):
                 found_file = True
                 name, version = crate_name_version_from_rel_path(tar_info.name)
                 if not name or not version:
                     common.abort(f"Invalid crate {tar_info.name}")
                 expected_rel_path = crate_rel_path_from_name_version(
```

### Comparing `romt-0.6.0/src/romt/dist.py` & `romt-0.6.1/src/romt/dist.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def expand_target_alias(target: str) -> str:
     if target == "linux":
         target = "x86_64-unknown-linux-gnu"
     elif target == "windows":
         target = "x86_64-pc-windows-msvc"
     elif target == "darwin":
-        target = "x86_64-apple-darwin"
+        target = "aarch64-apple-darwin"
     return target
 
 
 def target_exe_suffix(target: str) -> str:
     parts = target.split("-")
     if "windows" in parts:
         suffix = ".exe"
```

### Comparing `romt-0.6.0/src/romt/download.py` & `romt-0.6.1/src/romt/download.py`

 * *Files identical despite different names*

### Comparing `romt-0.6.0/src/romt/error.py` & `romt-0.6.1/src/romt/error.py`

 * *Files identical despite different names*

### Comparing `romt-0.6.0/src/romt/integrity.py` & `romt-0.6.1/src/romt/integrity.py`

 * *Files identical despite different names*

### Comparing `romt-0.6.0/src/romt/manifest.py` & `romt-0.6.1/src/romt/manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import collections
 import copy
+import functools
 from pathlib import Path
 from typing import (
     Any,
     Callable,
     Dict,
     Generator,
     Iterable,
@@ -59,21 +60,28 @@
                 f"Package {self.name}/{self.target} missing xz_url"
             )
         url = self.xz_url
         prefix = "/dist/"
         return url[url.index(prefix) + len(prefix) :]
 
 
+@functools.lru_cache
+def toml_loads(contents: str) -> Any:
+    return toml.loads(contents)
+
+
 class Manifest:
     def __init__(self, raw_dict: MutableMapping[str, Any]):
         self._dict = raw_dict
 
     @staticmethod
     def from_toml_path(toml_path: Path) -> "Manifest":
-        return Manifest(toml.load(toml_path))
+        with open(toml_path) as f:
+            contents = f.read()
+        return Manifest(toml_loads(contents))
 
     def clone(self) -> "Manifest":
         return Manifest(copy.deepcopy(self._dict))
 
     @property
     def _rust_src_version(self) -> str:
         version = str(self._dict["pkg"]["rust-src"]["version"])
```

### Comparing `romt-0.6.0/src/romt/rustup.py` & `romt-0.6.1/src/romt/rustup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 - <version> is: X.Y.Z
 - Multiple SPEC options may be given.
 - Each SPEC option will be split at commas and whitespace.
 
 TARGET is standard 3- or 4-tuple; common examples:
 - x86_64-unknown-linux-gnu (alias ``linux``)
 - x86_64-pc-windows-msvc (alias ``windows``)
-- x86_64-apple-darwin (alias ``darwin``)
+- aarch64-apple-darwin (alias ``darwin``)
 
 COMMAND values:
 
   download          download artifacts matching SPEC and TARGET to DEST
   verify            verify DEST artifacts matching SPEC and TARGET
   list              print DEST artifacts and targets matching SPEC
   all-targets       print all known targets (hard-coded; others are permitted)
```

### Comparing `romt-0.6.0/src/romt/serve.py` & `romt-0.6.1/src/romt/serve.py`

 * *Files identical despite different names*

### Comparing `romt-0.6.0/src/romt/signature.py` & `romt-0.6.1/src/romt/signature.py`

 * *Files identical despite different names*

### Comparing `romt-0.6.0/src/romt/toolchain.py` & `romt-0.6.1/src/romt/toolchain.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 - Single ``*`` represents date, not channel; equivalent to ``*-*``.
 - Multiple SPEC options may be given.
 - Each SPEC option will be split at commas and whitespace.
 
 TARGET is standard 3- or 4-tuple; common examples:
 - x86_64-unknown-linux-gnu (alias ``linux``)
 - x86_64-pc-windows-msvc (alias ``windows``)
-- x86_64-apple-darwin (alias ``darwin``)
+- aarch64-apple-darwin (alias ``darwin``)
 
 COMMAND values:
   Typical:
     download        download artifacts matching SPEC and TARGET to DEST
     pack            pack DEST artifacts matching SPEC and TARGET into ARCHIVE
     unpack          unpack ARCHIVE into DEST, setting SPEC and TARGET
   Less common:
```

### Comparing `romt-0.6.0/PKG-INFO` & `romt-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: romt
-Version: 0.6.0
+Version: 0.6.1
 Summary: Romt (Rust Offline Mirror Tool) enables mirroring of Rust programming language tools and crates for use in an offline context.
 Home-page: https://github.com/drmikehenry/romt
 License: MIT
 Keywords: Rust,mirror,toolchain,crates
 Author: Michael Henry
 Author-email: drmikehenry@drmikehenry.com
 Requires-Python: >=3.8,<3.13
@@ -196,39 +196,23 @@
     cd romt
 
 - Run a Poetry shell (which creates and activates a virtual environment
   installed with Romt and all dependencies)::
 
     poetry shell
 
-- Optionally build an executable for your platform:
+- Optionally build an executable for your platform::
 
-  - Linux:
-
-  .. code-block:: sh
-
-    ./make-exec-linux.sh
-
-  - Windows:
-
-  .. code-block:: sh
-
-    make-exec-windows.bat
-
-  - Mac:
-
-  .. code-block:: sh
-
-    ./make-exec-darwin.sh
+    nox -s build
 
-  Find executables at::
+  Find executables in ``dist/`` tree based on your platform, e.g.::
 
-    dist/linux/romt
-    dist/windows/romt.exe
-    dist/darwin/romt
+    dist/x86_64-linux/romt
+    dist/x86_64-windows/romt.exe
+    dist/aarch64-darwin/romt
 
 Romt usage overview
 ===================
 
 Romt is a Python-based command-line tool with several commands:
 
 - ``romt toolchain``: mirror and manage Rust toolchains.
@@ -451,15 +435,15 @@
   - Linux:
     http://localhost:8000/rustup/dist/x86_64-unknown-linux-gnu/rustup-init
 
   - Windows:
     http://localhost:8000/rustup/dist/x86_64-pc-windows-msvc/rustup-init.exe
 
   - Mac:
-    http://localhost:8000/rustup/dist/x86_64-apple-darwin/rustup-init
+    http://localhost:8000/rustup/dist/aarch64-apple-darwin/rustup-init
 
 - Run the installer, accepting the defaults:
 
   .. code-block:: sh
 
     # Linux/Mac:
     chmod +x rustup-init
@@ -605,15 +589,15 @@
 The TARGET specifies the platform for executables using standard tuple values
 (e.g., ``x86_64-unknown-linux-gnu``).  Any tuples supported by Rust are valid.
 Typical values are shown below; in parentheses are aliases Romt provides for
 ease of typing these common targets:
 
 - ``x86_64-unknown-linux-gnu`` (alias ``linux``)
 - ``x86_64-pc-windows-msvc`` (alias ``windows``)
-- ``x86_64-apple-darwin`` (alias ``darwin``)
+- ``aarch64-apple-darwin`` (alias ``darwin``)
 
 TARGET values are given by the option ``--target TARGET``.  Multiple TARGET
 options may be given, and each TARGET will be split at commas and whitespace to
 produce a list of desired TARGET values, e.g.::
 
   --target linux,windows --target 'darwin i686-pc-windows-msvc'
 
@@ -2093,19 +2077,49 @@
 
 Proxy server troubleshooting
 ----------------------------
 
 The author has not tested Romt with a proxy server, but user feedback indicates
 it's possible (see https://github.com/drmikehenry/romt/issues/10).  The
 ``httpx`` library's support for proxying is documented at:
-https://www.python-httpx.org/advanced/#http-proxying
+https://www.python-httpx.org/advanced/proxies/
+
+``httpx`` understands several environment variables (documented at
+https://www.python-httpx.org/environment_variables/ in the "Proxies" section)
+that may be used to influence proxy operation.  For example:
+
+- ``HTTP_PROXY``, ``HTTPS_PROXY``, ``ALL_PROXY``:
+
+  Valid values: A URL to a proxy
+
+  ``HTTP_PROXY``, ``HTTPS_PROXY``, ``ALL_PROXY`` set the proxy to be used for
+  http, https, or all requests respectively.
+
+  Example::
+
+    export HTTP_PROXY=http://my-external-proxy.com:1234
+
+    # This request will be sent through the proxy
+    python -c "import httpx; httpx.get('http://example.com')"
+
+    # This request will be sent directly, as we set `trust_env=False`
+    python -c "import httpx; httpx.get('http://example.com', trust_env=False)"
+
+- ``NO_PROXY``
+
+  Valid values: a comma-separated list of hostnames/urls
+
+  ``NO_PROXY`` disables the proxy for specific urls
+
+  Example::
+
+    export HTTP_PROXY=http://my-external-proxy.com:1234
+    export NO_PROXY=http://127.0.0.1,python-httpx.org
 
-``httpx`` understands several environment variables (documented at the page
-above) that may be used to influence proxy operation.  In addition, ``httpx``
-has information about debugging proxy-related issues at:
+In addition, ``httpx`` has information about debugging proxy-related issues at:
 https://www.python-httpx.org/contributing/#development-proxy-setup
 
 Also, ``httpx`` can produce more debugging information by setting the
 environment variable ``HTTPX_LOG_LEVEL`` to ``trace`` (as documented at
 https://www.python-httpx.org/environment_variables/).  As a sample invocation on
 Linux::
```

