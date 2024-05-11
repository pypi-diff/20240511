# Comparing `tmp/fastapi_mctools-0.4.0.tar.gz` & `tmp/fastapi_mctools-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_mctools-0.4.0.tar", max compression
+gzip compressed data, was "fastapi_mctools-0.4.1.tar", max compression
```

## Comparing `fastapi_mctools-0.4.0.tar` & `fastapi_mctools-0.4.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1072 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/LICENSE
--rw-r--r--   0        0        0     8669 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/README.md
--rw-r--r--   0        0        0        0 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/fastapi_mctools/__init__.py
--rw-r--r--   0        0        0        0 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/fastapi_mctools/aws/__init__.py
--rw-r--r--   0        0        0     2155 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/fastapi_mctools/aws/s3.py
--rw-r--r--   0        0        0      230 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/fastapi_mctools/cache/__init__.py
--rw-r--r--   0        0        0     1400 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/fastapi_mctools/cache/base.py
--rw-r--r--   0        0        0     2747 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/fastapi_mctools/cache/memory.py
--rw-r--r--   0        0        0     1807 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/fastapi_mctools/cache/redis.py
--rw-r--r--   0        0        0        0 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/fastapi_mctools/commands/__init__.py
--rw-r--r--   0        0        0      127 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/fastapi_mctools/commands/_templates/async_session.py-tpl
--rw-r--r--   0        0        0     3293 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/fastapi_mctools/commands/_templates/gitignore-tpl
--rw-r--r--   0        0        0      266 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/fastapi_mctools/commands/_templates/gunicorn.config.py-tpl
--rw-r--r--   0        0        0       46 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/fastapi_mctools/commands/_templates/main.py-tpl
--rw-r--r--   0        0        0      455 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/fastapi_mctools/commands/_templates/pre-commit-tpl
--rw-r--r--   0        0        0       53 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/fastapi_mctools/commands/_templates/routers.py-tpl
--rw-r--r--   0        0        0      578 2024-04-13 06:43:32.541092 fastapi_mctools-0.4.0/fastapi_mctools/commands/_templates/session.py-tpl
--rw-r--r--   0        0        0     2256 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/commands/_templates/settings.py-tpl
--rw-r--r--   0        0        0       82 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/commands/_templates/sqlalchemy_base.py-tpl
--rw-r--r--   0        0        0      500 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/commands/gunicorn.py
--rw-r--r--   0        0        0      675 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/commands/main.py
--rw-r--r--   0        0        0     2031 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/commands/run.py
--rw-r--r--   0        0        0      803 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/commands/shell.py
--rw-r--r--   0        0        0     1525 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/commands/startproject.py
--rw-r--r--   0        0        0     2313 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/commands/types.py
--rw-r--r--   0        0        0        0 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/db/__init__.py
--rw-r--r--   0        0        0     1617 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/db/sqlalchemy.py
--rw-r--r--   0        0        0     2297 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/dependencies.py
--rw-r--r--   0        0        0     1650 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/middlewares/__init__.py
--rw-r--r--   0        0        0     6828 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/middlewares/logging.py
--rw-r--r--   0        0        0     1173 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/middlewares/trustedhost.py
--rw-r--r--   0        0        0     2306 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/orms/__init__.py
--rw-r--r--   0        0        0        0 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/orms/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     3957 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/orms/sqlalchemy/async_base.py
--rw-r--r--   0        0        0     2507 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/orms/sqlalchemy/filters.py
--rw-r--r--   0        0        0     3404 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/orms/sqlalchemy/sync_base.py
--rw-r--r--   0        0        0        0 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/test_tools/__init__.py
--rw-r--r--   0        0        0     1964 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/test_tools/db_managers.py
--rw-r--r--   0        0        0        0 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/utils/__init__.py
--rw-r--r--   0        0        0     2805 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/utils/requests.py
--rw-r--r--   0        0        0     1277 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/utils/responses.py
--rw-r--r--   0        0        0     1625 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/fastapi_mctools/utils/time.py
--rw-r--r--   0        0        0     1029 2024-04-13 06:43:32.545092 fastapi_mctools-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     9476 1970-01-01 00:00:00.000000 fastapi_mctools-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-11 14:21:48.671138 fastapi_mctools-0.4.1/LICENSE
+-rw-r--r--   0        0        0     8747 2024-05-11 14:21:48.671138 fastapi_mctools-0.4.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-11 14:21:48.671138 fastapi_mctools-0.4.1/fastapi_mctools/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-11 14:21:48.671138 fastapi_mctools-0.4.1/fastapi_mctools/aws/__init__.py
+-rw-r--r--   0        0        0     2155 2024-05-11 14:21:48.671138 fastapi_mctools-0.4.1/fastapi_mctools/aws/s3.py
+-rw-r--r--   0        0        0      230 2024-05-11 14:21:48.671138 fastapi_mctools-0.4.1/fastapi_mctools/cache/__init__.py
+-rw-r--r--   0        0        0     1400 2024-05-11 14:21:48.671138 fastapi_mctools-0.4.1/fastapi_mctools/cache/base.py
+-rw-r--r--   0        0        0     2747 2024-05-11 14:21:48.671138 fastapi_mctools-0.4.1/fastapi_mctools/cache/memory.py
+-rw-r--r--   0        0        0     1807 2024-05-11 14:21:48.671138 fastapi_mctools-0.4.1/fastapi_mctools/cache/redis.py
+-rw-r--r--   0        0        0        0 2024-05-11 14:21:48.671138 fastapi_mctools-0.4.1/fastapi_mctools/commands/__init__.py
+-rw-r--r--   0        0        0      127 2024-05-11 14:21:48.671138 fastapi_mctools-0.4.1/fastapi_mctools/commands/_templates/async_session.py-tpl
+-rw-r--r--   0        0        0     3293 2024-05-11 14:21:48.671138 fastapi_mctools-0.4.1/fastapi_mctools/commands/_templates/gitignore-tpl
+-rw-r--r--   0        0        0      266 2024-05-11 14:21:48.671138 fastapi_mctools-0.4.1/fastapi_mctools/commands/_templates/gunicorn.config.py-tpl
+-rw-r--r--   0        0        0       46 2024-05-11 14:21:48.671138 fastapi_mctools-0.4.1/fastapi_mctools/commands/_templates/main.py-tpl
+-rw-r--r--   0        0        0      455 2024-05-11 14:21:48.671138 fastapi_mctools-0.4.1/fastapi_mctools/commands/_templates/pre-commit-tpl
+-rw-r--r--   0        0        0       53 2024-05-11 14:21:48.671138 fastapi_mctools-0.4.1/fastapi_mctools/commands/_templates/routers.py-tpl
+-rw-r--r--   0        0        0      578 2024-05-11 14:21:48.671138 fastapi_mctools-0.4.1/fastapi_mctools/commands/_templates/session.py-tpl
+-rw-r--r--   0        0        0     2256 2024-05-11 14:21:48.675138 fastapi_mctools-0.4.1/fastapi_mctools/commands/_templates/settings.py-tpl
+-rw-r--r--   0        0        0       82 2024-05-11 14:21:48.675138 fastapi_mctools-0.4.1/fastapi_mctools/commands/_templates/sqlalchemy_base.py-tpl
+-rw-r--r--   0        0        0      500 2024-05-11 14:21:48.675138 fastapi_mctools-0.4.1/fastapi_mctools/commands/gunicorn.py
+-rw-r--r--   0        0        0      675 2024-05-11 14:21:48.675138 fastapi_mctools-0.4.1/fastapi_mctools/commands/main.py
+-rw-r--r--   0        0        0     2031 2024-05-11 14:21:48.675138 fastapi_mctools-0.4.1/fastapi_mctools/commands/run.py
+-rw-r--r--   0        0        0      803 2024-05-11 14:21:48.675138 fastapi_mctools-0.4.1/fastapi_mctools/commands/shell.py
+-rw-r--r--   0        0        0     1525 2024-05-11 14:21:48.675138 fastapi_mctools-0.4.1/fastapi_mctools/commands/startproject.py
+-rw-r--r--   0        0        0     2313 2024-05-11 14:21:48.675138 fastapi_mctools-0.4.1/fastapi_mctools/commands/types.py
+-rw-r--r--   0        0        0        0 2024-05-11 14:21:48.675138 fastapi_mctools-0.4.1/fastapi_mctools/db/__init__.py
+-rw-r--r--   0        0        0     1617 2024-05-11 14:21:48.675138 fastapi_mctools-0.4.1/fastapi_mctools/db/sqlalchemy.py
+-rw-r--r--   0        0        0     2574 2024-05-11 14:21:48.675138 fastapi_mctools-0.4.1/fastapi_mctools/dependencies.py
+-rw-r--r--   0        0        0     1650 2024-05-11 14:21:48.675138 fastapi_mctools-0.4.1/fastapi_mctools/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-11 14:21:48.675138 fastapi_mctools-0.4.1/fastapi_mctools/middlewares/__init__.py
+-rw-r--r--   0        0        0     6828 2024-05-11 14:21:48.675138 fastapi_mctools-0.4.1/fastapi_mctools/middlewares/logging.py
+-rw-r--r--   0        0        0     1173 2024-05-11 14:21:48.675138 fastapi_mctools-0.4.1/fastapi_mctools/middlewares/trustedhost.py
+-rw-r--r--   0        0        0     2306 2024-05-11 14:21:48.675138 fastapi_mctools-0.4.1/fastapi_mctools/orms/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-11 14:21:48.675138 fastapi_mctools-0.4.1/fastapi_mctools/orms/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     3957 2024-05-11 14:21:48.675138 fastapi_mctools-0.4.1/fastapi_mctools/orms/sqlalchemy/async_base.py
+-rw-r--r--   0        0        0     2507 2024-05-11 14:21:48.675138 fastapi_mctools-0.4.1/fastapi_mctools/orms/sqlalchemy/filters.py
+-rw-r--r--   0        0        0     3404 2024-05-11 14:21:48.675138 fastapi_mctools-0.4.1/fastapi_mctools/orms/sqlalchemy/sync_base.py
+-rw-r--r--   0        0        0        0 2024-05-11 14:21:48.675138 fastapi_mctools-0.4.1/fastapi_mctools/test_tools/__init__.py
+-rw-r--r--   0        0        0     1964 2024-05-11 14:21:48.675138 fastapi_mctools-0.4.1/fastapi_mctools/test_tools/db_managers.py
+-rw-r--r--   0        0        0        0 2024-05-11 14:21:48.675138 fastapi_mctools-0.4.1/fastapi_mctools/utils/__init__.py
+-rw-r--r--   0        0        0     2805 2024-05-11 14:21:48.675138 fastapi_mctools-0.4.1/fastapi_mctools/utils/requests.py
+-rw-r--r--   0        0        0     1277 2024-05-11 14:21:48.675138 fastapi_mctools-0.4.1/fastapi_mctools/utils/responses.py
+-rw-r--r--   0        0        0     1625 2024-05-11 14:21:48.675138 fastapi_mctools-0.4.1/fastapi_mctools/utils/time.py
+-rw-r--r--   0        0        0     1029 2024-05-11 14:21:48.675138 fastapi_mctools-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     9554 1970-01-01 00:00:00.000000 fastapi_mctools-0.4.1/PKG-INFO
```

### Comparing `fastapi_mctools-0.4.0/LICENSE` & `fastapi_mctools-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.4.0/README.md` & `fastapi_mctools-0.4.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -212,23 +212,23 @@
     TempDep2=temp_dep_2,
     TempDep3=temp_dep_3
 )
 
 # in your route
 
 @app.get('/temp_1')
