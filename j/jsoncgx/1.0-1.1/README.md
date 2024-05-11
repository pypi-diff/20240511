# Comparing `tmp/jsoncgx-1.0.tar.gz` & `tmp/jsoncgx-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsoncgx-1.0.tar", last modified: Fri May 10 20:22:16 2024, max compression
+gzip compressed data, was "jsoncgx-1.1.tar", last modified: Sat May 11 17:43:51 2024, max compression
```

## Comparing `jsoncgx-1.0.tar` & `jsoncgx-1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:22:16.551943 jsoncgx-1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-10 20:22:07.000000 jsoncgx-1.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-05-10 20:22:16.551943 jsoncgx-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-10 20:22:07.000000 jsoncgx-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:22:16.551943 jsoncgx-1.0/jsoncgx/
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-10 20:22:07.000000 jsoncgx-1.0/jsoncgx/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12702 2024-05-10 20:22:07.000000 jsoncgx-1.0/jsoncgx/abstract.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10085 2024-05-10 20:22:07.000000 jsoncgx-1.0/jsoncgx/lexer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22940 2024-05-10 20:22:07.000000 jsoncgx-1.0/jsoncgx/parser.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    60788 2024-05-10 20:22:07.000000 jsoncgx-1.0/jsoncgx/rexel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:22:16.551943 jsoncgx-1.0/jsoncgx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-05-10 20:22:16.000000 jsoncgx-1.0/jsoncgx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-10 20:22:16.000000 jsoncgx-1.0/jsoncgx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 20:22:16.000000 jsoncgx-1.0/jsoncgx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 20:22:16.000000 jsoncgx-1.0/jsoncgx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-10 20:22:07.000000 jsoncgx-1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 20:22:16.551943 jsoncgx-1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:43:51.341149 jsoncgx-1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-11 17:43:47.000000 jsoncgx-1.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-05-11 17:43:51.341149 jsoncgx-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-11 17:43:47.000000 jsoncgx-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:43:51.341149 jsoncgx-1.1/jsoncgx/
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-11 17:43:47.000000 jsoncgx-1.1/jsoncgx/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12951 2024-05-11 17:43:47.000000 jsoncgx-1.1/jsoncgx/abstract.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10085 2024-05-11 17:43:47.000000 jsoncgx-1.1/jsoncgx/lexer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22940 2024-05-11 17:43:47.000000 jsoncgx-1.1/jsoncgx/parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    61663 2024-05-11 17:43:47.000000 jsoncgx-1.1/jsoncgx/rexel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:43:51.341149 jsoncgx-1.1/jsoncgx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-05-11 17:43:51.000000 jsoncgx-1.1/jsoncgx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-11 17:43:51.000000 jsoncgx-1.1/jsoncgx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 17:43:51.000000 jsoncgx-1.1/jsoncgx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-11 17:43:51.000000 jsoncgx-1.1/jsoncgx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-11 17:43:47.000000 jsoncgx-1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 17:43:51.341149 jsoncgx-1.1/setup.cfg
```

### Comparing `jsoncgx-1.0/LICENCE` & `jsoncgx-1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `jsoncgx-1.0/PKG-INFO` & `jsoncgx-1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsoncgx
-Version: 1.0
+Version: 1.1
 Summary: An overpowered JSON-with-comments parser with inplace edition
 Author-email: cigix <cigix@cigix.me>
 Project-URL: Repository, https://github.com/cigix/jsoncgx
 Project-URL: Issues, https://github.com/cigix/jsoncgx/issues
 Keywords: json,jsonc,json with comments,json editor
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -68,15 +68,15 @@
 </td>
 <td>
 
 ```python
 
 >>> import jsoncgx
 >>> editor = jsoncgx.loads('{ "answer": 42 }')
->>> editor.root["answer"][0].value()
+>>> editor.root["answer"][0]
 42
 ```
 
 </td>
    </tr>
    <tr>
       <td>Editing JSON data</td>
@@ -88,16 +88,15 @@
 '{"answer": "spam"}'
 ```
 
 </td>
 <td>
 
 ```python
->>> editor.root.editreplacevalue(0,
-...     jsoncgx.JSONString.create("spam"))
+>>> editor.root.editreplacevalue(0, "spam")
 >>> editor.dumps()
 '{ "answer": "spam" }'
 ```
 
 </td>
    </tr>
    <tr>
@@ -136,17 +135,17 @@
 
 </td>
 <td>
 
 ```python
 >>> editor = jsoncgx.loads(
 ...     '{ "answer": 42, "answer": "spam" }')
->>> editor.root["answer"][0].value()
+>>> editor.root["answer"][0]
 42
->>> editor.root["answer"][1].value()
+>>> editor.root["answer"][1]
 'spam'
 ```
 
 </td>
    </tr>
    <tr>
       <td>Comments</td>
@@ -162,16 +161,15 @@
 
 </td>
 <td>
 
 ```python
 >>> editor = jsoncgx.loads(
 ...     '{ "answer": /* eggs and */ 42 }')
->>> editor.root.editreplacevalue(0,
-...     jsoncgx.JSONString.create("spam"))
+>>> editor.root.editreplacevalue(0, "spam")
 >>> editor.dumps()
 '{ "answer": /* eggs and */ "spam" }'
 ```
 
 </td>
    </tr>
 </table>
@@ -193,7 +191,16 @@
   * U+002F.
 
 Those elements are considered like whitespace.
 
 ## Architecture
 
 ![jsoncgx architecture](architecture.png)
+
+## Changelog
+
+### V1.1:
+
+* `JSONNumber`, `JSONString`, `JSONBool`, and `JSONNull` have been replaced with
+  `JSONBuiltin`, for easier integration.
+* `edit*()` methods that accepted `JSONValue` now also accept `int`, `float`,
+  `str`, `bool`, and `None`. They are automatically turned into `JSONBuiltin`.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jsoncgx Version: 1.0 Summary: An overpowered JSON-
+Metadata-Version: 2.1 Name: jsoncgx Version: 1.1 Summary: An overpowered JSON-
 with-comments parser with inplace edition Author-email: cigix
 cigix.me> Project-URL: Repository, https://github.com/cigix/jsoncgx Project-
 URL: Issues, https://github.com/cigix/jsoncgx/issues Keywords: json,jsonc,json
 with comments,json editor Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: OSI Approved :: GNU General Public License v3 or
 later (GPLv3+) Classifier: Programming Language :: Python :: 3 Classifier:
 Topic :: File Formats :: JSON Classifier: Typing :: Typed Requires-Python:
@@ -22,47 +22,48 @@
 indentation, and serialisation reproduces it. ## Installation This library is
 [available on PyPI](https://pypi.org/project/jsoncgx/): ``` pip install --user
 jsoncgx ``` ## Comparison / Quickstart / Demo
                   SSttaannddaarrdd PPyytthhoonn mmoodduullee        ``jjssoonnccggxx``
                   ```python >>> import json >>> ```python >>> import jsoncgx
                   data = json.loads('           >>> editor = jsoncgx.loads('
 Loading JSON data { "answer": 42 }') >>> data   { "answer": 42 }') >>>
-                  ["answer"] 42 ```             editor.root["answer"]
-                                                [0].value() 42 ```
+                  ["answer"] 42 ```             editor.root["answer"][0] 42
+                                                ```
                                                 ```python >>>
                   ```python >>> data["answer"]  editor.root.editreplacevalue
-Editing JSON data = "spam" >>> json.dumps(data) (0, ...
-                  '{"answer": "spam"}' ```      jsoncgx.JSONString.create
-                                                ("spam")) >>> editor.dumps()
-                                                '{ "answer": "spam" }' ```
+Editing JSON data = "spam" >>> json.dumps(data) (0, "spam") >>> editor.dumps
+                  '{"answer": "spam"}' ```      () '{ "answer": "spam" }'
+                                                ```
                   ```python >>> with open       ```python >>> editor =
                   ("in.json") as f: ... data =  json.loadf("in.json") >>>
 Working with JSON json.load(f) ... >>> with     editor.dumpf("out.json") ```
 files             open("out.json", "w") as f:   Or use `jsoncgx.load()` and
                   ... json.dump(data, f) ...    `jsoncgx.JSONEditor.dump()`
                   ```                           with a file handle, like the
                                                 standard module.
                                                 ```python >>> editor =
                   ```python >>> data =          jsoncgx.loads( ... '
                   json.loads( ... '{ "answer":  { "answer": 42, "answer":
 Non unique name   42, "answer": "spam" }') >>>  "spam" }') >>> editor.root
-                  data["answer"] 'spam' ```     ["answer"][0].value() 42 >>>
-                                                editor.root["answer"]
-                                                [1].value() 'spam' ```
-                                                ```python >>> editor =
-                  ```python >>> data =          jsoncgx.loads( ... '
-                  json.loads( ... '{ "answer":  { "answer": /* eggs and */
-                  /* eggs and */ 42 }')         42 }') >>>
-Comments          Traceback (most recent call   editor.root.editreplacevalue
-                  last): ...                    (0, ...
-                  json.decoder.JSONDecodeError: jsoncgx.JSONString.create
-                  ... ```                       ("spam")) >>> editor.dumps()
-                                                '{ "answer": /* eggs and */
-                                                "spam" }' ```
+                  data["answer"] 'spam' ```     ["answer"][0] 42 >>>
+                                                editor.root["answer"][1]
+                                                'spam' ```
+                  ```python >>> data =          ```python >>> editor =
+                  json.loads( ... '{ "answer":  jsoncgx.loads( ... '
+                  /* eggs and */ 42 }')         { "answer": /* eggs and */
+Comments          Traceback (most recent call   42 }') >>>
+                  last): ...                    editor.root.editreplacevalue
+                  json.decoder.JSONDecodeError: (0, "spam") >>> editor.dumps
+                  ... ```                       () '{ "answer": /* eggs and
+                                                */ "spam" }' ```
 ## What syntax does this parse exactly? [ECMA-404](https://ecma-
 international.org/wp-content/uploads/ECMA-404_2nd_edition_december_2017.pdf)
 with the following additional lexical elements: * regex `//[^\n]*\n`, that is,
 the Unicode scalar sequence: * U+002F, * U+002F, * any amount of any scalars
 except U+000A, * U+000A. * lazy regex `/\*.*\*/`, that is, the Unicode scalar
 sequence: * U+002F, * U+002A, * any amount of any scalars except the sequence
 U+002A U+002F * U+002A, * U+002F. Those elements are considered like
-whitespace. ## Architecture ![jsoncgx architecture](architecture.png)
+whitespace. ## Architecture ![jsoncgx architecture](architecture.png) ##
+Changelog ### V1.1: * `JSONNumber`, `JSONString`, `JSONBool`, and `JSONNull`
+have been replaced with `JSONBuiltin`, for easier integration. * `edit*()`
+methods that accepted `JSONValue` now also accept `int`, `float`, `str`,
+`bool`, and `None`. They are automatically turned into `JSONBuiltin`.
```

### Comparing `jsoncgx-1.0/README.md` & `jsoncgx-1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 </td>
 <td>
 
 ```python
 
 >>> import jsoncgx
 >>> editor = jsoncgx.loads('{ "answer": 42 }')
->>> editor.root["answer"][0].value()
+>>> editor.root["answer"][0]
 42
 ```
 
 </td>
    </tr>
    <tr>
       <td>Editing JSON data</td>
@@ -71,16 +71,15 @@
 '{"answer": "spam"}'
 ```
 
 </td>
 <td>
 
 ```python
->>> editor.root.editreplacevalue(0,
-...     jsoncgx.JSONString.create("spam"))
+>>> editor.root.editreplacevalue(0, "spam")
 >>> editor.dumps()
 '{ "answer": "spam" }'
 ```
 
 </td>
    </tr>
    <tr>
@@ -119,17 +118,17 @@
 
 </td>
 <td>
 
 ```python
 >>> editor = jsoncgx.loads(
 ...     '{ "answer": 42, "answer": "spam" }')
->>> editor.root["answer"][0].value()
+>>> editor.root["answer"][0]
 42
->>> editor.root["answer"][1].value()
+>>> editor.root["answer"][1]
 'spam'
 ```
 
 </td>
    </tr>
    <tr>
       <td>Comments</td>
@@ -145,16 +144,15 @@
 
 </td>
 <td>
 
 ```python
 >>> editor = jsoncgx.loads(
 ...     '{ "answer": /* eggs and */ 42 }')
->>> editor.root.editreplacevalue(0,
-...     jsoncgx.JSONString.create("spam"))
+>>> editor.root.editreplacevalue(0, "spam")
 >>> editor.dumps()
 '{ "answer": /* eggs and */ "spam" }'
 ```
 
 </td>
    </tr>
 </table>
@@ -176,7 +174,16 @@
   * U+002F.
 
 Those elements are considered like whitespace.
 
 ## Architecture
 
 ![jsoncgx architecture](architecture.png)
+
+## Changelog
+
+### V1.1:
+
+* `JSONNumber`, `JSONString`, `JSONBool`, and `JSONNull` have been replaced with
+  `JSONBuiltin`, for easier integration.
+* `edit*()` methods that accepted `JSONValue` now also accept `int`, `float`,
+  `str`, `bool`, and `None`. They are automatically turned into `JSONBuiltin`.
```

#### html2text {}

