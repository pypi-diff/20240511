# Comparing `tmp/ngstoolkits-1.0.0rc7.tar.gz` & `tmp/ngstoolkits-1.0.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/liubo/git_sync/ngstoolkits/dist/.tmp-tynvbdkg/ngstoolkits-1.0.0rc7.tar", last modified: Tue May  7 06:25:23 2024, max compression
+gzip compressed data, was "/Users/liubo/git_sync/ngstoolkits/dist/.tmp-qy96k84n/ngstoolkits-1.0.0rc8.tar", last modified: Sat May 11 07:07:00 2024, max compression
```

## Comparing `ngstoolkits-1.0.0rc7.tar` & `ngstoolkits-1.0.0rc8.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-05-07 06:25:23.297282 ngstoolkits-1.0.0rc7/
--rw-r--r--   0 liubo      (501) staff       (20)      594 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc7/.coveragerc
--rw-r--r--   0 liubo      (501) staff       (20)      583 2024-05-07 05:55:29.000000 ngstoolkits-1.0.0rc7/.gitignore
--rw-r--r--   0 liubo      (501) staff       (20)      529 2024-05-07 05:57:20.000000 ngstoolkits-1.0.0rc7/.readthedocs.yml
--rw-r--r--   0 liubo      (501) staff       (20)       69 2024-05-07 03:50:19.000000 ngstoolkits-1.0.0rc7/AUTHORS.md
--rw-r--r--   0 liubo      (501) staff       (20)       51 2024-05-07 04:02:32.000000 ngstoolkits-1.0.0rc7/CHANGELOG.md
--rw-r--r--   0 liubo      (501) staff       (20)    13529 2024-05-07 03:50:33.000000 ngstoolkits-1.0.0rc7/CONTRIBUTING.md
--rw-r--r--   0 liubo      (501) staff       (20)     1084 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc7/LICENSE.txt
--rw-r--r--   0 liubo      (501) staff       (20)     2942 2024-05-07 06:25:23.296975 ngstoolkits-1.0.0rc7/PKG-INFO
--rw-r--r--   0 liubo      (501) staff       (20)     2058 2024-05-07 03:49:31.000000 ngstoolkits-1.0.0rc7/README.md
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-05-07 06:25:23.259857 ngstoolkits-1.0.0rc7/docs/
--rw-r--r--   0 liubo      (501) staff       (20)     1154 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc7/docs/Makefile
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-05-07 06:25:23.261295 ngstoolkits-1.0.0rc7/docs/_static/
--rw-r--r--   0 liubo      (501) staff       (20)       18 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc7/docs/_static/.gitignore
--rw-r--r--   0 liubo      (501) staff       (20)       71 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc7/docs/authors.md
--rw-r--r--   0 liubo      (501) staff       (20)       73 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc7/docs/changelog.md
--rw-r--r--   0 liubo      (501) staff       (20)    10054 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc7/docs/conf.py
--rw-r--r--   0 liubo      (501) staff       (20)       76 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc7/docs/contributing.md
--rw-r--r--   0 liubo      (501) staff       (20)      956 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc7/docs/index.md
--rw-r--r--   0 liubo      (501) staff       (20)       66 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc7/docs/license.md
--rw-r--r--   0 liubo      (501) staff       (20)       70 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc7/docs/readme.md
--rw-r--r--   0 liubo      (501) staff       (20)      254 2024-04-29 06:45:11.000000 ngstoolkits-1.0.0rc7/docs/requirements.txt
--rw-r--r--   0 liubo      (501) staff       (20)      353 2024-05-06 09:35:30.000000 ngstoolkits-1.0.0rc7/pyproject.toml
--rw-r--r--   0 liubo      (501) staff       (20)     1424 2024-05-07 06:25:23.302969 ngstoolkits-1.0.0rc7/setup.cfg
--rw-r--r--   0 liubo      (501) staff       (20)      982 2024-04-29 06:21:59.000000 ngstoolkits-1.0.0rc7/setup.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-05-07 06:25:23.218369 ngstoolkits-1.0.0rc7/src/
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-05-07 06:25:23.267482 ngstoolkits-1.0.0rc7/src/ngstoolkits/
--rw-r--r--   0 liubo      (501) staff       (20)      398 2024-05-07 06:11:10.000000 ngstoolkits-1.0.0rc7/src/ngstoolkits/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)    12876 2024-05-07 03:18:15.000000 ngstoolkits-1.0.0rc7/src/ngstoolkits/ngs_class.py
--rw-r--r--   0 liubo      (501) staff       (20)      883 2024-05-07 03:49:47.000000 ngstoolkits-1.0.0rc7/src/ngstoolkits/sequence.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-05-07 06:25:23.292964 ngstoolkits-1.0.0rc7/src/ngstoolkits.egg-info/
--rw-r--r--   0 liubo      (501) staff       (20)     2942 2024-05-07 06:25:23.000000 ngstoolkits-1.0.0rc7/src/ngstoolkits.egg-info/PKG-INFO
--rw-r--r--   0 liubo      (501) staff       (20)      671 2024-05-07 06:25:23.000000 ngstoolkits-1.0.0rc7/src/ngstoolkits.egg-info/SOURCES.txt
--rw-r--r--   0 liubo      (501) staff       (20)        1 2024-05-07 06:25:23.000000 ngstoolkits-1.0.0rc7/src/ngstoolkits.egg-info/dependency_links.txt
--rw-r--r--   0 liubo      (501) staff       (20)        1 2024-04-29 06:53:14.000000 ngstoolkits-1.0.0rc7/src/ngstoolkits.egg-info/not-zip-safe
--rw-r--r--   0 liubo      (501) staff       (20)       92 2024-05-07 06:25:23.000000 ngstoolkits-1.0.0rc7/src/ngstoolkits.egg-info/requires.txt
--rw-r--r--   0 liubo      (501) staff       (20)       12 2024-05-07 06:25:23.000000 ngstoolkits-1.0.0rc7/src/ngstoolkits.egg-info/top_level.txt
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-05-07 06:25:23.290961 ngstoolkits-1.0.0rc7/tests/
--rw-r--r--   0 liubo      (501) staff       (20)      279 2024-05-07 03:50:43.000000 ngstoolkits-1.0.0rc7/tests/conftest.py
--rw-r--r--   0 liubo      (501) staff       (20)      931 2024-05-07 03:32:45.000000 ngstoolkits-1.0.0rc7/tests/test_class.py
--rw-r--r--   0 liubo      (501) staff       (20)     2861 2024-04-29 06:44:15.000000 ngstoolkits-1.0.0rc7/tox.ini
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-05-11 07:07:00.324946 ngstoolkits-1.0.0rc8/
+-rw-r--r--   0 liubo      (501) staff       (20)      594 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc8/.coveragerc
+-rw-r--r--   0 liubo      (501) staff       (20)      583 2024-05-07 05:55:29.000000 ngstoolkits-1.0.0rc8/.gitignore
+-rw-r--r--   0 liubo      (501) staff       (20)      529 2024-05-07 05:57:20.000000 ngstoolkits-1.0.0rc8/.readthedocs.yml
+-rw-r--r--   0 liubo      (501) staff       (20)       69 2024-05-07 03:50:19.000000 ngstoolkits-1.0.0rc8/AUTHORS.md
+-rw-r--r--   0 liubo      (501) staff       (20)       51 2024-05-07 04:02:32.000000 ngstoolkits-1.0.0rc8/CHANGELOG.md
+-rw-r--r--   0 liubo      (501) staff       (20)    13529 2024-05-07 03:50:33.000000 ngstoolkits-1.0.0rc8/CONTRIBUTING.md
+-rw-r--r--   0 liubo      (501) staff       (20)     1084 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc8/LICENSE.txt
+-rw-r--r--   0 liubo      (501) staff       (20)     2965 2024-05-11 07:07:00.324582 ngstoolkits-1.0.0rc8/PKG-INFO
+-rw-r--r--   0 liubo      (501) staff       (20)     2058 2024-05-07 03:49:31.000000 ngstoolkits-1.0.0rc8/README.md
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-05-11 07:07:00.290261 ngstoolkits-1.0.0rc8/docs/
+-rw-r--r--   0 liubo      (501) staff       (20)     1154 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc8/docs/Makefile
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-05-11 07:07:00.292117 ngstoolkits-1.0.0rc8/docs/_static/
+-rw-r--r--   0 liubo      (501) staff       (20)       18 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc8/docs/_static/.gitignore
+-rw-r--r--   0 liubo      (501) staff       (20)       71 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc8/docs/authors.md
+-rw-r--r--   0 liubo      (501) staff       (20)       73 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc8/docs/changelog.md
+-rw-r--r--   0 liubo      (501) staff       (20)    10054 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc8/docs/conf.py
+-rw-r--r--   0 liubo      (501) staff       (20)       76 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc8/docs/contributing.md
+-rw-r--r--   0 liubo      (501) staff       (20)      956 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc8/docs/index.md
+-rw-r--r--   0 liubo      (501) staff       (20)       66 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc8/docs/license.md
+-rw-r--r--   0 liubo      (501) staff       (20)       70 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc8/docs/readme.md
+-rw-r--r--   0 liubo      (501) staff       (20)      254 2024-04-29 06:45:11.000000 ngstoolkits-1.0.0rc8/docs/requirements.txt
+-rw-r--r--   0 liubo      (501) staff       (20)      353 2024-05-06 09:35:30.000000 ngstoolkits-1.0.0rc8/pyproject.toml
+-rw-r--r--   0 liubo      (501) staff       (20)     1428 2024-05-11 07:07:00.327204 ngstoolkits-1.0.0rc8/setup.cfg
+-rw-r--r--   0 liubo      (501) staff       (20)      982 2024-05-11 07:06:48.000000 ngstoolkits-1.0.0rc8/setup.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-05-11 07:07:00.268961 ngstoolkits-1.0.0rc8/src/
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-05-11 07:07:00.300431 ngstoolkits-1.0.0rc8/src/ngstoolkits/
+-rw-r--r--   0 liubo      (501) staff       (20)      477 2024-05-11 07:06:49.000000 ngstoolkits-1.0.0rc8/src/ngstoolkits/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)    14156 2024-05-11 07:05:29.000000 ngstoolkits-1.0.0rc8/src/ngstoolkits/ngs_class.py
+-rw-r--r--   0 liubo      (501) staff       (20)      883 2024-05-07 03:49:47.000000 ngstoolkits-1.0.0rc8/src/ngstoolkits/sequence.py
+-rw-r--r--   0 liubo      (501) staff       (20)      107 2024-05-11 07:05:29.000000 ngstoolkits-1.0.0rc8/src/ngstoolkits/units.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-05-11 07:07:00.319813 ngstoolkits-1.0.0rc8/src/ngstoolkits.egg-info/
+-rw-r--r--   0 liubo      (501) staff       (20)     2965 2024-05-11 07:07:00.000000 ngstoolkits-1.0.0rc8/src/ngstoolkits.egg-info/PKG-INFO
+-rw-r--r--   0 liubo      (501) staff       (20)      696 2024-05-11 07:07:00.000000 ngstoolkits-1.0.0rc8/src/ngstoolkits.egg-info/SOURCES.txt
+-rw-r--r--   0 liubo      (501) staff       (20)        1 2024-05-11 07:07:00.000000 ngstoolkits-1.0.0rc8/src/ngstoolkits.egg-info/dependency_links.txt
+-rw-r--r--   0 liubo      (501) staff       (20)        1 2024-04-29 06:53:14.000000 ngstoolkits-1.0.0rc8/src/ngstoolkits.egg-info/not-zip-safe
+-rw-r--r--   0 liubo      (501) staff       (20)       92 2024-05-11 07:07:00.000000 ngstoolkits-1.0.0rc8/src/ngstoolkits.egg-info/requires.txt
+-rw-r--r--   0 liubo      (501) staff       (20)       12 2024-05-11 07:07:00.000000 ngstoolkits-1.0.0rc8/src/ngstoolkits.egg-info/top_level.txt
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-05-11 07:07:00.318053 ngstoolkits-1.0.0rc8/tests/
+-rw-r--r--   0 liubo      (501) staff       (20)      279 2024-05-07 03:50:43.000000 ngstoolkits-1.0.0rc8/tests/conftest.py
+-rw-r--r--   0 liubo      (501) staff       (20)      931 2024-05-07 08:00:29.000000 ngstoolkits-1.0.0rc8/tests/test_class.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2861 2024-04-29 06:44:15.000000 ngstoolkits-1.0.0rc8/tox.ini
```

### Comparing `ngstoolkits-1.0.0rc7/.coveragerc` & `ngstoolkits-1.0.0rc8/.coveragerc`

 * *Files identical despite different names*

### Comparing `ngstoolkits-1.0.0rc7/.gitignore` & `ngstoolkits-1.0.0rc8/.gitignore`

 * *Files identical despite different names*

### Comparing `ngstoolkits-1.0.0rc7/.readthedocs.yml` & `ngstoolkits-1.0.0rc8/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `ngstoolkits-1.0.0rc7/CONTRIBUTING.md` & `ngstoolkits-1.0.0rc8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ngstoolkits-1.0.0rc7/LICENSE.txt` & `ngstoolkits-1.0.0rc8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ngstoolkits-1.0.0rc7/PKG-INFO` & `ngstoolkits-1.0.0rc8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: ngstoolkits
-Version: 1.0.0rc7
+Version: 1.0.0rc8
 Summary: ngstools
 Home-page: https://github.com/Ben-unbelieveable/package_ngstoolkits/
 Author: Liubo
 Author-email: 614347533@qq.com
 License: MIT
 Project-URL: pypi, https://pypi.org/project/ngstoolkits/
 Project-URL: Changelog, https://github.com/Ben-unbelieveable/package_ngstoolkits/blob/master/CHANGELOG.md
 Project-URL: Tracker, https://github.com/Ben-unbelieveable/package_ngstoolkits/issues
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE.txt
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: pysam
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
```

