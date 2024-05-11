# Comparing `tmp/eralchemy2-1.3.8.tar.gz` & `tmp/eralchemy2-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eralchemy2-1.3.8.tar", max compression
+gzip compressed data, was "eralchemy2-1.4.0.tar", last modified: Sat May 11 20:30:12 2024, max compression
```

## Comparing `eralchemy2-1.3.8.tar` & `eralchemy2-1.4.0.tar`

### file list

```diff
@@ -1,12 +1,31 @@
--rw-r--r--   0        0        0    10778 2022-06-26 17:13:03.424365 eralchemy2-1.3.8/LICENSE.md
--rw-r--r--   0        0        0     3595 2022-09-11 20:03:10.738987 eralchemy2-1.3.8/README.md
--rw-r--r--   0        0        0      117 2022-10-07 12:39:26.511571 eralchemy2-1.3.8/eralchemy2/__init__.py
--rw-r--r--   0        0        0      626 2022-10-19 09:21:21.991971 eralchemy2-1.3.8/eralchemy2/cst.py
--rw-r--r--   0        0        0     1437 2022-10-07 12:39:26.511571 eralchemy2-1.3.8/eralchemy2/helpers.py
--rw-r--r--   0        0        0    11262 2023-04-24 19:20:15.046497 eralchemy2-1.3.8/eralchemy2/main.py
--rw-r--r--   0        0        0     7789 2023-10-30 13:51:33.583933 eralchemy2-1.3.8/eralchemy2/models.py
--rw-r--r--   0        0        0     5732 2022-10-07 12:39:26.511571 eralchemy2-1.3.8/eralchemy2/parser.py
--rw-r--r--   0        0        0        0 2022-10-07 12:39:26.511571 eralchemy2-1.3.8/eralchemy2/py.typed
--rw-r--r--   0        0        0     3413 2023-08-04 09:13:08.457641 eralchemy2-1.3.8/eralchemy2/sqla.py
--rw-r--r--   0        0        0     2662 2023-10-30 14:06:38.521496 eralchemy2-1.3.8/pyproject.toml
--rw-r--r--   0        0        0     4980 1970-01-01 00:00:00.000000 eralchemy2-1.3.8/PKG-INFO
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-11 20:30:12.524931 eralchemy2-1.4.0/
+-rw-r--r--   0 maurer    (1000) maurer    (1000)    10775 2023-11-23 10:27:49.000000 eralchemy2-1.4.0/LICENSE.md
+-rw-r--r--   0 maurer    (1000) maurer    (1000)       37 2022-09-11 17:50:47.000000 eralchemy2-1.4.0/MANIFEST.in
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     5211 2024-05-11 20:30:12.524931 eralchemy2-1.4.0/PKG-INFO
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     4112 2024-05-11 20:14:40.000000 eralchemy2-1.4.0/README.md
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-11 20:30:12.520931 eralchemy2-1.4.0/eralchemy2/
+-rw-r--r--   0 maurer    (1000) maurer    (1000)       81 2023-11-23 10:27:49.000000 eralchemy2-1.4.0/eralchemy2/__init__.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)      591 2024-05-11 16:10:47.000000 eralchemy2-1.4.0/eralchemy2/cst.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     1441 2024-05-11 16:03:23.000000 eralchemy2-1.4.0/eralchemy2/helpers.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)    12096 2024-05-11 16:10:47.000000 eralchemy2-1.4.0/eralchemy2/main.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     8675 2024-05-11 20:14:40.000000 eralchemy2-1.4.0/eralchemy2/models.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     5681 2024-05-11 20:14:40.000000 eralchemy2-1.4.0/eralchemy2/parser.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)        0 2022-10-07 12:39:26.000000 eralchemy2-1.4.0/eralchemy2/py.typed
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     4768 2024-05-11 20:17:52.000000 eralchemy2-1.4.0/eralchemy2/sqla.py
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-11 20:30:12.524931 eralchemy2-1.4.0/eralchemy2.egg-info/
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     5211 2024-05-11 20:30:12.000000 eralchemy2-1.4.0/eralchemy2.egg-info/PKG-INFO
+-rw-r--r--   0 maurer    (1000) maurer    (1000)      610 2024-05-11 20:30:12.000000 eralchemy2-1.4.0/eralchemy2.egg-info/SOURCES.txt
+-rw-r--r--   0 maurer    (1000) maurer    (1000)        1 2024-05-11 20:30:12.000000 eralchemy2-1.4.0/eralchemy2.egg-info/dependency_links.txt
+-rw-r--r--   0 maurer    (1000) maurer    (1000)       51 2024-05-11 20:30:12.000000 eralchemy2-1.4.0/eralchemy2.egg-info/entry_points.txt
+-rw-r--r--   0 maurer    (1000) maurer    (1000)      124 2024-05-11 20:30:12.000000 eralchemy2-1.4.0/eralchemy2.egg-info/requires.txt
+-rw-r--r--   0 maurer    (1000) maurer    (1000)       11 2024-05-11 20:30:12.000000 eralchemy2-1.4.0/eralchemy2.egg-info/top_level.txt
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     2669 2024-05-11 20:25:41.000000 eralchemy2-1.4.0/pyproject.toml
+-rw-r--r--   0 maurer    (1000) maurer    (1000)       38 2024-05-11 20:30:12.524931 eralchemy2-1.4.0/setup.cfg
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-11 20:30:12.524931 eralchemy2-1.4.0/tests/
+-rw-r--r--   0 maurer    (1000) maurer    (1000)      365 2023-11-23 09:51:34.000000 eralchemy2-1.4.0/tests/test_argparse.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     3142 2024-05-11 16:10:47.000000 eralchemy2-1.4.0/tests/test_intermediary_to_dot.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     1450 2024-05-11 20:14:40.000000 eralchemy2-1.4.0/tests/test_intermediary_to_er.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     3095 2024-05-11 16:10:47.000000 eralchemy2-1.4.0/tests/test_main.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     5297 2024-05-11 20:14:40.000000 eralchemy2-1.4.0/tests/test_parser.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     3147 2024-05-11 20:14:40.000000 eralchemy2-1.4.0/tests/test_sqla_multi_key.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     3344 2024-05-11 20:18:04.000000 eralchemy2-1.4.0/tests/test_sqla_to_intermediary.py
```

### Comparing `eralchemy2-1.3.8/LICENSE.md` & `eralchemy2-1.4.0/LICENSE.md`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
       on Your own behalf and on Your sole responsibility, not on behalf
       of any other Contributor, and only if You agree to indemnify,
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
 
    END OF TERMS AND CONDITIONS
-   
+
    Copyright 2022 Alexis Benoist, Florian Maurer
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `eralchemy2-1.3.8/README.md` & `eralchemy2-1.4.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -22,21 +22,33 @@
 ### Install
 To install eralchemy2, just do:
 
     $ pip install eralchemy2
 
 `eralchemy2` requires [GraphViz](http://www.graphviz.org/download) to generate the graphs and Python. Both are available for Windows, Mac and Linux.
 
+For Debian based systems, run:
+
+    $ apt install graphviz libgraphviz-dev
+
+before installing eralchemy2.
+
+### Install using conda
+
+There is also a packaged version in conda-forge, which directly installs the dependencies:
+
+    $ conda install -c conda-forge eralchemy2
+
 ### Usage from Command Line
 
 #### From a database
 
     $ eralchemy2 -i sqlite:///relative/path/to/db.db -o erd_from_sqlite.pdf
 
-The database is specified as a [SQLAlchemy](http://docs.sqlalchemy.org/en/rel_1_0/core/engines.html#database-urls)
+The database is specified as a [SQLAlchemy](https://docs.sqlalchemy.org/en/20/core/engines.html#database-urls)
 database url.
 
 #### From a markdown file.
 
     $ curl 'https://raw.githubusercontent.com/maurerle/eralchemy2/main/example/newsmeme.er' > markdown_file.er
     $ eralchemy2 -i 'markdown_file.er' -o erd_from_markdown_file.pdf
 
@@ -44,17 +56,21 @@
 
     $ eralchemy2 -i 'postgresql+psycopg2://username:password@hostname:5432/databasename' -o filtered.er --exclude-tables temp audit
 
 #### From a Postgresql DB to a markdown file excluding columns named `created_at` and `updated_at` from all tables
 
     $ eralchemy2 -i 'postgresql+psycopg2://username:password@hostname:5432/databasename' -o filtered.er --exclude-columns created_at updated_at
 
-#### From a Postgresql DB to a markdown file for the schema `schema`
+#### From a Postgresql DB to a markdown file for the schemas `schema1` and `schema2`
+
+    $ eralchemy2 -i 'postgresql+psycopg2://username:password@hostname:5432/databasename' -s "schema1, schema2"
+
+#### Specify Output Mode
 
-    $ eralchemy2 -i 'postgresql+psycopg2://username:password@hostname:5432/databasename' -s schema
+    $ eralchemy2 -i 'markdown_file.er' -o erd_from_markdown_file.md -m mermaid_er
 
 ### Usage from Python
 
 ```python
 from eralchemy2 import render_er
 ## Draw from SQLAlchemy base
 render_er(Base, 'erd_from_sqlalchemy.png')
@@ -75,18 +91,22 @@
 To run the tests, use : `$ py.test` or `$ tox`.
 Some tests require a local postgres database with a schema named test in a database
 named test all owned by a user named eralchemy with a password of eralchemy.
 This can be easily set up using docker-compose with: `docker-compose up -d`.
 
 All tested PR are welcome.
 
+## Publishing a release
+
+    $ rm -r dist && python -m build && python3 -m twine upload --repository pypi dist/*
+
 ## Notes
 
 eralchemy2 is a fork of its predecessor [ERAlchemy](https://github.com/Alexis-benoist/eralchemy) by @Alexis-benoist, which is not maintained anymore and does not work with SQLAlchemy > 1.4.
 If it is maintained again, I'd like to push the integrated changes upstream.
 
 ERAlchemy was inspired by [erd](https://github.com/BurntSushi/erd), though it is able to render the ER diagram directly
 from the database and not just only from the `ER` markup language.
 
 Released under an Apache License 2.0
 
-Initial Creator: Alexis Benoist [Alexis_Benoist](https://twitter.com/Alexis_Benoist)
+Initial Creator: Alexis Benoist [Alexis_Benoist](https://github.com/Alexis-benoist)
```

### Comparing `eralchemy2-1.3.8/eralchemy2/cst.py` & `eralchemy2-1.4.0/eralchemy2/cst.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
 All the constants used in the module.
 """
-from __future__ import annotations
 
 TABLE = (
     '"{}" [label=<<FONT FACE="Helvetica"><TABLE BORDER="0" CELLBORDER="1"'
     ' CELLPADDING="4" CELLSPACING="0">{}{}</TABLE></FONT>>];'
 )
 
 START_CELL = '<TR><TD ALIGN="LEFT"><FONT>'
```

### Comparing `eralchemy2-1.3.8/eralchemy2/helpers.py` & `eralchemy2-1.4.0/eralchemy2/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 
 def check_args(args: Namespace) -> None:
     """Checks that the args are coherent."""
     check_args_has_attributes(args)
     if args.v:
         non_version_attrs = [v for k, v in args.__dict__.items() if k != "v"]
-        print("non_version_attrs", non_version_attrs)
         if len([v for v in non_version_attrs if v is not None]) != 0:
+            print("non_version_attrs", non_version_attrs)
             fail("Cannot show the version number with another command.")
         return
     if args.i is None:
         fail("Cannot draw ER diagram of no database.")
     if args.o is None:
         fail("Cannot draw ER diagram with no output file.")
```

### Comparing `eralchemy2-1.3.8/eralchemy2/main.py` & `eralchemy2-1.4.0/eralchemy2/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from __future__ import annotations
-
 import argparse
 import base64
 import copy
 import sys
+from importlib.metadata import version
 
 from pygraphviz.agraph import AGraph
 from sqlalchemy.engine.url import make_url
 from sqlalchemy.exc import ArgumentError
 
 from .cst import GRAPH_BEGINNING
 from .helpers import check_args
@@ -18,20 +17,14 @@
 )
 from .sqla import (
     database_to_intermediary,
     declarative_to_intermediary,
     metadata_to_intermediary,
 )
 
-if sys.version_info >= (3, 8):
-    from importlib.metadata import version
-else:
-    # importlib.metadata not available for python 3.7
-    from importlib_metadata import version
-
 __version__ = version(__package__)
 
 
 def cli() -> None:
     """Entry point for the application script"""
     parser = get_argparser()
 
@@ -39,28 +32,34 @@
     check_args(args)
     if args.v:
         print("eralchemy2 version {}.".format(__version__))
         exit(0)
     render_er(
         args.i,
         args.o,
+        args.m or "auto",
         include_tables=args.include_tables,
         include_columns=args.include_columns,
         exclude_tables=args.exclude_tables,
         exclude_columns=args.exclude_columns,
         schema=args.s,
     )
 
 
 def get_argparser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(prog="eralchemy2")
     parser.add_argument("-i", nargs="?", help="Database URI to process.")
     parser.add_argument("-o", nargs="?", help="Name of the file to write.")
     parser.add_argument("-s", nargs="?", help="Name of the schema.")
     parser.add_argument(
+        "-m",
+        nargs="?",
+        help="Output mode to write format, default: auto",
+    )
+    parser.add_argument(
         "--exclude-tables", "-x", nargs="+", help="Name of tables not to be displayed."
     )
     parser.add_argument(
         "--exclude-columns",
         nargs="+",
         help="Name of columns not to be displayed (for all tables).",
     )
@@ -89,14 +88,24 @@
     md_markup = "<!--\n\n{}\n\n-->\n".format(markup)
     markup_b64 = base64.urlsafe_b64encode(markup.encode("utf8")).decode("ascii")
     md_markup += "![](https://mermaid.ink/img/{})\n".format(markup_b64)
     with open(output, "w") as file_out:
         file_out.write(md_markup)
 
 
+def intermediary_to_mermaid_er(tables, relationships, output):
+    """Saves the intermediary representation to markdown."""
+    markup = _intermediary_to_mermaid_er(tables, relationships)
+    md_markup = "<!--\n\n{}\n\n-->\n".format(markup)
+    markup_b64 = base64.urlsafe_b64encode(markup.encode("utf8")).decode("ascii")
+    md_markup += "![](https://mermaid.ink/img/{})\n".format(markup_b64)
+    with open(output, "w") as file_out:
+        file_out.write(md_markup)
+
+
 def intermediary_to_dot(tables, relationships, output):
     """Save the intermediary representation to dot format."""
     dot_file = _intermediary_to_dot(tables, relationships)
     with open(output, "w") as file_out:
         file_out.write(dot_file)
 
 
@@ -119,14 +128,21 @@
 def _intermediary_to_mermaid(tables, relationships):
     """Returns the er markup source in a string."""
     t = "\n".join(t.to_mermaid() for t in tables)
     r = "\n".join(r.to_mermaid() for r in relationships)
     return "classDiagram\n{}\n{}".format(t, r)
 
 
+def _intermediary_to_mermaid_er(tables, relationships):
+    """Returns the er markup source in a string."""
+    t = "\n".join(t.to_mermaid_er() for t in tables)
+    r = "\n".join(r.to_mermaid_er() for r in relationships)
+    return "erDiagram\n{}\n{}".format(t, r)
+
+
 def _intermediary_to_dot(tables, relationships):
     """Returns the dot source representing the database in a string."""
     t = "\n".join(t.to_dot() for t in tables)
     r = "\n".join(r.to_dot() for r in relationships)
     return "{}\n{}\n{}\n}}".format(GRAPH_BEGINNING, t, r)
 
 
@@ -143,14 +159,15 @@
 }
 
 # Routes from the mode to the method to transform the intermediary
 #  representation to the desired output.
 switch_output_mode_auto = {
     "er": intermediary_to_markdown,
     "mermaid": intermediary_to_mermaid,
+    "mermaid_er": intermediary_to_mermaid_er,
     "graph": intermediary_to_schema,
     "dot": intermediary_to_dot,
 }
 
 # Routes from the file extension to the method to transform
 # the intermediary representation to the desired output.
 switch_output_mode = {
@@ -278,14 +295,15 @@
         MetaData: SQLAlchemy Metadata
         DeclarativeMeta: SQLAlchemy declarative Base
     :param output: name of the file to output the
     :param mode: str in list:
         'er': writes to a file the markup to generate an ER style diagram.
         'graph': writes the image of the ER diagram.
         'mermaid': writes to a file the markup to generate an Mermaid-JS style diagram
+        'mermaid_er': writes the markup to generate an Mermaid-JS ER diagram
         'dot': write to file the diagram in dot format.
         'auto': choose from the filename:
             '*.er': writes to a file the markup to generate an ER style diagram.
             '.dot': returns the graph in the dot syntax.
             '.md': writes to a file the markup to generate an Mermaid-JS style diagram
             else: return a graph to the format graph
     :param include_tables: lst of str, table names to include, None means include all
```

### Comparing `eralchemy2-1.3.8/eralchemy2/models.py` & `eralchemy2-1.4.0/eralchemy2/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 """
 
 from __future__ import annotations
 
 import operator
 import re
 from abc import ABC, abstractmethod
-from typing import Any, ClassVar
+from typing import ClassVar
 
 from .cst import FONT_TAGS, ROW_TAGS, TABLE
 
 
 class Drawable(ABC):
     """Abstract class to represent all the objects which are drawable."""
 
     RE: ClassVar[re.Pattern[str]]
 
     def to_markdown(self) -> str:
         """Transforms the intermediary object to it's syntax in the er markup."""
+
         raise NotImplementedError()
 
     def to_dot(self) -> str:
         """Transforms the intermediary object to it's syntax in the dot format."""
         raise NotImplementedError()
 
     def __eq__(self, other) -> bool:
@@ -38,38 +39,38 @@
         return self.to_markdown()
 
 
 class Column(Drawable):
     """Represents a Column in the intermediaty syntax"""
 
     RE = re.compile(
-        '(?P<primary>\*?)(?P<name>\w+(\s*\w+)*)\s*(\{label:\s*"(?P<label>[^"]+)"\})?'
+        r'(?P<primary>\*?)(?P<name>\w+(\s*\w+)*)\s*(\{label:\s*"(?P<label>[^"]+)"\})?',
     )
 
     @staticmethod
     def make_from_match(match: re.Match) -> Column:
         return Column(
             name=match.group("name"),
             type=match.group("label"),
             is_key="*" in match.group("primary"),
-            is_null=not "*" in match.group("primary"),
+            is_null="*" not in match.group("primary"),
         )
 
     def __init__(self, name: str, type=None, is_key: bool = False, is_null=None):
         """
         :param name: (str) Name of the column
         :param type:
         :param is_key:
         :param is_null:
         :return:
         """
         self.name = name
         self.type = type
         self.is_key = is_key
-        if is_null == None:
+        if is_null is None:
             self.is_null = not is_key
         else:
             self.is_null = is_null
 
     def __lt__(self, other: Column) -> bool:
         if self.is_key > other.is_key:
             return True
@@ -79,51 +80,62 @@
             return self.name < other.name
 
     @property
     def key_symbol(self) -> str:
         return "*" if self.is_key else ""
 
     def to_markdown(self) -> str:
-        return '    {}{} {{label:"{}"}}'.format(self.key_symbol, self.name, self.type)
+        return f'    {self.key_symbol}{self.name} {{label:"{self.type}"}}'
 
     def to_mermaid(self) -> str:
         return " {}{} {}{}".format(
             self.key_symbol,
             self.type.replace("(", "<").replace(")", ">"),
             self.name,
             " NOT NULL" if not self.is_null else "",
         )
 
+    def to_mermaid_er(self) -> str:
+        type_str = self.type.replace(" ", "_")
+        return f" {type_str} {self.name} {'PK' if self.is_key else ''}"
+
     def to_dot(self) -> str:
         base = ROW_TAGS.format(
-            ' ALIGN="LEFT"', "{key_opening}{col_name}{key_closing}{type}{null}"
+            ' ALIGN="LEFT"', "{key_opening}{col_name}{key_closing} {type}{null}"
         )
         return base.format(
             key_opening="<u>" if self.is_key else "",
             key_closing="</u>" if self.is_key else "",
             col_name=FONT_TAGS.format(self.name),
-            type=FONT_TAGS.format(" [{}]").format(self.type)
-            if self.type is not None
-            else "",
+            type=(
+                FONT_TAGS.format(" [{}]").format(self.type)
+                if self.type is not None
+                else ""
+            ),
             null=" NOT NULL" if not self.is_null else "",
         )
 
 
 class Relation(Drawable):
     """Represents a Relation in the intermediaty syntax"""
 
     RE = re.compile(
-        "(?P<left_name>\S+(\s*\S+)?)\s+(?P<left_cardinality>[*?+1])--(?P<right_cardinality>[*?+1])\s*(?P<right_name>\S+(\s*\S+)?)"
-    )  # noqa: E501
+        r"(?P<left_name>\S+(\s*\S+)?)\s+(?P<left_cardinality>[*?+1])--(?P<right_cardinality>[*?+1])\s*(?P<right_name>\S+(\s*\S+)?)",
+    )
     cardinalities = {"*": "0..N", "?": "{0,1}", "+": "1..N", "1": "1", "": None}
     cardinalities_mermaid = {
         "*": "0..n",
         "?": "0..1",
         "+": "1..n",
     }
+    cardinalities_crowfoot = {
+        "*": "0+",
+        "?": "one or zero",
+        "+": "1+",
+    }
 
     @staticmethod
     def make_from_match(match: re.Match) -> Relation:
         return Relation(
             right_col=match.group("right_name"),
             left_col=match.group("left_name"),
             right_cardinality=match.group("right_cardinality"),
@@ -142,112 +154,122 @@
             )
         self.right_col = right_col
         self.left_col = left_col
         self.right_cardinality = right_cardinality
         self.left_cardinality = left_cardinality
 
     def to_markdown(self) -> str:
-        return "{} {}--{} {}".format(
-            self.left_col,
-            self.left_cardinality,
-            self.right_cardinality,
-            self.right_col,
-        )
+        return f"{self.left_col} {self.left_cardinality}--{self.right_cardinality} {self.right_col}"
 
     def to_mermaid(self) -> str:
         normalized = (
             Relation.cardinalities_mermaid.get(k, k)
             for k in (
-                self.left_col,
+                self.left_col.replace(".", "_"),
                 self.left_cardinality,
                 self.right_cardinality,
-                self.right_col,
+                self.right_col.replace(".", "_"),
             )
         )
         return '{} "{}" -- "{}" {}'.format(*normalized)
 
+    def to_mermaid_er(self) -> str:
+        left = Relation.cardinalities_crowfoot.get(
+            self.left_cardinality,
+            self.left_cardinality,
+        )
+        right = Relation.cardinalities_crowfoot.get(
+            self.right_cardinality,
+            self.right_cardinality,
+        )
+        left_col = self.left_col.replace(".", "_")
+        right_col = self.right_col.replace(".", "_")
+        return f"{left_col} {left}--{right} {right_col} : has"
+
     def graphviz_cardinalities(self, card) -> str:
         if card == "":
             return ""
-        return "label=<<FONT>{}</FONT>>".format(self.cardinalities[card])
+        return f"label=<<FONT>{self.cardinalities[card]}</FONT>>"
 
     def to_dot(self) -> str:
         if self.right_cardinality == self.left_cardinality == "":
             return ""
         cards = []
         if self.left_cardinality != "":
             cards.append("tail" + self.graphviz_cardinalities(self.left_cardinality))
         if self.right_cardinality != "":
             cards.append("head" + self.graphviz_cardinalities(self.right_cardinality))
         return '"{}" -- "{}" [{}];'.format(
             self.left_col, self.right_col, ",".join(cards)
         )
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other: object) -> bool:
         if super().__eq__(other):
             return True
+        if not isinstance(other, Relation):
+            return False
         other_inversed = Relation(
             right_col=other.left_col,
             left_col=other.right_col,
             right_cardinality=other.left_cardinality,
             left_cardinality=other.right_cardinality,
         )
         return other_inversed.__dict__ == self.__dict__
 
 
 class Table(Drawable):
     """Represents a Table in the intermediaty syntax"""
 
-    RE = re.compile("\[(?P<name>[^]]+)\]")
+    RE = re.compile(r"\[(?P<name>[^]]+)\]")
 
     def __init__(self, name: str, columns: list[Column]) -> None:
         self.name = name
         self.columns = columns
 
     @staticmethod
     def make_from_match(match: re.Match) -> Table:
         return Table(name=match.group("name"), columns=[])
 
     @property
     def header_markdown(self) -> str:
-        return "[{}]".format(self.name)
+        return f"[{self.name}]"
 
     def to_markdown(self) -> str:
         return (
             self.header_markdown
             + "\n"
             + "\n".join(c.to_markdown() for c in self.columns)
         )
 
     def to_mermaid(self) -> str:
         columns = [c.to_mermaid() for c in self.columns]
-        return (
-            "class {}{{\n  ".format(self.name)
-            + "\n  ".format(self.name).join(columns)  # type:ignore
-            + "\n}"
-        )
+        name = self.name.replace(".", "_")
+        return f"class {name}{{\n" + "\n  ".join(columns) + "\n}"
+
+    def to_mermaid_er(self) -> str:
+        columns = [c.to_mermaid_er() for c in self.columns]
+        name = self.name.replace(".", "_")
+        return f"{name} {{\n" + "\n  ".join(columns) + "\n}"
 
     @property
     def columns_sorted(self):
         return sorted(self.columns, key=operator.attrgetter("name"))
 
     @property
     def header_dot(self) -> str:
-        return ROW_TAGS.format("", '<B><FONT POINT-SIZE="16">{}</FONT></B>').format(
-            self.name
-        )
+        return ROW_TAGS.format("", f'<B><FONT POINT-SIZE="16">{self.name}</FONT></B>')
 
     def to_dot(self) -> str:
         body = "".join(c.to_dot() for c in self.columns)
         return TABLE.format(self.name, self.header_dot, body)
 
     def __str__(self) -> str:
         return self.header_markdown
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other: object) -> bool:
         if not isinstance(other, Table):
             return False
         if other.name != self.name:
             return False
 
         if self.columns_sorted != other.columns_sorted:
             return False
