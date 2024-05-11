# Comparing `tmp/expr_codegen-0.6.2.tar.gz` & `tmp/expr_codegen-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expr_codegen-0.6.2.tar", last modified: Sun Apr 28 06:58:26 2024, max compression
+gzip compressed data, was "expr_codegen-0.6.3.tar", last modified: Sat May 11 06:28:18 2024, max compression
```

## Comparing `expr_codegen-0.6.2.tar` & `expr_codegen-0.6.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:58:26.390576 expr_codegen-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-04-28 06:58:26.390576 expr_codegen-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:58:26.390576 expr_codegen-0.6.2/expr_codegen/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/dag.py
--rw-r--r--   0 runner    (1001) docker     (127)    14433 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/expr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:58:26.390576 expr_codegen-0.6.2/expr_codegen/latex/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/latex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/latex/printer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11190 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:58:26.390576 expr_codegen-0.6.2/expr_codegen/pandas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/pandas/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     7188 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/pandas/printer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/pandas/template.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:58:26.390576 expr_codegen-0.6.2/expr_codegen/polars/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/polars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/polars/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/polars/printer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/polars/template.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:58:26.390576 expr_codegen-0.6.2/expr_codegen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-04-28 06:58:26.000000 expr_codegen-0.6.2/expr_codegen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-28 06:58:26.000000 expr_codegen-0.6.2/expr_codegen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 06:58:26.000000 expr_codegen-0.6.2/expr_codegen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-28 06:58:26.000000 expr_codegen-0.6.2/expr_codegen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-28 06:58:26.000000 expr_codegen-0.6.2/expr_codegen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 06:58:26.390576 expr_codegen-0.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 06:28:18.291448 expr_codegen-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-11 06:28:13.000000 expr_codegen-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-05-11 06:28:18.291448 expr_codegen-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-05-11 06:28:13.000000 expr_codegen-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 06:28:18.287448 expr_codegen-0.6.3/expr_codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-11 06:28:13.000000 expr_codegen-0.6.3/expr_codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-11 06:28:13.000000 expr_codegen-0.6.3/expr_codegen/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-05-11 06:28:13.000000 expr_codegen-0.6.3/expr_codegen/codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-05-11 06:28:13.000000 expr_codegen-0.6.3/expr_codegen/dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14433 2024-05-11 06:28:13.000000 expr_codegen-0.6.3/expr_codegen/expr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 06:28:18.287448 expr_codegen-0.6.3/expr_codegen/latex/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 06:28:13.000000 expr_codegen-0.6.3/expr_codegen/latex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-05-11 06:28:13.000000 expr_codegen-0.6.3/expr_codegen/latex/printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11190 2024-05-11 06:28:13.000000 expr_codegen-0.6.3/expr_codegen/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 06:28:18.287448 expr_codegen-0.6.3/expr_codegen/pandas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 06:28:13.000000 expr_codegen-0.6.3/expr_codegen/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-05-11 06:28:13.000000 expr_codegen-0.6.3/expr_codegen/pandas/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7188 2024-05-11 06:28:13.000000 expr_codegen-0.6.3/expr_codegen/pandas/printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-11 06:28:13.000000 expr_codegen-0.6.3/expr_codegen/pandas/template.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 06:28:18.287448 expr_codegen-0.6.3/expr_codegen/polars/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 06:28:13.000000 expr_codegen-0.6.3/expr_codegen/polars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-11 06:28:13.000000 expr_codegen-0.6.3/expr_codegen/polars/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-11 06:28:13.000000 expr_codegen-0.6.3/expr_codegen/polars/printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-11 06:28:13.000000 expr_codegen-0.6.3/expr_codegen/polars/template.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     8008 2024-05-11 06:28:13.000000 expr_codegen-0.6.3/expr_codegen/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 06:28:18.291448 expr_codegen-0.6.3/expr_codegen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-05-11 06:28:18.000000 expr_codegen-0.6.3/expr_codegen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-11 06:28:18.000000 expr_codegen-0.6.3/expr_codegen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 06:28:18.000000 expr_codegen-0.6.3/expr_codegen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-11 06:28:18.000000 expr_codegen-0.6.3/expr_codegen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-11 06:28:18.000000 expr_codegen-0.6.3/expr_codegen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-11 06:28:13.000000 expr_codegen-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 06:28:18.291448 expr_codegen-0.6.3/setup.cfg
```

### Comparing `expr_codegen-0.6.2/LICENSE` & `expr_codegen-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.2/PKG-INFO` & `expr_codegen-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expr_codegen
-Version: 0.6.2
+Version: 0.6.3
 Summary: symbol expression to polars expression tool
 Author-email: wukan <wu-kan@163.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, wukan
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `expr_codegen-0.6.2/README.md` & `expr_codegen-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.2/expr_codegen/codes.py` & `expr_codegen-0.6.3/expr_codegen/codes.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,29 +56,32 @@
         if old_target_id != new_target_id:
             self.targets_new.add(new_target_id)
             target.id = new_target_id
             # 记录修改的变量名，之后会使用到
             self.args_map[old_target_id] = new_target_id
 
     def visit_Assign(self, node):
+        # 调整位置，支持循环赋值
+        # _A = _A+1 调整成 _A_001 = _A_000 + 1
+        self.generic_visit(node)
+
         # 提取输出变量名
         for target in node.targets:
             if isinstance(target, ast.Tuple):
                 for t in target.elts:
                     self.__visit_Assign(t)
             else:
                 self.__visit_Assign(target)
 
         # 处理 alpha=close 这种情况
         if isinstance(node.value, ast.Name):
             self.args_old.add(node.value.id)
             node.value.id = self.args_map.get(node.value.id, node.value.id)
             self.args_new.add(node.value.id)
 
-        self.generic_visit(node)
         return node
 
     def visit_Compare(self, node):
         # 比较符的左右也可能是变量，要处理
         if isinstance(node.left, ast.Name):
             self.args_old.add(node.left.id)
             node.left.id = self.args_map.get(node.left.id, node.left.id)
```

