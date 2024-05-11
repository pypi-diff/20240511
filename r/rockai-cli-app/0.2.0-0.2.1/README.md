# Comparing `tmp/rockai_cli_app-0.2.0.tar.gz` & `tmp/rockai_cli_app-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rockai_cli_app-0.2.0.tar", max compression
+gzip compressed data, was "rockai_cli_app-0.2.1.tar", max compression
```

## Comparing `rockai_cli_app-0.2.0.tar` & `rockai_cli_app-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       72 2024-03-05 09:01:49.763544 rockai_cli_app-0.2.0/README.md
--rw-r--r--   0        0        0      619 2024-04-07 03:13:26.916492 rockai_cli_app-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-07 03:29:24.441443 rockai_cli_app-0.2.0/rockai_cli_app/__init__.py
--rw-r--r--   0        0        0     2346 2024-04-03 07:24:35.496357 rockai_cli_app-0.2.0/rockai_cli_app/data_class.py
--rw-r--r--   0        0        0        0 2024-03-01 08:25:13.083771 rockai_cli_app-0.2.0/rockai_cli_app/docker/__init__.py
--rw-r--r--   0        0        0    11652 2024-04-02 08:30:02.204871 rockai_cli_app-0.2.0/rockai_cli_app/docker/docker_util.py
--rw-r--r--   0        0        0     2819 2024-03-01 08:15:55.566855 rockai_cli_app-0.2.0/rockai_cli_app/docker/tf_compat.json
--rw-r--r--   0        0        0      604 2024-03-26 06:45:43.007156 rockai_cli_app-0.2.0/rockai_cli_app/docker/torch_compat.json
--rw-r--r--   0        0        0     1406 2024-03-08 06:28:07.738273 rockai_cli_app-0.2.0/rockai_cli_app/main.py
--rw-r--r--   0        0        0        0 2024-02-28 08:04:20.239254 rockai_cli_app-0.2.0/rockai_cli_app/parser/__init__.py
--rw-r--r--   0        0        0      799 2024-02-28 09:29:39.709568 rockai_cli_app-0.2.0/rockai_cli_app/parser/config_util.py
--rw-r--r--   0        0        0      290 2024-02-07 03:35:01.202042 rockai_cli_app-0.2.0/rockai_cli_app/predictor.py
--rw-r--r--   0        0        0        0 2024-02-07 03:35:44.528854 rockai_cli_app-0.2.0/rockai_cli_app/server/__init__.py
--rw-r--r--   0        0        0     2569 2024-04-03 07:46:25.050529 rockai_cli_app-0.2.0/rockai_cli_app/server/http.py
--rw-r--r--   0        0        0       77 2024-02-07 06:52:07.739336 rockai_cli_app-0.2.0/rockai_cli_app/server/runner.py
--rw-r--r--   0        0        0        0 2024-02-20 09:20:10.188788 rockai_cli_app-0.2.0/rockai_cli_app/server/test/__init__.py
--rw-r--r--   0        0        0      783 2024-02-28 07:05:00.986936 rockai_cli_app-0.2.0/rockai_cli_app/server/test/predict.py
--rw-r--r--   0        0        0      149 2024-02-20 06:38:03.569237 rockai_cli_app-0.2.0/rockai_cli_app/server/test/test_config.yaml
--rw-r--r--   0        0        0     8582 2024-02-23 06:25:29.351387 rockai_cli_app-0.2.0/rockai_cli_app/server/types.py
--rw-r--r--   0        0        0     8639 2024-04-07 03:13:17.847123 rockai_cli_app-0.2.0/rockai_cli_app/server/utils.py
--rw-r--r--   0        0        0        0 2024-02-07 05:25:34.434644 rockai_cli_app-0.2.0/rockai_cli_app/server/worker.py
--rw-r--r--   0        0        0      703 2024-02-22 08:32:41.013574 rockai_cli_app-0.2.0/rockai_cli_app/test.py
--rw-r--r--   0        0        0      769 1970-01-01 00:00:00.000000 rockai_cli_app-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      128 2024-05-06 14:26:16.307703 rockai_cli_app-0.2.1/README.md
+-rw-r--r--   0        0        0      601 2024-05-11 15:41:21.522167 rockai_cli_app-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-06 14:26:16.309243 rockai_cli_app-0.2.1/rockai_cli_app/__init__.py
+-rw-r--r--   0        0        0     2346 2024-05-06 14:26:16.309393 rockai_cli_app-0.2.1/rockai_cli_app/data_class.py
+-rw-r--r--   0        0        0        0 2024-05-06 14:26:16.309507 rockai_cli_app-0.2.1/rockai_cli_app/docker/__init__.py
+-rw-r--r--   0        0        0    12108 2024-05-11 14:08:05.184260 rockai_cli_app-0.2.1/rockai_cli_app/docker/docker_util.py
+-rw-r--r--   0        0        0     2819 2024-05-06 14:26:16.309849 rockai_cli_app-0.2.1/rockai_cli_app/docker/tf_compat.json
+-rw-r--r--   0        0        0      604 2024-05-06 14:26:16.309950 rockai_cli_app-0.2.1/rockai_cli_app/docker/torch_compat.json
+-rw-r--r--   0        0        0     1285 2024-05-06 14:26:16.310077 rockai_cli_app-0.2.1/rockai_cli_app/main.py
+-rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310199 rockai_cli_app-0.2.1/rockai_cli_app/parser/__init__.py
+-rw-r--r--   0        0        0      799 2024-05-06 14:26:16.310349 rockai_cli_app-0.2.1/rockai_cli_app/parser/config_util.py
+-rw-r--r--   0        0        0      290 2024-05-06 14:26:16.310457 rockai_cli_app-0.2.1/rockai_cli_app/predictor.py
+-rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310565 rockai_cli_app-0.2.1/rockai_cli_app/server/__init__.py
+-rw-r--r--   0        0        0     2569 2024-05-06 14:26:16.310696 rockai_cli_app-0.2.1/rockai_cli_app/server/http.py
+-rw-r--r--   0        0        0       77 2024-05-06 14:26:16.310797 rockai_cli_app-0.2.1/rockai_cli_app/server/runner.py
+-rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310900 rockai_cli_app-0.2.1/rockai_cli_app/server/test/__init__.py
+-rw-r--r--   0        0        0      783 2024-05-06 14:26:16.311028 rockai_cli_app-0.2.1/rockai_cli_app/server/test/predict.py
+-rw-r--r--   0        0        0      149 2024-05-06 14:26:16.311129 rockai_cli_app-0.2.1/rockai_cli_app/server/test/test_config.yaml
+-rw-r--r--   0        0        0     8582 2024-05-06 14:26:16.311319 rockai_cli_app-0.2.1/rockai_cli_app/server/types.py
+-rw-r--r--   0        0        0     8718 2024-05-06 14:26:16.311504 rockai_cli_app-0.2.1/rockai_cli_app/server/utils.py
+-rw-r--r--   0        0        0        0 2024-05-06 14:26:16.311559 rockai_cli_app-0.2.1/rockai_cli_app/server/worker.py
+-rw-r--r--   0        0        0      703 2024-05-06 14:26:16.311710 rockai_cli_app-0.2.1/rockai_cli_app/test.py
+-rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 rockai_cli_app-0.2.1/PKG-INFO
```

### Comparing `rockai_cli_app-0.2.0/pyproject.toml` & `rockai_cli_app-0.2.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [tool.poetry]
 name = "rockai-cli-app"