```

### Comparing `eralchemy2-1.3.8/eralchemy2/parser.py` & `eralchemy2-1.4.0/eralchemy2/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     def traceback(self) -> str:
         rv = self.base_traceback.format(
             line_nb=getattr(self, "line_nb", "?"),
             line=getattr(self, "line", ""),
             error=self.args[0],
         )
         if self.hint is not None:
-            rv += "\nHINT: {}".format(self.hint)
+            rv += f"\nHINT: {self.hint}"
         return rv
 
 
 class DuplicateTableException(ParsingException):
     pass
 
 
@@ -90,16 +90,16 @@
         raise RelationNoColException(msg.format(column_name))
 
 
 def _check_not_creating_duplicates(
     new_name: str, names: list[str], type: str, exc: type[Exception]
 ) -> None:
     if new_name in names:
-        msg = 'Cannot add {} named "{}" which is ' "already present in the schema."
-        raise exc(msg.format(type, new_name))
+        msg = f'Cannot add {type} named "{new_name}" which is already present in the schema.'
+        raise exc(msg)
 
 
 def update_models(
     new_obj, current_table: Table | None, tables: list[Table], relations: list[Relation]
 ) -> tuple[Table | None, list[Table], list[Relation]]:
     """Update the state of the parsing."""
     _update_check_inputs(current_table, tables, relations)
