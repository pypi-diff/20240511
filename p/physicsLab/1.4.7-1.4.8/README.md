# Comparing `tmp/physicslab-1.4.7.tar.gz` & `tmp/physicslab-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "physicslab-1.4.7.tar", last modified: Tue Apr 23 15:07:33 2024, max compression
+gzip compressed data, was "physicslab-1.4.8.tar", last modified: Sat May 11 15:59:14 2024, max compression
```

## Comparing `physicslab-1.4.7.tar` & `physicslab-1.4.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:07:33.507228 physicslab-1.4.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-23 15:07:29.000000 physicslab-1.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-23 15:07:33.507228 physicslab-1.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-04-23 15:07:29.000000 physicslab-1.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:07:33.503228 physicslab-1.4.7/physicsLab/
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/_colorUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:07:33.503228 physicslab-1.4.7/physicsLab/celestial/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/celestial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/celestial/elementsClass.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:07:33.503228 physicslab-1.4.7/physicsLab/circuit/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/circuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/circuit/elementXYZ.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:07:33.503228 physicslab-1.4.7/physicsLab/circuit/elements/
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/circuit/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/circuit/elements/_elementBase.py
--rw-r--r--   0 runner    (1001) docker     (127)    17734 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/circuit/elements/artificialCircuit.py
--rw-r--r--   0 runner    (1001) docker     (127)    18434 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/circuit/elements/basicCircuit.py
--rw-r--r--   0 runner    (1001) docker     (127)    18290 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/circuit/elements/logicCircuit.py
--rw-r--r--   0 runner    (1001) docker     (127)    16354 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/circuit/elements/otherCircuit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/circuit/wire.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:07:33.503228 physicslab-1.4.7/physicsLab/electromagnetism/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/electromagnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/electromagnetism/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/element.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/elementBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    28336 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/experimentType.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:07:33.507228 physicslab-1.4.7/physicsLab/lib/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/lib/_unionClassHead.py
--rw-r--r--   0 runner    (1001) docker     (127)    19381 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/lib/logic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/lib/wires.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:07:33.507228 physicslab-1.4.7/physicsLab/music/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/music/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25439 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/music/music.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/savTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/typehint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:07:33.507228 physicslab-1.4.7/physicsLab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-23 15:07:33.000000 physicslab-1.4.7/physicsLab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-23 15:07:33.000000 physicslab-1.4.7/physicsLab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:07:33.000000 physicslab-1.4.7/physicsLab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-23 15:07:33.000000 physicslab-1.4.7/physicsLab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 15:07:33.000000 physicslab-1.4.7/physicsLab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 15:07:33.507228 physicslab-1.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-23 15:07:29.000000 physicslab-1.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:59:14.561728 physicslab-1.4.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-11 15:59:10.000000 physicslab-1.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-11 15:59:14.561728 physicslab-1.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-05-11 15:59:10.000000 physicslab-1.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:59:14.557728 physicslab-1.4.8/physicsLab/
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/_colorUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:59:14.557728 physicslab-1.4.8/physicsLab/celestial/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/celestial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/celestial/elementsClass.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:59:14.557728 physicslab-1.4.8/physicsLab/circuit/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/circuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/circuit/elementXYZ.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:59:14.561728 physicslab-1.4.8/physicsLab/circuit/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/circuit/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/circuit/elements/_elementBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17734 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/circuit/elements/artificialCircuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18434 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/circuit/elements/basicCircuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18290 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/circuit/elements/logicCircuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16354 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/circuit/elements/otherCircuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/circuit/wire.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:59:14.561728 physicslab-1.4.8/physicsLab/electromagnetism/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/electromagnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/electromagnetism/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/elementBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28498 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/experimentType.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:59:14.561728 physicslab-1.4.8/physicsLab/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/lib/_unionClassHead.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19381 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/lib/logic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/lib/wires.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:59:14.561728 physicslab-1.4.8/physicsLab/music/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/music/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26688 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/music/music.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/savTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-11 15:59:10.000000 physicslab-1.4.8/physicsLab/typehint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:59:14.561728 physicslab-1.4.8/physicsLab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-11 15:59:14.000000 physicslab-1.4.8/physicsLab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-11 15:59:14.000000 physicslab-1.4.8/physicsLab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 15:59:14.000000 physicslab-1.4.8/physicsLab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-11 15:59:14.000000 physicslab-1.4.8/physicsLab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-11 15:59:14.000000 physicslab-1.4.8/physicsLab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 15:59:14.561728 physicslab-1.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-11 15:59:10.000000 physicslab-1.4.8/setup.py
```

### Comparing `physicslab-1.4.7/LICENSE` & `physicslab-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.7/PKG-INFO` & `physicslab-1.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physicsLab
-Version: 1.4.7
+Version: 1.4.8
 Summary: Python API for Physics-Lab-AR
 Home-page: https://gitee.com/script2000/physicsLab
 Author: Goodenough
 Author-email: 2381642961@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `physicslab-1.4.7/README.md` & `physicslab-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.7/physicsLab/__init__.py` & `physicslab-1.4.8/physicsLab/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 # Win: 若存档对应文件夹不存在直接报错
 import os
 import platform
 if platform.system() == "Windows":
     if not os.path.exists(Experiment.FILE_HEAD):
         raise RuntimeError("The folder does not exist, try launching Physics-Lab-AR and try it out")
 else:
-    if not os.path.exists("physicsLabSav"):
-        os.mkdir("physicsLabSav")
+    if not os.path.exists(Experiment.FILE_HEAD):
+        os.mkdir(Experiment.FILE_HEAD)
 
 # 获取 Physics-Lab-AR 版本
 def get_Physics_Lab_AR_version() -> Optional[str]:
     if platform.system() == "Windows":
         from getpass import getuser
         version_file = f"C:/Users/{getuser()}/AppData/LocalLow/CIVITAS/Quantum Physics/Unity/" \
                        f"30fdf88e-c67c-4ae8-a0f5-83bb57b9a5c3/Analytics/values"
```

