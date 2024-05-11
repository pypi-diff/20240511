# Comparing `tmp/cvprocessor-0.1.0.tar.gz` & `tmp/cvprocessor-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvprocessor-0.1.0.tar", last modified: Thu May  9 11:02:23 2024, max compression
+gzip compressed data, was "cvprocessor-0.2.0.tar", last modified: Fri May 10 11:03:10 2024, max compression
```

## Comparing `cvprocessor-0.1.0.tar` & `cvprocessor-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-09 11:02:23.293621 cvprocessor-0.1.0/
--rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.1.0/LICENSE
--rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-09 11:02:23.293068 cvprocessor-0.1.0/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)     1053 2024-05-08 07:27:08.000000 cvprocessor-0.1.0/README.md
--rw-r--r--   0 fernando   (501) staff       (20)      769 2024-05-09 10:56:40.000000 cvprocessor-0.1.0/pyproject.toml
--rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-09 11:02:23.293726 cvprocessor-0.1.0/setup.cfg
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-09 11:02:23.270981 cvprocessor-0.1.0/src/
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-09 11:02:23.289009 cvprocessor-0.1.0/src/cvprocessor/
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.1.0/src/cvprocessor/__init__.py
--rw-r--r--   0 fernando   (501) staff       (20)     6651 2024-05-08 07:01:09.000000 cvprocessor-0.1.0/src/cvprocessor/authors.py
--rw-r--r--   0 fernando   (501) staff       (20)      148 2024-05-04 10:32:46.000000 cvprocessor-0.1.0/src/cvprocessor/common.py
--rw-r--r--   0 fernando   (501) staff       (20)     4724 2024-05-09 10:57:04.000000 cvprocessor-0.1.0/src/cvprocessor/cv.py
--rw-r--r--   0 fernando   (501) staff       (20)     4218 2024-05-08 07:28:24.000000 cvprocessor-0.1.0/src/cvprocessor/education.py
--rw-r--r--   0 fernando   (501) staff       (20)     4633 2024-05-08 08:22:41.000000 cvprocessor-0.1.0/src/cvprocessor/experience.py
--rw-r--r--   0 fernando   (501) staff       (20)     2619 2024-05-08 07:09:50.000000 cvprocessor-0.1.0/src/cvprocessor/grants_awards.py
--rw-r--r--   0 fernando   (501) staff       (20)     4064 2024-05-09 10:55:26.000000 cvprocessor-0.1.0/src/cvprocessor/institutes.py
--rw-r--r--   0 fernando   (501) staff       (20)     1652 2024-05-08 07:13:23.000000 cvprocessor-0.1.0/src/cvprocessor/intro.py
--rw-r--r--   0 fernando   (501) staff       (20)     1533 2024-05-09 01:57:53.000000 cvprocessor-0.1.0/src/cvprocessor/memberships.py
--rw-r--r--   0 fernando   (501) staff       (20)     2466 2024-05-08 07:13:59.000000 cvprocessor-0.1.0/src/cvprocessor/news.py
--rw-r--r--   0 fernando   (501) staff       (20)     9925 2024-05-08 07:18:36.000000 cvprocessor-0.1.0/src/cvprocessor/publications.py
--rw-r--r--   0 fernando   (501) staff       (20)     1866 2024-05-09 02:04:48.000000 cvprocessor-0.1.0/src/cvprocessor/references.py
--rw-r--r--   0 fernando   (501) staff       (20)     1133 2024-05-08 07:20:47.000000 cvprocessor-0.1.0/src/cvprocessor/research_interests.py
--rw-r--r--   0 fernando   (501) staff       (20)     1980 2024-05-09 01:44:15.000000 cvprocessor-0.1.0/src/cvprocessor/service.py
--rw-r--r--   0 fernando   (501) staff       (20)     2288 2024-05-09 01:28:30.000000 cvprocessor-0.1.0/src/cvprocessor/skills.py
--rw-r--r--   0 fernando   (501) staff       (20)     3509 2024-05-08 07:21:45.000000 cvprocessor-0.1.0/src/cvprocessor/software.py
--rw-r--r--   0 fernando   (501) staff       (20)     3754 2024-05-08 07:49:48.000000 cvprocessor-0.1.0/src/cvprocessor/supervision.py
--rw-r--r--   0 fernando   (501) staff       (20)     5799 2024-05-08 07:22:45.000000 cvprocessor-0.1.0/src/cvprocessor/teaching.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-09 11:02:23.292471 cvprocessor-0.1.0/src/cvprocessor.egg-info/
--rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-09 11:02:23.000000 cvprocessor-0.1.0/src/cvprocessor.egg-info/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      771 2024-05-09 11:02:23.000000 cvprocessor-0.1.0/src/cvprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-09 11:02:23.000000 cvprocessor-0.1.0/src/cvprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-09 11:02:23.000000 cvprocessor-0.1.0/src/cvprocessor.egg-info/requires.txt
--rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-09 11:02:23.000000 cvprocessor-0.1.0/src/cvprocessor.egg-info/top_level.txt
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-10 11:03:10.018468 cvprocessor-0.2.0/
+-rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.2.0/LICENSE
+-rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-10 11:03:10.017172 cvprocessor-0.2.0/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)     1053 2024-05-08 07:27:08.000000 cvprocessor-0.2.0/README.md
+-rw-r--r--   0 fernando   (501) staff       (20)      769 2024-05-10 11:02:10.000000 cvprocessor-0.2.0/pyproject.toml
+-rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-10 11:03:10.018731 cvprocessor-0.2.0/setup.cfg
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-10 11:03:09.985305 cvprocessor-0.2.0/src/
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-10 11:03:10.008233 cvprocessor-0.2.0/src/cvprocessor/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.2.0/src/cvprocessor/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)     6651 2024-05-08 07:01:09.000000 cvprocessor-0.2.0/src/cvprocessor/authors.py
+-rw-r--r--   0 fernando   (501) staff       (20)      148 2024-05-04 10:32:46.000000 cvprocessor-0.2.0/src/cvprocessor/common.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4724 2024-05-10 11:02:21.000000 cvprocessor-0.2.0/src/cvprocessor/cv.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4218 2024-05-08 07:28:24.000000 cvprocessor-0.2.0/src/cvprocessor/education.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4633 2024-05-08 08:22:41.000000 cvprocessor-0.2.0/src/cvprocessor/experience.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2619 2024-05-08 07:09:50.000000 cvprocessor-0.2.0/src/cvprocessor/grants_awards.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4581 2024-05-10 10:56:41.000000 cvprocessor-0.2.0/src/cvprocessor/institutes.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1652 2024-05-08 07:13:23.000000 cvprocessor-0.2.0/src/cvprocessor/intro.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1533 2024-05-09 01:57:53.000000 cvprocessor-0.2.0/src/cvprocessor/memberships.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2466 2024-05-08 07:13:59.000000 cvprocessor-0.2.0/src/cvprocessor/news.py
+-rw-r--r--   0 fernando   (501) staff       (20)     9925 2024-05-08 07:18:36.000000 cvprocessor-0.2.0/src/cvprocessor/publications.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1866 2024-05-09 02:04:48.000000 cvprocessor-0.2.0/src/cvprocessor/references.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1133 2024-05-08 07:20:47.000000 cvprocessor-0.2.0/src/cvprocessor/research_interests.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1980 2024-05-09 01:44:15.000000 cvprocessor-0.2.0/src/cvprocessor/service.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2288 2024-05-09 01:28:30.000000 cvprocessor-0.2.0/src/cvprocessor/skills.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3509 2024-05-08 07:21:45.000000 cvprocessor-0.2.0/src/cvprocessor/software.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3754 2024-05-08 07:49:48.000000 cvprocessor-0.2.0/src/cvprocessor/supervision.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5394 2024-05-10 11:01:39.000000 cvprocessor-0.2.0/src/cvprocessor/teaching.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-10 11:03:10.016018 cvprocessor-0.2.0/src/cvprocessor.egg-info/
+-rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-10 11:03:09.000000 cvprocessor-0.2.0/src/cvprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)      771 2024-05-10 11:03:09.000000 cvprocessor-0.2.0/src/cvprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-10 11:03:09.000000 cvprocessor-0.2.0/src/cvprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-10 11:03:09.000000 cvprocessor-0.2.0/src/cvprocessor.egg-info/requires.txt
+-rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-10 11:03:09.000000 cvprocessor-0.2.0/src/cvprocessor.egg-info/top_level.txt
```

### Comparing `cvprocessor-0.1.0/LICENSE` & `cvprocessor-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.1.0/PKG-INFO` & `cvprocessor-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.1.0
+Version: 0.2.0
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.1.0/README.md` & `cvprocessor-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.1.0/pyproject.toml` & `cvprocessor-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cvprocessor"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
     { name = "F. Fernando Jurado-Lasso", email = "fdo.jurado@gmail.com" },
 ]
 description = "CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cvprocessor-0.1.0/src/cvprocessor/authors.py` & `cvprocessor-0.2.0/src/cvprocessor/authors.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.1.0/src/cvprocessor/cv.py` & `cvprocessor-0.2.0/src/cvprocessor/cv.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.1.0/src/cvprocessor/education.py` & `cvprocessor-0.2.0/src/cvprocessor/education.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.1.0/src/cvprocessor/experience.py` & `cvprocessor-0.2.0/src/cvprocessor/experience.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.1.0/src/cvprocessor/grants_awards.py` & `cvprocessor-0.2.0/src/cvprocessor/grants_awards.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.1.0/src/cvprocessor/institutes.py` & `cvprocessor-0.2.0/src/cvprocessor/institutes.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 class InstituteData:
     def __init__(self, pd_dataframe):
         self._pd_dataframe = pd_dataframe
         self._id = None
         self._name = None
         self._name_abbr = None
