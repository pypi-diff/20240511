# Comparing `tmp/fastapi-utils-0.2.1.tar.gz` & `tmp/fastapi_utils-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-utils-0.2.1.tar", last modified: Sat Mar  7 05:54:58 2020, max compression
+gzip compressed data, was "fastapi_utils-0.6.0.tar", max compression
```

## Comparing `fastapi-utils-0.2.1.tar` & `fastapi_utils-0.6.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1081 2020-03-07 05:54:12.746268 fastapi-utils-0.2.1/LICENSE
--rw-r--r--   0        0        0     3255 2020-03-07 05:54:12.746268 fastapi-utils-0.2.1/README.md
--rw-r--r--   0        0        0       22 2020-03-07 05:54:12.750268 fastapi-utils-0.2.1/fastapi_utils/__init__.py
--rw-r--r--   0        0        0      858 2020-03-07 05:54:12.750268 fastapi-utils-0.2.1/fastapi_utils/api_model.py
--rw-r--r--   0        0        0     2488 2020-03-07 05:54:12.750268 fastapi-utils-0.2.1/fastapi_utils/api_settings.py
--rw-r--r--   0        0        0      846 2020-03-07 05:54:12.750268 fastapi-utils-0.2.1/fastapi_utils/camelcase.py
--rw-r--r--   0        0        0     4256 2020-03-07 05:54:12.750268 fastapi-utils-0.2.1/fastapi_utils/cbv.py
--rw-r--r--   0        0        0     1199 2020-03-07 05:54:12.750268 fastapi-utils-0.2.1/fastapi_utils/enums.py
--rw-r--r--   0        0        0     2226 2020-03-07 05:54:12.750268 fastapi-utils-0.2.1/fastapi_utils/guid_type.py
--rw-r--r--   0        0        0      608 2020-03-07 05:54:12.750268 fastapi-utils-0.2.1/fastapi_utils/inferring_router.py
--rw-r--r--   0        0        0      331 2020-03-07 05:54:12.750268 fastapi-utils-0.2.1/fastapi_utils/openapi.py
--rw-r--r--   0        0        0        0 2020-03-07 05:54:12.750268 fastapi-utils-0.2.1/fastapi_utils/py.typed
--rw-r--r--   0        0        0     5179 2020-03-07 05:54:12.750268 fastapi-utils-0.2.1/fastapi_utils/session.py
--rw-r--r--   0        0        0     3476 2020-03-07 05:54:12.750268 fastapi-utils-0.2.1/fastapi_utils/tasks.py
--rw-r--r--   0        0        0     6916 2020-03-07 05:54:12.750268 fastapi-utils-0.2.1/fastapi_utils/timing.py
--rw-r--r--   0        0        0     2441 2020-03-07 05:54:12.750268 fastapi-utils-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4027 2020-03-07 05:54:58.962682 fastapi-utils-0.2.1/setup.py
--rw-r--r--   0        0        0     4844 2020-03-07 05:54:58.963118 fastapi-utils-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1093 2024-05-11 14:54:47.551040 fastapi_utils-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3346 2024-05-11 14:54:47.551040 fastapi_utils-0.6.0/README.md
+-rw-r--r--   0        0        0      892 2024-05-11 14:54:47.551040 fastapi_utils-0.6.0/fastapi_utils/__init__.py
+-rw-r--r--   0        0        0     1251 2024-05-11 14:54:47.551040 fastapi_utils-0.6.0/fastapi_utils/api_model.py
+-rw-r--r--   0        0        0     2851 2024-05-11 14:54:47.551040 fastapi_utils-0.6.0/fastapi_utils/api_settings.py
+-rw-r--r--   0        0        0      882 2024-05-07 19:27:14.841761 fastapi_utils-0.6.0/fastapi_utils/camelcase.py
+-rw-r--r--   0        0        0     7261 2024-05-11 14:54:47.551040 fastapi_utils-0.6.0/fastapi_utils/cbv.py
+-rw-r--r--   0        0        0     1045 2024-05-11 14:54:47.551040 fastapi_utils-0.6.0/fastapi_utils/cbv_base.py
+-rw-r--r--   0        0        0     1226 2024-05-11 14:54:47.551040 fastapi_utils-0.6.0/fastapi_utils/enums.py
+-rw-r--r--   0        0        0     2251 2024-05-07 19:27:14.841761 fastapi_utils-0.6.0/fastapi_utils/guid_type.py
+-rw-r--r--   0        0        0      245 2024-05-07 19:27:14.841761 fastapi_utils-0.6.0/fastapi_utils/inferring_router.py
+-rw-r--r--   0        0        0      367 2024-05-07 19:27:14.841761 fastapi_utils-0.6.0/fastapi_utils/openapi.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:27:14.841761 fastapi_utils-0.6.0/fastapi_utils/py.typed
+-rw-r--r--   0        0        0     5205 2024-05-07 19:27:14.841761 fastapi_utils-0.6.0/fastapi_utils/session.py
+-rw-r--r--   0        0        0     3472 2024-05-11 14:54:47.551040 fastapi_utils-0.6.0/fastapi_utils/tasks.py
+-rw-r--r--   0        0        0     7114 2024-05-11 14:54:47.551040 fastapi_utils-0.6.0/fastapi_utils/timing.py
+-rw-r--r--   0        0        0     3739 2024-05-11 14:54:47.551040 fastapi_utils-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     5368 1970-01-01 00:00:00.000000 fastapi_utils-0.6.0/PKG-INFO
```

### Comparing `fastapi-utils-0.2.1/LICENSE` & `fastapi_utils-0.6.0/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2020 David Montague
+Copyright (c) 2024 David Montague, Yuval Levi
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `fastapi-utils-0.2.1/README.md` & `fastapi_utils-0.6.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,72 +1,74 @@
 <p align="center">
-    <em>Reusable utilities for FastAPI</em>
+    <em>Quicker FastApi developing tools</em>
 </p>
 <p align="center">
-<img src="https://img.shields.io/github/last-commit/dmontagu/fastapi-utils.svg">
 <a href="https://github.com/dmontagu/fastapi-utils" target="_blank">
-    <img src="https://github.com/dmontagu/fastapi-utils/workflows/build/badge.svg" alt="Build">
+	<img src="https://img.shields.io/github/last-commit/dmontagu/fastapi-utils.svg">
+	<img src="https://github.com/dmontagu/fastapi-utils/workflows/build/badge.svg" alt="Build CI">
 </a>
 <a href="https://codecov.io/gh/dmontagu/fastapi-utils" target="_blank">
     <img src="https://codecov.io/gh/dmontagu/fastapi-utils/branch/master/graph/badge.svg" alt="Coverage">
 </a>
-<a href="https://app.netlify.com/sites/trusting-archimedes-72b369/deploys">
-    <img src="https://img.shields.io/netlify/28b2a077-65b1-4d6c-9dba-13aaf6059877" alt="Netlify status">
-</a>
 <br />
 <a href="https://pypi.org/project/fastapi-utils" target="_blank">
     <img src="https://badge.fury.io/py/fastapi-utils.svg" alt="Package version">
 </a>
-    <img src="https://img.shields.io/pypi/pyversions/fastapi-utils.svg">
-    <img src="https://img.shields.io/github/license/dmontagu/fastapi-utils.svg">
+<a href="https://github.com/dmontagu/fastapi-utils" target="_blank">
+    <img src="https://img.shields.io/pypi/pyversions/fastapi-utils.svg" alt="Python versions">
+    <img src="https://img.shields.io/github/license/dmontagu/fastapi-utils.svg" alt="License">
+</a>
 </p>
 
 ---
-
 **Documentation**: <a href="https://fastapi-utils.davidmontague.xyz" target="_blank">https://fastapi-utils.davidmontague.xyz</a>
 
 **Source Code**: <a href="https://github.com/dmontagu/fastapi-utils" target="_blank">https://github.com/dmontagu/fastapi-utils</a>
 
 ---
 
-<a href="https://fastapi.tiangolo.com">FastAPI</a> is a modern, fast web framework for building APIs with Python 3.6+.
+<a href="https://fastapi.tiangolo.com">FastAPI</a> is a modern, fast web framework for building APIs with Python 3.7+.
 
 But if you're here, you probably already knew that!
 
 ---
 
 ## Features
 
 This package includes a number of utilities to help reduce boilerplate and reuse common functionality across projects:
 
+* **Resource Class**: Create CRUD with ease the OOP way with `Resource` base class that lets you implement methods quick.
 * **Class Based Views**: Stop repeating the same dependencies over and over in the signature of related endpoints.
-* **Response-Model Inferring Router**: Let FastAPI infer the `response_model` to use based on your return type annotation. 
 * **Repeated Tasks**: Easily trigger periodic tasks on server startup
 * **Timing Middleware**: Log basic timing information for every request
-* **SQLAlchemy Sessions**: The `FastAPISessionMaker` class provides an easily-customized SQLAlchemy Session dependency 
 * **OpenAPI Spec Simplification**: Simplify your OpenAPI Operation IDs for cleaner output from OpenAPI Generator
+* **SQLAlchemy Sessions**: The `FastAPISessionMaker` class provides an easily-customized SQLAlchemy Session dependency
 
 ---
 
 It also adds a variety of more basic utilities that are useful across a wide variety of projects:
 
 * **APIModel**: A reusable `pydantic.BaseModel`-derived base class with useful defaults
-* **APISettings**: A subclass of `pydantic.BaseSettings` that makes it easy to configure FastAPI through environment variables 
+* **APISettings**: A subclass of `pydantic.BaseSettings` that makes it easy to configure FastAPI through environment variables
 * **String-Valued Enums**: The `StrEnum` and `CamelStrEnum` classes make string-valued enums easier to maintain
 * **CamelCase Conversions**: Convenience functions for converting strings from `snake_case` to `camelCase` or `PascalCase` and back
 * **GUID Type**: The provided GUID type makes it easy to use UUIDs as the primary keys for your database tables
 
-See the [docs](https://fastapi-utils.davidmontague.xyz/) for more details and examples. 
+See the [docs](https://https://fastapi-utils.davidmontague.xyz/) for more details and examples.
 
 ## Requirements
 
-This package is intended for use with any recent version of FastAPI (depending on `pydantic>=1.0`), and Python 3.6+.
+This package is intended for use with any recent version of FastAPI (depending on `pydantic>=1.0`), and Python 3.7+.
 
 ## Installation
 
 ```bash
