# Comparing `tmp/ediri_azapi-1.8.1.tar.gz` & `tmp/ediri_azapi-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ediri_azapi-1.8.1.tar", last modified: Mon Aug 14 15:37:04 2023, max compression
+gzip compressed data, was "ediri_azapi-1.9.0.tar", last modified: Mon Sep 18 07:52:51 2023, max compression
```

## Comparing `ediri_azapi-1.8.1.tar` & `ediri_azapi-1.9.0.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 15:37:04.033919 ediri_azapi-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-08-14 15:37:04.033919 ediri_azapi-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-08-14 15:37:03.000000 ediri_azapi-1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 15:37:04.029919 ediri_azapi-1.8.1/ediri_azapi/
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-08-14 15:37:03.000000 ediri_azapi-1.8.1/ediri_azapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-08-14 15:37:03.000000 ediri_azapi-1.8.1/ediri_azapi/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-08-14 15:37:03.000000 ediri_azapi-1.8.1/ediri_azapi/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 15:37:04.033919 ediri_azapi-1.8.1/ediri_azapi/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-14 15:37:03.000000 ediri_azapi-1.8.1/ediri_azapi/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-08-14 15:37:03.000000 ediri_azapi-1.8.1/ediri_azapi/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    51844 2023-08-14 15:37:03.000000 ediri_azapi-1.8.1/ediri_azapi/data_plane_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-08-14 15:37:03.000000 ediri_azapi-1.8.1/ediri_azapi/get_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-08-14 15:37:03.000000 ediri_azapi-1.8.1/ediri_azapi/get_resource_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-08-14 15:37:03.000000 ediri_azapi-1.8.1/ediri_azapi/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35332 2023-08-14 15:37:03.000000 ediri_azapi-1.8.1/ediri_azapi/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-14 15:37:03.000000 ediri_azapi-1.8.1/ediri_azapi/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-14 15:37:03.000000 ediri_azapi-1.8.1/ediri_azapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    48794 2023-08-14 15:37:03.000000 ediri_azapi-1.8.1/ediri_azapi/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    26763 2023-08-14 15:37:03.000000 ediri_azapi-1.8.1/ediri_azapi/resource_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    39567 2023-08-14 15:37:03.000000 ediri_azapi-1.8.1/ediri_azapi/update_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 15:37:04.033919 ediri_azapi-1.8.1/ediri_azapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-08-14 15:37:04.000000 ediri_azapi-1.8.1/ediri_azapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-14 15:37:04.000000 ediri_azapi-1.8.1/ediri_azapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-14 15:37:04.000000 ediri_azapi-1.8.1/ediri_azapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-14 15:37:04.000000 ediri_azapi-1.8.1/ediri_azapi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-14 15:37:04.000000 ediri_azapi-1.8.1/ediri_azapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-14 15:37:04.000000 ediri_azapi-1.8.1/ediri_azapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-14 15:37:04.033919 ediri_azapi-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-08-14 15:37:03.000000 ediri_azapi-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 07:52:51.273319 ediri_azapi-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2023-09-18 07:52:51.269319 ediri_azapi-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2023-09-18 07:52:50.000000 ediri_azapi-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 07:52:51.269319 ediri_azapi-1.9.0/ediri_azapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2023-09-18 07:52:50.000000 ediri_azapi-1.9.0/ediri_azapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6273 2023-09-18 07:52:50.000000 ediri_azapi-1.9.0/ediri_azapi/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8122 2023-09-18 07:52:50.000000 ediri_azapi-1.9.0/ediri_azapi/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 07:52:51.269319 ediri_azapi-1.9.0/ediri_azapi/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2023-09-18 07:52:50.000000 ediri_azapi-1.9.0/ediri_azapi/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5700 2023-09-18 07:52:50.000000 ediri_azapi-1.9.0/ediri_azapi/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51844 2023-09-18 07:52:50.000000 ediri_azapi-1.9.0/ediri_azapi/data_plane_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12743 2023-09-18 07:52:50.000000 ediri_azapi-1.9.0/ediri_azapi/get_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9870 2023-09-18 07:52:50.000000 ediri_azapi-1.9.0/ediri_azapi/get_resource_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9590 2023-09-18 07:52:50.000000 ediri_azapi-1.9.0/ediri_azapi/get_resource_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6651 2023-09-18 07:52:50.000000 ediri_azapi-1.9.0/ediri_azapi/get_resource_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5815 2023-09-18 07:52:50.000000 ediri_azapi-1.9.0/ediri_azapi/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35332 2023-09-18 07:52:50.000000 ediri_azapi-1.9.0/ediri_azapi/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2023-09-18 07:52:50.000000 ediri_azapi-1.9.0/ediri_azapi/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-18 07:52:50.000000 ediri_azapi-1.9.0/ediri_azapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    53520 2023-09-18 07:52:50.000000 ediri_azapi-1.9.0/ediri_azapi/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26763 2023-09-18 07:52:50.000000 ediri_azapi-1.9.0/ediri_azapi/resource_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42476 2023-09-18 07:52:50.000000 ediri_azapi-1.9.0/ediri_azapi/update_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 07:52:51.269319 ediri_azapi-1.9.0/ediri_azapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2023-09-18 07:52:51.000000 ediri_azapi-1.9.0/ediri_azapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2023-09-18 07:52:51.000000 ediri_azapi-1.9.0/ediri_azapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-18 07:52:51.000000 ediri_azapi-1.9.0/ediri_azapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-18 07:52:51.000000 ediri_azapi-1.9.0/ediri_azapi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2023-09-18 07:52:51.000000 ediri_azapi-1.9.0/ediri_azapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-09-18 07:52:51.000000 ediri_azapi-1.9.0/ediri_azapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-18 07:52:51.273319 ediri_azapi-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2023-09-18 07:52:50.000000 ediri_azapi-1.9.0/setup.py
```

### Comparing `ediri_azapi-1.8.1/PKG-INFO` & `ediri_azapi-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ediri_azapi
-Version: 1.8.1
+Version: 1.9.0
 Summary: A Pulumi package for creating and managing Azapi resources
 Home-page: https://github.com/dirien/pulumi-azapi
 License: Apache-2.0
 Project-URL: Repository, https://github.com/dirien/pulumi-azapi
 Keywords: pulumi azapi category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `ediri_azapi-1.8.1/README.md` & `ediri_azapi-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.8.1/ediri_azapi/__init__.py` & `ediri_azapi-1.9.0/ediri_azapi/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 from . import _utilities
 import typing
 # Export this package's modules as members:
 from .data_plane_resource import *
 from .get_resource import *
 from .get_resource_action import *
+from .get_resource_id import *
+from .get_resource_list import *
 from .provider import *
 from .resource import *
 from .resource_action import *
 from .update_resource import *
 from ._inputs import *
 from . import outputs
```