+        self._department = None
+        self._department_abbr = None
         self._address = None
         self._city = None
         self._country = None
         self._coordinates = None
         self._url = None
         self._load_institute()
 
@@ -25,14 +27,22 @@
     @property
     def name(self):
         return self._name
 
     @property
     def name_abbr(self):
         return self._name_abbr
+    
+    @property
+    def department(self):
+        return self._department
+    
+    @property
+    def department_abbr(self):
+        return self._department_abbr
 
     @property
     def address(self):
         return self._address
 
     @property
     def city(self):
@@ -69,25 +79,29 @@
                 coord) for coord in coordinates]
             self._coordinates = tuple(coordinates)
 
     def _load_institute(self):
         self._id = self._pd_dataframe["id"]
         self._name = self._pd_dataframe["Name"]
         self._name_abbr = self._pd_dataframe["Name Abbreviation"]
+        self._department = self._pd_dataframe["Department"]
+        self._department_abbr = self._pd_dataframe["Department Abbreviation"]
         self._address = self._pd_dataframe["Address"]
         self._city = self._pd_dataframe["City"]
         self._country = self._pd_dataframe["Country"]
         self._url = self._pd_dataframe["URL"]
         self._coordinates = self._pd_dataframe["Coordinates"]
         self.process_coordinates()
 
     def __str__(self):
         string = f"Institute ID: {self._id}\n"
         string += f"Institute Name: {self._name}\n"
         string += f"Institute Name Abbreviation: {self._name_abbr}\n"
