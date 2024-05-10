# Comparing `tmp/matadi-0.1.9.tar.gz` & `tmp/matadi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matadi-0.1.9.tar", last modified: Sun Aug 14 22:36:21 2022, max compression
+gzip compressed data, was "matadi-0.2.0.tar", last modified: Fri May 10 22:49:41 2024, max compression
```

## Comparing `matadi-0.1.9.tar` & `matadi-0.2.0.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 22:36:21.782534 matadi-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (121)    35141 2022-08-14 22:36:13.000000 matadi-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    60192 2022-08-14 22:36:21.782534 matadi-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    18234 2022-08-14 22:36:13.000000 matadi-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 22:36:21.778534 matadi-0.1.9/matadi/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/__about__.py
--rw-r--r--   0 runner    (1001) docker     (121)      788 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/_apply.py
--rw-r--r--   0 runner    (1001) docker     (121)    11132 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/_lab_compressible.py
--rw-r--r--   0 runner    (1001) docker     (121)     7941 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/_lab_incompressible.py
--rw-r--r--   0 runner    (1001) docker     (121)     8804 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/_material.py
--rw-r--r--   0 runner    (1001) docker     (121)     6800 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/_templates.py
--rw-r--r--   0 runner    (1001) docker     (121)     2918 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/math.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 22:36:21.778534 matadi-0.1.9/matadi/models/
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/models/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1724 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/models/_hyperelasticity_anisotropic.py
--rw-r--r--   0 runner    (1001) docker     (121)     2577 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/models/_hyperelasticity_isotropic.py
--rw-r--r--   0 runner    (1001) docker     (121)     1969 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/models/_misc.py
--rw-r--r--   0 runner    (1001) docker     (121)      513 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/models/_pseudo_elasticity.py
--rw-r--r--   0 runner    (1001) docker     (121)     2382 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/models/_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 22:36:21.778534 matadi-0.1.9/matadi/models/microsphere/
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/models/microsphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1285 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/models/microsphere/_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 22:36:21.778534 matadi-0.1.9/matadi/models/microsphere/affine/
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/models/microsphere/affine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2014 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/models/microsphere/affine/_models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 22:36:21.778534 matadi-0.1.9/matadi/models/microsphere/nonaffine/
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/models/microsphere/nonaffine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1559 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/models/microsphere/nonaffine/_models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 22:36:21.778534 matadi-0.1.9/matadi/models/microsphere/quadrature/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/models/microsphere/quadrature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1766 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/models/microsphere/quadrature/_bazant_oh.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 22:36:21.778534 matadi-0.1.9/matadi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    60192 2022-08-14 22:36:21.000000 matadi-0.1.9/matadi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1209 2022-08-14 22:36:21.000000 matadi-0.1.9/matadi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-14 22:36:21.000000 matadi-0.1.9/matadi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-08-14 22:36:21.000000 matadi-0.1.9/matadi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-08-14 22:36:21.000000 matadi-0.1.9/matadi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1529 2022-08-14 22:36:13.000000 matadi-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1194 2022-08-14 22:36:21.782534 matadi-0.1.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 22:36:21.782534 matadi-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-14 22:36:13.000000 matadi-0.1.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3476 2022-08-14 22:36:13.000000 matadi-0.1.9/tests/test_displacement-pressure.py
--rw-r--r--   0 runner    (1001) docker     (121)     2658 2022-08-14 22:36:13.000000 matadi-0.1.9/tests/test_eigvals_grad.py
--rw-r--r--   0 runner    (1001) docker     (121)     1913 2022-08-14 22:36:13.000000 matadi-0.1.9/tests/test_fiber.py
--rw-r--r--   0 runner    (1001) docker     (121)     3567 2022-08-14 22:36:13.000000 matadi-0.1.9/tests/test_lab.py
--rw-r--r--   0 runner    (1001) docker     (121)     1097 2022-08-14 22:36:13.000000 matadi-0.1.9/tests/test_microsphere.py
--rw-r--r--   0 runner    (1001) docker     (121)     6690 2022-08-14 22:36:13.000000 matadi-0.1.9/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     3375 2022-08-14 22:36:13.000000 matadi-0.1.9/tests/test_plane.py
--rw-r--r--   0 runner    (1001) docker     (121)     3124 2022-08-14 22:36:13.000000 matadi-0.1.9/tests/test_scalar.py
--rw-r--r--   0 runner    (1001) docker     (121)     3933 2022-08-14 22:36:13.000000 matadi-0.1.9/tests/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (121)      697 2022-08-14 22:36:13.000000 matadi-0.1.9/tests/test_template-materials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:49:41.281592 matadi-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35140 2024-05-10 22:49:37.000000 matadi-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    61802 2024-05-10 22:49:41.281592 matadi-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19872 2024-05-10 22:49:37.000000 matadi-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-10 22:49:37.000000 matadi-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 22:49:41.281592 matadi-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:49:41.269592 matadi-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:49:41.273592 matadi-0.2.0/src/matadi/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 22:49:37.000000 matadi-0.2.0/src/matadi/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-10 22:49:37.000000 matadi-0.2.0/src/matadi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-10 22:49:37.000000 matadi-0.2.0/src/matadi/_apply.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11196 2024-05-10 22:49:37.000000 matadi-0.2.0/src/matadi/_lab_compressible.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7973 2024-05-10 22:49:37.000000 matadi-0.2.0/src/matadi/_lab_incompressible.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8791 2024-05-10 22:49:37.000000 matadi-0.2.0/src/matadi/_material.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-05-10 22:49:37.000000 matadi-0.2.0/src/matadi/_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-10 22:49:37.000000 matadi-0.2.0/src/matadi/_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-05-10 22:49:37.000000 matadi-0.2.0/src/matadi/math.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:49:41.277592 matadi-0.2.0/src/matadi/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-10 22:49:37.000000 matadi-0.2.0/src/matadi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-10 22:49:37.000000 matadi-0.2.0/src/matadi/models/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-10 22:49:37.000000 matadi-0.2.0/src/matadi/models/_hyperelasticity_anisotropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-10 22:49:37.000000 matadi-0.2.0/src/matadi/models/_hyperelasticity_isotropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-10 22:49:37.000000 matadi-0.2.0/src/matadi/models/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-10 22:49:37.000000 matadi-0.2.0/src/matadi/models/_pseudo_elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-10 22:49:37.000000 matadi-0.2.0/src/matadi/models/_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-10 22:49:37.000000 matadi-0.2.0/src/matadi/models/_viscoelasticity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:49:41.277592 matadi-0.2.0/src/matadi/models/microsphere/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-10 22:49:37.000000 matadi-0.2.0/src/matadi/models/microsphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-10 22:49:37.000000 matadi-0.2.0/src/matadi/models/microsphere/_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:49:41.277592 matadi-0.2.0/src/matadi/models/microsphere/affine/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-10 22:49:37.000000 matadi-0.2.0/src/matadi/models/microsphere/affine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-10 22:49:37.000000 matadi-0.2.0/src/matadi/models/microsphere/affine/_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:49:41.277592 matadi-0.2.0/src/matadi/models/microsphere/nonaffine/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-10 22:49:37.000000 matadi-0.2.0/src/matadi/models/microsphere/nonaffine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-10 22:49:37.000000 matadi-0.2.0/src/matadi/models/microsphere/nonaffine/_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:49:41.277592 matadi-0.2.0/src/matadi/models/microsphere/quadrature/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-10 22:49:37.000000 matadi-0.2.0/src/matadi/models/microsphere/quadrature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-10 22:49:37.000000 matadi-0.2.0/src/matadi/models/microsphere/quadrature/_bazant_oh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:49:41.281592 matadi-0.2.0/src/matadi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    61802 2024-05-10 22:49:41.000000 matadi-0.2.0/src/matadi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-10 22:49:41.000000 matadi-0.2.0/src/matadi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 22:49:41.000000 matadi-0.2.0/src/matadi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-10 22:49:41.000000 matadi-0.2.0/src/matadi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 22:49:41.000000 matadi-0.2.0/src/matadi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:49:41.281592 matadi-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-10 22:49:37.000000 matadi-0.2.0/tests/test_displacement-pressure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-10 22:49:37.000000 matadi-0.2.0/tests/test_eigvals_grad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-10 22:49:37.000000 matadi-0.2.0/tests/test_fiber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-10 22:49:37.000000 matadi-0.2.0/tests/test_lab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-10 22:49:37.000000 matadi-0.2.0/tests/test_microsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-05-10 22:49:37.000000 matadi-0.2.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-05-10 22:49:37.000000 matadi-0.2.0/tests/test_plane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-10 22:49:37.000000 matadi-0.2.0/tests/test_scalar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-10 22:49:37.000000 matadi-0.2.0/tests/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-10 22:49:37.000000 matadi-0.2.0/tests/test_template-materials.py
```

### Comparing `matadi-0.1.9/LICENSE` & `matadi-0.2.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -628,15 +628,15 @@
 
   To do so, attach the following notices to the program.  It is safest
 to attach them to the start of each source file to most effectively
 state the exclusion of warranty; and each file should have at least
 the "copyright" line and a pointer to where the full notice is found.
 
     <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) 2021  <name of author>
+    Copyright (C) 2023  Andreas Dutzler
 
     This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
     This program is distributed in the hope that it will be useful,
@@ -648,15 +648,15 @@
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 Also add information on how to contact you by electronic and paper mail.
 
   If the program does terminal interaction, make it output a short
 notice like this when it starts in an interactive mode:
 
-    matadi  Copyright (C) 2021  Andreas Dutzler
+    matadi  Copyright (C) 2023  Andreas Dutzler
     This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
     This is free software, and you are welcome to redistribute it
     under certain conditions; type `show c' for details.
 
 The hypothetical commands `show w' and `show c' should show the appropriate
 parts of the General Public License.  Of course, your program's commands
 might be different; for a GUI interface, you would use an "about box".
```

### Comparing `matadi-0.1.9/PKG-INFO` & `matadi-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: matadi
-Version: 0.1.9
+Version: 0.2.0
 Summary: Material Definition with Automatic Differentiation
-Home-page: https://github.com/adtzlr/matadi
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -635,15 +634,15 @@
         
           To do so, attach the following notices to the program.  It is safest
         to attach them to the start of each source file to most effectively
         state the exclusion of warranty; and each file should have at least
         the "copyright" line and a pointer to where the full notice is found.
         
             <one line to give the program's name and a brief idea of what it does.>
-            Copyright (C) 2021  <name of author>
+            Copyright (C) 2023  Andreas Dutzler
         
             This program is free software: you can redistribute it and/or modify
             it under the terms of the GNU General Public License as published by
             the Free Software Foundation, either version 3 of the License, or
             (at your option) any later version.
         
             This program is distributed in the hope that it will be useful,
@@ -655,15 +654,15 @@
             along with this program.  If not, see <https://www.gnu.org/licenses/>.
         
         Also add information on how to contact you by electronic and paper mail.
         
           If the program does terminal interaction, make it output a short
         notice like this when it starts in an interactive mode:
         
-            matadi  Copyright (C) 2021  Andreas Dutzler
+            matadi  Copyright (C) 2023  Andreas Dutzler
             This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
             This is free software, and you are welcome to redistribute it
             under certain conditions; type `show c' for details.
         
         The hypothetical commands `show w' and `show c' should show the appropriate
         parts of the General Public License.  Of course, your program's commands
         might be different; for a GUI interface, you would use an "about box".
@@ -676,46 +675,48 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
-Project-URL: homepage, https://github.com/adtzlr/matadi
-Project-URL: code, https://github.com/adtzlr/matadi
-Project-URL: issues, https://github.com/adtzlr/matadi/issues
+Project-URL: Code, https://github.com/adtzlr/matadi
+Project-URL: Issues, https://github.com/adtzlr/matadi/issues
 Keywords: python,constitution,automatic-differentiation,scientific-computing,fem,finite-elements-analysis,algorithmic-differentiation,hyperelasticity,constitutive-model
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: all
 License-File: LICENSE
+Requires-Dist: casadi
+Requires-Dist: numpy
+Provides-Extra: all
+Requires-Dist: matplotlib; extra == "all"
+Requires-Dist: scipy; extra == "all"
 