-pip install fastapi-utils
+pip install fastapi-restful  # For basic slim package :)
+
+pip install fastapi-restful[session]  # To add sqlalchemy session maker
+
+pip install fastapi-restful[all]  # For all the packages
 ```
 
 ## License
 
 This project is licensed under the terms of the MIT license.
```

#### html2text {}

```diff
@@ -1,32 +1,33 @@
-                        RReeuussaabbllee uuttiilliittiieess ffoorr FFaassttAAPPII
- [https://img.shields.io/github/last-commit/dmontagu/fastapi-utils.svg]_[_B_u_i_l_d_]
-                          _[_C_o_v_e_r_a_g_e_]_[_N_e_t_l_i_f_y_ _s_t_a_t_u_s_]
-  _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_][https://img.shields.io/pypi/pyversions/fastapi-utils.svg]
-      [https://img.shields.io/github/license/dmontagu/fastapi-utils.svg]
+                       QQuuiicckkeerr FFaassttAAppii ddeevveellooppiinngg ttoooollss
+ _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_a_s_t_-_c_o_m_m_i_t_/_d_m_o_n_t_a_g_u_/_f_a_s_t_a_p_i_-_u_t_i_l_s_._s_v_g_]_[_B_u_i_l_d
+                                 _C_I_]_[_C_o_v_e_r_a_g_e_]
+                  _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_L_i_c_e_n_s_e_]
 --- **Documentation**: _h_t_t_p_s_:_/_/_f_a_s_t_a_p_i_-_u_t_i_l_s_._d_a_v_i_d_m_o_n_t_a_g_u_e_._x_y_z **Source Code**:
 _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_d_m_o_n_t_a_g_u_/_f_a_s_t_a_p_i_-_u_t_i_l_s --- _F_a_s_t_A_P_I is a modern, fast web
-framework for building APIs with Python 3.6+. But if you're here, you probably
+framework for building APIs with Python 3.7+. But if you're here, you probably
 already knew that! --- ## Features This package includes a number of utilities
 to help reduce boilerplate and reuse common functionality across projects: *
-**Class Based Views**: Stop repeating the same dependencies over and over in
-the signature of related endpoints. * **Response-Model Inferring Router**: Let
-FastAPI infer the `response_model` to use based on your return type annotation.
-* **Repeated Tasks**: Easily trigger periodic tasks on server startup *
-**Timing Middleware**: Log basic timing information for every request *
-**SQLAlchemy Sessions**: The `FastAPISessionMaker` class provides an easily-
-customized SQLAlchemy Session dependency * **OpenAPI Spec Simplification**:
-Simplify your OpenAPI Operation IDs for cleaner output from OpenAPI Generator -
--- It also adds a variety of more basic utilities that are useful across a wide
-variety of projects: * **APIModel**: A reusable `pydantic.BaseModel`-derived
-base class with useful defaults * **APISettings**: A subclass of
-`pydantic.BaseSettings` that makes it easy to configure FastAPI through
-environment variables * **String-Valued Enums**: The `StrEnum` and
+**Resource Class**: Create CRUD with ease the OOP way with `Resource` base
+class that lets you implement methods quick. * **Class Based Views**: Stop
+repeating the same dependencies over and over in the signature of related
+endpoints. * **Repeated Tasks**: Easily trigger periodic tasks on server
+startup * **Timing Middleware**: Log basic timing information for every request
+* **OpenAPI Spec Simplification**: Simplify your OpenAPI Operation IDs for
+cleaner output from OpenAPI Generator * **SQLAlchemy Sessions**: The
+`FastAPISessionMaker` class provides an easily-customized SQLAlchemy Session
+dependency --- It also adds a variety of more basic utilities that are useful
+across a wide variety of projects: * **APIModel**: A reusable
+`pydantic.BaseModel`-derived base class with useful defaults * **APISettings**:
+A subclass of `pydantic.BaseSettings` that makes it easy to configure FastAPI
+through environment variables * **String-Valued Enums**: The `StrEnum` and
 `CamelStrEnum` classes make string-valued enums easier to maintain *
 **CamelCase Conversions**: Convenience functions for converting strings from
 `snake_case` to `camelCase` or `PascalCase` and back * **GUID Type**: The
 provided GUID type makes it easy to use UUIDs as the primary keys for your
-database tables See the [docs](https://fastapi-utils.davidmontague.xyz/) for
-more details and examples. ## Requirements This package is intended for use
-with any recent version of FastAPI (depending on `pydantic>=1.0`), and Python
-3.6+. ## Installation ```bash pip install fastapi-utils ``` ## License This
-project is licensed under the terms of the MIT license.
+database tables See the [docs](https://https://fastapi-utils.davidmontague.xyz/
+) for more details and examples. ## Requirements This package is intended for
+use with any recent version of FastAPI (depending on `pydantic>=1.0`), and
+Python 3.7+. ## Installation ```bash pip install fastapi-restful # For basic
+slim package :) pip install fastapi-restful[session] # To add sqlalchemy
+session maker pip install fastapi-restful[all] # For all the packages ``` ##
+License This project is licensed under the terms of the MIT license.
```

### Comparing `fastapi-utils-0.2.1/fastapi_utils/api_model.py` & `fastapi_utils-0.6.0/fastapi_utils/api_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,45 @@
+from __future__ import annotations
+
 from functools import partial
 
