# Comparing `tmp/tulona-0.7.6.tar.gz` & `tmp/tulona-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tulona-0.7.6.tar", last modified: Fri May 10 05:16:28 2024, max compression
+gzip compressed data, was "tulona-0.7.8.tar", last modified: Sat May 11 06:49:30 2024, max compression
```

## Comparing `tulona-0.7.6.tar` & `tulona-0.7.8.tar`

### file list

```diff
@@ -1,49 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:16:28.648059 tulona-0.7.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-10 05:16:18.000000 tulona-0.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14575 2024-05-10 05:16:28.648059 tulona-0.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13280 2024-05-10 05:16:18.000000 tulona-0.7.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:16:28.640059 tulona-0.7.6/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:16:28.640059 tulona-0.7.6/core/tulona/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:16:28.644059 tulona-0.7.6/core/tulona/adapter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:16:28.644059 tulona-0.7.6/core/tulona/adapter/base/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/adapter/base/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/adapter/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/adapter/mssql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/adapter/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/adapter/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/adapter/snowflake.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:16:28.644059 tulona-0.7.6/core/tulona/cli/
--rw-r--r--   0 runner    (1001) docker     (127)    19902 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/cli/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:16:28.644059 tulona-0.7.6/core/tulona/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/config/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/config/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/config/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:16:28.644059 tulona-0.7.6/core/tulona/task/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/task/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    22826 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/task/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/task/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/task/ping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/task/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    16757 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/task/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:16:28.648059 tulona-0.7.6/core/tulona/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/util/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/util/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/util/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/util/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/util/profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/util/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-10 05:16:18.000000 tulona-0.7.6/core/tulona/util/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:16:28.648059 tulona-0.7.6/core/tulona.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14575 2024-05-10 05:16:28.000000 tulona-0.7.6/core/tulona.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-10 05:16:28.000000 tulona-0.7.6/core/tulona.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 05:16:28.000000 tulona-0.7.6/core/tulona.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-10 05:16:28.000000 tulona-0.7.6/core/tulona.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-10 05:16:28.000000 tulona-0.7.6/core/tulona.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 05:16:28.000000 tulona-0.7.6/core/tulona.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-10 05:16:18.000000 tulona-0.7.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 05:16:28.648059 tulona-0.7.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 06:49:30.574219 tulona-0.7.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-11 06:49:25.000000 tulona-0.7.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14810 2024-05-11 06:49:30.574219 tulona-0.7.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13105 2024-05-11 06:49:25.000000 tulona-0.7.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 06:49:30.566219 tulona-0.7.8/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 06:49:30.566219 tulona-0.7.8/core/tulona/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-11 06:49:25.000000 tulona-0.7.8/core/tulona/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 06:49:30.570219 tulona-0.7.8/core/tulona/adapter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 06:49:30.570219 tulona-0.7.8/core/tulona/adapter/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-11 06:49:25.000000 tulona-0.7.8/core/tulona/adapter/base/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-11 06:49:25.000000 tulona-0.7.8/core/tulona/adapter/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-11 06:49:25.000000 tulona-0.7.8/core/tulona/adapter/mssql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-11 06:49:25.000000 tulona-0.7.8/core/tulona/adapter/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-11 06:49:25.000000 tulona-0.7.8/core/tulona/adapter/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-11 06:49:25.000000 tulona-0.7.8/core/tulona/adapter/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 06:49:30.570219 tulona-0.7.8/core/tulona/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)    16347 2024-05-11 06:49:25.000000 tulona-0.7.8/core/tulona/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-11 06:49:25.000000 tulona-0.7.8/core/tulona/cli/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 06:49:30.570219 tulona-0.7.8/core/tulona/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 06:49:25.000000 tulona-0.7.8/core/tulona/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-11 06:49:25.000000 tulona-0.7.8/core/tulona/config/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-11 06:49:25.000000 tulona-0.7.8/core/tulona/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-11 06:49:25.000000 tulona-0.7.8/core/tulona/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 06:49:30.570219 tulona-0.7.8/core/tulona/task/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-11 06:49:25.000000 tulona-0.7.8/core/tulona/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22645 2024-05-11 06:49:25.000000 tulona-0.7.8/core/tulona/task/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-11 06:49:25.000000 tulona-0.7.8/core/tulona/task/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-11 06:49:25.000000 tulona-0.7.8/core/tulona/task/ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-11 06:49:25.000000 tulona-0.7.8/core/tulona/task/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16644 2024-05-11 06:49:25.000000 tulona-0.7.8/core/tulona/task/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 06:49:30.570219 tulona-0.7.8/core/tulona/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 06:49:25.000000 tulona-0.7.8/core/tulona/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-11 06:49:25.000000 tulona-0.7.8/core/tulona/util/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-11 06:49:25.000000 tulona-0.7.8/core/tulona/util/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-05-11 06:49:25.000000 tulona-0.7.8/core/tulona/util/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-11 06:49:25.000000 tulona-0.7.8/core/tulona/util/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-11 06:49:25.000000 tulona-0.7.8/core/tulona/util/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-05-11 06:49:25.000000 tulona-0.7.8/core/tulona/util/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-11 06:49:25.000000 tulona-0.7.8/core/tulona/util/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 06:49:30.570219 tulona-0.7.8/core/tulona.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14810 2024-05-11 06:49:30.000000 tulona-0.7.8/core/tulona.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-11 06:49:30.000000 tulona-0.7.8/core/tulona.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 06:49:30.000000 tulona-0.7.8/core/tulona.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-11 06:49:30.000000 tulona-0.7.8/core/tulona.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-11 06:49:30.000000 tulona-0.7.8/core/tulona.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-11 06:49:30.000000 tulona-0.7.8/core/tulona.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-11 06:49:25.000000 tulona-0.7.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 06:49:30.574219 tulona-0.7.8/setup.cfg
```

### Comparing `tulona-0.7.6/LICENSE` & `tulona-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tulona-0.7.6/PKG-INFO` & `tulona-0.7.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulona
-Version: 0.7.6
+Version: 0.7.8
 Summary: A tool to compare data from different sources.
 Author: Mrinal Kanti Sardar
 Project-URL: Homepage, https://github.com/mrinalsardar/tulona
 Project-URL: Documentation, https://github.com/mrinalsardar/tulona
 Project-URL: Repository, https://github.com/mrinalsardar/tulona.git
 Project-URL: Issues, https://github.com/mrinalsardar/tulona/issues
 Keywords: tulona,comparison,data comparison,database scan,database profile
