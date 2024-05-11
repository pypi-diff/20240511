# Comparing `tmp/sqooler-0.7.0.tar.gz` & `tmp/sqooler-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqooler-0.7.0.tar", max compression
+gzip compressed data, was "sqooler-0.7.1.tar", max compression
```

## Comparing `sqooler-0.7.0.tar` & `sqooler-0.7.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1211 2024-04-18 18:44:41.208787 sqooler-0.7.0/LICENSE
--rw-r--r--   0        0        0     3928 2024-04-18 18:44:41.212121 sqooler-0.7.0/README.md
--rw-r--r--   0        0        0     1282 2024-05-09 11:09:37.943063 sqooler-0.7.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-18 18:44:41.212209 sqooler-0.7.0/src/sqooler/__init__.py
--rw-r--r--   0        0        0      810 2024-05-05 09:53:38.382220 sqooler-0.7.0/src/sqooler/cli.py
--rw-r--r--   0        0        0    12206 2024-05-09 11:09:37.944438 sqooler-0.7.0/src/sqooler/schemes.py
--rw-r--r--   0        0        0     8775 2024-04-18 18:44:42.470722 sqooler-0.7.0/src/sqooler/security.py
--rw-r--r--   0        0        0    27991 2024-04-19 14:40:24.524812 sqooler-0.7.0/src/sqooler/spoolers.py
--rw-r--r--   0        0        0        0 2024-04-18 18:44:42.471937 sqooler-0.7.0/src/sqooler/storage_providers/__init__.py
--rw-r--r--   0        0        0    30402 2024-05-09 11:09:37.945823 sqooler-0.7.0/src/sqooler/storage_providers/base.py
--rw-r--r--   0        0        0    30431 2024-05-09 11:09:37.946668 sqooler-0.7.0/src/sqooler/storage_providers/dropbox.py
--rw-r--r--   0        0        0    25852 2024-05-04 06:42:01.258236 sqooler-0.7.0/src/sqooler/storage_providers/local.py
--rw-r--r--   0        0        0    31201 2024-05-04 06:41:56.453899 sqooler-0.7.0/src/sqooler/storage_providers/mongodb.py
--rw-r--r--   0        0        0     6672 2024-05-03 19:00:26.771893 sqooler-0.7.0/src/sqooler/utils.py
--rw-r--r--   0        0        0     4965 1970-01-01 00:00:00.000000 sqooler-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-18 18:44:41.208787 sqooler-0.7.1/LICENSE
+-rw-r--r--   0        0        0     3928 2024-04-18 18:44:41.212121 sqooler-0.7.1/README.md
+-rw-r--r--   0        0        0     1282 2024-05-11 21:00:58.760099 sqooler-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-18 18:44:41.212209 sqooler-0.7.1/src/sqooler/__init__.py
+-rw-r--r--   0        0        0      810 2024-05-05 09:53:38.382220 sqooler-0.7.1/src/sqooler/cli.py
+-rw-r--r--   0        0        0    14269 2024-05-09 13:07:12.492631 sqooler-0.7.1/src/sqooler/schemes.py
+-rw-r--r--   0        0        0     8775 2024-04-18 18:44:42.470722 sqooler-0.7.1/src/sqooler/security.py
+-rw-r--r--   0        0        0    27991 2024-04-19 14:40:24.524812 sqooler-0.7.1/src/sqooler/spoolers.py
+-rw-r--r--   0        0        0        0 2024-04-18 18:44:42.471937 sqooler-0.7.1/src/sqooler/storage_providers/__init__.py
+-rw-r--r--   0        0        0    30364 2024-05-11 20:32:01.563176 sqooler-0.7.1/src/sqooler/storage_providers/base.py
+-rw-r--r--   0        0        0    30924 2024-05-11 21:01:09.976853 sqooler-0.7.1/src/sqooler/storage_providers/dropbox.py
+-rw-r--r--   0        0        0    26238 2024-05-11 21:01:09.979534 sqooler-0.7.1/src/sqooler/storage_providers/local.py
+-rw-r--r--   0        0        0    31587 2024-05-11 21:01:09.979964 sqooler-0.7.1/src/sqooler/storage_providers/mongodb.py
+-rw-r--r--   0        0        0     6672 2024-05-11 20:06:14.172608 sqooler-0.7.1/src/sqooler/utils.py
+-rw-r--r--   0        0        0     4965 1970-01-01 00:00:00.000000 sqooler-0.7.1/PKG-INFO
```

### Comparing `sqooler-0.7.0/LICENSE` & `sqooler-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqooler-0.7.0/README.md` & `sqooler-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `sqooler-0.7.0/pyproject.toml` & `sqooler-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqooler"
-version = "0.7.0"
+version = "0.7.1"
 description = "Code that enables validated cloud access to quantum hardware (simulators)"
 authors = ["fretchen <fred.jendrzejewski@gmail.com>"]
 repository = "https://github.com/Alqor-UG/sqooler"
 documentation = "https://alqor-ug.github.io/sqooler"
 license = "Unlicense"
 readme = "README.md"
 packages = [{include = "sqooler", from = "src"}]
```