-version = "0.2.0"
+version = "0.2.1"
 description = "For inference and training"
 authors = ["Rocky <some_developer@example.com>"]
 readme = "README.md"
 include = ["./rockai_cli_app/docker/tf_compat.json","./rockai_cli_app/docker/torch_compat.json"]
 
 [tool.poetry.scripts]
 rock = "rockai_cli_app.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 typer = {extras = ["all"], version = "^0.9.0"}
 fastapi = "^0.109.2"
 uvicorn = {extras = ["standard"], version = "^0.27.0.post1"}
 requests = "^2.31.0"
-docker = "^7.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `rockai_cli_app-0.2.0/rockai_cli_app/data_class.py` & `rockai_cli_app-0.2.1/rockai_cli_app/data_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             cls.__name__, __base__=cls, input=(input_type, None)
         )
         return dynamic_model
 
 
 class InferenceResponse(InferenceBase):
     output: t.Any
-
+    
     id: t.Optional[str] = None
     version: t.Optional[str] = None
 
     created_at: t.Optional[datetime] = None
     started_at: t.Optional[datetime] = None
     completed_at: t.Optional[datetime] = None
 
@@ -39,15 +39,15 @@
 
     @classmethod
     def get_pydantic_model(
         cls, input_type: t.Type[t.Any], output_type: t.Type[t.Any]
     ) -> t.Any:
         return create_model(
             cls.__name__,
-            __base__=InferenceResponse,
+            __base__=InferenceBase,
             input=(t.Optional[input_type], None),
             output=(output_type, None),
         )
 
 
 class BaseInput(BaseModel):
