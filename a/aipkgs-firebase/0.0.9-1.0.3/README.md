# Comparing `tmp/aipkgs_firebase-0.0.9.tar.gz` & `tmp/aipkgs_firebase-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aipkgs_firebase-0.0.9.tar", max compression
+gzip compressed data, was "aipkgs_firebase-1.0.3.tar", max compression
```

## Comparing `aipkgs_firebase-0.0.9.tar` & `aipkgs_firebase-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1058 2022-03-08 13:06:48.928787 aipkgs_firebase-0.0.9/LICENSE.md
--rw-r--r--   0        0        0       13 2022-03-08 13:06:48.929037 aipkgs_firebase-0.0.9/README.rst
--rw-r--r--   0        0        0       88 2022-03-08 13:06:48.928222 aipkgs_firebase-0.0.9/aipkgs_firebase/__init__.py
--rw-r--r--   0        0        0     2302 2023-11-26 13:02:33.501317 aipkgs_firebase-0.0.9/aipkgs_firebase/helpers.py
--rw-r--r--   0        0        0      136 2023-11-26 12:53:12.992955 aipkgs_firebase-0.0.9/aipkgs_firebase/messaging/__init__.py
--rw-r--r--   0        0        0     5155 2022-03-08 13:06:48.928493 aipkgs_firebase-0.0.9/aipkgs_firebase/messaging/core.py
--rw-r--r--   0        0        0       74 2022-03-08 13:06:48.928579 aipkgs_firebase-0.0.9/aipkgs_firebase/messaging/enums.py
--rw-r--r--   0        0        0     2474 2022-03-08 13:06:48.928861 aipkgs_firebase-0.0.9/aipkgs_firebase/messaging/helpers.py
--rw-r--r--   0        0        0     4215 2023-11-26 13:02:21.871322 aipkgs_firebase-0.0.9/aipkgs_firebase/storage/core.py
--rw-r--r--   0        0        0     2723 2024-05-09 11:42:43.751124 aipkgs_firebase-0.0.9/aipkgs_firebase/storage/helpers.py
--rw-r--r--   0        0        0     2689 2024-05-09 11:43:09.034133 aipkgs_firebase-0.0.9/aipkgs_firebase/storage/root.py
--rw-r--r--   0        0        0      571 2024-05-09 11:44:08.800804 aipkgs_firebase-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 aipkgs_firebase-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-05-09 12:25:47.460445 aipkgs_firebase-1.0.3/LICENSE.md
+-rw-r--r--   0        0        0       13 2022-03-08 13:06:48.929037 aipkgs_firebase-1.0.3/README.rst
+-rw-r--r--   0        0        0       88 2022-03-08 13:06:48.928222 aipkgs_firebase-1.0.3/aipkgs_firebase/__init__.py
+-rw-r--r--   0        0        0     1737 2024-05-11 14:14:48.035567 aipkgs_firebase-1.0.3/aipkgs_firebase/actions/core.py
+-rw-r--r--   0        0        0     2302 2023-11-26 13:02:33.501317 aipkgs_firebase-1.0.3/aipkgs_firebase/helpers.py
+-rw-r--r--   0        0        0     5948 2024-05-10 18:18:59.859448 aipkgs_firebase-1.0.3/aipkgs_firebase/messaging/core.py
+-rw-r--r--   0        0        0      132 2024-05-10 18:17:53.723527 aipkgs_firebase-1.0.3/aipkgs_firebase/messaging/enums.py
+-rw-r--r--   0        0        0     3079 2024-05-10 18:46:13.123781 aipkgs_firebase-1.0.3/aipkgs_firebase/messaging/helpers.py
+-rw-r--r--   0        0        0     5510 2024-05-10 16:47:09.357450 aipkgs_firebase-1.0.3/aipkgs_firebase/storage/core.py
+-rw-r--r--   0        0        0     3599 2024-05-10 16:48:36.758619 aipkgs_firebase-1.0.3/aipkgs_firebase/storage/helpers.py
+-rw-r--r--   0        0        0     3393 2024-05-10 17:20:12.608367 aipkgs_firebase-1.0.3/aipkgs_firebase/storage/root.py
+-rw-r--r--   0        0        0     2314 2024-05-10 18:47:03.096540 aipkgs_firebase-1.0.3/aipkgs_firebase/user/core.py
+-rw-r--r--   0        0        0      687 2024-05-11 14:16:12.436012 aipkgs_firebase-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 aipkgs_firebase-1.0.3/PKG-INFO
```

### Comparing `aipkgs_firebase-0.0.9/LICENSE.md` & `aipkgs_firebase-1.0.3/LICENSE.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-Copyright (C) 2022 Alexy Ibrahim
+Copyright (C) 2024 Alexy Ibrahim
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `aipkgs_firebase-0.0.9/aipkgs_firebase/helpers.py` & `aipkgs_firebase-1.0.3/aipkgs_firebase/helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-0.0.9/aipkgs_firebase/messaging/core.py` & `aipkgs_firebase-1.0.3/aipkgs_firebase/messaging/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,183 +1,179 @@
 import datetime
 
 from firebase_admin import messaging
 
 # region create message
-from aipkgs_firebase.messaging.enums import AndroidPriorityEnum
+from aipkgs_firebase.messaging.enums import FirebaseMessaging
 
 
-def create_message(token: str = None, notification: messaging.Notification = None,
-                   android_config: messaging.AndroidConfig = None, apns_config: messaging.APNSConfig = None,
-                   web_push: messaging.WebpushConfig = None, topic: str = None, data: dict = None,
-                   condition: str = None):
-    message = messaging.Message()
-    if token:
-        message.token = token
-    if notification:
-        message.notification = notification
-    if android_config:
-        message.android = android_config
-    if apns_config:
-        message.apns = apns_config
-    if web_push:
-        message.webpush = web_push
-    if topic:
-        message.topic = topic
-    if data:
-        message.data = data
-    if condition:
-        message.condition = condition
-    return message
-
-
-def create_multicast_message(tokens: list = None, notification: messaging.Notification = None,
-                             android_config: messaging.AndroidConfig = None, apns_config: messaging.APNSConfig = None,
-                             web_push: messaging.WebpushConfig = None, topic: str = None, data: dict = None):
-    message = messaging.MulticastMessage()
-    if tokens:
-        message.tokens = tokens
-    if notification:
-        message.notification = notification
-    if android_config:
-        message.android = android_config
-    if apns_config:
-        message.apns = apns_config
-    if web_push:
-        message.webpush = web_push
-    if topic:
-        message.topic = topic
-    if data:
-        message.data = data
-    return message
-
-
-# endregion
-
-
-# region notification
-def create_notification(title: str = None, body: str = None):
-    notification = messaging.Notification()
-    if title:
-        notification.title = title
-    if body:
-        notification.body = body
-    return notification
-
-
-# endregion
-
-
-# region ios
-def create_ios_apns_config(title: str = None, body: str = None, priority: int = None, badge: int = None):
-    # aps alert
-    aps_alert = messaging.ApsAlert(
-        title=title,
-        body=body,
-    )
-    if title:
-        aps_alert.title = title
-    if body:
-        aps_alert.body = body
-
-    # aps
-    aps = messaging.Aps()
-    if aps_alert:
-        aps.alert = aps_alert
-    if badge:
-        aps.badge = badge
-
-    # apns payload
-    payload = messaging.APNSPayload()
-    if aps:
-        payload.aps = aps
-
-    # apns config
-    apns_config = messaging.APNSConfig()
-    if payload:
-        apns_config.payload = payload
-
-    headers: dict = {}
-    if priority:
-        headers['apns-priority'] = f'{priority}'
-    apns_config.headers = headers
-
-    return apns_config
-
-
-# endregion
-
-
-# region android
-def create_android_configuration(title: str = None, body: str = None, icon: str = None, color: str = None,
-                                 ttl_seconds: int = None, priority: AndroidPriorityEnum = None):
-    notification = messaging.AndroidNotification()
-    if title:
-        notification.title = title
-    if body:
-        notification.body = body
-    if icon:
-        notification.icon = icon
-    if color:
-        notification.color = color
-
-    android_config = messaging.AndroidConfig()
-    notification.ttl = datetime.timedelta(seconds=ttl_seconds or 3600),
-    notification.priority = priority.value if priority else AndroidPriorityEnum.normal.value
-    if notification:
-        android_config.notification = notification
-
-    return android_config
-
-
-# endregion
-
-
-# region web notification
-def create_web_push_config(title: str = None, body: str = None, icon: str = None):
-    notification = messaging.WebpushNotification()
-    if title:
-        notification.title = title
-    if body:
-        notification.body = body
-    if icon:
-        notification.icon = icon
-
-    config = messaging.WebpushConfig()
-    if notification:
-        config.notification = notification
-
-    return config
-
-
-# eng region
-
-
-# region send messages
-def send_all_message(messages: [messaging.Message], dry_run: bool = None):
-    response = messaging.send_all(messages=messages, dry_run=dry_run or False)
-    print('{0} messages were sent successfully'.format(response.success_count))
-
-
-def send_message(message: messaging.Message, dry_run: bool = None):
-    response = messaging.send(message=message, dry_run=dry_run or False)
-    print('Successfully sent message:', response)
-
-
-def send_multicast_message(message: messaging.MulticastMessage, dry_run: bool = None):
-    response = messaging.send_multicast(multicast_message=message, dry_run=dry_run or False)
-    print('{0} messages were sent successfully'.format(response.success_count))
-
-
-# endregion
-
-
-# region topic
-def subscribe_to_topic(topic: str, tokens: list):
-    response = messaging.subscribe_to_topic(tokens, topic)
-    print(response.success_count, 'tokens were subscribed successfully')
-
-
-def unsubscribe_from_topic(topic: str, tokens: list):
-    response = messaging.unsubscribe_from_topic(tokens, topic)
-    print(response.success_count, 'tokens were unsubscribed successfully')
-# endregion
+class FirebaseMessagingCore:
+    @staticmethod
+    def create_message(token: str = None, notification: messaging.Notification = None,
+                       android_config: messaging.AndroidConfig = None, apns_config: messaging.APNSConfig = None,
+                       web_push: messaging.WebpushConfig = None, topic: str = None, data: dict = None,
+                       condition: str = None):
+        message = messaging.Message()
+        if token:
+            message.token = token
+        if notification:
+            message.notification = notification
+        if android_config:
+            message.android = android_config
+        if apns_config:
+            message.apns = apns_config
+        if web_push:
+            message.webpush = web_push
+        if topic:
+            message.topic = topic
+        if data:
+            message.data = data
+        if condition:
+            message.condition = condition
+        return message
+
+    @staticmethod
+    def create_multicast_message(tokens: list = None, notification: messaging.Notification = None,
+                                 android_config: messaging.AndroidConfig = None, apns_config: messaging.APNSConfig = None,
+                                 web_push: messaging.WebpushConfig = None, topic: str = None, data: dict = None):
+        message = messaging.MulticastMessage()
+        if tokens:
+            message.tokens = tokens
+        if notification:
+            message.notification = notification
+        if android_config:
+            message.android = android_config
+        if apns_config:
+            message.apns = apns_config
+        if web_push:
+            message.webpush = web_push
+        if topic:
+            message.topic = topic
+        if data:
+            message.data = data
+        return message
+
+    # endregion
+
+    # region notification
+    @staticmethod
+    def create_notification(title: str = None, body: str = None):
+        notification = messaging.Notification()
+        if title:
+            notification.title = title
+        if body:
+            notification.body = body
+        return notification
+
+    # endregion
+
+    # region ios
+    @staticmethod
+    def create_ios_apns_config(title: str = None, body: str = None, priority: int = None, badge: int = None):
+        # aps alert
+        aps_alert = messaging.ApsAlert(
+            title=title,
+            body=body,
+        )
+        if title:
+            aps_alert.title = title
+        if body:
+            aps_alert.body = body
+
+        # aps
+        aps = messaging.Aps()
+        if aps_alert:
+            aps.alert = aps_alert
+        if badge:
+            aps.badge = badge
+
+        # apns payload
+        payload = messaging.APNSPayload()
+        if aps:
+            payload.aps = aps
+
+        # apns config
+        apns_config = messaging.APNSConfig()
+        if payload:
+            apns_config.payload = payload
+
+        headers: dict = {}
+        if priority:
+            headers['apns-priority'] = f'{priority}'
+        apns_config.headers = headers
+
+        return apns_config
+
+    # endregion
+
+    # region android
+    @staticmethod
+    def create_android_configuration(title: str = None, body: str = None, icon: str = None, color: str = None,
+                                     ttl_seconds: int = None, priority: FirebaseMessaging.Enums.AndroidPriorityEnum = None):
+        notification = messaging.AndroidNotification()
+        if title:
+            notification.title = title
+        if body:
+            notification.body = body
+        if icon:
+            notification.icon = icon
+        if color:
+            notification.color = color
+
+        android_config = messaging.AndroidConfig()
+        notification.ttl = datetime.timedelta(seconds=ttl_seconds or 3600),
+        notification.priority = priority.value if priority else FirebaseMessaging.Enums.AndroidPriorityEnum.normal.value
+        if notification:
+            android_config.notification = notification
+
+        return android_config
+
+    # endregion
+
+    # region web notification
+    @staticmethod
+    def create_web_push_config(title: str = None, body: str = None, icon: str = None):
+        notification = messaging.WebpushNotification()
+        if title:
+            notification.title = title
+        if body:
+            notification.body = body
+        if icon:
+            notification.icon = icon
+
+        config = messaging.WebpushConfig()
+        if notification:
+            config.notification = notification
+
+        return config
+
+    # eng region
+
+    # region send messages
+    @staticmethod
+    def send_all_message(messages: [messaging.Message], dry_run: bool = None):
+        response = messaging.send_all(messages=messages, dry_run=dry_run or False)
+        print('{0} messages were sent successfully'.format(response.success_count))
+
+    @staticmethod
+    def send_message(message: messaging.Message, dry_run: bool = None):
+        response = messaging.send(message=message, dry_run=dry_run or False)
+        print('Successfully sent message:', response)
+
+    @staticmethod
+    def send_multicast_message(message: messaging.MulticastMessage, dry_run: bool = None):
+        response = messaging.send_multicast(multicast_message=message, dry_run=dry_run or False)
+        print('{0} messages were sent successfully'.format(response.success_count))
+
+    # endregion
+
+    # region topic
+    @staticmethod
+    def subscribe_to_topic(topic: str, tokens: list):
+        response = messaging.subscribe_to_topic(tokens, topic)
+        print(response.success_count, 'tokens were subscribed successfully')
+
+    @staticmethod
+    def unsubscribe_from_topic(topic: str, tokens: list):
+        response = messaging.unsubscribe_from_topic(tokens, topic)
+        print(response.success_count, 'tokens were unsubscribed successfully')
+    # endregion
```

