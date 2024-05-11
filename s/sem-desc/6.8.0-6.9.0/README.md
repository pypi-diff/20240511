# Comparing `tmp/sem_desc-6.8.0.tar.gz` & `tmp/sem_desc-6.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sem_desc-6.8.0.tar", max compression
+gzip compressed data, was "sem_desc-6.9.0.tar", max compression
```

## Comparing `sem_desc-6.8.0.tar` & `sem_desc-6.9.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0      205 2024-03-02 01:12:33.940806 sem_desc-6.8.0/README.md
--rw-r--r--   0        0        0     1113 2024-03-02 01:12:33.940806 sem_desc-6.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-02 01:12:33.940806 sem_desc-6.8.0/sm/__init__.py
--rw-r--r--   0        0        0     1854 2024-03-02 01:12:33.940806 sem_desc-6.8.0/sm/data/namespaces.yml
--rw-r--r--   0        0        0    15151 2024-03-02 01:12:33.940806 sem_desc-6.8.0/sm/dataset.py
--rw-r--r--   0        0        0        0 2024-03-02 01:12:33.940806 sem_desc-6.8.0/sm/evaluation/__init__.py
--rw-r--r--   0        0        0     3418 2024-03-02 01:12:33.940806 sem_desc-6.8.0/sm/evaluation/cpa_cta_metrics.py
--rw-r--r--   0        0        0     4064 2024-03-02 01:12:33.940806 sem_desc-6.8.0/sm/evaluation/hierarchy_scoring_fn.py
--rw-r--r--   0        0        0     2684 2024-03-02 01:12:33.940806 sem_desc-6.8.0/sm/evaluation/precision_recall_f1.py
--rw-r--r--   0        0        0      585 2024-03-02 01:12:33.940806 sem_desc-6.8.0/sm/evaluation/prelude.py
--rw-r--r--   0        0        0    23741 2024-03-02 01:12:33.944806 sem_desc-6.8.0/sm/evaluation/sm_metrics.py
--rw-r--r--   0        0        0     1844 2024-03-02 01:12:33.944806 sem_desc-6.8.0/sm/evaluation/transformation.py
--rw-r--r--   0        0        0     1174 2024-03-02 01:12:33.944806 sem_desc-6.8.0/sm/evaluation/utils.py
--rw-r--r--   0        0        0        0 2024-03-02 01:12:33.944806 sem_desc-6.8.0/sm/inputs/__init__.py
--rw-r--r--   0        0        0     2113 2024-03-02 01:12:33.944806 sem_desc-6.8.0/sm/inputs/column.py
--rw-r--r--   0        0        0     2968 2024-03-02 01:12:33.944806 sem_desc-6.8.0/sm/inputs/context.py
--rw-r--r--   0        0        0     4084 2024-03-02 01:12:33.944806 sem_desc-6.8.0/sm/inputs/link.py
--rw-r--r--   0        0        0      313 2024-03-02 01:12:33.944806 sem_desc-6.8.0/sm/inputs/prelude.py
--rw-r--r--   0        0        0     4292 2024-03-02 01:12:33.944806 sem_desc-6.8.0/sm/inputs/table.py
--rw-r--r--   0        0        0        0 2024-03-02 01:12:33.944806 sem_desc-6.8.0/sm/misc/__init__.py
--rw-r--r--   0        0        0     2505 2024-03-02 01:12:33.944806 sem_desc-6.8.0/sm/misc/bijection.py
--rw-r--r--   0        0        0     8221 2024-03-02 01:12:33.944806 sem_desc-6.8.0/sm/misc/deser.py
--rw-r--r--   0        0        0     6950 2024-03-02 01:12:33.944806 sem_desc-6.8.0/sm/misc/exp_manager.py
--rw-r--r--   0        0        0     3538 2024-03-02 01:12:33.944806 sem_desc-6.8.0/sm/misc/fn_cache.py
--rw-r--r--   0        0        0    15012 2024-03-02 01:12:33.944806 sem_desc-6.8.0/sm/misc/funcs.py
--rw-r--r--   0        0        0     1832 2024-03-02 01:12:33.944806 sem_desc-6.8.0/sm/misc/logger.py
--rw-r--r--   0        0        0     3009 2024-03-02 01:12:33.944806 sem_desc-6.8.0/sm/misc/matrix.py
--rw-r--r--   0        0        0      284 2024-03-02 01:12:33.944806 sem_desc-6.8.0/sm/misc/prelude.py
--rw-r--r--   0        0        0    11345 2024-03-02 01:12:33.944806 sem_desc-6.8.0/sm/misc/ray_helper.py
--rw-r--r--   0        0        0     3773 2024-03-02 01:12:33.944806 sem_desc-6.8.0/sm/misc/timer.py
--rw-r--r--   0        0        0        0 2024-03-02 01:12:33.944806 sem_desc-6.8.0/sm/namespaces/__init__.py
--rw-r--r--   0        0        0     7303 2024-03-02 01:12:33.944806 sem_desc-6.8.0/sm/namespaces/namespace.py
--rw-r--r--   0        0        0     2966 2024-03-02 01:12:33.944806 sem_desc-6.8.0/sm/namespaces/prefix_index.py
--rw-r--r--   0        0        0      329 2024-03-02 01:12:33.944806 sem_desc-6.8.0/sm/namespaces/prelude.py
--rw-r--r--   0        0        0      772 2024-03-02 01:12:33.944806 sem_desc-6.8.0/sm/namespaces/utils.py
--rw-r--r--   0        0        0     5637 2024-03-02 01:12:33.944806 sem_desc-6.8.0/sm/namespaces/wikidata.py
--rw-r--r--   0        0        0        0 2024-03-02 01:12:33.944806 sem_desc-6.8.0/sm/outputs/__init__.py
--rw-r--r--   0        0        0    34206 2024-03-02 01:12:33.944806 sem_desc-6.8.0/sm/outputs/semantic_model.py
--rw-r--r--   0        0        0      174 2024-03-02 01:12:33.944806 sem_desc-6.8.0/sm/prelude.py
--rw-r--r--   0        0        0        0 2024-03-02 01:12:33.944806 sem_desc-6.8.0/sm/py.typed
--rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 sem_desc-6.8.0/PKG-INFO
+-rw-r--r--   0        0        0      205 2024-03-04 02:49:26.180264 sem_desc-6.9.0/README.md
+-rw-r--r--   0        0        0     1113 2024-03-04 02:49:26.180264 sem_desc-6.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/__init__.py
+-rw-r--r--   0        0        0     1854 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/data/namespaces.yml
+-rw-r--r--   0        0        0    17819 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/dataset.py
+-rw-r--r--   0        0        0        0 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/evaluation/__init__.py
+-rw-r--r--   0        0        0     3418 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/evaluation/cpa_cta_metrics.py
+-rw-r--r--   0        0        0     4064 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/evaluation/hierarchy_scoring_fn.py
+-rw-r--r--   0        0        0     2684 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/evaluation/precision_recall_f1.py
+-rw-r--r--   0        0        0      585 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/evaluation/prelude.py
+-rw-r--r--   0        0        0    23741 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/evaluation/sm_metrics.py
+-rw-r--r--   0        0        0     1844 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/evaluation/transformation.py
+-rw-r--r--   0        0        0     1174 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/evaluation/utils.py
+-rw-r--r--   0        0        0        0 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/inputs/__init__.py
+-rw-r--r--   0        0        0     2113 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/inputs/column.py
+-rw-r--r--   0        0        0     2968 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/inputs/context.py
+-rw-r--r--   0        0        0     4084 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/inputs/link.py
+-rw-r--r--   0        0        0      313 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/inputs/prelude.py
+-rw-r--r--   0        0        0     4686 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/inputs/table.py
+-rw-r--r--   0        0        0        0 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/misc/__init__.py
+-rw-r--r--   0        0        0     2505 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/misc/bijection.py
+-rw-r--r--   0        0        0     8221 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/misc/deser.py
+-rw-r--r--   0        0        0     6950 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/misc/exp_manager.py
+-rw-r--r--   0        0        0     3538 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/misc/fn_cache.py
+-rw-r--r--   0        0        0    15012 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/misc/funcs.py
+-rw-r--r--   0        0        0     1832 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/misc/logger.py
+-rw-r--r--   0        0        0     3009 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/misc/matrix.py
+-rw-r--r--   0        0        0      284 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/misc/prelude.py
+-rw-r--r--   0        0        0    11345 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/misc/ray_helper.py
+-rw-r--r--   0        0        0     3773 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/misc/timer.py
+-rw-r--r--   0        0        0        0 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/namespaces/__init__.py
+-rw-r--r--   0        0        0     7303 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/namespaces/namespace.py
+-rw-r--r--   0        0        0     2966 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/namespaces/prefix_index.py
+-rw-r--r--   0        0        0      329 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/namespaces/prelude.py
+-rw-r--r--   0        0        0      772 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/namespaces/utils.py
+-rw-r--r--   0        0        0     5637 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/namespaces/wikidata.py
+-rw-r--r--   0        0        0        0 2024-03-04 02:49:26.180264 sem_desc-6.9.0/sm/outputs/__init__.py
+-rw-r--r--   0        0        0    34206 2024-03-04 02:49:26.184264 sem_desc-6.9.0/sm/outputs/semantic_model.py
+-rw-r--r--   0        0        0      174 2024-03-04 02:49:26.184264 sem_desc-6.9.0/sm/prelude.py
+-rw-r--r--   0        0        0        0 2024-03-04 02:49:26.184264 sem_desc-6.9.0/sm/py.typed
+-rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 sem_desc-6.9.0/PKG-INFO
```

### Comparing `sem_desc-6.8.0/pyproject.toml` & `sem_desc-6.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sem-desc"
-version = "6.8.0"
+version = "6.9.0"
 description = "Package providing basic functionalities for the semantic modeling problem"
 authors = ["Binh Vu <binh@toan2.com>"]
 license = "MIT"
 packages = [{ include = "sm" }]
 
 readme = "README.md"
 homepage = "https://github.com/binh-vu/sm"
