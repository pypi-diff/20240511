# Comparing `tmp/pheval_ai_marrvel-0.1.1.tar.gz` & `tmp/pheval_ai_marrvel-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheval_ai_marrvel-0.1.1.tar", max compression
+gzip compressed data, was "pheval_ai_marrvel-0.1.2.tar", max compression
```

## Comparing `pheval_ai_marrvel-0.1.1.tar` & `pheval_ai_marrvel-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     2472 2024-05-10 19:25:37.694420 pheval_ai_marrvel-0.1.1/README.md
--rw-r--r--   0        0        0      812 2024-05-10 19:25:37.698420 pheval_ai_marrvel-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-10 19:25:37.698420 pheval_ai_marrvel-0.1.1/src/pheval_ai_marrvel/__init__.py
--rw-r--r--   0        0        0        0 2024-05-10 19:25:37.698420 pheval_ai_marrvel-0.1.1/src/pheval_ai_marrvel/post_process/__init__.py
--rw-r--r--   0        0        0      263 2024-05-10 19:25:37.698420 pheval_ai_marrvel-0.1.1/src/pheval_ai_marrvel/post_process/post_process.py
--rw-r--r--   0        0        0     5688 2024-05-10 19:25:37.698420 pheval_ai_marrvel-0.1.1/src/pheval_ai_marrvel/post_process/post_process_results_format.py
--rw-r--r--   0        0        0        0 2024-05-10 19:25:37.698420 pheval_ai_marrvel-0.1.1/src/pheval_ai_marrvel/prepare/__init__.py
--rw-r--r--   0        0        0      190 2024-05-10 19:25:37.698420 pheval_ai_marrvel-0.1.1/src/pheval_ai_marrvel/prepare/prepare.py
--rw-r--r--   0        0        0     1177 2024-05-10 19:25:37.698420 pheval_ai_marrvel-0.1.1/src/pheval_ai_marrvel/prepare/prepare_input.py
--rw-r--r--   0        0        0        0 2024-05-10 19:25:37.698420 pheval_ai_marrvel-0.1.1/src/pheval_ai_marrvel/run/__init__.py
--rw-r--r--   0        0        0     2524 2024-05-10 19:25:37.698420 pheval_ai_marrvel-0.1.1/src/pheval_ai_marrvel/run/create_apptainer_commands.py
--rw-r--r--   0        0        0      494 2024-05-10 19:25:37.698420 pheval_ai_marrvel-0.1.1/src/pheval_ai_marrvel/run/run.py
--rw-r--r--   0        0        0     1354 2024-05-10 19:25:37.698420 pheval_ai_marrvel-0.1.1/src/pheval_ai_marrvel/runner.py
--rw-r--r--   0        0        0     2913 1970-01-01 00:00:00.000000 pheval_ai_marrvel-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2472 2024-05-11 12:57:18.552125 pheval_ai_marrvel-0.1.2/README.md
+-rw-r--r--   0        0        0      875 2024-05-11 12:57:18.552125 pheval_ai_marrvel-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-11 12:57:18.552125 pheval_ai_marrvel-0.1.2/src/pheval_ai_marrvel/__init__.py
+-rw-r--r--   0        0        0      211 2024-05-11 12:57:18.552125 pheval_ai_marrvel-0.1.2/src/pheval_ai_marrvel/cli.py
+-rw-r--r--   0        0        0        0 2024-05-11 12:57:18.552125 pheval_ai_marrvel-0.1.2/src/pheval_ai_marrvel/post_process/__init__.py
+-rw-r--r--   0        0        0      546 2024-05-11 12:57:18.552125 pheval_ai_marrvel-0.1.2/src/pheval_ai_marrvel/post_process/post_process.py
+-rw-r--r--   0        0        0     5688 2024-05-11 12:57:18.552125 pheval_ai_marrvel-0.1.2/src/pheval_ai_marrvel/post_process/post_process_results_format.py
+-rw-r--r--   0        0        0        0 2024-05-11 12:57:18.552125 pheval_ai_marrvel-0.1.2/src/pheval_ai_marrvel/prepare/__init__.py
+-rw-r--r--   0        0        0      248 2024-05-11 12:57:18.552125 pheval_ai_marrvel-0.1.2/src/pheval_ai_marrvel/prepare/prepare.py
+-rw-r--r--   0        0        0     1182 2024-05-11 12:57:18.552125 pheval_ai_marrvel-0.1.2/src/pheval_ai_marrvel/prepare/prepare_input.py
+-rw-r--r--   0        0        0        0 2024-05-11 12:57:18.556125 pheval_ai_marrvel-0.1.2/src/pheval_ai_marrvel/run/__init__.py
+-rw-r--r--   0        0        0     2571 2024-05-11 12:57:18.556125 pheval_ai_marrvel-0.1.2/src/pheval_ai_marrvel/run/create_apptainer_commands.py
+-rw-r--r--   0        0        0      505 2024-05-11 12:57:18.556125 pheval_ai_marrvel-0.1.2/src/pheval_ai_marrvel/run/run.py
+-rw-r--r--   0        0        0     1354 2024-05-11 12:57:18.556125 pheval_ai_marrvel-0.1.2/src/pheval_ai_marrvel/runner.py
+-rw-r--r--   0        0        0     2913 1970-01-01 00:00:00.000000 pheval_ai_marrvel-0.1.2/PKG-INFO
```

### Comparing `pheval_ai_marrvel-0.1.1/README.md` & `pheval_ai_marrvel-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pheval_ai_marrvel-0.1.1/pyproject.toml` & `pheval_ai_marrvel-0.1.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 [tool.poetry]
 name = "pheval-ai-marrvel"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Yasemin Bridges <y.bridges@qmul.ac.uk>"]
 readme = "README.md"
 packages = [{include = "pheval_ai_marrvel", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pheval = "^0.3.2"
 
+[tool.poetry.scripts]
+pheval-ai = "pheval_ai_marrvel.cli:main"
 
 [tool.poetry.plugins."pheval.plugins"]
 template = "pheval_ai_marrvel.runner:AIMARRVELRunner"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pylint = "^2.15.6"
```

### Comparing `pheval_ai_marrvel-0.1.1/src/pheval_ai_marrvel/post_process/post_process_results_format.py` & `pheval_ai_marrvel-0.1.2/src/pheval_ai_marrvel/post_process/post_process_results_format.py`

 * *Files identical despite different names*

### Comparing `pheval_ai_marrvel-0.1.1/src/pheval_ai_marrvel/prepare/prepare_input.py` & `pheval_ai_marrvel-0.1.2/src/pheval_ai_marrvel/prepare/prepare_input.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from phenopackets import Phenopacket
 from pheval.utils.file_utils import all_files
 from pheval.utils.phenopacket_utils import PhenopacketUtil, phenopacket_reader
 
 
 def obtain_observed_hpo_ids(phenopacket: Phenopacket) -> str:
     observed_phenotypes = PhenopacketUtil(phenopacket).observed_phenotypic_features()
-    observed_hpo_ids = [hpo_id.id for hpo_id in observed_phenotypes]
-    observed_hpo_ids = "/n".join(observed_hpo_ids)
+    observed_hpo_ids = [hpo_id.type.id for hpo_id in observed_phenotypes]
+    observed_hpo_ids = "\n".join(observed_hpo_ids)
     return observed_hpo_ids
 
 
 def write_txt_input(observed_hpo_ids: str, output_file_name: Path) -> None:
     with open(output_file_name, "w") as f:
         f.write(observed_hpo_ids)
     f.close()
```

### Comparing `pheval_ai_marrvel-0.1.1/src/pheval_ai_marrvel/run/create_apptainer_commands.py` & `pheval_ai_marrvel-0.1.2/src/pheval_ai_marrvel/run/create_apptainer_commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,46 +20,46 @@
     phenopacket_path: Path, testdata_dir: Path, input_dir: Path, output_dir: Path
 ) -> ApptainerArguments:
     phenopacket = phenopacket_reader(phenopacket_path)
     vcf_file_data = PhenopacketUtil(phenopacket).vcf_file_data(
         phenopacket_path, testdata_dir.joinpath("vcf")
     )
     return ApptainerArguments(
-        sample_id=phenopacket.proband.id,
+        sample_id=phenopacket.subject.id,
         vcf_path=vcf_file_data.uri,
         vcf_assembly=vcf_file_data.file_attributes["genomeAssembly"],
         hpo_txt_file_path=testdata_dir.joinpath(f"hpo_ids/{phenopacket_path.stem}.txt"),
         data_dependencies=input_dir,
         output_directory=output_dir,
     )
 
 
 def create_apptainer_command(apptainer_arguments: ApptainerArguments) -> str:
     return (
-        f"apptainer run --mount type=bind,source={apptainer_arguments.vcf_path}, destination=/input/vcf.gz"
-        f"--mount type=bind,source={apptainer_arguments.hpo_txt_file_path},destination=/input/hpo.txt"
-        f"--mount type=bind,source={apptainer_arguments.data_dependencies},destination=/run/data_dependencies"
-        f"--mount type=bind,source={apptainer_arguments.output_directory}, destination=/out"
-        f"docker://chaozhongliu/aim-lite /run/proc.sh {apptainer_arguments.sample_id} "
-        f"{apptainer_arguments.vcf_assembly} 32"
+        f"apptainer run --mount type=bind,source={apptainer_arguments.vcf_path},destination=/input/vcf.gz"
+        f" --mount type=bind,source={apptainer_arguments.hpo_txt_file_path},destination=/input/hpo.txt"
+        f" --mount type=bind,source={apptainer_arguments.data_dependencies},destination=/run/data_dependencies"
+        f" --mount type=bind,source={apptainer_arguments.output_directory},destination=/out"
+        f" docker://chaozhongliu/aim-lite /run/proc.sh {apptainer_arguments.sample_id}"
+        f" {apptainer_arguments.vcf_assembly} 32"
     )
 
 
-def write_commands(commands: List[str], tool_input_commands_dir: Path) -> None:
+def write_commands(commands: List[str], tool_input_commands_dir: Path, testdata_dir: Path) -> None:
     joined_commands_str = "\n".join(commands)
     with open(
-        f"{tool_input_commands_dir.joinpath('apptainer_commands.txt')}", "w"
+        f"{tool_input_commands_dir.joinpath(f'{testdata_dir.name}_commands.txt')}", "w"
     ) as commands_file:
         commands_file.write(joined_commands_str)
     commands_file.close()
 
 
 def create_apptainer_commands(
     tool_input_commands_dir: Path, testdata_dir: Path, input_dir: Path, output_dir: Path
 ) -> None:
     all_commands = []
     for phenopacket_path in all_files(testdata_dir.joinpath("phenopackets")):
         apptainer_arguments = get_apptainer_arguments(
             phenopacket_path, testdata_dir, input_dir, output_dir
         )
         all_commands.append(create_apptainer_command(apptainer_arguments))
-    write_commands(all_commands, tool_input_commands_dir)
+    write_commands(all_commands, tool_input_commands_dir, testdata_dir)
```

### Comparing `pheval_ai_marrvel-0.1.1/src/pheval_ai_marrvel/runner.py` & `pheval_ai_marrvel-0.1.2/src/pheval_ai_marrvel/runner.py`

 * *Files identical despite different names*

### Comparing `pheval_ai_marrvel-0.1.1/PKG-INFO` & `pheval_ai_marrvel-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheval-ai-marrvel
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Yasemin Bridges
 Author-email: y.bridges@qmul.ac.uk
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

