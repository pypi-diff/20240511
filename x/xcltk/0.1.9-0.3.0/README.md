# Comparing `tmp/xcltk-0.1.9.tar.gz` & `tmp/xcltk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xcltk-0.1.9.tar", last modified: Mon Jan  4 05:21:42 2021, max compression
+gzip compressed data, was "xcltk-0.3.0.tar", last modified: Sat May 11 01:53:46 2024, max compression
```

## Comparing `xcltk-0.1.9.tar` & `xcltk-0.3.0.tar`

### file list

```diff
@@ -1,43 +1,55 @@
-drwxr-x---   0 xianjie  (30008) yuanhua  (30002)        0 2021-01-04 05:21:09.458541 xcltk-0.1.9/
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)     1564 2021-01-04 05:21:09.457541 xcltk-0.1.9/PKG-INFO
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)     1001 2021-01-04 05:20:54.000000 xcltk-0.1.9/README.md
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)       38 2021-01-04 05:21:09.458541 xcltk-0.1.9/setup.cfg
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)     2030 2021-01-04 05:20:54.000000 xcltk-0.1.9/setup.py
-drwxr-x---   0 xianjie  (30008) yuanhua  (30002)        0 2021-01-04 05:21:09.425541 xcltk-0.1.9/xcltk/
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)       22 2021-01-04 05:20:53.000000 xcltk-0.1.9/xcltk/__init__.py
-drwxr-x---   0 xianjie  (30008) yuanhua  (30002)        0 2021-01-04 05:21:09.439541 xcltk-0.1.9/xcltk/baf/
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)        0 2021-01-04 05:20:53.000000 xcltk-0.1.9/xcltk/baf/__init__.py
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)      874 2021-01-04 05:20:53.000000 xcltk-0.1.9/xcltk/baf/baf.py
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)       93 2021-01-04 05:20:53.000000 xcltk-0.1.9/xcltk/baf/config.py
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)     7959 2021-01-04 05:20:53.000000 xcltk-0.1.9/xcltk/baf/fixref.py
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)    17847 2021-01-04 05:20:53.000000 xcltk-0.1.9/xcltk/baf/phase_snp.py
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)    13497 2021-01-04 05:20:53.000000 xcltk-0.1.9/xcltk/baf/pileup.py
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)       56 2021-01-04 05:20:53.000000 xcltk-0.1.9/xcltk/config.py
-drwxr-x---   0 xianjie  (30008) yuanhua  (30002)        0 2021-01-04 05:21:09.443541 xcltk-0.1.9/xcltk/rdr/
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)        0 2021-01-04 05:20:53.000000 xcltk-0.1.9/xcltk/rdr/__init__.py
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)     7030 2021-01-04 05:20:53.000000 xcltk-0.1.9/xcltk/rdr/basefc.py
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)       93 2021-01-04 05:20:53.000000 xcltk-0.1.9/xcltk/rdr/config.py
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)      689 2021-01-04 05:20:53.000000 xcltk-0.1.9/xcltk/rdr/rdr.py
-drwxr-x---   0 xianjie  (30008) yuanhua  (30002)        0 2021-01-04 05:21:09.447541 xcltk-0.1.9/xcltk/region/
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)        0 2021-01-04 05:20:53.000000 xcltk-0.1.9/xcltk/region/__init__.py
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)       96 2021-01-04 05:20:53.000000 xcltk-0.1.9/xcltk/region/config.py
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)     3140 2021-01-04 05:20:53.000000 xcltk-0.1.9/xcltk/region/convert.py
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)      848 2021-01-04 05:20:53.000000 xcltk-0.1.9/xcltk/region/region.py
-drwxr-x---   0 xianjie  (30008) yuanhua  (30002)        0 2021-01-04 05:21:09.456541 xcltk-0.1.9/xcltk/utils/
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)        0 2021-01-04 05:20:53.000000 xcltk-0.1.9/xcltk/utils/__init__.py
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)     4030 2021-01-04 05:20:53.000000 xcltk-0.1.9/xcltk/utils/base.py
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)     2996 2021-01-04 05:20:53.000000 xcltk-0.1.9/xcltk/utils/count.py
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)    11416 2021-01-04 05:20:53.000000 xcltk-0.1.9/xcltk/utils/gtf.py
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)    16309 2021-01-04 05:20:53.000000 xcltk-0.1.9/xcltk/utils/pileup.py
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)     5153 2021-01-04 05:20:53.000000 xcltk-0.1.9/xcltk/utils/pileup_regions.py
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)     8699 2021-01-04 05:20:53.000000 xcltk-0.1.9/xcltk/utils/region.py
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)     2902 2021-01-04 05:20:53.000000 xcltk-0.1.9/xcltk/utils/sam.py
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)    10279 2021-01-04 05:20:53.000000 xcltk-0.1.9/xcltk/utils/vcf.py
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)     2556 2021-01-04 05:20:53.000000 xcltk-0.1.9/xcltk/xcltk.py
-drwxr-x---   0 xianjie  (30008) yuanhua  (30002)        0 2021-01-04 05:21:09.433541 xcltk-0.1.9/xcltk.egg-info/
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)     1564 2021-01-04 05:21:05.000000 xcltk-0.1.9/xcltk.egg-info/PKG-INFO
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)      735 2021-01-04 05:21:06.000000 xcltk-0.1.9/xcltk.egg-info/SOURCES.txt
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)        1 2021-01-04 05:21:05.000000 xcltk-0.1.9/xcltk.egg-info/dependency_links.txt
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)       44 2021-01-04 05:21:05.000000 xcltk-0.1.9/xcltk.egg-info/entry_points.txt
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)       27 2021-01-04 05:21:05.000000 xcltk-0.1.9/xcltk.egg-info/requires.txt
--rw-r-----   0 xianjie  (30008) yuanhua  (30002)        6 2021-01-04 05:21:05.000000 xcltk-0.1.9/xcltk.egg-info/top_level.txt
+drwxr-xr-x   0 xianjie  (30008) yuanhua  (30002)        0 2024-05-11 01:53:46.000000 xcltk-0.3.0/
+-rw-r-----   0 xianjie  (30008) yuanhua  (30002)    11357 2023-05-16 03:16:46.000000 xcltk-0.3.0/LICENSE
+-rw-r--r--   0 xianjie  (30008) yuanhua  (30002)     3117 2024-05-11 01:53:46.000000 xcltk-0.3.0/PKG-INFO
+-rw-r--r--   0 xianjie  (30008) yuanhua  (30002)     2651 2024-05-11 01:50:47.000000 xcltk-0.3.0/README.md
+-rw-r--r--   0 xianjie  (30008) yuanhua  (30002)       38 2024-05-11 01:53:46.000000 xcltk-0.3.0/setup.cfg
+-rw-r-----   0 xianjie  (30008) yuanhua  (30002)     2115 2024-05-02 02:01:45.000000 xcltk-0.3.0/setup.py
+drwxr-xr-x   0 xianjie  (30008) yuanhua  (30002)        0 2024-05-11 01:53:46.000000 xcltk-0.3.0/xcltk/
+-rw-r-----   0 xianjie  (30008) yuanhua  (30002)      341 2024-05-03 00:46:33.000000 xcltk-0.3.0/xcltk/__init__.py
+drwxr-xr-x   0 xianjie  (30008) yuanhua  (30002)        0 2024-05-11 01:53:46.000000 xcltk-0.3.0/xcltk/baf/
+-rw-r-----   0 xianjie  (30008) yuanhua  (30002)      121 2024-05-09 09:46:16.000000 xcltk-0.3.0/xcltk/baf/__init__.py
+-rw-r--r--   0 xianjie  (30008) yuanhua  (30002)    16946 2024-05-10 00:44:14.000000 xcltk-0.3.0/xcltk/baf/count.py
+drwxr-xr-x   0 xianjie  (30008) yuanhua  (30002)        0 2024-05-11 01:53:46.000000 xcltk-0.3.0/xcltk/baf/fc/
+-rw-r-----   0 xianjie  (30008) yuanhua  (30002)        0 2023-05-16 03:16:46.000000 xcltk-0.3.0/xcltk/baf/fc/__init__.py
+-rw-r-----   0 xianjie  (30008) yuanhua  (30002)     4787 2024-05-09 10:15:21.000000 xcltk-0.3.0/xcltk/baf/fc/config.py
+-rw-r-----   0 xianjie  (30008) yuanhua  (30002)     8321 2024-05-10 02:09:03.000000 xcltk-0.3.0/xcltk/baf/fc/core.py
+-rw-r--r--   0 xianjie  (30008) yuanhua  (30002)     1597 2024-05-09 09:10:36.000000 xcltk-0.3.0/xcltk/baf/fc/gfeature.py
+-rw-r-----   0 xianjie  (30008) yuanhua  (30002)     7003 2024-05-10 02:21:47.000000 xcltk-0.3.0/xcltk/baf/fc/mcount.py
+-rw-r-----   0 xianjie  (30008) yuanhua  (30002)     1857 2024-05-09 09:13:06.000000 xcltk-0.3.0/xcltk/baf/fc/thread.py
+-rw-r-----   0 xianjie  (30008) yuanhua  (30002)     8840 2024-05-09 09:13:41.000000 xcltk-0.3.0/xcltk/baf/fc/utils.py
+-rw-r-----   0 xianjie  (30008) yuanhua  (30002)     9366 2024-05-09 10:09:17.000000 xcltk-0.3.0/xcltk/baf/fixref.py
+-rw-r--r--   0 xianjie  (30008) yuanhua  (30002)    11932 2024-05-09 09:28:31.000000 xcltk-0.3.0/xcltk/baf/genotype.py
+-rw-r--r--   0 xianjie  (30008) yuanhua  (30002)    10270 2024-05-09 10:20:10.000000 xcltk-0.3.0/xcltk/baf/pipeline.py
+-rw-r-----   0 xianjie  (30008) yuanhua  (30002)    24259 2024-05-09 09:48:39.000000 xcltk-0.3.0/xcltk/baf/rpc.py
+-rw-r--r--   0 xianjie  (30008) yuanhua  (30002)       78 2024-05-10 08:24:22.000000 xcltk-0.3.0/xcltk/config.py
+drwxr-xr-x   0 xianjie  (30008) yuanhua  (30002)        0 2024-05-11 01:53:46.000000 xcltk-0.3.0/xcltk/rdr/
+-rw-r-----   0 xianjie  (30008) yuanhua  (30002)       36 2024-05-09 10:02:23.000000 xcltk-0.3.0/xcltk/rdr/__init__.py
+-rw-r-----   0 xianjie  (30008) yuanhua  (30002)    13612 2024-05-09 10:21:28.000000 xcltk-0.3.0/xcltk/rdr/count.py
+drwxr-xr-x   0 xianjie  (30008) yuanhua  (30002)        0 2024-05-11 01:53:46.000000 xcltk-0.3.0/xcltk/rdr/fc/
+-rw-r-----   0 xianjie  (30008) yuanhua  (30002)        0 2024-05-09 01:48:28.000000 xcltk-0.3.0/xcltk/rdr/fc/__init__.py
+-rw-r-----   0 xianjie  (30008) yuanhua  (30002)     3891 2024-05-09 10:14:55.000000 xcltk-0.3.0/xcltk/rdr/fc/config.py
+-rw-r-----   0 xianjie  (30008) yuanhua  (30002)     4253 2024-05-10 02:41:04.000000 xcltk-0.3.0/xcltk/rdr/fc/core.py
+-rw-r-----   0 xianjie  (30008) yuanhua  (30002)     3809 2024-05-10 02:40:25.000000 xcltk-0.3.0/xcltk/rdr/fc/mcount.py
+-rw-r-----   0 xianjie  (30008) yuanhua  (30002)     1474 2024-05-09 09:51:31.000000 xcltk-0.3.0/xcltk/rdr/fc/thread.py
+-rw-r-----   0 xianjie  (30008) yuanhua  (30002)     3268 2024-05-09 09:51:53.000000 xcltk-0.3.0/xcltk/rdr/fc/utils.py
+drwxr-xr-x   0 xianjie  (30008) yuanhua  (30002)        0 2024-05-11 01:53:46.000000 xcltk-0.3.0/xcltk/tools/
+-rw-r-----   0 xianjie  (30008) yuanhua  (30002)       21 2024-05-02 02:15:06.000000 xcltk-0.3.0/xcltk/tools/__init__.py
+-rw-r-----   0 xianjie  (30008) yuanhua  (30002)     3128 2024-05-09 09:56:41.000000 xcltk-0.3.0/xcltk/tools/convert.py
+drwxr-xr-x   0 xianjie  (30008) yuanhua  (30002)        0 2024-05-11 01:53:46.000000 xcltk-0.3.0/xcltk/utils/
+-rw-r-----   0 xianjie  (30008) yuanhua  (30002)      154 2024-05-09 09:57:23.000000 xcltk-0.3.0/xcltk/utils/__init__.py
+-rw-r-----   0 xianjie  (30008) yuanhua  (30002)      167 2024-05-09 09:57:39.000000 xcltk-0.3.0/xcltk/utils/base.py
+-rw-r-----   0 xianjie  (30008) yuanhua  (30002)     6134 2024-05-09 09:57:52.000000 xcltk-0.3.0/xcltk/utils/grange.py
+-rw-r-----   0 xianjie  (30008) yuanhua  (30002)     8689 2024-05-09 09:58:14.000000 xcltk-0.3.0/xcltk/utils/gregion.py
+-rw-r-----   0 xianjie  (30008) yuanhua  (30002)    11446 2024-05-09 09:59:00.000000 xcltk-0.3.0/xcltk/utils/gtf.py
+-rw-r-----   0 xianjie  (30008) yuanhua  (30002)     3528 2024-05-09 09:59:30.000000 xcltk-0.3.0/xcltk/utils/sam.py
+-rw-r--r--   0 xianjie  (30008) yuanhua  (30002)    12633 2024-05-09 10:00:03.000000 xcltk-0.3.0/xcltk/utils/vcf.py
+-rw-r--r--   0 xianjie  (30008) yuanhua  (30002)     2675 2024-05-02 08:35:23.000000 xcltk-0.3.0/xcltk/utils/xlog.py
+-rw-r-----   0 xianjie  (30008) yuanhua  (30002)     3806 2024-05-09 10:01:12.000000 xcltk-0.3.0/xcltk/utils/zfile.py
+-rw-r--r--   0 xianjie  (30008) yuanhua  (30002)     2563 2024-05-11 01:36:27.000000 xcltk-0.3.0/xcltk/xcltk.py
+drwxr-xr-x   0 xianjie  (30008) yuanhua  (30002)        0 2024-05-11 01:53:46.000000 xcltk-0.3.0/xcltk.egg-info/
+-rw-r--r--   0 xianjie  (30008) yuanhua  (30002)     3117 2024-05-11 01:53:46.000000 xcltk-0.3.0/xcltk.egg-info/PKG-INFO
+-rw-r--r--   0 xianjie  (30008) yuanhua  (30002)      947 2024-05-11 01:53:46.000000 xcltk-0.3.0/xcltk.egg-info/SOURCES.txt
+-rw-r--r--   0 xianjie  (30008) yuanhua  (30002)        1 2024-05-11 01:53:46.000000 xcltk-0.3.0/xcltk.egg-info/dependency_links.txt
+-rw-r--r--   0 xianjie  (30008) yuanhua  (30002)       43 2024-05-11 01:53:46.000000 xcltk-0.3.0/xcltk.egg-info/entry_points.txt
+-rw-r--r--   0 xianjie  (30008) yuanhua  (30002)       66 2024-05-11 01:53:46.000000 xcltk-0.3.0/xcltk.egg-info/requires.txt
+-rw-r--r--   0 xianjie  (30008) yuanhua  (30002)        6 2024-05-11 01:53:46.000000 xcltk-0.3.0/xcltk.egg-info/top_level.txt
```

### Comparing `xcltk-0.1.9/setup.py` & `xcltk-0.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # setup.py
-# Author: Xianjie Huang (hxj5@hku.hk)
+# Author: Xianjie Huang (xianjie5@connect.hku.hk)
 
 from setuptools import setup, find_packages
 from codecs import open
 from os import path
 import sys
 
 here = path.abspath(path.dirname(__file__))
