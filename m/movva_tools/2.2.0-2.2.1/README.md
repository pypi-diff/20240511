# Comparing `tmp/movva_tools-2.2.0.tar.gz` & `tmp/movva_tools-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movva_tools-2.2.0.tar", max compression
+gzip compressed data, was "movva_tools-2.2.1.tar", max compression
```

## Comparing `movva_tools-2.2.0.tar` & `movva_tools-2.2.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0       87 2023-09-28 10:29:10.291654 movva_tools-2.2.0/README.md
--rw-r--r--   0        0        0      175 2023-11-30 17:04:01.622621 movva_tools-2.2.0/movva_tools/__init__.py
--rw-r--r--   0        0        0      154 2023-09-28 10:29:10.291654 movva_tools-2.2.0/movva_tools/base_exception.py
--rw-r--r--   0        0        0     3236 2024-05-08 17:01:08.411366 movva_tools-2.2.0/movva_tools/constants.py
--rw-r--r--   0        0        0     3007 2024-05-10 15:34:01.622843 movva_tools-2.2.0/movva_tools/databases.py
--rw-r--r--   0        0        0      637 2023-11-16 12:54:55.447688 movva_tools-2.2.0/movva_tools/decorators.py
--rw-r--r--   0        0        0     1997 2024-05-09 20:05:34.923176 movva_tools-2.2.0/movva_tools/examples/copy_flow_example.py
--rw-r--r--   0        0        0     1677 2024-05-09 20:05:37.787038 movva_tools-2.2.0/movva_tools/examples/import_contacts_example.py
--rw-r--r--   0        0        0     1641 2023-10-13 15:28:13.270038 movva_tools-2.2.0/movva_tools/exceptions.py
--rw-r--r--   0        0        0     8910 2023-09-28 15:44:14.538563 movva_tools-2.2.0/movva_tools/import_contacts.py
--rw-r--r--   0        0        0      233 2024-05-09 20:24:44.562562 movva_tools-2.2.0/movva_tools/integrations/__init__.py
--rw-r--r--   0        0        0     1726 2024-05-09 20:41:47.398073 movva_tools-2.2.0/movva_tools/integrations/google.py
--rw-r--r--   0        0        0     5713 2024-05-10 13:19:39.839625 movva_tools-2.2.0/movva_tools/integrations/google_drive.py
--rw-r--r--   0        0        0    11382 2024-05-10 13:19:50.727475 movva_tools-2.2.0/movva_tools/integrations/google_spreadsheets.py
--rw-r--r--   0        0        0      848 2023-11-30 16:38:20.085932 movva_tools-2.2.0/movva_tools/models/__init__.py
--rw-r--r--   0        0        0      490 2023-11-16 12:54:55.447688 movva_tools-2.2.0/movva_tools/models/api_token_model.py
--rw-r--r--   0        0        0     2507 2023-11-16 12:54:55.447688 movva_tools-2.2.0/movva_tools/models/campaign_models.py
--rw-r--r--   0        0        0     2014 2023-11-16 12:54:55.447688 movva_tools-2.2.0/movva_tools/models/channel_models.py
--rw-r--r--   0        0        0     3363 2024-05-06 12:45:47.658291 movva_tools-2.2.0/movva_tools/models/contacts_models.py
--rw-r--r--   0        0        0     9630 2023-11-16 12:54:55.447688 movva_tools-2.2.0/movva_tools/models/flow_models.py
--rw-r--r--   0        0        0     1348 2023-11-30 17:53:45.673645 movva_tools-2.2.0/movva_tools/models/messages_models.py
--rw-r--r--   0        0        0     1369 2023-09-28 15:17:44.535564 movva_tools-2.2.0/movva_tools/models/organization_models.py
--rw-r--r--   0        0        0      638 2023-09-28 15:17:43.643571 movva_tools-2.2.0/movva_tools/models/user_models.py
--rw-r--r--   0        0        0       76 2023-11-16 12:54:55.447688 movva_tools-2.2.0/movva_tools/notifications/__init__.py
--rw-r--r--   0        0        0     5710 2023-11-16 12:54:55.447688 movva_tools-2.2.0/movva_tools/notifications/slack.py
--rw-r--r--   0        0        0     1362 2023-09-28 10:29:10.291654 movva_tools-2.2.0/movva_tools/parsers.py
--rw-r--r--   0        0        0      479 2023-11-16 12:54:55.447688 movva_tools-2.2.0/movva_tools/serializers/__init__.py
--rw-r--r--   0        0        0      205 2023-11-16 12:54:55.447688 movva_tools-2.2.0/movva_tools/serializers/base_serializer.py
--rw-r--r--   0        0        0     1340 2023-11-16 13:02:39.308774 movva_tools-2.2.0/movva_tools/serializers/campaign_event_serializer.py
--rw-r--r--   0        0        0      469 2023-11-16 13:02:39.308774 movva_tools-2.2.0/movva_tools/serializers/campaign_serializer.py
--rw-r--r--   0        0        0      427 2023-11-16 13:02:39.312774 movva_tools-2.2.0/movva_tools/serializers/contact_group_serializer.py
--rw-r--r--   0        0        0      432 2023-11-16 13:18:23.218068 movva_tools-2.2.0/movva_tools/serializers/flow_revision_serializer.py
--rw-r--r--   0        0        0      453 2023-11-16 13:18:24.762033 movva_tools-2.2.0/movva_tools/serializers/flow_serializer.py
--rw-r--r--   0        0        0      422 2023-11-16 13:02:39.308774 movva_tools-2.2.0/movva_tools/serializers/organization_serializer.py
--rw-r--r--   0        0        0      658 2023-11-30 17:04:20.189985 movva_tools-2.2.0/movva_tools/services/__init__.py
--rw-r--r--   0        0        0     1205 2024-05-06 12:19:06.870867 movva_tools-2.2.0/movva_tools/services/api_token_service.py
--rw-r--r--   0        0        0     1553 2024-05-10 15:42:05.458080 movva_tools-2.2.0/movva_tools/services/base_service.py
--rw-r--r--   0        0        0     4892 2024-05-07 22:13:43.989611 movva_tools-2.2.0/movva_tools/services/campaign_service.py
--rw-r--r--   0        0        0     1822 2024-05-07 22:14:25.213343 movva_tools-2.2.0/movva_tools/services/channel_service.py
--rw-r--r--   0        0        0     4541 2024-05-07 22:14:48.069193 movva_tools-2.2.0/movva_tools/services/contacts_service.py
--rw-r--r--   0        0        0    24936 2024-05-09 20:05:40.130926 movva_tools-2.2.0/movva_tools/services/flow_service.py
--rw-r--r--   0        0        0     3122 2024-05-10 15:23:26.705294 movva_tools-2.2.0/movva_tools/services/messages_service.py
--rw-r--r--   0        0        0     1235 2024-05-07 22:16:46.020401 movva_tools-2.2.0/movva_tools/services/organization_service.py
--rw-r--r--   0        0        0      941 2024-05-08 17:00:52.559400 movva_tools-2.2.0/movva_tools/services/user_service.py
--rw-r--r--   0        0        0     1818 2023-11-16 12:54:55.447688 movva_tools-2.2.0/movva_tools/utils.py
--rw-r--r--   0        0        0      982 2023-09-28 16:52:41.474439 movva_tools-2.2.0/movva_tools/validators.py
--rw-r--r--   0        0        0      956 2024-05-10 17:39:15.750217 movva_tools-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     1294 1970-01-01 00:00:00.000000 movva_tools-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-09-28 10:29:10.291654 movva_tools-2.2.1/README.md
+-rw-r--r--   0        0        0      175 2023-11-30 17:04:01.622621 movva_tools-2.2.1/movva_tools/__init__.py
+-rw-r--r--   0        0        0      154 2023-09-28 10:29:10.291654 movva_tools-2.2.1/movva_tools/base_exception.py
+-rw-r--r--   0        0        0     3236 2024-05-08 17:01:08.411366 movva_tools-2.2.1/movva_tools/constants.py
+-rw-r--r--   0        0        0     3007 2024-05-10 15:34:01.622843 movva_tools-2.2.1/movva_tools/databases.py
+-rw-r--r--   0        0        0      637 2023-11-16 12:54:55.447688 movva_tools-2.2.1/movva_tools/decorators.py
+-rw-r--r--   0        0        0     1997 2024-05-09 20:05:34.923176 movva_tools-2.2.1/movva_tools/examples/copy_flow_example.py
+-rw-r--r--   0        0        0     1677 2024-05-09 20:05:37.787038 movva_tools-2.2.1/movva_tools/examples/import_contacts_example.py
+-rw-r--r--   0        0        0     1641 2023-10-13 15:28:13.270038 movva_tools-2.2.1/movva_tools/exceptions.py
+-rw-r--r--   0        0        0     8910 2023-09-28 15:44:14.538563 movva_tools-2.2.1/movva_tools/import_contacts.py
+-rw-r--r--   0        0        0      233 2024-05-09 20:24:44.562562 movva_tools-2.2.1/movva_tools/integrations/__init__.py
+-rw-r--r--   0        0        0     1726 2024-05-09 20:41:47.398073 movva_tools-2.2.1/movva_tools/integrations/google.py
+-rw-r--r--   0        0        0     5713 2024-05-10 18:18:01.812820 movva_tools-2.2.1/movva_tools/integrations/google_drive.py
+-rw-r--r--   0        0        0    11382 2024-05-10 13:19:50.727475 movva_tools-2.2.1/movva_tools/integrations/google_spreadsheets.py
+-rw-r--r--   0        0        0      848 2023-11-30 16:38:20.085932 movva_tools-2.2.1/movva_tools/models/__init__.py
+-rw-r--r--   0        0        0      490 2023-11-16 12:54:55.447688 movva_tools-2.2.1/movva_tools/models/api_token_model.py
+-rw-r--r--   0        0        0     2507 2023-11-16 12:54:55.447688 movva_tools-2.2.1/movva_tools/models/campaign_models.py
+-rw-r--r--   0        0        0     2014 2023-11-16 12:54:55.447688 movva_tools-2.2.1/movva_tools/models/channel_models.py
+-rw-r--r--   0        0        0     3363 2024-05-06 12:45:47.658291 movva_tools-2.2.1/movva_tools/models/contacts_models.py
+-rw-r--r--   0        0        0     9630 2023-11-16 12:54:55.447688 movva_tools-2.2.1/movva_tools/models/flow_models.py
+-rw-r--r--   0        0        0     1348 2023-11-30 17:53:45.673645 movva_tools-2.2.1/movva_tools/models/messages_models.py
+-rw-r--r--   0        0        0     1369 2023-09-28 15:17:44.535564 movva_tools-2.2.1/movva_tools/models/organization_models.py
+-rw-r--r--   0        0        0      638 2023-09-28 15:17:43.643571 movva_tools-2.2.1/movva_tools/models/user_models.py
+-rw-r--r--   0        0        0       76 2023-11-16 12:54:55.447688 movva_tools-2.2.1/movva_tools/notifications/__init__.py
+-rw-r--r--   0        0        0     5710 2023-11-16 12:54:55.447688 movva_tools-2.2.1/movva_tools/notifications/slack.py
+-rw-r--r--   0        0        0     1362 2023-09-28 10:29:10.291654 movva_tools-2.2.1/movva_tools/parsers.py
+-rw-r--r--   0        0        0      479 2023-11-16 12:54:55.447688 movva_tools-2.2.1/movva_tools/serializers/__init__.py
+-rw-r--r--   0        0        0      205 2023-11-16 12:54:55.447688 movva_tools-2.2.1/movva_tools/serializers/base_serializer.py
+-rw-r--r--   0        0        0     1340 2023-11-16 13:02:39.308774 movva_tools-2.2.1/movva_tools/serializers/campaign_event_serializer.py
+-rw-r--r--   0        0        0      469 2023-11-16 13:02:39.308774 movva_tools-2.2.1/movva_tools/serializers/campaign_serializer.py
+-rw-r--r--   0        0        0      427 2023-11-16 13:02:39.312774 movva_tools-2.2.1/movva_tools/serializers/contact_group_serializer.py
+-rw-r--r--   0        0        0      432 2023-11-16 13:18:23.218068 movva_tools-2.2.1/movva_tools/serializers/flow_revision_serializer.py
+-rw-r--r--   0        0        0      453 2023-11-16 13:18:24.762033 movva_tools-2.2.1/movva_tools/serializers/flow_serializer.py
+-rw-r--r--   0        0        0      422 2023-11-16 13:02:39.308774 movva_tools-2.2.1/movva_tools/serializers/organization_serializer.py
+-rw-r--r--   0        0        0      677 2024-05-11 18:59:21.492103 movva_tools-2.2.1/movva_tools/services/__init__.py
+-rw-r--r--   0        0        0     1205 2024-05-06 12:19:06.870867 movva_tools-2.2.1/movva_tools/services/api_token_service.py
+-rw-r--r--   0        0        0     1553 2024-05-10 15:42:05.458080 movva_tools-2.2.1/movva_tools/services/base_service.py
+-rw-r--r--   0        0        0     4892 2024-05-07 22:13:43.989611 movva_tools-2.2.1/movva_tools/services/campaign_service.py
+-rw-r--r--   0        0        0     1822 2024-05-07 22:14:25.213343 movva_tools-2.2.1/movva_tools/services/channel_service.py
+-rw-r--r--   0        0        0     4541 2024-05-07 22:14:48.069193 movva_tools-2.2.1/movva_tools/services/contacts_service.py
+-rw-r--r--   0        0        0    24936 2024-05-09 20:05:40.130926 movva_tools-2.2.1/movva_tools/services/flow_service.py
+-rw-r--r--   0        0        0     3122 2024-05-10 15:23:26.705294 movva_tools-2.2.1/movva_tools/services/messages_service.py
+-rw-r--r--   0        0        0     1235 2024-05-07 22:16:46.020401 movva_tools-2.2.1/movva_tools/services/organization_service.py
+-rw-r--r--   0        0        0      941 2024-05-08 17:00:52.559400 movva_tools-2.2.1/movva_tools/services/user_service.py
+-rw-r--r--   0        0        0     1818 2023-11-16 12:54:55.447688 movva_tools-2.2.1/movva_tools/utils.py
+-rw-r--r--   0        0        0      982 2023-09-28 16:52:41.474439 movva_tools-2.2.1/movva_tools/validators.py
+-rw-r--r--   0        0        0      956 2024-05-11 19:00:04.320507 movva_tools-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1294 1970-01-01 00:00:00.000000 movva_tools-2.2.1/PKG-INFO
```

### Comparing `movva_tools-2.2.0/movva_tools/constants.py` & `movva_tools-2.2.1/movva_tools/constants.py`

 * *Files identical despite different names*

### Comparing `movva_tools-2.2.0/movva_tools/databases.py` & `movva_tools-2.2.1/movva_tools/databases.py`

 * *Files identical despite different names*

### Comparing `movva_tools-2.2.0/movva_tools/decorators.py` & `movva_tools-2.2.1/movva_tools/decorators.py`

 * *Files identical despite different names*

### Comparing `movva_tools-2.2.0/movva_tools/examples/copy_flow_example.py` & `movva_tools-2.2.1/movva_tools/examples/copy_flow_example.py`

 * *Files identical despite different names*

### Comparing `movva_tools-2.2.0/movva_tools/examples/import_contacts_example.py` & `movva_tools-2.2.1/movva_tools/examples/import_contacts_example.py`

 * *Files identical despite different names*

### Comparing `movva_tools-2.2.0/movva_tools/exceptions.py` & `movva_tools-2.2.1/movva_tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `movva_tools-2.2.0/movva_tools/import_contacts.py` & `movva_tools-2.2.1/movva_tools/import_contacts.py`

 * *Files identical despite different names*