### Comparing `ngstoolkits-1.0.0rc7/README.md` & `ngstoolkits-1.0.0rc8/README.md`

 * *Files identical despite different names*

### Comparing `ngstoolkits-1.0.0rc7/docs/Makefile` & `ngstoolkits-1.0.0rc8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ngstoolkits-1.0.0rc7/docs/conf.py` & `ngstoolkits-1.0.0rc8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ngstoolkits-1.0.0rc7/docs/index.md` & `ngstoolkits-1.0.0rc8/docs/index.md`

 * *Files identical despite different names*

### Comparing `ngstoolkits-1.0.0rc7/setup.cfg` & `ngstoolkits-1.0.0rc8/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 [metadata]
 name = ngstoolkits
-versison = 1.0.0rc7
 description = some toolkits for NGS analysis
 author = Ben-unbelieveable
 author_email = 614347533@qq.com
 license = MIT
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
@@ -20,14 +19,15 @@
 
 [options]
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
+python_requires = >=3.8
 install_requires = 
 	importlib-metadata; python_version<"3.8"
 	pysam
 
 [options.packages.find]
 where = src
 exclude =
```

### Comparing `ngstoolkits-1.0.0rc7/setup.py` & `ngstoolkits-1.0.0rc8/setup.py`

 * *Files identical despite different names*

### Comparing `ngstoolkits-1.0.0rc7/src/ngstoolkits/ngs_class.py` & `ngstoolkits-1.0.0rc8/src/ngstoolkits/ngs_class.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,16 @@
         if not self._is_valid_nucleotide_sequence(REF):
             warnings.warn(f"Invalid REF sequence '{REF}'; using empty string instead.")
             self.ref = ""
 
         if not self._is_valid_nucleotide_sequence(ALT):
             warnings.warn(f"Invalid ALT sequence '{ALT}'; using empty string instead.")
             self.alt = ""
