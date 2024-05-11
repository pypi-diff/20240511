# Comparing `tmp/cvprocessor-0.2.0.tar.gz` & `tmp/cvprocessor-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvprocessor-0.2.0.tar", last modified: Fri May 10 11:03:10 2024, max compression
+gzip compressed data, was "cvprocessor-0.3.0.tar", last modified: Sat May 11 00:35:03 2024, max compression
```

## Comparing `cvprocessor-0.2.0.tar` & `cvprocessor-0.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-10 11:03:10.018468 cvprocessor-0.2.0/
--rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.2.0/LICENSE
--rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-10 11:03:10.017172 cvprocessor-0.2.0/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)     1053 2024-05-08 07:27:08.000000 cvprocessor-0.2.0/README.md
--rw-r--r--   0 fernando   (501) staff       (20)      769 2024-05-10 11:02:10.000000 cvprocessor-0.2.0/pyproject.toml
--rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-10 11:03:10.018731 cvprocessor-0.2.0/setup.cfg
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-10 11:03:09.985305 cvprocessor-0.2.0/src/
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-10 11:03:10.008233 cvprocessor-0.2.0/src/cvprocessor/
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.2.0/src/cvprocessor/__init__.py
--rw-r--r--   0 fernando   (501) staff       (20)     6651 2024-05-08 07:01:09.000000 cvprocessor-0.2.0/src/cvprocessor/authors.py
--rw-r--r--   0 fernando   (501) staff       (20)      148 2024-05-04 10:32:46.000000 cvprocessor-0.2.0/src/cvprocessor/common.py
--rw-r--r--   0 fernando   (501) staff       (20)     4724 2024-05-10 11:02:21.000000 cvprocessor-0.2.0/src/cvprocessor/cv.py
--rw-r--r--   0 fernando   (501) staff       (20)     4218 2024-05-08 07:28:24.000000 cvprocessor-0.2.0/src/cvprocessor/education.py
--rw-r--r--   0 fernando   (501) staff       (20)     4633 2024-05-08 08:22:41.000000 cvprocessor-0.2.0/src/cvprocessor/experience.py
--rw-r--r--   0 fernando   (501) staff       (20)     2619 2024-05-08 07:09:50.000000 cvprocessor-0.2.0/src/cvprocessor/grants_awards.py
--rw-r--r--   0 fernando   (501) staff       (20)     4581 2024-05-10 10:56:41.000000 cvprocessor-0.2.0/src/cvprocessor/institutes.py
--rw-r--r--   0 fernando   (501) staff       (20)     1652 2024-05-08 07:13:23.000000 cvprocessor-0.2.0/src/cvprocessor/intro.py
--rw-r--r--   0 fernando   (501) staff       (20)     1533 2024-05-09 01:57:53.000000 cvprocessor-0.2.0/src/cvprocessor/memberships.py
--rw-r--r--   0 fernando   (501) staff       (20)     2466 2024-05-08 07:13:59.000000 cvprocessor-0.2.0/src/cvprocessor/news.py
--rw-r--r--   0 fernando   (501) staff       (20)     9925 2024-05-08 07:18:36.000000 cvprocessor-0.2.0/src/cvprocessor/publications.py
--rw-r--r--   0 fernando   (501) staff       (20)     1866 2024-05-09 02:04:48.000000 cvprocessor-0.2.0/src/cvprocessor/references.py
--rw-r--r--   0 fernando   (501) staff       (20)     1133 2024-05-08 07:20:47.000000 cvprocessor-0.2.0/src/cvprocessor/research_interests.py
--rw-r--r--   0 fernando   (501) staff       (20)     1980 2024-05-09 01:44:15.000000 cvprocessor-0.2.0/src/cvprocessor/service.py
--rw-r--r--   0 fernando   (501) staff       (20)     2288 2024-05-09 01:28:30.000000 cvprocessor-0.2.0/src/cvprocessor/skills.py
--rw-r--r--   0 fernando   (501) staff       (20)     3509 2024-05-08 07:21:45.000000 cvprocessor-0.2.0/src/cvprocessor/software.py
--rw-r--r--   0 fernando   (501) staff       (20)     3754 2024-05-08 07:49:48.000000 cvprocessor-0.2.0/src/cvprocessor/supervision.py
--rw-r--r--   0 fernando   (501) staff       (20)     5394 2024-05-10 11:01:39.000000 cvprocessor-0.2.0/src/cvprocessor/teaching.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-10 11:03:10.016018 cvprocessor-0.2.0/src/cvprocessor.egg-info/
--rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-10 11:03:09.000000 cvprocessor-0.2.0/src/cvprocessor.egg-info/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      771 2024-05-10 11:03:09.000000 cvprocessor-0.2.0/src/cvprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-10 11:03:09.000000 cvprocessor-0.2.0/src/cvprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-10 11:03:09.000000 cvprocessor-0.2.0/src/cvprocessor.egg-info/requires.txt
--rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-10 11:03:09.000000 cvprocessor-0.2.0/src/cvprocessor.egg-info/top_level.txt
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-11 00:35:03.145398 cvprocessor-0.3.0/
+-rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.3.0/LICENSE
+-rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-11 00:35:03.144430 cvprocessor-0.3.0/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)     1053 2024-05-08 07:27:08.000000 cvprocessor-0.3.0/README.md
+-rw-r--r--   0 fernando   (501) staff       (20)      769 2024-05-11 00:33:20.000000 cvprocessor-0.3.0/pyproject.toml
+-rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-11 00:35:03.145519 cvprocessor-0.3.0/setup.cfg
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-11 00:35:03.124111 cvprocessor-0.3.0/src/
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-11 00:35:03.137230 cvprocessor-0.3.0/src/cvprocessor/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.3.0/src/cvprocessor/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)     6651 2024-05-08 07:01:09.000000 cvprocessor-0.3.0/src/cvprocessor/authors.py
+-rw-r--r--   0 fernando   (501) staff       (20)      148 2024-05-04 10:32:46.000000 cvprocessor-0.3.0/src/cvprocessor/common.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4722 2024-05-11 00:25:04.000000 cvprocessor-0.3.0/src/cvprocessor/cv.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4218 2024-05-08 07:28:24.000000 cvprocessor-0.3.0/src/cvprocessor/education.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4633 2024-05-08 08:22:41.000000 cvprocessor-0.3.0/src/cvprocessor/experience.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2619 2024-05-08 07:09:50.000000 cvprocessor-0.3.0/src/cvprocessor/grants_awards.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4581 2024-05-10 10:56:41.000000 cvprocessor-0.3.0/src/cvprocessor/institutes.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1652 2024-05-08 07:13:23.000000 cvprocessor-0.3.0/src/cvprocessor/intro.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1533 2024-05-09 01:57:53.000000 cvprocessor-0.3.0/src/cvprocessor/memberships.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2466 2024-05-08 07:13:59.000000 cvprocessor-0.3.0/src/cvprocessor/news.py
+-rw-r--r--   0 fernando   (501) staff       (20)     9925 2024-05-08 07:18:36.000000 cvprocessor-0.3.0/src/cvprocessor/publications.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1866 2024-05-09 02:04:48.000000 cvprocessor-0.3.0/src/cvprocessor/references.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1133 2024-05-08 07:20:47.000000 cvprocessor-0.3.0/src/cvprocessor/research_interests.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1980 2024-05-09 01:44:15.000000 cvprocessor-0.3.0/src/cvprocessor/service.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2288 2024-05-09 01:28:30.000000 cvprocessor-0.3.0/src/cvprocessor/skills.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3509 2024-05-08 07:21:45.000000 cvprocessor-0.3.0/src/cvprocessor/software.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3754 2024-05-08 07:49:48.000000 cvprocessor-0.3.0/src/cvprocessor/supervision.py
+-rw-r--r--   0 fernando   (501) staff       (20)     6387 2024-05-11 00:30:50.000000 cvprocessor-0.3.0/src/cvprocessor/teaching.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-11 00:35:03.143170 cvprocessor-0.3.0/src/cvprocessor.egg-info/
+-rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-11 00:35:03.000000 cvprocessor-0.3.0/src/cvprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)      771 2024-05-11 00:35:03.000000 cvprocessor-0.3.0/src/cvprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-11 00:35:03.000000 cvprocessor-0.3.0/src/cvprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-11 00:35:03.000000 cvprocessor-0.3.0/src/cvprocessor.egg-info/requires.txt
+-rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-11 00:35:03.000000 cvprocessor-0.3.0/src/cvprocessor.egg-info/top_level.txt
```

### Comparing `cvprocessor-0.2.0/LICENSE` & `cvprocessor-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.2.0/PKG-INFO` & `cvprocessor-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.2.0
+Version: 0.3.0
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.2.0/README.md` & `cvprocessor-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.2.0/pyproject.toml` & `cvprocessor-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cvprocessor"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
     { name = "F. Fernando Jurado-Lasso", email = "fdo.jurado@gmail.com" },
 ]
 description = "CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cvprocessor-0.2.0/src/cvprocessor/authors.py` & `cvprocessor-0.3.0/src/cvprocessor/authors.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.2.0/src/cvprocessor/cv.py` & `cvprocessor-0.3.0/src/cvprocessor/cv.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,9 +135,9 @@
     def __repr__(self):
         repr = f"CV(filename={self.filename}, education={self.education}, institutes={self.institutes}, software={self.software}, intro={self.intro}, authors={self.authors}, news={self.news}, publications={self.publications}, research_interests={self.research_interests}, grants_awards={self.grants_awards}, teaching={self.teaching}, supervision={self.supervision}, experience={self.experience}, skills={self.skills}, service={self.service}, memberships={self.memberships}, references={self.references})"
         return repr
 
 
 if __name__ == "__main__":
     cv = CV("cv.xlsx")
