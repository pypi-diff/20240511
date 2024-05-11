# Comparing `tmp/py2hackCraft2-1.0.8.tar.gz` & `tmp/py2hackCraft2-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py2hackCraft2-1.0.8.tar", last modified: Sat Feb 24 06:22:03 2024, max compression
+gzip compressed data, was "py2hackCraft2-1.0.9.tar", last modified: Sat Mar 30 11:56:13 2024, max compression
```

## Comparing `py2hackCraft2-1.0.8.tar` & `py2hackCraft2-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 masafumi   (501) staff       (20)        0 2024-02-24 06:22:03.848507 py2hackCraft2-1.0.8/
--rw-r--r--   0 masafumi   (501) staff       (20)      299 2024-02-24 06:22:03.848348 py2hackCraft2-1.0.8/PKG-INFO
--rw-r--r--   0 masafumi   (501) staff       (20)      267 2024-01-08 08:37:13.000000 py2hackCraft2-1.0.8/README.md
-drwxr-xr-x   0 masafumi   (501) staff       (20)        0 2024-02-24 06:22:03.847181 py2hackCraft2-1.0.8/py2hackCraft/
--rw-r--r--   0 masafumi   (501) staff       (20)        0 2024-01-07 05:03:54.000000 py2hackCraft2-1.0.8/py2hackCraft/__init__.py
--rw-r--r--   0 masafumi   (501) staff       (20)    72170 2024-01-15 08:48:58.000000 py2hackCraft2-1.0.8/py2hackCraft/material.py
--rw-r--r--   0 masafumi   (501) staff       (20)    28607 2024-02-24 06:17:24.000000 py2hackCraft2-1.0.8/py2hackCraft/modules.py
-drwxr-xr-x   0 masafumi   (501) staff       (20)        0 2024-02-24 06:22:03.848122 py2hackCraft2-1.0.8/py2hackCraft2.egg-info/
--rw-r--r--   0 masafumi   (501) staff       (20)      299 2024-02-24 06:22:03.000000 py2hackCraft2-1.0.8/py2hackCraft2.egg-info/PKG-INFO
--rw-r--r--   0 masafumi   (501) staff       (20)      276 2024-02-24 06:22:03.000000 py2hackCraft2-1.0.8/py2hackCraft2.egg-info/SOURCES.txt
--rw-r--r--   0 masafumi   (501) staff       (20)        1 2024-02-24 06:22:03.000000 py2hackCraft2-1.0.8/py2hackCraft2.egg-info/dependency_links.txt
--rw-r--r--   0 masafumi   (501) staff       (20)       17 2024-02-24 06:22:03.000000 py2hackCraft2-1.0.8/py2hackCraft2.egg-info/requires.txt
--rw-r--r--   0 masafumi   (501) staff       (20)       13 2024-02-24 06:22:03.000000 py2hackCraft2-1.0.8/py2hackCraft2.egg-info/top_level.txt
--rw-r--r--   0 masafumi   (501) staff       (20)       38 2024-02-24 06:22:03.848552 py2hackCraft2-1.0.8/setup.cfg
--rw-r--r--   0 masafumi   (501) staff       (20)      676 2024-02-24 06:21:52.000000 py2hackCraft2-1.0.8/setup.py
+drwxr-xr-x   0 masafumi   (501) staff       (20)        0 2024-03-30 11:56:13.368152 py2hackCraft2-1.0.9/
+-rw-r--r--   0 masafumi   (501) staff       (20)      299 2024-03-30 11:56:13.368019 py2hackCraft2-1.0.9/PKG-INFO
+-rw-r--r--   0 masafumi   (501) staff       (20)      267 2024-01-08 08:37:13.000000 py2hackCraft2-1.0.9/README.md
+drwxr-xr-x   0 masafumi   (501) staff       (20)        0 2024-03-30 11:56:13.367016 py2hackCraft2-1.0.9/py2hackCraft/
+-rw-r--r--   0 masafumi   (501) staff       (20)        0 2024-01-07 05:03:54.000000 py2hackCraft2-1.0.9/py2hackCraft/__init__.py
+-rw-r--r--   0 masafumi   (501) staff       (20)    72170 2024-01-15 08:48:58.000000 py2hackCraft2-1.0.9/py2hackCraft/material.py
+-rw-r--r--   0 masafumi   (501) staff       (20)    30410 2024-03-30 11:29:46.000000 py2hackCraft2-1.0.9/py2hackCraft/modules.py
+drwxr-xr-x   0 masafumi   (501) staff       (20)        0 2024-03-30 11:56:13.367854 py2hackCraft2-1.0.9/py2hackCraft2.egg-info/
+-rw-r--r--   0 masafumi   (501) staff       (20)      299 2024-03-30 11:56:13.000000 py2hackCraft2-1.0.9/py2hackCraft2.egg-info/PKG-INFO
+-rw-r--r--   0 masafumi   (501) staff       (20)      276 2024-03-30 11:56:13.000000 py2hackCraft2-1.0.9/py2hackCraft2.egg-info/SOURCES.txt
+-rw-r--r--   0 masafumi   (501) staff       (20)        1 2024-03-30 11:56:13.000000 py2hackCraft2-1.0.9/py2hackCraft2.egg-info/dependency_links.txt
+-rw-r--r--   0 masafumi   (501) staff       (20)       17 2024-03-30 11:56:13.000000 py2hackCraft2-1.0.9/py2hackCraft2.egg-info/requires.txt
+-rw-r--r--   0 masafumi   (501) staff       (20)       13 2024-03-30 11:56:13.000000 py2hackCraft2-1.0.9/py2hackCraft2.egg-info/top_level.txt
+-rw-r--r--   0 masafumi   (501) staff       (20)       38 2024-03-30 11:56:13.368191 py2hackCraft2-1.0.9/setup.cfg
+-rw-r--r--   0 masafumi   (501) staff       (20)      676 2024-03-06 13:23:59.000000 py2hackCraft2-1.0.9/setup.py
```

### Comparing `py2hackCraft2-1.0.8/py2hackCraft/material.py` & `py2hackCraft2-1.0.9/py2hackCraft/material.py`

 * *Files identical despite different names*

### Comparing `py2hackCraft2-1.0.8/py2hackCraft/modules.py` & `py2hackCraft2-1.0.9/py2hackCraft/modules.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,15 @@
         while not self.connected:
             time.sleep(0.1)  # Wait for connection to be established
 
     def send(self, message):
         logging.debug("send sending'%s'" % message)
         self.wait_for_connection()
         with self.lock:
+            self.result = None
             self.response_event.clear()  # イベントをクリアして新しいレスポンスの準備をする
             self.ws.send(message)
             self.response_event.wait()  # サーバーからのレスポンスを待つ
         return self.result  # 最後に受信したメッセージを返す
 
     def close(self):
         self.ws.close()
@@ -142,14 +143,27 @@
 class Location:
     x: int
     y: int
     z: int
     world: str = "world"
 
 @dataclass
+class InteractEvent:
+    action: str
+    type: str
+    name: str
+    block: str = None
+    data: int = 0
+    uuid: str = None
+    world: str = "world"
+    x: int = 0 
+    y: int = 0 
+    z: int = 0
+
+@dataclass
 class EventMessage:
     """
     イベントメッセージを表すデータクラス。
 
     Attributes:
         sender (str): 送信者の名前。
         uuid (str): 送信者の一意の識別子（UUID）。
@@ -200,30 +214,33 @@
         isLiquid (bool): 液体ブロックかどうか。
         isAir (bool): 空気ブロックかどうか。
         isBurnable (bool): 燃えるブロックかどうか。
         isFuel (bool): 燃料ブロックかどうか。
         isOccluding (bool): 透過しないブロックかどうか。
         isSolid (bool): 壁のあるブロックかどうか。
         isPassable (bool): 通過可能なブロックかどうか。
+        world (str): ブロックが存在するワールドの名前（デフォルトは"world"）。
         x (int): ブロックのX座標。
         y (int): ブロックのY座標。
         z (int): ブロックのZ座標。
     """
     name: str
+    type: str = "block"
     data: int = 0
     isLiquid: bool = False
     isAir: bool = False
     isBurnable: bool = False
     isFuel: bool = False
     isOccluding: bool = False
     isSolid: bool = False
     isPassable: bool = False
     x: int = 0
     y: int = 0
     z: int = 0
+    world: str = "world"
 
 @dataclass
 class ItemStack:
     slot: int = 0
     name: str = "air"
     amount: int = 0
 
@@ -245,14 +262,26 @@
         self.uuid = self.client.result['playerUUID']
         self.world = self.client.result['world']
         return self
 
     def logout(self):
         self.client.disconnect()    
 
