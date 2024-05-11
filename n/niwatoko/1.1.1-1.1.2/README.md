# Comparing `tmp/niwatoko-1.1.1.tar.gz` & `tmp/niwatoko-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niwatoko-1.1.1.tar", last modified: Sat May 11 00:21:15 2024, max compression
+gzip compressed data, was "niwatoko-1.1.2.tar", last modified: Sat May 11 04:46:07 2024, max compression
```

## Comparing `niwatoko-1.1.1.tar` & `niwatoko-1.1.2.tar`

### file list

```diff
@@ -1,49 +1,47 @@
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 00:21:15.428586 niwatoko-1.1.1/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    11356 2024-05-07 05:52:57.000000 niwatoko-1.1.1/LICENSE
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    16804 2024-05-11 00:21:15.428197 niwatoko-1.1.1/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    15918 2024-05-07 02:46:41.000000 niwatoko-1.1.1/README.md
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 00:21:15.418679 niwatoko-1.1.1/niwatoko/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      166 2024-05-07 22:46:07.000000 niwatoko-1.1.1/niwatoko/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     4619 2024-05-11 00:20:33.000000 niwatoko-1.1.1/niwatoko/cli.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 00:21:15.417505 niwatoko-1.1.1/niwatoko/foundation_model/
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 00:21:15.417546 niwatoko-1.1.1/niwatoko/foundation_model/interpretation/
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 00:21:15.419732 niwatoko-1.1.1/niwatoko/foundation_model/interpretation/llm/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1346 2024-05-08 23:04:24.000000 niwatoko-1.1.1/niwatoko/foundation_model/interpretation/llm/claude.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1428 2024-05-08 23:04:24.000000 niwatoko-1.1.1/niwatoko/foundation_model/interpretation/llm/gpt.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 00:21:15.419982 niwatoko-1.1.1/niwatoko/grammar/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      685 2024-05-08 23:04:24.000000 niwatoko-1.1.1/niwatoko/grammar/system.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       33 2024-05-11 00:20:33.000000 niwatoko-1.1.1/niwatoko/temp.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 00:21:15.419356 niwatoko-1.1.1/niwatoko.egg-info/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    16804 2024-05-11 00:21:15.000000 niwatoko-1.1.1/niwatoko.egg-info/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1123 2024-05-11 00:21:15.000000 niwatoko-1.1.1/niwatoko.egg-info/SOURCES.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-05-11 00:21:15.000000 niwatoko-1.1.1/niwatoko.egg-info/dependency_links.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-05-11 00:21:15.000000 niwatoko-1.1.1/niwatoko.egg-info/entry_points.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       34 2024-05-11 00:21:15.000000 niwatoko-1.1.1/niwatoko.egg-info/requires.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       15 2024-05-11 00:21:15.000000 niwatoko-1.1.1/niwatoko.egg-info/top_level.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-05-11 00:21:15.428628 niwatoko-1.1.1/setup.cfg
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1697 2024-05-11 00:21:14.000000 niwatoko-1.1.1/setup.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 00:21:15.421787 niwatoko-1.1.1/tests/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     5897 2024-05-08 23:04:24.000000 niwatoko-1.1.1/tests/README.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2077 2024-05-07 02:46:41.000000 niwatoko-1.1.1/tests/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3754 2024-05-08 23:03:26.000000 niwatoko-1.1.1/tests/test_compiler.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     4529 2024-05-08 23:03:26.000000 niwatoko-1.1.1/tests/test_compiler.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3940 2024-05-08 23:04:26.000000 niwatoko-1.1.1/tests/test_compiler_v1_2.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 00:21:15.427762 niwatoko-1.1.1/tests/test_docs/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2747 2024-05-07 02:46:41.000000 niwatoko-1.1.1/tests/test_docs/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2030 2024-05-11 00:20:33.000000 niwatoko-1.1.1/tests/test_docs/output copy.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1987 2024-05-11 00:20:33.000000 niwatoko-1.1.1/tests/test_docs/output.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1733 2024-05-11 00:20:33.000000 niwatoko-1.1.1/tests/test_docs/output_.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2609 2024-05-07 05:48:44.000000 niwatoko-1.1.1/tests/test_docs/test_doc1.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2853 2024-05-07 05:48:44.000000 niwatoko-1.1.1/tests/test_docs/test_doc2.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2625 2024-05-07 05:48:44.000000 niwatoko-1.1.1/tests/test_docs/test_doc3.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1678 2024-05-07 22:46:07.000000 niwatoko-1.1.1/tests/test_docs/test_gen_github_issue.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1950 2024-05-07 22:46:07.000000 niwatoko-1.1.1/tests/test_docs/test_gen_grimoire.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1909 2024-05-07 22:46:07.000000 niwatoko-1.1.1/tests/test_docs/test_gen_grimoire2.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1850 2024-05-07 22:46:07.000000 niwatoko-1.1.1/tests/test_docs/test_gen_grimoire_en.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     5307 2024-05-07 05:52:23.000000 niwatoko-1.1.1/tests/test_docs/test_gen_zoltraak_pypi.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     6179 2024-05-11 00:20:33.000000 niwatoko-1.1.1/tests/test_docs/test_import_function.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      201 2024-05-11 00:20:33.000000 niwatoko-1.1.1/tests/test_docs/test_import_md.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      787 2024-05-11 00:20:33.000000 niwatoko-1.1.1/tests/test_docs/test_import_module_add.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      800 2024-05-11 00:20:33.000000 niwatoko-1.1.1/tests/test_docs/test_import_module_multiple.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2216 2024-05-07 02:46:41.000000 niwatoko-1.1.1/tests/test_interpreter.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2632 2024-05-07 02:46:41.000000 niwatoko-1.1.1/tests/test_parser.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 04:46:07.057951 niwatoko-1.1.2/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    11356 2024-05-07 05:52:57.000000 niwatoko-1.1.2/LICENSE
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    16858 2024-05-11 04:46:07.057688 niwatoko-1.1.2/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    15972 2024-05-11 04:01:06.000000 niwatoko-1.1.2/README.md
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 04:46:07.043385 niwatoko-1.1.2/niwatoko/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      166 2024-05-07 22:46:07.000000 niwatoko-1.1.2/niwatoko/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     6554 2024-05-11 04:38:48.000000 niwatoko-1.1.2/niwatoko/cli.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 04:46:07.041998 niwatoko-1.1.2/niwatoko/foundation_model/
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 04:46:07.042036 niwatoko-1.1.2/niwatoko/foundation_model/interpretation/
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 04:46:07.045180 niwatoko-1.1.2/niwatoko/foundation_model/interpretation/llm/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1346 2024-05-08 23:04:24.000000 niwatoko-1.1.2/niwatoko/foundation_model/interpretation/llm/claude.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1428 2024-05-08 23:04:24.000000 niwatoko-1.1.2/niwatoko/foundation_model/interpretation/llm/gpt.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 04:46:07.045420 niwatoko-1.1.2/niwatoko/grammar/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      685 2024-05-08 23:04:24.000000 niwatoko-1.1.2/niwatoko/grammar/system.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       33 2024-05-11 00:20:33.000000 niwatoko-1.1.2/niwatoko/temp.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 04:46:07.044584 niwatoko-1.1.2/niwatoko.egg-info/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    16858 2024-05-11 04:46:06.000000 niwatoko-1.1.2/niwatoko.egg-info/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1026 2024-05-11 04:46:07.000000 niwatoko-1.1.2/niwatoko.egg-info/SOURCES.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-05-11 04:46:06.000000 niwatoko-1.1.2/niwatoko.egg-info/dependency_links.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-05-11 04:46:06.000000 niwatoko-1.1.2/niwatoko.egg-info/entry_points.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       34 2024-05-11 04:46:06.000000 niwatoko-1.1.2/niwatoko.egg-info/requires.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       15 2024-05-11 04:46:06.000000 niwatoko-1.1.2/niwatoko.egg-info/top_level.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-05-11 04:46:07.058002 niwatoko-1.1.2/setup.cfg
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1697 2024-05-11 04:44:21.000000 niwatoko-1.1.2/setup.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 04:46:07.047369 niwatoko-1.1.2/tests/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     5897 2024-05-08 23:04:24.000000 niwatoko-1.1.2/tests/README.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2077 2024-05-07 02:46:41.000000 niwatoko-1.1.2/tests/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3754 2024-05-08 23:03:26.000000 niwatoko-1.1.2/tests/test_compiler.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     4529 2024-05-08 23:03:26.000000 niwatoko-1.1.2/tests/test_compiler.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3940 2024-05-08 23:04:26.000000 niwatoko-1.1.2/tests/test_compiler_v1_2.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 04:46:07.056956 niwatoko-1.1.2/tests/test_docs/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2747 2024-05-07 02:46:41.000000 niwatoko-1.1.2/tests/test_docs/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2030 2024-05-11 00:20:33.000000 niwatoko-1.1.2/tests/test_docs/output copy.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3118 2024-05-11 00:55:54.000000 niwatoko-1.1.2/tests/test_docs/output.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     4172 2024-05-11 00:56:05.000000 niwatoko-1.1.2/tests/test_docs/output.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1733 2024-05-11 00:20:33.000000 niwatoko-1.1.2/tests/test_docs/output_.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2609 2024-05-07 05:48:44.000000 niwatoko-1.1.2/tests/test_docs/test_doc1.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2853 2024-05-07 05:48:44.000000 niwatoko-1.1.2/tests/test_docs/test_doc2.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2625 2024-05-07 05:48:44.000000 niwatoko-1.1.2/tests/test_docs/test_doc3.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1678 2024-05-07 22:46:07.000000 niwatoko-1.1.2/tests/test_docs/test_gen_github_issue.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1950 2024-05-07 22:46:07.000000 niwatoko-1.1.2/tests/test_docs/test_gen_grimoire.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1909 2024-05-07 22:46:07.000000 niwatoko-1.1.2/tests/test_docs/test_gen_grimoire2.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1850 2024-05-07 22:46:07.000000 niwatoko-1.1.2/tests/test_docs/test_gen_grimoire_en.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     5307 2024-05-07 05:52:23.000000 niwatoko-1.1.2/tests/test_docs/test_gen_zoltraak_pypi.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     6179 2024-05-11 00:20:33.000000 niwatoko-1.1.2/tests/test_docs/test_import_function.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2216 2024-05-07 02:46:41.000000 niwatoko-1.1.2/tests/test_interpreter.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2632 2024-05-07 02:46:41.000000 niwatoko-1.1.2/tests/test_parser.py
```

### Comparing `niwatoko-1.1.1/LICENSE` & `niwatoko-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.1/PKG-INFO` & `niwatoko-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niwatoko
-Version: 1.1.1
+Version: 1.1.2
 Summary: 自然言語でプログラミングを行うことができる新しいプログラミング言語
 Home-page: https://niwatoko2.vercel.app/
 Author: dai-motoki
 Author-email: dai.motoki1123@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
