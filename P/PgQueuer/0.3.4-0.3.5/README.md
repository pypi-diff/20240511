# Comparing `tmp/pgqueuer-0.3.4.tar.gz` & `tmp/pgqueuer-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgqueuer-0.3.4.tar", last modified: Wed May  8 07:44:15 2024, max compression
+gzip compressed data, was "pgqueuer-0.3.5.tar", last modified: Sat May 11 14:41:23 2024, max compression
```

## Comparing `pgqueuer-0.3.4.tar` & `pgqueuer-0.3.5.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:15.798206 pgqueuer-0.3.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:15.786206 pgqueuer-0.3.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:15.790207 pgqueuer-0.3.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-05-08 07:44:15.794206 pgqueuer-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 07:44:15.798206 pgqueuer-0.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:15.790207 pgqueuer-0.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:15.794206 pgqueuer-0.3.4/src/PgQueuer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/src/PgQueuer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/src/PgQueuer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/src/PgQueuer/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/src/PgQueuer/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/src/PgQueuer/logconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/src/PgQueuer/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/src/PgQueuer/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/src/PgQueuer/qm.py
--rw-r--r--   0 runner    (1001) docker     (127)    16242 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/src/PgQueuer/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/src/PgQueuer/tm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:15.794206 pgqueuer-0.3.4/src/PgQueuer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-05-08 07:44:15.000000 pgqueuer-0.3.4/src/PgQueuer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-08 07:44:15.000000 pgqueuer-0.3.4/src/PgQueuer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 07:44:15.000000 pgqueuer-0.3.4/src/PgQueuer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-08 07:44:15.000000 pgqueuer-0.3.4/src/PgQueuer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-08 07:44:15.000000 pgqueuer-0.3.4/src/PgQueuer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 07:44:15.000000 pgqueuer-0.3.4/src/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:15.794206 pgqueuer-0.3.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:15.794206 pgqueuer-0.3.4/test/db/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/test/db/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (127)      266 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/test/db/init_db.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/test/test_qm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/test/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/test/test_tm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:15.794206 pgqueuer-0.3.4/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/tools/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:41:23.566411 pgqueuer-0.3.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:41:23.558411 pgqueuer-0.3.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:41:23.558411 pgqueuer-0.3.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-05-11 14:41:23.566411 pgqueuer-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 14:41:23.566411 pgqueuer-0.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:41:23.558411 pgqueuer-0.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:41:23.562411 pgqueuer-0.3.5/src/PgQueuer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/src/PgQueuer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/src/PgQueuer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/src/PgQueuer/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6575 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/src/PgQueuer/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/src/PgQueuer/listeners.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/src/PgQueuer/logconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/src/PgQueuer/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/src/PgQueuer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/src/PgQueuer/qm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16242 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/src/PgQueuer/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/src/PgQueuer/tm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:41:23.566411 pgqueuer-0.3.5/src/PgQueuer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-05-11 14:41:23.000000 pgqueuer-0.3.5/src/PgQueuer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-11 14:41:23.000000 pgqueuer-0.3.5/src/PgQueuer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 14:41:23.000000 pgqueuer-0.3.5/src/PgQueuer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-11 14:41:23.000000 pgqueuer-0.3.5/src/PgQueuer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-11 14:41:23.000000 pgqueuer-0.3.5/src/PgQueuer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-11 14:41:23.000000 pgqueuer-0.3.5/src/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:41:23.562411 pgqueuer-0.3.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:41:23.562411 pgqueuer-0.3.5/test/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/test/db/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)      266 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/test/db/init_db.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/test/test_qm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/test/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/test/test_tm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:41:23.562411 pgqueuer-0.3.5/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/tools/benchmark.py
```

### Comparing `pgqueuer-0.3.4/.github/workflows/ci.yml` & `pgqueuer-0.3.5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.4/.github/workflows/linting.yml` & `pgqueuer-0.3.5/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.4/.github/workflows/release.yml` & `pgqueuer-0.3.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.4/.gitignore` & `pgqueuer-0.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.4/CONTRIBUTING.md` & `pgqueuer-0.3.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.4/LICENSE` & `pgqueuer-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.4/PKG-INFO` & `pgqueuer-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PgQueuer
-Version: 0.3.4
+Version: 0.3.5
 Summary: PgQueuer is a Python library leveraging PostgreSQL for efficient job queuing.
 Author: janbjorge
 License: MIT License
 Project-URL: Documentation, https://github.com/janbjorge/PgQueuer/wiki
 Project-URL: Homepage, https://github.com/janbjorge/PgQueuer/
 Project-URL: Issues, https://github.com/janbjorge/PgQueuer/issues
 Project-URL: Repository, https://github.com/janbjorge/PgQueuer/
@@ -24,15 +24,14 @@
 Classifier: Topic :: Utilities
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: anyio>=4.0
 Requires-Dist: asyncpg>=0.27.0
-Requires-Dist: pgcachewatch>=0.4
 Requires-Dist: pydantic>=2.0.0
 Requires-Dist: tabulate>=0.9.0
 Provides-Extra: dev
 Requires-Dist: asyncpg-stubs; extra == "dev"
 Requires-Dist: mypy-extensions; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
