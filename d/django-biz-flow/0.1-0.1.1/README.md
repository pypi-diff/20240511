# Comparing `tmp/django-biz-flow-0.1.tar.gz` & `tmp/django-biz-flow-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-biz-flow-0.1.tar", last modified: Thu May  9 16:50:00 2024, max compression
+gzip compressed data, was "dist/django-biz-flow-0.1.1.tar", last modified: Sat May 11 09:01:40 2024, max compression
```

## Comparing `django-biz-flow-0.1.tar` & `django-biz-flow-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 newuser    (501) staff       (20)        0 2024-05-09 16:50:00.000000 django-biz-flow-0.1/
--rw-r--r--   0 newuser    (501) staff       (20)      940 2024-05-09 16:50:00.000000 django-biz-flow-0.1/PKG-INFO
--rw-r--r--   0 newuser    (501) staff       (20)     1039 2024-05-09 16:34:19.000000 django-biz-flow-0.1/LICENSE
--rw-r--r--   0 newuser    (501) staff       (20)       34 2024-05-09 16:48:49.000000 django-biz-flow-0.1/MANIFEST.in
-drwxr-xr-x   0 newuser    (501) staff       (20)        0 2024-05-09 16:50:00.000000 django-biz-flow-0.1/django_biz_flow.egg-info/
--rw-r--r--   0 newuser    (501) staff       (20)      940 2024-05-09 16:50:00.000000 django-biz-flow-0.1/django_biz_flow.egg-info/PKG-INFO
--rw-r--r--   0 newuser    (501) staff       (20)      641 2024-05-09 16:50:00.000000 django-biz-flow-0.1/django_biz_flow.egg-info/SOURCES.txt
--rw-r--r--   0 newuser    (501) staff       (20)       12 2024-05-09 16:50:00.000000 django-biz-flow-0.1/django_biz_flow.egg-info/requires.txt
--rw-r--r--   0 newuser    (501) staff       (20)       11 2024-05-09 16:50:00.000000 django-biz-flow-0.1/django_biz_flow.egg-info/top_level.txt
--rw-r--r--   0 newuser    (501) staff       (20)        1 2024-05-09 16:50:00.000000 django-biz-flow-0.1/django_biz_flow.egg-info/dependency_links.txt
--rw-r--r--   0 newuser    (501) staff       (20)       36 2024-05-09 16:36:10.000000 django-biz-flow-0.1/setup.py
--rw-r--r--   0 newuser    (501) staff       (20)      923 2024-05-09 16:50:00.000000 django-biz-flow-0.1/setup.cfg
--rw-r--r--   0 newuser    (501) staff       (20)        0 2024-05-09 16:24:22.000000 django-biz-flow-0.1/README.rst
-drwxr-xr-x   0 newuser    (501) staff       (20)        0 2024-05-09 16:50:00.000000 django-biz-flow-0.1/onboarding/
-drwxr-xr-x   0 newuser    (501) staff       (20)        0 2024-05-09 16:50:00.000000 django-biz-flow-0.1/onboarding/migrations/
--rw-r--r--   0 newuser    (501) staff       (20)      564 2024-05-09 16:23:43.000000 django-biz-flow-0.1/onboarding/migrations/0003_personaldetails_user.py
--rw-r--r--   0 newuser    (501) staff       (20)      594 2024-05-09 16:23:43.000000 django-biz-flow-0.1/onboarding/migrations/0004_alter_personaldetails_user.py
--rw-r--r--   0 newuser    (501) staff       (20)     2348 2024-05-09 16:23:43.000000 django-biz-flow-0.1/onboarding/migrations/0002_personaldetails_businessprofile_and_more.py
--rw-r--r--   0 newuser    (501) staff       (20)        0 2024-05-09 16:23:43.000000 django-biz-flow-0.1/onboarding/migrations/__init__.py
--rw-r--r--   0 newuser    (501) staff       (20)     1237 2024-05-09 16:23:43.000000 django-biz-flow-0.1/onboarding/migrations/0001_initial.py
--rw-r--r--   0 newuser    (501) staff       (20)     1273 2024-05-09 16:23:43.000000 django-biz-flow-0.1/onboarding/models.py
--rw-r--r--   0 newuser    (501) staff       (20)        0 2024-05-09 16:23:43.000000 django-biz-flow-0.1/onboarding/__init__.py
--rw-r--r--   0 newuser    (501) staff       (20)      152 2024-05-09 16:23:43.000000 django-biz-flow-0.1/onboarding/apps.py
--rw-r--r--   0 newuser    (501) staff       (20)      584 2024-05-09 16:23:43.000000 django-biz-flow-0.1/onboarding/admin.py
--rw-r--r--   0 newuser    (501) staff       (20)     4390 2024-05-09 16:23:43.000000 django-biz-flow-0.1/onboarding/serializer.py
--rw-r--r--   0 newuser    (501) staff       (20)       60 2024-05-09 16:23:43.000000 django-biz-flow-0.1/onboarding/tests.py
--rw-r--r--   0 newuser    (501) staff       (20)      677 2024-05-09 16:23:43.000000 django-biz-flow-0.1/onboarding/urls.py
+drwxr-xr-x   0 newuser    (501) staff       (20)        0 2024-05-11 09:01:40.000000 django-biz-flow-0.1.1/
+-rw-r--r--   0 newuser    (501) staff       (20)      952 2024-05-11 09:01:40.000000 django-biz-flow-0.1.1/PKG-INFO
+-rw-r--r--   0 newuser    (501) staff       (20)     1039 2024-05-09 16:34:19.000000 django-biz-flow-0.1.1/LICENSE
+-rw-r--r--   0 newuser    (501) staff       (20)       34 2024-05-09 16:48:49.000000 django-biz-flow-0.1.1/MANIFEST.in
+drwxr-xr-x   0 newuser    (501) staff       (20)        0 2024-05-11 09:01:40.000000 django-biz-flow-0.1.1/django_biz_flow/
+-rw-r--r--   0 newuser    (501) staff       (20)        0 2024-05-11 08:53:55.000000 django-biz-flow-0.1.1/django_biz_flow/__init__.py
+drwxr-xr-x   0 newuser    (501) staff       (20)        0 2024-05-11 09:01:40.000000 django-biz-flow-0.1.1/django_biz_flow/onboarding/
+drwxr-xr-x   0 newuser    (501) staff       (20)        0 2024-05-11 09:01:40.000000 django-biz-flow-0.1.1/django_biz_flow/onboarding/migrations/
+-rw-r--r--   0 newuser    (501) staff       (20)      564 2024-05-09 16:23:43.000000 django-biz-flow-0.1.1/django_biz_flow/onboarding/migrations/0003_personaldetails_user.py
+-rw-r--r--   0 newuser    (501) staff       (20)      594 2024-05-09 16:23:43.000000 django-biz-flow-0.1.1/django_biz_flow/onboarding/migrations/0004_alter_personaldetails_user.py
+-rw-r--r--   0 newuser    (501) staff       (20)     2348 2024-05-09 16:23:43.000000 django-biz-flow-0.1.1/django_biz_flow/onboarding/migrations/0002_personaldetails_businessprofile_and_more.py
+-rw-r--r--   0 newuser    (501) staff       (20)        0 2024-05-09 16:23:43.000000 django-biz-flow-0.1.1/django_biz_flow/onboarding/migrations/__init__.py
+-rw-r--r--   0 newuser    (501) staff       (20)     1237 2024-05-09 16:23:43.000000 django-biz-flow-0.1.1/django_biz_flow/onboarding/migrations/0001_initial.py
+-rw-r--r--   0 newuser    (501) staff       (20)     1273 2024-05-09 16:23:43.000000 django-biz-flow-0.1.1/django_biz_flow/onboarding/models.py
+-rw-r--r--   0 newuser    (501) staff       (20)        0 2024-05-09 16:23:43.000000 django-biz-flow-0.1.1/django_biz_flow/onboarding/__init__.py
+-rw-r--r--   0 newuser    (501) staff       (20)      152 2024-05-09 16:23:43.000000 django-biz-flow-0.1.1/django_biz_flow/onboarding/apps.py
+-rw-r--r--   0 newuser    (501) staff       (20)      584 2024-05-09 16:23:43.000000 django-biz-flow-0.1.1/django_biz_flow/onboarding/admin.py
+-rw-r--r--   0 newuser    (501) staff       (20)     4390 2024-05-09 16:23:43.000000 django-biz-flow-0.1.1/django_biz_flow/onboarding/serializer.py
+-rw-r--r--   0 newuser    (501) staff       (20)       60 2024-05-09 16:23:43.000000 django-biz-flow-0.1.1/django_biz_flow/onboarding/tests.py
+-rw-r--r--   0 newuser    (501) staff       (20)      677 2024-05-09 16:23:43.000000 django-biz-flow-0.1.1/django_biz_flow/onboarding/urls.py
+drwxr-xr-x   0 newuser    (501) staff       (20)        0 2024-05-11 09:01:40.000000 django-biz-flow-0.1.1/django_biz_flow.egg-info/
+-rw-r--r--   0 newuser    (501) staff       (20)      952 2024-05-11 09:01:40.000000 django-biz-flow-0.1.1/django_biz_flow.egg-info/PKG-INFO
+-rw-r--r--   0 newuser    (501) staff       (20)      861 2024-05-11 09:01:40.000000 django-biz-flow-0.1.1/django_biz_flow.egg-info/SOURCES.txt
+-rw-r--r--   0 newuser    (501) staff       (20)       12 2024-05-11 09:01:40.000000 django-biz-flow-0.1.1/django_biz_flow.egg-info/requires.txt
+-rw-r--r--   0 newuser    (501) staff       (20)       16 2024-05-11 09:01:40.000000 django-biz-flow-0.1.1/django_biz_flow.egg-info/top_level.txt
+-rw-r--r--   0 newuser    (501) staff       (20)        1 2024-05-11 09:01:40.000000 django-biz-flow-0.1.1/django_biz_flow.egg-info/dependency_links.txt
+-rw-r--r--   0 newuser    (501) staff       (20)       36 2024-05-09 16:36:10.000000 django-biz-flow-0.1.1/setup.py
+-rw-r--r--   0 newuser    (501) staff       (20)      935 2024-05-11 09:01:40.000000 django-biz-flow-0.1.1/setup.cfg
+-rw-r--r--   0 newuser    (501) staff       (20)        0 2024-05-09 16:24:22.000000 django-biz-flow-0.1.1/README.rst
```

### Comparing `django-biz-flow-0.1/PKG-INFO` & `django-biz-flow-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 1.2
 Name: django-biz-flow