```

### Comparing `sem_desc-6.8.0/sm/data/namespaces.yml` & `sem_desc-6.9.0/sm/data/namespaces.yml`

 * *Files identical despite different names*

### Comparing `sem_desc-6.8.0/sm/dataset.py` & `sem_desc-6.9.0/sm/dataset.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import csv
 import random
 import shutil
 from contextlib import contextmanager
 from dataclasses import dataclass
 from hashlib import md5
 from io import BytesIO, StringIO
 from operator import attrgetter
@@ -24,22 +25,24 @@
 
 import orjson
 import pandas as pd
 import serde.csv
 import serde.yaml
 from ruamel.yaml import YAML
 from serde import json
+from serde.helper import DEFAULT_ORJSON_OPTS, get_open_fn
 from slugify import slugify
+from tqdm.auto import tqdm
+from typing_extensions import Self
+
 from sm.inputs.prelude import ColumnBasedTable, Context, Link
 from sm.misc.funcs import batch
 from sm.misc.matrix import Matrix
 from sm.namespaces.namespace import Namespace
 from sm.outputs.semantic_model import SemanticModel
-from tqdm.auto import tqdm
-from typing_extensions import Self
 
 T = TypeVar("T", covariant=True)
 T1 = TypeVar("T1")
 
 
 @dataclass
 class Example(Generic[T]):
