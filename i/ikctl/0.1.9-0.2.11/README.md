# Comparing `tmp/ikctl-0.1.9.tar.gz` & `tmp/ikctl-0.2.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ikctl-0.1.9.tar", last modified: Thu Apr 11 15:10:41 2024, max compression
+gzip compressed data, was "ikctl-0.2.11.tar", last modified: Sat May 11 21:08:15 2024, max compression
```

## Comparing `ikctl-0.1.9.tar` & `ikctl-0.2.11.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 dml       (1000) dml       (1000)        0 2024-04-11 15:10:41.798424 ikctl-0.1.9/
--rw-rw-r--   0 dml       (1000) dml       (1000)    11357 2023-10-03 19:19:30.000000 ikctl-0.1.9/LICENSE
--rw-r--r--   0 dml       (1000) dml       (1000)     2414 2024-04-11 15:10:41.798424 ikctl-0.1.9/PKG-INFO
--rw-rw-r--   0 dml       (1000) dml       (1000)     2033 2024-03-24 12:40:50.000000 ikctl-0.1.9/README.md
-drwxrwxr-x   0 dml       (1000) dml       (1000)        0 2024-04-11 15:10:41.794424 ikctl-0.1.9/ikctl/
--rw-rw-r--   0 dml       (1000) dml       (1000)       30 2024-03-24 12:13:52.000000 ikctl-0.1.9/ikctl/__init__.py
--rw-rw-r--   0 dml       (1000) dml       (1000)     1049 2024-04-11 10:24:08.000000 ikctl-0.1.9/ikctl/commands.py
--rw-rw-r--   0 dml       (1000) dml       (1000)     4078 2024-04-11 15:07:31.000000 ikctl-0.1.9/ikctl/config.py
--rw-rw-r--   0 dml       (1000) dml       (1000)     1607 2024-04-11 12:11:52.000000 ikctl-0.1.9/ikctl/connect.py
--rw-rw-r--   0 dml       (1000) dml       (1000)     1282 2023-10-19 21:13:41.000000 ikctl-0.1.9/ikctl/context.py
--rw-rw-r--   0 dml       (1000) dml       (1000)     1408 2024-03-24 10:59:09.000000 ikctl-0.1.9/ikctl/create_config_files.py
--rw-rw-r--   0 dml       (1000) dml       (1000)      970 2024-04-11 09:58:32.000000 ikctl-0.1.9/ikctl/execute.py
--rw-rw-r--   0 dml       (1000) dml       (1000)      327 2023-10-03 19:22:08.000000 ikctl-0.1.9/ikctl/logs.py
--rwxrwxr-x   0 dml       (1000) dml       (1000)      794 2024-04-11 09:56:10.000000 ikctl-0.1.9/ikctl/main.py
--rw-rw-r--   0 dml       (1000) dml       (1000)     2943 2024-04-11 14:46:17.000000 ikctl-0.1.9/ikctl/pipeline.py
--rw-rw-r--   0 dml       (1000) dml       (1000)      927 2024-01-06 11:24:38.000000 ikctl-0.1.9/ikctl/sftp.py
--rw-rw-r--   0 dml       (1000) dml       (1000)     1044 2024-01-06 11:47:49.000000 ikctl-0.1.9/ikctl/view.py
-drwxrwxr-x   0 dml       (1000) dml       (1000)        0 2024-04-11 15:10:41.798424 ikctl-0.1.9/ikctl.egg-info/
--rw-r--r--   0 dml       (1000) dml       (1000)     2414 2024-04-11 15:10:41.000000 ikctl-0.1.9/ikctl.egg-info/PKG-INFO
--rw-rw-r--   0 dml       (1000) dml       (1000)      408 2024-04-11 15:10:41.000000 ikctl-0.1.9/ikctl.egg-info/SOURCES.txt
--rw-rw-r--   0 dml       (1000) dml       (1000)        1 2024-04-11 15:10:41.000000 ikctl-0.1.9/ikctl.egg-info/dependency_links.txt
--rw-rw-r--   0 dml       (1000) dml       (1000)       51 2024-04-11 15:10:41.000000 ikctl-0.1.9/ikctl.egg-info/entry_points.txt
--rw-rw-r--   0 dml       (1000) dml       (1000)       23 2024-04-11 15:10:41.000000 ikctl-0.1.9/ikctl.egg-info/requires.txt
--rw-rw-r--   0 dml       (1000) dml       (1000)        6 2024-04-11 15:10:41.000000 ikctl-0.1.9/ikctl.egg-info/top_level.txt
--rw-rw-r--   0 dml       (1000) dml       (1000)       38 2024-04-11 15:10:41.798424 ikctl-0.1.9/setup.cfg
--rw-rw-r--   0 dml       (1000) dml       (1000)      735 2024-04-11 15:07:46.000000 ikctl-0.1.9/setup.py
+drwxr-xr-x   0 davidmoyalopez   (501) staff       (20)        0 2024-05-11 21:08:15.810305 ikctl-0.2.11/
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)    11357 2024-05-01 15:41:01.000000 ikctl-0.2.11/LICENSE
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)     2415 2024-05-11 21:08:15.810092 ikctl-0.2.11/PKG-INFO
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)     2033 2024-05-09 10:30:58.000000 ikctl-0.2.11/README.md
+drwxr-xr-x   0 davidmoyalopez   (501) staff       (20)        0 2024-05-11 21:08:15.808772 ikctl-0.2.11/ikctl/
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)       30 2024-05-01 15:41:01.000000 ikctl-0.2.11/ikctl/__init__.py
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)     1048 2024-05-11 21:04:11.000000 ikctl-0.2.11/ikctl/commands.py
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)     4427 2024-05-11 21:04:11.000000 ikctl-0.2.11/ikctl/config.py
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)     1607 2024-05-01 15:41:01.000000 ikctl-0.2.11/ikctl/connect.py
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)     1282 2024-05-01 15:41:01.000000 ikctl-0.2.11/ikctl/context.py
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)     3514 2024-05-11 21:04:11.000000 ikctl-0.2.11/ikctl/create_config_files.py
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)      970 2024-05-01 15:41:01.000000 ikctl-0.2.11/ikctl/execute.py
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)      327 2024-05-01 15:41:01.000000 ikctl-0.2.11/ikctl/logs.py
+-rwxr-xr-x   0 davidmoyalopez   (501) staff       (20)      794 2024-05-01 15:41:01.000000 ikctl-0.2.11/ikctl/main.py
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)     3023 2024-05-01 15:41:01.000000 ikctl-0.2.11/ikctl/pipeline.py
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)      927 2024-05-01 15:41:01.000000 ikctl-0.2.11/ikctl/sftp.py
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)     1044 2024-05-01 15:41:01.000000 ikctl-0.2.11/ikctl/view.py
+drwxr-xr-x   0 davidmoyalopez   (501) staff       (20)        0 2024-05-11 21:08:15.809877 ikctl-0.2.11/ikctl.egg-info/
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)     2415 2024-05-11 21:08:15.000000 ikctl-0.2.11/ikctl.egg-info/PKG-INFO
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)      408 2024-05-11 21:08:15.000000 ikctl-0.2.11/ikctl.egg-info/SOURCES.txt
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)        1 2024-05-11 21:08:15.000000 ikctl-0.2.11/ikctl.egg-info/dependency_links.txt
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)       51 2024-05-11 21:08:15.000000 ikctl-0.2.11/ikctl.egg-info/entry_points.txt
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)       23 2024-05-11 21:08:15.000000 ikctl-0.2.11/ikctl.egg-info/requires.txt
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)        6 2024-05-11 21:08:15.000000 ikctl-0.2.11/ikctl.egg-info/top_level.txt
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)       38 2024-05-11 21:08:15.810346 ikctl-0.2.11/setup.cfg
+-rw-r--r--   0 davidmoyalopez   (501) staff       (20)      736 2024-05-11 21:08:12.000000 ikctl-0.2.11/setup.py
```

### Comparing `ikctl-0.1.9/LICENSE` & `ikctl-0.2.11/LICENSE`

 * *Files identical despite different names*

### Comparing `ikctl-0.1.9/PKG-INFO` & `ikctl-0.2.11/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ikctl
-Version: 0.1.9
+Version: 0.2.11
 Summary: App to installer packages on remote servers
 Home-page: https://github.com/3nueves/ikctl
 Author: David Moya López
 Author-email: 3nueves@gmail.com
 License: Apache v2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ikctl-0.1.9/README.md` & `ikctl-0.2.11/README.md`

 * *Files identical despite different names*

### Comparing `ikctl-0.1.9/ikctl/commands.py` & `ikctl-0.2.11/ikctl/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self.logger = logging.basicConfig(level=logging.INFO)
         self.logger = logging.getLogger(__name__)
 
     def ssh_run_command(self):
         """ execute script bash in remote server """
 
         try:
-            self.logger.info(re.sub("echo (.*) \|","echo ************ |",f'EXEC: {self.command}\n'))
+            self.logger.info(re.sub("echo (.*) |","echo ************ |",f'EXEC: {self.command}\n'))
             stdin, stdout, stderr = self.client.exec_command(self.command)
             for l in stdout :
                 print(f"{l.strip()}")
             # for l in stderr:
             #     print(f"stderr: {l.strip()}")
             self.check = stdout.channel.recv_exit_status()
```

### Comparing `ikctl-0.1.9/ikctl/config.py` & `ikctl-0.2.11/ikctl/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,44 +30,59 @@
             self.config = EnvYAML(self.path_config_file, strict=False)
 
         except ValueError as error:
             print(f'\n--- {error} ---\n')
             sys.exit()
 
         except Exception as e:
-            print(f"\nERROR IN FILE: {self.path_config_file}\n\n", e)
+            # print(f"\nERROR IN FILE: {self.path_config_file}\n\n", e)
+            print("\n",e)
             sys.exit()
 
         return self.config
 
 
     def load_config_file_kits(self):
         """ Load kits """
-        kits = (self.config['contexts'][self.context]['path_kits'])
+
+        try:
+            kits = (self.config['contexts'][self.context]['path_kits'])
+
+        except (ValueError, KeyError) as error:
+            print(f'\n keyError: {error} has a mistake\n')
+            sys.exit()
+
         try:
             kit = EnvYAML(kits + "/ikctl.yaml")
             if kit.get("kits"):
                 return kit
             else:
                 print(f"\nERROR IN FILE: {kits}/ikctl.yaml\n")
                 sys.exit()
 
