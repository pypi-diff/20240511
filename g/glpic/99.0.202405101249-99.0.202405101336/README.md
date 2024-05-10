# Comparing `tmp/glpic-99.0.202405101249.tar.gz` & `tmp/glpic-99.0.202405101336.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glpic-99.0.202405101249.tar", last modified: Fri May 10 12:49:49 2024, max compression
+gzip compressed data, was "glpic-99.0.202405101336.tar", last modified: Fri May 10 13:36:23 2024, max compression
```

## Comparing `glpic-99.0.202405101249.tar` & `glpic-99.0.202405101336.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:49:49.346716 glpic-99.0.202405101249/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-10 12:49:49.346716 glpic-99.0.202405101249/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-10 12:49:36.000000 glpic-99.0.202405101249/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:49:49.346716 glpic-99.0.202405101249/glpic/
--rw-r--r--   0 runner    (1001) docker     (127)    10051 2024-05-10 12:49:36.000000 glpic-99.0.202405101249/glpic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11813 2024-05-10 12:49:36.000000 glpic-99.0.202405101249/glpic/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:49:49.346716 glpic-99.0.202405101249/glpic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-10 12:49:49.000000 glpic-99.0.202405101249/glpic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-10 12:49:49.000000 glpic-99.0.202405101249/glpic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:49:49.000000 glpic-99.0.202405101249/glpic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-10 12:49:49.000000 glpic-99.0.202405101249/glpic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:49:49.000000 glpic-99.0.202405101249/glpic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 12:49:49.000000 glpic-99.0.202405101249/glpic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 12:49:49.000000 glpic-99.0.202405101249/glpic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 12:49:49.346716 glpic-99.0.202405101249/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-10 12:49:48.000000 glpic-99.0.202405101249/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:36:23.644374 glpic-99.0.202405101336/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-10 13:36:23.644374 glpic-99.0.202405101336/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-10 13:36:09.000000 glpic-99.0.202405101336/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:36:23.640375 glpic-99.0.202405101336/glpic/
+-rw-r--r--   0 runner    (1001) docker     (127)    10111 2024-05-10 13:36:09.000000 glpic-99.0.202405101336/glpic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11655 2024-05-10 13:36:09.000000 glpic-99.0.202405101336/glpic/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:36:23.644374 glpic-99.0.202405101336/glpic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-10 13:36:23.000000 glpic-99.0.202405101336/glpic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-10 13:36:23.000000 glpic-99.0.202405101336/glpic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:36:23.000000 glpic-99.0.202405101336/glpic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-10 13:36:23.000000 glpic-99.0.202405101336/glpic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:36:23.000000 glpic-99.0.202405101336/glpic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 13:36:23.000000 glpic-99.0.202405101336/glpic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 13:36:23.000000 glpic-99.0.202405101336/glpic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 13:36:23.644374 glpic-99.0.202405101336/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-10 13:36:22.000000 glpic-99.0.202405101336/setup.py
```

### Comparing `glpic-99.0.202405101249/README.md` & `glpic-99.0.202405101336/README.md`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202405101249/glpic/__init__.py` & `glpic-99.0.202405101336/glpic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,16 +140,17 @@
             if key.isnumeric():
                 search_options[all_options[key]['uid']] = key
         return search_options
 
     def info_computer(self, overrides={}):
         computer = overrides.get('computer')
         if computer is not None:
+            field = 2 if computer.isnumeric() else 1
             search_data = "criteria[0][link]=AND&criteria[0][itemtype]=Computer"
-            search_data = "&criteria[0][field]=1&criteria[0][searchtype]=contains"
+            search_data = f"&criteria[0][field]={field}&criteria[0][searchtype]=contains"
             search_data += f"&criteria[0][value]={computer}"
         else:
             search_options = self.get_options('Computer')
             search_data = ''
             for index, key in enumerate(overrides):
                 value = overrides[key]
                 if not key.startswith('Computer'):
```

### Comparing `glpic-99.0.202405101249/glpic/cli.py` & `glpic-99.0.202405101336/glpic/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,19 +107,15 @@
     glpic = Glpic(args.url, args.user, args.token, args.debug)
     reservationstable = PrettyTable(["Id", "Item", "Begin", "End", "Comment"])
     for reservation in glpic.list_reservations(overrides=handle_parameters(args.param)):
         _id, begin, end, comment = reservation['id'], reservation['begin'], reservation['end'], reservation['comment']
         comment = fill(comment, width=100)
         reservation_id = reservation['reservationitems_id']
         computer_id = glpic.info_reservation(reservation_id)['items_id']
-        computer_data = glpic.info_computer({'computer': computer_id})
-        if computer_data:
-            reservation_name = glpic.info_computer({'computer': computer_id})[0]['Computer.name']
-        else:
-            reservation_name = computer_id
+        reservation_name = glpic.info_computer({'computer': computer_id})[0]['Computer.name']
         entry = [_id, reservation_name, begin, end, comment]
         reservationstable.add_row(entry)
     print(reservationstable)
 
 
 def cli():
     """
```

### Comparing `glpic-99.0.202405101249/setup.py` & `glpic-99.0.202405101336/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 description = 'Glpic wrapper'
 long_description = description
 if os.path.exists('README.rst'):
     long_description = open('README.rst').read()
 
 setup(
     name='glpic',
-    version='99.0.202405101249',
+    version='99.0.202405101336',
     include_package_data=True,
     packages=find_packages(),
     zip_safe=False,
     description=description,
     long_description=long_description,
     url='http://github.com/karmab/glpic',
     author='Karim Boumedhel',
```