-from pydantic import BaseConfig, BaseModel
+import pydantic
+from pydantic import BaseModel
+
+from .camelcase import snake2camel
+
+PYDANTIC_VERSION = pydantic.VERSION
 
-from fastapi_utils.camelcase import snake2camel
+if PYDANTIC_VERSION[0] == "2":
+    from pydantic import ConfigDict
+else:
+    from pydantic import BaseConfig
 
 
 class APIModel(BaseModel):
     """
     Intended for use as a base class for externally-facing models.
 
     Any models that inherit from this class will:
     * accept fields using snake_case or camelCase keys
     * use camelCase keys in the generated OpenAPI spec
     * have orm_mode on by default
         * Because of this, FastAPI will automatically attempt to parse returned orm instances into the model
     """
 
-    class Config(BaseConfig):
-        orm_mode = True
-        allow_population_by_field_name = True
-        alias_generator = partial(snake2camel, start_lower=True)
+    if PYDANTIC_VERSION[0] == "2":
+        model_config = ConfigDict(
+            from_attributes=True, populate_by_name=True, alias_generator=partial(snake2camel, start_lower=True)
+        )
+    else:
+
+        class Config(BaseConfig):
+            orm_mode = True
+            allow_population_by_field_name = True
+            alias_generator = partial(snake2camel, start_lower=True)
 
 
 class APIMessage(APIModel):
     """
     A lightweight utility class intended for use with simple message-returning endpoints.
     """
```

### Comparing `fastapi-utils-0.2.1/fastapi_utils/api_settings.py` & `fastapi_utils-0.6.0/fastapi_utils/api_settings.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,20 @@
+from __future__ import annotations
+
 from functools import lru_cache
-from typing import Any, Dict
+from typing import Any
+
+import pydantic
+
+PYDANTIC_VERSION = pydantic.VERSION
 
