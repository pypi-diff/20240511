# Comparing `tmp/rocketchat_async-4.0.0.tar.gz` & `tmp/rocketchat_async-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocketchat_async-4.0.0.tar", max compression
+gzip compressed data, was "rocketchat_async-4.1.0.tar", max compression
```

## Comparing `rocketchat_async-4.0.0.tar` & `rocketchat_async-4.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1079 2022-12-29 18:27:14.756067 rocketchat_async-4.0.0/LICENSE
--rw-r--r--   0        0        0     3482 2024-03-02 17:28:13.501520 rocketchat_async-4.0.0/README.md
--rw-r--r--   0        0        0      610 2024-03-02 17:28:13.505520 rocketchat_async-4.0.0/pyproject.toml
--rw-r--r--   0        0        0       22 2022-12-29 15:03:17.541726 rocketchat_async-4.0.0/rocketchat_async/.gitignore
--rw-r--r--   0        0        0       45 2022-12-29 19:30:01.886734 rocketchat_async-4.0.0/rocketchat_async/__init__.py
--rw-r--r--   0        0        0     1013 2022-12-30 15:35:26.313806 rocketchat_async-4.0.0/rocketchat_async/constants.py
--rw-r--r--   0        0        0     4714 2024-03-02 17:28:13.505520 rocketchat_async-4.0.0/rocketchat_async/core.py
--rw-r--r--   0        0        0     2695 2024-01-28 15:50:25.963742 rocketchat_async-4.0.0/rocketchat_async/dispatcher.py
--rw-r--r--   0        0        0     8064 2024-03-02 17:28:13.505520 rocketchat_async-4.0.0/rocketchat_async/methods.py
--rw-r--r--   0        0        0     4311 1970-01-01 00:00:00.000000 rocketchat_async-4.0.0/setup.py
--rw-r--r--   0        0        0     4348 1970-01-01 00:00:00.000000 rocketchat_async-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2022-12-29 18:27:14.756067 rocketchat_async-4.1.0/LICENSE
+-rw-r--r--   0        0        0     3543 2024-05-11 19:14:06.433465 rocketchat_async-4.1.0/README.md
+-rw-r--r--   0        0        0      610 2024-05-11 19:14:43.165933 rocketchat_async-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2022-12-29 15:03:17.541726 rocketchat_async-4.1.0/rocketchat_async/.gitignore
+-rw-r--r--   0        0        0       45 2022-12-29 19:30:01.886734 rocketchat_async-4.1.0/rocketchat_async/__init__.py
+-rw-r--r--   0        0        0     1013 2022-12-30 15:35:26.313806 rocketchat_async-4.1.0/rocketchat_async/constants.py
+-rw-r--r--   0        0        0     4741 2024-05-11 19:14:06.433465 rocketchat_async-4.1.0/rocketchat_async/core.py
+-rw-r--r--   0        0        0     2695 2024-01-28 15:50:25.963742 rocketchat_async-4.1.0/rocketchat_async/dispatcher.py
+-rw-r--r--   0        0        0     8198 2024-05-11 19:14:06.433465 rocketchat_async-4.1.0/rocketchat_async/methods.py
+-rw-r--r--   0        0        0     4372 1970-01-01 00:00:00.000000 rocketchat_async-4.1.0/setup.py
+-rw-r--r--   0        0        0     4409 1970-01-01 00:00:00.000000 rocketchat_async-4.1.0/PKG-INFO
```

### Comparing `rocketchat_async-4.0.0/LICENSE` & `rocketchat_async-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rocketchat_async-4.0.0/README.md` & `rocketchat_async-4.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -74,17 +74,17 @@
 
 Send a text message to a channel.
 
 #### `RocketChat.send_reaction(orig_msg_id, emoji)`
 
 Send a reaction to a specific message.
 
-#### `RocketChat.send_typing_event(channel_id)`
+#### `RocketChat.send_typing_event(channel_id, thread_id=None)`
 
