# Comparing `tmp/beancount_exporter-2.0.2.tar.gz` & `tmp/beancount_exporter-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beancount_exporter-2.0.2.tar", max compression
+gzip compressed data, was "beancount_exporter-2.0.3.tar", max compression
```

## Comparing `beancount_exporter-2.0.2.tar` & `beancount_exporter-2.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    18092 2024-01-06 07:06:19.934908 beancount_exporter-2.0.2/LICENSE
--rw-r--r--   0        0        0        0 2024-01-06 07:06:19.934908 beancount_exporter-2.0.2/beancount_exporter/__init__.py
--rw-r--r--   0        0        0        0 2024-01-06 07:06:19.934908 beancount_exporter-2.0.2/beancount_exporter/formats/__init__.py
--rw-r--r--   0        0        0     4568 2024-01-06 07:06:19.934908 beancount_exporter-2.0.2/beancount_exporter/formats/json_processor.py
--rw-r--r--   0        0        0       39 2024-01-06 07:06:19.934908 beancount_exporter-2.0.2/beancount_exporter/formats/pgcopy_processor/__init__.py
--rw-r--r--   0        0        0     1665 2024-01-06 07:06:19.934908 beancount_exporter-2.0.2/beancount_exporter/formats/pgcopy_processor/configs.py
--rw-r--r--   0        0        0      797 2024-01-06 07:06:19.934908 beancount_exporter-2.0.2/beancount_exporter/formats/pgcopy_processor/data_types.py
--rw-r--r--   0        0        0     8808 2024-01-06 07:06:19.934908 beancount_exporter-2.0.2/beancount_exporter/formats/pgcopy_processor/processor.py
--rw-r--r--   0        0        0    10002 2024-01-06 07:06:19.934908 beancount_exporter-2.0.2/beancount_exporter/formats/pgcopy_processor/tables.py
--rw-r--r--   0        0        0     1776 2024-01-06 07:06:19.934908 beancount_exporter-2.0.2/beancount_exporter/formats/pgcopy_processor/utils.py
--rw-r--r--   0        0        0      771 2024-01-06 07:06:19.934908 beancount_exporter-2.0.2/beancount_exporter/formats/processor.py
--rw-r--r--   0        0        0     3513 2024-01-06 07:06:19.934908 beancount_exporter-2.0.2/beancount_exporter/main.py
--rw-r--r--   0        0        0     1014 2024-01-06 07:06:19.934908 beancount_exporter-2.0.2/beancount_exporter/utils.py
--rw-r--r--   0        0        0      641 2024-01-06 07:06:19.938909 beancount_exporter-2.0.2/pyproject.toml
--rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 beancount_exporter-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0    18092 2024-01-06 10:00:03.229157 beancount_exporter-2.0.3/LICENSE
+-rw-r--r--   0        0        0        0 2024-01-06 10:00:03.229157 beancount_exporter-2.0.3/beancount_exporter/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-06 10:00:03.229157 beancount_exporter-2.0.3/beancount_exporter/formats/__init__.py
+-rw-r--r--   0        0        0     4568 2024-01-06 10:00:03.229157 beancount_exporter-2.0.3/beancount_exporter/formats/json_processor.py
+-rw-r--r--   0        0        0       39 2024-01-06 10:00:03.229157 beancount_exporter-2.0.3/beancount_exporter/formats/pgcopy_processor/__init__.py
+-rw-r--r--   0        0        0     1665 2024-01-06 10:00:03.229157 beancount_exporter-2.0.3/beancount_exporter/formats/pgcopy_processor/configs.py
+-rw-r--r--   0        0        0      797 2024-01-06 10:00:03.229157 beancount_exporter-2.0.3/beancount_exporter/formats/pgcopy_processor/data_types.py
+-rw-r--r--   0        0        0    10254 2024-01-06 10:00:03.229157 beancount_exporter-2.0.3/beancount_exporter/formats/pgcopy_processor/processor.py
+-rw-r--r--   0        0        0    10002 2024-01-06 10:00:03.229157 beancount_exporter-2.0.3/beancount_exporter/formats/pgcopy_processor/tables.py
+-rw-r--r--   0        0        0     2070 2024-01-06 10:00:03.229157 beancount_exporter-2.0.3/beancount_exporter/formats/pgcopy_processor/utils.py
+-rw-r--r--   0        0        0      771 2024-01-06 10:00:03.229157 beancount_exporter-2.0.3/beancount_exporter/formats/processor.py
+-rw-r--r--   0        0        0     3787 2024-01-06 10:00:03.229157 beancount_exporter-2.0.3/beancount_exporter/main.py
+-rw-r--r--   0        0        0     1014 2024-01-06 10:00:03.229157 beancount_exporter-2.0.3/beancount_exporter/utils.py
+-rw-r--r--   0        0        0      641 2024-01-06 10:00:03.233157 beancount_exporter-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 beancount_exporter-2.0.3/PKG-INFO
```

### Comparing `beancount_exporter-2.0.2/LICENSE` & `beancount_exporter-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `beancount_exporter-2.0.2/beancount_exporter/formats/json_processor.py` & `beancount_exporter-2.0.3/beancount_exporter/formats/json_processor.py`

 * *Files identical despite different names*

