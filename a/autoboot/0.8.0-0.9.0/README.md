# Comparing `tmp/autoboot-0.8.0.tar.gz` & `tmp/autoboot-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoboot-0.8.0.tar", last modified: Fri May 10 19:47:00 2024, max compression
+gzip compressed data, was "autoboot-0.9.0.tar", last modified: Sat May 11 20:02:56 2024, max compression
```

## Comparing `autoboot-0.8.0.tar` & `autoboot-0.9.0.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-10 19:47:00.788975 autoboot-0.8.0/
--rw-r--r--   0 yizzuide   (501) staff       (20)     1065 2023-11-15 08:28:44.000000 autoboot-0.8.0/LICENSE.txt
--rw-r--r--   0 yizzuide   (501) staff       (20)       62 2023-12-12 18:43:45.000000 autoboot-0.8.0/MANIFEST.in
--rw-r--r--   0 yizzuide   (501) staff       (20)     8476 2024-05-10 19:47:00.788807 autoboot-0.8.0/PKG-INFO
--rw-r--r--   0 yizzuide   (501) staff       (20)     7605 2024-05-10 19:30:18.000000 autoboot-0.8.0/README.md
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-10 19:47:00.771031 autoboot-0.8.0/autoboot/
--rw-r--r--   0 yizzuide   (501) staff       (20)      264 2024-05-10 19:31:47.000000 autoboot-0.8.0/autoboot/__init__.py
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-10 19:47:00.775406 autoboot-0.8.0/autoboot/annotation/
--rw-r--r--   0 yizzuide   (501) staff       (20)      236 2024-05-10 14:14:09.000000 autoboot-0.8.0/autoboot/annotation/__init__.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     1665 2023-11-30 09:28:44.000000 autoboot-0.8.0/autoboot/annotation/component.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      804 2023-11-23 09:22:19.000000 autoboot-0.8.0/autoboot/annotation/effect.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     1715 2024-05-10 19:23:56.000000 autoboot-0.8.0/autoboot/annotation/env.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     1149 2023-11-22 02:16:54.000000 autoboot-0.8.0/autoboot/annotation/log.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      703 2024-05-10 14:28:44.000000 autoboot-0.8.0/autoboot/application_properties.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     4351 2024-04-07 17:23:55.000000 autoboot-0.8.0/autoboot/applications.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      735 2023-11-18 02:00:00.000000 autoboot-0.8.0/autoboot/args.py
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-10 19:47:00.777146 autoboot-0.8.0/autoboot/event/
--rw-r--r--   0 yizzuide   (501) staff       (20)      325 2023-11-30 08:56:48.000000 autoboot-0.8.0/autoboot/event/__init__.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      245 2023-11-30 09:27:02.000000 autoboot-0.8.0/autoboot/event/application_listener.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      173 2023-11-30 09:17:22.000000 autoboot-0.8.0/autoboot/event/component_listener.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     1301 2024-04-07 17:24:04.000000 autoboot-0.8.0/autoboot/event/event_emitter.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     2497 2023-11-22 02:16:54.000000 autoboot-0.8.0/autoboot/logging.py
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-10 19:47:00.779630 autoboot-0.8.0/autoboot/meta/
--rw-r--r--   0 yizzuide   (501) staff       (20)      143 2023-11-30 09:44:03.000000 autoboot-0.8.0/autoboot/meta/__init__.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      416 2023-11-30 02:17:32.000000 autoboot-0.8.0/autoboot/meta/component.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      526 2023-11-30 02:17:32.000000 autoboot-0.8.0/autoboot/meta/component_metaclass.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      353 2023-11-30 09:46:42.000000 autoboot-0.8.0/autoboot/meta/listener.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      169 2023-09-23 12:42:36.000000 autoboot-0.8.0/autoboot/meta/property.py
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-10 19:47:00.780854 autoboot-0.8.0/autoboot/plugin/
--rw-r--r--   0 yizzuide   (501) staff       (20)       60 2023-11-30 03:14:32.000000 autoboot-0.8.0/autoboot/plugin/__init__.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     1059 2023-11-30 08:26:53.000000 autoboot-0.8.0/autoboot/plugin/app_plugin.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      285 2023-11-30 02:52:47.000000 autoboot-0.8.0/autoboot/plugin/app_plugin_metaclass.py
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-10 19:47:00.782308 autoboot-0.8.0/autoboot/process/
--rw-r--r--   0 yizzuide   (501) staff       (20)      840 2023-11-30 02:17:32.000000 autoboot-0.8.0/autoboot/process/__init__.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      370 2023-11-29 02:28:21.000000 autoboot-0.8.0/autoboot/process/env_process.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     1445 2023-11-30 02:17:32.000000 autoboot-0.8.0/autoboot/process/yaml_constructors.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      728 2023-11-30 02:17:32.000000 autoboot-0.8.0/autoboot/process/yaml_parser.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      489 2024-05-10 19:27:01.000000 autoboot-0.8.0/autoboot/server_properties.py
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-10 19:47:00.783158 autoboot-0.8.0/autoboot/thread/
--rw-r--r--   0 yizzuide   (501) staff       (20)       70 2023-11-25 09:39:12.000000 autoboot-0.8.0/autoboot/thread/__init__.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     1514 2023-11-30 02:17:32.000000 autoboot-0.8.0/autoboot/thread/thread_pool.py
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-10 19:47:00.786125 autoboot-0.8.0/autoboot/util/
--rw-r--r--   0 yizzuide   (501) staff       (20)        0 2023-11-16 02:54:04.000000 autoboot-0.8.0/autoboot/util/__init__.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     2712 2023-11-30 02:17:32.000000 autoboot-0.8.0/autoboot/util/capacity.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      302 2023-11-17 07:31:30.000000 autoboot-0.8.0/autoboot/util/json_model.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      560 2023-11-17 06:29:28.000000 autoboot-0.8.0/autoboot/util/local_cache.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      504 2023-11-14 09:04:15.000000 autoboot-0.8.0/autoboot/util/object_navigator.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     1092 2023-11-22 07:00:40.000000 autoboot-0.8.0/autoboot/util/type_reflect.py
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-10 19:47:00.788164 autoboot-0.8.0/autoboot.egg-info/
--rw-r--r--   0 yizzuide   (501) staff       (20)     8476 2024-05-10 19:47:00.000000 autoboot-0.8.0/autoboot.egg-info/PKG-INFO
--rw-r--r--   0 yizzuide   (501) staff       (20)     1397 2024-05-10 19:47:00.000000 autoboot-0.8.0/autoboot.egg-info/SOURCES.txt
--rw-r--r--   0 yizzuide   (501) staff       (20)        1 2024-05-10 19:47:00.000000 autoboot-0.8.0/autoboot.egg-info/dependency_links.txt
--rw-r--r--   0 yizzuide   (501) staff       (20)        1 2023-12-13 07:06:28.000000 autoboot-0.8.0/autoboot.egg-info/not-zip-safe
--rw-r--r--   0 yizzuide   (501) staff       (20)      177 2024-05-10 19:47:00.000000 autoboot-0.8.0/autoboot.egg-info/requires.txt
--rw-r--r--   0 yizzuide   (501) staff       (20)        9 2024-05-10 19:47:00.000000 autoboot-0.8.0/autoboot.egg-info/top_level.txt
--rw-r--r--   0 yizzuide   (501) staff       (20)     1419 2023-12-12 17:55:45.000000 autoboot-0.8.0/pyproject.toml
--rw-r--r--   0 yizzuide   (501) staff       (20)      184 2023-12-13 09:50:43.000000 autoboot-0.8.0/requirements.txt
--rw-r--r--   0 yizzuide   (501) staff       (20)      969 2024-05-10 19:47:00.789583 autoboot-0.8.0/setup.cfg
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-10 19:47:00.787756 autoboot-0.8.0/tests/
--rw-r--r--   0 yizzuide   (501) staff       (20)      834 2024-04-07 17:24:15.000000 autoboot-0.8.0/tests/test_event_emitter.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      523 2023-11-20 06:17:50.000000 autoboot-0.8.0/tests/test_json_model.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      137 2023-11-17 06:18:39.000000 autoboot-0.8.0/tests/test_pipy_repo.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      350 2023-11-24 06:20:43.000000 autoboot-0.8.0/tests/test_retry.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-11 20:02:56.535608 autoboot-0.9.0/
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1065 2023-11-15 08:28:44.000000 autoboot-0.9.0/LICENSE.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)       96 2024-05-11 11:21:08.000000 autoboot-0.9.0/MANIFEST.in
+-rw-r--r--   0 yizzuide   (501) staff       (20)     8468 2024-05-11 20:02:56.535409 autoboot-0.9.0/PKG-INFO
+-rw-r--r--   0 yizzuide   (501) staff       (20)     7605 2024-05-10 19:30:18.000000 autoboot-0.9.0/README.md
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-11 20:02:56.515228 autoboot-0.9.0/autoboot/
+-rw-r--r--   0 yizzuide   (501) staff       (20)      264 2024-05-11 10:47:19.000000 autoboot-0.9.0/autoboot/__init__.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-11 20:02:56.520725 autoboot-0.9.0/autoboot/annotation/
+-rw-r--r--   0 yizzuide   (501) staff       (20)      236 2024-05-10 14:14:09.000000 autoboot-0.9.0/autoboot/annotation/__init__.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1665 2023-11-30 09:28:44.000000 autoboot-0.9.0/autoboot/annotation/component.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      804 2023-11-23 09:22:19.000000 autoboot-0.9.0/autoboot/annotation/effect.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1715 2024-05-11 07:59:16.000000 autoboot-0.9.0/autoboot/annotation/env.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1149 2023-11-22 02:16:54.000000 autoboot-0.9.0/autoboot/annotation/log.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      803 2024-05-11 10:06:16.000000 autoboot-0.9.0/autoboot/application_properties.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     4398 2024-05-11 10:20:03.000000 autoboot-0.9.0/autoboot/applications.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      735 2023-11-18 02:00:00.000000 autoboot-0.9.0/autoboot/args.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     3690 2024-05-11 19:52:03.000000 autoboot-0.9.0/autoboot/autoboot.schema.json
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-11 20:02:56.524558 autoboot-0.9.0/autoboot/event/
+-rw-r--r--   0 yizzuide   (501) staff       (20)      325 2023-11-30 08:56:48.000000 autoboot-0.9.0/autoboot/event/__init__.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      245 2023-11-30 09:27:02.000000 autoboot-0.9.0/autoboot/event/application_listener.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      173 2023-11-30 09:17:22.000000 autoboot-0.9.0/autoboot/event/component_listener.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1301 2024-04-07 17:24:04.000000 autoboot-0.9.0/autoboot/event/event_emitter.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     2679 2024-05-11 10:04:44.000000 autoboot-0.9.0/autoboot/logging.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-11 20:02:56.526892 autoboot-0.9.0/autoboot/meta/
+-rw-r--r--   0 yizzuide   (501) staff       (20)      143 2023-11-30 09:44:03.000000 autoboot-0.9.0/autoboot/meta/__init__.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      416 2023-11-30 02:17:32.000000 autoboot-0.9.0/autoboot/meta/component.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      526 2023-11-30 02:17:32.000000 autoboot-0.9.0/autoboot/meta/component_metaclass.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      353 2023-11-30 09:46:42.000000 autoboot-0.9.0/autoboot/meta/listener.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      169 2023-09-23 12:42:36.000000 autoboot-0.9.0/autoboot/meta/property.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-11 20:02:56.528586 autoboot-0.9.0/autoboot/plugin/
+-rw-r--r--   0 yizzuide   (501) staff       (20)       60 2023-11-30 03:14:32.000000 autoboot-0.9.0/autoboot/plugin/__init__.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1059 2023-11-30 08:26:53.000000 autoboot-0.9.0/autoboot/plugin/app_plugin.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      285 2023-11-30 02:52:47.000000 autoboot-0.9.0/autoboot/plugin/app_plugin_metaclass.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-11 20:02:56.530301 autoboot-0.9.0/autoboot/process/
+-rw-r--r--   0 yizzuide   (501) staff       (20)      840 2023-11-30 02:17:32.000000 autoboot-0.9.0/autoboot/process/__init__.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      370 2023-11-29 02:28:21.000000 autoboot-0.9.0/autoboot/process/env_process.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1445 2023-11-30 02:17:32.000000 autoboot-0.9.0/autoboot/process/yaml_constructors.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      728 2023-11-30 02:17:32.000000 autoboot-0.9.0/autoboot/process/yaml_parser.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      431 2024-05-11 19:15:15.000000 autoboot-0.9.0/autoboot/server_properties.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-11 20:02:56.531089 autoboot-0.9.0/autoboot/thread/
+-rw-r--r--   0 yizzuide   (501) staff       (20)       70 2023-11-25 09:39:12.000000 autoboot-0.9.0/autoboot/thread/__init__.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1514 2024-05-11 19:15:35.000000 autoboot-0.9.0/autoboot/thread/thread_pool.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-11 20:02:56.533081 autoboot-0.9.0/autoboot/util/
+-rw-r--r--   0 yizzuide   (501) staff       (20)        0 2023-11-16 02:54:04.000000 autoboot-0.9.0/autoboot/util/__init__.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     2712 2023-11-30 02:17:32.000000 autoboot-0.9.0/autoboot/util/capacity.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      302 2023-11-17 07:31:30.000000 autoboot-0.9.0/autoboot/util/json_model.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      560 2023-11-17 06:29:28.000000 autoboot-0.9.0/autoboot/util/local_cache.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      504 2023-11-14 09:04:15.000000 autoboot-0.9.0/autoboot/util/object_navigator.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1092 2023-11-22 07:00:40.000000 autoboot-0.9.0/autoboot/util/type_reflect.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-11 20:02:56.534924 autoboot-0.9.0/autoboot.egg-info/
+-rw-r--r--   0 yizzuide   (501) staff       (20)     8468 2024-05-11 20:02:56.000000 autoboot-0.9.0/autoboot.egg-info/PKG-INFO
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1427 2024-05-11 20:02:56.000000 autoboot-0.9.0/autoboot.egg-info/SOURCES.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)        1 2024-05-11 20:02:56.000000 autoboot-0.9.0/autoboot.egg-info/dependency_links.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)        1 2024-05-11 11:01:58.000000 autoboot-0.9.0/autoboot.egg-info/not-zip-safe
+-rw-r--r--   0 yizzuide   (501) staff       (20)      169 2024-05-11 20:02:56.000000 autoboot-0.9.0/autoboot.egg-info/requires.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)        9 2024-05-11 20:02:56.000000 autoboot-0.9.0/autoboot.egg-info/top_level.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1419 2023-12-12 17:55:45.000000 autoboot-0.9.0/pyproject.toml
+-rw-r--r--   0 yizzuide   (501) staff       (20)      176 2024-05-10 19:55:21.000000 autoboot-0.9.0/requirements.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1013 2024-05-11 20:02:56.536280 autoboot-0.9.0/setup.cfg
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-11 20:02:56.534418 autoboot-0.9.0/tests/
+-rw-r--r--   0 yizzuide   (501) staff       (20)      834 2024-04-07 17:24:15.000000 autoboot-0.9.0/tests/test_event_emitter.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      523 2023-11-20 06:17:50.000000 autoboot-0.9.0/tests/test_json_model.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      137 2023-11-17 06:18:39.000000 autoboot-0.9.0/tests/test_pipy_repo.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      350 2023-11-24 06:20:43.000000 autoboot-0.9.0/tests/test_retry.py
```

### Comparing `autoboot-0.8.0/LICENSE.txt` & `autoboot-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autoboot-0.8.0/PKG-INFO` & `autoboot-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: autoboot
-Version: 0.8.0
+Version: 0.9.0
 Summary: IoC with auto config framework
 Home-page: https://github.com/yizzuide/autoboot
 Author: yizzuide
 Author-email: fu837014586@163.com
 License: MIT
 Keywords: IoC,event,auto config
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: python-dotenv<=2.0,>=1.0.0
-Requires-Dist: filetype<=2.0,>=1.2.0
-Requires-Dist: loguru<=1.0,>=0.7.0
-Requires-Dist: pyyaml<=7.0,>=6.0.1
-Requires-Dist: wrapt<=2.0,>=1.14.1
-Requires-Dist: pydantic<=2.0,>=1.10.12
-Requires-Dist: result<=1.0,>=0.14.0
-Requires-Dist: durations<=1.0,>=0.3.3
+Requires-Dist: python-dotenv<2.0,>=1.0.0
+Requires-Dist: filetype<2.0,>=1.2.0
+Requires-Dist: loguru<1.0,>=0.7.0
+Requires-Dist: pyyaml<7.0,>=6.0.1
+Requires-Dist: wrapt<2.0,>=1.14.1
+Requires-Dist: pydantic<2.0,>=1.10.12
+Requires-Dist: result<1.0,>=0.14.0
+Requires-Dist: durations<1.0,>=0.3.3
 
 # autoboot
 一个Python语言的仿SpringBoot开发方式，支持IoC组件容器、注解式注册、配置驱动开发、事件通知、插件扩展的快速开发框架。
 <p>
   <a href="https://pypi.org/project/autoboot">
       <img src="https://img.shields.io/pypi/v/autoboot?color=%2334D058&label=pypi%20package" alt="Version">
   </a>