```

### Comparing `rockai_cli_app-0.2.0/rockai_cli_app/docker/docker_util.py` & `rockai_cli_app-0.2.1/rockai_cli_app/docker/docker_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,23 +21,30 @@
                 if lib_to_be_deleted not in line:
                     file.write(line)
 
         print("Successfully removed {} from {}".format(lib_to_be_deleted,file_name))
     except FileNotFoundError:
         print("{} not found".format(file_name))
 
-def build_docker_image(image_tag, config_map, tag,platform='linux/amd64'):
-    
+def build_docker_image(image_tag, config_map, tag,platform='linux/amd64',port=5000):
+    #sed -i s@/archive.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list
+    #sed -i s@/security.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list
+    #apt-get clean
+    #apt-get update
+
     docker_list = []
     docker_list.append(add_base(image_tag))
     docker_list.append(add_env("DEBIAN_FRONTEND=noninteractive"))
     docker_list.append(add_work_dir('/src'))
-    docker_list.append(copy_files('rock.yaml','$WORKDIR'))
-    docker_list.append(copy_files("{}".format(config_map['build']['python_requirements']), "$WORKDIR"))
-    docker_list.append(copy_files("{}".format(config_map['predict'].split(':')[0]), "$WORKDIR"))
+    docker_list.append(copy_files('rock.yaml','/src'))
+    docker_list.append(copy_files("{}".format(config_map['build']['python_requirements']), "/src"))
+    docker_list.append(copy_files("{}".format(config_map['predict'].split(':')[0]), "/src"))
+    docker_list.append(add_run("sed -i s@/archive.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list"))
+    docker_list.append(add_run("sed -i s@/security.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list"))
+    docker_list.append(add_run("apt-get clean"))
     docker_list.append(add_run("apt update && apt-get update"))
     docker_list.append(add_env('PATH="/root/.pyenv/shims:/root/.pyenv/bin:$PATH"'))
     docker_list.append(
         add_run(
             """--mount=type=cache,target=/var/cache/apt apt-get update -qq && apt-get install -qqy --no-install-recommends \
 	make \
 	build-essential \
@@ -70,24 +77,24 @@
 	pip install "wheel<1"
 """.format(
                 config_map["build"]["python_version"],
                 config_map["build"]["python_version"],
             )
         )
     )
-    docker_list.append(add_expose(5000))
+    docker_list.append(add_expose(port))
     if config_map['build']['python_requirements']:
         remove_some_libs(config_map['build']['python_requirements'],'tensorflow-metal')
         remove_some_libs(config_map['build']['python_requirements'],'tensorflow-macos')
-        docker_list.append(add_run("pip install -r {}".format(config_map['build']['python_requirements'])))
+        docker_list.append(add_run("pip install -r {} {}".format(config_map['build']['python_requirements'],"-i https://mirrors.aliyun.com/pypi/simple/")))
 
     docker_list.append(add_cmd("rock start"))
     save_docker_file(docker_list)
     subprocess.run(["docker", "build", "--platform", platform,"-t", tag, "."])
