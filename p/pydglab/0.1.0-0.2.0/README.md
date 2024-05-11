# Comparing `tmp/pydglab-0.1.0.tar.gz` & `tmp/pydglab-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydglab-0.1.0.tar", max compression
+gzip compressed data, was "pydglab-0.2.0.tar", max compression
```

## Comparing `pydglab-0.1.0.tar` & `pydglab-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      433 2024-05-09 16:48:28.950228 pydglab-0.1.0/pydglab/__init__.py
--rw-r--r--   0        0        0     2865 2024-05-09 16:03:59.657805 pydglab-0.1.0/pydglab/bthandler.py
--rw-r--r--   0        0        0      863 2024-05-09 16:27:20.626534 pydglab-0.1.0/pydglab/model.py
--rw-r--r--   0        0        0     4147 2024-05-09 16:47:53.069229 pydglab-0.1.0/pydglab/service.py
--rw-r--r--   0        0        0      913 2024-05-09 12:50:38.471221 pydglab-0.1.0/pydglab/uuid.py
--rw-r--r--   0        0        0      431 2024-05-09 16:57:58.742981 pydglab-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      270 2024-05-09 16:54:18.502561 pydglab-0.1.0/README.md
--rw-r--r--   0        0        0      901 1970-01-01 00:00:00.000000 pydglab-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35823 2024-05-10 07:01:10.429022 pydglab-0.2.0/LICENSE
+-rw-r--r--   0        0        0      424 2024-05-11 16:46:11.750274 pydglab-0.2.0/pydglab/__init__.py
+-rw-r--r--   0        0        0     3636 2024-05-11 16:49:38.159328 pydglab-0.2.0/pydglab/bthandler.py
+-rw-r--r--   0        0        0     1224 2024-05-11 16:30:14.340564 pydglab-0.2.0/pydglab/model.py
+-rw-r--r--   0        0        0    12188 2024-05-11 16:30:14.340564 pydglab-0.2.0/pydglab/service.py
+-rw-r--r--   0        0        0     1176 2024-05-11 16:30:14.341563 pydglab-0.2.0/pydglab/uuid.py
+-rw-r--r--   0        0        0      431 2024-05-11 16:53:16.930360 pydglab-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      633 2024-05-10 07:01:10.429022 pydglab-0.2.0/README.md
+-rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 pydglab-0.2.0/PKG-INFO
```

### Comparing `pydglab-0.1.0/pydglab/bthandler.py` & `pydglab-0.2.0/pydglab/bthandler.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,64 +5,76 @@
 
 from pydglab.model import *
 from pydglab.uuid import *
 
 logger = logging.getLogger(__name__)
 
 
-async def scan_():
+async def scan():
+    """
+    Scan for DGLAB v2.0 devices and return a list of tuples with the address and the RSSI of the devices found.
+
+    Returns:
+        List[Tuple[str, int]]: (address, RSSI)
+    """
     devices = await BleakScanner().discover(return_adv=True)
-    dglab_v2: List[Tuple] = []
+    dglab_v2: List[Tuple[str, int]] = []
     for i, j in devices.values():
         if j.local_name == CoyoteV2.name and i.address is not None:
             logger.info(f"Found DGLAB v2.0 {i.address}")
             dglab_v2.append((i.address, j.rssi))
     if not dglab_v2:
         logger.error("No DGLAB v2.0 found")
+    return dglab_v2
+
+
+async def scan_():
+    dglab_v2 = await scan()
+    if not dglab_v2:
         raise Exception("No DGLAB v2.0 found")
     if len(dglab_v2) > 1:
         logger.warning("Multiple DGLAB v2.0 found, chosing the closest one")
     elif len(dglab_v2) == 0:
         raise Exception("No DGLAB v2.0 found")
     return sorted(dglab_v2, key=lambda device: device[1])[0][0]
 
 
