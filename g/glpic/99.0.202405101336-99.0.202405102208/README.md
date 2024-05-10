# Comparing `tmp/glpic-99.0.202405101336.tar.gz` & `tmp/glpic-99.0.202405102208.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glpic-99.0.202405101336.tar", last modified: Fri May 10 13:36:23 2024, max compression
+gzip compressed data, was "glpic-99.0.202405102208.tar", last modified: Fri May 10 22:08:34 2024, max compression
```

## Comparing `glpic-99.0.202405101336.tar` & `glpic-99.0.202405102208.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:36:23.644374 glpic-99.0.202405101336/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-10 13:36:23.644374 glpic-99.0.202405101336/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-10 13:36:09.000000 glpic-99.0.202405101336/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:36:23.640375 glpic-99.0.202405101336/glpic/
--rw-r--r--   0 runner    (1001) docker     (127)    10111 2024-05-10 13:36:09.000000 glpic-99.0.202405101336/glpic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11655 2024-05-10 13:36:09.000000 glpic-99.0.202405101336/glpic/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:36:23.644374 glpic-99.0.202405101336/glpic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-10 13:36:23.000000 glpic-99.0.202405101336/glpic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-10 13:36:23.000000 glpic-99.0.202405101336/glpic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:36:23.000000 glpic-99.0.202405101336/glpic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-10 13:36:23.000000 glpic-99.0.202405101336/glpic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:36:23.000000 glpic-99.0.202405101336/glpic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 13:36:23.000000 glpic-99.0.202405101336/glpic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 13:36:23.000000 glpic-99.0.202405101336/glpic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 13:36:23.644374 glpic-99.0.202405101336/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-10 13:36:22.000000 glpic-99.0.202405101336/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:08:34.925315 glpic-99.0.202405102208/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-10 22:08:34.925315 glpic-99.0.202405102208/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-10 22:08:01.000000 glpic-99.0.202405102208/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:08:34.921315 glpic-99.0.202405102208/glpic/
+-rw-r--r--   0 runner    (1001) docker     (127)    10594 2024-05-10 22:08:01.000000 glpic-99.0.202405102208/glpic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11963 2024-05-10 22:08:01.000000 glpic-99.0.202405102208/glpic/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:08:34.921315 glpic-99.0.202405102208/glpic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-10 22:08:34.000000 glpic-99.0.202405102208/glpic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-10 22:08:34.000000 glpic-99.0.202405102208/glpic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 22:08:34.000000 glpic-99.0.202405102208/glpic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-10 22:08:34.000000 glpic-99.0.202405102208/glpic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 22:08:34.000000 glpic-99.0.202405102208/glpic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 22:08:34.000000 glpic-99.0.202405102208/glpic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 22:08:34.000000 glpic-99.0.202405102208/glpic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 22:08:34.925315 glpic-99.0.202405102208/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-10 22:08:34.000000 glpic-99.0.202405102208/setup.py
```

### Comparing `glpic-99.0.202405101336/README.md` & `glpic-99.0.202405102208/README.md`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202405101336/glpic/__init__.py` & `glpic-99.0.202405102208/glpic/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,15 +140,15 @@
             if key.isnumeric():
                 search_options[all_options[key]['uid']] = key
         return search_options
 
     def info_computer(self, overrides={}):
         computer = overrides.get('computer')
         if computer is not None:
-            field = 2 if computer.isnumeric() else 1
+            field = 2 if isinstance(computer, int) or computer.isnumeric() else 1
             search_data = "criteria[0][link]=AND&criteria[0][itemtype]=Computer"
             search_data = f"&criteria[0][field]={field}&criteria[0][searchtype]=contains"
             search_data += f"&criteria[0][value]={computer}"
         else:
             search_options = self.get_options('Computer')
             search_data = ''
             for index, key in enumerate(overrides):
@@ -158,15 +158,18 @@
                 if key not in search_options:
                     warning("Invalid key {key}")
                     continue
                 key_id = search_options[key]
                 search_data += "criteria[{index}][link]=AND&criteria[{index}][itemtype]=Computer"
                 search_data = f"&criteria[{index}][field]={key_id}&criteria[{index}][searchtype]=contains"
                 search_data += f"&criteria[{index}][value]={value}"
-        computers = _get(f'{self.base_url}/search/Computer?{search_data}&uid_cols', headers=self.headers)
+        url = f'{self.base_url}/search/Computer?{search_data}&uid_cols'
+        if overrides.get('uid', False):
+            url += '&forcedisplay[0]=2'
+        computers = _get(url, headers=self.headers)
         return computers['data'] if 'data' in computers else []
 
     def info_reservation(self, reservation):
         return _get(f'{self.base_url}/ReservationItem/{reservation}', headers=self.headers)
 
     def list_reservations(self, overrides={}):
         user = overrides.get('user') or self.user
@@ -192,35 +195,43 @@
             if memory is not None and int(float(current_memory)) < int(memory):
                 continue
             results.append(computer)
             if number is not None and len(results) >= int(number):
                 break
         return results
 
-    def create_reservation(self, reservation, overrides):
-        valid_keys = list(_get(f'{self.base_url}/Reservation/', self.headers)[0].keys())
-        wrong_keys = [key for key in overrides if key not in valid_keys]
-        if wrong_keys:
-            error(f"Ignoring keys {','.join(wrong_keys)}")
-            for key in wrong_keys:
-                del overrides[key]
-        # post = {"reservationitems_id": reservation_id, "begin": begin, "end": end, "users_id": user_id,
-        #        "comment": f'reservation for {self.user}'}
-        if not overrides:
-            info("Nothing to create")
-            return
+    def create_reservation(self, computer, overrides):
+        overrides['begin'] = parse(str(date.today())).strftime('%Y-%m-%d 00:00:00')
         if 'end' not in overrides:
             overrides['end'] = date.today() + timedelta(days=30)
+        user = overrides.get('user', self.user)
+        if 'user_id' not in overrides:
+            user_id = self.get_user(user)['id']
+            overrides['user_id'] = user_id
         overrides['end'] = parse(str(overrides['end'])).strftime('%Y-%m-%d 00:00:00')
+        if 'comment' not in overrides:
+            overrides['comment'] = f'reservation for {user}'
+        reservation_id = self.info_computer({'computer': computer, 'uid': True})[0]['Computer.id']
+        overrides['reservationitems_id'] = reservation_id
+        # valid_keys = list(_get(f'{self.base_url}/Reservation/', self.headers)[0].keys())
+        # wrong_keys = [key for key in overrides if key not in valid_keys]
+        # if wrong_keys:
+        #    error(f"Ignoring keys {','.join(wrong_keys)}")
+        #    for key in wrong_keys:
+        #        del overrides[key]
+        if not overrides:
+            info("Nothing to create")
+            return
+        print(overrides)
         data = {'input': overrides}
         if self.debug:
             base_curl = curl_base(self.headers)
-            msg = f"{base_curl} -X POST -Lk {self.base_url}/Reservation/{reservation} -d \"{json.dumps(data)}\""
+            msg = f"{base_curl} -X POST -Lk {self.base_url}/Reservation -d \"{json.dumps(data)}\""
             print(msg)
-        return _post(f'{self.base_url}/Reservation/{reservation}', self.headers, data)
+        return _post(f'{self.base_url}/Reservation', self.headers, data)
 
     def delete_reservation(self, reservation):
         if self.debug:
             base_curl = curl_base(self.headers)
             print(f"{base_curl} -X DELETE -Lk {self.base_url}/Reservation/{reservation}")
         return _delete(f'{self.base_url}/Reservation/{reservation}', headers=self.headers)
```

