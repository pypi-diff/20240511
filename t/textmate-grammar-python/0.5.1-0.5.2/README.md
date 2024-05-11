# Comparing `tmp/textmate_grammar_python-0.5.1.tar.gz` & `tmp/textmate_grammar_python-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textmate_grammar_python-0.5.1.tar", max compression
+gzip compressed data, was "textmate_grammar_python-0.5.2.tar", max compression
```

## Comparing `textmate_grammar_python-0.5.1.tar` & `textmate_grammar_python-0.5.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1069 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/LICENSE
--rw-r--r--   0        0        0     5028 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/README.md
--rw-r--r--   0        0        0     2454 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/__init__.py
--rw-r--r--   0        0        0    20035 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/elements.py
--rw-r--r--   0        0        0    12051 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/handler.py
--rw-r--r--   0        0        0    35912 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/parser.py
--rw-r--r--   0        0        0        0 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/parsers/__init__.py
--rw-r--r--   0        0        0     6930 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/parsers/base.py
--rw-r--r--   0        0        0     1076 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/parsers/markdown/LICENSE.txt
--rw-r--r--   0        0        0      770 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/parsers/markdown/__init__.py
--rw-r--r--   0        0        0    22103 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/parsers/markdown/grammar.yaml
--rw-r--r--   0        0        0     2074 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/parsers/matlab/__init__.py
--rw-r--r--   0        0        0    36373 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/parsers/matlab/grammar.yaml
--rw-r--r--   0        0        0     1271 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/parsers/matlab/license.txt
--rw-r--r--   0        0        0        0 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/py.typed
--rw-r--r--   0        0        0        0 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/utils/__init__.py
--rw-r--r--   0        0        0     5107 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/utils/cache.py
--rw-r--r--   0        0        0     2133 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/utils/exceptions.py
--rw-r--r--   0        0        0     5673 2024-05-09 11:07:52.663096 textmate_grammar_python-0.5.1/src/textmate_grammar/utils/logger.py
--rw-r--r--   0        0        0     5990 1970-01-01 00:00:00.000000 textmate_grammar_python-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-11 10:24:22.058885 textmate_grammar_python-0.5.2/LICENSE
+-rw-r--r--   0        0        0     5028 2024-05-11 10:24:22.058885 textmate_grammar_python-0.5.2/README.md
+-rw-r--r--   0        0        0     2454 2024-05-11 10:24:22.058885 textmate_grammar_python-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-11 10:24:22.058885 textmate_grammar_python-0.5.2/src/textmate_grammar/__init__.py
+-rw-r--r--   0        0        0    20035 2024-05-11 10:24:22.058885 textmate_grammar_python-0.5.2/src/textmate_grammar/elements.py
+-rw-r--r--   0        0        0    12051 2024-05-11 10:24:22.058885 textmate_grammar_python-0.5.2/src/textmate_grammar/handler.py
+-rw-r--r--   0        0        0    35912 2024-05-11 10:24:22.058885 textmate_grammar_python-0.5.2/src/textmate_grammar/parser.py
+-rw-r--r--   0        0        0        0 2024-05-11 10:24:22.058885 textmate_grammar_python-0.5.2/src/textmate_grammar/parsers/__init__.py
+-rw-r--r--   0        0        0     6930 2024-05-11 10:24:22.058885 textmate_grammar_python-0.5.2/src/textmate_grammar/parsers/base.py
+-rw-r--r--   0        0        0     1076 2024-05-11 10:24:22.058885 textmate_grammar_python-0.5.2/src/textmate_grammar/parsers/markdown/LICENSE.txt
+-rw-r--r--   0        0        0      770 2024-05-11 10:24:22.058885 textmate_grammar_python-0.5.2/src/textmate_grammar/parsers/markdown/__init__.py
+-rw-r--r--   0        0        0    22103 2024-05-11 10:24:22.058885 textmate_grammar_python-0.5.2/src/textmate_grammar/parsers/markdown/grammar.yaml
+-rw-r--r--   0        0        0     2130 2024-05-11 10:24:22.062885 textmate_grammar_python-0.5.2/src/textmate_grammar/parsers/matlab/__init__.py
+-rw-r--r--   0        0        0    36373 2024-05-11 10:24:22.062885 textmate_grammar_python-0.5.2/src/textmate_grammar/parsers/matlab/grammar.yaml
+-rw-r--r--   0        0        0     1271 2024-05-11 10:24:22.062885 textmate_grammar_python-0.5.2/src/textmate_grammar/parsers/matlab/license.txt
+-rw-r--r--   0        0        0        0 2024-05-11 10:24:22.062885 textmate_grammar_python-0.5.2/src/textmate_grammar/py.typed
+-rw-r--r--   0        0        0        0 2024-05-11 10:24:22.062885 textmate_grammar_python-0.5.2/src/textmate_grammar/utils/__init__.py
+-rw-r--r--   0        0        0     5107 2024-05-11 10:24:22.062885 textmate_grammar_python-0.5.2/src/textmate_grammar/utils/cache.py
+-rw-r--r--   0        0        0     2133 2024-05-11 10:24:22.062885 textmate_grammar_python-0.5.2/src/textmate_grammar/utils/exceptions.py
+-rw-r--r--   0        0        0     5673 2024-05-11 10:24:22.062885 textmate_grammar_python-0.5.2/src/textmate_grammar/utils/logger.py
+-rw-r--r--   0        0        0     5990 1970-01-01 00:00:00.000000 textmate_grammar_python-0.5.2/PKG-INFO
```

### Comparing `textmate_grammar_python-0.5.1/LICENSE` & `textmate_grammar_python-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `textmate_grammar_python-0.5.1/README.md` & `textmate_grammar_python-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `textmate_grammar_python-0.5.1/pyproject.toml` & `textmate_grammar_python-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "textmate-grammar-python"
-version = "0.5.1"
+version = "0.5.2"
 description = "A lexer and tokenizer for grammar files as defined by TextMate and used in VSCode, implemented in Python."
 authors = ["Mark Shui Hu <watermarkhu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/watermarkhu/textmate-grammar-python"
 documentation = "https://textmate-grammar-python.readthedocs.io"
 keywords = ["textmate", "tokenization"]
```

### Comparing `textmate_grammar_python-0.5.1/src/textmate_grammar/elements.py` & `textmate_grammar_python-0.5.2/src/textmate_grammar/elements.py`

 * *Files identical despite different names*

### Comparing `textmate_grammar_python-0.5.1/src/textmate_grammar/handler.py` & `textmate_grammar_python-0.5.2/src/textmate_grammar/handler.py`

 * *Files identical despite different names*

### Comparing `textmate_grammar_python-0.5.1/src/textmate_grammar/parser.py` & `textmate_grammar_python-0.5.2/src/textmate_grammar/parser.py`

 * *Files identical despite different names*

### Comparing `textmate_grammar_python-0.5.1/src/textmate_grammar/parsers/base.py` & `textmate_grammar_python-0.5.2/src/textmate_grammar/parsers/base.py`

 * *Files identical despite different names*

### Comparing `textmate_grammar_python-0.5.1/src/textmate_grammar/parsers/markdown/LICENSE.txt` & `textmate_grammar_python-0.5.2/src/textmate_grammar/parsers/markdown/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `textmate_grammar_python-0.5.1/src/textmate_grammar/parsers/markdown/__init__.py` & `textmate_grammar_python-0.5.2/src/textmate_grammar/parsers/markdown/__init__.py`

 * *Files identical despite different names*

### Comparing `textmate_grammar_python-0.5.1/src/textmate_grammar/parsers/markdown/grammar.yaml` & `textmate_grammar_python-0.5.2/src/textmate_grammar/parsers/markdown/grammar.yaml`

 * *Files identical despite different names*

### Comparing `textmate_grammar_python-0.5.1/src/textmate_grammar/parsers/matlab/__init__.py` & `textmate_grammar_python-0.5.2/src/textmate_grammar/parsers/matlab/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -56,14 +56,16 @@
             input = self._remove_line_continuations(input)
         return input
 
     def _remove_line_continuations(self, input: str) -> str:
         """
         Removes line continuations from the input text.
         """
+        if "..." not in input:
+            return input
         output = ""
         for split in input.split("..."):
             matching = re.search(r"\n[\t\f\v ]*", split)
             if matching:
                 output += split[matching.span()[1] :]
             else:
                 output += split
```

### Comparing `textmate_grammar_python-0.5.1/src/textmate_grammar/parsers/matlab/grammar.yaml` & `textmate_grammar_python-0.5.2/src/textmate_grammar/parsers/matlab/grammar.yaml`

 * *Files identical despite different names*

### Comparing `textmate_grammar_python-0.5.1/src/textmate_grammar/parsers/matlab/license.txt` & `textmate_grammar_python-0.5.2/src/textmate_grammar/parsers/matlab/license.txt`

 * *Files identical despite different names*

### Comparing `textmate_grammar_python-0.5.1/src/textmate_grammar/utils/cache.py` & `textmate_grammar_python-0.5.2/src/textmate_grammar/utils/cache.py`

 * *Files identical despite different names*

### Comparing `textmate_grammar_python-0.5.1/src/textmate_grammar/utils/exceptions.py` & `textmate_grammar_python-0.5.2/src/textmate_grammar/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `textmate_grammar_python-0.5.1/src/textmate_grammar/utils/logger.py` & `textmate_grammar_python-0.5.2/src/textmate_grammar/utils/logger.py`

 * *Files identical despite different names*

### Comparing `textmate_grammar_python-0.5.1/PKG-INFO` & `textmate_grammar_python-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textmate-grammar-python
-Version: 0.5.1
+Version: 0.5.2
 Summary: A lexer and tokenizer for grammar files as defined by TextMate and used in VSCode, implemented in Python.
 Home-page: https://github.com/watermarkhu/textmate-grammar-python
 License: MIT
 Keywords: textmate,tokenization
 Author: Mark Shui Hu
 Author-email: watermarkhu@gmail.com
 Requires-Python: >=3.9,<4.0
```

