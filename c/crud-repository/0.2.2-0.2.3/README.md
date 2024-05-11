# Comparing `tmp/crud_repository-0.2.2.tar.gz` & `tmp/crud_repository-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crud_repository-0.2.2.tar", last modified: Fri May 10 08:37:31 2024, max compression
+gzip compressed data, was "crud_repository-0.2.3.tar", last modified: Sat May 11 15:49:12 2024, max compression
```

## Comparing `crud_repository-0.2.2.tar` & `crud_repository-0.2.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:31.946884 crud_repository-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-10 08:37:21.000000 crud_repository-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-10 08:37:21.000000 crud_repository-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-05-10 08:37:31.946884 crud_repository-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-05-10 08:37:21.000000 crud_repository-0.2.2/PYPI.md
--rw-r--r--   0 runner    (1001) docker     (127)    16267 2024-05-10 08:37:21.000000 crud_repository-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:31.942885 crud_repository-0.2.2/crud_repository/
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/__config__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:31.942885 crud_repository-0.2.2/crud_repository/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/db/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/db/idatabase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:31.942885 crud_repository-0.2.2/crud_repository/db/mariadb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/db/mariadb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/db/mariadb/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:31.942885 crud_repository-0.2.2/crud_repository/db/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/db/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/db/mysql/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:31.942885 crud_repository-0.2.2/crud_repository/db/postgres/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/db/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/db/postgres/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:31.942885 crud_repository-0.2.2/crud_repository/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/model/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:31.946884 crud_repository-0.2.2/crud_repository/my_logger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/my_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/my_logger/formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/my_logger/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/my_logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/my_logger/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:31.946884 crud_repository-0.2.2/crud_repository/repo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/repo/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:31.946884 crud_repository-0.2.2/crud_repository.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-05-10 08:37:31.000000 crud_repository-0.2.2/crud_repository.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-10 08:37:31.000000 crud_repository-0.2.2/crud_repository.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:37:31.000000 crud_repository-0.2.2/crud_repository.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:37:31.000000 crud_repository-0.2.2/crud_repository.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-10 08:37:31.000000 crud_repository-0.2.2/crud_repository.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-10 08:37:31.000000 crud_repository-0.2.2/crud_repository.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-10 08:37:30.000000 crud_repository-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-10 08:37:31.946884 crud_repository-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-10 08:37:21.000000 crud_repository-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:49:12.091772 crud_repository-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-11 15:49:01.000000 crud_repository-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-11 15:49:01.000000 crud_repository-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-05-11 15:49:12.091772 crud_repository-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-05-11 15:49:01.000000 crud_repository-0.2.3/PYPI.md
+-rw-r--r--   0 runner    (1001) docker     (127)    15860 2024-05-11 15:49:01.000000 crud_repository-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:49:12.087772 crud_repository-0.2.3/crud_repository/
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-11 15:49:01.000000 crud_repository-0.2.3/crud_repository/__config__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 15:49:01.000000 crud_repository-0.2.3/crud_repository/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:49:12.087772 crud_repository-0.2.3/crud_repository/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 15:49:01.000000 crud_repository-0.2.3/crud_repository/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-11 15:49:01.000000 crud_repository-0.2.3/crud_repository/db/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-11 15:49:01.000000 crud_repository-0.2.3/crud_repository/db/idatabase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:49:12.087772 crud_repository-0.2.3/crud_repository/db/mariadb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 15:49:01.000000 crud_repository-0.2.3/crud_repository/db/mariadb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-11 15:49:01.000000 crud_repository-0.2.3/crud_repository/db/mariadb/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:49:12.087772 crud_repository-0.2.3/crud_repository/db/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 15:49:01.000000 crud_repository-0.2.3/crud_repository/db/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-11 15:49:01.000000 crud_repository-0.2.3/crud_repository/db/mysql/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:49:12.087772 crud_repository-0.2.3/crud_repository/db/postgres/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 15:49:01.000000 crud_repository-0.2.3/crud_repository/db/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-11 15:49:01.000000 crud_repository-0.2.3/crud_repository/db/postgres/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:49:12.087772 crud_repository-0.2.3/crud_repository/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 15:49:01.000000 crud_repository-0.2.3/crud_repository/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-11 15:49:01.000000 crud_repository-0.2.3/crud_repository/model/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:49:12.091772 crud_repository-0.2.3/crud_repository/my_logger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 15:49:01.000000 crud_repository-0.2.3/crud_repository/my_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-11 15:49:01.000000 crud_repository-0.2.3/crud_repository/my_logger/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-11 15:49:01.000000 crud_repository-0.2.3/crud_repository/my_logger/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-11 15:49:01.000000 crud_repository-0.2.3/crud_repository/my_logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-11 15:49:01.000000 crud_repository-0.2.3/crud_repository/my_logger/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:49:12.091772 crud_repository-0.2.3/crud_repository/repo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 15:49:01.000000 crud_repository-0.2.3/crud_repository/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-11 15:49:01.000000 crud_repository-0.2.3/crud_repository/repo/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:49:12.091772 crud_repository-0.2.3/crud_repository.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-05-11 15:49:12.000000 crud_repository-0.2.3/crud_repository.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-11 15:49:12.000000 crud_repository-0.2.3/crud_repository.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 15:49:12.000000 crud_repository-0.2.3/crud_repository.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 15:49:11.000000 crud_repository-0.2.3/crud_repository.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-11 15:49:12.000000 crud_repository-0.2.3/crud_repository.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-11 15:49:12.000000 crud_repository-0.2.3/crud_repository.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-11 15:49:10.000000 crud_repository-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-11 15:49:12.091772 crud_repository-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-11 15:49:01.000000 crud_repository-0.2.3/setup.py
```

### Comparing `crud_repository-0.2.2/LICENSE` & `crud_repository-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `crud_repository-0.2.2/MANIFEST.in` & `crud_repository-0.2.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `crud_repository-0.2.2/PKG-INFO` & `crud_repository-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crud_repository
-Version: 0.2.2
+Version: 0.2.3
 Summary: The CRUDRepository is a Python project designed to provide a generic implementation of Create, Read, Update, and Delete (CRUD) operations for various databases.
 Home-page: https://github.com/dellius-alexander/CRUDRepository.git
 Author: Dellius Alexander
 Author-email: Dellius Alexander <dalexander@hyfisolutions.com>, info@hyfisolutions.com
 Maintainer-email: Dellius Alexander <dalexander@hyfisolutions.com>
 License: MIT License