```diff
@@ -13,47 +13,48 @@
 about the indentation, and serialisation reproduces it. ## Installation This
 library is [available on PyPI](https://pypi.org/project/jsoncgx/): ``` pip
 install --user jsoncgx ``` ## Comparison / Quickstart / Demo
                   SSttaannddaarrdd PPyytthhoonn mmoodduullee        ``jjssoonnccggxx``
                   ```python >>> import json >>> ```python >>> import jsoncgx
                   data = json.loads('           >>> editor = jsoncgx.loads('
 Loading JSON data { "answer": 42 }') >>> data   { "answer": 42 }') >>>
-                  ["answer"] 42 ```             editor.root["answer"]
-                                                [0].value() 42 ```
+                  ["answer"] 42 ```             editor.root["answer"][0] 42
+                                                ```
                                                 ```python >>>
                   ```python >>> data["answer"]  editor.root.editreplacevalue
-Editing JSON data = "spam" >>> json.dumps(data) (0, ...
-                  '{"answer": "spam"}' ```      jsoncgx.JSONString.create
-                                                ("spam")) >>> editor.dumps()
-                                                '{ "answer": "spam" }' ```
+Editing JSON data = "spam" >>> json.dumps(data) (0, "spam") >>> editor.dumps
+                  '{"answer": "spam"}' ```      () '{ "answer": "spam" }'
+                                                ```
                   ```python >>> with open       ```python >>> editor =
                   ("in.json") as f: ... data =  json.loadf("in.json") >>>
 Working with JSON json.load(f) ... >>> with     editor.dumpf("out.json") ```
 files             open("out.json", "w") as f:   Or use `jsoncgx.load()` and
                   ... json.dump(data, f) ...    `jsoncgx.JSONEditor.dump()`
                   ```                           with a file handle, like the
                                                 standard module.
                                                 ```python >>> editor =
                   ```python >>> data =          jsoncgx.loads( ... '
                   json.loads( ... '{ "answer":  { "answer": 42, "answer":
 Non unique name   42, "answer": "spam" }') >>>  "spam" }') >>> editor.root
-                  data["answer"] 'spam' ```     ["answer"][0].value() 42 >>>
-                                                editor.root["answer"]
-                                                [1].value() 'spam' ```
-                                                ```python >>> editor =
-                  ```python >>> data =          jsoncgx.loads( ... '
-                  json.loads( ... '{ "answer":  { "answer": /* eggs and */
-                  /* eggs and */ 42 }')         42 }') >>>
-Comments          Traceback (most recent call   editor.root.editreplacevalue
-                  last): ...                    (0, ...
-                  json.decoder.JSONDecodeError: jsoncgx.JSONString.create
-                  ... ```                       ("spam")) >>> editor.dumps()
-                                                '{ "answer": /* eggs and */
-                                                "spam" }' ```
+                  data["answer"] 'spam' ```     ["answer"][0] 42 >>>
+                                                editor.root["answer"][1]
+                                                'spam' ```
+                  ```python >>> data =          ```python >>> editor =
+                  json.loads( ... '{ "answer":  jsoncgx.loads( ... '
+                  /* eggs and */ 42 }')         { "answer": /* eggs and */
+Comments          Traceback (most recent call   42 }') >>>
+                  last): ...                    editor.root.editreplacevalue
+                  json.decoder.JSONDecodeError: (0, "spam") >>> editor.dumps
+                  ... ```                       () '{ "answer": /* eggs and
+                                                */ "spam" }' ```
 ## What syntax does this parse exactly? [ECMA-404](https://ecma-
 international.org/wp-content/uploads/ECMA-404_2nd_edition_december_2017.pdf)
 with the following additional lexical elements: * regex `//[^\n]*\n`, that is,
 the Unicode scalar sequence: * U+002F, * U+002F, * any amount of any scalars
 except U+000A, * U+000A. * lazy regex `/\*.*\*/`, that is, the Unicode scalar
 sequence: * U+002F, * U+002A, * any amount of any scalars except the sequence
 U+002A U+002F * U+002A, * U+002F. Those elements are considered like
-whitespace. ## Architecture ![jsoncgx architecture](architecture.png)
+whitespace. ## Architecture ![jsoncgx architecture](architecture.png) ##
+Changelog ### V1.1: * `JSONNumber`, `JSONString`, `JSONBool`, and `JSONNull`
+have been replaced with `JSONBuiltin`, for easier integration. * `edit*()`
+methods that accepted `JSONValue` now also accept `int`, `float`, `str`,
+`bool`, and `None`. They are automatically turned into `JSONBuiltin`.
```

### Comparing `jsoncgx-1.0/jsoncgx/__init__.py` & `jsoncgx-1.1/jsoncgx/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   - loadf(path): Parse a JSONC file.
   - loads(s): Parse a JSONC string.
 
 Re-exported classes:
   - lexer.JSONCString: A string containing JSONC data
   - lexer.LexCeption: An exception type for lexing issues
   - parser.ParseXception: An exception type for parsing issues
-  - rexel.JSONNumber, JSONString, JSONBool, JSONNull: JSON values
+  - rexel.JSONBuiltin: JSON values for numbers, strings, booleans, and null
   - rexel.JSONArray, JSONObject, JSONEditor: Editable JSON containers
 
 Re-exported functions:
   - abstract.abstract(cst): Turn a CST into an AST.
   - lexer.lex(origin): Lex JSONC data.
   - parser.parse(tokens): Parse a list of tokens into a CST.
 """
@@ -21,23 +21,21 @@
 from os import PathLike
 from typing import TYPE_CHECKING, IO, Optional
 
 try:
     from .lexer import JSONCString, lex, LexCeption
     from .parser import parse, ParseXception
     from .abstract import abstract
-    from .rexel import (JSONNumber, JSONString, JSONBool, JSONNull, JSONArray,
-                        JSONObject, JSONEditor)
+    from .rexel import JSONBuiltin, JSONArray, JSONObject, JSONEditor
 except ImportError:
     if not TYPE_CHECKING:
         from lexer import JSONCString, lex, LexCeption
         from parser import parse, ParseXception
         from abstract import abstract
-        from rexel import (JSONNumber, JSONString, JSONBool, JSONNull,
-                           JSONArray, JSONObject, JSONEditor)
+        from rexel import JSONBuiltin, JSONArray, JSONObject, JSONEditor
 
 def loads(s: str | bytes, name: Optional[str] =None,
           allow_comments: Optional[bool] =True) -> JSONEditor:
     """loads(s, name=None, allow_comments=True): Parse a JSONC string.
 
     Args:
       - s: str or bytes, the JSONC contents to parse
```

### Comparing `jsoncgx-1.0/jsoncgx/abstract.py` & `jsoncgx-1.1/jsoncgx/abstract.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,31 +76,42 @@
         raise NotImplementedError()
 
 
 class ANodeNumber(ANodeLeaf):
     """ANodeNumber: An AST node for a JSON number.
 
     Methods:
-      - float(ANodeNumber): alias for float(str(token))
+      - float(ANodeNumber): Get the value.
+      - int(ANodeNumber): Get the value.
 
-      - value(): alias for float(ANodeNumber)
+      - value(): Get the value.
     """
     def __init__(self, nodenumber: CNodeNumberValue):
         """ANodeNumber(nodenumber)
 
         Args:
           - nodenumber: CNodeNumberValue, the concrete number node
         """
         super().__init__(nodenumber.number.start())
 
     def __float__(self) -> float:
         return float(str(self))
 
-    def value(self) -> float:
-        return float(self)
+    def __int__(self) -> int:
+        return int(str(self))
+
+    def value(self) -> int | float:
+        """value(): Get the value.
+
+        Return: int or float, the value.
+        """
+        try:
+            return int(self)
+        except ValueError:
+            return float(self)
 
     def tographviz(self) -> str:
         return f'  "{id(self)}" [label="{str(self)}" shape=box];\n'
 
 
 class ANodeString(ANodeLeaf):
     """ANodeString: An AST node for a JSON string.
@@ -113,15 +124,15 @@
 
         Args:
           - nodestring: CNodeStringValue, the concrete string node
         """
         super().__init__(nodestring.string.start())
 
     def value(self) -> str:
-        return str(self)
+        return str(self)[1:-1]
 
     def tographviz(self) -> str:
         return f'  "{id(self)}" [label=<{str(self)}> shape=box];\n'
 
 
 class ANodeBool(ANodeLeaf):
     """ANodeBool: An AST node for a JSON bool.
```

### Comparing `jsoncgx-1.0/jsoncgx/lexer.py` & `jsoncgx-1.1/jsoncgx/lexer.py`

 * *Files identical despite different names*

### Comparing `jsoncgx-1.0/jsoncgx/parser.py` & `jsoncgx-1.1/jsoncgx/parser.py`

 * *Files identical despite different names*

### Comparing `jsoncgx-1.0/jsoncgx/rexel.py` & `jsoncgx-1.1/jsoncgx/rexel.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
   - JSONValue and subclasses: Objects representing JSON values
 """
 
 from __future__ import annotations
 
 import random # for FragmentList.tohtml()
 from os import PathLike
-from typing import TYPE_CHECKING, Any, IO, Iterable, cast
+from typing import TYPE_CHECKING, Any, IO, Iterable, NamedTuple, TypeAlias, cast
 
 try:
     from .lexer import JSONCString, Token
     from .abstract import (ANodeValue, ANodeNumber, ANodeString, ANodeBool,
                            ANodeNull, ANodeArray, ANodeObject, AST)
 except ImportError:
     if not TYPE_CHECKING:
@@ -400,34 +400,30 @@
         if self & newfragments:
             raise ValueError("Fragment is already present in list")
         start = self._fragments.index(startoldfragment)
         end = self._fragments.index(endoldfragment)
         self._fragments[start:end + 1] = newfragments
 
 
+BuiltinType: TypeAlias = int | float | str | bool | None
+
 class JSONValue:
     """JSONValue: A JSON value.
 
-    Class methods:
-      - create(...): Create a new instance of the value.
+    This is an abstract type; see implementations:
+      - JSONBuiltin
+      - JSONArray
+      - JSONObject
 
     Methods:
       - start(): Get the first fragment of the value.
       - end(): Get the last fragment of the value.
       - fragments(): Get the list of fragments of the value.
-      - tographviz(): Get a Graphviz representation of the subtree.
+      - tographviz(): Get a Graphviz representation of the value.
     """
-    @classmethod
-    def create(_, *__): # type: ignore
-        """create(...): Create a new instance of the value.
-
-        Subclasses must override this method.
-        """
-        raise NotImplementedError()
-
     def start(_) -> Fragment:
         """start(): Get the first fragment of the value.
 
         Return: Fragment, the first fragment of the value
 
         Note that this fragment may not be part of any FragmentList.
         """
@@ -444,224 +440,135 @@
 
     def fragments(_) -> list[Fragment]:
         """fragments(): Get the list of fragments of the value.
 
         Return: list of Fragment, the fragments of the value
 
         Note that this list may not be part of any FragmentList, and does not
-        include any FragmentFiller
+        include any FragmentFiller.
         """
         raise NotImplementedError()
 
     def tographviz(_) -> str:
         """tographviz(): Get a Graphviz representation of the subtree.
 
         Return: str, a Graphviz representation of the subtree
         """
         raise NotImplementedError()
 
 
-class JSONEditable:
-    """JSONEditable: An editable JSON container.
-
-    All JSONEditable are associated with a FragmentList with which they sync all
-    insertions, deletions, and replacements within the container.
-    """
-    # Private attributes:
-    #   - _fragmentlist: FragmentList, the list associated with the container
-    _fragmentlist: FragmentList
+class JSONBuiltin(JSONValue):
+    """JSONBuiltin: A non-container JSON value.
 
-    def __init__(self, fragmentlist: FragmentList):
-        """JSONEditable(fragmentlist)
-
-        Args:
-          - fragmentlist: FragmentList, the list to associate with this
-            container
-        """
-        self._fragmentlist = fragmentlist
-
-
-class JSONLeafValue(JSONValue):
-    """JSONLeafValue: A non-container JSON value.
-
-    These values have no children, they are leaves of the AST.
+    JSONBuiltin are a Python built-in type value, associated with a Fragment.
+    They do not support edition; turn to a JSONContainer for that.
 
     Attributes:
-      - fragment: Fragment, the fragment of this leaf
+      - value: int, float, str, bool, or None, the value
+      - fragment: Fragment, the fragment
 
-    Method:
-      - value(): Get the value.
+    Class methods:
+      - create(value): Create a new JSONBuiltin.
     """
+    value: BuiltinType
     fragment: Fragment
 
-    def __init__(self, fragment: Fragment):
-        """JSONLeafValue(fragment)
+    def __init__(self, value: BuiltinType, fragment: Fragment):
+        """JSONBuiltin(value, fragment)
 
         Args:
-          - fragment: Fragment, the fragment of this leaf
+          - value: int, float, str, bool, or None, the value
+          - fragment: Fragment, the fragment
         """
+        self.value = value
         self.fragment = fragment
 
+    @classmethod
+    def create(cls, value: BuiltinType) -> JSONBuiltin:
+        """JSONBuiltin.create(value): Create a new JSONBuiltin.
+
+        Args:
+          - value: int, float, str, bool, or None, the value
+
+        Return: JSONBuiltin, the new JSONBuiltin
+
+        Raise: ValueError, if value has an unsupported type.
+        """
+        match value:
+            case int() | float():
+                fragment = FragmentEdit(str(value))
+            case str():
+                fragment = FragmentEdit(f'"{value}"')
+            case bool():
+                fragment = FragmentEdit("true" if value else "false")
+            case None:
+                fragment = FragmentEdit("null")
+            case _:
+                raise ValueError("Cannot create JSONBuiltin from type "
+                                 + type(value).__name__)
+        return cls(value=value, fragment=fragment)
+
     def start(self) -> Fragment:
         return self.fragment
 
     def end(self) -> Fragment:
         return self.fragment
 
     def fragments(self) -> list[Fragment]:
         return [self.fragment]
 
     def tographviz(self) -> str:
         return f'  "{id(self)}" [label=<{self.fragment}> shape=box];\n'
 
-    def value(_) -> Any:
-        """value(): Get the value.
-
-        Subclasses must override this method.
-        """
-        raise NotImplementedError()
-
-
-class JSONNumber(JSONLeafValue):
-    """JSONNumber: A JSON number.
-
-    Methods:
-      - float(JSONNumber): Get the value.
-      - int(JSONNumber): Get the value.
-    """
-    def __float__(self) -> float:
-        return float(str(self.fragment))
-
     def __int__(self) -> int:
-        return int(str(self.fragment))
-
-    def value(self) -> int | float:
-        """value(): Get the value.
-
-        Return: int or float, the value.
-        """
-        try:
-            return int(self)
-        except ValueError:
-            return float(self)
-
-    @classmethod
-    def create(cls, value: float | str) -> JSONNumber:
-        """create(value): Create a new JSONNumber.
-
-        Args:
-          - value: float, the value
-
-        Return: JSONNumber, the new JSON number
-
-        Note that this method creates a new FragmentEdit, which is not part of
-        any FragmentList.
-        """
-        return cls(FragmentEdit(str(value)))
+        return int(self.value) # type: ignore
 
+    def __float__(self) -> float:
+        return float(self.value) # type: ignore
 