-Version: 0.1
-Summary: A Django app to conduct web-based polls.
+Version: 0.1.1
+Summary: A Django Package to streamline business functions.
 Home-page: https://www.example.com/
 Author: Joseph Braide
 Author-email: braidej@gmail.com
 License: BSD-3-Clause
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-biz-flow-0.1/LICENSE` & `django-biz-flow-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-biz-flow-0.1/django_biz_flow.egg-info/PKG-INFO` & `django-biz-flow-0.1.1/django_biz_flow.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 1.2
 Name: django-biz-flow
-Version: 0.1
-Summary: A Django app to conduct web-based polls.
+Version: 0.1.1
+Summary: A Django Package to streamline business functions.
 Home-page: https://www.example.com/
 Author: Joseph Braide
 Author-email: braidej@gmail.com
 License: BSD-3-Clause
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-biz-flow-0.1/setup.cfg` & `django-biz-flow-0.1.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = django-biz-flow
-version = 0.1
-description = A Django app to conduct web-based polls.
+version = 0.1.1
+description = A Django Package to streamline business functions.
 long_description = file: README.rst
 url = https://www.example.com/
 author = Joseph Braide
 author_email = braidej@gmail.com
 license = BSD-3-Clause
 classifiers = 
 	Environment :: Web Environment