@@ -26,14 +26,25 @@
 Requires-Dist: cryptography~=42.0
 Requires-Dist: snowflake-sqlalchemy~=1.5
 Requires-Dist: pyodbc~=5.1
 Requires-Dist: pandas~=1.5
 Requires-Dist: openpyxl~=3.1
 Requires-Dist: Jinja2~=3.1
 Requires-Dist: pydantic~=2.7
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: faker; extra == "dev"
+Requires-Dist: bump-my-version; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
 
 Tulona
 ======
 A utility to compare tables, espacially useful to perform validations for migration projects.
 
 .. list-table::
    :widths: 50 200
@@ -369,18 +380,14 @@
 
 and it will run all the `compare` tasks defined in the `task_config` section. From our example project config file above, it will run 2 `compare` tasks.
 
 Also setting up `task_config` can be greatly benificial as you can set up different instance of same/different tasks with different config to execute in one go with the `run` command.
 
 Please look at the sample project config from above to understand how to set up `task_config` property.
 
-For debug level log, add `-v` or `--verbose` flag along with any command. For example:
-
-``tulona ping -v --datasources employee_postgres``
-
 To know more about any specific command, execute `tulona <command> -h`.
 
 
 Supported Data Platforms
 ------------------------
 
 .. list-table::
@@ -397,15 +404,15 @@
      - snowflake
    * - Microsoft SQL Server
      - mssql
 
 
 Development Environment Setup
 -----------------------------
-* For live installation execute `pip install -e .` and `pip install -r dev-requirements.txt`.
+* For live installation execute `pip install -e ".[dev]"`.
 
 
 Build Wheel Executable
 ----------------------
 * Execute `python -m build`.
 
 Install Wheel Executable File
```

### Comparing `tulona-0.7.6/README.rst` & `tulona-0.7.8/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -336,18 +336,14 @@
 
 and it will run all the `compare` tasks defined in the `task_config` section. From our example project config file above, it will run 2 `compare` tasks.
 
 Also setting up `task_config` can be greatly benificial as you can set up different instance of same/different tasks with different config to execute in one go with the `run` command.
 
 Please look at the sample project config from above to understand how to set up `task_config` property.
 
-For debug level log, add `-v` or `--verbose` flag along with any command. For example:
-
-``tulona ping -v --datasources employee_postgres``
-
 To know more about any specific command, execute `tulona <command> -h`.
 
 
 Supported Data Platforms
 ------------------------
 
 .. list-table::
@@ -364,15 +360,15 @@
      - snowflake
    * - Microsoft SQL Server
      - mssql
 
 
 Development Environment Setup
 -----------------------------
-* For live installation execute `pip install -e .` and `pip install -r dev-requirements.txt`.
+* For live installation execute `pip install -e ".[dev]"`.
 
 
 Build Wheel Executable
 ----------------------
 * Execute `python -m build`.
 
 Install Wheel Executable File
```

### Comparing `tulona-0.7.6/core/tulona/adapter/connection.py` & `tulona-0.7.8/core/tulona/adapter/connection.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.6/core/tulona/adapter/mssql.py` & `tulona-0.7.8/core/tulona/adapter/mssql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.6/core/tulona/adapter/mysql.py` & `tulona-0.7.8/core/tulona/adapter/mysql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.6/core/tulona/adapter/postgres.py` & `tulona-0.7.8/core/tulona/adapter/postgres.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.6/core/tulona/adapter/snowflake.py` & `tulona-0.7.8/core/tulona/adapter/snowflake.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.6/core/tulona/cli/base.py` & `tulona-0.7.8/core/tulona/cli/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,21 +4,20 @@
 from pathlib import Path
 
 import click
 
 from tulona.cli import params as p
 from tulona.config.profile import Profile
 from tulona.config.project import Project
-from tulona.config.runtime import RunConfig
 from tulona.exceptions import TulonaMissingPropertyError
 from tulona.task.compare import CompareColumnTask, CompareRowTask, CompareTask
 from tulona.task.ping import PingTask
 from tulona.task.profile import ProfileTask
 from tulona.task.scan import ScanTask
-from tulona.util.filesystem import get_final_outdir
+from tulona.util.filesystem import get_run_result_dir, get_task_outdir
 
 log = logging.getLogger()
 log_formatter = logging.Formatter(
     "[%(asctime)s] {%(filename)s:%(lineno)d} %(levelname)s - %(message)s"
 )
 
 consloe_handler = logging.StreamHandler()
@@ -40,37 +39,34 @@
     context_settings={"help_option_names": ["-h", "--help"]},
     no_args_is_help=True,
     epilog="Execute: tulona <command> -h/--help for more help with specific commands",
 )
 @click.pass_context
 def cli(ctx):
     """Tulona compares data sources to find out differences"""