### Comparing `aipkgs_firebase-0.0.9/aipkgs_firebase/storage/helpers.py` & `aipkgs_firebase-1.0.3/aipkgs_firebase/storage/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,95 +1,112 @@
 from typing import Dict, List, Optional
 
-from aipkgs_firebase.storage import core
+from aipkgs_firebase.storage.core import FirebaseStorageCore
 
 
 # Use the application default credentials
 
-def document_exists(collection_name: str, filters: Dict[str, any]) -> bool:
-    docs = core.get_documents(
-        collection_name=collection_name, filters=filters
-    )
+class FirebaseStorageHelper:
 
-    if docs:
-        return True
+    @staticmethod
+    def document_exists(collection_name: str, filters: Dict[str, any]) -> bool:
+        docs = FirebaseStorageCore.get_documents(
+            collection_name=collection_name, filters=filters
+        )
+
+        if docs:
+            return True
+
+        return False
+
+    @staticmethod
+    def get_document(collection_name: str, document_id: str) -> Optional[dict]:
+        doc = FirebaseStorageCore.get_document(
+            collection_name=collection_name, document_id=document_id
+        )
 
-    return False
-
-def get_document(collection_name: str, document_id: str) -> Optional[dict]:
-    doc = core.get_document(
-        collection_name=collection_name, document_id=document_id
-    )
+        if doc.exists:
+            dictionary = doc.to_dict()
+            dictionary["id"] = doc.id
+            return dictionary
 
