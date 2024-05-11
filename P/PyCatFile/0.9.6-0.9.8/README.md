# Comparing `tmp/pycatfile-0.9.6.tar.gz` & `tmp/pycatfile-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycatfile-0.9.6.tar", last modified: Thu May  2 01:20:02 2024, max compression
+gzip compressed data, was "pycatfile-0.9.8.tar", last modified: Thu May  2 22:03:30 2024, max compression
```

## Comparing `pycatfile-0.9.6.tar` & `pycatfile-0.9.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:20:02.152612 pycatfile-0.9.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-02 01:19:48.000000 pycatfile-0.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-02 01:20:02.152612 pycatfile-0.9.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:20:02.152612 pycatfile-0.9.6/PyCatFile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-02 01:20:02.000000 pycatfile-0.9.6/PyCatFile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-02 01:20:02.000000 pycatfile-0.9.6/PyCatFile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 01:20:02.000000 pycatfile-0.9.6/PyCatFile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 01:20:02.000000 pycatfile-0.9.6/PyCatFile.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 01:20:02.000000 pycatfile-0.9.6/PyCatFile.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-02 01:19:48.000000 pycatfile-0.9.6/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     9956 2024-05-02 01:19:48.000000 pycatfile-0.9.6/catfile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4968 2024-05-02 01:19:48.000000 pycatfile-0.9.6/neocatfile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   305902 2024-05-02 01:19:48.000000 pycatfile-0.9.6/pycatfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-02 01:20:02.152612 pycatfile-0.9.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     5450 2024-05-02 01:19:48.000000 pycatfile-0.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:03:30.812369 pycatfile-0.9.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-02 22:03:19.000000 pycatfile-0.9.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-02 22:03:30.812369 pycatfile-0.9.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:03:30.808369 pycatfile-0.9.8/PyCatFile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-02 22:03:30.000000 pycatfile-0.9.8/PyCatFile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-02 22:03:30.000000 pycatfile-0.9.8/PyCatFile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 22:03:30.000000 pycatfile-0.9.8/PyCatFile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 22:03:30.000000 pycatfile-0.9.8/PyCatFile.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 22:03:30.000000 pycatfile-0.9.8/PyCatFile.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-02 22:03:19.000000 pycatfile-0.9.8/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9956 2024-05-02 22:03:19.000000 pycatfile-0.9.8/catfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4968 2024-05-02 22:03:19.000000 pycatfile-0.9.8/neocatfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   306721 2024-05-02 22:03:19.000000 pycatfile-0.9.8/pycatfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-02 22:03:30.812369 pycatfile-0.9.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5450 2024-05-02 22:03:19.000000 pycatfile-0.9.8/setup.py
```

### Comparing `pycatfile-0.9.6/LICENSE` & `pycatfile-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pycatfile-0.9.6/PKG-INFO` & `pycatfile-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCatFile
-Version: 0.9.6
+Version: 0.9.8
 Summary: A tar like file format name catfile after unix cat command (concatenate files) .
 Home-page: https://github.com/GameMaker2k/PyCatFile
 Download-URL: https://github.com/GameMaker2k/PyCatFile/archive/master.tar.gz
 Author: Kazuki Przyborowski
 Author-email: kazuki.przyborowski@gmail.com
 Maintainer: Kazuki Przyborowski
 Maintainer-email: kazuki.przyborowski@gmail.com
```

### Comparing `pycatfile-0.9.6/PyCatFile.egg-info/PKG-INFO` & `pycatfile-0.9.8/PyCatFile.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCatFile
-Version: 0.9.6
+Version: 0.9.8
 Summary: A tar like file format name catfile after unix cat command (concatenate files) .
 Home-page: https://github.com/GameMaker2k/PyCatFile
 Download-URL: https://github.com/GameMaker2k/PyCatFile/archive/master.tar.gz
 Author: Kazuki Przyborowski
 Author-email: kazuki.przyborowski@gmail.com
 Maintainer: Kazuki Przyborowski
 Maintainer-email: kazuki.przyborowski@gmail.com
```

### Comparing `pycatfile-0.9.6/catfile.py` & `pycatfile-0.9.8/catfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2018-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2018-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2018-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: catfile.py - Last Update: 5/1/2024 Ver. 0.9.6 RC 1 - Author: cooldude2k $
+    $FileInfo: catfile.py - Last Update: 5/2/2024 Ver. 0.9.8 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import sys, argparse, pycatfile, binascii;
 
 rarfile_support = pycatfile.rarfile_support;
 py7zr_support = pycatfile.py7zr_support;
```

### Comparing `pycatfile-0.9.6/neocatfile.py` & `pycatfile-0.9.8/neocatfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2018-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2018-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2018-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: neocatfile.py - Last Update: 5/1/2024 Ver. 0.9.6 RC 1 - Author: cooldude2k $
+    $FileInfo: neocatfile.py - Last Update: 5/2/2024 Ver. 0.9.8 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 import argparse
 import pycatfile
 
 # Compatibility layer for Python 2 and 3 input
```

### Comparing `pycatfile-0.9.6/pycatfile.py` & `pycatfile-0.9.8/pycatfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2018-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2018-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2018-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: pycatfile.py - Last Update: 5/1/2024 Ver. 0.9.6 RC 1 - Author: cooldude2k $
+    $FileInfo: pycatfile.py - Last Update: 5/2/2024 Ver. 0.9.8 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import io, os, re, sys, time, stat, zlib, base64, shutil, socket, hashlib, datetime, logging, binascii, tempfile, zipfile, platform;
 from ftplib import FTP, FTP_TLS;
 if(sys.version[0]=="2"):
  from urlparse import urlparse, urlunparse;