```

### Comparing `crud_repository-0.2.2/PYPI.md` & `crud_repository-0.2.3/PYPI.md`

 * *Files identical despite different names*

### Comparing `crud_repository-0.2.2/README.md` & `crud_repository-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -411,12 +411,7 @@
     # Create a new user
     user = User(username='Candy', password='password')
 
     # Add the user to the database
     user_repo.create(user)
 ```
 ---
-Models:
-  * User: Represents a user entity with attributes id, username, password, email (email.id), address (address.id), role (role.id) last_updated
-  * Address: Represents an address entity with attributes id, street, city, state, zipcode, last_updated
-  * Role: Represents a role entity with attributes id, name, last_updated
-  * Email: Represents an email entity with attributes id, email, last_updated
```

### Comparing `crud_repository-0.2.2/crud_repository/__config__.py` & `crud_repository-0.2.3/crud_repository/__config__.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.2.2/crud_repository/db/factory.py` & `crud_repository-0.2.3/crud_repository/db/factory.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.2.2/crud_repository/db/idatabase.py` & `crud_repository-0.2.3/crud_repository/db/idatabase.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.2.2/crud_repository/db/mariadb/db.py` & `crud_repository-0.2.3/crud_repository/db/mariadb/db.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.2.2/crud_repository/db/mysql/db.py` & `crud_repository-0.2.3/crud_repository/db/mysql/db.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.2.2/crud_repository/db/postgres/db.py` & `crud_repository-0.2.3/crud_repository/db/postgres/db.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.2.2/crud_repository/my_logger/formatters.py` & `crud_repository-0.2.3/crud_repository/my_logger/formatters.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.2.2/crud_repository/my_logger/handlers.py` & `crud_repository-0.2.3/crud_repository/my_logger/handlers.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.2.2/crud_repository/my_logger/logger.py` & `crud_repository-0.2.3/crud_repository/my_logger/logger.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.2.2/crud_repository/my_logger/monitor.py` & `crud_repository-0.2.3/crud_repository/my_logger/monitor.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.2.2/crud_repository/repo/repository.py` & `crud_repository-0.2.3/crud_repository/repo/repository.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.2.2/crud_repository.egg-info/PKG-INFO` & `crud_repository-0.2.3/crud_repository.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crud_repository
-Version: 0.2.2
+Version: 0.2.3
 Summary: The CRUDRepository is a Python project designed to provide a generic implementation of Create, Read, Update, and Delete (CRUD) operations for various databases.
 Home-page: https://github.com/dellius-alexander/CRUDRepository.git
 Author: Dellius Alexander
 Author-email: Dellius Alexander <dalexander@hyfisolutions.com>, info@hyfisolutions.com
 Maintainer-email: Dellius Alexander <dalexander@hyfisolutions.com>
 License: MIT License
```

### Comparing `crud_repository-0.2.2/crud_repository.egg-info/SOURCES.txt` & `crud_repository-0.2.3/crud_repository.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crud_repository-0.2.2/pyproject.toml` & `crud_repository-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "crud_repository"
-version = "0.2.2"
+version = "0.2.3"
 description = "The CRUDRepository is a Python project designed to provide a generic implementation of Create, Read, Update, and Delete (CRUD) operations for various databases."
 authors = [
   {name = "Dellius Alexander", email = "dalexander@hyfisolutions.com"},
   {email = "info@hyfisolutions.com"},
 ]
 maintainers = [
   {name = "Dellius Alexander", email = "dalexander@hyfisolutions.com"}
```

### Comparing `crud_repository-0.2.2/setup.py` & `crud_repository-0.2.3/setup.py`

 * *Files identical despite different names*