-    if doc.exists:
-        dictionary = doc.to_dict()
-        dictionary["id"] = doc.id
-        return dictionary
+        return None
 
-    return None
+    @staticmethod
+    def get_document_where(collection_name: str, filters: Dict[str, any] = None) -> Optional[dict]:
+        docs = FirebaseStorageCore.get_documents(
+            collection_name=collection_name, filters=filters
+        )
 
+        if docs:
+            doc = docs[0]
+            dictionary = doc.to_dict()
+            dictionary["id"] = doc.id
+            return dictionary
 
-def get_document_realtime(collection_name: str, document_id: str, callback):
-    def temp_callback(doc_snapshot, changes, read_time):
-        if len(doc_snapshot) == 1:
-            doc = doc_snapshot[0]
+        return None
 
-            if doc.exists:
-                dictionary = doc.to_dict()
-                dictionary["id"] = doc.id
-                
-                callback(dictionary)
+    @staticmethod
+    def get_document_realtime(collection_name: str, document_id: str, callback):
+        def temp_callback(doc_snapshot, changes, read_time):
+            if len(doc_snapshot) == 1:
+                doc = doc_snapshot[0]
+
+                if doc.exists:
+                    dictionary = doc.to_dict()
+                    dictionary["id"] = doc.id
+
+                    callback(dictionary)
+                else:
+                    callback(None)
             else:
                 callback(None)
