# Comparing `tmp/hc_log_tools-1.2.1.tar.gz` & `tmp/hc_log_tools-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hc_log_tools-1.2.1.tar", last modified: Wed May  8 09:27:21 2024, max compression
+gzip compressed data, was "hc_log_tools-1.2.2.tar", last modified: Sat May 11 03:14:16 2024, max compression
```

## Comparing `hc_log_tools-1.2.1.tar` & `hc_log_tools-1.2.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 shixukai   (501) staff       (20)        0 2024-05-08 09:27:21.402740 hc_log_tools-1.2.1/
--rw-r--r--   0 shixukai   (501) staff       (20)     1074 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/LICENSE
--rw-r--r--   0 shixukai   (501) staff       (20)       24 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/MANIFEST.in
--rw-r--r--   0 shixukai   (501) staff       (20)     1658 2024-05-08 09:27:21.402540 hc_log_tools-1.2.1/PKG-INFO
--rw-r--r--   0 shixukai   (501) staff       (20)     1272 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/README.md
-drwxr-xr-x   0 shixukai   (501) staff       (20)        0 2024-05-08 09:27:21.402315 hc_log_tools-1.2.1/hc_log_tools.egg-info/
--rw-r--r--   0 shixukai   (501) staff       (20)     1658 2024-05-08 09:27:21.000000 hc_log_tools-1.2.1/hc_log_tools.egg-info/PKG-INFO
--rw-r--r--   0 shixukai   (501) staff       (20)      525 2024-05-08 09:27:21.000000 hc_log_tools-1.2.1/hc_log_tools.egg-info/SOURCES.txt
--rw-r--r--   0 shixukai   (501) staff       (20)        1 2024-05-08 09:27:21.000000 hc_log_tools-1.2.1/hc_log_tools.egg-info/dependency_links.txt
--rw-r--r--   0 shixukai   (501) staff       (20)       94 2024-05-08 09:27:21.000000 hc_log_tools-1.2.1/hc_log_tools.egg-info/requires.txt
--rw-r--r--   0 shixukai   (501) staff       (20)        9 2024-05-08 09:27:21.000000 hc_log_tools-1.2.1/hc_log_tools.egg-info/top_level.txt
--rw-r--r--   0 shixukai   (501) staff       (20)      365 2024-05-08 09:27:18.000000 hc_log_tools-1.2.1/pyproject.toml
--rw-r--r--   0 shixukai   (501) staff       (20)       94 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/requirements.txt
--rw-r--r--   0 shixukai   (501) staff       (20)       38 2024-05-08 09:27:21.402786 hc_log_tools-1.2.1/setup.cfg
--rw-r--r--   0 shixukai   (501) staff       (20)      719 2024-05-08 09:24:58.000000 hc_log_tools-1.2.1/setup.py
-drwxr-xr-x   0 shixukai   (501) staff       (20)        0 2024-05-08 09:27:21.401164 hc_log_tools-1.2.1/src/
--rw-r--r--   0 shixukai   (501) staff       (20)        0 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/src/__init__.py
--rw-r--r--   0 shixukai   (501) staff       (20)     1283 2024-05-08 09:24:58.000000 hc_log_tools-1.2.1/src/entry.py
--rw-r--r--   0 shixukai   (501) staff       (20)    18729 2024-05-08 09:24:58.000000 hc_log_tools-1.2.1/src/log_utility.py
--rw-r--r--   0 shixukai   (501) staff       (20)     5306 2024-05-08 09:24:58.000000 hc_log_tools-1.2.1/src/pack_log.py
--rw-r--r--   0 shixukai   (501) staff       (20)       39 2024-05-08 09:24:58.000000 hc_log_tools-1.2.1/src/public.py
--rw-r--r--   0 shixukai   (501) staff       (20)     3986 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/src/v_t_chart.py
-drwxr-xr-x   0 shixukai   (501) staff       (20)        0 2024-05-08 09:27:21.402135 hc_log_tools-1.2.1/test/
--rw-r--r--   0 shixukai   (501) staff       (20)        0 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/test/__init__.py
--rw-r--r--   0 shixukai   (501) staff       (20)     3537 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/test/test_log_download.py
--rw-r--r--   0 shixukai   (501) staff       (20)     1093 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/test/test_log_file_name_match.py
--rw-r--r--   0 shixukai   (501) staff       (20)     1946 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/test/test_log_utility.py
--rw-r--r--   0 shixukai   (501) staff       (20)      595 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/test/test_read_pick_data.py
--rw-r--r--   0 shixukai   (501) staff       (20)     2601 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/test/test_read_sort_data.py
--rw-r--r--   0 shixukai   (501) staff       (20)     3784 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/test/test_tiem_range.py
+drwxr-xr-x   0 os         (501) staff       (20)        0 2024-05-11 03:14:16.479252 hc_log_tools-1.2.2/
+-rw-r--r--   0 os         (501) staff       (20)     1074 2024-04-28 07:49:30.000000 hc_log_tools-1.2.2/LICENSE
+-rw-r--r--   0 os         (501) staff       (20)       24 2024-04-28 07:49:30.000000 hc_log_tools-1.2.2/MANIFEST.in
+-rw-r--r--   0 os         (501) staff       (20)     1672 2024-05-11 03:14:16.478654 hc_log_tools-1.2.2/PKG-INFO
+-rw-r--r--   0 os         (501) staff       (20)     1272 2024-04-28 07:49:30.000000 hc_log_tools-1.2.2/README.md
+drwxr-xr-x   0 os         (501) staff       (20)        0 2024-05-11 03:14:16.477970 hc_log_tools-1.2.2/hc_log_tools.egg-info/
+-rw-r--r--   0 os         (501) staff       (20)     1672 2024-05-11 03:14:16.000000 hc_log_tools-1.2.2/hc_log_tools.egg-info/PKG-INFO
+-rw-r--r--   0 os         (501) staff       (20)      525 2024-05-11 03:14:16.000000 hc_log_tools-1.2.2/hc_log_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 os         (501) staff       (20)        1 2024-05-11 03:14:16.000000 hc_log_tools-1.2.2/hc_log_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 os         (501) staff       (20)       94 2024-05-11 03:14:16.000000 hc_log_tools-1.2.2/hc_log_tools.egg-info/requires.txt
+-rw-r--r--   0 os         (501) staff       (20)        9 2024-05-11 03:14:16.000000 hc_log_tools-1.2.2/hc_log_tools.egg-info/top_level.txt
+-rw-r--r--   0 os         (501) staff       (20)      379 2024-05-11 03:13:45.000000 hc_log_tools-1.2.2/pyproject.toml
+-rw-r--r--   0 os         (501) staff       (20)       94 2024-04-28 07:49:30.000000 hc_log_tools-1.2.2/requirements.txt
+-rw-r--r--   0 os         (501) staff       (20)       38 2024-05-11 03:14:16.479411 hc_log_tools-1.2.2/setup.cfg
+-rw-r--r--   0 os         (501) staff       (20)      749 2024-04-28 07:49:30.000000 hc_log_tools-1.2.2/setup.py
+drwxr-xr-x   0 os         (501) staff       (20)        0 2024-05-11 03:14:16.473421 hc_log_tools-1.2.2/src/
+-rw-r--r--   0 os         (501) staff       (20)        0 2024-04-28 07:49:30.000000 hc_log_tools-1.2.2/src/__init__.py
+-rw-r--r--   0 os         (501) staff       (20)     1318 2024-04-30 07:46:05.000000 hc_log_tools-1.2.2/src/entry.py
+-rw-r--r--   0 os         (501) staff       (20)    18729 2024-04-30 08:11:09.000000 hc_log_tools-1.2.2/src/log_utility.py
+-rw-r--r--   0 os         (501) staff       (20)     6125 2024-05-10 05:47:31.000000 hc_log_tools-1.2.2/src/pack_log.py
+-rw-r--r--   0 os         (501) staff       (20)       39 2024-04-30 03:52:15.000000 hc_log_tools-1.2.2/src/public.py
+-rw-r--r--   0 os         (501) staff       (20)     3986 2024-04-28 07:49:30.000000 hc_log_tools-1.2.2/src/v_t_chart.py
+drwxr-xr-x   0 os         (501) staff       (20)        0 2024-05-11 03:14:16.477200 hc_log_tools-1.2.2/test/
+-rw-r--r--   0 os         (501) staff       (20)        0 2024-04-28 07:49:30.000000 hc_log_tools-1.2.2/test/__init__.py
+-rw-r--r--   0 os         (501) staff       (20)     3537 2024-04-28 07:49:30.000000 hc_log_tools-1.2.2/test/test_log_download.py
+-rw-r--r--   0 os         (501) staff       (20)     1093 2024-04-28 07:49:30.000000 hc_log_tools-1.2.2/test/test_log_file_name_match.py
+-rw-r--r--   0 os         (501) staff       (20)     1946 2024-04-28 07:49:30.000000 hc_log_tools-1.2.2/test/test_log_utility.py
+-rw-r--r--   0 os         (501) staff       (20)      595 2024-04-28 07:49:30.000000 hc_log_tools-1.2.2/test/test_read_pick_data.py
+-rw-r--r--   0 os         (501) staff       (20)     2601 2024-04-28 07:49:30.000000 hc_log_tools-1.2.2/test/test_read_sort_data.py
+-rw-r--r--   0 os         (501) staff       (20)     3784 2024-04-28 07:49:30.000000 hc_log_tools-1.2.2/test/test_tiem_range.py
```

### Comparing `hc_log_tools-1.2.1/LICENSE` & `hc_log_tools-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.1/PKG-INFO` & `hc_log_tools-1.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: hc_log_tools
-Version: 1.2.1
-Author-email: "xukai.sh" <shixukai@163.com>, "xukai.sh" <shixukai@163.com>
+Version: 1.2.2
+Author-email: "xukai.shi" <xukai.shi@hcrobots.com>, "xukai.shi" <xukai.shi@hcrobots.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: alive_progress==2.4.1
 Requires-Dist: matplotlib==3.5.3
 Requires-Dist: pip>=20.0.2
 Requires-Dist: python_dateutil==2.8.2