+    logging.getLogger("tulona").setLevel(logging.DEBUG)
+
+    prof = Profile()
+    proj = Project()
+    ctx.obj = ctx.obj or {}
+    ctx.obj["project"] = proj.load_project_config()
+    ctx.obj["profile"] = prof.load_profile_config()[ctx.obj["project"]["name"]]
+    ctx.obj["project"]["run_result_dir"] = get_run_result_dir(
+        basedir=ctx.obj["project"]["outdir"]
+    )
 
 
 # command: tulona ping
 @cli.command("ping")
 @click.pass_context
 # @p.exec_engine
-@p.outdir
-@p.verbose
 @p.datasources
 def ping(ctx, **kwargs):
     """Test connectivity to datasources"""
 
-    if kwargs["verbose"]:
-        logging.getLogger("tulona").setLevel(logging.DEBUG)
-        logging.getLogger("snowflake").setLevel(logging.DEBUG)
-
-    prof = Profile()
-    proj = Project()
-
-    ctx.obj = ctx.obj or {}
-    ctx.obj["project"] = proj.load_project_config()
-    ctx.obj["profile"] = prof.load_profile_config()[ctx.obj["project"]["name"]]
-
     ping_tasks = []
     if kwargs["datasources"]:
         task_config = {
             "task": "compare",
             "datasources": kwargs["datasources"].split(","),
         }
         ping_tasks.append(task_config)
@@ -93,38 +89,20 @@
         ).execute()
 
 
 # command: tulona scan
 @cli.command("scan")
 @click.pass_context
 # @p.exec_engine
-@p.outdir
-@p.verbose
 @p.datasources
 @p.compare
 @p.sample_count
 @p.composite
 def scan(ctx, **kwargs):
     """Scan data sources to collect metadata"""
-
-    if kwargs["verbose"]:
-        logging.getLogger("tulona").setLevel(logging.DEBUG)
-
-    prof = Profile()
-    proj = Project()
-
-    ctx.obj = ctx.obj or {}
-    ctx.obj["project"] = proj.load_project_config()
-    ctx.obj["profile"] = prof.load_profile_config()[ctx.obj["project"]["name"]]
-    ctx.obj["runtime"] = RunConfig(options=kwargs, project=ctx.obj["project"])
-
-    # Override config outdir if provided in command line
-    if kwargs["outdir"]:
-        ctx.obj["project"]["outdir"] = kwargs["outdir"]
-
     scan_tasks = []
     if kwargs["datasources"]:
         task_config = {
             "task": "compare",
             "datasources": kwargs["datasources"].split(","),
         }
         if kwargs["compare"]:
@@ -142,57 +120,38 @@
             "Nothing to execute. Either define tasks in task_config section of the"
             " project config file or pass --datasources argument with values."
         )
     log.debug(f"Number of scan tasks to execute: {len(scan_tasks)}")
 
     for tconf in scan_tasks:
         log.debug(f"Executing scan with task profile: {tconf}")
-        final_outdir = get_final_outdir(
-            basedir=ctx.obj["project"]["outdir"],
+        final_outdir = get_task_outdir(
+            run_dir=ctx.obj["project"]["run_result_dir"],
             task_conf=tconf,
         )
 
         ScanTask(
             profile=ctx.obj["profile"],
             project=ctx.obj["project"],
-            runtime=ctx.obj["runtime"],
             datasources=tconf["datasources"],
             final_outdir=final_outdir,
             compare=tconf["compare"] if "compare" in tconf else None,
             sample_count=tconf["sample_count"] if "sample_count" in tconf else None,
             composite=tconf["composite"] if "composite" in tconf else None,
         ).execute()
 
 
 # command: tulona profile
 @cli.command("profile")
 @click.pass_context
 # @p.exec_engine
-@p.outdir
-@p.verbose
 @p.datasources
 @p.compare
 def profile(ctx, **kwargs):
     """Profile data sources to collect metadata [row count, column min/max/mean etc.]"""
-
-    if kwargs["verbose"]:
-        logging.getLogger("tulona").setLevel(logging.DEBUG)
-
-    prof = Profile()
-    proj = Project()
-
-    ctx.obj = ctx.obj or {}
-    ctx.obj["project"] = proj.load_project_config()
-    ctx.obj["profile"] = prof.load_profile_config()[ctx.obj["project"]["name"]]
-    ctx.obj["runtime"] = RunConfig(options=kwargs, project=ctx.obj["project"])
-
-    # Override config outdir if provided in command line
-    if kwargs["outdir"]:
-        ctx.obj["project"]["outdir"] = kwargs["outdir"]
-
     profile_tasks = []
     if kwargs["datasources"]:
         task_config = {
             "task": "compare",
             "datasources": kwargs["datasources"].split(","),
         }
         if kwargs["compare"]:
@@ -208,56 +167,37 @@
             "Nothing to execute. Either define tasks in task_config section of the"
             " project config file or pass --datasources argument with values."
         )
     log.debug(f"Number of profile tasks to execute: {len(profile_tasks)}")
 
     for tconf in profile_tasks:
         log.debug(f"Executing profile with task profile: {tconf}")
