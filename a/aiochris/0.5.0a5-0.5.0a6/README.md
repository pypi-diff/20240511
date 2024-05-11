# Comparing `tmp/aiochris-0.5.0a5.tar.gz` & `tmp/aiochris-0.5.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiochris-0.5.0a5.tar", max compression
+gzip compressed data, was "aiochris-0.5.0a6.tar", max compression
```

## Comparing `aiochris-0.5.0a5.tar` & `aiochris-0.5.0a6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1069 2024-04-12 20:03:17.466843 aiochris-0.5.0a5/LICENSE
--rw-r--r--   0        0        0     1848 2024-04-12 20:03:17.466843 aiochris-0.5.0a5/README.md
--rw-r--r--   0        0        0      594 2024-04-12 20:03:17.466843 aiochris-0.5.0a5/aiochris/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 20:03:17.466843 aiochris-0.5.0a5/aiochris/client/__init__.py
--rw-r--r--   0        0        0     6250 2024-04-12 20:03:17.466843 aiochris-0.5.0a5/aiochris/client/admin.py
--rw-r--r--   0        0        0     1335 2024-04-12 20:03:17.466843 aiochris-0.5.0a5/aiochris/client/anon.py
--rw-r--r--   0        0        0    11803 2024-04-12 20:03:17.466843 aiochris-0.5.0a5/aiochris/client/authed.py
--rw-r--r--   0        0        0     3820 2024-04-12 20:03:17.466843 aiochris-0.5.0a5/aiochris/client/base.py
--rw-r--r--   0        0        0     4049 2024-04-12 20:03:17.466843 aiochris-0.5.0a5/aiochris/client/from_chrs.py
--rw-r--r--   0        0        0     1702 2024-04-12 20:03:17.466843 aiochris-0.5.0a5/aiochris/client/normal.py
--rw-r--r--   0        0        0      644 2024-04-12 20:03:17.466843 aiochris-0.5.0a5/aiochris/enums.py
--rw-r--r--   0        0        0      788 2024-04-12 20:03:17.466843 aiochris-0.5.0a5/aiochris/errors.py
--rw-r--r--   0        0        0     2284 2024-04-12 20:03:17.466843 aiochris-0.5.0a5/aiochris/examples.md
--rw-r--r--   0        0        0     5231 2024-04-12 20:03:17.466843 aiochris-0.5.0a5/aiochris/home.md
--rw-r--r--   0        0        0       97 2024-04-12 20:03:17.466843 aiochris-0.5.0a5/aiochris/link/__init__.py
--rw-r--r--   0        0        0     1143 2024-04-12 20:03:17.466843 aiochris-0.5.0a5/aiochris/link/collection_client.py
--rw-r--r--   0        0        0     5027 2024-04-12 20:03:17.466843 aiochris-0.5.0a5/aiochris/link/http.py
--rw-r--r--   0        0        0     4659 2024-04-12 20:03:17.466843 aiochris-0.5.0a5/aiochris/link/linked.py
--rw-r--r--   0        0        0     1450 2024-04-12 20:03:17.466843 aiochris-0.5.0a5/aiochris/link/metaprog.py
--rw-r--r--   0        0        0      112 2024-04-12 20:03:17.466843 aiochris-0.5.0a5/aiochris/models/__init__.py
--rw-r--r--   0        0        0     2212 2024-04-12 20:03:17.466843 aiochris-0.5.0a5/aiochris/models/collection_links.py
--rw-r--r--   0        0        0     2898 2024-04-12 20:03:17.466843 aiochris-0.5.0a5/aiochris/models/data.py
--rw-r--r--   0        0        0     7348 2024-04-12 20:03:17.466843 aiochris-0.5.0a5/aiochris/models/logged_in.py
--rw-r--r--   0        0        0     2297 2024-04-12 20:03:17.466843 aiochris-0.5.0a5/aiochris/models/public.py
--rw-r--r--   0        0        0     3175 2024-04-12 20:03:17.466843 aiochris-0.5.0a5/aiochris/types.py
--rw-r--r--   0        0        0       31 2024-04-12 20:03:17.466843 aiochris-0.5.0a5/aiochris/util/__init__.py
--rw-r--r--   0        0        0     6932 2024-04-12 20:03:17.466843 aiochris-0.5.0a5/aiochris/util/search.py
--rw-r--r--   0        0        0     1191 2024-04-12 20:03:17.466843 aiochris-0.5.0a5/pyproject.toml
--rw-r--r--   0        0        0     2690 1970-01-01 00:00:00.000000 aiochris-0.5.0a5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-11 21:41:41.196594 aiochris-0.5.0a6/LICENSE
+-rw-r--r--   0        0        0     1848 2024-05-11 21:41:41.196594 aiochris-0.5.0a6/README.md
+-rw-r--r--   0        0        0      594 2024-05-11 21:41:41.196594 aiochris-0.5.0a6/aiochris/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-11 21:41:41.196594 aiochris-0.5.0a6/aiochris/client/__init__.py
+-rw-r--r--   0        0        0     6250 2024-05-11 21:41:41.196594 aiochris-0.5.0a6/aiochris/client/admin.py
+-rw-r--r--   0        0        0     1335 2024-05-11 21:41:41.196594 aiochris-0.5.0a6/aiochris/client/anon.py
+-rw-r--r--   0        0        0    11803 2024-05-11 21:41:41.196594 aiochris-0.5.0a6/aiochris/client/authed.py
+-rw-r--r--   0        0        0     3820 2024-05-11 21:41:41.196594 aiochris-0.5.0a6/aiochris/client/base.py
+-rw-r--r--   0        0        0     4049 2024-05-11 21:41:41.196594 aiochris-0.5.0a6/aiochris/client/from_chrs.py
+-rw-r--r--   0        0        0     1702 2024-05-11 21:41:41.196594 aiochris-0.5.0a6/aiochris/client/normal.py
+-rw-r--r--   0        0        0      644 2024-05-11 21:41:41.196594 aiochris-0.5.0a6/aiochris/enums.py
+-rw-r--r--   0        0        0      788 2024-05-11 21:41:41.196594 aiochris-0.5.0a6/aiochris/errors.py
+-rw-r--r--   0        0        0     2284 2024-05-11 21:41:41.196594 aiochris-0.5.0a6/aiochris/examples.md
+-rw-r--r--   0        0        0     5231 2024-05-11 21:41:41.196594 aiochris-0.5.0a6/aiochris/home.md
+-rw-r--r--   0        0        0       97 2024-05-11 21:41:41.196594 aiochris-0.5.0a6/aiochris/link/__init__.py
+-rw-r--r--   0        0        0     1143 2024-05-11 21:41:41.196594 aiochris-0.5.0a6/aiochris/link/collection_client.py
+-rw-r--r--   0        0        0     5027 2024-05-11 21:41:41.196594 aiochris-0.5.0a6/aiochris/link/http.py
+-rw-r--r--   0        0        0     4659 2024-05-11 21:41:41.196594 aiochris-0.5.0a6/aiochris/link/linked.py
+-rw-r--r--   0        0        0     1450 2024-05-11 21:41:41.196594 aiochris-0.5.0a6/aiochris/link/metaprog.py
+-rw-r--r--   0        0        0      112 2024-05-11 21:41:41.196594 aiochris-0.5.0a6/aiochris/models/__init__.py
+-rw-r--r--   0        0        0     2212 2024-05-11 21:41:41.196594 aiochris-0.5.0a6/aiochris/models/collection_links.py
+-rw-r--r--   0        0        0     2898 2024-05-11 21:41:41.196594 aiochris-0.5.0a6/aiochris/models/data.py
+-rw-r--r--   0        0        0     7367 2024-05-11 21:41:41.196594 aiochris-0.5.0a6/aiochris/models/logged_in.py
+-rw-r--r--   0        0        0     2297 2024-05-11 21:41:41.196594 aiochris-0.5.0a6/aiochris/models/public.py
+-rw-r--r--   0        0        0     3216 2024-05-11 21:41:41.196594 aiochris-0.5.0a6/aiochris/types.py
+-rw-r--r--   0        0        0       31 2024-05-11 21:41:41.196594 aiochris-0.5.0a6/aiochris/util/__init__.py
+-rw-r--r--   0        0        0     6932 2024-05-11 21:41:41.200594 aiochris-0.5.0a6/aiochris/util/search.py
+-rw-r--r--   0        0        0     1191 2024-05-11 21:41:41.200594 aiochris-0.5.0a6/pyproject.toml
+-rw-r--r--   0        0        0     2690 1970-01-01 00:00:00.000000 aiochris-0.5.0a6/PKG-INFO
```

### Comparing `aiochris-0.5.0a5/LICENSE` & `aiochris-0.5.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `aiochris-0.5.0a5/README.md` & `aiochris-0.5.0a6/README.md`

 * *Files identical despite different names*