-from pydantic import BaseSettings
+if PYDANTIC_VERSION[0] == "2":
+    from pydantic_settings import BaseSettings, SettingsConfigDict
+else:
+    from pydantic import BaseSettings  # type: ignore[no-redef]
 
 
 class APISettings(BaseSettings):
     """
     This class enables the configuration of your FastAPI instance through the use of environment variables.
 
     Any of the instance attributes can be overridden upon instantiation by either passing the desired value to the
@@ -27,37 +36,41 @@
     title: str = "FastAPI"
     version: str = "0.1.0"
 
     # Custom settings
     disable_docs: bool = False
 
     @property
-    def fastapi_kwargs(self) -> Dict[str, Any]:
+    def fastapi_kwargs(self) -> dict[str, Any]:
         """
         This returns a dictionary of the most commonly used keyword arguments when initializing a FastAPI instance
 
         If `self.disable_docs` is True, the various docs-related arguments are disabled, preventing your spec from being
         published.
         """
-        fastapi_kwargs: Dict[str, Any] = {
+        fastapi_kwargs: dict[str, Any] = {
             "debug": self.debug,
             "docs_url": self.docs_url,
             "openapi_prefix": self.openapi_prefix,
             "openapi_url": self.openapi_url,
             "redoc_url": self.redoc_url,
             "title": self.title,
             "version": self.version,
         }
         if self.disable_docs:
             fastapi_kwargs.update({"docs_url": None, "openapi_url": None, "redoc_url": None})
         return fastapi_kwargs
 
-    class Config:
-        env_prefix = "api_"
-        validate_assignment = True
+    if PYDANTIC_VERSION[0] == "2":
+        model_config = SettingsConfigDict(env_prefix="api_", validate_assignment=True)
+    else:
+
+        class Config:
+            env_prefix = "api_"
+            validate_assignment = True
 
 
 @lru_cache()
 def get_api_settings() -> APISettings:
     """
     This function returns a cached instance of the APISettings object.
```

### Comparing `fastapi-utils-0.2.1/fastapi_utils/camelcase.py` & `fastapi_utils-0.6.0/fastapi_utils/camelcase.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import re
 
 
 def snake2camel(snake: str, start_lower: bool = False) -> str:
     """
     Converts a snake_case string to camelCase.
```

### Comparing `fastapi-utils-0.2.1/fastapi_utils/enums.py` & `fastapi_utils-0.6.0/fastapi_utils/enums.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,37 @@
+from __future__ import annotations
+
 from enum import Enum
+from typing import List
 
-from fastapi_utils.camelcase import snake2camel
+from .camelcase import snake2camel
 
 
 class StrEnum(str, Enum):
     """
     StrEnum subclasses that create variants using `auto()` will have values equal to their names
     Enums inheriting from this class that set values using `enum.auto()` will have variant values equal to their names
     """
 
-    # noinspection PyMethodParameters
-    def _generate_next_value_(name, start, count, last_values) -> str:  # type: ignore
+    @staticmethod
+    def _generate_next_value_(name: str, start: int, count: int, last_values: List[str]) -> str:
         """
         Uses the name as the automatic value, rather than an integer
 
         See https://docs.python.org/3/library/enum.html#using-automatic-values for reference
         """
         return name
 
 
 class CamelStrEnum(str, Enum):
     """
     CamelStrEnum subclasses that create variants using `auto()` will have values equal to their camelCase names
     """
 
-    # noinspection PyMethodParameters
-    def _generate_next_value_(name, start, count, last_values) -> str:  # type: ignore
+    @staticmethod
+    def _generate_next_value_(name: str, start: int, count: int, last_values: List[str]) -> str:
         """
         Uses the camelCase name as the automatic value, rather than an integer
 
         See https://docs.python.org/3/library/enum.html#using-automatic-values for reference
         """
         return snake2camel(name, start_lower=True)
```

### Comparing `fastapi-utils-0.2.1/fastapi_utils/guid_type.py` & `fastapi_utils-0.6.0/fastapi_utils/guid_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# TODO: Add tests for postgres
+from __future__ import annotations
+
 import uuid
 from typing import TYPE_CHECKING, no_type_check
 
 import sqlalchemy as sa
 from sqlalchemy.dialects.postgresql.base import UUID
 from sqlalchemy.sql.sqltypes import CHAR
 from sqlalchemy.sql.type_api import TypeDecorator
@@ -23,14 +24,15 @@
 
     Uses PostgreSQL's UUID type, otherwise uses CHAR(32), storing as stringified hex values.
 
     Taken from SQLAlchemy docs: https://docs.sqlalchemy.org/en/13/core/custom_types.html#backend-agnostic-guid-type
     """
 
     impl = CHAR
+    cache_ok = True
 
     @no_type_check
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     @no_type_check
     def load_dialect_impl(self, dialect):
```

### Comparing `fastapi-utils-0.2.1/fastapi_utils/session.py` & `fastapi_utils-0.6.0/fastapi_utils/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from __future__ import annotations
+
+from collections.abc import Iterator
 from contextlib import contextmanager
-from typing import Iterator, Optional
 
 import sqlalchemy as sa
 from sqlalchemy.orm import Session
 
 
 class FastAPISessionMaker:
     """
@@ -22,16 +24,16 @@
 
             "<scheme>://<user>:<password>@<host>:<port>/<database>"
 
         A concrete example looks like "postgresql://db_user:password@db:5432/app"
         """
         self.database_uri = database_uri
 
-        self._cached_engine: Optional[sa.engine.Engine] = None
-        self._cached_sessionmaker: Optional[sa.orm.sessionmaker] = None
+        self._cached_engine: sa.engine.Engine | None = None
+        self._cached_sessionmaker: sa.orm.sessionmaker | None = None
 
     @property
     def cached_engine(self) -> sa.engine.Engine:
         """
         Returns a lazily-cached sqlalchemy engine for the instance's database_uri.
         """
         engine = self._cached_engine
@@ -53,15 +55,15 @@
 
     def get_new_engine(self) -> sa.engine.Engine:
         """
         Returns a new sqlalchemy engine using the instance's database_uri.
         """
         return get_engine(self.database_uri)
 
-    def get_new_sessionmaker(self, engine: Optional[sa.engine.Engine]) -> sa.orm.sessionmaker:
+    def get_new_sessionmaker(self, engine: sa.engine.Engine | None) -> sa.orm.sessionmaker:
         """
         Returns a new sessionmaker for the provided sqlalchemy engine. If no engine is provided, the
         instance's (lazily-cached) engine is used.
         """
         engine = engine or self.cached_engine
         return get_sessionmaker_for_engine(engine)
