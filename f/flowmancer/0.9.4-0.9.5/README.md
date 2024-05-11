# Comparing `tmp/flowmancer-0.9.4.tar.gz` & `tmp/flowmancer-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowmancer-0.9.4.tar", max compression
+gzip compressed data, was "flowmancer-0.9.5.tar", max compression
```

## Comparing `flowmancer-0.9.4.tar` & `flowmancer-0.9.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1065 2024-03-09 03:37:22.424209 flowmancer-0.9.4/LICENSE
--rw-r--r--   0        0        0    16873 2024-03-09 03:37:22.424209 flowmancer-0.9.4/README.md
--rw-r--r--   0        0        0      141 2024-03-09 03:37:22.424209 flowmancer-0.9.4/flowmancer/__init__.py
--rw-r--r--   0        0        0      279 2024-03-09 03:37:22.424209 flowmancer-0.9.4/flowmancer/checkpointer/__init__.py
--rw-r--r--   0        0        0     1085 2024-03-09 03:37:22.424209 flowmancer-0.9.4/flowmancer/checkpointer/checkpointer.py
--rw-r--r--   0        0        0     3115 2024-03-09 03:37:22.424209 flowmancer-0.9.4/flowmancer/checkpointer/database.py
--rw-r--r--   0        0        0     1199 2024-03-09 03:37:22.424209 flowmancer-0.9.4/flowmancer/checkpointer/file.py
--rw-r--r--   0        0        0     2172 2024-03-09 03:37:22.424209 flowmancer-0.9.4/flowmancer/eventbus/__init__.py
--rw-r--r--   0        0        0     1638 2024-03-09 03:37:22.424209 flowmancer-0.9.4/flowmancer/eventbus/execution.py
--rw-r--r--   0        0        0     1484 2024-03-09 03:37:22.424209 flowmancer-0.9.4/flowmancer/eventbus/log.py
--rw-r--r--   0        0        0      206 2024-03-09 03:37:22.424209 flowmancer-0.9.4/flowmancer/exceptions.py
--rw-r--r--   0        0        0     7536 2024-03-09 03:37:22.424209 flowmancer-0.9.4/flowmancer/executor.py
--rw-r--r--   0        0        0      176 2024-03-09 03:37:22.424209 flowmancer-0.9.4/flowmancer/extensions/__init__.py
--rw-r--r--   0        0        0      652 2024-03-09 03:37:22.424209 flowmancer-0.9.4/flowmancer/extensions/extension.py
--rw-r--r--   0        0        0      157 2024-03-09 03:37:22.424209 flowmancer-0.9.4/flowmancer/extensions/notifications/__init__.py
--rw-r--r--   0        0        0      626 2024-03-09 03:37:22.424209 flowmancer-0.9.4/flowmancer/extensions/notifications/email.py
--rw-r--r--   0        0        0     1269 2024-03-09 03:37:22.424209 flowmancer-0.9.4/flowmancer/extensions/notifications/notification.py
--rw-r--r--   0        0        0      514 2024-03-09 03:37:22.424209 flowmancer-0.9.4/flowmancer/extensions/notifications/pushover.py
--rw-r--r--   0        0        0      444 2024-03-09 03:37:22.424209 flowmancer-0.9.4/flowmancer/extensions/notifications/slack.py
--rw-r--r--   0        0        0     3010 2024-03-09 03:37:22.424209 flowmancer-0.9.4/flowmancer/extensions/progressbar.py
--rw-r--r--   0        0        0    19982 2024-03-09 03:37:22.424209 flowmancer-0.9.4/flowmancer/flowmancer.py
--rw-r--r--   0        0        0     2517 2024-03-09 03:37:22.424209 flowmancer-0.9.4/flowmancer/jobdefinition/__init__.py
--rw-r--r--   0        0        0     2490 2024-03-09 03:37:22.424209 flowmancer-0.9.4/flowmancer/jobdefinition/file.py
--rw-r--r--   0        0        0     1077 2024-03-09 03:37:22.424209 flowmancer-0.9.4/flowmancer/lifecycle.py
--rw-r--r--   0        0        0      139 2024-03-09 03:37:22.424209 flowmancer-0.9.4/flowmancer/loggers/__init__.py
--rw-r--r--   0        0        0     2577 2024-03-09 03:37:22.424209 flowmancer-0.9.4/flowmancer/loggers/file.py
--rw-r--r--   0        0        0      653 2024-03-09 03:37:22.424209 flowmancer-0.9.4/flowmancer/loggers/logger.py
--rw-r--r--   0        0        0        0 2024-03-09 03:37:22.424209 flowmancer-0.9.4/flowmancer/py.typed
--rw-r--r--   0        0        0      680 2024-03-09 03:37:22.424209 flowmancer-0.9.4/flowmancer/task.py
--rw-r--r--   0        0        0       22 2024-03-09 03:37:22.424209 flowmancer-0.9.4/flowmancer/version.py
--rw-r--r--   0        0        0     1158 2024-03-09 03:37:22.424209 flowmancer-0.9.4/pyproject.toml
--rw-r--r--   0        0        0    18275 1970-01-01 00:00:00.000000 flowmancer-0.9.4/setup.py
--rw-r--r--   0        0        0    17607 1970-01-01 00:00:00.000000 flowmancer-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-03-13 03:34:32.578667 flowmancer-0.9.5/LICENSE
+-rw-r--r--   0        0        0    16873 2024-03-13 03:34:32.578667 flowmancer-0.9.5/README.md
+-rw-r--r--   0        0        0      141 2024-03-13 03:34:32.578667 flowmancer-0.9.5/flowmancer/__init__.py
+-rw-r--r--   0        0        0      279 2024-03-13 03:34:32.578667 flowmancer-0.9.5/flowmancer/checkpointer/__init__.py
+-rw-r--r--   0        0        0     1085 2024-03-13 03:34:32.578667 flowmancer-0.9.5/flowmancer/checkpointer/checkpointer.py
+-rw-r--r--   0        0        0     3115 2024-03-13 03:34:32.578667 flowmancer-0.9.5/flowmancer/checkpointer/database.py
+-rw-r--r--   0        0        0     1199 2024-03-13 03:34:32.578667 flowmancer-0.9.5/flowmancer/checkpointer/file.py
+-rw-r--r--   0        0        0     2172 2024-03-13 03:34:32.578667 flowmancer-0.9.5/flowmancer/eventbus/__init__.py
+-rw-r--r--   0        0        0     1638 2024-03-13 03:34:32.578667 flowmancer-0.9.5/flowmancer/eventbus/execution.py
+-rw-r--r--   0        0        0     1484 2024-03-13 03:34:32.578667 flowmancer-0.9.5/flowmancer/eventbus/log.py
+-rw-r--r--   0        0        0      206 2024-03-13 03:34:32.578667 flowmancer-0.9.5/flowmancer/exceptions.py
+-rw-r--r--   0        0        0     7536 2024-03-13 03:34:32.578667 flowmancer-0.9.5/flowmancer/executor.py
+-rw-r--r--   0        0        0      176 2024-03-13 03:34:32.578667 flowmancer-0.9.5/flowmancer/extensions/__init__.py
+-rw-r--r--   0        0        0      652 2024-03-13 03:34:32.578667 flowmancer-0.9.5/flowmancer/extensions/extension.py
+-rw-r--r--   0        0        0      157 2024-03-13 03:34:32.578667 flowmancer-0.9.5/flowmancer/extensions/notifications/__init__.py
+-rw-r--r--   0        0        0      626 2024-03-13 03:34:32.578667 flowmancer-0.9.5/flowmancer/extensions/notifications/email.py
+-rw-r--r--   0        0        0     1269 2024-03-13 03:34:32.578667 flowmancer-0.9.5/flowmancer/extensions/notifications/notification.py
+-rw-r--r--   0        0        0      514 2024-03-13 03:34:32.578667 flowmancer-0.9.5/flowmancer/extensions/notifications/pushover.py
+-rw-r--r--   0        0        0      444 2024-03-13 03:34:32.578667 flowmancer-0.9.5/flowmancer/extensions/notifications/slack.py
+-rw-r--r--   0        0        0     3010 2024-03-13 03:34:32.578667 flowmancer-0.9.5/flowmancer/extensions/progressbar.py
+-rw-r--r--   0        0        0    20942 2024-03-13 03:34:32.578667 flowmancer-0.9.5/flowmancer/flowmancer.py
+-rw-r--r--   0        0        0     2580 2024-03-13 03:34:32.578667 flowmancer-0.9.5/flowmancer/jobdefinition/__init__.py
+-rw-r--r--   0        0        0     2949 2024-03-13 03:34:32.578667 flowmancer-0.9.5/flowmancer/jobdefinition/file.py
+-rw-r--r--   0        0        0     1077 2024-03-13 03:34:32.578667 flowmancer-0.9.5/flowmancer/lifecycle.py
+-rw-r--r--   0        0        0      139 2024-03-13 03:34:32.578667 flowmancer-0.9.5/flowmancer/loggers/__init__.py
+-rw-r--r--   0        0        0     2577 2024-03-13 03:34:32.578667 flowmancer-0.9.5/flowmancer/loggers/file.py
+-rw-r--r--   0        0        0      653 2024-03-13 03:34:32.578667 flowmancer-0.9.5/flowmancer/loggers/logger.py
+-rw-r--r--   0        0        0        0 2024-03-13 03:34:32.578667 flowmancer-0.9.5/flowmancer/py.typed
+-rw-r--r--   0        0        0      680 2024-03-13 03:34:32.578667 flowmancer-0.9.5/flowmancer/task.py
+-rw-r--r--   0        0        0       22 2024-03-13 03:34:32.578667 flowmancer-0.9.5/flowmancer/version.py
+-rw-r--r--   0        0        0     1158 2024-03-13 03:34:32.578667 flowmancer-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0    18275 1970-01-01 00:00:00.000000 flowmancer-0.9.5/setup.py
+-rw-r--r--   0        0        0    17607 1970-01-01 00:00:00.000000 flowmancer-0.9.5/PKG-INFO
```

### Comparing `flowmancer-0.9.4/LICENSE` & `flowmancer-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flowmancer-0.9.4/README.md` & `flowmancer-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `flowmancer-0.9.4/flowmancer/checkpointer/checkpointer.py` & `flowmancer-0.9.5/flowmancer/checkpointer/checkpointer.py`

 * *Files identical despite different names*

