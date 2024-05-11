# Comparing `tmp/gen3_tracker-0.0.4rc2.tar.gz` & `tmp/gen3_tracker-0.0.4rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen3_tracker-0.0.4rc2.tar", last modified: Sat May 11 18:17:12 2024, max compression
+gzip compressed data, was "gen3_tracker-0.0.4rc3.tar", last modified: Sat May 11 19:04:11 2024, max compression
```

## Comparing `gen3_tracker-0.0.4rc2.tar` & `gen3_tracker-0.0.4rc3.tar`

### file list

```diff
@@ -1,67 +1,22 @@
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 18:17:12.565878 gen3_tracker-0.0.4rc2/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1065 2023-05-04 14:32:05.000000 gen3_tracker-0.0.4rc2/LICENSE
--rw-r--r--   0 walsbr   (320923486) 1971611142     2409 2024-05-11 18:17:12.565310 gen3_tracker-0.0.4rc2/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     1524 2024-05-06 16:38:51.000000 gen3_tracker-0.0.4rc2/README.md
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 18:17:12.463900 gen3_tracker-0.0.4rc2/g3t/
--rw-r--r--   0 walsbr   (320923486) 1971611142     5965 2024-05-08 22:57:00.000000 gen3_tracker-0.0.4rc2/g3t/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2891 2024-05-02 01:38:13.000000 gen3_tracker-0.0.4rc2/g3t/cli.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 18:17:12.464690 gen3_tracker-0.0.4rc2/g3t/collaborator/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-10-19 18:09:26.000000 gen3_tracker-0.0.4rc2/g3t/collaborator/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 18:17:12.467361 gen3_tracker-0.0.4rc2/g3t/collaborator/access/
--rw-r--r--   0 walsbr   (320923486) 1971611142     3301 2024-04-27 12:56:43.000000 gen3_tracker-0.0.4rc2/g3t/collaborator/access/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     5079 2024-05-03 17:05:40.000000 gen3_tracker-0.0.4rc2/g3t/collaborator/access/cli.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 18:17:12.480759 gen3_tracker-0.0.4rc2/g3t/collaborator/access/policies/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:00:20.000000 gen3_tracker-0.0.4rc2/g3t/collaborator/access/policies/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      189 2024-02-29 16:26:49.000000 gen3_tracker-0.0.4rc2/g3t/collaborator/access/policies/add-project-default.yaml
--rw-r--r--   0 walsbr   (320923486) 1971611142       76 2024-02-26 20:40:22.000000 gen3_tracker-0.0.4rc2/g3t/collaborator/access/policies/add-user-read.yaml
--rw-r--r--   0 walsbr   (320923486) 1971611142      204 2024-05-09 02:02:53.000000 gen3_tracker-0.0.4rc2/g3t/collaborator/access/policies/add-user-write.yaml
--rw-r--r--   0 walsbr   (320923486) 1971611142     6802 2024-04-29 14:48:58.000000 gen3_tracker-0.0.4rc2/g3t/collaborator/access/requestor.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1105 2024-05-03 17:05:40.000000 gen3_tracker-0.0.4rc2/g3t/collaborator/access/submitter.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    13639 2024-05-09 22:58:55.000000 gen3_tracker-0.0.4rc2/g3t/collaborator/cli.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 18:17:12.484179 gen3_tracker-0.0.4rc2/g3t/common/
--rw-r--r--   0 walsbr   (320923486) 1971611142    18425 2024-05-06 14:21:17.000000 gen3_tracker-0.0.4rc2/g3t/common/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 18:17:12.485029 gen3_tracker-0.0.4rc2/g3t/config/
--rw-r--r--   0 walsbr   (320923486) 1971611142    10280 2024-04-29 04:46:34.000000 gen3_tracker-0.0.4rc2/g3t/config/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      137 2024-02-26 20:51:35.000000 gen3_tracker-0.0.4rc2/g3t/config.yaml
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 18:17:12.487134 gen3_tracker-0.0.4rc2/g3t/gen3/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2024-04-27 13:15:12.000000 gen3_tracker-0.0.4rc2/g3t/gen3/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 18:17:12.490714 gen3_tracker-0.0.4rc2/g3t/gen3/buckets/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1314 2024-04-25 20:19:51.000000 gen3_tracker-0.0.4rc2/g3t/gen3/buckets/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      883 2024-02-26 20:51:35.000000 gen3_tracker-0.0.4rc2/g3t/gen3/buckets/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      559 2024-02-26 20:51:35.000000 gen3_tracker-0.0.4rc2/g3t/gen3/buckets/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3345 2024-04-30 21:12:45.000000 gen3_tracker-0.0.4rc2/g3t/gen3/indexd.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4128 2024-04-29 13:40:35.000000 gen3_tracker-0.0.4rc2/g3t/gen3/jobs.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 18:17:12.499875 gen3_tracker-0.0.4rc2/g3t/git/
--rw-r--r--   0 walsbr   (320923486) 1971611142    20188 2024-05-06 16:23:20.000000 gen3_tracker-0.0.4rc2/g3t/git/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    11558 2024-05-08 22:16:58.000000 gen3_tracker-0.0.4rc2/g3t/git/adder.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    31775 2024-05-09 02:03:59.000000 gen3_tracker-0.0.4rc2/g3t/git/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2499 2024-05-01 18:43:40.000000 gen3_tracker-0.0.4rc2/g3t/git/cloner.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1439 2024-05-03 17:05:40.000000 gen3_tracker-0.0.4rc2/g3t/git/initializer.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2555 2024-05-02 22:49:35.000000 gen3_tracker-0.0.4rc2/g3t/git/snapshotter.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 18:17:12.507229 gen3_tracker-0.0.4rc2/g3t/meta/
--rw-r--r--   0 walsbr   (320923486) 1971611142     5915 2024-05-03 04:59:19.000000 gen3_tracker-0.0.4rc2/g3t/meta/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4907 2024-05-03 19:09:24.000000 gen3_tracker-0.0.4rc2/g3t/meta/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    13471 2024-05-03 19:08:14.000000 gen3_tracker-0.0.4rc2/g3t/meta/dataframer.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    11125 2024-05-03 17:05:40.000000 gen3_tracker-0.0.4rc2/g3t/meta/skeleton.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4419 2024-04-22 22:58:13.000000 gen3_tracker-0.0.4rc2/g3t/meta/validator.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1202 2024-04-28 11:58:11.000000 gen3_tracker-0.0.4rc2/g3t/meta/visualizer.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 18:17:12.544280 gen3_tracker-0.0.4rc2/g3t/projects/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2772 2024-04-26 19:19:19.000000 gen3_tracker-0.0.4rc2/g3t/projects/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4745 2024-05-09 02:02:53.000000 gen3_tracker-0.0.4rc2/g3t/projects/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2393 2024-05-03 17:05:40.000000 gen3_tracker-0.0.4rc2/g3t/projects/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1548 2024-05-03 17:05:40.000000 gen3_tracker-0.0.4rc2/g3t/projects/remover.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 18:17:12.564454 gen3_tracker-0.0.4rc2/gen3_tracker.egg-info/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2409 2024-05-11 18:17:12.000000 gen3_tracker-0.0.4rc2/gen3_tracker.egg-info/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     1327 2024-05-11 18:17:12.000000 gen3_tracker-0.0.4rc2/gen3_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142        1 2024-05-11 18:17:12.000000 gen3_tracker-0.0.4rc2/gen3_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       36 2024-05-11 18:17:12.000000 gen3_tracker-0.0.4rc2/gen3_tracker.egg-info/entry_points.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142      219 2024-05-11 18:17:12.000000 gen3_tracker-0.0.4rc2/gen3_tracker.egg-info/requires.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142        4 2024-05-11 18:17:12.000000 gen3_tracker-0.0.4rc2/gen3_tracker.egg-info/top_level.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       38 2024-05-11 18:17:12.565930 gen3_tracker-0.0.4rc2/setup.cfg
--rw-r--r--   0 walsbr   (320923486) 1971611142      723 2024-05-11 18:16:51.000000 gen3_tracker-0.0.4rc2/setup.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 18:17:12.448832 gen3_tracker-0.0.4rc2/tests/
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 18:17:12.563924 gen3_tracker-0.0.4rc2/tests/unit/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2024-05-02 22:49:35.000000 gen3_tracker-0.0.4rc2/tests/unit/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    20363 2024-05-01 22:45:46.000000 gen3_tracker-0.0.4rc2/tests/unit/test_flatten_fhir_example.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1267 2024-04-30 17:33:26.000000 gen3_tracker-0.0.4rc2/tests/unit/test_hash_types.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      592 2024-04-30 18:17:55.000000 gen3_tracker-0.0.4rc2/tests/unit/test_read_dvc.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 19:04:11.693314 gen3_tracker-0.0.4rc3/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1065 2023-05-04 14:32:05.000000 gen3_tracker-0.0.4rc3/LICENSE
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2369 2024-05-11 19:04:11.692799 gen3_tracker-0.0.4rc3/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1524 2024-05-06 16:38:51.000000 gen3_tracker-0.0.4rc3/README.md
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 19:04:11.674321 gen3_tracker-0.0.4rc3/gen3_tracker/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5974 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc3/gen3_tracker/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2963 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc3/gen3_tracker/cli.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 19:04:11.692115 gen3_tracker-0.0.4rc3/gen3_tracker.egg-info/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2369 2024-05-11 19:04:11.000000 gen3_tracker-0.0.4rc3/gen3_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142      410 2024-05-11 19:04:11.000000 gen3_tracker-0.0.4rc3/gen3_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142        1 2024-05-11 19:04:11.000000 gen3_tracker-0.0.4rc3/gen3_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       45 2024-05-11 19:04:11.000000 gen3_tracker-0.0.4rc3/gen3_tracker.egg-info/entry_points.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142      209 2024-05-11 19:04:11.000000 gen3_tracker-0.0.4rc3/gen3_tracker.egg-info/requires.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       13 2024-05-11 19:04:11.000000 gen3_tracker-0.0.4rc3/gen3_tracker.egg-info/top_level.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       38 2024-05-11 19:04:11.693376 gen3_tracker-0.0.4rc3/setup.cfg
+-rw-r--r--   0 walsbr   (320923486) 1971611142      741 2024-05-11 19:03:05.000000 gen3_tracker-0.0.4rc3/setup.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 19:04:11.669513 gen3_tracker-0.0.4rc3/tests/
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 19:04:11.691478 gen3_tracker-0.0.4rc3/tests/unit/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2024-05-02 22:49:35.000000 gen3_tracker-0.0.4rc3/tests/unit/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    20363 2024-05-01 22:45:46.000000 gen3_tracker-0.0.4rc3/tests/unit/test_flatten_fhir_example.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1285 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc3/tests/unit/test_hash_types.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      601 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc3/tests/unit/test_read_dvc.py
```

### Comparing `gen3_tracker-0.0.4rc2/LICENSE` & `gen3_tracker-0.0.4rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc2/PKG-INFO` & `gen3_tracker-0.0.4rc3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen3_tracker
-Version: 0.0.4rc2
+Version: 0.0.4rc3
 Summary: A CLI for adding version control to Gen3 data submission projects.
 Home-page: https://github.com/ACED-IDP/g3t-git
 Author: walsbr
 Author-email: walsbr@ohsu.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
