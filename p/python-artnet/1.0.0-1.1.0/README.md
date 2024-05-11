# Comparing `tmp/python_artnet-1.0.0.tar.gz` & `tmp/python_artnet-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_artnet-1.0.0.tar", last modified: Sun Dec 17 12:15:21 2023, max compression
+gzip compressed data, was "python_artnet-1.1.0.tar", last modified: Sat May 11 18:25:47 2024, max compression
```

## Comparing `python_artnet-1.0.0.tar` & `python_artnet-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 12:15:21.266680 python_artnet-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 12:15:21.262680 python_artnet-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 12:15:21.266680 python_artnet-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2023-12-17 12:15:08.000000 python_artnet-1.0.0/.github/workflows/publishToPypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2023-12-17 12:15:08.000000 python_artnet-1.0.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 12:15:21.266680 python_artnet-1.0.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2023-12-17 12:15:08.000000 python_artnet-1.0.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-12-17 12:15:08.000000 python_artnet-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5157 2023-12-17 12:15:21.266680 python_artnet-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2023-12-17 12:15:08.000000 python_artnet-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2023-12-17 12:15:08.000000 python_artnet-1.0.0/exampleReceiver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2023-12-17 12:15:08.000000 python_artnet-1.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 12:15:21.266680 python_artnet-1.0.0/python_artnet/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-12-17 12:15:08.000000 python_artnet-1.0.0/python_artnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12176 2023-12-17 12:15:08.000000 python_artnet-1.0.0/python_artnet/python_artnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 12:15:21.266680 python_artnet-1.0.0/python_artnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5157 2023-12-17 12:15:21.000000 python_artnet-1.0.0/python_artnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      334 2023-12-17 12:15:21.000000 python_artnet-1.0.0/python_artnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-17 12:15:21.000000 python_artnet-1.0.0/python_artnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-12-17 12:15:21.000000 python_artnet-1.0.0/python_artnet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-17 12:15:21.266680 python_artnet-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-17 12:15:08.000000 python_artnet-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:25:47.385928 python_artnet-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-11 18:25:43.000000 python_artnet-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6276 2024-05-11 18:25:47.385928 python_artnet-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-05-11 18:25:43.000000 python_artnet-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-11 18:25:43.000000 python_artnet-1.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:25:47.385928 python_artnet-1.1.0/python_artnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-11 18:25:43.000000 python_artnet-1.1.0/python_artnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12563 2024-05-11 18:25:43.000000 python_artnet-1.1.0/python_artnet/python_artnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:25:47.385928 python_artnet-1.1.0/python_artnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6276 2024-05-11 18:25:47.000000 python_artnet-1.1.0/python_artnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-11 18:25:47.000000 python_artnet-1.1.0/python_artnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 18:25:47.000000 python_artnet-1.1.0/python_artnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-11 18:25:47.000000 python_artnet-1.1.0/python_artnet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 18:25:47.385928 python_artnet-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-11 18:25:43.000000 python_artnet-1.1.0/setup.py
```

### Comparing `python_artnet-1.0.0/LICENSE` & `python_artnet-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_artnet-1.0.0/PKG-INFO` & `python_artnet-1.1.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_artnet
-Version: 1.0.0
+Version: 1.1.0
 Summary: Easy-to-use and simple python receiver for Art-Net (that also implements device polling).
 Author: sciencegey
 Maintainer: sciencegey
 License: MIT License
         
         Copyright (c) 2023 Sam Knowles
         
@@ -47,57 +47,81 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python_artnet
 Easy-to-use and simple python receiver for Art-Net (that also implements device polling).
 
 ## Installaton
-All you need to do is clone the repository and start using it!
+All you need to do is clone the repository
 ``` bash
 $ git clone https://github.com/sciencegey/python_artnet.git
 $ cd python_artnet
-$ python3 exampleReceiver.py
+$ python3 samples/exampleReceiver.py
+```
+***OR***
+
+Install using PIP
+``` bash
+$ pip install python_artnet
 ```
 
 ## Usage
 All you need to do to start receiving data is import the module, start the listener, then check for received data whenever you want!
 ```python
 import python_artnet as Artnet
 
 # By default it will listen on 0.0.0.0 (all interfaces)
 artNet = Artnet.Artnet()
 
-# Fetch the latest packet we received.
-artNetPacket = artNet.readPacket()
+# Fetch the latest packet we received from universe 0.
+artNetPacket = artNet.readBuffer()[0]
 # And extract the DMX data from that packet.
 dmxPacket = artNetPacket.data
 # You'll also want to check that there *is* data in the packet;
 # if there isn't then it returns None
 # See the example for more information
 
 # Close the listener nicely :)
 artNet.close()
 ```
 