-class JSONString(JSONLeafValue):
-    """JSONString: A JSON string.
+    def __str__(self) -> str:
+        return str(self.value)
 
-    Methods:
-      - repr(JSONString): Get the value.
-      - str(JSONString): Get the value.
-    """
     def __repr__(self) -> str:
+        if isinstance(self.value, str):
+            return repr(self.value)
         return str(self.fragment)
 
-    def __str__(self) -> str:
-        return repr(self)[1:-1]
-
-    def value(self) -> str:
-        """value(): Get the value.
-
-        Return: str, the value.
-
-        Alias for str(JSONString).
-        """
-        return str(self)
-
-    @classmethod
-    def create(cls, value: str) -> JSONString:
-        """create(value): Create a new JSONString.
-
-        Args:
-          - value: str, the value
-
-        Return: JSONString, the new JSON string
-
-        Note that this method creates a new FragmentEdit, which is not part of
-        any FragmentList.
-        """
-        return cls(FragmentEdit(f'"{value}"'))
 
+class JSONContainer:
+    """JSONContainer: An editable JSON container.
 
-class JSONBool(JSONLeafValue):
-    """JSONBool: A JSON boolean.
-
-    Methods:
-      - bool(JSONBool): Get the value.
+    All JSONContainer are associated with a FragmentList with which they sync
+    all insertions, deletions, and replacements within the container.
     """
-    def __bool__(self) -> bool:
-        return str(self.fragment) == "true"
-
-    def value(self) -> bool:
-        """value(): Get the value.
-
-        Return: bool, the value.
-
-        Alias for bool(JSONBool).
-        """
-        return bool(self)
+    # Private attributes:
+    #   - _fragmentlist: FragmentList, the list associated with the container
+    _fragmentlist: FragmentList
 
-    @classmethod
-    def create(cls, value: bool) -> JSONBool:
-        """create(value): Create a new JSONBool.
+    def __init__(self, fragmentlist: FragmentList):
+        """JSONContainer(fragmentlist)
 
         Args:
-          - value: bool, the value
-
-        Return: JSONBool, the new JSON boolean
-
-        Note that this method creates a new FragmentEdit, which is not part of
-        any FragmentList.
-        """
-        return cls(FragmentEdit("true" if value else "false"))
-
-
-class JSONNull(JSONLeafValue):
-    """JSONNull: A JSON null."""
-    def value(_) -> None:
-        """value(): Get the value.
-
-        Return: None
-        """
-        return None
-
-    @classmethod
-    def create(cls) -> JSONNull:
-        """create(): Create a new JSONNull.
-
-        Return: JSONNull, the new JSON null
-
-        Note that this method creates a new FragmentEdit, which is not part of
-        any FragmentList.
+          - fragmentlist: FragmentList, the list to associate with this
+            container
         """
-        return cls(FragmentEdit("null"))
+        self._fragmentlist = fragmentlist
 
 
-class JSONArray(JSONValue, JSONEditable):
+class JSONArray(JSONValue, JSONContainer):
     """JSONArray: A JSON array.
 
     Methods:
-      - JSONArray[index]: Get a value or slice of the array.
       - len(JSONArray): Get the length of the array.
+      - iter(JSONArray): Get an iterator over the values of the array.
+      - JSONArray[index]: Get a value of the array.
+      - JSONArray[slice]: Get a slice of values of the array.
+      - JSONArray[index] = value: Alias for JSONArray.editreplace(index, value)
+      - del JSONArray[index]: Alias for JSONArray.editdelete(index)
 
-      - values(): Get the values of the array.
       - editdelete(index): Delete a value.
       - editinsert(index, value): Insert a value.
       - editinsertnewarray(index): Insert a new, empty array.
       - editinsertnewobject(index): Insert a new, empty object.
       - editreplace(index, newvalue): Replace a value.
       - editreplacenewarray(index): Replace a value with a new, empty array.
       - editreplacenewobject(index): Replace a value with a new, empty object.
@@ -698,15 +605,15 @@
             raise ValueError("Too many commas")
         if len(commas) + 1 < len(values):
             raise ValueError("Not enough commas")
         self._leftbracket = leftbracket
         self._values = values
         self._commas = commas
         self._rightbracket = rightbracket
-        JSONEditable.__init__(self, fragmentlist)
+        JSONContainer.__init__(self, fragmentlist)
 
     def start(self) -> Fragment:
         return self._leftbracket
 
     def end(self) -> Fragment:
         return self._rightbracket
 
@@ -747,26 +654,28 @@
             new container
 
         Return: JSONArray, the new JSON array
         """
         return cls(FragmentEdit("["), list(), list(), FragmentEdit("]"),
                    fragmentlist)
 
-    def __getitem__(self, key: int | slice) -> JSONValue | list[JSONValue]:
-        return self._values[key]
-
     def __len__(self) -> int:
         return len(self._values)
 
-    def values(self) -> list[JSONValue]:
-        """values(): Get the values of the array.
+    def __iter__(self) -> Iterable[JSONValue]:
+        return iter(self._values)
 
-        Return: list of JSONValue, the values of the array
-        """
-        return list(self._values)
+    def __getitem__(self, key: int | slice) -> JSONValue | list[JSONValue]:
+        return self._values[key]
+
+    def __setitem__(self, key: int, value: JSONValue | BuiltinType) -> None:
+        self.editreplace(key, value)
+
+    def __delitem__(self, key: int) -> None:
+        self.editdelete(key)
 
     def editdelete(self, index: int) -> None:
         """editdelete(index): Delete a value.
 
         Args:
           - index: int, the position to delete
 
@@ -821,32 +730,35 @@
             f4 = self._fragmentlist.getfillerbetween(
                     comma, self._values[index + 1].start())
             end = f4[-1] if f4 else comma
             self._fragmentlist.delete(start, end)
             del self._values[index]
             del self._commas[index]
 
-    def editinsert(self, index: int, value: JSONValue) -> None:
+    def editinsert(self, index: int, value: JSONValue | BuiltinType) -> None:
         """editinsert(index, value): Insert a value.
 
         Args:
           - index: int, the position to insert at
-          - value: JSONValue, the value to insert
+          - value: JSONValue, int, float, str, bool, or None, the value to
+            insert
 
         Insertion is such that afterwards, value will be at position index in
         the array.
 
         If index is -1 or the length of the array, this is equivalent to
         inserting after the last element.
 
         All of the fragments of the value are registered with the FragmentList
         of the array. Notably, this will not include any filler they might have
         been associated with in another FragmentList.
 
-        Raise: IndexError, if index is not valid.
+        Raise:
+          - IndexError, if index is not valid.
+          - ValueError, if value has an unsupported type.
 
         Filler is reorganised around the inserted value:
         f is eventual filler, ^ is point of insertion, - is reused fragments
         If array is empty:
              [ f ]
                -^
           => [ f value f ]
@@ -867,14 +779,17 @@
                             --   --^
           => ... prev_value f1 , f2 value f1 , f2 next_value ...
         """
         assert -1 <= index <= len(self._values)
         if index == -1:
             index = len(self._values)
 
+        if not isinstance(value, JSONValue):
+            value = JSONBuiltin.create(value)
+
         if not self._values:
             #    [ f ]
             #      -^
             # => [ f value f ]
             f = self._fragmentlist.getfillerbetween(self._leftbracket,
                                                     self._rightbracket)
             toinsert = value.fragments()
@@ -968,23 +883,28 @@
 
         The new object has the same FragmentList as this container.
         """
         obj = JSONObject.create(self._fragmentlist)
         self.editinsert(index, obj)
         return obj
 