```

### Comparing `fastapi-utils-0.2.1/fastapi_utils/tasks.py` & `fastapi_utils-0.6.0/fastapi_utils/tasks.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,80 +1,81 @@
+from __future__ import annotations
+
 import asyncio
 import logging
-from asyncio import ensure_future
 from functools import wraps
 from traceback import format_exception
-from typing import Any, Callable, Coroutine, Optional, Union
+from typing import Any, Callable, Coroutine, Union
 
 from starlette.concurrency import run_in_threadpool
 
 NoArgsNoReturnFuncT = Callable[[], None]
 NoArgsNoReturnAsyncFuncT = Callable[[], Coroutine[Any, Any, None]]
 NoArgsNoReturnDecorator = Callable[[Union[NoArgsNoReturnFuncT, NoArgsNoReturnAsyncFuncT]], NoArgsNoReturnAsyncFuncT]
 
 
 def repeat_every(
     *,
     seconds: float,
-    wait_first: bool = False,
-    logger: Optional[logging.Logger] = None,
+    wait_first: float | None = None,
+    logger: logging.Logger | None = None,
     raise_exceptions: bool = False,
-    max_repetitions: Optional[int] = None,
+    max_repetitions: int | None = None,
 ) -> NoArgsNoReturnDecorator:
     """
     This function returns a decorator that modifies a function so it is periodically re-executed after its first call.
 
     The function it decorates should accept no arguments and return nothing. If necessary, this can be accomplished
     by using `functools.partial` or otherwise wrapping the target function prior to decoration.
 
     Parameters
     ----------
     seconds: float
         The number of seconds to wait between repeated calls
-    wait_first: bool (default False)
-        If True, the function will wait for a single period before the first call
+    wait_first: float (default None)
+        If not None, the function will wait for the given duration before the first call
     logger: Optional[logging.Logger] (default None)
         The logger to use to log any exceptions raised by calls to the decorated function.
         If not provided, exceptions will not be logged by this function (though they may be handled by the event loop).
     raise_exceptions: bool (default False)
         If True, errors raised by the decorated function will be raised to the event loop's exception handler.
         Note that if an error is raised, the repeated execution will stop.
         Otherwise, exceptions are just logged and the execution continues to repeat.
         See https://docs.python.org/3/library/asyncio-eventloop.html#asyncio.loop.set_exception_handler for more info.
     max_repetitions: Optional[int] (default None)
         The maximum number of times to call the repeated function. If `None`, the function is repeated forever.
     """
 
-    def decorator(func: Union[NoArgsNoReturnAsyncFuncT, NoArgsNoReturnFuncT]) -> NoArgsNoReturnAsyncFuncT:
+    def decorator(func: NoArgsNoReturnAsyncFuncT | NoArgsNoReturnFuncT) -> NoArgsNoReturnAsyncFuncT:
         """
         Converts the decorated function into a repeated, periodically-called version of itself.
         """
         is_coroutine = asyncio.iscoroutinefunction(func)
 
         @wraps(func)
         async def wrapped() -> None:
             repetitions = 0
 
             async def loop() -> None:
                 nonlocal repetitions
-                if wait_first:
-                    await asyncio.sleep(seconds)
+                if wait_first is not None:
+                    await asyncio.sleep(wait_first)
                 while max_repetitions is None or repetitions < max_repetitions:
                     try:
                         if is_coroutine:
                             await func()  # type: ignore
                         else:
                             await run_in_threadpool(func)
-                        repetitions += 1
                     except Exception as exc:
                         if logger is not None:
                             formatted_exception = "".join(format_exception(type(exc), exc, exc.__traceback__))
                             logger.error(formatted_exception)
                         if raise_exceptions:
                             raise exc
+                    repetitions += 1
                     await asyncio.sleep(seconds)
 
-            ensure_future(loop())
+            await loop()
 
         return wrapped
 
     return decorator
```

### Comparing `fastapi-utils-0.2.1/fastapi_utils/timing.py` & `fastapi_utils-0.6.0/fastapi_utils/timing.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,30 +3,35 @@
 
 The middleware from this module is intended for use during both development and production,
 but only reports timing data at the granularity of individual endpoint calls.
 
 For more detailed performance investigations (during development only, due to added overhead),
 consider using the coroutine-aware profiling library `yappi`.
 """
-import resource
+
+from __future__ import annotations
+
+import os
 import time
-from typing import Any, Callable, Optional
+from collections.abc import Callable
+from typing import Any
 
+import psutil
 from fastapi import FastAPI
 from starlette.middleware.base import RequestResponseEndpoint
 from starlette.requests import Request
 from starlette.responses import Response
 from starlette.routing import Match, Mount
 from starlette.types import Scope
 
 TIMER_ATTRIBUTE = "__fastapi_utils_timer__"
 
 
 def add_timing_middleware(
-    app: FastAPI, record: Optional[Callable[[str], None]] = None, prefix: str = "", exclude: Optional[str] = None
+    app: FastAPI, record: Callable[[str], None] | None = None, prefix: str = "", exclude: str | None = None
 ) -> None:
     """
     Adds a middleware to the provided `app` that records timing metrics using the provided `record` callable.
 
     Typically `record` would be something like `logger.info` for a `logging.Logger` instance.
 
     The provided `prefix` is used when generating route names.
@@ -44,26 +49,27 @@
         metric_name = metric_namer(request.scope)
         with _TimingStats(metric_name, record=record, exclude=exclude) as timer:
             setattr(request.state, TIMER_ATTRIBUTE, timer)
             response = await call_next(request)
         return response
 
 
-def record_timing(request: Request, note: Optional[str] = None) -> None:
+def record_timing(request: Request, note: str | None = None) -> None:
     """
     Call this function at any point that you want to display elapsed time during the handling of a single request
 
     This can help profile which piece of a request is causing a performance bottleneck.
 
     Note that for this function to succeed, the request should have been generated by a FastAPI app
     that has had timing middleware added using the `fastapi_utils.timing.add_timing_middleware` function.
     """
     timer = getattr(request.state, TIMER_ATTRIBUTE, None)
     if timer is not None:
-        assert isinstance(timer, _TimingStats)
+        if not isinstance(timer, _TimingStats):
+            raise ValueError("Timer should be of an instance of TimingStats")
         timer.emit(note)
     else:
         raise ValueError("No timer present on request")
 
 
 class _TimingStats:
     """
@@ -77,64 +83,73 @@
         The callable to call on generated messages. Defaults to `print`, but typically
         something like `logger.info` for a `logging.Logger` instance would be preferable.
     exclude:
         An optional string; if it is not None and occurs inside `name`, no stats will be emitted
     """
 
     def __init__(
-        self, name: Optional[str] = None, record: Callable[[str], None] = None, exclude: Optional[str] = None
+        self, name: str | None = None, record: Callable[[str], None] | None = None, exclude: str | None = None
     ) -> None:
         self.name = name
         self.record = record or print
 
+        self.process: psutil.Process = psutil.Process(os.getpid())
         self.start_time: float = 0
         self.start_cpu_time: float = 0
         self.end_cpu_time: float = 0
         self.end_time: float = 0
         self.silent: bool = False
 
         if self.name is not None and exclude is not None and (exclude in self.name):
             self.silent = True
 
     def start(self) -> None:
         self.start_time = time.time()
-        self.start_cpu_time = _get_cpu_time()
+        self.start_cpu_time = self._get_cpu_time()
 
     def take_split(self) -> None:
         self.end_time = time.time()
-        self.end_cpu_time = _get_cpu_time()
+        self.end_cpu_time = self._get_cpu_time()
 
     @property
     def time(self) -> float:
         return self.end_time - self.start_time
 
     @property
     def cpu_time(self) -> float:
         return self.end_cpu_time - self.start_cpu_time
 
-    def __enter__(self) -> "_TimingStats":
+    def __enter__(self) -> _TimingStats:
         self.start()
         return self
 
     def __exit__(self, exc_type: Any, exc_value: Any, traceback: Any) -> None:
         self.emit()
 
-    def emit(self, note: Optional[str] = None) -> None:
+    def emit(self, note: str | None = None) -> None:
         """
         Emit timing information, optionally including a specified note
         """
         if not self.silent:
             self.take_split()
             cpu_ms = 1000 * self.cpu_time
             wall_ms = 1000 * self.time
             message = f"TIMING: Wall: {wall_ms:6.1f}ms | CPU: {cpu_ms:6.1f}ms | {self.name}"
             if note is not None:
                 message += f" ({note})"
             self.record(message)
 