### Comparing `flowmancer-0.9.4/flowmancer/checkpointer/database.py` & `flowmancer-0.9.5/flowmancer/checkpointer/database.py`

 * *Files identical despite different names*

### Comparing `flowmancer-0.9.4/flowmancer/checkpointer/file.py` & `flowmancer-0.9.5/flowmancer/checkpointer/file.py`

 * *Files identical despite different names*

### Comparing `flowmancer-0.9.4/flowmancer/eventbus/__init__.py` & `flowmancer-0.9.5/flowmancer/eventbus/__init__.py`

 * *Files identical despite different names*

### Comparing `flowmancer-0.9.4/flowmancer/eventbus/execution.py` & `flowmancer-0.9.5/flowmancer/eventbus/execution.py`

 * *Files identical despite different names*

### Comparing `flowmancer-0.9.4/flowmancer/eventbus/log.py` & `flowmancer-0.9.5/flowmancer/eventbus/log.py`

 * *Files identical despite different names*

### Comparing `flowmancer-0.9.4/flowmancer/executor.py` & `flowmancer-0.9.5/flowmancer/executor.py`

 * *Files identical despite different names*

### Comparing `flowmancer-0.9.4/flowmancer/extensions/extension.py` & `flowmancer-0.9.5/flowmancer/extensions/extension.py`

 * *Files identical despite different names*