### Comparing `aiochris-0.5.0a5/aiochris/__init__.py` & `aiochris-0.5.0a6/aiochris/__init__.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.5.0a5/aiochris/client/admin.py` & `aiochris-0.5.0a6/aiochris/client/admin.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.5.0a5/aiochris/client/anon.py` & `aiochris-0.5.0a6/aiochris/client/anon.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.5.0a5/aiochris/client/authed.py` & `aiochris-0.5.0a6/aiochris/client/authed.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.5.0a5/aiochris/client/base.py` & `aiochris-0.5.0a6/aiochris/client/base.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.5.0a5/aiochris/client/from_chrs.py` & `aiochris-0.5.0a6/aiochris/client/from_chrs.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.5.0a5/aiochris/client/normal.py` & `aiochris-0.5.0a6/aiochris/client/normal.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.5.0a5/aiochris/enums.py` & `aiochris-0.5.0a6/aiochris/enums.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.5.0a5/aiochris/errors.py` & `aiochris-0.5.0a6/aiochris/errors.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.5.0a5/aiochris/examples.md` & `aiochris-0.5.0a6/aiochris/examples.md`

 * *Files identical despite different names*

### Comparing `aiochris-0.5.0a5/aiochris/home.md` & `aiochris-0.5.0a6/aiochris/home.md`

 * *Files identical despite different names*