-        final_outdir = get_final_outdir(
-            basedir=ctx.obj["project"]["outdir"],
+        final_outdir = get_task_outdir(
+            run_dir=ctx.obj["project"]["run_result_dir"],
             task_conf=tconf,
         )
         outfile_fqn = Path(final_outdir, "profile_metadata.xlsx")
 
         ProfileTask(
             profile=ctx.obj["profile"],
             project=ctx.obj["project"],
-            runtime=ctx.obj["runtime"],
             datasources=tconf["datasources"],
             outfile_fqn=outfile_fqn,
             compare=tconf["compare"] if "compare" in tconf else None,
         ).execute()
 
 
 # command: tulona compare-row
 @cli.command("compare-row")
 @click.pass_context
 # @p.exec_engine
-@p.outdir
-@p.verbose
 @p.datasources
 @p.sample_count
 def compare_row(ctx, **kwargs):
     """Compares rows from two data entities"""
-
-    if kwargs["verbose"]:
-        logging.getLogger("tulona").setLevel(logging.DEBUG)
-
-    prof = Profile()
-    proj = Project()
-
-    ctx.obj = ctx.obj or {}
-    ctx.obj["project"] = proj.load_project_config()
-    ctx.obj["profile"] = prof.load_profile_config()[ctx.obj["project"]["name"]]
-    ctx.obj["runtime"] = RunConfig(options=kwargs, project=ctx.obj["project"])
-
-    # Override config outdir if provided in command line
-    if kwargs["outdir"]:
-        ctx.obj["project"]["outdir"] = kwargs["outdir"]
-
     compare_row_tasks = []
     if kwargs["datasources"]:
         task_config = {
             "task": "compare",
             "datasources": kwargs["datasources"].split(","),
         }
         if kwargs["sample_count"]:
@@ -273,61 +213,42 @@
             "Nothing to execute. Either define tasks in task_config section of the"
             " project config file or pass --datasources argument with values."
         )
     log.debug(f"Number compare-row tasks to execute: {len(compare_row_tasks)}")
 
     for tconf in compare_row_tasks:
         log.debug(f"Executing compare-row with task profile: {tconf}")
-        final_outdir = get_final_outdir(
-            basedir=ctx.obj["project"]["outdir"],
+        final_outdir = get_task_outdir(
+            run_dir=ctx.obj["project"]["run_result_dir"],
             task_conf=tconf,
         )
         outfile_fqn = Path(final_outdir, "row_comparison.xlsx")
 
         CompareRowTask(
             profile=ctx.obj["profile"],
             project=ctx.obj["project"],
-            runtime=ctx.obj["runtime"],
             datasources=tconf["datasources"],
             outfile_fqn=outfile_fqn,
             sample_count=tconf["sample_count"] if "sample_count" in tconf else None,
         ).execute()
 
 
 # command: tulona compare-column
 @cli.command("compare-column")
 @click.pass_context
 # @p.exec_engine
-@p.outdir
-@p.verbose
 @p.datasources
 @p.composite
 def compare_column(ctx, **kwargs):
     """
     Column name must be specified for task: compare-column
     by specifying 'compare_column' property in
     all the datasource[project] configs
     (check sample tulona-project.yml file for example)
     """
-
-    if kwargs["verbose"]:
-        logging.getLogger("tulona").setLevel(logging.DEBUG)
-
-    prof = Profile()
-    proj = Project()
-
-    ctx.obj = ctx.obj or {}
-    ctx.obj["project"] = proj.load_project_config()
-    ctx.obj["profile"] = prof.load_profile_config()[ctx.obj["project"]["name"]]
-    ctx.obj["runtime"] = RunConfig(options=kwargs, project=ctx.obj["project"])
-
-    # Override config outdir if provided in command line
-    if kwargs["outdir"]:
-        ctx.obj["project"]["outdir"] = kwargs["outdir"]
-
     compare_column_tasks = []
     if kwargs["datasources"]:
         task_config = {
             "task": "compare-column",
             "datasources": kwargs["datasources"].split(","),
         }
         if kwargs["composite"]:
@@ -343,59 +264,40 @@
             "Nothing to execute. Either define tasks in task_config section of the"
             " project config file or pass --datasources argument with values."
         )
     log.debug(f"Number compare-column tasks to execute: {len(compare_column_tasks)}")
 
     for tconf in compare_column_tasks:
         log.debug(f"Executing compare-column with task profile: {tconf}")
-        final_outdir = get_final_outdir(
-            basedir=ctx.obj["project"]["outdir"],
+        final_outdir = get_task_outdir(
+            run_dir=ctx.obj["project"]["run_result_dir"],
             task_conf=tconf,
         )
         outfile_fqn = Path(final_outdir, "column_comparison.xlsx")
 
         CompareColumnTask(
             profile=ctx.obj["profile"],
             project=ctx.obj["project"],
-            runtime=ctx.obj["runtime"],
             datasources=tconf["datasources"],
             outfile_fqn=outfile_fqn,
             composite=tconf["composite"] if "composite" in tconf else None,
         ).execute()
 
 
 # command: tulona compare
 @cli.command("compare")
 @click.pass_context
 # @p.exec_engine
-@p.outdir
-@p.verbose
 @p.datasources
 @p.sample_count
 @p.composite
 def compare(ctx, **kwargs):
     """
     Compare everything(profiles, rows and columns) for the given datasoures
     """
-
-    if kwargs["verbose"]:
-        logging.getLogger("tulona").setLevel(logging.DEBUG)
-
-    prof = Profile()
-    proj = Project()
-
-    ctx.obj = ctx.obj or {}
-    ctx.obj["project"] = proj.load_project_config()
-    ctx.obj["profile"] = prof.load_profile_config()[ctx.obj["project"]["name"]]
-    ctx.obj["runtime"] = RunConfig(options=kwargs, project=ctx.obj["project"])
-
-    # Override config outdir if provided in command line
-    if kwargs["outdir"]:
-        ctx.obj["project"]["outdir"] = kwargs["outdir"]
-
     compare_tasks = []
     if kwargs["datasources"]:
         task_config = {
             "task": "compare",
             "datasources": kwargs["datasources"].split(","),
         }
         if kwargs["sample_count"]:
@@ -413,60 +315,41 @@
             "Nothing to execute. Either define tasks in task_config section of the"
             " project config file or pass --datasources argument with values."
         )
     log.debug(f"Number compare tasks to execute: {len(compare_tasks)}")
 
     for tconf in compare_tasks:
         log.debug(f"Executing compare with task profile: {tconf}")
