# Comparing `tmp/muti.basic-0.0.7.tar.gz` & `tmp/muti_basic-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muti.basic-0.0.7.tar", last modified: Tue Apr  2 10:13:24 2024, max compression
+gzip compressed data, was "muti_basic-0.0.8.tar", last modified: Sat May 11 02:54:56 2024, max compression
```

## Comparing `muti.basic-0.0.7.tar` & `muti_basic-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 10:13:24.545206 muti.basic-0.0.7/
--rw-rw-rw-   0        0        0     1088 2024-03-26 07:23:35.000000 muti.basic-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      437 2024-04-02 10:13:24.544207 muti.basic-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-03-25 03:22:38.000000 muti.basic-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 10:13:24.536698 muti.basic-0.0.7/basic/
--rw-rw-rw-   0        0        0      695 2024-03-29 10:47:00.000000 muti.basic-0.0.7/basic/__deps__.py
--rw-rw-rw-   0        0        0      139 2024-04-02 01:56:47.000000 muti.basic-0.0.7/basic/__init__.py
--rw-rw-rw-   0        0        0   246355 2024-04-02 01:56:39.000000 muti.basic-0.0.7/basic/carLam.py
--rw-rw-rw-   0        0        0     3576 2024-04-02 01:56:33.000000 muti.basic-0.0.7/basic/depLam.py
--rw-rw-rw-   0        0        0     3027 2024-04-02 01:57:00.000000 muti.basic-0.0.7/basic/getLam.py
--rw-rw-rw-   0        0        0     3400 2024-04-02 01:57:04.000000 muti.basic-0.0.7/basic/parLam.py
--rw-rw-rw-   0        0        0     2185 2024-04-02 01:58:44.000000 muti.basic-0.0.7/basic/typLas.py
-drwxrwxrwx   0        0        0        0 2024-04-02 10:13:24.544207 muti.basic-0.0.7/muti.basic.egg-info/
--rw-rw-rw-   0        0        0      437 2024-04-02 10:13:24.000000 muti.basic-0.0.7/muti.basic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2024-04-02 10:13:24.000000 muti.basic-0.0.7/muti.basic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 10:13:24.000000 muti.basic-0.0.7/muti.basic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-02 10:13:24.000000 muti.basic-0.0.7/muti.basic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 10:13:24.545206 muti.basic-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      616 2024-04-02 10:13:20.000000 muti.basic-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 02:54:56.307819 muti_basic-0.0.8/
+-rw-rw-rw-   0        0        0     1088 2024-04-24 08:40:13.000000 muti_basic-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      437 2024-05-11 02:54:56.306822 muti_basic-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-03-25 03:22:38.000000 muti_basic-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 02:54:56.280812 muti_basic-0.0.8/basic/
+-rw-rw-rw-   0        0        0    18633 2024-05-09 08:15:42.000000 muti_basic-0.0.8/basic/__deps__.py
+-rw-rw-rw-   0        0        0      254 2024-04-30 09:22:22.000000 muti_basic-0.0.8/basic/__init__.py
+-rw-rw-rw-   0        0        0     1042 2024-04-30 02:57:03.000000 muti_basic-0.0.8/basic/cetLam.py
+-rw-rw-rw-   0        0        0   246349 2024-04-17 13:36:31.000000 muti_basic-0.0.8/basic/chrLam.py
+-rw-rw-rw-   0        0        0     1013 2024-05-09 08:18:13.000000 muti_basic-0.0.8/basic/decLam.py
+-rw-rw-rw-   0        0        0     7207 2024-04-30 09:24:43.000000 muti_basic-0.0.8/basic/depLam.py
+-rw-rw-rw-   0        0        0     4486 2024-04-25 11:58:52.000000 muti_basic-0.0.8/basic/getLam.py
+-rw-rw-rw-   0        0        0        0 2024-04-12 02:49:19.000000 muti_basic-0.0.8/basic/itrLam.py
+-rw-rw-rw-   0        0        0    12045 2024-04-17 13:36:31.000000 muti_basic-0.0.8/basic/metLas.py
+-rw-rw-rw-   0        0        0      324 2024-04-12 08:49:33.000000 muti_basic-0.0.8/basic/nymLas.py
+-rw-rw-rw-   0        0        0     4489 2024-04-25 11:58:52.000000 muti_basic-0.0.8/basic/parLam.py
+-rw-rw-rw-   0        0        0      298 2024-04-17 12:39:46.000000 muti_basic-0.0.8/basic/proces.py
+-rw-rw-rw-   0        0        0      349 2024-04-09 02:23:12.000000 muti_basic-0.0.8/basic/setLam.py
+-rw-rw-rw-   0        0        0     9093 2024-04-16 02:41:13.000000 muti_basic-0.0.8/basic/tstLas.py
+-rw-rw-rw-   0        0        0     2662 2024-04-30 09:26:09.000000 muti_basic-0.0.8/basic/tyeLas.py
+-rw-rw-rw-   0        0        0      362 2024-04-03 02:34:43.000000 muti_basic-0.0.8/basic/typLam.py
+-rw-rw-rw-   0        0        0     8839 2024-05-10 02:58:47.000000 muti_basic-0.0.8/basic/typLas.py
+drwxrwxrwx   0        0        0        0 2024-05-11 02:54:56.305825 muti_basic-0.0.8/muti.basic.egg-info/
+-rw-rw-rw-   0        0        0      437 2024-05-11 02:54:56.000000 muti_basic-0.0.8/muti.basic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      438 2024-05-11 02:54:56.000000 muti_basic-0.0.8/muti.basic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 02:54:56.000000 muti_basic-0.0.8/muti.basic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-11 02:54:56.000000 muti_basic-0.0.8/muti.basic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-11 02:54:56.307819 muti_basic-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      616 2024-05-11 02:54:42.000000 muti_basic-0.0.8/setup.py
```

### Comparing `muti.basic-0.0.7/LICENSE` & `muti_basic-0.0.8/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -2,8 +2,8 @@
 
 Copyright (c) 王氾超 E.Codeine.Ares 2014
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUD OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `muti.basic-0.0.7/basic/carLam.py` & `muti_basic-0.0.8/basic/chrLam.py`

 * *Files 0% similar despite different names*

