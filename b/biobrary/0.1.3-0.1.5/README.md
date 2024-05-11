# Comparing `tmp/biobrary-0.1.3.tar.gz` & `tmp/biobrary-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biobrary-0.1.3.tar", last modified: Tue Oct 17 08:37:22 2023, max compression
+gzip compressed data, was "biobrary-0.1.5.tar", last modified: Sat May 11 02:27:44 2024, max compression
```

## Comparing `biobrary-0.1.3.tar` & `biobrary-0.1.5.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 fanghl    (1000) fanghl    (1000)        0 2023-10-17 08:37:22.678335 biobrary-0.1.3/
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)     1070 2023-04-07 06:30:35.000000 biobrary-0.1.3/LICENSE
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)     1437 2023-10-17 08:37:22.678335 biobrary-0.1.3/PKG-INFO
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)      942 2023-04-07 06:30:35.000000 biobrary-0.1.3/README.md
-drwxr-xr-x   0 fanghl    (1000) fanghl    (1000)        0 2023-10-17 08:37:22.675335 biobrary-0.1.3/biobrary/
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)      158 2023-10-17 07:42:05.000000 biobrary-0.1.3/biobrary/__init__.py
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)      324 2023-04-07 06:30:35.000000 biobrary-0.1.3/biobrary/amino_acids_mw.py
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)     1935 2023-10-17 07:29:27.000000 biobrary-0.1.3/biobrary/biocodon.py
-drwxr-xr-x   0 fanghl    (1000) fanghl    (1000)        0 2023-10-17 08:37:22.677335 biobrary-0.1.3/biobrary/bioparse/
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)      180 2023-10-17 07:40:17.000000 biobrary-0.1.3/biobrary/bioparse/__init__.py
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)    12458 2023-10-17 07:38:59.000000 biobrary-0.1.3/biobrary/bioparse/blast_parse.py
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)     4002 2023-10-17 07:39:15.000000 biobrary-0.1.3/biobrary/bioparse/fasta_parse.py
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)    13500 2023-10-17 07:39:28.000000 biobrary-0.1.3/biobrary/bioparse/gbk_parse.py
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)     2261 2023-10-17 07:39:48.000000 biobrary-0.1.3/biobrary/bioparse/gff_parse.py
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)     7456 2023-10-17 08:34:04.000000 biobrary-0.1.3/biobrary/bioparse/gtf_parse.py
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)    14178 2023-04-07 06:30:35.000000 biobrary-0.1.3/biobrary/score_matrix.py
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)       29 2023-10-17 08:14:24.000000 biobrary-0.1.3/biobrary/seq.py
-drwxr-xr-x   0 fanghl    (1000) fanghl    (1000)        0 2023-10-17 08:37:22.677335 biobrary-0.1.3/biobrary/tree/
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)    10708 2023-04-07 06:30:35.000000 biobrary-0.1.3/biobrary/tree/CircleNode.py
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)        0 2023-04-07 07:13:44.000000 biobrary-0.1.3/biobrary/tree/__init__.py
-drwxr-xr-x   0 fanghl    (1000) fanghl    (1000)        0 2023-10-17 08:37:22.675335 biobrary-0.1.3/biobrary.egg-info/
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)     1437 2023-10-17 08:37:22.000000 biobrary-0.1.3/biobrary.egg-info/PKG-INFO
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)      563 2023-10-17 08:37:22.000000 biobrary-0.1.3/biobrary.egg-info/SOURCES.txt
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)        1 2023-10-17 08:37:22.000000 biobrary-0.1.3/biobrary.egg-info/dependency_links.txt
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)       38 2023-10-17 08:37:22.000000 biobrary-0.1.3/biobrary.egg-info/requires.txt
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)        9 2023-10-17 08:37:22.000000 biobrary-0.1.3/biobrary.egg-info/top_level.txt
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)      551 2023-10-17 08:36:56.000000 biobrary-0.1.3/pyproject.toml
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)      235 2023-10-17 08:37:22.679335 biobrary-0.1.3/setup.cfg
--rw-r--r--   0 fanghl    (1000) fanghl    (1000)       68 2023-04-07 08:42:11.000000 biobrary-0.1.3/setup.py
+drwxr-xr-x   0 fanghl    (1000) fanghl    (1000)        0 2024-05-11 02:27:44.348541 biobrary-0.1.5/
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)     1069 2024-04-26 00:44:15.000000 biobrary-0.1.5/LICENSE
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)     2593 2024-05-11 02:27:44.348541 biobrary-0.1.5/PKG-INFO
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)      873 2023-10-23 05:51:46.000000 biobrary-0.1.5/README.md
+drwxr-xr-x   0 fanghl    (1000) fanghl    (1000)        0 2024-05-11 02:27:44.347541 biobrary-0.1.5/biobrary/
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)      160 2024-04-25 09:17:53.000000 biobrary-0.1.5/biobrary/__init__.py
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)      109 2024-04-25 09:17:53.000000 biobrary-0.1.5/biobrary/base_complement.py
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)     1825 2024-04-25 09:17:53.000000 biobrary-0.1.5/biobrary/biocodon.py
+drwxr-xr-x   0 fanghl    (1000) fanghl    (1000)        0 2024-05-11 02:27:44.348541 biobrary-0.1.5/biobrary/bioparse/
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)      166 2024-04-25 09:17:53.000000 biobrary-0.1.5/biobrary/bioparse/__init__.py
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)    12458 2024-04-25 09:17:53.000000 biobrary-0.1.5/biobrary/bioparse/blast_parse.py
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)     4849 2024-04-25 09:17:53.000000 biobrary-0.1.5/biobrary/bioparse/fasta_parse.py
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)    13500 2024-04-25 09:17:53.000000 biobrary-0.1.5/biobrary/bioparse/gbk_parse.py
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)     2261 2024-04-25 09:17:53.000000 biobrary-0.1.5/biobrary/bioparse/gff_parse.py
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)    14915 2024-04-25 09:17:53.000000 biobrary-0.1.5/biobrary/bioparse/gtf_parse.py
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)    10673 2024-04-25 09:17:53.000000 biobrary-0.1.5/biobrary/misc.py
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)      324 2024-04-25 09:17:53.000000 biobrary-0.1.5/biobrary/molecular_weight.py
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)    14178 2024-04-25 09:17:53.000000 biobrary-0.1.5/biobrary/score_matrix.py
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)     1874 2024-04-25 09:17:53.000000 biobrary-0.1.5/biobrary/seq.py
+drwxr-xr-x   0 fanghl    (1000) fanghl    (1000)        0 2024-05-11 02:27:44.348541 biobrary-0.1.5/biobrary/tree/
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)    10708 2024-04-25 09:17:53.000000 biobrary-0.1.5/biobrary/tree/CircleNode.py
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)        0 2024-04-25 09:17:53.000000 biobrary-0.1.5/biobrary/tree/__init__.py
+drwxr-xr-x   0 fanghl    (1000) fanghl    (1000)        0 2024-05-11 02:27:44.348541 biobrary-0.1.5/biobrary.egg-info/
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)     2593 2024-05-11 02:27:44.000000 biobrary-0.1.5/biobrary.egg-info/PKG-INFO
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)      625 2024-05-11 02:27:44.000000 biobrary-0.1.5/biobrary.egg-info/SOURCES.txt
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)        1 2024-05-11 02:27:44.000000 biobrary-0.1.5/biobrary.egg-info/dependency_links.txt
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)       38 2024-05-11 02:27:44.000000 biobrary-0.1.5/biobrary.egg-info/requires.txt
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)        9 2024-05-11 02:27:44.000000 biobrary-0.1.5/biobrary.egg-info/top_level.txt
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)      585 2024-05-11 02:26:01.000000 biobrary-0.1.5/pyproject.toml
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)       38 2024-05-11 02:27:44.348541 biobrary-0.1.5/setup.cfg
+drwxr-xr-x   0 fanghl    (1000) fanghl    (1000)        0 2024-05-11 02:27:44.348541 biobrary-0.1.5/test/
+-rw-r--r--   0 fanghl    (1000) fanghl    (1000)        0 2023-10-20 08:39:08.000000 biobrary-0.1.5/test/test_bioparse_fasta_parse.py
```

### Comparing `biobrary-0.1.3/LICENSE` & `biobrary-0.1.5/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2019 Benjamin Fang
+Copyright (c) 2019 Hailing Fang
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `biobrary-0.1.3/PKG-INFO` & `biobrary-0.1.5/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,68 +1,65 @@
-Metadata-Version: 2.1
-Name: biobrary
-Version: 0.1.3
-Summary: A library for biological computing works
-Author-email: Benjamin Fang <benjaminfang.ol@outlook.com>
-License: MIT License
-Project-URL: Homepage, https://github.com/benjaminfang/biobrary
-Keywords: biobrary,bioparse,tree
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: ete3>=3.1.1
-Requires-Dist: numpy>=1.21.2
-Requires-Dist: six>=1.15.0
-
 # Biobrary
 
 ## Introduction
+
 Biobrary is a python library, which contain data and methods for biological computation.
 
 ## Requirement  
+
 * ete3
+
     pyqt5 is needed by ete3. you maybe need install it manually.
  
 
 ## Install  
+
 * using pip  
+
 `pip install biobrary --user`
 
 * manally install  
+
 `git clone https://github.com/benjaminfang/biobrary.git`  
