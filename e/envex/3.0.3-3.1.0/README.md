# Comparing `tmp/envex-3.0.3.tar.gz` & `tmp/envex-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envex-3.0.3.tar", max compression
+gzip compressed data, was "envex-3.1.0.tar", max compression
```

## Comparing `envex-3.0.3.tar` & `envex-3.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1084 2024-01-10 01:25:45.520651 envex-3.0.3/LICENSE.md
--rw-r--r--   0        0        0     8453 2024-01-10 01:25:45.520651 envex-3.0.3/README.md
--rw-r--r--   0        0        0      173 2024-01-10 01:25:45.520651 envex-3.0.3/envex/__init__.py
--rw-r--r--   0        0        0     7836 2024-01-10 01:25:45.520651 envex-3.0.3/envex/dot_env.py
--rw-r--r--   0        0        0     7860 2024-01-10 01:25:45.520651 envex-3.0.3/envex/env_hvac.py
--rw-r--r--   0        0        0     9305 2024-01-10 01:25:45.520651 envex-3.0.3/envex/env_wrapper.py
--rw-r--r--   0        0        0      920 2024-01-10 01:25:45.520651 envex-3.0.3/pyproject.toml
--rw-r--r--   0        0        0     8993 1970-01-01 00:00:00.000000 envex-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-05-11 07:36:50.617055 envex-3.1.0/LICENSE.md
+-rw-r--r--   0        0        0     8453 2024-05-11 07:36:50.617055 envex-3.1.0/README.md
+-rw-r--r--   0        0        0      173 2024-05-11 07:36:50.617055 envex-3.1.0/envex/__init__.py
+-rw-r--r--   0        0        0     7836 2024-05-11 07:36:50.617055 envex-3.1.0/envex/dot_env.py
+-rw-r--r--   0        0        0     8352 2024-05-11 07:36:50.617055 envex-3.1.0/envex/env_hvac.py
+-rw-r--r--   0        0        0     9512 2024-05-11 07:36:50.617055 envex-3.1.0/envex/env_wrapper.py
+-rw-r--r--   0        0        0      929 2024-05-11 07:36:50.617055 envex-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8997 1970-01-01 00:00:00.000000 envex-3.1.0/PKG-INFO
```

### Comparing `envex-3.0.3/LICENSE.md` & `envex-3.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `envex-3.0.3/README.md` & `envex-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `envex-3.0.3/envex/dot_env.py` & `envex-3.1.0/envex/dot_env.py`

 * *Files identical despite different names*

### Comparing `envex-3.0.3/envex/env_hvac.py` & `envex-3.1.0/envex/env_hvac.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 This optional module is used to interface envex with the hvac (Hashicorp Vault) library.
 """
 import logging
 import os
-import sys
 from typing import Iterator
 
 __all__ = ("SecretsManager",)
 
 
 def expand(path: str):
     return os.path.expandvars(os.path.expanduser(path))
@@ -30,23 +29,26 @@
                 value = f.read()
                 intro = "PRIVATE KEY" if is_key else "BEGIN CERTIFICATE"
                 value = value if intro in value else None
     return value
 
 
 class SecretsManager:
+    hvac_disabled = False
+
     def __init__(
         self,
         url: str = None,
         token: str = None,
         cert=None,
         verify: bool | str = True,
         base_path: str = None,
         engine: str | None = None,
         mount_point: str | None = None,
+        timeout: int | None = None,
         **kwargs,
     ):
         """
         Initialises a Vault object with the given parameters.
 
         Parameters:
         :param url (str): Base URL for the Vault instance being addressed.
@@ -75,36 +77,48 @@
             )
             if cert[0] is None:
                 cert = None
         if base_path is None:
             base_path = os.getenv("VAULT_PATH", "")
         if not mount_point:
             mount_point = "secret"
-        # noinspection PyBroadException
-        try:
-            import hvac
-
-            self._client: hvac.Client
-            self._client = hvac.Client(url=url, token=token, cert=cert, verify=verify, **kwargs)
-            if engine:
-                self._engine = engine.lower()
-                response = self._client.sys.list_mounted_secrets_engines()
-                for path, config in response["data"].items():
-                    if config["type"] == self._engine:
-                        mount_point = path
-                        break
-            else:
-                self._engine = None  # assume kv
-        except Exception as e:
-            msg = f"{e.__class__.__name__} secrets manager disabled: {e}"
-            logging.debug(msg)
-            print(msg, file=sys.stderr)
-            # noinspection PyUnusedLocal
-            hvac = None
+        if SecretsManager.hvac_disabled:
             self._client = None
+        else:
+            # noinspection PyBroadException
+            try:
+                import hvac
+
+                timeout = timeout or int(os.getenv("VAULT_TIMEOUT", "5"))
+
+                self._client: hvac.Client
+                self._client = hvac.Client(
+                    url=url,
+                    token=token,
+                    cert=cert,
+                    verify=verify,
+                    timeout=timeout,
+                    **kwargs,
+                )
+                if engine:
+                    self._engine = engine.lower()
+                    response = self._client.sys.list_mounted_secrets_engines()
+                    for path, config in response["data"].items():
+                        if config["type"] == self._engine:
+                            mount_point = path
+                            break
+                else:
+                    self._engine = None  # assume kv
+            except Exception as e:
+                msg = f"{e.__class__.__name__} secrets manager disabled: {e}"
+                logging.debug(msg)
+                SecretsManager.hvac_disabled = True
+                # noinspection PyUnusedLocal
+                hvac = None
+                self._client = None
         self._mount_point = self.join(mount_point, "data")
         self._base_path = self.join(self._mount_point, base_path)
         self._secrets = {}
 
     @staticmethod
     def join(*args, sep="/"):
         return sep.join([a for a in args if a])