-        else:
-            callback(None)
-            
-    doc_watch = get_documents_changes_realtime(collection_name=collection_name, document_id=document_id, callback=temp_callback)
 
-    return doc_watch
+        doc_watch = FirebaseStorageHelper.get_documents_changes_realtime(collection_name=collection_name, document_id=document_id, callback=temp_callback)
 
+        return doc_watch
 
-def get_document_changes_realtime(collection_name: str, document_id: str, callback):
-    def temp_callback(doc_snapshot, changes, read_time):
-        if len(doc_snapshot) == 1:
-            doc = doc_snapshot[0]
-
-            if doc.exists:
-                dictionary = doc.to_dict()
-                dictionary["id"] = doc.id
-
-                callback(dictionary, changes, read_time)
+    @staticmethod
+    def get_document_changes_realtime(collection_name: str, document_id: str, callback):
+        def temp_callback(doc_snapshot, changes, read_time):
+            if len(doc_snapshot) == 1:
+                doc = doc_snapshot[0]
+
+                if doc.exists:
+                    dictionary = doc.to_dict()
+                    dictionary["id"] = doc.id
+
+                    callback(dictionary, changes, read_time)
+                else:
+                    callback(None, changes, read_time)
             else:
                 callback(None, changes, read_time)
-        else:
-            callback(None, changes, read_time)
-
-    doc_watch = get_documents_changes_realtime(collection_name=collection_name, document_id=document_id, callback=temp_callback)
-
-    return doc_watch
 
