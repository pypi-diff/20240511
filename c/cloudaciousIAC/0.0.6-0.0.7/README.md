# Comparing `tmp/cloudaciousiac-0.0.6.tar.gz` & `tmp/cloudaciousiac-0.0.7.tar.gz`

## Comparing `cloudaciousiac-0.0.6.tar` & `cloudaciousiac-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.6/.gitlab-ci.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.6/.pypirc
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.6/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.6/config.cfg
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.6/setup.py
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.6/src/cloudaciousIAC/ContainerImages.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.6/src/cloudaciousIAC/Naming.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.6/src/cloudaciousIAC/README.md
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.6/src/cloudaciousIAC/StackInfo.py
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.6/.gitignore
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.6/pyproject.toml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.7/.gitlab-ci.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.7/.pypirc
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.7/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.7/config.cfg
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.7/setup.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.7/src/cloudaciousIAC/Auth.py
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.7/src/cloudaciousIAC/ContainerImages.py
+-rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.7/src/cloudaciousIAC/LambdaFunction.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.7/src/cloudaciousIAC/Naming.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.7/src/cloudaciousIAC/README.md
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.7/src/cloudaciousIAC/StackInfo.py
+-rw-r--r--   0        0        0    13867 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.7/src/cloudaciousIAC/WebhookHandler.py
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.7/.gitignore
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.7/PKG-INFO
```

### Comparing `cloudaciousiac-0.0.6/.gitlab-ci.yml` & `cloudaciousiac-0.0.7/.gitlab-ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 
 pypi_prod:
   stage: deploy
   image: python:latest
   before_script:
     - echo $CI_COMMIT_TAG
     - cp .pypirc ~/
-    - cat ~/.pypirc
     - python -m pip install --upgrade build
     - python -m pip install --upgrade twine
   # environment:
   #   name: production
   #   url: https://prod.cloudacious.io
   rules:
     - if: $CI_COMMIT_TAG
```

### Comparing `cloudaciousiac-0.0.6/README.md` & `cloudaciousiac-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `cloudaciousiac-0.0.6/setup.py` & `cloudaciousiac-0.0.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import os
 from setuptools import setup, find_packages
 import pathlib
 
 
 # read the contents of your README file
 from pathlib import Path
+
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # here = pathlib.Path(__file__).parent.resolve()
 # long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
-    name="cloudaciousIAC,
-    version=os.getenv("CI_COMMIT_TAG"), 
+    name="cloudaciousIAC",
+    version=os.getenv("CI_COMMIT_TAG"),
     description="Cloudacious's object-oriented IaC tooling w/Pulumi. Call our classes all day long!",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    readme = "README.md",
+    readme="README.md",
     url="https://gitlab.com/money-marathon/cloudacious/cloudacious-iac.git",
     author="A. SurfingDoggo",
-    author_email="git@surfingdoggo.com",  
+    author_email="git@surfingdoggo.com",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
```

### Comparing `cloudaciousiac-0.0.6/src/cloudaciousIAC/ContainerImages.py` & `cloudaciousiac-0.0.7/src/cloudaciousIAC/ContainerImages.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,20 +49,20 @@
         self.container_registry_id: str = self.image_config["container_registry_id"]
         self.container_repo: str = self.image_config["container_repo"]
 
         self._resource_name: str = self.image_name.replace("-", "_")
 
     def create_image(
         self,
-        # auth_token: str,
+        auth_token: str,
     ):
         """
         Logs into ECR repo, builds image, and pushes it to ECR.
         """
-        # self._auth_token = auth_token
+        auth_token = auth_token
 
         self._container_build_image = docker.Image(
             resource_name=f"{self._resource_name}",
             build=docker.DockerBuildArgs(
                 args=self.build_args,
                 # cache_from=docker.CacheFromArgs(
                 #     images=[
@@ -75,15 +75,15 @@
                 dockerfile=f"{self.context}{self.dockerfile_name}",
                 platform="linux/amd64",
                 target=self.target,
             ),
             image_name=f"{self.container_registry_id}/{self.container_repo}:{self.image_name}",
             registry=docker.RegistryArgs(
                 username=self.container_registry_user,
-                password=pulumi.Output.secret(self._auth_token),
+                password=pulumi.Output.secret(auth_token),
                 server=self.container_registry_id,
             ),
         )
         self.base_image_name = self._container_build_image.base_image_name.apply(
             lambda base_image_name: base_image_name
         )
         pulumi.export("base_image_name", self.base_image_name)
```

### Comparing `cloudaciousiac-0.0.6/src/cloudaciousIAC/README.md` & `cloudaciousiac-0.0.7/src/cloudaciousIAC/README.md`

 * *Files identical despite different names*

### Comparing `cloudaciousiac-0.0.6/.gitignore` & `cloudaciousiac-0.0.7/.gitignore`

 * *Files identical despite different names*