-async def temp_1(result: temp_dep.TempDep1):
+async def temp_1(result: temp_dep.TempDep1): # temp_dep[0] is possible
     return result
 
 @app.get('/temp_2')
-async def temp_2(result: temp_dep.TempDep2):
+async def temp_2(result: temp_dep.TempDep2): # temp_dep[1] is possible
     return result
 
 @app.get('/temp_3')
-async def temp_3(result: temp_dep.TempDep3):
+async def temp_3(result: temp_dep.TempDep3): # temp_dep[2] is possible
     return result
 
 ```
 
 - create_simple_form_dependency
 - this is developed to avoid the tedious task of repeatedly writing out the Form.
 - especially when you make api with file upload, you can use this to make it simple
```

### Comparing `fastapi_mctools-0.4.0/fastapi_mctools/aws/s3.py` & `fastapi_mctools-0.4.1/fastapi_mctools/aws/s3.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.4.0/fastapi_mctools/cache/base.py` & `fastapi_mctools-0.4.1/fastapi_mctools/cache/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.4.0/fastapi_mctools/cache/memory.py` & `fastapi_mctools-0.4.1/fastapi_mctools/cache/memory.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.4.0/fastapi_mctools/cache/redis.py` & `fastapi_mctools-0.4.1/fastapi_mctools/cache/redis.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.4.0/fastapi_mctools/commands/_templates/gitignore-tpl` & `fastapi_mctools-0.4.1/fastapi_mctools/commands/_templates/gitignore-tpl`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.4.0/fastapi_mctools/commands/_templates/session.py-tpl` & `fastapi_mctools-0.4.1/fastapi_mctools/commands/_templates/session.py-tpl`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.4.0/fastapi_mctools/commands/_templates/settings.py-tpl` & `fastapi_mctools-0.4.1/fastapi_mctools/commands/_templates/settings.py-tpl`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.4.0/fastapi_mctools/commands/main.py` & `fastapi_mctools-0.4.1/fastapi_mctools/commands/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.4.0/fastapi_mctools/commands/run.py` & `fastapi_mctools-0.4.1/fastapi_mctools/commands/run.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.4.0/fastapi_mctools/commands/shell.py` & `fastapi_mctools-0.4.1/fastapi_mctools/commands/shell.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.4.0/fastapi_mctools/commands/startproject.py` & `fastapi_mctools-0.4.1/fastapi_mctools/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.4.0/fastapi_mctools/commands/types.py` & `fastapi_mctools-0.4.1/fastapi_mctools/commands/types.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.4.0/fastapi_mctools/db/sqlalchemy.py` & `fastapi_mctools-0.4.1/fastapi_mctools/db/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.4.0/fastapi_mctools/dependencies.py` & `fastapi_mctools-0.4.1/fastapi_mctools/dependencies.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,21 @@
             if not value.__annotations__.get("return"):
                 raise AttributeError(f"{value}에 반환값 annotation이 없습니다.")
 
             return_type = value.__annotations__.get("return")
             value = Annotated[return_type, Depends(value)]
             setattr(self, key, value)
 