+        doc_watch = FirebaseStorageHelper.get_documents_changes_realtime(collection_name=collection_name, document_id=document_id, callback=temp_callback)
 
-def get_documents_changes_realtime(collection_name: str, document_id: str, callback):
-    def temp_callback(doc_snapshot, changes, read_time):
-        callback(doc_snapshot, changes, read_time)
+        return doc_watch
 
-    doc_watch = core.get_document_realtime(
-        collection_name=collection_name, document_id=document_id, callback=temp_callback
-    )
+    @staticmethod
+    def get_documents_changes_realtime(collection_name: str, document_id: str, callback):
+        def temp_callback(doc_snapshot, changes, read_time):
+            callback(doc_snapshot, changes, read_time)
 
-    return doc_watch
+        doc_watch = FirebaseStorageCore.get_document_realtime(
+            collection_name=collection_name, document_id=document_id, callback=temp_callback
+        )
 
+        return doc_watch
 
-def get_documents(collection_name: str, filters: Dict[str, any] = None) -> List[dict]:
-    docs = core.get_documents(
-        collection_name=collection_name, filters=filters
-    )
+    def get_documents(collection_name: str, filters: Dict[str, any] = None) -> List[dict]:
+        docs = FirebaseStorageCore.get_documents(
+            collection_name=collection_name, filters=filters
+        )
 
-    if docs:
-        docs_dict: List[dict] = []
-        for doc in docs:
-            dictionary = doc.to_dict()
-            dictionary["id"] = doc.id
-            docs_dict.append(dictionary)
-        return docs_dict
+        if docs:
+            docs_dict: List[dict] = []
+            for doc in docs:
+                dictionary = doc.to_dict()
+                dictionary["id"] = doc.id
+                docs_dict.append(dictionary)
+            return docs_dict
 
-    return []
+        return []
```

### Comparing `aipkgs_firebase-0.0.9/aipkgs_firebase/storage/root.py` & `aipkgs_firebase-1.0.3/aipkgs_firebase/storage/root.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,77 +1,96 @@
-from typing import Dict, List
+from typing import Dict, List, Optional
 