### Comparing `beancount_exporter-2.0.2/beancount_exporter/formats/pgcopy_processor/configs.py` & `beancount_exporter-2.0.3/beancount_exporter/formats/pgcopy_processor/configs.py`

 * *Files identical despite different names*

### Comparing `beancount_exporter-2.0.2/beancount_exporter/formats/pgcopy_processor/data_types.py` & `beancount_exporter-2.0.3/beancount_exporter/formats/pgcopy_processor/data_types.py`

 * *Files identical despite different names*

### Comparing `beancount_exporter-2.0.2/beancount_exporter/formats/pgcopy_processor/processor.py` & `beancount_exporter-2.0.3/beancount_exporter/formats/pgcopy_processor/processor.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,40 +5,48 @@
 import uuid
 
 import orjson
 import pgcopy
 from beancount.core import data
 from beancount.loader import LoadError
 from beancount_data.data_types import EntryType
+from beancount_data.data_types import Transaction
+from beancount_data.data_types import ValidationError
+from beancount_data.data_types import ValidationResult
 
 from ..processor import Processor
 from .configs import ENTRY_TYPE_CONFIGS
 from .configs import EntryTypeConfig
 from .data_types import Table
 from .tables import ENTRY_BASE_TABLE
 from .tables import POSTING_TABLE
 from .utils import compile_formatter
 from .utils import convert_custom_value
 from .utils import orjson_default
+from .utils import orjson_option_maps_default
 from .utils import serialize_row
 
 
 class PgCopyProcessor(Processor):
     def __init__(
         self,
         base_path: pathlib.Path,
+        option_maps_file: io.BytesIO,
+        errors_file: io.BytesIO,
         entry_base_file: io.BytesIO,
         posting_file: io.BytesIO,
         entry_files: dict[typing.Type, io.BytesIO],
         entry_base_table: Table = ENTRY_BASE_TABLE,
         posting_table: Table = POSTING_TABLE,
         entry_configs: dict[typing.Type, EntryTypeConfig] | None = None,
         encoding: str = "utf8",
     ):
         super().__init__(base_path=base_path)
+        self.option_maps_file = option_maps_file
+        self.errors_file = errors_file
         self.entry_base_file = entry_base_file
         self.posting_file = posting_file
         self.entry_files = entry_files
         self.entry_base_table = entry_base_table
         self.posting_table = posting_table
         self.entry_configs = entry_configs or ENTRY_TYPE_CONFIGS
         self.encoding = encoding
@@ -213,18 +221,38 @@
             pgcopy_file.write(pgcopy.copy.BINCOPY_HEADER)
 
     def stop(self):
         for pgcopy_file in self.all_files:
             pgcopy_file.write(pgcopy.copy.BINCOPY_TRAILER)
 
     def process_options(self, options: dict[str, typing.Any]):
-        pass
+        self.option_maps_file.write(
+            orjson.dumps(options, default=orjson_option_maps_default)
+        )
 
     def process_errors(self, errors: list[LoadError]):
