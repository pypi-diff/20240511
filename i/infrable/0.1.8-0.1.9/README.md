# Comparing `tmp/infrable-0.1.8.tar.gz` & `tmp/infrable-0.1.9.tar.gz`

## Comparing `infrable-0.1.8.tar` & `infrable-0.1.9.tar`

### file list

```diff
@@ -1,53 +1,52 @@
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 infrable-0.1.8/.envrc
--rw-r--r--   0        0        0    17796 2020-02-02 00:00:00.000000 infrable-0.1.8/.null-ls_425841_README.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 infrable-0.1.8/.github/workflows/tests.yml
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 infrable-0.1.8/infrable/__init__.py
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 infrable-0.1.8/infrable/errors.py
--rw-r--r--   0        0        0     9657 2020-02-02 00:00:00.000000 infrable-0.1.8/infrable/files.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 infrable-0.1.8/infrable/host.py
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 infrable-0.1.8/infrable/infra.py
--rw-r--r--   0        0        0     5423 2020-02-02 00:00:00.000000 infrable-0.1.8/infrable/init.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 infrable-0.1.8/infrable/meta.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 infrable-0.1.8/infrable/paths.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 infrable-0.1.8/infrable/readfile.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 infrable-0.1.8/infrable/service.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 infrable-0.1.8/infrable/switch.py
--rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 infrable-0.1.8/infrable/template.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 infrable-0.1.8/infrable/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrable-0.1.8/infrable/cli/__init__.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 infrable-0.1.8/infrable/cli/files.py
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 infrable-0.1.8/infrable/cli/main.py
--rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 infrable-0.1.8/infrable/cli/remote.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 infrable-0.1.8/infrable/cli/switch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrable-0.1.8/infrable/distro/__init__.py
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 infrable-0.1.8/infrable/distro/linux.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 infrable-0.1.8/infrable/distro/ubuntu.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 infrable-0.1.8/tests/data/files_diff
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 infrable-0.1.8/tests/data/hosts
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 infrable-0.1.8/tests/data/hosts_format
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 infrable-0.1.8/tests/data/hosts_repr
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 infrable-0.1.8/tests/data/post_files_gen
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 infrable-0.1.8/tests/data/post_init
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 infrable-0.1.8/tests/data/pre_files_gen
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 infrable-0.1.8/tests/data/pre_init
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 infrable-0.1.8/tests/data/services
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 infrable-0.1.8/tests/data/services_format
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 infrable-0.1.8/tests/data/services_repr
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 infrable-0.1.8/tests/data/switches
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 infrable-0.1.8/tests/data/switches_format
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 infrable-0.1.8/tests/data/switches_repr
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 infrable-0.1.8/tests/functional/test_custom_module.py
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 infrable-0.1.8/tests/functional/test_files.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 infrable-0.1.8/tests/functional/test_hosts.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 infrable-0.1.8/tests/functional/test_init.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 infrable-0.1.8/tests/functional/test_remote.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 infrable-0.1.8/tests/functional/test_services.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 infrable-0.1.8/tests/functional/test_switch.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 infrable-0.1.8/tests/functional/test_switches.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 infrable-0.1.8/tests/functional/test_tasks.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 infrable-0.1.8/tests/functional/test_workflows.py
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 infrable-0.1.8/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 infrable-0.1.8/LICENSE
--rw-r--r--   0        0        0    17796 2020-02-02 00:00:00.000000 infrable-0.1.8/README.md
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 infrable-0.1.8/pyproject.toml
--rw-r--r--   0        0        0    31622 2020-02-02 00:00:00.000000 infrable-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 infrable-0.1.9/.envrc
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 infrable-0.1.9/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 infrable-0.1.9/infrable/__init__.py
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 infrable-0.1.9/infrable/errors.py
+-rw-r--r--   0        0        0     9657 2020-02-02 00:00:00.000000 infrable-0.1.9/infrable/files.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 infrable-0.1.9/infrable/host.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 infrable-0.1.9/infrable/infra.py
+-rw-r--r--   0        0        0     5423 2020-02-02 00:00:00.000000 infrable-0.1.9/infrable/init.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 infrable-0.1.9/infrable/meta.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 infrable-0.1.9/infrable/paths.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 infrable-0.1.9/infrable/readfile.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 infrable-0.1.9/infrable/service.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 infrable-0.1.9/infrable/switch.py
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 infrable-0.1.9/infrable/template.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 infrable-0.1.9/infrable/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrable-0.1.9/infrable/cli/__init__.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 infrable-0.1.9/infrable/cli/files.py
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 infrable-0.1.9/infrable/cli/main.py
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 infrable-0.1.9/infrable/cli/remote.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 infrable-0.1.9/infrable/cli/switch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrable-0.1.9/infrable/distro/__init__.py
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 infrable-0.1.9/infrable/distro/linux.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 infrable-0.1.9/infrable/distro/ubuntu.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 infrable-0.1.9/tests/data/files_diff
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 infrable-0.1.9/tests/data/hosts
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 infrable-0.1.9/tests/data/hosts_format
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 infrable-0.1.9/tests/data/hosts_repr
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 infrable-0.1.9/tests/data/post_files_gen
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 infrable-0.1.9/tests/data/post_init
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 infrable-0.1.9/tests/data/pre_files_gen
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 infrable-0.1.9/tests/data/pre_init
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 infrable-0.1.9/tests/data/services
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 infrable-0.1.9/tests/data/services_format
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 infrable-0.1.9/tests/data/services_repr
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 infrable-0.1.9/tests/data/switches
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 infrable-0.1.9/tests/data/switches_format
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 infrable-0.1.9/tests/data/switches_repr
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 infrable-0.1.9/tests/functional/test_custom_module.py
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 infrable-0.1.9/tests/functional/test_files.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 infrable-0.1.9/tests/functional/test_hosts.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 infrable-0.1.9/tests/functional/test_init.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 infrable-0.1.9/tests/functional/test_remote.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 infrable-0.1.9/tests/functional/test_services.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 infrable-0.1.9/tests/functional/test_switch.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 infrable-0.1.9/tests/functional/test_switches.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 infrable-0.1.9/tests/functional/test_tasks.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 infrable-0.1.9/tests/functional/test_workflows.py
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 infrable-0.1.9/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 infrable-0.1.9/LICENSE
+-rw-r--r--   0        0        0    17886 2020-02-02 00:00:00.000000 infrable-0.1.9/README.md
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 infrable-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    31712 2020-02-02 00:00:00.000000 infrable-0.1.9/PKG-INFO
```