```

### Comparing `autoboot-0.8.0/README.md` & `autoboot-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `autoboot-0.8.0/autoboot/annotation/component.py` & `autoboot-0.9.0/autoboot/annotation/component.py`

 * *Files identical despite different names*

### Comparing `autoboot-0.8.0/autoboot/annotation/effect.py` & `autoboot-0.9.0/autoboot/annotation/effect.py`

 * *Files identical despite different names*

### Comparing `autoboot-0.8.0/autoboot/annotation/env.py` & `autoboot-0.9.0/autoboot/annotation/env.py`

 * *Files identical despite different names*

### Comparing `autoboot-0.8.0/autoboot/annotation/log.py` & `autoboot-0.9.0/autoboot/annotation/log.py`

 * *Files identical despite different names*

### Comparing `autoboot-0.8.0/autoboot/application_properties.py` & `autoboot-0.9.0/autoboot/application_properties.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,14 +12,18 @@
   def module() -> str:
     return "api"
   
   @static_property("autoboot.application.scan_listener_packages")
   def scan_listener_packages() -> list[str]:
     pass
   
+  @static_property("autoboot.application.log.level")
+  def log_level() -> str:
+    return "INFO"
+  
   @static_property("autoboot.application.log.dir")
   def log_dir() -> str:
     return "logs"
   
   @static_property("autoboot.application.log.max_size")
   def log_max_size() -> str:
     return "100 MB"