```

### Comparing `django-biz-flow-0.1/onboarding/migrations/0003_personaldetails_user.py` & `django-biz-flow-0.1.1/django_biz_flow/onboarding/migrations/0003_personaldetails_user.py`

 * *Files identical despite different names*

### Comparing `django-biz-flow-0.1/onboarding/migrations/0004_alter_personaldetails_user.py` & `django-biz-flow-0.1.1/django_biz_flow/onboarding/migrations/0004_alter_personaldetails_user.py`

 * *Files identical despite different names*

### Comparing `django-biz-flow-0.1/onboarding/migrations/0002_personaldetails_businessprofile_and_more.py` & `django-biz-flow-0.1.1/django_biz_flow/onboarding/migrations/0002_personaldetails_businessprofile_and_more.py`

 * *Files identical despite different names*

### Comparing `django-biz-flow-0.1/onboarding/migrations/0001_initial.py` & `django-biz-flow-0.1.1/django_biz_flow/onboarding/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-biz-flow-0.1/onboarding/models.py` & `django-biz-flow-0.1.1/django_biz_flow/onboarding/models.py`

 * *Files identical despite different names*

### Comparing `django-biz-flow-0.1/onboarding/admin.py` & `django-biz-flow-0.1.1/django_biz_flow/onboarding/admin.py`

 * *Files identical despite different names*

### Comparing `django-biz-flow-0.1/onboarding/serializer.py` & `django-biz-flow-0.1.1/django_biz_flow/onboarding/serializer.py`

 * *Files identical despite different names*

### Comparing `django-biz-flow-0.1/onboarding/urls.py` & `django-biz-flow-0.1.1/django_biz_flow/onboarding/urls.py`

 * *Files identical despite different names*