### Comparing `movva_tools-2.2.0/movva_tools/integrations/google.py` & `movva_tools-2.2.1/movva_tools/integrations/google.py`

 * *Files identical despite different names*

### Comparing `movva_tools-2.2.0/movva_tools/integrations/google_drive.py` & `movva_tools-2.2.1/movva_tools/integrations/google_drive.py`

 * *Files identical despite different names*

### Comparing `movva_tools-2.2.0/movva_tools/integrations/google_spreadsheets.py` & `movva_tools-2.2.1/movva_tools/integrations/google_spreadsheets.py`

 * *Files identical despite different names*

### Comparing `movva_tools-2.2.0/movva_tools/models/__init__.py` & `movva_tools-2.2.1/movva_tools/models/__init__.py`

 * *Files identical despite different names*

### Comparing `movva_tools-2.2.0/movva_tools/models/campaign_models.py` & `movva_tools-2.2.1/movva_tools/models/campaign_models.py`

 * *Files identical despite different names*

### Comparing `movva_tools-2.2.0/movva_tools/models/channel_models.py` & `movva_tools-2.2.1/movva_tools/models/channel_models.py`

 * *Files identical despite different names*

### Comparing `movva_tools-2.2.0/movva_tools/models/contacts_models.py` & `movva_tools-2.2.1/movva_tools/models/contacts_models.py`

 * *Files identical despite different names*

