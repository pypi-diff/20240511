# Comparing `tmp/mcbootflash-8.0.1.tar.gz` & `tmp/mcbootflash-8.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcbootflash-8.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mcbootflash-8.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mcbootflash-8.0.1.tar` & `mcbootflash-8.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      578 2024-02-08 10:24:45.013478 mcbootflash-8.0.1/.github/workflows/main.yml
--rw-r--r--   0        0        0     3090 2024-02-05 09:08:21.921739 mcbootflash-8.0.1/.gitignore
--rw-r--r--   0        0        0    10160 2024-02-08 11:49:24.208695 mcbootflash-8.0.1/CHANGELOG.md
--rw-r--r--   0        0        0     1058 2024-02-08 10:24:45.021478 mcbootflash-8.0.1/LICENSE
--rw-r--r--   0        0        0     3583 2024-02-07 12:53:19.748024 mcbootflash-8.0.1/README.md
--rw-r--r--   0        0        0      465 2024-02-07 12:53:19.752024 mcbootflash-8.0.1/docs/api.md
--rw-r--r--   0        0        0       44 2024-02-05 09:08:21.921739 mcbootflash-8.0.1/docs/changelog.md
--rw-r--r--   0        0        0     3473 2024-02-05 09:08:21.921739 mcbootflash-8.0.1/docs/develop.md
--rw-r--r--   0        0        0       41 2024-02-05 09:08:21.921739 mcbootflash-8.0.1/docs/index.md
--rw-r--r--   0        0        0      836 2024-02-08 10:24:45.021478 mcbootflash-8.0.1/mkdocs.yml
--rw-r--r--   0        0        0     1732 2024-02-08 11:43:20.300736 mcbootflash-8.0.1/pyproject.toml
--rw-r--r--   0        0        0      685 2024-02-08 11:52:00.513832 mcbootflash-8.0.1/src/mcbootflash/__init__.py
--rw-r--r--   0        0        0     7590 2024-02-08 10:24:45.021478 mcbootflash-8.0.1/src/mcbootflash/__main__.py
--rw-r--r--   0        0        0      989 2024-02-05 09:08:21.921739 mcbootflash-8.0.1/src/mcbootflash/error.py
--rw-r--r--   0        0        0    11714 2024-02-08 10:24:45.021478 mcbootflash-8.0.1/src/mcbootflash/flash.py
--rw-r--r--   0        0        0     8770 2024-02-07 12:53:19.776025 mcbootflash-8.0.1/src/mcbootflash/types.py
--rw-r--r--   0        0        0     1545 2024-02-08 10:24:45.021478 mcbootflash-8.0.1/src/mcbootflash/util.py
--rw-r--r--   0        0        0    24817 2024-02-08 10:24:45.021478 mcbootflash-8.0.1/tests/test_mcbootflash.json
--rw-r--r--   0        0        0     5802 2024-02-08 10:24:45.021478 mcbootflash-8.0.1/tests/test_mcbootflash.py
--rw-r--r--   0        0        0     5628 2024-02-05 09:08:21.921739 mcbootflash-8.0.1/tests/testcases/checksum_error/test.hex
--rw-r--r--   0        0        0     5628 2024-02-05 09:08:21.925739 mcbootflash-8.0.1/tests/testcases/flash/test.hex
--rw-r--r--   0        0        0     5628 2024-02-05 09:08:21.925739 mcbootflash-8.0.1/tests/testcases/flash_empty/test.hex
--rw-r--r--   0        0        0     2932 2024-02-05 09:08:21.925739 mcbootflash-8.0.1/tests/testcases/no_data/test.hex
--rw-r--r--   0        0        0     5628 2024-02-05 09:08:21.925739 mcbootflash-8.0.1/tests/testcases/no_response/test.hex
--rw-r--r--   0        0        0      565 2024-02-08 10:24:45.021478 mcbootflash-8.0.1/tox.ini
--rw-r--r--   0        0        0     5025 1970-01-01 00:00:00.000000 mcbootflash-8.0.1/PKG-INFO
+-rw-r--r--   0        0        0      578 2024-02-10 19:54:03.187436 mcbootflash-8.0.2/.github/workflows/main.yml
+-rw-r--r--   0        0        0     3090 2022-06-08 18:37:37.758584 mcbootflash-8.0.2/.gitignore
+-rw-r--r--   0        0        0    10422 2024-05-11 15:49:58.395449 mcbootflash-8.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1058 2024-02-10 19:54:03.187436 mcbootflash-8.0.2/LICENSE
+-rw-r--r--   0        0        0     3583 2023-11-10 18:57:54.826438 mcbootflash-8.0.2/README.md
+-rw-r--r--   0        0        0      465 2024-02-10 19:54:03.187436 mcbootflash-8.0.2/docs/api.md
+-rw-r--r--   0        0        0       44 2023-11-09 22:11:17.471011 mcbootflash-8.0.2/docs/changelog.md
+-rw-r--r--   0        0        0     3473 2023-11-09 22:11:17.471011 mcbootflash-8.0.2/docs/develop.md
+-rw-r--r--   0        0        0       41 2023-11-09 22:11:17.471011 mcbootflash-8.0.2/docs/index.md
+-rw-r--r--   0        0        0      836 2024-02-10 19:54:03.187436 mcbootflash-8.0.2/mkdocs.yml
+-rw-r--r--   0        0        0     1732 2024-02-10 19:54:03.191436 mcbootflash-8.0.2/pyproject.toml
+-rw-r--r--   0        0        0      685 2024-05-11 15:43:36.176115 mcbootflash-8.0.2/src/mcbootflash/__init__.py
+-rw-r--r--   0        0        0     7590 2024-05-11 15:43:36.176115 mcbootflash-8.0.2/src/mcbootflash/__main__.py
+-rw-r--r--   0        0        0      989 2023-11-09 22:11:17.471011 mcbootflash-8.0.2/src/mcbootflash/error.py
+-rw-r--r--   0        0        0    12015 2024-05-11 15:43:36.180115 mcbootflash-8.0.2/src/mcbootflash/flash.py
+-rw-r--r--   0        0        0     8775 2024-02-10 19:54:46.070837 mcbootflash-8.0.2/src/mcbootflash/types.py
+-rw-r--r--   0        0        0     1545 2024-02-10 19:54:03.191436 mcbootflash-8.0.2/src/mcbootflash/util.py
+-rw-r--r--   0        0        0   107316 2024-05-11 15:43:36.180115 mcbootflash-8.0.2/tests/test_mcbootflash.json
+-rw-r--r--   0        0        0     6248 2024-05-11 15:49:58.395449 mcbootflash-8.0.2/tests/test_mcbootflash.py
+-rw-r--r--   0        0        0     5628 2022-12-03 16:05:22.909458 mcbootflash-8.0.2/tests/testcases/checksum_error/test.hex
+-rw-r--r--   0        0        0     5628 2022-12-03 16:05:22.909458 mcbootflash-8.0.2/tests/testcases/flash/test.hex
+-rw-r--r--   0        0        0     5628 2022-12-03 16:05:22.909458 mcbootflash-8.0.2/tests/testcases/flash_empty/test.hex
+-rw-r--r--   0        0        0     2932 2022-12-03 16:05:22.909458 mcbootflash-8.0.2/tests/testcases/no_data/test.hex
+-rw-r--r--   0        0        0     5628 2022-12-03 16:05:22.909458 mcbootflash-8.0.2/tests/testcases/no_response/test.hex
+-rw-r--r--   0        0        0      565 2024-02-10 19:54:03.191436 mcbootflash-8.0.2/tox.ini
+-rw-r--r--   0        0        0     5025 1970-01-01 00:00:00.000000 mcbootflash-8.0.2/PKG-INFO
```

### Comparing `mcbootflash-8.0.1/.github/workflows/main.yml` & `mcbootflash-8.0.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `mcbootflash-8.0.1/.gitignore` & `mcbootflash-8.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mcbootflash-8.0.1/CHANGELOG.md` & `mcbootflash-8.0.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 # Changelog
 
-## [8.0.2] - Development
+## [8.0.3] - Development
+
+## [8.0.2] - 2024-05-11
+
+### Fixed
+
+- Continue with warning on `BadAddress` during checksum ([`b8734ea`](https://github.com/bessman/mcbootflash/commit/b8734ea2d4b63a3ae005031629a1b6c73c83dd49))
 
 ## [8.0.1] - 2024-02-08
 
 ### Changed
 
 - Bump development status trove classifier: Beta -> Stable ([`418142e`](https://github.com/bessman/mcbootflash/commit/418142e1df232219b472027a52020ffe074fab28))
 - Begin argument descriptions with lowercase letter ([`103a331`](https://github.com/bessman/mcbootflash/commit/103a3313aec6fb6eb4c08ee35ecadd97055b0335))
@@ -234,14 +240,15 @@
 
 - Fix off-by-one error when firmware uses all available space
 
 ## [1.0.0] - 2022-05-27
 
 _Initial release._
 
+[8.0.2]: https://github.com/bessman/mcbootflash/releases/tag/8.0.2
 [8.0.1]: https://github.com/bessman/mcbootflash/releases/tag/8.0.1
 [8.0.0]: https://github.com/bessman/mcbootflash/releases/tag/v8.0.0
 [7.0.6]: https://github.com/bessman/mcbootflash/releases/tag/v7.0.6
 [7.0.5]: https://github.com/bessman/mcbootflash/releases/tag/v7.0.5
 [7.0.4]: https://github.com/bessman/mcbootflash/releases/tag/v7.0.4
 [7.0.3]: https://github.com/bessman/mcbootflash/releases/tag/v7.0.3
 [7.0.0]: https://github.com/bessman/mcbootflash/releases/tag/v7.0.0
```

