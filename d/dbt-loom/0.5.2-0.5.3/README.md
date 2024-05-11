# Comparing `tmp/dbt_loom-0.5.2.tar.gz` & `tmp/dbt_loom-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_loom-0.5.2.tar", max compression
+gzip compressed data, was "dbt_loom-0.5.3.tar", max compression
```

## Comparing `dbt_loom-0.5.2.tar` & `dbt_loom-0.5.3.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1211 2024-05-06 19:53:58.008566 dbt_loom-0.5.2/LICENSE
--rw-r--r--   0        0        0     6654 2024-05-06 19:53:58.008566 dbt_loom-0.5.2/README.md
--rw-r--r--   0        0        0     5823 2024-05-06 19:53:58.008566 dbt_loom-0.5.2/dbt_loom/__init__.py
--rw-r--r--   0        0        0     2088 2024-05-06 19:53:58.008566 dbt_loom-0.5.2/dbt_loom/clients/az_blob.py
--rw-r--r--   0        0        0     2675 2024-05-06 19:53:58.008566 dbt_loom-0.5.2/dbt_loom/clients/dbt_cloud.py
--rw-r--r--   0        0        0     1603 2024-05-06 19:53:58.008566 dbt_loom-0.5.2/dbt_loom/clients/gcs.py
--rw-r--r--   0        0        0     1641 2024-05-06 19:53:58.008566 dbt_loom-0.5.2/dbt_loom/clients/s3.py
--rw-r--r--   0        0        0     1161 2024-05-06 19:53:58.008566 dbt_loom-0.5.2/dbt_loom/config.py
--rw-r--r--   0        0        0     4550 2024-05-06 19:53:58.008566 dbt_loom-0.5.2/dbt_loom/manifests.py
--rw-r--r--   0        0        0     1059 2024-05-06 19:53:58.012566 dbt_loom-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     7505 1970-01-01 00:00:00.000000 dbt_loom-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-05-11 01:00:32.151226 dbt_loom-0.5.3/LICENSE
+-rw-r--r--   0        0        0     6654 2024-05-11 01:00:32.151226 dbt_loom-0.5.3/README.md
+-rw-r--r--   0        0        0     6762 2024-05-11 01:00:32.151226 dbt_loom-0.5.3/dbt_loom/__init__.py
+-rw-r--r--   0        0        0     2088 2024-05-11 01:00:32.151226 dbt_loom-0.5.3/dbt_loom/clients/az_blob.py
+-rw-r--r--   0        0        0     2632 2024-05-11 01:00:32.151226 dbt_loom-0.5.3/dbt_loom/clients/dbt_cloud.py
+-rw-r--r--   0        0        0     1603 2024-05-11 01:00:32.151226 dbt_loom-0.5.3/dbt_loom/clients/gcs.py
+-rw-r--r--   0        0        0     1641 2024-05-11 01:00:32.151226 dbt_loom-0.5.3/dbt_loom/clients/s3.py
+-rw-r--r--   0        0        0     1161 2024-05-11 01:00:32.151226 dbt_loom-0.5.3/dbt_loom/config.py
+-rw-r--r--   0        0        0      396 2024-05-11 01:00:32.151226 dbt_loom-0.5.3/dbt_loom/logging.py
+-rw-r--r--   0        0        0     4716 2024-05-11 01:00:32.151226 dbt_loom-0.5.3/dbt_loom/manifests.py
+-rw-r--r--   0        0        0     1061 2024-05-11 01:00:32.151226 dbt_loom-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     7506 1970-01-01 00:00:00.000000 dbt_loom-0.5.3/PKG-INFO
```

### Comparing `dbt_loom-0.5.2/LICENSE` & `dbt_loom-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_loom-0.5.2/README.md` & `dbt_loom-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `dbt_loom-0.5.2/dbt_loom/__init__.py` & `dbt_loom-0.5.3/dbt_loom/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,58 @@
+from dataclasses import dataclass
 import os
 import re
 from pathlib import Path
 from typing import Callable, Dict, Optional
 
 import yaml
 from dbt.contracts.graph.node_args import ModelNodeArgs
-from dbt.events.functions import fire_event
-from dbt.events.types import Note
+
+
 from dbt.plugins.manager import dbt_hook, dbtPlugin
 from dbt.plugins.manifest import PluginNodes
 from dbt.config.project import VarProvider
-from dbt.node_types import NodeType
+
+try:
+    from dbt.artifacts.resources.types import NodeType
+except ModuleNotFoundError:
+    from dbt.node_types import NodeType  # type: ignore
+
 
 from dbt_loom.config import dbtLoomConfig
+from dbt_loom.logging import fire_event
 from dbt_loom.manifests import ManifestLoader, ManifestNode
 
+import importlib.metadata
+
+
+@dataclass
+class LoomModelNodeArgs(ModelNodeArgs):
+    """A dbt-loom extension of ModelNodeArgs to preserve resource types across lineages."""
+
+    resource_type: NodeType = NodeType.Model
+
+    def __init__(self, **kwargs):
+        super().__init__(
+            **{
+                key: value
+                for key, value in kwargs.items()
+                if key not in ("resource_type")
+            }
+        )
+        self.resource_type = kwargs["resource_type"]
+
+    @property
+    def unique_id(self) -> str:
+        unique_id = f"{self.resource_type}.{self.package_name}.{self.name}"
+        if self.version:
+            unique_id = f"{unique_id}.v{self.version}"
+
+        return unique_id
+
 
 def identify_node_subgraph(manifest) -> Dict[str, ManifestNode]:
     """
     Identify all nodes that should be selected from the manifest, and return ManifestNodes.
     """
 
     output = {}
@@ -44,18 +78,18 @@
         output[unique_id] = ManifestNode(**(node))
 
     return output
 
 
 def convert_model_nodes_to_model_node_args(
     selected_nodes: Dict[str, ManifestNode],
-) -> Dict[str, ModelNodeArgs]:
+) -> Dict[str, LoomModelNodeArgs]:
     """Generate a dictionary of ModelNodeArgs based on a dictionary of ModelNodes"""
     return {
-        unique_id: ModelNodeArgs(
+        unique_id: LoomModelNodeArgs(
             schema=node.schema_name,
             identifier=node.identifier,
             **(
                 # Small bit of logic to support both pydantic 2 and pydantic 1
                 node.model_dump(exclude={"schema_name", "depends_on", "node_config"})
                 if hasattr(node, "model_dump")
                 else node.dict(exclude={"schema_name", "depends_on", "node_config"})
@@ -76,29 +110,32 @@
 class dbtLoom(dbtPlugin):
     """
     dbtLoom is a dbt plugin that loads manifest files, parses a DAG from the manifest,
     and injects public nodes from imported manifest.
     """
 
     def __init__(self, project_name: str):
+        # Log the version of dbt-loom being intialized
+        fire_event(
+            msg=f'Initializing dbt-loom={importlib.metadata.version("dbt-loom")}'
+        )
+
         configuration_path = Path(
             os.environ.get("DBT_LOOM_CONFIG", "dbt_loom.config.yml")
         )
 
         self._manifest_loader = ManifestLoader()
 
         self.config: Optional[dbtLoomConfig] = self.read_config(configuration_path)
-        self.models: Dict[str, ModelNodeArgs] = {}
+        self.models: Dict[str, LoomModelNodeArgs] = {}
 
         import dbt.contracts.graph.manifest
 
         fire_event(
-            Note(
-                msg="dbt-loom: Patching ref protection methods to support dbt-loom dependencies."
-            )
+            msg="dbt-loom: Patching ref protection methods to support dbt-loom dependencies."
         )
         dbt.contracts.graph.manifest.Manifest.is_invalid_protected_ref = (  # type: ignore
             self.dependency_wrapper(
                 dbt.contracts.graph.manifest.Manifest.is_invalid_protected_ref
             )
         )
         dbt.contracts.graph.manifest.Manifest.is_invalid_private_ref = (  # type: ignore
@@ -147,30 +184,28 @@
         """Initialize the plugin"""
 
         if self.models != {} or not self.config:
             return
 
         for manifest_reference in self.config.manifests:
             fire_event(
-                Note(
-                    msg=f"dbt-loom: Loading manifest for `{manifest_reference.name}`"
-                    f" from `{manifest_reference.type.value}`"
-                )
+                msg=f"dbt-loom: Loading manifest for `{manifest_reference.name}`"
+                f" from `{manifest_reference.type.value}`"
             )
 
             manifest = self._manifest_loader.load(manifest_reference)
             if manifest is None:
                 continue
 
             selected_nodes = identify_node_subgraph(manifest)
             self.models.update(convert_model_nodes_to_model_node_args(selected_nodes))
 
     @dbt_hook
     def get_nodes(self) -> PluginNodes:
         """
         Inject PluginNodes to dbt for injection into dbt's DAG.
         """
-        fire_event(Note(msg="dbt-loom: Injecting nodes"))
-        return PluginNodes(models=self.models)
+        fire_event(msg="dbt-loom: Injecting nodes")
+        return PluginNodes(models=self.models)  # type: ignore
 
 
 plugins = [dbtLoom]
```