@@ -11,15 +11,16 @@
 # load configures
 exec(open("./xcltk/config.py").read())
 
 # Get the long description from the relevant file
 with open(path.join(here, "README.md"), encoding='utf-8') as f:
     long_description = f.read()
 
-reqs = ['numpy>=1.9.0', 'pysam>=0.15.2']
+reqs = ['numpy>=1.9.0', 'pysam>=0.15.2', 'intervaltree', 'scipy', 'h5py',
+        'pandas', 'anndata']
 
 setup(
     name = "xcltk",
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
@@ -30,15 +31,15 @@
     long_description_content_type = "text/markdown",
 
     # The project's main homepage.
     url = "https://github.com/hxj5/xcltk",
 
     # Author details
     author = 'Xianjie Huang',
-    author_email = 'hxj5@hku.hk',
+    author_email = 'xianjie5@connect.hku.hk',
 
     # Choose your license
     license='Apache-2.0',
 
     # What does your project relate to?
     keywords=['xclone', 'toolkit'],
 
@@ -68,8 +69,8 @@
     install_requires = reqs,
 
     py_modules = ['xcltk']
 
     # buid the distribution: python setup.py sdist
     # upload to pypi: twine upload dist/...
 
-)
+)
```

### Comparing `xcltk-0.1.9/xcltk/region/convert.py` & `xcltk-0.3.0/xcltk/tools/convert.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-# Convert Region file format
-# Author: Xianjie Huang 
+# convert.py - convert formats between genomic features.
+
+#TODO:
+#- use getopt to re-implement cmdline.
 
 import os
 import sys