-There are also plenty of arguments you can pass when you start the listner:
+There are also plenty of arguments you can pass when you start the listener:
 
 - **BINDIP** - Which IP address you want to *listen* on (usually a broadcast address). This is the only one you really ever need to change. *(Defaults to "" AKA 0.0.0.0 AKA all interfaces)*
 - **PORT** - Which UDP port you want to listen on. Shouldn't need to ever 
 change this. *(Defaults to 6454)*
 
 <details>
 <summary>The following are used for purely management purposes:</summary>
 
 - **SYSIP** - What the IP address of your system is. Purely cosmetic and only used to identify the system to ArtNet controllers. *(Defaults to "10.10.10.1")*
 - **MAC** - What the MAC address of your system is. Same as above. *(Defaults to ["AA","BB","CC","DD","EE","FF"])*
 - **SWVER** - What version of Art-Net we're using. In this case, V1.4 *(Defaults to "14")*
-- **SHORTNAME** and **LONGAME** - Used to see what devices are what on a controller. *(Shortname is truncated to 17 bytes long, longname is truncated to 63)*
+- **SHORTNAME** and **LONGNAME** - Used to see what devices are what on a controller. *(Shortname is truncated to 17 bytes long, longname is truncated to 63)*
 - **OEMCODE** - What the Art-Net OEM code your device has. Only needs to be set if you have one. *(In hex)*
 - **ESTACODE** - What the ESTA Manafacturer Code your device has. Only needs to be set if you have one. *(In hex)*
 - **PORTTYPE** - Used to tell the controller what type of physical ports your device has. *(Defaults to [0x80,0x00,0x00,0x00])* *See the Art-Net documentation for more information*
 - **REFRESH** - What the refresh rate (in Hz) of your device. *(Defaults to 44 (the max for DMX))*
 - **DEBUG** - Used to turn on debug output. *(Defaults to False)*
 </details>
 