### Comparing `movva_tools-2.2.0/movva_tools/models/flow_models.py` & `movva_tools-2.2.1/movva_tools/models/flow_models.py`

 * *Files identical despite different names*

### Comparing `movva_tools-2.2.0/movva_tools/models/messages_models.py` & `movva_tools-2.2.1/movva_tools/models/messages_models.py`

 * *Files identical despite different names*

### Comparing `movva_tools-2.2.0/movva_tools/models/organization_models.py` & `movva_tools-2.2.1/movva_tools/models/organization_models.py`

 * *Files identical despite different names*

### Comparing `movva_tools-2.2.0/movva_tools/models/user_models.py` & `movva_tools-2.2.1/movva_tools/models/user_models.py`

 * *Files identical despite different names*

### Comparing `movva_tools-2.2.0/movva_tools/notifications/slack.py` & `movva_tools-2.2.1/movva_tools/notifications/slack.py`

 * *Files identical despite different names*

### Comparing `movva_tools-2.2.0/movva_tools/parsers.py` & `movva_tools-2.2.1/movva_tools/parsers.py`

 * *Files identical despite different names*

### Comparing `movva_tools-2.2.0/movva_tools/serializers/campaign_event_serializer.py` & `movva_tools-2.2.1/movva_tools/serializers/campaign_event_serializer.py`

 * *Files identical despite different names*