-
+        if hasattr(self,'bam'):
+            self.get_suppot()
 
     @staticmethod
     def _is_valid_nucleotide_sequence(sequence: str) -> bool:
         valid_nucleotides = set('ATCGatcg')
         return all(nucleotide in valid_nucleotides for nucleotide in sequence)
 
     def _is_valid_ref_sequence(self)->int:
@@ -73,20 +74,17 @@
 
     @property
     def info(self):
         """
         return the information of the mutation
         """
         if hasattr(self,'support_readsID_list'):
-            supportNum=len(self.support_readsID_list)
-            coverDepth=len(self.cover_readsID_list)
-            ratio=supportNum/coverDepth
-            return f"{self.chrom}:{self.pos}\t{self.ref}\t{self.alt}\t{self.muttype()}\t{supportNum}\t{coverDepth}\t{ratio}"
+            return f"{self.chrom}\t{self.pos}\t{self.ref}\t{self.alt}\t{self.muttype}\t{self.supportReadNum}\t{self.CoverReadNum}\t{self.ratio}"
         else:
-            return f"{self.chrom}:{self.pos}:{self.ref}:{self.alt}"
+            return f"{self.chrom}\t{self.pos}\t{self.ref}\t{self.alt}\t*\t*\t*\t*"
 
     @property
     def muttype(self):
         if len(self.ref)>len(self.alt):
             return "DEL"
         elif len(self.ref)<len(self.alt):
             return "INS"