-    print(str(cv.references))
+    print(str(cv.teaching))
     sys.exit(0)
```

### Comparing `cvprocessor-0.2.0/src/cvprocessor/education.py` & `cvprocessor-0.3.0/src/cvprocessor/education.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.2.0/src/cvprocessor/experience.py` & `cvprocessor-0.3.0/src/cvprocessor/experience.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.2.0/src/cvprocessor/grants_awards.py` & `cvprocessor-0.3.0/src/cvprocessor/grants_awards.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.2.0/src/cvprocessor/institutes.py` & `cvprocessor-0.3.0/src/cvprocessor/institutes.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.2.0/src/cvprocessor/intro.py` & `cvprocessor-0.3.0/src/cvprocessor/intro.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.2.0/src/cvprocessor/memberships.py` & `cvprocessor-0.3.0/src/cvprocessor/memberships.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.2.0/src/cvprocessor/news.py` & `cvprocessor-0.3.0/src/cvprocessor/news.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.2.0/src/cvprocessor/publications.py` & `cvprocessor-0.3.0/src/cvprocessor/publications.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.2.0/src/cvprocessor/references.py` & `cvprocessor-0.3.0/src/cvprocessor/references.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.2.0/src/cvprocessor/research_interests.py` & `cvprocessor-0.3.0/src/cvprocessor/research_interests.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.2.0/src/cvprocessor/service.py` & `cvprocessor-0.3.0/src/cvprocessor/service.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.2.0/src/cvprocessor/skills.py` & `cvprocessor-0.3.0/src/cvprocessor/skills.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.2.0/src/cvprocessor/software.py` & `cvprocessor-0.3.0/src/cvprocessor/software.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.2.0/src/cvprocessor/supervision.py` & `cvprocessor-0.3.0/src/cvprocessor/supervision.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.2.0/src/cvprocessor/teaching.py` & `cvprocessor-0.3.0/src/cvprocessor/teaching.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,59 @@
 import pandas as pd
 
 