@@ -279,15 +279,15 @@
 
 はい、VercelでSphinxのドキュメントを公開することができます。Vercelは静的サイトホスティングに特化したサービスで、Sphinxのような静的サイトジェネレーターとの相性が良いです。
 
 Vercelを使ってSphinxドキュメントを公開する手順は以下の通りです。
 
 1. Sphinxプロジェクトをビルドする
 ```bash
-$ make html
+sphinx-build -b html . _build/html && open _build/html/index.html
 ```
 
 2. Vercel用の設定ファイル `vercel.json` をプロジェクトルートに作成する
 ```json
 {
   "version": 2,
   "builds": [
```

### Comparing `niwatoko-1.1.1/README.md` & `niwatoko-1.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -257,15 +257,15 @@
 
 はい、VercelでSphinxのドキュメントを公開することができます。Vercelは静的サイトホスティングに特化したサービスで、Sphinxのような静的サイトジェネレーターとの相性が良いです。
 
 Vercelを使ってSphinxドキュメントを公開する手順は以下の通りです。
 
 1. Sphinxプロジェクトをビルドする
 ```bash
-$ make html
+sphinx-build -b html . _build/html && open _build/html/index.html
 ```
 
 2. Vercel用の設定ファイル `vercel.json` をプロジェクトルートに作成する
 ```json
 {
   "version": 2,
   "builds": [
```