-        except (ValueError, KeyError) as error:
-            print(f'\n--- {error} ---\n')
+        except (ValueError, KeyError):
+            print(f'\n KeyError: {error} there is a mistake\n')
             sys.exit()
 
         except Exception as e:
             print()
             print("[ikctl - kits configs]",e,"\n")
             sys.exit()
         
 
     def load_config_file_servers(self):
         """ Load Hosts """
-        servers = (self.config['contexts'][self.context]['path_servers'])
+
+        try:
+            servers = (self.config['contexts'][self.context]['path_servers'])
+        
+        except (ValueError, KeyError) as error:
+            print(f'\n keyError: {error} has a mistake\n')
+            sys.exit()
+
         try:
             return EnvYAML(servers + "/config.yaml")
 
         except (ValueError) as error:
             print(f'\n--- {error} ---\n')
             sys.exit()
```

### Comparing `ikctl-0.1.9/ikctl/connect.py` & `ikctl-0.2.11/ikctl/connect.py`

 * *Files identical despite different names*

### Comparing `ikctl-0.1.9/ikctl/context.py` & `ikctl-0.2.11/ikctl/context.py`

 * *Files identical despite different names*

### Comparing `ikctl-0.1.9/ikctl/execute.py` & `ikctl-0.2.11/ikctl/execute.py`

 * *Files identical despite different names*

### Comparing `ikctl-0.1.9/ikctl/main.py` & `ikctl-0.2.11/ikctl/main.py`

 * *Files identical despite different names*

### Comparing `ikctl-0.1.9/ikctl/pipeline.py` & `ikctl-0.2.11/ikctl/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,32 +55,32 @@
 
             # Load kit
             kits = self.data.extrac_config_kits(self.config_kits, options.install)
             if kits is None:
                 print("Kit not found")
                 sys.exit()
 
