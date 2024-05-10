# Comparing `tmp/pulumi_docker-4.7.0a1705607229.tar.gz` & `tmp/pulumi_docker-4.7.0a1705628423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_docker-4.7.0a1705607229.tar", last modified: Thu Jan 18 19:51:24 2024, max compression
+gzip compressed data, was "pulumi_docker-4.7.0a1705628423.tar", last modified: Fri Jan 19 01:47:51 2024, max compression
```

## Comparing `pulumi_docker-4.7.0a1705607229.tar` & `pulumi_docker-4.7.0a1705628423.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 19:51:24.774437 pulumi_docker-4.7.0a1705607229/
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-01-18 19:51:24.774437 pulumi_docker-4.7.0a1705607229/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-01-18 19:51:11.000000 pulumi_docker-4.7.0a1705607229/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 19:51:24.770437 pulumi_docker-4.7.0a1705607229/pulumi_docker/
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-01-18 19:51:11.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-01-18 19:51:11.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker/_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)   176300 2024-01-18 19:51:11.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-01-18 19:51:11.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 19:51:24.770437 pulumi_docker-4.7.0a1705607229/pulumi_docker/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-01-18 19:51:11.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-01-18 19:51:11.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-01-18 19:51:11.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-01-18 19:51:11.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)   155348 2024-01-18 19:51:11.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     9548 2024-01-18 19:51:11.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker/get_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-01-18 19:51:11.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker/get_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-01-18 19:51:11.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker/get_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-01-18 19:51:11.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker/get_registry_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-01-18 19:51:11.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker/get_remote_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    20473 2024-01-18 19:51:11.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    32844 2024-01-18 19:51:11.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker/network.py
--rw-r--r--   0 runner    (1001) docker     (127)   146055 2024-01-18 19:51:11.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    24751 2024-01-18 19:51:11.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-01-18 19:51:11.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-18 19:51:11.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 19:51:11.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    16148 2024-01-18 19:51:11.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker/registry_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    25845 2024-01-18 19:51:11.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker/remote_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     9540 2024-01-18 19:51:11.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    26126 2024-01-18 19:51:11.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-01-18 19:51:11.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker/service_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8994 2024-01-18 19:51:11.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)    14437 2024-01-18 19:51:11.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 19:51:24.770437 pulumi_docker-4.7.0a1705607229/pulumi_docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-01-18 19:51:24.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-01-18 19:51:24.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 19:51:24.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-18 19:51:24.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-18 19:51:24.000000 pulumi_docker-4.7.0a1705607229/pulumi_docker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-01-18 19:51:11.000000 pulumi_docker-4.7.0a1705607229/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 19:51:24.774437 pulumi_docker-4.7.0a1705607229/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 01:47:51.132898 pulumi_docker-4.7.0a1705628423/
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-01-19 01:47:51.132898 pulumi_docker-4.7.0a1705628423/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-01-19 01:47:39.000000 pulumi_docker-4.7.0a1705628423/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 01:47:51.128898 pulumi_docker-4.7.0a1705628423/pulumi_docker/
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-01-19 01:47:39.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-01-19 01:47:39.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)   176300 2024-01-19 01:47:39.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-01-19 01:47:39.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 01:47:51.132898 pulumi_docker-4.7.0a1705628423/pulumi_docker/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-01-19 01:47:39.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-01-19 01:47:39.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-01-19 01:47:39.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-01-19 01:47:39.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)   155348 2024-01-19 01:47:39.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9548 2024-01-19 01:47:39.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker/get_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-01-19 01:47:39.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker/get_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-01-19 01:47:39.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker/get_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-01-19 01:47:39.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker/get_registry_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-01-19 01:47:39.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker/get_remote_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20473 2024-01-19 01:47:39.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32844 2024-01-19 01:47:39.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)   146055 2024-01-19 01:47:39.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24751 2024-01-19 01:47:39.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-01-19 01:47:39.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-19 01:47:39.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 01:47:39.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16148 2024-01-19 01:47:39.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker/registry_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25845 2024-01-19 01:47:39.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker/remote_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9540 2024-01-19 01:47:39.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26126 2024-01-19 01:47:39.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-01-19 01:47:39.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker/service_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8994 2024-01-19 01:47:39.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14437 2024-01-19 01:47:39.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 01:47:51.132898 pulumi_docker-4.7.0a1705628423/pulumi_docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-01-19 01:47:51.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-01-19 01:47:51.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 01:47:51.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-19 01:47:51.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-19 01:47:51.000000 pulumi_docker-4.7.0a1705628423/pulumi_docker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-01-19 01:47:39.000000 pulumi_docker-4.7.0a1705628423/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-19 01:47:51.132898 pulumi_docker-4.7.0a1705628423/setup.cfg
```

### Comparing `pulumi_docker-4.7.0a1705607229/PKG-INFO` & `pulumi_docker-4.7.0a1705628423/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_docker
-Version: 4.7.0a1705607229
+Version: 4.7.0a1705628423
 Summary: A Pulumi package for interacting with Docker in Pulumi programs
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-docker
 Keywords: pulumi,docker
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_docker-4.7.0a1705607229/README.md` & `pulumi_docker-4.7.0a1705628423/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.7.0a1705607229/pulumi_docker/__init__.py` & `pulumi_docker-4.7.0a1705628423/pulumi_docker/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.7.0a1705607229/pulumi_docker/_enums.py` & `pulumi_docker-4.7.0a1705628423/pulumi_docker/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.7.0a1705607229/pulumi_docker/_inputs.py` & `pulumi_docker-4.7.0a1705628423/pulumi_docker/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.7.0a1705607229/pulumi_docker/_utilities.py` & `pulumi_docker-4.7.0a1705628423/pulumi_docker/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.7.0a1705607229/pulumi_docker/config/__init__.pyi` & `pulumi_docker-4.7.0a1705628423/pulumi_docker/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.7.0a1705607229/pulumi_docker/config/outputs.py` & `pulumi_docker-4.7.0a1705628423/pulumi_docker/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.7.0a1705607229/pulumi_docker/config/vars.py` & `pulumi_docker-4.7.0a1705628423/pulumi_docker/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.7.0a1705607229/pulumi_docker/container.py` & `pulumi_docker-4.7.0a1705628423/pulumi_docker/container.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.7.0a1705607229/pulumi_docker/get_logs.py` & `pulumi_docker-4.7.0a1705628423/pulumi_docker/get_logs.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.7.0a1705607229/pulumi_docker/get_network.py` & `pulumi_docker-4.7.0a1705628423/pulumi_docker/get_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.7.0a1705607229/pulumi_docker/get_plugin.py` & `pulumi_docker-4.7.0a1705628423/pulumi_docker/get_plugin.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.7.0a1705607229/pulumi_docker/get_registry_image.py` & `pulumi_docker-4.7.0a1705628423/pulumi_docker/get_registry_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.7.0a1705607229/pulumi_docker/get_remote_image.py` & `pulumi_docker-4.7.0a1705628423/pulumi_docker/get_remote_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.7.0a1705607229/pulumi_docker/image.py` & `pulumi_docker-4.7.0a1705628423/pulumi_docker/image.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.7.0a1705607229/pulumi_docker/network.py` & `pulumi_docker-4.7.0a1705628423/pulumi_docker/network.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.7.0a1705607229/pulumi_docker/outputs.py` & `pulumi_docker-4.7.0a1705628423/pulumi_docker/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.7.0a1705607229/pulumi_docker/plugin.py` & `pulumi_docker-4.7.0a1705628423/pulumi_docker/plugin.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.7.0a1705607229/pulumi_docker/provider.py` & `pulumi_docker-4.7.0a1705628423/pulumi_docker/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.7.0a1705607229/pulumi_docker/registry_image.py` & `pulumi_docker-4.7.0a1705628423/pulumi_docker/registry_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.7.0a1705607229/pulumi_docker/remote_image.py` & `pulumi_docker-4.7.0a1705628423/pulumi_docker/remote_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.7.0a1705607229/pulumi_docker/secret.py` & `pulumi_docker-4.7.0a1705628423/pulumi_docker/secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.7.0a1705607229/pulumi_docker/service.py` & `pulumi_docker-4.7.0a1705628423/pulumi_docker/service.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.7.0a1705607229/pulumi_docker/service_config.py` & `pulumi_docker-4.7.0a1705628423/pulumi_docker/service_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.7.0a1705607229/pulumi_docker/tag.py` & `pulumi_docker-4.7.0a1705628423/pulumi_docker/tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.7.0a1705607229/pulumi_docker/volume.py` & `pulumi_docker-4.7.0a1705628423/pulumi_docker/volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.7.0a1705607229/pulumi_docker.egg-info/PKG-INFO` & `pulumi_docker-4.7.0a1705628423/pulumi_docker.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_docker
-Version: 4.7.0a1705607229
+Version: 4.7.0a1705628423
 Summary: A Pulumi package for interacting with Docker in Pulumi programs
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-docker
 Keywords: pulumi,docker
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_docker-4.7.0a1705607229/pulumi_docker.egg-info/SOURCES.txt` & `pulumi_docker-4.7.0a1705628423/pulumi_docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.7.0a1705607229/pyproject.toml` & `pulumi_docker-4.7.0a1705628423/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_docker"
   description = "A Pulumi package for interacting with Docker in Pulumi programs"
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "docker"]
   readme = "README.md"
   requires-python = ">=3.7"
-  version = "4.7.0a1705607229"
+  version = "4.7.0a1705628423"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-docker"
 
 [build-system]
```