### Comparing `niwatoko-1.1.1/niwatoko/foundation_model/interpretation/llm/claude.py` & `niwatoko-1.1.2/niwatoko/foundation_model/interpretation/llm/claude.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.1/niwatoko/foundation_model/interpretation/llm/gpt.py` & `niwatoko-1.1.2/niwatoko/foundation_model/interpretation/llm/gpt.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.1/niwatoko/grammar/system.md` & `niwatoko-1.1.2/niwatoko/grammar/system.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.1/niwatoko.egg-info/PKG-INFO` & `niwatoko-1.1.2/niwatoko.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niwatoko
-Version: 1.1.1
+Version: 1.1.2
 Summary: 自然言語でプログラミングを行うことができる新しいプログラミング言語
 Home-page: https://niwatoko2.vercel.app/
 Author: dai-motoki
 Author-email: dai.motoki1123@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
@@ -279,15 +279,15 @@
 
 はい、VercelでSphinxのドキュメントを公開することができます。Vercelは静的サイトホスティングに特化したサービスで、Sphinxのような静的サイトジェネレーターとの相性が良いです。
 
 Vercelを使ってSphinxドキュメントを公開する手順は以下の通りです。
 
 1. Sphinxプロジェクトをビルドする
 ```bash
-$ make html
+sphinx-build -b html . _build/html && open _build/html/index.html
 ```
 
 2. Vercel用の設定ファイル `vercel.json` をプロジェクトルートに作成する
 ```json
 {
   "version": 2,
   "builds": [
```

