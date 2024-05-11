# Comparing `tmp/ezomero-2.1.0.tar.gz` & `tmp/ezomero-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezomero-2.1.0.tar", last modified: Wed Sep 13 13:50:17 2023, max compression
+gzip compressed data, was "ezomero-3.0.0.tar", last modified: Wed Apr  3 13:40:36 2024, max compression
```

## Comparing `ezomero-2.1.0.tar` & `ezomero-3.0.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 13:50:17.942172 ezomero-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    17987 2023-09-13 13:50:04.000000 ezomero-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2023-09-13 13:50:17.942172 ezomero-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2023-09-13 13:50:04.000000 ezomero-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 13:50:17.938172 ezomero-2.1.0/ezomero/
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2023-09-13 13:50:04.000000 ezomero-2.1.0/ezomero/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16015 2023-09-13 13:50:04.000000 ezomero-2.1.0/ezomero/_ezomero.py
--rw-r--r--   0 runner    (1001) docker     (127)    48793 2023-09-13 13:50:04.000000 ezomero-2.1.0/ezomero/_gets.py
--rw-r--r--   0 runner    (1001) docker     (127)    18741 2023-09-13 13:50:04.000000 ezomero-2.1.0/ezomero/_importer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11052 2023-09-13 13:50:04.000000 ezomero-2.1.0/ezomero/_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    29317 2023-09-13 13:50:04.000000 ezomero-2.1.0/ezomero/_posts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9234 2023-09-13 13:50:04.000000 ezomero-2.1.0/ezomero/json_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    18974 2023-09-13 13:50:04.000000 ezomero-2.1.0/ezomero/rois.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 13:50:17.938172 ezomero-2.1.0/ezomero.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2023-09-13 13:50:17.000000 ezomero-2.1.0/ezomero.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      555 2023-09-13 13:50:17.000000 ezomero-2.1.0/ezomero.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-13 13:50:17.000000 ezomero-2.1.0/ezomero.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-09-13 13:50:17.000000 ezomero-2.1.0/ezomero.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-09-13 13:50:17.000000 ezomero-2.1.0/ezomero.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-13 13:50:17.942172 ezomero-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      810 2023-09-13 13:50:04.000000 ezomero-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 13:50:17.942172 ezomero-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-13 13:50:04.000000 ezomero-2.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21977 2023-09-13 13:50:04.000000 ezomero-2.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2023-09-13 13:50:04.000000 ezomero-2.1.0/tests/test_connect.py
--rw-r--r--   0 runner    (1001) docker     (127)     4341 2023-09-13 13:50:04.000000 ezomero-2.1.0/tests/test_ezimport.py
--rw-r--r--   0 runner    (1001) docker     (127)    22995 2023-09-13 13:50:04.000000 ezomero-2.1.0/tests/test_gets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2023-09-13 13:50:04.000000 ezomero-2.1.0/tests/test_json_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8035 2023-09-13 13:50:04.000000 ezomero-2.1.0/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    21933 2023-09-13 13:50:04.000000 ezomero-2.1.0/tests/test_posts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2023-09-13 13:50:04.000000 ezomero-2.1.0/tests/test_puts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2023-09-13 13:50:04.000000 ezomero-2.1.0/tests/test_rois.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2023-09-13 13:50:04.000000 ezomero-2.1.0/tests/test_users_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:40:36.181206 ezomero-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    17987 2024-04-03 13:40:26.000000 ezomero-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-03 13:40:36.181206 ezomero-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-03 13:40:26.000000 ezomero-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:40:36.177206 ezomero-3.0.0/ezomero/
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-03 13:40:26.000000 ezomero-3.0.0/ezomero/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16015 2024-04-03 13:40:26.000000 ezomero-3.0.0/ezomero/_ezomero.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48793 2024-04-03 13:40:26.000000 ezomero-3.0.0/ezomero/_gets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18788 2024-04-03 13:40:26.000000 ezomero-3.0.0/ezomero/_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11052 2024-04-03 13:40:26.000000 ezomero-3.0.0/ezomero/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29902 2024-04-03 13:40:26.000000 ezomero-3.0.0/ezomero/_posts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-04-03 13:40:26.000000 ezomero-3.0.0/ezomero/json_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18974 2024-04-03 13:40:26.000000 ezomero-3.0.0/ezomero/rois.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:40:36.177206 ezomero-3.0.0/ezomero.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-03 13:40:35.000000 ezomero-3.0.0/ezomero.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-03 13:40:36.000000 ezomero-3.0.0/ezomero.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:40:35.000000 ezomero-3.0.0/ezomero.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 13:40:35.000000 ezomero-3.0.0/ezomero.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 13:40:35.000000 ezomero-3.0.0/ezomero.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 13:40:36.181206 ezomero-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-03 13:40:26.000000 ezomero-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:40:36.181206 ezomero-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:40:26.000000 ezomero-3.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21978 2024-04-03 13:40:26.000000 ezomero-3.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-03 13:40:26.000000 ezomero-3.0.0/tests/test_connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-04-03 13:40:26.000000 ezomero-3.0.0/tests/test_ezimport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23186 2024-04-03 13:40:26.000000 ezomero-3.0.0/tests/test_gets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-03 13:40:26.000000 ezomero-3.0.0/tests/test_json_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-04-03 13:40:26.000000 ezomero-3.0.0/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23155 2024-04-03 13:40:26.000000 ezomero-3.0.0/tests/test_posts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-03 13:40:26.000000 ezomero-3.0.0/tests/test_puts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-04-03 13:40:26.000000 ezomero-3.0.0/tests/test_rois.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-03 13:40:26.000000 ezomero-3.0.0/tests/test_users_group.py
```

### Comparing `ezomero-2.1.0/LICENSE` & `ezomero-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ezomero-2.1.0/PKG-INFO` & `ezomero-3.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ezomero
-Version: 2.1.0
+Version: 3.0.0
 Summary: A suite of convenience functions for working with OMERO. Written and maintained by the Research IT team at The Jackson Laboratory.
 Home-page: https://github.com/TheJacksonLaboratory/ezomero
 Maintainer: Dave Mellert
 Maintainer-email: Dave.Mellert@jax.org
 License: UNKNOWN