-    def editreplace(self, index: int, newvalue: JSONValue) -> None:
+    def editreplace(self, index: int, newvalue: JSONValue | BuiltinType
+                    ) -> None:
         """editreplace(index, newvalue): Replace a value.
 
         Args:
           - index: int, the position to replace
-          - newvalue: JSONValue, the new value
+          - newvalue: JSONValue, int, float, str, bool, or None, the new value
 
-        Raise: IndexError, if index is not valid.
+        Raise:
+          - IndexError, if index is not valid.
+          - ValueError, if value has an unsupported type.
         """
+        if not isinstance(newvalue, JSONValue):
+            newvalue = JSONBuiltin.create(newvalue)
         oldvalue = self._values[index]
         newfragments = newvalue.fragments()
         self._fragmentlist.replace(oldvalue.start(), oldvalue.end(),
                                    newfragments)
         self._values[index] = newvalue
 
     def editreplacenewarray(self, index: int) -> JSONArray:
@@ -1023,22 +943,27 @@
         The new object has the same FragmentList as this container.
         """
         obj = JSONObject.create(self._fragmentlist)
         self.editreplace(index, obj)
         return obj
 
 
-class JSONObject(JSONValue, JSONEditable):
+class JSONObject(JSONValue, JSONContainer):
     """JSONObject: A JSON object.
 
     Methods:
-      - JSONObject[name]: Get the values of the object.
       - len(JSONObject): Get the number of entries in the object.
+      - iter(JSONObject): Alias for JSONObject.keys()
+      - JSONObject[key]: Get the values of the object.
+      - name in JSONObject: Is a name in the object.
 
+      - keys(): Get the names of the object.
+      - values(): Get the values of the object.
       - items(): Get the name:value entries of the object.
+      - lookup(key): Get the indices of entries of the object.
       - editdelete(index): Delete an entry.
       - editinsert(index, name, value): Insert a new name:value entry.
       - editinsertnewarray(index, name): Insert an entry with a new, empty
         array.
       - editinsertnewobject(index, name): Insert an entry with a new, empty
         object.
       - editreplacename(index, newname): Replace the name of an entry.
@@ -1046,52 +971,54 @@
       - editreplacenewarray(index): Replace the value of an entry with a new,
         empty array.
       - editreplacenewobject(index): Replace the value of an entry with a new,
         empty object.
     """
     # Private attributes:
     #   - _leftbracket: Fragment, the opening bracket fragment
-    #   - _items: list of tuple (JSONString, Fragment, JSONValue), the (name,
+    #   - _items: list of tuple (JSONBuiltin, Fragment, JSONValue), the (name,
     #     colon, value) entries
     #   - _commas: list of Fragment, the list of commas
     #   - _rightbracket: Fragment, the closing bracket fragment
     # Either both _items and _commas are empty, or len(_items) == len(_commas) +
     # 1.
     _leftbracket: Fragment
-    _items: list[tuple[JSONString, Fragment, JSONValue]]
+    _items: list[tuple[JSONBuiltin, Fragment, JSONValue]]
     _commas: list[Fragment]
     _rightbracket: Fragment
 
     def __init__(self, leftbracket: Fragment,
-                 items: list[tuple[JSONString, Fragment, JSONValue]],
+                 items: list[tuple[JSONBuiltin, Fragment, JSONValue]],
                  commas: list[Fragment], rightbracket: Fragment,
                  fragmentlist: FragmentList):
         """JSONObject(leftbracket, items, commas, rightbracket, fragmentlist)
 
         Args:
           - leftbracket: Fragment, the opening bracket fragment
