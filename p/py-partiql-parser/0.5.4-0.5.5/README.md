# Comparing `tmp/py_partiql_parser-0.5.4.tar.gz` & `tmp/py_partiql_parser-0.5.5.tar.gz`

## Comparing `py_partiql_parser-0.5.4.tar` & `py_partiql_parser-0.5.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.4/py_partiql_parser/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.4/py_partiql_parser/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.4/py_partiql_parser/_internal/__init__.py
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.4/py_partiql_parser/_internal/clause_tokenizer.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.4/py_partiql_parser/_internal/csv_converter.py
--rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.4/py_partiql_parser/_internal/delete_parser.py
--rw-r--r--   0        0        0     6964 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.4/py_partiql_parser/_internal/from_parser.py
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.4/py_partiql_parser/_internal/insert_parser.py
--rw-r--r--   0        0        0     8135 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.4/py_partiql_parser/_internal/json_parser.py
--rw-r--r--   0        0        0     8250 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.4/py_partiql_parser/_internal/parser.py
--rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.4/py_partiql_parser/_internal/select_parser.py
--rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.4/py_partiql_parser/_internal/update_parser.py
--rw-r--r--   0        0        0     8698 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.4/py_partiql_parser/_internal/utils.py
--rw-r--r--   0        0        0    12947 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.4/py_partiql_parser/_internal/where_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.4/py_partiql_parser/_packages/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.4/py_partiql_parser/_packages/boto3/__init__.py
--rw-r--r--   0        0        0    10172 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.4/py_partiql_parser/_packages/boto3/types.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.4/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.4/LICENSE
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.4/README.md
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.5/py_partiql_parser/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.5/py_partiql_parser/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.5/py_partiql_parser/_internal/__init__.py
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.5/py_partiql_parser/_internal/clause_tokenizer.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.5/py_partiql_parser/_internal/csv_converter.py
+-rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.5/py_partiql_parser/_internal/delete_parser.py
+-rw-r--r--   0        0        0     6872 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.5/py_partiql_parser/_internal/from_parser.py
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.5/py_partiql_parser/_internal/insert_parser.py
+-rw-r--r--   0        0        0     7675 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.5/py_partiql_parser/_internal/json_parser.py
+-rw-r--r--   0        0        0     8250 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.5/py_partiql_parser/_internal/parser.py
+-rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.5/py_partiql_parser/_internal/select_parser.py
+-rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.5/py_partiql_parser/_internal/update_parser.py
+-rw-r--r--   0        0        0     8698 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.5/py_partiql_parser/_internal/utils.py
+-rw-r--r--   0        0        0    12947 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.5/py_partiql_parser/_internal/where_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.5/py_partiql_parser/_packages/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.5/py_partiql_parser/_packages/boto3/__init__.py
+-rw-r--r--   0        0        0    10172 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.5/py_partiql_parser/_packages/boto3/types.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.5/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.5/LICENSE
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.5/README.md
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 py_partiql_parser-0.5.5/PKG-INFO
```

### Comparing `py_partiql_parser-0.5.4/py_partiql_parser/_internal/clause_tokenizer.py` & `py_partiql_parser-0.5.5/py_partiql_parser/_internal/clause_tokenizer.py`

 * *Files identical despite different names*

### Comparing `py_partiql_parser-0.5.4/py_partiql_parser/_internal/csv_converter.py` & `py_partiql_parser-0.5.5/py_partiql_parser/_internal/csv_converter.py`

 * *Files identical despite different names*

### Comparing `py_partiql_parser-0.5.4/py_partiql_parser/_internal/delete_parser.py` & `py_partiql_parser-0.5.5/py_partiql_parser/_internal/delete_parser.py`

 * *Files identical despite different names*

### Comparing `py_partiql_parser-0.5.4/py_partiql_parser/_internal/from_parser.py` & `py_partiql_parser-0.5.5/py_partiql_parser/_internal/from_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,23 +84,20 @@
         key_has_asterix = from_query.endswith("[*]")
         from_query = from_query[0:-3] if key_has_asterix else from_query
         from_alias = from_alias[0:-3] if from_alias.endswith("[*]") else from_alias
         doc_is_list = documents[from_query].startswith("[") and documents[
             from_query
         ].endswith("]")
 