### Comparing `sqooler-0.7.0/src/sqooler/cli.py` & `sqooler-0.7.1/src/sqooler/cli.py`

 * *Files identical despite different names*

### Comparing `sqooler-0.7.0/src/sqooler/schemes.py` & `sqooler-0.7.1/src/sqooler/schemes.py`

 * *Files 9% similar despite different names*

```diff
@@ -156,14 +156,66 @@
         default=False,
         description="True if the results are signed by the backend provider.",
     )
     kid: Optional[str] = Field(
         default=None,
         description="The identifier for the public and private key of the backend.",
     )
+    operational: Optional[bool] = Field(
+        default=True, description="True if the backend is operational", deprecated=True
+    )
+
+
+class BackendConfigSchemaOld(BaseModel, validate_assignment=True):
+    """
+    The schema send in to detail the configuration of the backend.
+    This is uploaded to the storage provider.
+    """
+
+    description: str = Field(description="A description for the backend")
+    version: str = Field(description="The backend version in the form X.Y.Z")
+    display_name: Optional[DisplayNameStr]
+    cold_atom_type: ColdAtomStr
+    gates: list = Field(
+        description="The list of GateConfig objects for the basis gates of the backend"
+    )
+    max_experiments: int = Field(
+        description="The maximum number of experiments per job"
+    )
+    max_shots: int = Field(
+        description="The maximum number of shots allowed on the backend"
+    )
+    simulator: bool = Field(description="True if the backend is a simulator")
+    supported_instructions: list[str] = Field(
+        description="Instructions supported by the backend."
+    )
+    num_wires: int = Field(description="The number of qubits / wires for the backend")
+    wire_order: WireOrderStr
+    num_species: int = Field(description="The number of species in the system.")
+
+    pending_jobs: Optional[int] = Field(
+        default=None, description="The number of pending jobs on the backend"
+    )
+    status_msg: Optional[str] = Field(
+        default=None, description="The status message for the backend"
+    )
+    last_queue_check: Optional[datetime] = Field(
+        default=None, description="The last time the queue was checked."
+    )
+    sign: bool = Field(
+        default=False,
+        description="True if the results are signed by the backend provider.",
+    )
+    kid: Optional[str] = Field(
+        default=None,
+        description="The identifier for the public and private key of the backend.",
+    )
+    operational: Optional[bool] = Field(
+        default=True, description="True if the backend is operational", deprecated=True
+    )
 
 
 class BackendConfigSchemaOut(BaseModel, validate_assignment=True):
     """
     The schema send out to detail the configuration of the backend. We follow the
     conventions of the qiskit configuration dictionary here.
```

### Comparing `sqooler-0.7.0/src/sqooler/security.py` & `sqooler-0.7.1/src/sqooler/security.py`

 * *Files identical despite different names*

### Comparing `sqooler-0.7.0/src/sqooler/spoolers.py` & `sqooler-0.7.1/src/sqooler/spoolers.py`

 * *Files identical despite different names*

### Comparing `sqooler-0.7.0/src/sqooler/storage_providers/base.py` & `sqooler-0.7.1/src/sqooler/storage_providers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -583,20 +583,15 @@
         status_json_name: Optional[str] = None,
     ) -> None:
         """
         Allows us to upload the appropiate status dict to the storage provider.
         """
         # get the backend config
         config_dict = self.get_config(display_name)
