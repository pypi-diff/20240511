# Comparing `tmp/sumologic-appclient-sdk-2.0.8.tar.gz` & `tmp/sumologic-appclient-sdk-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sumologic-appclient-sdk-2.0.8.tar", last modified: Thu Jun 23 04:54:18 2022, max compression
+gzip compressed data, was "sumologic-appclient-sdk-2.0.9.tar", last modified: Wed Dec 13 11:43:49 2023, max compression
```

## Comparing `sumologic-appclient-sdk-2.0.8.tar` & `sumologic-appclient-sdk-2.0.9.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 hpal       (501) staff       (20)        0 2022-06-23 04:54:18.003759 sumologic-appclient-sdk-2.0.8/
--rw-r--r--   0 hpal       (501) staff       (20)    11346 2019-10-01 04:36:53.000000 sumologic-appclient-sdk-2.0.8/LICENSE
--rw-r--r--   0 hpal       (501) staff       (20)      315 2020-11-24 15:38:58.000000 sumologic-appclient-sdk-2.0.8/MANIFEST.in
--rw-r--r--   0 hpal       (501) staff       (20)     1942 2022-06-23 04:54:18.003423 sumologic-appclient-sdk-2.0.8/PKG-INFO
--rw-r--r--   0 hpal       (501) staff       (20)      972 2020-12-29 15:16:17.000000 sumologic-appclient-sdk-2.0.8/README.md
--rw-r--r--   0 hpal       (501) staff       (20)        6 2022-06-23 04:49:02.000000 sumologic-appclient-sdk-2.0.8/VERSION
--rw-r--r--   0 hpal       (501) staff       (20)      102 2020-11-24 15:38:58.000000 sumologic-appclient-sdk-2.0.8/requirements.txt
--rw-r--r--   0 hpal       (501) staff       (20)       38 2022-06-23 04:54:18.003855 sumologic-appclient-sdk-2.0.8/setup.cfg
--rw-r--r--   0 hpal       (501) staff       (20)     2156 2019-10-01 04:36:53.000000 sumologic-appclient-sdk-2.0.8/setup.py
-drwxr-xr-x   0 hpal       (501) staff       (20)        0 2022-06-23 04:54:17.969841 sumologic-appclient-sdk-2.0.8/sumoappclient/
--rw-r--r--   0 hpal       (501) staff       (20)      103 2020-11-23 04:12:26.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/__init__.py
-drwxr-xr-x   0 hpal       (501) staff       (20)        0 2022-06-23 04:54:17.973574 sumologic-appclient-sdk-2.0.8/sumoappclient/common/
--rw-r--r--   0 hpal       (501) staff       (20)        0 2019-10-01 04:36:53.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/common/__init__.py
--rw-r--r--   0 hpal       (501) staff       (20)     3205 2021-12-21 17:52:32.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/common/ctocstatus.py
--rw-r--r--   0 hpal       (501) staff       (20)      711 2021-12-21 17:52:32.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/common/errors.py
--rw-r--r--   0 hpal       (501) staff       (20)     2640 2021-12-21 17:52:32.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/common/logger.py
--rw-r--r--   0 hpal       (501) staff       (20)     1257 2020-12-29 15:16:17.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/common/mixin.py
--rw-r--r--   0 hpal       (501) staff       (20)     4198 2021-12-21 17:52:32.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/common/utils.py
-drwxr-xr-x   0 hpal       (501) staff       (20)        0 2022-06-23 04:54:17.977676 sumologic-appclient-sdk-2.0.8/sumoappclient/configmanager/
--rw-r--r--   0 hpal       (501) staff       (20)        0 2020-12-29 15:16:17.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/configmanager/__init__.py
--rw-r--r--   0 hpal       (501) staff       (20)     3268 2020-12-29 15:16:17.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/configmanager/aws.py
--rw-r--r--   0 hpal       (501) staff       (20)      369 2020-12-29 15:16:17.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/configmanager/azure.py
--rw-r--r--   0 hpal       (501) staff       (20)     4900 2022-06-23 04:45:52.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/configmanager/base.py
--rw-r--r--   0 hpal       (501) staff       (20)     2157 2021-12-21 17:52:32.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/configmanager/ctoc.py
--rw-r--r--   0 hpal       (501) staff       (20)      367 2020-12-29 15:16:17.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/configmanager/gcp.py
--rw-r--r--   0 hpal       (501) staff       (20)      580 2020-12-29 15:16:17.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/configmanager/onprem.py
--rw-r--r--   0 hpal       (501) staff       (20)     1515 2020-12-29 15:16:17.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/console.py
-drwxr-xr-x   0 hpal       (501) staff       (20)        0 2022-06-23 04:54:17.982430 sumologic-appclient-sdk-2.0.8/sumoappclient/omnistorage/
--rw-r--r--   0 hpal       (501) staff       (20)        0 2019-10-01 04:36:53.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/omnistorage/__init__.py
--rw-r--r--   0 hpal       (501) staff       (20)    13650 2020-12-29 15:16:17.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/omnistorage/aws.py
--rw-r--r--   0 hpal       (501) staff       (20)     5179 2020-12-29 15:16:17.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/omnistorage/azure.py
--rw-r--r--   0 hpal       (501) staff       (20)     1606 2020-12-29 15:16:17.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/omnistorage/base.py
--rw-r--r--   0 hpal       (501) staff       (20)     4514 2021-12-21 17:52:32.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/omnistorage/ctoc.py
--rw-r--r--   0 hpal       (501) staff       (20)     3023 2020-12-29 15:16:17.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/omnistorage/gcp.py
--rw-r--r--   0 hpal       (501) staff       (20)     8485 2020-12-29 15:16:17.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/omnistorage/onprem.py
-drwxr-xr-x   0 hpal       (501) staff       (20)        0 2022-06-23 04:54:17.986697 sumologic-appclient-sdk-2.0.8/sumoappclient/pkggenerator/
--rw-r--r--   0 hpal       (501) staff       (20)        0 2019-10-01 04:36:53.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/pkggenerator/__init__.py
--rw-r--r--   0 hpal       (501) staff       (20)    16830 2021-12-21 17:52:32.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/pkggenerator/aws.py
--rw-r--r--   0 hpal       (501) staff       (20)     3742 2021-12-21 17:52:32.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/pkggenerator/base.py
--rw-r--r--   0 hpal       (501) staff       (20)     3022 2020-12-29 15:16:17.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/pkggenerator/onprem.py
-drwxr-xr-x   0 hpal       (501) staff       (20)        0 2022-06-23 04:54:17.965051 sumologic-appclient-sdk-2.0.8/sumoappclient/pkggenerator/resources/
-drwxr-xr-x   0 hpal       (501) staff       (20)        0 2022-06-23 04:54:17.988114 sumologic-appclient-sdk-2.0.8/sumoappclient/pkggenerator/resources/aws/
--rw-r--r--   0 hpal       (501) staff       (20)     1567 2020-11-24 15:38:58.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/pkggenerator/resources/aws/basesamtemplate.yaml
--rw-r--r--   0 hpal       (501) staff       (20)     4720 2021-12-21 17:52:32.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/pkggenerator/resources/aws/basesamwithkms.yaml
-drwxr-xr-x   0 hpal       (501) staff       (20)        0 2022-06-23 04:54:17.991990 sumologic-appclient-sdk-2.0.8/sumoappclient/pkggenerator/resources/setup/
--rw-r--r--   0 hpal       (501) staff       (20)    11346 2019-10-01 04:36:54.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/pkggenerator/resources/setup/LICENSE
--rw-r--r--   0 hpal       (501) staff       (20)      116 2019-10-01 04:36:54.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/pkggenerator/resources/setup/MANIFEST.in
--rw-r--r--   0 hpal       (501) staff       (20)      146 2020-11-24 15:38:58.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/pkggenerator/resources/setup/README.md
--rw-r--r--   0 hpal       (501) staff       (20)        6 2019-10-01 04:36:54.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/pkggenerator/resources/setup/VERSION
--rw-r--r--   0 hpal       (501) staff       (20)     1002 2020-12-29 15:16:17.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/pkggenerator/resources/setup/baseconfig.yaml
--rw-r--r--   0 hpal       (501) staff       (20)     2008 2020-11-24 15:38:58.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/pkggenerator/resources/setup/setup.py
--rw-r--r--   0 hpal       (501) staff       (20)     3066 2020-12-29 15:16:17.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/pkggenerator/setupgen.py
--rw-r--r--   0 hpal       (501) staff       (20)      842 2021-12-21 17:52:32.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/pkggenerator/utils.py
-drwxr-xr-x   0 hpal       (501) staff       (20)        0 2022-06-23 04:54:17.996898 sumologic-appclient-sdk-2.0.8/sumoappclient/provider/
--rw-r--r--   0 hpal       (501) staff       (20)        0 2020-12-29 15:16:17.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/provider/__init__.py
--rw-r--r--   0 hpal       (501) staff       (20)      598 2020-12-29 15:16:17.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/provider/aws.py
--rw-r--r--   0 hpal       (501) staff       (20)      552 2020-12-29 15:16:17.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/provider/azure.py
--rw-r--r--   0 hpal       (501) staff       (20)     1240 2020-12-29 15:16:17.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/provider/base.py
--rw-r--r--   0 hpal       (501) staff       (20)      607 2020-12-29 15:16:17.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/provider/ctoc.py
--rw-r--r--   0 hpal       (501) staff       (20)      868 2020-12-29 15:16:17.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/provider/factory.py
--rw-r--r--   0 hpal       (501) staff       (20)      485 2020-12-29 15:16:17.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/provider/gcp.py
--rw-r--r--   0 hpal       (501) staff       (20)      506 2020-12-29 15:16:17.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/provider/onprem.py
-drwxr-xr-x   0 hpal       (501) staff       (20)        0 2022-06-23 04:54:18.000738 sumologic-appclient-sdk-2.0.8/sumoappclient/sumoclient/
--rw-r--r--   0 hpal       (501) staff       (20)        0 2019-10-01 04:36:54.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/sumoclient/__init__.py
--rw-r--r--   0 hpal       (501) staff       (20)    19617 2021-12-21 17:52:32.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/sumoclient/base.py
--rw-r--r--   0 hpal       (501) staff       (20)      725 2021-01-25 11:35:17.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/sumoclient/factory.py
--rw-r--r--   0 hpal       (501) staff       (20)     5825 2021-12-21 17:52:32.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/sumoclient/httputils.py
--rw-r--r--   0 hpal       (501) staff       (20)     9257 2022-01-25 14:12:19.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/sumoclient/outputhandlers.py
--rw-r--r--   0 hpal       (501) staff       (20)      378 2022-01-25 13:59:27.000000 sumologic-appclient-sdk-2.0.8/sumoappclient/sumoclient/utils.py
-drwxr-xr-x   0 hpal       (501) staff       (20)        0 2022-06-23 04:54:18.003039 sumologic-appclient-sdk-2.0.8/sumologic_appclient_sdk.egg-info/
--rw-r--r--   0 hpal       (501) staff       (20)     1942 2022-06-23 04:54:17.000000 sumologic-appclient-sdk-2.0.8/sumologic_appclient_sdk.egg-info/PKG-INFO
--rw-r--r--   0 hpal       (501) staff       (20)     2271 2022-06-23 04:54:17.000000 sumologic-appclient-sdk-2.0.8/sumologic_appclient_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 hpal       (501) staff       (20)        1 2022-06-23 04:54:17.000000 sumologic-appclient-sdk-2.0.8/sumologic_appclient_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 hpal       (501) staff       (20)       62 2022-06-23 04:54:17.000000 sumologic-appclient-sdk-2.0.8/sumologic_appclient_sdk.egg-info/entry_points.txt
--rw-r--r--   0 hpal       (501) staff       (20)      582 2022-06-23 04:54:17.000000 sumologic-appclient-sdk-2.0.8/sumologic_appclient_sdk.egg-info/requires.txt
--rw-r--r--   0 hpal       (501) staff       (20)       20 2022-06-23 04:54:17.000000 sumologic-appclient-sdk-2.0.8/sumologic_appclient_sdk.egg-info/top_level.txt
--rw-r--r--   0 hpal       (501) staff       (20)        1 2022-06-23 04:54:17.000000 sumologic-appclient-sdk-2.0.8/sumologic_appclient_sdk.egg-info/zip-safe
+drwxr-xr-x   0 hsharma    (501) staff       (20)        0 2023-12-13 11:43:49.384616 sumologic-appclient-sdk-2.0.9/
+-rw-r--r--   0 hsharma    (501) staff       (20)    11346 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/LICENSE
+-rw-r--r--   0 hsharma    (501) staff       (20)      315 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/MANIFEST.in
+-rw-r--r--   0 hsharma    (501) staff       (20)     2027 2023-12-13 11:43:49.383821 sumologic-appclient-sdk-2.0.9/PKG-INFO
+-rw-r--r--   0 hsharma    (501) staff       (20)     1226 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/README.md
+-rw-r--r--   0 hsharma    (501) staff       (20)        6 2023-12-13 11:43:20.000000 sumologic-appclient-sdk-2.0.9/VERSION
+-rw-r--r--   0 hsharma    (501) staff       (20)       77 2023-12-12 11:11:19.000000 sumologic-appclient-sdk-2.0.9/requirements.txt
+-rw-r--r--   0 hsharma    (501) staff       (20)       38 2023-12-13 11:43:49.384941 sumologic-appclient-sdk-2.0.9/setup.cfg
+-rw-r--r--   0 hsharma    (501) staff       (20)     2156 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/setup.py
+drwxr-xr-x   0 hsharma    (501) staff       (20)        0 2023-12-13 11:43:49.242161 sumologic-appclient-sdk-2.0.9/sumoappclient/
+-rw-r--r--   0 hsharma    (501) staff       (20)      103 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/__init__.py
+drwxr-xr-x   0 hsharma    (501) staff       (20)        0 2023-12-13 11:43:49.251071 sumologic-appclient-sdk-2.0.9/sumoappclient/common/
+-rw-r--r--   0 hsharma    (501) staff       (20)        0 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/common/__init__.py
+-rw-r--r--   0 hsharma    (501) staff       (20)     3205 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/common/ctocstatus.py
+-rw-r--r--   0 hsharma    (501) staff       (20)      711 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/common/errors.py
+-rw-r--r--   0 hsharma    (501) staff       (20)     2640 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/common/logger.py
+-rw-r--r--   0 hsharma    (501) staff       (20)     1257 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/common/mixin.py
+-rw-r--r--   0 hsharma    (501) staff       (20)     4198 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/common/utils.py
+drwxr-xr-x   0 hsharma    (501) staff       (20)        0 2023-12-13 11:43:49.267273 sumologic-appclient-sdk-2.0.9/sumoappclient/configmanager/
+-rw-r--r--   0 hsharma    (501) staff       (20)        0 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/configmanager/__init__.py
+-rw-r--r--   0 hsharma    (501) staff       (20)     3268 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/configmanager/aws.py
+-rw-r--r--   0 hsharma    (501) staff       (20)      369 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/configmanager/azure.py
+-rw-r--r--   0 hsharma    (501) staff       (20)     4900 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/configmanager/base.py
+-rw-r--r--   0 hsharma    (501) staff       (20)     2157 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/configmanager/ctoc.py
+-rw-r--r--   0 hsharma    (501) staff       (20)      367 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/configmanager/gcp.py
+-rw-r--r--   0 hsharma    (501) staff       (20)      580 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/configmanager/onprem.py
+-rw-r--r--   0 hsharma    (501) staff       (20)     1515 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/console.py
+drwxr-xr-x   0 hsharma    (501) staff       (20)        0 2023-12-13 11:43:49.294248 sumologic-appclient-sdk-2.0.9/sumoappclient/omnistorage/
+-rw-r--r--   0 hsharma    (501) staff       (20)        0 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/omnistorage/__init__.py
+-rw-r--r--   0 hsharma    (501) staff       (20)    13650 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/omnistorage/aws.py
+-rw-r--r--   0 hsharma    (501) staff       (20)     5179 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/omnistorage/azure.py
+-rw-r--r--   0 hsharma    (501) staff       (20)     1606 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/omnistorage/base.py
+-rw-r--r--   0 hsharma    (501) staff       (20)     4514 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/omnistorage/ctoc.py
+-rw-r--r--   0 hsharma    (501) staff       (20)     3023 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/omnistorage/gcp.py
+-rw-r--r--   0 hsharma    (501) staff       (20)     8485 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/omnistorage/onprem.py
+drwxr-xr-x   0 hsharma    (501) staff       (20)        0 2023-12-13 11:43:49.306206 sumologic-appclient-sdk-2.0.9/sumoappclient/pkggenerator/
+-rw-r--r--   0 hsharma    (501) staff       (20)        0 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/pkggenerator/__init__.py
+-rw-r--r--   0 hsharma    (501) staff       (20)    16830 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/pkggenerator/aws.py
+-rw-r--r--   0 hsharma    (501) staff       (20)     3742 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/pkggenerator/base.py
+-rw-r--r--   0 hsharma    (501) staff       (20)     3022 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/pkggenerator/onprem.py
+drwxr-xr-x   0 hsharma    (501) staff       (20)        0 2023-12-13 11:43:49.230219 sumologic-appclient-sdk-2.0.9/sumoappclient/pkggenerator/resources/
+drwxr-xr-x   0 hsharma    (501) staff       (20)        0 2023-12-13 11:43:49.312469 sumologic-appclient-sdk-2.0.9/sumoappclient/pkggenerator/resources/aws/
+-rw-r--r--   0 hsharma    (501) staff       (20)     1567 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/pkggenerator/resources/aws/basesamtemplate.yaml
+-rw-r--r--   0 hsharma    (501) staff       (20)     4720 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/pkggenerator/resources/aws/basesamwithkms.yaml
+drwxr-xr-x   0 hsharma    (501) staff       (20)        0 2023-12-13 11:43:49.326864 sumologic-appclient-sdk-2.0.9/sumoappclient/pkggenerator/resources/setup/
+-rw-r--r--   0 hsharma    (501) staff       (20)    11346 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/pkggenerator/resources/setup/LICENSE
+-rw-r--r--   0 hsharma    (501) staff       (20)      116 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/pkggenerator/resources/setup/MANIFEST.in
+-rw-r--r--   0 hsharma    (501) staff       (20)      146 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/pkggenerator/resources/setup/README.md
+-rw-r--r--   0 hsharma    (501) staff       (20)        6 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/pkggenerator/resources/setup/VERSION
+-rw-r--r--   0 hsharma    (501) staff       (20)     1002 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/pkggenerator/resources/setup/baseconfig.yaml
+-rw-r--r--   0 hsharma    (501) staff       (20)     2008 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/pkggenerator/resources/setup/setup.py
+-rw-r--r--   0 hsharma    (501) staff       (20)     3066 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/pkggenerator/setupgen.py
+-rw-r--r--   0 hsharma    (501) staff       (20)      842 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/pkggenerator/utils.py
+drwxr-xr-x   0 hsharma    (501) staff       (20)        0 2023-12-13 11:43:49.345649 sumologic-appclient-sdk-2.0.9/sumoappclient/provider/
+-rw-r--r--   0 hsharma    (501) staff       (20)        0 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/provider/__init__.py
+-rw-r--r--   0 hsharma    (501) staff       (20)      598 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/provider/aws.py
+-rw-r--r--   0 hsharma    (501) staff       (20)      552 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/provider/azure.py
+-rw-r--r--   0 hsharma    (501) staff       (20)     1240 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/provider/base.py
+-rw-r--r--   0 hsharma    (501) staff       (20)      607 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/provider/ctoc.py
+-rw-r--r--   0 hsharma    (501) staff       (20)      868 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/provider/factory.py
+-rw-r--r--   0 hsharma    (501) staff       (20)      485 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/provider/gcp.py
+-rw-r--r--   0 hsharma    (501) staff       (20)      506 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/provider/onprem.py
+drwxr-xr-x   0 hsharma    (501) staff       (20)        0 2023-12-13 11:43:49.358146 sumologic-appclient-sdk-2.0.9/sumoappclient/sumoclient/
+-rw-r--r--   0 hsharma    (501) staff       (20)        0 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/sumoclient/__init__.py
+-rw-r--r--   0 hsharma    (501) staff       (20)    19617 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/sumoclient/base.py
+-rw-r--r--   0 hsharma    (501) staff       (20)      725 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/sumoclient/factory.py
+-rw-r--r--   0 hsharma    (501) staff       (20)     5825 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/sumoclient/httputils.py
+-rw-r--r--   0 hsharma    (501) staff       (20)     9257 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/sumoclient/outputhandlers.py
+-rw-r--r--   0 hsharma    (501) staff       (20)      378 2023-12-06 13:59:39.000000 sumologic-appclient-sdk-2.0.9/sumoappclient/sumoclient/utils.py
+drwxr-xr-x   0 hsharma    (501) staff       (20)        0 2023-12-13 11:43:49.380072 sumologic-appclient-sdk-2.0.9/sumologic_appclient_sdk.egg-info/
+-rw-r--r--   0 hsharma    (501) staff       (20)     2027 2023-12-13 11:43:48.000000 sumologic-appclient-sdk-2.0.9/sumologic_appclient_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 hsharma    (501) staff       (20)     2271 2023-12-13 11:43:48.000000 sumologic-appclient-sdk-2.0.9/sumologic_appclient_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 hsharma    (501) staff       (20)        1 2023-12-13 11:43:48.000000 sumologic-appclient-sdk-2.0.9/sumologic_appclient_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 hsharma    (501) staff       (20)       61 2023-12-13 11:43:48.000000 sumologic-appclient-sdk-2.0.9/sumologic_appclient_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 hsharma    (501) staff       (20)      558 2023-12-13 11:43:48.000000 sumologic-appclient-sdk-2.0.9/sumologic_appclient_sdk.egg-info/requires.txt
+-rw-r--r--   0 hsharma    (501) staff       (20)       20 2023-12-13 11:43:48.000000 sumologic-appclient-sdk-2.0.9/sumologic_appclient_sdk.egg-info/top_level.txt
+-rw-r--r--   0 hsharma    (501) staff       (20)        1 2023-12-06 15:14:35.000000 sumologic-appclient-sdk-2.0.9/sumologic_appclient_sdk.egg-info/zip-safe
```

### Comparing `sumologic-appclient-sdk-2.0.8/LICENSE` & `sumologic-appclient-sdk-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/PKG-INFO` & `sumologic-appclient-sdk-2.0.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,51 @@
 Metadata-Version: 2.1
 Name: sumologic-appclient-sdk
