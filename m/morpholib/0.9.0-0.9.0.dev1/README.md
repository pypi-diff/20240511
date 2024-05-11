# Comparing `tmp/morpholib-0.9.0.tar.gz` & `tmp/morpholib-0.9.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\ksmall\Documents\Kenneth's stuff\Python\Morpho\pip\v0.9.0-final\dist\.tmp-shvxq3ue\morpholib-0.9.0.tar", last modified: Mon Nov 27 17:32:10 2023, max compression
+gzip compressed data, was "C:\Users\ksmall\Documents\Kenneth's stuff\Python\Morpho\pip\v0.9.0-test\dist\.tmp-wsn1b8ew\morpholib-0.9.0.dev1.tar", last modified: Mon Nov 27 17:08:55 2023, max compression
```

## Comparing `morpholib-0.9.0.tar` & `morpholib-0.9.0.dev1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-11-27 17:32:10.942853 morpholib-0.9.0/
--rw-rw-rw-   0        0        0     1091 2021-09-29 20:39:14.000000 morpholib-0.9.0/LICENSE
--rw-rw-rw-   0        0        0     4548 2023-11-27 17:32:10.942853 morpholib-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     3967 2023-05-27 15:02:41.000000 morpholib-0.9.0/README.md
--rw-rw-rw-   0        0        0      110 2021-09-27 17:28:21.000000 morpholib-0.9.0/pyproject.toml
--rw-rw-rw-   0        0        0      660 2023-11-27 17:32:10.942853 morpholib-0.9.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-11-27 17:32:10.832852 morpholib-0.9.0/src/
-drwxrwxrwx   0        0        0        0 2023-11-27 17:32:10.892852 morpholib-0.9.0/src/morpholib/
--rw-rw-rw-   0        0        0      470 2023-10-09 20:47:48.000000 morpholib-0.9.0/src/morpholib/__init__.py
--rw-rw-rw-   0        0        0    12158 2023-11-21 04:04:30.000000 morpholib-0.9.0/src/morpholib/actions.py
--rw-rw-rw-   0        0        0   189421 2023-11-21 04:04:30.000000 morpholib-0.9.0/src/morpholib/anim.py
--rw-rw-rw-   0        0        0    28969 2023-11-27 17:05:27.000000 morpholib-0.9.0/src/morpholib/base.py
--rw-rw-rw-   0        0        0     4241 2023-03-12 21:13:07.000000 morpholib-0.9.0/src/morpholib/bezier.py
--rw-rw-rw-   0        0        0    29327 2023-03-09 16:23:34.000000 morpholib-0.9.0/src/morpholib/calculus.py
--rw-rw-rw-   0        0        0    36216 2023-11-21 04:04:30.000000 morpholib-0.9.0/src/morpholib/color.py
--rw-rw-rw-   0        0        0    21228 2023-11-27 17:05:27.000000 morpholib-0.9.0/src/morpholib/combo.py
--rw-rw-rw-   0        0        0    96245 2023-11-24 04:33:55.000000 morpholib-0.9.0/src/morpholib/figure.py
--rw-rw-rw-   0        0        0    10392 2023-11-21 04:04:30.000000 morpholib-0.9.0/src/morpholib/gadgets.py
--rw-rw-rw-   0        0        0     2513 2022-03-08 00:05:51.000000 morpholib-0.9.0/src/morpholib/giffer.py
--rw-rw-rw-   0        0        0     9907 2023-09-12 20:40:57.000000 morpholib-0.9.0/src/morpholib/graph.py
--rw-rw-rw-   0        0        0    42021 2023-11-21 04:04:30.000000 morpholib-0.9.0/src/morpholib/graphics.py
--rw-rw-rw-   0        0        0   193674 2023-11-21 23:58:27.000000 morpholib-0.9.0/src/morpholib/grid.py
--rw-rw-rw-   0        0        0     6666 2023-11-21 04:04:30.000000 morpholib-0.9.0/src/morpholib/latex.py
--rw-rw-rw-   0        0        0    13144 2023-10-03 17:43:31.000000 morpholib-0.9.0/src/morpholib/matrix.py
--rw-rw-rw-   0        0        0      709 2022-08-01 17:17:30.000000 morpholib-0.9.0/src/morpholib/sample.py
--rw-rw-rw-   0        0        0   121608 2023-11-27 17:05:27.000000 morpholib-0.9.0/src/morpholib/shapes.py
--rw-rw-rw-   0        0        0    77308 2023-11-21 04:04:30.000000 morpholib-0.9.0/src/morpholib/text.py
-drwxrwxrwx   0        0        0        0 2023-11-27 17:32:10.932853 morpholib-0.9.0/src/morpholib/tools/
--rw-rw-rw-   0        0        0       72 2022-03-08 00:05:51.000000 morpholib-0.9.0/src/morpholib/tools/__init__.py
--rw-rw-rw-   0        0        0        4 2022-03-08 00:05:51.000000 morpholib-0.9.0/src/morpholib/tools/base.py
--rw-rw-rw-   0        0        0    13752 2023-11-21 04:04:30.000000 morpholib-0.9.0/src/morpholib/tools/basics.py
--rw-rw-rw-   0        0        0       31 2022-06-16 19:16:16.000000 morpholib-0.9.0/src/morpholib/tools/color.py
--rw-rw-rw-   0        0        0    27622 2023-11-21 04:04:30.000000 morpholib-0.9.0/src/morpholib/tools/dev.py
--rw-rw-rw-   0        0        0     2117 2023-11-21 04:04:30.000000 morpholib-0.9.0/src/morpholib/tools/ktimer.py
--rw-rw-rw-   0        0        0     6348 2023-04-25 17:14:02.000000 morpholib-0.9.0/src/morpholib/tools/latex2svg.py
--rw-rw-rw-   0        0        0      811 2022-03-08 00:05:51.000000 morpholib-0.9.0/src/morpholib/tools/subimporter.py
--rw-rw-rw-   0        0        0     7137 2023-09-13 03:05:07.000000 morpholib-0.9.0/src/morpholib/transitions.py
--rw-rw-rw-   0        0        0     9128 2022-06-16 19:16:16.000000 morpholib-0.9.0/src/morpholib/video.py
-drwxrwxrwx   0        0        0        0 2023-11-27 17:32:10.942853 morpholib-0.9.0/src/morpholib.egg-info/
--rw-rw-rw-   0        0        0     4548 2023-11-27 17:32:10.000000 morpholib-0.9.0/src/morpholib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      974 2023-11-27 17:32:10.000000 morpholib-0.9.0/src/morpholib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-27 17:32:10.000000 morpholib-0.9.0/src/morpholib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-11-27 17:32:10.000000 morpholib-0.9.0/src/morpholib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-11-27 17:32:10.000000 morpholib-0.9.0/src/morpholib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-11-27 17:08:55.199966 morpholib-0.9.0.dev1/
+-rw-rw-rw-   0        0        0     1091 2021-09-29 20:39:14.000000 morpholib-0.9.0.dev1/LICENSE
+-rw-rw-rw-   0        0        0     4553 2023-11-27 17:08:55.199966 morpholib-0.9.0.dev1/PKG-INFO
+-rw-rw-rw-   0        0        0     3967 2023-05-27 15:02:41.000000 morpholib-0.9.0.dev1/README.md
+-rw-rw-rw-   0        0        0      110 2021-09-27 17:28:21.000000 morpholib-0.9.0.dev1/pyproject.toml
+-rw-rw-rw-   0        0        0      665 2023-11-27 17:08:55.202466 morpholib-0.9.0.dev1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-11-27 17:08:55.057464 morpholib-0.9.0.dev1/src/
+drwxrwxrwx   0        0        0        0 2023-11-27 17:08:55.147465 morpholib-0.9.0.dev1/src/morpholib/
+-rw-rw-rw-   0        0        0      470 2023-10-09 20:47:48.000000 morpholib-0.9.0.dev1/src/morpholib/__init__.py
+-rw-rw-rw-   0        0        0    12158 2023-11-21 04:04:30.000000 morpholib-0.9.0.dev1/src/morpholib/actions.py
+-rw-rw-rw-   0        0        0   189421 2023-11-21 04:04:30.000000 morpholib-0.9.0.dev1/src/morpholib/anim.py
+-rw-rw-rw-   0        0        0    28974 2023-11-27 17:07:27.000000 morpholib-0.9.0.dev1/src/morpholib/base.py
+-rw-rw-rw-   0        0        0     4241 2023-03-12 21:13:07.000000 morpholib-0.9.0.dev1/src/morpholib/bezier.py
+-rw-rw-rw-   0        0        0    29327 2023-03-09 16:23:34.000000 morpholib-0.9.0.dev1/src/morpholib/calculus.py
+-rw-rw-rw-   0        0        0    36216 2023-11-21 04:04:30.000000 morpholib-0.9.0.dev1/src/morpholib/color.py
+-rw-rw-rw-   0        0        0    21228 2023-11-27 17:05:27.000000 morpholib-0.9.0.dev1/src/morpholib/combo.py
+-rw-rw-rw-   0        0        0    96245 2023-11-24 04:33:55.000000 morpholib-0.9.0.dev1/src/morpholib/figure.py
+-rw-rw-rw-   0        0        0    10392 2023-11-21 04:04:30.000000 morpholib-0.9.0.dev1/src/morpholib/gadgets.py
+-rw-rw-rw-   0        0        0     2513 2022-03-08 00:05:51.000000 morpholib-0.9.0.dev1/src/morpholib/giffer.py
+-rw-rw-rw-   0        0        0     9907 2023-09-12 20:40:57.000000 morpholib-0.9.0.dev1/src/morpholib/graph.py
+-rw-rw-rw-   0        0        0    42021 2023-11-21 04:04:30.000000 morpholib-0.9.0.dev1/src/morpholib/graphics.py
+-rw-rw-rw-   0        0        0   193674 2023-11-21 23:58:27.000000 morpholib-0.9.0.dev1/src/morpholib/grid.py
+-rw-rw-rw-   0        0        0     6666 2023-11-21 04:04:30.000000 morpholib-0.9.0.dev1/src/morpholib/latex.py
+-rw-rw-rw-   0        0        0    13144 2023-10-03 17:43:31.000000 morpholib-0.9.0.dev1/src/morpholib/matrix.py
+-rw-rw-rw-   0        0        0      709 2022-08-01 17:17:30.000000 morpholib-0.9.0.dev1/src/morpholib/sample.py
+-rw-rw-rw-   0        0        0   121608 2023-11-27 17:05:27.000000 morpholib-0.9.0.dev1/src/morpholib/shapes.py
+-rw-rw-rw-   0        0        0    77308 2023-11-21 04:04:30.000000 morpholib-0.9.0.dev1/src/morpholib/text.py
+drwxrwxrwx   0        0        0        0 2023-11-27 17:08:55.192466 morpholib-0.9.0.dev1/src/morpholib/tools/
+-rw-rw-rw-   0        0        0       72 2022-03-08 00:05:51.000000 morpholib-0.9.0.dev1/src/morpholib/tools/__init__.py
+-rw-rw-rw-   0        0        0        4 2022-03-08 00:05:51.000000 morpholib-0.9.0.dev1/src/morpholib/tools/base.py
+-rw-rw-rw-   0        0        0    13752 2023-11-21 04:04:30.000000 morpholib-0.9.0.dev1/src/morpholib/tools/basics.py
+-rw-rw-rw-   0        0        0       31 2022-06-16 19:16:16.000000 morpholib-0.9.0.dev1/src/morpholib/tools/color.py
+-rw-rw-rw-   0        0        0    27622 2023-11-21 04:04:30.000000 morpholib-0.9.0.dev1/src/morpholib/tools/dev.py
+-rw-rw-rw-   0        0        0     2117 2023-11-21 04:04:30.000000 morpholib-0.9.0.dev1/src/morpholib/tools/ktimer.py
+-rw-rw-rw-   0        0        0     6348 2023-04-25 17:14:02.000000 morpholib-0.9.0.dev1/src/morpholib/tools/latex2svg.py
+-rw-rw-rw-   0        0        0      811 2022-03-08 00:05:51.000000 morpholib-0.9.0.dev1/src/morpholib/tools/subimporter.py
+-rw-rw-rw-   0        0        0     7137 2023-09-13 03:05:07.000000 morpholib-0.9.0.dev1/src/morpholib/transitions.py
+-rw-rw-rw-   0        0        0     9128 2022-06-16 19:16:16.000000 morpholib-0.9.0.dev1/src/morpholib/video.py
+drwxrwxrwx   0        0        0        0 2023-11-27 17:08:55.197466 morpholib-0.9.0.dev1/src/morpholib.egg-info/
+-rw-rw-rw-   0        0        0     4553 2023-11-27 17:08:55.000000 morpholib-0.9.0.dev1/src/morpholib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      974 2023-11-27 17:08:55.000000 morpholib-0.9.0.dev1/src/morpholib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-11-27 17:08:55.000000 morpholib-0.9.0.dev1/src/morpholib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-11-27 17:08:55.000000 morpholib-0.9.0.dev1/src/morpholib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-11-27 17:08:55.000000 morpholib-0.9.0.dev1/src/morpholib.egg-info/top_level.txt
```

### Comparing `morpholib-0.9.0/LICENSE` & `morpholib-0.9.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `morpholib-0.9.0/PKG-INFO` & `morpholib-0.9.0.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morpholib
-Version: 0.9.0
+Version: 0.9.0.dev1
 Summary: A general-purpose programmatic animation tool
 Home-page: https://github.com/morpho-matters/morpholib
 Author: Kenneth Small
 Author-email: morpho.matters@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `morpholib-0.9.0/README.md` & `morpholib-0.9.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `morpholib-0.9.0/setup.cfg` & `morpholib-0.9.0.dev1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6f72 7068 6f6c 6962 0d0a 7665   = morpholib..ve
-00000020: 7273 696f 6e20 3d20 302e 392e 300d 0a61  rsion = 0.9.0..a
-00000030: 7574 686f 7220 3d20 4b65 6e6e 6574 6820  uthor = Kenneth 
-00000040: 536d 616c 6c0d 0a61 7574 686f 725f 656d  Small..author_em
-00000050: 6169 6c20 3d20 6d6f 7270 686f 2e6d 6174  ail = morpho.mat
-00000060: 7465 7273 4067 6d61 696c 2e63 6f6d 0d0a  ters@gmail.com..
-00000070: 6465 7363 7269 7074 696f 6e20 3d20 4120  description = A 
-00000080: 6765 6e65 7261 6c2d 7075 7270 6f73 6520  general-purpose 
-00000090: 7072 6f67 7261 6d6d 6174 6963 2061 6e69  programmatic ani
-000000a0: 6d61 7469 6f6e 2074 6f6f 6c0d 0a6c 6f6e  mation tool..lon
-000000b0: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description = 
-000000c0: 6669 6c65 3a20 5245 4144 4d45 2e6d 640d  file: README.md.
-000000d0: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
-000000e0: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
-000000f0: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
-00000100: 7572 6c20 3d20 6874 7470 733a 2f2f 6769  url = https://gi
-00000110: 7468 7562 2e63 6f6d 2f6d 6f72 7068 6f2d  thub.com/morpho-
-00000120: 6d61 7474 6572 732f 6d6f 7270 686f 6c69  matters/morpholi
-00000130: 620d 0a6c 6963 656e 7365 203d 204d 4954  b..license = MIT
-00000140: 0d0a 636c 6173 7369 6669 6572 7320 3d20  ..classifiers = 
-00000150: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-00000160: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000170: 6e20 3a3a 2033 0d0a 0d0a 5b6f 7074 696f  n :: 3....[optio
-00000180: 6e73 5d0d 0a70 6163 6b61 6765 5f64 6972  ns]..package_dir
-00000190: 203d 200d 0a09 3d20 7372 630d 0a70 6163   = ...= src..pac
-000001a0: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a70  kages = find:..p
-000001b0: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
-000001c0: 203e 3d33 2e38 0d0a 696e 7374 616c 6c5f   >=3.8..install_
-000001d0: 7265 7175 6972 6573 203d 200d 0a09 6e75  requires = ...nu
-000001e0: 6d70 793c 322e 300d 0a09 7069 6c6c 6f77  mpy<2.0...pillow
-000001f0: 0d0a 0969 6d61 6765 696f 3c33 2e30 0d0a  ...imageio<3.0..
-00000200: 0970 7967 6c65 743c 322e 300d 0a09 7079  .pyglet<2.0...py
-00000210: 6361 6972 6f3c 322e 300d 0a09 7079 7065  cairo<2.0...pype
-00000220: 7263 6c69 703c 322e 300d 0a09 7376 6765  rclip<2.0...svge
-00000230: 6c65 6d65 6e74 733e 3d31 2e35 2e34 0d0a  lements>=1.5.4..
-00000240: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
-00000250: 6765 732e 6669 6e64 5d0d 0a77 6865 7265  ges.find]..where
-00000260: 203d 2073 7263 0d0a 0d0a 5b65 6767 5f69   = src....[egg_i
-00000270: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
-00000280: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
-00000290: 0d0a 0d0a                                ....
+00000020: 7273 696f 6e20 3d20 302e 392e 302e 6465  rsion = 0.9.0.de
+00000030: 7631 0d0a 6175 7468 6f72 203d 204b 656e  v1..author = Ken
+00000040: 6e65 7468 2053 6d61 6c6c 0d0a 6175 7468  neth Small..auth
+00000050: 6f72 5f65 6d61 696c 203d 206d 6f72 7068  or_email = morph
+00000060: 6f2e 6d61 7474 6572 7340 676d 6169 6c2e  o.matters@gmail.
+00000070: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
+00000080: 203d 2041 2067 656e 6572 616c 2d70 7572   = A general-pur
+00000090: 706f 7365 2070 726f 6772 616d 6d61 7469  pose programmati
+000000a0: 6320 616e 696d 6174 696f 6e20 746f 6f6c  c animation tool
+000000b0: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
+000000c0: 6f6e 203d 2066 696c 653a 2052 4541 444d  on = file: READM
+000000d0: 452e 6d64 0d0a 6c6f 6e67 5f64 6573 6372  E.md..long_descr
+000000e0: 6970 7469 6f6e 5f63 6f6e 7465 6e74 5f74  iption_content_t
+000000f0: 7970 6520 3d20 7465 7874 2f6d 6172 6b64  ype = text/markd
+00000100: 6f77 6e0d 0a75 726c 203d 2068 7474 7073  own..url = https
+00000110: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d6f  ://github.com/mo
+00000120: 7270 686f 2d6d 6174 7465 7273 2f6d 6f72  rpho-matters/mor
+00000130: 7068 6f6c 6962 0d0a 6c69 6365 6e73 6520  pholib..license 
+00000140: 3d20 4d49 540d 0a63 6c61 7373 6966 6965  = MIT..classifie
+00000150: 7273 203d 200d 0a09 5072 6f67 7261 6d6d  rs = ...Programm
+00000160: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000170: 5079 7468 6f6e 203a 3a20 330d 0a0d 0a5b  Python :: 3....[
+00000180: 6f70 7469 6f6e 735d 0d0a 7061 636b 6167  options]..packag
+00000190: 655f 6469 7220 3d20 0d0a 093d 2073 7263  e_dir = ...= src
+000001a0: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
+000001b0: 643a 0d0a 7079 7468 6f6e 5f72 6571 7569  d:..python_requi
+000001c0: 7265 7320 3d20 3e3d 332e 380d 0a69 6e73  res = >=3.8..ins
+000001d0: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
+000001e0: 0d0a 096e 756d 7079 3c32 2e30 0d0a 0970  ...numpy<2.0...p
+000001f0: 696c 6c6f 770d 0a09 696d 6167 6569 6f3c  illow...imageio<
+00000200: 332e 300d 0a09 7079 676c 6574 3c32 2e30  3.0...pyglet<2.0
+00000210: 0d0a 0970 7963 6169 726f 3c32 2e30 0d0a  ...pycairo<2.0..
+00000220: 0970 7970 6572 636c 6970 3c32 2e30 0d0a  .pyperclip<2.0..
+00000230: 0973 7667 656c 656d 656e 7473 3e3d 312e  .svgelements>=1.
+00000240: 352e 340d 0a0d 0a5b 6f70 7469 6f6e 732e  5.4....[options.
+00000250: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
+00000260: 7768 6572 6520 3d20 7372 630d 0a0d 0a5b  where = src....[
+00000270: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
+00000280: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
+00000290: 6520 3d20 300d 0a0d 0a                   e = 0....
```

