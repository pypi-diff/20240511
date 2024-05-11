# Comparing `tmp/pdfsyntax-0.1.0.tar.gz` & `tmp/pdfsyntax-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfsyntax-0.1.0.tar", last modified: Sun Apr 14 20:58:52 2024, max compression
+gzip compressed data, was "pdfsyntax-0.1.1.tar", last modified: Sat May 11 15:01:57 2024, max compression
```

## Comparing `pdfsyntax-0.1.0.tar` & `pdfsyntax-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 dej       (1000) dej       (1000)        0 2024-04-14 20:58:52.217604 pdfsyntax-0.1.0/
--rw-r--r--   0 dej       (1000) dej       (1000)     1092 2024-01-20 19:09:05.000000 pdfsyntax-0.1.0/LICENSE
--rw-r--r--   0 dej       (1000) dej       (1000)     6011 2024-04-14 20:58:52.216604 pdfsyntax-0.1.0/PKG-INFO
--rw-r--r--   0 dej       (1000) dej       (1000)     4019 2024-04-14 16:40:39.000000 pdfsyntax-0.1.0/README.md
-drwxr-xr-x   0 dej       (1000) dej       (1000)        0 2024-04-14 20:58:52.205604 pdfsyntax-0.1.0/pdfsyntax/
--rw-r--r--   0 dej       (1000) dej       (1000)       58 2022-08-09 20:53:21.000000 pdfsyntax-0.1.0/pdfsyntax/__init__.py
--rw-r--r--   0 dej       (1000) dej       (1000)       32 2022-05-02 17:43:04.000000 pdfsyntax-0.1.0/pdfsyntax/__main__.py
--rw-r--r--   0 dej       (1000) dej       (1000)     9155 2024-03-17 19:03:38.000000 pdfsyntax-0.1.0/pdfsyntax/api.py
--rw-r--r--   0 dej       (1000) dej       (1000)    11497 2024-04-14 16:30:54.000000 pdfsyntax-0.1.0/pdfsyntax/cli.py
--rw-r--r--   0 dej       (1000) dej       (1000)     9185 2023-12-31 21:04:26.000000 pdfsyntax-0.1.0/pdfsyntax/display.py
--rw-r--r--   0 dej       (1000) dej       (1000)    23271 2024-04-14 15:39:42.000000 pdfsyntax-0.1.0/pdfsyntax/docstruct.py
--rw-r--r--   0 dej       (1000) dej       (1000)    21565 2024-04-14 09:53:18.000000 pdfsyntax-0.1.0/pdfsyntax/filestruct.py
--rw-r--r--   0 dej       (1000) dej       (1000)     4131 2024-04-13 21:33:36.000000 pdfsyntax-0.1.0/pdfsyntax/filters.py
--rw-r--r--   0 dej       (1000) dej       (1000)     4672 2023-12-29 22:30:13.000000 pdfsyntax-0.1.0/pdfsyntax/graphics.py
--rw-r--r--   0 dej       (1000) dej       (1000)     4561 2023-12-29 22:31:00.000000 pdfsyntax-0.1.0/pdfsyntax/layout.py
--rw-r--r--   0 dej       (1000) dej       (1000)    16331 2024-04-14 09:54:39.000000 pdfsyntax-0.1.0/pdfsyntax/objects.py
--rw-r--r--   0 dej       (1000) dej       (1000)     7093 2024-01-14 16:11:22.000000 pdfsyntax-0.1.0/pdfsyntax/text.py
-drwxr-xr-x   0 dej       (1000) dej       (1000)        0 2024-04-14 20:58:52.216604 pdfsyntax-0.1.0/pdfsyntax.egg-info/
--rw-r--r--   0 dej       (1000) dej       (1000)     6011 2024-04-14 20:58:52.000000 pdfsyntax-0.1.0/pdfsyntax.egg-info/PKG-INFO
--rw-r--r--   0 dej       (1000) dej       (1000)      622 2024-04-14 20:58:52.000000 pdfsyntax-0.1.0/pdfsyntax.egg-info/SOURCES.txt
--rw-r--r--   0 dej       (1000) dej       (1000)        1 2024-04-14 20:58:52.000000 pdfsyntax-0.1.0/pdfsyntax.egg-info/dependency_links.txt
--rw-r--r--   0 dej       (1000) dej       (1000)       10 2024-04-14 20:58:52.000000 pdfsyntax-0.1.0/pdfsyntax.egg-info/top_level.txt
--rw-r--r--   0 dej       (1000) dej       (1000)      855 2024-04-14 20:46:18.000000 pdfsyntax-0.1.0/pyproject.toml
--rw-r--r--   0 dej       (1000) dej       (1000)       38 2024-04-14 20:58:52.217604 pdfsyntax-0.1.0/setup.cfg
-drwxr-xr-x   0 dej       (1000) dej       (1000)        0 2024-04-14 20:58:52.215604 pdfsyntax-0.1.0/tests/
--rw-r--r--   0 dej       (1000) dej       (1000)     1499 2024-01-06 20:43:45.000000 pdfsyntax-0.1.0/tests/test_bdata.py
--rw-r--r--   0 dej       (1000) dej       (1000)      705 2023-09-10 19:21:38.000000 pdfsyntax-0.1.0/tests/test_dependencies.py
--rw-r--r--   0 dej       (1000) dej       (1000)     2668 2023-06-29 21:07:04.000000 pdfsyntax-0.1.0/tests/test_parsing.py
--rw-r--r--   0 dej       (1000) dej       (1000)      303 2022-09-13 20:49:14.000000 pdfsyntax-0.1.0/tests/test_serialization.py
--rw-r--r--   0 dej       (1000) dej       (1000)      458 2023-09-10 19:21:40.000000 pdfsyntax-0.1.0/tests/test_simplefile.py
--rw-r--r--   0 dej       (1000) dej       (1000)     1044 2023-04-20 21:04:55.000000 pdfsyntax-0.1.0/tests/test_text.py
--rw-r--r--   0 dej       (1000) dej       (1000)     2548 2024-03-29 23:39:04.000000 pdfsyntax-0.1.0/tests/test_tokenization.py
--rw-r--r--   0 dej       (1000) dej       (1000)      359 2023-09-10 19:21:36.000000 pdfsyntax-0.1.0/tests/test_updating.py
--rw-r--r--   0 dej       (1000) dej       (1000)      980 2024-04-07 15:30:15.000000 pdfsyntax-0.1.0/tests/test_xref.py
+drwxr-xr-x   0 dej       (1000) dej       (1000)        0 2024-05-11 15:01:57.101629 pdfsyntax-0.1.1/
+-rw-r--r--   0 dej       (1000) dej       (1000)     1092 2024-01-20 19:09:05.000000 pdfsyntax-0.1.1/LICENSE
+-rw-r--r--   0 dej       (1000) dej       (1000)     4762 2024-05-11 15:01:57.098629 pdfsyntax-0.1.1/PKG-INFO
+-rw-r--r--   0 dej       (1000) dej       (1000)     4019 2024-04-14 16:40:39.000000 pdfsyntax-0.1.1/README.md
+drwxr-xr-x   0 dej       (1000) dej       (1000)        0 2024-05-11 15:01:57.077629 pdfsyntax-0.1.1/pdfsyntax/
+-rw-r--r--   0 dej       (1000) dej       (1000)       58 2022-08-09 20:53:21.000000 pdfsyntax-0.1.1/pdfsyntax/__init__.py
+-rw-r--r--   0 dej       (1000) dej       (1000)       32 2022-05-02 17:43:04.000000 pdfsyntax-0.1.1/pdfsyntax/__main__.py
+-rw-r--r--   0 dej       (1000) dej       (1000)     9221 2024-05-11 14:32:53.000000 pdfsyntax-0.1.1/pdfsyntax/api.py
+-rw-r--r--   0 dej       (1000) dej       (1000)    11497 2024-04-14 16:30:54.000000 pdfsyntax-0.1.1/pdfsyntax/cli.py
+-rw-r--r--   0 dej       (1000) dej       (1000)     9185 2023-12-31 21:04:26.000000 pdfsyntax-0.1.1/pdfsyntax/display.py
+-rw-r--r--   0 dej       (1000) dej       (1000)    24273 2024-05-10 22:00:23.000000 pdfsyntax-0.1.1/pdfsyntax/docstruct.py
+-rw-r--r--   0 dej       (1000) dej       (1000)    21581 2024-05-08 19:35:00.000000 pdfsyntax-0.1.1/pdfsyntax/filestruct.py
+-rw-r--r--   0 dej       (1000) dej       (1000)     4131 2024-05-11 14:32:28.000000 pdfsyntax-0.1.1/pdfsyntax/filters.py
+-rw-r--r--   0 dej       (1000) dej       (1000)     4672 2023-12-29 22:30:13.000000 pdfsyntax-0.1.1/pdfsyntax/graphics.py
+-rw-r--r--   0 dej       (1000) dej       (1000)     4561 2023-12-29 22:31:00.000000 pdfsyntax-0.1.1/pdfsyntax/layout.py
+-rw-r--r--   0 dej       (1000) dej       (1000)     8523 2024-05-09 09:08:00.000000 pdfsyntax-0.1.1/pdfsyntax/markdown.py
+-rw-r--r--   0 dej       (1000) dej       (1000)    16506 2024-05-11 14:28:49.000000 pdfsyntax-0.1.1/pdfsyntax/objects.py
+-rw-r--r--   0 dej       (1000) dej       (1000)     7093 2024-01-14 16:11:22.000000 pdfsyntax-0.1.1/pdfsyntax/text.py
+drwxr-xr-x   0 dej       (1000) dej       (1000)        0 2024-05-11 15:01:57.097629 pdfsyntax-0.1.1/pdfsyntax.egg-info/
+-rw-r--r--   0 dej       (1000) dej       (1000)     4762 2024-05-11 15:01:57.000000 pdfsyntax-0.1.1/pdfsyntax.egg-info/PKG-INFO
+-rw-r--r--   0 dej       (1000) dej       (1000)      644 2024-05-11 15:01:57.000000 pdfsyntax-0.1.1/pdfsyntax.egg-info/SOURCES.txt
+-rw-r--r--   0 dej       (1000) dej       (1000)        1 2024-05-11 15:01:57.000000 pdfsyntax-0.1.1/pdfsyntax.egg-info/dependency_links.txt
+-rw-r--r--   0 dej       (1000) dej       (1000)       10 2024-05-11 15:01:57.000000 pdfsyntax-0.1.1/pdfsyntax.egg-info/top_level.txt
+-rw-r--r--   0 dej       (1000) dej       (1000)      861 2024-05-11 14:57:38.000000 pdfsyntax-0.1.1/pyproject.toml
+-rw-r--r--   0 dej       (1000) dej       (1000)       38 2024-05-11 15:01:57.102630 pdfsyntax-0.1.1/setup.cfg
+drwxr-xr-x   0 dej       (1000) dej       (1000)        0 2024-05-11 15:01:57.097629 pdfsyntax-0.1.1/tests/
+-rw-r--r--   0 dej       (1000) dej       (1000)     1499 2024-01-06 20:43:45.000000 pdfsyntax-0.1.1/tests/test_bdata.py
+-rw-r--r--   0 dej       (1000) dej       (1000)      705 2023-09-10 19:21:38.000000 pdfsyntax-0.1.1/tests/test_dependencies.py
+-rw-r--r--   0 dej       (1000) dej       (1000)     2668 2023-06-29 21:07:04.000000 pdfsyntax-0.1.1/tests/test_parsing.py
+-rw-r--r--   0 dej       (1000) dej       (1000)      303 2022-09-13 20:49:14.000000 pdfsyntax-0.1.1/tests/test_serialization.py
+-rw-r--r--   0 dej       (1000) dej       (1000)      458 2023-09-10 19:21:40.000000 pdfsyntax-0.1.1/tests/test_simplefile.py
+-rw-r--r--   0 dej       (1000) dej       (1000)     1044 2023-04-20 21:04:55.000000 pdfsyntax-0.1.1/tests/test_text.py
+-rw-r--r--   0 dej       (1000) dej       (1000)     2548 2024-03-29 23:39:04.000000 pdfsyntax-0.1.1/tests/test_tokenization.py
+-rw-r--r--   0 dej       (1000) dej       (1000)      359 2023-09-10 19:21:36.000000 pdfsyntax-0.1.1/tests/test_updating.py
+-rw-r--r--   0 dej       (1000) dej       (1000)      980 2024-04-07 15:30:15.000000 pdfsyntax-0.1.1/tests/test_xref.py
```

### Comparing `pdfsyntax-0.1.0/LICENSE` & `pdfsyntax-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfsyntax-0.1.0/PKG-INFO` & `pdfsyntax-0.1.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,13 @@
 Metadata-Version: 2.1
 Name: pdfsyntax
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python library to inspect and modify the internal structure of a PDF file
 Author-email: "Martin D." <desgeeko@gmail.com>