-Description: ![Run Tests](https://github.com/TheJacksonLaboratory/ezomero/workflows/Run%20Tests/badge.svg?event=push) ![](https://raw.githubusercontent.com/TheJacksonLaboratory/ezomero/main/coverage.svg)
+Description: ![](https://raw.githubusercontent.com/TheJacksonLaboratory/ezomero/main/coverage.svg) [![badge-doi](https://img.shields.io/badge/doi-10.1101%2F2023.06.29.546930-purple)](https://doi.org/10.1101/2023.06.29.546930) 
         
         # ezomero
         A module with convenience functions for writing Python code that interacts with OMERO.
         
         
         # Installation
         
@@ -23,11 +23,31 @@
         In general, you will need to create a `BlitzGateway` object using `ezomero.connect()`, then pass the `conn` object to most of these helper functions along with function-specific parameters.
         
         
         # Documentation
         
         Documentation is available at https://thejacksonlaboratory.github.io/ezomero/
         
+        # Development
+        
+        You will need Docker installed and running to run the tests.
+        
+        Setup your "omero" python environment with a local ezomero and pytest:
+        ```
+        > conda activate omero  # Activate your omero environment with conda or pip
+        (omero) > cd /your_local_clone/ezomero
+        (omero) > pip install -e .
+        (omero) > pip install pytest
+        ```
+        
+        To run the tests, startup the test OMERO server with Docker and run pytest
+        ```
+        > cd /your_local_clone/ezomero
+        > docker-compose -f tests/docker-compose.yml up -d
+        > conda activate omero
+        (omero) > python -m pytest .\tests
+        ```
+        
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tables
```

### Comparing `ezomero-2.1.0/ezomero/__init__.py` & `ezomero-3.0.0/ezomero/__init__.py`

 * *Files identical despite different names*

### Comparing `ezomero-2.1.0/ezomero/_ezomero.py` & `ezomero-3.0.0/ezomero/_ezomero.py`

 * *Files identical despite different names*

### Comparing `ezomero-2.1.0/ezomero/_gets.py` & `ezomero-3.0.0/ezomero/_gets.py`

 * *Files identical despite different names*

### Comparing `ezomero-2.1.0/ezomero/_importer.py` & `ezomero-3.0.0/ezomero/_importer.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,51 +15,56 @@
 
 
 # import
 def ezimport(conn: BlitzGateway, target: str,
              project: Optional[Union[str, int]] = None,
              dataset: Optional[Union[str, int]] = None,
              screen: Optional[Union[str, int]] = None,
-             ln_s: Optional[bool] = False, ann: Optional[dict] = None,
-             ns: Optional[str] = None) -> Union[List[int], None]:
+             ann: Optional[dict] = None,
+             ns: Optional[str] = None, *args: str,
+             **kwargs: str
+             ) -> Union[List[int], None]:
     """Entry point that creates Importer and runs import.
 
     Parameters
     ----------
     conn : ``omero.gateway.BlitzGateway`` object.
         OMERO connection.
     target : string
         Path to the import target to be imported into OMERO.
     project : str or int, optional
         The name or ID of the Project data will be imported into.
     dataset : str or int, optional
         The name or ID of the Dataset data will be imported into.
     screen : str or int, optional
         The name or ID of the Screen data will be imported into.
-    ln_s : boolean, optional
-        Whether to use ``ln_s`` softlinking during imports or not.
     ann : dict, optional
         Dictionary with key-value pairs to be added to imported images.
     ns : str, optional
         Namespace for the added key-value pairs.
+    *args, **kwargs : str, optional
+        You can also add any extra arguments you would like to pass to
+        ``omero import`` to the end of the argument list in ``ezimport``.
+        For example, an in-place import can be done by adding
+        ``transfer="ln_s"`` as an extra argument when calling `ezimport``.
 
     Returns
     -------
     plate_ids or image_ids : list of ints
         The ids of the Images/Plates that were generated by importing the
         specified target.
 
     Notes
     -------
     This function is EXPERIMENTAL and has seen minimal testing. Use at
     your own risk! We do not recommend using this in production.
     """
 
     imp_ctl = Importer(conn, target, project, dataset, screen,
-                       ln_s, ann, ns)
+                       ann, ns, *args, **kwargs)
     imp_ctl.ezimport()
     if imp_ctl.screen:
         imp_ctl.get_plate_ids()
         imp_ctl.organize_plates()
         imp_ctl.annotate_plates()
         return imp_ctl.plate_ids
 