### Comparing `aiochris-0.5.0a5/aiochris/link/collection_client.py` & `aiochris-0.5.0a6/aiochris/link/collection_client.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.5.0a5/aiochris/link/http.py` & `aiochris-0.5.0a6/aiochris/link/http.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.5.0a5/aiochris/link/linked.py` & `aiochris-0.5.0a6/aiochris/link/linked.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.5.0a5/aiochris/link/metaprog.py` & `aiochris-0.5.0a6/aiochris/link/metaprog.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.5.0a5/aiochris/models/collection_links.py` & `aiochris-0.5.0a6/aiochris/models/collection_links.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.5.0a5/aiochris/models/data.py` & `aiochris-0.5.0a6/aiochris/models/data.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.5.0a5/aiochris/models/logged_in.py` & `aiochris-0.5.0a6/aiochris/models/logged_in.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     """
     A file from a PACS server which was pushed into ChRIS.
     A PACSFile is usually a DICOM file.
 
     See https://github.com/FNNDSC/ChRIS_ultron_backEnd/blob/a1bf499144df79622eb3f8a459cdb80d8e34cb04/chris_backend/pacsfiles/models.py#L16-L33
     """
 
+    id: PacsFileId
     PatientID: str
     PatientName: str
     PatientBirthDate: str
     PatientAge: int
     PatientSex: str
     StudyDate: str  # TODO deserialize
     AccessionNumber: str
```

### Comparing `aiochris-0.5.0a5/aiochris/models/public.py` & `aiochris-0.5.0a6/aiochris/models/public.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.5.0a5/aiochris/types.py` & `aiochris-0.5.0a6/aiochris/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,7 +99,9 @@
 """
 PluginParametersUrl = NewType("PluginParametersUrl", str)
 TagsUrl = NewType("TagsUrl", str)
 TaggingsUrl = NewType("TaggingsUrl", str)
 CommentsUrl = NewType("CommentsUrl", str)
 
 PluginParameterUrl = NewType("PluginParameterUrl", str)
+
+PacsFileId = NewType("PacsFileId", int)
```

### Comparing `aiochris-0.5.0a5/aiochris/util/search.py` & `aiochris-0.5.0a6/aiochris/util/search.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.5.0a5/pyproject.toml` & `aiochris-0.5.0a6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiochris"
-version = "0.5.0a5"
+version = "0.5.0a6"
 description = "ChRIS client built on aiohttp"
 authors = ["FNNDSC <dev@babyMRI.org>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `aiochris-0.5.0a5/PKG-INFO` & `aiochris-0.5.0a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiochris
-Version: 0.5.0a5
+Version: 0.5.0a6
 Summary: ChRIS client built on aiohttp
 License: MIT
 Author: FNNDSC
 Author-email: dev@babyMRI.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