### Comparing `physicslab-1.4.7/physicsLab/_colorUtils.py` & `physicslab-1.4.8/physicsLab/_colorUtils.py`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.7/physicsLab/_tools.py` & `physicslab-1.4.8/physicsLab/_tools.py`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.7/physicsLab/circuit/elementXYZ.py` & `physicslab-1.4.8/physicsLab/circuit/elementXYZ.py`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.7/physicsLab/circuit/elements/_elementBase.py` & `physicslab-1.4.8/physicsLab/circuit/elements/_elementBase.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,16 +91,14 @@
 
         self._position = _tools.position(x, y, z)
 
         #元件坐标系
         if elementXYZ is True or _elementXYZ.is_elementXYZ() is True and elementXYZ is None:
             x, y, z = _elementXYZ.xyzTranslate(x, y, z, self.is_bigElement)
             self.is_elementXYZ = True
-            # if self.is_bigElement:
-            #     x, y, z = _elementXYZ.amend_big_Element(x, y, z)
 
         for _, self_list in stack_Experiment.top().elements_Position.items():
             if self in self_list:
                 self_list.remove(self)
 
         self._arguments['Position'] = f"{x},{z},{y}" # type: ignore -> define _arguments in metaclass
```

### Comparing `physicslab-1.4.7/physicsLab/circuit/elements/artificialCircuit.py` & `physicslab-1.4.8/physicsLab/circuit/elements/artificialCircuit.py`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.7/physicsLab/circuit/elements/basicCircuit.py` & `physicslab-1.4.8/physicsLab/circuit/elements/basicCircuit.py`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.7/physicsLab/circuit/elements/logicCircuit.py` & `physicslab-1.4.8/physicsLab/circuit/elements/logicCircuit.py`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.7/physicsLab/circuit/elements/otherCircuit.py` & `physicslab-1.4.8/physicsLab/circuit/elements/otherCircuit.py`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.7/physicsLab/circuit/wire.py` & `physicslab-1.4.8/physicsLab/circuit/wire.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from physicsLab import errors
 from physicsLab.experiment import get_Experiment
 from physicsLab.experimentType import experimentType