+
 from optparse import OptionParser
-from ..utils.region import get_fixsize_regions, load_regions, output_regions
-from .config import APP
-from ..config import VERSION
+
+from ..config import APP, VERSION
+from ..utils.gregion import get_fixsize_regions, load_regions, output_regions
 
 COMMAND = "convert"
 
-def convert(argv):
+def convert_main(argv):
     # parse command line options
     if len(argv) < 3:
         sys.stderr.write("Welcome to %s %s v%s!\n\n" % (APP, COMMAND, VERSION))
         sys.stderr.write("use -h or --help for help on argument.\n")
         sys.exit(1)
 
     parser = OptionParser(usage = "Usage: %s %s [options]" % (APP, COMMAND))
@@ -73,11 +76,8 @@
     else:
         reg_list = load_regions(in_file, in_type)
     if not reg_list:
         sys.stderr.write("Error: empty region file or failed to parse regions.\n")
         sys.exit(1)
 
     # output regions
-    output_regions(reg_list, out_file, out_type)
-
-if __name__ == "__main__":
-    convert(sys.argv)
+    output_regions(reg_list, out_file, out_type)
```

### Comparing `xcltk-0.1.9/xcltk/utils/gtf.py` & `xcltk-0.3.0/xcltk/utils/gtf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+# gtf.py - simple GTF/GFF file parser.
+
 # This module is to parse the gtf file, whoes format can be found at:
 # www.ensembl.org/info/website/upload/gff.html
 # Author: Yuanhua Huang
 
 # Note: here we need the order of feature lines like this: gene --> transcript
 # --> exon 1 --> exon 2 ..., which is not required for the gtf format. But this
 # assumption is usually right for the gtf file downloaded from Ensembl database.
 
