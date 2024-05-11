# Comparing `tmp/openagents_grpc_proto-0.8.2.tar.gz` & `tmp/openagents_grpc_proto-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openagents_grpc_proto-0.8.2.tar", last modified: Fri May 10 08:32:17 2024, max compression
+gzip compressed data, was "openagents_grpc_proto-0.8.3.tar", last modified: Sat May 11 08:39:10 2024, max compression
```

## Comparing `openagents_grpc_proto-0.8.2.tar` & `openagents_grpc_proto-0.8.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:32:17.560743 openagents_grpc_proto-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-10 08:32:17.000000 openagents_grpc_proto-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-10 08:32:17.560743 openagents_grpc_proto-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 08:32:17.000000 openagents_grpc_proto-0.8.2/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:32:17.560743 openagents_grpc_proto-0.8.2/openagents_grpc_proto/
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-10 08:32:17.000000 openagents_grpc_proto-0.8.2/openagents_grpc_proto/JobInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-10 08:32:17.000000 openagents_grpc_proto-0.8.2/openagents_grpc_proto/JobInput_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-10 08:32:17.000000 openagents_grpc_proto-0.8.2/openagents_grpc_proto/JobParam_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-10 08:32:17.000000 openagents_grpc_proto-0.8.2/openagents_grpc_proto/JobParam_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-10 08:32:17.000000 openagents_grpc_proto-0.8.2/openagents_grpc_proto/JobResult_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-10 08:32:17.000000 openagents_grpc_proto-0.8.2/openagents_grpc_proto/JobResult_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-10 08:32:17.000000 openagents_grpc_proto-0.8.2/openagents_grpc_proto/JobState_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-10 08:32:17.000000 openagents_grpc_proto-0.8.2/openagents_grpc_proto/JobState_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-10 08:32:17.000000 openagents_grpc_proto-0.8.2/openagents_grpc_proto/JobStatus_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-10 08:32:17.000000 openagents_grpc_proto-0.8.2/openagents_grpc_proto/JobStatus_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-10 08:32:17.000000 openagents_grpc_proto-0.8.2/openagents_grpc_proto/Job_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-10 08:32:17.000000 openagents_grpc_proto-0.8.2/openagents_grpc_proto/Job_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-10 08:32:17.000000 openagents_grpc_proto-0.8.2/openagents_grpc_proto/Log_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-10 08:32:17.000000 openagents_grpc_proto-0.8.2/openagents_grpc_proto/Log_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-10 08:32:17.000000 openagents_grpc_proto-0.8.2/openagents_grpc_proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17234 2024-05-10 08:32:17.000000 openagents_grpc_proto-0.8.2/openagents_grpc_proto/rpc_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    55560 2024-05-10 08:32:17.000000 openagents_grpc_proto-0.8.2/openagents_grpc_proto/rpc_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:32:17.560743 openagents_grpc_proto-0.8.2/openagents_grpc_proto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-10 08:32:17.000000 openagents_grpc_proto-0.8.2/openagents_grpc_proto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-10 08:32:17.000000 openagents_grpc_proto-0.8.2/openagents_grpc_proto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:32:17.000000 openagents_grpc_proto-0.8.2/openagents_grpc_proto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-10 08:32:17.000000 openagents_grpc_proto-0.8.2/openagents_grpc_proto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 08:32:17.000000 openagents_grpc_proto-0.8.2/openagents_grpc_proto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 08:32:17.560743 openagents_grpc_proto-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-10 08:32:17.000000 openagents_grpc_proto-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:39:10.749891 openagents_grpc_proto-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-11 08:39:10.000000 openagents_grpc_proto-0.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-11 08:39:10.749891 openagents_grpc_proto-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-11 08:39:10.000000 openagents_grpc_proto-0.8.3/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:39:10.749891 openagents_grpc_proto-0.8.3/openagents_grpc_proto/
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-11 08:39:10.000000 openagents_grpc_proto-0.8.3/openagents_grpc_proto/JobInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-11 08:39:10.000000 openagents_grpc_proto-0.8.3/openagents_grpc_proto/JobInput_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-11 08:39:10.000000 openagents_grpc_proto-0.8.3/openagents_grpc_proto/JobParam_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-11 08:39:10.000000 openagents_grpc_proto-0.8.3/openagents_grpc_proto/JobParam_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-11 08:39:10.000000 openagents_grpc_proto-0.8.3/openagents_grpc_proto/JobResult_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-11 08:39:10.000000 openagents_grpc_proto-0.8.3/openagents_grpc_proto/JobResult_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-11 08:39:10.000000 openagents_grpc_proto-0.8.3/openagents_grpc_proto/JobState_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-11 08:39:10.000000 openagents_grpc_proto-0.8.3/openagents_grpc_proto/JobState_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-11 08:39:10.000000 openagents_grpc_proto-0.8.3/openagents_grpc_proto/JobStatus_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-11 08:39:10.000000 openagents_grpc_proto-0.8.3/openagents_grpc_proto/JobStatus_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-11 08:39:10.000000 openagents_grpc_proto-0.8.3/openagents_grpc_proto/Job_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-11 08:39:10.000000 openagents_grpc_proto-0.8.3/openagents_grpc_proto/Job_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-11 08:39:10.000000 openagents_grpc_proto-0.8.3/openagents_grpc_proto/Log_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-11 08:39:10.000000 openagents_grpc_proto-0.8.3/openagents_grpc_proto/Log_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-11 08:39:10.000000 openagents_grpc_proto-0.8.3/openagents_grpc_proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17303 2024-05-11 08:39:10.000000 openagents_grpc_proto-0.8.3/openagents_grpc_proto/rpc_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55560 2024-05-11 08:39:10.000000 openagents_grpc_proto-0.8.3/openagents_grpc_proto/rpc_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:39:10.749891 openagents_grpc_proto-0.8.3/openagents_grpc_proto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-11 08:39:10.000000 openagents_grpc_proto-0.8.3/openagents_grpc_proto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-11 08:39:10.000000 openagents_grpc_proto-0.8.3/openagents_grpc_proto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 08:39:10.000000 openagents_grpc_proto-0.8.3/openagents_grpc_proto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-11 08:39:10.000000 openagents_grpc_proto-0.8.3/openagents_grpc_proto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-11 08:39:10.000000 openagents_grpc_proto-0.8.3/openagents_grpc_proto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 08:39:10.749891 openagents_grpc_proto-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-11 08:39:10.000000 openagents_grpc_proto-0.8.3/setup.py
```

### Comparing `openagents_grpc_proto-0.8.2/openagents_grpc_proto/JobInput_pb2.py` & `openagents_grpc_proto-0.8.3/openagents_grpc_proto/JobInput_pb2.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.8.2/openagents_grpc_proto/JobInput_pb2_grpc.py` & `openagents_grpc_proto-0.8.3/openagents_grpc_proto/JobInput_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.8.2/openagents_grpc_proto/JobParam_pb2.py` & `openagents_grpc_proto-0.8.3/openagents_grpc_proto/JobParam_pb2.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.8.2/openagents_grpc_proto/JobParam_pb2_grpc.py` & `openagents_grpc_proto-0.8.3/openagents_grpc_proto/JobParam_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.8.2/openagents_grpc_proto/JobResult_pb2.py` & `openagents_grpc_proto-0.8.3/openagents_grpc_proto/JobResult_pb2.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.8.2/openagents_grpc_proto/JobResult_pb2_grpc.py` & `openagents_grpc_proto-0.8.3/openagents_grpc_proto/JobResult_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.8.2/openagents_grpc_proto/JobState_pb2.py` & `openagents_grpc_proto-0.8.3/openagents_grpc_proto/JobState_pb2.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.8.2/openagents_grpc_proto/JobState_pb2_grpc.py` & `openagents_grpc_proto-0.8.3/openagents_grpc_proto/JobState_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.8.2/openagents_grpc_proto/JobStatus_pb2.py` & `openagents_grpc_proto-0.8.3/openagents_grpc_proto/JobStatus_pb2.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.8.2/openagents_grpc_proto/JobStatus_pb2_grpc.py` & `openagents_grpc_proto-0.8.3/openagents_grpc_proto/JobStatus_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.8.2/openagents_grpc_proto/Job_pb2.py` & `openagents_grpc_proto-0.8.3/openagents_grpc_proto/Job_pb2.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.8.2/openagents_grpc_proto/Job_pb2_grpc.py` & `openagents_grpc_proto-0.8.3/openagents_grpc_proto/Job_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.8.2/openagents_grpc_proto/Log_pb2.py` & `openagents_grpc_proto-0.8.3/openagents_grpc_proto/Log_pb2.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.8.2/openagents_grpc_proto/Log_pb2_grpc.py` & `openagents_grpc_proto-0.8.3/openagents_grpc_proto/Log_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.8.2/openagents_grpc_proto/rpc_pb2.py` & `openagents_grpc_proto-0.8.3/openagents_grpc_proto/rpc_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,120 +17,120 @@
 import JobState_pb2 as JobState__pb2
 import JobParam_pb2 as JobParam__pb2
 import JobInput_pb2 as JobInput__pb2
 import JobResult_pb2 as JobResult__pb2
 import Job_pb2 as Job__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\trpc.proto\x1a\tLog.proto\x1a\x0fJobStatus.proto\x1a\x0eJobState.proto\x1a\x0eJobParam.proto\x1a\x0eJobInput.proto\x1a\x0fJobResult.proto\x1a\tJob.proto\"\x9c\x02\n\rRpcRequestJob\x12\r\n\x05runOn\x18\x01 \x01(\t\x12\x13\n\x0b\x65xpireAfter\x18\x02 \x01(\x04\x12\x18\n\x05input\x18\x03 \x03(\x0b\x32\t.JobInput\x12\x18\n\x05param\x18\x04 \x03(\x0b\x32\t.JobParam\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\x12\x11\n\x04kind\x18\x07 \x01(\rH\x00\x88\x01\x01\x12\x19\n\x0coutputFormat\x18\x08 \x01(\tH\x01\x88\x01\x01\x12\x1c\n\x0frequestProvider\x18\t \x01(\tH\x02\x88\x01\x01\x12\x16\n\tencrypted\x18\n \x01(\x08H\x03\x88\x01\x01\x42\x07\n\x05_kindB\x0f\n\r_outputFormatB\x12\n\x10_requestProviderB\x0c\n\n_encrypted\"6\n\tRpcGetJob\x12\r\n\x05jobId\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x63 \x01(\rH\x00\x88\x01\x01\x42\x07\n\x05_wait\"\xb2\x02\n\x11RpcGetPendingJobs\x12\x1a\n\rfilterByRunOn\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x1d\n\x10\x66ilterByCustomer\x18\x02 \x01(\tH\x01\x88\x01\x01\x12 \n\x13\x66ilterByDescription\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x17\n\nfilterById\x18\x04 \x01(\tH\x03\x88\x01\x01\x12\x19\n\x0c\x66ilterByKind\x18\x05 \x01(\tH\x04\x88\x01\x01\x12\x11\n\texcludeId\x18\x62 \x03(\t\x12\x11\n\x04wait\x18\x63 \x01(\rH\x05\x88\x01\x01\x42\x10\n\x0e_filterByRunOnB\x13\n\x11_filterByCustomerB\x16\n\x14_filterByDescriptionB\r\n\x0b_filterByIdB\x0f\n\r_filterByKindB\x07\n\x05_wait\"!\n\x0bPendingJobs\x12\x12\n\x04jobs\x18\x01 \x03(\x0b\x32\x04.Job\"\x1e\n\x0cRpcIsJobDone\x12\x0e\n\x06isDone\x18\x01 \x01(\x08\"\x1d\n\x0cRpcAcceptJob\x12\r\n\x05jobId\x18\x01 \x01(\t\"-\n\x0cRpcCancelJob\x12\r\n\x05jobId\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"-\n\x0cRpcJobOutput\x12\r\n\x05jobId\x18\x01 \x01(\t\x12\x0e\n\x06output\x18\x02 \x01(\t\"K\n\x0eRpcJobComplete\x12\r\n\x05jobId\x18\x01 \x01(\t\x12\x0e\n\x06output\x18\x02 \x01(\t\x12\x11\n\x04info\x18\x03 \x01(\tH\x00\x88\x01\x01\x42\x07\n\x05_info\"\'\n\tRpcJobLog\x12\r\n\x05jobId\x18\x01 \x01(\t\x12\x0b\n\x03log\x18\x02 \x01(\t\";\n\x19RpcSendSignedEventRequest\x12\x0f\n\x07groupId\x18\x01 \x01(\t\x12\r\n\x05\x65vent\x18\x02 \x01(\t\"?\n\x1bRpcSubscribeToEventsRequest\x12\x0f\n\x07groupId\x18\x01 \x01(\t\x12\x0f\n\x07\x66ilters\x18\x02 \x03(\t\"G\n\x1cRpcSubscribeToEventsResponse\x12\x0f\n\x07groupId\x18\x01 \x01(\t\x12\x16\n\x0esubscriptionId\x18\x02 \x01(\t\"M\n\x13RpcGetEventsRequest\x12\x0f\n\x07groupId\x18\x01 \x01(\t\x12\x16\n\x0esubscriptionId\x18\x02 \x01(\t\x12\r\n\x05limit\x18\x03 \x01(\r\"^\n\x14RpcGetEventsResponse\x12\x0f\n\x07groupId\x18\x01 \x01(\t\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12\x16\n\x0esubscriptionId\x18\x03 \x01(\t\x12\x0e\n\x06\x65vents\x18\x04 \x03(\t\">\n\x1aRpcSendSignedEventResponse\x12\x0f\n\x07groupId\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\"J\n\x1fRpcUnsubscribeFromEventsRequest\x12\x0f\n\x07groupId\x18\x01 \x01(\t\x12\x16\n\x0esubscriptionId\x18\x02 \x01(\t\"3\n RpcUnsubscribeFromEventsResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"L\n\x16RpcAnnounceNodeRequest\x12\x0f\n\x07iconUrl\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\"C\n\x17RpcAnnounceNodeResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x17\n\x0frefreshInterval\x18\x04 \x01(\x04\"M\n\x1aRpcAnnounceTemplateRequest\x12\x0c\n\x04meta\x18\x01 \x01(\t\x12\x10\n\x08template\x18\x02 \x01(\t\x12\x0f\n\x07sockets\x18\x03 \x01(\t\"G\n\x1bRpcAnnounceTemplateResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x17\n\x0frefreshInterval\x18\x04 \x01(\x04\"\xa6\x01\n\x14RpcCreateDiskRequest\x12\x11\n\x04name\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x1a\n\rencryptionKey\x18\x02 \x01(\tH\x01\x88\x01\x01\x12&\n\x19includeEncryptionKeyInUrl\x18\x03 \x01(\x08H\x02\x88\x01\x01\x42\x07\n\x05_nameB\x10\n\x0e_encryptionKeyB\x1c\n\x1a_includeEncryptionKeyInUrl\"$\n\x15RpcCreateDiskResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\"O\n\x12RpcOpenDiskRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x1a\n\rencryptionKey\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x10\n\x0e_encryptionKey\"G\n\x13RpcOpenDiskResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x0e\n\x06\x64iskId\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\x04\"%\n\x13RpcCloseDiskRequest\x12\x0e\n\x06\x64iskId\x18\x01 \x01(\t\"\'\n\x14RpcCloseDiskResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"8\n\x18RpcDiskDeleteFileRequest\x12\x0e\n\x06\x64iskId\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\",\n\x19RpcDiskDeleteFileResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"7\n\x17RpcDiskListFilesRequest\x12\x0e\n\x06\x64iskId\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\")\n\x18RpcDiskListFilesResponse\x12\r\n\x05\x66iles\x18\x01 \x03(\t\"6\n\x16RpcDiskReadFileRequest\x12\x0e\n\x06\x64iskId\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"7\n\x17RpcDiskReadFileResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\x12\x0e\n\x06\x65xists\x18\x02 \x01(\x08\"E\n\x17RpcDiskWriteFileRequest\x12\x0e\n\x06\x64iskId\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\"+\n\x18RpcDiskWriteFileResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"u\n\x12RpcCacheSetRequest\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\x12\x14\n\x07version\x18\x03 \x01(\x04H\x00\x88\x01\x01\x12\x15\n\x08\x65xpireAt\x18\x04 \x01(\x04H\x01\x88\x01\x01\x42\n\n\x08_versionB\x0b\n\t_expireAt\"&\n\x13RpcCacheSetResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"K\n\x12RpcCacheGetRequest\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x18\n\x0blastVersion\x18\x02 \x01(\x04H\x00\x88\x01\x01\x42\x0e\n\x0c_lastVersion\"3\n\x13RpcCacheGetResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\x12\x0e\n\x06\x65xists\x18\x02 \x01(\x08\"\x19\n\x17RpcDiscoverPoolsRequest\")\n\x18RpcDiscoverPoolsResponse\x12\r\n\x05pools\x18\x01 \x03(\t\"z\n\x17RpcDiscoverNodesRequest\x12\x15\n\rfilterByKinds\x18\x01 \x03(\x05\x12\x15\n\rfilterByPools\x18\x02 \x03(\t\x12\x15\n\rfilterByNodes\x18\x03 \x03(\t\x12\x1a\n\x12\x66ilterByKindRanges\x18\x04 \x03(\t\")\n\x18RpcDiscoverNodesResponse\x12\r\n\x05nodes\x18\x01 \x03(\t\"\x92\x01\n\x19RpcDiscoverActionsRequest\x12\x15\n\rfilterByKinds\x18\x01 \x03(\x05\x12\x15\n\rfilterByPools\x18\x02 \x03(\t\x12\x15\n\rfilterByNodes\x18\x03 \x03(\t\x12\x14\n\x0c\x66ilterByTags\x18\x04 \x03(\t\x12\x1a\n\x12\x66ilterByKindRanges\x18\x05 \x03(\t\"-\n\x1aRpcDiscoverActionsResponse\x12\x0f\n\x07\x61\x63tions\x18\x01 \x03(\t\"i\n\x1dRpcDiscoverNearbyNodesRequest\x12\x15\n\rfilterByKinds\x18\x01 \x03(\x05\x12\x15\n\rfilterByNodes\x18\x03 \x03(\t\x12\x1a\n\x12\x66ilterByKindRanges\x18\x05 \x03(\t\"/\n\x1eRpcDiscoverNearbyNodesResponse\x12\r\n\x05nodes\x18\x01 \x03(\t\"\x81\x01\n\x1fRpcDiscoverNearbyActionsRequest\x12\x15\n\rfilterByKinds\x18\x01 \x03(\x05\x12\x15\n\rfilterByNodes\x18\x03 \x03(\t\x12\x14\n\x0c\x66ilterByTags\x18\x04 \x03(\t\x12\x1a\n\x12\x66ilterByKindRanges\x18\x05 \x03(\t\"3\n RpcDiscoverNearbyActionsResponse\x12\x0f\n\x07\x61\x63tions\x18\x01 \x03(\t\"h\n\rRpcJobRequest\x12\r\n\x05\x65vent\x18\x01 \x01(\t\x12\x15\n\x08provider\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x16\n\tencrypted\x18\x03 \x01(\x08H\x01\x88\x01\x01\x42\x0b\n\t_providerB\x0c\n\n_encrypted2\xab\x0f\n\rPoolConnector\x12\"\n\nrequestJob\x12\x0e.RpcRequestJob\x1a\x04.Job\x12&\n\x0esendJobRequest\x12\x0e.RpcJobRequest\x1a\x04.Job\x12\x1a\n\x06getJob\x12\n.RpcGetJob\x1a\x04.Job\x12\x32\n\x0egetPendingJobs\x12\x12.RpcGetPendingJobs\x1a\x0c.PendingJobs\x12&\n\tisJobDone\x12\n.RpcGetJob\x1a\r.RpcIsJobDone\x12 \n\tacceptJob\x12\r.RpcAcceptJob\x1a\x04.Job\x12 \n\tcancelJob\x12\r.RpcCancelJob\x1a\x04.Job\x12#\n\x0coutputForJob\x12\r.RpcJobOutput\x1a\x04.Job\x12$\n\x0b\x63ompleteJob\x12\x0f.RpcJobComplete\x1a\x04.Job\x12\x1d\n\tlogForJob\x12\n.RpcJobLog\x1a\x04.Job\x12\x41\n\x0c\x61nnounceNode\x12\x17.RpcAnnounceNodeRequest\x1a\x18.RpcAnnounceNodeResponse\x12R\n\x15\x61nnounceEventTemplate\x12\x1b.RpcAnnounceTemplateRequest\x1a\x1c.RpcAnnounceTemplateResponse\x12\x44\n\rdiscoverPools\x12\x18.RpcDiscoverPoolsRequest\x1a\x19.RpcDiscoverPoolsResponse\x12\x44\n\rdiscoverNodes\x12\x18.RpcDiscoverNodesRequest\x1a\x19.RpcDiscoverNodesResponse\x12J\n\x0f\x64iscoverActions\x12\x1a.RpcDiscoverActionsRequest\x1a\x1b.RpcDiscoverActionsResponse\x12V\n\x13\x64iscoverNearbyNodes\x12\x1e.RpcDiscoverNearbyNodesRequest\x1a\x1f.RpcDiscoverNearbyNodesResponse\x12\\\n\x15\x64iscoverNearbyActions\x12 .RpcDiscoverNearbyActionsRequest\x1a!.RpcDiscoverNearbyActionsResponse\x12J\n\x0fsendSignedEvent\x12\x1a.RpcSendSignedEventRequest\x1a\x1b.RpcSendSignedEventResponse\x12P\n\x11subscribeToEvents\x12\x1c.RpcSubscribeToEventsRequest\x1a\x1d.RpcSubscribeToEventsResponse\x12\\\n\x15unsubscribeFromEvents\x12 .RpcUnsubscribeFromEventsRequest\x1a!.RpcUnsubscribeFromEventsResponse\x12\x38\n\tgetEvents\x12\x14.RpcGetEventsRequest\x1a\x15.RpcGetEventsResponse\x12;\n\ncreateDisk\x12\x15.RpcCreateDiskRequest\x1a\x16.RpcCreateDiskResponse\x12\x35\n\x08openDisk\x12\x13.RpcOpenDiskRequest\x1a\x14.RpcOpenDiskResponse\x12\x38\n\tcloseDisk\x12\x14.RpcCloseDiskRequest\x1a\x15.RpcCloseDiskResponse\x12G\n\x0e\x64iskDeleteFile\x12\x19.RpcDiskDeleteFileRequest\x1a\x1a.RpcDiskDeleteFileResponse\x12\x44\n\rdiskListFiles\x12\x18.RpcDiskListFilesRequest\x1a\x19.RpcDiskListFilesResponse\x12\x43\n\x0c\x64iskReadFile\x12\x17.RpcDiskReadFileRequest\x1a\x18.RpcDiskReadFileResponse0\x01\x12\x46\n\x11\x64iskReadSmallFile\x12\x17.RpcDiskReadFileRequest\x1a\x18.RpcDiskReadFileResponse\x12\x46\n\rdiskWriteFile\x12\x18.RpcDiskWriteFileRequest\x1a\x19.RpcDiskWriteFileResponse(\x01\x12I\n\x12\x64iskWriteSmallFile\x12\x18.RpcDiskWriteFileRequest\x1a\x19.RpcDiskWriteFileResponse\x12\x37\n\x08\x63\x61\x63heSet\x12\x13.RpcCacheSetRequest\x1a\x14.RpcCacheSetResponse(\x01\x12\x37\n\x08\x63\x61\x63heGet\x12\x13.RpcCacheGetRequest\x1a\x14.RpcCacheGetResponse0\x01\x42.\xca\x02\x0e\x41pp\\Grpc\\nostr\xe2\x02\x1a\x41pp\\Grpc\\nostr\\GPBMetadatab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\trpc.proto\x1a\tLog.proto\x1a\x0fJobStatus.proto\x1a\x0eJobState.proto\x1a\x0eJobParam.proto\x1a\x0eJobInput.proto\x1a\x0fJobResult.proto\x1a\tJob.proto\"\xbc\x02\n\rRpcRequestJob\x12\r\n\x05runOn\x18\x01 \x01(\t\x12\x13\n\x0b\x65xpireAfter\x18\x02 \x01(\x04\x12\x18\n\x05input\x18\x03 \x03(\x0b\x32\t.JobInput\x12\x18\n\x05param\x18\x04 \x03(\x0b\x32\t.JobParam\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\x12\x11\n\x04kind\x18\x07 \x01(\rH\x00\x88\x01\x01\x12\x19\n\x0coutputFormat\x18\x08 \x01(\tH\x01\x88\x01\x01\x12\x1c\n\x0frequestProvider\x18\t \x01(\tH\x02\x88\x01\x01\x12\x16\n\tencrypted\x18\n \x01(\x08H\x03\x88\x01\x01\x12\x13\n\x06userId\x18\x0b \x01(\tH\x04\x88\x01\x01\x42\x07\n\x05_kindB\x0f\n\r_outputFormatB\x12\n\x10_requestProviderB\x0c\n\n_encryptedB\t\n\x07_userId\"6\n\tRpcGetJob\x12\r\n\x05jobId\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x63 \x01(\rH\x00\x88\x01\x01\x42\x07\n\x05_wait\"\xb2\x02\n\x11RpcGetPendingJobs\x12\x1a\n\rfilterByRunOn\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x1d\n\x10\x66ilterByCustomer\x18\x02 \x01(\tH\x01\x88\x01\x01\x12 \n\x13\x66ilterByDescription\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x17\n\nfilterById\x18\x04 \x01(\tH\x03\x88\x01\x01\x12\x19\n\x0c\x66ilterByKind\x18\x05 \x01(\tH\x04\x88\x01\x01\x12\x11\n\texcludeId\x18\x62 \x03(\t\x12\x11\n\x04wait\x18\x63 \x01(\rH\x05\x88\x01\x01\x42\x10\n\x0e_filterByRunOnB\x13\n\x11_filterByCustomerB\x16\n\x14_filterByDescriptionB\r\n\x0b_filterByIdB\x0f\n\r_filterByKindB\x07\n\x05_wait\"!\n\x0bPendingJobs\x12\x12\n\x04jobs\x18\x01 \x03(\x0b\x32\x04.Job\"\x1e\n\x0cRpcIsJobDone\x12\x0e\n\x06isDone\x18\x01 \x01(\x08\"\x1d\n\x0cRpcAcceptJob\x12\r\n\x05jobId\x18\x01 \x01(\t\"-\n\x0cRpcCancelJob\x12\r\n\x05jobId\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"-\n\x0cRpcJobOutput\x12\r\n\x05jobId\x18\x01 \x01(\t\x12\x0e\n\x06output\x18\x02 \x01(\t\"K\n\x0eRpcJobComplete\x12\r\n\x05jobId\x18\x01 \x01(\t\x12\x0e\n\x06output\x18\x02 \x01(\t\x12\x11\n\x04info\x18\x03 \x01(\tH\x00\x88\x01\x01\x42\x07\n\x05_info\"\'\n\tRpcJobLog\x12\r\n\x05jobId\x18\x01 \x01(\t\x12\x0b\n\x03log\x18\x02 \x01(\t\";\n\x19RpcSendSignedEventRequest\x12\x0f\n\x07groupId\x18\x01 \x01(\t\x12\r\n\x05\x65vent\x18\x02 \x01(\t\"?\n\x1bRpcSubscribeToEventsRequest\x12\x0f\n\x07groupId\x18\x01 \x01(\t\x12\x0f\n\x07\x66ilters\x18\x02 \x03(\t\"G\n\x1cRpcSubscribeToEventsResponse\x12\x0f\n\x07groupId\x18\x01 \x01(\t\x12\x16\n\x0esubscriptionId\x18\x02 \x01(\t\"M\n\x13RpcGetEventsRequest\x12\x0f\n\x07groupId\x18\x01 \x01(\t\x12\x16\n\x0esubscriptionId\x18\x02 \x01(\t\x12\r\n\x05limit\x18\x03 \x01(\r\"^\n\x14RpcGetEventsResponse\x12\x0f\n\x07groupId\x18\x01 \x01(\t\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12\x16\n\x0esubscriptionId\x18\x03 \x01(\t\x12\x0e\n\x06\x65vents\x18\x04 \x03(\t\">\n\x1aRpcSendSignedEventResponse\x12\x0f\n\x07groupId\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\"J\n\x1fRpcUnsubscribeFromEventsRequest\x12\x0f\n\x07groupId\x18\x01 \x01(\t\x12\x16\n\x0esubscriptionId\x18\x02 \x01(\t\"3\n RpcUnsubscribeFromEventsResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"L\n\x16RpcAnnounceNodeRequest\x12\x0f\n\x07iconUrl\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\"C\n\x17RpcAnnounceNodeResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x17\n\x0frefreshInterval\x18\x04 \x01(\x04\"M\n\x1aRpcAnnounceTemplateRequest\x12\x0c\n\x04meta\x18\x01 \x01(\t\x12\x10\n\x08template\x18\x02 \x01(\t\x12\x0f\n\x07sockets\x18\x03 \x01(\t\"G\n\x1bRpcAnnounceTemplateResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x17\n\x0frefreshInterval\x18\x04 \x01(\x04\"\xa6\x01\n\x14RpcCreateDiskRequest\x12\x11\n\x04name\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x1a\n\rencryptionKey\x18\x02 \x01(\tH\x01\x88\x01\x01\x12&\n\x19includeEncryptionKeyInUrl\x18\x03 \x01(\x08H\x02\x88\x01\x01\x42\x07\n\x05_nameB\x10\n\x0e_encryptionKeyB\x1c\n\x1a_includeEncryptionKeyInUrl\"$\n\x15RpcCreateDiskResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\"O\n\x12RpcOpenDiskRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x1a\n\rencryptionKey\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x10\n\x0e_encryptionKey\"G\n\x13RpcOpenDiskResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x0e\n\x06\x64iskId\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\x04\"%\n\x13RpcCloseDiskRequest\x12\x0e\n\x06\x64iskId\x18\x01 \x01(\t\"\'\n\x14RpcCloseDiskResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"8\n\x18RpcDiskDeleteFileRequest\x12\x0e\n\x06\x64iskId\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\",\n\x19RpcDiskDeleteFileResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"7\n\x17RpcDiskListFilesRequest\x12\x0e\n\x06\x64iskId\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\")\n\x18RpcDiskListFilesResponse\x12\r\n\x05\x66iles\x18\x01 \x03(\t\"6\n\x16RpcDiskReadFileRequest\x12\x0e\n\x06\x64iskId\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"7\n\x17RpcDiskReadFileResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\x12\x0e\n\x06\x65xists\x18\x02 \x01(\x08\"E\n\x17RpcDiskWriteFileRequest\x12\x0e\n\x06\x64iskId\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\"+\n\x18RpcDiskWriteFileResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"u\n\x12RpcCacheSetRequest\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\x12\x14\n\x07version\x18\x03 \x01(\x04H\x00\x88\x01\x01\x12\x15\n\x08\x65xpireAt\x18\x04 \x01(\x04H\x01\x88\x01\x01\x42\n\n\x08_versionB\x0b\n\t_expireAt\"&\n\x13RpcCacheSetResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"K\n\x12RpcCacheGetRequest\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x18\n\x0blastVersion\x18\x02 \x01(\x04H\x00\x88\x01\x01\x42\x0e\n\x0c_lastVersion\"3\n\x13RpcCacheGetResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\x12\x0e\n\x06\x65xists\x18\x02 \x01(\x08\"\x19\n\x17RpcDiscoverPoolsRequest\")\n\x18RpcDiscoverPoolsResponse\x12\r\n\x05pools\x18\x01 \x03(\t\"z\n\x17RpcDiscoverNodesRequest\x12\x15\n\rfilterByKinds\x18\x01 \x03(\x05\x12\x15\n\rfilterByPools\x18\x02 \x03(\t\x12\x15\n\rfilterByNodes\x18\x03 \x03(\t\x12\x1a\n\x12\x66ilterByKindRanges\x18\x04 \x03(\t\")\n\x18RpcDiscoverNodesResponse\x12\r\n\x05nodes\x18\x01 \x03(\t\"\x92\x01\n\x19RpcDiscoverActionsRequest\x12\x15\n\rfilterByKinds\x18\x01 \x03(\x05\x12\x15\n\rfilterByPools\x18\x02 \x03(\t\x12\x15\n\rfilterByNodes\x18\x03 \x03(\t\x12\x14\n\x0c\x66ilterByTags\x18\x04 \x03(\t\x12\x1a\n\x12\x66ilterByKindRanges\x18\x05 \x03(\t\"-\n\x1aRpcDiscoverActionsResponse\x12\x0f\n\x07\x61\x63tions\x18\x01 \x03(\t\"i\n\x1dRpcDiscoverNearbyNodesRequest\x12\x15\n\rfilterByKinds\x18\x01 \x03(\x05\x12\x15\n\rfilterByNodes\x18\x03 \x03(\t\x12\x1a\n\x12\x66ilterByKindRanges\x18\x05 \x03(\t\"/\n\x1eRpcDiscoverNearbyNodesResponse\x12\r\n\x05nodes\x18\x01 \x03(\t\"\x81\x01\n\x1fRpcDiscoverNearbyActionsRequest\x12\x15\n\rfilterByKinds\x18\x01 \x03(\x05\x12\x15\n\rfilterByNodes\x18\x03 \x03(\t\x12\x14\n\x0c\x66ilterByTags\x18\x04 \x03(\t\x12\x1a\n\x12\x66ilterByKindRanges\x18\x05 \x03(\t\"3\n RpcDiscoverNearbyActionsResponse\x12\x0f\n\x07\x61\x63tions\x18\x01 \x03(\t\"h\n\rRpcJobRequest\x12\r\n\x05\x65vent\x18\x01 \x01(\t\x12\x15\n\x08provider\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x16\n\tencrypted\x18\x03 \x01(\x08H\x01\x88\x01\x01\x42\x0b\n\t_providerB\x0c\n\n_encrypted2\xab\x0f\n\rPoolConnector\x12\"\n\nrequestJob\x12\x0e.RpcRequestJob\x1a\x04.Job\x12&\n\x0esendJobRequest\x12\x0e.RpcJobRequest\x1a\x04.Job\x12\x1a\n\x06getJob\x12\n.RpcGetJob\x1a\x04.Job\x12\x32\n\x0egetPendingJobs\x12\x12.RpcGetPendingJobs\x1a\x0c.PendingJobs\x12&\n\tisJobDone\x12\n.RpcGetJob\x1a\r.RpcIsJobDone\x12 \n\tacceptJob\x12\r.RpcAcceptJob\x1a\x04.Job\x12 \n\tcancelJob\x12\r.RpcCancelJob\x1a\x04.Job\x12#\n\x0coutputForJob\x12\r.RpcJobOutput\x1a\x04.Job\x12$\n\x0b\x63ompleteJob\x12\x0f.RpcJobComplete\x1a\x04.Job\x12\x1d\n\tlogForJob\x12\n.RpcJobLog\x1a\x04.Job\x12\x41\n\x0c\x61nnounceNode\x12\x17.RpcAnnounceNodeRequest\x1a\x18.RpcAnnounceNodeResponse\x12R\n\x15\x61nnounceEventTemplate\x12\x1b.RpcAnnounceTemplateRequest\x1a\x1c.RpcAnnounceTemplateResponse\x12\x44\n\rdiscoverPools\x12\x18.RpcDiscoverPoolsRequest\x1a\x19.RpcDiscoverPoolsResponse\x12\x44\n\rdiscoverNodes\x12\x18.RpcDiscoverNodesRequest\x1a\x19.RpcDiscoverNodesResponse\x12J\n\x0f\x64iscoverActions\x12\x1a.RpcDiscoverActionsRequest\x1a\x1b.RpcDiscoverActionsResponse\x12V\n\x13\x64iscoverNearbyNodes\x12\x1e.RpcDiscoverNearbyNodesRequest\x1a\x1f.RpcDiscoverNearbyNodesResponse\x12\\\n\x15\x64iscoverNearbyActions\x12 .RpcDiscoverNearbyActionsRequest\x1a!.RpcDiscoverNearbyActionsResponse\x12J\n\x0fsendSignedEvent\x12\x1a.RpcSendSignedEventRequest\x1a\x1b.RpcSendSignedEventResponse\x12P\n\x11subscribeToEvents\x12\x1c.RpcSubscribeToEventsRequest\x1a\x1d.RpcSubscribeToEventsResponse\x12\\\n\x15unsubscribeFromEvents\x12 .RpcUnsubscribeFromEventsRequest\x1a!.RpcUnsubscribeFromEventsResponse\x12\x38\n\tgetEvents\x12\x14.RpcGetEventsRequest\x1a\x15.RpcGetEventsResponse\x12;\n\ncreateDisk\x12\x15.RpcCreateDiskRequest\x1a\x16.RpcCreateDiskResponse\x12\x35\n\x08openDisk\x12\x13.RpcOpenDiskRequest\x1a\x14.RpcOpenDiskResponse\x12\x38\n\tcloseDisk\x12\x14.RpcCloseDiskRequest\x1a\x15.RpcCloseDiskResponse\x12G\n\x0e\x64iskDeleteFile\x12\x19.RpcDiskDeleteFileRequest\x1a\x1a.RpcDiskDeleteFileResponse\x12\x44\n\rdiskListFiles\x12\x18.RpcDiskListFilesRequest\x1a\x19.RpcDiskListFilesResponse\x12\x43\n\x0c\x64iskReadFile\x12\x17.RpcDiskReadFileRequest\x1a\x18.RpcDiskReadFileResponse0\x01\x12\x46\n\x11\x64iskReadSmallFile\x12\x17.RpcDiskReadFileRequest\x1a\x18.RpcDiskReadFileResponse\x12\x46\n\rdiskWriteFile\x12\x18.RpcDiskWriteFileRequest\x1a\x19.RpcDiskWriteFileResponse(\x01\x12I\n\x12\x64iskWriteSmallFile\x12\x18.RpcDiskWriteFileRequest\x1a\x19.RpcDiskWriteFileResponse\x12\x37\n\x08\x63\x61\x63heSet\x12\x13.RpcCacheSetRequest\x1a\x14.RpcCacheSetResponse(\x01\x12\x37\n\x08\x63\x61\x63heGet\x12\x13.RpcCacheGetRequest\x1a\x14.RpcCacheGetResponse0\x01\x42.\xca\x02\x0e\x41pp\\Grpc\\nostr\xe2\x02\x1a\x41pp\\Grpc\\nostr\\GPBMetadatab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'rpc_pb2', _globals)
 if not _descriptor._USE_C_DESCRIPTORS:
   _globals['DESCRIPTOR']._loaded_options = None
   _globals['DESCRIPTOR']._serialized_options = b'\312\002\016App\\Grpc\\nostr\342\002\032App\\Grpc\\nostr\\GPBMetadata'
   _globals['_RPCREQUESTJOB']._serialized_start=118
-  _globals['_RPCREQUESTJOB']._serialized_end=402
-  _globals['_RPCGETJOB']._serialized_start=404
-  _globals['_RPCGETJOB']._serialized_end=458
-  _globals['_RPCGETPENDINGJOBS']._serialized_start=461
-  _globals['_RPCGETPENDINGJOBS']._serialized_end=767
-  _globals['_PENDINGJOBS']._serialized_start=769
-  _globals['_PENDINGJOBS']._serialized_end=802
-  _globals['_RPCISJOBDONE']._serialized_start=804
-  _globals['_RPCISJOBDONE']._serialized_end=834
-  _globals['_RPCACCEPTJOB']._serialized_start=836
-  _globals['_RPCACCEPTJOB']._serialized_end=865
-  _globals['_RPCCANCELJOB']._serialized_start=867
-  _globals['_RPCCANCELJOB']._serialized_end=912
-  _globals['_RPCJOBOUTPUT']._serialized_start=914
-  _globals['_RPCJOBOUTPUT']._serialized_end=959
-  _globals['_RPCJOBCOMPLETE']._serialized_start=961
-  _globals['_RPCJOBCOMPLETE']._serialized_end=1036
-  _globals['_RPCJOBLOG']._serialized_start=1038
-  _globals['_RPCJOBLOG']._serialized_end=1077
-  _globals['_RPCSENDSIGNEDEVENTREQUEST']._serialized_start=1079
-  _globals['_RPCSENDSIGNEDEVENTREQUEST']._serialized_end=1138
-  _globals['_RPCSUBSCRIBETOEVENTSREQUEST']._serialized_start=1140
-  _globals['_RPCSUBSCRIBETOEVENTSREQUEST']._serialized_end=1203
-  _globals['_RPCSUBSCRIBETOEVENTSRESPONSE']._serialized_start=1205
-  _globals['_RPCSUBSCRIBETOEVENTSRESPONSE']._serialized_end=1276
-  _globals['_RPCGETEVENTSREQUEST']._serialized_start=1278
-  _globals['_RPCGETEVENTSREQUEST']._serialized_end=1355
-  _globals['_RPCGETEVENTSRESPONSE']._serialized_start=1357
-  _globals['_RPCGETEVENTSRESPONSE']._serialized_end=1451
-  _globals['_RPCSENDSIGNEDEVENTRESPONSE']._serialized_start=1453
-  _globals['_RPCSENDSIGNEDEVENTRESPONSE']._serialized_end=1515
-  _globals['_RPCUNSUBSCRIBEFROMEVENTSREQUEST']._serialized_start=1517
-  _globals['_RPCUNSUBSCRIBEFROMEVENTSREQUEST']._serialized_end=1591
-  _globals['_RPCUNSUBSCRIBEFROMEVENTSRESPONSE']._serialized_start=1593
-  _globals['_RPCUNSUBSCRIBEFROMEVENTSRESPONSE']._serialized_end=1644
-  _globals['_RPCANNOUNCENODEREQUEST']._serialized_start=1646
-  _globals['_RPCANNOUNCENODEREQUEST']._serialized_end=1722
-  _globals['_RPCANNOUNCENODERESPONSE']._serialized_start=1724
-  _globals['_RPCANNOUNCENODERESPONSE']._serialized_end=1791
-  _globals['_RPCANNOUNCETEMPLATEREQUEST']._serialized_start=1793
-  _globals['_RPCANNOUNCETEMPLATEREQUEST']._serialized_end=1870
-  _globals['_RPCANNOUNCETEMPLATERESPONSE']._serialized_start=1872
-  _globals['_RPCANNOUNCETEMPLATERESPONSE']._serialized_end=1943
-  _globals['_RPCCREATEDISKREQUEST']._serialized_start=1946
-  _globals['_RPCCREATEDISKREQUEST']._serialized_end=2112
-  _globals['_RPCCREATEDISKRESPONSE']._serialized_start=2114
-  _globals['_RPCCREATEDISKRESPONSE']._serialized_end=2150
-  _globals['_RPCOPENDISKREQUEST']._serialized_start=2152
-  _globals['_RPCOPENDISKREQUEST']._serialized_end=2231
-  _globals['_RPCOPENDISKRESPONSE']._serialized_start=2233
-  _globals['_RPCOPENDISKRESPONSE']._serialized_end=2304
-  _globals['_RPCCLOSEDISKREQUEST']._serialized_start=2306
-  _globals['_RPCCLOSEDISKREQUEST']._serialized_end=2343
-  _globals['_RPCCLOSEDISKRESPONSE']._serialized_start=2345
-  _globals['_RPCCLOSEDISKRESPONSE']._serialized_end=2384
-  _globals['_RPCDISKDELETEFILEREQUEST']._serialized_start=2386
-  _globals['_RPCDISKDELETEFILEREQUEST']._serialized_end=2442
-  _globals['_RPCDISKDELETEFILERESPONSE']._serialized_start=2444
-  _globals['_RPCDISKDELETEFILERESPONSE']._serialized_end=2488
-  _globals['_RPCDISKLISTFILESREQUEST']._serialized_start=2490
-  _globals['_RPCDISKLISTFILESREQUEST']._serialized_end=2545
-  _globals['_RPCDISKLISTFILESRESPONSE']._serialized_start=2547
-  _globals['_RPCDISKLISTFILESRESPONSE']._serialized_end=2588
-  _globals['_RPCDISKREADFILEREQUEST']._serialized_start=2590
-  _globals['_RPCDISKREADFILEREQUEST']._serialized_end=2644
-  _globals['_RPCDISKREADFILERESPONSE']._serialized_start=2646
-  _globals['_RPCDISKREADFILERESPONSE']._serialized_end=2701
-  _globals['_RPCDISKWRITEFILEREQUEST']._serialized_start=2703
-  _globals['_RPCDISKWRITEFILEREQUEST']._serialized_end=2772
-  _globals['_RPCDISKWRITEFILERESPONSE']._serialized_start=2774
-  _globals['_RPCDISKWRITEFILERESPONSE']._serialized_end=2817
-  _globals['_RPCCACHESETREQUEST']._serialized_start=2819
-  _globals['_RPCCACHESETREQUEST']._serialized_end=2936
-  _globals['_RPCCACHESETRESPONSE']._serialized_start=2938
-  _globals['_RPCCACHESETRESPONSE']._serialized_end=2976
-  _globals['_RPCCACHEGETREQUEST']._serialized_start=2978
-  _globals['_RPCCACHEGETREQUEST']._serialized_end=3053
-  _globals['_RPCCACHEGETRESPONSE']._serialized_start=3055
-  _globals['_RPCCACHEGETRESPONSE']._serialized_end=3106
-  _globals['_RPCDISCOVERPOOLSREQUEST']._serialized_start=3108
-  _globals['_RPCDISCOVERPOOLSREQUEST']._serialized_end=3133
-  _globals['_RPCDISCOVERPOOLSRESPONSE']._serialized_start=3135
-  _globals['_RPCDISCOVERPOOLSRESPONSE']._serialized_end=3176
-  _globals['_RPCDISCOVERNODESREQUEST']._serialized_start=3178
-  _globals['_RPCDISCOVERNODESREQUEST']._serialized_end=3300
-  _globals['_RPCDISCOVERNODESRESPONSE']._serialized_start=3302
-  _globals['_RPCDISCOVERNODESRESPONSE']._serialized_end=3343
-  _globals['_RPCDISCOVERACTIONSREQUEST']._serialized_start=3346
-  _globals['_RPCDISCOVERACTIONSREQUEST']._serialized_end=3492
-  _globals['_RPCDISCOVERACTIONSRESPONSE']._serialized_start=3494
-  _globals['_RPCDISCOVERACTIONSRESPONSE']._serialized_end=3539
-  _globals['_RPCDISCOVERNEARBYNODESREQUEST']._serialized_start=3541
-  _globals['_RPCDISCOVERNEARBYNODESREQUEST']._serialized_end=3646
-  _globals['_RPCDISCOVERNEARBYNODESRESPONSE']._serialized_start=3648
-  _globals['_RPCDISCOVERNEARBYNODESRESPONSE']._serialized_end=3695
-  _globals['_RPCDISCOVERNEARBYACTIONSREQUEST']._serialized_start=3698
-  _globals['_RPCDISCOVERNEARBYACTIONSREQUEST']._serialized_end=3827
-  _globals['_RPCDISCOVERNEARBYACTIONSRESPONSE']._serialized_start=3829
-  _globals['_RPCDISCOVERNEARBYACTIONSRESPONSE']._serialized_end=3880
-  _globals['_RPCJOBREQUEST']._serialized_start=3882
-  _globals['_RPCJOBREQUEST']._serialized_end=3986
-  _globals['_POOLCONNECTOR']._serialized_start=3989
-  _globals['_POOLCONNECTOR']._serialized_end=5952
+  _globals['_RPCREQUESTJOB']._serialized_end=434
+  _globals['_RPCGETJOB']._serialized_start=436
+  _globals['_RPCGETJOB']._serialized_end=490
+  _globals['_RPCGETPENDINGJOBS']._serialized_start=493
+  _globals['_RPCGETPENDINGJOBS']._serialized_end=799
+  _globals['_PENDINGJOBS']._serialized_start=801
+  _globals['_PENDINGJOBS']._serialized_end=834
+  _globals['_RPCISJOBDONE']._serialized_start=836
+  _globals['_RPCISJOBDONE']._serialized_end=866
+  _globals['_RPCACCEPTJOB']._serialized_start=868
+  _globals['_RPCACCEPTJOB']._serialized_end=897
+  _globals['_RPCCANCELJOB']._serialized_start=899
+  _globals['_RPCCANCELJOB']._serialized_end=944
+  _globals['_RPCJOBOUTPUT']._serialized_start=946
+  _globals['_RPCJOBOUTPUT']._serialized_end=991
+  _globals['_RPCJOBCOMPLETE']._serialized_start=993
+  _globals['_RPCJOBCOMPLETE']._serialized_end=1068
+  _globals['_RPCJOBLOG']._serialized_start=1070
+  _globals['_RPCJOBLOG']._serialized_end=1109
+  _globals['_RPCSENDSIGNEDEVENTREQUEST']._serialized_start=1111
+  _globals['_RPCSENDSIGNEDEVENTREQUEST']._serialized_end=1170
+  _globals['_RPCSUBSCRIBETOEVENTSREQUEST']._serialized_start=1172
+  _globals['_RPCSUBSCRIBETOEVENTSREQUEST']._serialized_end=1235
+  _globals['_RPCSUBSCRIBETOEVENTSRESPONSE']._serialized_start=1237
+  _globals['_RPCSUBSCRIBETOEVENTSRESPONSE']._serialized_end=1308
+  _globals['_RPCGETEVENTSREQUEST']._serialized_start=1310
+  _globals['_RPCGETEVENTSREQUEST']._serialized_end=1387
+  _globals['_RPCGETEVENTSRESPONSE']._serialized_start=1389
+  _globals['_RPCGETEVENTSRESPONSE']._serialized_end=1483
+  _globals['_RPCSENDSIGNEDEVENTRESPONSE']._serialized_start=1485
+  _globals['_RPCSENDSIGNEDEVENTRESPONSE']._serialized_end=1547
+  _globals['_RPCUNSUBSCRIBEFROMEVENTSREQUEST']._serialized_start=1549
+  _globals['_RPCUNSUBSCRIBEFROMEVENTSREQUEST']._serialized_end=1623
+  _globals['_RPCUNSUBSCRIBEFROMEVENTSRESPONSE']._serialized_start=1625
+  _globals['_RPCUNSUBSCRIBEFROMEVENTSRESPONSE']._serialized_end=1676
+  _globals['_RPCANNOUNCENODEREQUEST']._serialized_start=1678
+  _globals['_RPCANNOUNCENODEREQUEST']._serialized_end=1754
+  _globals['_RPCANNOUNCENODERESPONSE']._serialized_start=1756
+  _globals['_RPCANNOUNCENODERESPONSE']._serialized_end=1823
+  _globals['_RPCANNOUNCETEMPLATEREQUEST']._serialized_start=1825
+  _globals['_RPCANNOUNCETEMPLATEREQUEST']._serialized_end=1902
+  _globals['_RPCANNOUNCETEMPLATERESPONSE']._serialized_start=1904
+  _globals['_RPCANNOUNCETEMPLATERESPONSE']._serialized_end=1975
+  _globals['_RPCCREATEDISKREQUEST']._serialized_start=1978
+  _globals['_RPCCREATEDISKREQUEST']._serialized_end=2144
+  _globals['_RPCCREATEDISKRESPONSE']._serialized_start=2146
+  _globals['_RPCCREATEDISKRESPONSE']._serialized_end=2182
+  _globals['_RPCOPENDISKREQUEST']._serialized_start=2184
+  _globals['_RPCOPENDISKREQUEST']._serialized_end=2263
+  _globals['_RPCOPENDISKRESPONSE']._serialized_start=2265
+  _globals['_RPCOPENDISKRESPONSE']._serialized_end=2336
+  _globals['_RPCCLOSEDISKREQUEST']._serialized_start=2338
+  _globals['_RPCCLOSEDISKREQUEST']._serialized_end=2375
+  _globals['_RPCCLOSEDISKRESPONSE']._serialized_start=2377
+  _globals['_RPCCLOSEDISKRESPONSE']._serialized_end=2416
+  _globals['_RPCDISKDELETEFILEREQUEST']._serialized_start=2418
+  _globals['_RPCDISKDELETEFILEREQUEST']._serialized_end=2474
+  _globals['_RPCDISKDELETEFILERESPONSE']._serialized_start=2476
+  _globals['_RPCDISKDELETEFILERESPONSE']._serialized_end=2520
+  _globals['_RPCDISKLISTFILESREQUEST']._serialized_start=2522
+  _globals['_RPCDISKLISTFILESREQUEST']._serialized_end=2577
+  _globals['_RPCDISKLISTFILESRESPONSE']._serialized_start=2579
+  _globals['_RPCDISKLISTFILESRESPONSE']._serialized_end=2620
+  _globals['_RPCDISKREADFILEREQUEST']._serialized_start=2622
+  _globals['_RPCDISKREADFILEREQUEST']._serialized_end=2676
+  _globals['_RPCDISKREADFILERESPONSE']._serialized_start=2678
+  _globals['_RPCDISKREADFILERESPONSE']._serialized_end=2733
+  _globals['_RPCDISKWRITEFILEREQUEST']._serialized_start=2735
+  _globals['_RPCDISKWRITEFILEREQUEST']._serialized_end=2804
+  _globals['_RPCDISKWRITEFILERESPONSE']._serialized_start=2806
+  _globals['_RPCDISKWRITEFILERESPONSE']._serialized_end=2849
+  _globals['_RPCCACHESETREQUEST']._serialized_start=2851
+  _globals['_RPCCACHESETREQUEST']._serialized_end=2968
+  _globals['_RPCCACHESETRESPONSE']._serialized_start=2970
+  _globals['_RPCCACHESETRESPONSE']._serialized_end=3008
+  _globals['_RPCCACHEGETREQUEST']._serialized_start=3010
+  _globals['_RPCCACHEGETREQUEST']._serialized_end=3085
+  _globals['_RPCCACHEGETRESPONSE']._serialized_start=3087
+  _globals['_RPCCACHEGETRESPONSE']._serialized_end=3138
+  _globals['_RPCDISCOVERPOOLSREQUEST']._serialized_start=3140
+  _globals['_RPCDISCOVERPOOLSREQUEST']._serialized_end=3165
+  _globals['_RPCDISCOVERPOOLSRESPONSE']._serialized_start=3167
+  _globals['_RPCDISCOVERPOOLSRESPONSE']._serialized_end=3208
+  _globals['_RPCDISCOVERNODESREQUEST']._serialized_start=3210
+  _globals['_RPCDISCOVERNODESREQUEST']._serialized_end=3332
+  _globals['_RPCDISCOVERNODESRESPONSE']._serialized_start=3334
+  _globals['_RPCDISCOVERNODESRESPONSE']._serialized_end=3375
+  _globals['_RPCDISCOVERACTIONSREQUEST']._serialized_start=3378
+  _globals['_RPCDISCOVERACTIONSREQUEST']._serialized_end=3524
+  _globals['_RPCDISCOVERACTIONSRESPONSE']._serialized_start=3526
+  _globals['_RPCDISCOVERACTIONSRESPONSE']._serialized_end=3571
+  _globals['_RPCDISCOVERNEARBYNODESREQUEST']._serialized_start=3573
+  _globals['_RPCDISCOVERNEARBYNODESREQUEST']._serialized_end=3678
+  _globals['_RPCDISCOVERNEARBYNODESRESPONSE']._serialized_start=3680
+  _globals['_RPCDISCOVERNEARBYNODESRESPONSE']._serialized_end=3727
+  _globals['_RPCDISCOVERNEARBYACTIONSREQUEST']._serialized_start=3730
+  _globals['_RPCDISCOVERNEARBYACTIONSREQUEST']._serialized_end=3859
+  _globals['_RPCDISCOVERNEARBYACTIONSRESPONSE']._serialized_start=3861
+  _globals['_RPCDISCOVERNEARBYACTIONSRESPONSE']._serialized_end=3912
+  _globals['_RPCJOBREQUEST']._serialized_start=3914
+  _globals['_RPCJOBREQUEST']._serialized_end=4018
+  _globals['_POOLCONNECTOR']._serialized_start=4021
+  _globals['_POOLCONNECTOR']._serialized_end=5984
 # @@protoc_insertion_point(module_scope)
```

### Comparing `openagents_grpc_proto-0.8.2/openagents_grpc_proto/rpc_pb2_grpc.py` & `openagents_grpc_proto-0.8.3/openagents_grpc_proto/rpc_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.8.2/openagents_grpc_proto.egg-info/SOURCES.txt` & `openagents_grpc_proto-0.8.3/openagents_grpc_proto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