-from physicsLab.typehint import WireDict, Optional
+from physicsLab.typehint import WireDict, Optional, Callable
 
 # 电学元件引脚类, 模电元件引脚无明确的输入输出之分, 因此用这个
 class Pin:
     __slots__ = ("element_self", "pinLabel")
     is_input = False
     is_output = False
     def __init__(self, input_self, pinLabel: int) -> None:
@@ -52,17 +52,20 @@
 # 导线类
 class Wire:
     __slots__ = ("Source", "Target", "color")
     def __init__(self, Source: Pin, Target: Pin, color: str = '蓝') -> None:
         if not isinstance(Source, Pin) or not isinstance(Target, Pin):
             raise TypeError
 
-        if Source.element_self.experiment != Target.element_self.experiment:
+        if Source.element_self.experiment is not Target.element_self.experiment:
             raise errors.ExperimentError("can't link wire in two experiment")
 
+        if Source == Target:
+            raise errors.ExperimentError()
+
         if color in ("black", "blue", "red", "green", "yellow"):
             color = {"black": "黑", "blue": "蓝", "red": "红", "green": "绿", "yellow": "黄"}[color]
         if color not in ('蓝', '绿', '黄', '红', '紫'):
             raise errors.WireColorError
 
         self.Source: Pin = Source
         self.Target: Pin = Target
@@ -97,15 +100,15 @@
             "SourcePin": self.Source.pinLabel,
             "Target": self.Target.element_self._arguments["Identifier"],
             "TargetPin": self.Target.pinLabel,
             "ColorName": f"{self.color}色导线"
         }
 
 # 检查函数参数是否是导线
-def _check_typeWire(func: callable):
+def _check_typeWire(func: Callable):
     def result(SourcePin: Pin, TargetPin: Pin, *args, **kwargs) -> None:
         if not (
                 isinstance(SourcePin, Pin) and
                 isinstance(TargetPin, Pin)
         ):
             raise TypeError
```

### Comparing `physicslab-1.4.7/physicsLab/electromagnetism/elements.py` & `physicslab-1.4.8/physicsLab/electromagnetism/elements.py`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.7/physicsLab/element.py` & `physicslab-1.4.8/physicsLab/element.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from physicsLab import errors
 from physicsLab.circuit import elements
 
 from physicsLab.experiment import stack_Experiment
 from physicsLab.typehint import numType, Optional, Union, List
 from physicsLab.circuit.elements._elementBase import CircuitBase
 
-NnumType = Optional[numType]
-
 def crt_Element(name: str,
                 x: numType = 0,
                 y: numType = 0,
                 z: numType = 0,
                 elementXYZ: Optional[bool] = None,
                 *args,
                 **kwargs
@@ -35,19 +33,19 @@
         return elements.eight_bit_Input(x, y, z, elementXYZ)
     elif (name == '8bit Display'):
         return elements.eight_bit_Display(x, y, z, elementXYZ)
     else:
         return eval(f"elements.{name.replace(' ', '_').replace('-', '_')}"
                     f"({x}, {y}, {z}, {elementXYZ}, *{args}, **{kwargs})")
 
-def get_Element(x: NnumType=None,
-                y: NnumType=None,
-                z: NnumType=None,
+def get_Element(x: Optional[numType] = None,
+                y: Optional[numType] = None,
+                z: Optional[numType] = None,
                 *,
-                index: NnumType=None,
+                index: Optional[numType] = None,
                 **kwargs
 ) -> Union[CircuitBase, List[CircuitBase]]:
     ''' 获取对应坐标的id '''
     # 通过坐标索引元件
     def position_get(x: numType, y: numType, z: numType):
         if not (
             isinstance(x, (int, float))
```