-        if config_dict.sign:
-            # get the private key
-            if private_jwk is None:
-                raise ValueError(
-                    "The private key is not given, but the backend needs to be signed."
-                )
+        if config_dict.sign and private_jwk:
             # we sign the result now
             signed_status = sign_payload(status_dict.model_dump(), private_jwk)
             upload_dict = signed_status.model_dump()
         else:
             upload_dict = status_dict.model_dump()
 
         # now upload the status dict
@@ -642,19 +637,15 @@
                 )
             if set(old_config_jws.keys()) == expected_keys_for_jws:
                 # the old config is signed and we need to check if the private key is the same
                 payload = old_config_jws["payload"]
 
                 # now proof that the new private key would create the same signature for the old
                 # config to validate that we still have the same private key
-
-                # the following transformation is necessary to make avoid slight differences
-                # in the serialization and then the signing
-                old_config_dict = BackendConfigSchemaIn(**payload)
-                test_signature = sign_payload(old_config_dict.model_dump(), private_jwk)
+                test_signature = sign_payload(payload, private_jwk)
                 if not test_signature.signature == old_config_jws["signature"]:
                     raise ValueError(
                         "The new private key does not create the same signature as the old one."
                     )
 
             # now that we know that the private key is the same, we can sign the new config
             config_dict.kid = private_jwk.kid
@@ -740,18 +731,25 @@
         Args:
             display_name : The name of the backend
             private_jwk: The private JWK to sign the result with
 
         Returns:
             None
         """
-
         # first let us get the current configuration
-        config_dict = self.get_config(display_name)
-
+        try:
+            config_dict = self.get_config(display_name)
+        except FileNotFoundError as exc:
+            # if the config does not exist, we raise the informed error
+            logging.error(
+                "The configuration for the backend %s does not exist.", display_name
+            )
+            raise FileNotFoundError(
+                f"The configuration for the backend {display_name} does not exist."
+            ) from exc
         # get the current time
         current_time = datetime.now(timezone.utc).replace(microsecond=0)
 
         # update the time stamp
         config_dict.last_queue_check = current_time
 
         # upload the new configuration
```

### Comparing `sqooler-0.7.0/src/sqooler/storage_providers/dropbox.py` & `sqooler-0.7.1/src/sqooler/storage_providers/dropbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 The module that contains all the necessary logic for communication with the Dropbox providers.
 """
 
 # necessary for the dropbox provider
 import datetime
 import json
+import logging
 import sys
 import uuid
 from datetime import timezone
 from typing import Mapping, Optional
 
 import dropbox
 from dropbox.exceptions import ApiError, AuthError
@@ -72,14 +73,15 @@
         ) as dbx:
             # Check that the access token is valid
             dbx.users_get_current_account()
             dbx.files_upload(
                 content_string.encode("utf-8"), full_path, mode=WriteMode("overwrite")
             )
 
+    @validate_active
     def upload(self, content_dict: Mapping, storage_path: str, job_id: str) -> None:
         """
         Upload the content_dict as a json file to the dropbox
 
         Args:
             content_dict: the content of the file that should be uploaded
             storage_path: the path where the file should be stored, but excluding the file name
@@ -87,14 +89,15 @@
         """
 
         # create the appropriate string for the dropbox API
         dump_str = json.dumps(content_dict, default=datetime_handler)
 
         self.upload_string(dump_str, storage_path, job_id)
 
+    @validate_active
     def get_file_content(self, storage_path: str, job_id: str) -> dict:
         """
         Get the file content from the dropbox
 
         storage_path: the path where the file should be stored, but excluding the file name
         job_id: the name of the file. Is a json file
         """
@@ -441,16 +444,28 @@
             self.move_file(job_json_start_dir, job_finished_json_dir, job_json_name)
 
         elif status_msg_dict.status == "ERROR":
             # because there was an error, we move the job to the deleted jobs
             deleted_json_dir = "Backend_files/Deleted_Jobs"
             self.move_file(job_json_start_dir, deleted_json_dir, job_json_name)
 