@@ -98,14 +96,55 @@
         '''获取变异的侧翼10bp序列
         使用前需要通过loadReference(reference) 完成参考基因组的加载
         param length: 侧翼序列长度
         '''
         lbase = self.reference.fetch(self.chrom, self.pos-length,self.pos)
         rbase = self.reference.fetch(self.chrom, self.pos+len(self.ref), self.pos+len(self.ref)+length)
         return '..'.join((lbase, rbase))
+    
+    @property
+    def CoverReadList(self):
+        if hasattr(self,'cover_readsID_list'):
+            return self.cover_readsID_list
+        else :
+            self.get_suppot()
+            return self.cover_readsID_list
+    @property
+    def CoverReadNum(self):
+        if hasattr(self,'cover_readsID_list'):
+            return len(self.cover_readsID_list)
+        else :
+            self.get_suppot()
+            return len(self.cover_readsID_list)
+
+    @property
+    def supportReads(self):
+        if hasattr(self,'support_reads'):
+            return self.support_reads
+        else :
+            self.get_suppot()
+            return self.support_reads
+
+    @property
+    def support_readsID_list(self):
+        if hasattr(self,'support_readsID_list'):
+            return self.support_readsID_list
+        else :
+            self.get_suppot()
+            return self.support_readsID_list
+
+    @property
+    def supportReadNum(self):
+        if hasattr(self,'support_readsID_list'):
+            return len(self.support_readsID_list)
+        else :
+            self.get_suppot()
+            return len(self.support_readsID_list)
+    def ratio(self):
+        return self.supportReadNum/self.CoverReadNum
 
     def flank(self, length:int):
         '''获取变异的任意长度侧翼序列
         使用前需要通过loadReference(reference) 完成参考基因组的加载
         param length: 侧翼序列长度
         '''
         lbase = self.reference.fetch(self.chrom, self.pos-length,self.pos)
