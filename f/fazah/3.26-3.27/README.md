# Comparing `tmp/fazah-3.26.tar.gz` & `tmp/fazah-3.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fazah-3.26.tar", last modified: Fri May  3 22:23:27 2024, max compression
+gzip compressed data, was "fazah-3.27.tar", last modified: Sat May 11 19:22:50 2024, max compression
```

## Comparing `fazah-3.26.tar` & `fazah-3.27.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 22:23:27.396772 fazah-3.26/
-drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 22:23:27.395114 fazah-3.26/Fazah/
--rw-r--r--   0 aidenlang   (502) staff       (20)       30 2024-05-03 22:21:19.000000 fazah-3.26/Fazah/__init__.py
--rw-r--r--   0 aidenlang   (502) staff       (20)     1219 2024-05-03 22:21:03.000000 fazah-3.26/Fazah/fazahclass.py
--rw-r--r--   0 aidenlang   (502) staff       (20)      365 2024-05-03 22:23:27.396564 fazah-3.26/PKG-INFO
-drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 22:23:27.396318 fazah-3.26/fazah.egg-info/
--rw-r--r--   0 aidenlang   (502) staff       (20)      365 2024-05-03 22:23:27.000000 fazah-3.26/fazah.egg-info/PKG-INFO
--rw-r--r--   0 aidenlang   (502) staff       (20)      232 2024-05-03 22:23:27.000000 fazah-3.26/fazah.egg-info/SOURCES.txt
--rw-r--r--   0 aidenlang   (502) staff       (20)        1 2024-05-03 22:23:27.000000 fazah-3.26/fazah.egg-info/dependency_links.txt
--rw-r--r--   0 aidenlang   (502) staff       (20)       27 2024-05-03 22:23:27.000000 fazah-3.26/fazah.egg-info/requires.txt
--rw-r--r--   0 aidenlang   (502) staff       (20)        6 2024-05-03 22:23:27.000000 fazah-3.26/fazah.egg-info/top_level.txt
--rw-r--r--   0 aidenlang   (502) staff       (20)       38 2024-05-03 22:23:27.396813 fazah-3.26/setup.cfg
--rw-r--r--   0 aidenlang   (502) staff       (20)      496 2024-05-03 22:23:11.000000 fazah-3.26/setup.py
-drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 22:23:27.396009 fazah-3.26/tests/
--rw-r--r--   0 aidenlang   (502) staff       (20)     1218 2024-05-03 06:26:06.000000 fazah-3.26/tests/test.openai.py
--rw-r--r--   0 aidenlang   (502) staff       (20)     1320 2024-05-03 06:22:39.000000 fazah-3.26/tests/test_gemini.py
+drwxr-xr-x   0 will       (501) staff       (20)        0 2024-05-11 19:22:50.889044 fazah-3.27/
+drwxr-xr-x   0 will       (501) staff       (20)        0 2024-05-11 19:22:50.887585 fazah-3.27/Fazah/
+-rw-r--r--   0 will       (501) staff       (20)       30 2024-05-11 19:19:48.000000 fazah-3.27/Fazah/__init__.py
+-rw-r--r--   0 will       (501) staff       (20)     1219 2024-05-11 19:19:43.000000 fazah-3.27/Fazah/fazahclass.py
+-rw-r--r--   0 will       (501) staff       (20)      308 2024-05-11 19:22:50.888920 fazah-3.27/PKG-INFO
+drwxr-xr-x   0 will       (501) staff       (20)        0 2024-05-11 19:22:50.888462 fazah-3.27/fazah.egg-info/
+-rw-r--r--   0 will       (501) staff       (20)      308 2024-05-11 19:22:50.000000 fazah-3.27/fazah.egg-info/PKG-INFO
+-rw-r--r--   0 will       (501) staff       (20)      232 2024-05-11 19:22:50.000000 fazah-3.27/fazah.egg-info/SOURCES.txt
+-rw-r--r--   0 will       (501) staff       (20)        1 2024-05-11 19:22:50.000000 fazah-3.27/fazah.egg-info/dependency_links.txt
+-rw-r--r--   0 will       (501) staff       (20)       27 2024-05-11 19:22:50.000000 fazah-3.27/fazah.egg-info/requires.txt
+-rw-r--r--   0 will       (501) staff       (20)        6 2024-05-11 19:22:50.000000 fazah-3.27/fazah.egg-info/top_level.txt
+-rw-r--r--   0 will       (501) staff       (20)       38 2024-05-11 19:22:50.889100 fazah-3.27/setup.cfg
+-rw-r--r--   0 will       (501) staff       (20)      496 2024-05-11 19:22:26.000000 fazah-3.27/setup.py
+drwxr-xr-x   0 will       (501) staff       (20)        0 2024-05-11 19:22:50.888739 fazah-3.27/tests/
+-rw-r--r--   0 will       (501) staff       (20)     1218 2024-05-03 22:27:31.000000 fazah-3.27/tests/test.openai.py
+-rw-r--r--   0 will       (501) staff       (20)     1320 2024-05-11 19:21:49.000000 fazah-3.27/tests/test_gemini.py
```

### Comparing `fazah-3.26/Fazah/fazahclass.py` & `fazah-3.27/Fazah/fazahclass.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from deep_translator import GoogleTranslator
 from langdetect import detect
 
-class fazah:
+class Fazah:
     def __init__(self, llm_model):
         self.llm_model = llm_model
         self.translator = GoogleTranslator(source='auto', target='en')
 
     def process_text(self, text):
         try:
             if not text.strip():
```

### Comparing `fazah-3.26/tests/test.openai.py` & `fazah-3.27/tests/test.openai.py`

 * *Files identical despite different names*

### Comparing `fazah-3.26/tests/test_gemini.py` & `fazah-3.27/tests/test_gemini.py`

 * *Files identical despite different names*

