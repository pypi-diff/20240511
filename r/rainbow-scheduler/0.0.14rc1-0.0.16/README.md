# Comparing `tmp/rainbow-scheduler-0.0.14rc1.tar.gz` & `tmp/rainbow-scheduler-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rainbow-scheduler-0.0.14rc1.tar", last modified: Thu Mar 21 08:11:14 2024, max compression
+gzip compressed data, was "rainbow-scheduler-0.0.16.tar", last modified: Sat May 11 17:25:45 2024, max compression
```

## Comparing `rainbow-scheduler-0.0.14rc1.tar` & `rainbow-scheduler-0.0.16.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-03-21 08:11:14.269810 rainbow-scheduler-0.0.14rc1/
--rw-r--r--   0 vanessa   (1000) vanessa   (1000)      135 2024-02-15 07:18:52.000000 rainbow-scheduler-0.0.14rc1/MANIFEST.in
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8585 2024-03-21 08:11:14.269810 rainbow-scheduler-0.0.14rc1/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7793 2024-03-09 21:47:02.000000 rainbow-scheduler-0.0.14rc1/README.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      168 2024-03-06 23:13:04.000000 rainbow-scheduler-0.0.14rc1/pyproject.toml
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-03-21 08:11:14.265810 rainbow-scheduler-0.0.14rc1/rainbow/
--rw-r--r--   0 vanessa   (1000) vanessa   (1000)        0 2024-02-15 07:18:52.000000 rainbow-scheduler-0.0.14rc1/rainbow/__init__.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-03-21 08:11:14.265810 rainbow-scheduler-0.0.14rc1/rainbow/backends/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      276 2024-03-06 23:13:04.000000 rainbow-scheduler-0.0.14rc1/rainbow/backends/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      714 2024-03-06 23:13:04.000000 rainbow-scheduler-0.0.14rc1/rainbow/backends/base.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      983 2024-03-06 23:13:04.000000 rainbow-scheduler-0.0.14rc1/rainbow/backends/memory.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7810 2024-03-21 08:09:29.000000 rainbow-scheduler-0.0.14rc1/rainbow/client.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3710 2024-03-06 23:13:04.000000 rainbow-scheduler-0.0.14rc1/rainbow/config.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       82 2024-03-06 23:13:04.000000 rainbow-scheduler-0.0.14rc1/rainbow/defaults.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-03-21 08:11:14.269810 rainbow-scheduler-0.0.14rc1/rainbow/protos/
--rw-r--r--   0 vanessa   (1000) vanessa   (1000)        0 2024-02-15 07:18:52.000000 rainbow-scheduler-0.0.14rc1/rainbow/protos/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2796 2024-03-21 08:06:30.000000 rainbow-scheduler-0.0.14rc1/rainbow/protos/memory_pb2.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2481 2024-03-20 19:40:49.000000 rainbow-scheduler-0.0.14rc1/rainbow/protos/memory_pb2.pyi
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3961 2024-03-21 08:06:30.000000 rainbow-scheduler-0.0.14rc1/rainbow/protos/memory_pb2_grpc.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6688 2024-03-21 08:09:29.000000 rainbow-scheduler-0.0.14rc1/rainbow/protos/rainbow_pb2.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7773 2024-03-21 08:09:29.000000 rainbow-scheduler-0.0.14rc1/rainbow/protos/rainbow_pb2.pyi
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     9207 2024-03-21 08:06:30.000000 rainbow-scheduler-0.0.14rc1/rainbow/protos/rainbow_pb2_grpc.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1709 2024-03-21 08:09:29.000000 rainbow-scheduler-0.0.14rc1/rainbow/schema.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      673 2024-03-06 23:13:04.000000 rainbow-scheduler-0.0.14rc1/rainbow/server.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      581 2024-03-06 23:13:04.000000 rainbow-scheduler-0.0.14rc1/rainbow/utils.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-03-21 08:11:14.269810 rainbow-scheduler-0.0.14rc1/rainbow_scheduler.egg-info/
--rw-r--r--   0 vanessa   (1000) vanessa   (1000)     8585 2024-03-21 08:11:14.000000 rainbow-scheduler-0.0.14rc1/rainbow_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 vanessa   (1000) vanessa   (1000)      725 2024-03-21 08:11:14.000000 rainbow-scheduler-0.0.14rc1/rainbow_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 vanessa   (1000) vanessa   (1000)        1 2024-03-21 08:11:14.000000 rainbow-scheduler-0.0.14rc1/rainbow_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 vanessa   (1000) vanessa   (1000)        1 2024-02-15 07:18:52.000000 rainbow-scheduler-0.0.14rc1/rainbow_scheduler.egg-info/not-zip-safe
--rw-r--r--   0 vanessa   (1000) vanessa   (1000)       46 2024-03-21 08:11:14.000000 rainbow-scheduler-0.0.14rc1/rainbow_scheduler.egg-info/requires.txt
--rw-r--r--   0 vanessa   (1000) vanessa   (1000)        8 2024-03-21 08:11:14.000000 rainbow-scheduler-0.0.14rc1/rainbow_scheduler.egg-info/top_level.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      152 2024-03-21 08:11:14.269810 rainbow-scheduler-0.0.14rc1/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1852 2024-03-21 08:11:06.000000 rainbow-scheduler-0.0.14rc1/setup.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-05-11 17:25:45.535792 rainbow-scheduler-0.0.16/
+-rw-r--r--   0 vanessa   (1000) vanessa   (1000)      135 2024-02-15 07:18:52.000000 rainbow-scheduler-0.0.16/MANIFEST.in
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     9596 2024-05-11 17:25:45.535792 rainbow-scheduler-0.0.16/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8807 2024-04-06 00:56:38.000000 rainbow-scheduler-0.0.16/README.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      168 2024-03-06 23:13:04.000000 rainbow-scheduler-0.0.16/pyproject.toml
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-05-11 17:25:45.531792 rainbow-scheduler-0.0.16/rainbow/
+-rw-r--r--   0 vanessa   (1000) vanessa   (1000)        0 2024-02-15 07:18:52.000000 rainbow-scheduler-0.0.16/rainbow/__init__.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-05-11 17:25:45.531792 rainbow-scheduler-0.0.16/rainbow/backends/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      276 2024-03-06 23:13:04.000000 rainbow-scheduler-0.0.16/rainbow/backends/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      714 2024-03-06 23:13:04.000000 rainbow-scheduler-0.0.16/rainbow/backends/base.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1017 2024-04-01 07:48:44.000000 rainbow-scheduler-0.0.16/rainbow/backends/memory.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    10001 2024-05-11 17:25:18.000000 rainbow-scheduler-0.0.16/rainbow/client.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5325 2024-05-11 17:25:18.000000 rainbow-scheduler-0.0.16/rainbow/config.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       82 2024-03-06 23:13:04.000000 rainbow-scheduler-0.0.16/rainbow/defaults.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-05-11 17:25:45.535792 rainbow-scheduler-0.0.16/rainbow/protos/
+-rw-r--r--   0 vanessa   (1000) vanessa   (1000)        0 2024-02-15 07:18:52.000000 rainbow-scheduler-0.0.16/rainbow/protos/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2970 2024-04-08 03:59:56.000000 rainbow-scheduler-0.0.16/rainbow/protos/memory_pb2.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2968 2024-04-08 03:46:37.000000 rainbow-scheduler-0.0.16/rainbow/protos/memory_pb2.pyi
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3961 2024-04-08 03:59:56.000000 rainbow-scheduler-0.0.16/rainbow/protos/memory_pb2_grpc.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8341 2024-04-08 21:52:49.000000 rainbow-scheduler-0.0.16/rainbow/protos/rainbow_pb2.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     9922 2024-04-08 21:52:49.000000 rainbow-scheduler-0.0.16/rainbow/protos/rainbow_pb2.pyi
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    10908 2024-04-08 03:59:56.000000 rainbow-scheduler-0.0.16/rainbow/protos/rainbow_pb2_grpc.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2263 2024-04-01 07:48:44.000000 rainbow-scheduler-0.0.16/rainbow/schema.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      673 2024-03-06 23:13:04.000000 rainbow-scheduler-0.0.16/rainbow/server.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      195 2024-04-08 21:52:49.000000 rainbow-scheduler-0.0.16/rainbow/types.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      581 2024-03-06 23:13:04.000000 rainbow-scheduler-0.0.16/rainbow/utils.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-05-11 17:25:45.535792 rainbow-scheduler-0.0.16/rainbow_scheduler.egg-info/
+-rw-r--r--   0 vanessa   (1000) vanessa   (1000)     9596 2024-05-11 17:25:45.000000 rainbow-scheduler-0.0.16/rainbow_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 vanessa   (1000) vanessa   (1000)      742 2024-05-11 17:25:45.000000 rainbow-scheduler-0.0.16/rainbow_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 vanessa   (1000) vanessa   (1000)        1 2024-05-11 17:25:45.000000 rainbow-scheduler-0.0.16/rainbow_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 vanessa   (1000) vanessa   (1000)        1 2024-02-15 07:18:52.000000 rainbow-scheduler-0.0.16/rainbow_scheduler.egg-info/not-zip-safe
+-rw-r--r--   0 vanessa   (1000) vanessa   (1000)       46 2024-05-11 17:25:45.000000 rainbow-scheduler-0.0.16/rainbow_scheduler.egg-info/requires.txt
+-rw-r--r--   0 vanessa   (1000) vanessa   (1000)        8 2024-05-11 17:25:45.000000 rainbow-scheduler-0.0.16/rainbow_scheduler.egg-info/top_level.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      152 2024-05-11 17:25:45.535792 rainbow-scheduler-0.0.16/setup.cfg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1849 2024-05-11 17:25:31.000000 rainbow-scheduler-0.0.16/setup.py
```

### Comparing `rainbow-scheduler-0.0.14rc1/PKG-INFO` & `rainbow-scheduler-0.0.16/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rainbow-scheduler
-Version: 0.0.14rc1
+Version: 0.0.16
 Summary: Python gRPC functions for the Rainbow Scheduler
 Home-page: https://github.com/converged-computing/rainbow/tree/main/python/v1
 Author: Vanessasaurus
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessasaurus
 License: MIT
 Keywords: multi-cluster,scheduler
