# Comparing `tmp/glpic-99.0.202405102329.tar.gz` & `tmp/glpic-99.0.202405102337.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glpic-99.0.202405102329.tar", last modified: Fri May 10 23:29:49 2024, max compression
+gzip compressed data, was "glpic-99.0.202405102337.tar", last modified: Fri May 10 23:37:54 2024, max compression
```

## Comparing `glpic-99.0.202405102329.tar` & `glpic-99.0.202405102337.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:29:49.396372 glpic-99.0.202405102329/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-10 23:29:49.396372 glpic-99.0.202405102329/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-10 23:29:36.000000 glpic-99.0.202405102329/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:29:49.396372 glpic-99.0.202405102329/glpic/
--rw-r--r--   0 runner    (1001) docker     (127)    10566 2024-05-10 23:29:36.000000 glpic-99.0.202405102329/glpic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11963 2024-05-10 23:29:36.000000 glpic-99.0.202405102329/glpic/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:29:49.396372 glpic-99.0.202405102329/glpic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-10 23:29:49.000000 glpic-99.0.202405102329/glpic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-10 23:29:49.000000 glpic-99.0.202405102329/glpic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 23:29:49.000000 glpic-99.0.202405102329/glpic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-10 23:29:49.000000 glpic-99.0.202405102329/glpic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 23:29:49.000000 glpic-99.0.202405102329/glpic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 23:29:49.000000 glpic-99.0.202405102329/glpic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 23:29:49.000000 glpic-99.0.202405102329/glpic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 23:29:49.396372 glpic-99.0.202405102329/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-10 23:29:49.000000 glpic-99.0.202405102329/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:37:54.640247 glpic-99.0.202405102337/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-10 23:37:54.640247 glpic-99.0.202405102337/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-10 23:37:24.000000 glpic-99.0.202405102337/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:37:54.636247 glpic-99.0.202405102337/glpic/
+-rw-r--r--   0 runner    (1001) docker     (127)    10564 2024-05-10 23:37:24.000000 glpic-99.0.202405102337/glpic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11963 2024-05-10 23:37:24.000000 glpic-99.0.202405102337/glpic/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:37:54.640247 glpic-99.0.202405102337/glpic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-10 23:37:54.000000 glpic-99.0.202405102337/glpic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-10 23:37:54.000000 glpic-99.0.202405102337/glpic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 23:37:54.000000 glpic-99.0.202405102337/glpic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-10 23:37:54.000000 glpic-99.0.202405102337/glpic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 23:37:54.000000 glpic-99.0.202405102337/glpic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 23:37:54.000000 glpic-99.0.202405102337/glpic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 23:37:54.000000 glpic-99.0.202405102337/glpic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 23:37:54.640247 glpic-99.0.202405102337/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-10 23:37:54.000000 glpic-99.0.202405102337/setup.py
```

### Comparing `glpic-99.0.202405102329/README.md` & `glpic-99.0.202405102337/README.md`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202405102329/glpic/__init__.py` & `glpic-99.0.202405102337/glpic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,15 +217,15 @@
         if wrong_keys:
             error(f"Ignoring keys {','.join(wrong_keys)}")
             for key in wrong_keys:
                 del overrides[key]
         if not overrides:
             info("Nothing to create")
             return
-        data = {'input': [overrides]}
+        data = {'input': overrides}
         if self.debug:
             base_curl = curl_base(self.headers)
             msg = f"{base_curl} -X POST -Lk {self.base_url}/Reservation -d \"{json.dumps(data)}\""
             print(msg)
         return _post(f'{self.base_url}/Reservation', self.headers, data)
 
     def delete_reservation(self, reservation):
```

### Comparing `glpic-99.0.202405102329/glpic/cli.py` & `glpic-99.0.202405102337/glpic/cli.py`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202405102329/setup.py` & `glpic-99.0.202405102337/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 description = 'Glpic wrapper'
 long_description = description
 if os.path.exists('README.rst'):
     long_description = open('README.rst').read()
 
 setup(
     name='glpic',
-    version='99.0.202405102329',
+    version='99.0.202405102337',
     include_package_data=True,
     packages=find_packages(),
     zip_safe=False,
     description=description,
     long_description=long_description,
     url='http://github.com/karmab/glpic',
     author='Karim Boumedhel',
```