```

### Comparing `autoboot-0.8.0/autoboot/applications.py` & `autoboot-0.9.0/autoboot/applications.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,15 @@
     self._config_data = load_yaml_file(self.config.config_dir, self.config.yml_config)
     
     # config logger
     from autoboot.application_properties import ApplicationProperties
     AutoBoot.logger = Logging(
       app_name=ApplicationProperties.app_name(),
       module=ApplicationProperties.module(),
+      level=ApplicationProperties.log_level(),
       log_dir=ApplicationProperties.log_dir(),
       max_size=ApplicationProperties.log_max_size(),
       retention=ApplicationProperties.log_retention(),
       env_name=env_name
     ).logger
     
     AutoBoot.logger.info(f"application finish load env: {env_name}")
```

### Comparing `autoboot-0.8.0/autoboot/args.py` & `autoboot-0.9.0/autoboot/args.py`

 * *Files identical despite different names*

### Comparing `autoboot-0.8.0/autoboot/event/event_emitter.py` & `autoboot-0.9.0/autoboot/event/event_emitter.py`

 * *Files identical despite different names*

### Comparing `autoboot-0.8.0/autoboot/logging.py` & `autoboot-0.9.0/autoboot/logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,46 +10,50 @@
 LoggingType = TypeVar("LoggingType", bound="Logging")
 
 class Logging:
   """
   Logging class wrapper with loguru.
   """
   