### Comparing `ediri_azapi-1.8.1/ediri_azapi/_inputs.py` & `ediri_azapi-1.9.0/ediri_azapi/_inputs.py`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.8.1/ediri_azapi/_utilities.py` & `ediri_azapi-1.9.0/ediri_azapi/_utilities.py`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.8.1/ediri_azapi/config/vars.py` & `ediri_azapi-1.9.0/ediri_azapi/config/vars.py`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.8.1/ediri_azapi/data_plane_resource.py` & `ediri_azapi-1.9.0/ediri_azapi/data_plane_resource.py`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.8.1/ediri_azapi/get_resource.py` & `ediri_azapi-1.9.0/ediri_azapi/get_resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         value = jsondecode(azapi_resource.example.output).properties.loginServer
         }
         """
         return pulumi.get(self, "output")
 
     @property
     @pulumi.getter(name="parentId")
-    def parent_id(self) -> Optional[str]:
+    def parent_id(self) -> str:
         return pulumi.get(self, "parent_id")
 
     @property
     @pulumi.getter(name="resourceId")
     def resource_id(self) -> Optional[str]:
         return pulumi.get(self, "resource_id")
 
@@ -166,14 +166,16 @@
            - resource group scope: `parent_id` should be the ID of a resource group, it's recommended to manage a resource group by azurerm_resource_group.
            - management group scope: `parent_id` should be the ID of a management group, it's recommended to manage a management group by azurerm_management_group.
            - extension scope: `parent_id` should be the ID of the resource you're adding the extension to.
            - subscription scope: `parent_id` should be like `/subscriptions/00000000-0000-0000-0000-000000000000`
            - tenant scope: `parent_id` should be `/`
            
            For child level resources, the `parent_id` should be the ID of its parent resource, for example, subnet resource's `parent_id` is the ID of the vnet.
+           
+           For type `Microsoft.Resources/resourceGroups`, the `parent_id` could be omitted, it defaults to subscription ID specified in provider or the default subscription(You could check the default subscription by azure cli command: `az account show`).
     :param str resource_id: The ID of an existing azure source.
            
            > **Note:** Configuring `name` and `parent_id` is an alternative way to configure `resource_id`.
     :param Sequence[str] response_export_values: A list of path that needs to be exported from response body.
            Setting it to `["*"]` will export the full response body.
            Here's an example. If it sets to `["properties.loginServer", "properties.policies.quarantinePolicy.status"]`, it will set the following json to computed property `output`.
            ```
@@ -234,14 +236,16 @@
            - resource group scope: `parent_id` should be the ID of a resource group, it's recommended to manage a resource group by azurerm_resource_group.
            - management group scope: `parent_id` should be the ID of a management group, it's recommended to manage a management group by azurerm_management_group.
            - extension scope: `parent_id` should be the ID of the resource you're adding the extension to.
            - subscription scope: `parent_id` should be like `/subscriptions/00000000-0000-0000-0000-000000000000`
            - tenant scope: `parent_id` should be `/`
            
            For child level resources, the `parent_id` should be the ID of its parent resource, for example, subnet resource's `parent_id` is the ID of the vnet.
+           
+           For type `Microsoft.Resources/resourceGroups`, the `parent_id` could be omitted, it defaults to subscription ID specified in provider or the default subscription(You could check the default subscription by azure cli command: `az account show`).
     :param str resource_id: The ID of an existing azure source.
            
            > **Note:** Configuring `name` and `parent_id` is an alternative way to configure `resource_id`.
     :param Sequence[str] response_export_values: A list of path that needs to be exported from response body.
            Setting it to `["*"]` will export the full response body.
            Here's an example. If it sets to `["properties.loginServer", "properties.policies.quarantinePolicy.status"]`, it will set the following json to computed property `output`.
            ```
```

### Comparing `ediri_azapi-1.8.1/ediri_azapi/get_resource_action.py` & `ediri_azapi-1.9.0/ediri_azapi/get_resource_action.py`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.8.1/ediri_azapi/outputs.py` & `ediri_azapi-1.9.0/ediri_azapi/outputs.py`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.8.1/ediri_azapi/provider.py` & `ediri_azapi-1.9.0/ediri_azapi/provider.py`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.8.1/ediri_azapi/resource.py` & `ediri_azapi-1.9.0/ediri_azapi/resource.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,46 +12,50 @@
 from ._inputs import *
 
 __all__ = ['ResourceArgs', 'Resource']
 
 @pulumi.input_type
 class ResourceArgs:
     def __init__(__self__, *,
-                 parent_id: pulumi.Input[str],
                  type: pulumi.Input[str],
                  body: Optional[pulumi.Input[str]] = None,
                  identity: Optional[pulumi.Input['ResourceIdentityArgs']] = None,
+                 ignore_body_changes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ignore_casing: Optional[pulumi.Input[bool]] = None,
                  ignore_missing_property: Optional[pulumi.Input[bool]] = None,
                  location: Optional[pulumi.Input[str]] = None,
                  locks: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
+                 parent_id: Optional[pulumi.Input[str]] = None,
                  removing_special_chars: Optional[pulumi.Input[bool]] = None,
                  response_export_values: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  schema_validation_enabled: Optional[pulumi.Input[bool]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a Resource resource.
-        :param pulumi.Input[str] parent_id: The ID of the azure resource in which this resource is created. Changing this forces a new resource to be created. It supports different kinds of deployment scope for **top level** resources: 
-               - resource group scope: `parent_id` should be the ID of a resource group, it's recommended to manage a resource group by azurerm_resource_group.
-               - management group scope: `parent_id` should be the ID of a management group, it's recommended to manage a management group by azurerm_management_group.
-               - extension scope: `parent_id` should be the ID of the resource you're adding the extension to.
-               - subscription scope: `parent_id` should be like `/subscriptions/00000000-0000-0000-0000-000000000000`
-               - tenant scope: `parent_id` should be `/`
-               
-               For child level resources, the `parent_id` should be the ID of its parent resource, for example, subnet resource's `parent_id` is the ID of the vnet.
         :param pulumi.Input[str] type: It is in a format like `<resource-type>@<api-version>`. `<resource-type>` is the Azure resource type, for example, `Microsoft.Storage/storageAccounts`.
                `<api-version>` is version of the API used to manage this azure resource.
         :param pulumi.Input[str] body: A JSON object that contains the request body used to create and update azure resource.
         :param pulumi.Input['ResourceIdentityArgs'] identity: A `identity` block as defined below.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] ignore_body_changes: A list of properties that should be ignored when comparing the `body` with its current state.
         :param pulumi.Input[bool] ignore_casing: Whether ignore incorrect casing returned in `body` to suppress plan-diff. Defaults to `false`.
         :param pulumi.Input[bool] ignore_missing_property: Whether ignore not returned properties like credentials in `body` to suppress plan-diff. Defaults to `true`.
         :param pulumi.Input[str] location: The Azure Region where the azure resource should exist.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] locks: A list of ARM resource IDs which are used to avoid create/modify/delete azapi resources at the same time.
         :param pulumi.Input[str] name: Specifies the name of the azure resource. Changing this forces a new resource to be created.
+        :param pulumi.Input[str] parent_id: The ID of the azure resource in which this resource is created. Changing this forces a new resource to be created. It supports different kinds of deployment scope for **top level** resources: 
+               - resource group scope: `parent_id` should be the ID of a resource group, it's recommended to manage a resource group by azurerm_resource_group.
+               - management group scope: `parent_id` should be the ID of a management group, it's recommended to manage a management group by azurerm_management_group.
+               - extension scope: `parent_id` should be the ID of the resource you're adding the extension to.
+               - subscription scope: `parent_id` should be like `/subscriptions/00000000-0000-0000-0000-000000000000`
+               - tenant scope: `parent_id` should be `/`
+               
+               For child level resources, the `parent_id` should be the ID of its parent resource, for example, subnet resource's `parent_id` is the ID of the vnet.
+               
+               For type `Microsoft.Resources/resourceGroups`, the `parent_id` could be omitted, it defaults to subscription ID specified in provider or the default subscription(You could check the default subscription by azure cli command: `az account show`).
         :param pulumi.Input[bool] removing_special_chars: Whether to remove special characters in resource name. Defaults to `false`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] response_export_values: A list of path that needs to be exported from response body.
                Setting it to `["*"]` will export the full response body.
                Here's an example. If it sets to `["properties.loginServer", "properties.policies.quarantinePolicy.status"]`, it will set the following json to computed property `output`.
                ```
                {
                "properties" : {
@@ -63,59 +67,43 @@
                }
                }
                }
                ```
         :param pulumi.Input[bool] schema_validation_enabled: Whether enabled the validation on `type` and `body` with embedded schema. Defaults to `true`.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: A mapping of tags which should be assigned to the azure resource.
         """
