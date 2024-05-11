# Comparing `tmp/niwatoko-1.1.0.tar.gz` & `tmp/niwatoko-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niwatoko-1.1.0.tar", last modified: Sat May 11 00:20:12 2024, max compression
+gzip compressed data, was "niwatoko-1.1.1.tar", last modified: Sat May 11 00:21:15 2024, max compression
```

## Comparing `niwatoko-1.1.0.tar` & `niwatoko-1.1.1.tar`

### file list

```diff
@@ -1,41 +1,49 @@
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 00:20:12.783287 niwatoko-1.1.0/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    11356 2024-05-07 05:52:57.000000 niwatoko-1.1.0/LICENSE
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    16804 2024-05-11 00:20:12.783051 niwatoko-1.1.0/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    15918 2024-05-07 02:46:41.000000 niwatoko-1.1.0/README.md
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 00:20:12.777667 niwatoko-1.1.0/niwatoko/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      166 2024-05-07 22:46:07.000000 niwatoko-1.1.0/niwatoko/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3258 2024-05-11 00:13:31.000000 niwatoko-1.1.0/niwatoko/cli.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 00:20:12.776614 niwatoko-1.1.0/niwatoko/foundation_model/
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 00:20:12.776652 niwatoko-1.1.0/niwatoko/foundation_model/interpretation/
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 00:20:12.778839 niwatoko-1.1.0/niwatoko/foundation_model/interpretation/llm/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1346 2024-05-08 23:04:24.000000 niwatoko-1.1.0/niwatoko/foundation_model/interpretation/llm/claude.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1428 2024-05-08 23:04:24.000000 niwatoko-1.1.0/niwatoko/foundation_model/interpretation/llm/gpt.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 00:20:12.779035 niwatoko-1.1.0/niwatoko/grammar/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      685 2024-05-08 23:04:24.000000 niwatoko-1.1.0/niwatoko/grammar/system.md
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 00:20:12.778524 niwatoko-1.1.0/niwatoko.egg-info/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    16804 2024-05-11 00:20:12.000000 niwatoko-1.1.0/niwatoko.egg-info/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      859 2024-05-11 00:20:12.000000 niwatoko-1.1.0/niwatoko.egg-info/SOURCES.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-05-11 00:20:12.000000 niwatoko-1.1.0/niwatoko.egg-info/dependency_links.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-05-11 00:20:12.000000 niwatoko-1.1.0/niwatoko.egg-info/entry_points.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       34 2024-05-11 00:20:12.000000 niwatoko-1.1.0/niwatoko.egg-info/requires.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       15 2024-05-11 00:20:12.000000 niwatoko-1.1.0/niwatoko.egg-info/top_level.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-05-11 00:20:12.783330 niwatoko-1.1.0/setup.cfg
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1697 2024-05-11 00:19:20.000000 niwatoko-1.1.0/setup.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 00:20:12.780742 niwatoko-1.1.0/tests/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     5897 2024-05-08 23:04:24.000000 niwatoko-1.1.0/tests/README.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2077 2024-05-07 02:46:41.000000 niwatoko-1.1.0/tests/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3754 2024-05-08 23:03:26.000000 niwatoko-1.1.0/tests/test_compiler.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     4529 2024-05-08 23:03:26.000000 niwatoko-1.1.0/tests/test_compiler.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3940 2024-05-08 23:04:26.000000 niwatoko-1.1.0/tests/test_compiler_v1_2.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 00:20:12.782700 niwatoko-1.1.0/tests/test_docs/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2747 2024-05-07 02:46:41.000000 niwatoko-1.1.0/tests/test_docs/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2609 2024-05-07 05:48:44.000000 niwatoko-1.1.0/tests/test_docs/test_doc1.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2853 2024-05-07 05:48:44.000000 niwatoko-1.1.0/tests/test_docs/test_doc2.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2625 2024-05-07 05:48:44.000000 niwatoko-1.1.0/tests/test_docs/test_doc3.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1678 2024-05-07 22:46:07.000000 niwatoko-1.1.0/tests/test_docs/test_gen_github_issue.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1950 2024-05-07 22:46:07.000000 niwatoko-1.1.0/tests/test_docs/test_gen_grimoire.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1909 2024-05-07 22:46:07.000000 niwatoko-1.1.0/tests/test_docs/test_gen_grimoire2.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1850 2024-05-07 22:46:07.000000 niwatoko-1.1.0/tests/test_docs/test_gen_grimoire_en.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     5307 2024-05-07 05:52:23.000000 niwatoko-1.1.0/tests/test_docs/test_gen_zoltraak_pypi.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2216 2024-05-07 02:46:41.000000 niwatoko-1.1.0/tests/test_interpreter.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2632 2024-05-07 02:46:41.000000 niwatoko-1.1.0/tests/test_parser.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 00:21:15.428586 niwatoko-1.1.1/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    11356 2024-05-07 05:52:57.000000 niwatoko-1.1.1/LICENSE
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    16804 2024-05-11 00:21:15.428197 niwatoko-1.1.1/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    15918 2024-05-07 02:46:41.000000 niwatoko-1.1.1/README.md
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 00:21:15.418679 niwatoko-1.1.1/niwatoko/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      166 2024-05-07 22:46:07.000000 niwatoko-1.1.1/niwatoko/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     4619 2024-05-11 00:20:33.000000 niwatoko-1.1.1/niwatoko/cli.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 00:21:15.417505 niwatoko-1.1.1/niwatoko/foundation_model/
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 00:21:15.417546 niwatoko-1.1.1/niwatoko/foundation_model/interpretation/
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 00:21:15.419732 niwatoko-1.1.1/niwatoko/foundation_model/interpretation/llm/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1346 2024-05-08 23:04:24.000000 niwatoko-1.1.1/niwatoko/foundation_model/interpretation/llm/claude.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1428 2024-05-08 23:04:24.000000 niwatoko-1.1.1/niwatoko/foundation_model/interpretation/llm/gpt.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 00:21:15.419982 niwatoko-1.1.1/niwatoko/grammar/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      685 2024-05-08 23:04:24.000000 niwatoko-1.1.1/niwatoko/grammar/system.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       33 2024-05-11 00:20:33.000000 niwatoko-1.1.1/niwatoko/temp.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 00:21:15.419356 niwatoko-1.1.1/niwatoko.egg-info/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    16804 2024-05-11 00:21:15.000000 niwatoko-1.1.1/niwatoko.egg-info/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1123 2024-05-11 00:21:15.000000 niwatoko-1.1.1/niwatoko.egg-info/SOURCES.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-05-11 00:21:15.000000 niwatoko-1.1.1/niwatoko.egg-info/dependency_links.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-05-11 00:21:15.000000 niwatoko-1.1.1/niwatoko.egg-info/entry_points.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       34 2024-05-11 00:21:15.000000 niwatoko-1.1.1/niwatoko.egg-info/requires.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       15 2024-05-11 00:21:15.000000 niwatoko-1.1.1/niwatoko.egg-info/top_level.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-05-11 00:21:15.428628 niwatoko-1.1.1/setup.cfg
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1697 2024-05-11 00:21:14.000000 niwatoko-1.1.1/setup.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 00:21:15.421787 niwatoko-1.1.1/tests/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     5897 2024-05-08 23:04:24.000000 niwatoko-1.1.1/tests/README.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2077 2024-05-07 02:46:41.000000 niwatoko-1.1.1/tests/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3754 2024-05-08 23:03:26.000000 niwatoko-1.1.1/tests/test_compiler.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     4529 2024-05-08 23:03:26.000000 niwatoko-1.1.1/tests/test_compiler.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3940 2024-05-08 23:04:26.000000 niwatoko-1.1.1/tests/test_compiler_v1_2.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 00:21:15.427762 niwatoko-1.1.1/tests/test_docs/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2747 2024-05-07 02:46:41.000000 niwatoko-1.1.1/tests/test_docs/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2030 2024-05-11 00:20:33.000000 niwatoko-1.1.1/tests/test_docs/output copy.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1987 2024-05-11 00:20:33.000000 niwatoko-1.1.1/tests/test_docs/output.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1733 2024-05-11 00:20:33.000000 niwatoko-1.1.1/tests/test_docs/output_.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2609 2024-05-07 05:48:44.000000 niwatoko-1.1.1/tests/test_docs/test_doc1.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2853 2024-05-07 05:48:44.000000 niwatoko-1.1.1/tests/test_docs/test_doc2.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2625 2024-05-07 05:48:44.000000 niwatoko-1.1.1/tests/test_docs/test_doc3.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1678 2024-05-07 22:46:07.000000 niwatoko-1.1.1/tests/test_docs/test_gen_github_issue.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1950 2024-05-07 22:46:07.000000 niwatoko-1.1.1/tests/test_docs/test_gen_grimoire.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1909 2024-05-07 22:46:07.000000 niwatoko-1.1.1/tests/test_docs/test_gen_grimoire2.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1850 2024-05-07 22:46:07.000000 niwatoko-1.1.1/tests/test_docs/test_gen_grimoire_en.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     5307 2024-05-07 05:52:23.000000 niwatoko-1.1.1/tests/test_docs/test_gen_zoltraak_pypi.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     6179 2024-05-11 00:20:33.000000 niwatoko-1.1.1/tests/test_docs/test_import_function.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      201 2024-05-11 00:20:33.000000 niwatoko-1.1.1/tests/test_docs/test_import_md.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      787 2024-05-11 00:20:33.000000 niwatoko-1.1.1/tests/test_docs/test_import_module_add.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      800 2024-05-11 00:20:33.000000 niwatoko-1.1.1/tests/test_docs/test_import_module_multiple.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2216 2024-05-07 02:46:41.000000 niwatoko-1.1.1/tests/test_interpreter.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2632 2024-05-07 02:46:41.000000 niwatoko-1.1.1/tests/test_parser.py
```

### Comparing `niwatoko-1.1.0/LICENSE` & `niwatoko-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.0/PKG-INFO` & `niwatoko-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niwatoko
-Version: 1.1.0
+Version: 1.1.1
 Summary: 自然言語でプログラミングを行うことができる新しいプログラミング言語
 Home-page: https://niwatoko2.vercel.app/
 Author: dai-motoki
 Author-email: dai.motoki1123@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