+  # Object memory and allocation optimization
+  __slot__ = ["level", "log_dir", "app_name", "module", "max_size", "retention", "logger"]
+  
   _instance: LoggingType = None
   
-  def __init__(self, log_dir: str, app_name: str, module: str, max_size: str, retention: str, env_name: str):
+  def __init__(self, level: str, log_dir: str, app_name: str, module: str, max_size: str, retention: str, env_name: str):
+    self.level = level
     self.log_dir = log_dir
     self.app_name = app_name
     self.module = module
     self.max_size = max_size
     self.retention = retention
     self.logger = self.console_logger() if env_name == Env.DEV.value else self.file_rotation_logger()
     Logging._instance = self
     
   def console_logger(self) -> loguru.Logger:
     logger.configure(
       handlers=[{
         "sink": sys.stdout,
         "format": "<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green> | <level>{level: <8}</level> | <cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan> - <level>{message}</level>",
-        "level": "DEBUG",
+        "level": self.level,
         "colorize": True,
         "backtrace": True,
       }])
     return logger
     
   def file_rotation_logger(self) -> loguru.Logger:
     log_app_dir = os.path.join(self.log_dir, self.app_name)
     if not os.path.exists(log_app_dir):
       os.makedirs(log_app_dir)
     logger.configure(
       handlers=[{
         "sink": f"{log_app_dir}/{self.module}-{{time:YYYY-MM-DD}}.log",
         "rotation": self.max_size,
         "retention": self.retention,
-        "level": "INFO",
+        "level": self.level,
         "format": "{time:YYYY-MM-DD HH:mm:ss.SSS} | {level: <8} | {name}:{module}:{function}:{line} - {message}",
         "colorize": False,
         "enqueue": True,
         "backtrace": True,
       }])
     return logger