### Comparing `expr_codegen-0.6.2/expr_codegen/dag.py` & `expr_codegen-0.6.3/expr_codegen/dag.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.2/expr_codegen/expr.py` & `expr_codegen-0.6.3/expr_codegen/expr.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.2/expr_codegen/latex/printer.py` & `expr_codegen-0.6.3/expr_codegen/latex/printer.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.2/expr_codegen/model.py` & `expr_codegen-0.6.3/expr_codegen/model.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.2/expr_codegen/pandas/code.py` & `expr_codegen-0.6.3/expr_codegen/pandas/code.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.2/expr_codegen/pandas/printer.py` & `expr_codegen-0.6.3/expr_codegen/pandas/printer.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.2/expr_codegen/pandas/template.py.j2` & `expr_codegen-0.6.3/expr_codegen/pandas/template.py.j2`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.2/expr_codegen/polars/code.py` & `expr_codegen-0.6.3/expr_codegen/polars/code.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.2/expr_codegen/polars/printer.py` & `expr_codegen-0.6.3/expr_codegen/polars/printer.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.2/expr_codegen/polars/template.py.j2` & `expr_codegen-0.6.3/expr_codegen/polars/template.py.j2`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.2/expr_codegen/tool.py` & `expr_codegen-0.6.3/expr_codegen/tool.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import inspect
-from typing import Sequence, Dict
+from functools import lru_cache
+from typing import Sequence, Dict, Optional
 
 from black import Mode, format_str
 from sympy import simplify, cse, symbols, numbered_symbols
 
+from expr_codegen.codes import sources_to_exprs
 from expr_codegen.expr import get_current_by_prefix, get_children, replace_exprs
 from expr_codegen.model import dag_start, dag_end, dag_middle
 
 
 class ExprTool:
 
     def __init__(self):
         self.get_current_func = get_current_by_prefix
         self.get_current_func_kwargs = {}
         self.exprs_dict = {}
         self.exprs_names = []
+        self.globals_ = {}
 
     def set_current(self, func, **kwargs):
         self.get_current_func = func
         self.get_current_func_kwargs = kwargs
 
     def extract(self, expr):
         """抽取分割后的子公式
@@ -202,7 +205,59 @@
                         extra_codes=extra_codes)
 
         if format:
             # 格式化。在遗传算法中没有必要
             codes = format_str(codes, mode=Mode(line_length=600, magic_trailing_comma=True))
 
         return codes, G
+
+    def exec(self, codes: str, df_input):
+        """执行代码
+
+        Notes
+        -----
+        注意生成的代码已经约定输入用df_input，输出用df_output
+
+        """
+        globals_ = {'df_input': df_input}
+        exec(codes, globals_)
+        return globals_['df_output']
+
+    @lru_cache(maxsize=64)
+    def _get_codes(self, source: str, extra_codes: str, output_file: str) -> str:
+        """通过字符串生成代码， 加了缓存，多次调用不重复生成"""
+        raw, exprs_dict = sources_to_exprs(self.globals_, source, safe=False)
+
+        # 生成代码
+        codes, G = _TOOL_.all(exprs_dict, style='polars', template_file='template.py.j2',
+                              replace=True, regroup=True, format=True,
+                              date='date', asset='asset',
+                              # 复制了需要使用的函数，还复制了最原始的表达式
+                              extra_codes=(raw,
+                                           # 传入多个列的方法
+                                           extra_codes,
+                                           ))
+
+        if output_file is not None:
+            with open(output_file, 'w', encoding='utf-8') as f:
+                f.write(codes)
+
+        return codes
+
+
+_TOOL_ = ExprTool()
+
+
+def codegen_exec(globals_, code_block, df_input,
+                 extra_codes: str = r'CS_SW_L1 = pl.col(r"^sw_l1_\d+$")',
+                 output_file: Optional[str] = None):
+    """快速转换源代码并执行"""
+    _TOOL_.globals_ = globals_
+
+    if isinstance(code_block, str):
+        source = code_block
+    else:
+        source = inspect.getsource(code_block)
+
+    codes = _TOOL_._get_codes(source, extra_codes, output_file)
+
+    return _TOOL_.exec(codes, df_input)
```

### Comparing `expr_codegen-0.6.2/expr_codegen.egg-info/PKG-INFO` & `expr_codegen-0.6.3/expr_codegen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expr_codegen
-Version: 0.6.2
+Version: 0.6.3
 Summary: symbol expression to polars expression tool
 Author-email: wukan <wu-kan@163.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, wukan
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `expr_codegen-0.6.2/expr_codegen.egg-info/SOURCES.txt` & `expr_codegen-0.6.3/expr_codegen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.2/pyproject.toml` & `expr_codegen-0.6.3/pyproject.toml`

 * *Files identical despite different names*

