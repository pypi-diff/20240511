# Comparing `tmp/pisa_ssh-0.1.2.tar.gz` & `tmp/pisa_ssh-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pisa_ssh-0.1.2.tar", last modified: Wed May  8 21:52:19 2024, max compression
+gzip compressed data, was "pisa_ssh-0.1.3.tar", last modified: Sat May 11 15:43:32 2024, max compression
```

## Comparing `pisa_ssh-0.1.2.tar` & `pisa_ssh-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:52:19.627584 pisa_ssh-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-08 21:52:05.000000 pisa_ssh-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-08 21:52:19.627584 pisa_ssh-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-08 21:52:05.000000 pisa_ssh-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-08 21:52:05.000000 pisa_ssh-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 21:52:19.627584 pisa_ssh-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:52:19.623584 pisa_ssh-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:52:19.627584 pisa_ssh-0.1.2/src/pisa/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-08 21:52:05.000000 pisa_ssh-0.1.2/src/pisa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-08 21:52:05.000000 pisa_ssh-0.1.2/src/pisa/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-08 21:52:05.000000 pisa_ssh-0.1.2/src/pisa/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:52:19.627584 pisa_ssh-0.1.2/src/pisa/dispatcher/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-08 21:52:05.000000 pisa_ssh-0.1.2/src/pisa/dispatcher/cluster_conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-08 21:52:05.000000 pisa_ssh-0.1.2/src/pisa/dispatcher/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-08 21:52:05.000000 pisa_ssh-0.1.2/src/pisa/dispatcher/task_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:52:19.627584 pisa_ssh-0.1.2/src/pisa/ssh/
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-08 21:52:05.000000 pisa_ssh-0.1.2/src/pisa/ssh/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:52:19.627584 pisa_ssh-0.1.2/src/pisa_ssh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-08 21:52:19.000000 pisa_ssh-0.1.2/src/pisa_ssh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-08 21:52:19.000000 pisa_ssh-0.1.2/src/pisa_ssh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 21:52:19.000000 pisa_ssh-0.1.2/src/pisa_ssh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-08 21:52:19.000000 pisa_ssh-0.1.2/src/pisa_ssh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 21:52:19.000000 pisa_ssh-0.1.2/src/pisa_ssh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-08 21:52:19.000000 pisa_ssh-0.1.2/src/pisa_ssh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:43:32.779174 pisa_ssh-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-11 15:43:17.000000 pisa_ssh-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-11 15:43:32.779174 pisa_ssh-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-11 15:43:17.000000 pisa_ssh-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-11 15:43:17.000000 pisa_ssh-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 15:43:32.779174 pisa_ssh-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:43:32.775174 pisa_ssh-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:43:32.779174 pisa_ssh-0.1.3/src/pisa/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-11 15:43:17.000000 pisa_ssh-0.1.3/src/pisa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-11 15:43:17.000000 pisa_ssh-0.1.3/src/pisa/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-11 15:43:17.000000 pisa_ssh-0.1.3/src/pisa/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:43:32.779174 pisa_ssh-0.1.3/src/pisa/dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-11 15:43:17.000000 pisa_ssh-0.1.3/src/pisa/dispatcher/cluster_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-11 15:43:17.000000 pisa_ssh-0.1.3/src/pisa/dispatcher/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-11 15:43:17.000000 pisa_ssh-0.1.3/src/pisa/dispatcher/task_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:43:32.779174 pisa_ssh-0.1.3/src/pisa/ssh/
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-11 15:43:17.000000 pisa_ssh-0.1.3/src/pisa/ssh/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:43:32.779174 pisa_ssh-0.1.3/src/pisa_ssh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-11 15:43:32.000000 pisa_ssh-0.1.3/src/pisa_ssh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-11 15:43:32.000000 pisa_ssh-0.1.3/src/pisa_ssh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 15:43:32.000000 pisa_ssh-0.1.3/src/pisa_ssh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-11 15:43:32.000000 pisa_ssh-0.1.3/src/pisa_ssh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-11 15:43:32.000000 pisa_ssh-0.1.3/src/pisa_ssh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-11 15:43:32.000000 pisa_ssh-0.1.3/src/pisa_ssh.egg-info/top_level.txt
```

### Comparing `pisa_ssh-0.1.2/LICENSE` & `pisa_ssh-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pisa_ssh-0.1.2/PKG-INFO` & `pisa_ssh-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pisa-ssh
-Version: 0.1.2
+Version: 0.1.3
 Summary: Pseudo Infrastructure for Scalable Applications (PISA)
 Author-email: Michael Hohenstein <michael@hohenste.in>
 License: MIT
 Project-URL: Homepage, https://github.com/MitchiLaser/pisa/blob/main/docs/README.md
 Project-URL: Repository, https://github.com/MitchiLaser/pisa
 Keywords: data,analysis,education,university,students,physics
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,10 +25,10 @@
 Requires-Dist: twine; extra == "dev"
 
 # pisa
 Pseudo Infrastructure for Scalable Applications (PISA)
 
 PISA is a simple but powerful program that allows to combine the computational power of multiple computers and turn them into a batch system using only the SSH access. It is designed to be simple and therefore only runs on a some machines from the computer pool of the physics department at KIT. It is not designed to be a general purpose batch system and is only maintained for this environment. Furthermore it is not designed to be used by many users at the same time because there is no limit provided for the allocated resources (our estimation is that only one person at the time will be using it). The large benefit of PISA is that it runs completely within the userspace and requires neither root access or higher privileges for installation nor to run the program.
 