+        string += f"Institute Department: {self._department}\n"
+        string += f"Institute Department Abbreviation: {self._department_abbr}\n"
         string += f"Institute Address: {self._address}\n"
         string += f"Institute City: {self._city}\n"
         string += f"Institute Country: {self._country}\n"
         string += f"Institute URL: {self._url}\n"
         string += f"Institute Coordinates: {self._coordinates}\n\n"
         return string
```

### Comparing `cvprocessor-0.1.0/src/cvprocessor/intro.py` & `cvprocessor-0.2.0/src/cvprocessor/intro.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.1.0/src/cvprocessor/memberships.py` & `cvprocessor-0.2.0/src/cvprocessor/memberships.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.1.0/src/cvprocessor/news.py` & `cvprocessor-0.2.0/src/cvprocessor/news.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.1.0/src/cvprocessor/publications.py` & `cvprocessor-0.2.0/src/cvprocessor/publications.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.1.0/src/cvprocessor/references.py` & `cvprocessor-0.2.0/src/cvprocessor/references.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.1.0/src/cvprocessor/research_interests.py` & `cvprocessor-0.2.0/src/cvprocessor/research_interests.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.1.0/src/cvprocessor/service.py` & `cvprocessor-0.2.0/src/cvprocessor/service.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.1.0/src/cvprocessor/skills.py` & `cvprocessor-0.2.0/src/cvprocessor/skills.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.1.0/src/cvprocessor/software.py` & `cvprocessor-0.2.0/src/cvprocessor/software.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.1.0/src/cvprocessor/supervision.py` & `cvprocessor-0.2.0/src/cvprocessor/supervision.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.1.0/src/cvprocessor/teaching.py` & `cvprocessor-0.2.0/src/cvprocessor/teaching.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,16 +8,14 @@
         self._start_year = None
         self._end_year = None
         self._position = None
         self._course = None
         self._link = None
         self._type = None
         self._institution = None