-        pulumi.set(__self__, "parent_id", parent_id)
         pulumi.set(__self__, "type", type)
         if body is not None:
             pulumi.set(__self__, "body", body)
         if identity is not None:
             pulumi.set(__self__, "identity", identity)
+        if ignore_body_changes is not None:
+            pulumi.set(__self__, "ignore_body_changes", ignore_body_changes)
         if ignore_casing is not None:
             pulumi.set(__self__, "ignore_casing", ignore_casing)
         if ignore_missing_property is not None:
             pulumi.set(__self__, "ignore_missing_property", ignore_missing_property)
         if location is not None:
             pulumi.set(__self__, "location", location)
         if locks is not None:
             pulumi.set(__self__, "locks", locks)
         if name is not None:
             pulumi.set(__self__, "name", name)
+        if parent_id is not None:
+            pulumi.set(__self__, "parent_id", parent_id)
         if removing_special_chars is not None:
             pulumi.set(__self__, "removing_special_chars", removing_special_chars)
         if response_export_values is not None:
             pulumi.set(__self__, "response_export_values", response_export_values)
         if schema_validation_enabled is not None:
             pulumi.set(__self__, "schema_validation_enabled", schema_validation_enabled)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
-    @pulumi.getter(name="parentId")
-    def parent_id(self) -> pulumi.Input[str]:
-        """
-        The ID of the azure resource in which this resource is created. Changing this forces a new resource to be created. It supports different kinds of deployment scope for **top level** resources: 
-        - resource group scope: `parent_id` should be the ID of a resource group, it's recommended to manage a resource group by azurerm_resource_group.
-        - management group scope: `parent_id` should be the ID of a management group, it's recommended to manage a management group by azurerm_management_group.
-        - extension scope: `parent_id` should be the ID of the resource you're adding the extension to.
-        - subscription scope: `parent_id` should be like `/subscriptions/00000000-0000-0000-0000-000000000000`
-        - tenant scope: `parent_id` should be `/`
-
-        For child level resources, the `parent_id` should be the ID of its parent resource, for example, subnet resource's `parent_id` is the ID of the vnet.
-        """
-        return pulumi.get(self, "parent_id")
-
-    @parent_id.setter
-    def parent_id(self, value: pulumi.Input[str]):
-        pulumi.set(self, "parent_id", value)
-
-    @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
         """
         It is in a format like `<resource-type>@<api-version>`. `<resource-type>` is the Azure resource type, for example, `Microsoft.Storage/storageAccounts`.
         `<api-version>` is version of the API used to manage this azure resource.
         """
         return pulumi.get(self, "type")
@@ -145,14 +133,26 @@
         return pulumi.get(self, "identity")
 
     @identity.setter
     def identity(self, value: Optional[pulumi.Input['ResourceIdentityArgs']]):
         pulumi.set(self, "identity", value)
 
     @property
+    @pulumi.getter(name="ignoreBodyChanges")
+    def ignore_body_changes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        A list of properties that should be ignored when comparing the `body` with its current state.
+        """
+        return pulumi.get(self, "ignore_body_changes")
+
+    @ignore_body_changes.setter
+    def ignore_body_changes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "ignore_body_changes", value)
+
+    @property
     @pulumi.getter(name="ignoreCasing")
     def ignore_casing(self) -> Optional[pulumi.Input[bool]]:
         """
         Whether ignore incorrect casing returned in `body` to suppress plan-diff. Defaults to `false`.
         """
         return pulumi.get(self, "ignore_casing")
 
@@ -205,14 +205,35 @@
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
+    @pulumi.getter(name="parentId")
+    def parent_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        The ID of the azure resource in which this resource is created. Changing this forces a new resource to be created. It supports different kinds of deployment scope for **top level** resources: 
+        - resource group scope: `parent_id` should be the ID of a resource group, it's recommended to manage a resource group by azurerm_resource_group.
+        - management group scope: `parent_id` should be the ID of a management group, it's recommended to manage a management group by azurerm_management_group.
+        - extension scope: `parent_id` should be the ID of the resource you're adding the extension to.
+        - subscription scope: `parent_id` should be like `/subscriptions/00000000-0000-0000-0000-000000000000`
+        - tenant scope: `parent_id` should be `/`
+
+        For child level resources, the `parent_id` should be the ID of its parent resource, for example, subnet resource's `parent_id` is the ID of the vnet.
+
+        For type `Microsoft.Resources/resourceGroups`, the `parent_id` could be omitted, it defaults to subscription ID specified in provider or the default subscription(You could check the default subscription by azure cli command: `az account show`).
+        """
+        return pulumi.get(self, "parent_id")
+
+    @parent_id.setter
+    def parent_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "parent_id", value)
+
+    @property
     @pulumi.getter(name="removingSpecialChars")
     def removing_special_chars(self) -> Optional[pulumi.Input[bool]]:
         """
         Whether to remove special characters in resource name. Defaults to `false`.
         """
         return pulumi.get(self, "removing_special_chars")
 