-# matADi
-Material Definition with Automatic Differentiation (AD)
-
-![matADi](https://raw.githubusercontent.com/adtzlr/matadi/main/docs/logo/matadi-logo.svg)
+<p align="center">
+  <img src="https://user-images.githubusercontent.com/5793153/235784656-c77d705d-7b4e-4310-bf6e-feb1f1569dce.png" height="80px"/>
+  <p align="center">Material Definition with Automatic Differentiation.</p>
+</p>
 
 [![PyPI version shields.io](https://img.shields.io/pypi/v/matadi.svg)](https://pypi.python.org/pypi/matadi/) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/matadi/branch/main/graph/badge.svg?token=2EY2U4ZL35)](https://codecov.io/gh/adtzlr/matadi) [![DOI](https://zenodo.org/badge/408564756.svg)](https://zenodo.org/badge/latestdoi/408564756) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black) ![GitHub Repo stars](https://img.shields.io/github/stars/adtzlr/matadi?logo=github) ![PyPI - Downloads](https://img.shields.io/pypi/dm/matadi)
 
-matADi is a Python module for the definition of a constitutive hyperelastic material formulation by a strain energy density function. Both [gradient](https://en.wikipedia.org/wiki/Gradient) (stress) and [hessian](https://en.wikipedia.org/wiki/Hessian_matrix) (elasticity tensor) are carried out by [**Automatic Differentiation (AD)**](https://en.wikipedia.org/wiki/Automatic_differentiation) using [casADi](https://web.casadi.org/) [[1](https://doi.org/10.1007/s12532-018-0139-4)] as a backend. A high-level interface for hyperelastic materials based on the deformation gradient exists. Several isotropic hyperelastic material formulations like the Neo-Hookean or the Ogden model are included in the model library. Gradient and hessian methods allow input data with trailing axes which is especially useful for Python-based finite element modules, e.g. [scikit-fem](https://scikit-fem.readthedocs.io/en/latest/) or [FElupe](https://github.com/adtzlr/felupe). Mixed-field formulations suitable for nearly-incompressible material behavior are supported as well as single-field formulations based on the deformation gradient. A numerical lab is included to run, plot and analyze homogenous uniaxial, equi-biaxial, planar shear and simple shear load cases.
+matADi is a 3.8+ Python package for the definition of a constitutive hyperelastic material formulation by a strain energy density function. Both [gradient](https://en.wikipedia.org/wiki/Gradient) (stress) and [hessian](https://en.wikipedia.org/wiki/Hessian_matrix) (elasticity tensor) are carried out by [**Automatic Differentiation (AD)**](https://en.wikipedia.org/wiki/Automatic_differentiation) using [casADi](https://web.casadi.org/) [[1](https://doi.org/10.1007/s12532-018-0139-4)] as a backend. A high-level interface for hyperelastic materials based on the deformation gradient exists. Several isotropic hyperelastic material formulations like the Neo-Hookean or the Ogden model are included in the model library. Gradient and hessian methods allow input data with trailing axes which is especially useful for Python-based finite element modules, e.g. [scikit-fem](https://scikit-fem.readthedocs.io/en/latest/) or [FElupe](https://github.com/adtzlr/felupe). Mixed-field formulations suitable for nearly-incompressible material behavior are supported as well as single-field formulations based on the deformation gradient. A numerical lab is included to run, plot and analyze homogeneous uniaxial, equi-biaxial, planar shear and simple shear load cases.
 
 ## Installation
 Install `matADi` from PyPI via pip.
 
 ```shell
 pip install matadi
 ```
@@ -805,64 +806,64 @@
 W_upJ = NH_upJ.function([defgrad, pressure, volratio])
 P_upJ = NH_upJ.gradient([defgrad, pressure, volratio])
 A_upJ = NH_upJ.hessian([defgrad, pressure, volratio])
 ```
 
 The output of `NH_upJ.gradient([defgrad, pressure, volratio])` is a list with gradients of the functional as `[dWdF, dWdp, dWdJ]`. Hessian entries are provided as a list of upper triangle entries, e.g. `NH_upJ.hessian([defgrad, pressure, volratio])` returns `[d2WdFdF, d2WdFdp, d2WdFdJ, d2Wdpdp, d2WdpdJ, d2WdJdJ]`.
 
-Available [isotropic hyperelastic material models](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py):
-- [Linear Elastic](https://en.wikipedia.org/wiki/Linear_elasticity) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py#L5-L7))
-- [Saint Venant Kirchhoff](https://en.wikipedia.org/wiki/Hyperelastic_material#Saint_Venant%E2%80%93Kirchhoff_model) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py#L10-L14))
-- [Neo-Hooke](https://en.wikipedia.org/wiki/Neo-Hookean_solid) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py#L17-L21))
-- [Mooney-Rivlin](https://en.wikipedia.org/wiki/Mooney%E2%80%93Rivlin_solid) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py#L24-L29))
-- [Yeoh](https://en.wikipedia.org/wiki/Yeoh_(hyperelastic_model)) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py#L32-L37))
-- [Third-Order-Deformation (James-Green-Simpson)](https://onlinelibrary.wiley.com/doi/abs/10.1002/app.1975.070190723) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py#L40-L51))
-- [Ogden](https://en.wikipedia.org/wiki/Ogden_(hyperelastic_model)) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py#L54-L64))
-- [Arruda-Boyce](https://en.wikipedia.org/wiki/Arruda%E2%80%93Boyce_model) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py#L67-L80))
-- [Extended-Tube](https://meridian.allenpress.com/rct/article-abstract/72/4/602/92819/An-Extended-Tube-Model-for-Rubber-Elasticity?redirectedFrom=fulltext) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py#L83-L91))
-- [Van-der-Waals (Kilian)](https://doi.org/10.1016/0032-3861(81)90200-7) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py#L94-L103))
-
-Available [anisotropic hyperelastic material models](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_anisotropic.py):
-- Fiber ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_anisotropic.py#L17-L35))
-- Fiber-family (+/- combination of single Fiber) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_anisotropic.py#L38-L45))
-- [Holzapfel Gasser Ogden](https://royalsocietypublishing.org/doi/full/10.1098/rsif.2005.0073) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_anisotropic.py#L48-L77))
-
-Available [micro-sphere hyperelastic frameworks](https://github.com/adtzlr/matadi/blob/main/matadi/models/microsphere) (Miehe, Göktepe, Lulei) [[2](https://doi.org/10.1016/j.jmps.2004.03.011)]:
-- [affine stretch](https://doi.org/10.1016/j.jmps.2004.03.011) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/microsphere/affine/_models.py#L6-L16))
-- [affine tube](https://doi.org/10.1016/j.jmps.2004.03.011) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/microsphere/affine/_models.py#L19-L30))
-- [non-affine stretch](https://doi.org/10.1016/j.jmps.2004.03.011) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/microsphere/nonaffine/_models.py#L7-L17))
-- [non-affine tube](https://doi.org/10.1016/j.jmps.2004.03.011) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/microsphere/nonaffine/_models.py#L20-L32))
+Available [isotropic hyperelastic material models](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py):
+- [Linear Elastic](https://en.wikipedia.org/wiki/Linear_elasticity) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py#L5-L7))
+- [Saint Venant Kirchhoff](https://en.wikipedia.org/wiki/Hyperelastic_material#Saint_Venant%E2%80%93Kirchhoff_model) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py#L10-L14))
+- [Neo-Hooke](https://en.wikipedia.org/wiki/Neo-Hookean_solid) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py#L17-L21))
+- [Mooney-Rivlin](https://en.wikipedia.org/wiki/Mooney%E2%80%93Rivlin_solid) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py#L24-L29))
+- [Yeoh](https://en.wikipedia.org/wiki/Yeoh_(hyperelastic_model)) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py#L32-L37))
+- [Third-Order-Deformation (James-Green-Simpson)](https://onlinelibrary.wiley.com/doi/abs/10.1002/app.1975.070190723) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py#L40-L51))
+- [Ogden](https://en.wikipedia.org/wiki/Ogden_(hyperelastic_model)) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py#L54-L64))
+- [Arruda-Boyce](https://en.wikipedia.org/wiki/Arruda%E2%80%93Boyce_model) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py#L67-L80))
+- [Extended-Tube](https://meridian.allenpress.com/rct/article-abstract/72/4/602/92819/An-Extended-Tube-Model-for-Rubber-Elasticity?redirectedFrom=fulltext) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py#L83-L91))
+- [Van-der-Waals (Kilian)](https://doi.org/10.1016/0032-3861(81)90200-7) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py#L94-L103))
+
+Available [anisotropic hyperelastic material models](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_anisotropic.py):
+- Fiber ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_anisotropic.py#L17-L35))
+- Fiber-family (+/- combination of single Fiber) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_anisotropic.py#L38-L45))
+- [Holzapfel Gasser Ogden](https://royalsocietypublishing.org/doi/full/10.1098/rsif.2005.0073) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_anisotropic.py#L48-L77))
+
+Available [micro-sphere hyperelastic frameworks](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/microsphere) (Miehe, Göktepe, Lulei) [[2](https://doi.org/10.1016/j.jmps.2004.03.011)]:
+- [affine stretch](https://doi.org/10.1016/j.jmps.2004.03.011) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/microsphere/affine/_models.py#L6-L16))
+- [affine tube](https://doi.org/10.1016/j.jmps.2004.03.011) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/microsphere/affine/_models.py#L19-L30))
+- [non-affine stretch](https://doi.org/10.1016/j.jmps.2004.03.011) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/microsphere/nonaffine/_models.py#L7-L17))
+- [non-affine tube](https://doi.org/10.1016/j.jmps.2004.03.011) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/microsphere/nonaffine/_models.py#L20-L32))
 
-Available [micro-sphere hyperelastic material models](https://github.com/adtzlr/matadi/blob/main/matadi/models/microsphere) (Miehe, Göktepe, Lulei) [[2](https://doi.org/10.1016/j.jmps.2004.03.011)]:
-- [Miehe Göktepe Lulei](https://doi.org/10.1016/j.jmps.2004.03.011) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/microsphere/nonaffine/_models.py#L35-L49))
+Available [micro-sphere hyperelastic material models](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/microsphere) (Miehe, Göktepe, Lulei) [[2](https://doi.org/10.1016/j.jmps.2004.03.011)]:
+- [Miehe Göktepe Lulei](https://doi.org/10.1016/j.jmps.2004.03.011) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/microsphere/nonaffine/_models.py#L35-L49))
 
 Any user-defined isotropic hyperelastic strain energy density function may be passed as the `fun` argument of `MaterialHyperelastic` by using the following template:
 
 ```python
 def fun(F, **kwargs):
     # user code
     return W
 ```
 
-In order to apply the above material model only on the isochoric part of the deformation gradient [[3](https://doi.org/10.1016/0045-7825(85)90033-7)], use the decorator [`@isochoric_volumetric_split`](https://github.com/adtzlr/matadi/blob/main/matadi/models/_helpers.py#L7-L31). If the keyword `bulk` is passed, an additional [volumetric strain energy function](https://github.com/adtzlr/matadi/blob/main/matadi/models/_helpers.py#L34-L35) is added to the base material formulation.
+In order to apply the above material model only on the isochoric part of the deformation gradient [[3](https://doi.org/10.1016/0045-7825(85)90033-7)], use the decorator [`@isochoric_volumetric_split`](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_helpers.py#L7-L31). If the keyword `bulk` is passed, an additional [volumetric strain energy function](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_helpers.py#L34-L35) is added to the base material formulation.
 
 ```python
 from matadi.models import isochoric_volumetric_split
 from matadi.math import trace, transpose
 
 @isochoric_volumetric_split
 def nh(F, C10=0.5):
     # user code of strain energy function, e.g. neo-hooke
     return C10 * (trace(transpose(F) @ F) - 3)
 
 NH = MaterialHyperelastic(nh, C10=0.5, bulk=200.0)
 ```
 
 ## Lab
-In matADi's `Lab` :lab_coat: numeric experiments on homogenous loadcases on compressible or nearly-incompressible material formulations are performed. For incompressible materials use `LabIncompressible` instead. Let's take the non-affine micro-sphere material model suitable for rubber elasticity with parameters from [[2](https://doi.org/10.1016/j.jmps.2004.03.011), Fig. 19] and run **uniaxial**, **biaxial** and **planar shear** tests.
+In matADi's `Lab` :lab_coat: numeric experiments on homogeneous loadcases on compressible or nearly-incompressible material formulations are performed. For incompressible materials use `LabIncompressible` instead. Let's take the non-affine micro-sphere material model suitable for rubber elasticity with parameters from [[2](https://doi.org/10.1016/j.jmps.2004.03.011), Fig. 19] and run **uniaxial**, **biaxial** and **planar shear** tests.
 
 ```python
 from matadi import Lab, MaterialHyperelastic
 from matadi.models import miehe_goektepe_lulei
 
 mat = MaterialHyperelastic(
     miehe_goektepe_lulei, 
@@ -897,21 +898,26 @@
 b) the monotonic increasing slope of force per undeformed area vs. stretch and
 c) the sign of the resulting stretch from a small superposed force in one direction.
 
 ## Hints and usage in FEM modules
 For tensor-valued material definitions use `MaterialTensor` (e.g. any stress-strain relation). Also, please have a look at [casADi's documentation](https://web.casadi.org/). It is very powerful but unfortunately does not support all the Python stuff you would expect. For example Python's default if-else-statements can't be used in combination with symbolic conditions (use `math.if_else(cond, if_true, if_false)` instead). Contrary to [casADi](https://web.casadi.org/), the gradient of the eigenvalue function is stabilized by a perturbation of the diagonal components.
 
 ### A **Material** with state variables
-A generalized material model with optional state variables for the (u/p)-formulation is created by an instance of `MaterialTensor`. If the argument `triu` is set to `True` the gradient method returns only the upper triangle entries of the gradient components. If some of the input variables are internal state variables the number of these variables have to be passed to the optional argument `statevars`. While the hyperelastic material classes are defined by a strain energy function, this one is defined by the first Piola-Kirchhoff stress tensor. Internally, state variables are equal to default variables but they are excluded from gradient calculations. State variables may also be used as placeholders for additional quantities, e.g. the initial deformation gradient at the beginning of an increment or the time increment. Hence, it is a very flexible class not restricted to hyperelasticity.
+A generalized material model with optional state variables, optionally for the (u/p)-formulation, is created by an instance of `MaterialTensor`. If the argument `triu` is set to `True` the gradient method returns only the upper triangle entries of the gradient components. If some of the input variables are internal state variables the number of these variables have to be passed to the optional argument `statevars`. While the hyperelastic material classes are defined by a strain energy function, this one is defined by the first Piola-Kirchhoff stress tensor. Internally, state variables are equal to default variables but they are excluded from gradient calculations. State variables may also be used as placeholders for additional quantities, e.g. the initial deformation gradient at the beginning of an increment or the time increment. Hence, it is a very flexible class not restricted to hyperelasticity. For consistency, the methods `gradient` and `hessian` of a tensor-based material refer to the gradient and hessian of the strain energy function.
+
+Included [pseudo-elastic material models](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_pseudo_elasticity.py):
+- [Ogden-Roxburgh](https://doi.org/10.1098%2Frspa.1999.0431) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_pseudo_elasticity.py#L4-L16))
 
-Included [pseudo-elastic material models](https://github.com/adtzlr/matadi/blob/main/matadi/models/_pseudo_elasticity.py):
-- [Ogden-Roxburgh](https://doi.org/10.1098%2Frspa.1999.0431) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_pseudo_elasticity.py#L4-L16))
 
-Included [other material models](https://github.com/adtzlr/matadi/blob/main/matadi/models/_misc.py):
-- [MORPH](https://doi.org/10.1016/S0749-6419(02)00091-8) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_misc.py#L19-L75))
+Included [viscoelastic material models](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_viscoelasticity.py):
+- [Finite-Strain-Viscoelastic](https://doi.org/10.1016/j.cma.2013.07.004) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_viscoelasticity.py#L4-L18))
+- [Finite-Strain-Viscoelastic (Mooney-Rivlin)](https://doi.org/10.1002/nme.5724) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_viscoelasticity.py#L21-L51))
+
+Included [other material models](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_misc.py):
+- [MORPH](https://doi.org/10.1016/S0749-6419(02)00091-8) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_misc.py#L19-L75))
 
 ```python
 import numpy as np
 
 from matadi.models import (
     displacement_pressure_split, neo_hooke, volumetric, ogden_roxburgh
 )
@@ -950,22 +956,30 @@
 defgrad = np.random.rand(3, 3, 5, 100) - 0.5
 pressure = np.random.rand(1, 5, 100)
 statevars = np.random.rand(1, 1, 5, 100)
 
 for a in range(3):
     defgrad[a, a] += 1.0
 
-dWdF, dWdp, statevars_new = NH.function([defgrad, pressure, statevars])
-d2WdFdF, d2WdFdp, d2Wdpdp = NH.gradient([defgrad, pressure, statevars])
+dWdF, dWdp, statevars_new = NH.gradient([defgrad, pressure, statevars])
+d2WdFdF, d2WdFdp, d2Wdpdp = NH.hessian([defgrad, pressure, statevars])
 ```
 
-**Hint**: *The above Neo-Hooke as well as the MORPH material model formulation within the u/p-framework are available as template-materials in `matadi.models` as `NeoHookeOgdenRoxburgh()`and `Morph()`. The state variable concept is also implemented for the `Material` class.*
+The Neo-Hooke, the MORPH and the Finite-Strain-Viscoelastic [[4](https://doi.org/10.1016/j.cma.2013.07.004)] material model formulations are available as ready-to-go materials in `matadi.models` as:
+
+* [`NeoHookeOgdenRoxburgh()`](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_templates.py), 
+* [`Morph()`](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_templates.py),
+* [`Viscoelastic()`](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_templates.py) and
+* [`ViscoelasticMooneyRivlin()`](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_templates.py).
+
+**Hint**: *The state variable concept is also implemented for the `Material` class.*
 
 Simple examples for using `matadi` with [`scikit-fem`](https://github.com/adtzlr/matadi/discussions/14#) as well as with [`felupe`](https://github.com/adtzlr/matadi/discussions/22) are shown in the Discussion section.
 
 ## References
 [1] J. A. E. Andersson, J. Gillis, G. Horn, J. B. Rawlings, and M. Diehl, *CasADi - A software framework for nonlinear optimization and optimal control*, Math. Prog. Comp., vol. 11, no. 1, pp. 1–36, 2019, [![DOI:10.1007/s12532-018-0139-4](https://zenodo.org/badge/DOI/10.1007/s12532-018-0139-4.svg)](https://doi.org/10.1007/s12532-018-0139-4)
 
 [2] C. Miehe, S. Göktepe and F. Lulei, *A micro-macro approach to rubber-like materials. Part I: the non-affine micro-sphere model of rubber elasticity*, Journal of the Mechanics and Physics of Solids, vol. 52, no. 11. Elsevier BV, pp. 2617–2660, Nov. 2004. [![DOI:10.1016/j.jmps.2004.03.011](https://zenodo.org/badge/DOI/10.1016/j.jmps.2004.03.011.svg)](https://doi.org/10.1016/j.jmps.2004.03.011)
 
 [3] J. C. Simo, R. L. Taylor, and K. S. Pister, *Variational and projection methods for the volume constraint in finite deformation elasto-plasticity*, Computer Methods in Applied Mechanics and Engineering, vol. 51, no. 1–3, pp. 177–208, Sep. 1985, [![DOI:10.1016/0045-7825(85)90033-7](https://zenodo.org/badge/DOI/10.1016/0045-7825(85)90033-7.svg)](https://doi.org/10.1016/0045-7825(85)90033-7)
 
+[4] A. V. Shutov, R. Landgraf, and J. Ihlemann, *An explicit solution for implicit time stepping in multiplicative finite strain viscoelasticity*, Computer Methods in Applied Mechanics and Engineering, vol. 265. Elsevier BV, pp. 213–225, Oct. 2013, [![DOI:10.1016/j.cma.2013.07.004](https://zenodo.org/badge/DOI/10.1016/j.cma.2013.07.004.svg)](https://doi.org/10.1016/j.cma.2013.07.004)
```

### Comparing `matadi-0.1.9/README.md` & `matadi-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# matADi
-Material Definition with Automatic Differentiation (AD)
-
-![matADi](https://raw.githubusercontent.com/adtzlr/matadi/main/docs/logo/matadi-logo.svg)
+<p align="center">
+  <img src="https://user-images.githubusercontent.com/5793153/235784656-c77d705d-7b4e-4310-bf6e-feb1f1569dce.png" height="80px"/>
+  <p align="center">Material Definition with Automatic Differentiation.</p>
+</p>
 
 [![PyPI version shields.io](https://img.shields.io/pypi/v/matadi.svg)](https://pypi.python.org/pypi/matadi/) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/matadi/branch/main/graph/badge.svg?token=2EY2U4ZL35)](https://codecov.io/gh/adtzlr/matadi) [![DOI](https://zenodo.org/badge/408564756.svg)](https://zenodo.org/badge/latestdoi/408564756) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black) ![GitHub Repo stars](https://img.shields.io/github/stars/adtzlr/matadi?logo=github) ![PyPI - Downloads](https://img.shields.io/pypi/dm/matadi)
 
-matADi is a Python module for the definition of a constitutive hyperelastic material formulation by a strain energy density function. Both [gradient](https://en.wikipedia.org/wiki/Gradient) (stress) and [hessian](https://en.wikipedia.org/wiki/Hessian_matrix) (elasticity tensor) are carried out by [**Automatic Differentiation (AD)**](https://en.wikipedia.org/wiki/Automatic_differentiation) using [casADi](https://web.casadi.org/) [[1](https://doi.org/10.1007/s12532-018-0139-4)] as a backend. A high-level interface for hyperelastic materials based on the deformation gradient exists. Several isotropic hyperelastic material formulations like the Neo-Hookean or the Ogden model are included in the model library. Gradient and hessian methods allow input data with trailing axes which is especially useful for Python-based finite element modules, e.g. [scikit-fem](https://scikit-fem.readthedocs.io/en/latest/) or [FElupe](https://github.com/adtzlr/felupe). Mixed-field formulations suitable for nearly-incompressible material behavior are supported as well as single-field formulations based on the deformation gradient. A numerical lab is included to run, plot and analyze homogenous uniaxial, equi-biaxial, planar shear and simple shear load cases.
+matADi is a 3.8+ Python package for the definition of a constitutive hyperelastic material formulation by a strain energy density function. Both [gradient](https://en.wikipedia.org/wiki/Gradient) (stress) and [hessian](https://en.wikipedia.org/wiki/Hessian_matrix) (elasticity tensor) are carried out by [**Automatic Differentiation (AD)**](https://en.wikipedia.org/wiki/Automatic_differentiation) using [casADi](https://web.casadi.org/) [[1](https://doi.org/10.1007/s12532-018-0139-4)] as a backend. A high-level interface for hyperelastic materials based on the deformation gradient exists. Several isotropic hyperelastic material formulations like the Neo-Hookean or the Ogden model are included in the model library. Gradient and hessian methods allow input data with trailing axes which is especially useful for Python-based finite element modules, e.g. [scikit-fem](https://scikit-fem.readthedocs.io/en/latest/) or [FElupe](https://github.com/adtzlr/felupe). Mixed-field formulations suitable for nearly-incompressible material behavior are supported as well as single-field formulations based on the deformation gradient. A numerical lab is included to run, plot and analyze homogeneous uniaxial, equi-biaxial, planar shear and simple shear load cases.
 
 ## Installation
 Install `matADi` from PyPI via pip.
 
 ```shell
 pip install matadi
 ```
@@ -99,64 +99,64 @@
 W_upJ = NH_upJ.function([defgrad, pressure, volratio])
 P_upJ = NH_upJ.gradient([defgrad, pressure, volratio])
 A_upJ = NH_upJ.hessian([defgrad, pressure, volratio])
 ```
 
 The output of `NH_upJ.gradient([defgrad, pressure, volratio])` is a list with gradients of the functional as `[dWdF, dWdp, dWdJ]`. Hessian entries are provided as a list of upper triangle entries, e.g. `NH_upJ.hessian([defgrad, pressure, volratio])` returns `[d2WdFdF, d2WdFdp, d2WdFdJ, d2Wdpdp, d2WdpdJ, d2WdJdJ]`.
 
-Available [isotropic hyperelastic material models](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py):
-- [Linear Elastic](https://en.wikipedia.org/wiki/Linear_elasticity) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py#L5-L7))
-- [Saint Venant Kirchhoff](https://en.wikipedia.org/wiki/Hyperelastic_material#Saint_Venant%E2%80%93Kirchhoff_model) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py#L10-L14))
-- [Neo-Hooke](https://en.wikipedia.org/wiki/Neo-Hookean_solid) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py#L17-L21))
-- [Mooney-Rivlin](https://en.wikipedia.org/wiki/Mooney%E2%80%93Rivlin_solid) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py#L24-L29))
-- [Yeoh](https://en.wikipedia.org/wiki/Yeoh_(hyperelastic_model)) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py#L32-L37))
-- [Third-Order-Deformation (James-Green-Simpson)](https://onlinelibrary.wiley.com/doi/abs/10.1002/app.1975.070190723) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py#L40-L51))
-- [Ogden](https://en.wikipedia.org/wiki/Ogden_(hyperelastic_model)) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py#L54-L64))
-- [Arruda-Boyce](https://en.wikipedia.org/wiki/Arruda%E2%80%93Boyce_model) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py#L67-L80))
-- [Extended-Tube](https://meridian.allenpress.com/rct/article-abstract/72/4/602/92819/An-Extended-Tube-Model-for-Rubber-Elasticity?redirectedFrom=fulltext) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py#L83-L91))
-- [Van-der-Waals (Kilian)](https://doi.org/10.1016/0032-3861(81)90200-7) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py#L94-L103))
-
-Available [anisotropic hyperelastic material models](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_anisotropic.py):
-- Fiber ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_anisotropic.py#L17-L35))
-- Fiber-family (+/- combination of single Fiber) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_anisotropic.py#L38-L45))
-- [Holzapfel Gasser Ogden](https://royalsocietypublishing.org/doi/full/10.1098/rsif.2005.0073) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_anisotropic.py#L48-L77))
-
-Available [micro-sphere hyperelastic frameworks](https://github.com/adtzlr/matadi/blob/main/matadi/models/microsphere) (Miehe, Göktepe, Lulei) [[2](https://doi.org/10.1016/j.jmps.2004.03.011)]:
-- [affine stretch](https://doi.org/10.1016/j.jmps.2004.03.011) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/microsphere/affine/_models.py#L6-L16))
-- [affine tube](https://doi.org/10.1016/j.jmps.2004.03.011) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/microsphere/affine/_models.py#L19-L30))
-- [non-affine stretch](https://doi.org/10.1016/j.jmps.2004.03.011) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/microsphere/nonaffine/_models.py#L7-L17))
-- [non-affine tube](https://doi.org/10.1016/j.jmps.2004.03.011) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/microsphere/nonaffine/_models.py#L20-L32))
+Available [isotropic hyperelastic material models](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py):
+- [Linear Elastic](https://en.wikipedia.org/wiki/Linear_elasticity) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py#L5-L7))
+- [Saint Venant Kirchhoff](https://en.wikipedia.org/wiki/Hyperelastic_material#Saint_Venant%E2%80%93Kirchhoff_model) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py#L10-L14))
+- [Neo-Hooke](https://en.wikipedia.org/wiki/Neo-Hookean_solid) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py#L17-L21))
+- [Mooney-Rivlin](https://en.wikipedia.org/wiki/Mooney%E2%80%93Rivlin_solid) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py#L24-L29))
+- [Yeoh](https://en.wikipedia.org/wiki/Yeoh_(hyperelastic_model)) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py#L32-L37))
+- [Third-Order-Deformation (James-Green-Simpson)](https://onlinelibrary.wiley.com/doi/abs/10.1002/app.1975.070190723) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py#L40-L51))
+- [Ogden](https://en.wikipedia.org/wiki/Ogden_(hyperelastic_model)) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py#L54-L64))
+- [Arruda-Boyce](https://en.wikipedia.org/wiki/Arruda%E2%80%93Boyce_model) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py#L67-L80))
+- [Extended-Tube](https://meridian.allenpress.com/rct/article-abstract/72/4/602/92819/An-Extended-Tube-Model-for-Rubber-Elasticity?redirectedFrom=fulltext) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py#L83-L91))
+- [Van-der-Waals (Kilian)](https://doi.org/10.1016/0032-3861(81)90200-7) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py#L94-L103))
+
+Available [anisotropic hyperelastic material models](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_anisotropic.py):
+- Fiber ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_anisotropic.py#L17-L35))
+- Fiber-family (+/- combination of single Fiber) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_anisotropic.py#L38-L45))
+- [Holzapfel Gasser Ogden](https://royalsocietypublishing.org/doi/full/10.1098/rsif.2005.0073) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_anisotropic.py#L48-L77))
+
+Available [micro-sphere hyperelastic frameworks](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/microsphere) (Miehe, Göktepe, Lulei) [[2](https://doi.org/10.1016/j.jmps.2004.03.011)]:
+- [affine stretch](https://doi.org/10.1016/j.jmps.2004.03.011) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/microsphere/affine/_models.py#L6-L16))
+- [affine tube](https://doi.org/10.1016/j.jmps.2004.03.011) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/microsphere/affine/_models.py#L19-L30))
+- [non-affine stretch](https://doi.org/10.1016/j.jmps.2004.03.011) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/microsphere/nonaffine/_models.py#L7-L17))
+- [non-affine tube](https://doi.org/10.1016/j.jmps.2004.03.011) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/microsphere/nonaffine/_models.py#L20-L32))
 
-Available [micro-sphere hyperelastic material models](https://github.com/adtzlr/matadi/blob/main/matadi/models/microsphere) (Miehe, Göktepe, Lulei) [[2](https://doi.org/10.1016/j.jmps.2004.03.011)]:
-- [Miehe Göktepe Lulei](https://doi.org/10.1016/j.jmps.2004.03.011) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/microsphere/nonaffine/_models.py#L35-L49))
+Available [micro-sphere hyperelastic material models](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/microsphere) (Miehe, Göktepe, Lulei) [[2](https://doi.org/10.1016/j.jmps.2004.03.011)]:
+- [Miehe Göktepe Lulei](https://doi.org/10.1016/j.jmps.2004.03.011) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/microsphere/nonaffine/_models.py#L35-L49))
 
 Any user-defined isotropic hyperelastic strain energy density function may be passed as the `fun` argument of `MaterialHyperelastic` by using the following template:
 
 ```python
 def fun(F, **kwargs):
     # user code
     return W
 ```
 
-In order to apply the above material model only on the isochoric part of the deformation gradient [[3](https://doi.org/10.1016/0045-7825(85)90033-7)], use the decorator [`@isochoric_volumetric_split`](https://github.com/adtzlr/matadi/blob/main/matadi/models/_helpers.py#L7-L31). If the keyword `bulk` is passed, an additional [volumetric strain energy function](https://github.com/adtzlr/matadi/blob/main/matadi/models/_helpers.py#L34-L35) is added to the base material formulation.
+In order to apply the above material model only on the isochoric part of the deformation gradient [[3](https://doi.org/10.1016/0045-7825(85)90033-7)], use the decorator [`@isochoric_volumetric_split`](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_helpers.py#L7-L31). If the keyword `bulk` is passed, an additional [volumetric strain energy function](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_helpers.py#L34-L35) is added to the base material formulation.
 
 ```python
 from matadi.models import isochoric_volumetric_split
 from matadi.math import trace, transpose
 
 @isochoric_volumetric_split
 def nh(F, C10=0.5):
     # user code of strain energy function, e.g. neo-hooke
     return C10 * (trace(transpose(F) @ F) - 3)
 
 NH = MaterialHyperelastic(nh, C10=0.5, bulk=200.0)
 ```
 
 ## Lab
-In matADi's `Lab` :lab_coat: numeric experiments on homogenous loadcases on compressible or nearly-incompressible material formulations are performed. For incompressible materials use `LabIncompressible` instead. Let's take the non-affine micro-sphere material model suitable for rubber elasticity with parameters from [[2](https://doi.org/10.1016/j.jmps.2004.03.011), Fig. 19] and run **uniaxial**, **biaxial** and **planar shear** tests.
+In matADi's `Lab` :lab_coat: numeric experiments on homogeneous loadcases on compressible or nearly-incompressible material formulations are performed. For incompressible materials use `LabIncompressible` instead. Let's take the non-affine micro-sphere material model suitable for rubber elasticity with parameters from [[2](https://doi.org/10.1016/j.jmps.2004.03.011), Fig. 19] and run **uniaxial**, **biaxial** and **planar shear** tests.
 
 ```python
 from matadi import Lab, MaterialHyperelastic
 from matadi.models import miehe_goektepe_lulei
 
 mat = MaterialHyperelastic(
     miehe_goektepe_lulei, 
@@ -191,21 +191,26 @@
 b) the monotonic increasing slope of force per undeformed area vs. stretch and
 c) the sign of the resulting stretch from a small superposed force in one direction.
 
 ## Hints and usage in FEM modules
 For tensor-valued material definitions use `MaterialTensor` (e.g. any stress-strain relation). Also, please have a look at [casADi's documentation](https://web.casadi.org/). It is very powerful but unfortunately does not support all the Python stuff you would expect. For example Python's default if-else-statements can't be used in combination with symbolic conditions (use `math.if_else(cond, if_true, if_false)` instead). Contrary to [casADi](https://web.casadi.org/), the gradient of the eigenvalue function is stabilized by a perturbation of the diagonal components.
 
 ### A **Material** with state variables
-A generalized material model with optional state variables for the (u/p)-formulation is created by an instance of `MaterialTensor`. If the argument `triu` is set to `True` the gradient method returns only the upper triangle entries of the gradient components. If some of the input variables are internal state variables the number of these variables have to be passed to the optional argument `statevars`. While the hyperelastic material classes are defined by a strain energy function, this one is defined by the first Piola-Kirchhoff stress tensor. Internally, state variables are equal to default variables but they are excluded from gradient calculations. State variables may also be used as placeholders for additional quantities, e.g. the initial deformation gradient at the beginning of an increment or the time increment. Hence, it is a very flexible class not restricted to hyperelasticity.
+A generalized material model with optional state variables, optionally for the (u/p)-formulation, is created by an instance of `MaterialTensor`. If the argument `triu` is set to `True` the gradient method returns only the upper triangle entries of the gradient components. If some of the input variables are internal state variables the number of these variables have to be passed to the optional argument `statevars`. While the hyperelastic material classes are defined by a strain energy function, this one is defined by the first Piola-Kirchhoff stress tensor. Internally, state variables are equal to default variables but they are excluded from gradient calculations. State variables may also be used as placeholders for additional quantities, e.g. the initial deformation gradient at the beginning of an increment or the time increment. Hence, it is a very flexible class not restricted to hyperelasticity. For consistency, the methods `gradient` and `hessian` of a tensor-based material refer to the gradient and hessian of the strain energy function.
+
+Included [pseudo-elastic material models](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_pseudo_elasticity.py):
+- [Ogden-Roxburgh](https://doi.org/10.1098%2Frspa.1999.0431) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_pseudo_elasticity.py#L4-L16))
+
 
-Included [pseudo-elastic material models](https://github.com/adtzlr/matadi/blob/main/matadi/models/_pseudo_elasticity.py):
-- [Ogden-Roxburgh](https://doi.org/10.1098%2Frspa.1999.0431) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_pseudo_elasticity.py#L4-L16))
+Included [viscoelastic material models](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_viscoelasticity.py):
+- [Finite-Strain-Viscoelastic](https://doi.org/10.1016/j.cma.2013.07.004) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_viscoelasticity.py#L4-L18))
+- [Finite-Strain-Viscoelastic (Mooney-Rivlin)](https://doi.org/10.1002/nme.5724) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_viscoelasticity.py#L21-L51))
 
-Included [other material models](https://github.com/adtzlr/matadi/blob/main/matadi/models/_misc.py):
-- [MORPH](https://doi.org/10.1016/S0749-6419(02)00091-8) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_misc.py#L19-L75))
+Included [other material models](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_misc.py):
+- [MORPH](https://doi.org/10.1016/S0749-6419(02)00091-8) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_misc.py#L19-L75))
 
 ```python
 import numpy as np
 
 from matadi.models import (
     displacement_pressure_split, neo_hooke, volumetric, ogden_roxburgh
 )
@@ -244,22 +249,30 @@
 defgrad = np.random.rand(3, 3, 5, 100) - 0.5
 pressure = np.random.rand(1, 5, 100)
 statevars = np.random.rand(1, 1, 5, 100)
 
 for a in range(3):
     defgrad[a, a] += 1.0
 
-dWdF, dWdp, statevars_new = NH.function([defgrad, pressure, statevars])
-d2WdFdF, d2WdFdp, d2Wdpdp = NH.gradient([defgrad, pressure, statevars])
+dWdF, dWdp, statevars_new = NH.gradient([defgrad, pressure, statevars])
+d2WdFdF, d2WdFdp, d2Wdpdp = NH.hessian([defgrad, pressure, statevars])
 ```
 
-**Hint**: *The above Neo-Hooke as well as the MORPH material model formulation within the u/p-framework are available as template-materials in `matadi.models` as `NeoHookeOgdenRoxburgh()`and `Morph()`. The state variable concept is also implemented for the `Material` class.*
+The Neo-Hooke, the MORPH and the Finite-Strain-Viscoelastic [[4](https://doi.org/10.1016/j.cma.2013.07.004)] material model formulations are available as ready-to-go materials in `matadi.models` as:
+
+* [`NeoHookeOgdenRoxburgh()`](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_templates.py), 
+* [`Morph()`](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_templates.py),
+* [`Viscoelastic()`](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_templates.py) and
+* [`ViscoelasticMooneyRivlin()`](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_templates.py).
+
+**Hint**: *The state variable concept is also implemented for the `Material` class.*
 
 Simple examples for using `matadi` with [`scikit-fem`](https://github.com/adtzlr/matadi/discussions/14#) as well as with [`felupe`](https://github.com/adtzlr/matadi/discussions/22) are shown in the Discussion section.
 
 ## References
 [1] J. A. E. Andersson, J. Gillis, G. Horn, J. B. Rawlings, and M. Diehl, *CasADi - A software framework for nonlinear optimization and optimal control*, Math. Prog. Comp., vol. 11, no. 1, pp. 1–36, 2019, [![DOI:10.1007/s12532-018-0139-4](https://zenodo.org/badge/DOI/10.1007/s12532-018-0139-4.svg)](https://doi.org/10.1007/s12532-018-0139-4)
 
 [2] C. Miehe, S. Göktepe and F. Lulei, *A micro-macro approach to rubber-like materials. Part I: the non-affine micro-sphere model of rubber elasticity*, Journal of the Mechanics and Physics of Solids, vol. 52, no. 11. Elsevier BV, pp. 2617–2660, Nov. 2004. [![DOI:10.1016/j.jmps.2004.03.011](https://zenodo.org/badge/DOI/10.1016/j.jmps.2004.03.011.svg)](https://doi.org/10.1016/j.jmps.2004.03.011)
 
 [3] J. C. Simo, R. L. Taylor, and K. S. Pister, *Variational and projection methods for the volume constraint in finite deformation elasto-plasticity*, Computer Methods in Applied Mechanics and Engineering, vol. 51, no. 1–3, pp. 177–208, Sep. 1985, [![DOI:10.1016/0045-7825(85)90033-7](https://zenodo.org/badge/DOI/10.1016/0045-7825(85)90033-7.svg)](https://doi.org/10.1016/0045-7825(85)90033-7)
 
+[4] A. V. Shutov, R. Landgraf, and J. Ihlemann, *An explicit solution for implicit time stepping in multiplicative finite strain viscoelasticity*, Computer Methods in Applied Mechanics and Engineering, vol. 265. Elsevier BV, pp. 213–225, Oct. 2013, [![DOI:10.1016/j.cma.2013.07.004](https://zenodo.org/badge/DOI/10.1016/j.cma.2013.07.004.svg)](https://doi.org/10.1016/j.cma.2013.07.004)
```

### Comparing `matadi-0.1.9/matadi/_apply.py` & `matadi-0.2.0/src/matadi/_apply.py`

 * *Files identical despite different names*

### Comparing `matadi-0.1.9/matadi/_lab_compressible.py` & `matadi-0.2.0/src/matadi/_lab_compressible.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-import numpy as np
-import matplotlib.pyplot as plt
 from collections import namedtuple
+
+import matplotlib.pyplot as plt
+import numpy as np
 from scipy.optimize import root
 
 
 class LabCompressible:
-    def __init__(self, material):
-
+    def __init__(self, material, title=None):
         self.material = material
-        self.title = self._get_title()
+        self.title = title
+        if title is None:
+            self.title = self._get_title()
 
     def _get_title(self):
         return "Material Formulation: " + "-".join(
             [m.title() for m in self.material.fun.__name__.split("_")]
         )
 
     def _uniaxial(self, stretch):
@@ -99,15 +101,15 @@
             df = np.zeros(3)
             df[0] = 1
 
             # calculate linear solution of stretch 1 resulting from unit load
             dl = (np.linalg.inv(B) @ df)[0]
 
             # check volume ratio
-            J = stretch ** 2 * stretch_3
+            J = stretch**2 * stretch_3
 
             # check slope of force
             Q = self.material.gradient([G])[0][0, 0]
             P = self.material.gradient([F])[0][0, 0]
 
             return True if dl > 0 and J > 0 and (Q - P) > 0 else False
 
@@ -300,17 +302,15 @@
             "planar": {"color": "C2"},
         }
 
         if data[-1].label == "shear":
             data = data[:-1]
 
         for d in data:
-
             if stability:
-
                 stable = np.array(d.stability, dtype=bool)
 
                 unstable_idx = np.arange(len(d.stretch))[~stable]
                 stable_idx = np.arange(len(d.stretch))[stable]
 
                 stress_stable = d.stress.copy()
                 stress_stable[unstable_idx] = np.nan
@@ -323,15 +323,14 @@
                     d.stretch,
                     stress_unstable,
                     **lineargs[d.label],
                     linestyle="--",
                 )
 
             else:
-
                 ax.plot(d.stretch, d.stress, **lineargs[d.label], label=d.label)
 
         ax.grid()
         ax.set_title(self.title, fontsize=10)
         ax.set_xlabel(r"stretch $\lambda_1 \quad \longrightarrow$")
         ax.set_ylabel(r"force per undeformed area $P_{11} \quad \longrightarrow$")
         ax.legend()
```

### Comparing `matadi-0.1.9/matadi/_lab_incompressible.py` & `matadi-0.2.0/src/matadi/_lab_incompressible.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,32 @@
-import numpy as np
-import matplotlib.pyplot as plt
 from collections import namedtuple
-from scipy.optimize import root
 
+import matplotlib.pyplot as plt
+import numpy as np
 
-class LabIncompressible:
-    def __init__(self, material):
 
+class LabIncompressible:
+    def __init__(self, material, title=None):
         self.material = material
-        self.title = self._get_title()
+        self.title = title
+        if title is None:
+            self.title = self._get_title()
 
     def _get_title(self):
         return "Material Formulation: " + "-".join(
             [m.title() for m in self.material.fun.__name__.split("_")]
         )
 
     def _ux(self, stretch):
         "Principal stretches of incompressible uniaxial load case."
         return stretch, 1 / np.sqrt(stretch), 1 / np.sqrt(stretch)
 
     def _bx(self, stretch):
         "Principal stretches of incompressible equi-biaxial load case."
-        return stretch, stretch, 1 / stretch ** 2
+        return stretch, stretch, 1 / stretch**2
 
     def _ps(self, stretch):
         "Principal stretches of incompressible planar shear load case."
         return stretch, 1, 1 / stretch
 
     def _loadcase(self, stretch, kinematics):
         "Generalized load case `UX/BX/PS (Incompressible)`."
@@ -199,17 +200,15 @@
             "planar": {"color": "C2"},
         }
 
         if data[-1].label == "shear":
             data = data[:-1]
 
         for d in data:
-
             if stability:
-
                 stable = np.array(d.stability, dtype=bool)
 
                 unstable_idx = np.arange(len(d.stretch))[~stable]
                 stable_idx = np.arange(len(d.stretch))[stable]
 
                 stress_stable = d.stress.copy()
                 stress_stable[unstable_idx] = np.nan
@@ -222,15 +221,14 @@
                     d.stretch,
                     stress_unstable,
                     **lineargs[d.label],
                     linestyle="--",
                 )
 
             else:
-
                 ax.plot(d.stretch, d.stress, **lineargs[d.label], label=d.label)
 
         ax.grid()
         ax.set_title(self.title, fontsize=10)
         ax.set_xlabel(r"stretch $\lambda_1 \quad \longrightarrow$")
         ax.set_ylabel(r"force per undeformed area $P_{11} \quad \longrightarrow$")
         ax.legend()
```

### Comparing `matadi-0.1.9/matadi/_material.py` & `matadi-0.2.0/src/matadi/_material.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from multiprocessing import cpu_count
 
-import numpy as np
 import casadi as ca
+import numpy as np
 
 from ._apply import apply
-from . import Variable
+from ._variable import Variable
 
 
 class Function:
     def __init__(self, x, fun, args=(), kwargs={}, compress=False):
-
         self.x = x
         self._fun = fun
 
         self.args = args
         self.kwargs = kwargs
 
         # generate function
@@ -41,15 +40,14 @@
             fun_shape=self._idx_function,
             threads=threads,
         )
 
 
 class FunctionTensor:
     def __init__(self, x, fun, args=(), kwargs={}, compress=False):
-
         self.x = x
         self._fun = fun
 
         self.args = args
         self.kwargs = kwargs
 
         # generate function
@@ -79,15 +77,14 @@
         )
 
 
 class Material(Function):
     def __init__(
         self, x, fun, args=(), kwargs={}, compress=False, triu=True, statevars=0
     ):
-
         # init Function
         super().__init__(x=x, fun=fun, args=args, kwargs=kwargs)
 
         # no. of active variables
         n = len(self.x) - statevars
         self._idx_gradient = self._idx_x[:n]
 
@@ -202,17 +199,17 @@
         )
 
 
 class MaterialTensor(FunctionTensor):
     def __init__(
         self, x, fun, args=(), kwargs={}, compress=False, triu=True, statevars=0
     ):
-
         # init Function
         super().__init__(x=x, fun=fun, args=args, kwargs=kwargs)
+        self.gradient = self.function
 
         # no. of active variables
         n = len(self.x) - statevars
 
         # generate vector for gradient-vector-product
         self.v = [Variable("v%d" % a, *x.shape) for a, x in enumerate(self.x)]
 
@@ -220,17 +217,14 @@
         self._g = [ca.jacobian(f, x) for x in self.x[:n] for f in self._f[:n]]
         self._gvp = [
             ca.jtimes(f, x, v)
             for x, v in zip(self.x[:n], self.v[:n])
             for f in self._f[:n]
         ]
 
-        # alias
-        self.jacobian = self.gradient
-
         # store only upper-triangle entries of gradients
         if triu:
             i, j = np.triu_indices(len(self.x[:n]))
             a = (
                 np.arange(len(self.x[:n]) ** 2)
                 .reshape(len(self.x[:n]), len(self.x[:n]))[i, j]
                 .ravel()
@@ -262,15 +256,15 @@
 
                 if triu:
                     if j >= i:
                         self._idx_gradient.append((*a, *b))
                 else:
                     self._idx_gradient.append((*a, *b))
 
-    def gradient(self, x, threads=cpu_count()):
+    def hessian(self, x, threads=cpu_count()):
         "Return list of gradients."
         return apply(
             x,
             fun=self._gradient,
             x_shape=self._idx_x,
             fun_shape=self._idx_gradient,
             threads=threads,
```

### Comparing `matadi-0.1.9/matadi/models/_helpers.py` & `matadi-0.2.0/src/matadi/models/_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from functools import wraps
 from copy import deepcopy
+from functools import wraps
 
-from .. import Variable
-from ..math import det, cof, trace, gradient
+from .._variable import Variable
+from ..math import cof, det, gradient, trace
 
 
 def isochoric_volumetric_split(fun):
     """Apply the material formulation only on the isochoric part of the
     multiplicative split of the deformation gradient. Optionally, if
     the bulk keyword is passed, add a volumetric term."""
 
@@ -42,15 +42,14 @@
     . The additional hydrostatic stress variable `p` is attached as an
     attribute `fun.p` to the augmented function."""
 
     p = Variable("p")
 
     @wraps(fun)
     def apply_up(*args, **kwargs):
-
         F = args[0][0]
 
         f = fun(*args, **kwargs)
 
         # check if function is list or tuple
         if not (isinstance(f, list) or isinstance(f, tuple)):
             f = [f]
```

### Comparing `matadi-0.1.9/matadi/models/_hyperelasticity_anisotropic.py` & `matadi-0.2.0/src/matadi/models/_hyperelasticity_anisotropic.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-from ._helpers import isochoric_volumetric_split
 from ..math import (
-    transpose,
-    det,
     DM,
+    cos,
     exp,
+    if_else,
+    invariants,
     log,
-    cos,
-    sin,
     pi,
+    sin,
     sqrt,
-    if_else,
-    invariants,
     trace,
+    transpose,
 )
+from ._helpers import isochoric_volumetric_split
 
 
 @isochoric_volumetric_split
 def fiber(F, E, angle, k=1, axis=2, compression=False):
     "Fiber"
 
     a = angle * pi / 180
@@ -28,20 +27,20 @@
     C = transpose(F) @ F
 
     stretch = sqrt((transpose(N) @ C @ N))[0, 0]
 
     if k == 0:
         strain = log(stretch)
     else:
-        strain = 1 / k * (stretch ** k - 1)
+        strain = 1 / k * (stretch**k - 1)
 
     if not compression:
         strain = if_else(strain < 0, 0, strain)
 
-    return E * strain ** 2 / 2
+    return E * strain**2 / 2
 
 
 @isochoric_volumetric_split
 def fiber_family(F, E, angle, k=1, axis=2, compression=False):
     "Fiber Family"
 
     f1 = fiber(F, E, angle=angle, k=k, axis=axis, compression=compression)
```

### Comparing `matadi-0.1.9/matadi/models/_hyperelasticity_isotropic.py` & `matadi-0.2.0/src/matadi/models/_hyperelasticity_isotropic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,48 @@
+from ..math import det, dot, eigvals, eye, log, sqrt, sum1, sym, trace, transpose
 from ._helpers import isochoric_volumetric_split
-from ..math import dot, det, transpose, trace, eigvals, sum1, log, sqrt, eye, sym
 
 
 def linear_elastic(F, mu, lmbda):
     strain = sym(F - eye(3))
     return mu * trace(strain @ strain) + lmbda / 2 * trace(strain) ** 2
 
 
 def saint_venant_kirchhoff(F, mu, lmbda):
-    C = dot(transpose(F), F)
+    C = transpose(F) @ F
     I1 = trace(C) / 2 - 3 / 2
     I2 = trace(C @ C) / 4 - trace(C) / 2 + 3 / 4
-    return mu * I2 + lmbda * I1 ** 2 / 2
+    return mu * I2 + lmbda * I1**2 / 2
 
 
 @isochoric_volumetric_split
 def neo_hooke(F, C10):
     C = transpose(F) @ F
     I1 = trace(C)
     return C10 * (I1 - 3)
 
 
 @isochoric_volumetric_split
-def mooney_rivlin(F, C10, C01):
+def mooney_rivlin(F, C10, C01=0):
     C = transpose(F) @ F
     I1 = trace(C)
     I2 = (trace(C) ** 2 - trace(C @ C)) / 2
     return C10 * (I1 - 3) + C01 * (I2 - 3)
 
 
 @isochoric_volumetric_split
-def yeoh(F, C10, C20, C30):
+def yeoh(F, C10, C20=0, C30=0):
     J = det(F)
     C = transpose(F) @ F
     I1 = J ** (-2 / 3) * trace(C)
     return C10 * (I1 - 3) + C20 * (I1 - 3) ** 2 + C30 * (I1 - 3) ** 3
 
 
 @isochoric_volumetric_split
-def third_order_deformation(F, C10, C01, C11, C20, C30):
+def third_order_deformation(F, C10, C01=0, C11=0, C20=0, C30=0):
     C = transpose(F) @ F
     I1 = trace(C)
     I2 = (trace(C) ** 2 - trace(C @ C)) / 2
     return (
         C10 * (I1 - 3)
         + C01 * (I2 - 3)
         + C11 * (I1 - 3) * (I2 - 3)
@@ -55,49 +55,49 @@
 def ogden(F, mu, alpha):
     C = transpose(F) @ F
     wC = eigvals(C)
 
     out = 0
     for m, a in zip(mu, alpha):
         wk = wC ** (a / 2)
-        out += 2 * m / a ** 2 * (sum1(wk)[0, 0] - 3)
+        out += 2 * m / a**2 * (sum1(wk)[0, 0] - 3)
 
     return out
 
 
 @isochoric_volumetric_split
 def arruda_boyce(F, C1, limit):
     C = transpose(F) @ F
     I1 = trace(C)
 
     alpha = [1 / 2, 1 / 20, 11 / 1050, 19 / 7000, 519 / 673750]
-    beta = 1 / limit ** 2
+    beta = 1 / limit**2
 
     out = 0
     for i, a in enumerate(alpha):
         j = i + 1
-        out += a * beta ** (2 * j - 2) * (I1 ** j - 3 ** j)
+        out += a * beta ** (2 * j - 2) * (I1**j - 3**j)
 
     return C1 * out
 
 
 @isochoric_volumetric_split
 def extended_tube(F, Gc, delta, Ge, beta):
     C = transpose(F) @ F
     D = trace(C)
     wC = eigvals(C)
-    g = (1 - delta ** 2) * (D - 3) / (1 - delta ** 2 * (D - 3))
-    Wc = Gc / 2 * (g + log(1 - delta ** 2 * (D - 3)))
-    We = 2 * Ge / beta ** 2 * sum1(wC ** (-beta / 2) - 1)
+    g = (1 - delta**2) * (D - 3) / (1 - delta**2 * (D - 3))
+    Wc = Gc / 2 * (g + log(1 - delta**2 * (D - 3)))
+    We = 2 * Ge / beta**2 * sum1(wC ** (-beta / 2) - 1)
     return Wc + We
 
 
 @isochoric_volumetric_split
 def van_der_waals(F, mu, limit, a, beta):
     C = transpose(F) @ F
     I1 = trace(C)
     I2 = (trace(C) ** 2 - trace(C @ C)) / 2
-    I = (1 - beta) * I1 + beta * I2
-    eta = sqrt((I - 3) / (limit ** 2 - 3))
+    Im = (1 - beta) * I1 + beta * I2
+    eta = sqrt((Im - 3) / (limit**2 - 3))
     return mu * (
-        -(limit ** 2 - 3) * (log(1 - eta) + eta) - 2 / 3 * a * ((I - 3) / 2) ** (3 / 2)
+        -(limit**2 - 3) * (log(1 - eta) + eta) - 2 / 3 * a * ((Im - 3) / 2) ** (3 / 2)
     )
```

### Comparing `matadi-0.1.9/matadi/models/_misc.py` & `matadi-0.2.0/src/matadi/models/_misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from ._hyperelasticity_isotropic import neo_hooke
 from ..math import (
+    astensor,
+    asvoigt,
     det,
-    inv,
     dev,
-    sym,
-    sqrt,
+    gradient,
     if_else,
-    vertsplit,
-    vertcat,
-    asvoigt,
-    astensor,
-    tresca,
+    inv,
     mexp,
-    gradient,
+    sqrt,
+    sym,
+    tresca,
+    vertcat,
+    vertsplit,
 )
+from ._hyperelasticity_isotropic import neo_hooke
 
 
 def morph(x, p1, p2, p3, p4, p5, p6, p7, p8):
     "MORPH consitutive material formulation."
 
     # split input into the deformation gradient and the vector of state variables
     F, statevars = x[0], x[-1]
@@ -39,23 +39,25 @@
     # (isochoric part of) lagrangian rate of deformation tensor
     L = dev(sym(dC @ inv(C))) @ CG
 
     # tresca invariants of (distortional part of) C and L
     CT = tresca(CG)
     LT = tresca(L)
 
-    # maximum historical von mises invariant of CG
+    # maximum historical tresca invariant of (distortional part of) C
     CTS = if_else(CT > CTSn, CT, CTSn)
 
     # stable normalizations: L / LT and CT / CTS
     L_LT = if_else(LT > 0, L / LT, L)
     CT_CTS = if_else(CTS > 0, CT / CTS, CT)
 
     # MORPH deformation-dependent material parameters
-    f = lambda x: 1 / sqrt(1 + x ** 2)
+    def f(x):
+        return 1 / sqrt(1 + x**2)
+
     a = p1 + p2 * f(p3 * CTS)
     b = p4 * f(p3 * CTS)
     c = p5 * CTS * (1 - f(CTS / p6))
 
     # Hull stress
     SH = (c * mexp(p7 * L_LT * CT_CTS) + p8 * L_LT) @ inv(C)
```

### Comparing `matadi-0.1.9/matadi/models/_pseudo_elasticity.py` & `matadi-0.2.0/src/matadi/models/_pseudo_elasticity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..math import fmax, erf
+from ..math import erf, fmax
 
 
 def ogden_roxburgh(W, Wmaxn, r, m, beta):
     """An isotropic pseudo-elastic material formulation for the description of
     the Mullins-softening of rubber-like materials according to
     Ogden & Roxburgh."""
```

### Comparing `matadi-0.1.9/matadi/models/_templates.py` & `matadi-0.2.0/tests/test_displacement-pressure.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,83 +1,129 @@
-from ._misc import morph
-from ._hyperelasticity_isotropic import neo_hooke
-from ._pseudo_elasticity import ogden_roxburgh
-from ._helpers import volumetric, displacement_pressure_split
-from ..math import det, gradient
-from .._material import MaterialTensor
-from .. import Variable
-
-
-class NeoHookeOgdenRoxburgh(MaterialTensor):
-    "Neo-Hooke and Ogden-Roxburgh material formulations within the u/p framework."
-
-    def __init__(self, C10=0.5, r=3, m=1, beta=0, bulk=5000):
-        @displacement_pressure_split
-        def fun(x, C10, r, m, beta, bulk):
-
-            # split `x` into the deformation gradient and the state variable
-            F, Wmaxn = x[0], x[-1]
-
-            # isochoric and volumetric parts of the hyperelastic
-            # strain energy function
-            W = neo_hooke(F, C10)
-            U = volumetric(det(F), bulk)
-
-            # pseudo-elastic softening function
-            eta, Wmax = ogden_roxburgh(W, Wmaxn, r, m, beta)
-
-            # first Piola-Kirchhoff stress and updated state variable
-            # for a pseudo-elastic material formulation
-            return eta * gradient(W, F) + gradient(U, F), Wmax
+import numpy as np
+import pytest
 
-        F = Variable("F", 3, 3)
-        p = fun.p
-        z = Variable("z", 1, 1)
+from matadi import MaterialTensor, Variable
+from matadi.math import astensor, asvoigt, det, dev, gradient, inv, triu, vertcat, zeros
+from matadi.models import (
+    displacement_pressure_split,
+    morph,
+    neo_hooke,
+    ogden_roxburgh,
+    volumetric,
+)
+
+
+@displacement_pressure_split
+def fun_nh_or(x, C10=0.5, bulk=5000, r=3, m=1, beta=0):
+    "Strain energy function: Neo-Hooke & Ogden-Roxburgh."
+
+    # split `x` into the deformation gradient and the state variable
+    F, Wmaxn = x[0], x[-1]
+
+    # isochoric and volumetric parts of the hyperelastic strain energy function
+    W = neo_hooke(F, C10)
+    U = volumetric(det(F), bulk)
+
+    # pseudo-elastic softening
+    eta, Wmax = ogden_roxburgh(W, Wmaxn, r, m, beta)
+
+    # softened first Piola-Kirchhoff stress and updated state variable
+    return eta * gradient(W, F) + gradient(U, F), Wmax
 
-        kwargs = {"C10": C10, "r": r, "m": m, "beta": beta, "bulk": bulk}
 
-        super().__init__(x=[F, p, z], fun=fun, triu=True, statevars=1, kwargs=kwargs)
+@displacement_pressure_split
+def fun_morph(x, p1=0.035, p2=0.37, p3=0.17, p4=2.4, p5=0.01, p6=6.4, p7=5.5, p8=0.24):
+    "Strain energy function: Neo-Hooke & Ogden-Roxburgh."
 
+    # split `x` into the deformation gradient and the state variable
+    F = x[0]
 
-class Morph(MaterialTensor):
-    "MORPH consitutive material formulation within the u/p framework."
+    P, statevars = morph(x, p1, p2, p3, p4, p5, p6, p7, p8)
+    U = volumetric(det(F), 5000 * 2 * (p1 + p2))
 
-    def __init__(
-        self,
-        p1=0.035,
-        p2=0.37,
-        p3=0.17,
-        p4=2.4,
-        p5=0.01,
-        p6=6.4,
-        p7=5.5,
-        p8=0.24,
-        bulk=4050,
-    ):
-        @displacement_pressure_split
-        def fun(x, p1, p2, p3, p4, p5, p6, p7, p8, bulk):
+    # first Piola-Kirchhoff stress and updated state variable
+    return P + gradient(U, F), statevars
 
-            F = x[0]
-            J = det(F)
 
-            P, statevars = morph(x, p1, p2, p3, p4, p5, p6, p7, p8)
-            U = volumetric(J, bulk)
+def test_up_state():
+    # deformation gradient
+    F = Variable("F", 3, 3)
 
-            return P + gradient(U, F), statevars
+    # state variables
+    statevars = [Variable("z", 1, 1), Variable("z", 13, 1)]
+    functions = [fun_nh_or, fun_morph]
 
-        F = Variable("F", 3, 3)
+    for fun, z in zip(functions, statevars):
+        # get pressure variable from augmented function
         p = fun.p
-        z = Variable("z", 13, 1)
 
-        kwargs = {
-            "p1": p1,
-            "p2": p2,
-            "p3": p3,
-            "p4": p4,
-            "p5": p5,
-            "p6": p6,
-            "p7": p7,
-            "p8": p8,
-            "bulk": bulk,
-        }
+        # Material as a function of `F` and `p`
+        # with additional state variables `z`
+        M = MaterialTensor([F, p, z], fun, triu=True, statevars=1)
+
+        FF = (np.random.rand(3, 3, 8, 100) - 0.5) / 2
+        pp = np.random.rand(1, 8, 100)
+        zz = np.random.rand(*z.shape, 8, 100)
+
+        for a in range(3):
+            FF[a, a] += 1
+
+        P = M.gradient([FF, pp, zz])  # stress, constraint, statevars_new
+        A = M.hessian([FF, pp, zz])
+
+        assert len(P) == 3
+        assert len(A) == 3
+
+
+def test_up_basic():
+    # deformation gradient
+    F = Variable("F", 3, 3)
+
+    @displacement_pressure_split
+    def fun(x):
+        F = x[0]
+        C = F.T @ F
+
+        # (begin) test `asvoigt()` and `astensor()`
+        C_3D = F.T @ F
+        C_2D = vertcat(C_3D[0, 0], C_3D[1, 0], C_3D[0, 1], C_3D[1, 1]).reshape((2, 2))
+
+        C_6 = asvoigt(C_3D)
+        C_4 = asvoigt(C_2D)
+
+        C_from_C_6 = astensor(C_6)
+        C_2D_from_C_4 = astensor(C_4)
+
+        assert C_3D[0, 1] == C_from_C_6[0, 1]
+        assert C_2D[0, 1] == C_2D_from_C_4[0, 1]
+
+        with pytest.raises(ValueError):
+            asvoigt(C_6)
+
+        with pytest.raises(ValueError):
+            astensor(C_3D)
+        # (end) test `asvoigt()` and `astensor()`
+
+        return det(F) ** (-2 / 3) * dev(C) @ inv(C)
+
+    # get pressure variable from augmented function
+    p = fun.p
+
+    # Material as a function of `F` and `p`
+    M = MaterialTensor([F, p], fun, triu=True)
+
+    FF = np.random.rand(3, 3, 8, 100)
+    pp = np.random.rand(1, 8, 100)
+
+    for a in range(3):
+        FF[a, a] += 1
+
+    P = M.gradient([FF, pp])  # stress, constraint
+    A = M.hessian([FF, pp])
+
+    assert len(P) == 2
+    assert len(A) == 3
+
 
-        super().__init__(x=[F, p, z], fun=fun, triu=True, statevars=1, kwargs=kwargs)
+if __name__ == "__main__":
+    test_up_basic()
+    test_up_state()
```

### Comparing `matadi-0.1.9/matadi/models/microsphere/_chain.py` & `matadi-0.2.0/src/matadi/models/microsphere/_chain.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,37 +3,37 @@
 
 def langevin(stretch, mu, N):
     """Langevin model given by the free energy of a single chain as a function
     of the stretch (assuming a complex valued logarithm). The inverse
     Langevin function is defined by a Padé approximation."""
 
     x = stretch / sqrt(N)
-    L = x * (3 - x ** 2) / (1 - x ** 2)
+    L = x * (3 - x**2) / (1 - x**2)
 
     return mu * N * (x * L + log(L / sinh(L)))
 
 
 def langevin2(stretch, mu, N):
     """Langevin model given by the free energy of a single chain as a function
     of the stretch (assuming a complex valued logarithm). The inverse Langevin
     function is defined by a Padé approximation.
 
     **Note**: This function is optimized for fast gradient evaluation but
     cannot be used to calculate the actual free energy - only its derivative
     w.r.t. the stretch gives a real-valued result for the region of interest
     `N > stretch ** 2`."""
 
-    return mu * (stretch ** 2 / 2 - N * log(stretch ** 2 - N))
+    return mu * (stretch**2 / 2 - N * log(stretch**2 - N))
 
 
 def gauss(stretch, mu):
     """Gaussian model given by the free energy
     of a single chain as a function of the stretch."""
 
-    return 3 * mu / 2 * (stretch ** 2 - 1)
+    return 3 * mu / 2 * (stretch**2 - 1)
 
 
 def linear(stretch, mu):
     """Linear model given by the free energy
     of a single chain as a function of the stretch."""
 
     return mu * (stretch - 1)
```

### Comparing `matadi-0.1.9/matadi/models/microsphere/affine/_models.py` & `matadi-0.2.0/src/matadi/models/microsphere/affine/_models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from ..._helpers import isochoric_volumetric_split, displacement_pressure_split
-from ....math import transpose, sum1, diag, sqrt, inv, det, reshape, dev
+from ....math import det, dev, diag, inv, reshape, sqrt, sum1, transpose
+from ..._helpers import displacement_pressure_split, isochoric_volumetric_split
 from ..quadrature._bazant_oh import BazantOh
 
 
 @isochoric_volumetric_split
 def microsphere_affine_stretch(F, f, kwargs, quadrature=BazantOh(n=21)):
     "Micro-sphere model: Affine stretch part."
 
@@ -27,42 +27,38 @@
     Cs = transpose(Fs) @ Fs
     affine_areastretch = sqrt(diag(r.T @ Cs @ r))
 
     return sum1(f(affine_areastretch, **kwargs) * w)
 
 
 @displacement_pressure_split
-def microsphere_affine_force(x, fun, *args, **kwargs):
+def microsphere_affine_force(x, f, *args, **kwargs):
     """Micro-sphere model: Forces of affine stretch model as first Piola-
     Kirchhoff stress tensor embedded into a (u/p)-framework."""
 
     # sphere quadrature
     sphere = BazantOh(n=21)
 
     # extract current and initial deformation gradient and state variables
     F = x[0]
-    Fn = x[-2]
     statevars_n = x[-1]
 
     # volume ratios
     J = det(F)
-    Jn = det(Fn)
 
     # unimodular part of current and initial right Cauchy-Green deformation tensor
     C = F.T @ F
     CG = J ** (-2 / 3) * (C)
-    CGn = Jn ** (-2 / 3) * (Fn.T @ Fn)
 
     # affine stretches
-    lam_n = sqrt(diag(sphere.points.T @ CGn @ sphere.points))
     lam = sqrt(diag(sphere.points.T @ CG @ sphere.points))
 
     bulk = kwargs.pop("bulk")
 
     # fiber forces and state variable update
-    f, statevars = fun(lam, lam_n, statevars_n, *args, **kwargs)
+    f, statevars = f(lam, statevars_n, *args, **kwargs)
 
     # Second Piola-Kirchhoff stress tensor
     SG = reshape(sum1(f / lam * sphere.weights * sphere.bases), 3, 3)
     S = dev(SG @ CG) @ inv(C) + bulk * (J - 1) * J * inv(C)
 
     return F @ S, statevars
```

### Comparing `matadi-0.1.9/matadi/models/microsphere/nonaffine/_models.py` & `matadi-0.2.0/src/matadi/models/microsphere/nonaffine/_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+from ....math import det, diag, inv, sqrt, sum1, transpose
 from ..._helpers import isochoric_volumetric_split
-from ....math import transpose, sum1, diag, sqrt, inv, det
-from ..quadrature._bazant_oh import BazantOh
 from .._chain import langevin, linear
+from ..quadrature._bazant_oh import BazantOh
 
 
 @isochoric_volumetric_split
 def microsphere_nonaffine_stretch(F, p, f, kwargs, quadrature=BazantOh(n=21)):
     "Micro-sphere model: Non-affine stretch part."
 
     r = quadrature.points
```

### Comparing `matadi-0.1.9/matadi/models/microsphere/quadrature/_bazant_oh.py` & `matadi-0.2.0/src/matadi/models/microsphere/quadrature/_bazant_oh.py`

 * *Files identical despite different names*

### Comparing `matadi-0.1.9/matadi.egg-info/PKG-INFO` & `matadi-0.2.0/src/matadi.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: matadi
-Version: 0.1.9
+Version: 0.2.0
 Summary: Material Definition with Automatic Differentiation
-Home-page: https://github.com/adtzlr/matadi
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -635,15 +634,15 @@
         
           To do so, attach the following notices to the program.  It is safest
         to attach them to the start of each source file to most effectively
         state the exclusion of warranty; and each file should have at least
         the "copyright" line and a pointer to where the full notice is found.
         
             <one line to give the program's name and a brief idea of what it does.>
-            Copyright (C) 2021  <name of author>
+            Copyright (C) 2023  Andreas Dutzler
         
             This program is free software: you can redistribute it and/or modify
             it under the terms of the GNU General Public License as published by
             the Free Software Foundation, either version 3 of the License, or
             (at your option) any later version.
         
             This program is distributed in the hope that it will be useful,
@@ -655,15 +654,15 @@
             along with this program.  If not, see <https://www.gnu.org/licenses/>.
         
         Also add information on how to contact you by electronic and paper mail.
         
           If the program does terminal interaction, make it output a short
         notice like this when it starts in an interactive mode:
         
-            matadi  Copyright (C) 2021  Andreas Dutzler
+            matadi  Copyright (C) 2023  Andreas Dutzler
             This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
             This is free software, and you are welcome to redistribute it
             under certain conditions; type `show c' for details.
         
         The hypothetical commands `show w' and `show c' should show the appropriate
         parts of the General Public License.  Of course, your program's commands
         might be different; for a GUI interface, you would use an "about box".
@@ -676,46 +675,48 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
-Project-URL: homepage, https://github.com/adtzlr/matadi
-Project-URL: code, https://github.com/adtzlr/matadi
-Project-URL: issues, https://github.com/adtzlr/matadi/issues
+Project-URL: Code, https://github.com/adtzlr/matadi
+Project-URL: Issues, https://github.com/adtzlr/matadi/issues
 Keywords: python,constitution,automatic-differentiation,scientific-computing,fem,finite-elements-analysis,algorithmic-differentiation,hyperelasticity,constitutive-model
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: all
 License-File: LICENSE
+Requires-Dist: casadi
+Requires-Dist: numpy
+Provides-Extra: all
+Requires-Dist: matplotlib; extra == "all"
+Requires-Dist: scipy; extra == "all"
 
-# matADi
-Material Definition with Automatic Differentiation (AD)
-
-![matADi](https://raw.githubusercontent.com/adtzlr/matadi/main/docs/logo/matadi-logo.svg)
+<p align="center">
+  <img src="https://user-images.githubusercontent.com/5793153/235784656-c77d705d-7b4e-4310-bf6e-feb1f1569dce.png" height="80px"/>
+  <p align="center">Material Definition with Automatic Differentiation.</p>
+</p>
 
 [![PyPI version shields.io](https://img.shields.io/pypi/v/matadi.svg)](https://pypi.python.org/pypi/matadi/) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/matadi/branch/main/graph/badge.svg?token=2EY2U4ZL35)](https://codecov.io/gh/adtzlr/matadi) [![DOI](https://zenodo.org/badge/408564756.svg)](https://zenodo.org/badge/latestdoi/408564756) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black) ![GitHub Repo stars](https://img.shields.io/github/stars/adtzlr/matadi?logo=github) ![PyPI - Downloads](https://img.shields.io/pypi/dm/matadi)
 
-matADi is a Python module for the definition of a constitutive hyperelastic material formulation by a strain energy density function. Both [gradient](https://en.wikipedia.org/wiki/Gradient) (stress) and [hessian](https://en.wikipedia.org/wiki/Hessian_matrix) (elasticity tensor) are carried out by [**Automatic Differentiation (AD)**](https://en.wikipedia.org/wiki/Automatic_differentiation) using [casADi](https://web.casadi.org/) [[1](https://doi.org/10.1007/s12532-018-0139-4)] as a backend. A high-level interface for hyperelastic materials based on the deformation gradient exists. Several isotropic hyperelastic material formulations like the Neo-Hookean or the Ogden model are included in the model library. Gradient and hessian methods allow input data with trailing axes which is especially useful for Python-based finite element modules, e.g. [scikit-fem](https://scikit-fem.readthedocs.io/en/latest/) or [FElupe](https://github.com/adtzlr/felupe). Mixed-field formulations suitable for nearly-incompressible material behavior are supported as well as single-field formulations based on the deformation gradient. A numerical lab is included to run, plot and analyze homogenous uniaxial, equi-biaxial, planar shear and simple shear load cases.
+matADi is a 3.8+ Python package for the definition of a constitutive hyperelastic material formulation by a strain energy density function. Both [gradient](https://en.wikipedia.org/wiki/Gradient) (stress) and [hessian](https://en.wikipedia.org/wiki/Hessian_matrix) (elasticity tensor) are carried out by [**Automatic Differentiation (AD)**](https://en.wikipedia.org/wiki/Automatic_differentiation) using [casADi](https://web.casadi.org/) [[1](https://doi.org/10.1007/s12532-018-0139-4)] as a backend. A high-level interface for hyperelastic materials based on the deformation gradient exists. Several isotropic hyperelastic material formulations like the Neo-Hookean or the Ogden model are included in the model library. Gradient and hessian methods allow input data with trailing axes which is especially useful for Python-based finite element modules, e.g. [scikit-fem](https://scikit-fem.readthedocs.io/en/latest/) or [FElupe](https://github.com/adtzlr/felupe). Mixed-field formulations suitable for nearly-incompressible material behavior are supported as well as single-field formulations based on the deformation gradient. A numerical lab is included to run, plot and analyze homogeneous uniaxial, equi-biaxial, planar shear and simple shear load cases.
 
 ## Installation
 Install `matADi` from PyPI via pip.
 
 ```shell
 pip install matadi
 ```
@@ -805,64 +806,64 @@
 W_upJ = NH_upJ.function([defgrad, pressure, volratio])
 P_upJ = NH_upJ.gradient([defgrad, pressure, volratio])
 A_upJ = NH_upJ.hessian([defgrad, pressure, volratio])
 ```
 
 The output of `NH_upJ.gradient([defgrad, pressure, volratio])` is a list with gradients of the functional as `[dWdF, dWdp, dWdJ]`. Hessian entries are provided as a list of upper triangle entries, e.g. `NH_upJ.hessian([defgrad, pressure, volratio])` returns `[d2WdFdF, d2WdFdp, d2WdFdJ, d2Wdpdp, d2WdpdJ, d2WdJdJ]`.
 
-Available [isotropic hyperelastic material models](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py):
-- [Linear Elastic](https://en.wikipedia.org/wiki/Linear_elasticity) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py#L5-L7))
-- [Saint Venant Kirchhoff](https://en.wikipedia.org/wiki/Hyperelastic_material#Saint_Venant%E2%80%93Kirchhoff_model) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py#L10-L14))
-- [Neo-Hooke](https://en.wikipedia.org/wiki/Neo-Hookean_solid) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py#L17-L21))
-- [Mooney-Rivlin](https://en.wikipedia.org/wiki/Mooney%E2%80%93Rivlin_solid) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py#L24-L29))
-- [Yeoh](https://en.wikipedia.org/wiki/Yeoh_(hyperelastic_model)) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py#L32-L37))
-- [Third-Order-Deformation (James-Green-Simpson)](https://onlinelibrary.wiley.com/doi/abs/10.1002/app.1975.070190723) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py#L40-L51))
-- [Ogden](https://en.wikipedia.org/wiki/Ogden_(hyperelastic_model)) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py#L54-L64))
-- [Arruda-Boyce](https://en.wikipedia.org/wiki/Arruda%E2%80%93Boyce_model) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py#L67-L80))
-- [Extended-Tube](https://meridian.allenpress.com/rct/article-abstract/72/4/602/92819/An-Extended-Tube-Model-for-Rubber-Elasticity?redirectedFrom=fulltext) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py#L83-L91))
-- [Van-der-Waals (Kilian)](https://doi.org/10.1016/0032-3861(81)90200-7) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_isotropic.py#L94-L103))
-
-Available [anisotropic hyperelastic material models](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_anisotropic.py):
-- Fiber ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_anisotropic.py#L17-L35))
-- Fiber-family (+/- combination of single Fiber) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_anisotropic.py#L38-L45))
-- [Holzapfel Gasser Ogden](https://royalsocietypublishing.org/doi/full/10.1098/rsif.2005.0073) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_hyperelasticity_anisotropic.py#L48-L77))
-
-Available [micro-sphere hyperelastic frameworks](https://github.com/adtzlr/matadi/blob/main/matadi/models/microsphere) (Miehe, Göktepe, Lulei) [[2](https://doi.org/10.1016/j.jmps.2004.03.011)]:
-- [affine stretch](https://doi.org/10.1016/j.jmps.2004.03.011) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/microsphere/affine/_models.py#L6-L16))
-- [affine tube](https://doi.org/10.1016/j.jmps.2004.03.011) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/microsphere/affine/_models.py#L19-L30))
-- [non-affine stretch](https://doi.org/10.1016/j.jmps.2004.03.011) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/microsphere/nonaffine/_models.py#L7-L17))
-- [non-affine tube](https://doi.org/10.1016/j.jmps.2004.03.011) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/microsphere/nonaffine/_models.py#L20-L32))
+Available [isotropic hyperelastic material models](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py):
+- [Linear Elastic](https://en.wikipedia.org/wiki/Linear_elasticity) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py#L5-L7))
+- [Saint Venant Kirchhoff](https://en.wikipedia.org/wiki/Hyperelastic_material#Saint_Venant%E2%80%93Kirchhoff_model) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py#L10-L14))
+- [Neo-Hooke](https://en.wikipedia.org/wiki/Neo-Hookean_solid) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py#L17-L21))
+- [Mooney-Rivlin](https://en.wikipedia.org/wiki/Mooney%E2%80%93Rivlin_solid) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py#L24-L29))
+- [Yeoh](https://en.wikipedia.org/wiki/Yeoh_(hyperelastic_model)) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py#L32-L37))
+- [Third-Order-Deformation (James-Green-Simpson)](https://onlinelibrary.wiley.com/doi/abs/10.1002/app.1975.070190723) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py#L40-L51))
+- [Ogden](https://en.wikipedia.org/wiki/Ogden_(hyperelastic_model)) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py#L54-L64))
+- [Arruda-Boyce](https://en.wikipedia.org/wiki/Arruda%E2%80%93Boyce_model) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py#L67-L80))
+- [Extended-Tube](https://meridian.allenpress.com/rct/article-abstract/72/4/602/92819/An-Extended-Tube-Model-for-Rubber-Elasticity?redirectedFrom=fulltext) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py#L83-L91))
+- [Van-der-Waals (Kilian)](https://doi.org/10.1016/0032-3861(81)90200-7) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_isotropic.py#L94-L103))
+
+Available [anisotropic hyperelastic material models](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_anisotropic.py):
+- Fiber ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_anisotropic.py#L17-L35))
+- Fiber-family (+/- combination of single Fiber) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_anisotropic.py#L38-L45))
+- [Holzapfel Gasser Ogden](https://royalsocietypublishing.org/doi/full/10.1098/rsif.2005.0073) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_hyperelasticity_anisotropic.py#L48-L77))
+
+Available [micro-sphere hyperelastic frameworks](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/microsphere) (Miehe, Göktepe, Lulei) [[2](https://doi.org/10.1016/j.jmps.2004.03.011)]:
+- [affine stretch](https://doi.org/10.1016/j.jmps.2004.03.011) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/microsphere/affine/_models.py#L6-L16))
+- [affine tube](https://doi.org/10.1016/j.jmps.2004.03.011) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/microsphere/affine/_models.py#L19-L30))
+- [non-affine stretch](https://doi.org/10.1016/j.jmps.2004.03.011) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/microsphere/nonaffine/_models.py#L7-L17))
+- [non-affine tube](https://doi.org/10.1016/j.jmps.2004.03.011) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/microsphere/nonaffine/_models.py#L20-L32))
 
-Available [micro-sphere hyperelastic material models](https://github.com/adtzlr/matadi/blob/main/matadi/models/microsphere) (Miehe, Göktepe, Lulei) [[2](https://doi.org/10.1016/j.jmps.2004.03.011)]:
-- [Miehe Göktepe Lulei](https://doi.org/10.1016/j.jmps.2004.03.011) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/microsphere/nonaffine/_models.py#L35-L49))
+Available [micro-sphere hyperelastic material models](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/microsphere) (Miehe, Göktepe, Lulei) [[2](https://doi.org/10.1016/j.jmps.2004.03.011)]:
+- [Miehe Göktepe Lulei](https://doi.org/10.1016/j.jmps.2004.03.011) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/microsphere/nonaffine/_models.py#L35-L49))
 
 Any user-defined isotropic hyperelastic strain energy density function may be passed as the `fun` argument of `MaterialHyperelastic` by using the following template:
 
 ```python
 def fun(F, **kwargs):
     # user code
     return W
 ```
 
-In order to apply the above material model only on the isochoric part of the deformation gradient [[3](https://doi.org/10.1016/0045-7825(85)90033-7)], use the decorator [`@isochoric_volumetric_split`](https://github.com/adtzlr/matadi/blob/main/matadi/models/_helpers.py#L7-L31). If the keyword `bulk` is passed, an additional [volumetric strain energy function](https://github.com/adtzlr/matadi/blob/main/matadi/models/_helpers.py#L34-L35) is added to the base material formulation.
+In order to apply the above material model only on the isochoric part of the deformation gradient [[3](https://doi.org/10.1016/0045-7825(85)90033-7)], use the decorator [`@isochoric_volumetric_split`](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_helpers.py#L7-L31). If the keyword `bulk` is passed, an additional [volumetric strain energy function](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_helpers.py#L34-L35) is added to the base material formulation.
 
 ```python
 from matadi.models import isochoric_volumetric_split
 from matadi.math import trace, transpose
 
 @isochoric_volumetric_split
 def nh(F, C10=0.5):
     # user code of strain energy function, e.g. neo-hooke
     return C10 * (trace(transpose(F) @ F) - 3)
 
 NH = MaterialHyperelastic(nh, C10=0.5, bulk=200.0)
 ```
 
 ## Lab
-In matADi's `Lab` :lab_coat: numeric experiments on homogenous loadcases on compressible or nearly-incompressible material formulations are performed. For incompressible materials use `LabIncompressible` instead. Let's take the non-affine micro-sphere material model suitable for rubber elasticity with parameters from [[2](https://doi.org/10.1016/j.jmps.2004.03.011), Fig. 19] and run **uniaxial**, **biaxial** and **planar shear** tests.
+In matADi's `Lab` :lab_coat: numeric experiments on homogeneous loadcases on compressible or nearly-incompressible material formulations are performed. For incompressible materials use `LabIncompressible` instead. Let's take the non-affine micro-sphere material model suitable for rubber elasticity with parameters from [[2](https://doi.org/10.1016/j.jmps.2004.03.011), Fig. 19] and run **uniaxial**, **biaxial** and **planar shear** tests.
 
 ```python
 from matadi import Lab, MaterialHyperelastic
 from matadi.models import miehe_goektepe_lulei
 
 mat = MaterialHyperelastic(
     miehe_goektepe_lulei, 
@@ -897,21 +898,26 @@
 b) the monotonic increasing slope of force per undeformed area vs. stretch and
 c) the sign of the resulting stretch from a small superposed force in one direction.
 
 ## Hints and usage in FEM modules
 For tensor-valued material definitions use `MaterialTensor` (e.g. any stress-strain relation). Also, please have a look at [casADi's documentation](https://web.casadi.org/). It is very powerful but unfortunately does not support all the Python stuff you would expect. For example Python's default if-else-statements can't be used in combination with symbolic conditions (use `math.if_else(cond, if_true, if_false)` instead). Contrary to [casADi](https://web.casadi.org/), the gradient of the eigenvalue function is stabilized by a perturbation of the diagonal components.
 
 ### A **Material** with state variables
-A generalized material model with optional state variables for the (u/p)-formulation is created by an instance of `MaterialTensor`. If the argument `triu` is set to `True` the gradient method returns only the upper triangle entries of the gradient components. If some of the input variables are internal state variables the number of these variables have to be passed to the optional argument `statevars`. While the hyperelastic material classes are defined by a strain energy function, this one is defined by the first Piola-Kirchhoff stress tensor. Internally, state variables are equal to default variables but they are excluded from gradient calculations. State variables may also be used as placeholders for additional quantities, e.g. the initial deformation gradient at the beginning of an increment or the time increment. Hence, it is a very flexible class not restricted to hyperelasticity.
+A generalized material model with optional state variables, optionally for the (u/p)-formulation, is created by an instance of `MaterialTensor`. If the argument `triu` is set to `True` the gradient method returns only the upper triangle entries of the gradient components. If some of the input variables are internal state variables the number of these variables have to be passed to the optional argument `statevars`. While the hyperelastic material classes are defined by a strain energy function, this one is defined by the first Piola-Kirchhoff stress tensor. Internally, state variables are equal to default variables but they are excluded from gradient calculations. State variables may also be used as placeholders for additional quantities, e.g. the initial deformation gradient at the beginning of an increment or the time increment. Hence, it is a very flexible class not restricted to hyperelasticity. For consistency, the methods `gradient` and `hessian` of a tensor-based material refer to the gradient and hessian of the strain energy function.
+
+Included [pseudo-elastic material models](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_pseudo_elasticity.py):
+- [Ogden-Roxburgh](https://doi.org/10.1098%2Frspa.1999.0431) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_pseudo_elasticity.py#L4-L16))
 
-Included [pseudo-elastic material models](https://github.com/adtzlr/matadi/blob/main/matadi/models/_pseudo_elasticity.py):
-- [Ogden-Roxburgh](https://doi.org/10.1098%2Frspa.1999.0431) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_pseudo_elasticity.py#L4-L16))
 
-Included [other material models](https://github.com/adtzlr/matadi/blob/main/matadi/models/_misc.py):
-- [MORPH](https://doi.org/10.1016/S0749-6419(02)00091-8) ([code](https://github.com/adtzlr/matadi/blob/main/matadi/models/_misc.py#L19-L75))
+Included [viscoelastic material models](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_viscoelasticity.py):
+- [Finite-Strain-Viscoelastic](https://doi.org/10.1016/j.cma.2013.07.004) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_viscoelasticity.py#L4-L18))
+- [Finite-Strain-Viscoelastic (Mooney-Rivlin)](https://doi.org/10.1002/nme.5724) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_viscoelasticity.py#L21-L51))
+
+Included [other material models](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_misc.py):
+- [MORPH](https://doi.org/10.1016/S0749-6419(02)00091-8) ([code](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_misc.py#L19-L75))
 
 ```python
 import numpy as np
 
 from matadi.models import (
     displacement_pressure_split, neo_hooke, volumetric, ogden_roxburgh
 )
@@ -950,22 +956,30 @@
 defgrad = np.random.rand(3, 3, 5, 100) - 0.5
 pressure = np.random.rand(1, 5, 100)
 statevars = np.random.rand(1, 1, 5, 100)
 
 for a in range(3):
     defgrad[a, a] += 1.0
 
-dWdF, dWdp, statevars_new = NH.function([defgrad, pressure, statevars])
-d2WdFdF, d2WdFdp, d2Wdpdp = NH.gradient([defgrad, pressure, statevars])
+dWdF, dWdp, statevars_new = NH.gradient([defgrad, pressure, statevars])
+d2WdFdF, d2WdFdp, d2Wdpdp = NH.hessian([defgrad, pressure, statevars])
 ```
 
-**Hint**: *The above Neo-Hooke as well as the MORPH material model formulation within the u/p-framework are available as template-materials in `matadi.models` as `NeoHookeOgdenRoxburgh()`and `Morph()`. The state variable concept is also implemented for the `Material` class.*
+The Neo-Hooke, the MORPH and the Finite-Strain-Viscoelastic [[4](https://doi.org/10.1016/j.cma.2013.07.004)] material model formulations are available as ready-to-go materials in `matadi.models` as:
+
+* [`NeoHookeOgdenRoxburgh()`](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_templates.py), 
+* [`Morph()`](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_templates.py),
+* [`Viscoelastic()`](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_templates.py) and
+* [`ViscoelasticMooneyRivlin()`](https://github.com/adtzlr/matadi/blob/main/src/matadi/models/_templates.py).
+
+**Hint**: *The state variable concept is also implemented for the `Material` class.*
 
 Simple examples for using `matadi` with [`scikit-fem`](https://github.com/adtzlr/matadi/discussions/14#) as well as with [`felupe`](https://github.com/adtzlr/matadi/discussions/22) are shown in the Discussion section.
 
 ## References
 [1] J. A. E. Andersson, J. Gillis, G. Horn, J. B. Rawlings, and M. Diehl, *CasADi - A software framework for nonlinear optimization and optimal control*, Math. Prog. Comp., vol. 11, no. 1, pp. 1–36, 2019, [![DOI:10.1007/s12532-018-0139-4](https://zenodo.org/badge/DOI/10.1007/s12532-018-0139-4.svg)](https://doi.org/10.1007/s12532-018-0139-4)
 
 [2] C. Miehe, S. Göktepe and F. Lulei, *A micro-macro approach to rubber-like materials. Part I: the non-affine micro-sphere model of rubber elasticity*, Journal of the Mechanics and Physics of Solids, vol. 52, no. 11. Elsevier BV, pp. 2617–2660, Nov. 2004. [![DOI:10.1016/j.jmps.2004.03.011](https://zenodo.org/badge/DOI/10.1016/j.jmps.2004.03.011.svg)](https://doi.org/10.1016/j.jmps.2004.03.011)
 
 [3] J. C. Simo, R. L. Taylor, and K. S. Pister, *Variational and projection methods for the volume constraint in finite deformation elasto-plasticity*, Computer Methods in Applied Mechanics and Engineering, vol. 51, no. 1–3, pp. 177–208, Sep. 1985, [![DOI:10.1016/0045-7825(85)90033-7](https://zenodo.org/badge/DOI/10.1016/0045-7825(85)90033-7.svg)](https://doi.org/10.1016/0045-7825(85)90033-7)
 
+[4] A. V. Shutov, R. Landgraf, and J. Ihlemann, *An explicit solution for implicit time stepping in multiplicative finite strain viscoelasticity*, Computer Methods in Applied Mechanics and Engineering, vol. 265. Elsevier BV, pp. 213–225, Oct. 2013, [![DOI:10.1016/j.cma.2013.07.004](https://zenodo.org/badge/DOI/10.1016/j.cma.2013.07.004.svg)](https://doi.org/10.1016/j.cma.2013.07.004)
```

### Comparing `matadi-0.1.9/matadi.egg-info/SOURCES.txt` & `matadi-0.2.0/src/matadi.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 LICENSE
 README.md
 pyproject.toml
-setup.cfg
-matadi/__about__.py
-matadi/__init__.py
-matadi/_apply.py
-matadi/_lab_compressible.py
-matadi/_lab_incompressible.py
-matadi/_material.py
-matadi/_templates.py
-matadi/math.py
-matadi.egg-info/PKG-INFO
-matadi.egg-info/SOURCES.txt
-matadi.egg-info/dependency_links.txt
-matadi.egg-info/requires.txt
-matadi.egg-info/top_level.txt
-matadi/models/__init__.py
-matadi/models/_helpers.py
-matadi/models/_hyperelasticity_anisotropic.py
-matadi/models/_hyperelasticity_isotropic.py
-matadi/models/_misc.py
-matadi/models/_pseudo_elasticity.py
-matadi/models/_templates.py
-matadi/models/microsphere/__init__.py
-matadi/models/microsphere/_chain.py
-matadi/models/microsphere/affine/__init__.py
-matadi/models/microsphere/affine/_models.py
-matadi/models/microsphere/nonaffine/__init__.py
-matadi/models/microsphere/nonaffine/_models.py
-matadi/models/microsphere/quadrature/__init__.py
-matadi/models/microsphere/quadrature/_bazant_oh.py
-tests/__init__.py
+src/matadi/__about__.py
+src/matadi/__init__.py
+src/matadi/_apply.py
+src/matadi/_lab_compressible.py
+src/matadi/_lab_incompressible.py
+src/matadi/_material.py
+src/matadi/_templates.py
+src/matadi/_variable.py
+src/matadi/math.py
+src/matadi.egg-info/PKG-INFO
+src/matadi.egg-info/SOURCES.txt
+src/matadi.egg-info/dependency_links.txt
+src/matadi.egg-info/requires.txt
+src/matadi.egg-info/top_level.txt
+src/matadi/models/__init__.py
+src/matadi/models/_helpers.py
+src/matadi/models/_hyperelasticity_anisotropic.py
+src/matadi/models/_hyperelasticity_isotropic.py
+src/matadi/models/_misc.py
+src/matadi/models/_pseudo_elasticity.py
+src/matadi/models/_templates.py
+src/matadi/models/_viscoelasticity.py
+src/matadi/models/microsphere/__init__.py
+src/matadi/models/microsphere/_chain.py
+src/matadi/models/microsphere/affine/__init__.py
+src/matadi/models/microsphere/affine/_models.py
+src/matadi/models/microsphere/nonaffine/__init__.py
+src/matadi/models/microsphere/nonaffine/_models.py
+src/matadi/models/microsphere/quadrature/__init__.py
+src/matadi/models/microsphere/quadrature/_bazant_oh.py
 tests/test_displacement-pressure.py
 tests/test_eigvals_grad.py
 tests/test_fiber.py
 tests/test_lab.py
 tests/test_microsphere.py
 tests/test_models.py
 tests/test_plane.py
```

### Comparing `matadi-0.1.9/pyproject.toml` & `matadi-0.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,61 +1,56 @@
+[build-system]
+requires = ["setuptools>=61"]
+build-backend = "setuptools.build_meta"
+
+[tool.isort]
+profile = "black"
+
 [project]
 name = "matadi"
-version = "0.1.9"
+authors = [
+  {email = "a.dutzler@gmail.com"},
+  {name = "Andreas Dutzler"}
+]
 description = "Material Definition with Automatic Differentiation"
 readme = "README.md"
-requires-python = ">=3.6"
 license = {file = "LICENSE"}
 keywords = [
   "python", 
   "constitution", 
   "automatic-differentiation", 
   "scientific-computing", 
   "fem", 
   "finite-elements-analysis", 
   "algorithmic-differentiation", 
   "hyperelasticity", 
   "constitutive-model"
 ]
-
-authors = [
-  {email = "a.dutzler@gmail.com"},
-  {name = "Andreas Dutzler"}
-]
-
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Programming Language :: Python",
   "Intended Audience :: Science/Research",
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.6",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Topic :: Scientific/Engineering",
   "Topic :: Scientific/Engineering :: Mathematics",
   "Topic :: Utilities"
 ]
-
-dependencies = [
-  "casadi",
-  "numpy"
-]
+dynamic = ["version"]
+requires-python = ">=3.7"
+dependencies = ["casadi", "numpy"]
 
 [project.optional-dependencies]
-all = [
-    "matplotlib",
-    "scipy"
-]
+all = ["matplotlib", "scipy"]
 
-[project.urls]
-homepage = "https://github.com/adtzlr/matadi"
-code = "https://github.com/adtzlr/matadi"
-issues = "https://github.com/adtzlr/matadi/issues"
+[tool.setuptools.dynamic]
+version = {attr = "matadi.__about__.__version__"}
 
-[build-system]
-requires = ["setuptools>=42", "wheel"]
-build-backend = "setuptools.build_meta"
+[project.urls]
+Code = "https://github.com/adtzlr/matadi"
+Issues = "https://github.com/adtzlr/matadi/issues"
```

### Comparing `matadi-0.1.9/tests/test_fiber.py` & `matadi-0.2.0/tests/test_fiber.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import numpy as np
 
-from matadi import Variable, MaterialHyperelastic
+from matadi import MaterialHyperelastic, Variable
+from matadi.math import det, invariants, sqrt, trace, transpose
 from matadi.models import fiber, fiber_family, holzapfel_gasser_ogden
-from matadi.math import det, transpose, trace, invariants, sqrt
 
 
 def test_fiber():
-
     # data
     FF = np.zeros((3, 3, 2))
     for a in range(3):
         FF[a, a] += 1
 
     for model in [fiber, fiber_family]:
-
         # init Material without bulk
         M = MaterialHyperelastic(model, E=1, angle=30, axis=2, k=0)
 
         W0 = M.function([FF])
         assert W0[0].shape == (1, 1, 2)
 
         # init Material
@@ -39,22 +37,20 @@
             3,
             3,
             2,
         )
 
 
 def test_hgo():
-
     # data
     FF = np.zeros((3, 3, 2))
     for a in range(3):
         FF[a, a] += 1
 
     for model in [holzapfel_gasser_ogden]:
-
         # init Material without bulk
         M = MaterialHyperelastic(
             model, c=0.0764, k1=996.6, k2=524.6, kappa=0.2, angle=49.98, axis=2
         )
 
         # init Material
         M = MaterialHyperelastic(
```

### Comparing `matadi-0.1.9/tests/test_lab.py` & `matadi-0.2.0/tests/test_lab.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from matadi import MaterialHyperelastic, Lab, LabCompressible, LabIncompressible
-import matadi.models as md
-from matadi.models import neo_hooke, extended_tube, van_der_waals, mooney_rivlin
-
 import matplotlib.pyplot as plt
-
 import pytest
 
+import matadi.models as md
+from matadi import Lab, LabCompressible, LabIncompressible, MaterialHyperelastic
+from matadi.models import extended_tube, mooney_rivlin, neo_hooke, van_der_waals
+
 
 def library():
     "Library with models and parameters."
 
     database = {
         md.saint_venant_kirchhoff: {"mu": 1.0, "lmbda": 20.0},
         md.neo_hooke: {"C10": 0.5},
@@ -39,15 +38,14 @@
     plot=False,
     plot_shear=False,
     close=True,
     run_all=False,
     run_kwargs={},
     LabClass=Lab,
 ):
-
     lib = library()
     kwargs = lib[model]
 
     if test_without_bulk:
         # init material without bulk modulus
         mat = MaterialHyperelastic(model, **kwargs)
 
@@ -91,17 +89,15 @@
         data_x = lab.run(ux=True, bx=True, ps=True, shear=False, num=num, **run_kwargs)
         lab.plot_shear(data_x)
 
     return data
 
 
 def test_lab():
-
     for LabClass in [LabIncompressible, LabCompressible, Lab]:
-
         data = pre(neo_hooke, test_without_bulk=True, LabClass=LabClass)
         data = pre(
             neo_hooke,
             run_all=True,
             plot=True,
             plot_shear=True,
             close=True,
```

### Comparing `matadi-0.1.9/tests/test_microsphere.py` & `matadi-0.2.0/tests/test_microsphere.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,50 +1,45 @@
 import numpy as np
 
 from matadi import MaterialTensor, Variable
-from matadi.models.microsphere.affine import force
+from matadi.models.microsphere import affine
 
 
-def nh(stretch, stretch_n, statevars_n, mu=1.0):
+def nh(stretch, statevars_n, mu=1.0):
     "1d-Linear force-stretch consitututive material formulation."
 
     return 3 * mu * stretch, statevars_n
 
 
 def test_microsphere_force():
-
-    param = [nh, 1.0]
-
     F = Variable("F", 3, 3)
     Fn = Variable("Fn", 3, 3)
-    Zn = Variable("Zn", 2, 21)
+    Zn = Variable("Zn", 5, 21)
 
     umat = MaterialTensor(
-        x=[F, force.p, Fn, Zn],
-        fun=force,
-        args=param,
-        kwargs={"bulk": 5000},
-        statevars=2,
+        x=[F, affine.force.p, Zn],
+        fun=affine.force,
+        kwargs={"f": nh, "mu": 1.0, "bulk": 5000},
+        statevars=1,
         triu=True,
     )
 
     F = np.random.rand(3, 3, 8, 100) / 2
-    Fn = np.random.rand(3, 3, 8, 100) / 2
     p = np.random.rand(1, 8, 100)
-    Zn = np.random.rand(2, 21, 8, 100)
+    Zn = np.random.rand(5, 21, 8, 100)
 
     for a in range(3):
         F[a, a] += 1
         Fn[a, a] += 1
 
-    P, Q, Z = umat.function([F, p, Fn, Zn])
-    A = umat.gradient([F, p, Fn, Zn])
+    P, Q, Z = umat.function([F, p, Zn])
+    A = umat.gradient([F, p, Zn])
 
     assert P.shape == (3, 3, 8, 100)
     assert Q.shape == (1, 1, 8, 100)
-    assert Z.shape == (2, 21, 8, 100)
+    assert Z.shape == (5, 21, 8, 100)
 
     assert len(A) == 3
 
 
 if __name__ == "__main__":
     test_microsphere_force()
```

### Comparing `matadi-0.1.9/tests/test_models.py` & `matadi-0.2.0/tests/test_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,15 +64,14 @@
         },
     }
 
     return database
 
 
 def test_models():
-
     # data
     np.random.seed(2345537)
     dF = np.random.rand(3, 3, 5, 100) - 0.5
     DF = np.random.rand(3, 3, 5, 100) - 0.5
     FF = np.random.rand(3, 3, 5, 100) - 0.5
     for a in range(3):
         FF[a, a] += 1
@@ -84,15 +83,14 @@
     JJ = 1 + np.random.rand(5, 100) / 10
     dJ = np.random.rand(5, 100) / 10
     DJ = np.random.rand(5, 100) / 10
 
     lib = library()
 
     for model, kwargs in lib.items():
-
         if model not in [md.saint_venant_kirchhoff, md.linear_elastic]:
             kwargs["bulk"] = 5000.0
 
         HM = matadi.MaterialHyperelastic(model, **kwargs)
         HM_mixed = matadi.ThreeFieldVariation(HM)
         HM_mixed2 = matadi.TwoFieldVariation(HM)
 
@@ -100,29 +98,29 @@
         P = HM.gradient([FF], threads=1)
         A = HM.hessian([FF])
 
         dW = HM.gradient_vector_product([FF], [dF])
         DW = HM.hessian_vector_product([FF], [dF], [DF])
 
         assert len(W) == 1
-        assert len(P) == 1
+        assert len(P) == 1 + 1
         assert len(A) == 1
 
         dW_check = np.einsum("ij...,ij...->...", P[0], dF)
         DW_check = np.einsum("ij...,ijkl...,kl...->...", dF, A[0], DF)
 
         assert np.allclose(dW_check, dW[0])
         assert np.allclose(DW_check, DW[0])
 
         W = HM_mixed.function([FF, pp, JJ])
         P = HM_mixed.gradient([FF, pp, JJ])
         A = HM_mixed.hessian([FF, pp, JJ])
 
         assert len(W) == 1
-        assert len(P) == 3
+        assert len(P) == 3 + 1
         assert len(A) == 6
 
         dW = HM_mixed.gradient_vector_product([FF, pp, JJ], [dF, dp, dJ])
         DW = HM_mixed.hessian_vector_product([FF, pp, JJ], [dF, dp, dJ], [DF, Dp, DJ])
 
         dWF = np.einsum("ij...,ij...->...", P[0], dF)
         dWp = P[1] * dp
@@ -152,15 +150,15 @@
         assert np.allclose(dWdJdJ, DW[5])
 
         W = HM_mixed2.function([FF, pp])
         P = HM_mixed2.gradient([FF, pp])
         A = HM_mixed2.hessian([FF, pp])
 
         assert len(W) == 1
-        assert len(P) == 2
+        assert len(P) == 2 + 1
         assert len(A) == 3
 
         dW = HM_mixed2.gradient_vector_product([FF, pp], [dF, dp])
         DW = HM_mixed2.hessian_vector_product([FF, pp], [dF, dp], [DF, Dp])
 
         dWF = np.einsum("ij...,ij...->...", P[0], dF)
         dWp = P[1] * dp
@@ -190,39 +188,39 @@
     comp.fun()
 
     W = comp.function([FF])
     P = comp.gradient([FF])
     A = comp.hessian([FF])
 
     assert len(W) == 1
-    assert len(P) == 1
+    assert len(P) == 1 + 1
     assert len(A) == 1
 
     nh_mixed = matadi.ThreeFieldVariation(nh)
     mr_mixed = matadi.ThreeFieldVariation(mr)
 
     comp = matadi.MaterialComposite([nh_mixed, mr_mixed])
 
     W = comp.function([FF, pp, JJ])
     P = comp.gradient([FF, pp, JJ])
     A = comp.hessian([FF, pp, JJ])
 
     assert len(W) == 1
-    assert len(P) == 3
+    assert len(P) == 3 + 1
     assert len(A) == 6
 
     nh_mixed2 = matadi.TwoFieldVariation(nh)
     mr_mixed2 = matadi.TwoFieldVariation(mr)
 
     comp = matadi.MaterialComposite([nh_mixed2, mr_mixed2])
 
     W = comp.function([FF, pp])
     P = comp.gradient([FF, pp])
     A = comp.hessian([FF, pp])
 
     assert len(W) == 1
-    assert len(P) == 2
+    assert len(P) == 2 + 1
     assert len(A) == 3
 
 
 if __name__ == "__main__":
     test_models()
```

### Comparing `matadi-0.1.9/tests/test_plane.py` & `matadi-0.2.0/tests/test_plane.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,40 +3,37 @@
 from matadi import (
     MaterialHyperelasticPlaneStrain,
     MaterialHyperelasticPlaneStressIncompressible,
     MaterialHyperelasticPlaneStressLinearElastic,
     ThreeFieldVariationPlaneStrain,
     TwoFieldVariationPlaneStrain,
 )
-from matadi.models import neo_hooke, linear_elastic
+from matadi.models import linear_elastic, neo_hooke
 
 
 def pre():
-
     FF = np.random.rand(2, 2, 8, 1000)
     for a in range(2):
         FF[a, a] += 1
 
     return FF
 
 
 def pre_mixed():
-
     FF = np.random.rand(2, 2, 8, 1000)
     for a in range(2):
         FF[a, a] += 1
 
     pp = np.random.rand(1, 1, 8, 1000)
     JJ = np.random.rand(1, 1, 8, 1000) + 1
 
     return FF, pp, JJ
 
 
 def test_plane_strain():
-
     # data
     FF = pre()
 
     # init Material
     W = MaterialHyperelasticPlaneStrain(
         fun=neo_hooke,
         C10=0.5,
@@ -52,15 +49,14 @@
 
     assert W0[0].shape == (1, 1, 8, 1000)
     assert dW[0].shape == (2, 2, 8, 1000)
     assert DW[0].shape == (2, 2, 2, 2, 8, 1000)
 
 
 def test_plane_strain_mixed():
-
     # data
     FF, pp, JJ = pre_mixed()
 
     # init Material
     W = MaterialHyperelasticPlaneStrain(
         fun=neo_hooke,
         C10=0.5,
@@ -92,15 +88,14 @@
 
     assert W0[0].shape == (1, 1, 8, 1000)
     assert dW[0].shape == (2, 2, 8, 1000)
     assert DW[0].shape == (2, 2, 2, 2, 8, 1000)
 
 
 def test_plane_stress_incompr():
-
     # data
     FF = pre()
 
     # init Material
     W = MaterialHyperelasticPlaneStressIncompressible(
         fun=neo_hooke,
         C10=0.5,
@@ -116,15 +111,14 @@
 
     assert W0[0].shape == (1, 1, 8, 1000)
     assert dW[0].shape == (2, 2, 8, 1000)
     assert DW[0].shape == (2, 2, 2, 2, 8, 1000)
 
 
 def test_plane_stress_linear():
-
     # data
     FF = pre()
 
     # init Material
     W = MaterialHyperelasticPlaneStressLinearElastic(
         fun=linear_elastic,
         mu=1.0,
```

### Comparing `matadi-0.1.9/tests/test_scalar.py` & `matadi-0.2.0/tests/test_scalar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import numpy as np
 
-from matadi import Variable, Material
-from matadi.math import det, transpose, trace
+from matadi import Material, Variable
+from matadi.math import det, trace, transpose
 
 
 def test_scalar():
-
     # variables
     F = Variable("F", 3, 3)
     p = Variable("p", 1)
     J = Variable("J", 1)
 
     def neohooke(x, mu=1.0, bulk=200.0):
         "Strain energy function of nearly-incompressible Neo-Hookean material."
@@ -59,15 +58,14 @@
     )
 
     dW = W.gradient([FF, pp, JJ])
     DW = W.hessian([FF, pp, JJ])
 
 
 def test_scalar_compress():
-
     # variables
     F = Variable("F", 3, 3)
     p = Variable("p", 1)
     J = Variable("J", 1)
 
     def neohooke(x, mu=1.0, bulk=200.0):
         "Strain energy function of nearly-incompressible Neo-Hookean material."
```

### Comparing `matadi-0.1.9/tests/test_simple.py` & `matadi-0.2.0/tests/test_simple.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 
-from matadi import Variable, Material, MaterialTensor
-from matadi.math import det, transpose, trace, invariants, sqrt, dev, ddot
+from matadi import Material, MaterialTensor, Variable
+from matadi.math import ddot, det, dev, invariants, sqrt, trace, transpose
 
 
 def neohooke(x, mu=1.0, bulk=200.0):
     """Strain energy density function of nearly-incompressible
     Neo-Hookean isotropic hyperelastic material formulation."""
 
     F = x[0]
@@ -20,15 +20,14 @@
 
 
 def nh_aslist(x, mu=1.0, bulk=200.0):
     return [neohooke(x, mu, bulk)]
 
 
 def test_simple():
-
     # variables
     F = Variable("F", 3, 3)
 
     # data
     FF = np.random.rand(3, 3, 8, 1000)
     for a in range(3):
         FF[a, a] += 1
@@ -69,15 +68,14 @@
     # test single value input
     W00 = W.function([FF[:, :, 0, 0]])
 
     assert W00[0].shape == (1,)
 
 
 def test_tensor():
-
     # variables
     F = Variable("F", 3, 3)
     p = Variable("p", 1, 1)
     z = Variable("z", 5, 16)
 
     # data
     FF = np.random.rand(3, 3, 8, 1000)
@@ -85,69 +83,64 @@
     zz = np.random.rand(5, 16, 8, 1000)
 
     for a in range(3):
         FF[a, a] += 1
 
     # init Material
     for fun in [lambda x: dev(x[0]) + ddot(x[0], x[0]), lambda x: x]:
-
         W = MaterialTensor(x=[F], fun=fun)
 
-        W0 = W.function([FF])
-        dW = W.gradient([FF])
-        DW = W.jacobian([FF])
-
+        W0 = W.gradient([FF])
+        dW = W.hessian([FF])
         # dW and DW are always lists...
         assert W0[0].shape == (3, 3, 8, 1000)
         assert dW[0].shape == (3, 3, 3, 3, 8, 1000)
-        assert DW[0].shape == (3, 3, 3, 3, 8, 1000)
 
         # check output of parallel evaluation
-        W0 = W.function([FF], threads=2)
-        dW = W.gradient([FF], threads=2)
-        DW = W.jacobian([FF], threads=2)
+        W0 = W.gradient([FF], threads=2)
+        dW = W.hessian([FF], threads=2)
 
         assert W0[0].shape == (3, 3, 8, 1000)
         assert dW[0].shape == (3, 3, 3, 3, 8, 1000)
 
     # init Material
     pp = np.random.rand(8, 1000)
 
     W = MaterialTensor(x=[p], fun=lambda x: x[0], compress=True)
-    W0 = W.function([pp], threads=2)
+    W0 = W.gradient([pp], threads=2)
 
     assert W0[0].shape == (8, 1000)
 
     pp = np.random.rand(1, 1, 8, 1000)
 
     W = MaterialTensor(x=[p], fun=lambda x: x[0])
-    W0 = W.function([pp])
+    W0 = W.gradient([pp])
 
     assert W0[0].shape == (1, 1, 8, 1000)
 
     # init mixed Material with upper triangle gradient
     W = MaterialTensor(x=[F, p], fun=lambda x: x, triu=True)
-    P = W.function([FF, pp])
-    A = W.gradient([FF, pp])
+    P = W.gradient([FF, pp])
+    A = W.hessian([FF, pp])
 
     assert len(P) == 2
     assert len(A) == 3
 
     # init mixed Material with full gradient
     W = MaterialTensor(x=[F, p], fun=lambda x: x, triu=False)
-    P = W.function([FF, pp])
-    A = W.gradient([FF, pp])
+    P = W.gradient([FF, pp])
+    A = W.hessian([FF, pp])
 
     assert len(P) == 2
     assert len(A) == 4
 
     # init mixed Material with upper triangle gradient and state variables
     W = MaterialTensor(x=[F, p, z], fun=lambda x: [*x, z], triu=True, statevars=1)
-    P = W.function([FF, pp, zz])
-    A = W.gradient([FF, pp, zz])
+    P = W.gradient([FF, pp, zz])
+    A = W.hessian([FF, pp, zz])
 
     assert len(P) == 4
     assert len(A) == 3
 
 
 if __name__ == "__main__":
     test_simple()
```