+    def __getitem__(self, index: int) -> Annotated:
+        try:
+            values = list(self.__dict__.values())[index]
+            return values
+        except IndexError:
+            raise IndexError(f"{self.__class__.__name__} has only {len(self.__dict__)} dependency.")
+
 
 def create_simple_form_dependency(input_dict: dict) -> type:
     """
     Creates a class for using FastAPI's Form.
     Developed to avoid the tedious task of repeatedly writing out the Form.
     It can be used as a class dependency.
```

### Comparing `fastapi_mctools-0.4.0/fastapi_mctools/exceptions.py` & `fastapi_mctools-0.4.1/fastapi_mctools/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.4.0/fastapi_mctools/middlewares/logging.py` & `fastapi_mctools-0.4.1/fastapi_mctools/middlewares/logging.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.4.0/fastapi_mctools/middlewares/trustedhost.py` & `fastapi_mctools-0.4.1/fastapi_mctools/middlewares/trustedhost.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.4.0/fastapi_mctools/orms/__init__.py` & `fastapi_mctools-0.4.1/fastapi_mctools/orms/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.4.0/fastapi_mctools/orms/sqlalchemy/async_base.py` & `fastapi_mctools-0.4.1/fastapi_mctools/orms/sqlalchemy/async_base.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.4.0/fastapi_mctools/orms/sqlalchemy/filters.py` & `fastapi_mctools-0.4.1/fastapi_mctools/orms/sqlalchemy/filters.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.4.0/fastapi_mctools/orms/sqlalchemy/sync_base.py` & `fastapi_mctools-0.4.1/fastapi_mctools/orms/sqlalchemy/sync_base.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.4.0/fastapi_mctools/test_tools/db_managers.py` & `fastapi_mctools-0.4.1/fastapi_mctools/test_tools/db_managers.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.4.0/fastapi_mctools/utils/requests.py` & `fastapi_mctools-0.4.1/fastapi_mctools/utils/requests.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.4.0/fastapi_mctools/utils/responses.py` & `fastapi_mctools-0.4.1/fastapi_mctools/utils/responses.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.4.0/fastapi_mctools/utils/time.py` & `fastapi_mctools-0.4.1/fastapi_mctools/utils/time.py`

 * *Files identical despite different names*

### Comparing `fastapi_mctools-0.4.0/pyproject.toml` & `fastapi_mctools-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-mctools"
-version = "0.4.0"
+version = "0.4.1"
 description = "Fastapi mc style tools to make it easier to develop."
 authors = ["Jungminchae <minchae3618@gmail.com>"]
 readme = "README.md"
 packages = [{include = "fastapi_mctools"}]
 
 [tool.poetry.dependencies]
 python =  ">=3.10,<4.0"
```

### Comparing `fastapi_mctools-0.4.0/PKG-INFO` & `fastapi_mctools-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-mctools
-Version: 0.4.0
+Version: 0.4.1
 Summary: Fastapi mc style tools to make it easier to develop.
 Author: Jungminchae
 Author-email: minchae3618@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -232,23 +232,23 @@
     TempDep2=temp_dep_2,
     TempDep3=temp_dep_3
 )
 
 # in your route
 
 @app.get('/temp_1')
-async def temp_1(result: temp_dep.TempDep1):
+async def temp_1(result: temp_dep.TempDep1): # temp_dep[0] is possible
     return result
 
 @app.get('/temp_2')
-async def temp_2(result: temp_dep.TempDep2):
+async def temp_2(result: temp_dep.TempDep2): # temp_dep[1] is possible
     return result
 
 @app.get('/temp_3')
-async def temp_3(result: temp_dep.TempDep3):
+async def temp_3(result: temp_dep.TempDep3): # temp_dep[2] is possible
     return result
 
 ```
 
 - create_simple_form_dependency
 - this is developed to avoid the tedious task of repeatedly writing out the Form.
 - especially when you make api with file upload, you can use this to make it simple
```