@@ -129,22 +168,23 @@
             else:
                 raise ValueError("reference genome is not set, set it with cpra.loadReference(referencePath)")
         self.pos_fit = self.pos+ self._is_valid_ref_sequence()
         self.support_reads = []
         self.support_readsID_list = []
         self.cover_readsID_list = []
         if self.muttype == "SNV":
-            self.support_reads,self.support_readsID_list,self.cover_readsID_list = self.get_snv_support_reads(coverflank)
+            self.support_reads,self.support_readsID_list,self.cover_readsID_list = self._get_snv_support_reads(coverflank)
         elif self.muttype == "INS":
-            self.support_reads,self.support_readsID_list,self.cover_readsID_list = self.get_ins_support_reads(coverflank)
+            self.support_reads,self.support_readsID_list,self.cover_readsID_list = self._get_ins_support_reads(coverflank)
         elif self.muttype == "DEL":
-            self.support_reads,self.support_readsID_list,self.cover_readsID_list = self.get_del_support_reads(coverflank)
-
+            self.support_reads,self.support_readsID_list,self.cover_readsID_list = self._get_del_support_reads(coverflank)
+        self.support_depth = len(self.support_readsID_list)
+        self.cover_depth= len(self.cover_readsID_list)
     @lru_cache
-    def get_snv_support_reads(self, coverflank=5, mapq=20, baseq=20, overlaps=True, stepper="all", orphans=True):
+    def _get_snv_support_reads(self, coverflank=5, mapq=20, baseq=20, overlaps=True, stepper="all", orphans=True):
         Read = namedtuple('Read', ['read_name', 'pair', 'strand'])
         support_reads = []
         cover_reads = []
         start_reads = {}
         EndSite = self.pos_fit + len(self.ref)
         for pileup_column in self.bam.pileup(region=str(self.chrom) + ':' + str(self.pos_fit) + '-' + str(self.pos_fit),mapq=mapq , baseq = baseq,
                                             stepper=stepper, fastaFile=self.reference, max_depth=200000, **{"truncate": True}):
@@ -181,15 +221,15 @@
         for aln in cover_reads:
             cover_readID_list.append(aln.query_name)
         for aln in support_reads:
             support_readIDs.append(aln.query_name)
         return [support_reads,support_readIDs,cover_readID_list]
 
     @lru_cache