### Comparing `mcbootflash-8.0.1/LICENSE` & `mcbootflash-8.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mcbootflash-8.0.1/README.md` & `mcbootflash-8.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mcbootflash-8.0.1/docs/develop.md` & `mcbootflash-8.0.2/docs/develop.md`

 * *Files identical despite different names*

### Comparing `mcbootflash-8.0.1/mkdocs.yml` & `mcbootflash-8.0.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mcbootflash-8.0.1/pyproject.toml` & `mcbootflash-8.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mcbootflash-8.0.1/src/mcbootflash/__init__.py` & `mcbootflash-8.0.2/src/mcbootflash/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,8 +32,8 @@
     "erase_flash",
     "get_boot_attrs",
     "reset",
     "self_verify",
     "write_flash",
 ]
 
-__version__ = "8.0.1"
+__version__ = "8.0.2"
```

### Comparing `mcbootflash-8.0.1/src/mcbootflash/__main__.py` & `mcbootflash-8.0.2/src/mcbootflash/__main__.py`

 * *Files identical despite different names*

### Comparing `mcbootflash-8.0.1/src/mcbootflash/error.py` & `mcbootflash-8.0.2/src/mcbootflash/error.py`

 * *Files identical despite different names*

### Comparing `mcbootflash-8.0.1/src/mcbootflash/flash.py` & `mcbootflash-8.0.2/src/mcbootflash/flash.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,15 +267,24 @@
 
     Raises
     ------
     BootloaderError
         If checksums do not match.
     """
     checksum1 = _get_local_checksum(chunk.data)
-    checksum2 = _get_remote_checksum(connection, chunk.address, len(chunk.data))
+
+    try:
+        checksum2 = _get_remote_checksum(connection, chunk.address, len(chunk.data))
+    except BadAddress:
+        _logger.warning(
+            "Got BadAddress while checksumming, continuing anyway. "
+            "This is probably a bug in the bootloader, not in mcbootflash. "
+            "See https://github.com/bessman/mcbootflash/issues/54",
+        )
+        return
 
     if checksum1 != checksum2:
         _logger.debug(f"Checksum mismatch: {checksum1} != {checksum2}")
         _logger.debug("unlock_sequence field may be incorrect")
         msg = "Checksum mismatch"
         raise BootloaderError(msg)
```

### Comparing `mcbootflash-8.0.1/src/mcbootflash/types.py` & `mcbootflash-8.0.2/src/mcbootflash/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,15 +252,15 @@
 
     Attributes
     ----------
     address : int
         The address associated with the start of the data. Must be aligned with (i.e. be
         a multiple of) the bootloader's `write_size` attribute.
     data : bytes
-        Data to be written to the bootloader. The data length be a multiple of the
+        Data to be written to the bootloader. The data length must be a multiple of the
         bootloader's `write_size` attribute, and must be no longer than the bootloader's
         `max_packet_length` attribute minus the size of the command packet header (which
         can be gotten with `Command.get_size`).
     """
 
     address: int
     data: bytes