@@ -117,14 +117,46 @@
    "nvme": 1,
    "shm": 1
   }
  }
 }
 ```
 
+### Update State
+
+While we likely will have clusters sending back state when they accept jobs, for now we have a separate endpoint to do a one-off request to update the state. You can test that here.
+
+```bash
+python ./examples/flux/update-state.py keebler --config-path ./rainbow-config.yaml
+```
+```console
+status: UPDATE_STATE_SUCCESS
+```
+
+In the server terminal (depending on your level of logging) you'll see the state update.
+
+```console
+2024/04/05 18:45:16 We have made an in memory graph (subsystem io) with 7 vertices, with 15 connections to the dominant!
+Metrics for subsystem io{
+ "io": 1,
+ "mtl1unit": 1,
+ "mtl2unit": 1,
+ "mtl3unit": 1,
+ "nvme": 1,
+ "shm": 1
+}
+2024/04/05 18:47:18 📝️ received state update: keebler
+Updating state cost-per-node to 12
+Updating state max-jobs to 100
+```
+
+Note that the path to the state metadata file is provided as a default to make the demo simple.
+This state metadata will be provided to the selection algorithm to use as needed to make choice for
+a final cluster.
+
 ### Submit Job (Simple)
 
 Now let's submit a job to our faux cluster. We need to provide the token we received above. Remember that this is a two stage process:
 
 1. Query the graph database for one or more cluster matches.
 2. Send that request to rainbow.
 
@@ -239,15 +271,15 @@
   --config-path CONFIG_PATH
                         config path with cluster metadata
 ```
 
 And then request and accept jobs:
 
 ```console
- python examples/flux/receive-jobs.py --config-path ./rainbow-config.yaml
+python examples/flux/receive-jobs.py --config-path ./rainbow-config.yaml
 Status: REQUEST_JOBS_SUCCESS
 Received 1 jobs to accept...
 ```
 
 If this were running in Flux, we would be able to run it, and the response above has told rainbow that you've accepted it (and rainbow deletes the record of it).
```

### Comparing `rainbow-scheduler-0.0.14rc1/README.md` & `rainbow-scheduler-0.0.16/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -96,14 +96,46 @@
    "nvme": 1,
    "shm": 1
   }
  }
 }
 ```
 
+### Update State
+
+While we likely will have clusters sending back state when they accept jobs, for now we have a separate endpoint to do a one-off request to update the state. You can test that here.
+
+```bash
+python ./examples/flux/update-state.py keebler --config-path ./rainbow-config.yaml
+```
+```console
+status: UPDATE_STATE_SUCCESS
+```
+
+In the server terminal (depending on your level of logging) you'll see the state update.
+
+```console
+2024/04/05 18:45:16 We have made an in memory graph (subsystem io) with 7 vertices, with 15 connections to the dominant!
+Metrics for subsystem io{
+ "io": 1,
+ "mtl1unit": 1,
+ "mtl2unit": 1,
+ "mtl3unit": 1,
+ "nvme": 1,
+ "shm": 1
+}
+2024/04/05 18:47:18 📝️ received state update: keebler
+Updating state cost-per-node to 12
+Updating state max-jobs to 100
+```
+
+Note that the path to the state metadata file is provided as a default to make the demo simple.
+This state metadata will be provided to the selection algorithm to use as needed to make choice for
+a final cluster.
+
 ### Submit Job (Simple)
 
 Now let's submit a job to our faux cluster. We need to provide the token we received above. Remember that this is a two stage process:
 
 1. Query the graph database for one or more cluster matches.
 2. Send that request to rainbow.
 
@@ -218,15 +250,15 @@
   --config-path CONFIG_PATH
                         config path with cluster metadata
 ```
 
 And then request and accept jobs:
 
 ```console
- python examples/flux/receive-jobs.py --config-path ./rainbow-config.yaml
+python examples/flux/receive-jobs.py --config-path ./rainbow-config.yaml
 Status: REQUEST_JOBS_SUCCESS
 Received 1 jobs to accept...
 ```
 
 If this were running in Flux, we would be able to run it, and the response above has told rainbow that you've accepted it (and rainbow deletes the record of it).
```

### Comparing `rainbow-scheduler-0.0.14rc1/rainbow/backends/base.py` & `rainbow-scheduler-0.0.16/rainbow/backends/base.py`

 * *Files identical despite different names*

### Comparing `rainbow-scheduler-0.0.14rc1/rainbow/backends/memory.py` & `rainbow-scheduler-0.0.16/rainbow/backends/memory.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 class MemoryBackend(GraphBackend):
     """
     A MemoryBackend is the rainbow default.
 
     This graph database backend is primarily for development.
     """
 
-    def satisfies(self, jobspec):
+    def satisfies(self, jobspec, matcher="match"):
         """
         Determine if a jobspec can be satisfied by the graph.
         """
         # Prepare a satisfy request with the jobspec
         # TODO if auth is in the graph, that needs to be done here too
-        request = memory_pb2.SatisfyRequest(payload=jobspec.to_str())
+        request = memory_pb2.SatisfyRequest(payload=jobspec.to_str(), matcher=matcher)
 
         # Host should be set from the database_options from the client
         with grpc.insecure_channel(self.host) as channel:
             stub = memory_pb2_grpc.MemoryGraphStub(channel)
             response = stub.Satisfy(request)
         return response
```

### Comparing `rainbow-scheduler-0.0.14rc1/rainbow/client.py` & `rainbow-scheduler-0.0.16/rainbow/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,31 +4,30 @@
 import grpc
 import jobspec.core as js
 import jobspec.core.converter as converter
 
 import rainbow.backends as backends
 import rainbow.config as config
 import rainbow.defaults as defaults
+import rainbow.types as types
 import rainbow.utils as utils
 from rainbow.protos import rainbow_pb2, rainbow_pb2_grpc
 
-# TODO need to register the databases here...
-
 
 class RainbowClient:
     """
     A RainbowClient is able to interact with a Rainbow cluster from Python.
     """
 
     def __init__(self, host="localhost:50051", config_file=None, database=None):
         """
         Create a new rainbow client to interact with a rainbow cluster.
         """
         self.cfg = config.RainbowConfig(config_file)