@@ -153,12 +153,10 @@
                 new_obj, current_table, tables, relations
             )
         except ParsingException as e:
             e.line_nb = line_nb  # type:ignore
             e.line = raw_line  # type:ignore
             errors.append(e)
     if len(errors) != 0:
-        msg = "eralchemy2 couldn't complete the generation due the {} following errors".format(
-            len(errors)
-        )
+        msg = f"eralchemy2 couldn't complete the generation due the {len(errors)} following errors"
         raise ParsingException(msg + "\n\n".join(e.traceback for e in errors))
     return tables, relations
```

### Comparing `eralchemy2-1.3.8/eralchemy2/sqla.py` & `eralchemy2-1.4.0/eralchemy2/sqla.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,20 +16,47 @@
 if TYPE_CHECKING:
     from typing_extensions import Protocol
 
     class DeclarativeBase(Protocol):
         metadata: sa.MetaData
 
 
+def check_all_compound_same_parent(fk: sa.ForeignKey):
+    """Checks if all other ForeignKey Constraints of our table are on the same parent table as the current one"""
+    table = fk.column.table.fullname
+    if not fk.constraint:
+        return True
+    for col in fk.constraint.table.columns:
+        if not col.foreign_keys:
+            return False
+        for foreign_column in col.foreign_keys:
+            if table != foreign_column.column.table.fullname:
+                return False
+    return True
+
+
 def relation_to_intermediary(fk: sa.ForeignKey) -> Relation:
-    """Transform an SQLAlchemy ForeignKey object to it's intermediary representation."""
+    """Transform an SQLAlchemy ForeignKey object to its intermediary representation."""
+
+    primkey_count = 0
+    if fk.constraint:
+        primkey_count = sum(
+            [True for x in fk.constraint.table.columns if x.primary_key]
+        )
+    # when there is only a single primary key column of the current key
+    if (primkey_count == 1 and fk.parent.primary_key) or fk.parent.unique:
+        right_cardinality = "1"
+    else:
+        # check if the other primkeys have a foreign key onto the same table
+        # if this is the case, we are not optional and must be unique
+        right_cardinality = "1" if check_all_compound_same_parent(fk) else "*"
     return Relation(
         right_col=format_name(fk.parent.table.fullname),
-        left_col=format_name(fk._column_tokens[1]),
-        right_cardinality="1" if fk.parent.primary_key or fk.parent.unique else "*",
+        left_col=format_name(fk.column.table.fullname),
+        right_cardinality=right_cardinality,
         left_cardinality="?" if fk.parent.nullable else "1",
     )
 
 
 def format_type(typ: Any) -> str:
     """Transforms the type into a nice string representation."""
     try:
@@ -97,15 +124,24 @@
 def database_to_intermediary(
     database_uri: str, schema: str | None = None
 ) -> tuple[list[Table], list[Relation]]:
     """Introspect from the database (given the database_uri) to create the intermediary representation."""
     Base = automap_base()
     engine = create_engine(database_uri)
     if schema is not None:
-        Base.metadata.schema = schema
+        schemas = schema.split(",")
+        for schema in schemas:
+            schema = schema.strip()
+            # reflect the tables
+            Base.metadata.schema = schema
+            Base.prepare(
+                engine,
+                name_for_scalar_relationship=name_for_scalar_relationship,
+            )
+    else:
+        # reflect the tables
+        Base.prepare(
+            engine,
+            name_for_scalar_relationship=name_for_scalar_relationship,
+        )
 
-    # reflect the tables
-    Base.prepare(
-        engine,
-        name_for_scalar_relationship=name_for_scalar_relationship,
-    )
     return declarative_to_intermediary(Base)
```

### Comparing `eralchemy2-1.3.8/pyproject.toml` & `eralchemy2-1.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,88 +1,77 @@
-[tool.poetry]
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+
+[project]
 name = "eralchemy2"
-version = "1.3.8"
+version = "1.4.0"
 description = "Simple entity relation (ER) diagrams generation"
-authors = ["Florian Maurer <fmaurer@disroot.org>"]
-license = "Apache License 2.0"
+authors = [{ name = "Florian Maurer", email = "fmaurer@disroot.org"}]
+license = {text = "Apache-2.0"}
 readme = "README.md"
 
-homepage = "https://github.com/maurerle/eralchemy2"
-repository = "https://github.com/maurerle/eralchemy2"
-
 keywords = ["sql", "ORM", "relational databases", "ER diagram", "render"]
 
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
-    "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Visualization",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Database",
 ]