-        pass
+        validation_result = ValidationResult(
+            errors=list(map(ValidationError.from_orm, errors))
+        )
+        for error in validation_result.errors:
+            filename = error.source.get("filename")
+            if filename is not None:
+                error.source["filename"] = self.strip_path(filename)
+            if error.entry is not None:
+                if "filename" in error.entry.meta:
+                    error.entry.meta["filename"] = self.strip_path(
+                        error.entry.meta["filename"]
+                    )
+                if isinstance(error.entry, Transaction):
+                    for posting in error.entry.postings:
+                        posting_filename = posting.meta.get("filename")
+                        if posting_filename is None:
+                            continue
+                        posting.meta["filename"] = self.strip_path(posting_filename)
+        self.errors_file.write(validation_result.json().encode("utf8"))
 
     def process_entries(self, entries: data.Entries):
         extractors = {
             data.Open: self._extract_open,
             data.Close: self._extract_close,
             data.Commodity: self._extract_commodity,
             data.Pad: self._extract_pad,
```

### Comparing `beancount_exporter-2.0.2/beancount_exporter/formats/pgcopy_processor/tables.py` & `beancount_exporter-2.0.3/beancount_exporter/formats/pgcopy_processor/tables.py`

 * *Files identical despite different names*

### Comparing `beancount_exporter-2.0.2/beancount_exporter/formats/pgcopy_processor/utils.py` & `beancount_exporter-2.0.3/beancount_exporter/formats/pgcopy_processor/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import datetime
 import decimal
+import enum
 import functools
 import json
 import struct
 import typing
 
 import pgcopy.copy
 from beancount.core import account
@@ -34,14 +35,24 @@
 
 def orjson_default(value: typing.Any) -> typing.Any:
     if isinstance(value, decimal.Decimal):
         return str(value)
     raise TypeError
 
 
+def orjson_option_maps_default(value: typing.Any) -> typing.Any:
+    if isinstance(value, set):
+        return list(value)
+    elif isinstance(value, decimal.Decimal):
+        return str(value)
+    elif isinstance(value, enum.Enum):
+        return value.value
+    raise TypeError
+
+
 def compile_formatter(encoding: str, column: Column):
     funcs = [
         pgcopy.copy.encode,
         pgcopy.copy.maxsize,
         pgcopy.copy.array,
         pgcopy.copy.diagnostic,
         pgcopy.copy.null,
```

### Comparing `beancount_exporter-2.0.2/beancount_exporter/formats/processor.py` & `beancount_exporter-2.0.3/beancount_exporter/formats/processor.py`

 * *Files identical despite different names*

### Comparing `beancount_exporter-2.0.2/beancount_exporter/main.py` & `beancount_exporter-2.0.3/beancount_exporter/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,14 +75,20 @@
     with contextlib.ExitStack() as stack:
         if format == ExportFormat.JSON:
             processor = JsonProcessor(base_path=pathlib.Path(str(base_path)))
         elif format == ExportFormat.PGCOPY:
             output_dir_path = pathlib.Path(str(output_dir))
             processor = PgCopyProcessor(
                 base_path=pathlib.Path(str(base_path)),
+                option_maps_file=stack.enter_context(
+                    open(output_dir_path / "option_maps.json", "wb")
+                ),
+                errors_file=stack.enter_context(
+                    open(output_dir_path / "errors.json", "wb")
+                ),
                 entry_base_file=stack.enter_context(
                     open(output_dir_path / "entry_base.bin", "wb")
                 ),
                 posting_file=stack.enter_context(
                     open(output_dir_path / "posting.bin", "wb")
                 ),
                 entry_files={
```

### Comparing `beancount_exporter-2.0.2/beancount_exporter/utils.py` & `beancount_exporter-2.0.3/beancount_exporter/utils.py`

 * *Files identical despite different names*

### Comparing `beancount_exporter-2.0.2/pyproject.toml` & `beancount_exporter-2.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beancount-exporter"
-version = "2.0.2"
+version = "2.0.3"
 description = "Command line tool for exporting Beancount data as JSON"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "GNU GPLv2"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 beancount = "^2.3.5"
```

### Comparing `beancount_exporter-2.0.2/PKG-INFO` & `beancount_exporter-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beancount-exporter
-Version: 2.0.2
+Version: 2.0.3
 Summary: Command line tool for exporting Beancount data as JSON
 License: GNU GPLv2
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