@@ -230,24 +235,25 @@
         Path to the import target to be imported into OMERO.
     project : str or int, optional
         The name or ID of the Project data will be imported into.
     dataset : str or int, optional
         The name or ID of the Dataset data will be imported into.
     screen : str or int, optional
         The name or ID of the Screen data will be imported into.
-    ln_s : boolean, optional
-        Whether to use ``ln_s`` softlinking during imports or not.
     ann : dict, optional
         Dictionary with key-value pairs to be added to imported images.
     ns : str, optional
         Namespace for the added key-value pairs.
     host : str, optional
         Hostname of the OMERO server to which data will be imported.
     port : int, optional
         Port of the OMERO server to which data will be imported.
+    *args, **kwargs : str, optional
+        Receives the ``*args``, ``**kwargs`` from ``ezimport`` to pass it
+        onto ``omero import``.
 
     Important notes:
     1) Setting ``project`` also requires setting ``dataset``. Failing to do so
     will raise a ValueError.
     2) To annotate images, both ``ann`` and ``ns`` need to be set. If one of
     them is not set, no annotations will be made.
     3) For automating purposes, the arguments ``host`` and ``port`` can be set,
@@ -260,28 +266,30 @@
     getting more image IDs than you were expecting!
     """
 
     def __init__(self, conn: BlitzGateway, file_path: str,
                  project: Optional[Union[str, int]],
                  dataset: Optional[Union[str, int]],
                  screen: Optional[Union[str, int]],
-                 ln_s: Optional[bool], ann: Optional[dict],
-                 ns: Optional[str]):
+                 ann: Optional[dict],
+                 ns: Optional[str], *args, **kwargs):
         self.conn = conn
         self.file_path = abspath(file_path)
         self.session_uuid = conn.getSession().getUuid().val
         self.project = project
         self.dataset = dataset
+        self.common_args = args
+        self.named_args = kwargs
+
         if self.project and not self.dataset:
             raise ValueError("Cannot define project but no dataset!")
         self.screen = screen
         self.imported = False
         self.image_ids: Union[List[int], None] = None
         self.plate_ids: Union[List[int], None] = None
-        self.ln_s = ln_s
         self.ann = ann
         self.ns = ns
 
     def get_my_image_ids(self) -> Union[List[int], None]:
         """Get the Ids of imported images.
 
         Note that this will not find images if they have not been imported.
@@ -297,14 +305,16 @@
             logging.error(f'File {self.file_path} has not been imported')
             return None
         else:
             q = self.conn.getQueryService()
             params = Parameters()
             path_query = self.make_substitutions()
             path_query = path_query.strip('/')