```

### Comparing `autoboot-0.8.0/autoboot/meta/component_metaclass.py` & `autoboot-0.9.0/autoboot/meta/component_metaclass.py`

 * *Files identical despite different names*

### Comparing `autoboot-0.8.0/autoboot/plugin/app_plugin.py` & `autoboot-0.9.0/autoboot/plugin/app_plugin.py`

 * *Files identical despite different names*

### Comparing `autoboot-0.8.0/autoboot/process/__init__.py` & `autoboot-0.9.0/autoboot/process/__init__.py`

 * *Files identical despite different names*

### Comparing `autoboot-0.8.0/autoboot/process/yaml_constructors.py` & `autoboot-0.9.0/autoboot/process/yaml_constructors.py`

 * *Files identical despite different names*

### Comparing `autoboot-0.8.0/autoboot/process/yaml_parser.py` & `autoboot-0.9.0/autoboot/process/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `autoboot-0.8.0/autoboot/thread/thread_pool.py` & `autoboot-0.9.0/autoboot/thread/thread_pool.py`

 * *Files identical despite different names*

### Comparing `autoboot-0.8.0/autoboot/util/capacity.py` & `autoboot-0.9.0/autoboot/util/capacity.py`

 * *Files identical despite different names*

### Comparing `autoboot-0.8.0/autoboot/util/local_cache.py` & `autoboot-0.9.0/autoboot/util/local_cache.py`

 * *Files identical despite different names*