-License: MIT License
-        
-        Copyright (c) 2022-2024 Martin D. <desgeeko@gmail.com>
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
+License: MIT license
 Project-URL: Homepage, https://github.com/desgeeko/pdfsyntax
 Project-URL: Bug Tracker, https://github.com/desgeeko/pdfsyntax/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pdfsyntax-0.1.0/README.md` & `pdfsyntax-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pdfsyntax-0.1.0/pdfsyntax/api.py` & `pdfsyntax-0.1.1/pdfsyntax/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from copy import deepcopy
 from .docstruct import *
 from .filestruct import *
 from .objects import *
 from .text import *
 from .graphics import *
 from .layout import *
+from .markdown import *
 
 
 METADATA_ATTRS = '/Title /Author /Subject /Keywords /Creator /Producer'.split()
 
 def in2pt(inches: float) -> int:
     """Convert inches into points."""
     return int(inches*72)
@@ -158,27 +159,28 @@
         obj = deepcopy(get_object(doc, iref))
         obj['/Rotate'] = (old_degrees + degrees) % 360
         doc = update_object(doc, int(iref.imag), obj)
     return doc
 
 
 def flate_compress(doc: Doc) -> Doc:
-    """Squash doc and apply FlateDecode filter on all streams."""
-    doc = squash(doc)
-    cache = doc.cache
-    for i, o in enumerate(cache):
+    """Apply FlateDecode filter on all streams and squash doc."""
+    for iref in in_use(doc):
+        o = get_object(doc, iref)
         if type(o) == Stream:
             entries = o['entries']
             if '/Filter' in entries and entries['/Filter'] == '/FlateDecode':
                 continue
             else:
                 entries = deepcopy(entries)
                 entries['/Filter'] = '/FlateDecode'
                 s, length = forge_stream(entries, o['stream'])