+requires-python = ">=3.8"
+dependencies = [
+  "sqlalchemy >= 1.4",
+  "pygraphviz >= 1.9",
+]
 
-[tool.poetry.dependencies]
-python = "^3.7"
-sqlalchemy = ">=1.4"
-pygraphviz = "^1.7,!=1.8"
-flask-sqlalchemy = {version = ">=2.5.1", optional = true}
-psycopg2 = {version = "^2.9.3", optional = true}
-importlib_metadata = { version = ">=4.0.0", markers = "python_version < '3.8'" }
-
-[tool.poetry.group.dev.dependencies]
-black = "^22.8.0"
-tox = "^4.4.6"
-isort = "^5.10.1"
-towncrier = "^22.8.0"
-mypy  = "^0.971"
+[project.urls]
+homepage = "https://github.com/maurerle/eralchemy2"
+repository = "https://github.com/maurerle/eralchemy2"
 
-[tool.poetry.extras]
-    ci = ["flask-sqlalchemy", "psycopg2"]
+[project.optional-dependencies]
+ci = [
+  "flask-sqlalchemy >= 2.5.1",
+  "psycopg2 >= 2.9.3",
+  "pytest >= 7.4.3",
+]
+test = [
+  "isort>=5.12",
+  "mypy>=1.7.0",
+]
 