-          - items: list of tuple (JSONString, Fragment, JSONValue), the (name,
+          - items: list of tuple (JSONBuiltin, Fragment, JSONValue), the (name,
             colon, value) entries
           - commas: list of Fragment, the list of commas
           - rightbracket: Fragment, the closing bracket fragment
           - fragmentlist: FragmentList, the fragment list associated with this
             container
 
         Raise: ValueError, if items and commas are neither both empty nor
-        len(items) == len(commas) + 1.
+        len(items) == len(commas) + 1, or if the names are not all strings.
         """
         if 0 < len(items) <= len(commas):
             raise ValueError("Too many commas")
         if len(commas) + 1 < len(items):
             raise ValueError("Not enough commas")
+        if not all(isinstance(name.value, str) for name, _, __ in items):
+            raise ValueError("Names must be str")
         self._leftbracket = leftbracket
         self._items = items
         self._commas = commas
         self._rightbracket = rightbracket
-        JSONEditable.__init__(self, fragmentlist)
+        JSONContainer.__init__(self, fragmentlist)
 
     def start(self) -> Fragment:
         return self._leftbracket
 
     def end(self) -> Fragment:
         return self._rightbracket
 
@@ -1142,27 +1069,62 @@
             new container
 
         Return: JSONObject, the new JSON object
         """
         return cls(FragmentEdit("{"), list(), list(), FragmentEdit("}"),
                    fragmentlist)
 
-    def __getitem__(self, key: str) -> list[JSONValue]:
-        return [value for name, _, value in self._items if str(name) == key]
-
     def __len__(self) -> int:
         return len(self._items)
 
-    def items(self) -> list[tuple[JSONString, JSONValue]]:
+    def __iter__(self) -> Iterable[str]:
+        return self.keys()
+
+    def __getitem__(self, key: str | JSONBuiltin) -> list[JSONValue]:
+        return [value
+                for name, _, value in self._items
+                if str(name) == str(key)]
+
+    def __contains__(self, key: str | JSONBuiltin) -> bool:
+        key = str(key)
+        return any(key == str(name) for name, _, __ in self._items)
+
+    def keys(self) -> Iterable[str]:
+        """keys(): Get the names of the object.
+
+        Return: iterable of str, the names in the object
+
+        Names can appear multiple times.
+        """
+        return (str(name) for name, _, __ in self._items)
+
+    def values(self) -> Iterable[JSONValue]:
+        """values(): Get the values of the object.
+
+        Return: iterable of JSONValue, the values in the object
+        """
+        return (value for _, __, value in self._items)
+
+    def items(self) -> Iterable[tuple[str, JSONValue]]:
         """items(): Get the name:value entries of the object.
 
-        Return: list of tuple (JSONString, JSONValue), the name:value entries of
+        Return: iterable of tuple (str, JSONValue), the name:value entries of
         the array.
         """
-        return [(name, value) for name, _, value in self._items]
+        return ((str(name), value) for name, _, value in self._items)
+
+    def lookup(self, key: str | JSONBuiltin) -> Iterable[int]:
+        """lookup(key): Get the indices of entries of the object.
+
+        Return: iterable of int, the indices of the entries that have this name
+        """
+        key = str(key)
+        return (i
+                for i, (name, _, __) in enumerate(self._items)
+                if key == str(name))
 
     def editdelete(self, index: int) -> None:
         """editdelete(index): Delete an entry.
 
         Args:
           - index: int, the position to delete
 
@@ -1196,33 +1158,37 @@
             f4 = self._fragmentlist.getfillerbetween(
                     comma, self._items[index + 1][0].start())
             end = f4[-1] if f4 else comma
             self._fragmentlist.delete(start, end)
             del self._items[index]
             del self._commas[index]
 
-    def editinsert(self, index: int, name: str, value: JSONValue) -> None:
+    def editinsert(self, index: int, name: str, value: JSONValue | BuiltinType
+                   ) -> None:
         """editinsert(index, name, value): Insert a new name:value entry.
 
         Args:
           - index: int, the position to insert at
           - name: str, the name of the entry to insert
-          - value: JSONValue, the value of the entry to insert
+          - value: JSONValue, int, float, str, bool, or None, the value to
+            insert
 
         Insertion is such that afterwards, the inserted entry will be at
         position index in the object.
 
         If index is -1 or the length of the object, this is equivalent to
         inserting after the last entry.
 
         All of the fragments of the value are registered with the FragmentList
         of the object. Notably, this will not include any filler they might have
         been associated with in another FragmentList.
 
-        Raise: IndexError, if index is not valid.
+        Raise:
+          - IndexError, if index is not valid.
+          - ValueError, if value has an unsupported type.
 
         Filler is reorganised around the inserted value:
         f is eventual filler, ^ is point of insertion, - is reused fragments
         If object is empty:
              [ f ]
                -^
           => [ f name : value f ]
@@ -1243,15 +1209,17 @@
                            --   --            --   --^
           => ... prev_name f1 : f2 prev_value f3 , f4 name f1 : f2 value f3 , f4 next_name ...
         """
         assert -1 <= index <= len(self._items)
         if index == -1:
             index = len(self._items)
 
-        jname = JSONString.create(name)
+        jname = JSONBuiltin.create(name)
+        if not isinstance(value, JSONValue):
+            value = JSONBuiltin.create(value)
         colon = FragmentEdit(":")
         if not self._items:
             #    [ f ]
             #      -^
             # => [ f name : value f ]
             f = self._fragmentlist.getfillerbetween(self._leftbracket,
                                                     self._rightbracket)
@@ -1387,28 +1355,33 @@
         Args:
           - index: int, the position to replace
           - newname: str, the new name
 
         Raise: IndexError, if index is not valid.
         """
         oldname, colon, value = self._items[index]
-        jnewname = JSONString.create(newname)
+        jnewname = JSONBuiltin.create(newname)
         newfragments = jnewname.fragments()
         self._fragmentlist.replace(oldname.start(), oldname.end(), newfragments)
         self._items[index] = (jnewname, colon, value)
 
-    def editreplacevalue(self, index: int, newvalue: JSONValue) -> None:
+    def editreplacevalue(self, index: int, newvalue: JSONValue | BuiltinType
+                         ) -> None:
         """editreplacevalue(index, newvalue): Replace the value of an entry.
 
         Args:
           - index: int, the position to replace
-          - newvalue: JSONValue, the new value
+          - newvalue: JSONValue, int, float, str, bool, or None, the new value
 
-        Raise: IndexError, if index is not valid.
+        Raise:
+          - IndexError, if index is not valid.
+          - ValueError, if value has an unsupported type.
         """
+        if not isinstance(newvalue, JSONValue):
+            newvalue = JSONBuiltin.create(newvalue)
         name, colon, oldvalue = self._items[index]
         newfragments = newvalue.fragments()
         self._fragmentlist.replace(oldvalue.start(), oldvalue.end(),
                                    newfragments)
         self._items[index] = (name, colon, newvalue)
 
     def editreplacenewarray(self, index: int) -> JSONArray:
@@ -1503,49 +1476,44 @@
 
     Only FragmentOrigin will be produced. They will not be registered to
     fragmentlist, you should call xel() after this function.
 
     Return: JSONValue, the editable JSON value
     """
     match anode:
-        case ANodeNumber():
-            return JSONNumber(FragmentOrigin(anode.token))
-        case ANodeString():
-            return JSONString(FragmentOrigin(anode.token))
-        case ANodeBool():
-            return JSONBool(FragmentOrigin(anode.token))
-        case ANodeNull():
-            return JSONNull(FragmentOrigin(anode.token))
+        case ANodeNumber() | ANodeString() | ANodeBool() | ANodeNull():
+            return JSONBuiltin(value=anode.value(),
+                               fragment=FragmentOrigin(anode.token))
         case ANodeArray():
             leftbracket = FragmentOrigin(anode.leftbracket)
             values = list(editableify(value, fragmentlist)
                           for value in anode.values)
             arrcommas: list[Fragment] = list(
                     FragmentOrigin(comma) for comma in anode.commas)
             rightbracket = FragmentOrigin(anode.rightbracket)
             return JSONArray(leftbracket, values, arrcommas, rightbracket,
                              fragmentlist)
         case ANodeObject():
             leftbracket = FragmentOrigin(anode.leftbracket)
             items = list()
             for item in anode.items:
-                name = cast(JSONString, editableify(item[0], fragmentlist))
+                name = cast(JSONBuiltin, editableify(item[0], fragmentlist))
                 colon: Fragment = FragmentOrigin(item[1])
                 value = editableify(item[2], fragmentlist)
                 items.append((name, colon, value))
             objcommas: list[Fragment] = list(
                     FragmentOrigin(comma) for comma in anode.commas)
             rightbracket = FragmentOrigin(anode.rightbracket)
             return JSONObject(leftbracket, items, objcommas, rightbracket,
                               fragmentlist)
 
     raise ValueError(f"Unrecognised AST node type: {type(anode).__name__}")
 
 
-class JSONEditor(JSONEditable):
+class JSONEditor(JSONContainer):
     """JSONEditor: Editable JSON data.
 
     Attributes:
       - root: JSONValue, the root of the editable AST
 
     Class methods:
       - JSONEditor.fromAST(ast): Make an AST editable.
```

### Comparing `jsoncgx-1.0/jsoncgx.egg-info/PKG-INFO` & `jsoncgx-1.1/jsoncgx.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsoncgx
-Version: 1.0
+Version: 1.1
 Summary: An overpowered JSON-with-comments parser with inplace edition
 Author-email: cigix <cigix@cigix.me>
 Project-URL: Repository, https://github.com/cigix/jsoncgx
 Project-URL: Issues, https://github.com/cigix/jsoncgx/issues
 Keywords: json,jsonc,json with comments,json editor
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -68,15 +68,15 @@
 </td>
 <td>
 
 ```python
 
 >>> import jsoncgx
 >>> editor = jsoncgx.loads('{ "answer": 42 }')
->>> editor.root["answer"][0].value()
+>>> editor.root["answer"][0]
 42
 ```
 
 </td>
    </tr>
    <tr>
       <td>Editing JSON data</td>
@@ -88,16 +88,15 @@
 '{"answer": "spam"}'
 ```
 
 </td>
 <td>
 
 ```python
->>> editor.root.editreplacevalue(0,
-...     jsoncgx.JSONString.create("spam"))
+>>> editor.root.editreplacevalue(0, "spam")
 >>> editor.dumps()
 '{ "answer": "spam" }'
 ```
 
 </td>
    </tr>
    <tr>
@@ -136,17 +135,17 @@
 
 </td>
 <td>
 
 ```python
 >>> editor = jsoncgx.loads(
 ...     '{ "answer": 42, "answer": "spam" }')
->>> editor.root["answer"][0].value()
+>>> editor.root["answer"][0]
 42
->>> editor.root["answer"][1].value()
+>>> editor.root["answer"][1]
 'spam'
 ```
 
 </td>
    </tr>
    <tr>
       <td>Comments</td>
@@ -162,16 +161,15 @@
 
 </td>
 <td>
 
 ```python
 >>> editor = jsoncgx.loads(
 ...     '{ "answer": /* eggs and */ 42 }')
->>> editor.root.editreplacevalue(0,
-...     jsoncgx.JSONString.create("spam"))
+>>> editor.root.editreplacevalue(0, "spam")
 >>> editor.dumps()
 '{ "answer": /* eggs and */ "spam" }'
 ```
 
 </td>
    </tr>
 </table>
@@ -193,7 +191,16 @@
   * U+002F.
 
 Those elements are considered like whitespace.
 
 ## Architecture
 
 ![jsoncgx architecture](architecture.png)
+
+## Changelog
+
+### V1.1:
+
+* `JSONNumber`, `JSONString`, `JSONBool`, and `JSONNull` have been replaced with
+  `JSONBuiltin`, for easier integration.
+* `edit*()` methods that accepted `JSONValue` now also accept `int`, `float`,
+  `str`, `bool`, and `None`. They are automatically turned into `JSONBuiltin`.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jsoncgx Version: 1.0 Summary: An overpowered JSON-
+Metadata-Version: 2.1 Name: jsoncgx Version: 1.1 Summary: An overpowered JSON-
 with-comments parser with inplace edition Author-email: cigix
 cigix.me> Project-URL: Repository, https://github.com/cigix/jsoncgx Project-
 URL: Issues, https://github.com/cigix/jsoncgx/issues Keywords: json,jsonc,json
 with comments,json editor Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: OSI Approved :: GNU General Public License v3 or
 later (GPLv3+) Classifier: Programming Language :: Python :: 3 Classifier:
 Topic :: File Formats :: JSON Classifier: Typing :: Typed Requires-Python:
@@ -22,47 +22,48 @@
 indentation, and serialisation reproduces it. ## Installation This library is
 [available on PyPI](https://pypi.org/project/jsoncgx/): ``` pip install --user
 jsoncgx ``` ## Comparison / Quickstart / Demo
                   SSttaannddaarrdd PPyytthhoonn mmoodduullee        ``jjssoonnccggxx``
                   ```python >>> import json >>> ```python >>> import jsoncgx
                   data = json.loads('           >>> editor = jsoncgx.loads('
 Loading JSON data { "answer": 42 }') >>> data   { "answer": 42 }') >>>
-                  ["answer"] 42 ```             editor.root["answer"]
-                                                [0].value() 42 ```
+                  ["answer"] 42 ```             editor.root["answer"][0] 42
+                                                ```
                                                 ```python >>>
                   ```python >>> data["answer"]  editor.root.editreplacevalue
-Editing JSON data = "spam" >>> json.dumps(data) (0, ...
-                  '{"answer": "spam"}' ```      jsoncgx.JSONString.create
-                                                ("spam")) >>> editor.dumps()
-                                                '{ "answer": "spam" }' ```
+Editing JSON data = "spam" >>> json.dumps(data) (0, "spam") >>> editor.dumps
+                  '{"answer": "spam"}' ```      () '{ "answer": "spam" }'
+                                                ```
                   ```python >>> with open       ```python >>> editor =
                   ("in.json") as f: ... data =  json.loadf("in.json") >>>
 Working with JSON json.load(f) ... >>> with     editor.dumpf("out.json") ```
 files             open("out.json", "w") as f:   Or use `jsoncgx.load()` and
                   ... json.dump(data, f) ...    `jsoncgx.JSONEditor.dump()`
                   ```                           with a file handle, like the
                                                 standard module.
                                                 ```python >>> editor =
                   ```python >>> data =          jsoncgx.loads( ... '
                   json.loads( ... '{ "answer":  { "answer": 42, "answer":
 Non unique name   42, "answer": "spam" }') >>>  "spam" }') >>> editor.root
-                  data["answer"] 'spam' ```     ["answer"][0].value() 42 >>>
-                                                editor.root["answer"]
-                                                [1].value() 'spam' ```
-                                                ```python >>> editor =
-                  ```python >>> data =          jsoncgx.loads( ... '
-                  json.loads( ... '{ "answer":  { "answer": /* eggs and */
-                  /* eggs and */ 42 }')         42 }') >>>
-Comments          Traceback (most recent call   editor.root.editreplacevalue
-                  last): ...                    (0, ...
-                  json.decoder.JSONDecodeError: jsoncgx.JSONString.create
-                  ... ```                       ("spam")) >>> editor.dumps()
-                                                '{ "answer": /* eggs and */
-                                                "spam" }' ```
+                  data["answer"] 'spam' ```     ["answer"][0] 42 >>>
+                                                editor.root["answer"][1]
+                                                'spam' ```
+                  ```python >>> data =          ```python >>> editor =
+                  json.loads( ... '{ "answer":  jsoncgx.loads( ... '
+                  /* eggs and */ 42 }')         { "answer": /* eggs and */
+Comments          Traceback (most recent call   42 }') >>>
+                  last): ...                    editor.root.editreplacevalue
+                  json.decoder.JSONDecodeError: (0, "spam") >>> editor.dumps
+                  ... ```                       () '{ "answer": /* eggs and
+                                                */ "spam" }' ```
 ## What syntax does this parse exactly? [ECMA-404](https://ecma-
 international.org/wp-content/uploads/ECMA-404_2nd_edition_december_2017.pdf)
 with the following additional lexical elements: * regex `//[^\n]*\n`, that is,
 the Unicode scalar sequence: * U+002F, * U+002F, * any amount of any scalars
 except U+000A, * U+000A. * lazy regex `/\*.*\*/`, that is, the Unicode scalar
 sequence: * U+002F, * U+002A, * any amount of any scalars except the sequence
 U+002A U+002F * U+002A, * U+002F. Those elements are considered like
-whitespace. ## Architecture ![jsoncgx architecture](architecture.png)
+whitespace. ## Architecture ![jsoncgx architecture](architecture.png) ##
+Changelog ### V1.1: * `JSONNumber`, `JSONString`, `JSONBool`, and `JSONNull`
+have been replaced with `JSONBuiltin`, for easier integration. * `edit*()`
+methods that accepted `JSONValue` now also accept `int`, `float`, `str`,
+`bool`, and `None`. They are automatically turned into `JSONBuiltin`.
```

### Comparing `jsoncgx-1.0/pyproject.toml` & `jsoncgx-1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "jsoncgx"
-version = "1.0"
+version = "1.1"
 requires-python = ">=3.9"
 
 description = "An overpowered JSON-with-comments parser with inplace edition"
 readme = "README.md"
 authors = [{name = "cigix", email="cigix@cigix.me"}]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
@@ -21,9 +21,9 @@
 
 [tool.mypy]
 disallow_untyped_defs = true
 disallow_untyped_calls = true
 warn_return_any = true
 
 [[tool.mypy.overrides]]
-module = "jsoncgx.tests"
+module = "tests"
 disallow_untyped_defs = false
```