-import sys
-import subprocess
 import numpy as np
+import subprocess
+
 
 class Transcript:
     def __init__(self, chrom, strand, start, stop, tran_id, tran_name="*", 
         biotype="*"):
         """a general purpose transcript object with the basic information.
         """
         self.chrom  = chrom
```

### Comparing `xcltk-0.1.9/xcltk/utils/region.py` & `xcltk-0.3.0/xcltk/utils/gregion.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-# Utils for Genome Region Processing
-# Author: Xianjie Huang 
+# gregion.py - utils for genome region processing
+
 
 # TODO: add bgzip support
 
+import gzip 
 import os
 import sys
-import gzip 
+
 from .gtf import load_genes
 
 CHROM_LEN_HG19 = (249250621, 243199373, 198022430, 191154276, 180915260, 171115067,  # chr1 - chr6
                   159138663, 146364022, 141213431, 135534747, 135006516, 133851895,  # chr7 - chr12
                   115169878, 107349540, 102531392, 90354753, 81195210, 78077248,     # chr13 - chr 18
                   59128983, 63025520, 48129895, 51304566, 155270560, 59373566)       # chr19 - chrY
```

### Comparing `xcltk-0.1.9/xcltk/utils/sam.py` & `xcltk-0.3.0/xcltk/utils/sam.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,9 @@
-# Copied from cellSNP, https://github.com/single-cell-genetics/cellSNP/blob/purePython/cellSNP/utils/cellsnp_utils.py
-# SAM file utils 
-# Author: Xianjie Huang
+# sam.py - SAM/BAM file routine
 