### Comparing `niwatoko-1.1.1/niwatoko.egg-info/SOURCES.txt` & `niwatoko-1.1.2/niwatoko.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -19,20 +19,18 @@
 tests/test_compiler.py
 tests/test_compiler_v1_2.py
 tests/test_interpreter.py
 tests/test_parser.py
 tests/test_docs/__init__.py
 tests/test_docs/output copy.md
 tests/test_docs/output.md
+tests/test_docs/output.py
 tests/test_docs/output_.md
 tests/test_docs/test_doc1.md
 tests/test_docs/test_doc2.md
 tests/test_docs/test_doc3.md
 tests/test_docs/test_gen_github_issue.md
 tests/test_docs/test_gen_grimoire.md
 tests/test_docs/test_gen_grimoire2.md
 tests/test_docs/test_gen_grimoire_en.md
 tests/test_docs/test_gen_zoltraak_pypi.md
-tests/test_docs/test_import_function.md
-tests/test_docs/test_import_md.md
-tests/test_docs/test_import_module_add.py
-tests/test_docs/test_import_module_multiple.py
+tests/test_docs/test_import_function.md
```

### Comparing `niwatoko-1.1.1/setup.py` & `niwatoko-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # niwatoko - 自然言語プログラミング言語のPythonパッケージのsetup.pyファイルです。
 # このファイルはパッケージのインストールや配布に必要な情報を含んでいます。
 
 from setuptools import setup, find_packages
 
 setup(
     name='niwatoko',
-    version='1.1.1',
+    version='1.1.2',
     description='自然言語でプログラミングを行うことができる新しいプログラミング言語',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='dai-motoki',
     author_email='dai.motoki1123@gmail.com',
     url='https://niwatoko2.vercel.app/',
     packages=find_packages(),
```

### Comparing `niwatoko-1.1.1/tests/README.md` & `niwatoko-1.1.2/tests/README.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.1/tests/__init__.py` & `niwatoko-1.1.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.1/tests/test_compiler.md` & `niwatoko-1.1.2/tests/test_compiler.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.1/tests/test_compiler.py` & `niwatoko-1.1.2/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.1/tests/test_compiler_v1_2.py` & `niwatoko-1.1.2/tests/test_compiler_v1_2.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.1/tests/test_docs/__init__.py` & `niwatoko-1.1.2/tests/test_docs/__init__.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.1/tests/test_docs/output copy.md` & `niwatoko-1.1.2/tests/test_docs/output copy.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.1/tests/test_docs/output.md` & `niwatoko-1.1.2/tests/test_docs/output_.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,41 @@
-日本語の要件定義書:
+## 要件定義書
 
-# 足し算モジュール
+### 機能概要
+この Python モジュールは、2つの数値を足し算する機能、数値のリストの合計を計算する機能、および可変長引数の数値を足し算する機能を提供します。
 
-## 概要
-2つの数値を足し算する関数、数値のリストの合計を計算する関数、複数の数値を足し算する関数を提供します。
+### 機能詳細
 
-## 機能
-1. `add(a, b)`: 2つの数値 `a` と `b` を足し算する関数
-   - 入力: 2つの数値 (`a`, `b`)
-   - 出力: `a` と `b` の和
-
-2. `add_list(numbers)`: 数値のリスト `numbers` の合計を計算する関数
-   - 入力: 数値のリスト (`numbers`)
-   - 出力: `numbers` の合計値
-
-3. `add_multiple(*args)`: 複数の数値を足し算する関数
-   - 入力: 任意の数の数値 (`*args`)
-   - 出力: 引数として渡された数値の合計
-
-## 使用方法
-1. `add(a, b)` 関数を使用して、2つの数値の和を計算できます。
-2. `add_list(numbers)` 関数を使用して、数値のリストの合計を計算できます。
-3. `add_multiple(*args)` 関数を使用して、任意の数の数値の合計を計算できます。
-
-# 掛け算モジュール
-
-## 概要
-2つの数値を掛け算する関数、数値のリストの積を計算する関数、複数の数値を掛け算する関数を提供します。
-
-## 機能
-1. `multiply(a, b)`: 2つの数値 `a` と `b` を掛け算する関数
-   - 入力: 2つの数値 (`a`, `b`)
-   - 出力: `a` と `b` の積
-
-2. `multiply_list(numbers)`: 数値のリスト `numbers` の積を計算する関数
-   - 入力: 数値のリスト (`numbers`)
-   - 出力: `numbers` の積
-
-3. `multiply_multiple(*args)`: 複数の数値を掛け算する関数
-   - 入力: 任意の数の数値 (`*args`)
-   - 出力: 引数として渡された数値の積
-
-## 使用方法
-1. `multiply(a, b)` 関数を使用して、2つの数値の積を計算できます。
-2. `multiply_list(numbers)` 関数を使用して、数値のリストの積を計算できます。
-3. `multiply_multiple(*args)` 関数を使用して、任意の数の数値の積を計算できます。
+#### 1. 2つの数値を足し算する関数 `add(a, b)`
+- 2つの数値 `a` と `b` を受け取り、それらの和を返す関数です。
+- `a` と `b` は整数型または浮動小数点型を受け付けます。
+- 戻り値は整数型または浮動小数点型になります。
+
+#### 2. 数値のリストの合計を計算する関数 `add_list(numbers)`
+- 数値のリスト `numbers` を受け取り、その合計値を返す関数です。
+- `numbers` は数値のリストを受け付けます。
+- 戻り値は整数型または浮動小数点型になります。
+
+#### 3. 可変長引数の数値を足し算する関数 `add_multiple(*args)`
+- 任意の数の数値引数 `*args` を受け取り、それらの合計値を返す関数です。
+- `*args` は可変長引数で、任意の数の数値を受け付けます。
+- 戻り値は整数型または浮動小数点型になります。
+
+### 使用方法
+この Python モジュールをインポートし、上記の3つの関数を呼び出すことで、数値の足し算を行うことができます。
+
+```python
+from test_import_module_add import add, add_list, add_multiple
+
+# 2つの数値を足し算
+result1 = add(3, 4)
+print(result1)  # 出力: 7
+
+# 数値のリストの合計を計算
+numbers = [1, 2, 3, 4, 5]
+result2 = add_list(numbers)
+print(result2)  # 出力: 15
+
+# 可変長引数の数値を足し算
+result3 = add_multiple(1, 2, 3, 4, 5)
+print(result3)  # 出力: 15
+```
```

### Comparing `niwatoko-1.1.1/tests/test_docs/test_doc1.md` & `niwatoko-1.1.2/tests/test_docs/test_doc1.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.1/tests/test_docs/test_doc2.md` & `niwatoko-1.1.2/tests/test_docs/test_doc2.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.1/tests/test_docs/test_doc3.md` & `niwatoko-1.1.2/tests/test_docs/test_doc3.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.1/tests/test_docs/test_gen_github_issue.md` & `niwatoko-1.1.2/tests/test_docs/test_gen_github_issue.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.1/tests/test_docs/test_gen_grimoire.md` & `niwatoko-1.1.2/tests/test_docs/test_gen_grimoire.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.1/tests/test_docs/test_gen_grimoire2.md` & `niwatoko-1.1.2/tests/test_docs/test_gen_grimoire2.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.1/tests/test_docs/test_gen_grimoire_en.md` & `niwatoko-1.1.2/tests/test_docs/test_gen_grimoire_en.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.1/tests/test_docs/test_gen_zoltraak_pypi.md` & `niwatoko-1.1.2/tests/test_docs/test_gen_zoltraak_pypi.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.1/tests/test_docs/test_import_function.md` & `niwatoko-1.1.2/tests/test_docs/test_import_function.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.1/tests/test_interpreter.py` & `niwatoko-1.1.2/tests/test_interpreter.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.1/tests/test_parser.py` & `niwatoko-1.1.2/tests/test_parser.py`

 * *Files identical despite different names*

