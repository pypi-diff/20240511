# Comparing `tmp/python_telegram_broadcast-0.9.6.tar.gz` & `tmp/python_telegram_broadcast-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_telegram_broadcast-0.9.6.tar", last modified: Wed May  8 08:52:47 2024, max compression
+gzip compressed data, was "python_telegram_broadcast-0.9.7.tar", last modified: Sat May 11 14:22:00 2024, max compression
```

## Comparing `python_telegram_broadcast-0.9.6.tar` & `python_telegram_broadcast-0.9.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-08 08:52:47.910956 python_telegram_broadcast-0.9.6/
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     1067 2024-05-06 01:52:00.000000 python_telegram_broadcast-0.9.6/LICENSE
--rw-r--r--   0 jonah     (1000) jonah     (1000)     3782 2024-05-08 08:52:47.910956 python_telegram_broadcast-0.9.6/PKG-INFO
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     3193 2024-05-08 08:51:51.000000 python_telegram_broadcast-0.9.6/README.md
-drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-08 08:52:47.910956 python_telegram_broadcast-0.9.6/python_telegram_broadcast/
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     4119 2024-05-08 08:48:37.000000 python_telegram_broadcast-0.9.6/python_telegram_broadcast/__init__.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     4039 2024-05-07 06:58:19.000000 python_telegram_broadcast-0.9.6/python_telegram_broadcast/custom_dataclass.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     1616 2024-05-06 08:35:01.000000 python_telegram_broadcast-0.9.6/python_telegram_broadcast/custom_exception.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     3338 2024-05-07 06:58:49.000000 python_telegram_broadcast-0.9.6/python_telegram_broadcast/custom_util.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     4223 2024-05-08 08:37:54.000000 python_telegram_broadcast-0.9.6/python_telegram_broadcast/main.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)    19099 2024-05-08 08:33:16.000000 python_telegram_broadcast-0.9.6/python_telegram_broadcast/send_method.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)    17860 2024-05-07 06:57:50.000000 python_telegram_broadcast-0.9.6/python_telegram_broadcast/strategy.py
-drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-08 08:52:47.910956 python_telegram_broadcast-0.9.6/python_telegram_broadcast.egg-info/
--rw-r--r--   0 jonah     (1000) jonah     (1000)     3782 2024-05-08 08:52:47.000000 python_telegram_broadcast-0.9.6/python_telegram_broadcast.egg-info/PKG-INFO
--rw-rw-r--   0 jonah     (1000) jonah     (1000)      554 2024-05-08 08:52:47.000000 python_telegram_broadcast-0.9.6/python_telegram_broadcast.egg-info/SOURCES.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)        1 2024-05-08 08:52:47.000000 python_telegram_broadcast-0.9.6/python_telegram_broadcast.egg-info/dependency_links.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)       33 2024-05-08 08:52:47.000000 python_telegram_broadcast-0.9.6/python_telegram_broadcast.egg-info/requires.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)       26 2024-05-08 08:52:47.000000 python_telegram_broadcast-0.9.6/python_telegram_broadcast.egg-info/top_level.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)       38 2024-05-08 08:52:47.910956 python_telegram_broadcast-0.9.6/setup.cfg
--rw-rw-r--   0 jonah     (1000) jonah     (1000)      952 2024-05-08 08:52:19.000000 python_telegram_broadcast-0.9.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 14:22:00.194429 python_telegram_broadcast-0.9.7/
+-rw-rw-rw-   0        0        0     1088 2024-05-06 01:23:14.000000 python_telegram_broadcast-0.9.7/LICENSE
+-rw-rw-rw-   0        0        0     3917 2024-05-11 14:22:00.190575 python_telegram_broadcast-0.9.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3310 2024-05-11 14:19:25.000000 python_telegram_broadcast-0.9.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 14:22:00.170199 python_telegram_broadcast-0.9.7/python_telegram_broadcast/
+-rw-rw-rw-   0        0        0     4225 2024-05-11 14:19:25.000000 python_telegram_broadcast-0.9.7/python_telegram_broadcast/__init__.py
+-rw-rw-rw-   0        0        0     4039 2024-05-11 14:19:25.000000 python_telegram_broadcast-0.9.7/python_telegram_broadcast/custom_dataclass.py
+-rw-rw-rw-   0        0        0     1616 2024-05-11 14:19:25.000000 python_telegram_broadcast-0.9.7/python_telegram_broadcast/custom_exception.py
+-rw-rw-rw-   0        0        0     3338 2024-05-11 14:19:25.000000 python_telegram_broadcast-0.9.7/python_telegram_broadcast/custom_util.py
+-rw-rw-rw-   0        0        0     4223 2024-05-11 14:19:25.000000 python_telegram_broadcast-0.9.7/python_telegram_broadcast/main.py
+-rw-rw-rw-   0        0        0    19099 2024-05-11 14:19:25.000000 python_telegram_broadcast-0.9.7/python_telegram_broadcast/send_method.py
+-rw-rw-rw-   0        0        0    18264 2024-05-11 14:20:26.000000 python_telegram_broadcast-0.9.7/python_telegram_broadcast/strategy.py
+drwxrwxrwx   0        0        0        0 2024-05-11 14:22:00.187342 python_telegram_broadcast-0.9.7/python_telegram_broadcast.egg-info/
+-rw-rw-rw-   0        0        0     3917 2024-05-11 14:22:00.000000 python_telegram_broadcast-0.9.7/python_telegram_broadcast.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      554 2024-05-11 14:22:00.000000 python_telegram_broadcast-0.9.7/python_telegram_broadcast.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 14:22:00.000000 python_telegram_broadcast-0.9.7/python_telegram_broadcast.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-11 14:22:00.000000 python_telegram_broadcast-0.9.7/python_telegram_broadcast.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-11 14:22:00.000000 python_telegram_broadcast-0.9.7/python_telegram_broadcast.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-11 14:22:00.194429 python_telegram_broadcast-0.9.7/setup.cfg
+-rw-rw-rw-   0        0        0      952 2024-05-11 14:21:11.000000 python_telegram_broadcast-0.9.7/setup.py
```

### Comparing `python_telegram_broadcast-0.9.6/PKG-INFO` & `python_telegram_broadcast-0.9.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,135 +1,135 @@
-Metadata-Version: 2.1
-Name: python_telegram_broadcast
-Version: 0.9.6
-Summary: Package that wraps the python-telegram-bot library to make broadcasting easier.
-Author: jonah_whaler_2348
-Author-email: jk_saga@proton.me
-License: MIT
-Keywords: python,telegram,broadcast,bot
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: python-telegram-bot==21.1.1
-Requires-Dist: mypy
-
-![my-logo](https://jonahtzuchi.github.io/python-telegram-broadcast/logo-mini.jpg "Python-Telegram-Broadcast-Logo")
-
-# Python Telegram Broadcast
-
-This is a simple Python package that build on top of [python-telegram-bot](https://pypi.org/project/python-telegram-bot/) to make broadcasting easier.
-
-
-## Features
-- Broadcast message to multiple users
-- Support media type:
-  - Text
-  - Photo
-  - Document
-  - Video
-- Support broadcast strategy:
-  - Asynchronous Sequentially
-  - Asynchronous Process Pool
-  - Asynchronous Multiprocessing Pool
-
-## Dependencies
-- [python-telegram-bot](https://pypi.org/project/python-telegram-bot/)=21.1.1
-- [mypy](https://pypi.org/project/mypy/)
-
-## Installation
-  ```bash
-  pip3 install python_telegram_broadcast
-  ```
-
-## Example
-
-### Get File ID from Telegram
-```python
-import asyncio
-from python_telegram_broadcast import (
-    get_file_id, select_broadcast_method, BroadcastMethodType
-)
-
-
-def wrapper(token, method, target_id, payload):
-  caption = ""
-  seconds = 0.0 # 0.0 means no timeout
-  max_retry = 5 # Maximum retry
-  
-  loop = asyncio.get_event_loop()
-  return loop.run_until_complete(
-      get_file_id(
-          token, method, target_id, payload, caption, seconds, max_retry
-      )
-  )
-  
-
-if __name__ == "__main__":
-  bot_token: str = "TELEGRAM_BOT_TOKEN"   # << Change to your bot token
-  user_telegram_id: int = 123456789       # << Change to your telegram id
-  file_path: str = ""                     # << Change to your file path or the URL of your file
-  
-  broadcast_method = select_broadcast_method(BroadcastMethodType.PHOTO)
-  
-  # If file_path is a URL
-  file_id = wrapper(bot_token, broadcast_method, user_telegram_id, file_path)
-  
-  print(file_id)
-```
-    
-
-### Broadcast Photo
-```python
-from typing import Tuple
-from python_telegram_broadcast import (
-    handle_broadcast,
-    select_broadcast_strategy, BroadcastStrategyType,
-    write_sent_result
-)
-
-def broadcast_wrapper(token, method, stg, slist, payload):
-    loop = asyncio.get_event_loop()
-    return loop.run_until_complete(
-        handle_broadcast(
-            slist, token, method, stg, payload, "...", 
-            use_multiproc=False, use_nproc=1, seconds=0.0, max_retry=5
-        )
-    )
-
-# Use bot_token, broadcast_method, file_path from the previous example!!!
-export_path = "./asset"
-broadcast_strategy = select_broadcast_strategy(BroadcastStrategyType.ASYNCIO_SEQUENTIAL)
-# Read subscriber list from file, but you can also read from database of your choice
-subscriber_list: list[Tuple[int, str]] = []
-with open("./asset/subscriber.txt", "r") as file:
-    header = file.readline()
-    while True:
-        line = file.readline()
-        if not line:
-            break
-        telegram_id, username = line.strip().split(",")
-        subscriber_list.append((int(telegram_id), username))
-
-s, f = broadcast_wrapper(
-    bot_token, broadcast_method, broadcast_strategy,
-    subscriber_list,
-    file_id
-)
-for S in s:
-    print(f"Success: {s}")
-
-for F in f:
-    print(f"Failed: {f}")
-
-if len(f) > 0:
-    write_sent_result(f"{export_path}/result_{file_path}.txt", f, file_path)
-
-```
-
-## Tests
-TODO
-
-## Source Code
-- https://github.com/JonahTzuChi/python-telegram-broadcast
+Metadata-Version: 2.1
+Name: python_telegram_broadcast
+Version: 0.9.7
+Summary: Package that wraps the python-telegram-bot library to make broadcasting easier.
+Author: jonah_whaler_2348
+Author-email: jk_saga@proton.me
+License: MIT
+Keywords: python,telegram,broadcast,bot
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: python-telegram-bot==21.1.1
+Requires-Dist: mypy
+
+![my-logo](https://jonahtzuchi.github.io/python-telegram-broadcast/logo-mini.jpg "Python-Telegram-Broadcast-Logo")
+
+# Python Telegram Broadcast
+
+This is a simple Python package that build on top of [python-telegram-bot](https://pypi.org/project/python-telegram-bot/) to make broadcasting easier.
+
+
+## Features
+- Broadcast message to multiple users
+- Support media type:
+  - Text
+  - Photo
+  - Document
+  - Video
+- Support broadcast strategy:
+  - Asynchronous Sequentially
+  - Asynchronous Process Pool
+  - Asynchronous Multiprocessing Pool
+
+## Dependencies
+- [python-telegram-bot](https://pypi.org/project/python-telegram-bot/)=21.1.1
+- [mypy](https://pypi.org/project/mypy/)
+
+## Installation
+  ```bash
+  pip3 install python_telegram_broadcast
+  ```
+
+## Example
+
+### Get File ID from Telegram
+```python
+import asyncio
+from python_telegram_broadcast import (
+    get_file_id, select_broadcast_method, BroadcastMethodType
+)
+
+
+def wrapper(token, method, target_id, payload):
+  caption = ""
+  seconds = 0.0 # 0.0 means no timeout
+  max_retry = 5 # Maximum retry
+  
+  loop = asyncio.get_event_loop()
+  return loop.run_until_complete(
+      get_file_id(
+          token, method, target_id, payload, caption, seconds, max_retry
+      )
+  )
+  
+
+if __name__ == "__main__":
+  bot_token: str = "TELEGRAM_BOT_TOKEN"   # << Change to your bot token
+  user_telegram_id: int = 123456789       # << Change to your telegram id
+  file_path: str = ""                     # << Change to your file path or the URL of your file
+  
+  broadcast_method = select_broadcast_method(BroadcastMethodType.PHOTO)
+  
+  # If file_path is a URL
+  file_id = wrapper(bot_token, broadcast_method, user_telegram_id, file_path)
+  
+  print(file_id)
+```
+    
+
+### Broadcast Photo
+```python
+from typing import Tuple
+from python_telegram_broadcast import (
+    handle_broadcast,
+    select_broadcast_strategy, BroadcastStrategyType,
+    write_sent_result
+)
+
+def broadcast_wrapper(token, method, stg, slist, payload):
+    loop = asyncio.get_event_loop()
+    return loop.run_until_complete(
+        handle_broadcast(
+            slist, token, method, stg, payload, "...", 
+            use_multiproc=False, use_nproc=1, seconds=0.0, max_retry=5
+        )
+    )
+
+# Use bot_token, broadcast_method, file_path from the previous example!!!
+export_path = "./asset"
+broadcast_strategy = select_broadcast_strategy(BroadcastStrategyType.ASYNCIO_SEQUENTIAL)
+# Read subscriber list from file, but you can also read from database of your choice
+subscriber_list: list[Tuple[int, str]] = []
+with open("./asset/subscriber.txt", "r") as file:
+    header = file.readline()
+    while True:
+        line = file.readline()
+        if not line:
+            break
+        telegram_id, username = line.strip().split(",")
+        subscriber_list.append((int(telegram_id), username))
+
+s, f = broadcast_wrapper(
+    bot_token, broadcast_method, broadcast_strategy,
+    subscriber_list,
+    file_id
+)
+for S in s:
+    print(f"Success: {s}")
+
+for F in f:
+    print(f"Failed: {f}")
+
+if len(f) > 0:
+    write_sent_result(f"{export_path}/result_{file_path}.txt", f, file_path)
+
+```
+
+## Tests
+TODO
+
+## Source Code
+- https://github.com/JonahTzuChi/python-telegram-broadcast
```

### Comparing `python_telegram_broadcast-0.9.6/README.md` & `python_telegram_broadcast-0.9.7/README.md`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-![my-logo](https://jonahtzuchi.github.io/python-telegram-broadcast/logo-mini.jpg "Python-Telegram-Broadcast-Logo")
-
-# Python Telegram Broadcast
-
-This is a simple Python package that build on top of [python-telegram-bot](https://pypi.org/project/python-telegram-bot/) to make broadcasting easier.
-
-
-## Features
-- Broadcast message to multiple users
-- Support media type:
-  - Text
-  - Photo
-  - Document
-  - Video
-- Support broadcast strategy:
-  - Asynchronous Sequentially
-  - Asynchronous Process Pool
-  - Asynchronous Multiprocessing Pool
-
-## Dependencies
-- [python-telegram-bot](https://pypi.org/project/python-telegram-bot/)=21.1.1
-- [mypy](https://pypi.org/project/mypy/)
-
-## Installation
-  ```bash
-  pip3 install python_telegram_broadcast
-  ```
-
-## Example
-
-### Get File ID from Telegram
-```python
-import asyncio
-from python_telegram_broadcast import (
-    get_file_id, select_broadcast_method, BroadcastMethodType
-)
-
-
-def wrapper(token, method, target_id, payload):
-  caption = ""
-  seconds = 0.0 # 0.0 means no timeout
-  max_retry = 5 # Maximum retry
-  
-  loop = asyncio.get_event_loop()
-  return loop.run_until_complete(
-      get_file_id(
-          token, method, target_id, payload, caption, seconds, max_retry
-      )
-  )
-  
-
-if __name__ == "__main__":
-  bot_token: str = "TELEGRAM_BOT_TOKEN"   # << Change to your bot token
-  user_telegram_id: int = 123456789       # << Change to your telegram id
-  file_path: str = ""                     # << Change to your file path or the URL of your file
-  
-  broadcast_method = select_broadcast_method(BroadcastMethodType.PHOTO)
-  
-  # If file_path is a URL
-  file_id = wrapper(bot_token, broadcast_method, user_telegram_id, file_path)
-  
-  print(file_id)
-```
-    
-
-### Broadcast Photo
-```python
-from typing import Tuple
-from python_telegram_broadcast import (
-    handle_broadcast,
-    select_broadcast_strategy, BroadcastStrategyType,
-    write_sent_result
-)
-
-def broadcast_wrapper(token, method, stg, slist, payload):
-    loop = asyncio.get_event_loop()
-    return loop.run_until_complete(
-        handle_broadcast(
-            slist, token, method, stg, payload, "...", 
-            use_multiproc=False, use_nproc=1, seconds=0.0, max_retry=5
-        )
-    )
-
-# Use bot_token, broadcast_method, file_path from the previous example!!!
-export_path = "./asset"
-broadcast_strategy = select_broadcast_strategy(BroadcastStrategyType.ASYNCIO_SEQUENTIAL)
-# Read subscriber list from file, but you can also read from database of your choice
-subscriber_list: list[Tuple[int, str]] = []
-with open("./asset/subscriber.txt", "r") as file:
-    header = file.readline()
-    while True:
-        line = file.readline()
-        if not line:
-            break
-        telegram_id, username = line.strip().split(",")
-        subscriber_list.append((int(telegram_id), username))
-
-s, f = broadcast_wrapper(
-    bot_token, broadcast_method, broadcast_strategy,
-    subscriber_list,
-    file_id
-)
-for S in s:
-    print(f"Success: {s}")
-
-for F in f:
-    print(f"Failed: {f}")
-
-if len(f) > 0:
-    write_sent_result(f"{export_path}/result_{file_path}.txt", f, file_path)
-
-```
-
-## Tests
-TODO
-
-## Source Code
+![my-logo](https://jonahtzuchi.github.io/python-telegram-broadcast/logo-mini.jpg "Python-Telegram-Broadcast-Logo")
+
+# Python Telegram Broadcast
+
+This is a simple Python package that build on top of [python-telegram-bot](https://pypi.org/project/python-telegram-bot/) to make broadcasting easier.
+
+
+## Features
+- Broadcast message to multiple users
+- Support media type:
+  - Text
+  - Photo
+  - Document
+  - Video
+- Support broadcast strategy:
+  - Asynchronous Sequentially
+  - Asynchronous Process Pool
+  - Asynchronous Multiprocessing Pool
+
+## Dependencies
+- [python-telegram-bot](https://pypi.org/project/python-telegram-bot/)=21.1.1
+- [mypy](https://pypi.org/project/mypy/)
+
+## Installation
+  ```bash
+  pip3 install python_telegram_broadcast
+  ```
+
+## Example
+
+### Get File ID from Telegram
+```python
+import asyncio
+from python_telegram_broadcast import (
+    get_file_id, select_broadcast_method, BroadcastMethodType
+)
+
+
+def wrapper(token, method, target_id, payload):
+  caption = ""
+  seconds = 0.0 # 0.0 means no timeout
+  max_retry = 5 # Maximum retry
+  
+  loop = asyncio.get_event_loop()
+  return loop.run_until_complete(
+      get_file_id(
+          token, method, target_id, payload, caption, seconds, max_retry
+      )
+  )
+  
+
+if __name__ == "__main__":
+  bot_token: str = "TELEGRAM_BOT_TOKEN"   # << Change to your bot token
+  user_telegram_id: int = 123456789       # << Change to your telegram id
+  file_path: str = ""                     # << Change to your file path or the URL of your file
+  
+  broadcast_method = select_broadcast_method(BroadcastMethodType.PHOTO)
+  
+  # If file_path is a URL
+  file_id = wrapper(bot_token, broadcast_method, user_telegram_id, file_path)
+  
+  print(file_id)
+```
+    
+
+### Broadcast Photo
+```python
+from typing import Tuple
+from python_telegram_broadcast import (
+    handle_broadcast,
+    select_broadcast_strategy, BroadcastStrategyType,
+    write_sent_result
+)
+
+def broadcast_wrapper(token, method, stg, slist, payload):
+    loop = asyncio.get_event_loop()
+    return loop.run_until_complete(
+        handle_broadcast(
+            slist, token, method, stg, payload, "...", 
+            use_multiproc=False, use_nproc=1, seconds=0.0, max_retry=5
+        )
+    )
+
+# Use bot_token, broadcast_method, file_path from the previous example!!!
+export_path = "./asset"
+broadcast_strategy = select_broadcast_strategy(BroadcastStrategyType.ASYNCIO_SEQUENTIAL)
+# Read subscriber list from file, but you can also read from database of your choice
+subscriber_list: list[Tuple[int, str]] = []
+with open("./asset/subscriber.txt", "r") as file:
+    header = file.readline()
+    while True:
+        line = file.readline()
+        if not line:
+            break
+        telegram_id, username = line.strip().split(",")
+        subscriber_list.append((int(telegram_id), username))
+
+s, f = broadcast_wrapper(
+    bot_token, broadcast_method, broadcast_strategy,
+    subscriber_list,
+    file_id
+)
+for S in s:
+    print(f"Success: {s}")
+
+for F in f:
+    print(f"Failed: {f}")
+
+if len(f) > 0:
+    write_sent_result(f"{export_path}/result_{file_path}.txt", f, file_path)
+
+```
+
+## Tests
+TODO
+
+## Source Code
 - https://github.com/JonahTzuChi/python-telegram-broadcast
```

### Comparing `python_telegram_broadcast-0.9.6/python_telegram_broadcast/__init__.py` & `python_telegram_broadcast-0.9.7/python_telegram_broadcast/__init__.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-"""
-MIT License
-
-Copyright (c) 2024 Jonah Whaler
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-"""
-
-__title__ = "python-telegram-broadcast"
-__author__ = "Jonah Whaler"
-__license__ = "MIT"
-__copyright__ = "Copyright (c) 2024 Jonah Whaler"
-
-import asyncio
-from typing import Tuple
-from .main import handle_broadcast, get_file_id
-from .send_method import BroadcastMethodType, select_broadcast_method, string_to_BroadcastMethodType
-from .strategy import BroadcastStrategyType, select_broadcast_strategy, string_to_BroadcastStrategyType
-from .custom_util import write_sent_result, evaluate_broadcast_stats
-from .custom_dataclass import JobResponse, BroadcastStats, ErrorInformation
-
-__all__ = [
-    "handle_broadcast", "get_file_id",
-    "select_broadcast_method", "BroadcastMethodType", "string_to_BroadcastMethodType",
-    "select_broadcast_strategy", "BroadcastStrategyType", "string_to_BroadcastStrategyType",
-    "write_sent_result", "evaluate_broadcast_stats",
-    "JobResponse", "BroadcastStats", "ErrorInformation"
-]
-
-
-def wrapper(token, method, target_id, payload):
-    caption = ""
-    seconds = 0.0  # 0.0 means no timeout
-    max_retry = 5  # Maximum retry
-
-    loop = asyncio.get_event_loop()
-    return loop.run_until_complete(
-        get_file_id(
-            token, method, target_id, payload, caption, seconds, max_retry
-        )
-    )
-
-
-def broadcast_wrapper(token, method, stg, slist, payload):
-    loop = asyncio.get_event_loop()
-    return loop.run_until_complete(
-        handle_broadcast(
-            slist, token, method, stg, payload, "...",
-            use_multiproc=False, use_nproc=1, seconds=0.0, max_retry=5
-        )
-    )
-
-
-# CLI: python3 -m python_telegram_broadcast.__init__
-if __name__ == "__main__":
-    bot_token: str = ""                             # << Change to your bot token
-    user_telegram_id: int = 12345678                # << Change to your telegram id
-    file_path: str = "./asset/sample_photo.jpeg"    # << Change to your file path or the URL of your file
-
-    broadcast_method = select_broadcast_method(BroadcastMethodType.PHOTO)
-
-    file_id = wrapper(bot_token, broadcast_method, user_telegram_id, file_path)
-
-    # Use bot_token, broadcast_method, file_path from the previous example!!!
-    export_path = "./asset"
-    broadcast_strategy = select_broadcast_strategy(BroadcastStrategyType.ASYNCIO_SEQUENTIAL)
-    # Read subscriber list from file, but you can also read from database of your choice
-    subscriber_list: list[Tuple[int, str]] = []
-    with open("./asset/subscriber.txt", "r") as file:
-        header = file.readline()
-        while True:
-            line = file.readline()
-            if not line:
-                break
-            telegram_id, username = line.strip().split(",")
-            subscriber_list.append((int(telegram_id), username))
-
-    s, f = broadcast_wrapper(
-        bot_token, broadcast_method, broadcast_strategy,
-        subscriber_list,
-        file_id
-    )
-    for S in s:
-        print(f"Success: {s}")
-
-    for F in f:
-        print(f"Failed: {f}")
-
-    if len(f) > 0:
-        write_sent_result(f"{export_path}/result_{file_path}.txt", f, file_path)
+"""
+MIT License
+
+Copyright (c) 2024 Jonah Whaler
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+
+__title__ = "python-telegram-broadcast"
+__author__ = "Jonah Whaler"
+__license__ = "MIT"
+__copyright__ = "Copyright (c) 2024 Jonah Whaler"
+
+import asyncio
+from typing import Tuple
+from .main import handle_broadcast, get_file_id
+from .send_method import BroadcastMethodType, select_broadcast_method, string_to_BroadcastMethodType
+from .strategy import BroadcastStrategyType, select_broadcast_strategy, string_to_BroadcastStrategyType
+from .custom_util import write_sent_result, evaluate_broadcast_stats
+from .custom_dataclass import JobResponse, BroadcastStats, ErrorInformation
+
+__all__ = [
+    "handle_broadcast", "get_file_id",
+    "select_broadcast_method", "BroadcastMethodType", "string_to_BroadcastMethodType",
+    "select_broadcast_strategy", "BroadcastStrategyType", "string_to_BroadcastStrategyType",
+    "write_sent_result", "evaluate_broadcast_stats",
+    "JobResponse", "BroadcastStats", "ErrorInformation"
+]
+
+
+def wrapper(token, method, target_id, payload):
+    caption = ""
+    seconds = 0.0  # 0.0 means no timeout
+    max_retry = 5  # Maximum retry
+
+    loop = asyncio.get_event_loop()
+    return loop.run_until_complete(
+        get_file_id(
+            token, method, target_id, payload, caption, seconds, max_retry
+        )
+    )
+
+
+def broadcast_wrapper(token, method, stg, slist, payload):
+    loop = asyncio.get_event_loop()
+    return loop.run_until_complete(
+        handle_broadcast(
+            slist, token, method, stg, payload, "...",
+            use_multiproc=False, use_nproc=1, seconds=0.0, max_retry=5
+        )
+    )
+
+
+# CLI: python3 -m python_telegram_broadcast.__init__
+if __name__ == "__main__":
+    bot_token: str = ""                             # << Change to your bot token
+    user_telegram_id: int = 12345678                # << Change to your telegram id
+    file_path: str = "./asset/sample_photo.jpeg"    # << Change to your file path or the URL of your file
+
+    broadcast_method = select_broadcast_method(BroadcastMethodType.PHOTO)
+
+    file_id = wrapper(bot_token, broadcast_method, user_telegram_id, file_path)
+
+    # Use bot_token, broadcast_method, file_path from the previous example!!!
+    export_path = "./asset"
+    broadcast_strategy = select_broadcast_strategy(BroadcastStrategyType.ASYNCIO_SEQUENTIAL)
+    # Read subscriber list from file, but you can also read from database of your choice
+    subscriber_list: list[Tuple[int, str]] = []
+    with open("./asset/subscriber.txt", "r") as file:
+        header = file.readline()
+        while True:
+            line = file.readline()
+            if not line:
+                break
+            telegram_id, username = line.strip().split(",")
+            subscriber_list.append((int(telegram_id), username))
+
+    s, f = broadcast_wrapper(
+        bot_token, broadcast_method, broadcast_strategy,
+        subscriber_list,
+        file_id
+    )
+    for S in s:
+        print(f"Success: {s}")
+
+    for F in f:
+        print(f"Failed: {f}")
+
+    if len(f) > 0:
+        write_sent_result(f"{export_path}/result_{file_path}.txt", f, file_path)
```

### Comparing `python_telegram_broadcast-0.9.6/python_telegram_broadcast/custom_dataclass.py` & `python_telegram_broadcast-0.9.7/python_telegram_broadcast/custom_dataclass.py`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.6/python_telegram_broadcast/custom_exception.py` & `python_telegram_broadcast-0.9.7/python_telegram_broadcast/custom_exception.py`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.6/python_telegram_broadcast/custom_util.py` & `python_telegram_broadcast-0.9.7/python_telegram_broadcast/custom_util.py`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.6/python_telegram_broadcast/main.py` & `python_telegram_broadcast-0.9.7/python_telegram_broadcast/main.py`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.6/python_telegram_broadcast/send_method.py` & `python_telegram_broadcast-0.9.7/python_telegram_broadcast/send_method.py`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.6/python_telegram_broadcast.egg-info/PKG-INFO` & `python_telegram_broadcast-0.9.7/python_telegram_broadcast.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,135 +1,135 @@
-Metadata-Version: 2.1
-Name: python-telegram-broadcast
-Version: 0.9.6
-Summary: Package that wraps the python-telegram-bot library to make broadcasting easier.
-Author: jonah_whaler_2348
-Author-email: jk_saga@proton.me
-License: MIT
-Keywords: python,telegram,broadcast,bot
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: python-telegram-bot==21.1.1
-Requires-Dist: mypy
-
-![my-logo](https://jonahtzuchi.github.io/python-telegram-broadcast/logo-mini.jpg "Python-Telegram-Broadcast-Logo")
-
-# Python Telegram Broadcast
-
-This is a simple Python package that build on top of [python-telegram-bot](https://pypi.org/project/python-telegram-bot/) to make broadcasting easier.
-
-
-## Features
-- Broadcast message to multiple users
-- Support media type:
-  - Text
-  - Photo
-  - Document
-  - Video
-- Support broadcast strategy:
-  - Asynchronous Sequentially
-  - Asynchronous Process Pool
-  - Asynchronous Multiprocessing Pool
-
-## Dependencies
-- [python-telegram-bot](https://pypi.org/project/python-telegram-bot/)=21.1.1
-- [mypy](https://pypi.org/project/mypy/)
-
-## Installation
-  ```bash
-  pip3 install python_telegram_broadcast
-  ```
-
-## Example
-
-### Get File ID from Telegram
-```python
-import asyncio
-from python_telegram_broadcast import (
-    get_file_id, select_broadcast_method, BroadcastMethodType
-)
-
-
-def wrapper(token, method, target_id, payload):
-  caption = ""
-  seconds = 0.0 # 0.0 means no timeout
-  max_retry = 5 # Maximum retry
-  
-  loop = asyncio.get_event_loop()
-  return loop.run_until_complete(
-      get_file_id(
-          token, method, target_id, payload, caption, seconds, max_retry
-      )
-  )
-  
-
-if __name__ == "__main__":
-  bot_token: str = "TELEGRAM_BOT_TOKEN"   # << Change to your bot token
-  user_telegram_id: int = 123456789       # << Change to your telegram id
-  file_path: str = ""                     # << Change to your file path or the URL of your file
-  
-  broadcast_method = select_broadcast_method(BroadcastMethodType.PHOTO)
-  
-  # If file_path is a URL
-  file_id = wrapper(bot_token, broadcast_method, user_telegram_id, file_path)
-  
-  print(file_id)
-```
-    
-
-### Broadcast Photo
-```python
-from typing import Tuple
-from python_telegram_broadcast import (
-    handle_broadcast,
-    select_broadcast_strategy, BroadcastStrategyType,
-    write_sent_result
-)
-
-def broadcast_wrapper(token, method, stg, slist, payload):
-    loop = asyncio.get_event_loop()
-    return loop.run_until_complete(
-        handle_broadcast(
-            slist, token, method, stg, payload, "...", 
-            use_multiproc=False, use_nproc=1, seconds=0.0, max_retry=5
-        )
-    )
-
-# Use bot_token, broadcast_method, file_path from the previous example!!!
-export_path = "./asset"
-broadcast_strategy = select_broadcast_strategy(BroadcastStrategyType.ASYNCIO_SEQUENTIAL)
-# Read subscriber list from file, but you can also read from database of your choice
-subscriber_list: list[Tuple[int, str]] = []
-with open("./asset/subscriber.txt", "r") as file:
-    header = file.readline()
-    while True:
-        line = file.readline()
-        if not line:
-            break
-        telegram_id, username = line.strip().split(",")
-        subscriber_list.append((int(telegram_id), username))
-
-s, f = broadcast_wrapper(
-    bot_token, broadcast_method, broadcast_strategy,
-    subscriber_list,
-    file_id
-)
-for S in s:
-    print(f"Success: {s}")
-
-for F in f:
-    print(f"Failed: {f}")
-
-if len(f) > 0:
-    write_sent_result(f"{export_path}/result_{file_path}.txt", f, file_path)
-
-```
-
-## Tests
-TODO
-
-## Source Code
-- https://github.com/JonahTzuChi/python-telegram-broadcast
+Metadata-Version: 2.1
+Name: python-telegram-broadcast
+Version: 0.9.7
+Summary: Package that wraps the python-telegram-bot library to make broadcasting easier.
+Author: jonah_whaler_2348
+Author-email: jk_saga@proton.me
+License: MIT
+Keywords: python,telegram,broadcast,bot
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: python-telegram-bot==21.1.1
+Requires-Dist: mypy
+
+![my-logo](https://jonahtzuchi.github.io/python-telegram-broadcast/logo-mini.jpg "Python-Telegram-Broadcast-Logo")
+
+# Python Telegram Broadcast
+
+This is a simple Python package that build on top of [python-telegram-bot](https://pypi.org/project/python-telegram-bot/) to make broadcasting easier.
+
+
+## Features
+- Broadcast message to multiple users
+- Support media type:
+  - Text
+  - Photo
+  - Document
+  - Video
+- Support broadcast strategy:
+  - Asynchronous Sequentially
+  - Asynchronous Process Pool
+  - Asynchronous Multiprocessing Pool
+
+## Dependencies
+- [python-telegram-bot](https://pypi.org/project/python-telegram-bot/)=21.1.1
+- [mypy](https://pypi.org/project/mypy/)
+
+## Installation
+  ```bash
+  pip3 install python_telegram_broadcast
+  ```
+
+## Example
+
+### Get File ID from Telegram
+```python
+import asyncio
+from python_telegram_broadcast import (
+    get_file_id, select_broadcast_method, BroadcastMethodType
+)
+
+
+def wrapper(token, method, target_id, payload):
+  caption = ""
+  seconds = 0.0 # 0.0 means no timeout
+  max_retry = 5 # Maximum retry
+  
+  loop = asyncio.get_event_loop()
+  return loop.run_until_complete(
+      get_file_id(
+          token, method, target_id, payload, caption, seconds, max_retry
+      )
+  )
+  
+
+if __name__ == "__main__":
+  bot_token: str = "TELEGRAM_BOT_TOKEN"   # << Change to your bot token
+  user_telegram_id: int = 123456789       # << Change to your telegram id
+  file_path: str = ""                     # << Change to your file path or the URL of your file
+  
+  broadcast_method = select_broadcast_method(BroadcastMethodType.PHOTO)
+  
+  # If file_path is a URL
+  file_id = wrapper(bot_token, broadcast_method, user_telegram_id, file_path)
+  
+  print(file_id)
+```
+    
+
+### Broadcast Photo
+```python
+from typing import Tuple
+from python_telegram_broadcast import (
+    handle_broadcast,
+    select_broadcast_strategy, BroadcastStrategyType,
+    write_sent_result
+)
+
+def broadcast_wrapper(token, method, stg, slist, payload):
+    loop = asyncio.get_event_loop()
+    return loop.run_until_complete(
+        handle_broadcast(
+            slist, token, method, stg, payload, "...", 
+            use_multiproc=False, use_nproc=1, seconds=0.0, max_retry=5
+        )
+    )
+
+# Use bot_token, broadcast_method, file_path from the previous example!!!
+export_path = "./asset"
+broadcast_strategy = select_broadcast_strategy(BroadcastStrategyType.ASYNCIO_SEQUENTIAL)
+# Read subscriber list from file, but you can also read from database of your choice
+subscriber_list: list[Tuple[int, str]] = []
+with open("./asset/subscriber.txt", "r") as file:
+    header = file.readline()
+    while True:
+        line = file.readline()
+        if not line:
+            break
+        telegram_id, username = line.strip().split(",")
+        subscriber_list.append((int(telegram_id), username))
+
+s, f = broadcast_wrapper(
+    bot_token, broadcast_method, broadcast_strategy,
+    subscriber_list,
+    file_id
+)
+for S in s:
+    print(f"Success: {s}")
+
+for F in f:
+    print(f"Failed: {f}")
+
+if len(f) > 0:
+    write_sent_result(f"{export_path}/result_{file_path}.txt", f, file_path)
+
+```
+
+## Tests
+TODO
+
+## Source Code
+- https://github.com/JonahTzuChi/python-telegram-broadcast
```

### Comparing `python_telegram_broadcast-0.9.6/python_telegram_broadcast.egg-info/SOURCES.txt` & `python_telegram_broadcast-0.9.7/python_telegram_broadcast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.6/setup.py` & `python_telegram_broadcast-0.9.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 DESCRIPTION = 'Package that wraps the python-telegram-bot library to make broadcasting easier.'
 
 # python3 setup.py sdist bdist_wheel
 # twine upload --skip-existing dist/*
 
-VERSION = '0.9.6'
+VERSION = '0.9.7'
 
 setup(
     name='python_telegram_broadcast',
     version=VERSION,
     packages=find_packages(),
     description=DESCRIPTION,
     long_description=open('README.md').read(),
```

