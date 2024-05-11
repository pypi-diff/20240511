# Comparing `tmp/magia_flow-0.1.0.tar.gz` & `tmp/magia_flow-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magia_flow-0.1.0.tar", max compression
+gzip compressed data, was "magia_flow-0.2.0.tar", max compression
```

## Comparing `magia_flow-0.1.0.tar` & `magia_flow-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,18 @@
--rw-r--r--   0        0        0     1069 2024-02-26 21:26:36.738261 magia_flow-0.1.0/LICENSE
--rw-r--r--   0        0        0      472 2024-02-26 21:26:36.738261 magia_flow-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-02-26 21:26:36.738261 magia_flow-0.1.0/magia_flow/__init__.py
--rw-r--r--   0        0        0      487 2024-02-26 21:26:36.738261 magia_flow-0.1.0/magia_flow/online/__init__.py
--rw-r--r--   0        0        0     1549 2024-02-26 21:26:36.738261 magia_flow-0.1.0/magia_flow/online/digitaljs.py
--rw-r--r--   0        0        0        0 2024-02-26 21:26:36.738261 magia_flow-0.1.0/magia_flow/simulation/__init__.py
--rw-r--r--   0        0        0     3440 2024-02-26 21:26:36.738261 magia_flow-0.1.0/magia_flow/simulation/general.py
--rw-r--r--   0        0        0     2782 2024-02-26 21:26:36.738261 magia_flow-0.1.0/magia_flow/simulation/surfer.py
--rw-r--r--   0        0        0     1851 2024-02-26 21:26:36.738261 magia_flow-0.1.0/magia_flow/simulation/verilator.py
--rw-r--r--   0        0        0     1419 2024-02-26 21:26:36.738261 magia_flow-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1421 1970-01-01 00:00:00.000000 magia_flow-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-11 21:00:55.314060 magia_flow-0.2.0/LICENSE
+-rw-r--r--   0        0        0      472 2024-05-11 21:00:55.314060 magia_flow-0.2.0/README.md
+-rw-r--r--   0        0        0      104 2024-05-11 21:00:55.314060 magia_flow-0.2.0/magia_flow/__init__.py
+-rw-r--r--   0        0        0     1302 2024-05-11 21:00:55.314060 magia_flow-0.2.0/magia_flow/__main__.py
+-rw-r--r--   0        0        0       89 2024-05-11 21:00:55.314060 magia_flow-0.2.0/magia_flow/formal/__init__.py
+-rw-r--r--   0        0        0     7828 2024-05-11 21:00:55.314060 magia_flow-0.2.0/magia_flow/formal/sby.py
+-rw-r--r--   0        0        0      487 2024-05-11 21:00:55.314060 magia_flow-0.2.0/magia_flow/online/__init__.py
+-rw-r--r--   0        0        0     1374 2024-05-11 21:00:55.314060 magia_flow-0.2.0/magia_flow/online/digitaljs/Dockerfile
+-rw-r--r--   0        0        0      224 2024-05-11 21:00:55.314060 magia_flow-0.2.0/magia_flow/online/digitaljs/docker-compose.yml
+-rw-r--r--   0        0        0      232 2024-05-11 21:00:55.314060 magia_flow-0.2.0/magia_flow/online/digitaljs/nginx.conf
+-rw-r--r--   0        0        0     2861 2024-05-11 21:00:55.314060 magia_flow-0.2.0/magia_flow/online/digitaljs.py
+-rw-r--r--   0        0        0     1863 2024-05-11 21:00:55.314060 magia_flow-0.2.0/magia_flow/oss_cad.py
+-rw-r--r--   0        0        0      126 2024-05-11 21:00:55.314060 magia_flow-0.2.0/magia_flow/simulation/__init__.py
+-rw-r--r--   0        0        0     3808 2024-05-11 21:00:55.314060 magia_flow-0.2.0/magia_flow/simulation/general.py
+-rw-r--r--   0        0        0     2782 2024-05-11 21:00:55.314060 magia_flow-0.2.0/magia_flow/simulation/surfer.py
+-rw-r--r--   0        0        0     1888 2024-05-11 21:00:55.314060 magia_flow-0.2.0/magia_flow/simulation/verilator.py
+-rw-r--r--   0        0        0     1557 2024-05-11 21:00:55.314060 magia_flow-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1537 1970-01-01 00:00:00.000000 magia_flow-0.2.0/PKG-INFO
```

### Comparing `magia_flow-0.1.0/LICENSE` & `magia_flow-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `magia_flow-0.1.0/magia_flow/simulation/general.py` & `magia_flow-0.2.0/magia_flow/simulation/general.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+Generalized Simulator with Magia Module Elaboration.
+
+This shall be used with test cases scripted with cocotb.
+"""
 import inspect
 import os
 import sys
 from contextlib import contextmanager
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import Optional, Sequence, Union
@@ -24,22 +29,25 @@
 
         self.output_file = f"{self.build_dir}/magia.generated.sv"
         self.top_level = hdl_toplevel
         self.source_files = []
         self.elaborated_sv = []
 
     def add_source(self, source_file: os.PathLike):
+        """Add a SystemVerilog file for simulation."""
         self.source_files.append(source_file)
 
     def add_magia_module(self, *module: Module):
+        """Elaborate Magia Modules for simulation."""
         self.elaborated_sv.append(
             Elaborator.to_string(*module)
         )
 
     def compile(self, waves: bool = False, **kwargs):
+        """Compile the SV code into the simulator."""
         if waves:
             kwargs["build_args"] = kwargs.get("build_args", []) + ["--trace", "--trace-fst"]
 
         with open(self.output_file, mode="w") as f:
             f.write("\n\n".join(self.elaborated_sv))
         self.runner.build(
             verilog_sources=self.source_files + [self.output_file],
@@ -53,14 +61,15 @@
             self,
             test_module: Union[str, Sequence[str]],
             python_search_path: Optional[Union[str, Sequence[str]]] = None,
             testcase: Optional[Union[str, Sequence[str]]] = None,
             waves: bool = False,
             **kwargs
     ):
+        """Simulate the test module with the testcases provided."""
         if waves:
             if self.simulator_type == "verilator":
                 kwargs["test_args"] = kwargs.get("test_args", []) + ["--trace", "--trace-fst"]
             else:
                 kwargs["waves"] = waves
 
         with self._patch_sys_path(python_search_path):
@@ -72,31 +81,28 @@
                 test_dir=self.build_dir,
                 results_xml="results.xml",
                 **kwargs
             )
 
     @property
     def wave_file(self):
+        """Return the path to the waveform file."""
         if self.simulator_type == "verilator":
             return Path(self.build_dir, "dump.fst")
         raise NotImplementedError("Wave file not supported for this simulator")
 
     @staticmethod
     def current_dir():
-        """
-        Return the directory of the caller script file
-        """
+        """Return the directory of the caller script file."""
         caller_frame = inspect.stack()[1]
         return str(Path(caller_frame.filename).parent.absolute())
 
     @staticmethod
     def current_package():
-        """
-        Return the package name of the caller script file
-        """
+        """Return the package name of the caller script file."""
         caller_frame = inspect.stack()[1]
         return str(Path(caller_frame.filename).stem)
 
     @staticmethod
     @contextmanager
     def _patch_sys_path(paths):
         cur_paths = sys.path
```