```

### Comparing `hc_log_tools-1.2.1/README.md` & `hc_log_tools-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.1/hc_log_tools.egg-info/PKG-INFO` & `hc_log_tools-1.2.2/hc_log_tools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: hc_log_tools
-Version: 1.2.1
-Author-email: "xukai.sh" <shixukai@163.com>, "xukai.sh" <shixukai@163.com>
+Version: 1.2.2
+Author-email: "xukai.shi" <xukai.shi@hcrobots.com>, "xukai.shi" <xukai.shi@hcrobots.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: alive_progress==2.4.1
 Requires-Dist: matplotlib==3.5.3
 Requires-Dist: pip>=20.0.2
 Requires-Dist: python_dateutil==2.8.2
```

### Comparing `hc_log_tools-1.2.1/hc_log_tools.egg-info/SOURCES.txt` & `hc_log_tools-1.2.2/hc_log_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.1/src/entry.py` & `hc_log_tools-1.2.2/src/entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,34 +7,40 @@
     # only can run one process at a time
     lock_file = open("/tmp/log-tool-lock", "w")
     try:
         fcntl.flock(lock_file, fcntl.LOCK_EX | fcntl.LOCK_NB)
     except IOError:
         print("another process is running, exit")
         sys.exit(-1)
+    
 
     parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.set_defaults(func=lambda args: parser.print_help())
 
     subparsers = parser.add_subparsers(title='subcommands', dest='command', help='sub-command help')
 
     subparsers_pack = subparsers.add_parser("pack", help='pack help')
     src.pack_log.init_input_args(subparsers_pack)
     subparsers_pack.set_defaults(func=src.pack_log.pack_log)
 
     subparsers_chart = subparsers.add_parser("chart", help='chart help')
     src.v_t_chart.init_input_args(subparsers_chart)
     subparsers_chart.set_defaults(func=src.v_t_chart.generate_chart)