-Further information on how it all works can be found in the [Art-Net documentation](https://www.artisticlicence.com/WebSiteMaster/User%20Guides/art-net.pdf).
+### The artnet packet consists of the following:
+- **ver** - Which version of Art-Net the packet is using. *Latest is V1.4 (14)*
+- **sequence** - Sequence number, used to check if the packets have arrived in the correct order *(counts up to 255)*
+- **physical** - The physical DMX512 port this data came from
+- **universe** - Which universe this packet is meant for
+- **data** - The data in the packet
+- **length** - How much DMX data we have *(full packet is 18+length)*
+
+
+### The following functions are available to use:
+- **readPacket** - Returns the last Art-Net packet that we received. *(Returns ArtnetPacket)*
+- **readBuffer** - Returns the last Art-Net packet that we received for each universe. *(Returns an array of ArtnetPacket, one per universe)*
+- **close** - Make sure to run this at the end of your program. Tells the socket to stop running and joins the thread back. *(Returns None)*
+- **version** - Returns the library version. *(Returns String)*
+
+
+Further information on how it all works can be found in the [Art-Net documentation](https://www.artisticlicence.com/WebSiteMaster/User%20Guides/art-net.pdf).\
+*Art-Net™ Designed by and Copyright Artistic Licence Engineering Ltd*
+
 ## License
 This project is licensed under an MIT License (see the [LICENSE](LICENSE) file).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `python_artnet-1.0.0/README.md` & `python_artnet-1.1.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,78 @@
 # python_artnet
 Easy-to-use and simple python receiver for Art-Net (that also implements device polling).
 
 ## Installaton
-All you need to do is clone the repository and start using it!
+All you need to do is clone the repository
 ``` bash
 $ git clone https://github.com/sciencegey/python_artnet.git
 $ cd python_artnet
-$ python3 exampleReceiver.py
+$ python3 samples/exampleReceiver.py
+```
+***OR***
+
+Install using PIP
+``` bash
+$ pip install python_artnet
 ```
 
 ## Usage
 All you need to do to start receiving data is import the module, start the listener, then check for received data whenever you want!
 ```python
 import python_artnet as Artnet
 
 # By default it will listen on 0.0.0.0 (all interfaces)
 artNet = Artnet.Artnet()
 
-# Fetch the latest packet we received.
-artNetPacket = artNet.readPacket()
+# Fetch the latest packet we received from universe 0.
+artNetPacket = artNet.readBuffer()[0]
 # And extract the DMX data from that packet.
 dmxPacket = artNetPacket.data
 # You'll also want to check that there *is* data in the packet;
 # if there isn't then it returns None
 # See the example for more information
 
 # Close the listener nicely :)
 artNet.close()
 ```
 
-There are also plenty of arguments you can pass when you start the listner:
+There are also plenty of arguments you can pass when you start the listener:
 
 - **BINDIP** - Which IP address you want to *listen* on (usually a broadcast address). This is the only one you really ever need to change. *(Defaults to "" AKA 0.0.0.0 AKA all interfaces)*
 - **PORT** - Which UDP port you want to listen on. Shouldn't need to ever 
 change this. *(Defaults to 6454)*
 
 <details>
 <summary>The following are used for purely management purposes:</summary>
 
 - **SYSIP** - What the IP address of your system is. Purely cosmetic and only used to identify the system to ArtNet controllers. *(Defaults to "10.10.10.1")*
 - **MAC** - What the MAC address of your system is. Same as above. *(Defaults to ["AA","BB","CC","DD","EE","FF"])*
 - **SWVER** - What version of Art-Net we're using. In this case, V1.4 *(Defaults to "14")*
-- **SHORTNAME** and **LONGAME** - Used to see what devices are what on a controller. *(Shortname is truncated to 17 bytes long, longname is truncated to 63)*
+- **SHORTNAME** and **LONGNAME** - Used to see what devices are what on a controller. *(Shortname is truncated to 17 bytes long, longname is truncated to 63)*
 - **OEMCODE** - What the Art-Net OEM code your device has. Only needs to be set if you have one. *(In hex)*
 - **ESTACODE** - What the ESTA Manafacturer Code your device has. Only needs to be set if you have one. *(In hex)*
 - **PORTTYPE** - Used to tell the controller what type of physical ports your device has. *(Defaults to [0x80,0x00,0x00,0x00])* *See the Art-Net documentation for more information*
 - **REFRESH** - What the refresh rate (in Hz) of your device. *(Defaults to 44 (the max for DMX))*
 - **DEBUG** - Used to turn on debug output. *(Defaults to False)*
 </details>
 
-Further information on how it all works can be found in the [Art-Net documentation](https://www.artisticlicence.com/WebSiteMaster/User%20Guides/art-net.pdf).
+### The artnet packet consists of the following:
+- **ver** - Which version of Art-Net the packet is using. *Latest is V1.4 (14)*
+- **sequence** - Sequence number, used to check if the packets have arrived in the correct order *(counts up to 255)*
+- **physical** - The physical DMX512 port this data came from
+- **universe** - Which universe this packet is meant for
+- **data** - The data in the packet
+- **length** - How much DMX data we have *(full packet is 18+length)*
+
+
+### The following functions are available to use:
+- **readPacket** - Returns the last Art-Net packet that we received. *(Returns ArtnetPacket)*
+- **readBuffer** - Returns the last Art-Net packet that we received for each universe. *(Returns an array of ArtnetPacket, one per universe)*
+- **close** - Make sure to run this at the end of your program. Tells the socket to stop running and joins the thread back. *(Returns None)*
+- **version** - Returns the library version. *(Returns String)*
+
+
+Further information on how it all works can be found in the [Art-Net documentation](https://www.artisticlicence.com/WebSiteMaster/User%20Guides/art-net.pdf).\
+*Art-Net™ Designed by and Copyright Artistic Licence Engineering Ltd*
+
 ## License
-This project is licensed under an MIT License (see the [LICENSE](LICENSE) file).
+This project is licensed under an MIT License (see the [LICENSE](LICENSE) file).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `python_artnet-1.0.0/pyproject.toml` & `python_artnet-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
-requires = ["setuptools","setuptools_scm"]
+requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python_artnet"
 authors = [
     {name = "sciencegey"}
 ]
 maintainers = [
     {name = "sciencegey"}
 ]
 description = "Easy-to-use and simple python receiver for Art-Net (that also implements device polling)."
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.8"
-version = "1.0.0"
+version = "1.1.0"
 keywords = ["Art-Net", "ArtNet", "DMX", "Lighting", "Lighting Control"]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 4 - Beta",
 
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Artistic Software",
@@ -36,8 +36,10 @@
 ]
 
 [project.urls]
 Homepage = "https://github.com/sciencegey/python_artnet"
 Repository = "https://github.com/sciencegey/python_artnet.git"
 Issues = "https://github.com/sciencegey/python_artnet/issues"
 
-[tool.setuptools_scm]
+[tool.setuptools]
+packages = ["python_artnet"]
+include-package-data = false
```

### Comparing `python_artnet-1.0.0/python_artnet/python_artnet.py` & `python_artnet-1.1.0/python_artnet/python_artnet.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-'''Simple library that takes Artnet (DMX) packets and converts them to data that Python can use.
+'''Simple library that takes Art-Net (DMX) packets and converts them to data that Python can use.
 
 Made in Python 3.8
 Artnet spec: https://www.artisticlicence.com/WebSiteMaster/User%20Guides/art-net.pdf
 '''
 import threading
 
 from time import sleep
@@ -76,32 +76,33 @@
             if isinstance(each,list):
                for j in each:
                    yield j
             else:
                 yield each
 
 class Artnet:
-    ARTNET_HEADER = b'Art-Net\x00' # the header for artnet packets
+    ARTNET_HEADER = b'Art-Net\x00' # the header for Art-Net packets
 
     def __init__(self, BINDIP = "", PORT = 6454, SYSIP = "10.10.10.1", MAC = ["AA","BB","CC","DD","EE","FF"], SWVER = "14", SHORTNAME = "python_artnet", LONGNAME = "python_artnet", OEMCODE = 0xabcd, ESTACODE = 0x7FF0, PORTTYPE = [0x80,0x00,0x00,0x00], REFRESH = 44, DEBUG = False):
-        self.BINDIP = BINDIP        # IP to listen on (either 0.0.0.0 (all interfaces) or a broadcast address)
-        self.SYSIP = SYSIP          # IP of the system itself
-        self.PORT = PORT            # Port to listen on (default is 6454)
-        self.MAC = MAC              # MAC address of the ArtNet port
-        self.SWVER = SWVER          # Software version
+        self.BINDIP = BINDIP            # IP to listen on (either 0.0.0.0 (all interfaces) or a broadcast address)
+        self.SYSIP = SYSIP              # IP of the system itself
+        self.PORT = PORT                # Port to listen on (default is 6454)
+        self.MAC = MAC                  # MAC address of the ArtNet port
+        self.SWVER = SWVER              # Software version
         self.SHORTNAME = SHORTNAME[:17] # Short name
         self.LONGNAME = LONGNAME[:63]   # Long name
-        self.OEMCODE = OEMCODE      # ArtNet OEM code
-        self.ESTACODE = ESTACODE    # ESTA Manufacturer code
-        self.PORTTYPE = PORTTYPE    # 
-        self.REFRESH = REFRESH      # Refresh rate of the node
+        self.OEMCODE = OEMCODE          # Art-Net OEM code
+        self.ESTACODE = ESTACODE        # ESTA Manufacturer code
+        self.PORTTYPE = PORTTYPE        # 
+        self.REFRESH = REFRESH          # Refresh rate of the node
 
         self.debug = DEBUG
 
         self.packet = None
+        self.packetBuffer = [ArtnetPacket()]*16
 
         # Starts the listner in it's own thread
         self.listen = True
         self.t = threading.Thread(target=self.__init_socket, daemon=True)
         self.t.start()
 
     def __init_socket(self):
@@ -124,14 +125,15 @@
                 # print("Recieved from:" + str(addr))
                 self.packet = Artnet.artnet_packet_to_array(self, data, addr)
 
     def close(self):
         '''Tells the socket to stop running and joins the thread back'''
         self.listen = False
         self.t.join()
+        return None
 
     def art_pol_reply(self, senderAddr):
         '''Sends a reply to an ArtPoll packet; this allows other devices on the network to know who we are.'''
         reply = ArtPollReplyPacket()
         
         reply.ipAddress = [int(i) for i in self.SYSIP.split(".")]
         reply.port = pack('<H', self.PORT)
@@ -152,23 +154,23 @@
         sleep(random.random())
         self.sock.sendto(packedReply, senderAddr)
         if self.debug: print("sent!")
         
         return None
         
     def artnet_packet_to_array(self, raw_data, senderAddr):
-        '''Extracts DMX data from the Artnet packet and returns it as a nice array.'''
+        '''Extracts DMX data from the Art-Net packet and returns it as a nice array.'''
         if unpack('!8s', raw_data[:8])[0] != Artnet.ARTNET_HEADER:
-            # The packet doesn't have a valid header, so it's probably not an Artnet packet (or it's broken... :V)
+            # The packet doesn't have a valid header, so it's probably not an Art-Net packet (or it's broken... :V)
             if self.debug: print("Received a non Art-Net packet")
             return None
 
         # Extracts the opcode from the packed (little endian int16)
         opCode = unpack('<H', raw_data[8:10])
-        # and checks to see if the packet is an DMX Artnet packet (0x5000)
+        # and checks to see if the packet is an DMX Art-Net packet (0x5000)
         if opCode[0] == 0x5000:
             length = unpack('!H', raw_data[16:18])
             # makes sure the packet is the correct length (if it fetches them too quickly it comes through all malformed)
             if len(raw_data) == 18+length[0]:
                 # stores the packet...
                 packet = ArtnetPacket()
                 # ...then unpacks it into it's constituent parts
@@ -181,14 +183,15 @@
                 # this takes the DMX data and converts it to an array
                 rawData = unpack(
                     '{0}s'.format(int(packet.length)),
                     raw_data[18:18+int(packet.length)])[0]
                 
                 packet.data = list(rawData)
                 # then returns it
+                self.packetBuffer[packet.universe] = packet
                 return packet
             else:
                 return None
 
         # or checks to see if the packet is an ArtPoll packet (0x2000)
         elif opCode[0] == 0x2000:
             if self.debug: print("poll!")
@@ -212,30 +215,39 @@
                 return None
             
         else:
             # otherwise, nothing happened so return it
             return None
 
     def readPacket(self):
-        '''Returns the last ArtNet packet that we received.'''
+        '''Returns the last Art-Net packet that we received.'''
         return(self.packet)
     
+    def readBuffer(self):
+        '''Returns the Art-Net packet buffer'''
+        return(self.packetBuffer)
+    
+def version():
+    '''Returns the library version'''
+    return "1.1.0"
+    
 if __name__ == "__main__":
-    ### ArtNet Config ###
+    ### Art-Net Config ###
     artnetBindIp = ""
     systemIp = "192.168.1.165"
     artnetPort = 6454
     artnetUniverse = 0
     
     artNet = Artnet(artnetBindIp,artnetPort,systemIp,DEBUG=True)
     while True:
         try:
-            artNetPacket = artNet.readPacket()
+            artNetPacket = artNet.readBuffer()
+            # Makes sure the packet is valid and that there's some data available
             if artNetPacket is not None:
-                # Checks to see if the current packet is for the specified DMX Universe
-                if artNetPacket.universe == artnetUniverse:
+                if artNetPacket[artnetUniverse].data is not None:
                     # Stores the packet data array
-                    dmx = artNetPacket.data
+                    dmx = artNetPacket[artnetUniverse].data
                     print(*dmx[:12])
                     sleep(1)
+        
         except KeyboardInterrupt:
             break
```

### Comparing `python_artnet-1.0.0/python_artnet.egg-info/PKG-INFO` & `python_artnet-1.1.0/python_artnet.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: python-artnet
-Version: 1.0.0
+Name: python_artnet
+Version: 1.1.0
 Summary: Easy-to-use and simple python receiver for Art-Net (that also implements device polling).
 Author: sciencegey
 Maintainer: sciencegey
 License: MIT License
         
         Copyright (c) 2023 Sam Knowles
         
@@ -47,57 +47,81 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python_artnet
 Easy-to-use and simple python receiver for Art-Net (that also implements device polling).
 
 ## Installaton
-All you need to do is clone the repository and start using it!
+All you need to do is clone the repository
 ``` bash
 $ git clone https://github.com/sciencegey/python_artnet.git
 $ cd python_artnet
-$ python3 exampleReceiver.py
+$ python3 samples/exampleReceiver.py
+```
+***OR***
+
+Install using PIP
+``` bash
+$ pip install python_artnet
 ```
 
 ## Usage
 All you need to do to start receiving data is import the module, start the listener, then check for received data whenever you want!
 ```python
 import python_artnet as Artnet
 
 # By default it will listen on 0.0.0.0 (all interfaces)
 artNet = Artnet.Artnet()
 
-# Fetch the latest packet we received.
-artNetPacket = artNet.readPacket()
+# Fetch the latest packet we received from universe 0.
+artNetPacket = artNet.readBuffer()[0]
 # And extract the DMX data from that packet.
 dmxPacket = artNetPacket.data
 # You'll also want to check that there *is* data in the packet;
 # if there isn't then it returns None
 # See the example for more information
 
 # Close the listener nicely :)
 artNet.close()
 ```
 
-There are also plenty of arguments you can pass when you start the listner:
+There are also plenty of arguments you can pass when you start the listener:
 
 - **BINDIP** - Which IP address you want to *listen* on (usually a broadcast address). This is the only one you really ever need to change. *(Defaults to "" AKA 0.0.0.0 AKA all interfaces)*
 - **PORT** - Which UDP port you want to listen on. Shouldn't need to ever 
 change this. *(Defaults to 6454)*
 
 <details>
 <summary>The following are used for purely management purposes:</summary>
 
 - **SYSIP** - What the IP address of your system is. Purely cosmetic and only used to identify the system to ArtNet controllers. *(Defaults to "10.10.10.1")*
 - **MAC** - What the MAC address of your system is. Same as above. *(Defaults to ["AA","BB","CC","DD","EE","FF"])*
 - **SWVER** - What version of Art-Net we're using. In this case, V1.4 *(Defaults to "14")*
-- **SHORTNAME** and **LONGAME** - Used to see what devices are what on a controller. *(Shortname is truncated to 17 bytes long, longname is truncated to 63)*
+- **SHORTNAME** and **LONGNAME** - Used to see what devices are what on a controller. *(Shortname is truncated to 17 bytes long, longname is truncated to 63)*
 - **OEMCODE** - What the Art-Net OEM code your device has. Only needs to be set if you have one. *(In hex)*
 - **ESTACODE** - What the ESTA Manafacturer Code your device has. Only needs to be set if you have one. *(In hex)*
 - **PORTTYPE** - Used to tell the controller what type of physical ports your device has. *(Defaults to [0x80,0x00,0x00,0x00])* *See the Art-Net documentation for more information*
 - **REFRESH** - What the refresh rate (in Hz) of your device. *(Defaults to 44 (the max for DMX))*
 - **DEBUG** - Used to turn on debug output. *(Defaults to False)*
 </details>
 
-Further information on how it all works can be found in the [Art-Net documentation](https://www.artisticlicence.com/WebSiteMaster/User%20Guides/art-net.pdf).
+### The artnet packet consists of the following:
+- **ver** - Which version of Art-Net the packet is using. *Latest is V1.4 (14)*
+- **sequence** - Sequence number, used to check if the packets have arrived in the correct order *(counts up to 255)*
+- **physical** - The physical DMX512 port this data came from
+- **universe** - Which universe this packet is meant for
+- **data** - The data in the packet
+- **length** - How much DMX data we have *(full packet is 18+length)*
+
+
+### The following functions are available to use:
+- **readPacket** - Returns the last Art-Net packet that we received. *(Returns ArtnetPacket)*
+- **readBuffer** - Returns the last Art-Net packet that we received for each universe. *(Returns an array of ArtnetPacket, one per universe)*
+- **close** - Make sure to run this at the end of your program. Tells the socket to stop running and joins the thread back. *(Returns None)*
+- **version** - Returns the library version. *(Returns String)*
+
+
+Further information on how it all works can be found in the [Art-Net documentation](https://www.artisticlicence.com/WebSiteMaster/User%20Guides/art-net.pdf).\
+*Art-Net™ Designed by and Copyright Artistic Licence Engineering Ltd*
+
 ## License
 This project is licensed under an MIT License (see the [LICENSE](LICENSE) file).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