-PISA connects to all the available machines using SSH. This only works when the authentication via an SSH key was set up before. Otherwise the connection cannot be established. Furthermore it requires the working directory (usually the home directory of all the users) to be the same on all machines. This is usual for our environment because the user home directories are mounted via NFS. The user interface is kept as simple as possible: Everything is dome from the command line. PISA gets a list of all the available machines and starts to connect to every one of them.
+PISA connects to all the available machines using SSH. This only works when the authentication via an SSH key was set up before. Otherwise the connection cannot be established. Furthermore it requires the working directory (usually the home directory of all the users) to be the same on all machines. This is usual for our environment because the user home directories are mounted via NFS. To run a program on multiple machines a cluster configuration file and a task configuration file are required. An example for both can be seen in the [config](./config) directory. This directory also contains the example program for the provided task configuration. It is a good benchmark because all the tasks take a different time to run. The configuration file contains a virtual environment because you always need one!
 
-TODO: Write more about the architecture.
+Now you know everything to use it. If there are any questions or problems feel free to create an issue.
```

### Comparing `pisa_ssh-0.1.2/README.md` & `pisa_ssh-0.1.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 # pisa
 Pseudo Infrastructure for Scalable Applications (PISA)
 
 PISA is a simple but powerful program that allows to combine the computational power of multiple computers and turn them into a batch system using only the SSH access. It is designed to be simple and therefore only runs on a some machines from the computer pool of the physics department at KIT. It is not designed to be a general purpose batch system and is only maintained for this environment. Furthermore it is not designed to be used by many users at the same time because there is no limit provided for the allocated resources (our estimation is that only one person at the time will be using it). The large benefit of PISA is that it runs completely within the userspace and requires neither root access or higher privileges for installation nor to run the program.
 
-PISA connects to all the available machines using SSH. This only works when the authentication via an SSH key was set up before. Otherwise the connection cannot be established. Furthermore it requires the working directory (usually the home directory of all the users) to be the same on all machines. This is usual for our environment because the user home directories are mounted via NFS. The user interface is kept as simple as possible: Everything is dome from the command line. PISA gets a list of all the available machines and starts to connect to every one of them.
+PISA connects to all the available machines using SSH. This only works when the authentication via an SSH key was set up before. Otherwise the connection cannot be established. Furthermore it requires the working directory (usually the home directory of all the users) to be the same on all machines. This is usual for our environment because the user home directories are mounted via NFS. To run a program on multiple machines a cluster configuration file and a task configuration file are required. An example for both can be seen in the [config](./config) directory. This directory also contains the example program for the provided task configuration. It is a good benchmark because all the tasks take a different time to run. The configuration file contains a virtual environment because you always need one!
 