```

### Comparing `mcbootflash-8.0.1/src/mcbootflash/util.py` & `mcbootflash-8.0.2/src/mcbootflash/util.py`

 * *Files identical despite different names*

### Comparing `mcbootflash-8.0.1/tests/test_mcbootflash.py` & `mcbootflash-8.0.2/tests/test_mcbootflash.py`

 * *Files 4% similar despite different names*

```diff
@@ -193,7 +193,20 @@
 def test_format_debug_bytes():
     testbytes_tx = b"0123"
     testbytes_rx = b"456789"
     formatted_tx = mcbootflash.flash._format_debug_bytes(testbytes_tx)
     formatted_rx = mcbootflash.flash._format_debug_bytes(testbytes_rx, testbytes_tx)
     expected = "30 31 32 33\n            34 35 36 37 38 39"
     assert formatted_tx + "\n" + formatted_rx == expected
+
+
+def test_checksum_bad_address_warning(reserial, caplog, connection):
+    boot_attrs = bf.get_boot_attrs(connection)
+    payload_size = 240
+    chunk = bincopy.Segment(
+        minimum_address=boot_attrs.memory_range[1] - payload_size // 2,
+        maximum_address=boot_attrs.memory_range[1],
+        data=b"\xff" * payload_size,
+        word_size_bytes=1,
+    )
+    bf.checksum(connection, chunk)
+    assert "BadAddress" in caplog.messages[-1]
```

### Comparing `mcbootflash-8.0.1/tests/testcases/checksum_error/test.hex` & `mcbootflash-8.0.2/tests/testcases/checksum_error/test.hex`

 * *Files identical despite different names*

### Comparing `mcbootflash-8.0.1/tests/testcases/flash/test.hex` & `mcbootflash-8.0.2/tests/testcases/flash/test.hex`

 * *Files identical despite different names*

### Comparing `mcbootflash-8.0.1/tests/testcases/flash_empty/test.hex` & `mcbootflash-8.0.2/tests/testcases/flash_empty/test.hex`

 * *Files identical despite different names*

### Comparing `mcbootflash-8.0.1/tests/testcases/no_data/test.hex` & `mcbootflash-8.0.2/tests/testcases/no_data/test.hex`

 * *Files identical despite different names*

### Comparing `mcbootflash-8.0.1/tests/testcases/no_response/test.hex` & `mcbootflash-8.0.2/tests/testcases/no_response/test.hex`

 * *Files identical despite different names*

### Comparing `mcbootflash-8.0.1/tox.ini` & `mcbootflash-8.0.2/tox.ini`

 * *Files identical despite different names*

### Comparing `mcbootflash-8.0.1/PKG-INFO` & `mcbootflash-8.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcbootflash
-Version: 8.0.1
+Version: 8.0.2
 Summary: Flash firmware to devices running Microchip's 16-bit bootloader.
 Keywords: firmware,flashing,bootloader,serial,uart,microchip,pic24,dspic33,16-bit
 Author-email: Alexander Bessman <alexander.bessman@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

