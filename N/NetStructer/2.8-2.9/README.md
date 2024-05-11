# Comparing `tmp/NetStructer-2.8.tar.gz` & `tmp/netstructer-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NetStructer-2.8.tar", last modified: Sun Mar 24 14:54:57 2024, max compression
+gzip compressed data, was "netstructer-2.9.tar", last modified: Sat May 11 20:40:32 2024, max compression
```

## Comparing `NetStructer-2.8.tar` & `netstructer-2.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-03-24 14:54:56.000000 NetStructer-2.8/
-drwxrwxrwx   0        0        0        0 2024-03-24 14:54:56.000000 NetStructer-2.8/NetStructer/
--rw-rw-rw-   0        0        0    10974 2024-03-22 21:32:42.000000 NetStructer-2.8/NetStructer/__init__.py
--rw-rw-rw-   0        0        0      983 2024-03-08 21:32:54.000000 NetStructer-2.8/NetStructer/const.py
--rw-rw-rw-   0        0        0       61 2024-03-24 14:48:30.000000 NetStructer-2.8/NetStructer/utlist.py
-drwxrwxrwx   0        0        0        0 2024-03-24 14:54:56.000000 NetStructer-2.8/NetStructer.egg-info/
--rw-rw-rw-   0        0        0     4246 2024-03-24 14:54:56.000000 NetStructer-2.8/NetStructer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2024-03-24 14:54:56.000000 NetStructer-2.8/NetStructer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-24 14:54:56.000000 NetStructer-2.8/NetStructer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-03-24 14:54:56.000000 NetStructer-2.8/NetStructer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-24 14:54:56.000000 NetStructer-2.8/NetStructer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4246 2024-03-24 14:54:56.000000 NetStructer-2.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-03-24 14:54:58.000000 NetStructer-2.8/setup.cfg
--rw-rw-rw-   0        0        0      792 2024-03-24 14:54:48.000000 NetStructer-2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 20:40:32.000000 netstructer-2.9/
+drwxrwxrwx   0        0        0        0 2024-05-11 20:40:32.000000 netstructer-2.9/NetStructer/
+-rw-rw-rw-   0        0        0    10938 2024-05-11 20:26:34.000000 netstructer-2.9/NetStructer/__init__.py
+-rw-rw-rw-   0        0        0       61 2024-04-06 04:48:10.000000 netstructer-2.9/NetStructer/const.py
+-rw-rw-rw-   0        0        0     1321 2024-05-11 20:26:18.000000 netstructer-2.9/NetStructer/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-11 20:40:34.000000 netstructer-2.9/NetStructer.egg-info/
+-rw-rw-rw-   0        0        0      347 2024-05-11 20:40:32.000000 netstructer-2.9/NetStructer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-05-11 20:40:32.000000 netstructer-2.9/NetStructer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 20:40:32.000000 netstructer-2.9/NetStructer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-05-11 20:40:32.000000 netstructer-2.9/NetStructer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-11 20:40:32.000000 netstructer-2.9/NetStructer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      347 2024-05-11 20:40:34.000000 netstructer-2.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-11 20:40:34.000000 netstructer-2.9/setup.cfg
+-rw-rw-rw-   0        0        0      748 2024-05-11 20:39:00.000000 netstructer-2.9/setup.py
```

### Comparing `NetStructer-2.8/NetStructer/__init__.py` & `netstructer-2.9/NetStructer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,14 @@
-import os , sys
-	
-__file = __file__ if __file__ not in sys.path else ''
-	
-sys.path.append(os.path.dirname(__file))
 import pickle as json
 import socket
 from threading import Thread
 from cryptography.fernet import Fernet
 from time import sleep
-from utlist import *
-from const import *
+from NetStructer.const import *
+from NetStructer.tools import *
 
 __session__ = {}
 
 class _encryption:
 
 	def __init__(self,key=DEFAULT_ENC):
 		self.__Key = Fernet(key)
@@ -28,43 +23,44 @@
 		try:
 			return self.__Key.decrypt(data)
 		except:
 			raise KeyError(f'bad key {self.__code}')
 
 class Bridge:
 
-	def __init__(self,serv,code=DEFAULT_ENC):
+	def __init__(self,serv,enckey=DEFAULT_ENC,timeout=None):
 		assert isTCP(serv),'Bridge accepts only TCP server'
 		self.__server = serv
 		self.__end_of_bytes = b'<end_of_bytes>'
-		self.__enc = _encryption(key=code)
+		self.__enc = _encryption(key=enckey)
 		self.__data = b'' ; self.__error = 0
+		self.TimeOut(timeout)
 		
 	def __Check(data):
 		try:
 			json.dumps(data)
 			return True
 		except:
 			return False
 		
-	def Link(addr):
+	def Link(addr,**keys):
 		"""
 		Description:
 			The Link() method is a class method used to establish a connection to a server. It creates a new instance of the Bridge class representing the client side of the connection.
 		Parameters:
 			addr: A tuple containing the IP address and port number of the server to connect to.
 		Returns:
 			An instance of the Bridge class representing the client side of the connection.
 		Example Usage:
 			server_address = ('127.0.0.1', 8000)
 			client_bridge = Bridge.Link(server_address)
 		"""
 		soc = socket.socket()
 		soc.connect(addr)
-		return Bridge(soc)
+		return Bridge(soc,**keys)
 		
 	def SetEncKey(self,Key):
 		"""
 		Description:
 			The SetEncMode() method allows changing the encryption mode used by the Bridge object. It updates the encryption key used for encrypting and decrypting data transmitted over the socket connection.
 		Parameters:
 			mode: The new encryption mode to be set. This should be a 32-byte URL-safe base64-encoded string, typically generated by the Fernet.generate_key() method.
@@ -83,15 +79,15 @@
 		Returns:
 			length: The length of the original data buffer that was successfully sent.
 		"""
 		try:
 			if Bridge.__Check(buffer):
 				Buffer = self.__enc.encrypt(json.dumps(buffer))
 				self.__server.send(Buffer+self.__end_of_bytes)
-				return len(buffer)
+				return len(str(buffer))
 			else:
 				raise ValueError(f"can't not encode {buffer}")
 		except TypeError:
 			raise ValueError(f"can't not encode {buffer}")
 		except ConnectionAbortedError as er:
 			raise er
 		except ConnectionResetError:
```