-        # and create the status json file
-        self.upload(status_msg_dict.model_dump(), status_json_dir, status_json_name)
+        try:
+            self.update_file(
+                status_msg_dict.model_dump(), status_json_dir, status_json_name
+            )
+        except FileNotFoundError:
+            logging.warning(
+                "The status file was missing for %s with job_id %s was missing.",
+                display_name,
+                job_id,
+            )
+            self.upload_status(display_name, username=extracted_username, job_id=job_id)
+            self.update_file(
+                status_msg_dict.model_dump(), status_json_dir, status_json_name
+            )
 
     def get_file_queue(self, storage_path: str) -> list[str]:
         """
         Get a list of files. Typically we are looking for the queued jobs of a backend here.
 
         Args:
             storage_path: Where are we looking for the files.
```

### Comparing `sqooler-0.7.0/src/sqooler/storage_providers/local.py` & `sqooler-0.7.1/src/sqooler/storage_providers/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 The module that contains all the necessary logic for communication with the local storage providers.
 """
 
 import json
+import logging
 import os
 
 # necessary for the local provider
 import shutil
 import uuid
 from typing import Mapping, Optional
 
@@ -682,15 +683,24 @@
         elif status_msg_dict.status == "ERROR":
             # because there was an error, we move the job to the deleted jobs
             deleted_json_dir = "jobs/deleted"
             self.move_file(job_json_start_dir, deleted_json_dir, job_id)
 
         # and create the status json file
         status_json_dir = "status/" + display_name
-        self.update_file(status_msg_dict.model_dump(), status_json_dir, job_id)
+        try:
+            self.update_file(status_msg_dict.model_dump(), status_json_dir, job_id)
+        except FileNotFoundError:
+            logging.warning(
+                "The status file was missing for %s with job_id %s was missing.",
+                display_name,
+                job_id,
+            )
+            self.upload_status(display_name, "", job_id)
+            self.update_file(status_msg_dict.model_dump(), status_json_dir, job_id)
 
     def get_file_queue(self, storage_path: str) -> list[str]:
         """
         Get a list of files
 
         Args:
             storage_path: Where are we looking for the files.
```

### Comparing `sqooler-0.7.0/src/sqooler/storage_providers/mongodb.py` & `sqooler-0.7.1/src/sqooler/storage_providers/mongodb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 The module that contains all the necessary logic for communication with the MongoDb storage providers.
 """
 
+import logging
 import uuid
 from datetime import timezone
 from typing import Optional
 
 from bson.codec_options import CodecOptions
 from bson.errors import InvalidId
 from bson.objectid import ObjectId
@@ -802,15 +803,24 @@
             deleted_json_dir = "jobs/deleted"
             self.move_file(job_json_start_dir, deleted_json_dir, job_id)
 
         # TODO: most likely we should raise an error if the status of the job is not DONE or ERROR
 
         # and create the status json file
         status_json_dir = "status/" + display_name
-        self.update_file(status_msg_dict.model_dump(), status_json_dir, job_id)
+        try:
+            self.update_file(status_msg_dict.model_dump(), status_json_dir, job_id)
+        except FileNotFoundError:
+            logging.warning(
+                "The status file was missing for %s with job_id %s was missing.",
+                display_name,
+                job_id,
+            )
+            self.upload_status(display_name, "", job_id)
+            self.update_file(status_msg_dict.model_dump(), status_json_dir, job_id)
 
     def get_file_queue(self, storage_path: str) -> list[str]:
         """
         Get a list of documents in the collection of all the queued jobs.
 
         Args:
             storage_path: Where are we looking for the files.
```

### Comparing `sqooler-0.7.0/src/sqooler/utils.py` & `sqooler-0.7.1/src/sqooler/utils.py`

 * *Files identical despite different names*

### Comparing `sqooler-0.7.0/PKG-INFO` & `sqooler-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqooler
-Version: 0.7.0
+Version: 0.7.1
 Summary: Code that enables validated cloud access to quantum hardware (simulators)
 Home-page: https://github.com/Alqor-UG/sqooler
 License: Unlicense
 Keywords: pydantic,quantum-hardware,sdk-python
 Author: fretchen
 Author-email: fred.jendrzejewski@gmail.com
 Requires-Python: >=3.10,<4.0
```

