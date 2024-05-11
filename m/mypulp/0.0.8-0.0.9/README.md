# Comparing `tmp/mypulp-0.0.8.zip` & `tmp/mypulp-0.0.9.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 7879 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat    14082 b- defN 16-Feb-03 09:22 mypulp-0.0.8/mypulp.py
--rw-rw-rw-  2.0 fat     1980 b- defN 16-Feb-03 09:23 mypulp-0.0.8/PKG-INFO
--rw-rw-rw-  2.0 fat       64 b- defN 16-Feb-03 09:23 mypulp-0.0.8/setup.cfg
--rw-rw-rw-  2.0 fat     1895 b- defN 16-Feb-03 09:23 mypulp-0.0.8/setup.py
--rw-rw-rw-  2.0 fat        1 b- defN 16-Feb-03 09:23 mypulp-0.0.8/mypulp.egg-info/dependency_links.txt
--rw-rw-rw-  2.0 fat     1980 b- defN 16-Feb-03 09:23 mypulp-0.0.8/mypulp.egg-info/PKG-INFO
--rw-rw-rw-  2.0 fat        5 b- defN 16-Feb-03 09:23 mypulp-0.0.8/mypulp.egg-info/requires.txt
--rw-rw-rw-  2.0 fat      167 b- defN 16-Feb-03 09:23 mypulp-0.0.8/mypulp.egg-info/SOURCES.txt
--rw-rw-rw-  2.0 fat        7 b- defN 16-Feb-03 09:23 mypulp-0.0.8/mypulp.egg-info/top_level.txt
-9 files, 20181 bytes uncompressed, 6583 bytes compressed:  67.4%
+Zip file size: 8259 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat    14082 b- defN 16-Feb-03 09:22 mypulp-0.0.9/mypulp.py
+-rw-rw-rw-  2.0 fat     2176 b- defN 16-Aug-08 08:11 mypulp-0.0.9/PKG-INFO
+-rw-rw-rw-  2.0 fat       64 b- defN 16-Aug-08 08:11 mypulp-0.0.9/setup.cfg
+-rw-rw-rw-  2.0 fat     2083 b- defN 16-Aug-08 08:11 mypulp-0.0.9/setup.py
+-rw-rw-rw-  2.0 fat        1 b- defN 16-Aug-08 08:11 mypulp-0.0.9/mypulp.egg-info/dependency_links.txt
+-rw-rw-rw-  2.0 fat     2176 b- defN 16-Aug-08 08:11 mypulp-0.0.9/mypulp.egg-info/PKG-INFO
+-rw-rw-rw-  2.0 fat        5 b- defN 16-Aug-08 08:11 mypulp-0.0.9/mypulp.egg-info/requires.txt
+-rw-rw-rw-  2.0 fat      167 b- defN 16-Aug-08 08:11 mypulp-0.0.9/mypulp.egg-info/SOURCES.txt
+-rw-rw-rw-  2.0 fat        7 b- defN 16-Aug-08 08:11 mypulp-0.0.9/mypulp.egg-info/top_level.txt
+9 files, 20761 bytes uncompressed, 6963 bytes compressed:  66.5%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
-Filename: mypulp-0.0.8/mypulp.py
+Filename: mypulp-0.0.9/mypulp.py
 Comment: 
 
-Filename: mypulp-0.0.8/PKG-INFO
+Filename: mypulp-0.0.9/PKG-INFO
 Comment: 
 
-Filename: mypulp-0.0.8/setup.cfg
+Filename: mypulp-0.0.9/setup.cfg
 Comment: 
 
-Filename: mypulp-0.0.8/setup.py
+Filename: mypulp-0.0.9/setup.py
 Comment: 
 
-Filename: mypulp-0.0.8/mypulp.egg-info/dependency_links.txt
+Filename: mypulp-0.0.9/mypulp.egg-info/dependency_links.txt
 Comment: 
 
-Filename: mypulp-0.0.8/mypulp.egg-info/PKG-INFO
+Filename: mypulp-0.0.9/mypulp.egg-info/PKG-INFO
 Comment: 
 
-Filename: mypulp-0.0.8/mypulp.egg-info/requires.txt
+Filename: mypulp-0.0.9/mypulp.egg-info/requires.txt
 Comment: 
 
-Filename: mypulp-0.0.8/mypulp.egg-info/SOURCES.txt
+Filename: mypulp-0.0.9/mypulp.egg-info/SOURCES.txt
 Comment: 
 
-Filename: mypulp-0.0.8/mypulp.egg-info/top_level.txt
+Filename: mypulp-0.0.9/mypulp.egg-info/top_level.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `mypulp-0.0.8/mypulp.py` & `mypulp-0.0.9/mypulp.py`

 * *Files identical despite different names*

## Comparing `mypulp-0.0.8/PKG-INFO` & `mypulp-0.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 1.1
 Name: mypulp
-Version: 0.0.8
+Version: 0.0.9
 Summary: `mypulp` is a package for mypulp.
 Home-page: https://pypi.python.org/pypi/mypulp
 Author: Mikio Kubo
 Author-email: kubomikio@gmail.com
 License: PSFL
-Description: `mypulp` is a package for mypulp.
+Description: Mypulp is a wrapper module for PuLP. It supports to call PuLP using the same functions and classes as in Gurobi, a commercial mixed integer optimization solver.
+        For more details, see the Gurobi HP http://www.gurobi.com/.
         ::
         
             from mypulp import *
             model = Model("lo1")
             J, v = multidict({1:16, 2:19, 3:23, 4:28})
             x1 = model.addVar(vtype=GRB.CONTINUOUS, name="x1")
             x2 = model.addVar(vtype="C", name="x2")
```

## Comparing `mypulp-0.0.8/setup.py` & `mypulp-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from setuptools import setup
 
-version = '0.0.8'
+version = '0.0.9'
 name = 'mypulp'
 short_description = '`mypulp` is a package for mypulp.'
 long_description = """\
-`mypulp` is a package for mypulp.
+Mypulp is a wrapper module for PuLP. It supports to call PuLP using the same functions and classes as in Gurobi, a commercial mixed integer optimization solver.
+For more details, see the Gurobi HP http://www.gurobi.com/.
 ::
 
     from mypulp import *
     model = Model("lo1")
     J, v = multidict({1:16, 2:19, 3:23, 4:28})
     x1 = model.addVar(vtype=GRB.CONTINUOUS, name="x1")
     x2 = model.addVar(vtype="C", name="x2")
```

## Comparing `mypulp-0.0.8/mypulp.egg-info/PKG-INFO` & `mypulp-0.0.9/mypulp.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 1.1
 Name: mypulp
-Version: 0.0.8
+Version: 0.0.9
 Summary: `mypulp` is a package for mypulp.
 Home-page: https://pypi.python.org/pypi/mypulp
 Author: Mikio Kubo
 Author-email: kubomikio@gmail.com
 License: PSFL
-Description: `mypulp` is a package for mypulp.
+Description: Mypulp is a wrapper module for PuLP. It supports to call PuLP using the same functions and classes as in Gurobi, a commercial mixed integer optimization solver.
+        For more details, see the Gurobi HP http://www.gurobi.com/.
         ::
         
             from mypulp import *
             model = Model("lo1")
             J, v = multidict({1:16, 2:19, 3:23, 4:28})
             x1 = model.addVar(vtype=GRB.CONTINUOUS, name="x1")
             x2 = model.addVar(vtype="C", name="x2")
```