### Comparing `infrable-0.1.8/.null-ls_425841_README.md` & `infrable-0.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -338,17 +338,17 @@
 
 environments = {dev, beta, prod}
 env = Switch(environments, init=dev)  # <-- Defining a switch for different environments
 current_env = env()
 # /Environments ----------------------------------------------------------------
 
 # Hosts/ -----------------------------------------------------------------------
-dev_host = Host(fqdn="dev.example.com", ip="127.0.0.2")
-beta_host = Host(fqdn="beta.example.com", ip="127.0.0.3")
-prod_host = Host(fqdn="prod.example.com", ip="127.0.0.4")
+dev_host = Host(fqdn="dev.example.com", ip="127.0.0.1")
+beta_host = Host(fqdn="beta.example.com", ip="127.0.0.2")
+prod_host = Host(fqdn="prod.example.com", ip="127.0.0.3")
 
 managed_hosts = env(  # <-- Switching hosts based on the environment
     dev=[dev_host],
     beta=[beta_host],
     prod=[prod_host],
 )
 # /Hosts -----------------------------------------------------------------------
@@ -387,14 +387,17 @@
 
 Managing switches:
 
 ```bash
 # Switch current environment
 infrable switch env [dev|beta|prod]
 
+# If you name a switch "env", you get an alias for convenience
+infra env [dev|beta|prod]
+
 # Check all switch values
 infrable switches
 ```
 
 ## Chapter 7 - Meta and Secrets
 
 A veil of mystery cloaked Hanny's latest quest. She coveted the ability to access **secret