### Comparing `morpholib-0.9.0/src/morpholib/actions.py` & `morpholib-0.9.0.dev1/src/morpholib/actions.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.9.0/src/morpholib/anim.py` & `morpholib-0.9.0.dev1/src/morpholib/anim.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.9.0/src/morpholib/base.py` & `morpholib-0.9.0.dev1/src/morpholib/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from morpholib.tools.basics import tau, argShift, argShiftArray, arcCenter, arcCenterArray, isequal
 import math
 import numpy as np
 import cairo
 cr = cairo
 
 
-version = "0.9.0"  # Current public morpho version
+version = "0.9.0.dev1"  # Current public morpho version
 internalVersion = "2.4.1ip"  # Current internal morpho version
 subversion = ""
 DEBUG_MODE = False
 
 
 ### CLASSES ###
```

### Comparing `morpholib-0.9.0/src/morpholib/bezier.py` & `morpholib-0.9.0.dev1/src/morpholib/bezier.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.9.0/src/morpholib/calculus.py` & `morpholib-0.9.0.dev1/src/morpholib/calculus.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.9.0/src/morpholib/color.py` & `morpholib-0.9.0.dev1/src/morpholib/color.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.9.0/src/morpholib/combo.py` & `morpholib-0.9.0.dev1/src/morpholib/combo.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.9.0/src/morpholib/figure.py` & `morpholib-0.9.0.dev1/src/morpholib/figure.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.9.0/src/morpholib/gadgets.py` & `morpholib-0.9.0.dev1/src/morpholib/gadgets.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.9.0/src/morpholib/giffer.py` & `morpholib-0.9.0.dev1/src/morpholib/giffer.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.9.0/src/morpholib/graph.py` & `morpholib-0.9.0.dev1/src/morpholib/graph.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.9.0/src/morpholib/graphics.py` & `morpholib-0.9.0.dev1/src/morpholib/graphics.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.9.0/src/morpholib/grid.py` & `morpholib-0.9.0.dev1/src/morpholib/grid.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.9.0/src/morpholib/latex.py` & `morpholib-0.9.0.dev1/src/morpholib/latex.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.9.0/src/morpholib/matrix.py` & `morpholib-0.9.0.dev1/src/morpholib/matrix.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.9.0/src/morpholib/sample.py` & `morpholib-0.9.0.dev1/src/morpholib/sample.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.9.0/src/morpholib/shapes.py` & `morpholib-0.9.0.dev1/src/morpholib/shapes.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.9.0/src/morpholib/text.py` & `morpholib-0.9.0.dev1/src/morpholib/text.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.9.0/src/morpholib/tools/basics.py` & `morpholib-0.9.0.dev1/src/morpholib/tools/basics.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.9.0/src/morpholib/tools/dev.py` & `morpholib-0.9.0.dev1/src/morpholib/tools/dev.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.9.0/src/morpholib/tools/ktimer.py` & `morpholib-0.9.0.dev1/src/morpholib/tools/ktimer.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.9.0/src/morpholib/tools/latex2svg.py` & `morpholib-0.9.0.dev1/src/morpholib/tools/latex2svg.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.9.0/src/morpholib/tools/subimporter.py` & `morpholib-0.9.0.dev1/src/morpholib/tools/subimporter.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.9.0/src/morpholib/transitions.py` & `morpholib-0.9.0.dev1/src/morpholib/transitions.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.9.0/src/morpholib/video.py` & `morpholib-0.9.0.dev1/src/morpholib/video.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.9.0/src/morpholib.egg-info/PKG-INFO` & `morpholib-0.9.0.dev1/src/morpholib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morpholib
-Version: 0.9.0
+Version: 0.9.0.dev1
 Summary: A general-purpose programmatic animation tool
 Home-page: https://github.com/morpho-matters/morpholib
 Author: Kenneth Small
 Author-email: morpho.matters@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `morpholib-0.9.0/src/morpholib.egg-info/SOURCES.txt` & `morpholib-0.9.0.dev1/src/morpholib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