### Comparing `glpic-99.0.202405101336/glpic/cli.py` & `glpic-99.0.202405102208/glpic/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,21 @@
     for subparsers_action in subparsers_actions:
         for choice, subparser in subparsers_action.choices.items():
             if choice == subcommand:
                 return subparser
 
 
 def create_reservation(args):
-    print("TODO")
+    glpic = Glpic(args.url, args.user, args.token, args.debug)
+    overrides = handle_parameters(args.param)
+    computer = args.computer or overrides.get('computer')
+    if computer is None:
+        error("Missing computer")
+        sys.exit(1)
+    glpic.create_reservation(computer, overrides)
 
 
 def delete_reservation(args):
     yes = args.yes
     yes_top = args.yes_top
     if not yes and not yes_top:
         confirm("Are you sure?")
@@ -71,15 +77,16 @@
     for reservation in args.reservations:
         info(f"Updating reservation {reservation}")
         glpic.update_reservation(reservation, overrides=handle_parameters(args.param))
 
 
 def info_computer(args):
     glpic = Glpic(args.url, args.user, args.token, args.debug)
-    overrides = {'computer': args.computer} if args.computer is not None else handle_parameters(args.param)
+    overrides = {'computer': args.computer} if args.computer is not None else {}
+    overrides.update(handle_parameters(args.param))
     data = glpic.info_computer(overrides)
     for computer in data:
         for key in computer:
             print(f"{key}: {computer[key]}")
         print('-----------------')
 
 
@@ -137,15 +144,15 @@
     reservationcreate_epilog = None
     reservationcreate_parser = create_subparsers.add_parser('reservation', description=reservationcreate_desc,
                                                             help=reservationcreate_desc,
                                                             epilog=reservationcreate_epilog, formatter_class=rawhelp)
     reservationcreate_parser.add_argument('-f', '--force', action='store_true',
                                           help='Delete existing reservation if needed')
     reservationcreate_parser.add_argument('-P', '--param', action='append', help=PARAMHELP, metavar='PARAM')
-    reservationcreate_parser.add_argument('reservation', metavar='RESERVATION')
+    reservationcreate_parser.add_argument('computer', metavar='COMPUTER', nargs='?')
     reservationcreate_parser.set_defaults(func=create_reservation)
 
     delete_desc = 'Delete Object'
     delete_parser = subparsers.add_parser('delete', description=delete_desc, help=delete_desc, aliases=['remove'])
     delete_parser.add_argument('-y', '--yes', action='store_true', help='Dont ask for confirmation', dest="yes_top")
     delete_subparsers = delete_parser.add_subparsers(metavar='', dest='subcommand_delete')
```

### Comparing `glpic-99.0.202405101336/setup.py` & `glpic-99.0.202405102208/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 description = 'Glpic wrapper'
 long_description = description
 if os.path.exists('README.rst'):
     long_description = open('README.rst').read()
 
 setup(
     name='glpic',
-    version='99.0.202405101336',
+    version='99.0.202405102208',
     include_package_data=True,
     packages=find_packages(),
     zip_safe=False,
     description=description,
     long_description=long_description,
     url='http://github.com/karmab/glpic',
     author='Karim Boumedhel',
```