-        self._department = None
-        self._country = None
         self._supervisor = None
         self._responsibilities = None
         self._load_teaching()
 
     @property
     def filename(self):
         return self._filename
@@ -51,22 +49,14 @@
         return self._type
 
     @property
     def institution(self):
         return self._institution
 
     @property
-    def department(self):
-        return self._department
-
-    @property
-    def country(self):
-        return self._country
-
-    @property
     def supervisor(self):
         return self._supervisor
 
     @property
     def responsibilities(self):
         return self._responsibilities
 
@@ -121,30 +111,26 @@
         self._start_year = self.get_start_year()
         self._end_year = self.get_end_year()
         self._position = self.filename["Position"]
         self._course = self.filename["Course"]
         self._link = self.filename["Link"]
         self._type = self.filename["Type"]
         self._institution = self.filename["Institution"]
-        self._department = self.filename["Department"]
-        self._country = self.filename["Country"]
         self._supervisor = self.filename["Supervisor"]
         self._responsibilities = self.filename["Responsibilities"]
 
     def __str__(self):
         string = f"Year: {self.year}\n"
         string += f"Start year: {self.start_year}\n"
         string += f"End year: {self.end_year}\n"
         string += f"Position: {self.position}\n"
         string += f"Course: {self.course}\n"
         string += f"Link: {self.link}\n"
         string += f"Type: {self.type}\n"
         string += f"Institution: {self.institution}\n"
-        string += f"Department: {self.department}\n"
-        string += f"Country: {self.country}\n"
         string += f"Supervisor: {self.supervisor}\n"
         string += f"Responsibilities: {self.responsibilities}\n\n"
         return string
 
     def __repr__(self):
         string = f"TeachingData(year={self.year}, start_year={self.start_year}, end_year={self.end_year}, position={self.position}, course={self.course}, link={self.link}, type={self.type}, institution={self.institution}, department={self.department}, country={self.country}, supervisor={self.supervisor}, responsibilities={self.responsibilities})"
         return string
```

### Comparing `cvprocessor-0.1.0/src/cvprocessor.egg-info/PKG-INFO` & `cvprocessor-0.2.0/src/cvprocessor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.1.0
+Version: 0.2.0
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.1.0/src/cvprocessor.egg-info/SOURCES.txt` & `cvprocessor-0.2.0/src/cvprocessor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

