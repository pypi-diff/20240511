# Comparing `tmp/partial_json_parser-0.2.0.1.tar.gz` & `tmp/partial_json_parser-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "partial_json_parser-0.2.0.1.tar", last modified: Fri May 10 16:09:47 2024, max compression
+gzip compressed data, was "partial_json_parser-0.2.1.tar", last modified: Sat May 11 06:39:04 2024, max compression
```

## Comparing `partial_json_parser-0.2.0.1.tar` & `partial_json_parser-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     4349 2024-03-19 22:29:06.717053 partial_json_parser-0.2.0.1/README.md
--rw-r--r--   0        0        0     1432 2024-05-10 16:09:47.050000 partial_json_parser-0.2.0.1/pyproject.toml
--rw-r--r--   0        0        0     7748 2024-05-10 16:04:30.655203 partial_json_parser-0.2.0.1/src/partial_json_parser/__init__.py
--rw-r--r--   0        0        0      992 2024-04-03 08:20:30.049307 partial_json_parser-0.2.0.1/src/partial_json_parser/options.py
--rw-r--r--   0        0        0     1132 2024-05-10 13:51:09.110094 partial_json_parser-0.2.0.1/src/partial_json_parser/playground.py
--rw-r--r--   0        0        0    19024 2024-05-10 15:51:01.796128 partial_json_parser-0.2.0.1/tests/__pycache__/test_examples.cpython-312-pytest-7.4.4.pyo
--rw-r--r--   0        0        0     4870 2024-05-10 15:51:01.804081 partial_json_parser-0.2.0.1/tests/__pycache__/test_hypotheses.cpython-312-pytest-7.4.4.pyo
--rw-r--r--   0        0        0     2353 2024-05-10 16:04:23.967712 partial_json_parser-0.2.0.1/tests/test_examples.py
--rw-r--r--   0        0        0     1332 2024-05-10 16:04:30.655203 partial_json_parser-0.2.0.1/tests/test_hypotheses.py
--rw-r--r--   0        0        0     4841 1970-01-01 00:00:00.000000 partial_json_parser-0.2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     5774 2024-05-11 06:34:06.584003 partial_json_parser-0.2.1/README.md
+-rw-r--r--   0        0        0     1430 2024-05-11 06:39:04.021403 partial_json_parser-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7753 2024-05-11 06:35:52.232447 partial_json_parser-0.2.1/src/partial_json_parser/__init__.py
+-rw-r--r--   0        0        0      992 2024-04-03 08:20:30.049307 partial_json_parser-0.2.1/src/partial_json_parser/options.py
+-rw-r--r--   0        0        0      885 2024-05-11 06:10:13.960124 partial_json_parser-0.2.1/src/partial_json_parser/playground.py
+-rw-r--r--   0        0        0    19024 2024-05-10 15:51:01.796128 partial_json_parser-0.2.1/tests/__pycache__/test_examples.cpython-312-pytest-7.4.4.pyo
+-rw-r--r--   0        0        0     4870 2024-05-10 15:51:01.804081 partial_json_parser-0.2.1/tests/__pycache__/test_hypotheses.cpython-312-pytest-7.4.4.pyo
+-rw-r--r--   0        0        0     2662 2024-05-11 06:10:13.960124 partial_json_parser-0.2.1/tests/test_examples.py
+-rw-r--r--   0        0        0     1332 2024-05-11 06:35:52.232447 partial_json_parser-0.2.1/tests/test_hypotheses.py
+-rw-r--r--   0        0        0     6221 1970-01-01 00:00:00.000000 partial_json_parser-0.2.1/PKG-INFO
```

### Comparing `partial_json_parser-0.2.0.1/README.md` & `partial_json_parser-0.2.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -7,22 +7,44 @@
 Here comes `partial-json-parser`, a lightweight and customizable library for parsing partial JSON strings. Here is a [demo](https://promplate.dev/partial-json-parser).
 
 (Note that there is [a JavaScript implementation](https://github.com/promplate/partial-json-parser-js) too)
 
 ## Installation
 
 ```sh
-pip install partial-json-parser # or poetry / pdm / conda
+pip install partial-json-parser # or poetry / pdm / uv
 ```
 
-`partial-json-parser` is implemented purely in Python, with good type hints.
+`partial-json-parser` is implemented purely in Python, with good type hints. It is zero-dependency and works with Python 3.6+.
+
+You can install run its demo playground by installing `rich` too or:
+
+```sh
+pip install partial-json-parser[playground]
+```
+
+Then run the `json-playground` in your terminal, and you can try the parser interactively.
 
 ## Usage
 
-### Importing the library
+```py
+from partial_json_parser import loads
+
+>>> loads('{"key": "v')  # {'key': 'v'}
+```
+
+Alternatively, you can use `ensure_json` to get the completed JSON string:
+
+```py
+from partial_json_parser import ensure_json
+
+>>> ensure_json('{"key": "v')  # '{"key": "v"}'
+```
+
+### Detailed Usage
 
 You can import the `loads` function and the `Allow` object from the library like this:
 
 ```py
 from partial_json_parser import loads, Allow
 ```
 
@@ -79,21 +101,42 @@
 
 ```py
 loads("wrong")  # MalformedJSON: Malformed node or string on line 1
 ```
 
 ## API Reference
 
-### loads(json_string, [allow_partial])
+### loads(json_string, [allow_partial], [parser])
 
-- `json_string` `<string>`: The JSON string to parse.
+- `json_string` `<string>`: The (incomplete) JSON string to parse.
 - `allow_partial` `<Allow | int>`: Specify what kind of partialness is allowed during JSON parsing (default: `Allow.ALL`).
+- `parser` `(str) -> JSON`: An ordinary JSON parser. Default is `json.loads`.
+
+Complete the JSON string and parse it with `parser` function.
 
 Returns the parsed Python value.
 
+Alias: `decode`, `parse_json`.
+
+### ensure_json(json_string, [allow_partial])
+
+- `json_string` `<string>`: The (incomplete) JSON string to complete.
+- `allow_partial` `<Allow | int>`: Specify what kind of partialness is allowed during JSON parsing (default: `Allow.ALL`).
+
+Returns the completed JSON string.
+
+### fix(json_string, [allow_partial])
+
+- `json_string` `<string>`: The (incomplete) JSON string to complete.
+- `allow_partial` `<Allow | int>`: Specify what kind of partialness is allowed during JSON parsing (default: `Allow.ALL`).
+
+Returns a tuple of a slice of the input string and the completion.
+
+Note that this is a low-level API, only useful for debugging and demonstration.
+
 ### Allow
 
 Enum class that specifies what kind of partialness is allowed during JSON parsing. It has the following members:
 
 - `STR`: Allow partial string.
 - `NUM`: Allow partial number.
 - `ARR`: Allow partial array.
```

### Comparing `partial_json_parser-0.2.0.1/pyproject.toml` & `partial_json_parser-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "partial-json-parser"
-version = "0.2.0.1"
+version = "0.2.1"
 description = "Parse partial JSON generated by LLM"
 authors = [
     { name = "Muspi Merol", email = "me@promplate.dev" },
 ]
 dependencies = []
-requires-python = ">=3.6"
+requires-python = ">=3.8"
 readme = "README.md"
 keywords = [
     "JSON",
     "parser",
     "LLM",
     "nlp",
 ]
```

### Comparing `partial_json_parser-0.2.0.1/src/partial_json_parser/__init__.py` & `partial_json_parser-0.2.1/src/partial_json_parser/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,31 +23,37 @@
     pass
 
 
 def parse_json(json_string: str, allow_partial: Union[Allow, int] = ALL, parser: Optional[Callable[[str], JSON]] = None) -> JSON:
     if parser is None:
         from json import loads as parser
 
-    if not isinstance(json_string, str):
-        raise TypeError(f"Expected str, got {type(json_string).__name__}")
-    if not json_string.strip():
-        raise ValueError(f"{json_string!r} is empty")
-    return _parse_json(json_string.strip(), Allow(allow_partial), parser)
+    return parser(ensure_json(json_string, allow_partial))
 
 
-def _parse_json(json_string: str, allow: Allow, parser: Callable[[str], JSON]):
+def ensure_json(json_string: str, allow_partial: Union[Allow, int] = ALL):
+    """get the completed JSON string"""
+
+    head, tail = fix(json_string, allow_partial)
+    return head + tail
+
+
+def fix(json_string: str, allow_partial: Union[Allow, int] = ALL):
+    """get the original slice and the trailing suffix separately"""
+
     try:
-        result = complete_any(json_string, allow, is_top_level=True)  # setting is_top_level to True to treat literal numbers as complete
+        result = complete_any(json_string.strip(), Allow(allow_partial), is_top_level=True)
+        if result is False:
+            raise PartialJSON
+
+        index, completion = result
+        return json_string[:index], ("" if completion is True else completion)
+
     except (AssertionError, IndexError) as err:
         raise MalformedJSON(*err.args) from err
-    if result is False:
-        raise PartialJSON
-    if result[1] is True:
-        return parser(json_string[: result[0]])
-    return parser(json_string[: result[0]] + result[1])
 
 
 def skip_blank(text: str, index: int):
     try:
         while text[index].isspace():
             index += 1
     finally:
@@ -253,8 +259,8 @@
     else:
         return i, True
 
 
 loads = decode = parse_json
 
 
-__all__ = ["loads", "decode", "parse_json", "JSONDecodeError", "PartialJSON", "MalformedJSON", "Allow", "JSON"]
+__all__ = ["loads", "decode", "parse_json", "fix", "ensure_json", "JSONDecodeError", "PartialJSON", "MalformedJSON", "Allow", "JSON"]
```

### Comparing `partial_json_parser-0.2.0.1/src/partial_json_parser/options.py` & `partial_json_parser-0.2.1/src/partial_json_parser/options.py`

 * *Files identical despite different names*

### Comparing `partial_json_parser-0.2.0.1/tests/__pycache__/test_examples.cpython-312-pytest-7.4.4.pyo` & `partial_json_parser-0.2.1/tests/__pycache__/test_examples.cpython-312-pytest-7.4.4.pyo`

 * *Files identical despite different names*

### Comparing `partial_json_parser-0.2.0.1/tests/__pycache__/test_hypotheses.cpython-312-pytest-7.4.4.pyo` & `partial_json_parser-0.2.1/tests/__pycache__/test_hypotheses.cpython-312-pytest-7.4.4.pyo`

 * *Files identical despite different names*

### Comparing `partial_json_parser-0.2.0.1/tests/test_hypotheses.py` & `partial_json_parser-0.2.1/tests/test_hypotheses.py`

 * *Files identical despite different names*

### Comparing `partial_json_parser-0.2.0.1/PKG-INFO` & `partial_json_parser-0.2.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: partial-json-parser
-Version: 0.2.0.1
+Version: 0.2.1
 Summary: Parse partial JSON generated by LLM
 Keywords: JSON,parser,LLM,nlp
 Home-page: https://promplate.dev/partial-json-parser
 Author-Email: Muspi Merol <me@promplate.dev>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Project-URL: Repository, https://github.com/promplate/partial-json-parser
 Project-URL: Homepage, https://promplate.dev/partial-json-parser
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Provides-Extra: playground
 Requires-Dist: rich; extra == "playground"
 Description-Content-Type: text/markdown
 
 # Partial JSON Parser
 
 Sometimes we need **LLM (Large Language Models)** to produce **structural information** instead of natural language. The easiest way is to use JSON.
@@ -24,22 +24,44 @@
 Here comes `partial-json-parser`, a lightweight and customizable library for parsing partial JSON strings. Here is a [demo](https://promplate.dev/partial-json-parser).
 
 (Note that there is [a JavaScript implementation](https://github.com/promplate/partial-json-parser-js) too)
 
 ## Installation
 
 ```sh
-pip install partial-json-parser # or poetry / pdm / conda
+pip install partial-json-parser # or poetry / pdm / uv
 ```
 
-`partial-json-parser` is implemented purely in Python, with good type hints.
+`partial-json-parser` is implemented purely in Python, with good type hints. It is zero-dependency and works with Python 3.6+.
+
+You can install run its demo playground by installing `rich` too or:
+
+```sh
+pip install partial-json-parser[playground]
+```
+
+Then run the `json-playground` in your terminal, and you can try the parser interactively.
 
 ## Usage
 
-### Importing the library
+```py
+from partial_json_parser import loads
+
+>>> loads('{"key": "v')  # {'key': 'v'}
+```
+
+Alternatively, you can use `ensure_json` to get the completed JSON string:
+
+```py
+from partial_json_parser import ensure_json
+
+>>> ensure_json('{"key": "v')  # '{"key": "v"}'
+```
+
+### Detailed Usage
 
 You can import the `loads` function and the `Allow` object from the library like this:
 
 ```py
 from partial_json_parser import loads, Allow
 ```
 
@@ -96,21 +118,42 @@
 
 ```py
 loads("wrong")  # MalformedJSON: Malformed node or string on line 1
 ```
 
 ## API Reference
 
-### loads(json_string, [allow_partial])
+### loads(json_string, [allow_partial], [parser])
 
-- `json_string` `<string>`: The JSON string to parse.
+- `json_string` `<string>`: The (incomplete) JSON string to parse.
 - `allow_partial` `<Allow | int>`: Specify what kind of partialness is allowed during JSON parsing (default: `Allow.ALL`).
+- `parser` `(str) -> JSON`: An ordinary JSON parser. Default is `json.loads`.
+
+Complete the JSON string and parse it with `parser` function.
 
 Returns the parsed Python value.
 
+Alias: `decode`, `parse_json`.
+
+### ensure_json(json_string, [allow_partial])
+
+- `json_string` `<string>`: The (incomplete) JSON string to complete.
+- `allow_partial` `<Allow | int>`: Specify what kind of partialness is allowed during JSON parsing (default: `Allow.ALL`).
+
+Returns the completed JSON string.
+
+### fix(json_string, [allow_partial])
+
+- `json_string` `<string>`: The (incomplete) JSON string to complete.
+- `allow_partial` `<Allow | int>`: Specify what kind of partialness is allowed during JSON parsing (default: `Allow.ALL`).
+
+Returns a tuple of a slice of the input string and the completion.
+
+Note that this is a low-level API, only useful for debugging and demonstration.
+
 ### Allow
 
 Enum class that specifies what kind of partialness is allowed during JSON parsing. It has the following members:
 
 - `STR`: Allow partial string.
 - `NUM`: Allow partial number.
 - `ARR`: Allow partial array.
```