-# Operations of CIGAR, copied from pysam (https://pysam.readthedocs.io/en/latest/api.html#pysam.AlignedSegment.cigartuples)
-# Do not change these values unless you know what you are doing.
-BAM_CMATCH = 0
-BAM_CINS = 1
-BAM_CDEL = 2
-BAM_CREF_SKIP = 3
-BAM_CSOFT_CLIP = 4
-BAM_CHARD_CLIP = 5
-BAM_CPAD = 6
-BAM_CEQUAL = 7
-BAM_CDIFF = 8
-BAM_CBACK = 9
 
 def get_query_bases(read, full_length=False):
     """
     @abstract            Return a list of bases in qurey sequence that are within the alignment.
     @param read          An AlignedSegment object. [AlignedSegment]
     @param full_length   If full_length is set, None values will be included for any soft-clipped or 
                          unaligned positions within the read. The returned list will thus be of the 
@@ -41,14 +27,15 @@
         elif op == BAM_CMATCH or op == BAM_CEQUAL or op == BAM_CDIFF:
             for i in range(pos, pos + l):
                 result.append(s[i])
             pos += l
         # else: do nothing.
     return result
 
+
 def get_query_qualities(read, full_length=False):
     """
     @abstract            Return a list of qualities in qurey quality sequence that are within the alignment.
     @param read          An AlignedSegment object. [AlignedSegment]
     @param full_length   If full_length is set, None values will be included for any soft-clipped or 
                          unaligned positions within the read. The returned list will thus be of the 
                          same length as the read. [bint]