+
 `cd biobrary`  
-`mv biobrary PYTHONPATH`  
+
+`mv biobrary $PYTHONPATH`  
+
 where PYTHONPATH is python library searching path.
 
 ## Usage  
+
 ```
 import biobrary  
 dir(biobrary)  
 ```
 
 ## Data and Method  
 
-* biopaser  
-    * Fasta_parser  
+* bioparse  
+
+    * FASTA  
+
         class for fasta file.
-    * Gff_parser  
+
+    * GTF  
+
+        class for gtf file.
+
+    * GFF
+
         class for gff file.
 
 
 * biocondon  
-    * CODON_AA  
-        python dictionary of codon and amino acids.  
-    * base_complement
-    * start_codon
-    * stop_codon
-
 
 
 * amino_acids_mw  
 
+* tree
 
+    * CircleNode  
 
-* CircleNode  
-    class for phylogenic tree traverse and operations. And divide tree to circle node according
-    to phylogenic distance.
+        class for phylogenic tree traverse and operations. And divide tree to circle node according
+        to phylogenic distance.
```

### Comparing `biobrary-0.1.3/biobrary/biocodon.py` & `biobrary-0.1.5/biobrary/biocodon.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,12 +41,10 @@
           'tgg':'W',
           'cgt':'R','cgc':'R','cga':'R','cgg':'R','aga':'R','agg':'R',
           'ggt':'G','ggc':'G','gga':'G','ggg':'G',
           'taa':'*','tag':'*','tga':'*',
          }
 
 