-    def get_ins_support_reads(self, coverflank=5, mapq=20, baseq=20, overlaps=True, stepper="all", orphans=True):
+    def _get_ins_support_reads(self, coverflank=5, mapq=20, baseq=20, overlaps=True, stepper="all", orphans=True):
         support_reads = []
         cover_reads = []
         bam = {}
         EndSite = self.pos_fit + len(self.ref)
         CoverStart = self.pos_fit-coverflank
         CoverEnd = EndSite + coverflank
         insLength=len(self.alt)-len(self.ref)
@@ -218,15 +258,15 @@
         for aln in cover_reads:
             cover_readID_list.append(aln.query_name)
         for aln in support_reads:
             support_readID_list.append(aln.query_name)
         return [support_reads,support_readID_list,cover_readID_list]
 
     @lru_cache
-    def get_del_support_reads(self, coverflank=5, mapq=20, baseq=20, overlaps=True, stepper="all", orphans=True):
+    def _get_del_support_reads(self, coverflank=5, mapq=20, baseq=20, overlaps=True, stepper="all", orphans=True):
         support_reads = []
         cover_reads = []
         bam = {}
         EndSite = self.pos_fit + len(self.ref)
         CoverStart = self.pos_fit-coverflank
         CoverEnd = EndSite + coverflank
         for pileup_column in self.bam.pileup(region=str(self.chrom) + ':' + str(self.pos_fit) + '-' + str(EndSite), mapq=mapq , baseq = baseq,
```

### Comparing `ngstoolkits-1.0.0rc7/src/ngstoolkits/sequence.py` & `ngstoolkits-1.0.0rc8/src/ngstoolkits/sequence.py`

 * *Files identical despite different names*

### Comparing `ngstoolkits-1.0.0rc7/src/ngstoolkits.egg-info/PKG-INFO` & `ngstoolkits-1.0.0rc8/src/ngstoolkits.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: ngstoolkits
-Version: 1.0.0rc7
+Version: 1.0.0rc8
 Summary: ngstools
 Home-page: https://github.com/Ben-unbelieveable/package_ngstoolkits/
 Author: Liubo
 Author-email: 614347533@qq.com
 License: MIT
 Project-URL: pypi, https://pypi.org/project/ngstoolkits/
 Project-URL: Changelog, https://github.com/Ben-unbelieveable/package_ngstoolkits/blob/master/CHANGELOG.md
 Project-URL: Tracker, https://github.com/Ben-unbelieveable/package_ngstoolkits/issues
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE.txt
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: pysam
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
```

### Comparing `ngstoolkits-1.0.0rc7/src/ngstoolkits.egg-info/SOURCES.txt` & `ngstoolkits-1.0.0rc8/src/ngstoolkits.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 docs/license.md
 docs/readme.md
 docs/requirements.txt
 docs/_static/.gitignore
 src/ngstoolkits/__init__.py
 src/ngstoolkits/ngs_class.py
 src/ngstoolkits/sequence.py
+src/ngstoolkits/units.py
 src/ngstoolkits.egg-info/PKG-INFO
 src/ngstoolkits.egg-info/SOURCES.txt
 src/ngstoolkits.egg-info/dependency_links.txt
 src/ngstoolkits.egg-info/not-zip-safe
 src/ngstoolkits.egg-info/requires.txt
 src/ngstoolkits.egg-info/top_level.txt
 tests/conftest.py
```

### Comparing `ngstoolkits-1.0.0rc7/tests/test_class.py` & `ngstoolkits-1.0.0rc8/tests/test_class.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
     - https://docs.pytest.org/en/stable/fixture.html
     - https://docs.pytest.org/en/stable/writing_plugins.html
 """
 
 # import pytest
 import sys
 sys.path.append('../src')
-from ngstoolkits import CPRA
 import pytest
 from ngstoolkits import Seq
+from ngstoolkits import CPRA
 CPRA.loadBam("test_data/pancancer689__DX2083_sijuan_20S12590085_20B12590085__Cancer.realign.bam")
 CPRA.loadReference("test_data/hg19.fa")
 
 
 def test_single_mutation():
     sitea=CPRA("chr6",159188398,"C","T")
     siteb=CPRA("chr1",65332550,"","T")
```

### Comparing `ngstoolkits-1.0.0rc7/tox.ini` & `ngstoolkits-1.0.0rc8/tox.ini`

 * *Files identical despite different names*