+                i = int(iref.imag)
                 doc = update_object(doc, i, s)
+    doc = squash(doc)
     return doc
 
 
 def add_text_annotation(doc: Doc, page_num: int, text: str, rect: list, opened: bool = False) -> Doc:
     """Add simple text annotation."""
     annot = {
         '/Type': '/Annot',
```

### Comparing `pdfsyntax-0.1.0/pdfsyntax/cli.py` & `pdfsyntax-0.1.1/pdfsyntax/cli.py`

 * *Files identical despite different names*

### Comparing `pdfsyntax-0.1.0/pdfsyntax/display.py` & `pdfsyntax-0.1.1/pdfsyntax/display.py`

 * *Files identical despite different names*

### Comparing `pdfsyntax-0.1.0/pdfsyntax/docstruct.py` & `pdfsyntax-0.1.1/pdfsyntax/docstruct.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,36 @@
             res += f", cache=None>\n"
         return res
 
 EOL = b'\r\n'
 SPACE = EOL + b'\x00\x09\x0c\x20'
 
 
+def pprint_cache(doc: Doc):
+    """."""
+    idx = {}
+    for iref, action in changes(doc):
+        idx[int(iref.imag)] = action
+    markers = '0123456789'
+    header = ' ' * 6 + markers
+    print(header)
+    line = ''
+    for i, x in enumerate(doc.cache):
+        status = idx.get(i, 'x')
+        if status == 'x' and doc.cache[i] is None:
+            status = '-'
+        line += status
+        if i % 10 == 9 or i == len(doc.cache) - 1:
+            prefix = f"{(i-i%10)//10}_"
+            line = f"{prefix:>5} " + line
+            print(line)
+            line = ''
+    print(line)
+
+
 def memoize_obj_in_cache(idx: list, fdata: Callable, key: int, cache=None, rev=-1) -> list:
     """Parse indirect object whose number is [key] and return a cache filled at index [key].
 
     cache argument may be:
     - a list that is updated
     - or None that is replaced with an empty list
     """
@@ -114,14 +136,22 @@
         ref = int(obj.imag)
         res = memoize_obj_in_cache(doc.index, doc.data[-1]['fdata'], ref, doc.cache)
         return deepcopy(res[ref])
     else: 
         return deepcopy(obj)
 
 
+def object(doc: Doc, o_num, o_gen = None):
+    """For direct access to an indirect object without reference resolution (see get_object)."""
+    if o_gen is None:
+        o_gen = doc.index[-1][o_num]['o_gen']
+    iref = complex(o_gen, o_num)
+    return get_object(doc, iref)
+
+
 def flat_page_tree(doc: Doc, num=None, inherited={}, max_nb=None) -> list:
     """Recursively list the pages of a node."""
     accu = []
     if num:
         node = get_object(doc, num)
     else:
         node = get_object(doc, catalog(doc)[0]['/Pages'])
@@ -144,39 +174,44 @@
     memoize_obj_in_cache(index, fdata, 0, cache)
     return cache
 
 
 def get_iref(doc: Doc, o_num: int, rev: int=-1) -> complex:
     """Build the relevant indirect reference for o_num in a doc revision."""
     current = doc.index[rev]
-    o_gen = current[o_num]['o_gen']
-    return complex(o_gen, o_num)
+    if current[o_num]:
+        o_gen = current[o_num]['o_gen']
+        return complex(o_gen, o_num)
+    else:
+        return None
 
 
 def in_use(doc: Doc, rev: int=-1) -> list:
-    """List objects in use (not deleted)."""
+    """List objects in use (not empty from the start and not deleted)."""
     res = []
     current = doc.index[rev]
     for i in range(1, len(current)):
         iref = get_iref(doc, i, rev)
-        if 'DELETED' not in current[i]:
+        if iref and 'DELETED' not in current[i]:
             res.append(iref)
     return res
 
 
 def changes(doc: Doc, rev: int=-1):
     """List deleted/updated/added objects."""
     res = []
     current = doc.index[rev]
     if len(doc.index) == 1:
         previous = [None] * len(current)
     else:
         previous = doc.index[rev-1]
     for i in range(1, len(current)):
         iref = get_iref(doc, i, rev)
+        if not iref:
+            continue
         if i > len(previous)-1:
             res.append((iref, 'a'))
         elif i < len(previous) and previous[i] == current[i]:
             pass
         elif previous[i] != None and 'DELETED' not in previous[i] and 'DELETED' in current[i]:
             res.append((iref, 'd'))
         elif previous[i] != None and current[i] != previous[i]:
```

### Comparing `pdfsyntax-0.1.0/pdfsyntax/filestruct.py` & `pdfsyntax-0.1.1/pdfsyntax/filestruct.py`

 * *Files 0% similar despite different names*

```diff
@@ -578,15 +578,16 @@
     """ """
     HEADER = b'%PDF-X.Y'
     bdata, a0, o0, _ = fdata(len(HEADER), 1024 - len(HEADER))
     i, j, _ = next_token(bdata, a0) #comment
     i, j, _ = next_token(bdata, j)  #o_num
     i, j, _ = next_token(bdata, j)  #gen_num
     i, j, _ = next_token(bdata, j)  #obj keyword
-    i, _, t = next_token(bdata, j)  #dict ?
+    i, j, t = next_token(bdata, j)  #dict ?
     if t == 'DICT':
-        first_obj = parse_obj(bdata, i)
+        o = bdata[i:j]
+        first_obj = parse_obj(o)
         if type(first_obj) == dict and '/Linearized' in first_obj:
             return first_obj
     return None
```

### Comparing `pdfsyntax-0.1.0/pdfsyntax/filters.py` & `pdfsyntax-0.1.1/pdfsyntax/filters.py`

 * *Files identical despite different names*

### Comparing `pdfsyntax-0.1.0/pdfsyntax/graphics.py` & `pdfsyntax-0.1.1/pdfsyntax/graphics.py`

 * *Files identical despite different names*

### Comparing `pdfsyntax-0.1.0/pdfsyntax/layout.py` & `pdfsyntax-0.1.1/pdfsyntax/layout.py`

 * *Files identical despite different names*

### Comparing `pdfsyntax-0.1.0/pdfsyntax/objects.py` & `pdfsyntax-0.1.1/pdfsyntax/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,14 +148,16 @@
         elif search == "STREAM":
             if text[i:i+11] == b'\r\nendstream':
                 return (h, i+11, 'STREAM')
             elif  text[i:i+10] == b'\nendstream':
                 return (h, i+10, 'STREAM')
             elif  text[i:i+10] == b'\rendstream':
                 return (h, i+10, 'STREAM')
+            elif  text[i:i+9] == b'endstream':
+                return (h, i+9, 'STREAM')
         elif search == "ARRAY":
             if single == b'(':
                 text_in_array = 1
             elif single == b')':
                 text_in_array = 0
             elif text_in_array == 0 and single == b'[':
                 nested += 1
@@ -252,26 +254,29 @@
         return res
     elif t1 == 'STREAM':
         b1 = b'stream' + b'\r\n'
         b2 = b'stream' + b'\n'
         e1 = b'\r\n' + b'endstream'
         e2 = b'\n' + b'endstream'
         e3 = b'\r' + b'endstream'
+        e4 = b'endstream'
         if obj[:len(b1)] == b1:
             b = len(b1)
         elif obj[:len(b2)] == b2:
             b = len(b2)
         else:
             return None
         if obj[-len(e1):] == e1:
             e = len(e1)
         elif obj[-len(e2):] == e2:
             e = len(e2)
         elif obj[-len(e3):] == e3:
             e = len(e3)
+        elif obj[-len(e4):] == e4:
+            e = len(e4)
         else:
             return None
         s = obj[b:-e]
         return s
     elif t1 == 'COMMENT':
         return ''
     else:
@@ -465,15 +470,15 @@
             ret += b' '
             ret += value
             ret += b' '
         ret += b' ' * depth
         ret += b'>>'
         if content:
             ret += b'\nstream\n'
-            ret += b'\n'
+            #ret += b'\n'
             ret += content
             ret += b'\nendstream'
     elif type(obj) == list:
         ret += b'[ '
         for i in obj:
             value = serialize(i)
             ret += value
```

### Comparing `pdfsyntax-0.1.0/pdfsyntax/text.py` & `pdfsyntax-0.1.1/pdfsyntax/text.py`

 * *Files identical despite different names*

### Comparing `pdfsyntax-0.1.0/pdfsyntax.egg-info/PKG-INFO` & `pdfsyntax-0.1.1/pdfsyntax.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,13 @@
 Metadata-Version: 2.1
 Name: pdfsyntax
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python library to inspect and modify the internal structure of a PDF file
 Author-email: "Martin D." <desgeeko@gmail.com>
-License: MIT License
-        
-        Copyright (c) 2022-2024 Martin D. <desgeeko@gmail.com>
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
+License: MIT license
 Project-URL: Homepage, https://github.com/desgeeko/pdfsyntax
 Project-URL: Bug Tracker, https://github.com/desgeeko/pdfsyntax/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pdfsyntax-0.1.0/pdfsyntax.egg-info/SOURCES.txt` & `pdfsyntax-0.1.1/pdfsyntax.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 pdfsyntax/cli.py
 pdfsyntax/display.py
 pdfsyntax/docstruct.py
 pdfsyntax/filestruct.py
 pdfsyntax/filters.py
 pdfsyntax/graphics.py
 pdfsyntax/layout.py
+pdfsyntax/markdown.py
 pdfsyntax/objects.py
 pdfsyntax/text.py
 pdfsyntax.egg-info/PKG-INFO
 pdfsyntax.egg-info/SOURCES.txt
 pdfsyntax.egg-info/dependency_links.txt
 pdfsyntax.egg-info/top_level.txt
 tests/test_bdata.py
```

### Comparing `pdfsyntax-0.1.0/tests/test_bdata.py` & `pdfsyntax-0.1.1/tests/test_bdata.py`

 * *Files identical despite different names*

### Comparing `pdfsyntax-0.1.0/tests/test_dependencies.py` & `pdfsyntax-0.1.1/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `pdfsyntax-0.1.0/tests/test_parsing.py` & `pdfsyntax-0.1.1/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `pdfsyntax-0.1.0/tests/test_text.py` & `pdfsyntax-0.1.1/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `pdfsyntax-0.1.0/tests/test_tokenization.py` & `pdfsyntax-0.1.1/tests/test_tokenization.py`

 * *Files identical despite different names*

### Comparing `pdfsyntax-0.1.0/tests/test_xref.py` & `pdfsyntax-0.1.1/tests/test_xref.py`

 * *Files identical despite different names*