```

### Comparing `niwatoko-1.1.0/README.md` & `niwatoko-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.0/niwatoko/foundation_model/interpretation/llm/claude.py` & `niwatoko-1.1.1/niwatoko/foundation_model/interpretation/llm/claude.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.0/niwatoko/foundation_model/interpretation/llm/gpt.py` & `niwatoko-1.1.1/niwatoko/foundation_model/interpretation/llm/gpt.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.0/niwatoko/grammar/system.md` & `niwatoko-1.1.1/niwatoko/grammar/system.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.0/niwatoko.egg-info/PKG-INFO` & `niwatoko-1.1.1/niwatoko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niwatoko
-Version: 1.1.0
+Version: 1.1.1
 Summary: 自然言語でプログラミングを行うことができる新しいプログラミング言語
 Home-page: https://niwatoko2.vercel.app/
 Author: dai-motoki
 Author-email: dai.motoki1123@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
```

### Comparing `niwatoko-1.1.0/niwatoko.egg-info/SOURCES.txt` & `niwatoko-1.1.1/niwatoko.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.py
 niwatoko/__init__.py
 niwatoko/cli.py
+niwatoko/temp.py
 niwatoko.egg-info/PKG-INFO
 niwatoko.egg-info/SOURCES.txt
 niwatoko.egg-info/dependency_links.txt
 niwatoko.egg-info/entry_points.txt
 niwatoko.egg-info/requires.txt
 niwatoko.egg-info/top_level.txt
 niwatoko/foundation_model/interpretation/llm/claude.py
