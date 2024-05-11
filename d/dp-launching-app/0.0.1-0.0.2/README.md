# Comparing `tmp/dp-launching-app-0.0.1.tar.gz` & `tmp/dp-launching-app-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dp-launching-app-0.0.1.tar", last modified: Tue Apr  9 02:07:07 2024, max compression
+gzip compressed data, was "dp-launching-app-0.0.2.tar", last modified: Sat May 11 03:01:37 2024, max compression
```

## Comparing `dp-launching-app-0.0.1.tar` & `dp-launching-app-0.0.2.tar`

### file list

```diff
@@ -1,50 +1,11 @@
-drwxr-xr-x   0 shanliu    (501) staff       (20)        0 2024-04-09 02:07:07.352613 dp-launching-app-0.0.1/
--rw-r--r--   0 shanliu    (501) staff       (20)       94 2024-04-07 09:36:58.000000 dp-launching-app-0.0.1/MANIFEST.in
--rw-r--r--   0 shanliu    (501) staff       (20)      384 2024-04-09 02:07:07.352169 dp-launching-app-0.0.1/PKG-INFO
--rw-r--r--   0 shanliu    (501) staff       (20)        0 2024-04-07 09:36:58.000000 dp-launching-app-0.0.1/README.md
-drwxr-xr-x   0 shanliu    (501) staff       (20)        0 2024-04-09 02:07:07.341402 dp-launching-app-0.0.1/dp/
--rw-r--r--   0 shanliu    (501) staff       (20)      154 2024-04-07 09:36:58.000000 dp-launching-app-0.0.1/dp/__init__.py
-drwxr-xr-x   0 shanliu    (501) staff       (20)        0 2024-04-09 02:07:07.341856 dp-launching-app-0.0.1/dp/launching/
--rw-r--r--   0 shanliu    (501) staff       (20)       22 2024-04-07 09:36:58.000000 dp-launching-app-0.0.1/dp/launching/__init__.py
-drwxr-xr-x   0 shanliu    (501) staff       (20)        0 2024-04-09 02:07:07.342298 dp-launching-app-0.0.1/dp/launching/cli/
--rw-r--r--   0 shanliu    (501) staff       (20)    12636 2024-04-09 01:57:53.000000 dp-launching-app-0.0.1/dp/launching/cli/__init__.py
-drwxr-xr-x   0 shanliu    (501) staff       (20)        0 2024-04-09 02:07:07.343524 dp-launching-app-0.0.1/dp/launching/cli/api/
--rw-r--r--   0 shanliu    (501) staff       (20)        0 2024-04-07 09:36:58.000000 dp-launching-app-0.0.1/dp/launching/cli/api/__init__.py
--rw-r--r--   0 shanliu    (501) staff       (20)    21712 2024-04-07 09:36:58.000000 dp-launching-app-0.0.1/dp/launching/cli/api/model.py
--rw-r--r--   0 shanliu    (501) staff       (20)     5386 2024-04-08 11:36:52.000000 dp-launching-app-0.0.1/dp/launching/cli/api/persistent_service.py
-drwxr-xr-x   0 shanliu    (501) staff       (20)        0 2024-04-09 02:07:07.344186 dp-launching-app-0.0.1/dp/launching/cli/commands/
--rw-r--r--   0 shanliu    (501) staff       (20)        0 2024-04-07 09:36:58.000000 dp-launching-app-0.0.1/dp/launching/cli/commands/__init__.py
--rw-r--r--   0 shanliu    (501) staff       (20)     1315 2024-04-07 09:36:58.000000 dp-launching-app-0.0.1/dp/launching/cli/commands/launching.py
-drwxr-xr-x   0 shanliu    (501) staff       (20)        0 2024-04-09 02:07:07.339608 dp-launching-app-0.0.1/dp/launching/cli/commands/scaffold/
-drwxr-xr-x   0 shanliu    (501) staff       (20)        0 2024-04-09 02:07:07.344499 dp-launching-app-0.0.1/dp/launching/cli/commands/scaffold/basic/
--rw-r--r--   0 shanliu    (501) staff       (20)     1858 2024-04-07 09:36:58.000000 dp-launching-app-0.0.1/dp/launching/cli/commands/scaffold/basic/basic.py
-drwxr-xr-x   0 shanliu    (501) staff       (20)        0 2024-04-09 02:07:07.344938 dp-launching-app-0.0.1/dp/launching/cli/commands/scaffold/bohrium/
--rw-r--r--   0 shanliu    (501) staff       (20)     2595 2024-04-07 09:36:58.000000 dp-launching-app-0.0.1/dp/launching/cli/commands/scaffold/bohrium/bohrium.py
-drwxr-xr-x   0 shanliu    (501) staff       (20)        0 2024-04-09 02:07:07.345335 dp-launching-app-0.0.1/dp/launching/cli/commands/scaffold/dflow/
--rw-r--r--   0 shanliu    (501) staff       (20)     2606 2024-04-07 09:36:58.000000 dp-launching-app-0.0.1/dp/launching/cli/commands/scaffold/dflow/dflow.py
-drwxr-xr-x   0 shanliu    (501) staff       (20)        0 2024-04-09 02:07:07.346171 dp-launching-app-0.0.1/dp/launching/cli/utils/
--rw-r--r--   0 shanliu    (501) staff       (20)        0 2024-04-07 09:36:58.000000 dp-launching-app-0.0.1/dp/launching/cli/utils/__init__.py
--rw-r--r--   0 shanliu    (501) staff       (20)      147 2024-04-07 09:36:58.000000 dp-launching-app-0.0.1/dp/launching/cli/utils/random.py
-drwxr-xr-x   0 shanliu    (501) staff       (20)        0 2024-04-09 02:07:07.346547 dp-launching-app-0.0.1/dp/launching/report/
--rw-r--r--   0 shanliu    (501) staff       (20)     2940 2024-04-07 09:36:58.000000 dp-launching-app-0.0.1/dp/launching/report/__init__.py
-drwxr-xr-x   0 shanliu    (501) staff       (20)        0 2024-04-09 02:07:07.349249 dp-launching-app-0.0.1/dp/launching/typing/
--rw-r--r--   0 shanliu    (501) staff       (20)      175 2024-04-07 09:36:58.000000 dp-launching-app-0.0.1/dp/launching/typing/__init__.py
-drwxr-xr-x   0 shanliu    (501) staff       (20)        0 2024-04-09 02:07:07.350182 dp-launching-app-0.0.1/dp/launching/typing/addon/
--rw-r--r--   0 shanliu    (501) staff       (20)        0 2024-04-07 09:36:58.000000 dp-launching-app-0.0.1/dp/launching/typing/addon/__init__.py
--rw-r--r--   0 shanliu    (501) staff       (20)      867 2024-04-07 09:36:58.000000 dp-launching-app-0.0.1/dp/launching/typing/addon/sysmbol.py
--rw-r--r--   0 shanliu    (501) staff       (20)     6866 2024-04-07 09:36:58.000000 dp-launching-app-0.0.1/dp/launching/typing/addon/ui.py
--rw-r--r--   0 shanliu    (501) staff       (20)     7114 2024-04-07 09:36:58.000000 dp-launching-app-0.0.1/dp/launching/typing/basic.py
--rw-r--r--   0 shanliu    (501) staff       (20)      749 2024-04-07 09:36:58.000000 dp-launching-app-0.0.1/dp/launching/typing/benchmark.py
--rw-r--r--   0 shanliu    (501) staff       (20)     1774 2024-04-07 09:36:58.000000 dp-launching-app-0.0.1/dp/launching/typing/bio.py
--rw-r--r--   0 shanliu    (501) staff       (20)     9731 2024-04-07 09:36:58.000000 dp-launching-app-0.0.1/dp/launching/typing/bohrium.py
--rw-r--r--   0 shanliu    (501) staff       (20)     4908 2024-04-07 09:36:58.000000 dp-launching-app-0.0.1/dp/launching/typing/dflow.py
--rw-r--r--   0 shanliu    (501) staff       (20)     6371 2024-04-07 09:36:58.000000 dp-launching-app-0.0.1/dp/launching/typing/io.py
-drwxr-xr-x   0 shanliu    (501) staff       (20)        0 2024-04-09 02:07:07.351815 dp-launching-app-0.0.1/dp_launching_app.egg-info/
--rw-r--r--   0 shanliu    (501) staff       (20)      384 2024-04-09 02:07:07.000000 dp-launching-app-0.0.1/dp_launching_app.egg-info/PKG-INFO
--rw-r--r--   0 shanliu    (501) staff       (20)     1092 2024-04-09 02:07:07.000000 dp-launching-app-0.0.1/dp_launching_app.egg-info/SOURCES.txt
--rw-r--r--   0 shanliu    (501) staff       (20)        1 2024-04-09 02:07:07.000000 dp-launching-app-0.0.1/dp_launching_app.egg-info/dependency_links.txt
--rw-r--r--   0 shanliu    (501) staff       (20)       75 2024-04-09 02:07:07.000000 dp-launching-app-0.0.1/dp_launching_app.egg-info/entry_points.txt
--rw-r--r--   0 shanliu    (501) staff       (20)      108 2024-04-09 02:07:07.000000 dp-launching-app-0.0.1/dp_launching_app.egg-info/requires.txt
--rw-r--r--   0 shanliu    (501) staff       (20)        3 2024-04-09 02:07:07.000000 dp-launching-app-0.0.1/dp_launching_app.egg-info/top_level.txt
--rw-r--r--   0 shanliu    (501) staff       (20)       38 2024-04-09 02:07:07.352660 dp-launching-app-0.0.1/setup.cfg
--rw-r--r--   0 shanliu    (501) staff       (20)      714 2024-04-09 02:06:44.000000 dp-launching-app-0.0.1/setup.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-11 03:01:37.110686 dp-launching-app-0.0.2/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      156 2024-05-11 03:01:37.110527 dp-launching-app-0.0.2/PKG-INFO
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      709 2024-05-10 07:03:20.000000 dp-launching-app-0.0.2/README.md
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-11 03:01:37.110312 dp-launching-app-0.0.2/dp_launching_app.egg-info/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      156 2024-05-11 03:01:36.000000 dp-launching-app-0.0.2/dp_launching_app.egg-info/PKG-INFO
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      251 2024-05-11 03:01:37.000000 dp-launching-app-0.0.2/dp_launching_app.egg-info/SOURCES.txt
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)        1 2024-05-11 03:01:36.000000 dp-launching-app-0.0.2/dp_launching_app.egg-info/dependency_links.txt
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)       75 2024-05-11 03:01:36.000000 dp-launching-app-0.0.2/dp_launching_app.egg-info/entry_points.txt
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      108 2024-05-11 03:01:37.000000 dp-launching-app-0.0.2/dp_launching_app.egg-info/requires.txt
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)        1 2024-05-11 03:01:37.000000 dp-launching-app-0.0.2/dp_launching_app.egg-info/top_level.txt
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)       38 2024-05-11 03:01:37.110734 dp-launching-app-0.0.2/setup.cfg
```