+    def _get_cpu_time(self) -> float:
+        """
+        Generates the cpu time to report. Adds the user and system time, following the implementation from timing-asgi
+        """
+        resources = self.process.cpu_times()
+        # add up user time and system time
+        return resources[0] + resources[1]
+
 
 class _MetricNamer:
     """
     This class generates the route "name" used when logging timing records.
 
     If the route has `endpoint` and `name` attributes, the endpoint's module and route's name will be used
     (along with an optional prefix that can be used, e.g., to distinguish between multiple mounted ASGI apps).
@@ -169,16 +184,7 @@
         if hasattr(route, "endpoint") and hasattr(route, "name"):
             name = f"{self.prefix}{route.endpoint.__module__}.{route.name}"  # type: ignore
         elif isinstance(route, Mount):
             name = f"{type(route.app).__name__}<{route.name!r}>"
         else:
             name = str(f"<Path: {scope['path']}>")
         return name
-
-
-def _get_cpu_time() -> float:
-    """
-    Generates the cpu time to report. Adds the user and system time, following the implementation from timing-asgi
-    """
-    resources = resource.getrusage(resource.RUSAGE_SELF)
-    # add up user time (ru_utime) and system time (ru_stime)
-    return resources[0] + resources[1]
```

### Comparing `fastapi-utils-0.2.1/PKG-INFO` & `fastapi_utils-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,112 +1,123 @@
 Metadata-Version: 2.1
 Name: fastapi-utils
-Version: 0.2.1
+Version: 0.6.0
 Summary: Reusable utilities for FastAPI
 Home-page: https://fastapi-utils.davidmontague.xyz
 License: MIT
-Keywords: fastapi,utilities,utils
-Author: David Montague
-Author-email: davwmont@gmail.com
-Requires-Python: >=3.6,<4.0
-Classifier: Development Status :: 3 - Alpha
+Keywords: fastapi,OOP,RESTful
+Author: Yuval Levi
+Author-email: yuvall9313@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO
+Classifier: Framework :: FastAPI
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Dist: fastapi
-Requires-Dist: pydantic (>=1.0,<2.0)
-Requires-Dist: sqlalchemy (>=1.3.12,<2.0.0)
+Provides-Extra: all
+Provides-Extra: session
+Requires-Dist: fastapi (>=0.89,<1.0)
+Requires-Dist: psutil (>=5,<6)
+Requires-Dist: pydantic (>1.0,<3.0)
+Requires-Dist: pydantic-settings (>=2.0.1,<3.0.0) ; extra == "all"
+Requires-Dist: sqlalchemy (>=1.4,<3.0) ; extra == "all" or extra == "session"
+Requires-Dist: typing-inspect (>=0.9.0,<0.10.0) ; extra == "all"
 Project-URL: Documentation, https://fastapi-utils.davidmontague.xyz
 Project-URL: Repository, https://github.com/dmontagu/fastapi-utils
 Description-Content-Type: text/markdown
 
 <p align="center">
-    <em>Reusable utilities for FastAPI</em>
+    <em>Quicker FastApi developing tools</em>
 </p>
 <p align="center">
-<img src="https://img.shields.io/github/last-commit/dmontagu/fastapi-utils.svg">
 <a href="https://github.com/dmontagu/fastapi-utils" target="_blank">
-    <img src="https://github.com/dmontagu/fastapi-utils/workflows/build/badge.svg" alt="Build">
+	<img src="https://img.shields.io/github/last-commit/dmontagu/fastapi-utils.svg">
+	<img src="https://github.com/dmontagu/fastapi-utils/workflows/build/badge.svg" alt="Build CI">
 </a>
 <a href="https://codecov.io/gh/dmontagu/fastapi-utils" target="_blank">
     <img src="https://codecov.io/gh/dmontagu/fastapi-utils/branch/master/graph/badge.svg" alt="Coverage">
 </a>
-<a href="https://app.netlify.com/sites/trusting-archimedes-72b369/deploys">
-    <img src="https://img.shields.io/netlify/28b2a077-65b1-4d6c-9dba-13aaf6059877" alt="Netlify status">
-</a>
 <br />
 <a href="https://pypi.org/project/fastapi-utils" target="_blank">
     <img src="https://badge.fury.io/py/fastapi-utils.svg" alt="Package version">
 </a>
-    <img src="https://img.shields.io/pypi/pyversions/fastapi-utils.svg">
-    <img src="https://img.shields.io/github/license/dmontagu/fastapi-utils.svg">
+<a href="https://github.com/dmontagu/fastapi-utils" target="_blank">
+    <img src="https://img.shields.io/pypi/pyversions/fastapi-utils.svg" alt="Python versions">
+    <img src="https://img.shields.io/github/license/dmontagu/fastapi-utils.svg" alt="License">
+</a>
 </p>
 
 ---
-
 **Documentation**: <a href="https://fastapi-utils.davidmontague.xyz" target="_blank">https://fastapi-utils.davidmontague.xyz</a>
 
 **Source Code**: <a href="https://github.com/dmontagu/fastapi-utils" target="_blank">https://github.com/dmontagu/fastapi-utils</a>
 
 ---
 
-<a href="https://fastapi.tiangolo.com">FastAPI</a> is a modern, fast web framework for building APIs with Python 3.6+.
+<a href="https://fastapi.tiangolo.com">FastAPI</a> is a modern, fast web framework for building APIs with Python 3.7+.
 
 But if you're here, you probably already knew that!
 
 ---
 
 ## Features
 
 This package includes a number of utilities to help reduce boilerplate and reuse common functionality across projects:
 
+* **Resource Class**: Create CRUD with ease the OOP way with `Resource` base class that lets you implement methods quick.
 * **Class Based Views**: Stop repeating the same dependencies over and over in the signature of related endpoints.
-* **Response-Model Inferring Router**: Let FastAPI infer the `response_model` to use based on your return type annotation. 
 * **Repeated Tasks**: Easily trigger periodic tasks on server startup
 * **Timing Middleware**: Log basic timing information for every request
-* **SQLAlchemy Sessions**: The `FastAPISessionMaker` class provides an easily-customized SQLAlchemy Session dependency 
 * **OpenAPI Spec Simplification**: Simplify your OpenAPI Operation IDs for cleaner output from OpenAPI Generator
+* **SQLAlchemy Sessions**: The `FastAPISessionMaker` class provides an easily-customized SQLAlchemy Session dependency
 
 ---
 
 It also adds a variety of more basic utilities that are useful across a wide variety of projects:
 
 * **APIModel**: A reusable `pydantic.BaseModel`-derived base class with useful defaults
-* **APISettings**: A subclass of `pydantic.BaseSettings` that makes it easy to configure FastAPI through environment variables 
+* **APISettings**: A subclass of `pydantic.BaseSettings` that makes it easy to configure FastAPI through environment variables
 * **String-Valued Enums**: The `StrEnum` and `CamelStrEnum` classes make string-valued enums easier to maintain
 * **CamelCase Conversions**: Convenience functions for converting strings from `snake_case` to `camelCase` or `PascalCase` and back
 * **GUID Type**: The provided GUID type makes it easy to use UUIDs as the primary keys for your database tables
 
-See the [docs](https://fastapi-utils.davidmontague.xyz/) for more details and examples. 
+See the [docs](https://https://fastapi-utils.davidmontague.xyz/) for more details and examples.
 
 ## Requirements
 
-This package is intended for use with any recent version of FastAPI (depending on `pydantic>=1.0`), and Python 3.6+.
+This package is intended for use with any recent version of FastAPI (depending on `pydantic>=1.0`), and Python 3.7+.
 
 ## Installation
 
 ```bash
-pip install fastapi-utils
+pip install fastapi-restful  # For basic slim package :)
+
+pip install fastapi-restful[session]  # To add sqlalchemy session maker
+
+pip install fastapi-restful[all]  # For all the packages
 ```
 
 ## License
 
 This project is licensed under the terms of the MIT license.
```

#### html2text {}

```diff
@@ -1,53 +1,60 @@
-Metadata-Version: 2.1 Name: fastapi-utils Version: 0.2.1 Summary: Reusable
+Metadata-Version: 2.1 Name: fastapi-utils Version: 0.6.0 Summary: Reusable
 utilities for FastAPI Home-page: https://fastapi-utils.davidmontague.xyz
-License: MIT Keywords: fastapi,utilities,utils Author: David Montague Author-
-email: davwmont@gmail.com Requires-Python: >=3.6,<4.0 Classifier: Development
-Status :: 3 - Alpha Classifier: Environment :: Web Environment Classifier:
-Framework :: AsyncIO Classifier: Intended Audience :: Developers Classifier:
-Intended Audience :: Information Technology Classifier: Intended Audience ::
-System Administrators Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
-Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Topic :: Internet Classifier:
-Topic :: Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP :: HTTP
-Servers Classifier: Topic :: Software Development Classifier: Topic :: Software
-Development :: Libraries Classifier: Topic :: Software Development :: Libraries
-:: Python Modules Classifier: Topic :: Utilities Classifier: Typing :: Typed
-Requires-Dist: fastapi Requires-Dist: pydantic (>=1.0,<2.0) Requires-Dist:
-sqlalchemy (>=1.3.12,<2.0.0) Project-URL: Documentation, https://fastapi-
+License: MIT Keywords: fastapi,OOP,RESTful Author: Yuval Levi Author-email:
+yuvall9313@gmail.com Requires-Python: >=3.7,<4.0 Classifier: Development Status
+:: 4 - Beta Classifier: Environment :: Web Environment Classifier: Framework ::
+AsyncIO Classifier: Framework :: FastAPI Classifier: Intended Audience ::
+Developers Classifier: Intended Audience :: Information Technology Classifier:
+Intended Audience :: System Administrators Classifier: License :: OSI Approved
+:: MIT License Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
+Only Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
+Internet Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic ::
+Internet :: WWW/HTTP :: HTTP Servers Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Classifier: Topic ::
+Utilities Classifier: Typing :: Typed Provides-Extra: all Provides-Extra:
+session Requires-Dist: fastapi (>=0.89,<1.0) Requires-Dist: psutil (>=5,<6)
+Requires-Dist: pydantic (>1.0,<3.0) Requires-Dist: pydantic-settings
+(>=2.0.1,<3.0.0) ; extra == "all" Requires-Dist: sqlalchemy (>=1.4,<3.0) ;
+extra == "all" or extra == "session" Requires-Dist: typing-inspect
+(>=0.9.0,<0.10.0) ; extra == "all" Project-URL: Documentation, https://fastapi-
 utils.davidmontague.xyz Project-URL: Repository, https://github.com/dmontagu/
 fastapi-utils Description-Content-Type: text/markdown
-                        RReeuussaabbllee uuttiilliittiieess ffoorr FFaassttAAPPII
- [https://img.shields.io/github/last-commit/dmontagu/fastapi-utils.svg]_[_B_u_i_l_d_]
-                          _[_C_o_v_e_r_a_g_e_]_[_N_e_t_l_i_f_y_ _s_t_a_t_u_s_]
-  _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_][https://img.shields.io/pypi/pyversions/fastapi-utils.svg]
-      [https://img.shields.io/github/license/dmontagu/fastapi-utils.svg]
+                       QQuuiicckkeerr FFaassttAAppii ddeevveellooppiinngg ttoooollss
+ _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_a_s_t_-_c_o_m_m_i_t_/_d_m_o_n_t_a_g_u_/_f_a_s_t_a_p_i_-_u_t_i_l_s_._s_v_g_]_[_B_u_i_l_d
+                                 _C_I_]_[_C_o_v_e_r_a_g_e_]
+                  _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_L_i_c_e_n_s_e_]
 --- **Documentation**: _h_t_t_p_s_:_/_/_f_a_s_t_a_p_i_-_u_t_i_l_s_._d_a_v_i_d_m_o_n_t_a_g_u_e_._x_y_z **Source Code**:
 _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_d_m_o_n_t_a_g_u_/_f_a_s_t_a_p_i_-_u_t_i_l_s --- _F_a_s_t_A_P_I is a modern, fast web
-framework for building APIs with Python 3.6+. But if you're here, you probably
+framework for building APIs with Python 3.7+. But if you're here, you probably
 already knew that! --- ## Features This package includes a number of utilities
 to help reduce boilerplate and reuse common functionality across projects: *
-**Class Based Views**: Stop repeating the same dependencies over and over in
-the signature of related endpoints. * **Response-Model Inferring Router**: Let
-FastAPI infer the `response_model` to use based on your return type annotation.
-* **Repeated Tasks**: Easily trigger periodic tasks on server startup *
-**Timing Middleware**: Log basic timing information for every request *
-**SQLAlchemy Sessions**: The `FastAPISessionMaker` class provides an easily-
-customized SQLAlchemy Session dependency * **OpenAPI Spec Simplification**:
-Simplify your OpenAPI Operation IDs for cleaner output from OpenAPI Generator -
--- It also adds a variety of more basic utilities that are useful across a wide
-variety of projects: * **APIModel**: A reusable `pydantic.BaseModel`-derived
-base class with useful defaults * **APISettings**: A subclass of
-`pydantic.BaseSettings` that makes it easy to configure FastAPI through
-environment variables * **String-Valued Enums**: The `StrEnum` and
+**Resource Class**: Create CRUD with ease the OOP way with `Resource` base
+class that lets you implement methods quick. * **Class Based Views**: Stop
+repeating the same dependencies over and over in the signature of related
+endpoints. * **Repeated Tasks**: Easily trigger periodic tasks on server
+startup * **Timing Middleware**: Log basic timing information for every request
+* **OpenAPI Spec Simplification**: Simplify your OpenAPI Operation IDs for
+cleaner output from OpenAPI Generator * **SQLAlchemy Sessions**: The
+`FastAPISessionMaker` class provides an easily-customized SQLAlchemy Session
+dependency --- It also adds a variety of more basic utilities that are useful
+across a wide variety of projects: * **APIModel**: A reusable
+`pydantic.BaseModel`-derived base class with useful defaults * **APISettings**:
+A subclass of `pydantic.BaseSettings` that makes it easy to configure FastAPI
+through environment variables * **String-Valued Enums**: The `StrEnum` and
 `CamelStrEnum` classes make string-valued enums easier to maintain *
 **CamelCase Conversions**: Convenience functions for converting strings from
 `snake_case` to `camelCase` or `PascalCase` and back * **GUID Type**: The
 provided GUID type makes it easy to use UUIDs as the primary keys for your
-database tables See the [docs](https://fastapi-utils.davidmontague.xyz/) for
-more details and examples. ## Requirements This package is intended for use
-with any recent version of FastAPI (depending on `pydantic>=1.0`), and Python
-3.6+. ## Installation ```bash pip install fastapi-utils ``` ## License This
-project is licensed under the terms of the MIT license.
+database tables See the [docs](https://https://fastapi-utils.davidmontague.xyz/
+) for more details and examples. ## Requirements This package is intended for
+use with any recent version of FastAPI (depending on `pydantic>=1.0`), and
+Python 3.7+. ## Installation ```bash pip install fastapi-restful # For basic
+slim package :) pip install fastapi-restful[session] # To add sqlalchemy
+session maker pip install fastapi-restful[all] # For all the packages ``` ##
+License This project is licensed under the terms of the MIT license.
```

