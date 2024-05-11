# Comparing `tmp/plutobook-0.0.11.tar.gz` & `tmp/plutobook-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plutobook-0.0.11.tar", last modified: Fri May 10 21:40:47 2024, max compression
+gzip compressed data, was "plutobook-0.0.9.tar", last modified: Thu May  9 13:24:52 2024, max compression
```

## Comparing `plutobook-0.0.11.tar` & `plutobook-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1962 2024-05-10 21:40:07.000000 plutobook-0.0.11/.github/workflows/main.yml
--rw-r--r--   0        0        0       14 2024-05-10 21:40:07.000000 plutobook-0.0.11/.gitignore
--rw-r--r--   0        0        0     1073 2024-05-10 21:40:07.000000 plutobook-0.0.11/LICENSE
--rw-r--r--   0        0        0       18 2024-05-10 21:40:07.000000 plutobook-0.0.11/README.md
--rw-r--r--   0        0        0      376 2024-05-10 21:40:07.000000 plutobook-0.0.11/meson.build
--rw-r--r--   0        0        0    34337 2024-05-10 21:40:07.000000 plutobook-0.0.11/plutobook-module.c
--rw-r--r--   0        0        0      321 2024-05-10 21:40:07.000000 plutobook-0.0.11/pyproject.toml
--rw-r--r--   0        0        0      124 2024-05-10 21:40:07.000000 plutobook-0.0.11/subprojects/plutobook.wrap
--rw-r--r--   0        0        0      239 2024-05-10 21:40:07.000000 plutobook-0.0.11/windows-build/meson.build
--rw-r--r--   0        0        0      408 2024-05-10 21:40:07.000000 plutobook-0.0.11/windows-build/subprojects/pkgconf.wrap
--rw-r--r--   0        0        0      124 2024-05-10 21:40:07.000000 plutobook-0.0.11/windows-build/subprojects/plutobook.wrap
--rw-r--r--   0        0        0     1473 2024-05-10 21:40:47.268088 plutobook-0.0.11/PKG-INFO
+-rw-r--r--   0        0        0     1962 2024-05-09 13:24:06.000000 plutobook-0.0.9/.github/workflows/main.yml
+-rw-r--r--   0        0        0       14 2024-05-09 13:24:06.000000 plutobook-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1073 2024-05-09 13:24:06.000000 plutobook-0.0.9/LICENSE
+-rw-r--r--   0        0        0       18 2024-05-09 13:24:06.000000 plutobook-0.0.9/README.md
+-rw-r--r--   0        0        0      347 2024-05-09 13:24:06.000000 plutobook-0.0.9/meson.build
+-rw-r--r--   0        0        0    34337 2024-05-09 13:24:06.000000 plutobook-0.0.9/plutobook-module.c
+-rw-r--r--   0        0        0      320 2024-05-09 13:24:06.000000 plutobook-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      124 2024-05-09 13:24:06.000000 plutobook-0.0.9/subprojects/plutobook.wrap
+-rw-r--r--   0        0        0      205 2024-05-09 13:24:06.000000 plutobook-0.0.9/windows-build/meson.build
+-rw-r--r--   0        0        0      408 2024-05-09 13:24:06.000000 plutobook-0.0.9/windows-build/subprojects/pkgconf.wrap
+-rw-r--r--   0        0        0      124 2024-05-09 13:24:06.000000 plutobook-0.0.9/windows-build/subprojects/plutobook.wrap
+-rw-r--r--   0        0        0     1472 2024-05-09 13:24:52.605115 plutobook-0.0.9/PKG-INFO
```

### Comparing `plutobook-0.0.11/.github/workflows/main.yml` & `plutobook-0.0.9/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `plutobook-0.0.11/LICENSE` & `plutobook-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `plutobook-0.0.11/plutobook-module.c` & `plutobook-0.0.9/plutobook-module.c`

 * *Files identical despite different names*

### Comparing `plutobook-0.0.11/PKG-INFO` & `plutobook-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plutobook
-Version: 0.0.11
+Version: 0.0.9
 Summary: Paged HTML rendering library
 Author-Email: Samuel Ugochukwu <sammycageagle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Samuel Ugochukwu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