@@ -179,56 +182,31 @@
         deserialization functions.
 
         Args:
             data_dir:
 
         Returns:
         """
-
-        def deser_table(table_id: str, data: bytes, ext: str):
-            if ext == ".json":
-                return FullTable.from_dict(orjson.loads(data))
-            if ext == ".csv":
-                column_based_table = ColumnBasedTable.from_dataframe(
-                    pd.read_csv(BytesIO(data)),
-                    table_id=table_id,
-                )
-                return FullTable(
-                    table=column_based_table,
-                    context=Context(),
-                    links=Matrix.default(column_based_table.shape(), list),
-                )
-            if ext == ".xlsx":
-                column_based_table = ColumnBasedTable.from_dataframe(
-                    pd.read_excel(BytesIO(data)),
-                    table_id=table_id,
-                )
-                return FullTable(
-                    table=column_based_table,
-                    context=Context(),
-                    links=Matrix.default(column_based_table.shape(), list),
-                )
-
-            raise ValueError(f"Unknown file type: {ext}")
-
         examples = []
         with self._open() as root:
             descdir = self.description_dir(root)
             tabledir = self.table_dir(root)
 
             for infile in tqdm(
                 sorted(tabledir.iterdir(), key=attrgetter("name")), disable=not verbose
             ):
                 suffixes = Path(infile.name).suffixes
                 if infile.name.startswith(".") or len(suffixes) == 0:
                     continue
 
                 if suffixes[-1] != ".zip":
                     example_id = infile.name[: -sum(len(x) for x in suffixes)]
-                    table = deser_table(example_id, infile.read_bytes(), suffixes[0])
+                    table = self._deser_table(
+                        example_id, infile.read_bytes(), suffixes[0]
+                    )
 
                     if descdir.exists():
                         if (descdir / example_id).exists():
                             desc_file = max(
                                 (descdir / example_id).iterdir(),
                                 key=lambda file: int(file.name.split(".")[1]),
                             )
@@ -267,15 +245,15 @@
                     with ZipFile(infile, mode="r") as zf:
                         for file in zf.infolist():
                             if not file.filename.endswith(".json"):
                                 continue
 
                             table_id = Path(file.filename).stem
                             with zf.open(file, mode="r") as f:
-                                table = deser_table(
+                                table = self._deser_table(
                                     table_id, f.read(), Path(file.filename).suffixes[0]
                                 )
                             part[table_id] = table
 
                     if descdir.exists():
                         lst = []
                         with ZipFile(descdir / infile.name, mode="r") as zf:
@@ -309,14 +287,15 @@
 
     def save(
         self,
         examples: list[Example[FullTable]],
         individual_table_compressed: Optional[Literal["gz", "bz2", "lz4"]] = None,
         batch_compressed: bool = False,
         batch_size: int = 100,
+        table_fmt: Literal["json", "txt"] = "json",
         table_fmt_indent: Literal[0, 2] = 0,
         clean_previous_data: bool = True,
     ):
         descdir = self.description_dir(self.location)
         tabledir = self.table_dir(self.location)
         assert (
             not self.is_zip_file()
@@ -336,41 +315,137 @@
             for i, bexamples in enumerate(batch(batch_size, examples)):
                 bexamples: list[Example[FullTable]]
                 filename = f"part-{i:04d}.zip"
                 with ZipFile(descdir / filename, "w") as dzf, ZipFile(
                     tabledir / filename, "w"
                 ) as tzf:
                     for e in bexamples:
-                        ename = get_friendly_fs_id(e.table.table.table_id) + ".json"
+                        ename = (
+                            get_friendly_fs_id(e.table.table.table_id) + f".{table_fmt}"
+                        )
                         dzf.writestr(
                             ename,
                             data=orjson.dumps([sm.to_dict() for sm in e.sms]),
                         )
                         tzf.writestr(
                             ename,
-                            data=orjson.dumps(e.table.to_dict()),
+                            data=self._ser_table(e.table, table_fmt, table_fmt_indent),
                         )
         else:
             for e in examples:
                 filename = get_friendly_fs_id(e.table.table.table_id)
                 (descdir / filename).mkdir(exist_ok=True)
                 compressed_filename = (
-                    filename + f".json.{individual_table_compressed}"
+                    filename + f".{table_fmt}.{individual_table_compressed}"
                     if individual_table_compressed is not None
-                    else filename + ".json"
+                    else filename + f".{table_fmt}"
                 )
                 json.ser(
                     [sm.to_dict() for sm in e.sms],
                     descdir / filename / "version.01.json",
                     indent=2,
                 )
-                json.ser(
-                    e.table, tabledir / compressed_filename, indent=table_fmt_indent
+                with get_open_fn(tabledir / compressed_filename)(
+                    tabledir / compressed_filename, "wb"
+                ) as f:
+                    f.write(self._ser_table(e.table, table_fmt, table_fmt_indent))
+
+    @staticmethod
+    def _deser_table(table_id: str, data: bytes, ext: str) -> FullTable:
+        if ext == ".json":
+            return FullTable.from_dict(orjson.loads(data))
+        if ext == ".csv":
+            column_based_table = ColumnBasedTable.from_dataframe(
+                pd.read_csv(BytesIO(data)),
+                table_id=table_id,
+            )
+            return FullTable(
+                table=column_based_table,
+                context=Context(),
+                links=Matrix.default(column_based_table.shape(), list),
+            )
+        if ext == ".xlsx":
+            column_based_table = ColumnBasedTable.from_dataframe(
+                pd.read_excel(BytesIO(data)),
+                table_id=table_id,
+            )
+            return FullTable(
+                table=column_based_table,
+                context=Context(),
+                links=Matrix.default(column_based_table.shape(), list),
+            )
+        if ext == ".txt":
+            part1_csv, part2_json = data.split(b"\n" + b"-" * 80 + b"\n\n")
+            column_based_table = ColumnBasedTable.from_dataframe(
+                pd.read_csv(BytesIO(part1_csv)),
+                table_id=table_id,
+            )
+            obj = orjson.loads(part2_json)
+            return FullTable(
+                table=column_based_table,
+                context=Context.from_dict(obj["context"]),
+                links=Matrix(
+                    [
+                        [[Link.from_dict(link) for link in cell] for cell in row]
+                        for row in obj["links"]
+                    ]
+                ),
+            )
+
+        raise ValueError(f"Unknown file type: {ext}")
+
+    @staticmethod
+    def _ser_table(
+        table: FullTable,
+        table_fmt: Literal["json", "txt"] = "json",
+        table_fmt_indent: Literal[0, 2] = 0,
+    ):
+        if table_fmt == "json":
+            if table_fmt_indent > 0:
+                orjson_opts = DEFAULT_ORJSON_OPTS | orjson.OPT_INDENT_2
+            else:
+                orjson_opts = DEFAULT_ORJSON_OPTS
+
+            return orjson.dumps(table.to_dict(), option=orjson_opts)
+
+        if table_fmt == "txt":
+            out = StringIO()
+            nrows, ncols = table.table.shape()
+
+            writer = csv.writer(
+                out, delimiter=",", quoting=csv.QUOTE_MINIMAL, lineterminator="\n"
+            )
+            writer.writerow([c.name for c in table.table.columns])
+            for ri in range(nrows):
+                writer.writerow(
+                    [table.table.columns[ci].values[ri] for ci in range(ncols)]
                 )
 
+            out.write("\n" + "-" * 80 + "\n\n")
+            if table_fmt_indent > 0:
+                orjson_opts = DEFAULT_ORJSON_OPTS | orjson.OPT_INDENT_2
+            else:
+                orjson_opts = DEFAULT_ORJSON_OPTS
+
+            out.write(
+                orjson.dumps(
+                    {
+                        "context": table.context.to_dict(),
+                        "links": [
+                            [[link.to_dict() for link in cell] for cell in row]
+                            for row in table.links.data
+                        ],
+                    },
+                    option=orjson_opts,
+                ).decode()
+            )
+            return out.getvalue().encode()
+
+        raise ValueError(f"Unsupported format: {table_fmt}")
+
 
 def get_friendly_fs_id(id: str) -> str:
     if id.startswith("http://") or id.startswith("https://"):
         if id.find("dbpedia.org") != -1:
             return (
                 slugify(
                     urlparse(id).path.replace("/resource/", "").replace("/", "_")
@@ -389,19 +464,17 @@
             )
 
         raise NotImplementedError()
     return slugify(id.replace("/", "_"), lowercase=False).replace("-", "_")
 
 
 class SampleableTable(Protocol):
-    def nrows(self) -> int:
-        ...
+    def nrows(self) -> int: ...
 
-    def select_rows(self, indices: list[int]) -> Self:
-        ...
+    def select_rows(self, indices: list[int]) -> Self: ...
 
 
 ST = TypeVar("ST", bound=SampleableTable, covariant=True)
 
 
 def sample_table_data(
     examples: Sequence[Example[ST]], n_rows: int, seed: Optional[int] = None
```

### Comparing `sem_desc-6.8.0/sm/evaluation/cpa_cta_metrics.py` & `sem_desc-6.9.0/sm/evaluation/cpa_cta_metrics.py`

 * *Files identical despite different names*

### Comparing `sem_desc-6.8.0/sm/evaluation/hierarchy_scoring_fn.py` & `sem_desc-6.9.0/sm/evaluation/hierarchy_scoring_fn.py`

 * *Files identical despite different names*

### Comparing `sem_desc-6.8.0/sm/evaluation/precision_recall_f1.py` & `sem_desc-6.9.0/sm/evaluation/precision_recall_f1.py`

 * *Files identical despite different names*

### Comparing `sem_desc-6.8.0/sm/evaluation/prelude.py` & `sem_desc-6.9.0/sm/evaluation/prelude.py`

 * *Files identical despite different names*

### Comparing `sem_desc-6.8.0/sm/evaluation/sm_metrics.py` & `sem_desc-6.9.0/sm/evaluation/sm_metrics.py`

 * *Files identical despite different names*

### Comparing `sem_desc-6.8.0/sm/evaluation/transformation.py` & `sem_desc-6.9.0/sm/evaluation/transformation.py`

 * *Files identical despite different names*

### Comparing `sem_desc-6.8.0/sm/evaluation/utils.py` & `sem_desc-6.9.0/sm/evaluation/utils.py`

 * *Files identical despite different names*

### Comparing `sem_desc-6.8.0/sm/inputs/column.py` & `sem_desc-6.9.0/sm/inputs/column.py`

 * *Files identical despite different names*

### Comparing `sem_desc-6.8.0/sm/inputs/context.py` & `sem_desc-6.9.0/sm/inputs/context.py`

 * *Files identical despite different names*

### Comparing `sem_desc-6.8.0/sm/inputs/link.py` & `sem_desc-6.9.0/sm/inputs/link.py`

 * *Files identical despite different names*

### Comparing `sem_desc-6.8.0/sm/inputs/table.py` & `sem_desc-6.9.0/sm/inputs/table.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,27 @@
 
     def select_rows(self, indices: list[int]) -> ColumnBasedTable:
         """Select a subset of rows based on a boolean mask"""
         return ColumnBasedTable(
             self.table_id, [col.select_rows(indices) for col in self.columns]
         )
 
+    def remove_empty_rows(self):
+        nrows, ncols = self.shape()
+        select_rows = []
+        for ri in range(nrows):
+            if not all(
+                self.columns[ci].values[ri].strip() == "" for ci in range(ncols)
+            ):
+                select_rows.append(ri)
+
+        if len(select_rows) != nrows:
+            return self.select_rows(select_rows)
+        return self
+
     def ncols(self) -> int:
         return len(self.columns)
 
     def nrows(self) -> int:
         if len(self.columns) == 0:
             return 0
         return len(self.columns[0].values)
```

### Comparing `sem_desc-6.8.0/sm/misc/bijection.py` & `sem_desc-6.9.0/sm/misc/bijection.py`

 * *Files identical despite different names*

### Comparing `sem_desc-6.8.0/sm/misc/deser.py` & `sem_desc-6.9.0/sm/misc/deser.py`

 * *Files identical despite different names*

### Comparing `sem_desc-6.8.0/sm/misc/exp_manager.py` & `sem_desc-6.9.0/sm/misc/exp_manager.py`

 * *Files identical despite different names*

### Comparing `sem_desc-6.8.0/sm/misc/fn_cache.py` & `sem_desc-6.9.0/sm/misc/fn_cache.py`

 * *Files identical despite different names*

### Comparing `sem_desc-6.8.0/sm/misc/funcs.py` & `sem_desc-6.9.0/sm/misc/funcs.py`

 * *Files identical despite different names*

### Comparing `sem_desc-6.8.0/sm/misc/logger.py` & `sem_desc-6.9.0/sm/misc/logger.py`

 * *Files identical despite different names*

### Comparing `sem_desc-6.8.0/sm/misc/matrix.py` & `sem_desc-6.9.0/sm/misc/matrix.py`

 * *Files identical despite different names*

### Comparing `sem_desc-6.8.0/sm/misc/ray_helper.py` & `sem_desc-6.9.0/sm/misc/ray_helper.py`

 * *Files identical despite different names*

### Comparing `sem_desc-6.8.0/sm/misc/timer.py` & `sem_desc-6.9.0/sm/misc/timer.py`

 * *Files identical despite different names*

### Comparing `sem_desc-6.8.0/sm/namespaces/namespace.py` & `sem_desc-6.9.0/sm/namespaces/namespace.py`

 * *Files identical despite different names*

### Comparing `sem_desc-6.8.0/sm/namespaces/prefix_index.py` & `sem_desc-6.9.0/sm/namespaces/prefix_index.py`

 * *Files identical despite different names*

### Comparing `sem_desc-6.8.0/sm/namespaces/utils.py` & `sem_desc-6.9.0/sm/namespaces/utils.py`

 * *Files identical despite different names*

### Comparing `sem_desc-6.8.0/sm/namespaces/wikidata.py` & `sem_desc-6.9.0/sm/namespaces/wikidata.py`

 * *Files identical despite different names*

### Comparing `sem_desc-6.8.0/sm/outputs/semantic_model.py` & `sem_desc-6.9.0/sm/outputs/semantic_model.py`

 * *Files identical despite different names*

### Comparing `sem_desc-6.8.0/PKG-INFO` & `sem_desc-6.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sem-desc
-Version: 6.8.0
+Version: 6.9.0
 Summary: Package providing basic functionalities for the semantic modeling problem
 Home-page: https://github.com/binh-vu/sm
 License: MIT
 Author: Binh Vu
 Author-email: binh@toan2.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