### Comparing `flowmancer-0.9.4/flowmancer/extensions/notifications/email.py` & `flowmancer-0.9.5/flowmancer/extensions/notifications/email.py`

 * *Files identical despite different names*

### Comparing `flowmancer-0.9.4/flowmancer/extensions/notifications/notification.py` & `flowmancer-0.9.5/flowmancer/extensions/notifications/notification.py`

 * *Files identical despite different names*

### Comparing `flowmancer-0.9.4/flowmancer/extensions/notifications/pushover.py` & `flowmancer-0.9.5/flowmancer/extensions/notifications/pushover.py`

 * *Files identical despite different names*

### Comparing `flowmancer-0.9.4/flowmancer/extensions/progressbar.py` & `flowmancer-0.9.5/flowmancer/extensions/progressbar.py`

 * *Files identical despite different names*

### Comparing `flowmancer-0.9.4/flowmancer/flowmancer.py` & `flowmancer-0.9.5/flowmancer/flowmancer.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,27 @@
         self._registered_loggers: Dict[str, Logger] = dict()
         self._checkpointer_instance: Checkpointer = FileCheckpointer()
         self._checkpointer_interval_seconds = 10.0
         self._extensions_interval_seconds = 0.25
         self._loggers_interval_seconds = 0.25
         self._synchro_interval_seconds = 0.25
         self._is_restart = False
+        self._jobdef_vars: Dict[str, str] = dict()
+
+    def set_jobdef_var(self, key: str, value: str) -> None:
+        if not isinstance(key, str):
+            raise TypeError(f'str expected for `key`, not {type(key)}')
+        if not isinstance(value, str):
+            raise TypeError(f'str expected for `value`, not {type(value)}')
+        self._jobdef_vars[key] = value
+
+    def unset_jobdef_var(self, key: str) -> None:
+        if not isinstance(key, str):
+            raise TypeError(f'str expected for `key`, not {type(key)}')
+        del self._jobdef_vars[key]
 
     def start(self, default_jobdef_path: Optional[str] = None, default_jobdef_type: str = 'yaml') -> int:
         orig_cwd = os.getcwd()
         try:
             # Ensure any components, such as file loggers, work with respect to the .py file in which the `start`
             # command is invoked, which is usually the project root dir.
             app_root_dir = os.path.dirname(os.path.abspath(inspect.stack()[-1][1]))
@@ -169,18 +182,25 @@
         parser.add_argument('-t', '--type', action='store', dest='jobdef_type', default=default_jobdef_type)
         parser.add_argument('-r', '--restart', action='store_true', dest='restart', default=False)
         parser.add_argument('-d', '--debug', action='store_true', dest='debug', default=False)
         parser.add_argument('--skip', action='append', dest='skip', default=[])
         parser.add_argument('--run-to', action='store', dest='run_to')
         parser.add_argument('--run-from', action='store', dest='run_from')
         parser.add_argument('--max-concurrency', action='store', type=int, dest='max_concurrency')
+        parser.add_argument('--var', action='append', dest='jobdef_vars', default=[])
 
         args = parser.parse_args()
         self._debug = args.debug
 