@@ -272,14 +293,15 @@
 
 
 @pulumi.input_type
 class _ResourceState:
     def __init__(__self__, *,
                  body: Optional[pulumi.Input[str]] = None,
                  identity: Optional[pulumi.Input['ResourceIdentityArgs']] = None,
+                 ignore_body_changes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ignore_casing: Optional[pulumi.Input[bool]] = None,
                  ignore_missing_property: Optional[pulumi.Input[bool]] = None,
                  location: Optional[pulumi.Input[str]] = None,
                  locks: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  output: Optional[pulumi.Input[str]] = None,
                  parent_id: Optional[pulumi.Input[str]] = None,
@@ -288,14 +310,15 @@
                  schema_validation_enabled: Optional[pulumi.Input[bool]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  type: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Resource resources.
         :param pulumi.Input[str] body: A JSON object that contains the request body used to create and update azure resource.
         :param pulumi.Input['ResourceIdentityArgs'] identity: A `identity` block as defined below.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] ignore_body_changes: A list of properties that should be ignored when comparing the `body` with its current state.
         :param pulumi.Input[bool] ignore_casing: Whether ignore incorrect casing returned in `body` to suppress plan-diff. Defaults to `false`.
         :param pulumi.Input[bool] ignore_missing_property: Whether ignore not returned properties like credentials in `body` to suppress plan-diff. Defaults to `true`.
         :param pulumi.Input[str] location: The Azure Region where the azure resource should exist.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] locks: A list of ARM resource IDs which are used to avoid create/modify/delete azapi resources at the same time.
         :param pulumi.Input[str] name: Specifies the name of the azure resource. Changing this forces a new resource to be created.
         :param pulumi.Input[str] output: The output json containing the properties specified in `response_export_values`. Here're some examples to decode json and extract the value.
                ```
@@ -307,14 +330,16 @@
                - resource group scope: `parent_id` should be the ID of a resource group, it's recommended to manage a resource group by azurerm_resource_group.
                - management group scope: `parent_id` should be the ID of a management group, it's recommended to manage a management group by azurerm_management_group.
                - extension scope: `parent_id` should be the ID of the resource you're adding the extension to.
                - subscription scope: `parent_id` should be like `/subscriptions/00000000-0000-0000-0000-000000000000`
                - tenant scope: `parent_id` should be `/`
                
                For child level resources, the `parent_id` should be the ID of its parent resource, for example, subnet resource's `parent_id` is the ID of the vnet.
+               
+               For type `Microsoft.Resources/resourceGroups`, the `parent_id` could be omitted, it defaults to subscription ID specified in provider or the default subscription(You could check the default subscription by azure cli command: `az account show`).
         :param pulumi.Input[bool] removing_special_chars: Whether to remove special characters in resource name. Defaults to `false`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] response_export_values: A list of path that needs to be exported from response body.
                Setting it to `["*"]` will export the full response body.
                Here's an example. If it sets to `["properties.loginServer", "properties.policies.quarantinePolicy.status"]`, it will set the following json to computed property `output`.
                ```
                {
                "properties" : {
@@ -332,14 +357,16 @@
         :param pulumi.Input[str] type: It is in a format like `<resource-type>@<api-version>`. `<resource-type>` is the Azure resource type, for example, `Microsoft.Storage/storageAccounts`.
                `<api-version>` is version of the API used to manage this azure resource.
         """
         if body is not None:
             pulumi.set(__self__, "body", body)
         if identity is not None:
             pulumi.set(__self__, "identity", identity)
+        if ignore_body_changes is not None:
+            pulumi.set(__self__, "ignore_body_changes", ignore_body_changes)
         if ignore_casing is not None:
             pulumi.set(__self__, "ignore_casing", ignore_casing)
         if ignore_missing_property is not None:
             pulumi.set(__self__, "ignore_missing_property", ignore_missing_property)
         if location is not None:
             pulumi.set(__self__, "location", location)
         if locks is not None:
@@ -382,14 +409,26 @@
         return pulumi.get(self, "identity")
 
     @identity.setter
     def identity(self, value: Optional[pulumi.Input['ResourceIdentityArgs']]):
         pulumi.set(self, "identity", value)
 
     @property
+    @pulumi.getter(name="ignoreBodyChanges")
+    def ignore_body_changes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        A list of properties that should be ignored when comparing the `body` with its current state.
+        """
+        return pulumi.get(self, "ignore_body_changes")
+
+    @ignore_body_changes.setter
+    def ignore_body_changes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "ignore_body_changes", value)
+
+    @property
     @pulumi.getter(name="ignoreCasing")
     def ignore_casing(self) -> Optional[pulumi.Input[bool]]:
         """
         Whether ignore incorrect casing returned in `body` to suppress plan-diff. Defaults to `false`.
         """
         return pulumi.get(self, "ignore_casing")
 
@@ -470,14 +509,16 @@
         - resource group scope: `parent_id` should be the ID of a resource group, it's recommended to manage a resource group by azurerm_resource_group.
         - management group scope: `parent_id` should be the ID of a management group, it's recommended to manage a management group by azurerm_management_group.
         - extension scope: `parent_id` should be the ID of the resource you're adding the extension to.
         - subscription scope: `parent_id` should be like `/subscriptions/00000000-0000-0000-0000-000000000000`
         - tenant scope: `parent_id` should be `/`
 
         For child level resources, the `parent_id` should be the ID of its parent resource, for example, subnet resource's `parent_id` is the ID of the vnet.
+
+        For type `Microsoft.Resources/resourceGroups`, the `parent_id` could be omitted, it defaults to subscription ID specified in provider or the default subscription(You could check the default subscription by azure cli command: `az account show`).
         """
         return pulumi.get(self, "parent_id")
 
     @parent_id.setter
     def parent_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "parent_id", value)
 
@@ -560,14 +601,15 @@
 class Resource(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  body: Optional[pulumi.Input[str]] = None,
                  identity: Optional[pulumi.Input[pulumi.InputType['ResourceIdentityArgs']]] = None,
+                 ignore_body_changes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ignore_casing: Optional[pulumi.Input[bool]] = None,
                  ignore_missing_property: Optional[pulumi.Input[bool]] = None,
                  location: Optional[pulumi.Input[str]] = None,
                  locks: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  parent_id: Optional[pulumi.Input[str]] = None,
                  removing_special_chars: Optional[pulumi.Input[bool]] = None,
@@ -585,27 +627,30 @@
 
         Azure resource can be imported using the `resource id`, e.g. <break><break>```sh<break> $ pulumi import azapi:index/resource:Resource example /subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/resGroup1/providers/Microsoft.MachineLearningServices/workspaces/workspace1/computes/cluster1 <break>```<break><break> It also supports specifying API version by using the `resource id` with `api-version` as a query parameter, e.g. <break><break>```sh<break> $ pulumi import azapi:index/resource:Resource example /subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/resGroup1/providers/Microsoft.MachineLearningServices/workspaces/workspace1/computes/cluster1?api-version=2021-07-01 <break>```<break><break>
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] body: A JSON object that contains the request body used to create and update azure resource.
         :param pulumi.Input[pulumi.InputType['ResourceIdentityArgs']] identity: A `identity` block as defined below.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] ignore_body_changes: A list of properties that should be ignored when comparing the `body` with its current state.
         :param pulumi.Input[bool] ignore_casing: Whether ignore incorrect casing returned in `body` to suppress plan-diff. Defaults to `false`.
         :param pulumi.Input[bool] ignore_missing_property: Whether ignore not returned properties like credentials in `body` to suppress plan-diff. Defaults to `true`.
         :param pulumi.Input[str] location: The Azure Region where the azure resource should exist.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] locks: A list of ARM resource IDs which are used to avoid create/modify/delete azapi resources at the same time.
         :param pulumi.Input[str] name: Specifies the name of the azure resource. Changing this forces a new resource to be created.
         :param pulumi.Input[str] parent_id: The ID of the azure resource in which this resource is created. Changing this forces a new resource to be created. It supports different kinds of deployment scope for **top level** resources: 
                - resource group scope: `parent_id` should be the ID of a resource group, it's recommended to manage a resource group by azurerm_resource_group.
                - management group scope: `parent_id` should be the ID of a management group, it's recommended to manage a management group by azurerm_management_group.
                - extension scope: `parent_id` should be the ID of the resource you're adding the extension to.
                - subscription scope: `parent_id` should be like `/subscriptions/00000000-0000-0000-0000-000000000000`
                - tenant scope: `parent_id` should be `/`
                
                For child level resources, the `parent_id` should be the ID of its parent resource, for example, subnet resource's `parent_id` is the ID of the vnet.
+               
+               For type `Microsoft.Resources/resourceGroups`, the `parent_id` could be omitted, it defaults to subscription ID specified in provider or the default subscription(You could check the default subscription by azure cli command: `az account show`).
         :param pulumi.Input[bool] removing_special_chars: Whether to remove special characters in resource name. Defaults to `false`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] response_export_values: A list of path that needs to be exported from response body.
                Setting it to `["*"]` will export the full response body.
                Here's an example. If it sets to `["properties.loginServer", "properties.policies.quarantinePolicy.status"]`, it will set the following json to computed property `output`.
                ```
                {
                "properties" : {
@@ -651,14 +696,15 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  body: Optional[pulumi.Input[str]] = None,
                  identity: Optional[pulumi.Input[pulumi.InputType['ResourceIdentityArgs']]] = None,
+                 ignore_body_changes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ignore_casing: Optional[pulumi.Input[bool]] = None,
                  ignore_missing_property: Optional[pulumi.Input[bool]] = None,
                  location: Optional[pulumi.Input[str]] = None,
                  locks: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  parent_id: Optional[pulumi.Input[str]] = None,
                  removing_special_chars: Optional[pulumi.Input[bool]] = None,
@@ -673,21 +719,20 @@
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ResourceArgs.__new__(ResourceArgs)
 
             __props__.__dict__["body"] = body
             __props__.__dict__["identity"] = identity
+            __props__.__dict__["ignore_body_changes"] = ignore_body_changes
             __props__.__dict__["ignore_casing"] = ignore_casing
             __props__.__dict__["ignore_missing_property"] = ignore_missing_property
             __props__.__dict__["location"] = location
             __props__.__dict__["locks"] = locks
             __props__.__dict__["name"] = name
-            if parent_id is None and not opts.urn:
-                raise TypeError("Missing required property 'parent_id'")
             __props__.__dict__["parent_id"] = parent_id
             __props__.__dict__["removing_special_chars"] = removing_special_chars
             __props__.__dict__["response_export_values"] = response_export_values
             __props__.__dict__["schema_validation_enabled"] = schema_validation_enabled
             __props__.__dict__["tags"] = tags
             if type is None and not opts.urn:
                 raise TypeError("Missing required property 'type'")
@@ -701,14 +746,15 @@
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             body: Optional[pulumi.Input[str]] = None,
             identity: Optional[pulumi.Input[pulumi.InputType['ResourceIdentityArgs']]] = None,
+            ignore_body_changes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             ignore_casing: Optional[pulumi.Input[bool]] = None,
             ignore_missing_property: Optional[pulumi.Input[bool]] = None,
             location: Optional[pulumi.Input[str]] = None,
             locks: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             name: Optional[pulumi.Input[str]] = None,
             output: Optional[pulumi.Input[str]] = None,
             parent_id: Optional[pulumi.Input[str]] = None,
@@ -722,14 +768,15 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] body: A JSON object that contains the request body used to create and update azure resource.
         :param pulumi.Input[pulumi.InputType['ResourceIdentityArgs']] identity: A `identity` block as defined below.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] ignore_body_changes: A list of properties that should be ignored when comparing the `body` with its current state.
         :param pulumi.Input[bool] ignore_casing: Whether ignore incorrect casing returned in `body` to suppress plan-diff. Defaults to `false`.
         :param pulumi.Input[bool] ignore_missing_property: Whether ignore not returned properties like credentials in `body` to suppress plan-diff. Defaults to `true`.
         :param pulumi.Input[str] location: The Azure Region where the azure resource should exist.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] locks: A list of ARM resource IDs which are used to avoid create/modify/delete azapi resources at the same time.
         :param pulumi.Input[str] name: Specifies the name of the azure resource. Changing this forces a new resource to be created.
         :param pulumi.Input[str] output: The output json containing the properties specified in `response_export_values`. Here're some examples to decode json and extract the value.
                ```
@@ -741,14 +788,16 @@
                - resource group scope: `parent_id` should be the ID of a resource group, it's recommended to manage a resource group by azurerm_resource_group.
                - management group scope: `parent_id` should be the ID of a management group, it's recommended to manage a management group by azurerm_management_group.
                - extension scope: `parent_id` should be the ID of the resource you're adding the extension to.
                - subscription scope: `parent_id` should be like `/subscriptions/00000000-0000-0000-0000-000000000000`
                - tenant scope: `parent_id` should be `/`
                
                For child level resources, the `parent_id` should be the ID of its parent resource, for example, subnet resource's `parent_id` is the ID of the vnet.
+               
+               For type `Microsoft.Resources/resourceGroups`, the `parent_id` could be omitted, it defaults to subscription ID specified in provider or the default subscription(You could check the default subscription by azure cli command: `az account show`).
         :param pulumi.Input[bool] removing_special_chars: Whether to remove special characters in resource name. Defaults to `false`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] response_export_values: A list of path that needs to be exported from response body.
                Setting it to `["*"]` will export the full response body.
                Here's an example. If it sets to `["properties.loginServer", "properties.policies.quarantinePolicy.status"]`, it will set the following json to computed property `output`.
                ```
                {
                "properties" : {
@@ -768,14 +817,15 @@
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ResourceState.__new__(_ResourceState)
 
         __props__.__dict__["body"] = body
         __props__.__dict__["identity"] = identity
+        __props__.__dict__["ignore_body_changes"] = ignore_body_changes
         __props__.__dict__["ignore_casing"] = ignore_casing
         __props__.__dict__["ignore_missing_property"] = ignore_missing_property
         __props__.__dict__["location"] = location
         __props__.__dict__["locks"] = locks
         __props__.__dict__["name"] = name
         __props__.__dict__["output"] = output
         __props__.__dict__["parent_id"] = parent_id
@@ -799,14 +849,22 @@
     def identity(self) -> pulumi.Output['outputs.ResourceIdentity']:
         """
         A `identity` block as defined below.
         """
         return pulumi.get(self, "identity")
 
     @property
+    @pulumi.getter(name="ignoreBodyChanges")
+    def ignore_body_changes(self) -> pulumi.Output[Optional[Sequence[str]]]:
+        """
+        A list of properties that should be ignored when comparing the `body` with its current state.
+        """
+        return pulumi.get(self, "ignore_body_changes")
+
+    @property
     @pulumi.getter(name="ignoreCasing")
     def ignore_casing(self) -> pulumi.Output[Optional[bool]]:
         """
         Whether ignore incorrect casing returned in `body` to suppress plan-diff. Defaults to `false`.
         """
         return pulumi.get(self, "ignore_casing")
 
@@ -863,14 +921,16 @@
         - resource group scope: `parent_id` should be the ID of a resource group, it's recommended to manage a resource group by azurerm_resource_group.
         - management group scope: `parent_id` should be the ID of a management group, it's recommended to manage a management group by azurerm_management_group.
         - extension scope: `parent_id` should be the ID of the resource you're adding the extension to.
         - subscription scope: `parent_id` should be like `/subscriptions/00000000-0000-0000-0000-000000000000`
         - tenant scope: `parent_id` should be `/`
 
         For child level resources, the `parent_id` should be the ID of its parent resource, for example, subnet resource's `parent_id` is the ID of the vnet.
+
+        For type `Microsoft.Resources/resourceGroups`, the `parent_id` could be omitted, it defaults to subscription ID specified in provider or the default subscription(You could check the default subscription by azure cli command: `az account show`).
         """
         return pulumi.get(self, "parent_id")
 
     @property
     @pulumi.getter(name="removingSpecialChars")
     def removing_special_chars(self) -> pulumi.Output[Optional[bool]]:
         """
```

### Comparing `ediri_azapi-1.8.1/ediri_azapi/resource_action.py` & `ediri_azapi-1.9.0/ediri_azapi/resource_action.py`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.8.1/ediri_azapi/update_resource.py` & `ediri_azapi-1.9.0/ediri_azapi/update_resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,26 +12,28 @@
 __all__ = ['UpdateResourceArgs', 'UpdateResource']
 
 @pulumi.input_type
 class UpdateResourceArgs:
     def __init__(__self__, *,
                  type: pulumi.Input[str],
                  body: Optional[pulumi.Input[str]] = None,
+                 ignore_body_changes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ignore_casing: Optional[pulumi.Input[bool]] = None,
                  ignore_missing_property: Optional[pulumi.Input[bool]] = None,
                  locks: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  parent_id: Optional[pulumi.Input[str]] = None,
                  resource_id: Optional[pulumi.Input[str]] = None,
                  response_export_values: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a UpdateResource resource.
         :param pulumi.Input[str] type: It is in a format like `<resource-type>@<api-version>`. `<resource-type>` is the Azure resource type, for example, `Microsoft.Storage/storageAccounts`.
                `<api-version>` is version of the API used to manage this azure resource.
         :param pulumi.Input[str] body: A JSON object that contains the request body used to add on an existing azure resource.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] ignore_body_changes: A list of properties that should be ignored when comparing the `body` with its current state.
         :param pulumi.Input[bool] ignore_casing: Whether ignore incorrect casing returned in `body` to suppress plan-diff. Defaults to `false`.
         :param pulumi.Input[bool] ignore_missing_property: Whether ignore not returned properties like credentials in `body` to suppress plan-diff. Defaults to `true`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] locks: A list of ARM resource IDs which are used to avoid create/modify/delete azapi resources at the same time.
         :param pulumi.Input[str] name: Specifies the name of the azure resource. Changing this forces a new resource to be created.
         :param pulumi.Input[str] parent_id: The ID of the azure resource in which this resource is created. Changing this forces a new resource to be created. It supports different kinds of deployment scope for **top level** resources: 
                - resource group scope: `parent_id` should be the ID of a resource group, it's recommended to manage a resource group by azurerm_resource_group.
                - management group scope: `parent_id` should be the ID of a management group, it's recommended to manage a management group by azurerm_management_group.
@@ -58,14 +60,16 @@
                }
                }
                ```
         """
         pulumi.set(__self__, "type", type)
         if body is not None:
             pulumi.set(__self__, "body", body)
+        if ignore_body_changes is not None:
+            pulumi.set(__self__, "ignore_body_changes", ignore_body_changes)
         if ignore_casing is not None:
             pulumi.set(__self__, "ignore_casing", ignore_casing)
         if ignore_missing_property is not None:
             pulumi.set(__self__, "ignore_missing_property", ignore_missing_property)
         if locks is not None:
             pulumi.set(__self__, "locks", locks)
         if name is not None:
@@ -99,14 +103,26 @@
         return pulumi.get(self, "body")
 
     @body.setter
     def body(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "body", value)
 
     @property
+    @pulumi.getter(name="ignoreBodyChanges")
+    def ignore_body_changes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        A list of properties that should be ignored when comparing the `body` with its current state.
+        """
+        return pulumi.get(self, "ignore_body_changes")
+
+    @ignore_body_changes.setter
+    def ignore_body_changes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "ignore_body_changes", value)
+
+    @property
     @pulumi.getter(name="ignoreCasing")
     def ignore_casing(self) -> Optional[pulumi.Input[bool]]:
         """
         Whether ignore incorrect casing returned in `body` to suppress plan-diff. Defaults to `false`.
         """
         return pulumi.get(self, "ignore_casing")
 
@@ -210,26 +226,28 @@
         pulumi.set(self, "response_export_values", value)
 
 
 @pulumi.input_type
 class _UpdateResourceState:
     def __init__(__self__, *,
                  body: Optional[pulumi.Input[str]] = None,
+                 ignore_body_changes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ignore_casing: Optional[pulumi.Input[bool]] = None,
                  ignore_missing_property: Optional[pulumi.Input[bool]] = None,
                  locks: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  output: Optional[pulumi.Input[str]] = None,
                  parent_id: Optional[pulumi.Input[str]] = None,
                  resource_id: Optional[pulumi.Input[str]] = None,
                  response_export_values: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  type: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering UpdateResource resources.
         :param pulumi.Input[str] body: A JSON object that contains the request body used to add on an existing azure resource.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] ignore_body_changes: A list of properties that should be ignored when comparing the `body` with its current state.
         :param pulumi.Input[bool] ignore_casing: Whether ignore incorrect casing returned in `body` to suppress plan-diff. Defaults to `false`.
         :param pulumi.Input[bool] ignore_missing_property: Whether ignore not returned properties like credentials in `body` to suppress plan-diff. Defaults to `true`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] locks: A list of ARM resource IDs which are used to avoid create/modify/delete azapi resources at the same time.
         :param pulumi.Input[str] name: Specifies the name of the azure resource. Changing this forces a new resource to be created.
         :param pulumi.Input[str] output: The output json containing the properties specified in `response_export_values`. Here're some examples to decode json and extract the value.
                ```
                // it will output "registry1.azurecr.io"
@@ -263,14 +281,16 @@
                }
                ```
         :param pulumi.Input[str] type: It is in a format like `<resource-type>@<api-version>`. `<resource-type>` is the Azure resource type, for example, `Microsoft.Storage/storageAccounts`.
                `<api-version>` is version of the API used to manage this azure resource.
         """
         if body is not None:
             pulumi.set(__self__, "body", body)
+        if ignore_body_changes is not None:
+            pulumi.set(__self__, "ignore_body_changes", ignore_body_changes)
         if ignore_casing is not None:
             pulumi.set(__self__, "ignore_casing", ignore_casing)
         if ignore_missing_property is not None:
             pulumi.set(__self__, "ignore_missing_property", ignore_missing_property)
         if locks is not None:
             pulumi.set(__self__, "locks", locks)
         if name is not None:
@@ -295,14 +315,26 @@
         return pulumi.get(self, "body")
 
     @body.setter
     def body(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "body", value)
 
     @property
+    @pulumi.getter(name="ignoreBodyChanges")
+    def ignore_body_changes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        A list of properties that should be ignored when comparing the `body` with its current state.
+        """
+        return pulumi.get(self, "ignore_body_changes")
+
+    @ignore_body_changes.setter
+    def ignore_body_changes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "ignore_body_changes", value)
+
+    @property
     @pulumi.getter(name="ignoreCasing")
     def ignore_casing(self) -> Optional[pulumi.Input[bool]]:
         """
         Whether ignore incorrect casing returned in `body` to suppress plan-diff. Defaults to `false`.
         """
         return pulumi.get(self, "ignore_casing")
 
@@ -438,14 +470,15 @@
 
 class UpdateResource(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  body: Optional[pulumi.Input[str]] = None,
+                 ignore_body_changes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ignore_casing: Optional[pulumi.Input[bool]] = None,
                  ignore_missing_property: Optional[pulumi.Input[bool]] = None,
                  locks: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  parent_id: Optional[pulumi.Input[str]] = None,
                  resource_id: Optional[pulumi.Input[str]] = None,
                  response_export_values: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
@@ -459,14 +492,15 @@
         If you want to restore the modified properties to some values, you must apply the restored properties before deleting.
 
         ## Example Usage
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] body: A JSON object that contains the request body used to add on an existing azure resource.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] ignore_body_changes: A list of properties that should be ignored when comparing the `body` with its current state.
         :param pulumi.Input[bool] ignore_casing: Whether ignore incorrect casing returned in `body` to suppress plan-diff. Defaults to `false`.
         :param pulumi.Input[bool] ignore_missing_property: Whether ignore not returned properties like credentials in `body` to suppress plan-diff. Defaults to `true`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] locks: A list of ARM resource IDs which are used to avoid create/modify/delete azapi resources at the same time.
         :param pulumi.Input[str] name: Specifies the name of the azure resource. Changing this forces a new resource to be created.
         :param pulumi.Input[str] parent_id: The ID of the azure resource in which this resource is created. Changing this forces a new resource to be created. It supports different kinds of deployment scope for **top level** resources: 
                - resource group scope: `parent_id` should be the ID of a resource group, it's recommended to manage a resource group by azurerm_resource_group.
                - management group scope: `parent_id` should be the ID of a management group, it's recommended to manage a management group by azurerm_management_group.
@@ -523,14 +557,15 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  body: Optional[pulumi.Input[str]] = None,
+                 ignore_body_changes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ignore_casing: Optional[pulumi.Input[bool]] = None,
                  ignore_missing_property: Optional[pulumi.Input[bool]] = None,
                  locks: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  parent_id: Optional[pulumi.Input[str]] = None,
                  resource_id: Optional[pulumi.Input[str]] = None,
                  response_export_values: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
@@ -541,14 +576,15 @@
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = UpdateResourceArgs.__new__(UpdateResourceArgs)
 
             __props__.__dict__["body"] = body
+            __props__.__dict__["ignore_body_changes"] = ignore_body_changes
             __props__.__dict__["ignore_casing"] = ignore_casing
             __props__.__dict__["ignore_missing_property"] = ignore_missing_property
             __props__.__dict__["locks"] = locks
             __props__.__dict__["name"] = name
             __props__.__dict__["parent_id"] = parent_id
             __props__.__dict__["resource_id"] = resource_id
             __props__.__dict__["response_export_values"] = response_export_values
@@ -563,14 +599,15 @@
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             body: Optional[pulumi.Input[str]] = None,
+            ignore_body_changes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             ignore_casing: Optional[pulumi.Input[bool]] = None,
             ignore_missing_property: Optional[pulumi.Input[bool]] = None,
             locks: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             name: Optional[pulumi.Input[str]] = None,
             output: Optional[pulumi.Input[str]] = None,
             parent_id: Optional[pulumi.Input[str]] = None,
             resource_id: Optional[pulumi.Input[str]] = None,
@@ -580,14 +617,15 @@
         Get an existing UpdateResource resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] body: A JSON object that contains the request body used to add on an existing azure resource.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] ignore_body_changes: A list of properties that should be ignored when comparing the `body` with its current state.
         :param pulumi.Input[bool] ignore_casing: Whether ignore incorrect casing returned in `body` to suppress plan-diff. Defaults to `false`.
         :param pulumi.Input[bool] ignore_missing_property: Whether ignore not returned properties like credentials in `body` to suppress plan-diff. Defaults to `true`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] locks: A list of ARM resource IDs which are used to avoid create/modify/delete azapi resources at the same time.
         :param pulumi.Input[str] name: Specifies the name of the azure resource. Changing this forces a new resource to be created.
         :param pulumi.Input[str] output: The output json containing the properties specified in `response_export_values`. Here're some examples to decode json and extract the value.
                ```
                // it will output "registry1.azurecr.io"
@@ -624,14 +662,15 @@
                `<api-version>` is version of the API used to manage this azure resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _UpdateResourceState.__new__(_UpdateResourceState)
 
         __props__.__dict__["body"] = body
+        __props__.__dict__["ignore_body_changes"] = ignore_body_changes
         __props__.__dict__["ignore_casing"] = ignore_casing
         __props__.__dict__["ignore_missing_property"] = ignore_missing_property
         __props__.__dict__["locks"] = locks
         __props__.__dict__["name"] = name
         __props__.__dict__["output"] = output
         __props__.__dict__["parent_id"] = parent_id
         __props__.__dict__["resource_id"] = resource_id
@@ -644,14 +683,22 @@
     def body(self) -> pulumi.Output[Optional[str]]:
         """
         A JSON object that contains the request body used to add on an existing azure resource.
         """
         return pulumi.get(self, "body")
 
     @property
+    @pulumi.getter(name="ignoreBodyChanges")
+    def ignore_body_changes(self) -> pulumi.Output[Optional[Sequence[str]]]:
+        """
+        A list of properties that should be ignored when comparing the `body` with its current state.
+        """
+        return pulumi.get(self, "ignore_body_changes")
+
+    @property
     @pulumi.getter(name="ignoreCasing")
     def ignore_casing(self) -> pulumi.Output[Optional[bool]]:
         """
         Whether ignore incorrect casing returned in `body` to suppress plan-diff. Defaults to `false`.
         """
         return pulumi.get(self, "ignore_casing")
```

### Comparing `ediri_azapi-1.8.1/ediri_azapi.egg-info/PKG-INFO` & `ediri_azapi-1.9.0/ediri_azapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ediri-azapi
-Version: 1.8.1
+Version: 1.9.0
 Summary: A Pulumi package for creating and managing Azapi resources
 Home-page: https://github.com/dirien/pulumi-azapi
 License: Apache-2.0
 Project-URL: Repository, https://github.com/dirien/pulumi-azapi
 Keywords: pulumi azapi category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `ediri_azapi-1.8.1/ediri_azapi.egg-info/SOURCES.txt` & `ediri_azapi-1.9.0/ediri_azapi.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 setup.py
 ediri_azapi/__init__.py
 ediri_azapi/_inputs.py
 ediri_azapi/_utilities.py
 ediri_azapi/data_plane_resource.py
 ediri_azapi/get_resource.py
 ediri_azapi/get_resource_action.py
+ediri_azapi/get_resource_id.py
+ediri_azapi/get_resource_list.py
 ediri_azapi/outputs.py
 ediri_azapi/provider.py
 ediri_azapi/pulumi-plugin.json
 ediri_azapi/py.typed
 ediri_azapi/resource.py
 ediri_azapi/resource_action.py
 ediri_azapi/update_resource.py
```

### Comparing `ediri_azapi-1.8.1/setup.py` & `ediri_azapi-1.9.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,52 +4,29 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.8.1"
-PLUGIN_VERSION = "1.8.1"
-
-class InstallPluginCommand(install):
-    def run(self):
-        install.run(self)
-        try:
-            check_call(['pulumi', 'plugin', 'install', 'resource', 'azapi', PLUGIN_VERSION, '--server', 'github://api.github.com/dirien/pulumi-azapi'])
-        except OSError as error:
-            if error.errno == errno.ENOENT:
-                print(f"""
-                There was an error installing the azapi resource provider plugin.
-                It looks like `pulumi` is not installed on your system.
-                Please visit https://pulumi.com/ to install the Pulumi CLI.
-                You may try manually installing the plugin by running
-                `pulumi plugin install resource azapi {PLUGIN_VERSION}`
-                """)
-            else:
-                raise
-
-
+VERSION = "1.9.0"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "azapi Pulumi Package - Development Version"
 
 
 setup(name='ediri_azapi',
       python_requires='>=3.7',
       version=VERSION,
       description="A Pulumi package for creating and managing Azapi resources",
       long_description=readme(),
       long_description_content_type='text/markdown',
-      cmdclass={
-          'install': InstallPluginCommand,
-      },
       keywords='pulumi azapi category/cloud',
       url='https://github.com/dirien/pulumi-azapi',
       project_urls={
           'Repository': 'https://github.com/dirien/pulumi-azapi'
       },
       license='Apache-2.0',
       packages=find_packages(),
```