+    def setOnBlockBreak(self, callbackFunc: Callable[['Block'], Any]):
+        """
+        プレイヤーがブロックをこわした時に呼び出されるコールバック関数を設定する。
+        """
+        def callbackWrapper(data):
+            logging.debug("onPlayerBlockBreak callbackWrapper '%s'" % data)
+            if(data['playerUuid'] == self.uuid):
+                logging.debug("callbackWrapper '%s'" % data)
+                block = Block(**data['block'])
+                callbackFunc(self, block)
+        self.client.setCallback('onPlayerBlockBreak', callbackWrapper)
+
     def getEntity(self, name: str) -> 'Entity': 
         """
         指定された名前のエンティティを取得する。
 
         Args:
             name (str): エンティティの名前。
 
@@ -266,40 +295,40 @@
             raise UninitializedClientError("Client is not initialized")
 
         message = {
             "type": "attach",
             "data": {"entity": name}
         }
         self.client.send(json.dumps(message))
-        uuid = self.client.result
-        if(uuid is None):
+        result = self.client.result
+        if(result is None):
             raise ValueError("Entity '%s' not found" % name)
 
-        return Entity(self.client, self.world, uuid)
+        return Entity(self.client, self.world, result)
 
 class World:
     """
     ワールドを表すクラス。
     """
     def __init__(self, client: _WebSocketClient, world: str, entityUUID: str):
         self.client = client
         self.name = world
         self.entityUUID = entityUUID
 
-    def setBlock(self, x: int, y: int, z: int, block: str):
+    def setBlock(self, x: int, y: int, z: int, block: str, data: int = 0):
         """
         指定された座標にブロックを設置する。
 
         Args:
             x (int): 絶対的なX座標。
             y (int): 絶対的なY座標。
             z (int): 絶対的なZ座標。
             block (str): 設置するブロックの種類。
         """
-        self.client.sendCall(self.entityUUID, "setBlock", [x, y, z, block])
+        self.client.sendCall(self.entityUUID, "setBlock", [x, y, z, block, data])
 
     def getBlock(self, x: int, y: int, z: int) -> Block :
         """
         指定された座標のブロックを取得する。
 
         Args:
             x (int): 絶対的なX座標。
@@ -412,14 +441,26 @@
             logging.debug("setOnRedstoneChange callbackWrapper '%s'" % data)
             if(data['entityUuid'] == self.uuid):
                 logging.debug("callbackWrapper '%s'" % data)
                 power = RedstonePower(**data)
                 callbackFunc(self, power)
         self.client.setCallback('onEntityRedstone', callbackWrapper)
 
+    def setOnInteractEvent(self, callbackFunc: Callable[['Entity', 'InteractEvent'], Any]):
+        """
+        レッドストーンを受信したときに呼び出されるコールバック関数を設定する。
+        """
+        def callbackWrapper(data):
+            logging.debug("onInteractEvent callbackWrapper '%s'" % data)
+            if(data['entityUuid'] == self.uuid):
+                logging.debug("callbackWrapper '%s'" % data)
+                event = InteractEvent(**data["event"])
+                callbackFunc(self, event)
+        self.client.setCallback('onInteractEvent', callbackWrapper)    
+
     def setOnMessage(self, callbackFunc: Callable[['Entity', str], Any]):
         """
         メッセージを受信したときに呼び出されるコールバック関数を設定する。
         """
         def callbackWrapper(data):
             logging.debug("setOnMessage callbackWrapper '%s'" % data)
             if(data['entityUuid'] == self.uuid):
@@ -434,14 +475,23 @@
 
         Args:
             target (str): 送信先のEntityの名前。
             message (str): 送信するメッセージの内容。
         """
         self.client.sendCall(self.uuid, "sendEvent", [target, message])
 
+    def executeCommand(self, command: str):
+        """
+        コマンドを実行する。
+
+        Args:
+            command (str): 実行するコマンドの内容。
+        """
+        self.client.sendCall(self.uuid, "executeCommand", [command])
+
     def getWorld(self) -> 'World': 
         """
         指定された名前のワールドを取得する。
 
         Args:
             name (str): ワールドの名前。
 
@@ -537,28 +587,22 @@
     def makeSound(self) -> bool :
         """
         自分を鳴かせる。
         """
         self.client.sendCall(self.uuid, "sound")
         return str_to_bool(self.client.result)
 
-    def walk(self) -> bool :
-        """
-        歩く。
-
+    def move(self, speed: float) -> bool :
         """
-        self.client.sendCall(self.uuid, "move", [0.5])
-        return str_to_bool(self.client.result)
-
-    def sprint(self) -> bool :
-        """
-        走る。
+        前方へ移動する。
 
+        Args:
+            speed (float): 移動速度。
         """
-        self.client.sendCall(self.uuid, "move", [1.0])
+        self.client.sendCall(self.uuid, "move", [speed])
         return str_to_bool(self.client.result)
 
     def turn(self, degrees: int):
         """
         自分を回転させる。
 
         Args:
```

### Comparing `py2hackCraft2-1.0.8/setup.py` & `py2hackCraft2-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="py2hackCraft2",
-    version="1.0.8",
+    version="1.0.9",
     packages=find_packages(),
     install_requires=[
         "websocket-client"  # websocketライブラリの追加
         # 他にも依存する外部ライブラリがあれば、同様にリストに追加
     ],
     # その他のメタデータ
     author="Masafumi Terazono",
```

