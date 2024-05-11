# Comparing `tmp/port_pulumi-1.9.1.tar.gz` & `tmp/port_pulumi-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "port_pulumi-1.9.1.tar", last modified: Sun Jan 21 14:27:02 2024, max compression
+gzip compressed data, was "port_pulumi-2.0.0.tar", last modified: Sat May 11 09:52:22 2024, max compression
```

## Comparing `port_pulumi-1.9.1.tar` & `port_pulumi-2.0.0.tar`

### file list

```diff
@@ -1,32 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 14:27:02.457555 port_pulumi-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-01-21 14:27:02.457555 port_pulumi-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 14:27:02.457555 port_pulumi-1.9.1/port_pulumi/
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   131924 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9292 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    40529 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/action.py
--rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/action_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9416 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/aggregation_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    21679 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/aggregation_property.py
--rw-r--r--   0 runner    (1001) docker     (127)    34831 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/blueprint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 14:27:02.457555 port_pulumi-1.9.1/port_pulumi/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    22683 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)   107846 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    15511 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/scorecard.py
--rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/team.py
--rw-r--r--   0 runner    (1001) docker     (127)    22651 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 14:27:02.457555 port_pulumi-1.9.1/port_pulumi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-21 14:27:02.457555 port_pulumi-1.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 09:52:22.334064 port_pulumi-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-11 09:52:22.334064 port_pulumi-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 09:52:22.334064 port_pulumi-2.0.0/port_pulumi/
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   196235 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9291 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43486 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11880 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/action_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30278 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/aggregation_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21679 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/aggregation_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36508 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8083 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/blueprint_permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 09:52:22.334064 port_pulumi-2.0.0/port_pulumi/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22571 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)   167091 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24949 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/page_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    21899 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/scorecard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11901 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22539 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 09:52:22.334064 port_pulumi-2.0.0/port_pulumi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-11 09:52:22.000000 port_pulumi-2.0.0/port_pulumi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-11 09:52:22.000000 port_pulumi-2.0.0/port_pulumi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 09:52:22.000000 port_pulumi-2.0.0/port_pulumi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 09:52:22.000000 port_pulumi-2.0.0/port_pulumi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-11 09:52:22.000000 port_pulumi-2.0.0/port_pulumi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-11 09:52:22.000000 port_pulumi-2.0.0/port_pulumi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 09:52:22.338064 port_pulumi-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-11 09:52:22.000000 port_pulumi-2.0.0/setup.py
```

### Comparing `port_pulumi-1.9.1/PKG-INFO` & `port_pulumi-2.0.0/port_pulumi.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
-Name: port_pulumi
-Version: 1.9.1
+Name: port-pulumi
+Version: 2.0.0
 Summary: A Pulumi package for creating and managing Port resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/port-labs/pulumi-port
 Keywords: pulumi port category/utility
 Platform: UNKNOWN
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Port Resource Provider
 