@@ -16,15 +17,22 @@
 tests/__init__.py
 tests/test_compiler.md
 tests/test_compiler.py
 tests/test_compiler_v1_2.py
 tests/test_interpreter.py
 tests/test_parser.py
 tests/test_docs/__init__.py
+tests/test_docs/output copy.md
+tests/test_docs/output.md
+tests/test_docs/output_.md
 tests/test_docs/test_doc1.md
 tests/test_docs/test_doc2.md
 tests/test_docs/test_doc3.md
 tests/test_docs/test_gen_github_issue.md
 tests/test_docs/test_gen_grimoire.md
 tests/test_docs/test_gen_grimoire2.md
 tests/test_docs/test_gen_grimoire_en.md
-tests/test_docs/test_gen_zoltraak_pypi.md
+tests/test_docs/test_gen_zoltraak_pypi.md
+tests/test_docs/test_import_function.md
+tests/test_docs/test_import_md.md
+tests/test_docs/test_import_module_add.py
+tests/test_docs/test_import_module_multiple.py
```

### Comparing `niwatoko-1.1.0/setup.py` & `niwatoko-1.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # niwatoko - 自然言語プログラミング言語のPythonパッケージのsetup.pyファイルです。
 # このファイルはパッケージのインストールや配布に必要な情報を含んでいます。
 
 from setuptools import setup, find_packages
 
 setup(
     name='niwatoko',
-    version='1.1.0',
+    version='1.1.1',
     description='自然言語でプログラミングを行うことができる新しいプログラミング言語',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='dai-motoki',
     author_email='dai.motoki1123@gmail.com',
     url='https://niwatoko2.vercel.app/',
     packages=find_packages(),
```

### Comparing `niwatoko-1.1.0/tests/README.md` & `niwatoko-1.1.1/tests/README.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.0/tests/__init__.py` & `niwatoko-1.1.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.0/tests/test_compiler.md` & `niwatoko-1.1.1/tests/test_compiler.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.0/tests/test_compiler.py` & `niwatoko-1.1.1/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.0/tests/test_compiler_v1_2.py` & `niwatoko-1.1.1/tests/test_compiler_v1_2.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.0/tests/test_docs/__init__.py` & `niwatoko-1.1.1/tests/test_docs/__init__.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.0/tests/test_docs/test_doc1.md` & `niwatoko-1.1.1/tests/test_docs/test_doc1.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.0/tests/test_docs/test_doc2.md` & `niwatoko-1.1.1/tests/test_docs/test_doc2.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.0/tests/test_docs/test_doc3.md` & `niwatoko-1.1.1/tests/test_docs/test_doc3.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.0/tests/test_docs/test_gen_github_issue.md` & `niwatoko-1.1.1/tests/test_docs/test_gen_github_issue.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.0/tests/test_docs/test_gen_grimoire.md` & `niwatoko-1.1.1/tests/test_docs/test_gen_grimoire.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.0/tests/test_docs/test_gen_grimoire2.md` & `niwatoko-1.1.1/tests/test_docs/test_gen_grimoire2.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.0/tests/test_docs/test_gen_grimoire_en.md` & `niwatoko-1.1.1/tests/test_docs/test_gen_grimoire_en.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.0/tests/test_docs/test_gen_zoltraak_pypi.md` & `niwatoko-1.1.1/tests/test_docs/test_gen_zoltraak_pypi.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.0/tests/test_interpreter.py` & `niwatoko-1.1.1/tests/test_interpreter.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.0/tests/test_parser.py` & `niwatoko-1.1.1/tests/test_parser.py`

 * *Files identical despite different names*

