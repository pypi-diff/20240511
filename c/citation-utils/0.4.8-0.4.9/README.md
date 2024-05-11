# Comparing `tmp/citation_utils-0.4.8.tar.gz` & `tmp/citation_utils-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citation_utils-0.4.8.tar", max compression
+gzip compressed data, was "citation_utils-0.4.9.tar", max compression
```

## Comparing `citation_utils-0.4.8.tar` & `citation_utils-0.4.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1491 2023-06-23 10:27:21.228309 citation_utils-0.4.8/LICENSE
--rw-r--r--   0        0        0      653 2023-06-25 09:54:14.887730 citation_utils-0.4.8/citation_utils/__init__.py
--rw-r--r--   0        0        0    18063 2023-07-01 03:42:49.795835 citation_utils-0.4.8/citation_utils/citation.py
--rw-r--r--   0        0        0     1179 2023-06-25 09:54:14.891749 citation_utils-0.4.8/citation_utils/dockets/__init__.py
--rw-r--r--   0        0        0     3125 2023-06-29 03:28:48.048714 citation_utils-0.4.8/citation_utils/dockets/constructed_ac.py
--rw-r--r--   0        0        0     3164 2023-06-29 03:28:29.361313 citation_utils-0.4.8/citation_utils/dockets/constructed_am.py
--rw-r--r--   0        0        0     2457 2023-06-25 09:54:14.895608 citation_utils-0.4.8/citation_utils/dockets/constructed_bm.py
--rw-r--r--   0        0        0     2866 2023-06-29 03:27:47.112900 citation_utils-0.4.8/citation_utils/dockets/constructed_gr.py
--rw-r--r--   0        0        0     2094 2023-06-25 09:54:14.896184 citation_utils-0.4.8/citation_utils/dockets/constructed_jib.py
--rw-r--r--   0        0        0     2692 2023-06-28 10:55:51.445938 citation_utils-0.4.8/citation_utils/dockets/constructed_oca.py
--rw-r--r--   0        0        0     1597 2023-06-25 09:54:14.896710 citation_utils-0.4.8/citation_utils/dockets/constructed_pet.py
--rw-r--r--   0        0        0     2055 2023-06-28 10:33:49.974829 citation_utils-0.4.8/citation_utils/dockets/constructed_udk.py
--rw-r--r--   0        0        0      364 2023-06-25 10:00:40.543092 citation_utils-0.4.8/citation_utils/dockets/models/__init__.py
--rw-r--r--   0        0        0     4834 2023-06-25 09:54:14.900031 citation_utils-0.4.8/citation_utils/dockets/models/constructor.py
--rw-r--r--   0        0        0     1373 2023-06-25 09:54:14.900293 citation_utils-0.4.8/citation_utils/dockets/models/docket_category.py
--rw-r--r--   0        0        0     1778 2023-07-01 03:41:01.932253 citation_utils-0.4.8/citation_utils/dockets/models/docket_citation.py
--rw-r--r--   0        0        0     5839 2023-07-01 03:42:14.972022 citation_utils-0.4.8/citation_utils/dockets/models/docket_model.py
--rw-r--r--   0        0        0     3404 2023-06-28 02:34:55.066065 citation_utils-0.4.8/citation_utils/dockets/models/docket_rules.py
--rw-r--r--   0        0        0     2911 2023-06-25 09:54:14.901368 citation_utils-0.4.8/citation_utils/dockets/models/gr_clean.py
--rw-r--r--   0        0        0       81 2023-06-25 09:54:14.902014 citation_utils-0.4.8/citation_utils/dockets/models/misc/__init__.py
--rw-r--r--   0        0        0      746 2023-06-25 09:54:14.903593 citation_utils-0.4.8/citation_utils/dockets/models/misc/extra.py
--rw-r--r--   0        0        0     1514 2023-06-25 09:54:14.903861 citation_utils-0.4.8/citation_utils/dockets/models/misc/num.py
--rw-r--r--   0        0        0      242 2023-06-25 09:54:14.904129 citation_utils-0.4.8/citation_utils/dockets/models/misc/x.py
--rw-r--r--   0        0        0     5861 2023-06-29 03:34:11.063815 citation_utils-0.4.8/citation_utils/document.py
--rw-r--r--   0        0        0     2531 2023-06-25 09:54:14.904670 citation_utils-0.4.8/citation_utils/special.py
--rw-r--r--   0        0        0     1312 2023-07-01 03:47:11.964121 citation_utils-0.4.8/pyproject.toml
--rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 citation_utils-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-06-23 10:27:21.228309 citation_utils-0.4.9/LICENSE
+-rw-r--r--   0        0        0      653 2023-06-25 09:54:14.887730 citation_utils-0.4.9/citation_utils/__init__.py
+-rw-r--r--   0        0        0    21296 2023-08-13 02:26:56.012026 citation_utils-0.4.9/citation_utils/citation.py
+-rw-r--r--   0        0        0     1179 2023-06-25 09:54:14.891749 citation_utils-0.4.9/citation_utils/dockets/__init__.py
+-rw-r--r--   0        0        0     3125 2023-06-29 03:28:48.048714 citation_utils-0.4.9/citation_utils/dockets/constructed_ac.py
+-rw-r--r--   0        0        0     3164 2023-06-29 03:28:29.361313 citation_utils-0.4.9/citation_utils/dockets/constructed_am.py
+-rw-r--r--   0        0        0     2457 2023-06-25 09:54:14.895608 citation_utils-0.4.9/citation_utils/dockets/constructed_bm.py
+-rw-r--r--   0        0        0     2866 2023-06-29 03:27:47.112900 citation_utils-0.4.9/citation_utils/dockets/constructed_gr.py
+-rw-r--r--   0        0        0     2094 2023-06-25 09:54:14.896184 citation_utils-0.4.9/citation_utils/dockets/constructed_jib.py
+-rw-r--r--   0        0        0     2692 2023-06-28 10:55:51.445938 citation_utils-0.4.9/citation_utils/dockets/constructed_oca.py
+-rw-r--r--   0        0        0     1597 2023-06-25 09:54:14.896710 citation_utils-0.4.9/citation_utils/dockets/constructed_pet.py
+-rw-r--r--   0        0        0     2055 2023-06-28 10:33:49.974829 citation_utils-0.4.9/citation_utils/dockets/constructed_udk.py
+-rw-r--r--   0        0        0      364 2023-06-25 10:00:40.543092 citation_utils-0.4.9/citation_utils/dockets/models/__init__.py
+-rw-r--r--   0        0        0     4834 2023-06-25 09:54:14.900031 citation_utils-0.4.9/citation_utils/dockets/models/constructor.py
+-rw-r--r--   0        0        0     1373 2023-06-25 09:54:14.900293 citation_utils-0.4.9/citation_utils/dockets/models/docket_category.py
+-rw-r--r--   0        0        0     1778 2023-07-01 03:41:01.932253 citation_utils-0.4.9/citation_utils/dockets/models/docket_citation.py
+-rw-r--r--   0        0        0     5839 2023-07-01 03:42:14.972022 citation_utils-0.4.9/citation_utils/dockets/models/docket_model.py
+-rw-r--r--   0        0        0     3404 2023-06-28 02:34:55.066065 citation_utils-0.4.9/citation_utils/dockets/models/docket_rules.py
+-rw-r--r--   0        0        0     2911 2023-06-25 09:54:14.901368 citation_utils-0.4.9/citation_utils/dockets/models/gr_clean.py
+-rw-r--r--   0        0        0       81 2023-06-25 09:54:14.902014 citation_utils-0.4.9/citation_utils/dockets/models/misc/__init__.py
+-rw-r--r--   0        0        0      746 2023-06-25 09:54:14.903593 citation_utils-0.4.9/citation_utils/dockets/models/misc/extra.py
+-rw-r--r--   0        0        0     1514 2023-06-25 09:54:14.903861 citation_utils-0.4.9/citation_utils/dockets/models/misc/num.py
+-rw-r--r--   0        0        0      242 2023-06-25 09:54:14.904129 citation_utils-0.4.9/citation_utils/dockets/models/misc/x.py
+-rw-r--r--   0        0        0     5861 2023-06-29 03:34:11.063815 citation_utils-0.4.9/citation_utils/document.py
+-rw-r--r--   0        0        0     2531 2023-06-25 09:54:14.904670 citation_utils-0.4.9/citation_utils/special.py
+-rw-r--r--   0        0        0     1312 2023-08-10 06:31:40.562640 citation_utils-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 citation_utils-0.4.9/PKG-INFO
```

### Comparing `citation_utils-0.4.8/LICENSE` & `citation_utils-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.8/citation_utils/__init__.py` & `citation_utils-0.4.9/citation_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.8/citation_utils/citation.py` & `citation_utils-0.4.9/citation_utils/citation.py`

 * *Files 10% similar despite different names*

```diff
@@ -303,14 +303,102 @@
             Self | None: First item found from `extract_citations`, if it exists.
         """
         try:
             return next(cls.extract_citations(text))
         except StopIteration:
             return None
 
+    @classmethod
+    def create_docket_slug(cls, v: str) -> str | None:
+        """Given a docket string, format the string into a slug
+        that can be a database primary key.
+
+        Examples:
+            >>> text = "GR 138570, Oct. 10, 2000"
+            >>> Citation.create_docket_slug(text)
+            'gr-138570-2000-10-10'
+
+        Args:
+            v (str): The text to evaluate
+
+        Returns:
+            str | None: The slug to use, if possible.
+        """
+        if cite := cls.extract_citation(v):
+            if cite.is_docket:
+                return "-".join(
+                    [
+                        cite.docket_category.name.lower(),  # type: ignore
+                        cite.docket_serial.lower(),  # type: ignore
+                        cite.docket_date.isoformat(),  # type: ignore
+                    ]
+                )
+        return None
+
+    @classmethod
+    def make_citation_string(
+        cls,
+        cat: str,
+        num: str,
+        date: str,
+        phil: str | None = None,
+        scra: str | None = None,
+        offg: str | None = None,
+    ) -> str | None:
+        """Assume that because of citation-utils, the extracted values are inputted into a database.
+
+        When the values are pulled from the database, it becomes necessary to convert these database (lowercased) values
+        to a unified properly-cased citation string with readable date (vs. isoformat db-counterpart).
+
+        Examples:
+            >>> Citation.make_citation_string(cat='gr', num='111', date='2000-01-01', phil='100 phil. 100', scra='122 scra 100-a')
+            'G.R. No. 111, Jan. 1, 2000, 100 Phil. 100, 122 SCRA 100-A'
+
+        Args:
+            cat (str): The shorthand code for docket category
+            num (str): The serial identifier of the docket category
+            date (str): The date of `cat` + `num`
+            phil (str | None, optional): Phil. Reports. Defaults to None.
+            scra (str | None, optional): Supreme Court Reports Annotated. Defaults to None.
+            offg (str | None, optional): Official Gazette. Defaults to None.
+
+        Returns:
+            str | None: The combination of citation bits.
+        """  # noqa: E501
+        bits = [
+            phil.title().split() if phil else None,
+            scra.upper().split() if scra else None,
+            offg.upper().split() if offg else None,
+        ]
+        cased_bits = [
+            f"{bit[0].upper()} {bit[1]} {bit[2].upper()}" for bit in bits if bit
+        ]
+        reports = ", ".join(cased_bits) if any(bits) else None
+        dt = datetime.date.fromisoformat(date).strftime("%b. %-d, %Y")
+        match cat:
+            case "gr":
+                prefix = "G.R."
+            case "am":
+                prefix = "A.M."
+            case "ac":
+                prefix = "A.C."
+            case "bm":
+                prefix = "B.M."
+            case "udk":
+                prefix = "UDK"
+            case "jib":
+                prefix = "JIB-FPI"
+            case "oca":
+                prefix = "OCA IPI"
+            case _:
+                return None
+        docket = f"{prefix} No. {num.upper()}"
+        bits = [bit for bit in [docket, dt, reports] if bit]
+        return ", ".join(bits)
+
 
 class CountedCitation(Citation):
     mentions: int = Field(default=1, description="Get count via Citation __eq__")
 
     def __repr__(self) -> str:
         return f"{str(self)}: {self.mentions}"
```

### Comparing `citation_utils-0.4.8/citation_utils/dockets/__init__.py` & `citation_utils-0.4.9/citation_utils/dockets/__init__.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.8/citation_utils/dockets/constructed_ac.py` & `citation_utils-0.4.9/citation_utils/dockets/constructed_ac.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.8/citation_utils/dockets/constructed_am.py` & `citation_utils-0.4.9/citation_utils/dockets/constructed_am.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.8/citation_utils/dockets/constructed_bm.py` & `citation_utils-0.4.9/citation_utils/dockets/constructed_bm.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.8/citation_utils/dockets/constructed_gr.py` & `citation_utils-0.4.9/citation_utils/dockets/constructed_gr.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.8/citation_utils/dockets/constructed_jib.py` & `citation_utils-0.4.9/citation_utils/dockets/constructed_jib.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.8/citation_utils/dockets/constructed_oca.py` & `citation_utils-0.4.9/citation_utils/dockets/constructed_oca.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.8/citation_utils/dockets/constructed_pet.py` & `citation_utils-0.4.9/citation_utils/dockets/constructed_pet.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.8/citation_utils/dockets/constructed_udk.py` & `citation_utils-0.4.9/citation_utils/dockets/constructed_udk.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.8/citation_utils/dockets/models/constructor.py` & `citation_utils-0.4.9/citation_utils/dockets/models/constructor.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.8/citation_utils/dockets/models/docket_category.py` & `citation_utils-0.4.9/citation_utils/dockets/models/docket_category.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.8/citation_utils/dockets/models/docket_citation.py` & `citation_utils-0.4.9/citation_utils/dockets/models/docket_citation.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.8/citation_utils/dockets/models/docket_model.py` & `citation_utils-0.4.9/citation_utils/dockets/models/docket_model.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.8/citation_utils/dockets/models/docket_rules.py` & `citation_utils-0.4.9/citation_utils/dockets/models/docket_rules.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.8/citation_utils/dockets/models/gr_clean.py` & `citation_utils-0.4.9/citation_utils/dockets/models/gr_clean.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.8/citation_utils/dockets/models/misc/extra.py` & `citation_utils-0.4.9/citation_utils/dockets/models/misc/extra.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.8/citation_utils/dockets/models/misc/num.py` & `citation_utils-0.4.9/citation_utils/dockets/models/misc/num.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.8/citation_utils/document.py` & `citation_utils-0.4.9/citation_utils/document.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.8/citation_utils/special.py` & `citation_utils-0.4.9/citation_utils/special.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.8/pyproject.toml` & `citation_utils-0.4.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "citation_utils"
-version = "0.4.8"
+version = "0.4.9"
 description = "Pattern matching Philippine Supreme Court citations."
 authors = ["Marcelino G. Veloso III <contact@mv3.dev>"]
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/citation-utils"
 documentation = "https://justmars.github.io/citation-utils"
 classifiers = [
   "Topic :: Text Processing :: General",
```

### Comparing `citation_utils-0.4.8/PKG-INFO` & `citation_utils-0.4.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citation-utils
-Version: 0.4.8
+Version: 0.4.9
 Summary: Pattern matching Philippine Supreme Court citations.
 Home-page: https://lawsql.com
 Author: Marcelino G. Veloso III
 Author-email: contact@mv3.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pydantic
```