@@ -119,15 +133,17 @@
     @property
     def client(self):
         # returns hvac.Client | None
         try:
             if self._client.is_authenticated():
                 return self._client
         except Exception as exc:
-            logging.debug(f"{exc.__class__.__name__} Vault client cannot authenticate {exc}")
+            logging.debug(
+                f"{exc.__class__.__name__} Vault client cannot authenticate {exc}"
+            )
 
     @property
     def secrets(self) -> dict:
         return self._secrets
 
     def get_secrets(self, path: str = "") -> dict:
         if self.client:
```

### Comparing `envex-3.0.3/envex/env_wrapper.py` & `envex-3.1.0/envex/env_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,15 @@
             url=url,
             token=token,
             cert=cert,
             verify=verify,
             base_path=base_path,
             engine=engine,
             mount_point=mount_point,
+            timeout=kwargs.get("timeout", None),
         )
         self.exception = exception or self._EXCEPTION_CLS
 
     @staticmethod
     def os_env():
         import os
 
@@ -197,15 +198,17 @@
         return self.get(var, default)
 
     def export(self, *args, **kwargs):
         import os
 
         for arg in args:
             if not isinstance(arg, (dict,)):
-                raise TypeError("export() requires either dictionaries or keyword=value pairs")
+                raise TypeError(
+                    "export() requires either dictionaries or keyword=value pairs"
+                )
             kwargs |= {k: v for k, v in arg.items()}
         if not args and not kwargs:
             kwargs = self.env
         for k, v in kwargs.items():
             k = str(k)
             try:
                 if v is None:
@@ -215,36 +218,46 @@
                     self.set(k, v)
                     os.environ[k] = str(v)
             except KeyError:
                 ...
 
     @classmethod
     def _true_values(cls, val):
-        return cls._BOOLEAN_TRUE_STRINGS if isinstance(val, str) else cls._BOOLEAN_TRUE_BYTES
+        return (
+            cls._BOOLEAN_TRUE_STRINGS
+            if isinstance(val, str)
+            else cls._BOOLEAN_TRUE_BYTES
+        )
 
     @classmethod
     def is_true(cls, val):
         if val in (None, False, "", 0, "0"):
             return False
         if not isinstance(val, (str, bytes)):
             return bool(val)
         true_vals = cls._true_values(val)
         return True if val and any([val.startswith(v) for v in true_vals]) else False
 
     @classmethod
     def _int(cls, val):
-        return val if isinstance(val, int) else int(val) if val and str.isdigit(val) else 0
+        return (
+            val if isinstance(val, int) else int(val) if val and str.isdigit(val) else 0
+        )
 
     @classmethod
     def _float(cls, val):
         return val if isinstance(val, float) else float(val) if val else 0
 
     @classmethod
     def _list(cls, val):
-        return [] if val is None else [unquote(part) for part in re.split(r"\s*,\s*", str(val))]
+        return (
+            []
+            if val is None
+            else [unquote(part) for part in re.split(r"\s*,\s*", str(val))]
+        )
 
     def __contains__(self, var):
         return self.get(var, None) is not None
 
     def __setitem__(self, var: str, value: Any):
         self.set(var, value)
```

### Comparing `envex-3.0.3/pyproject.toml` & `envex-3.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 [tool.poetry]
 name = "envex"
-version = "3.0.3"
+version = "3.1.0"
 description = "Environment interface with .env and hashicorp vault support"
 authors = ["David Nugent <davidn@uniquode.io>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Framework :: Django",
     "Programming Language :: Python :: 3",
 ]
 
 [tool.poetry.dependencies]
-python = ">= 3.10, < 4.0"
+python = ">=3.10.0,<4.0.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.7.0"
-isort = "^5.12.0"
-ruff = "^0.0.285"
-pre-commit = "^3.3.3"
+ruff = ">= 0.4.4"
+pre-commit = ">= 3.7"
 
 [tool.poetry.group.test.dependencies]
 pytest = ">=7.0"
 pytest-mock = "^3.11.1"
 pytest-cov = "^4.1.0"
 
 [tool.poetry.group.vault.dependencies]
 hvac = ">= 1.1.1"
 
 [tool.poetry.scripts]
 env2hvac = "scripts.env2hvac:main"
 envsecrets = "scripts.envsecrets:main"
 seal = "scripts.seal:main"
 
+[tool.ruff]
+namespace-packages = ["envex"]
+
 [tool.pytest.ini_options]
 minversion = "7.0"
 pythonpath = ["."]
 testpaths = ["tests"]
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `envex-3.0.3/PKG-INFO` & `envex-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: envex
-Version: 3.0.3
+Version: 3.1.0
 Summary: Environment interface with .env and hashicorp vault support
 License: MIT
 Author: David Nugent
 Author-email: davidn@uniquode.io
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10.0,<4.0.0
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
```