+class YearData:
+    def __init__(self, year_range):
+        self._year_range = year_range
+        self._start_year = None
+        self._end_year = None
+        self._process_year_range()
+
+    @property
+    def year_range(self):
+        return self._year_range
+
+    @property
+    def start_year(self):
+        return self._start_year
+
+    @property
+    def end_year(self):
+        return self._end_year
+
+    def format_year(self, year):
+        year = year.strip()
+        year = pd.to_datetime(year, format="%b %Y")
+        return year
+
+    def _process_year_range(self):
+        year_range = self.year_range.split("-")
+        self._start_year = self.format_year(year_range[0])
+        self._start_year = pd.to_datetime(self.start_year, format="%b %Y")
+        if len(year_range) > 1:
+            self._end_year = self.format_year(year_range[1])
+            self._end_year = pd.to_datetime(self.end_year, format="%b %Y")
+        else:
+            self._end_year = None
+
+    def __str__(self):
+        string = f"Year range: {self.year_range}\n"
+        string += f"Start year: {self.start_year}\n"
+        string += f"End year: {self.end_year}\n"
+        return string
+
+    def __repr__(self):
+        string = f"YearData(year_range={self.year_range}, start_year={self.start_year}, end_year={self.end_year})"
+        return string
+
+
 class TeachingData:
     def __init__(self, filename):
         self._filename = filename