```

### Comparing `infrable-0.1.8/.github/workflows/tests.yml` & `infrable-0.1.9/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `infrable-0.1.8/infrable/__init__.py` & `infrable-0.1.9/infrable/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 
 
 from pathlib import Path
 
 INFRA_MODULE_NAME = "infra"
 IS_PROJECT_DIR = Path(f"{INFRA_MODULE_NAME}.py").exists()
```

### Comparing `infrable-0.1.8/infrable/errors.py` & `infrable-0.1.9/infrable/errors.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.8/infrable/files.py` & `infrable-0.1.9/infrable/files.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.8/infrable/host.py` & `infrable-0.1.9/infrable/host.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.8/infrable/infra.py` & `infrable-0.1.9/infrable/infra.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.8/infrable/init.py` & `infrable-0.1.9/infrable/init.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.8/infrable/readfile.py` & `infrable-0.1.9/infrable/readfile.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.8/infrable/service.py` & `infrable-0.1.9/infrable/service.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.8/infrable/switch.py` & `infrable-0.1.9/infrable/switch.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.8/infrable/template.py` & `infrable-0.1.9/infrable/template.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.8/infrable/utils.py` & `infrable-0.1.9/infrable/utils.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.8/infrable/cli/files.py` & `infrable-0.1.9/infrable/cli/files.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.8/infrable/cli/main.py` & `infrable-0.1.9/infrable/cli/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import typer
+from click import Choice
 
 app = typer.Typer(no_args_is_help=True)
 
 from infrable import IS_PROJECT_DIR, __version__, init
 
 
 @app.command()
@@ -59,7 +60,15 @@
 
     app.add_typer(files.app, name="files", help="Manage files.")
     app.add_typer(switch.app, name="switch", help="Manage switches.")
     app.add_typer(remote.app, name="remote", help="Execute remote commands.")
 
     for name, ext in infra.typers.items():
         app.add_typer(ext, name=name.replace("_", "-"))
+
+    if sw := infra.switches.get("env"):
+        # Alias for 'infrable switch env'
+        def env(value: str = typer.Argument(..., click_type=Choice(list(sw.options)))):
+            """Alias for `infrable switch env`."""
+            sw.set(value)
+
+        app.command()(env)
```

### Comparing `infrable-0.1.8/infrable/cli/remote.py` & `infrable-0.1.9/infrable/cli/remote.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.8/infrable/distro/linux.py` & `infrable-0.1.9/infrable/distro/linux.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.8/infrable/distro/ubuntu.py` & `infrable-0.1.9/infrable/distro/ubuntu.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.8/tests/data/files_diff` & `infrable-0.1.9/tests/data/files_diff`

 * *Files identical despite different names*

### Comparing `infrable-0.1.8/tests/functional/test_files.py` & `infrable-0.1.9/tests/functional/test_files.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.8/tests/functional/test_hosts.py` & `infrable-0.1.9/tests/functional/test_hosts.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.8/tests/functional/test_services.py` & `infrable-0.1.9/tests/functional/test_services.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.8/tests/functional/test_switches.py` & `infrable-0.1.9/tests/functional/test_switches.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.8/.gitignore` & `infrable-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `infrable-0.1.8/LICENSE` & `infrable-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `infrable-0.1.8/pyproject.toml` & `infrable-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `infrable-0.1.8/PKG-INFO` & `infrable-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: infrable
-Version: 0.1.8
+Version: 0.1.9
 Summary: Hanny's legendary infrastructure as code solution.
 Project-URL: Homepage, https://github.com/stckme/infrable
 Author-email: Arijit Basu <sayanarijit@gmail.com>
 Maintainer-email: Arijit Basu <sayanarijit@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -615,14 +615,17 @@
 
 Managing switches:
 
 ```bash
 # Switch current environment
 infrable switch env [dev|beta|prod]
 
+# If you name a switch "env", you get an alias for convenience
+infra env [dev|beta|prod]
+
 # Check all switch values
 infrable switches
 ```
 
 ## Chapter 7 - Meta and Secrets
 
 A veil of mystery cloaked Hanny's latest quest. She coveted the ability to access **secret
```

