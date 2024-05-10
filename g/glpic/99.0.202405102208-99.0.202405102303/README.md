# Comparing `tmp/glpic-99.0.202405102208.tar.gz` & `tmp/glpic-99.0.202405102303.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glpic-99.0.202405102208.tar", last modified: Fri May 10 22:08:34 2024, max compression
+gzip compressed data, was "glpic-99.0.202405102303.tar", last modified: Fri May 10 23:03:43 2024, max compression
```

## Comparing `glpic-99.0.202405102208.tar` & `glpic-99.0.202405102303.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:08:34.925315 glpic-99.0.202405102208/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-10 22:08:34.925315 glpic-99.0.202405102208/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-10 22:08:01.000000 glpic-99.0.202405102208/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:08:34.921315 glpic-99.0.202405102208/glpic/
--rw-r--r--   0 runner    (1001) docker     (127)    10594 2024-05-10 22:08:01.000000 glpic-99.0.202405102208/glpic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11963 2024-05-10 22:08:01.000000 glpic-99.0.202405102208/glpic/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:08:34.921315 glpic-99.0.202405102208/glpic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-10 22:08:34.000000 glpic-99.0.202405102208/glpic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-10 22:08:34.000000 glpic-99.0.202405102208/glpic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 22:08:34.000000 glpic-99.0.202405102208/glpic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-10 22:08:34.000000 glpic-99.0.202405102208/glpic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 22:08:34.000000 glpic-99.0.202405102208/glpic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 22:08:34.000000 glpic-99.0.202405102208/glpic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 22:08:34.000000 glpic-99.0.202405102208/glpic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 22:08:34.925315 glpic-99.0.202405102208/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-10 22:08:34.000000 glpic-99.0.202405102208/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:03:43.855396 glpic-99.0.202405102303/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-10 23:03:43.855396 glpic-99.0.202405102303/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-10 23:03:30.000000 glpic-99.0.202405102303/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:03:43.851396 glpic-99.0.202405102303/glpic/
+-rw-r--r--   0 runner    (1001) docker     (127)    10562 2024-05-10 23:03:30.000000 glpic-99.0.202405102303/glpic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11963 2024-05-10 23:03:30.000000 glpic-99.0.202405102303/glpic/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:03:43.851396 glpic-99.0.202405102303/glpic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-10 23:03:43.000000 glpic-99.0.202405102303/glpic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-10 23:03:43.000000 glpic-99.0.202405102303/glpic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 23:03:43.000000 glpic-99.0.202405102303/glpic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-10 23:03:43.000000 glpic-99.0.202405102303/glpic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 23:03:43.000000 glpic-99.0.202405102303/glpic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 23:03:43.000000 glpic-99.0.202405102303/glpic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 23:03:43.000000 glpic-99.0.202405102303/glpic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 23:03:43.855396 glpic-99.0.202405102303/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-10 23:03:43.000000 glpic-99.0.202405102303/setup.py
```

### Comparing `glpic-99.0.202405102208/README.md` & `glpic-99.0.202405102303/README.md`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202405102208/glpic/__init__.py` & `glpic-99.0.202405102303/glpic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,32 +200,31 @@
         return results
 
     def create_reservation(self, computer, overrides):
         overrides['begin'] = parse(str(date.today())).strftime('%Y-%m-%d 00:00:00')
         if 'end' not in overrides:
             overrides['end'] = date.today() + timedelta(days=30)
         user = overrides.get('user', self.user)
-        if 'user_id' not in overrides:
+        if 'users_id' not in overrides:
             user_id = self.get_user(user)['id']
-            overrides['user_id'] = user_id
+            overrides['users_id'] = user_id
         overrides['end'] = parse(str(overrides['end'])).strftime('%Y-%m-%d 00:00:00')
         if 'comment' not in overrides:
             overrides['comment'] = f'reservation for {user}'
         reservation_id = self.info_computer({'computer': computer, 'uid': True})[0]['Computer.id']
         overrides['reservationitems_id'] = reservation_id
-        # valid_keys = list(_get(f'{self.base_url}/Reservation/', self.headers)[0].keys())
-        # wrong_keys = [key for key in overrides if key not in valid_keys]
-        # if wrong_keys:
-        #    error(f"Ignoring keys {','.join(wrong_keys)}")
-        #    for key in wrong_keys:
-        #        del overrides[key]
+        valid_keys = list(_get(f'{self.base_url}/Reservation/', self.headers)[0].keys())
+        wrong_keys = [key for key in overrides if key not in valid_keys]
+        if wrong_keys:
+            error(f"Ignoring keys {','.join(wrong_keys)}")
+            for key in wrong_keys:
+                del overrides[key]
         if not overrides:
             info("Nothing to create")
             return
-        print(overrides)
         data = {'input': overrides}
         if self.debug:
             base_curl = curl_base(self.headers)
             msg = f"{base_curl} -X POST -Lk {self.base_url}/Reservation -d \"{json.dumps(data)}\""
             print(msg)
         return _post(f'{self.base_url}/Reservation', self.headers, data)
```

### Comparing `glpic-99.0.202405102208/glpic/cli.py` & `glpic-99.0.202405102303/glpic/cli.py`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202405102208/setup.py` & `glpic-99.0.202405102303/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 description = 'Glpic wrapper'
 long_description = description
 if os.path.exists('README.rst'):
     long_description = open('README.rst').read()
 
 setup(
     name='glpic',
-    version='99.0.202405102208',
+    version='99.0.202405102303',
     include_package_data=True,
     packages=find_packages(),
     zip_safe=False,
     description=description,
     long_description=long_description,
     url='http://github.com/karmab/glpic',
     author='Karim Boumedhel',
```