-        self.host = host or self.cfg.get("scheduler", {}).get("host")
+        self.host = self.cfg.get("graphdatabase", {}).get("options", {}).get("host") or host
 
         # load the graph database backend
         self.set_database(database)
         self.load_backend()
 
     def receive_jobs(self, max_jobs=None):
         """
@@ -99,14 +98,43 @@
         )
 
         with grpc.insecure_channel(self.host) as channel:
             stub = rainbow_pb2_grpc.RainbowSchedulerStub(channel)
             response = stub.Register(registerRequest)
         return response
 
+    def update_state(self, cluster, state_data, secret):
+        """
+        Update a cluster state
+        """
+        if not cluster:
+            raise ValueError("A cluster name is required to register")
+        if not secret:
+            raise ValueError("A secret is required to register")
+
+        # State file can be a file path or loaded state metadata
+        if not isinstance(state_data, dict) and not os.path.exists(state_data):
+            raise ValueError(f"State metadata file {state_data} does not exist.")
+
+        if isinstance(state_data, dict):
+            payload = state_data
+        else:
+            payload = utils.read_file(state_data)
+
+        # These are the variables for our cluster - name for now
+        request = rainbow_pb2.UpdateStateRequest(
+            cluster=cluster,
+            secret=secret,
+            payload=json.dumps(payload),
+        )
+        with grpc.insecure_channel(self.host) as channel:
+            stub = rainbow_pb2_grpc.RainbowSchedulerStub(channel)
+            response = stub.UpdateState(request)
+        return response
+
     def register_subsystem(self, cluster, subsystem, secret, nodes):
         """
         Register subsystem nodes to rainbow
         """
         if not cluster:
             raise ValueError("A cluster name is required to register")
         if not secret:
@@ -151,52 +179,81 @@
 
         # If we get here and no database, use the default
         if not database:
             database = defaults.database_backend
         self.database = database
         self.database_options = options
 
-    def submit_jobspec(self, jobspec):
+    def submit_jobspec(
+        self,
+        jobspec,
+        name=None,
+        match_algo=None,
+        select_algo=None,
+        select_options=None,
+        satisfy_only=False,
+    ):
         """
         Submit a jobspec directly. This is useful if you want to generate
         it custom with your own special logic.
         """
+        # Generate a random name if does not exist
+        name = name or jobspec.name
+
         # Ask the database backend if our jobspec can be satisfied
-        response = self.backend.satisfies(jobspec)
-        matches = response.clusters
+        match_algo = match_algo or self.cfg.match_algorithm
+        select_algo = select_algo or self.cfg.selection_algorithm
+        select_options = select_options or self.cfg.selection_algorithm_options
+        satisfy_response = self.backend.satisfies(jobspec, match_algo)
+        matches = satisfy_response.clusters
 
         # No matches?
         if not matches:
             print("No clusters match the request")
-            return response
+            return satisfy_response
 
         # TODO these need to have (again) the token and name checked
         # This is backwards because we check the token AFTER getting it, and it needs
         # to go to the graph (request above). I haven't implemented this yet.
         matches = self.cfg.get_clusters(matches)
         clusters = []
         for match in matches:
             clusters.append(
                 rainbow_pb2.SubmitJobRequest.Cluster(name=match["name"], token=match["token"])
             )
 
-        # THEN contact rainbwo with clusters
+        # THEN contact rainbow with clusters
         # These are submit variables. A more substantial submit script would have argparse, etc.
+
         submitRequest = rainbow_pb2.SubmitJobRequest(
-            name=jobspec.name,
+            name=name,
+            satisfy_only=satisfy_only,
             clusters=clusters,
+            select_algorithm=select_algo,
+            select_options=select_options,
             jobspec=jobspec.to_yaml(),
         )
 
         with grpc.insecure_channel(self.host) as channel:
             stub = rainbow_pb2_grpc.RainbowSchedulerStub(channel)
             response = stub.SubmitJob(submitRequest)
-        return response
 
-    def submit_job(self, command, nodes=1, tasks=1):
+        res = types.SatisfyResponse(
+            cluster=response.cluster,
+            total_matches=satisfy_response.total_matches,
+            total_mismatches=satisfy_response.total_mismatches,
+            total_clusters=satisfy_response.total_clusters,
+            status=response.status,
+            clusters=response.clusters,
+        )
+        return res
+
+    def submit_job(
+        self, command, nodes=1, tasks=1, match_algo=None, select_algo=None, satisfy_only=False
+    ):
         """
         Submit a simple job to rainbow. This includes:
 
         1. Converting the basic attributes into a jobspec (and validating)
         2. Reading and validating the cluster config
         3. Asking the graph for which clusters satisfy
         4. Then submitting to rainbow
@@ -209,8 +266,10 @@
         if isinstance(cmd, list):
             command = " ".join(cmd)
             print(f"⭐️ Submitting job: {cmd}")
 
         # Generate the jobspec dictionary
         raw = converter.new_simple_jobspec(nodes=nodes, command=command, tasks=tasks)
         jobspec = js.Jobspec(raw)