@@ -71,26 +71,26 @@
 try:
  import py7zr;
  py7zr_support = True;
 except ImportError:
  py7zr_support = False;
 
 try:
- from safetar import is_tarfile;
+ from xtarfile import is_tarfile;
 except ImportError:
  try:
-  from xtarfile import is_tarfile;
+  from safetar import is_tarfile;
  except ImportError:
   from tarfile import is_tarfile;
 
 try:
- import safetar as tarfile;
+ import xtarfile as tarfile;
 except ImportError:
  try:
-  import xtarfile as tarfile;
+  import safetar as tarfile;
  except ImportError:
   import tarfile;
 
 haveparamiko = False;
 try:
  import paramiko;
  haveparamiko = True;
@@ -170,19 +170,19 @@
 __file_format_ver__ = "001";
 __use_new_style__ = True;
 __use_advanced_list__ = True;
 __use_alt_inode__ = False;
 __file_format_list__ = [__file_format_name__, __file_format_magic__, __file_format_lower__, __file_format_len__, __file_format_hex__, __file_format_delimiter__, __file_format_ver__, __use_new_style__, __use_advanced_list__, __use_alt_inode__];
 __project__ = __program_name__;
 __project_url__ = "https://github.com/GameMaker2k/PyCatFile";
-__version_info__ = (0, 9, 6, "RC 1", 1);
-__version_date_info__ = (2024, 5, 1, "RC 1", 1);
+__version_info__ = (0, 9, 8, "RC 1", 1);
+__version_date_info__ = (2024, 5, 2, "RC 1", 1);
 __version_date__ = str(__version_date_info__[0]) + "." + str(__version_date_info__[1]).zfill(2) + "." + str(__version_date_info__[2]).zfill(2);
 __revision__ = __version_info__[3];
-__revision_id__ = "$Id: 4567eb777c3f1cb3b1adf49788eb5c726205e3a4 $";
+__revision_id__ = "$Id: ad42ecf2819cb02c641b22df40a08ef89c87beed $";
 if(__version_info__[4] is not None):
  __version_date_plusrc__ = __version_date__ + "-" + str(__version_date_info__[4]);
 if(__version_info__[4] is None):
  __version_date_plusrc__ = __version_date__;
 if(__version_info__[3] is not None):
  __version__ = str(__version_info__[0]) + "." + str(__version_info__[1]) + "." + str(__version_info__[2]) + " " + str(__version_info__[3]);
 if(__version_info__[3] is None):
@@ -1758,14 +1758,27 @@
  if(prefp==binascii.unhexlify("894c5a4f000d0a1a0a")):
   filetype = "lzo";
  catfp.seek(0, 0);
  prefp = catfp.read(10);
  if(prefp==binascii.unhexlify("7061785f676c6f62616c")):
   filetype = "tarfile";
  catfp.seek(0, 0);
+ if(filetype=="gzip" or filetype=="bzip2" or filetype=="lzma" or filetype=="zstd" or filetype=="lz4"):
+  if(is_tarfile(catfp)):
+   filetype = "tarfile";
+ if(not filetype):
+  if(is_tarfile(catfp)):
+   filetype = "tarfile";
+  elif(zipfile.is_zipfile(catfp)):
+   filetype = "zipfile";
+  elif(rarfile.is_rarfile(catfp) or rarfile.is_rarfile_sfx(catfp)):
+   filetype = "rarile";
+  else:
+   filetype = False;
+ catfp.seek(0, 0);
  if(closefp):
   catfp.close();
  return filetype;
 
 def CheckCompressionTypeFromString(instring, formatspecs=__file_format_list__, closefp=True):
  try:
   instringsfile = BytesIO(instring);
@@ -1998,15 +2011,26 @@
    compresscheck = "lz4";
   elif(fextname==".lzo" or fextname==".lzop"):
    compresscheck = "lzo";
   elif(fextname==".lzma" or fextname==".xz"):
    compresscheck = "lzma";
   else:
    return False;
+ if(compresscheck=="gzip" or compresscheck=="bzip2" or compresscheck=="lzma" or compresscheck=="zstd" or compresscheck=="lz4"):
+  if(is_tarfile(catfp)):
+   filetype = "tarfile";
  if(not compresscheck):
+  if(is_tarfile(infile)):
+   return "tarfile";
+  elif(zipfile.is_zipfile(infile)):
+   return "zipfile";
+  elif(rarfile.is_rarfile(infile) or rarfile.is_rarfile_sfx(infile)):
+   return "rarile";
+  else:
+   return False;
   return False;
  if(compresscheck=="catfile"):
   return "catfile";
  if(compresscheck==formatspecs[2]):
   return formatspecs[2];
  if(compresscheck=="tarfile"):
   return "tarfile";
```

### Comparing `pycatfile-0.9.6/setup.py` & `pycatfile-0.9.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2016-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2016-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2016-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: setup.py - Last Update: 5/1/2024 Ver. 0.9.6 RC 1 - Author: cooldude2k $
+    $FileInfo: setup.py - Last Update: 5/2/2024 Ver. 0.9.8 RC 1 - Author: cooldude2k $
 '''
 
 import os, re, sys, pkg_resources;
 from setuptools import setup;
 
 verinfofilename = os.path.realpath("."+os.path.sep+os.path.sep+"pycatfile.py");
 verinfofile = open(verinfofilename, "r");
```