### Comparing `autoboot-0.8.0/autoboot/util/type_reflect.py` & `autoboot-0.9.0/autoboot/util/type_reflect.py`

 * *Files identical despite different names*

### Comparing `autoboot-0.8.0/autoboot.egg-info/PKG-INFO` & `autoboot-0.9.0/autoboot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: autoboot
-Version: 0.8.0
+Version: 0.9.0
 Summary: IoC with auto config framework
 Home-page: https://github.com/yizzuide/autoboot
 Author: yizzuide
 Author-email: fu837014586@163.com
 License: MIT
 Keywords: IoC,event,auto config
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: python-dotenv<=2.0,>=1.0.0
-Requires-Dist: filetype<=2.0,>=1.2.0
-Requires-Dist: loguru<=1.0,>=0.7.0
-Requires-Dist: pyyaml<=7.0,>=6.0.1
-Requires-Dist: wrapt<=2.0,>=1.14.1
-Requires-Dist: pydantic<=2.0,>=1.10.12
-Requires-Dist: result<=1.0,>=0.14.0
-Requires-Dist: durations<=1.0,>=0.3.3
+Requires-Dist: python-dotenv<2.0,>=1.0.0
+Requires-Dist: filetype<2.0,>=1.2.0
+Requires-Dist: loguru<1.0,>=0.7.0
+Requires-Dist: pyyaml<7.0,>=6.0.1
+Requires-Dist: wrapt<2.0,>=1.14.1
+Requires-Dist: pydantic<2.0,>=1.10.12
+Requires-Dist: result<1.0,>=0.14.0
+Requires-Dist: durations<1.0,>=0.3.3
 
 # autoboot
 一个Python语言的仿SpringBoot开发方式，支持IoC组件容器、注解式注册、配置驱动开发、事件通知、插件扩展的快速开发框架。
 <p>
   <a href="https://pypi.org/project/autoboot">
       <img src="https://img.shields.io/pypi/v/autoboot?color=%2334D058&label=pypi%20package" alt="Version">
   </a>