-base_complement = {'A':'T', 'T':'A', 'G':'C', 'C':'G', 'N':'N', 'a':'t', 't':'a', 'c':'g', 'g':'c', 'n':'n'}
-
 start_codon = ['ATG']
 
 stop_codon = ['TAA', 'TAG', 'TGA']
```

### Comparing `biobrary-0.1.3/biobrary/bioparse/blast_parse.py` & `biobrary-0.1.5/biobrary/bioparse/blast_parse.py`

 * *Files identical despite different names*

### Comparing `biobrary-0.1.3/biobrary/bioparse/gbk_parse.py` & `biobrary-0.1.5/biobrary/bioparse/gbk_parse.py`

 * *Files identical despite different names*

### Comparing `biobrary-0.1.3/biobrary/bioparse/gff_parse.py` & `biobrary-0.1.5/biobrary/bioparse/gff_parse.py`

 * *Files identical despite different names*

### Comparing `biobrary-0.1.3/biobrary/score_matrix.py` & `biobrary-0.1.5/biobrary/score_matrix.py`

 * *Files identical despite different names*

### Comparing `biobrary-0.1.3/biobrary/tree/CircleNode.py` & `biobrary-0.1.5/biobrary/tree/CircleNode.py`

 * *Files identical despite different names*

### Comparing `biobrary-0.1.3/biobrary.egg-info/SOURCES.txt` & `biobrary-0.1.5/biobrary.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 LICENSE
 README.md
 pyproject.toml
-setup.cfg
-setup.py
 biobrary/__init__.py
-biobrary/amino_acids_mw.py
+biobrary/base_complement.py
 biobrary/biocodon.py
+biobrary/misc.py
+biobrary/molecular_weight.py
 biobrary/score_matrix.py
 biobrary/seq.py
 biobrary.egg-info/PKG-INFO
 biobrary.egg-info/SOURCES.txt
 biobrary.egg-info/dependency_links.txt
 biobrary.egg-info/requires.txt
 biobrary.egg-info/top_level.txt
 biobrary/bioparse/__init__.py
 biobrary/bioparse/blast_parse.py
 biobrary/bioparse/fasta_parse.py
 biobrary/bioparse/gbk_parse.py
 biobrary/bioparse/gff_parse.py
 biobrary/bioparse/gtf_parse.py
 biobrary/tree/CircleNode.py
-biobrary/tree/__init__.py
+biobrary/tree/__init__.py
+test/test_bioparse_fasta_parse.py
```

### Comparing `biobrary-0.1.3/pyproject.toml` & `biobrary-0.1.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [build-system]
-requires=["setuptools", "wheel"]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
 
 [project]
 name = "biobrary"
-version = "0.1.3"
-authors = [{name="Benjamin Fang", email="benjaminfang.ol@outlook.com"}]
+version = "0.1.5"
+authors = [{name="Hailing Fang", email="benjaminfang.ol@outlook.com"}]
 description = "A library for biological computing works"
 readme = "README.md"
-requires-python = ">=3.6"
-license = {text = "MIT License"}
+requires-python = ">=3.7"
+license = {file = "LICENSE"}
 keywords = ["biobrary", "bioparse", "tree"]
 classifiers = ["Programming Language :: Python :: 3"]
 dependencies = [
     "ete3>=3.1.1",
     "numpy>=1.21.2",
     "six>=1.15.0"
 ]
```

