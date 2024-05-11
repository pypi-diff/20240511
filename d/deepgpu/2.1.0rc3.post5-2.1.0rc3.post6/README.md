# Comparing `tmp/deepgpu-2.1.0rc3.post5.tar.gz` & `tmp/deepgpu-2.1.0rc3.post6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepgpu-2.1.0rc3.post5.tar", last modified: Tue Apr 30 07:08:16 2024, max compression
+gzip compressed data, was "deepgpu-2.1.0rc3.post6.tar", last modified: Sat May 11 05:54:26 2024, max compression
```

## Comparing `deepgpu-2.1.0rc3.post5.tar` & `deepgpu-2.1.0rc3.post6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 du         (502) staff       (20)        0 2024-04-30 07:08:16.665018 deepgpu-2.1.0rc3.post5/
--rw-r--r--   0 du         (502) staff       (20)       30 2023-10-10 07:39:14.000000 deepgpu-2.1.0rc3.post5/MANIFEST.in
--rw-r--r--   0 du         (502) staff       (20)      621 2024-04-30 07:08:16.664652 deepgpu-2.1.0rc3.post5/PKG-INFO
--rw-r--r--   0 du         (502) staff       (20)      292 2024-04-26 09:23:15.000000 deepgpu-2.1.0rc3.post5/README.md
-drwxr-xr-x   0 du         (502) staff       (20)        0 2024-04-30 07:08:16.662932 deepgpu-2.1.0rc3.post5/deepgpu/
--rw-r--r--   0 du         (502) staff       (20)       17 2023-10-09 07:10:39.000000 deepgpu-2.1.0rc3.post5/deepgpu/__init__.py
-drwxr-xr-x   0 du         (502) staff       (20)        0 2024-04-30 07:08:16.664275 deepgpu-2.1.0rc3.post5/deepgpu.egg-info/
--rw-r--r--   0 du         (502) staff       (20)      621 2024-04-30 07:08:16.000000 deepgpu-2.1.0rc3.post5/deepgpu.egg-info/PKG-INFO
--rw-r--r--   0 du         (502) staff       (20)      196 2024-04-30 07:08:16.000000 deepgpu-2.1.0rc3.post5/deepgpu.egg-info/SOURCES.txt
--rw-r--r--   0 du         (502) staff       (20)        1 2024-04-30 07:08:16.000000 deepgpu-2.1.0rc3.post5/deepgpu.egg-info/dependency_links.txt
--rw-r--r--   0 du         (502) staff       (20)        8 2024-04-30 07:08:16.000000 deepgpu-2.1.0rc3.post5/deepgpu.egg-info/top_level.txt
--rw-r--r--   0 du         (502) staff       (20)       38 2024-04-30 07:08:16.665082 deepgpu-2.1.0rc3.post5/setup.cfg
--rw-r--r--   0 du         (502) staff       (20)     6975 2024-04-30 07:07:38.000000 deepgpu-2.1.0rc3.post5/setup.py
+drwxr-xr-x   0 du         (502) staff       (20)        0 2024-05-11 05:54:26.495954 deepgpu-2.1.0rc3.post6/
+-rw-r--r--   0 du         (502) staff       (20)       30 2023-10-10 07:39:14.000000 deepgpu-2.1.0rc3.post6/MANIFEST.in
+-rw-r--r--   0 du         (502) staff       (20)      621 2024-05-11 05:54:26.494542 deepgpu-2.1.0rc3.post6/PKG-INFO
+-rw-r--r--   0 du         (502) staff       (20)      292 2024-04-26 09:23:15.000000 deepgpu-2.1.0rc3.post6/README.md
+drwxr-xr-x   0 du         (502) staff       (20)        0 2024-05-11 05:54:26.492434 deepgpu-2.1.0rc3.post6/deepgpu/
+-rw-r--r--   0 du         (502) staff       (20)       17 2023-10-09 07:10:39.000000 deepgpu-2.1.0rc3.post6/deepgpu/__init__.py
+drwxr-xr-x   0 du         (502) staff       (20)        0 2024-05-11 05:54:26.493937 deepgpu-2.1.0rc3.post6/deepgpu.egg-info/
+-rw-r--r--   0 du         (502) staff       (20)      621 2024-05-11 05:54:26.000000 deepgpu-2.1.0rc3.post6/deepgpu.egg-info/PKG-INFO
+-rw-r--r--   0 du         (502) staff       (20)      196 2024-05-11 05:54:26.000000 deepgpu-2.1.0rc3.post6/deepgpu.egg-info/SOURCES.txt
+-rw-r--r--   0 du         (502) staff       (20)        1 2024-05-11 05:54:26.000000 deepgpu-2.1.0rc3.post6/deepgpu.egg-info/dependency_links.txt
+-rw-r--r--   0 du         (502) staff       (20)        8 2024-05-11 05:54:26.000000 deepgpu-2.1.0rc3.post6/deepgpu.egg-info/top_level.txt
+-rw-r--r--   0 du         (502) staff       (20)       38 2024-05-11 05:54:26.496093 deepgpu-2.1.0rc3.post6/setup.cfg
+-rw-r--r--   0 du         (502) staff       (20)     6975 2024-05-11 05:53:01.000000 deepgpu-2.1.0rc3.post6/setup.py
```

### Comparing `deepgpu-2.1.0rc3.post5/setup.py` & `deepgpu-2.1.0rc3.post6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 import subprocess
 from setuptools.command.install import install
 import os
 
 NAME="deepgpu"
 DEEPGPU_VERSION = "2.1.0rc3"
 DEEPYTORCH_PKG_VERSION = DEEPGPU_VERSION # same as DEEPGPU version so far
-DEEPGPU_VERSION = "2.1.0rc3.post5"
+DEEPGPU_VERSION = "2.1.0rc3.post6"
 support_os_list = ['ubuntu', 'centos', 'alinux'] # add version later
 support_pytorch_version = ['1.10', '1.11', '1.12', '1.13', '2.0', '2.1']
 support_cuda_version = ['11.1', '11.3', '11.6', '11.7', '11.8', '12.1', '12.3']
 support_python_version = ['38', '39', '310', '311']
 
 _root_path_deepgpu = "https://mirrors.aliyun.com/deepgpu/"
 _root_path_deepytorch = f"{_root_path_deepgpu}/deepytorch/{DEEPYTORCH_PKG_VERSION}/"
-_root_path_deepytorch = f"https://aiacc.oss-cn-beijing.aliyuncs.com/deepytorch/dev/2.1.0/24e35df4/"
+_root_path_deepytorch = f"https://aiacc.oss-cn-beijing.aliyuncs.com/deepytorch/dev/2.1.0/a8b7b99a/"
 _temp_path = f"{os.environ['HOME']}/.deepgpu/"
 _temp_log = f"{_temp_path}/log"
 
 tsinghua_source = "https://pypi.tuna.tsinghua.edu.cn/simple"
 
 
 class PostInstallCommand(install):
```