-Version: 2.0.8
+Version: 2.0.9
 Summary: Sumo Logic appclient sdk for api based collection
 Home-page: https://github.com/SumoLogic/sumologic-appclient-sdk
 Author: SumoLogic
 Author-email: it@sumologic.com, apps-team@sumologic.com
 License: PSF
-Description: # sumologic-appclient-sdk
-        SDK with utility libraries for App team's collection clients
-        
-        ## omnistorage
-        Omnistorage is a persistent key value store library which provides a unified and easy to use API and can be used with both oncloud and onprem applications.
-        It hides the differences between datastores from major cloud providers like aws, gcp, azure and prevent data lock-in on a single vendor. 
-        
-        ## common
-        Contains common utilities for config management, log management etc.
-        
-        ## sumoclient
-        Sumo Logic Client supporting multiple output handlers like http, file, s3 etc.
-        
-        
-        ## pkggenerator
-        This module is responsible for building and deploying packages for both oncloud(aws, gcp and azure) and onprem enviroments(in pypi repo).
-        
-        ## Documentation
-        * [Design Doc](https://docs.google.com/document/d/11UCaLRtRVoO2u58L_P85ri_fbgQ2vuoDpxIyaV_jt4U/edit?usp=sharing) 
-        * [Usage Doc](https://docs.google.com/document/d/1lpwcvHB4IUtN3gkCcMTo4F2cCig-pClIwa-XVVWl6SQ/edit?usp=sharing) 
-        
 Keywords: sumologic python rest api log management analytics logreduce api appclient agent security siem collector forwarder
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: aws
 Provides-Extra: gcp
+Provides-Extra: azure
 Provides-Extra: all
 Provides-Extra: dev
-Provides-Extra: azure
+License-File: LICENSE
+
+# sumologic-appclient-sdk
+SDK with utility libraries for App team's collection clients
+
+## omnistorage
+Omnistorage is a persistent key value store library which provides a unified and easy to use API and can be used with both oncloud and onprem applications.
+It hides the differences between datastores from major cloud providers like aws, gcp, azure and prevent data lock-in on a single vendor. 
+
+## common
+Contains common utilities for config management, log management etc.
+
+## sumoclient
+Sumo Logic Client supporting multiple output handlers like http, file, s3 etc.
+
+
+## pkggenerator
+This module is responsible for building and deploying packages for both oncloud(aws, gcp and azure) and onprem enviroments(in pypi repo).
+
+## Build and Publish
+Run below command to publish to pypi repository
+
+`sumoappclient -e onprem -d prod -c sumoappclient/metadata.yaml`
+
+To create a local build for generating whl files
+
+`sumoappclient -e onprem -d local -c sumoappclient/metadata.yaml` 
+
+## Documentation
+* [Design Doc](https://docs.google.com/document/d/11UCaLRtRVoO2u58L_P85ri_fbgQ2vuoDpxIyaV_jt4U/edit?usp=sharing) 
+* [Usage Doc](https://docs.google.com/document/d/1lpwcvHB4IUtN3gkCcMTo4F2cCig-pClIwa-XVVWl6SQ/edit?usp=sharing)
```

### Comparing `sumologic-appclient-sdk-2.0.8/setup.py` & `sumologic-appclient-sdk-2.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/common/ctocstatus.py` & `sumologic-appclient-sdk-2.0.9/sumoappclient/common/ctocstatus.py`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/common/errors.py` & `sumologic-appclient-sdk-2.0.9/sumoappclient/common/errors.py`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/common/logger.py` & `sumologic-appclient-sdk-2.0.9/sumoappclient/common/logger.py`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/common/mixin.py` & `sumologic-appclient-sdk-2.0.9/sumoappclient/common/mixin.py`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/common/utils.py` & `sumologic-appclient-sdk-2.0.9/sumoappclient/common/utils.py`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/configmanager/aws.py` & `sumologic-appclient-sdk-2.0.9/sumoappclient/configmanager/aws.py`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/configmanager/base.py` & `sumologic-appclient-sdk-2.0.9/sumoappclient/configmanager/base.py`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/configmanager/ctoc.py` & `sumologic-appclient-sdk-2.0.9/sumoappclient/configmanager/ctoc.py`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/configmanager/onprem.py` & `sumologic-appclient-sdk-2.0.9/sumoappclient/configmanager/onprem.py`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/console.py` & `sumologic-appclient-sdk-2.0.9/sumoappclient/console.py`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/omnistorage/aws.py` & `sumologic-appclient-sdk-2.0.9/sumoappclient/omnistorage/aws.py`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/omnistorage/azure.py` & `sumologic-appclient-sdk-2.0.9/sumoappclient/omnistorage/azure.py`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/omnistorage/base.py` & `sumologic-appclient-sdk-2.0.9/sumoappclient/omnistorage/base.py`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/omnistorage/ctoc.py` & `sumologic-appclient-sdk-2.0.9/sumoappclient/omnistorage/ctoc.py`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/omnistorage/gcp.py` & `sumologic-appclient-sdk-2.0.9/sumoappclient/omnistorage/gcp.py`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/omnistorage/onprem.py` & `sumologic-appclient-sdk-2.0.9/sumoappclient/omnistorage/onprem.py`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/pkggenerator/aws.py` & `sumologic-appclient-sdk-2.0.9/sumoappclient/pkggenerator/aws.py`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/pkggenerator/base.py` & `sumologic-appclient-sdk-2.0.9/sumoappclient/pkggenerator/base.py`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/pkggenerator/onprem.py` & `sumologic-appclient-sdk-2.0.9/sumoappclient/pkggenerator/onprem.py`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/pkggenerator/resources/aws/basesamtemplate.yaml` & `sumologic-appclient-sdk-2.0.9/sumoappclient/pkggenerator/resources/aws/basesamtemplate.yaml`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/pkggenerator/resources/aws/basesamwithkms.yaml` & `sumologic-appclient-sdk-2.0.9/sumoappclient/pkggenerator/resources/aws/basesamwithkms.yaml`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/pkggenerator/resources/setup/LICENSE` & `sumologic-appclient-sdk-2.0.9/sumoappclient/pkggenerator/resources/setup/LICENSE`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/pkggenerator/resources/setup/baseconfig.yaml` & `sumologic-appclient-sdk-2.0.9/sumoappclient/pkggenerator/resources/setup/baseconfig.yaml`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/pkggenerator/resources/setup/setup.py` & `sumologic-appclient-sdk-2.0.9/sumoappclient/pkggenerator/resources/setup/setup.py`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/pkggenerator/setupgen.py` & `sumologic-appclient-sdk-2.0.9/sumoappclient/pkggenerator/setupgen.py`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/pkggenerator/utils.py` & `sumologic-appclient-sdk-2.0.9/sumoappclient/pkggenerator/utils.py`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/provider/aws.py` & `sumologic-appclient-sdk-2.0.9/sumoappclient/provider/aws.py`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/provider/azure.py` & `sumologic-appclient-sdk-2.0.9/sumoappclient/provider/azure.py`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/provider/base.py` & `sumologic-appclient-sdk-2.0.9/sumoappclient/provider/base.py`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/provider/ctoc.py` & `sumologic-appclient-sdk-2.0.9/sumoappclient/provider/ctoc.py`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/provider/factory.py` & `sumologic-appclient-sdk-2.0.9/sumoappclient/provider/factory.py`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/sumoclient/base.py` & `sumologic-appclient-sdk-2.0.9/sumoappclient/sumoclient/base.py`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/sumoclient/factory.py` & `sumologic-appclient-sdk-2.0.9/sumoappclient/sumoclient/factory.py`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/sumoclient/httputils.py` & `sumologic-appclient-sdk-2.0.9/sumoappclient/sumoclient/httputils.py`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumoappclient/sumoclient/outputhandlers.py` & `sumologic-appclient-sdk-2.0.9/sumoappclient/sumoclient/outputhandlers.py`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumologic_appclient_sdk.egg-info/PKG-INFO` & `sumologic-appclient-sdk-2.0.9/sumologic_appclient_sdk.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,51 @@
 Metadata-Version: 2.1
 Name: sumologic-appclient-sdk
-Version: 2.0.8
+Version: 2.0.9
 Summary: Sumo Logic appclient sdk for api based collection
 Home-page: https://github.com/SumoLogic/sumologic-appclient-sdk
 Author: SumoLogic
 Author-email: it@sumologic.com, apps-team@sumologic.com
 License: PSF
-Description: # sumologic-appclient-sdk
-        SDK with utility libraries for App team's collection clients
-        
-        ## omnistorage
-        Omnistorage is a persistent key value store library which provides a unified and easy to use API and can be used with both oncloud and onprem applications.
-        It hides the differences between datastores from major cloud providers like aws, gcp, azure and prevent data lock-in on a single vendor. 
-        
-        ## common
-        Contains common utilities for config management, log management etc.
-        
-        ## sumoclient
-        Sumo Logic Client supporting multiple output handlers like http, file, s3 etc.
-        
-        
-        ## pkggenerator
-        This module is responsible for building and deploying packages for both oncloud(aws, gcp and azure) and onprem enviroments(in pypi repo).
-        
-        ## Documentation
-        * [Design Doc](https://docs.google.com/document/d/11UCaLRtRVoO2u58L_P85ri_fbgQ2vuoDpxIyaV_jt4U/edit?usp=sharing) 
-        * [Usage Doc](https://docs.google.com/document/d/1lpwcvHB4IUtN3gkCcMTo4F2cCig-pClIwa-XVVWl6SQ/edit?usp=sharing) 
-        
 Keywords: sumologic python rest api log management analytics logreduce api appclient agent security siem collector forwarder
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: aws
 Provides-Extra: gcp
+Provides-Extra: azure
 Provides-Extra: all
 Provides-Extra: dev
-Provides-Extra: azure
+License-File: LICENSE
+
+# sumologic-appclient-sdk
+SDK with utility libraries for App team's collection clients
+
+## omnistorage
+Omnistorage is a persistent key value store library which provides a unified and easy to use API and can be used with both oncloud and onprem applications.
+It hides the differences between datastores from major cloud providers like aws, gcp, azure and prevent data lock-in on a single vendor. 
+
+## common
+Contains common utilities for config management, log management etc.
+
+## sumoclient
+Sumo Logic Client supporting multiple output handlers like http, file, s3 etc.
+
+
+## pkggenerator
+This module is responsible for building and deploying packages for both oncloud(aws, gcp and azure) and onprem enviroments(in pypi repo).
+
+## Build and Publish
+Run below command to publish to pypi repository
+
+`sumoappclient -e onprem -d prod -c sumoappclient/metadata.yaml`
+
+To create a local build for generating whl files
+
+`sumoappclient -e onprem -d local -c sumoappclient/metadata.yaml` 
+
+## Documentation
+* [Design Doc](https://docs.google.com/document/d/11UCaLRtRVoO2u58L_P85ri_fbgQ2vuoDpxIyaV_jt4U/edit?usp=sharing) 
+* [Usage Doc](https://docs.google.com/document/d/1lpwcvHB4IUtN3gkCcMTo4F2cCig-pClIwa-XVVWl6SQ/edit?usp=sharing)
```

### Comparing `sumologic-appclient-sdk-2.0.8/sumologic_appclient_sdk.egg-info/SOURCES.txt` & `sumologic-appclient-sdk-2.0.9/sumologic_appclient_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sumologic-appclient-sdk-2.0.8/sumologic_appclient_sdk.egg-info/requires.txt` & `sumologic-appclient-sdk-2.0.9/sumologic_appclient_sdk.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-requests>=2.21.0
-PyYAML>=3.13
+requests>=2.31.0
+PyYAML>=6.0
 six>=1.11.0
 python-dateutil>=2.7.3
-future-fstrings>=1.2.0
-psutil>=5.6.3
+psutil>=5.9.6
 
 [:python_version < "3.2"]
 futures
 
 [:python_version < "3.6"]
 future-fstrings
```