-[tool.poetry.scripts]
+[project.scripts]
 eralchemy2 = "eralchemy2.main:cli"
 
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
-
-[tool.flake8]
-max-line-length = 120
-
-[tool.isort]
-profile = "black"
-add_imports = ["from __future__ import annotations"]
-
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 isolated_build = True
-envlist = py37, py38, py39, py310, py310-SA20, py311, py311-SA20, py312
+envlist = py38, py39, py310, py310-SA20, py311, py311-SA20, py312
 
 [tox:.package]
 # note tox will use the same python version as under what tox is installed to package
 # so unless this is python 3 you can require a given python version for the packaging
 # environment via the basepython key
 basepython = python3
 
 [gh-actions]
 python =
-    3.7: py37
     3.8: py38
     3.9: py39
     3.10: py310, py310-SA14, py310-SA20
     3.11: py311, py311-SA14, py311-SA20
     3.12: py312
 
 [testenv]
 extras = ci
 deps =
-  pytest
   py310-SA20: sqlalchemy~=2.0.4
   py311-SA20: sqlalchemy~=2.0.4
 commands =
   pytest
 """
 
 [tool.pytest]
@@ -106,7 +95,25 @@
 show_column_numbers = true
 show_error_codes = true
 pretty = true
 
 [[tool.mypy.overrides]]
 module = ["pygraphviz.*", "sqlalchemy.*"]
 ignore_missing_imports = true
+
+
+[tool.ruff]
+include = ["eralchemy2/**/*.py", "tests/**/*.py"]
+
+[tool.ruff.lint]
+select = ["E", "F", "I"]
+ignore = ["E501"]
+
+[tool.ruff.lint.per-file-ignores]
+"__init__.py" = [
+    "I001", # allow unsorted imports in __init__.py
+    "F401", # allow unused imports in __init__.py
+]
+"tests/*" = [
+    "S101", # allow assert statements for pytest
+    "ARG",  # allow unused arguments for pytest fixtures
+]
```

### Comparing `eralchemy2-1.3.8/PKG-INFO` & `eralchemy2-1.4.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 Metadata-Version: 2.1
 Name: eralchemy2
-Version: 1.3.8
+Version: 1.4.0
 Summary: Simple entity relation (ER) diagrams generation
-Home-page: https://github.com/maurerle/eralchemy2
+Author-email: Florian Maurer <fmaurer@disroot.org>
 License: Apache-2.0
+Project-URL: homepage, https://github.com/maurerle/eralchemy2
+Project-URL: repository, https://github.com/maurerle/eralchemy2
 Keywords: sql,ORM,relational databases,ER diagram,render
-Author: Florian Maurer
-Author-email: fmaurer@disroot.org
-Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Provides-Extra: ci
-Requires-Dist: flask-sqlalchemy (>=2.5.1) ; extra == "ci"
-Requires-Dist: importlib_metadata (>=4.0.0) ; python_version < "3.8"
-Requires-Dist: psycopg2 (>=2.9.3,<3.0.0) ; extra == "ci"
-Requires-Dist: pygraphviz (>=1.7,<2.0,!=1.8)
-Requires-Dist: sqlalchemy (>=1.4)
-Project-URL: Repository, https://github.com/maurerle/eralchemy2
+Classifier: Topic :: Database
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: sqlalchemy>=1.4
+Requires-Dist: pygraphviz>=1.9
+Provides-Extra: ci
+Requires-Dist: flask-sqlalchemy>=2.5.1; extra == "ci"
+Requires-Dist: psycopg2>=2.9.3; extra == "ci"
+Requires-Dist: pytest>=7.4.3; extra == "ci"
+Provides-Extra: test
+Requires-Dist: isort>=5.12; extra == "test"
+Requires-Dist: mypy>=1.7.0; extra == "test"
 
 
 [![PyPI Version](https://img.shields.io/pypi/v/eralchemy2.svg)](
 https://pypi.org/project/eralchemy2/)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/eralchemy2.svg)](
 https://pypi.org/project/eralchemy2/)
 ![Github Actions](https://github.com/maurerle/eralchemy2/actions/workflows/python-app.yml/badge.svg)
@@ -54,21 +50,33 @@
 ### Install
 To install eralchemy2, just do:
 
     $ pip install eralchemy2
 
 `eralchemy2` requires [GraphViz](http://www.graphviz.org/download) to generate the graphs and Python. Both are available for Windows, Mac and Linux.
 
+For Debian based systems, run:
+
+    $ apt install graphviz libgraphviz-dev
+
+before installing eralchemy2.
+
+### Install using conda
+
+There is also a packaged version in conda-forge, which directly installs the dependencies:
+
+    $ conda install -c conda-forge eralchemy2
+
 ### Usage from Command Line
 
 #### From a database
 
     $ eralchemy2 -i sqlite:///relative/path/to/db.db -o erd_from_sqlite.pdf
 
-The database is specified as a [SQLAlchemy](http://docs.sqlalchemy.org/en/rel_1_0/core/engines.html#database-urls)
+The database is specified as a [SQLAlchemy](https://docs.sqlalchemy.org/en/20/core/engines.html#database-urls)
 database url.
 
 #### From a markdown file.
 
     $ curl 'https://raw.githubusercontent.com/maurerle/eralchemy2/main/example/newsmeme.er' > markdown_file.er
     $ eralchemy2 -i 'markdown_file.er' -o erd_from_markdown_file.pdf
 
@@ -76,17 +84,21 @@
 
     $ eralchemy2 -i 'postgresql+psycopg2://username:password@hostname:5432/databasename' -o filtered.er --exclude-tables temp audit
 
 #### From a Postgresql DB to a markdown file excluding columns named `created_at` and `updated_at` from all tables
 
     $ eralchemy2 -i 'postgresql+psycopg2://username:password@hostname:5432/databasename' -o filtered.er --exclude-columns created_at updated_at
 
-#### From a Postgresql DB to a markdown file for the schema `schema`
+#### From a Postgresql DB to a markdown file for the schemas `schema1` and `schema2`
+
+    $ eralchemy2 -i 'postgresql+psycopg2://username:password@hostname:5432/databasename' -s "schema1, schema2"
+
+#### Specify Output Mode
 
-    $ eralchemy2 -i 'postgresql+psycopg2://username:password@hostname:5432/databasename' -s schema
+    $ eralchemy2 -i 'markdown_file.er' -o erd_from_markdown_file.md -m mermaid_er
 
 ### Usage from Python
 
 ```python
 from eralchemy2 import render_er
 ## Draw from SQLAlchemy base
 render_er(Base, 'erd_from_sqlalchemy.png')
@@ -107,19 +119,22 @@
 To run the tests, use : `$ py.test` or `$ tox`.
 Some tests require a local postgres database with a schema named test in a database
 named test all owned by a user named eralchemy with a password of eralchemy.
 This can be easily set up using docker-compose with: `docker-compose up -d`.
 
 All tested PR are welcome.
 
+## Publishing a release
+
+    $ rm -r dist && python -m build && python3 -m twine upload --repository pypi dist/*
+
 ## Notes
 
 eralchemy2 is a fork of its predecessor [ERAlchemy](https://github.com/Alexis-benoist/eralchemy) by @Alexis-benoist, which is not maintained anymore and does not work with SQLAlchemy > 1.4.
 If it is maintained again, I'd like to push the integrated changes upstream.
 
 ERAlchemy was inspired by [erd](https://github.com/BurntSushi/erd), though it is able to render the ER diagram directly
 from the database and not just only from the `ER` markup language.
 
 Released under an Apache License 2.0
 
-Initial Creator: Alexis Benoist [Alexis_Benoist](https://twitter.com/Alexis_Benoist)
-
+Initial Creator: Alexis Benoist [Alexis_Benoist](https://github.com/Alexis-benoist)
```