### Comparing `magia_flow-0.1.0/magia_flow/simulation/surfer.py` & `magia_flow-0.2.0/magia_flow/simulation/surfer.py`

 * *Files identical despite different names*

### Comparing `magia_flow-0.1.0/magia_flow/simulation/verilator.py` & `magia_flow-0.2.0/magia_flow/simulation/verilator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
+"""Utility functions related to Verilator."""
 import os
 import shutil
 import subprocess
 import sys
 from pathlib import Path
 
 
 def init_verilator():
-    """
-    Initialize Verilator in virtual environment for cocotb tests
-    """
+    """Initialize Verilator in virtual environment for cocotb tests."""
     if not (verilator := shutil.which("verilator")):
         raise RuntimeError("Verilator not found in PATH")
 
     version = subprocess.check_output([verilator, "--version"]).decode().strip().split()[1]  # noqa: S603
     if float(version) < 5.006:
         raise RuntimeError("Verilator version >= 5.006 is required")
```

### Comparing `magia_flow-0.1.0/pyproject.toml` & `magia_flow-0.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 line-length = 120
-lint.select = ["F", "E", "W", "I001", "U", "N", "S", "B", "A", "C4", "T10", "ISC", "ICN", "T20", "Q", "RET", "SIM", "TID", "ERA"]
+lint.select = ["D2", "D3", "D4", "F", "E", "W", "I001", "U", "N", "S", "B", "A", "C4", "T10", "ISC", "ICN", "T20", "Q", "RET", "SIM", "TID", "ERA"]
 lint.ignore = ["F821", "A003"]
+lint.pydocstyle.convention = "pep257"
 
 [tool.ruff.lint.per-file-ignores]
 
 "tests/**" = ["S101", "S311"]
 
 [tool.poetry]
 name = "magia-flow"
-version = "0.1.0"
+version = "0.2.0"
 description = "Design flow integration and automation with Magia"
 readme = "README.md"
 authors = ["khwong-c64 <kin.hin.wong.c@gmail.com>"]
 license = "LICENSE"
 
 packages = [
     { include = "magia_flow" },
@@ -34,25 +35,29 @@
 keywords = [
     "Verilog HDL", "SystemVerilog",
     "Synthesizable", "RTL", "HDL", "Hardware Description Language",
     "Code Generation", "FPGA", "ASIC", "EDA", "RTL Design"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 magia-hdl = "^0.5"
 httpx = "*"
+click = "^8.1.7"
+flask = "^3.0.2"
+ruamel-yaml = "^0.18.6"
+defusedxml = "^0.7.1"
 
 [tool.poetry.group.dev.dependencies]
 cocotb = "*"
 cocotb-test = "*"
 pytest = "*"
 pytest-xdist = "*"
 pytest-github-report = "*"
-ruff = "~0.2.1"
+ruff = "==0.3.3"
 hdlConvertor-binary = "~2.3"
 
 [tool.poetry.urls]
 Repository = "https://github.com/magia-hdl/magia-flow"
 
 [tool.pytest.ini_options]
 norecursedirs = "tests/helpers"
```

### Comparing `magia_flow-0.1.0/PKG-INFO` & `magia_flow-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: magia-flow
-Version: 0.1.0
+Version: 0.2.0
 Summary: Design flow integration and automation with Magia
 License: LICENSE
 Keywords: Verilog HDL,SystemVerilog,Synthesizable,RTL,HDL,Hardware Description Language,Code Generation,FPGA,ASIC,EDA,RTL Design
 Author: khwong-c64
 Author-email: kin.hin.wong.c@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: click (>=8.1.7,<9.0.0)
+Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
+Requires-Dist: flask (>=3.0.2,<4.0.0)
 Requires-Dist: httpx
 Requires-Dist: magia-hdl (>=0.5,<0.6)
+Requires-Dist: ruamel-yaml (>=0.18.6,<0.19.0)
 Project-URL: Repository, https://github.com/magia-hdl/magia-flow
 Description-Content-Type: text/markdown
 
 # Magia Flow
 
 ## Brief
```