### Comparing `physicslab-1.4.7/physicsLab/errors.py` & `physicslab-1.4.8/physicsLab/errors.py`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.7/physicsLab/experiment.py` & `physicslab-1.4.8/physicsLab/experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,18 +41,23 @@
 
 def get_Experiment() -> "Experiment":
     ''' 获取当前正在操作的存档 '''
     return stack_Experiment.top()
 
 class Experiment:
     ''' 实验（存档）类 '''
-    FILE_HEAD = "physicsLabSav"
     if platform.system() == "Windows":
         from getpass import getuser
         FILE_HEAD = f"C:/Users/{getuser()}/AppData/LocalLow/CIVITAS/Quantum Physics/Circuit"
+    else:
+        _home = os.environ.get('PHYSICSLAB_HOME_PATH')
+        if _home is None:
+            FILE_HEAD = "physicsLabSav"
+        else:
+            FILE_HEAD = f"{_home}/physicsLabSav"
 
     def __init__(self, sav_name: Optional[str] = None) -> None:
         self.is_open_or_crt: bool = False
         self.is_open: bool = False
         self.is_crt: bool = False
         self.is_read: bool = False
```

### Comparing `physicslab-1.4.7/physicsLab/lib/_unionClassHead.py` & `physicslab-1.4.8/physicsLab/lib/_unionClassHead.py`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.7/physicsLab/lib/logic.py` & `physicslab-1.4.8/physicsLab/lib/logic.py`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.7/physicsLab/lib/wires.py` & `physicslab-1.4.8/physicsLab/lib/wires.py`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.7/physicsLab/music/music.py` & `physicslab-1.4.8/physicsLab/music/music.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from physicsLab.circuit import elements
 from physicsLab._tools import roundData
 from physicsLab.lib import crt_Wires, D_WaterLamp
 from physicsLab.typehint import Optional, Union, List, Iterator, Dict, Self, numType
 
 def _format_velocity(velocity: float) -> float:
     velocity = min(1, velocity)
-    velocity = max(0.05, velocity)
 
     return velocity
 
 # midi类，用于提供physicsLab与midi文件之间的桥梁
 ''' 重要midi事件及作用:
     note_on        -> message: 播放音符
     note_off       -> message: 停止播放音符
@@ -184,66 +183,76 @@
 
         for msg in self.messages:
             msg.time *= num
 
         return self
 
     # 返回 [Note(...), Chord(...), ...]
-    def _get_notes_list(self, div_time: numType, max_notes: Optional[int]) -> List[Union["Note", "Chord"]]:
-        res: List[Union[Note, Chord]] = []
+    def _get_notes_list(self,
+                        div_time: numType, max_notes: Optional[int],
+                        is_fix_strange_note: bool = False,
+                        ) -> List[Union["Note", "Chord"]]:
 
+        res: List[Union[Note, Chord]] = []
         wait_time: int = 0
         len_res: int = 0
+
         for msg in self.messages:
-            if msg.type == "note_on": # type: ignore -> Message/MetaMessage must have attr type
+            if msg.type == "note_on":
+                velocity: float = _format_velocity(msg.velocity / 127) # 音符的响度
+                ins: int = self.channels[msg.channel]
+
+                if velocity == 0 or (is_fix_strange_note and ins == 0 and velocity >= 0.85):
+                    if msg.time != 0:
+                        wait_time += msg.time
+                    continue
+
                 len_res += 1
                 note_time = round((msg.time + wait_time) / div_time)
 
-                velocity = _format_velocity(msg.velocity / 127) # 音符的响度
-
                 if note_time != 0 or len(res) == 0:
                     if note_time == 0:
                         note_time = 1
-                    res.append(
-                        Note(note_time,
-                             instrument=self.channels[msg.channel],
-                             pitch=msg.note, velocity=velocity)
-                    )
+                    res.append(Note(time=note_time, instrument=ins, pitch=msg.note, velocity=velocity))
                 else:
                     # res[-1]是`Note`或`Chord`且在赋值之后一定是Chord, 此时Note的time的值不重要(因为和弦的音符是同时播放的)
-                    res[-1] = res[-1].append(
-                        Note(time=1, instrument=self.channels[msg.channel], pitch=msg.note, velocity=velocity)
-                    )
+                    res[-1] = res[-1].append(Note(time=1, instrument=ins, pitch=msg.note, velocity=velocity))
                 wait_time = 0
             elif msg.time != 0:
                 wait_time += msg.time
 
             if max_notes is not None and len_res >= max_notes:
                 break
 
         return res
 
-    # 转换为physicsLab的piece类
-    def to_piece(self, div_time: numType = 100, max_notes: Optional[int] = 800) -> "Piece":
-        return Piece(self._get_notes_list(div_time, max_notes))
+    def to_piece(self,
+                 div_time: numType = 100,
+                 max_notes: Optional[int] = 800,
+                 is_optimize: bool = True, # 是否将多个音符优化为和弦
+                 is_fix_strange_note: bool = False, # 是否修正一些奇怪的音符
+                 ) -> "Piece":
+        ''' 转换为Piece类 '''
+        return Piece(self._get_notes_list(div_time, max_notes, is_fix_strange_note),
+                     is_optimize=is_optimize)
 
     ''' *.pl.py文件:
         pl即为 physicsLab file
         为了更方便于手动调控物实音乐电路的生成而诞生的文件格式
         该文件运行之后即可生成对应的物实播放音乐电路
     '''
     '''
         *.mido.py
         为了更方便的研究Midi而诞生的文件格式
         为了修改方便, 默认使用 str(mido.MidiTrack) 的方式导出
         而且是个Py文件, 大家想要自己修改也是很方便的
     '''
 
-    # 导出一个 .mido.py 文件
     def write_midopy(self, path: str="temp.mido.py") -> Self:
+        ''' 导出一个 .mido.py 文件 '''
         if not path.endswith(".mido.py"):
             path += ".mido.py"
 
         with open(path, "w", encoding="utf-8") as f:
             f.write(f"import os\n"
                     f"os.environ['PYGAME_HIDE_SUPPORT_PROMPT'] = '1'\n"
                     f"from mido import MidiFile, MidiTrack, MetaMessage, Message\n"
@@ -293,17 +302,17 @@
             f.write(f"from physicsLab import experiment\n"
                     f"from physicsLab.music import Note, Piece, Chord\n"
                     f"with experiment(\"{sav_name}\"):\n"
                     f"    Piece([\n{notes_str}    ]).release(-1, -1, 0)")
 
         return self
 
-# 音符类
 # TODO 增加更多的设置pitch的方法 -> 参考Simple_Instrument
 class Note:
+    ''' 音符类 '''
     def __init__(self,
                  time: int, # 间隔多少时间才播放此Note
                  playTime: int = 1,  # 音符发出声音的时长 暂时不支持相关机制
                  instrument: int = 0, # 演奏的乐器，暂时只支持传入数字
                  pitch: int = 60, # 音高/音调
                  velocity: Union[int, float] = 0.64 # 音量/响度
     ) -> None:
@@ -326,16 +335,16 @@
     def __repr__(self) -> str:
         return f"Note(time={self.time}, playTime={self.playTime}, instrument={self.instrument}, " \
                f"pitch={self.pitch}, velocity={self.velocity})"
 
     def append(self, other: "Note") -> "Chord":
         return Chord(self, other, time=self.time)
 
-# 和弦类
 class Chord:
+    ''' 和弦类 '''
     def __init__(self, *notes: Note, time: int) -> None:
         if len(notes) < 1 or time < 1:
             raise TypeError
 
         self.time = time
         self._notes = []
         # {instrument: List[Note], ...}
@@ -380,38 +389,58 @@
         return self
 
     # 将Chord存储的数据转变为对应的物实的电路
     def release(self,
                 x: numType = 0,
                 y: numType = 0,
                 z: numType = 0,
-                elementXYZ: Optional[bool] = None
-    ) -> elements.Simple_Instrument:
+                elementXYZ: Optional[bool] = None,
+                is_optimize: bool = True,
+                ) -> elements.Simple_Instrument:
         # 元件坐标系，如果输入坐标不是元件坐标系就强转为元件坐标系
         if not (elementXYZ is True or (_elementXYZ.is_elementXYZ() is True and elementXYZ is None)):
             x, y, z = _elementXYZ.translateXYZ(x, y, z)
         x, y, z = roundData(x, y, z) # type: ignore -> result type: tuple
 
-        first_ins = None # 第一个音符
-        for delta_z, ins in enumerate(self.ins_notes):
-            notes: List[Note] = self.ins_notes[ins]
-            temp: elements.Simple_Instrument = elements.Simple_Instrument(
-                x, y, z + delta_z, elementXYZ=True,instrument=ins,
-                pitch=notes[0].pitch, is_ideal_model=True, velocity=self._get_velocity(notes, is_average=True)
-            ).set_Rotation(0, 0, 0)
-            if first_ins is None:
-                first_ins = temp
-            else:
-                temp.i - first_ins.i
-                temp.o - first_ins.o
+        first_ins: Optional[elements.Simple_Instrument] = None # 第一个音符
+        if is_optimize:
+            for delta_z, ins in enumerate(self.ins_notes):
+                notes: List[Note] = self.ins_notes[ins]
+                temp: elements.Simple_Instrument = elements.Simple_Instrument(
+                    x, y, z + delta_z, elementXYZ=True,instrument=ins,
+                    pitch=notes[0].pitch, is_ideal_model=True, velocity=self._get_velocity(notes, is_average=True)
+                ).set_Rotation(0, 0, 0)
 
-            for a_note in notes:
-                temp.add_note(a_note.pitch) # type: ignore
+                if first_ins is None:
+                    first_ins = temp
+                else:
+                    temp.i - first_ins.i
+                    temp.o - first_ins.o
+
+                for a_note in notes:
+                    temp.add_note(a_note.pitch)
+        else:
+            delta_z = 0
+            for ins, notes in self.ins_notes.items():
+                for a_note in notes:
+                    temp = elements.Simple_Instrument(
+                        x, y, z + delta_z, elementXYZ=True,instrument=ins,
+                        pitch=a_note.pitch, is_ideal_model=True, velocity=a_note.velocity
+                    ).set_Rotation(0, 0, 0)
+
+                    if first_ins is None:
+                        first_ins = temp
+                    else:
+                        temp.i - first_ins.i
+                        temp.o - first_ins.o
 
-        return first_ins # type: ignore -> first_ins 不会是None
+                    delta_z += 1
+
+        assert first_ins is not None
+        return first_ins
 
 # 循环类，用于创建一段循环的音乐片段
 # TODO: 完善Loop存储的数据结构
 class Loop:
     def __init__(self, loop_time: int = 2, *notes: Union[Note, "Loop"]) -> None:
         if not(
             isinstance(notes, (Loop, tuple, list)) or
@@ -433,54 +462,52 @@
 
     def __iter__(self):
         pass
 
     def __next__(self):
         pass
 
-# 乐曲类
+class Rest_symbol:
+    ''' 休止符 '''
+    __singleton: Optional[Self] = None
+    def __new__(cls) -> Self:
+        if cls.__singleton is None:
+            cls.__singleton = super().__new__(cls)
+        return cls.__singleton
+
 class Piece:
+    ''' 乐曲类 '''
     def __init__(self,
                  notes: Optional[List[Union[Note, Chord]]] = None, # TODO: support Loop
-                 # 设置整个音轨的默认参数 Track global variable
-                 instrument: int = 0, # 演奏的乐器，暂时只支持传入数字
-                 pitch: int = 60, # 音高/音调
-                 bpm: int = 100, # 节奏
-                 volume: float = 1.0 # 音量/响度
-    ) -> None:
-        if not (
-                isinstance(instrument, int) and
-                isinstance(pitch, int) and
-                isinstance(bpm, int) and
-                0 < volume <= 1
-        ) or (
-            ( not isinstance(notes, (list, Loop))
+                 is_optimize: bool = True, # 是否将多个音符优化为和弦
+                 ) -> None:
+        if (
+            ( not isinstance(notes, list)
             or not all(isinstance(val, (Note, Chord)) for val in notes) )
             and notes is not None
         ):
             raise TypeError
 
-        if notes is None:
-            notes = []
+        self.is_optimize = is_optimize
 
-        self.instrument = instrument
-        self.pitch = pitch
-        self.bpm = bpm
-        self.volume = volume
-        self.notes: List[Optional[Union[Note, Chord]]] = []
-        for a_note in notes:
-            self.append(a_note)
+        # self.notes会将Note与Chord中用time表示的休止符展开为Rest_symbol
+        if notes is None:
+            self.notes = []
+        else:
+            self.notes: List[Union[Note, Chord, Rest_symbol]] = []
+            for a_note in notes:
+                self.append(a_note)
 
     # 向Piece类添加数据成员
     def append(self, other: Union[Note, Chord]) -> Self:
         if not isinstance(other, (Note, Chord)):
             raise TypeError
 
         while other.time > 1:
-            self.notes.append(None)
+            self.notes.append(Rest_symbol())
             other.time -= 1
         self.notes.append(other)
         return self
 
     # 将Piece转化为midi文件(暂不支持Chord)
     def write_midi(self,
                    filepath: str = "temp.mid",
@@ -517,15 +544,15 @@
         mid = mido.MidiFile(tracks=[track])
         channels: List[int] = [0] * 16
 
         none_counter: int = 0
          # 500_000 / 100, 500_000是Midi.tempo的默认数字，100是self.bpm的默认数字
         track.append(mido.MetaMessage("set_tempo", tempo=self.bpm * 5000, time=0))
         for a_note in self.notes:
-            if a_note is None:
+            if isinstance(a_note, Rest_symbol):
                 none_counter += 1
             elif isinstance(a_note, Chord):
                 for note_list in a_note.ins_notes.values():
                     for _a_note in note_list:
                         write_a_midi_note(_a_note)
                         none_counter = 0
             elif isinstance(a_note, Note):
@@ -543,28 +570,28 @@
     # 将Piece类转换为Midi
     def to_midi(self, filepath="temp.mid") -> Midi:
         self.write_midi(filepath)
         return Midi(filepath)
 
     # 将Piece转换为物实对应的电路
     def release(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None) -> "Player":
-        return Player(self, x, y, z, elementXYZ)
+        return Player(self, x, y, z, elementXYZ, self.is_optimize)
 
     # Piece中所有Notes与Chord的数量
     def count_notes(self) -> int:
         res = 0
         for note in self.notes:
             if isinstance(note, (Note, Chord)):
                 res += 1
         return res
 
     def __len__(self) -> int:
         return len(self.notes)
 
-    def __getitem__(self, item: int) -> Optional[Union[Note, Chord]]:
+    def __getitem__(self, item: int) -> Union[Note, Chord, Rest_symbol]:
         if not isinstance(item, int):
             raise TypeError
         return self.notes[item]
 
     def __setitem__(self, item: int, value) -> None:
         if not isinstance(item, int):
             raise TypeError
@@ -583,16 +610,17 @@
 # 将piece的数据生成为物实的电路
 class Player:
     def __init__(self,
                  musicArray: Piece,
                  x: numType = 0,
                  y: numType = 0,
                  z: numType = 0,
-                 elementXYZ = None
-    ) -> None:
+                 elementXYZ = None,
+                 is_optimize: bool = True,
+                 ) -> None:
         from physicsLab.element import count_Elements
         count_elements_start: int = count_Elements()
 
         if not (
                 isinstance(x, (int, float)) and
                 isinstance(y, (int, float)) and
                 isinstance(z, (int, float)) and
@@ -600,17 +628,17 @@
         ):
             raise TypeError
 
         if not (elementXYZ is True or (_elementXYZ.is_elementXYZ() is True and elementXYZ is None)):
             x, y, z = _elementXYZ.translateXYZ(x, y, z)
 
         # 给乐器增加休止符
-        while musicArray.notes[-1] is None:
+        while isinstance(musicArray.notes[-1], Rest_symbol):
             musicArray.notes.pop()
-        while musicArray.notes[0] is None:
+        while isinstance(musicArray.notes[0], Rest_symbol):
             musicArray.notes.pop(0)
 
         len_musicArray: int = len(musicArray)
 
         # 计算音乐矩阵的长宽
         side = None
         if len_musicArray >= 2:
@@ -657,29 +685,29 @@
         check2.i_lowmid - and_gate.o
         counter.o_upmid - check2.i_up
         crt_Wires(check2.o_lowmid, xPlayer.data_Input)
 
         # main
         xcor, ycor = -1, 0
         for a_note in musicArray:
-            if a_note is None:
+            if isinstance(a_note, Rest_symbol):
                 xcor += 1
                 if xcor == side:
                     xcor = 0
                     ycor += 2
                 continue
 
             # 当time==0时，则为和弦（几个音同时播放）
             # 此时生成的简单乐器与z轴平行
             xcor += 1
             if xcor == side:
                 xcor = 0
                 ycor += 2
             if isinstance(a_note, Chord):
-                ins = a_note.release(1 + x + xcor,  4 + y + ycor, z, elementXYZ=True)
+                ins = a_note.release(1 + x + xcor,  4 + y + ycor, z, elementXYZ=True, is_optimize=is_optimize)
             elif isinstance(a_note, Note):
                 ins = elements.Simple_Instrument(
                     1 + x + xcor, 4 + y + ycor, z, pitch=a_note.pitch,
                     instrument=a_note.instrument,
                     elementXYZ=True,
                     is_ideal_model=True,
                     velocity=a_note.velocity
```

### Comparing `physicslab-1.4.7/physicsLab/savTemplate.py` & `physicslab-1.4.8/physicsLab/savTemplate.py`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.7/physicsLab.egg-info/PKG-INFO` & `physicslab-1.4.8/physicsLab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physicsLab
-Version: 1.4.7
+Version: 1.4.8
 Summary: Python API for Physics-Lab-AR
 Home-page: https://gitee.com/script2000/physicsLab
 Author: Goodenough
 Author-email: 2381642961@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `physicslab-1.4.7/physicsLab.egg-info/SOURCES.txt` & `physicslab-1.4.8/physicsLab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `physicslab-1.4.7/setup.py` & `physicslab-1.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 import setuptools
 
 setuptools.setup(
     name="physicsLab",
-    version="1.4.7",
+    version="1.4.8",
     license="MIT",
     author="Goodenough",
     author_email="2381642961@qq.com",
     description="Python API for Physics-Lab-AR",
     long_description="click \"[there](https://gitee.com/script2000/physicsLab)\" to show more information",
     long_description_content_type="text/markdown",
     url="https://gitee.com/script2000/physicsLab",
```