-        return self.submit_jobspec(jobspec)
+        return self.submit_jobspec(
+            jobspec, match_algo=match_algo, select_algo=select_algo, satisfy_only=satisfy_only
+        )
```

### Comparing `rainbow-scheduler-0.0.14rc1/rainbow/protos/memory_pb2.py` & `rainbow-scheduler-0.0.16/rainbow/protos/memory_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,33 +10,33 @@
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x0cmemory.proto\x12\x07service"C\n\x0fRegisterRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07payload\x18\x02 \x01(\t\x12\x11\n\tsubsystem\x18\x03 \x01(\t"!\n\x0eSatisfyRequest\x12\x0f\n\x07payload\x18\x01 \x01(\t"\xb3\x01\n\x0fSatisfyResponse\x12\x10\n\x08\x63lusters\x18\x01 \x03(\t\x12\x33\n\x06status\x18\x02 \x01(\x0e\x32#.service.SatisfyResponse.ResultType"Y\n\nResultType\x12\x1b\n\x17RESULT_TYPE_UNSPECIFIED\x10\x00\x12\x17\n\x13RESULT_TYPE_SUCCESS\x10\x01\x12\x15\n\x11RESULT_TYPE_ERROR\x10\x02"\x93\x01\n\x08Response\x12,\n\x06status\x18\x01 \x01(\x0e\x32\x1c.service.Response.ResultType"Y\n\nResultType\x12\x1b\n\x17RESULT_TYPE_UNSPECIFIED\x10\x00\x12\x17\n\x13RESULT_TYPE_SUCCESS\x10\x01\x12\x15\n\x11RESULT_TYPE_ERROR\x10\x02\x32\x88\x01\n\x0bMemoryGraph\x12>\n\x07Satisfy\x12\x17.service.SatisfyRequest\x1a\x18.service.SatisfyResponse"\x00\x12\x39\n\x08Register\x12\x18.service.RegisterRequest\x1a\x11.service.Response"\x00\x42@Z>github.com/converged-computing/rainbow/backends/memory/serviceb\x06proto3'
+    b'\n\x0cmemory.proto\x12\x07service"C\n\x0fRegisterRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07payload\x18\x02 \x01(\t\x12\x11\n\tsubsystem\x18\x03 \x01(\t"2\n\x0eSatisfyRequest\x12\x0f\n\x07payload\x18\x01 \x01(\t\x12\x0f\n\x07matcher\x18\x02 \x01(\t"\xfc\x01\n\x0fSatisfyResponse\x12\x10\n\x08\x63lusters\x18\x01 \x03(\t\x12\x33\n\x06status\x18\x02 \x01(\x0e\x32#.service.SatisfyResponse.ResultType\x12\x16\n\x0etotal_clusters\x18\x03 \x01(\x05\x12\x15\n\rtotal_matches\x18\x04 \x01(\x05\x12\x18\n\x10total_mismatches\x18\x05 \x01(\x05"Y\n\nResultType\x12\x1b\n\x17RESULT_TYPE_UNSPECIFIED\x10\x00\x12\x17\n\x13RESULT_TYPE_SUCCESS\x10\x01\x12\x15\n\x11RESULT_TYPE_ERROR\x10\x02"\x93\x01\n\x08Response\x12,\n\x06status\x18\x01 \x01(\x0e\x32\x1c.service.Response.ResultType"Y\n\nResultType\x12\x1b\n\x17RESULT_TYPE_UNSPECIFIED\x10\x00\x12\x17\n\x13RESULT_TYPE_SUCCESS\x10\x01\x12\x15\n\x11RESULT_TYPE_ERROR\x10\x02\x32\x88\x01\n\x0bMemoryGraph\x12>\n\x07Satisfy\x12\x17.service.SatisfyRequest\x1a\x18.service.SatisfyResponse"\x00\x12\x39\n\x08Register\x12\x18.service.RegisterRequest\x1a\x11.service.Response"\x00\x42@Z>github.com/converged-computing/rainbow/backends/memory/serviceb\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "memory_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     _globals["DESCRIPTOR"]._options = None
     _globals[
         "DESCRIPTOR"
     ]._serialized_options = b"Z>github.com/converged-computing/rainbow/backends/memory/service"
     _globals["_REGISTERREQUEST"]._serialized_start = 25
     _globals["_REGISTERREQUEST"]._serialized_end = 92
     _globals["_SATISFYREQUEST"]._serialized_start = 94
-    _globals["_SATISFYREQUEST"]._serialized_end = 127
-    _globals["_SATISFYRESPONSE"]._serialized_start = 130
-    _globals["_SATISFYRESPONSE"]._serialized_end = 309
-    _globals["_SATISFYRESPONSE_RESULTTYPE"]._serialized_start = 220
-    _globals["_SATISFYRESPONSE_RESULTTYPE"]._serialized_end = 309
-    _globals["_RESPONSE"]._serialized_start = 312
-    _globals["_RESPONSE"]._serialized_end = 459
-    _globals["_RESPONSE_RESULTTYPE"]._serialized_start = 220
-    _globals["_RESPONSE_RESULTTYPE"]._serialized_end = 309
-    _globals["_MEMORYGRAPH"]._serialized_start = 462
-    _globals["_MEMORYGRAPH"]._serialized_end = 598
+    _globals["_SATISFYREQUEST"]._serialized_end = 144
+    _globals["_SATISFYRESPONSE"]._serialized_start = 147
+    _globals["_SATISFYRESPONSE"]._serialized_end = 399
+    _globals["_SATISFYRESPONSE_RESULTTYPE"]._serialized_start = 310
+    _globals["_SATISFYRESPONSE_RESULTTYPE"]._serialized_end = 399
+    _globals["_RESPONSE"]._serialized_start = 402
+    _globals["_RESPONSE"]._serialized_end = 549
+    _globals["_RESPONSE_RESULTTYPE"]._serialized_start = 310
+    _globals["_RESPONSE_RESULTTYPE"]._serialized_end = 399
+    _globals["_MEMORYGRAPH"]._serialized_start = 552
+    _globals["_MEMORYGRAPH"]._serialized_end = 688
 # @@protoc_insertion_point(module_scope)
```

### Comparing `rainbow-scheduler-0.0.14rc1/rainbow/protos/memory_pb2.pyi` & `rainbow-scheduler-0.0.16/rainbow/protos/memory_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -13,34 +13,42 @@
     SUBSYSTEM_FIELD_NUMBER: _ClassVar[int]
     name: str
     payload: str
     subsystem: str
     def __init__(self, name: _Optional[str] = ..., payload: _Optional[str] = ..., subsystem: _Optional[str] = ...) -> None: ...
 
 class SatisfyRequest(_message.Message):
-    __slots__ = ("payload",)
+    __slots__ = ("payload", "matcher")
     PAYLOAD_FIELD_NUMBER: _ClassVar[int]
+    MATCHER_FIELD_NUMBER: _ClassVar[int]
     payload: str
-    def __init__(self, payload: _Optional[str] = ...) -> None: ...
+    matcher: str
+    def __init__(self, payload: _Optional[str] = ..., matcher: _Optional[str] = ...) -> None: ...
 
 class SatisfyResponse(_message.Message):
-    __slots__ = ("clusters", "status")
+    __slots__ = ("clusters", "status", "total_clusters", "total_matches", "total_mismatches")
     class ResultType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = ()
         RESULT_TYPE_UNSPECIFIED: _ClassVar[SatisfyResponse.ResultType]
         RESULT_TYPE_SUCCESS: _ClassVar[SatisfyResponse.ResultType]
         RESULT_TYPE_ERROR: _ClassVar[SatisfyResponse.ResultType]
     RESULT_TYPE_UNSPECIFIED: SatisfyResponse.ResultType
     RESULT_TYPE_SUCCESS: SatisfyResponse.ResultType
     RESULT_TYPE_ERROR: SatisfyResponse.ResultType
     CLUSTERS_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
+    TOTAL_CLUSTERS_FIELD_NUMBER: _ClassVar[int]
+    TOTAL_MATCHES_FIELD_NUMBER: _ClassVar[int]
+    TOTAL_MISMATCHES_FIELD_NUMBER: _ClassVar[int]
     clusters: _containers.RepeatedScalarFieldContainer[str]
     status: SatisfyResponse.ResultType
-    def __init__(self, clusters: _Optional[_Iterable[str]] = ..., status: _Optional[_Union[SatisfyResponse.ResultType, str]] = ...) -> None: ...
+    total_clusters: int
+    total_matches: int
+    total_mismatches: int
+    def __init__(self, clusters: _Optional[_Iterable[str]] = ..., status: _Optional[_Union[SatisfyResponse.ResultType, str]] = ..., total_clusters: _Optional[int] = ..., total_matches: _Optional[int] = ..., total_mismatches: _Optional[int] = ...) -> None: ...
 
 class Response(_message.Message):
     __slots__ = ("status",)
     class ResultType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = ()
         RESULT_TYPE_UNSPECIFIED: _ClassVar[Response.ResultType]
         RESULT_TYPE_SUCCESS: _ClassVar[Response.ResultType]
```

### Comparing `rainbow-scheduler-0.0.14rc1/rainbow/protos/memory_pb2_grpc.py` & `rainbow-scheduler-0.0.16/rainbow/protos/memory_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `rainbow-scheduler-0.0.14rc1/rainbow/protos/rainbow_pb2.py` & `rainbow-scheduler-0.0.16/rainbow/protos/rainbow_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,51 +12,61 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\rrainbow.proto\x12\x1e\x63onvergedcomputing.org.grpc.v1\x1a\x1fgoogle/protobuf/timestamp.proto"{\n\x0fRegisterRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06secret\x18\x02 \x01(\t\x12\r\n\x05nodes\x18\x03 \x01(\t\x12\x11\n\tsubsystem\x18\x04 \x01(\t\x12(\n\x04sent\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp"\xcf\x01\n\x10SubmitJobRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12J\n\x08\x63lusters\x18\x02 \x03(\x0b\x32\x38.convergedcomputing.org.grpc.v1.SubmitJobRequest.Cluster\x12\x0f\n\x07jobspec\x18\x03 \x01(\t\x12(\n\x04sent\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x1a&\n\x07\x43luster\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05token\x18\x02 \x01(\t"p\n\x12ReceiveJobsRequest\x12\x0f\n\x07\x63luster\x18\x01 \x01(\t\x12\x0e\n\x06secret\x18\x02 \x01(\t\x12\x0f\n\x07maxJobs\x18\x03 \x01(\x05\x12(\n\x04sent\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp"n\n\x11\x41\x63\x63\x65ptJobsRequest\x12\x0f\n\x07\x63luster\x18\x01 \x01(\t\x12\x0e\n\x06secret\x18\x02 \x01(\t\x12\x0e\n\x06jobids\x18\x03 \x03(\x05\x12(\n\x04sent\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp"\x8e\x02\n\x10RegisterResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\t\x12\r\n\x05token\x18\x02 \x01(\t\x12\x0e\n\x06secret\x18\x03 \x01(\t\x12K\n\x06status\x18\x04 \x01(\x0e\x32;.convergedcomputing.org.grpc.v1.RegisterResponse.ResultType"z\n\nResultType\x12\x18\n\x14REGISTER_UNSPECIFIED\x10\x00\x12\x14\n\x10REGISTER_SUCCESS\x10\x01\x12\x12\n\x0eREGISTER_ERROR\x10\x02\x12\x13\n\x0fREGISTER_DENIED\x10\x03\x12\x13\n\x0fREGISTER_EXISTS\x10\x04"\xf4\x01\n\x11SubmitJobResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\t\x12\r\n\x05jobid\x18\x02 \x01(\x05\x12\x0f\n\x07\x63luster\x18\x03 \x01(\t\x12L\n\x06status\x18\x04 \x01(\x0e\x32<.convergedcomputing.org.grpc.v1.SubmitJobResponse.ResultType"]\n\nResultType\x12\x16\n\x12SUBMIT_UNSPECIFIED\x10\x00\x12\x12\n\x0eSUBMIT_SUCCESS\x10\x01\x12\x10\n\x0cSUBMIT_ERROR\x10\x02\x12\x11\n\rSUBMIT_DENIED\x10\x03"\xe8\x02\n\x13ReceiveJobsResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\t\x12K\n\x04jobs\x18\x02 \x03(\x0b\x32=.convergedcomputing.org.grpc.v1.ReceiveJobsResponse.JobsEntry\x12N\n\x06status\x18\x03 \x01(\x0e\x32>.convergedcomputing.org.grpc.v1.ReceiveJobsResponse.ResultType\x1a+\n\tJobsEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01"s\n\nResultType\x12\x1a\n\x16REQUEST_JOBS_NORESULTS\x10\x00\x12\x18\n\x14REQUEST_JOBS_SUCCESS\x10\x01\x12\x16\n\x12REQUEST_JOBS_ERROR\x10\x02\x12\x17\n\x13REQUEST_JOBS_DENIED\x10\x03"\xd7\x01\n\x12\x41\x63\x63\x65ptJobsResponse\x12M\n\x06status\x18\x01 \x01(\x0e\x32=.convergedcomputing.org.grpc.v1.AcceptJobsResponse.ResultType"r\n\nResultType\x12\x1b\n\x17RESULT_TYPE_UNSPECIFIED\x10\x00\x12\x17\n\x13RESULT_TYPE_PARTIAL\x10\x01\x12\x17\n\x13RESULT_TYPE_SUCCESS\x10\x02\x12\x15\n\x11RESULT_TYPE_ERROR\x10\x03\x32\xd8\x04\n\x10RainbowScheduler\x12m\n\x08Register\x12/.convergedcomputing.org.grpc.v1.RegisterRequest\x1a\x30.convergedcomputing.org.grpc.v1.RegisterResponse\x12v\n\x11RegisterSubsystem\x12/.convergedcomputing.org.grpc.v1.RegisterRequest\x1a\x30.convergedcomputing.org.grpc.v1.RegisterResponse\x12p\n\tSubmitJob\x12\x30.convergedcomputing.org.grpc.v1.SubmitJobRequest\x1a\x31.convergedcomputing.org.grpc.v1.SubmitJobResponse\x12v\n\x0bReceiveJobs\x12\x32.convergedcomputing.org.grpc.v1.ReceiveJobsRequest\x1a\x33.convergedcomputing.org.grpc.v1.ReceiveJobsResponse\x12s\n\nAcceptJobs\x12\x31.convergedcomputing.org.grpc.v1.AcceptJobsRequest\x1a\x32.convergedcomputing.org.grpc.v1.AcceptJobsResponseB3Z1github.com/converged-computing/rainbow/pkg/api/v1b\x06proto3'
+    b'\n\rrainbow.proto\x12\x1e\x63onvergedcomputing.org.grpc.v1\x1a\x1fgoogle/protobuf/timestamp.proto"{\n\x0fRegisterRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06secret\x18\x02 \x01(\t\x12\r\n\x05nodes\x18\x03 \x01(\t\x12\x11\n\tsubsystem\x18\x04 \x01(\t\x12(\n\x04sent\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp"F\n\x12UpdateStateRequest\x12\x0f\n\x07\x63luster\x18\x01 \x01(\t\x12\x0e\n\x06secret\x18\x02 \x01(\t\x12\x0f\n\x07payload\x18\x03 \x01(\t"\xdd\x01\n\x13UpdateStateResponse\x12N\n\x06status\x18\x01 \x01(\x0e\x32>.convergedcomputing.org.grpc.v1.UpdateStateResponse.ResultType"v\n\nResultType\x12\x1c\n\x18UPDATE_STATE_UNSPECIFIED\x10\x00\x12\x18\n\x14UPDATE_STATE_PARTIAL\x10\x01\x12\x18\n\x14UPDATE_STATE_SUCCESS\x10\x02\x12\x16\n\x12UPDATE_STATE_ERROR\x10\x03"\x92\x03\n\x10SubmitJobRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12J\n\x08\x63lusters\x18\x02 \x03(\x0b\x32\x38.convergedcomputing.org.grpc.v1.SubmitJobRequest.Cluster\x12\x0f\n\x07jobspec\x18\x03 \x01(\t\x12\x18\n\x10select_algorithm\x18\x04 \x01(\t\x12[\n\x0eselect_options\x18\x05 \x03(\x0b\x32\x43.convergedcomputing.org.grpc.v1.SubmitJobRequest.SelectOptionsEntry\x12\x14\n\x0csatisfy_only\x18\x06 \x01(\x08\x12(\n\x04sent\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x1a\x34\n\x12SelectOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a&\n\x07\x43luster\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05token\x18\x02 \x01(\t"p\n\x12ReceiveJobsRequest\x12\x0f\n\x07\x63luster\x18\x01 \x01(\t\x12\x0e\n\x06secret\x18\x02 \x01(\t\x12\x0f\n\x07maxJobs\x18\x03 \x01(\x05\x12(\n\x04sent\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp"n\n\x11\x41\x63\x63\x65ptJobsRequest\x12\x0f\n\x07\x63luster\x18\x01 \x01(\t\x12\x0e\n\x06secret\x18\x02 \x01(\t\x12\x0e\n\x06jobids\x18\x03 \x03(\x05\x12(\n\x04sent\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp"\x8e\x02\n\x10RegisterResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\t\x12\r\n\x05token\x18\x02 \x01(\t\x12\x0e\n\x06secret\x18\x03 \x01(\t\x12K\n\x06status\x18\x04 \x01(\x0e\x32;.convergedcomputing.org.grpc.v1.RegisterResponse.ResultType"z\n\nResultType\x12\x18\n\x14REGISTER_UNSPECIFIED\x10\x00\x12\x14\n\x10REGISTER_SUCCESS\x10\x01\x12\x12\n\x0eREGISTER_ERROR\x10\x02\x12\x13\n\x0fREGISTER_DENIED\x10\x03\x12\x13\n\x0fREGISTER_EXISTS\x10\x04"\x86\x02\n\x11SubmitJobResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\t\x12\r\n\x05jobid\x18\x02 \x01(\x05\x12\x0f\n\x07\x63luster\x18\x03 \x01(\t\x12L\n\x06status\x18\x04 \x01(\x0e\x32<.convergedcomputing.org.grpc.v1.SubmitJobResponse.ResultType\x12\x10\n\x08\x63lusters\x18\x05 \x03(\t"]\n\nResultType\x12\x16\n\x12SUBMIT_UNSPECIFIED\x10\x00\x12\x12\n\x0eSUBMIT_SUCCESS\x10\x01\x12\x10\n\x0cSUBMIT_ERROR\x10\x02\x12\x11\n\rSUBMIT_DENIED\x10\x03"\xe8\x02\n\x13ReceiveJobsResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\t\x12K\n\x04jobs\x18\x02 \x03(\x0b\x32=.convergedcomputing.org.grpc.v1.ReceiveJobsResponse.JobsEntry\x12N\n\x06status\x18\x03 \x01(\x0e\x32>.convergedcomputing.org.grpc.v1.ReceiveJobsResponse.ResultType\x1a+\n\tJobsEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01"s\n\nResultType\x12\x1a\n\x16REQUEST_JOBS_NORESULTS\x10\x00\x12\x18\n\x14REQUEST_JOBS_SUCCESS\x10\x01\x12\x16\n\x12REQUEST_JOBS_ERROR\x10\x02\x12\x17\n\x13REQUEST_JOBS_DENIED\x10\x03"\xd7\x01\n\x12\x41\x63\x63\x65ptJobsResponse\x12M\n\x06status\x18\x01 \x01(\x0e\x32=.convergedcomputing.org.grpc.v1.AcceptJobsResponse.ResultType"r\n\nResultType\x12\x1b\n\x17RESULT_TYPE_UNSPECIFIED\x10\x00\x12\x17\n\x13RESULT_TYPE_PARTIAL\x10\x01\x12\x17\n\x13RESULT_TYPE_SUCCESS\x10\x02\x12\x15\n\x11RESULT_TYPE_ERROR\x10\x03\x32\xd0\x05\n\x10RainbowScheduler\x12m\n\x08Register\x12/.convergedcomputing.org.grpc.v1.RegisterRequest\x1a\x30.convergedcomputing.org.grpc.v1.RegisterResponse\x12v\n\x11RegisterSubsystem\x12/.convergedcomputing.org.grpc.v1.RegisterRequest\x1a\x30.convergedcomputing.org.grpc.v1.RegisterResponse\x12p\n\tSubmitJob\x12\x30.convergedcomputing.org.grpc.v1.SubmitJobRequest\x1a\x31.convergedcomputing.org.grpc.v1.SubmitJobResponse\x12v\n\x0bUpdateState\x12\x32.convergedcomputing.org.grpc.v1.UpdateStateRequest\x1a\x33.convergedcomputing.org.grpc.v1.UpdateStateResponse\x12v\n\x0bReceiveJobs\x12\x32.convergedcomputing.org.grpc.v1.ReceiveJobsRequest\x1a\x33.convergedcomputing.org.grpc.v1.ReceiveJobsResponse\x12s\n\nAcceptJobs\x12\x31.convergedcomputing.org.grpc.v1.AcceptJobsRequest\x1a\x32.convergedcomputing.org.grpc.v1.AcceptJobsResponseB3Z1github.com/converged-computing/rainbow/pkg/api/v1b\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "rainbow_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     _globals["DESCRIPTOR"]._options = None
     _globals[
         "DESCRIPTOR"
     ]._serialized_options = b"Z1github.com/converged-computing/rainbow/pkg/api/v1"
+    _globals["_SUBMITJOBREQUEST_SELECTOPTIONSENTRY"]._options = None
+    _globals["_SUBMITJOBREQUEST_SELECTOPTIONSENTRY"]._serialized_options = b"8\001"
     _globals["_RECEIVEJOBSRESPONSE_JOBSENTRY"]._options = None
     _globals["_RECEIVEJOBSRESPONSE_JOBSENTRY"]._serialized_options = b"8\001"
     _globals["_REGISTERREQUEST"]._serialized_start = 82
     _globals["_REGISTERREQUEST"]._serialized_end = 205
-    _globals["_SUBMITJOBREQUEST"]._serialized_start = 208
-    _globals["_SUBMITJOBREQUEST"]._serialized_end = 415
-    _globals["_SUBMITJOBREQUEST_CLUSTER"]._serialized_start = 377
-    _globals["_SUBMITJOBREQUEST_CLUSTER"]._serialized_end = 415
-    _globals["_RECEIVEJOBSREQUEST"]._serialized_start = 417
-    _globals["_RECEIVEJOBSREQUEST"]._serialized_end = 529
-    _globals["_ACCEPTJOBSREQUEST"]._serialized_start = 531
-    _globals["_ACCEPTJOBSREQUEST"]._serialized_end = 641
-    _globals["_REGISTERRESPONSE"]._serialized_start = 644
-    _globals["_REGISTERRESPONSE"]._serialized_end = 914
-    _globals["_REGISTERRESPONSE_RESULTTYPE"]._serialized_start = 792
-    _globals["_REGISTERRESPONSE_RESULTTYPE"]._serialized_end = 914
-    _globals["_SUBMITJOBRESPONSE"]._serialized_start = 917
-    _globals["_SUBMITJOBRESPONSE"]._serialized_end = 1161
-    _globals["_SUBMITJOBRESPONSE_RESULTTYPE"]._serialized_start = 1068
-    _globals["_SUBMITJOBRESPONSE_RESULTTYPE"]._serialized_end = 1161
-    _globals["_RECEIVEJOBSRESPONSE"]._serialized_start = 1164
-    _globals["_RECEIVEJOBSRESPONSE"]._serialized_end = 1524
-    _globals["_RECEIVEJOBSRESPONSE_JOBSENTRY"]._serialized_start = 1364
-    _globals["_RECEIVEJOBSRESPONSE_JOBSENTRY"]._serialized_end = 1407
-    _globals["_RECEIVEJOBSRESPONSE_RESULTTYPE"]._serialized_start = 1409
-    _globals["_RECEIVEJOBSRESPONSE_RESULTTYPE"]._serialized_end = 1524
-    _globals["_ACCEPTJOBSRESPONSE"]._serialized_start = 1527
-    _globals["_ACCEPTJOBSRESPONSE"]._serialized_end = 1742
-    _globals["_ACCEPTJOBSRESPONSE_RESULTTYPE"]._serialized_start = 1628
-    _globals["_ACCEPTJOBSRESPONSE_RESULTTYPE"]._serialized_end = 1742
-    _globals["_RAINBOWSCHEDULER"]._serialized_start = 1745
-    _globals["_RAINBOWSCHEDULER"]._serialized_end = 2345
+    _globals["_UPDATESTATEREQUEST"]._serialized_start = 207
+    _globals["_UPDATESTATEREQUEST"]._serialized_end = 277
+    _globals["_UPDATESTATERESPONSE"]._serialized_start = 280
+    _globals["_UPDATESTATERESPONSE"]._serialized_end = 501
+    _globals["_UPDATESTATERESPONSE_RESULTTYPE"]._serialized_start = 383
+    _globals["_UPDATESTATERESPONSE_RESULTTYPE"]._serialized_end = 501
+    _globals["_SUBMITJOBREQUEST"]._serialized_start = 504
+    _globals["_SUBMITJOBREQUEST"]._serialized_end = 906
+    _globals["_SUBMITJOBREQUEST_SELECTOPTIONSENTRY"]._serialized_start = 814
+    _globals["_SUBMITJOBREQUEST_SELECTOPTIONSENTRY"]._serialized_end = 866
+    _globals["_SUBMITJOBREQUEST_CLUSTER"]._serialized_start = 868
+    _globals["_SUBMITJOBREQUEST_CLUSTER"]._serialized_end = 906
+    _globals["_RECEIVEJOBSREQUEST"]._serialized_start = 908
+    _globals["_RECEIVEJOBSREQUEST"]._serialized_end = 1020
+    _globals["_ACCEPTJOBSREQUEST"]._serialized_start = 1022
+    _globals["_ACCEPTJOBSREQUEST"]._serialized_end = 1132
+    _globals["_REGISTERRESPONSE"]._serialized_start = 1135
+    _globals["_REGISTERRESPONSE"]._serialized_end = 1405
+    _globals["_REGISTERRESPONSE_RESULTTYPE"]._serialized_start = 1283
+    _globals["_REGISTERRESPONSE_RESULTTYPE"]._serialized_end = 1405
+    _globals["_SUBMITJOBRESPONSE"]._serialized_start = 1408
+    _globals["_SUBMITJOBRESPONSE"]._serialized_end = 1670
+    _globals["_SUBMITJOBRESPONSE_RESULTTYPE"]._serialized_start = 1577
+    _globals["_SUBMITJOBRESPONSE_RESULTTYPE"]._serialized_end = 1670
+    _globals["_RECEIVEJOBSRESPONSE"]._serialized_start = 1673
+    _globals["_RECEIVEJOBSRESPONSE"]._serialized_end = 2033
+    _globals["_RECEIVEJOBSRESPONSE_JOBSENTRY"]._serialized_start = 1873
+    _globals["_RECEIVEJOBSRESPONSE_JOBSENTRY"]._serialized_end = 1916
+    _globals["_RECEIVEJOBSRESPONSE_RESULTTYPE"]._serialized_start = 1918
+    _globals["_RECEIVEJOBSRESPONSE_RESULTTYPE"]._serialized_end = 2033
+    _globals["_ACCEPTJOBSRESPONSE"]._serialized_start = 2036
+    _globals["_ACCEPTJOBSRESPONSE"]._serialized_end = 2251
+    _globals["_ACCEPTJOBSRESPONSE_RESULTTYPE"]._serialized_start = 2137
+    _globals["_ACCEPTJOBSRESPONSE_RESULTTYPE"]._serialized_end = 2251
+    _globals["_RAINBOWSCHEDULER"]._serialized_start = 2254
+    _globals["_RAINBOWSCHEDULER"]._serialized_end = 2974
 # @@protoc_insertion_point(module_scope)
```

### Comparing `rainbow-scheduler-0.0.14rc1/rainbow/protos/rainbow_pb2.pyi` & `rainbow-scheduler-0.0.16/rainbow/protos/rainbow_pb2.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -17,32 +17,71 @@
     name: str
     secret: str
     nodes: str
     subsystem: str
     sent: _timestamp_pb2.Timestamp
     def __init__(self, name: _Optional[str] = ..., secret: _Optional[str] = ..., nodes: _Optional[str] = ..., subsystem: _Optional[str] = ..., sent: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
 
+class UpdateStateRequest(_message.Message):
+    __slots__ = ("cluster", "secret", "payload")
+    CLUSTER_FIELD_NUMBER: _ClassVar[int]
+    SECRET_FIELD_NUMBER: _ClassVar[int]
+    PAYLOAD_FIELD_NUMBER: _ClassVar[int]
+    cluster: str
+    secret: str
+    payload: str
+    def __init__(self, cluster: _Optional[str] = ..., secret: _Optional[str] = ..., payload: _Optional[str] = ...) -> None: ...
+
+class UpdateStateResponse(_message.Message):
+    __slots__ = ("status",)
+    class ResultType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = ()
+        UPDATE_STATE_UNSPECIFIED: _ClassVar[UpdateStateResponse.ResultType]
+        UPDATE_STATE_PARTIAL: _ClassVar[UpdateStateResponse.ResultType]
+        UPDATE_STATE_SUCCESS: _ClassVar[UpdateStateResponse.ResultType]
+        UPDATE_STATE_ERROR: _ClassVar[UpdateStateResponse.ResultType]
+    UPDATE_STATE_UNSPECIFIED: UpdateStateResponse.ResultType
+    UPDATE_STATE_PARTIAL: UpdateStateResponse.ResultType
+    UPDATE_STATE_SUCCESS: UpdateStateResponse.ResultType
+    UPDATE_STATE_ERROR: UpdateStateResponse.ResultType
+    STATUS_FIELD_NUMBER: _ClassVar[int]
+    status: UpdateStateResponse.ResultType
+    def __init__(self, status: _Optional[_Union[UpdateStateResponse.ResultType, str]] = ...) -> None: ...
+
 class SubmitJobRequest(_message.Message):
-    __slots__ = ("name", "clusters", "jobspec", "sent")
+    __slots__ = ("name", "clusters", "jobspec", "select_algorithm", "select_options", "satisfy_only", "sent")
+    class SelectOptionsEntry(_message.Message):
+        __slots__ = ("key", "value")
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: str
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
     class Cluster(_message.Message):
         __slots__ = ("name", "token")
         NAME_FIELD_NUMBER: _ClassVar[int]
         TOKEN_FIELD_NUMBER: _ClassVar[int]
         name: str
         token: str
         def __init__(self, name: _Optional[str] = ..., token: _Optional[str] = ...) -> None: ...
     NAME_FIELD_NUMBER: _ClassVar[int]
     CLUSTERS_FIELD_NUMBER: _ClassVar[int]
     JOBSPEC_FIELD_NUMBER: _ClassVar[int]
+    SELECT_ALGORITHM_FIELD_NUMBER: _ClassVar[int]
+    SELECT_OPTIONS_FIELD_NUMBER: _ClassVar[int]
+    SATISFY_ONLY_FIELD_NUMBER: _ClassVar[int]
     SENT_FIELD_NUMBER: _ClassVar[int]
     name: str
     clusters: _containers.RepeatedCompositeFieldContainer[SubmitJobRequest.Cluster]
     jobspec: str
+    select_algorithm: str
+    select_options: _containers.ScalarMap[str, str]
+    satisfy_only: bool
     sent: _timestamp_pb2.Timestamp
-    def __init__(self, name: _Optional[str] = ..., clusters: _Optional[_Iterable[_Union[SubmitJobRequest.Cluster, _Mapping]]] = ..., jobspec: _Optional[str] = ..., sent: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
+    def __init__(self, name: _Optional[str] = ..., clusters: _Optional[_Iterable[_Union[SubmitJobRequest.Cluster, _Mapping]]] = ..., jobspec: _Optional[str] = ..., select_algorithm: _Optional[str] = ..., select_options: _Optional[_Mapping[str, str]] = ..., satisfy_only: bool = ..., sent: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
 
 class ReceiveJobsRequest(_message.Message):
     __slots__ = ("cluster", "secret", "maxJobs", "sent")
     CLUSTER_FIELD_NUMBER: _ClassVar[int]
     SECRET_FIELD_NUMBER: _ClassVar[int]
     MAXJOBS_FIELD_NUMBER: _ClassVar[int]
     SENT_FIELD_NUMBER: _ClassVar[int]
@@ -85,34 +124,36 @@
     request_id: str
     token: str
     secret: str
     status: RegisterResponse.ResultType
     def __init__(self, request_id: _Optional[str] = ..., token: _Optional[str] = ..., secret: _Optional[str] = ..., status: _Optional[_Union[RegisterResponse.ResultType, str]] = ...) -> None: ...
 
 class SubmitJobResponse(_message.Message):
-    __slots__ = ("request_id", "jobid", "cluster", "status")
+    __slots__ = ("request_id", "jobid", "cluster", "status", "clusters")
     class ResultType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = ()
         SUBMIT_UNSPECIFIED: _ClassVar[SubmitJobResponse.ResultType]
         SUBMIT_SUCCESS: _ClassVar[SubmitJobResponse.ResultType]
         SUBMIT_ERROR: _ClassVar[SubmitJobResponse.ResultType]
         SUBMIT_DENIED: _ClassVar[SubmitJobResponse.ResultType]
     SUBMIT_UNSPECIFIED: SubmitJobResponse.ResultType
     SUBMIT_SUCCESS: SubmitJobResponse.ResultType
     SUBMIT_ERROR: SubmitJobResponse.ResultType
     SUBMIT_DENIED: SubmitJobResponse.ResultType
     REQUEST_ID_FIELD_NUMBER: _ClassVar[int]
     JOBID_FIELD_NUMBER: _ClassVar[int]
     CLUSTER_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
+    CLUSTERS_FIELD_NUMBER: _ClassVar[int]
     request_id: str
     jobid: int
     cluster: str
     status: SubmitJobResponse.ResultType
-    def __init__(self, request_id: _Optional[str] = ..., jobid: _Optional[int] = ..., cluster: _Optional[str] = ..., status: _Optional[_Union[SubmitJobResponse.ResultType, str]] = ...) -> None: ...
+    clusters: _containers.RepeatedScalarFieldContainer[str]
+    def __init__(self, request_id: _Optional[str] = ..., jobid: _Optional[int] = ..., cluster: _Optional[str] = ..., status: _Optional[_Union[SubmitJobResponse.ResultType, str]] = ..., clusters: _Optional[_Iterable[str]] = ...) -> None: ...
 
 class ReceiveJobsResponse(_message.Message):
     __slots__ = ("request_id", "jobs", "status")
     class ResultType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = ()
         REQUEST_JOBS_NORESULTS: _ClassVar[ReceiveJobsResponse.ResultType]
         REQUEST_JOBS_SUCCESS: _ClassVar[ReceiveJobsResponse.ResultType]
```

### Comparing `rainbow-scheduler-0.0.14rc1/rainbow/protos/rainbow_pb2_grpc.py` & `rainbow-scheduler-0.0.16/rainbow/protos/rainbow_pb2_grpc.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,14 +25,19 @@
             response_deserializer=rainbow__pb2.RegisterResponse.FromString,
         )
         self.SubmitJob = channel.unary_unary(
             "/convergedcomputing.org.grpc.v1.RainbowScheduler/SubmitJob",
             request_serializer=rainbow__pb2.SubmitJobRequest.SerializeToString,
             response_deserializer=rainbow__pb2.SubmitJobResponse.FromString,
         )
+        self.UpdateState = channel.unary_unary(
+            "/convergedcomputing.org.grpc.v1.RainbowScheduler/UpdateState",
+            request_serializer=rainbow__pb2.UpdateStateRequest.SerializeToString,
+            response_deserializer=rainbow__pb2.UpdateStateResponse.FromString,
+        )
         self.ReceiveJobs = channel.unary_unary(
             "/convergedcomputing.org.grpc.v1.RainbowScheduler/ReceiveJobs",
             request_serializer=rainbow__pb2.ReceiveJobsRequest.SerializeToString,
             response_deserializer=rainbow__pb2.ReceiveJobsResponse.FromString,
         )
         self.AcceptJobs = channel.unary_unary(
             "/convergedcomputing.org.grpc.v1.RainbowScheduler/AcceptJobs",
@@ -58,14 +63,22 @@
 
     def SubmitJob(self, request, context):
         """Job Submission - request for submitting a job to a named cluster"""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
+    def UpdateState(self, request, context):
+        """Update State - allow a cluster to provide state metadata
+        This is intended for use by a selection algorithm
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details("Method not implemented!")
+        raise NotImplementedError("Method not implemented!")
+
     def ReceiveJobs(self, request, context):
         """Request Job - ask the rainbow scheduler for up to max jobs"""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def AcceptJobs(self, request, context):
@@ -88,14 +101,19 @@
             response_serializer=rainbow__pb2.RegisterResponse.SerializeToString,
         ),
         "SubmitJob": grpc.unary_unary_rpc_method_handler(
             servicer.SubmitJob,
             request_deserializer=rainbow__pb2.SubmitJobRequest.FromString,
             response_serializer=rainbow__pb2.SubmitJobResponse.SerializeToString,
         ),
+        "UpdateState": grpc.unary_unary_rpc_method_handler(
+            servicer.UpdateState,
+            request_deserializer=rainbow__pb2.UpdateStateRequest.FromString,
+            response_serializer=rainbow__pb2.UpdateStateResponse.SerializeToString,
+        ),
         "ReceiveJobs": grpc.unary_unary_rpc_method_handler(
             servicer.ReceiveJobs,
             request_deserializer=rainbow__pb2.ReceiveJobsRequest.FromString,
             response_serializer=rainbow__pb2.ReceiveJobsResponse.SerializeToString,
         ),
         "AcceptJobs": grpc.unary_unary_rpc_method_handler(
             servicer.AcceptJobs,
@@ -193,14 +211,43 @@
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
+            metadata,
+        )
+
+    @staticmethod
+    def UpdateState(
+        request,
+        target,
+        options=(),
+        channel_credentials=None,
+        call_credentials=None,
+        insecure=False,
+        compression=None,
+        wait_for_ready=None,
+        timeout=None,
+        metadata=None,
+    ):
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            "/convergedcomputing.org.grpc.v1.RainbowScheduler/UpdateState",
+            rainbow__pb2.UpdateStateRequest.SerializeToString,
+            rainbow__pb2.UpdateStateResponse.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
             metadata,
         )
 
     @staticmethod
     def ReceiveJobs(
         request,
         target,
```

### Comparing `rainbow-scheduler-0.0.14rc1/rainbow/schema.py` & `rainbow-scheduler-0.0.16/rainbow/schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,29 +8,42 @@
     "properties": {
         "scheduler": {
             "description": "metadata for the rainbow scheduler",
             "type": "object",
             "properties": {
                 "name": {"type": "string"},
                 "secret": {"type": "string"},
-                "algorithm": {
+                "algorithms": {
                     "type": "object",
                     "properties": {
-                        "name": {"type": "string"},
-                        "options": {"type": "object"},
+                        "selection": {
+                            "type": "object",
+                            "properties": {
+                                "name": {"type": "string"},
+                                "options": {"type": "object"},
+                            },
+                        },
+                        "match": {
+                            "type": "object",
+                            "properties": {
+                                "name": {"type": "string"},
+                                "options": {"type": "object"},
+                            },
+                        },
                     },
                 },
                 "user": {"type": "object"},
             },
             "additionalProperties": False,
         },
         "graphdatabase": {
             "description": "metadata for the rainbow graph database",
             "type": "object",
             "properties": {
+                "host": {"type": "string"},
                 "name": {"type": "string"},
                 "options": {"type": "object"},
             },
             "additionalProperties": False,
         },
         "clusters": {
             "description": "listing of known clusters to submit to",
```

### Comparing `rainbow-scheduler-0.0.14rc1/rainbow/server.py` & `rainbow-scheduler-0.0.16/rainbow/server.py`

 * *Files identical despite different names*

### Comparing `rainbow-scheduler-0.0.14rc1/rainbow/utils.py` & `rainbow-scheduler-0.0.16/rainbow/utils.py`

 * *Files identical despite different names*

### Comparing `rainbow-scheduler-0.0.14rc1/rainbow_scheduler.egg-info/PKG-INFO` & `rainbow-scheduler-0.0.16/rainbow_scheduler.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rainbow-scheduler
-Version: 0.0.14rc1
+Version: 0.0.16
 Summary: Python gRPC functions for the Rainbow Scheduler
 Home-page: https://github.com/converged-computing/rainbow/tree/main/python/v1
 Author: Vanessasaurus
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessasaurus
 License: MIT
 Keywords: multi-cluster,scheduler
@@ -117,14 +117,46 @@
    "nvme": 1,
    "shm": 1
   }
  }
 }
 ```
 
+### Update State
+
+While we likely will have clusters sending back state when they accept jobs, for now we have a separate endpoint to do a one-off request to update the state. You can test that here.
+
+```bash
+python ./examples/flux/update-state.py keebler --config-path ./rainbow-config.yaml
+```
+```console
+status: UPDATE_STATE_SUCCESS
+```
+
+In the server terminal (depending on your level of logging) you'll see the state update.
+
+```console
+2024/04/05 18:45:16 We have made an in memory graph (subsystem io) with 7 vertices, with 15 connections to the dominant!
+Metrics for subsystem io{
+ "io": 1,
+ "mtl1unit": 1,
+ "mtl2unit": 1,
+ "mtl3unit": 1,
+ "nvme": 1,
+ "shm": 1
+}
+2024/04/05 18:47:18 📝️ received state update: keebler
+Updating state cost-per-node to 12
+Updating state max-jobs to 100
+```
+
+Note that the path to the state metadata file is provided as a default to make the demo simple.
+This state metadata will be provided to the selection algorithm to use as needed to make choice for
+a final cluster.
+
 ### Submit Job (Simple)
 
 Now let's submit a job to our faux cluster. We need to provide the token we received above. Remember that this is a two stage process:
 
 1. Query the graph database for one or more cluster matches.
 2. Send that request to rainbow.
 
@@ -239,15 +271,15 @@
   --config-path CONFIG_PATH
                         config path with cluster metadata
 ```
 
 And then request and accept jobs:
 
 ```console
- python examples/flux/receive-jobs.py --config-path ./rainbow-config.yaml
+python examples/flux/receive-jobs.py --config-path ./rainbow-config.yaml
 Status: REQUEST_JOBS_SUCCESS
 Received 1 jobs to accept...
 ```
 
 If this were running in Flux, we would be able to run it, and the response above has told rainbow that you've accepted it (and rainbow deletes the record of it).
```

### Comparing `rainbow-scheduler-0.0.14rc1/rainbow_scheduler.egg-info/SOURCES.txt` & `rainbow-scheduler-0.0.16/rainbow_scheduler.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 setup.py
 rainbow/__init__.py
 rainbow/client.py
 rainbow/config.py
 rainbow/defaults.py
 rainbow/schema.py
 rainbow/server.py
+rainbow/types.py
 rainbow/utils.py
 rainbow/backends/__init__.py
 rainbow/backends/base.py
 rainbow/backends/memory.py
 rainbow/protos/__init__.py
 rainbow/protos/memory_pb2.py
 rainbow/protos/memory_pb2.pyi
```

### Comparing `rainbow-scheduler-0.0.14rc1/setup.py` & `rainbow-scheduler-0.0.16/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ################################################################################
 # MAIN #########################################################################
 ################################################################################
 
 if __name__ == "__main__":
     setup(
         name="rainbow-scheduler",
-        version="0.0.14rc1",
+        version="0.0.16",
         author="Vanessasaurus",
         author_email="vsoch@users.noreply.github.com",
         maintainer="Vanessasaurus",
         packages=find_packages(),
         include_package_data=True,
         zip_safe=False,
         url="https://github.com/converged-computing/rainbow/tree/main/python/v1",
```