```diff
@@ -15368,31 +15368,30 @@
 0003c070: 7cef bfa7 7cef bfa8 7cef bfa9 7cef bfaa  |...|...|...|...
 0003c080: 7cef bfab 7cef bfac 7cef bfad 7cef bfae  |...|...|...|...
 0003c090: 7cef bfaf 7cef bfb9 7cef bfba 7cef bfbb  |...|...|...|...
 0003c0a0: 7cef bfbc 7cef bfbd 2220 7d0d 0a0d 0a64  |...|..." }....d
 0003c0b0: 6566 2067 6574 7243 4944 2820 6c69 2c20  ef getrCID( li, 
 0003c0c0: 6663 3d27 554e 4943 4f44 4527 293a 0d0a  fc='UNICODE'):..
 0003c0d0: 2020 2020 2372 6574 7572 6e20 6765 7472      #return getr
-0003c0e0: 4349 445f 4469 6328 206c 692c 2067 6c6f  CID_Dic( li, glo
-0003c0f0: 6261 6c73 2829 5b66 635d 290d 0a20 2020  bals()[fc])..   
-0003c100: 2069 6620 6663 2069 6e20 5b27 554e 4943   if fc in ['UNIC
-0003c110: 4f44 4527 5d3a 2072 6574 7572 6e20 6765  ODE']: return ge
-0003c120: 7472 4349 445f 4469 6328 206c 692c 2055  trCID_Dic( li, U
-0003c130: 4e49 434f 4445 290d 0a20 2020 2065 6c73  NICODE)..    els
-0003c140: 653a 2072 6574 7572 6e20 300d 0a0d 0a64  e: return 0....d
-0003c150: 6566 2067 6574 7243 4944 5f44 6963 2820  ef getrCID_Dic( 
-0003c160: 6c69 2c20 6469 6329 3a0d 0a20 2020 2066  li, dic):..    f
-0003c170: 6f72 206b 2c76 2069 6e20 7265 7665 7273  or k,v in revers
-0003c180: 6564 2864 6963 2e69 7465 6d73 2829 293a  ed(dic.items()):
-0003c190: 0d0a 2020 2020 2020 2020 5f6b 203d 206b  ..        _k = k
-0003c1a0: 202a 2031 3620 2330 7846 2b31 0d0a 2020   * 16 #0xF+1..  
-0003c1b0: 2020 2020 2020 6966 2020 6c69 203c 205f        if  li < _
-0003c1c0: 6b20 3a20 636f 6e74 696e 7565 0d0a 2020  k : continue..  
-0003c1d0: 2020 2020 2020 7265 7475 726e 2020 2020        return    
-0003c1e0: 765b 322a 286c 692d 5f6b 295d 0d0a 0d0a  v[2*(li-_k)]....
-0003c1f0: 2320 6465 6620 6869 6d28 293f 20e6 8ab1  # def him()? ...
-0003c200: e6ad 89ef bc8c e6af 8de7 8988 e4b8 8de5  ................
-0003c210: ae9a e4b9 8920 6869 6d2d 6c61 6d0d 0a69  ..... him-lam..i
-0003c220: 6620 4865 7228 5f5f 6e61 6d65 5f5f 293a  f Her(__name__):
-0003c230: 2070 7269 6e74 2867 6574 7243 4944 2820   print(getrCID( 
-0003c240: 3131 302c 2066 633d 2755 4e49 434f 4445  110, fc='UNICODE
-0003c250: 2729 29                                  '))
+0003c0e0: 4349 445f 4469 6328 206c 692c 2054 414c  CID_Dic( li, TAL
+0003c0f0: 2866 6329 290d 0a20 2020 2069 6620 6663  (fc))..    if fc
+0003c100: 2069 6e20 5b27 554e 4943 4f44 4527 5d3a   in ['UNICODE']:
+0003c110: 2072 6574 7572 6e20 6765 7472 4349 445f   return getrCID_
+0003c120: 4469 6328 206c 692c 2055 4e49 434f 4445  Dic( li, UNICODE
+0003c130: 290d 0a20 2020 2065 6c73 653a 2072 6574  )..    else: ret
+0003c140: 7572 6e20 300d 0a0d 0a64 6566 2067 6574  urn 0....def get
+0003c150: 7243 4944 5f44 6963 2820 6c69 2c20 6469  rCID_Dic( li, di
+0003c160: 6329 3a0d 0a20 2020 2066 6f72 206b 2c76  c):..    for k,v
+0003c170: 2069 6e20 7265 7665 7273 6564 2864 6963   in reversed(dic
+0003c180: 2e69 7465 6d73 2829 293a 0d0a 2020 2020  .items()):..    
+0003c190: 2020 2020 5f6b 203d 206b 202a 2031 3620      _k = k * 16 
+0003c1a0: 2330 7846 2b31 0d0a 2020 2020 2020 2020  #0xF+1..        
+0003c1b0: 6966 2020 6c69 203c 205f 6b20 3a20 636f  if  li < _k : co
+0003c1c0: 6e74 696e 7565 0d0a 2020 2020 2020 2020  ntinue..        
+0003c1d0: 7265 7475 726e 2020 2020 765b 322a 286c  return    v[2*(l
+0003c1e0: 692d 5f6b 295d 0d0a 0d0a 2320 6465 6620  i-_k)]....# def 
+0003c1f0: 6869 6d28 293f 20e6 8ab1 e6ad 89ef bc8c  him()? .........
+0003c200: e6af 8de7 8988 e4b8 8de5 ae9a e4b9 8920  ............... 
+0003c210: 6869 6d2d 6c61 6d0d 0a69 6620 4865 7228  him-lam..if Her(
+0003c220: 5f5f 6e61 6d65 5f5f 293a 2070 7269 6e74  __name__): print
+0003c230: 2867 6574 7243 4944 2820 3131 302c 2066  (getrCID( 110, f
+0003c240: 633d 2755 4e49 434f 4445 2729 29         c='UNICODE'))
```

### Comparing `muti.basic-0.0.7/setup.py` & `muti_basic-0.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name         = "muti.basic",
-  version      = "0.0.7",
+  version      = "0.0.8",
   author       = "E.C.Ares",
   author_email = "E.C.Ares@outlook.com",
   url          = "https://github.com/E-C-Ares/",
   description  = "utils for pytorch",
   packages     = setuptools.find_packages(),
   classifiers  = [
   "Programming Language :: Python :: 3",
```