```

### Comparing `pgqueuer-0.3.4/README.md` & `pgqueuer-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.4/pyproject.toml` & `pgqueuer-0.3.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     "Topic :: Utilities",
     "Topic :: System :: Distributed Computing"
 ]
 
 dependencies = [
     "anyio>=4.0",
     "asyncpg>=0.27.0",
-    "pgcachewatch>=0.4",
     "pydantic>=2.0.0",
     "tabulate>=0.9.0",
 ]
 
 [project.urls]
 Documentation = "https://github.com/janbjorge/PgQueuer/wiki"
 Homepage = "https://github.com/janbjorge/PgQueuer/"
```

### Comparing `pgqueuer-0.3.4/src/PgQueuer/cli.py` & `pgqueuer-0.3.5/src/PgQueuer/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
             "environment variable if set"
         ),
         default=os.environ.get("PGPASSWORD"),
     )
 
     parser = argparse.ArgumentParser(
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-        prog="pgcachewatch",
+        prog="pgqueuer",
     )
 
     subparsers = parser.add_subparsers(
         dest="command",
         required=True,
     )
```

### Comparing `pgqueuer-0.3.4/src/PgQueuer/qm.py` & `pgqueuer-0.3.5/src/PgQueuer/qm.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,19 +13,18 @@
     TypeVar,
     overload,
 )
 
 import anyio
 import anyio.to_thread
 import asyncpg
-from pgcachewatch.listeners import PGEventQueue, _critical_termination_listener
-from pgcachewatch.models import PGChannel
 
+from .listeners import _critical_termination_listener, initialize_event_listener
 from .logconfig import logger
-from .models import Job
+from .models import Job, PGChannel
 from .queries import DBSettings, Queries
 from .tm import TaskManager
 
 if TYPE_CHECKING:
     AsyncEntrypoint: TypeAlias = Callable[[Job], Awaitable[None]]
     SyncEntrypoint: TypeAlias = Callable[[Job], None]
     Entrypoint: TypeAlias = AsyncEntrypoint | SyncEntrypoint
@@ -114,16 +113,15 @@
         Continuously listens for events and dispatches jobs. Manages connections and
         tasks, logs timeouts, and resets connections upon termination.
         """
         async with (
             self.pool.acquire() as connection,
             TaskManager() as tm,
         ):
-            listener = PGEventQueue()
-            await listener.connect(connection, self.channel)
+            listener = await initialize_event_listener(connection, self.channel)  # type: ignore[arg-type]
 
             while self.alive:
                 while self.alive and (job := await self.queries.dequeue()):
                     tm.add(asyncio.create_task(self._dispatch(job)))
 
                 try:
                     await asyncio.wait_for(
```

### Comparing `pgqueuer-0.3.4/src/PgQueuer/queries.py` & `pgqueuer-0.3.5/src/PgQueuer/queries.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.4/src/PgQueuer/tm.py` & `pgqueuer-0.3.5/src/PgQueuer/tm.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.4/src/PgQueuer.egg-info/PKG-INFO` & `pgqueuer-0.3.5/src/PgQueuer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PgQueuer
-Version: 0.3.4
+Version: 0.3.5
 Summary: PgQueuer is a Python library leveraging PostgreSQL for efficient job queuing.
 Author: janbjorge
 License: MIT License
 Project-URL: Documentation, https://github.com/janbjorge/PgQueuer/wiki
 Project-URL: Homepage, https://github.com/janbjorge/PgQueuer/
 Project-URL: Issues, https://github.com/janbjorge/PgQueuer/issues
 Project-URL: Repository, https://github.com/janbjorge/PgQueuer/
@@ -24,15 +24,14 @@
 Classifier: Topic :: Utilities
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: anyio>=4.0
 Requires-Dist: asyncpg>=0.27.0
-Requires-Dist: pgcachewatch>=0.4
 Requires-Dist: pydantic>=2.0.0
 Requires-Dist: tabulate>=0.9.0
 Provides-Extra: dev
 Requires-Dist: asyncpg-stubs; extra == "dev"
 Requires-Dist: mypy-extensions; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
```

### Comparing `pgqueuer-0.3.4/src/PgQueuer.egg-info/SOURCES.txt` & `pgqueuer-0.3.5/src/PgQueuer.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 .github/workflows/linting.yml
 .github/workflows/release.yml
 src/_version.py
 src/PgQueuer/__init__.py
 src/PgQueuer/__main__.py
 src/PgQueuer/_version.py
 src/PgQueuer/cli.py
+src/PgQueuer/listeners.py
 src/PgQueuer/logconfig.py
 src/PgQueuer/models.py
 src/PgQueuer/py.typed
 src/PgQueuer/qm.py
 src/PgQueuer/queries.py
 src/PgQueuer/tm.py
 src/PgQueuer.egg-info/PKG-INFO
```

### Comparing `pgqueuer-0.3.4/test/conftest.py` & `pgqueuer-0.3.5/test/conftest.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.4/test/db/Dockerfile` & `pgqueuer-0.3.5/test/db/Dockerfile`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.4/test/test_qm.py` & `pgqueuer-0.3.5/test/test_qm.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.4/test/test_queries.py` & `pgqueuer-0.3.5/test/test_queries.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.4/test/test_tm.py` & `pgqueuer-0.3.5/test/test_tm.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.4/tools/benchmark.py` & `pgqueuer-0.3.5/tools/benchmark.py`

 * *Files identical despite different names*