### Comparing `dbt_loom-0.5.2/dbt_loom/clients/az_blob.py` & `dbt_loom-0.5.3/dbt_loom/clients/az_blob.py`

 * *Files identical despite different names*

### Comparing `dbt_loom-0.5.2/dbt_loom/clients/dbt_cloud.py` & `dbt_loom-0.5.3/dbt_loom/clients/dbt_cloud.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from typing import Any, Dict, Optional
 
 from pydantic import BaseModel
 import requests
-from dbt.events.functions import fire_event
-from dbt.events.types import Note
+
+from dbt_loom.logging import fire_event
 
 
 class DbtCloudReferenceConfig(BaseModel):
     """Configuration for a dbt Cloud reference."""
 
     account_id: int
     job_id: int
@@ -37,15 +37,15 @@
 
         self.account_id = account_id
         self.api_endpoint = api_endpoint or "https://cloud.getdbt.com/api/v2"
 
     def _query(self, endpoint: str, **kwargs) -> Dict:
         """Query the dbt Cloud Administrative API."""
         url = f"{self.api_endpoint}/{endpoint}"
-        fire_event(Note(msg=f"Querying {url}"))
+        fire_event(msg=f"Querying {url}")
         response = requests.get(
             url,
             headers={
                 "authorization": "Bearer " + self.__token,
                 "content-type": "application/json",
             },
             **kwargs,
```

### Comparing `dbt_loom-0.5.2/dbt_loom/clients/gcs.py` & `dbt_loom-0.5.3/dbt_loom/clients/gcs.py`

 * *Files identical despite different names*

### Comparing `dbt_loom-0.5.2/dbt_loom/clients/s3.py` & `dbt_loom-0.5.3/dbt_loom/clients/s3.py`

 * *Files identical despite different names*

### Comparing `dbt_loom-0.5.2/dbt_loom/config.py` & `dbt_loom-0.5.3/dbt_loom/config.py`

 * *Files identical despite different names*

### Comparing `dbt_loom-0.5.2/dbt_loom/manifests.py` & `dbt_loom-0.5.3/dbt_loom/manifests.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import datetime
 import json
-from typing import Dict, List, Optional, Union
+from typing import Dict, List, Optional
 
 from pydantic import BaseModel, Field, validator
 
+try:
+    from dbt.artifacts.resources.types import NodeType
+except ModuleNotFoundError:
+    from dbt.node_types import NodeType  # type: ignore
+
 from dbt_loom.clients.az_blob import AzureClient, AzureReferenceConfig
 from dbt_loom.clients.dbt_cloud import DbtCloud, DbtCloudReferenceConfig
 from dbt_loom.clients.gcs import GCSClient, GCSReferenceConfig
 from dbt_loom.clients.s3 import S3Client, S3ReferenceConfig
 from dbt_loom.config import (
     FileReferenceConfig,
     LoomConfigurationError,
@@ -23,14 +28,15 @@
     macros: List[str] = Field(default_factory=list)
 
 
 class ManifestNode(BaseModel):
     """A basic ManifestNode that can be referenced across projects."""
 
     name: str
+    resource_type: NodeType
     package_name: str
     schema_name: str = Field(alias="schema")
     database: Optional[str] = None
     relation_name: Optional[str] = None
     version: Optional[str] = None
     latest_version: Optional[str] = None
     deprecation_date: Optional[datetime.datetime] = None
```

### Comparing `dbt_loom-0.5.2/pyproject.toml` & `dbt_loom-0.5.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 [tool.poetry]
 name = "dbt-loom"
-version = "0.5.2"
+version = "0.5.3"
 description = "A dbt-core plugin to import public nodes in multi-project deployments."
 authors = ["Nicholas Yager <yager@nicholasyager.com>"]
 readme = "README.md"
 packages = [{ include = "dbt_loom" }]
 
 [tool.commitizen]
-version = "0.5.2"
+version = "0.5.3"
 version_files = ["pyproject.toml:^version"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
-dbt-core = ">=1.6.0,<1.8.0"
+dbt-core = ">=1.6.0,<=1.8.0"
 requests = "^2.31.0"
 google-cloud-storage = "^2.13.0"
 boto3 = "^1.28.84"
 azure-storage-blob = "^12.19.0"
 azure-identity = "^1.15.0"
 types-pyyaml = "^6.0.12.12"
 types-networkx = "^3.2.1.20240313"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.3.0"
 pytest = "^7.4.0"
 isort = "^5.12.0"
-dbt-duckdb = ">=1.6.0,<1.8.0"
+dbt-duckdb = ">=1.6.0,<=1.8.0"
 duckdb = ">=0.8.0"
 pre-commit = "^3.6.0"
 mypy = "^1.8.0"
 
 [tool.ruff]
 line-length = 88
```

### Comparing `dbt_loom-0.5.2/PKG-INFO` & `dbt_loom-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: dbt-loom
-Version: 0.5.2
+Version: 0.5.3
 Summary: A dbt-core plugin to import public nodes in multi-project deployments.
 Author: Nicholas Yager
 Author-email: yager@nicholasyager.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: azure-identity (>=1.15.0,<2.0.0)
 Requires-Dist: azure-storage-blob (>=12.19.0,<13.0.0)
 Requires-Dist: boto3 (>=1.28.84,<2.0.0)
-Requires-Dist: dbt-core (>=1.6.0,<1.8.0)
+Requires-Dist: dbt-core (>=1.6.0,<=1.8.0)
 Requires-Dist: google-cloud-storage (>=2.13.0,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: types-networkx (>=3.2.1.20240313,<4.0.0.0)
 Requires-Dist: types-pyyaml (>=6.0.12.12,<7.0.0.0)
 Description-Content-Type: text/markdown
 
 # dbt-loom
```