```

### Comparing `autoboot-0.8.0/autoboot.egg-info/SOURCES.txt` & `autoboot-0.9.0/autoboot.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 pyproject.toml
 requirements.txt
 setup.cfg
 autoboot/__init__.py
 autoboot/application_properties.py
 autoboot/applications.py
 autoboot/args.py
+autoboot/autoboot.schema.json
 autoboot/logging.py
 autoboot/server_properties.py
 autoboot.egg-info/PKG-INFO
 autoboot.egg-info/SOURCES.txt
 autoboot.egg-info/dependency_links.txt
 autoboot.egg-info/not-zip-safe
 autoboot.egg-info/requires.txt
```

### Comparing `autoboot-0.8.0/pyproject.toml` & `autoboot-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autoboot-0.8.0/setup.cfg` & `autoboot-0.9.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 packages = find:
 python_requires = >=3.8
 install_requires = file: requirements.txt
 tests_require = 
 	pytest>=6.2.0
 	pytest-cov>=2.10.0
 
+[options.package_data]
+autoboot = 
+	*.json
+
 [options.entry_points]
 console_scripts = 
 executable_name = 
 
 [options.packages.find]
 exclude = 
 	examples*
```

### Comparing `autoboot-0.8.0/tests/test_event_emitter.py` & `autoboot-0.9.0/tests/test_event_emitter.py`

 * *Files identical despite different names*

### Comparing `autoboot-0.8.0/tests/test_json_model.py` & `autoboot-0.9.0/tests/test_json_model.py`

 * *Files identical despite different names*