@@ -14,22 +14,20 @@
 Requires-Dist: tqdm
 Requires-Dist: deepdiff
 Requires-Dist: fhir.resources==7.1.0
 Requires-Dist: orjson
 Requires-Dist: nested_lookup
 Requires-Dist: gen3
 Requires-Dist: PyJWT==2.8.0
-Requires-Dist: g3t
 Requires-Dist: pydantic
 Requires-Dist: requests
 Requires-Dist: pandas
 Requires-Dist: matplotlib==3.8.4
 Requires-Dist: numpy
 Requires-Dist: pyvis==0.3.2
-Requires-Dist: dtale
 Requires-Dist: ndjson
 Requires-Dist: inflection
 Requires-Dist: python-dateutil
 Provides-Extra: dtale
 Requires-Dist: dtale; extra == "dtale"
```

### Comparing `gen3_tracker-0.0.4rc2/README.md` & `gen3_tracker-0.0.4rc3/README.md`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc2/g3t/__init__.py` & `gen3_tracker-0.0.4rc3/gen3_tracker/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         # print('resolve_command', args)
         try:
             return super().resolve_command(ctx, args)
         except Exception as e:
             if 'No such command' in str(e):
                 # delegate to git
                 try:
-                    from g3t.git import run_command
+                    from gen3_tracker.git import run_command
                     result = run_command(f'git {" ".join(args)}', dry_run=False, no_capture=True)
                     sys.exit(result.return_code)
                     # os._exit(result.return_code)  # noqa
                 except subprocess.CalledProcessError as e2:
                     # os._exit(e2.returncode)  # noqa
                     sys.exit(e2.returncode)
```