-from aipkgs_firebase.storage import core, helpers
+from aipkgs_firebase.storage.core import FirebaseStorageCore
+from aipkgs_firebase.storage.helpers import FirebaseStorageHelper
 
 
-class Root:
-
+class FirebaseRootModel:
     collection_name = ""
 
+    @staticmethod
     def __init__(self, collection_name: str = None) -> None:
         self.collection_name = collection_name
 
+    @staticmethod
     def exists(self, document_id: str) -> bool:
-        return core.document_exists(
+        return FirebaseStorageCore.document_exists(
             collection_name=self.collection_name, document_id=document_id
         )
 
+    @staticmethod
     def exists_where(self, filters: Dict[str, any]) -> bool:
-        return helpers.document_exists(
+        return FirebaseStorageHelper.document_exists(
             collection_name=self.collection_name, filters=filters
         )
 
-    def get_document(self, document_id: str) -> dict:
-        return helpers.get_document(
+    @staticmethod
+    def get_document(self, document_id: str) -> Optional[dict]:
+        return FirebaseStorageHelper.get_document(
             collection_name=self.collection_name, document_id=document_id
         )
 
+    @staticmethod
+    def get_document_where(self, filters: Dict[str, any]) -> dict:
+        return FirebaseStorageHelper.get_document_where(
+            collection_name=self.collection_name, filters=filters
+        )
+
+    @staticmethod
     def get_document_realtime(self, document_id: str, callback):
         def temp_callback(document):
             callback(document)
-        return helpers.get_document_realtime(
+
+        return FirebaseStorageHelper.get_document_realtime(
             collection_name=self.collection_name, document_id=document_id, callback=temp_callback
         )
 
+    @staticmethod
     def get_document_changes_realtime(self, document_id: str, callback):
         def temp_callback(document, changes, read_time):
             callback(document, changes, read_time)
 
-        return helpers.get_document_changes_realtime(
+        return FirebaseStorageHelper.get_document_changes_realtime(
             collection_name=self.collection_name, document_id=document_id, callback=temp_callback
         )
 
+    @staticmethod
     def get_documents_changes_realtime(self, document_id: str, callback):
         def temp_callback(doc_snapshot, changes, read_time):
             callback(doc_snapshot, changes, read_time)
 
-        return helpers.get_documents_changes_realtime(
+        return FirebaseStorageHelper.get_documents_changes_realtime(
             collection_name=self.collection_name, document_id=document_id, callback=temp_callback
         )
 
+    @staticmethod
     def get_documents(self, filters: Dict[str, any] = None) -> List[dict]:
-        return helpers.get_documents(
+        return FirebaseStorageHelper.get_documents(
             collection_name=self.collection_name, filters=filters
         )
 
+    @staticmethod
     def create(self, dictionary: dict, document_id: str = None) -> bool:
-        return core.create_document_from_data(
+        return FirebaseStorageCore.create_document_from_data(
             dictionary_data=dictionary,
             collection_name=self.collection_name,
             document_id=document_id,
         )
 
+    @staticmethod
     def update(self, dictionary: dict, document_id: str):
-        core.update_document_with_data(
+        FirebaseStorageCore.update_document_with_data(
             dictionary_data=dictionary,
             collection_name=self.collection_name,
             document_id=document_id,
         )
 
+    @staticmethod
     def remove(self, document_id: str):
-        core.remove_document(
+        FirebaseStorageCore.remove_document(
             collection_name=self.collection_name, document_id=document_id
         )
 
+    @staticmethod
     def remove_all(self):
-        core.remove_documents(
+        FirebaseStorageCore.remove_documents(
             collection_name=self.collection_name)
```

### Comparing `aipkgs_firebase-0.0.9/PKG-INFO` & `aipkgs_firebase-1.0.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: aipkgs-firebase
-Version: 0.0.9
-Summary: 
+Version: 1.0.3
+Summary: A utility package for interacting with Firebase, specifically Firestore, in a more streamlined and efficient manner.
 Home-page: https://gitlab.com/aipy/public/packages.git
 License: MIT
 Keywords: ai
 Author: Alexy
 Author-email: alexy.ib@outlook.com
 Requires-Python: >=3.11.3,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