-        for host in hosts:
-            conn = Connection(user, port, host, pkey, password)
-            folder = self.sftp.list_dir(conn.connection_sftp, conn.user)
-            if ".ikctl" not in folder:
-                self.logger.info("Create folder ikctl")
-                self.sftp.create_folder(conn.connection_sftp)
-
-            print("###  Starting ikctl ###\n")
-
-            self.logger.info('HOST: %s\n', conn.host)
-
-            for local_kit in kits:
-                # Destination route where we will upload the kits to the remote server
-                remote_kit = ".ikctl/" + path.basename(local_kit)
-                self.logger.info('UPLOAD: %s\n', remote_kit)
-                self.sftp.upload_file(conn.connection_sftp, local_kit, remote_kit)
-                self.kit_not_match = False
-                    
-            if ".sh" in remote_kit:
-                check, log, err = self.exe.run(conn, options, remote_kit, "script", password)
-                self.log.stdout(self.logger, log, err, check, level="DEBUG")
+            for host in hosts:
+                conn = Connection(user, port, host, pkey, password)
+                folder = self.sftp.list_dir(conn.connection_sftp, conn.user)
+                if ".ikctl" not in folder:
+                    self.logger.info("Create folder ikctl")
+                    self.sftp.create_folder(conn.connection_sftp)
+
+                print("###  Starting ikctl ###\n")
+
+                self.logger.info('HOST: %s\n', conn.host)
+
+                for local_kit in kits:
+                    # Destination route where we will upload the kits to the remote server
+                    remote_kit = ".ikctl/" + path.basename(local_kit)
+                    self.logger.info('UPLOAD: %s\n', remote_kit)
+                    self.sftp.upload_file(conn.connection_sftp, local_kit, remote_kit)
+                    self.kit_not_match = False
+                        
+                if ".sh" in remote_kit:
+                    check, log, err = self.exe.run(conn, options, remote_kit, "script", password)
+                    self.log.stdout(self.logger, log, err, check, level="DEBUG")
 
-            self.logger.info(":END\n")
+                self.logger.info(":END\n")
 
-            conn.close_conn_sftp()
+                conn.close_conn_sftp()
```

### Comparing `ikctl-0.1.9/ikctl/sftp.py` & `ikctl-0.2.11/ikctl/sftp.py`

 * *Files identical despite different names*

### Comparing `ikctl-0.1.9/ikctl/view.py` & `ikctl-0.2.11/ikctl/view.py`

 * *Files identical despite different names*

### Comparing `ikctl-0.1.9/ikctl.egg-info/PKG-INFO` & `ikctl-0.2.11/ikctl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ikctl
-Version: 0.1.9
+Version: 0.2.11
 Summary: App to installer packages on remote servers
 Home-page: https://github.com/3nueves/ikctl
 Author: David Moya López
 Author-email: 3nueves@gmail.com
 License: Apache v2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ikctl-0.1.9/setup.py` & `ikctl-0.2.11/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='ikctl',
-    version='0.1.9',
+    version='0.2.11',
     description="App to installer packages on remote servers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/3nueves/ikctl",
     author="David Moya López",
     author_email="3nueves@gmail.com",
     license="Apache v2.0",
```