### Comparing `gen3_tracker-0.0.4rc2/g3t/cli.py` & `gen3_tracker-0.0.4rc3/gen3_tracker/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import logging
 import sys
 
 import click
 
-import g3t
-from g3t import NaturalOrderGroup, ENV_VARIABLE_PREFIX
-from g3t.collaborator.cli import collaborator
-from g3t.config import gen3_client_profiles
-from g3t.git.cli import cli as git
-from g3t.meta.cli import meta
-from g3t.projects.cli import project_group as project
+import gen3_tracker
+from gen3_tracker import NaturalOrderGroup, ENV_VARIABLE_PREFIX
+from gen3_tracker.collaborator.cli import collaborator
+from gen3_tracker.config import gen3_client_profiles
+from gen3_tracker.git.cli import cli as git
+from gen3_tracker.meta.cli import meta
+from gen3_tracker.projects.cli import project_group as project
 
 logging.basicConfig(level=logging.INFO)
 _logger = logging.getLogger(__package__)
 
 
 @click.group(cls=NaturalOrderGroup)
 @click.option('--format', 'output_format',
@@ -31,15 +31,15 @@
               )
 @click.option('--debug', is_flag=True, envvar='G3T_DEBUG', help='Enable debug mode. G3T_DEBUG environment variable can also be used.')
 @click.option('--dry-run', is_flag=True, envvar='G3T_DRYRUN', help='Print the commands that would be executed, but do not execute them. G3T_DRYRUN environment variable can also be used.')
 @click.version_option()
 @click.pass_context
 def cli(ctx: click.Context, output_format: str, profile: str, debug: bool, dry_run: bool):
     """A CLI for adding version control to Gen3 projects."""