-        self._year = None
+        self._year_range = None
         self._start_year = None
         self._end_year = None
         self._position = None
         self._course = None
         self._link = None
         self._type = None
         self._institution = None
@@ -18,15 +63,15 @@
 
     @property
     def filename(self):
         return self._filename
 
     @property
     def year(self):
-        return self._year
+        return self._year_range
 
     @property
     def start_year(self):
         return self._start_year
 
     @property
     def end_year(self):
@@ -57,86 +102,71 @@
         return self._supervisor
 
     @property
     def responsibilities(self):
         return self._responsibilities
 
     def get_start_year(self):
-        year = 1e6
+        min_year = 1e6
         date = None
-        for start, _ in self.year:
-            if not start:
-                continue
-            if int(start.year) < year:
-                year = int(start.year)
-                date = start
+        for year in self.year:
+            if int(year.start_year.year) < min_year:
+                min_year = int(year.start_year.year)
+                date = year.start_year
         return date
 
     def get_end_year(self):
-        year = 0
+        max_year = -1
         date = None
-        for _, end in self.year:
-            if not end:
-                continue
-            if int(end.year) > year:
-                year = int(end.year)
-                date = end
+        for year in self.year:
+            if year.end_year is not None:
+                if int(year.end_year.year) > max_year:
+                    max_year = int(year.end_year.year)
+                    date = year.end_year
         return date
 
-    def format_year(self, year):
-        year = year.strip()
-        year = pd.to_datetime(year, format="%b %Y")
-        return year
-
     def process_year_data(self):
-        self._year = self.filename["Year"]
-        self._year = self._year.split(";")
-        self._year = list(filter(None, self._year))
+        self._year_range = self.filename["Year"]
+        self._year_range = self._year_range.split(";")
+        self._year_range = list(filter(None, self._year_range))
         year_list = []
-        for year in self._year:
-            year_split = year.split("-")
-            if len(year_split) > 1:
-                start_year = year_split[0]
-                end_year = year_split[1]
-            else:
-                start_year = year_split[0]
-                end_year = None
-            start_year = self.format_year(start_year)
-            if end_year:
-                end_year = self.format_year(end_year)
-            year_list.append((start_year, end_year))
-        self._year = year_list
+        for year in self._year_range:
+            year_list.append(YearData(year))
+        self._year_range = year_list
 
     def _load_teaching(self):
         self.process_year_data()
         self._start_year = self.get_start_year()
         self._end_year = self.get_end_year()
         self._position = self.filename["Position"]
         self._course = self.filename["Course"]
         self._link = self.filename["Link"]
         self._type = self.filename["Type"]
         self._institution = self.filename["Institution"]
         self._supervisor = self.filename["Supervisor"]
         self._responsibilities = self.filename["Responsibilities"]
 
     def __str__(self):
-        string = f"Year: {self.year}\n"
+        year_data = ""
+        for year in self.year:
+            year_data += str(year)
+        string = f"Year range: {year_data}\n"
         string += f"Start year: {self.start_year}\n"
         string += f"End year: {self.end_year}\n"
         string += f"Position: {self.position}\n"
         string += f"Course: {self.course}\n"
         string += f"Link: {self.link}\n"
         string += f"Type: {self.type}\n"
         string += f"Institution: {self.institution}\n"
         string += f"Supervisor: {self.supervisor}\n"
         string += f"Responsibilities: {self.responsibilities}\n\n"
         return string
 
     def __repr__(self):
-        string = f"TeachingData(year={self.year}, start_year={self.start_year}, end_year={self.end_year}, position={self.position}, course={self.course}, link={self.link}, type={self.type}, institution={self.institution}, department={self.department}, country={self.country}, supervisor={self.supervisor}, responsibilities={self.responsibilities})"
+        string = f"TeachingData(year_range={self.year}, start_year={self.start_year}, end_year={self.end_year}, position={self.position}, course={self.course}, link={self.link}, type={self.type}, institution={self.institution}, department={self.department}, country={self.country}, supervisor={self.supervisor}, responsibilities={self.responsibilities})"
         return string
 
 
 class Teaching:
     def __init__(self, filename):
         self._filename = filename
         self._teaching = self._load_teaching()
```

### Comparing `cvprocessor-0.2.0/src/cvprocessor.egg-info/PKG-INFO` & `cvprocessor-0.3.0/src/cvprocessor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.2.0
+Version: 0.3.0
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.2.0/src/cvprocessor.egg-info/SOURCES.txt` & `cvprocessor-0.3.0/src/cvprocessor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