-        source_data = JsonParser().parse(documents[from_query])
+        source_data = list(JsonParser.parse(documents[from_query]))
 
         if doc_is_list:
-            return {"_1": source_data}
+            return {"_1": source_data[0]}
         elif from_alias:
-            if isinstance(source_data, list):
-                return [CaseInsensitiveDict({from_alias: doc}) for doc in source_data]
-            else:
-                return CaseInsensitiveDict({from_alias: source_data})
+            return [CaseInsensitiveDict({from_alias: doc}) for doc in source_data]
         else:
             return source_data
 
     def _get_nested_source_data(self, documents: Dict[str, Any]) -> Any:
         """
         Our FROM-clauses are nested, meaning we need to dig into the provided document to return the key that we need
            --> FROM s3object.name as name
@@ -131,18 +128,18 @@
             else:
                 # The previous key was a regular key
                 # Assume that the result consists of a singular JSON document
                 if new_key in source_data:
                     doc_is_list = source_data[new_key].startswith("[") and source_data[
                         new_key
                     ].endswith("]")
-                    source_data = JsonParser().parse(source_data[new_key])
+                    source_data = list(JsonParser.parse(source_data[new_key]))  # type: ignore
                     if root_doc and doc_is_list:
                         # AWS behaviour when the root-document is a list
-                        source_data = {"_1": source_data}
+                        source_data = {"_1": source_data[0]}  # type: ignore
                     elif key_so_far == entire_key:
                         if isinstance(source_data, list):  # type: ignore[unreachable]
                             source_data = [{alias: doc} for doc in source_data]  # type: ignore[unreachable]
                         else:
                             source_data = {alias: source_data}
                 else:
                     source_data = {}
```

### Comparing `py_partiql_parser-0.5.4/py_partiql_parser/_internal/insert_parser.py` & `py_partiql_parser-0.5.5/py_partiql_parser/_internal/insert_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
                     ), f"{current_phrase} should be INTO"
                     current_phrase = ""
                     section = "TABLE_NAME"
                     continue
                 if section == "SECTION_VALUE":
                     assert current_phrase.upper() in ["VALUE"]
                     tokenizer.skip_white_space()
-                    attr = JsonParser().parse(tokenizer.give_remaining())
+                    attr = next(JsonParser.parse(tokenizer.give_remaining()))
                     for key, value in attr.items():
                         attr[key] = serializer.serialize(value)
                 if section == "TABLE_NAME":
                     table_name = current_phrase
                     current_phrase = ""
                     tokenizer.skip_white_space()
                     section = "SECTION_VALUE"
```

### Comparing `py_partiql_parser-0.5.4/py_partiql_parser/_internal/json_parser.py` & `py_partiql_parser-0.5.5/py_partiql_parser/_internal/json_parser.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,76 +1,89 @@
 from json import JSONEncoder
-from typing import Any, List, Optional
+from typing import Any, List, Iterator, Optional
 
 from .clause_tokenizer import ClauseTokenizer
 from .utils import CaseInsensitiveDict, Variable
 
 ACCEPTED_QUOTES = ["'", '"', "’"]
 NEW_LINE = "\n"
 
 
 class JsonParser:
     """
     Input can be a multiple documents, separated by a new-line (\n) characters
     So we can't use the builtin JSON parser
     """
 
-    def parse(
-        self,
+    @staticmethod
+    def parse(original: str) -> Iterator[Any]:  # type: ignore[misc]
+        if not (original.startswith("{") or original.startswith("[")):
+            # Doesn't look like JSON - let's return as a variable
+            yield original if original.isnumeric() else Variable(original)
+        tokenizer = ClauseTokenizer(original)
+        while tokenizer.current() is not None:
+            result = JsonParser._get_next_document(original, tokenizer)
+            if result is not None:
+                yield result
+
+    @staticmethod
+    def _get_next_document(  # type: ignore[misc]
         original: str,
-        tokenizer: Optional[ClauseTokenizer] = None,
+        tokenizer: ClauseTokenizer,
         only_parse_initial: bool = False,
     ) -> Any:
-        if not (original.startswith("{") or original.startswith("[")):
-            # Doesn't look like JSON - let's return as a variable
-            return original if original.isnumeric() else Variable(original)
         section: Optional[str] = None  # DICT_KEY | KEY_TO_VALUE | DICT_VAL | OBJECT_END
         dict_key = ""
         current_phrase = ""
         result = CaseInsensitiveDict()
-        tokenizer = tokenizer or ClauseTokenizer(original)
+        level = 0
         while True:
             c = tokenizer.next()
             if not c:
-                break
+                return None
             elif c == "[" and (not section or section == "KEY_TO_VALUE"):
+                level += 1
                 # Start of a list
                 if not section:
-                    return self._parse_list(original, tokenizer)
+                    return JsonParser._parse_list(original, tokenizer)
                 else:
-                    result[dict_key] = self._parse_list(original, tokenizer)
+                    result[dict_key] = JsonParser._parse_list(original, tokenizer)
                     section = None
                     current_phrase = ""
             elif c in ["{", ","] and (not section or section == "OBJECT_END"):
+                if c == "{":
+                    level += 1
                 # Start of a key
                 section = "DICT_KEY"
                 tokenizer.skip_until(ACCEPTED_QUOTES)
                 current_phrase = ""
             elif c in ACCEPTED_QUOTES and section == "DICT_KEY":
                 # End of a key
                 dict_key = current_phrase
                 tokenizer.skip_until([":"])
                 section = "KEY_TO_VALUE"
                 current_phrase = ""
             elif c in ["{"] and section == "KEY_TO_VALUE":
+                level += 1
                 # Start of a value with a new dictionary
                 tokenizer.revert()  # Ensure we start the new parser with the initial {
-                result[dict_key] = self.parse(original, tokenizer)
+                result[dict_key] = JsonParser._get_next_document(original, tokenizer)
                 section = None
                 current_phrase = ""
             elif c in ACCEPTED_QUOTES and section == "KEY_TO_VALUE":
                 # Start of a value
                 section = "DICT_VAL"
                 current_phrase = ""
             elif c in ACCEPTED_QUOTES and section == "DICT_VAL":
                 # End of a value
                 result[dict_key] = current_phrase
                 section = None
                 current_phrase = ""
             elif c in ["}"] and section in ["VAR_VALUE", "INT_VALUE"]:
+                level -= 1
                 # End of a variable/number
                 if section == "INT_VALUE":
                     result[dict_key] = int(current_phrase)
                 elif current_phrase.lower() in ["true", "false"]:
                     result[dict_key] = current_phrase.lower() == "true"
                 else:
                     result[dict_key] = Variable(current_phrase)
@@ -86,64 +99,50 @@
                 elif current_phrase.lower() in ["true", "false"]:
                     result[dict_key] = current_phrase.lower() == "true"
                 else:
                     result[dict_key] = Variable(current_phrase)
                 tokenizer.revert()
                 section = None
                 current_phrase = ""
-            elif section in ["OBJECT_END"]:
-                next_documents = self.parse(original, tokenizer)
-                if next_documents == {}:
-                    return result
-                elif isinstance(next_documents, list):
-                    return [result] + next_documents
-                else:
-                    return [result, next_documents]
             elif c == "}" and section is None:
-                section = "OBJECT_END"
-                # We know whether we are at the end of an object at this point
-                # But we don't know whether this is:
-                # - end of the root object
-                # - end of a nested object
-                # - inbetween multiple objects (separated by new-line)
-                tokenizer.skip_white_space()
-                if tokenizer.current() == "{":
-                    # we're inbetween multiple objects - continue parsing
-                    tokenizer.revert()
-                    pass
+                level -= 1
+                if level == 0:
+                    return result
                 else:
-                    # we're at the end of the root object - next char is probably None. Break and return to the user
-                    # we're at the end of a nested object - next char is probably }.    Break and let the parent processor takeover
                     break
             elif c in [" ", NEW_LINE] and section not in ["DICT_KEY", "DICT_VAL"]:
                 pass
             else:
                 if section == "KEY_TO_VALUE":
                     # We found a value directly after the key, unquoted
                     # That means it's either a variable, or a number
                     if c.isnumeric():
                         section = "INT_VALUE"
                     else:
                         section = "VAR_VALUE"
                 if section in ["DICT_KEY", "DICT_VAL", "INT_VALUE", "VAR_VALUE"]:
                     current_phrase += c
-
         return result
 
-    def _parse_list(self, original: str, tokenizer: ClauseTokenizer) -> Any:
+    @staticmethod
+    def _parse_list(original: str, tokenizer: ClauseTokenizer) -> List[Any]:  # type: ignore
         result: List[Any] = list()
         section = None
         current_phrase = ""
         while True:
             c = tokenizer.next()
             if not c:
                 break
             if c == "{":
                 tokenizer.revert()  # Ensure we start the new parser with the initial {
-                result.append(self.parse(original, tokenizer, only_parse_initial=True))
+                result.append(
+                    JsonParser._get_next_document(
+                        original, tokenizer, only_parse_initial=True
+                    )
+                )
                 if tokenizer.current() == "]":
                     break
                 tokenizer.skip_until([","])
                 tokenizer.skip_white_space()
             elif c in ACCEPTED_QUOTES and section is None:
                 section = "VALUE"
             elif c in ACCEPTED_QUOTES and section == "VALUE":
```

### Comparing `py_partiql_parser-0.5.4/py_partiql_parser/_internal/parser.py` & `py_partiql_parser-0.5.5/py_partiql_parser/_internal/parser.py`

 * *Files identical despite different names*

### Comparing `py_partiql_parser-0.5.4/py_partiql_parser/_internal/select_parser.py` & `py_partiql_parser-0.5.5/py_partiql_parser/_internal/select_parser.py`

 * *Files identical despite different names*

### Comparing `py_partiql_parser-0.5.4/py_partiql_parser/_internal/update_parser.py` & `py_partiql_parser-0.5.5/py_partiql_parser/_internal/update_parser.py`

 * *Files identical despite different names*

### Comparing `py_partiql_parser-0.5.4/py_partiql_parser/_internal/utils.py` & `py_partiql_parser-0.5.5/py_partiql_parser/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `py_partiql_parser-0.5.4/py_partiql_parser/_internal/where_parser.py` & `py_partiql_parser-0.5.5/py_partiql_parser/_internal/where_parser.py`

 * *Files identical despite different names*

### Comparing `py_partiql_parser-0.5.4/py_partiql_parser/_packages/boto3/types.py` & `py_partiql_parser-0.5.5/py_partiql_parser/_packages/boto3/types.py`

 * *Files identical despite different names*

### Comparing `py_partiql_parser-0.5.4/.gitignore` & `py_partiql_parser-0.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `py_partiql_parser-0.5.4/LICENSE` & `py_partiql_parser-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py_partiql_parser-0.5.4/README.md` & `py_partiql_parser-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `py_partiql_parser-0.5.4/pyproject.toml` & `py_partiql_parser-0.5.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "py-partiql-parser"
-version = "0.5.4"
+version = "0.5.5"
 description = "Pure Python PartiQL Parser"
 readme = "README.md"
 keywords = ["pypartiql", "parser"]
 license = {text = "MIT"}
 authors = [{name="Bert Blommers", email="info@bertblommers.nl"}]
 
 dependencies = []
```

### Comparing `py_partiql_parser-0.5.4/PKG-INFO` & `py_partiql_parser-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: py-partiql-parser
-Version: 0.5.4
+Version: 0.5.5
 Summary: Pure Python PartiQL Parser
 Project-URL: Homepage, https://github.com/getmoto/py-partiql-parser
 Project-URL: Bug Tracker, https://github.com/getmoto/py-partiql-parser/issues
 Project-URL: ChangeLog, https://github.com/getmoto/py-partiql-parser/blob/main/CHANGELOG.md
 Author-email: Bert Blommers <info@bertblommers.nl>
 License: MIT
 License-File: LICENSE
```

