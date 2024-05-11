# Comparing `tmp/pheval_ai_marrvel-0.1.0.tar.gz` & `tmp/pheval_ai_marrvel-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheval_ai_marrvel-0.1.0.tar", max compression
+gzip compressed data, was "pheval_ai_marrvel-0.1.1.tar", max compression
```

## Comparing `pheval_ai_marrvel-0.1.0.tar` & `pheval_ai_marrvel-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     2472 2024-05-10 18:43:41.111933 pheval_ai_marrvel-0.1.0/README.md
--rw-r--r--   0        0        0      812 2024-05-10 18:43:41.111933 pheval_ai_marrvel-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-10 18:43:41.111933 pheval_ai_marrvel-0.1.0/src/pheval_ai_marrvel/__init__.py
--rw-r--r--   0        0        0        0 2024-05-10 18:43:41.111933 pheval_ai_marrvel-0.1.0/src/pheval_ai_marrvel/post_process/__init__.py
--rw-r--r--   0        0        0      263 2024-05-10 18:43:41.111933 pheval_ai_marrvel-0.1.0/src/pheval_ai_marrvel/post_process/post_process.py
--rw-r--r--   0        0        0     5688 2024-05-10 18:43:41.111933 pheval_ai_marrvel-0.1.0/src/pheval_ai_marrvel/post_process/post_process_results_format.py
--rw-r--r--   0        0        0        0 2024-05-10 18:43:41.111933 pheval_ai_marrvel-0.1.0/src/pheval_ai_marrvel/prepare/__init__.py
--rw-r--r--   0        0        0      190 2024-05-10 18:43:41.111933 pheval_ai_marrvel-0.1.0/src/pheval_ai_marrvel/prepare/prepare.py
--rw-r--r--   0        0        0     1111 2024-05-10 18:43:41.111933 pheval_ai_marrvel-0.1.0/src/pheval_ai_marrvel/prepare/prepare_input.py
--rw-r--r--   0        0        0        0 2024-05-10 18:43:41.111933 pheval_ai_marrvel-0.1.0/src/pheval_ai_marrvel/run/__init__.py
--rw-r--r--   0        0        0     2524 2024-05-10 18:43:41.111933 pheval_ai_marrvel-0.1.0/src/pheval_ai_marrvel/run/create_apptainer_commands.py
--rw-r--r--   0        0        0      494 2024-05-10 18:43:41.111933 pheval_ai_marrvel-0.1.0/src/pheval_ai_marrvel/run/run.py
--rw-r--r--   0        0        0     1354 2024-05-10 18:43:41.115933 pheval_ai_marrvel-0.1.0/src/pheval_ai_marrvel/runner.py
--rw-r--r--   0        0        0     2913 1970-01-01 00:00:00.000000 pheval_ai_marrvel-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2472 2024-05-10 19:25:37.694420 pheval_ai_marrvel-0.1.1/README.md
+-rw-r--r--   0        0        0      812 2024-05-10 19:25:37.698420 pheval_ai_marrvel-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-10 19:25:37.698420 pheval_ai_marrvel-0.1.1/src/pheval_ai_marrvel/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:25:37.698420 pheval_ai_marrvel-0.1.1/src/pheval_ai_marrvel/post_process/__init__.py
+-rw-r--r--   0        0        0      263 2024-05-10 19:25:37.698420 pheval_ai_marrvel-0.1.1/src/pheval_ai_marrvel/post_process/post_process.py
+-rw-r--r--   0        0        0     5688 2024-05-10 19:25:37.698420 pheval_ai_marrvel-0.1.1/src/pheval_ai_marrvel/post_process/post_process_results_format.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:25:37.698420 pheval_ai_marrvel-0.1.1/src/pheval_ai_marrvel/prepare/__init__.py
+-rw-r--r--   0        0        0      190 2024-05-10 19:25:37.698420 pheval_ai_marrvel-0.1.1/src/pheval_ai_marrvel/prepare/prepare.py
+-rw-r--r--   0        0        0     1177 2024-05-10 19:25:37.698420 pheval_ai_marrvel-0.1.1/src/pheval_ai_marrvel/prepare/prepare_input.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:25:37.698420 pheval_ai_marrvel-0.1.1/src/pheval_ai_marrvel/run/__init__.py
+-rw-r--r--   0        0        0     2524 2024-05-10 19:25:37.698420 pheval_ai_marrvel-0.1.1/src/pheval_ai_marrvel/run/create_apptainer_commands.py
+-rw-r--r--   0        0        0      494 2024-05-10 19:25:37.698420 pheval_ai_marrvel-0.1.1/src/pheval_ai_marrvel/run/run.py
+-rw-r--r--   0        0        0     1354 2024-05-10 19:25:37.698420 pheval_ai_marrvel-0.1.1/src/pheval_ai_marrvel/runner.py
+-rw-r--r--   0        0        0     2913 1970-01-01 00:00:00.000000 pheval_ai_marrvel-0.1.1/PKG-INFO
```

### Comparing `pheval_ai_marrvel-0.1.0/README.md` & `pheval_ai_marrvel-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pheval_ai_marrvel-0.1.0/pyproject.toml` & `pheval_ai_marrvel-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pheval-ai-marrvel"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Yasemin Bridges <y.bridges@qmul.ac.uk>"]
 readme = "README.md"
 packages = [{include = "pheval_ai_marrvel", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `pheval_ai_marrvel-0.1.0/src/pheval_ai_marrvel/post_process/post_process_results_format.py` & `pheval_ai_marrvel-0.1.1/src/pheval_ai_marrvel/post_process/post_process_results_format.py`

 * *Files identical despite different names*

### Comparing `pheval_ai_marrvel-0.1.0/src/pheval_ai_marrvel/prepare/prepare_input.py` & `pheval_ai_marrvel-0.1.1/src/pheval_ai_marrvel/prepare/prepare_input.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from phenopackets import Phenopacket
 from pheval.utils.file_utils import all_files
 from pheval.utils.phenopacket_utils import PhenopacketUtil, phenopacket_reader
 
 
 def obtain_observed_hpo_ids(phenopacket: Phenopacket) -> str:
     observed_phenotypes = PhenopacketUtil(phenopacket).observed_phenotypic_features()
-    observed_hpo_ids = "/n".join(observed_phenotypes)
+    observed_hpo_ids = [hpo_id.id for hpo_id in observed_phenotypes]
+    observed_hpo_ids = "/n".join(observed_hpo_ids)
     return observed_hpo_ids
 
 
 def write_txt_input(observed_hpo_ids: str, output_file_name: Path) -> None:
     with open(output_file_name, "w") as f:
         f.write(observed_hpo_ids)
     f.close()
```

### Comparing `pheval_ai_marrvel-0.1.0/src/pheval_ai_marrvel/run/create_apptainer_commands.py` & `pheval_ai_marrvel-0.1.1/src/pheval_ai_marrvel/run/create_apptainer_commands.py`

 * *Files identical despite different names*

### Comparing `pheval_ai_marrvel-0.1.0/src/pheval_ai_marrvel/runner.py` & `pheval_ai_marrvel-0.1.1/src/pheval_ai_marrvel/runner.py`

 * *Files identical despite different names*

### Comparing `pheval_ai_marrvel-0.1.0/PKG-INFO` & `pheval_ai_marrvel-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheval-ai-marrvel
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Yasemin Bridges
 Author-email: y.bridges@qmul.ac.uk
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