+        for v in args.jobdef_vars:
+            parts = v.split('=')
+            if len(parts) <= 1:
+                raise ValueError('`var` arguments must follow the pattern: <key>=<value>')
+            self.set_jobdef_var(parts[0], '='.join(parts[1:]))
+
         if args.jobdef:
             jobdef_path = args.jobdef if args.jobdef.startswith('/') else os.path.join(caller_cwd, args.jobdef)
             self.load_job_definition(jobdef_path, app_root_dir, args.jobdef_type)
 
         if args.restart:
             try:
                 cp = asyncio.run(self._checkpointer_instance.read_checkpoint(self._config.name))
@@ -397,15 +417,17 @@
         j: Union[JobDefinition, str],
         app_root_dir: str,
         jobdef_type: str = 'yaml'
     ) -> Flowmancer:
         if isinstance(j, JobDefinition):
             jobdef = j
         else:
-            jobdef = _job_definition_classes[jobdef_type]().load(j, LoadParams(APP_ROOT_DIR=app_root_dir))
+            jobdef = _job_definition_classes[jobdef_type]().load(
+                j, LoadParams(APP_ROOT_DIR=app_root_dir), self._jobdef_vars
+            )
 
         # Configurations
         self._config = jobdef.config
         self._synchro_interval_seconds = jobdef.config.synchro_interval_seconds
         self._loggers_interval_seconds = jobdef.config.loggers_interval_seconds
         self._extensions_interval_seconds = jobdef.config.extensions_interval_seconds
         self._checkpointer_interval_seconds = jobdef.config.checkpointer_interval_seconds
```

### Comparing `flowmancer-0.9.4/flowmancer/jobdefinition/__init__.py` & `flowmancer-0.9.5/flowmancer/jobdefinition/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import Any, Callable, Dict, List, Type, Union
+from typing import Any, Callable, Dict, List, Optional, Type, Union
 
 from pydantic import BaseModel, ConfigDict
 
 _job_definition_classes = dict()
 
 
 def job_definition(key: str) -> Callable:
@@ -69,13 +69,15 @@
 class LoadParams(BaseModel):
     model_config = ConfigDict(extra='forbid', use_enum_values=True)
     APP_ROOT_DIR: str = '.'
 
 
 class SerializableJobDefinition(ABC):
     @abstractmethod
-    def load(self, filename: Union[Path, str], params: LoadParams = LoadParams()) -> JobDefinition:
+    def load(
+        self, filename: Union[Path, str], params: LoadParams = LoadParams(), vars: Optional[Dict[str, str]] = None
+    ) -> JobDefinition:
         pass
 
     @abstractmethod
     def dump(self, jdef: JobDefinition, filename: Union[Path, str]) -> None:
         pass
```

### Comparing `flowmancer-0.9.4/flowmancer/jobdefinition/file.py` & `flowmancer-0.9.5/flowmancer/jobdefinition/file.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import re
 from pathlib import Path
-from typing import Any, Callable, Dict, Pattern, Union
+from typing import Any, Callable, Dict, Optional, Pattern, Union
 
 import yaml
 
 from . import JobDefinition, LoadParams, SerializableJobDefinition, job_definition
 
 
 def _merge(a: Any, b: Any) -> None:
@@ -23,33 +23,41 @@
             return val_dict.get(parts[0], parts[1])
         return var_matcher.sub(replace_fn, node.value)
     return _path_constructor
 
 
 @job_definition('yaml')
 class YAMLJobDefinition(SerializableJobDefinition):
-    def load(self, filename: Union[Path, str], params: LoadParams = LoadParams()) -> JobDefinition:
+    def load(
+        self, filename: Union[Path, str], params: LoadParams = LoadParams(), vars: Optional[Dict[str, str]] = None
+    ) -> JobDefinition:
         # Add constructor for built-in vars
         sys_tag = re.compile(r'[^$]*\$SYS{([^}^{]+)}.*')
         sys_var = re.compile(r'\$SYS{([^}^{]+)}')
         yaml.add_implicit_resolver("!sysvar", sys_tag, None, yaml.SafeLoader)
         yaml.add_constructor("!sysvar", _build_path_constructor(sys_var, dict(params)), yaml.SafeLoader)
 
         # Add constructor for env vars
         env_tag = re.compile(r'[^$]*\$ENV{([^}^{]+)}.*')
         env_var = re.compile(r'\$ENV{([^}^{]+)}')
         yaml.add_implicit_resolver("!envvar", env_tag, None, yaml.SafeLoader)
         yaml.add_constructor("!envvar", _build_path_constructor(env_var, dict(os.environ)), yaml.SafeLoader)
 
+        # Add constructor for input vars
+        input_tag = re.compile(r'[^$]*\$VAR{([^}^{]+)}.*')
+        input_var = re.compile(r'\$VAR{([^}^{]+)}')
+        yaml.add_implicit_resolver("!inputvar", input_tag, None, yaml.SafeLoader)
+        yaml.add_constructor("!inputvar", _build_path_constructor(input_var, vars or dict()), yaml.SafeLoader)
+
         def process_includes(jdef, merged, seen):
             for p in jdef.get('include', []):
                 if not p.startswith('/'):
                     p = os.path.abspath(os.path.join(params.APP_ROOT_DIR, p))
                 if p in seen:
-                    raise RuntimeError('asdf')
+                    raise RuntimeError(f'JobDef YAML file has already been processed once: {p}')
                 seen.add(p)
                 with open(p, 'r') as f:
                     cur = yaml.safe_load(f.read())
                     process_includes(cur, merged, seen)
             _merge(merged, jdef)
 
         merged: Dict[str, Any] = dict()
```

### Comparing `flowmancer-0.9.4/flowmancer/lifecycle.py` & `flowmancer-0.9.5/flowmancer/lifecycle.py`

 * *Files identical despite different names*

### Comparing `flowmancer-0.9.4/flowmancer/loggers/file.py` & `flowmancer-0.9.5/flowmancer/loggers/file.py`

 * *Files identical despite different names*

### Comparing `flowmancer-0.9.4/flowmancer/loggers/logger.py` & `flowmancer-0.9.5/flowmancer/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `flowmancer-0.9.4/flowmancer/task.py` & `flowmancer-0.9.5/flowmancer/task.py`

 * *Files identical despite different names*

### Comparing `flowmancer-0.9.4/pyproject.toml` & `flowmancer-0.9.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flowmancer"
-version = "0.9.4"
+version = "0.9.5"
 description = "The Python Thing-Doer"
 authors = ["Nathan Lee <lee.nathan.sh@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = '^3.8.1'
```

### Comparing `flowmancer-0.9.4/setup.py` & `flowmancer-0.9.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'requests>=2.31.0,<3.0.0',
  'rich>=13.7.1,<14.0.0',
  'types-pyyaml>=6.0.12.12,<7.0.0.0',
  'urllib3>=2.2.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'flowmancer',
-    'version': '0.9.4',
+    'version': '0.9.5',
     'description': 'The Python Thing-Doer',
     'long_description': '# Flowmancer\n\n[![pypi-version](https://img.shields.io/pypi/v/flowmancer?style=flat-square)](https://pypi.org/project/flowmancer)\n[![python-version](https://img.shields.io/badge/dynamic/json?query=info.requires_python&label=python&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fflowmancer%2Fjson&style=flat-square)](https://pypi.org/project/flowmancer)\n[![license](https://img.shields.io/github/license/natsunlee/flowmancer?style=flat-square)](LICENSE)\n[![circle-ci](https://img.shields.io/circleci/build/github/natsunlee/flowmancer?style=flat-square)](https://app.circleci.com/pipelines/github/natsunlee/flowmancer)\n[![coveralls](https://img.shields.io/coveralls/github/natsunlee/flowmancer?style=flat-square)](https://coveralls.io/github/natsunlee/flowmancer?branch=main)\n[![pypi-downloads](https://img.shields.io/pypi/dm/flowmancer?style=flat-square)](https://pypistats.org/packages/flowmancer)\n[![Ko-Fi](https://img.shields.io/badge/Support%20Me%20On%20Ko--fi-F16061?style=flat-square&logo=ko-fi&logoColor=white)](https://ko-fi.com/natsunlee)\n\nFlowmancer aims to help you do *things* in a sequential or parallel manner. It enables you to write tasks in Python, describe their order, then execute them with as little effort as possible.\n\nBut why do I need this? Couldn\'t I just write my own Python code to do *stuff*?\n\nYou certainly could!\n\nThough Flowmancer provides gives you a head-start to building your custom processes with optional add-ons for logging, checkpoint/restarts in the event of failures, or even custom task observers to do...things while your things do things!\n\n## Installation\nSimply install the `flowmancer` package with:\n```bash\npip3 install flowmancer\n```\n\nNOTE: `flowmancer` supports only Python 3.7 and higher.\n\n## Basic Usage\nLet\'s assume you have a new project with a basic structure like so:\n```\nmy_project\n├─ job.yaml\n├─ main.py\n└─ tasks/\n   ├─ __init__.py\n   └─ mytasks.py\n```\n\nTo use `flowmancer`, you\'ll need to provide a few things:\n* `Task` implementations (`mytasks.py`)\n* A job YAML file (`job.yaml`)\n* Your main/driver code (`main.py`)\n\n### Tasks\nBy default, Flowmancer recursively searches in the `./tasks` directory (relative to where `Flowmancer()` is initialized - in this case, `main.py`) for `Task` implementations decorated with `@task`. See the Advanced Usage section for details on how to add other directories or packages that contain `Task` implementations.\n\nA `flowmancer` task is simply a class that extends the `Task` abstract class, which, at minimum requires that the `run` method be implemented:\n```python\nimport time\nfrom flowmancer.task import Task, task\n\n@task\nclass WaitAndSucceed(Task):\n    # All variables should be given type hints and optional vars should be given default values.\n    my_required_string_var: str\n    my_optional_int_var: int = 5\n\n    def run(self):\n        # Store string input var in the shared dictionary accessible by other tasks.\n        self.shared_dict["my_var"] = f"Hello from: {self.my_required_string_var}!"\n\n        # Sleep for seconds defined by input var (using default of 5).\n        print(f"Starting up and sleeping for {self.my_optional_int_var} seconds!")\n        time.sleep(self.my_optional_int_var)\n        print("Done!")\n\n@task\nclass ImmediatelySucceed(Task):\n    def run(self):\n        # Print statements will automatically be sent to configured loggers.\n        print("Success!")\n\n@task\nclass FailImmediately(Task):\n    def run(self):\n        print(f"Printing `my_var` value: {self.shared_dict[\'my_var\']}")\n        # Raise errors to cause tasks to fail and additionally block dependent tasks, if any.\n        raise RuntimeError("Let this be caught by Flowmancer")\n```\n\nAny `print()` or exceptions will write log messages to any configured loggers (zero or more loggers may be defined).\n\n### Job Definition YAML File\nThis file describes what code to run, in what order, as well as additional add-ons to supplement the job during execution:\n```yaml\nversion: 0.1\n\n# This entire config block is currently optional, however, it is recommended to at least provide a unique name for each\n# Job Definition YAML file, as this name is used for checkpointing jobs in the event of failures.\nconfig:\n  name: \'my-flowmancer-job\'\n\ntasks:\n  # No dependency - run right away\n  # Add `parameters` key-value pairs for any required and optional task variables.\n  succeed-task-a:\n    task: WaitAndSucceed\n    parameters:\n      my_required_string_var: "My First Task!"\n\n  # No dependency - run right away\n  succeed-task-b:\n    task: ImmediatelySucceed\n\n  # Only run if prior 2 tasks complete successfully\n  final-fail-task:\n    task: FailImmediately\n    max_attempts: 3  # Retry uup to 2 times upon failure (1 initial exec + 2 retries = 3 attempts)\n    dependencies:\n      - succeed-task-a\n      - succeed-task-b\n```\n\n### Driver\nThe driver is super simple and simply requires running an instance of `Flowmancer`\n```python\n# main.py\nimport sys\nfrom flowmancer import Flowmancer\n\nif __name__ == \'__main__\':\n    # The `start()` method will return a non-zero integer on failure, typically equal to the number of failed tasks.\n    ret = Flowmancer().start()\n\n    # Exceptions from tasks will be captured and logged, rather than being raised up to this level. To cause this\n    # driver program to fail, either explicitly raise your own error OR call sys.exit.\n    if ret:\n      raise RuntimeError(\'Flowmancer job has failed!\')\n\n    # Alternatively, instead of crashing w/ an exception, simply exit with a non-zero value.\n    # sys.exit(ret)\n```\n\n### Executing the Job\n```bash\npython3 main.py -j ./path/to/job.yaml\n```\n\nTo run from point-of-failure (if any):\n```bash\npython3 main.py -j ./path/to/job.yaml -r\n```\nIf no prior failure is detected, the job will start as if no `-r` flag were given.\n\nNote that the job definition must still be provided with the `-r` flag.\n\n## Advanced Usage\n\n### Optional Configurations\nIn the `config` block of the Job Definition, the following optional parameters may be given:\n|Parameter|Type|Default Value|Description|\n|---|---|---|---|\n|name|str|\'flowmancer\'|Name/identifier for Job Definition. Used for saving checkpoints used for job restarts in the event of a failure.|\n|max_concurrency|int|0|Maximum number tasks that can run in parallel. If 0 or less, then there is no limit.|\n|extension_directories|List[str]|[]|List of paths, either absolute or relative to driver `.py` file, that contain any `@task`, `@logger`, or `@extension` decorated classes to make accessible to Flowmancer. The `./task`, `./extensions`, and `./loggers` directories are ALWAYS checked by default.|\n|extension_packages|List[str]|[]|List of installed Python packages that contain `@task`, `@logger`, or `@extension` decorated classes to make accessible to Flowmancer.|\n|synchro_interval_seconds|float|0.25|Core execution loop interval for waking and checking status of tasks and whether loggers/extensions/checkpointer should trigger.|\n|loggers_interval_seconds|float|0.25|Interval in seconds to wait before emitting log messages to configured `Logger` instances.|\n|extensions_interval_seconds|float|0.25|Interval in seconds to wait before emitting state change information to configured `Extension` instances.|\n|checkpointer_interval_seconds|float|10.0|Interval in seconds to wait before writing checkpoint information to the configured `Checkpointer`.|\n\nFor example:\n```yaml\nconfig:\n  name: \'most-important-job\'\n  max_concurrency: 20\n  extension_directories:\n    - ./client_implementations\n    - /opt/flowmancer/tasks\n  extension_packages:\n    - internal_flowmancer_package\n```\n\n### Include YAML Files\nAn optional `include` block may be defined in the Job Definition in order to merge multiple Job Definition YAML files.\nYAML files are provided in a list and processed in the order given, with the containing YAML being processed last.\n\nFor example:\n```yaml\n# <app_root_dir>/jobdefs/template.yaml\nconfig:\n  name: generic-template\n\ntasks:\n  do-something:\n    task: DoSomething\n    parameters:\n      some_required_param: I am a required string parameter\n```\n\n```yaml\n# <app_root_dir>/jobdefs/cleanup_addon.yaml\ninclude:\n  - ./jobdefs/template.yaml\n\ntasks:\n  cleanup:\n    task: Cleanup\n    dependencies:\n      - do-something\n```\n\n```yaml\n# <app_root_dir>/jobdefs/complete.yaml\nconfig:\n  name: complete-job\n\ninclude:\n  - ./jobdefs/cleanup_addon.yaml\n\ntasks:\n  do-something:\n    task: Do Something\n    parameters:\n      added_optional_param: 99\n```\n\nLoading the `complete.yaml` job definition will result in a YAML equivalent to:\n```yaml\nconfig:\n  name: complete-job\n\ntasks:\n  do-something:\n    task: Do Something\n    parameters:\n      some_required_param: I am a required string parameter\n      added_optional_param: 99\n```\n\n> :warning: Array values are **NOT** merged like dictionaries are. Any array values (and therfore any nested structures) within them will be replaced if modified in a later YAML.\n\nAdditionally, the above example could have all `include` values in the `complete.yaml` file and the `include` block removed from `cleanup_addon.yaml`:\n```yaml\n# <app_root_dir>/jobdefs/complete.yaml\nconfig:\n  name: complete-job\n\n# As with most paths in Job Definition, paths to `include` YAML files are relative to `.py` file where the `.start()`\n# method for Flowmancer is invoked.\ninclude:\n  - ./jobdefs/template.yaml\n  - ./jobdefs/cleanup_addon.yaml\n\ntasks:\n  do-something:\n    task: Do Something\n    parameters:\n      added_optional_param: 99\n```\n\nThe `include` values are processed in order and results in the same outcome as the original example.\n\n### Changing Default File Logger Directory\nThe Job Definition accepts an optional `loggers` section, which if left empty will default to using a `FileLogger` with default settings.\nTo utilize the default `FileLogger`, but with a different configuration, explicitly provide the `loggers` block:\n```yaml\nloggers:\n  my-file-logger:\n    logger: FileLogger\n    parameters:\n      # NOTE: this path is relative to the `.py` file where `Flowmancer().start()` is invoked.\n      base_log_dir: ./my_custom_log_dir  # ./logs is the default, if omitted.\n      retention_days: 3  # 10 is the default, if omitted.\n```\n\n### Complex Parameters\nWhile this is mostly used for `Task` implementations, the details outlined here apply for any built-in and custom `Extension` and `Logger` implementations.\n\nFlowmancer makes heavy use of [Pydantic](https://docs.pydantic.dev/latest/) to validate parameters and ensure that values loaded from the Job Definition are of the appropriate type.\n\nThis means that a `Task` can have complex types (including custom models) like:\n```python\nfrom enum import Enum\nfrom flowmancer.task import Task, task\nfrom pydantic import BaseModel\nfrom typing import Dict, List\n\nclass Protocol(Enum):\n    HTTP: \'HTTP\'\n    HTTPS: \'HTTPS\'\n\nclass APIDetails(BaseModel):\n    protocol: Protocol = Protocol.HTTPS\n    base_url: str\n    endpoint: str\n\n@task\nclass DownloadDataFromRestApi(Task):\n    api_details: APIDetails\n    target_dir: str\n    target_filename: str = \'data.json\'\n\n    def run(self) -> None:\n        url = f\'{self.api_details.protocol}://{self.api_details.base_url}/{self.api_details.endpoint}\'\n        # Continued implementation...\n```\n\nAnd the Job Definition snippet for this task might be:\n```yaml\ntasks:\n  download-file-one:\n    task: DownloadDataFromRestApi\n    parameters:\n      api_details:\n        # We leave out `protocol` because we want to just use the default `HTTPS` value.\n        base_url: www.some_data_api.com\n        endpoint: /v1/data/weather/today\n      target_dir: /data/todays_weather\n      # Override the default `target_filename` value given in the class implementation.\n      target_filename: weather.json\n```\n\n### Task Lifecycle Methods\nIn addition to the required `run` method, an implementation of `Task` may optionally include the following methods:\n|Method|Required|Order|Description|\n|---|---|---|---|\n|on_create|No|1|First method executed when a task is released for execution. Note that a task is not considered "created" until it enters the `RUNNING` state.|\n|on_restart|No|2|Executed only if a task is running from the result of a recovery from `FAILED` state. If a task was failed in `DEFAULTED` state, this method will not be executed.|\n|run|Yes|3|Always required and always executed once task is in `RUNNING` state, unless prior lifecycle methods have failed.|\n|on_success|No|4|Executed only if `run` method ends in success.|\n|on_failure|No|5|Executed only if `run` method ends in failure/exception.|\n|on_destroy|No|6|Always executed after all other lifecycle methods.|\n|on_abort|No|-|Executed when `SIGINT` signal is sent to tasks/Flowmancer.|\n\nJust as with `run`, all lifecycle methods have access to `self.shared_dict` and any parameters.\n\n### Custom Loggers\nCustom implementations of the `Logger` may be provided to Flowmancer to either replace OR write to in addition to the default `FileLogger`.\n\nA custom implementation must extend the `Logger` class, be decorated with the `logger` decorator, and implement the async `update` method at minimum:\n```python\n@logger\nimport json\nimport requests\nfrom flowmancer.loggers.logger import Logger, logger\n\nclass SlackMessageLogger(Logger):\n    webhook: str\n\n    def _post_to_slack(self, msg: str) -> None:\n        requests.post(\n            self.webhook,\n            data=json.dumps({\'text\': title, \'attachments\': [{\'text\': msg}]}),\n            headers={\'Content-Type\': \'application/json\'},\n        )\n\n    async def update(self, evt: SerializableLogEvent) -> None:\n        # The `LogStartEvent` and `LogEndEvent` events only have a `name` property.\n        if isinstance(evt, LogStartEvent):\n            self._post_to_slack(f\'[{evt.name}] START: Logging is beginning\')\n        elif isinstance(evt, LogEndEvent):\n            self._post_to_slack(f\'[{evt.name}] END: Logging is ending\')\n        # The `LogWriteEvent` additionally has `severity` and `message` properties.\n        elif isinstance(evt, LogWriteEvent):\n            self._post_to_slack(f\'[{evt.name}] {evt.severity.value}: {evt.message}\')\n```\n\nThe `Logger` implementation may also have the following optional `async` lifecycle methods:\n* `on_create`\n* `on_restart`\n* `on_success`\n* `on_failure`\n* `on_destroy`\n* `on_abort`\n\nTo incorporate your custom `Logger` into Flowmancer, ensure that it exists in a module either in `./loggers` or in a module listed in `config.extension_directories` in the Job Definition.\n\nThis allows it to be provided in the `loggers` section of the Job Definition.\n> :warning: Providing the `loggers` section will remove the default logger (`FileLogger`) from your job\'s configuration.\n> If you want to add your custom logger alongside the default logger, the `FileLogger` must explicitly be configured.\n\n```yaml\nloggers:\n  # Load the default logger with default parameters\n  default-logger:\n    logger: FileLogger\n\n  # Custom logger implementation\n  slack-logger:\n    logger: SlackMessageLogger\n    parameters:\n      webhook: https://some.webhook.url\n```\n\n### Custom Extensions\nComing soon.\n\n### Custom Checkpointers\nCustom implementations of the `Checkpointer` may be provided to Flowmancer to replace the default `FileCheckpointer`.\n> :warning: Unlike loggers and extensions, only one checkpointer can be configured per Job Definition.\n\nA custom implementation must extend the `Checkpointer` class, be decorated with the `checkpointer` decorator, and implement the async `write_checkpoint`, `read_checkpoint`, and `clear_checkpoints` methods at minimum. It may also optinoally implement async lifecycle methods, similar to [Custom Loggers](#custom-loggers):\n```python\nfrom .checkpointer import CheckpointContents, Checkpointer, NoCheckpointAvailableError, checkpointer\n\n@checkpointer\nclass DatabaseCheckpointer(Checkpointer):\n    host: str\n    port: int\n    username: str\n    password: str\n\n    def write_checkpoint(self, name: str, content: CheckpointContents) -> None:\n        # Store checkpoint state - must be able to store contents of\n        # `CheckpointContents` in a way that it can be reconstructed later.\n\n    def read_checkpoint(self, name: str) -> CheckpointContents:\n        # Recall checkpoint state - reconstruct and return `CheckpointContents`\n        # if exists for `name`. Otherwise raise `NoCheckpointAvailableError`\n        # to indicate no valid checkpoint exists to restart from.\n\n    def clear_checkpoint(self, name: str) -> None:\n        # Remove checkpoint state for `name`.\n```\n\nTo incorporate your custom `Checkpointer` into Flowmancer, ensure that it exists in a module either in `./extensions` or in a module listed in `config.extension_directories` in the Job Definition.\n\nThis allows it to be provided in the `checkpointer` section of the Job Definition:\n```yaml\ncheckpointer:\n  checkpointer: DatabaseCheckpointer\n  parameters:\n    host: something\n    port: 9999\n    username: user\n    password: 1234\n```\n',
     'author': 'Nathan Lee',
     'author_email': 'lee.nathan.sh@outlook.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `flowmancer-0.9.4/PKG-INFO` & `flowmancer-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowmancer
-Version: 0.9.4
+Version: 0.9.5
 Summary: The Python Thing-Doer
 License: MIT
 Author: Nathan Lee
 Author-email: lee.nathan.sh@outlook.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