+    
 
     # parse the args and call whatever function was selected
+    
+    
     args = parser.parse_args()
     args.func(args)
 
     # pack_log(args)
 
     # if args.up_to_cloud:
     #     pass
     # else:
     #     print(f'output_file_path: {Public.output_file_path}')
 
 if __name__=="__main__":
     sys.exit(entry())
+       
+
```

### Comparing `hc_log_tools-1.2.1/src/log_utility.py` & `hc_log_tools-1.2.2/src/log_utility.py`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.1/src/v_t_chart.py` & `hc_log_tools-1.2.2/src/v_t_chart.py`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.1/test/test_log_download.py` & `hc_log_tools-1.2.2/test/test_log_download.py`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.1/test/test_log_file_name_match.py` & `hc_log_tools-1.2.2/test/test_log_file_name_match.py`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.1/test/test_log_utility.py` & `hc_log_tools-1.2.2/test/test_log_utility.py`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.1/test/test_read_pick_data.py` & `hc_log_tools-1.2.2/test/test_read_pick_data.py`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.1/test/test_read_sort_data.py` & `hc_log_tools-1.2.2/test/test_read_sort_data.py`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.1/test/test_tiem_range.py` & `hc_log_tools-1.2.2/test/test_tiem_range.py`

 * *Files identical despite different names*