-    subprocess.run(["docker", "run", "--rm", tag])
+    # subprocess.run(["docker", "run", "--rm", tag])
         
 
 
 def tf_compat_matrix():
     json_data = [{"tf_version": "tensorflow-2.16.1", "python": "3.9-3.12", "cuDNN": "8.9", "CUDA": "12.3"},{"tf_version": "tensorflow-2.15.0", "python": "3.9-3.11", "cuDNN": "8.9", "CUDA": "12.2"}, {"tf_version": "tensorflow-2.14.0", "python": "3.9-3.11", "cuDNN": "8.7", "CUDA": "11.8"}, {"tf_version": "tensorflow-2.13.0", "python": "3.8-3.11", "cuDNN": "8.6", "CUDA": "11.8"}, {"tf_version": "tensorflow-2.12.0", "python": "3.8-3.11", "cuDNN": "8.6", "CUDA": "11.8"}, {"tf_version": "tensorflow-2.11.0", "python": "3.7-3.10", "cuDNN": "8.1", "CUDA": "11.2"}, {"tf_version": "tensorflow-2.10.0", "python": "3.7-3.10", "cuDNN": "8.1", "CUDA": "11.2"}, {"tf_version": "tensorflow-2.9.0", "python": "3.7-3.10", "cuDNN": "8.1", "CUDA": "11.2"}, {"tf_version": "tensorflow-2.8.0", "python": "3.7-3.10", "cuDNN": "8.1", "CUDA": "11.2"}, {"tf_version": "tensorflow-2.7.0", "python": "3.7-3.9", "cuDNN": "8.1", "CUDA": "11.2"}, {"tf_version": "tensorflow-2.6.0", "python": "3.6-3.9", "cuDNN": "8.1", "CUDA": "11.2"}, {"tf_version": "tensorflow-2.5.0", "python": "3.6-3.9", "cuDNN": "8.1", "CUDA": "11.2"}, {"tf_version": "tensorflow-2.4.0", "python": "3.6-3.8", "cuDNN": "8.0", "CUDA": "11.0"}, {"tf_version": "tensorflow-2.3.0", "python": "3.5-3.8", "cuDNN": "7.6", "CUDA": "10.1"}, {"tf_version": "tensorflow-2.2.0", "python": "3.5-3.8", "cuDNN": "7.6", "CUDA": "10.1"}, {"tf_version": "tensorflow-2.1.0", "python": "2.7,", "cuDNN": "7.6", "CUDA": "10.1"}, {"tf_version": "tensorflow-2.0.0", "python": "2.7,", "cuDNN": "7.4", "CUDA": "10.0"}, {"tf_version": "tensorflow_gpu-1.15.0", "python": "2.7,", "cuDNN": "7.4", "CUDA": "10.0"}, {"tf_version": "tensorflow_gpu-1.14.0", "python": "2.7,", "cuDNN": "7.4", "CUDA": "10.0"}, {"tf_version": "tensorflow_gpu-1.13.1", "python": "2.7,", "cuDNN": "7.4", "CUDA": "10.0"}, {"tf_version": "tensorflow_gpu-1.12.0", "python": "2.7,", "cuDNN": "7", "CUDA": "9"}, {"tf_version": "tensorflow_gpu-1.11.0", "python": "2.7,", "cuDNN": "7", "CUDA": "9"}, {"tf_version": "tensorflow_gpu-1.10.0", "python": "2.7,", "cuDNN": "7", "CUDA": "9"}, {"tf_version": "tensorflow_gpu-1.9.0", "python": "2.7,", "cuDNN": "7", "CUDA": "9"}, {"tf_version": "tensorflow_gpu-1.8.0", "python": "2.7,", "cuDNN": "7", "CUDA": "9"}, {"tf_version": "tensorflow_gpu-1.7.0", "python": "2.7,", "cuDNN": "7", "CUDA": "9"}, {"tf_version": "tensorflow_gpu-1.6.0", "python": "2.7,", "cuDNN": "7", "CUDA": "9"}, {"tf_version": "tensorflow_gpu-1.5.0", "python": "2.7,", "cuDNN": "7", "CUDA": "9"}, {"tf_version": "tensorflow_gpu-1.4.0", "python": "2.7,", "cuDNN": "6", "CUDA": "8"}, {"tf_version": "tensorflow_gpu-1.3.0", "python": "2.7,", "cuDNN": "6", "CUDA": "8"}, {"tf_version": "tensorflow_gpu-1.2.0", "python": "2.7,", "cuDNN": "5.1", "CUDA": "8"}, {"tf_version": "tensorflow_gpu-1.1.0", "python": "2.7,", "cuDNN": "5.1", "CUDA": "8"}, {"tf_version": "tensorflow_gpu-1.0.0", "python": "2.7,", "cuDNN": "5.1", "CUDA": "8"}]
     return json_data
 
@@ -221,31 +228,28 @@
             line_spl = line.split("==")
             if "tensorflow" == line_spl[0]:
                 return "tensorflow", line_spl[1]
             if "torch" == line_spl[0]:
                 return "torch", line_spl[1]
 
 
-def build_final_image(config_map):
+def build_final_image(config_map,port=5000):
     if config_map["build"]["gpu"] is True:
-        # build GPU image
-        print(Path.cwd() / config_map["build"]["python_requirements"])
+        # Build GPU image
         framework, version = process_requirements(
             Path.cwd() / config_map["build"]["python_requirements"]
         )
         if framework == "tensorflow":
             image_tag = find_correct_image_by_tf_gpu_only(version)
-            print(image_tag)
-            build_docker_image(image_tag, config_map, config_map["image"])
+            build_docker_image(image_tag, config_map, config_map["image"],port=port)
         elif framework == "torch":
-            print("building torch image")
             image_tag = find_correct_image_by_torch_gpu_only(version)
-            build_docker_image(image_tag, config_map, config_map["image"])
+            build_docker_image(image_tag, config_map, config_map["image"],port=port)
         else:
-            raise Exception("No tensorflow or pytorch found in requirements file")
+            raise Exception("No TensorFlow or PyTorch found in {} file".format(Path.cwd() / config_map['build']['python_requirements']))
     else:
         # build CPU image
         py_version = config_map["build"]["python_version"]
         # TODO
 
 
 def add_base(base):
```

### Comparing `rockai_cli_app-0.2.0/rockai_cli_app/docker/tf_compat.json` & `rockai_cli_app-0.2.1/rockai_cli_app/docker/tf_compat.json`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.0/rockai_cli_app/docker/torch_compat.json` & `rockai_cli_app-0.2.1/rockai_cli_app/docker/torch_compat.json`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.0/rockai_cli_app/main.py` & `rockai_cli_app-0.2.1/rockai_cli_app/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import typer
 from rockai_cli_app.server.http import start_server
 from pathlib import Path
 from rockai_cli_app.parser.config_util import parse_config_file
 from typing_extensions import Annotated
-from typing import Optional
-import docker
 from rockai_cli_app.docker.docker_util import build_final_image
-from rich.progress import Progress, SpinnerColumn, TextColumn
-import subprocess
+
 
 app = typer.Typer()
 
 APP_NAME = "rockai-cli-app"
 
 
 @app.callback()
```

### Comparing `rockai_cli_app-0.2.0/rockai_cli_app/parser/config_util.py` & `rockai_cli_app-0.2.1/rockai_cli_app/parser/config_util.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.0/rockai_cli_app/server/http.py` & `rockai_cli_app-0.2.1/rockai_cli_app/server/http.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.0/rockai_cli_app/server/test/predict.py` & `rockai_cli_app-0.2.1/rockai_cli_app/server/test/predict.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.0/rockai_cli_app/server/types.py` & `rockai_cli_app-0.2.1/rockai_cli_app/server/types.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.0/rockai_cli_app/server/utils.py` & `rockai_cli_app-0.2.1/rockai_cli_app/server/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from rockai_cli_app.predictor import BasePredictor
 import importlib.util
 import os.path
 from rockai_cli_app.data_class import BaseInput
 from typing import Type, Any, Union, List, Dict
 import inspect
-from pydantic import create_model, BaseModel, Field
+from pydantic import create_model, BaseModel, Field,ConfigDict
 import enum
 from typing import get_args, get_origin, Iterator
 from pydantic.fields import FieldInfo
 from rockai_cli_app.server.types import File as CogFile, Path as CogPath, Input, URLPath
 import types
 from typing_extensions import Annotated
 
@@ -234,11 +234,12 @@
 
         class Output(OutputType):  # type: ignore
             pass
 
         return Output
     else:
         class Output(OutputType):
+            model_config = ConfigDict(arbitrary_types_allowed=True)
             # __root__: OutputType  # type: ignore
             pass
 
         return Output
```

### Comparing `rockai_cli_app-0.2.0/rockai_cli_app/test.py` & `rockai_cli_app-0.2.1/rockai_cli_app/test.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.0/PKG-INFO` & `rockai_cli_app-0.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: rockai-cli-app
-Version: 0.2.0
+Version: 0.2.1
 Summary: For inference and training
 Author: Rocky
 Author-email: some_developer@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: docker (>=7.0.0,<8.0.0)
 Requires-Dist: fastapi (>=0.109.2,<0.110.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Requires-Dist: uvicorn[standard] (>=0.27.0.post1,<0.28.0)
 Description-Content-Type: text/markdown
 
+# setup
+python 3.11.5, use this version when developing
 ```
 # clean docker space
 docker system prune --all --force --volumes
 ```
```