-async def get_batterylevel_(client: BleakClient):
-    r = await client.read_gatt_char(CoyoteV2.characteristicBattery)
+async def get_batterylevel_(client: BleakClient, characteristics: CoyoteV2 | CoyoteV3):
+    r = await client.read_gatt_char(characteristics.characteristicBattery)
     return r
 
 
-async def get_strength_(client: BleakClient):
-    r = await client.read_gatt_char(CoyoteV2.characteristicEStimPower)
+async def get_strength_(client: BleakClient, characteristics: CoyoteV2 | CoyoteV3):
+    r = await client.read_gatt_char(characteristics.characteristicEStimPower)
     r = BitArray(r).bin
-    return int(r[-11:], 2), int(r[-22:-11], 2)
+    return int(r[-11:], 2) / 7, int(r[-22:-11], 2) / 7
 
 
-async def set_strength_(client: BleakClient, value: Coyote):
+async def set_strength_(client: BleakClient, value: Coyote, characteristics: CoyoteV2 | CoyoteV3):
     # Create a byte array with the strength values.
     # The values are multiplied by 7 to convert them to the correct range.
     binArray = '0b00'+'{0:011b}'.format(value.ChannelB.strength * 7)+'{0:011b}'.format(value.ChannelA.strength * 7)
     array = bytearray(BitArray(bin=binArray).tobytes())
     
-    r = await client.write_gatt_char(CoyoteV2.characteristicEStimPower, array)
-    return r
+    r = await client.write_gatt_char(characteristics.characteristicEStimPower, array)
+    return value.ChannelB.strength * 7, value.ChannelA.strength * 7
 
 
-async def set_wave_(client: BleakClient, value: ChannelA | ChannelB):
+async def set_wave_(client: BleakClient, value: ChannelA | ChannelB, characteristics: CoyoteV2 | CoyoteV3):
     # Create a byte array with the wave values.
     binArray = '0b0000'+'{0:05b}'.format(value.waveZ)+'{0:010b}'.format(value.waveY)+'{0:05b}'.format(value.waveX)
     array = bytearray(BitArray(bin=binArray).tobytes())
 
-    r = await client.write_gatt_char(CoyoteV2.characteristicEStimA if type(value) is ChannelA else CoyoteV2.characteristicEStimB, array)
-    return r
+    r = await client.write_gatt_char(characteristics.characteristicEStimA if type(value) is ChannelA else characteristics.characteristicEStimB, array)
+    return value.waveX, value.waveY, value.waveZ
 
 
-async def set_wave_sync_(client: BleakClient, value: Coyote):
+async def set_wave_sync_(client: BleakClient, value: Coyote, characteristics: CoyoteV2 | CoyoteV3):
     # Create a byte array with the wave values.
     binArrayA = '0b0000'+'{0:05b}'.format(value.ChannelA.waveZ)+'{0:010b}'.format(value.ChannelA.waveY)+'{0:05b}'.format(value.ChannelA.waveX)
     arrayA = bytearray(BitArray(bin=binArrayA).tobytes())
     
     binArrayB = '0b0000'+'{0:05b}'.format(value.ChannelB.waveZ)+'{0:010b}'.format(value.ChannelB.waveY)+'{0:05b}'.format(value.ChannelB.waveX)
     arrayB = bytearray(BitArray(bin=binArrayB).tobytes())
     
-    r = await client.write_gatt_char(CoyoteV2.characteristicEStimA, arrayA), await client.write_gatt_char(CoyoteV2.characteristicEStimB, arrayB)
-    return r
+    r = await client.write_gatt_char(characteristics.characteristicEStimA, arrayA), await client.write_gatt_char(characteristics.characteristicEStimB, arrayB)
+    return (value.ChannelA.waveX, value.ChannelA.waveY, value.ChannelA.waveZ), (value.ChannelB.waveX, value.ChannelB.waveY, value.ChannelB.waveZ)
```