-![Port](./img/port.svg)
+<img src="img/port.svg" width="300px">
 
 The Port Resource Provider lets you manage [Port](https://www.getport.io) resources.
 
 ## Installing
 
 This package is available for several languages/platforms:
```

### Comparing `port_pulumi-1.9.1/README.md` & `port_pulumi-2.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Port Resource Provider
 
-![Port](./img/port.svg)
+<img src="img/port.svg" width="300px">
 
 The Port Resource Provider lets you manage [Port](https://www.getport.io) resources.
 
 ## Installing
 
 This package is available for several languages/platforms:
```

### Comparing `port_pulumi-1.9.1/port_pulumi/__init__.py` & `port_pulumi-2.0.0/port_pulumi/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 from . import _utilities
 import typing
 # Export this package's modules as members:
 from .action import *
 from .action_permissions import *
 from .aggregation_properties import *
 from .blueprint import *
+from .blueprint_permissions import *
 from .entity import *
+from .page import *
+from .page_permissions import *
 from .provider import *
 from .scorecard import *
 from .team import *
 from .webhook import *
 from ._inputs import *
 from . import outputs
 
@@ -57,22 +60,46 @@
   "fqn": "port_pulumi",
   "classes": {
    "port:index/blueprint:Blueprint": "Blueprint"
   }
  },
  {
   "pkg": "port",
+  "mod": "index/blueprintPermissions",
+  "fqn": "port_pulumi",
+  "classes": {
+   "port:index/blueprintPermissions:BlueprintPermissions": "BlueprintPermissions"
+  }
+ },
+ {
+  "pkg": "port",
   "mod": "index/entity",
   "fqn": "port_pulumi",
   "classes": {
    "port:index/entity:Entity": "Entity"
   }
  },
  {
   "pkg": "port",
+  "mod": "index/page",
+  "fqn": "port_pulumi",
+  "classes": {
+   "port:index/page:Page": "Page"
+  }
+ },
+ {
+  "pkg": "port",
+  "mod": "index/pagePermissions",
+  "fqn": "port_pulumi",
+  "classes": {
+   "port:index/pagePermissions:PagePermissions": "PagePermissions"
+  }
+ },
+ {
+  "pkg": "port",
   "mod": "index/scorecard",
   "fqn": "port_pulumi",
   "classes": {
    "port:index/scorecard:Scorecard": "Scorecard"
   }
  },
  {
```

### Comparing `port_pulumi-1.9.1/port_pulumi/_utilities.py` & `port_pulumi-2.0.0/port_pulumi/_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 
 import asyncio
+import importlib.metadata
 import importlib.util
 import inspect
 import json
 import os
-import pkg_resources
 import sys
 import typing
 
 import pulumi
 import pulumi.runtime
 from pulumi.runtime.sync_await import _sync_await
 
@@ -68,15 +68,15 @@
     # pkg_resources uses setuptools to inspect the set of installed packages. We use it here to ask
     # for the currently installed version of the root package (i.e. us) and get its version.
 
     # Unfortunately, PEP440 and semver differ slightly in incompatible ways. The Pulumi engine expects
     # to receive a valid semver string when receiving requests from the language host, so it's our
     # responsibility as the library to convert our own PEP440 version into a valid semver string.
 
-    pep440_version_string = pkg_resources.require(root_package)[0].version
+    pep440_version_string = importlib.metadata.version(root_package)
     pep440_version = PEP440Version.parse(pep440_version_string)
     (major, minor, patch) = pep440_version.release
     prerelease = None
     if pep440_version.pre_tag == 'a':
         prerelease = f"alpha.{pep440_version.pre}"
     elif pep440_version.pre_tag == 'b':
         prerelease = f"beta.{pep440_version.pre}"
```

### Comparing `port_pulumi-1.9.1/port_pulumi/action.py` & `port_pulumi-2.0.0/port_pulumi/action.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,131 +12,93 @@
 from ._inputs import *
 
 __all__ = ['ActionArgs', 'Action']
 
 @pulumi.input_type
 class ActionArgs:
     def __init__(__self__, *,
-                 blueprint: pulumi.Input[str],
                  identifier: pulumi.Input[str],
-                 title: pulumi.Input[str],
-                 trigger: pulumi.Input[str],
                  approval_email_notification: Optional[pulumi.Input['ActionApprovalEmailNotificationArgs']] = None,
                  approval_webhook_notification: Optional[pulumi.Input['ActionApprovalWebhookNotificationArgs']] = None,
                  azure_method: Optional[pulumi.Input['ActionAzureMethodArgs']] = None,
+                 blueprint: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  github_method: Optional[pulumi.Input['ActionGithubMethodArgs']] = None,
                  gitlab_method: Optional[pulumi.Input['ActionGitlabMethodArgs']] = None,
                  icon: Optional[pulumi.Input[str]] = None,
                  kafka_method: Optional[pulumi.Input['ActionKafkaMethodArgs']] = None,
-                 order_properties: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 publish: Optional[pulumi.Input[bool]] = None,
                  required_approval: Optional[pulumi.Input[bool]] = None,
-                 required_jq_query: Optional[pulumi.Input[str]] = None,
-                 user_properties: Optional[pulumi.Input['ActionUserPropertiesArgs']] = None,
+                 self_service_trigger: Optional[pulumi.Input['ActionSelfServiceTriggerArgs']] = None,
+                 title: Optional[pulumi.Input[str]] = None,
                  webhook_method: Optional[pulumi.Input['ActionWebhookMethodArgs']] = None):
         """
         The set of arguments for constructing a Action resource.
-        :param pulumi.Input[str] blueprint: The blueprint identifier the action relates to
         :param pulumi.Input[str] identifier: Identifier
-        :param pulumi.Input[str] title: Title
-        :param pulumi.Input[str] trigger: The trigger type of the action
         :param pulumi.Input['ActionApprovalEmailNotificationArgs'] approval_email_notification: The email notification of the approval
         :param pulumi.Input['ActionApprovalWebhookNotificationArgs'] approval_webhook_notification: The webhook notification of the approval
-        :param pulumi.Input['ActionAzureMethodArgs'] azure_method: The invocation method of the action
+        :param pulumi.Input['ActionAzureMethodArgs'] azure_method: Azure DevOps invocation method
+        :param pulumi.Input[str] blueprint: The blueprint identifier the action relates to
         :param pulumi.Input[str] description: Description
-        :param pulumi.Input['ActionGithubMethodArgs'] github_method: The invocation method of the action
-        :param pulumi.Input['ActionGitlabMethodArgs'] gitlab_method: The invocation method of the action
+        :param pulumi.Input['ActionGithubMethodArgs'] github_method: GitHub invocation method
+        :param pulumi.Input['ActionGitlabMethodArgs'] gitlab_method: Gitlab invocation method
         :param pulumi.Input[str] icon: Icon
-        :param pulumi.Input['ActionKafkaMethodArgs'] kafka_method: The invocation method of the action
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] order_properties: Order properties
+        :param pulumi.Input['ActionKafkaMethodArgs'] kafka_method: Kafka invocation method
+        :param pulumi.Input[bool] publish: Publish action
         :param pulumi.Input[bool] required_approval: Require approval before invoking the action
-        :param pulumi.Input[str] required_jq_query: The required jq query of the property
-        :param pulumi.Input['ActionUserPropertiesArgs'] user_properties: User properties
-        :param pulumi.Input['ActionWebhookMethodArgs'] webhook_method: The invocation method of the action
+        :param pulumi.Input['ActionSelfServiceTriggerArgs'] self_service_trigger: Self service trigger for the action
+        :param pulumi.Input[str] title: Title
+        :param pulumi.Input['ActionWebhookMethodArgs'] webhook_method: Webhook invocation method
         """
-        pulumi.set(__self__, "blueprint", blueprint)
         pulumi.set(__self__, "identifier", identifier)
-        pulumi.set(__self__, "title", title)
-        pulumi.set(__self__, "trigger", trigger)
         if approval_email_notification is not None:
             pulumi.set(__self__, "approval_email_notification", approval_email_notification)
         if approval_webhook_notification is not None:
             pulumi.set(__self__, "approval_webhook_notification", approval_webhook_notification)
         if azure_method is not None:
             pulumi.set(__self__, "azure_method", azure_method)
+        if blueprint is not None:
+            warnings.warn("""Action is not attached to blueprint anymore. This value is ignored""", DeprecationWarning)
+            pulumi.log.warn("""blueprint is deprecated: Action is not attached to blueprint anymore. This value is ignored""")
+        if blueprint is not None:
+            pulumi.set(__self__, "blueprint", blueprint)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if github_method is not None:
             pulumi.set(__self__, "github_method", github_method)
         if gitlab_method is not None:
             pulumi.set(__self__, "gitlab_method", gitlab_method)
         if icon is not None:
             pulumi.set(__self__, "icon", icon)
         if kafka_method is not None:
             pulumi.set(__self__, "kafka_method", kafka_method)
-        if order_properties is not None:
-            pulumi.set(__self__, "order_properties", order_properties)
+        if publish is not None:
+            pulumi.set(__self__, "publish", publish)
         if required_approval is not None:
             pulumi.set(__self__, "required_approval", required_approval)
-        if required_jq_query is not None:
-            pulumi.set(__self__, "required_jq_query", required_jq_query)
-        if user_properties is not None:
-            pulumi.set(__self__, "user_properties", user_properties)
+        if self_service_trigger is not None:
+            pulumi.set(__self__, "self_service_trigger", self_service_trigger)
+        if title is not None:
+            pulumi.set(__self__, "title", title)
         if webhook_method is not None:
             pulumi.set(__self__, "webhook_method", webhook_method)
 
     @property
     @pulumi.getter
-    def blueprint(self) -> pulumi.Input[str]:
-        """
-        The blueprint identifier the action relates to
-        """
-        return pulumi.get(self, "blueprint")
-
-    @blueprint.setter
-    def blueprint(self, value: pulumi.Input[str]):
-        pulumi.set(self, "blueprint", value)
-
-    @property
-    @pulumi.getter
     def identifier(self) -> pulumi.Input[str]:
         """
         Identifier
         """
         return pulumi.get(self, "identifier")
 
     @identifier.setter
     def identifier(self, value: pulumi.Input[str]):
         pulumi.set(self, "identifier", value)
 
     @property
-    @pulumi.getter
-    def title(self) -> pulumi.Input[str]:
-        """
-        Title
-        """
-        return pulumi.get(self, "title")
-
-    @title.setter
-    def title(self, value: pulumi.Input[str]):
-        pulumi.set(self, "title", value)
-
-    @property
-    @pulumi.getter
-    def trigger(self) -> pulumi.Input[str]:
-        """
-        The trigger type of the action
-        """
-        return pulumi.get(self, "trigger")
-
-    @trigger.setter
-    def trigger(self, value: pulumi.Input[str]):
-        pulumi.set(self, "trigger", value)
-
-    @property
     @pulumi.getter(name="approvalEmailNotification")
     def approval_email_notification(self) -> Optional[pulumi.Input['ActionApprovalEmailNotificationArgs']]:
         """
         The email notification of the approval
         """
         return pulumi.get(self, "approval_email_notification")
 
@@ -156,51 +118,66 @@
     def approval_webhook_notification(self, value: Optional[pulumi.Input['ActionApprovalWebhookNotificationArgs']]):
         pulumi.set(self, "approval_webhook_notification", value)
 
     @property
     @pulumi.getter(name="azureMethod")
     def azure_method(self) -> Optional[pulumi.Input['ActionAzureMethodArgs']]:
         """
-        The invocation method of the action
+        Azure DevOps invocation method
         """
         return pulumi.get(self, "azure_method")
 
     @azure_method.setter
     def azure_method(self, value: Optional[pulumi.Input['ActionAzureMethodArgs']]):
         pulumi.set(self, "azure_method", value)
 
     @property
     @pulumi.getter
+    def blueprint(self) -> Optional[pulumi.Input[str]]:
+        """
+        The blueprint identifier the action relates to
+        """
+        warnings.warn("""Action is not attached to blueprint anymore. This value is ignored""", DeprecationWarning)
+        pulumi.log.warn("""blueprint is deprecated: Action is not attached to blueprint anymore. This value is ignored""")
+
+        return pulumi.get(self, "blueprint")
+
+    @blueprint.setter
+    def blueprint(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "blueprint", value)
+
+    @property
+    @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
         Description
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter(name="githubMethod")
     def github_method(self) -> Optional[pulumi.Input['ActionGithubMethodArgs']]:
         """
-        The invocation method of the action
+        GitHub invocation method
         """
         return pulumi.get(self, "github_method")
 
     @github_method.setter
     def github_method(self, value: Optional[pulumi.Input['ActionGithubMethodArgs']]):
         pulumi.set(self, "github_method", value)
 
     @property
     @pulumi.getter(name="gitlabMethod")
     def gitlab_method(self) -> Optional[pulumi.Input['ActionGitlabMethodArgs']]:
         """
-        The invocation method of the action
+        Gitlab invocation method
         """
         return pulumi.get(self, "gitlab_method")
 
     @gitlab_method.setter
     def gitlab_method(self, value: Optional[pulumi.Input['ActionGitlabMethodArgs']]):
         pulumi.set(self, "gitlab_method", value)
 
@@ -216,75 +193,75 @@
     def icon(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "icon", value)
 
     @property
     @pulumi.getter(name="kafkaMethod")
     def kafka_method(self) -> Optional[pulumi.Input['ActionKafkaMethodArgs']]:
         """
-        The invocation method of the action
+        Kafka invocation method
         """
         return pulumi.get(self, "kafka_method")
 
     @kafka_method.setter
     def kafka_method(self, value: Optional[pulumi.Input['ActionKafkaMethodArgs']]):
         pulumi.set(self, "kafka_method", value)
 
     @property
-    @pulumi.getter(name="orderProperties")
-    def order_properties(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter
+    def publish(self) -> Optional[pulumi.Input[bool]]:
         """
-        Order properties
+        Publish action
         """
-        return pulumi.get(self, "order_properties")
+        return pulumi.get(self, "publish")
 
-    @order_properties.setter
-    def order_properties(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "order_properties", value)
+    @publish.setter
+    def publish(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "publish", value)
 
     @property
     @pulumi.getter(name="requiredApproval")
     def required_approval(self) -> Optional[pulumi.Input[bool]]:
         """
         Require approval before invoking the action
         """
         return pulumi.get(self, "required_approval")
 
     @required_approval.setter
     def required_approval(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "required_approval", value)
 
     @property
-    @pulumi.getter(name="requiredJqQuery")
-    def required_jq_query(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="selfServiceTrigger")
+    def self_service_trigger(self) -> Optional[pulumi.Input['ActionSelfServiceTriggerArgs']]:
         """
-        The required jq query of the property
+        Self service trigger for the action
         """
-        return pulumi.get(self, "required_jq_query")
+        return pulumi.get(self, "self_service_trigger")
 
-    @required_jq_query.setter
-    def required_jq_query(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "required_jq_query", value)
+    @self_service_trigger.setter
+    def self_service_trigger(self, value: Optional[pulumi.Input['ActionSelfServiceTriggerArgs']]):
+        pulumi.set(self, "self_service_trigger", value)
 
     @property
-    @pulumi.getter(name="userProperties")
-    def user_properties(self) -> Optional[pulumi.Input['ActionUserPropertiesArgs']]:
+    @pulumi.getter
+    def title(self) -> Optional[pulumi.Input[str]]:
         """
-        User properties
+        Title
         """
-        return pulumi.get(self, "user_properties")
+        return pulumi.get(self, "title")
 
-    @user_properties.setter
-    def user_properties(self, value: Optional[pulumi.Input['ActionUserPropertiesArgs']]):
-        pulumi.set(self, "user_properties", value)
+    @title.setter
+    def title(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "title", value)
 
     @property
     @pulumi.getter(name="webhookMethod")
     def webhook_method(self) -> Optional[pulumi.Input['ActionWebhookMethodArgs']]:
         """
-        The invocation method of the action
+        Webhook invocation method
         """
         return pulumi.get(self, "webhook_method")
 
     @webhook_method.setter
     def webhook_method(self, value: Optional[pulumi.Input['ActionWebhookMethodArgs']]):
         pulumi.set(self, "webhook_method", value)
 
@@ -298,73 +275,68 @@
                  blueprint: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  github_method: Optional[pulumi.Input['ActionGithubMethodArgs']] = None,
                  gitlab_method: Optional[pulumi.Input['ActionGitlabMethodArgs']] = None,
                  icon: Optional[pulumi.Input[str]] = None,
                  identifier: Optional[pulumi.Input[str]] = None,
                  kafka_method: Optional[pulumi.Input['ActionKafkaMethodArgs']] = None,
-                 order_properties: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 publish: Optional[pulumi.Input[bool]] = None,
                  required_approval: Optional[pulumi.Input[bool]] = None,
-                 required_jq_query: Optional[pulumi.Input[str]] = None,
+                 self_service_trigger: Optional[pulumi.Input['ActionSelfServiceTriggerArgs']] = None,
                  title: Optional[pulumi.Input[str]] = None,
-                 trigger: Optional[pulumi.Input[str]] = None,
-                 user_properties: Optional[pulumi.Input['ActionUserPropertiesArgs']] = None,
                  webhook_method: Optional[pulumi.Input['ActionWebhookMethodArgs']] = None):
         """
         Input properties used for looking up and filtering Action resources.
         :param pulumi.Input['ActionApprovalEmailNotificationArgs'] approval_email_notification: The email notification of the approval
         :param pulumi.Input['ActionApprovalWebhookNotificationArgs'] approval_webhook_notification: The webhook notification of the approval
-        :param pulumi.Input['ActionAzureMethodArgs'] azure_method: The invocation method of the action
+        :param pulumi.Input['ActionAzureMethodArgs'] azure_method: Azure DevOps invocation method
         :param pulumi.Input[str] blueprint: The blueprint identifier the action relates to
         :param pulumi.Input[str] description: Description
-        :param pulumi.Input['ActionGithubMethodArgs'] github_method: The invocation method of the action
-        :param pulumi.Input['ActionGitlabMethodArgs'] gitlab_method: The invocation method of the action
+        :param pulumi.Input['ActionGithubMethodArgs'] github_method: GitHub invocation method
+        :param pulumi.Input['ActionGitlabMethodArgs'] gitlab_method: Gitlab invocation method
         :param pulumi.Input[str] icon: Icon
         :param pulumi.Input[str] identifier: Identifier
-        :param pulumi.Input['ActionKafkaMethodArgs'] kafka_method: The invocation method of the action
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] order_properties: Order properties
+        :param pulumi.Input['ActionKafkaMethodArgs'] kafka_method: Kafka invocation method
+        :param pulumi.Input[bool] publish: Publish action
         :param pulumi.Input[bool] required_approval: Require approval before invoking the action
-        :param pulumi.Input[str] required_jq_query: The required jq query of the property
+        :param pulumi.Input['ActionSelfServiceTriggerArgs'] self_service_trigger: Self service trigger for the action
         :param pulumi.Input[str] title: Title
-        :param pulumi.Input[str] trigger: The trigger type of the action
-        :param pulumi.Input['ActionUserPropertiesArgs'] user_properties: User properties
-        :param pulumi.Input['ActionWebhookMethodArgs'] webhook_method: The invocation method of the action
+        :param pulumi.Input['ActionWebhookMethodArgs'] webhook_method: Webhook invocation method
         """
         if approval_email_notification is not None:
             pulumi.set(__self__, "approval_email_notification", approval_email_notification)
         if approval_webhook_notification is not None:
             pulumi.set(__self__, "approval_webhook_notification", approval_webhook_notification)
         if azure_method is not None:
             pulumi.set(__self__, "azure_method", azure_method)
         if blueprint is not None:
+            warnings.warn("""Action is not attached to blueprint anymore. This value is ignored""", DeprecationWarning)
+            pulumi.log.warn("""blueprint is deprecated: Action is not attached to blueprint anymore. This value is ignored""")
+        if blueprint is not None:
             pulumi.set(__self__, "blueprint", blueprint)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if github_method is not None:
             pulumi.set(__self__, "github_method", github_method)
         if gitlab_method is not None:
             pulumi.set(__self__, "gitlab_method", gitlab_method)
         if icon is not None:
             pulumi.set(__self__, "icon", icon)
         if identifier is not None:
             pulumi.set(__self__, "identifier", identifier)
         if kafka_method is not None:
             pulumi.set(__self__, "kafka_method", kafka_method)
-        if order_properties is not None:
-            pulumi.set(__self__, "order_properties", order_properties)
+        if publish is not None:
+            pulumi.set(__self__, "publish", publish)
         if required_approval is not None:
             pulumi.set(__self__, "required_approval", required_approval)
-        if required_jq_query is not None:
-            pulumi.set(__self__, "required_jq_query", required_jq_query)
+        if self_service_trigger is not None:
+            pulumi.set(__self__, "self_service_trigger", self_service_trigger)
         if title is not None:
             pulumi.set(__self__, "title", title)
-        if trigger is not None:
-            pulumi.set(__self__, "trigger", trigger)
-        if user_properties is not None:
-            pulumi.set(__self__, "user_properties", user_properties)
         if webhook_method is not None:
             pulumi.set(__self__, "webhook_method", webhook_method)
 
     @property
     @pulumi.getter(name="approvalEmailNotification")
     def approval_email_notification(self) -> Optional[pulumi.Input['ActionApprovalEmailNotificationArgs']]:
         """
@@ -388,28 +360,31 @@
     def approval_webhook_notification(self, value: Optional[pulumi.Input['ActionApprovalWebhookNotificationArgs']]):
         pulumi.set(self, "approval_webhook_notification", value)
 
     @property
     @pulumi.getter(name="azureMethod")
     def azure_method(self) -> Optional[pulumi.Input['ActionAzureMethodArgs']]:
         """
-        The invocation method of the action
+        Azure DevOps invocation method
         """
         return pulumi.get(self, "azure_method")
 
     @azure_method.setter
     def azure_method(self, value: Optional[pulumi.Input['ActionAzureMethodArgs']]):
         pulumi.set(self, "azure_method", value)
 
     @property
     @pulumi.getter
     def blueprint(self) -> Optional[pulumi.Input[str]]:
         """
         The blueprint identifier the action relates to
         """
+        warnings.warn("""Action is not attached to blueprint anymore. This value is ignored""", DeprecationWarning)
+        pulumi.log.warn("""blueprint is deprecated: Action is not attached to blueprint anymore. This value is ignored""")
+
         return pulumi.get(self, "blueprint")
 
     @blueprint.setter
     def blueprint(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "blueprint", value)
 
     @property
@@ -424,27 +399,27 @@
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter(name="githubMethod")
     def github_method(self) -> Optional[pulumi.Input['ActionGithubMethodArgs']]:
         """
-        The invocation method of the action
+        GitHub invocation method
         """
         return pulumi.get(self, "github_method")
 
     @github_method.setter
     def github_method(self, value: Optional[pulumi.Input['ActionGithubMethodArgs']]):
         pulumi.set(self, "github_method", value)
 
     @property
     @pulumi.getter(name="gitlabMethod")
     def gitlab_method(self) -> Optional[pulumi.Input['ActionGitlabMethodArgs']]:
         """
-        The invocation method of the action
+        Gitlab invocation method
         """
         return pulumi.get(self, "gitlab_method")
 
     @gitlab_method.setter
     def gitlab_method(self, value: Optional[pulumi.Input['ActionGitlabMethodArgs']]):
         pulumi.set(self, "gitlab_method", value)
 
@@ -472,99 +447,75 @@
     def identifier(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "identifier", value)
 
     @property
     @pulumi.getter(name="kafkaMethod")
     def kafka_method(self) -> Optional[pulumi.Input['ActionKafkaMethodArgs']]:
         """
-        The invocation method of the action
+        Kafka invocation method
         """
         return pulumi.get(self, "kafka_method")
 
     @kafka_method.setter
     def kafka_method(self, value: Optional[pulumi.Input['ActionKafkaMethodArgs']]):
         pulumi.set(self, "kafka_method", value)
 
     @property
-    @pulumi.getter(name="orderProperties")
-    def order_properties(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter
+    def publish(self) -> Optional[pulumi.Input[bool]]:
         """
-        Order properties
+        Publish action
         """
-        return pulumi.get(self, "order_properties")
+        return pulumi.get(self, "publish")
 
-    @order_properties.setter
-    def order_properties(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "order_properties", value)
+    @publish.setter
+    def publish(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "publish", value)
 
     @property
     @pulumi.getter(name="requiredApproval")
     def required_approval(self) -> Optional[pulumi.Input[bool]]:
         """
         Require approval before invoking the action
         """
         return pulumi.get(self, "required_approval")
 
     @required_approval.setter
     def required_approval(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "required_approval", value)
 
     @property
-    @pulumi.getter(name="requiredJqQuery")
-    def required_jq_query(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="selfServiceTrigger")
+    def self_service_trigger(self) -> Optional[pulumi.Input['ActionSelfServiceTriggerArgs']]:
         """
-        The required jq query of the property
+        Self service trigger for the action
         """
-        return pulumi.get(self, "required_jq_query")
+        return pulumi.get(self, "self_service_trigger")
 
-    @required_jq_query.setter
-    def required_jq_query(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "required_jq_query", value)
+    @self_service_trigger.setter
+    def self_service_trigger(self, value: Optional[pulumi.Input['ActionSelfServiceTriggerArgs']]):
+        pulumi.set(self, "self_service_trigger", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
         """
         Title
         """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
-    @pulumi.getter
-    def trigger(self) -> Optional[pulumi.Input[str]]:
-        """
-        The trigger type of the action
-        """
-        return pulumi.get(self, "trigger")
-
-    @trigger.setter
-    def trigger(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "trigger", value)
-
-    @property
-    @pulumi.getter(name="userProperties")
-    def user_properties(self) -> Optional[pulumi.Input['ActionUserPropertiesArgs']]:
-        """
-        User properties
-        """
-        return pulumi.get(self, "user_properties")
-
-    @user_properties.setter
-    def user_properties(self, value: Optional[pulumi.Input['ActionUserPropertiesArgs']]):
-        pulumi.set(self, "user_properties", value)
-
-    @property
     @pulumi.getter(name="webhookMethod")
     def webhook_method(self) -> Optional[pulumi.Input['ActionWebhookMethodArgs']]:
         """
-        The invocation method of the action
+        Webhook invocation method
         """
         return pulumi.get(self, "webhook_method")
 
     @webhook_method.setter
     def webhook_method(self, value: Optional[pulumi.Input['ActionWebhookMethodArgs']]):
         pulumi.set(self, "webhook_method", value)
 
@@ -580,52 +531,210 @@
                  blueprint: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  github_method: Optional[pulumi.Input[pulumi.InputType['ActionGithubMethodArgs']]] = None,
                  gitlab_method: Optional[pulumi.Input[pulumi.InputType['ActionGitlabMethodArgs']]] = None,
                  icon: Optional[pulumi.Input[str]] = None,
                  identifier: Optional[pulumi.Input[str]] = None,
                  kafka_method: Optional[pulumi.Input[pulumi.InputType['ActionKafkaMethodArgs']]] = None,
-                 order_properties: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 publish: Optional[pulumi.Input[bool]] = None,
                  required_approval: Optional[pulumi.Input[bool]] = None,
-                 required_jq_query: Optional[pulumi.Input[str]] = None,
+                 self_service_trigger: Optional[pulumi.Input[pulumi.InputType['ActionSelfServiceTriggerArgs']]] = None,
                  title: Optional[pulumi.Input[str]] = None,
-                 trigger: Optional[pulumi.Input[str]] = None,
-                 user_properties: Optional[pulumi.Input[pulumi.InputType['ActionUserPropertiesArgs']]] = None,
                  webhook_method: Optional[pulumi.Input[pulumi.InputType['ActionWebhookMethodArgs']]] = None,
                  __props__=None):
         """
-        Create a Action resource with the given unique name, props, and options.
+        Docs for the Action resource can be found [here](https://docs.getport.io/create-self-service-experiences/).
+
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import json
+        import pulumi_port as port
+
+        create_microservice = port.index.Port_action("createMicroservice",
+            title=Create Microservice,
+            identifier=create-microservice,
+            icon=Terraform,
+            self_service_trigger={
+                operation: CREATE,
+                blueprintIdentifier: port_blueprint.microservice.identifier,
+                userProperties: {
+                    stringProps: {
+                        myStringIdentifier: {
+                            title: My String Identifier,
+                            required: True,
+                            format: entity,
+                            blueprint: port_blueprint.parent.identifier,
+                            dataset: {
+                                combinator: and,
+                                rules: [{
+                                    property: $title,
+                                    operator: contains,
+                                    value: {
+                                        jqQuery: "specificValue",
+                                    },
+                                }],
+                            },
+                        },
+                    },
+                    numberProps: {
+                        myNumberIdentifier: {
+                            title: My Number Identifier,
+                            required: True,
+                            maximum: 100,
+                            minimum: 0,
+                        },
+                    },
+                    booleanProps: {
+                        myBooleanIdentifier: {
+                            title: My Boolean Identifier,
+                            required: True,
+                        },
+                    },
+                    objectProps: {
+                        myObjectIdentifier: {
+                            title: My Object Identifier,
+                            required: True,
+                        },
+                    },
+                    arrayProps: {
+                        myArrayIdentifier: {
+                            title: My Array Identifier,
+                            required: True,
+                            stringItems: {
+                                format: entity,
+                                blueprint: port_blueprint.parent.identifier,
+                                dataset: json.dumps({
+                                    combinator: and,
+                                    rules: [{
+                                        property: $title,
+                                        operator: contains,
+                                        value: specificValue,
+                                    }],
+                                }),
+                            },
+                        },
+                    },
+                },
+            },
+            kafka_method={
+                payload: json.dumps({
+                    runId: {{.run.id}},
+                }),
+            })
+        ```
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['ActionApprovalEmailNotificationArgs']] approval_email_notification: The email notification of the approval
         :param pulumi.Input[pulumi.InputType['ActionApprovalWebhookNotificationArgs']] approval_webhook_notification: The webhook notification of the approval
-        :param pulumi.Input[pulumi.InputType['ActionAzureMethodArgs']] azure_method: The invocation method of the action
+        :param pulumi.Input[pulumi.InputType['ActionAzureMethodArgs']] azure_method: Azure DevOps invocation method
         :param pulumi.Input[str] blueprint: The blueprint identifier the action relates to
         :param pulumi.Input[str] description: Description
-        :param pulumi.Input[pulumi.InputType['ActionGithubMethodArgs']] github_method: The invocation method of the action
-        :param pulumi.Input[pulumi.InputType['ActionGitlabMethodArgs']] gitlab_method: The invocation method of the action
+        :param pulumi.Input[pulumi.InputType['ActionGithubMethodArgs']] github_method: GitHub invocation method
+        :param pulumi.Input[pulumi.InputType['ActionGitlabMethodArgs']] gitlab_method: Gitlab invocation method
         :param pulumi.Input[str] icon: Icon
         :param pulumi.Input[str] identifier: Identifier
-        :param pulumi.Input[pulumi.InputType['ActionKafkaMethodArgs']] kafka_method: The invocation method of the action
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] order_properties: Order properties
+        :param pulumi.Input[pulumi.InputType['ActionKafkaMethodArgs']] kafka_method: Kafka invocation method
+        :param pulumi.Input[bool] publish: Publish action
         :param pulumi.Input[bool] required_approval: Require approval before invoking the action
-        :param pulumi.Input[str] required_jq_query: The required jq query of the property
+        :param pulumi.Input[pulumi.InputType['ActionSelfServiceTriggerArgs']] self_service_trigger: Self service trigger for the action
         :param pulumi.Input[str] title: Title
-        :param pulumi.Input[str] trigger: The trigger type of the action
-        :param pulumi.Input[pulumi.InputType['ActionUserPropertiesArgs']] user_properties: User properties
-        :param pulumi.Input[pulumi.InputType['ActionWebhookMethodArgs']] webhook_method: The invocation method of the action
+        :param pulumi.Input[pulumi.InputType['ActionWebhookMethodArgs']] webhook_method: Webhook invocation method
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ActionArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a Action resource with the given unique name, props, and options.
+        Docs for the Action resource can be found [here](https://docs.getport.io/create-self-service-experiences/).
+
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import json
+        import pulumi_port as port
+
+        create_microservice = port.index.Port_action("createMicroservice",
+            title=Create Microservice,
+            identifier=create-microservice,
+            icon=Terraform,
+            self_service_trigger={
+                operation: CREATE,
+                blueprintIdentifier: port_blueprint.microservice.identifier,
+                userProperties: {
+                    stringProps: {
+                        myStringIdentifier: {
+                            title: My String Identifier,
+                            required: True,
+                            format: entity,
+                            blueprint: port_blueprint.parent.identifier,
+                            dataset: {
+                                combinator: and,
+                                rules: [{
+                                    property: $title,
+                                    operator: contains,
+                                    value: {
+                                        jqQuery: "specificValue",
+                                    },
+                                }],
+                            },
+                        },
+                    },
+                    numberProps: {
+                        myNumberIdentifier: {
+                            title: My Number Identifier,
+                            required: True,
+                            maximum: 100,
+                            minimum: 0,
+                        },
+                    },
+                    booleanProps: {
+                        myBooleanIdentifier: {
+                            title: My Boolean Identifier,
+                            required: True,
+                        },
+                    },
+                    objectProps: {
+                        myObjectIdentifier: {
+                            title: My Object Identifier,
+                            required: True,
+                        },
+                    },
+                    arrayProps: {
+                        myArrayIdentifier: {
+                            title: My Array Identifier,
+                            required: True,
+                            stringItems: {
+                                format: entity,
+                                blueprint: port_blueprint.parent.identifier,
+                                dataset: json.dumps({
+                                    combinator: and,
+                                    rules: [{
+                                        property: $title,
+                                        operator: contains,
+                                        value: specificValue,
+                                    }],
+                                }),
+                            },
+                        },
+                    },
+                },
+            },
+            kafka_method={
+                payload: json.dumps({
+                    runId: {{.run.id}},
+                }),
+            })
+        ```
+
         :param str resource_name: The name of the resource.
         :param ActionArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(ActionArgs, pulumi.ResourceOptions, *args, **kwargs)
@@ -643,54 +752,44 @@
                  blueprint: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  github_method: Optional[pulumi.Input[pulumi.InputType['ActionGithubMethodArgs']]] = None,
                  gitlab_method: Optional[pulumi.Input[pulumi.InputType['ActionGitlabMethodArgs']]] = None,
                  icon: Optional[pulumi.Input[str]] = None,
                  identifier: Optional[pulumi.Input[str]] = None,
                  kafka_method: Optional[pulumi.Input[pulumi.InputType['ActionKafkaMethodArgs']]] = None,
-                 order_properties: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 publish: Optional[pulumi.Input[bool]] = None,
                  required_approval: Optional[pulumi.Input[bool]] = None,
-                 required_jq_query: Optional[pulumi.Input[str]] = None,
+                 self_service_trigger: Optional[pulumi.Input[pulumi.InputType['ActionSelfServiceTriggerArgs']]] = None,
                  title: Optional[pulumi.Input[str]] = None,
-                 trigger: Optional[pulumi.Input[str]] = None,
-                 user_properties: Optional[pulumi.Input[pulumi.InputType['ActionUserPropertiesArgs']]] = None,
                  webhook_method: Optional[pulumi.Input[pulumi.InputType['ActionWebhookMethodArgs']]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ActionArgs.__new__(ActionArgs)
 
             __props__.__dict__["approval_email_notification"] = approval_email_notification
             __props__.__dict__["approval_webhook_notification"] = approval_webhook_notification
             __props__.__dict__["azure_method"] = azure_method
-            if blueprint is None and not opts.urn:
-                raise TypeError("Missing required property 'blueprint'")
             __props__.__dict__["blueprint"] = blueprint
             __props__.__dict__["description"] = description
             __props__.__dict__["github_method"] = github_method
             __props__.__dict__["gitlab_method"] = gitlab_method
             __props__.__dict__["icon"] = icon
             if identifier is None and not opts.urn:
                 raise TypeError("Missing required property 'identifier'")
             __props__.__dict__["identifier"] = identifier
             __props__.__dict__["kafka_method"] = kafka_method
-            __props__.__dict__["order_properties"] = order_properties
+            __props__.__dict__["publish"] = publish
             __props__.__dict__["required_approval"] = required_approval
-            __props__.__dict__["required_jq_query"] = required_jq_query
-            if title is None and not opts.urn:
-                raise TypeError("Missing required property 'title'")
+            __props__.__dict__["self_service_trigger"] = self_service_trigger
             __props__.__dict__["title"] = title
-            if trigger is None and not opts.urn:
-                raise TypeError("Missing required property 'trigger'")
-            __props__.__dict__["trigger"] = trigger
-            __props__.__dict__["user_properties"] = user_properties
             __props__.__dict__["webhook_method"] = webhook_method
         super(Action, __self__).__init__(
             'port:index/action:Action',
             resource_name,
             __props__,
             opts)
 
@@ -704,45 +803,41 @@
             blueprint: Optional[pulumi.Input[str]] = None,
             description: Optional[pulumi.Input[str]] = None,
             github_method: Optional[pulumi.Input[pulumi.InputType['ActionGithubMethodArgs']]] = None,
             gitlab_method: Optional[pulumi.Input[pulumi.InputType['ActionGitlabMethodArgs']]] = None,
             icon: Optional[pulumi.Input[str]] = None,
             identifier: Optional[pulumi.Input[str]] = None,
             kafka_method: Optional[pulumi.Input[pulumi.InputType['ActionKafkaMethodArgs']]] = None,
-            order_properties: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            publish: Optional[pulumi.Input[bool]] = None,
             required_approval: Optional[pulumi.Input[bool]] = None,
-            required_jq_query: Optional[pulumi.Input[str]] = None,
+            self_service_trigger: Optional[pulumi.Input[pulumi.InputType['ActionSelfServiceTriggerArgs']]] = None,
             title: Optional[pulumi.Input[str]] = None,
-            trigger: Optional[pulumi.Input[str]] = None,
-            user_properties: Optional[pulumi.Input[pulumi.InputType['ActionUserPropertiesArgs']]] = None,
             webhook_method: Optional[pulumi.Input[pulumi.InputType['ActionWebhookMethodArgs']]] = None) -> 'Action':
         """
         Get an existing Action resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['ActionApprovalEmailNotificationArgs']] approval_email_notification: The email notification of the approval
         :param pulumi.Input[pulumi.InputType['ActionApprovalWebhookNotificationArgs']] approval_webhook_notification: The webhook notification of the approval
-        :param pulumi.Input[pulumi.InputType['ActionAzureMethodArgs']] azure_method: The invocation method of the action
+        :param pulumi.Input[pulumi.InputType['ActionAzureMethodArgs']] azure_method: Azure DevOps invocation method
         :param pulumi.Input[str] blueprint: The blueprint identifier the action relates to
         :param pulumi.Input[str] description: Description
-        :param pulumi.Input[pulumi.InputType['ActionGithubMethodArgs']] github_method: The invocation method of the action
-        :param pulumi.Input[pulumi.InputType['ActionGitlabMethodArgs']] gitlab_method: The invocation method of the action
+        :param pulumi.Input[pulumi.InputType['ActionGithubMethodArgs']] github_method: GitHub invocation method
+        :param pulumi.Input[pulumi.InputType['ActionGitlabMethodArgs']] gitlab_method: Gitlab invocation method
         :param pulumi.Input[str] icon: Icon
         :param pulumi.Input[str] identifier: Identifier
-        :param pulumi.Input[pulumi.InputType['ActionKafkaMethodArgs']] kafka_method: The invocation method of the action
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] order_properties: Order properties
+        :param pulumi.Input[pulumi.InputType['ActionKafkaMethodArgs']] kafka_method: Kafka invocation method
+        :param pulumi.Input[bool] publish: Publish action
         :param pulumi.Input[bool] required_approval: Require approval before invoking the action
-        :param pulumi.Input[str] required_jq_query: The required jq query of the property
+        :param pulumi.Input[pulumi.InputType['ActionSelfServiceTriggerArgs']] self_service_trigger: Self service trigger for the action
         :param pulumi.Input[str] title: Title
-        :param pulumi.Input[str] trigger: The trigger type of the action
-        :param pulumi.Input[pulumi.InputType['ActionUserPropertiesArgs']] user_properties: User properties
-        :param pulumi.Input[pulumi.InputType['ActionWebhookMethodArgs']] webhook_method: The invocation method of the action
+        :param pulumi.Input[pulumi.InputType['ActionWebhookMethodArgs']] webhook_method: Webhook invocation method
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ActionState.__new__(_ActionState)
 
         __props__.__dict__["approval_email_notification"] = approval_email_notification
         __props__.__dict__["approval_webhook_notification"] = approval_webhook_notification
@@ -750,20 +845,18 @@
         __props__.__dict__["blueprint"] = blueprint
         __props__.__dict__["description"] = description
         __props__.__dict__["github_method"] = github_method
         __props__.__dict__["gitlab_method"] = gitlab_method
         __props__.__dict__["icon"] = icon
         __props__.__dict__["identifier"] = identifier
         __props__.__dict__["kafka_method"] = kafka_method
-        __props__.__dict__["order_properties"] = order_properties
+        __props__.__dict__["publish"] = publish
         __props__.__dict__["required_approval"] = required_approval
-        __props__.__dict__["required_jq_query"] = required_jq_query
+        __props__.__dict__["self_service_trigger"] = self_service_trigger
         __props__.__dict__["title"] = title
-        __props__.__dict__["trigger"] = trigger
-        __props__.__dict__["user_properties"] = user_properties
         __props__.__dict__["webhook_method"] = webhook_method
         return Action(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="approvalEmailNotification")
     def approval_email_notification(self) -> pulumi.Output[Optional['outputs.ActionApprovalEmailNotification']]:
         """
@@ -779,47 +872,50 @@
         """
         return pulumi.get(self, "approval_webhook_notification")
 
     @property
     @pulumi.getter(name="azureMethod")
     def azure_method(self) -> pulumi.Output[Optional['outputs.ActionAzureMethod']]:
         """
-        The invocation method of the action
+        Azure DevOps invocation method
         """
         return pulumi.get(self, "azure_method")
 
     @property
     @pulumi.getter
-    def blueprint(self) -> pulumi.Output[str]:
+    def blueprint(self) -> pulumi.Output[Optional[str]]:
         """
         The blueprint identifier the action relates to
         """
+        warnings.warn("""Action is not attached to blueprint anymore. This value is ignored""", DeprecationWarning)
+        pulumi.log.warn("""blueprint is deprecated: Action is not attached to blueprint anymore. This value is ignored""")
+
         return pulumi.get(self, "blueprint")
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Output[Optional[str]]:
         """
         Description
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter(name="githubMethod")
     def github_method(self) -> pulumi.Output[Optional['outputs.ActionGithubMethod']]:
         """
-        The invocation method of the action
+        GitHub invocation method
         """
         return pulumi.get(self, "github_method")
 
     @property
     @pulumi.getter(name="gitlabMethod")
     def gitlab_method(self) -> pulumi.Output[Optional['outputs.ActionGitlabMethod']]:
         """
-        The invocation method of the action
+        Gitlab invocation method
         """
         return pulumi.get(self, "gitlab_method")
 
     @property
     @pulumi.getter
     def icon(self) -> pulumi.Output[Optional[str]]:
         """
@@ -835,67 +931,51 @@
         """
         return pulumi.get(self, "identifier")
 
     @property
     @pulumi.getter(name="kafkaMethod")
     def kafka_method(self) -> pulumi.Output[Optional['outputs.ActionKafkaMethod']]:
         """
-        The invocation method of the action
+        Kafka invocation method
         """
         return pulumi.get(self, "kafka_method")
 
     @property
-    @pulumi.getter(name="orderProperties")
-    def order_properties(self) -> pulumi.Output[Optional[Sequence[str]]]:
+    @pulumi.getter
+    def publish(self) -> pulumi.Output[bool]:
         """
-        Order properties
+        Publish action
         """
-        return pulumi.get(self, "order_properties")
+        return pulumi.get(self, "publish")
 
     @property
     @pulumi.getter(name="requiredApproval")
     def required_approval(self) -> pulumi.Output[Optional[bool]]:
         """
         Require approval before invoking the action
         """
         return pulumi.get(self, "required_approval")
 
     @property
-    @pulumi.getter(name="requiredJqQuery")
-    def required_jq_query(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="selfServiceTrigger")
+    def self_service_trigger(self) -> pulumi.Output[Optional['outputs.ActionSelfServiceTrigger']]:
         """
-        The required jq query of the property
+        Self service trigger for the action
         """
-        return pulumi.get(self, "required_jq_query")
+        return pulumi.get(self, "self_service_trigger")
 
     @property
     @pulumi.getter
-    def title(self) -> pulumi.Output[str]:
+    def title(self) -> pulumi.Output[Optional[str]]:
         """
         Title
         """
         return pulumi.get(self, "title")
 
     @property
-    @pulumi.getter
-    def trigger(self) -> pulumi.Output[str]:
-        """
-        The trigger type of the action
-        """
-        return pulumi.get(self, "trigger")
-
-    @property
-    @pulumi.getter(name="userProperties")
-    def user_properties(self) -> pulumi.Output[Optional['outputs.ActionUserProperties']]:
-        """
-        User properties
-        """
-        return pulumi.get(self, "user_properties")
-
-    @property
     @pulumi.getter(name="webhookMethod")
     def webhook_method(self) -> pulumi.Output[Optional['outputs.ActionWebhookMethod']]:
         """
-        The invocation method of the action
+        Webhook invocation method
         """
         return pulumi.get(self, "webhook_method")
```

### Comparing `port_pulumi-1.9.1/port_pulumi/action_permissions.py` & `port_pulumi-2.0.0/port_pulumi/action_permissions.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,63 +13,69 @@
 
 __all__ = ['ActionPermissionsArgs', 'ActionPermissions']
 
 @pulumi.input_type
 class ActionPermissionsArgs:
     def __init__(__self__, *,
                  action_identifier: pulumi.Input[str],
-                 blueprint_identifier: pulumi.Input[str],
-                 permissions: Optional[pulumi.Input['ActionPermissionsPermissionsArgs']] = None):
+                 permissions: pulumi.Input['ActionPermissionsPermissionsArgs'],
+                 blueprint_identifier: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a ActionPermissions resource.
         :param pulumi.Input[str] action_identifier: The ID of the action
-        :param pulumi.Input[str] blueprint_identifier: The ID of the blueprint
         :param pulumi.Input['ActionPermissionsPermissionsArgs'] permissions: The permissions for the action
+        :param pulumi.Input[str] blueprint_identifier: The ID of the blueprint
         """
         pulumi.set(__self__, "action_identifier", action_identifier)
-        pulumi.set(__self__, "blueprint_identifier", blueprint_identifier)
-        if permissions is not None:
-            pulumi.set(__self__, "permissions", permissions)
+        pulumi.set(__self__, "permissions", permissions)
+        if blueprint_identifier is not None:
+            warnings.warn("""Action is not attached to blueprint anymore. This value is ignored""", DeprecationWarning)
+            pulumi.log.warn("""blueprint_identifier is deprecated: Action is not attached to blueprint anymore. This value is ignored""")
+        if blueprint_identifier is not None:
+            pulumi.set(__self__, "blueprint_identifier", blueprint_identifier)
 
     @property
     @pulumi.getter(name="actionIdentifier")
     def action_identifier(self) -> pulumi.Input[str]:
         """
         The ID of the action
         """
         return pulumi.get(self, "action_identifier")
 
     @action_identifier.setter
     def action_identifier(self, value: pulumi.Input[str]):
         pulumi.set(self, "action_identifier", value)
 
     @property
-    @pulumi.getter(name="blueprintIdentifier")
-    def blueprint_identifier(self) -> pulumi.Input[str]:
-        """
-        The ID of the blueprint
-        """
-        return pulumi.get(self, "blueprint_identifier")
-
-    @blueprint_identifier.setter
-    def blueprint_identifier(self, value: pulumi.Input[str]):
-        pulumi.set(self, "blueprint_identifier", value)
-
-    @property
     @pulumi.getter
-    def permissions(self) -> Optional[pulumi.Input['ActionPermissionsPermissionsArgs']]:
+    def permissions(self) -> pulumi.Input['ActionPermissionsPermissionsArgs']:
         """
         The permissions for the action
         """
         return pulumi.get(self, "permissions")
 
     @permissions.setter
-    def permissions(self, value: Optional[pulumi.Input['ActionPermissionsPermissionsArgs']]):
+    def permissions(self, value: pulumi.Input['ActionPermissionsPermissionsArgs']):
         pulumi.set(self, "permissions", value)
 
+    @property
+    @pulumi.getter(name="blueprintIdentifier")
+    def blueprint_identifier(self) -> Optional[pulumi.Input[str]]:
+        """
+        The ID of the blueprint
+        """
+        warnings.warn("""Action is not attached to blueprint anymore. This value is ignored""", DeprecationWarning)
+        pulumi.log.warn("""blueprint_identifier is deprecated: Action is not attached to blueprint anymore. This value is ignored""")
+
+        return pulumi.get(self, "blueprint_identifier")
+
+    @blueprint_identifier.setter
+    def blueprint_identifier(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "blueprint_identifier", value)
+
 
 @pulumi.input_type
 class _ActionPermissionsState:
     def __init__(__self__, *,
                  action_identifier: Optional[pulumi.Input[str]] = None,
                  blueprint_identifier: Optional[pulumi.Input[str]] = None,
                  permissions: Optional[pulumi.Input['ActionPermissionsPermissionsArgs']] = None):
@@ -78,14 +84,17 @@
         :param pulumi.Input[str] action_identifier: The ID of the action
         :param pulumi.Input[str] blueprint_identifier: The ID of the blueprint
         :param pulumi.Input['ActionPermissionsPermissionsArgs'] permissions: The permissions for the action
         """
         if action_identifier is not None:
             pulumi.set(__self__, "action_identifier", action_identifier)
         if blueprint_identifier is not None:
+            warnings.warn("""Action is not attached to blueprint anymore. This value is ignored""", DeprecationWarning)
+            pulumi.log.warn("""blueprint_identifier is deprecated: Action is not attached to blueprint anymore. This value is ignored""")
+        if blueprint_identifier is not None:
             pulumi.set(__self__, "blueprint_identifier", blueprint_identifier)
         if permissions is not None:
             pulumi.set(__self__, "permissions", permissions)
 
     @property
     @pulumi.getter(name="actionIdentifier")
     def action_identifier(self) -> Optional[pulumi.Input[str]]:
@@ -100,14 +109,17 @@
 
     @property
     @pulumi.getter(name="blueprintIdentifier")
     def blueprint_identifier(self) -> Optional[pulumi.Input[str]]:
         """
         The ID of the blueprint
         """
+        warnings.warn("""Action is not attached to blueprint anymore. This value is ignored""", DeprecationWarning)
+        pulumi.log.warn("""blueprint_identifier is deprecated: Action is not attached to blueprint anymore. This value is ignored""")
+
         return pulumi.get(self, "blueprint_identifier")
 
     @blueprint_identifier.setter
     def blueprint_identifier(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "blueprint_identifier", value)
 
     @property
@@ -174,17 +186,17 @@
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ActionPermissionsArgs.__new__(ActionPermissionsArgs)
 
             if action_identifier is None and not opts.urn:
                 raise TypeError("Missing required property 'action_identifier'")
             __props__.__dict__["action_identifier"] = action_identifier
-            if blueprint_identifier is None and not opts.urn:
-                raise TypeError("Missing required property 'blueprint_identifier'")
             __props__.__dict__["blueprint_identifier"] = blueprint_identifier
+            if permissions is None and not opts.urn:
+                raise TypeError("Missing required property 'permissions'")
             __props__.__dict__["permissions"] = permissions
         super(ActionPermissions, __self__).__init__(
             'port:index/actionPermissions:ActionPermissions',
             resource_name,
             __props__,
             opts)
 
@@ -221,21 +233,24 @@
         """
         The ID of the action
         """
         return pulumi.get(self, "action_identifier")
 
     @property
     @pulumi.getter(name="blueprintIdentifier")
-    def blueprint_identifier(self) -> pulumi.Output[str]:
+    def blueprint_identifier(self) -> pulumi.Output[Optional[str]]:
         """
         The ID of the blueprint
         """
+        warnings.warn("""Action is not attached to blueprint anymore. This value is ignored""", DeprecationWarning)
+        pulumi.log.warn("""blueprint_identifier is deprecated: Action is not attached to blueprint anymore. This value is ignored""")
+
         return pulumi.get(self, "blueprint_identifier")
 
     @property
     @pulumi.getter
-    def permissions(self) -> pulumi.Output[Optional['outputs.ActionPermissionsPermissions']]:
+    def permissions(self) -> pulumi.Output['outputs.ActionPermissionsPermissions']:
         """
         The permissions for the action
         """
         return pulumi.get(self, "permissions")
```

### Comparing `port_pulumi-1.9.1/port_pulumi/aggregation_property.py` & `port_pulumi-2.0.0/port_pulumi/aggregation_property.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.9.1/port_pulumi/blueprint.py` & `port_pulumi-2.0.0/port_pulumi/blueprint.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 @pulumi.input_type
 class BlueprintArgs:
     def __init__(__self__, *,
                  identifier: pulumi.Input[str],
                  title: pulumi.Input[str],
                  calculation_properties: Optional[pulumi.Input[Mapping[str, pulumi.Input['BlueprintCalculationPropertiesArgs']]]] = None,
                  description: Optional[pulumi.Input[str]] = None,
+                 force_delete_entities: Optional[pulumi.Input[bool]] = None,
                  icon: Optional[pulumi.Input[str]] = None,
                  kafka_changelog_destination: Optional[pulumi.Input['BlueprintKafkaChangelogDestinationArgs']] = None,
                  mirror_properties: Optional[pulumi.Input[Mapping[str, pulumi.Input['BlueprintMirrorPropertiesArgs']]]] = None,
                  properties: Optional[pulumi.Input['BlueprintPropertiesArgs']] = None,
                  relations: Optional[pulumi.Input[Mapping[str, pulumi.Input['BlueprintRelationsArgs']]]] = None,
                  team_inheritance: Optional[pulumi.Input['BlueprintTeamInheritanceArgs']] = None,
                  webhook_changelog_destination: Optional[pulumi.Input['BlueprintWebhookChangelogDestinationArgs']] = None):
@@ -43,14 +44,16 @@
         """
         pulumi.set(__self__, "identifier", identifier)
         pulumi.set(__self__, "title", title)
         if calculation_properties is not None:
             pulumi.set(__self__, "calculation_properties", calculation_properties)
         if description is not None:
             pulumi.set(__self__, "description", description)
+        if force_delete_entities is not None:
+            pulumi.set(__self__, "force_delete_entities", force_delete_entities)
         if icon is not None:
             pulumi.set(__self__, "icon", icon)
         if kafka_changelog_destination is not None:
             pulumi.set(__self__, "kafka_changelog_destination", kafka_changelog_destination)
         if mirror_properties is not None:
             pulumi.set(__self__, "mirror_properties", mirror_properties)
         if properties is not None:
@@ -107,14 +110,23 @@
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
+    @pulumi.getter(name="forceDeleteEntities")
+    def force_delete_entities(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "force_delete_entities")
+
+    @force_delete_entities.setter
+    def force_delete_entities(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "force_delete_entities", value)
+
+    @property
     @pulumi.getter
     def icon(self) -> Optional[pulumi.Input[str]]:
         """
         The icon of the blueprint
         """
         return pulumi.get(self, "icon")
 
@@ -198,14 +210,15 @@
 @pulumi.input_type
 class _BlueprintState:
     def __init__(__self__, *,
                  calculation_properties: Optional[pulumi.Input[Mapping[str, pulumi.Input['BlueprintCalculationPropertiesArgs']]]] = None,
                  created_at: Optional[pulumi.Input[str]] = None,
                  created_by: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
+                 force_delete_entities: Optional[pulumi.Input[bool]] = None,
                  icon: Optional[pulumi.Input[str]] = None,
                  identifier: Optional[pulumi.Input[str]] = None,
                  kafka_changelog_destination: Optional[pulumi.Input['BlueprintKafkaChangelogDestinationArgs']] = None,
                  mirror_properties: Optional[pulumi.Input[Mapping[str, pulumi.Input['BlueprintMirrorPropertiesArgs']]]] = None,
                  properties: Optional[pulumi.Input['BlueprintPropertiesArgs']] = None,
                  relations: Optional[pulumi.Input[Mapping[str, pulumi.Input['BlueprintRelationsArgs']]]] = None,
                  team_inheritance: Optional[pulumi.Input['BlueprintTeamInheritanceArgs']] = None,
@@ -235,14 +248,16 @@
             pulumi.set(__self__, "calculation_properties", calculation_properties)
         if created_at is not None:
             pulumi.set(__self__, "created_at", created_at)
         if created_by is not None:
             pulumi.set(__self__, "created_by", created_by)
         if description is not None:
             pulumi.set(__self__, "description", description)
+        if force_delete_entities is not None:
+            pulumi.set(__self__, "force_delete_entities", force_delete_entities)
         if icon is not None:
             pulumi.set(__self__, "icon", icon)
         if identifier is not None:
             pulumi.set(__self__, "identifier", identifier)
         if kafka_changelog_destination is not None:
             pulumi.set(__self__, "kafka_changelog_destination", kafka_changelog_destination)
         if mirror_properties is not None:
@@ -307,14 +322,23 @@
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
+    @pulumi.getter(name="forceDeleteEntities")
+    def force_delete_entities(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "force_delete_entities")
+
+    @force_delete_entities.setter
+    def force_delete_entities(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "force_delete_entities", value)
+
+    @property
     @pulumi.getter
     def icon(self) -> Optional[pulumi.Input[str]]:
         """
         The icon of the blueprint
         """
         return pulumi.get(self, "icon")
 
@@ -446,14 +470,15 @@
 class Blueprint(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  calculation_properties: Optional[pulumi.Input[Mapping[str, pulumi.Input[pulumi.InputType['BlueprintCalculationPropertiesArgs']]]]] = None,
                  description: Optional[pulumi.Input[str]] = None,
+                 force_delete_entities: Optional[pulumi.Input[bool]] = None,
                  icon: Optional[pulumi.Input[str]] = None,
                  identifier: Optional[pulumi.Input[str]] = None,
                  kafka_changelog_destination: Optional[pulumi.Input[pulumi.InputType['BlueprintKafkaChangelogDestinationArgs']]] = None,
                  mirror_properties: Optional[pulumi.Input[Mapping[str, pulumi.Input[pulumi.InputType['BlueprintMirrorPropertiesArgs']]]]] = None,
                  properties: Optional[pulumi.Input[pulumi.InputType['BlueprintPropertiesArgs']]] = None,
                  relations: Optional[pulumi.Input[Mapping[str, pulumi.Input[pulumi.InputType['BlueprintRelationsArgs']]]]] = None,
                  team_inheritance: Optional[pulumi.Input[pulumi.InputType['BlueprintTeamInheritanceArgs']]] = None,
@@ -497,14 +522,15 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  calculation_properties: Optional[pulumi.Input[Mapping[str, pulumi.Input[pulumi.InputType['BlueprintCalculationPropertiesArgs']]]]] = None,
                  description: Optional[pulumi.Input[str]] = None,
+                 force_delete_entities: Optional[pulumi.Input[bool]] = None,
                  icon: Optional[pulumi.Input[str]] = None,
                  identifier: Optional[pulumi.Input[str]] = None,
                  kafka_changelog_destination: Optional[pulumi.Input[pulumi.InputType['BlueprintKafkaChangelogDestinationArgs']]] = None,
                  mirror_properties: Optional[pulumi.Input[Mapping[str, pulumi.Input[pulumi.InputType['BlueprintMirrorPropertiesArgs']]]]] = None,
                  properties: Optional[pulumi.Input[pulumi.InputType['BlueprintPropertiesArgs']]] = None,
                  relations: Optional[pulumi.Input[Mapping[str, pulumi.Input[pulumi.InputType['BlueprintRelationsArgs']]]]] = None,
                  team_inheritance: Optional[pulumi.Input[pulumi.InputType['BlueprintTeamInheritanceArgs']]] = None,
@@ -517,14 +543,15 @@
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = BlueprintArgs.__new__(BlueprintArgs)
 
             __props__.__dict__["calculation_properties"] = calculation_properties
             __props__.__dict__["description"] = description
+            __props__.__dict__["force_delete_entities"] = force_delete_entities
             __props__.__dict__["icon"] = icon
             if identifier is None and not opts.urn:
                 raise TypeError("Missing required property 'identifier'")
             __props__.__dict__["identifier"] = identifier
             __props__.__dict__["kafka_changelog_destination"] = kafka_changelog_destination
             __props__.__dict__["mirror_properties"] = mirror_properties
             __props__.__dict__["properties"] = properties
@@ -548,14 +575,15 @@
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             calculation_properties: Optional[pulumi.Input[Mapping[str, pulumi.Input[pulumi.InputType['BlueprintCalculationPropertiesArgs']]]]] = None,
             created_at: Optional[pulumi.Input[str]] = None,
             created_by: Optional[pulumi.Input[str]] = None,
             description: Optional[pulumi.Input[str]] = None,
+            force_delete_entities: Optional[pulumi.Input[bool]] = None,
             icon: Optional[pulumi.Input[str]] = None,
             identifier: Optional[pulumi.Input[str]] = None,
             kafka_changelog_destination: Optional[pulumi.Input[pulumi.InputType['BlueprintKafkaChangelogDestinationArgs']]] = None,
             mirror_properties: Optional[pulumi.Input[Mapping[str, pulumi.Input[pulumi.InputType['BlueprintMirrorPropertiesArgs']]]]] = None,
             properties: Optional[pulumi.Input[pulumi.InputType['BlueprintPropertiesArgs']]] = None,
             relations: Optional[pulumi.Input[Mapping[str, pulumi.Input[pulumi.InputType['BlueprintRelationsArgs']]]]] = None,
             team_inheritance: Optional[pulumi.Input[pulumi.InputType['BlueprintTeamInheritanceArgs']]] = None,
@@ -590,14 +618,15 @@
 
         __props__ = _BlueprintState.__new__(_BlueprintState)
 
         __props__.__dict__["calculation_properties"] = calculation_properties
         __props__.__dict__["created_at"] = created_at
         __props__.__dict__["created_by"] = created_by
         __props__.__dict__["description"] = description
+        __props__.__dict__["force_delete_entities"] = force_delete_entities
         __props__.__dict__["icon"] = icon
         __props__.__dict__["identifier"] = identifier
         __props__.__dict__["kafka_changelog_destination"] = kafka_changelog_destination
         __props__.__dict__["mirror_properties"] = mirror_properties
         __props__.__dict__["properties"] = properties
         __props__.__dict__["relations"] = relations
         __props__.__dict__["team_inheritance"] = team_inheritance
@@ -636,14 +665,19 @@
     def description(self) -> pulumi.Output[Optional[str]]:
         """
         The description of the blueprint
         """
         return pulumi.get(self, "description")
 
     @property
+    @pulumi.getter(name="forceDeleteEntities")
+    def force_delete_entities(self) -> pulumi.Output[bool]:
+        return pulumi.get(self, "force_delete_entities")
+
+    @property
     @pulumi.getter
     def icon(self) -> pulumi.Output[Optional[str]]:
         """
         The icon of the blueprint
         """
         return pulumi.get(self, "icon")
```

### Comparing `port_pulumi-1.9.1/port_pulumi/config/vars.py` & `port_pulumi-2.0.0/port_pulumi/config/vars.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.9.1/port_pulumi/entity.py` & `port_pulumi-2.0.0/port_pulumi/entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -359,15 +359,16 @@
                  properties: Optional[pulumi.Input[pulumi.InputType['EntityPropertiesArgs']]] = None,
                  relations: Optional[pulumi.Input[pulumi.InputType['EntityRelationsArgs']]] = None,
                  run_id: Optional[pulumi.Input[str]] = None,
                  teams: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Create a Entity resource with the given unique name, props, and options.
+        Entity resource
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] blueprint: The blueprint identifier the entity relates to
         :param pulumi.Input[str] icon: The icon of the entity
         :param pulumi.Input[str] identifier: The identifier of the entity
         :param pulumi.Input[pulumi.InputType['EntityPropertiesArgs']] properties: The properties of the entity
         :param pulumi.Input[pulumi.InputType['EntityRelationsArgs']] relations: The relations of the entity
@@ -378,15 +379,16 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: EntityArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a Entity resource with the given unique name, props, and options.
+        Entity resource
+
         :param str resource_name: The name of the resource.
         :param EntityArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(EntityArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `port_pulumi-1.9.1/port_pulumi/provider.py` & `port_pulumi-2.0.0/port_pulumi/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  base_url: Optional[pulumi.Input[str]] = None,
                  client_id: Optional[pulumi.Input[str]] = None,
                  secret: Optional[pulumi.Input[str]] = None,
                  token: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        The provider type for the port package. By default, resources use package-wide configuration
+        The provider type for the port-labs package. By default, resources use package-wide configuration
         settings, however an explicit `Provider` instance may be created and passed during resource
         construction to achieve fine-grained programmatic control over provider settings. See the
         [documentation](https://www.pulumi.com/docs/reference/programming-model/#providers) for more information.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] client_id: Client ID for Port-labs
@@ -104,15 +104,15 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[ProviderArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        The provider type for the port package. By default, resources use package-wide configuration
+        The provider type for the port-labs package. By default, resources use package-wide configuration
         settings, however an explicit `Provider` instance may be created and passed during resource
         construction to achieve fine-grained programmatic control over provider settings. See the
         [documentation](https://www.pulumi.com/docs/reference/programming-model/#providers) for more information.
 
         :param str resource_name: The name of the resource.
         :param ProviderArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
```

### Comparing `port_pulumi-1.9.1/port_pulumi/scorecard.py` & `port_pulumi-2.0.0/port_pulumi/scorecard.py`

 * *Files 24% similar despite different names*

```diff
@@ -224,30 +224,222 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  blueprint: Optional[pulumi.Input[str]] = None,
                  identifier: Optional[pulumi.Input[str]] = None,
                  rules: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ScorecardRuleArgs']]]]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Create a Scorecard resource with the given unique name, props, and options.
+        This resource allows you to manage a scorecard.
+
+        See the [Port documentation](https://docs.getport.io/promote-scorecards/) for more information about scorecards.
+
+        ## Example Usage
+
+        Create a parent blueprint with a child blueprint and an aggregation property to count the parent kids:
+
+        ```python
+        import pulumi
+        import json
+        import pulumi_port as port
+
+        microservice = port.index.Port_blueprint("microservice",
+            title=microservice,
+            icon=Terraform,
+            identifier=microservice,
+            properties={
+                stringProps: {
+                    author: {
+                        title: Author,
+                    },
+                    url: {
+                        title: URL,
+                    },
+                },
+                booleanProps: {
+                    required: {
+                        type: boolean,
+                    },
+                },
+                numberProps: {
+                    sum: {
+                        type: number,
+                    },
+                },
+            })
+        readiness = port.index.Port_scorecard("readiness",
+            identifier=Readiness,
+            title=Readiness,
+            blueprint=microservice.identifier,
+            rules=[
+                {
+                    identifier: hasOwner,
+                    title: Has Owner,
+                    level: Gold,
+                    query: {
+                        combinator: and,
+                        conditions: [
+                            json.dumps({
+                                property: $team,
+                                operator: isNotEmpty,
+                            }),
+                            json.dumps({
+                                property: author,
+                                operator: =,
+                                value: myValue,
+                            }),
+                        ],
+                    },
+                },
+                {
+                    identifier: hasUrl,
+                    title: Has URL,
+                    level: Silver,
+                    query: {
+                        combinator: and,
+                        conditions: [json.dumps({
+                            property: url,
+                            operator: isNotEmpty,
+                        })],
+                    },
+                },
+                {
+                    identifier: checkSumIfRequired,
+                    title: Check Sum If Required,
+                    level: Bronze,
+                    query: {
+                        combinator: or,
+                        conditions: [
+                            json.dumps({
+                                property: required,
+                                operator: =,
+                                value: False,
+                            }),
+                            json.dumps({
+                                property: sum,
+                                operator: >,
+                                value: 2,
+                            }),
+                        ],
+                    },
+                },
+            ],
+            opts=pulumi.ResourceOptions(depends_on=[microservice]))
+        ```
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] blueprint: The blueprint of the scorecard
         :param pulumi.Input[str] identifier: The identifier of the scorecard
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ScorecardRuleArgs']]]] rules: The rules of the scorecard
         :param pulumi.Input[str] title: The title of the scorecard
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ScorecardArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a Scorecard resource with the given unique name, props, and options.
+        This resource allows you to manage a scorecard.
+
+        See the [Port documentation](https://docs.getport.io/promote-scorecards/) for more information about scorecards.
+
+        ## Example Usage
+
+        Create a parent blueprint with a child blueprint and an aggregation property to count the parent kids:
+
+        ```python
+        import pulumi
+        import json
+        import pulumi_port as port
+
+        microservice = port.index.Port_blueprint("microservice",
+            title=microservice,
+            icon=Terraform,
+            identifier=microservice,
+            properties={
+                stringProps: {
+                    author: {
+                        title: Author,
+                    },
+                    url: {
+                        title: URL,
+                    },
+                },
+                booleanProps: {
+                    required: {
+                        type: boolean,
+                    },
+                },
+                numberProps: {
+                    sum: {
+                        type: number,
+                    },
+                },
+            })
+        readiness = port.index.Port_scorecard("readiness",
+            identifier=Readiness,
+            title=Readiness,
+            blueprint=microservice.identifier,
+            rules=[
+                {
+                    identifier: hasOwner,
+                    title: Has Owner,
+                    level: Gold,
+                    query: {
+                        combinator: and,
+                        conditions: [
+                            json.dumps({
+                                property: $team,
+                                operator: isNotEmpty,
+                            }),
+                            json.dumps({
+                                property: author,
+                                operator: =,
+                                value: myValue,
+                            }),
+                        ],
+                    },
+                },
+                {
+                    identifier: hasUrl,
+                    title: Has URL,
+                    level: Silver,
+                    query: {
+                        combinator: and,
+                        conditions: [json.dumps({
+                            property: url,
+                            operator: isNotEmpty,
+                        })],
+                    },
+                },
+                {
+                    identifier: checkSumIfRequired,
+                    title: Check Sum If Required,
+                    level: Bronze,
+                    query: {
+                        combinator: or,
+                        conditions: [
+                            json.dumps({
+                                property: required,
+                                operator: =,
+                                value: False,
+                            }),
+                            json.dumps({
+                                property: sum,
+                                operator: >,
+                                value: 2,
+                            }),
+                        ],
+                    },
+                },
+            ],
+            opts=pulumi.ResourceOptions(depends_on=[microservice]))
+        ```
+
         :param str resource_name: The name of the resource.
         :param ScorecardArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(ScorecardArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `port_pulumi-1.9.1/port_pulumi/team.py` & `port_pulumi-2.0.0/port_pulumi/team.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,29 +176,31 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  users: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
-        Create a Team resource with the given unique name, props, and options.
+        Team resource
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: The description of the team
         :param pulumi.Input[str] name: The name of the team
         :param pulumi.Input[Sequence[pulumi.Input[str]]] users: The users of the team
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: TeamArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a Team resource with the given unique name, props, and options.
+        Team resource
+
         :param str resource_name: The name of the resource.
         :param TeamArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(TeamArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `port_pulumi-1.9.1/port_pulumi/webhook.py` & `port_pulumi-2.0.0/port_pulumi/webhook.py`

 * *Files 0% similar despite different names*

```diff
@@ -359,15 +359,16 @@
                  icon: Optional[pulumi.Input[str]] = None,
                  identifier: Optional[pulumi.Input[str]] = None,
                  mappings: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['WebhookMappingArgs']]]]] = None,
                  security: Optional[pulumi.Input[pulumi.InputType['WebhookSecurityArgs']]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Create a Webhook resource with the given unique name, props, and options.
+        Webhook resource
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: The description of the webhook
         :param pulumi.Input[bool] enabled: Whether the webhook is enabled
         :param pulumi.Input[str] icon: The icon of the webhook
         :param pulumi.Input[str] identifier: The identifier of the webhook
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['WebhookMappingArgs']]]] mappings: The mappings of the webhook
@@ -377,15 +378,16 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[WebhookArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a Webhook resource with the given unique name, props, and options.
+        Webhook resource
+
         :param str resource_name: The name of the resource.
         :param WebhookArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(WebhookArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `port_pulumi-1.9.1/port_pulumi.egg-info/PKG-INFO` & `port_pulumi-2.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
-Name: port-pulumi
-Version: 1.9.1
+Name: port_pulumi
+Version: 2.0.0
 Summary: A Pulumi package for creating and managing Port resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/port-labs/pulumi-port
 Keywords: pulumi port category/utility
 Platform: UNKNOWN
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Port Resource Provider
 
-![Port](./img/port.svg)
+<img src="img/port.svg" width="300px">
 
 The Port Resource Provider lets you manage [Port](https://www.getport.io) resources.
 
 ## Installing
 
 This package is available for several languages/platforms:
```

### Comparing `port_pulumi-1.9.1/port_pulumi.egg-info/SOURCES.txt` & `port_pulumi-2.0.0/port_pulumi.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -4,16 +4,19 @@
 port_pulumi/_inputs.py
 port_pulumi/_utilities.py
 port_pulumi/action.py
 port_pulumi/action_permissions.py
 port_pulumi/aggregation_properties.py
 port_pulumi/aggregation_property.py
 port_pulumi/blueprint.py
+port_pulumi/blueprint_permissions.py
 port_pulumi/entity.py
 port_pulumi/outputs.py
+port_pulumi/page.py
+port_pulumi/page_permissions.py
 port_pulumi/provider.py
 port_pulumi/pulumi-plugin.json
 port_pulumi/py.typed
 port_pulumi/scorecard.py
 port_pulumi/team.py
 port_pulumi/webhook.py
 port_pulumi.egg-info/PKG-INFO
```

### Comparing `port_pulumi-1.9.1/setup.py` & `port_pulumi-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.9.1"
+VERSION = "2.0.0"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "port Pulumi Package - Development Version"
 
 
 setup(name='port_pulumi',
-      python_requires='>=3.7',
+      python_requires='>=3.8',
       version=VERSION,
       description="A Pulumi package for creating and managing Port resources.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       keywords='pulumi port category/utility',
       url='https://www.pulumi.com',
       project_urls={
```