-    config__ = g3t.config.default()
+    config__ = gen3_tracker.config.default()
     logging.basicConfig(format=config__.log.format, level=config__.log.level, stream=sys.stderr)
 
     if output_format:
         config__.output.format = output_format
 
     _profiles = gen3_client_profiles()
     is_help = '--help' in sys.argv[1:]
```

### Comparing `gen3_tracker-0.0.4rc2/gen3_tracker.egg-info/PKG-INFO` & `gen3_tracker-0.0.4rc3/gen3_tracker.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen3_tracker
-Version: 0.0.4rc2
+Version: 0.0.4rc3
 Summary: A CLI for adding version control to Gen3 data submission projects.
 Home-page: https://github.com/ACED-IDP/g3t-git
 Author: walsbr
 Author-email: walsbr@ohsu.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
@@ -14,22 +14,20 @@
 Requires-Dist: tqdm
 Requires-Dist: deepdiff
 Requires-Dist: fhir.resources==7.1.0
 Requires-Dist: orjson
 Requires-Dist: nested_lookup
 Requires-Dist: gen3
 Requires-Dist: PyJWT==2.8.0
-Requires-Dist: g3t
 Requires-Dist: pydantic
 Requires-Dist: requests
 Requires-Dist: pandas
 Requires-Dist: matplotlib==3.8.4
 Requires-Dist: numpy
 Requires-Dist: pyvis==0.3.2
-Requires-Dist: dtale
 Requires-Dist: ndjson
 Requires-Dist: inflection
 Requires-Dist: python-dateutil
 Provides-Extra: dtale
 Requires-Dist: dtale; extra == "dtale"
```

### Comparing `gen3_tracker-0.0.4rc2/setup.py` & `gen3_tracker-0.0.4rc3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,25 +4,25 @@
     requirements = f.read().splitlines()
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='gen3_tracker',
-    version='0.0.4rc2',
+    version='0.0.4rc3',
     description='A CLI for adding version control to Gen3 data submission projects.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='walsbr',
     author_email='walsbr@ohsu.edu',
     url='https://github.com/ACED-IDP/g3t-git',
-    packages=['g3t'],
+    packages=['gen3_tracker'],
     install_requires=requirements,
     extras_require={
         'dtale': ['dtale'],
     },
     entry_points={
         'console_scripts': [
-            'g3t=g3t.cli:cli',
+            'g3t=gen3_tracker.cli:cli',
         ],
     },
 )
```

### Comparing `gen3_tracker-0.0.4rc2/tests/unit/test_flatten_fhir_example.py` & `gen3_tracker-0.0.4rc3/tests/unit/test_flatten_fhir_example.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc2/tests/unit/test_hash_types.py` & `gen3_tracker-0.0.4rc3/tests/unit/test_hash_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 from pydantic import ValidationError
 
-from g3t.common import ACCEPTABLE_HASHES
-from g3t.git import DVCItem
+from gen3_tracker.common import ACCEPTABLE_HASHES
+from gen3_tracker.git import DVCItem
 
 VALID_HASHES = {
     'md5': 'acbd18db4cc2f85cedef654fccc4a4d8',
     'sha1': '2ef7bde608ce5404e97d5f042f95f89f1c232871',
     'sha256': '5bf8aa57fc5a6bc547decf1cc6db63f10deb55a3c6c5df497d631fb3d95e1abf',
     'sha512': '3ba2942ed1d05551d4360a2a7bb6298c2359061dc07b368949bd3fb7feca3344221257672d772ce456075b7cfa50fd7ce41eaefe529d056bf23dd665de668b78',
     'crc': '3e25960a',
```

### Comparing `gen3_tracker-0.0.4rc2/tests/unit/test_read_dvc.py` & `gen3_tracker-0.0.4rc3/tests/unit/test_read_dvc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from g3t.git import to_dvc, DVCItem
+from gen3_tracker.git import to_dvc, DVCItem
 
 
 def test_read_dvc():
     dvc = to_dvc('tests/fixtures/hello.txt.dvc')
     assert dvc
     assert dvc.outs
     assert dvc.outs[0].path == 'my-project-data/hello.txt'
```