-Send the "typing" event to a channel.
+Send the "typing" event to a channel or to a specified thread within that channel.
 
 #### `RocketChat.subscribe_to_channel_messages(channel_id, callback)`
 
 Subscribe to all messages in the given channel. Returns the subscription ID.
 
 The provided callback should accept eight arguments: `channel_id`,
 `sender_id`, `msg_id`, `thread_id`, `msg_text`, `msg_qualifier`
```

### Comparing `rocketchat_async-4.0.0/pyproject.toml` & `rocketchat_async-4.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rocketchat-async"
-version = "4.0.0"
+version = "4.1.0"
 description = "asyncio-based Python wrapper for the Rocket.Chat Realtime API."
 authors = ["Hynek Urban <hynek.urban@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "rocketchat_async"}]
 homepage = "https://github.com/hynek-urban/rocketchat-async"
 documentation = "https://github.com/hynek-urban/rocketchat-async"
```

### Comparing `rocketchat_async-4.0.0/rocketchat_async/constants.py` & `rocketchat_async-4.1.0/rocketchat_async/constants.py`

 * *Files identical despite different names*

### Comparing `rocketchat_async-4.0.0/rocketchat_async/core.py` & `rocketchat_async-4.1.0/rocketchat_async/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,17 +92,17 @@
         """Send a text message to a channel."""
         await SendMessage.call(self._dispatcher, text, channel_id, thread_id)
 
     async def send_reaction(self, orig_msg_id, emoji):
         """Send a reaction to a specific message."""
         await SendReaction.call(self._dispatcher, orig_msg_id, emoji)
 
-    async def send_typing_event(self, channel_id):
+    async def send_typing_event(self, channel_id, thread_id=None):
         """Send the `typing` event to a channel."""
-        await SendTypingEvent.call(self._dispatcher, channel_id, self.username)
+        await SendTypingEvent.call(self._dispatcher, channel_id, self.username, thread_id)
 
     async def subscribe_to_channel_messages(self, channel_id, callback):
         """
         Subscribe to all messages in the given channel.
 
         Returns the subscription ID.
```

### Comparing `rocketchat_async-4.0.0/rocketchat_async/dispatcher.py` & `rocketchat_async-4.1.0/rocketchat_async/dispatcher.py`

 * *Files identical despite different names*

### Comparing `rocketchat_async-4.0.0/rocketchat_async/methods.py` & `rocketchat_async-4.1.0/rocketchat_async/methods.py`

 * *Files 8% similar despite different names*

```diff
@@ -163,31 +163,34 @@
         await dispatcher.call_method(msg)
 
 
 class SendTypingEvent(RealtimeRequest):
     """Send the `typing` event to a channel."""
 
     @staticmethod
-    def _get_request_msg(msg_id, channel_id, username):
-        return {
+    def _get_request_msg(msg_id, channel_id, username, thread_id=None):
+        msg = {
             "msg": "method",
             "method": "stream-notify-room",
             "id": msg_id,
             "params": [
                 f'{channel_id}/user-activity',
                 username,
                 ["user-typing"],
                 {}
             ]
         }
+        if(thread_id):
+            msg["params"][-1]["tmid"] = thread_id
+        return msg
 
     @classmethod
-    async def call(cls, dispatcher, channel_id, username):
+    async def call(cls, dispatcher, channel_id, username, thread_id=None):
         msg_id = cls._get_new_id()
-        msg = cls._get_request_msg(msg_id, channel_id, username)
+        msg = cls._get_request_msg(msg_id, channel_id, username, thread_id)
         await dispatcher.call_method(msg, msg_id)
 
 
 class SubscribeToChannelMessages(RealtimeRequest):
     """Subscribe to all messages in the given channel."""
 
     @staticmethod
```

### Comparing `rocketchat_async-4.0.0/setup.py` & `rocketchat_async-4.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'rocketchat-async',
-    'version': '4.0.0',
+    'version': '4.1.0',
     'description': 'asyncio-based Python wrapper for the Rocket.Chat Realtime API.',
-    'long_description': '# rocketchat-async\n\nasyncio-based Python wrapper for the Rocket.Chat Realtime API.\n\nSupported Rocket.Chat versions: 6.x. (The library might also work or partially work with other versions.)\n\n## When should you use this library?\n\nUse this library if you:\n\n- want to integrate with Rocket.Chat from Python\n- are using [asyncio](https://docs.python.org/3/library/asyncio.html) to drive your code\n- want to use Rocket.Chat\'s efficient websockets-based Realtime API\n\n## Installation\n\n`pip install rocketchat-async`\n\n## Example usage\n\n```python\nimport asyncio\nimport random\nfrom rocketchat_async import RocketChat\n\n\ndef handle_message(channel_id, sender_id, msg_id, thread_id, msg, qualifier,\n                   unread, repeated):\n    """Simply print the message that arrived."""\n    print(msg)\n\n\nasync def main(address, username, password):\n    while True:\n        try:\n            rc = RocketChat()\n            await rc.start(address, username, password)\n            # Alternatively, use rc.resume for token-based authentication:\n            # await rc.resume(address, username, token)\n\n            # A possible workflow consists of two steps:\n            #\n            # 1. Set up the desired callbacks...\n            for channel_id, channel_type in await rc.get_channels():\n                await rc.subscribe_to_channel_messages(channel_id,\n                                                       handle_message)\n            # 2. ...and then simply wait for the registered events.\n            await rc.run_forever()\n        except (RocketChat.ConnectionClosed,\n                RocketChat.ConnectCallFailed) as e:\n            print(f\'Connection failed: {e}. Waiting a few seconds...\')\n            await asyncio.sleep(random.uniform(4, 8))\n            print(\'Reconnecting...\')\n\n\n# Side note: Don\'t forget to use the wss:// scheme when TLS is used.\nasyncio.run(main(\'ws://localhost:3000/websocket\', \'username\', \'password\'))\n```\n\n## API Overview\n\nBrief overview of the currently implemented methods.\n\nAs of now, Rocket.Chat\'s API is only covered partially (based on my original\nneeds). I am open to both feature requests as well as pull requests.\n\n### Methods\n\n#### `RocketChat.get_channels()`\n\nGet a list of channels the logged-in user is currently member of.\n\n#### `RocketChat.send_message(text, channel_id, thread_id=None)`\n\nSend a text message to a channel.\n\n#### `RocketChat.send_reaction(orig_msg_id, emoji)`\n\nSend a reaction to a specific message.\n\n#### `RocketChat.send_typing_event(channel_id)`\n\nSend the "typing" event to a channel.\n\n#### `RocketChat.subscribe_to_channel_messages(channel_id, callback)`\n\nSubscribe to all messages in the given channel. Returns the subscription ID.\n\nThe provided callback should accept eight arguments: `channel_id`,\n`sender_id`, `msg_id`, `thread_id`, `msg_text`, `msg_qualifier`\n and `repeated`. The qualifier can help to determine if e.g. the\nmessage is a system message about the user being removed from\nthe channel.  The `repeated` flag assists in distinguishing \nwhether the message has been received again as a result of \nthread replies, or if it is a new message post.\n\n#### `RocketChat.subscribe_to_channel_changes(callback)`\n\nSubscribe to all changes in channels. Returns the subscription ID.\n\nThe provided callback should accept two arguments: `channel_id`\nand `channel_qualifier`. The qualifier helps to determine e.g.\nif it\'s a direct message or a normal room.\n\n#### `RocketChat.unsubscribe(subscription_id)`\n\nCancel a subscription.\n',
+    'long_description': '# rocketchat-async\n\nasyncio-based Python wrapper for the Rocket.Chat Realtime API.\n\nSupported Rocket.Chat versions: 6.x. (The library might also work or partially work with other versions.)\n\n## When should you use this library?\n\nUse this library if you:\n\n- want to integrate with Rocket.Chat from Python\n- are using [asyncio](https://docs.python.org/3/library/asyncio.html) to drive your code\n- want to use Rocket.Chat\'s efficient websockets-based Realtime API\n\n## Installation\n\n`pip install rocketchat-async`\n\n## Example usage\n\n```python\nimport asyncio\nimport random\nfrom rocketchat_async import RocketChat\n\n\ndef handle_message(channel_id, sender_id, msg_id, thread_id, msg, qualifier,\n                   unread, repeated):\n    """Simply print the message that arrived."""\n    print(msg)\n\n\nasync def main(address, username, password):\n    while True:\n        try:\n            rc = RocketChat()\n            await rc.start(address, username, password)\n            # Alternatively, use rc.resume for token-based authentication:\n            # await rc.resume(address, username, token)\n\n            # A possible workflow consists of two steps:\n            #\n            # 1. Set up the desired callbacks...\n            for channel_id, channel_type in await rc.get_channels():\n                await rc.subscribe_to_channel_messages(channel_id,\n                                                       handle_message)\n            # 2. ...and then simply wait for the registered events.\n            await rc.run_forever()\n        except (RocketChat.ConnectionClosed,\n                RocketChat.ConnectCallFailed) as e:\n            print(f\'Connection failed: {e}. Waiting a few seconds...\')\n            await asyncio.sleep(random.uniform(4, 8))\n            print(\'Reconnecting...\')\n\n\n# Side note: Don\'t forget to use the wss:// scheme when TLS is used.\nasyncio.run(main(\'ws://localhost:3000/websocket\', \'username\', \'password\'))\n```\n\n## API Overview\n\nBrief overview of the currently implemented methods.\n\nAs of now, Rocket.Chat\'s API is only covered partially (based on my original\nneeds). I am open to both feature requests as well as pull requests.\n\n### Methods\n\n#### `RocketChat.get_channels()`\n\nGet a list of channels the logged-in user is currently member of.\n\n#### `RocketChat.send_message(text, channel_id, thread_id=None)`\n\nSend a text message to a channel.\n\n#### `RocketChat.send_reaction(orig_msg_id, emoji)`\n\nSend a reaction to a specific message.\n\n#### `RocketChat.send_typing_event(channel_id, thread_id=None)`\n\nSend the "typing" event to a channel or to a specified thread within that channel.\n\n#### `RocketChat.subscribe_to_channel_messages(channel_id, callback)`\n\nSubscribe to all messages in the given channel. Returns the subscription ID.\n\nThe provided callback should accept eight arguments: `channel_id`,\n`sender_id`, `msg_id`, `thread_id`, `msg_text`, `msg_qualifier`\n and `repeated`. The qualifier can help to determine if e.g. the\nmessage is a system message about the user being removed from\nthe channel.  The `repeated` flag assists in distinguishing \nwhether the message has been received again as a result of \nthread replies, or if it is a new message post.\n\n#### `RocketChat.subscribe_to_channel_changes(callback)`\n\nSubscribe to all changes in channels. Returns the subscription ID.\n\nThe provided callback should accept two arguments: `channel_id`\nand `channel_qualifier`. The qualifier helps to determine e.g.\nif it\'s a direct message or a normal room.\n\n#### `RocketChat.unsubscribe(subscription_id)`\n\nCancel a subscription.\n',
     'author': 'Hynek Urban',
     'author_email': 'hynek.urban@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/hynek-urban/rocketchat-async',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `rocketchat_async-4.0.0/PKG-INFO` & `rocketchat_async-4.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocketchat-async
-Version: 4.0.0
+Version: 4.1.0
 Summary: asyncio-based Python wrapper for the Rocket.Chat Realtime API.
 Home-page: https://github.com/hynek-urban/rocketchat-async
 License: MIT
 Author: Hynek Urban
 Author-email: hynek.urban@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
@@ -95,17 +95,17 @@
 
 Send a text message to a channel.
 
 #### `RocketChat.send_reaction(orig_msg_id, emoji)`
 
 Send a reaction to a specific message.
 
-#### `RocketChat.send_typing_event(channel_id)`
+#### `RocketChat.send_typing_event(channel_id, thread_id=None)`
 
-Send the "typing" event to a channel.
+Send the "typing" event to a channel or to a specified thread within that channel.
 
 #### `RocketChat.subscribe_to_channel_messages(channel_id, callback)`
 
 Subscribe to all messages in the given channel. Returns the subscription ID.
 
 The provided callback should accept eight arguments: `channel_id`,
 `sender_id`, `msg_id`, `thread_id`, `msg_text`, `msg_qualifier`
```