-TODO: Write more about the architecture.
+Now you know everything to use it. If there are any questions or problems feel free to create an issue.
```

### Comparing `pisa_ssh-0.1.2/pyproject.toml` & `pisa_ssh-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pisa_ssh-0.1.2/src/pisa/__main__.py` & `pisa_ssh-0.1.3/src/pisa/__main__.py`

 * *Files identical despite different names*

### Comparing `pisa_ssh-0.1.2/src/pisa/dispatcher/cluster_conf.py` & `pisa_ssh-0.1.3/src/pisa/dispatcher/cluster_conf.py`

 * *Files identical despite different names*

### Comparing `pisa_ssh-0.1.2/src/pisa/dispatcher/dispatcher.py` & `pisa_ssh-0.1.3/src/pisa/dispatcher/dispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
             ssh.Session(node.get_address()) \
                 .connect() \
                 .send_command(f"cd {task.w_dir}") \
                 .send_command(f"./{task.env}/bin/activate") \
                 .send_command(f"mkdir -p {task.out}") \
                 .send_command(f"mkdir -p {task.err}") \
-                .send_command(f"{task.cmd} >{task.out}/{task.num}.out 2>{task.err}/{task.num}.err") \
+                .send_command(f"nice -n 19 {task.cmd} >{task.out}/{task.num}.out 2>{task.err}/{task.num}.err") \
                 .close()
             # log.debug(f"{task.cmd} >{task.out}/{task.num}.out 2>{task.err}/{task.num}.err &")  # TODO: remove
         except queue.Empty:  # queue is empty: exit thread
             has_task = False
             break
         except FileNotFoundError as e:  # file not found: program is not available
             log.error(f"file not found: {e}")
```

### Comparing `pisa_ssh-0.1.2/src/pisa/dispatcher/task_list.py` & `pisa_ssh-0.1.3/src/pisa/dispatcher/task_list.py`

 * *Files identical despite different names*

### Comparing `pisa_ssh-0.1.2/src/pisa/ssh/ssh.py` & `pisa_ssh-0.1.3/src/pisa/ssh/ssh.py`

 * *Files identical despite different names*

### Comparing `pisa_ssh-0.1.2/src/pisa_ssh.egg-info/PKG-INFO` & `pisa_ssh-0.1.3/src/pisa_ssh.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pisa-ssh
-Version: 0.1.2
+Version: 0.1.3
 Summary: Pseudo Infrastructure for Scalable Applications (PISA)
 Author-email: Michael Hohenstein <michael@hohenste.in>
 License: MIT
 Project-URL: Homepage, https://github.com/MitchiLaser/pisa/blob/main/docs/README.md
 Project-URL: Repository, https://github.com/MitchiLaser/pisa
 Keywords: data,analysis,education,university,students,physics
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,10 +25,10 @@
 Requires-Dist: twine; extra == "dev"
 
 # pisa
 Pseudo Infrastructure for Scalable Applications (PISA)
 
 PISA is a simple but powerful program that allows to combine the computational power of multiple computers and turn them into a batch system using only the SSH access. It is designed to be simple and therefore only runs on a some machines from the computer pool of the physics department at KIT. It is not designed to be a general purpose batch system and is only maintained for this environment. Furthermore it is not designed to be used by many users at the same time because there is no limit provided for the allocated resources (our estimation is that only one person at the time will be using it). The large benefit of PISA is that it runs completely within the userspace and requires neither root access or higher privileges for installation nor to run the program.
 
-PISA connects to all the available machines using SSH. This only works when the authentication via an SSH key was set up before. Otherwise the connection cannot be established. Furthermore it requires the working directory (usually the home directory of all the users) to be the same on all machines. This is usual for our environment because the user home directories are mounted via NFS. The user interface is kept as simple as possible: Everything is dome from the command line. PISA gets a list of all the available machines and starts to connect to every one of them.
+PISA connects to all the available machines using SSH. This only works when the authentication via an SSH key was set up before. Otherwise the connection cannot be established. Furthermore it requires the working directory (usually the home directory of all the users) to be the same on all machines. This is usual for our environment because the user home directories are mounted via NFS. To run a program on multiple machines a cluster configuration file and a task configuration file are required. An example for both can be seen in the [config](./config) directory. This directory also contains the example program for the provided task configuration. It is a good benchmark because all the tasks take a different time to run. The configuration file contains a virtual environment because you always need one!
 
-TODO: Write more about the architecture.
+Now you know everything to use it. If there are any questions or problems feel free to create an issue.
```