### Comparing `movva_tools-2.2.0/movva_tools/services/__init__.py` & `movva_tools-2.2.1/movva_tools/services/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from movva_tools.services.api_token_service import APITokenService
 from movva_tools.services.base_service import BaseService
 from movva_tools.services.campaign_service import CampaingService
 from movva_tools.services.channel_service import ChannelService
-from movva_tools.services.contacts_service import ContactService
+from movva_tools.services.contacts_service import ContactService, ContactURNService
 from movva_tools.services.flow_service import (
     FlowService, FlowLabelService, CopyFlowAndScheduleService,
     FlowDependenciesService
 )
 from movva_tools.services.organization_service import OrganizationService
 from movva_tools.services.user_service import UserService
 from movva_tools.services.messages_service import MessageService
```

### Comparing `movva_tools-2.2.0/movva_tools/services/api_token_service.py` & `movva_tools-2.2.1/movva_tools/services/api_token_service.py`

 * *Files identical despite different names*

### Comparing `movva_tools-2.2.0/movva_tools/services/base_service.py` & `movva_tools-2.2.1/movva_tools/services/base_service.py`

 * *Files identical despite different names*

### Comparing `movva_tools-2.2.0/movva_tools/services/campaign_service.py` & `movva_tools-2.2.1/movva_tools/services/campaign_service.py`

 * *Files identical despite different names*

### Comparing `movva_tools-2.2.0/movva_tools/services/channel_service.py` & `movva_tools-2.2.1/movva_tools/services/channel_service.py`

 * *Files identical despite different names*

### Comparing `movva_tools-2.2.0/movva_tools/services/contacts_service.py` & `movva_tools-2.2.1/movva_tools/services/contacts_service.py`

 * *Files identical despite different names*

### Comparing `movva_tools-2.2.0/movva_tools/services/flow_service.py` & `movva_tools-2.2.1/movva_tools/services/flow_service.py`

 * *Files identical despite different names*

### Comparing `movva_tools-2.2.0/movva_tools/services/messages_service.py` & `movva_tools-2.2.1/movva_tools/services/messages_service.py`

 * *Files identical despite different names*

### Comparing `movva_tools-2.2.0/movva_tools/services/organization_service.py` & `movva_tools-2.2.1/movva_tools/services/organization_service.py`

 * *Files identical despite different names*

### Comparing `movva_tools-2.2.0/movva_tools/services/user_service.py` & `movva_tools-2.2.1/movva_tools/services/user_service.py`

 * *Files identical despite different names*

### Comparing `movva_tools-2.2.0/movva_tools/utils.py` & `movva_tools-2.2.1/movva_tools/utils.py`

 * *Files identical despite different names*

### Comparing `movva_tools-2.2.0/movva_tools/validators.py` & `movva_tools-2.2.1/movva_tools/validators.py`

 * *Files identical despite different names*

### Comparing `movva_tools-2.2.0/pyproject.toml` & `movva_tools-2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "movva_tools"
-version = "2.2.0"
+version = "2.2.1"
 description = "Package that contains integrations and tools to use in issues of Movva organization."
 authors = ["WillamesCampos <willwjccampos@gmail.com>"]
 readme = "README.md"
 packages = [{include = "movva_tools"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `movva_tools-2.2.0/PKG-INFO` & `movva_tools-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: movva_tools
-Version: 2.2.0
+Version: 2.2.1
 Summary: Package that contains integrations and tools to use in issues of Movva organization.
 Author: WillamesCampos
 Author-email: willwjccampos@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