@@ -74,7 +61,47 @@
         elif op == BAM_CMATCH or op == BAM_CEQUAL or op == BAM_CDIFF:
             for i in range(pos, pos + l):
                 result.append(s[i])
             pos += l
         # else: do nothing.
     return result
 
+
+def sam_fetch(sam, chrom, start, end):
+    """Provide a wrapper for sam-fetch method that could automatically
+       handle chrom with or without "chr" prefix.
+    @param sam    A pysam.AlignmentFile object.
+    @param chrom  Chromosome name [str]
+    @param start  1-based, inclusive [int]
+    @param end    1-based, inclusive [int]
+    @return       Iterator if success, None otherwise. 
+    """
+    try:   # sam.fetch(): start and stop denote 0-based, half-open intervals.
+        itr = sam.fetch(chrom, start - 1, end) 
+    except:
+        pass
+    else:
+        if itr:
+            return itr
+    chrom = chrom[3:] if chrom.startswith("chr") else "chr" + chrom
+    try:
+        itr = sam.fetch(chrom, start - 1, end)
+    except:
+        return None
+    else:
+        return itr if itr else None
+
+BAM_FPAIRED = 1
+BAM_FPROPER_PAIR = 2
+
+# Cigar
+# reference: https://pysam.readthedocs.io/en/latest/api.html#pysam.AlignedSegment.cigartuples
+BAM_CMATCH = 0
+BAM_CINS = 1
+BAM_CDEL = 2
+BAM_CREF_SKIP = 3
+BAM_CSOFT_CLIP = 4
+BAM_CHARD_CLIP = 5
+BAM_CPAD = 6
+BAM_CEQUAL = 7
+BAM_CDIFF = 8
+BAM_CBACK = 9
```