+            if path_query.endswith(".zarr"):
+                path_query = f"{path_query}/.zattrs"
             params.map = {"cpath": rstring(path_query)}
             results = q.projection(
                 "SELECT i.id FROM Image i"
                 " JOIN i.fileset fs"
                 " JOIN fs.usedFiles u"
                 " WHERE u.clientPath=:cpath",
                 params,
@@ -449,58 +459,44 @@
                 if self.screen:
                     screen_id = set_or_create_screen(self.conn, self.screen)
                     link_plates_to_screen(self.conn, [pl_id], screen_id)
                     print(f'Moved Plate:{pl_id} to Screen:{screen_id}')
             return True
         return False
 
-    def ezimport_ln_s(self) -> bool:
-        """Import file using the ``--transfer=ln_s`` option.
+    def ezimport(self) -> bool:
+        """Import file.
         Returns
         -------
         import_status : boolean
             True if OMERO import returns a 0 exit status, else False.
         """
-
+        args = ""
+        if self.common_args:
+            args = args + " ".join(self.common_args)
+        if self.named_args:
+            for k, v in self.named_args.items():
+                args = args + " " + str(k) + "=" + str(v)
         cli = CLI()
         cli.register('import', ImportControl, '_')
         cli.register('sessions', SessionsControl, '_')
-        cli.invoke(['import',
-                    '-k', self.conn.getSession().getUuid().val,
-                    '-s', self.conn.host,
-                    '-p', str(self.conn.port),
-                    '--transfer', 'ln_s',
-                    str(self.file_path)])
-        if cli.rv == 0:
-            self.imported = True
-            print(f'Imported {self.file_path}')
-            return True
-        else:
-            logging.error(f'Import of {self.file_path} has failed!')
-            return False
-
-    def ezimport(self) -> bool:
-        """Import file.
-        Returns
-        -------
-        import_status : boolean
-            True if OMERO import returns a 0 exit status, else False.
-        """
-        if self.ln_s:
-            rs = self.ezimport_ln_s()
-            return rs
-        else:
-            cli = CLI()
-            cli.register('import', ImportControl, '_')
-            cli.register('sessions', SessionsControl, '_')
-            cli.invoke(['import',
-                        '-k', self.conn.getSession().getUuid().val,
-                        '-s', self.conn.host,
-                        '-p', str(self.conn.port),
-                        str(self.file_path)])
+        arguments = ['import',
+                     '-k', self.conn.getSession().getUuid().val,
+                     '-s', self.conn.host,
+                     '-p', str(self.conn.port)]
+        if self.common_args:
+            str_args = ['--{}'.format(v) for v in self.common_args]
+            arguments.extend(str_args)
+        if self.named_args:
+            str_kwargs = ['--{}={}'.format(k, v) for k, v in
+                          self.named_args.items()]
+            arguments.extend(str_kwargs)
+        arguments.append(str(self.file_path))
+        print(arguments)
+        cli.invoke(arguments)
         if cli.rv == 0:
             self.imported = True
             print(f'Imported {self.file_path}')
             return True
         else:
             logging.error(f'Import of {self.file_path} has failed!')
             return False
```

### Comparing `ezomero-2.1.0/ezomero/_misc.py` & `ezomero-3.0.0/ezomero/_misc.py`

 * *Files identical despite different names*

### Comparing `ezomero-2.1.0/ezomero/_posts.py` & `ezomero-3.0.0/ezomero/_posts.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from omero.grid import BoolColumn, LongColumn
 from omero.grid import StringColumn, DoubleColumn, Column
 from omero.gateway import ProjectWrapper, DatasetWrapper
 from omero.gateway import ScreenWrapper, FileAnnotationWrapper
 from omero.gateway import MapAnnotationWrapper, OriginalFileWrapper
 from omero.gateway import CommentAnnotationWrapper
 from omero.rtypes import rstring, rint, rdouble
+from omero import SecurityViolation
 from .rois import Point, Line, Rectangle, Ellipse
 from .rois import Polygon, Polyline, Label
 import importlib.util
 
 if (importlib.util.find_spec('pandas')):
     import pandas as pd
     has_pandas = True
@@ -92,16 +93,24 @@
     dataset = DatasetWrapper(conn, DatasetI())
     dataset.setName(dataset_name)
     if description is not None:
         dataset.setDescription(description)
     dataset.save()
 
     if project_id is not None:
-        link_datasets_to_project(conn, [dataset.getId()], project_id)
-    return dataset.getId()
+        try:
+            link_datasets_to_project(conn, [dataset.getId()], project_id)
+            return dataset.getId()
+        except SecurityViolation:
+            logging.warning('You do not have permission to create new '
+                            f'datasets in project {project_id}.')
+            conn.deleteObject("Dataset", dataset.getId())
+            return None
+    else:
+        return dataset.getId()
 
 
 def post_image(conn: BlitzGateway, image: np.ndarray, image_name: str,
                description: Optional[str] = None,
                dataset_id: Optional[int] = None,
                source_image_id: Optional[int] = None,
                channel_list: Optional[List[int]] = None,
@@ -372,86 +381,88 @@
                         'check if you have permissions to do so')
         return None
 
     return comment_ann.getId()
 
 
 @do_across_groups
-def post_file_annotation(conn: BlitzGateway, object_type: str, object_id: int,
+def post_file_annotation(conn: BlitzGateway,
                          file_path: str, ns: str,
+                         object_type: Optional[str] = None,
+                         object_id: Optional[int] = None,
                          mimetype: Optional[str] = None,
                          description: Optional[str] = None,
                          across_groups: Optional[bool] = True
                          ) -> Union[int, None]:
     """Create new FileAnnotation and link to images.
 
     Parameters
     ----------
     conn : ``omero.gateway.BlitzGateway`` object
         OMERO connection.
-    object_type : str
-       OMERO object type, passed to ``BlitzGateway.getObjects``
-    object_ids : int
-        ID of object to which the new MapAnnotation will be linked.
     file_path : string
         local path to file to be added as FileAnnotation
     ns : str
         Namespace for the FileAnnotation
-    mimetype : str
+    object_type : str, optional
+       OMERO object type, passed to ``BlitzGateway.getObject``
+    object_id : int, optional
+        ID of object to which the new FileAnnotation will be linked.
+    mimetype : str, optional
         String of the form 'type/subtype', usable for a MIME content-type
         header.
-    description : str
+    description : str, optional
         File description to be added to FileAnnotation
     across_groups : bool, optional
         Defines cross-group behavior of function - set to
         ``False`` to disable it.
 
     Notes
     -----
     All keys and values are converted to strings before saving in OMERO.
 
     Returns
     -------
     file_ann_id : int
-        IDs of newly created MapAnnotation
+        IDs of newly created FileAnnotation
 
     Examples
     --------
     >>> ns = 'jax.org/jax/example/namespace'
     >>> path = '/home/user/Downloads/file_ann.txt'
-    >>> post_file_annotation(conn, "Image", 56, path, ns)
+    >>> post_file_annotation(conn, path, ns, "Image", 56)
     234
     """
 
     if type(file_path) is not str:
         raise TypeError('file_path must be of type `str`')
 
     obj = None
-    if object_id is not None:
+    if object_id is not None and object_type is not None:
         if type(object_id) is not int:
             raise TypeError('object_ids must be integer')
         obj = conn.getObject(object_type, object_id)
         if obj is not None:
             ret = set_group(conn, obj.getDetails().group.id.val)
             if ret is False:
                 logging.warning('Cannot change into group '
                                 f'where object {object_id} is.')
                 return None
         else:
             logging.warning(f'Object {object_id} could not be found '
                             '(check if you have permissions to it)')
             return None
     else:
-        raise TypeError('Object ID cannot be empty')
+        set_group(conn, conn.getGroupFromContext().id)
     if not mimetype:
         mimetype, _ = mimetypes.guess_type(file_path)
     file_ann = conn.createFileAnnfromLocalFile(
         file_path, mimetype=mimetype, ns=ns, desc=description)
-    obj.linkAnnotation(file_ann)
-
+    if object_id is not None and object_type is not None:
+        obj.linkAnnotation(file_ann)
     return file_ann.getId()
 
 
 def post_project(conn: BlitzGateway, project_name: str,
                  description: Optional[str] = None) -> int:
     """Create a new project.
 
@@ -685,15 +696,15 @@
     return file_ann.id
 
 
 def create_columns(table: Any,
                    headers: bool) -> List[Column]:
     """Helper function to create the correct column types from a table"""
     cols = []
-    if type(table) == list:
+    if isinstance(table, list):
         if headers:
             titles = table[0]
             data = table[1:]
         else:
             titles = [f"column {i}" for i in range(len(table[0]))]
             data = table
         # transposing data matrix to have columns as first dimension
@@ -708,15 +719,15 @@
                 cols.append(LongColumn(titles[i], '', data[i]))
             if types[0] == float:
                 cols.append(DoubleColumn(titles[i], '', data[i]))
             if types[0] == str:
                 max_size = len(max(data[i], key=len))
                 cols.append(StringColumn(titles[i], '',
                             max_size, data[i]))
-    elif type(table) == pd.core.frame.DataFrame:
+    elif isinstance(table, pd.core.frame.DataFrame):
         df = table.convert_dtypes()
         ints = df.select_dtypes(include='int')
         for col in ints:
             cols.append(LongColumn(col, '', df[col].tolist()))
         floats = df.select_dtypes(include='float')
         for col in floats:
             cols.append(DoubleColumn(col, '', df[col].tolist()))
@@ -761,21 +772,21 @@
         omero_shape = EllipseI()
         omero_shape.x = rdouble(shape.x)
         omero_shape.y = rdouble(shape.y)
         omero_shape.radiusX = rdouble(shape.x_rad)
         omero_shape.radiusY = rdouble(shape.y_rad)
     elif isinstance(shape, Polygon):
         omero_shape = PolygonI()
-        points_str = "".join("".join([str(x), ',', str(y), ', '])
-                             for x, y in shape.points)[:-2]
+        points_str = "".join("".join([str(x), ',', str(y), ' '])
+                             for x, y in shape.points).rstrip()
         omero_shape.points = rstring(points_str)
     elif isinstance(shape, Polyline):
         omero_shape = PolylineI()
-        points_str = "".join("".join([str(x), ',', str(y), ', '])
-                             for x, y in shape.points)[:-2]
+        points_str = "".join("".join([str(x), ',', str(y), ' '])
+                             for x, y in shape.points).rstrip()
         omero_shape.points = rstring(points_str)
     elif isinstance(shape, Label):
         omero_shape = LabelI()
         omero_shape.x = rdouble(shape.x)
         omero_shape.y = rdouble(shape.y)
         omero_shape.fontSize = LengthI(shape.fontSize,
                                        enums.UnitsLength.POINT)
```

### Comparing `ezomero-2.1.0/ezomero/json_api.py` & `ezomero-3.0.0/ezomero/json_api.py`

 * *Files identical despite different names*

### Comparing `ezomero-2.1.0/ezomero/rois.py` & `ezomero-3.0.0/ezomero/rois.py`

 * *Files identical despite different names*

### Comparing `ezomero-2.1.0/ezomero.egg-info/PKG-INFO` & `ezomero-3.0.0/ezomero.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ezomero
-Version: 2.1.0
+Version: 3.0.0
 Summary: A suite of convenience functions for working with OMERO. Written and maintained by the Research IT team at The Jackson Laboratory.
 Home-page: https://github.com/TheJacksonLaboratory/ezomero
 Maintainer: Dave Mellert
 Maintainer-email: Dave.Mellert@jax.org
 License: UNKNOWN
-Description: ![Run Tests](https://github.com/TheJacksonLaboratory/ezomero/workflows/Run%20Tests/badge.svg?event=push) ![](https://raw.githubusercontent.com/TheJacksonLaboratory/ezomero/main/coverage.svg)
+Description: ![](https://raw.githubusercontent.com/TheJacksonLaboratory/ezomero/main/coverage.svg) [![badge-doi](https://img.shields.io/badge/doi-10.1101%2F2023.06.29.546930-purple)](https://doi.org/10.1101/2023.06.29.546930) 
         
         # ezomero
         A module with convenience functions for writing Python code that interacts with OMERO.
         
         
         # Installation
         
@@ -23,11 +23,31 @@
         In general, you will need to create a `BlitzGateway` object using `ezomero.connect()`, then pass the `conn` object to most of these helper functions along with function-specific parameters.
         
         
         # Documentation
         
         Documentation is available at https://thejacksonlaboratory.github.io/ezomero/
         
+        # Development
+        
+        You will need Docker installed and running to run the tests.
+        
+        Setup your "omero" python environment with a local ezomero and pytest:
+        ```
+        > conda activate omero  # Activate your omero environment with conda or pip
+        (omero) > cd /your_local_clone/ezomero
+        (omero) > pip install -e .
+        (omero) > pip install pytest
+        ```
+        
+        To run the tests, startup the test OMERO server with Docker and run pytest
+        ```
+        > cd /your_local_clone/ezomero
+        > docker-compose -f tests/docker-compose.yml up -d
+        > conda activate omero
+        (omero) > python -m pytest .\tests
+        ```
+        
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tables
```

### Comparing `ezomero-2.1.0/ezomero.egg-info/SOURCES.txt` & `ezomero-3.0.0/ezomero.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ezomero-2.1.0/setup.py` & `ezomero-3.0.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import setuptools
-import os
-
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name="ezomero",
-    version=os.environ.get('VERSION', '0.0.0'),
-    maintainer="Dave Mellert",
-    maintainer_email="Dave.Mellert@jax.org",
-    description=("A suite of convenience functions for working"
-                 " with OMERO. Written and maintained by the "
-                 "Research IT team at The Jackson Laboratory."),
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/TheJacksonLaboratory/ezomero",
-    packages=setuptools.find_packages(),
-    install_requires=[
-        'omero-py==5.13.1',
-        'numpy>=1.22'
-    ],
-    extras_require={
-        "tables": ["pandas"],
-    },
-    python_requires='>=3.8'
-)
+import setuptools
+import os
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+    name="ezomero",
+    version=os.environ.get('VERSION', '0.0.0'),
+    maintainer="Dave Mellert",
+    maintainer_email="Dave.Mellert@jax.org",
+    description=("A suite of convenience functions for working"
+                 " with OMERO. Written and maintained by the "
+                 "Research IT team at The Jackson Laboratory."),
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/TheJacksonLaboratory/ezomero",
+    packages=setuptools.find_packages(),
+    install_requires=[
+        'omero-py == 5.19.0',
+        'numpy >= 1.22, < 2.0'
+    ],
+    extras_require={
+        "tables": ["pandas"],
+    },
+    python_requires='>=3.8'
+)
```

### Comparing `ezomero-2.1.0/tests/conftest.py` & `ezomero-3.0.0/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 def omero_params(request):
     user = request.config.getoption("--omero-user")
     password = request.config.getoption("--omero-pass")
     host = request.config.getoption("--omero-host")
     web_host = request.config.getoption("--omero-web-host")
     port = request.config.getoption("--omero-port")
     secure = request.config.getoption("--omero-secure")
-    return(user, password, host, web_host, port, secure)
+    return (user, password, host, web_host, port, secure)
 
 
 @pytest.fixture(scope='session')
 def users_groups(conn, omero_params):
     session_uuid = conn.getSession().getUuid().val
     user = omero_params[0]
     host = omero_params[2]
```

### Comparing `ezomero-2.1.0/tests/test_connect.py` & `ezomero-3.0.0/tests/test_connect.py`

 * *Files identical despite different names*

### Comparing `ezomero-2.1.0/tests/test_ezimport.py` & `ezomero-3.0.0/tests/test_ezimport.py`

 * *Files identical despite different names*

### Comparing `ezomero-2.1.0/tests/test_gets.py` & `ezomero-3.0.0/tests/test_gets.py`

 * *Files 1% similar despite different names*

```diff
@@ -385,23 +385,27 @@
 
     d = tmp_path / "input"
     d.mkdir()
     file_path = d / "hello.txt"
     file_path.write_text("hello world!")
     file_ann = str(file_path)
     ns = "jax.org/omeroutils/tests/v0"
-    file_ann_id = ezomero.post_file_annotation(conn, "Image", im_id,
-                                               file_ann, ns)
-    file_ann_id2 = ezomero.post_file_annotation(conn, "Image", im_id,
-                                                file_ann, ns)
-    file_ann_id3 = ezomero.post_file_annotation(conn, "Image", im_id,
-                                                file_ann, ns)
+    file_ann_id = ezomero.post_file_annotation(conn,
+                                               file_ann, ns,
+                                               "Image", im_id)
+    file_ann_id2 = ezomero.post_file_annotation(conn,
+                                                file_ann, ns,
+                                                "Image", im_id)
+    file_ann_id3 = ezomero.post_file_annotation(conn,
+                                                file_ann, ns,
+                                                "Image", im_id)
     ns2 = "different namespace"
-    file_ann_id4 = ezomero.post_file_annotation(conn, "Image", im_id,
-                                                file_ann, ns2)
+    file_ann_id4 = ezomero.post_file_annotation(conn,
+                                                file_ann, ns2,
+                                                "Image", im_id)
 
     # Test sanitizing inputs
     with pytest.raises(TypeError):
         _ = ezomero.get_file_annotation_ids(conn, 10, 10)
     with pytest.raises(TypeError):
         _ = ezomero.get_file_annotation_ids(conn, 'Image', '10')
     with pytest.raises(TypeError):
@@ -534,15 +538,15 @@
                               description=roi_fixture['desc'])
     shape_ids = ezomero.get_shape_ids(conn, roi_id)
     assert len(shape_ids) == len(roi_fixture['shapes'])
     for i in range(len(shape_ids)):
         shape = ezomero.get_shape(conn, shape_ids[i])
         assert hasattr(shape, 'label')
         for pre_shape in shapes:
-            if type(shape) == type(pre_shape):
+            if type(shape) is type(pre_shape):
                 assert shape.fill_color == pre_shape.fill_color
                 assert shape.stroke_color == pre_shape.stroke_color
                 assert shape.stroke_width == pre_shape.stroke_width
     roi_id2 = ezomero.post_roi(conn, im_id,
                                shapes=[arrow],
                                name=roi_fixture['name'],
                                description=roi_fixture['desc'])
```

### Comparing `ezomero-2.1.0/tests/test_json_api.py` & `ezomero-3.0.0/tests/test_json_api.py`

 * *Files identical despite different names*

### Comparing `ezomero-2.1.0/tests/test_misc.py` & `ezomero-3.0.0/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `ezomero-2.1.0/tests/test_posts.py` & `ezomero-3.0.0/tests/test_posts.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,17 @@
     ds_names = [d.getName() for d in ds]
     assert ds_test_name2 in ds_names
 
     # Dataset in non-existing project ID
     ds_test_name3 = 'test_post_dataset3_' + timestamp
     pid = 99999999
     did3 = ezomero.post_dataset(conn, ds_test_name3, project_id=pid)
+    ds_ids = ezomero.get_dataset_ids(conn)
     assert did3 is None
+    assert len(ds_ids) == 2
 
     # Dataset in cross-group project, valid permissions
     username = users_groups[1][0][0]  # test_user1
     groupname = users_groups[0][0][0]   # test_group_1
     current_conn = conn.suConn(username, groupname)
     ds_test_name4 = 'test_post_dataset4_' + timestamp
     project_info = project_structure[0]
@@ -58,14 +60,16 @@
     username = users_groups[1][2][0]  # test_user3
     groupname = users_groups[0][1][0]  # test_group_2
     current_conn = conn.suConn(username, groupname)
     ds_test_name5 = 'test_post_dataset5_' + timestamp
     project_info = project_structure[0]
     pid = project_info[1][1]  # proj1 (in test_group_1)
     did5 = ezomero.post_dataset(current_conn, ds_test_name5, project_id=pid)
+    ds_ids = ezomero.get_dataset_ids(current_conn)
+    assert len(ds_ids) == 1
     current_conn.close()
     assert did5 is None
 
     # Dataset in cross-group project, valid permissions
     # across_groups flag unset
     username = users_groups[1][0][0]  # test_user1
     groupname = users_groups[0][0][0]   # test_group_1
@@ -310,66 +314,90 @@
     file_path = d / "hello.txt"
     file_path.write_text("hello world!")
     file_ann = str(file_path)
 
     ns = "jax.org/omeroutils/tests/v0"
     # test sanitized input on post
     with pytest.raises(TypeError):
-        _ = ezomero.post_file_annotation(conn, "Image", im_id, 10, ns)
+        _ = ezomero.post_file_annotation(conn, 10, ns, "Image", im_id)
     with pytest.raises(TypeError):
-        _ = ezomero.post_file_annotation(conn, "Image", '10', file_ann, ns)
-    with pytest.raises(TypeError):
-        _ = ezomero.post_file_annotation(conn, "Image", None, file_ann, ns)
+        _ = ezomero.post_file_annotation(conn, file_ann, ns, "Image", '10')
 
-    file_ann_id = ezomero.post_file_annotation(conn, "Image", im_id, file_ann,
-                                               ns)
+    file_ann_id = ezomero.post_file_annotation(conn, file_ann, ns,
+                                               "Image", im_id)
     return_ann = ezomero.get_file_annotation(conn, file_ann_id)
     assert filecmp.cmp(return_ann, file_ann)
     os.remove(return_ann)
 
     # Test posting to non-existing object
     im_id2 = 999999999
-    file_ann_id2 = ezomero.post_file_annotation(conn, "Image", im_id2,
-                                                file_ann, ns)
+    file_ann_id2 = ezomero.post_file_annotation(conn,
+                                                file_ann, ns,
+                                                "Image", im_id2)
     assert file_ann_id2 is None
 
     # Test posting cross-group
     username = users_groups[1][0][0]  # test_user1
     groupname = users_groups[0][0][0]  # test_group_1
     current_conn = conn.suConn(username, groupname)
     im_id3 = image_info[2][1]  # im2, in test_group_2
-    file_ann_id3 = ezomero.post_file_annotation(current_conn, "Image", im_id3,
-                                                file_ann, ns)
+    file_ann_id3 = ezomero.post_file_annotation(current_conn,
+                                                file_ann, ns,
+                                                "Image", im_id3)
     return_ann3 = ezomero.get_file_annotation(current_conn, file_ann_id3)
     assert filecmp.cmp(return_ann3, file_ann)
     os.remove(return_ann3)
     current_conn.close()
 
     # Test posting to an invalid cross-group
     username = users_groups[1][2][0]  # test_user3
     groupname = users_groups[0][1][0]  # test_group_2
     current_conn = conn.suConn(username, groupname)
     im_id4 = image_info[1][1]  # im1(in test_group_1)
-    file_ann_id4 = ezomero.post_file_annotation(current_conn, "Image", im_id4,
-                                                file_ann, ns)
+    file_ann_id4 = ezomero.post_file_annotation(current_conn,
+                                                file_ann, ns,
+                                                "Image", im_id4)
     assert file_ann_id4 is None
     current_conn.close()
 
     # Test posting cross-group, across_groups unset
     username = users_groups[1][0][0]  # test_user1
     groupname = users_groups[0][0][0]  # test_group_1
     current_conn = conn.suConn(username, groupname)
     im_id5 = image_info[2][1]  # im2, in test_group_2
-    file_ann_id5 = ezomero.post_file_annotation(current_conn, "Image", im_id5,
+    file_ann_id5 = ezomero.post_file_annotation(current_conn,
                                                 file_ann, ns,
+                                                "Image", im_id5,
                                                 across_groups=False)
     assert file_ann_id5 is None
     current_conn.close()
 
-    conn.deleteObjects("Annotation", [file_ann_id, file_ann_id3],
+    # Test posting orphaned
+    current_conn = conn.suConn(username, groupname)
+    file_ann_id6 = ezomero.post_file_annotation(current_conn, file_ann, ns)
+    print(file_ann_id6)
+    return_ann6 = ezomero.get_file_annotation(current_conn, file_ann_id6)
+    assert filecmp.cmp(return_ann6, file_ann)
+    os.remove(return_ann6)
+
+    # Test posting orphaned, partial completion
+    file_ann_id7 = ezomero.post_file_annotation(conn, file_ann, ns, "Image")
+    return_ann7 = ezomero.get_file_annotation(conn, file_ann_id7)
+    assert filecmp.cmp(return_ann7, file_ann)
+    os.remove(return_ann7)
+
+    # Test posting orphaned, partial completion
+    file_ann_id8 = ezomero.post_file_annotation(conn, file_ann, ns,
+                                                object_id=10)
+    return_ann8 = ezomero.get_file_annotation(conn, file_ann_id8)
+    assert filecmp.cmp(return_ann8, file_ann)
+    os.remove(return_ann8)
+
+    conn.deleteObjects("Annotation", [file_ann_id, file_ann_id3, file_ann_id6,
+                                      file_ann_id7, file_ann_id8],
                        deleteAnns=True, deleteChildren=True, wait=True)
 
 
 def test_post_roi(conn, project_structure, roi_fixture, users_groups):
     image_info = project_structure[2]
     im_id = image_info[0][1]
```

### Comparing `ezomero-2.1.0/tests/test_puts.py` & `ezomero-3.0.0/tests/test_puts.py`

 * *Files identical despite different names*

### Comparing `ezomero-2.1.0/tests/test_rois.py` & `ezomero-3.0.0/tests/test_rois.py`

 * *Files identical despite different names*