-        final_outdir = get_final_outdir(
-            basedir=ctx.obj["project"]["outdir"],
+        final_outdir = get_task_outdir(
+            run_dir=ctx.obj["project"]["run_result_dir"],
             task_conf=tconf,
         )
         outfile_fqn = Path(final_outdir, "comparison.xlsx")
 
         CompareTask(
             profile=ctx.obj["profile"],
             project=ctx.obj["project"],
-            runtime=ctx.obj["runtime"],
             datasources=tconf["datasources"],
             outfile_fqn=outfile_fqn,
             sample_count=tconf["sample_count"] if "sample_count" in tconf else None,
             composite=tconf["composite"] if "composite" in tconf else None,
         ).execute()
 
 
 # command: tulona run
 @cli.command("run")
 @click.pass_context
 # @p.exec_engine
-@p.outdir
-@p.verbose
 def run(ctx, **kwargs):
     """Run all tasks defined by `task_config` attribute in the project config file"""
-
-    if kwargs["verbose"]:
-        logging.getLogger("tulona").setLevel(logging.DEBUG)
-
-    prof = Profile()
-    proj = Project()
-
-    ctx.obj = ctx.obj or {}
-    ctx.obj["project"] = proj.load_project_config()
-    ctx.obj["profile"] = prof.load_profile_config()[ctx.obj["project"]["name"]]
-    ctx.obj["runtime"] = RunConfig(options=kwargs, project=ctx.obj["project"])
-
     if "task_config" not in ctx.obj["project"]:
         raise TulonaMissingPropertyError(
             "Attribute `task_config` is not defined in project config"
         )
 
-    # Override config outdir if provided in command line
-    if kwargs["outdir"]:
-        ctx.obj["project"]["outdir"] = kwargs["outdir"]
-
     # Extract tasks
     ping_tasks = [t for t in ctx.obj["project"]["task_config"] if t["task"] == "ping"]
     profile_tasks = [
         t for t in ctx.obj["project"]["task_config"] if t["task"] == "profile"
     ]
     compare_row_tasks = [
         t for t in ctx.obj["project"]["task_config"] if t["task"] == "compare-row"
@@ -487,105 +370,100 @@
             project=ctx.obj["project"],
             datasources=tconf["datasources"],
         ).execute()
 
     # ProfileTask
     for tconf in profile_tasks:
         log.debug(f"Executing profile with task profile: {tconf}")
-        final_outdir = get_final_outdir(
-            basedir=ctx.obj["project"]["outdir"],
+        final_outdir = get_task_outdir(
+            run_dir=ctx.obj["project"]["run_result_dir"],
             task_conf=tconf,
         )
         outfile_fqn = Path(final_outdir, "profile_metadata.xlsx")
 
         try:
             ProfileTask(
                 profile=ctx.obj["profile"],
                 project=ctx.obj["project"],
-                runtime=ctx.obj["runtime"],
                 datasources=tconf["datasources"],
                 outfile_fqn=outfile_fqn,
                 compare=tconf["compare"] if "compare" in tconf else None,
             ).execute()
         except Exception:
             log.error(f"Profiling failed with error: {traceback.format_exc()}")
 
     # CompareRowTask
     for tconf in compare_row_tasks:
         log.debug(f"Executing compare-row with task profile: {tconf}")
-        final_outdir = get_final_outdir(
-            basedir=ctx.obj["project"]["outdir"],
+        final_outdir = get_task_outdir(
+            run_dir=ctx.obj["project"]["run_result_dir"],
             task_conf=tconf,
         )
         outfile_fqn = Path(final_outdir, "row_comparison.xlsx")
 
         try:
             CompareRowTask(
                 profile=ctx.obj["profile"],
                 project=ctx.obj["project"],
-                runtime=ctx.obj["runtime"],
                 datasources=tconf["datasources"],
                 outfile_fqn=outfile_fqn,
                 sample_count=tconf["sample_count"] if "sample_count" in tconf else None,
             ).execute()
         except Exception:
             log.error(f"Row comparison failed with error: {traceback.format_exc()}")
 
     # CompareColumnTask
     for tconf in compare_column_tasks:
         log.debug(f"Executing compare-column with task profile: {tconf}")
-        final_outdir = get_final_outdir(
-            basedir=ctx.obj["project"]["outdir"],
+        final_outdir = get_task_outdir(
+            run_dir=ctx.obj["project"]["run_result_dir"],
             task_conf=tconf,
         )
         outfile_fqn = Path(final_outdir, "column_comparison.xlsx")
 
         try:
             CompareColumnTask(
                 profile=ctx.obj["profile"],
                 project=ctx.obj["project"],
-                runtime=ctx.obj["runtime"],
                 datasources=tconf["datasources"],
                 outfile_fqn=outfile_fqn,
                 composite=tconf["composite"] if "composite" in tconf else None,
             ).execute()
         except Exception:
             log.error(f"Column comparison failed with errorr: {traceback.format_exc()}")
 
     # CompareTask
     for tconf in compare_tasks:
         log.debug(f"Executing compare with task profile: {tconf}")
-        final_outdir = get_final_outdir(
-            basedir=ctx.obj["project"]["outdir"],
+        final_outdir = get_task_outdir(
+            run_dir=ctx.obj["project"]["run_result_dir"],
             task_conf=tconf,
         )
         outfile_fqn = Path(final_outdir, "comparison.xlsx")
 
         CompareTask(
             profile=ctx.obj["profile"],
             project=ctx.obj["project"],
-            runtime=ctx.obj["runtime"],
             datasources=tconf["datasources"],
             outfile_fqn=outfile_fqn,
             sample_count=tconf["sample_count"] if "sample_count" in tconf else None,
             composite=tconf["composite"] if "composite" in tconf else None,
         ).execute()
 
     # ScanTask
     for tconf in scan_tasks:
         log.debug(f"Executing scan with task profile: {tconf}")
-        final_outdir = get_final_outdir(
-            basedir=ctx.obj["project"]["outdir"],
+        final_outdir = get_task_outdir(
+            run_dir=ctx.obj["project"]["run_result_dir"],
             task_conf=tconf,
         )
 
         ScanTask(
             profile=ctx.obj["profile"],
             project=ctx.obj["project"],
-            runtime=ctx.obj["runtime"],
             datasources=tconf["datasources"],
             final_outdir=final_outdir,
             compare=tconf["compare"] if "compare" in tconf else None,
             sample_count=tconf["sample_count"] if "sample_count" in tconf else None,
             composite=tconf["composite"] if "composite" in tconf else None,
         ).execute()
```

### Comparing `tulona-0.7.6/core/tulona/cli/params.py` & `tulona-0.7.8/core/tulona/cli/params.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,13 @@
 import click
 
 exec_engine = click.option(
     "--engine", help="Execution engine. Can be one of Pandas right now", type=click.STRING
 )
 
-outdir = click.option(
-    "--outdir",
-    help="Directory to write the result of the comparison and other related metadata",
-    type=click.STRING,
-)
-
-verbose = click.option("--verbose", "-v", is_flag=True, help="Show debug level logs")
-
 datasources = click.option(
     "--datasources",
     help="Comma separated list of one or more datasource names defined in tulona-conf.yml file",
 )
 
 sample_count = click.option(
     "--sample-count", type=int, help="Number of maximum records to be compared"
```

### Comparing `tulona-0.7.6/core/tulona/config/profile.py` & `tulona-0.7.8/core/tulona/config/profile.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 from pathlib import Path
+from typing import Dict
 
 from tulona.exceptions import TulonaMissingPropertyError, TulonaProfileException
 from tulona.util.filesystem import path_exists
 from tulona.util.yaml_parser import read_yaml
 
 log = logging.getLogger(__name__)
 
@@ -16,30 +17,30 @@
     def get_profile_root(self):
         return Path(Path.home(), ".tulona")
 
     @property
     def profile_conf_path(self) -> str:
         return Path(self.get_profile_root, PROFILE_FILE_NAME)
 
-    def validate_profile_config(self, profile_dict_raw: dict) -> bool:
+    def validate_profile_config(self, profile_dict_raw: dict) -> bool | None:
         for proj in profile_dict_raw:
             proj_dict = profile_dict_raw[proj]
             if "profiles" not in proj_dict:
                 raise TulonaMissingPropertyError(
                     f"Project {proj} doesn't have any connection profiles defined"
                 )
 
             for prof in proj_dict["profiles"]:
                 prof_dict = proj_dict["profiles"][prof]
                 if "type" not in prof_dict:
                     raise TulonaMissingPropertyError(
                         f"Connection profile {prof} doesn't 'type' specified"
                     )
 
-    def load_profile_config(self) -> None:
+    def load_profile_config(self) -> Dict | None:
         profile_file_uri = self.profile_conf_path
         log.debug(f"Attempting to load profile config from {profile_file_uri}")
 
         if not path_exists(profile_file_uri):
             raise TulonaProfileException(
                 f"Profile file {profile_file_uri} does not exist."
             )
```

### Comparing `tulona-0.7.6/core/tulona/config/project.py` & `tulona-0.7.8/core/tulona/config/project.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.6/core/tulona/exceptions.py` & `tulona-0.7.8/core/tulona/exceptions.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.6/core/tulona/task/base.py` & `tulona-0.7.8/core/tulona/task/base.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.6/core/tulona/task/compare.py` & `tulona-0.7.8/core/tulona/task/compare.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from copy import deepcopy
 from dataclasses import _MISSING_TYPE, dataclass, fields
 from pathlib import Path
 from typing import Dict, List, Union
 
 import pandas as pd
 
-from tulona.config.runtime import RunConfig
 from tulona.exceptions import TulonaMissingPrimaryKeyError, TulonaMissingPropertyError
 from tulona.task.base import BaseTask
 from tulona.task.helper import perform_comparison
 from tulona.task.profile import ProfileTask
 from tulona.util.database import get_table_primary_keys
 from tulona.util.dataframe import apply_column_exclusion
 from tulona.util.excel import highlight_mismatch_cells
@@ -36,15 +35,14 @@
 }
 
 
 @dataclass
 class CompareRowTask(BaseTask):
     profile: Dict
     project: Dict
-    runtime: RunConfig
     datasources: List[str]
     outfile_fqn: Union[Path, str]
     sample_count: int = DEFAULT_VALUES["sample_count"]
 
     # Support for default values
     def __post_init__(self):
         for field in fields(self):
@@ -225,15 +223,17 @@
                     dbtype1, table_fqn1, self.sample_count, query_expr
                 )
 
             sanitized_query1 = re.sub(r"where(.*)\(.*\)", r"where\g<1>(...)", query1)
             log.debug(f"Executing query: {sanitized_query1}")
             df1 = get_query_output_as_df(connection_manager=conman1, query_text=query1)
             if df1.shape[0] == 0:
-                raise ValueError(f"Table {table_fqn1} doesn't have any data")
+                log.warning(f"Couldn't extract rows from {table_fqn1}")
+                i += 1
+                continue
 
             df1 = df1.rename(columns={c: c.lower() for c in df1.columns})
             for k in primary_key:
                 if k not in df1.columns.tolist():
                     raise ValueError(f"Primary key {k} not present in {table_fqn1}")
 
             # Exclude columns
@@ -325,15 +325,14 @@
         log.info(f"Finished task: compare-row in {exec_time:.2f} seconds")
 
 
 @dataclass
 class CompareColumnTask(BaseTask):
     profile: Dict
     project: Dict
-    runtime: RunConfig
     datasources: List[str]
     outfile_fqn: Union[Path, str]
     composite: bool = DEFAULT_VALUES["compare_column_composite"]
 
     def execute(self):
         log.info("------------------------ Starting task: compare-column")
         start_time = time.time()
@@ -489,15 +488,14 @@
         log.info(f"Finished task: compare-column in {exec_time:.2f} seconds")
 
 
 @dataclass
 class CompareTask(BaseTask):
     profile: Dict
     project: Dict
-    runtime: RunConfig
     datasources: List[str]
     outfile_fqn: Union[Path, str]
     sample_count: int = DEFAULT_VALUES["sample_count"]
     composite: bool = DEFAULT_VALUES["compare_column_composite"]
 
     # Support for default values
     def __post_init__(self):
@@ -514,28 +512,26 @@
         start_time = time.time()
 
         # Metadata comparison
         try:
             ProfileTask(
                 profile=self.profile,
                 project=self.project,
-                runtime=self.runtime,
                 datasources=self.datasources,
                 outfile_fqn=self.outfile_fqn,
                 compare=True,
             ).execute()
         except Exception:
             log.error(f"Profiling failed with error: {traceback.format_exc()}")
 
         # Row comparison
         primary_key = None
         cdt = CompareRowTask(
             profile=self.profile,
             project=self.project,
-            runtime=self.runtime,
             datasources=self.datasources,
             outfile_fqn=self.outfile_fqn,
             sample_count=self.sample_count,
         )
         try:
             primary_key = cdt.extract_confs()["primary_key"]
             cdt.execute()
@@ -547,15 +543,14 @@
         for ds in project_copy["datasources"]:
             if "compare_column" not in ds and primary_key:
                 project_copy["datasources"][ds]["compare_column"] = primary_key
         try:
             CompareColumnTask(
                 profile=self.profile,
                 project=project_copy,
-                runtime=self.runtime,
                 datasources=self.datasources,
                 outfile_fqn=self.outfile_fqn,
                 composite=self.composite,
             ).execute()
         except Exception:
             log.error(f"Column comparison failed with error: {traceback.format_exc()}")
```

### Comparing `tulona-0.7.6/core/tulona/task/helper.py` & `tulona-0.7.8/core/tulona/task/helper.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.6/core/tulona/task/ping.py` & `tulona-0.7.8/core/tulona/task/ping.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.6/core/tulona/task/profile.py` & `tulona-0.7.8/core/tulona/task/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import time
 from dataclasses import _MISSING_TYPE, dataclass, fields
 from pathlib import Path
 from typing import Dict, List, Union
 
 import pandas as pd
 
-from tulona.config.runtime import RunConfig
 from tulona.task.base import BaseTask
 from tulona.task.helper import create_profile, perform_comparison
 from tulona.util.excel import highlight_mismatch_cells
 from tulona.util.filesystem import create_dir_if_not_exist
 from tulona.util.profiles import extract_profile_name, get_connection_profile
 
 log = logging.getLogger(__name__)
@@ -21,15 +20,14 @@
 }
 
 
 @dataclass
 class ProfileTask(BaseTask):
     profile: Dict
     project: Dict
-    runtime: RunConfig
     datasources: List[str]
     outfile_fqn: Union[Path, str]
     compare: bool = DEFAULT_VALUES["compare_profiles"]
 
     # Support for default values
     def __post_init__(self):
         for field in fields(self):
```

### Comparing `tulona-0.7.6/core/tulona/task/scan.py` & `tulona-0.7.8/core/tulona/task/scan.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import os
 import time
 from copy import deepcopy
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Dict, List, Union
 
-from tulona.config.runtime import RunConfig
 from tulona.exceptions import TulonaMissingPropertyError, TulonaUnSupportedTaskError
 from tulona.task.base import BaseTask
 from tulona.task.compare import CompareTask
 from tulona.task.helper import perform_comparison
 from tulona.util.excel import dataframes_into_excel
 from tulona.util.filesystem import create_dir_if_not_exist
 from tulona.util.profiles import extract_profile_name, get_connection_profile
@@ -28,15 +27,14 @@
 }
 
 
 @dataclass
 class ScanTask(BaseTask):
     profile: Dict
     project: Dict
-    runtime: RunConfig
     datasources: List[str]
     final_outdir: Union[Path, str]
     compare: bool = DEFAULT_VALUES["compare_scans"]
     sample_count: int = DEFAULT_VALUES["sample_count"]
     composite: bool = DEFAULT_VALUES["compare_column_composite"]
 
     def execute(self):
@@ -368,15 +366,14 @@
                     )
 
                     # Execute CompareTask
                     log.debug(f"Executing CompareTask for: {source_map_item}")
                     CompareTask(
                         profile=self.profile,
                         project=dynamic_project_config,
-                        runtime=self.runtime,
                         datasources=source_map_item,
                         outfile_fqn=table_outfile_fqn,
                         sample_count=self.sample_count,
                         composite=self.composite,
                     ).execute()
 
         exec_time = time.time() - start_time
```

### Comparing `tulona-0.7.6/core/tulona/util/database.py` & `tulona-0.7.8/core/tulona/util/database.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.6/core/tulona/util/dataframe.py` & `tulona-0.7.8/core/tulona/util/dataframe.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.6/core/tulona/util/excel.py` & `tulona-0.7.8/core/tulona/util/excel.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.6/core/tulona/util/profiles.py` & `tulona-0.7.8/core/tulona/util/profiles.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.6/core/tulona/util/sql.py` & `tulona-0.7.8/core/tulona/util/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,18 @@
     return table_fqn
 
 
 def get_sample_row_query(dbtype: str, table_name: str, sample_count: int):
     dbtype = dbtype.lower()
 
     # TODO: validate sampling mechanism for maximum possible randomness
-    if dbtype in ["snowflake", "mssql"]:
+    if dbtype == "snowflake":
         query = f"select * from {table_name} tablesample ({sample_count} rows)"
+    elif dbtype == "mssql":
+        query = f"select top {sample_count} * from {table_name}"
     elif dbtype == "postgres":
         # TODO: system_rows method not implemented, tablesample works for percentage selection
         # query = f"select * from {table_name} tablesample system_rows({sample_count})"
         query = f"select * from {table_name} limit {sample_count}"
     elif dbtype == "mysql":
         query = f"select * from {table_name} limit {sample_count}"
     else:
```

### Comparing `tulona-0.7.6/core/tulona.egg-info/PKG-INFO` & `tulona-0.7.8/core/tulona.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulona
-Version: 0.7.6
+Version: 0.7.8
 Summary: A tool to compare data from different sources.
 Author: Mrinal Kanti Sardar
 Project-URL: Homepage, https://github.com/mrinalsardar/tulona
 Project-URL: Documentation, https://github.com/mrinalsardar/tulona
 Project-URL: Repository, https://github.com/mrinalsardar/tulona.git
 Project-URL: Issues, https://github.com/mrinalsardar/tulona/issues
 Keywords: tulona,comparison,data comparison,database scan,database profile
@@ -26,14 +26,25 @@
 Requires-Dist: cryptography~=42.0
 Requires-Dist: snowflake-sqlalchemy~=1.5
 Requires-Dist: pyodbc~=5.1
 Requires-Dist: pandas~=1.5
 Requires-Dist: openpyxl~=3.1
 Requires-Dist: Jinja2~=3.1
 Requires-Dist: pydantic~=2.7
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: faker; extra == "dev"
+Requires-Dist: bump-my-version; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
 
 Tulona
 ======
 A utility to compare tables, espacially useful to perform validations for migration projects.
 
 .. list-table::
    :widths: 50 200
@@ -369,18 +380,14 @@
 
 and it will run all the `compare` tasks defined in the `task_config` section. From our example project config file above, it will run 2 `compare` tasks.
 
 Also setting up `task_config` can be greatly benificial as you can set up different instance of same/different tasks with different config to execute in one go with the `run` command.
 
 Please look at the sample project config from above to understand how to set up `task_config` property.
 
-For debug level log, add `-v` or `--verbose` flag along with any command. For example:
-
-``tulona ping -v --datasources employee_postgres``
-
 To know more about any specific command, execute `tulona <command> -h`.
 
 
 Supported Data Platforms
 ------------------------
 
 .. list-table::
@@ -397,15 +404,15 @@
      - snowflake
    * - Microsoft SQL Server
      - mssql
 
 
 Development Environment Setup
 -----------------------------
-* For live installation execute `pip install -e .` and `pip install -r dev-requirements.txt`.
+* For live installation execute `pip install -e ".[dev]"`.
 
 
 Build Wheel Executable
 ----------------------
 * Execute `python -m build`.
 
 Install Wheel Executable File
```

### Comparing `tulona-0.7.6/core/tulona.egg-info/SOURCES.txt` & `tulona-0.7.8/core/tulona.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 core/tulona/adapter/snowflake.py
 core/tulona/adapter/base/connection.py
 core/tulona/cli/base.py
 core/tulona/cli/params.py
 core/tulona/config/__init__.py
 core/tulona/config/profile.py
 core/tulona/config/project.py
-core/tulona/config/runtime.py
 core/tulona/task/base.py
 core/tulona/task/compare.py
 core/tulona/task/helper.py
 core/tulona/task/ping.py
 core/tulona/task/profile.py
 core/tulona/task/scan.py
 core/tulona/util/__init__.py
```

### Comparing `tulona-0.7.6/pyproject.toml` & `tulona-0.7.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tulona"
-version = "0.7.6"
+version = "0.7.8"
 description = "A tool to compare data from different sources."
 dependencies = [
   "click~=8.1",
   "ruamel.yaml~=0.18",
   "psycopg2-binary~=2.9",
   "pymysql~=1.1",
   "cryptography~=42.0",
@@ -35,14 +35,28 @@
   "tulona",
   "comparison",
   "data comparison",
   "database scan",
   "database profile",
 ]
 
+[project.optional-dependencies]
+dev = [
+  "pytest",
+  "flake8",
+  "coverage",
+  "black",
+  "isort",
+  "pytest-cov",
+  "faker",
+  "bump-my-version",
+  "build",
+  "twine",
+]
+
 [project.scripts]
 tulona = "tulona.cli.base:cli"
 
 [project.urls]
 Homepage = "https://github.com/mrinalsardar/tulona"
 Documentation = "https://github.com/mrinalsardar/tulona"
 Repository = "https://github.com/mrinalsardar/tulona.git"
@@ -111,15 +125,15 @@
 
 [tool.isort]
 profile = "black"
 line_length = 90
 skip = [".gitignore"]
 
 [tool.bumpversion]
-current_version = "0.7.6"
+current_version = "0.7.8"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
 ignore_missing_version = false
 tag = false
```

