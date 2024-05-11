# Comparing `tmp/pyCubes-0.4.1.tar.gz` & `tmp/pycubes-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyCubes-0.4.1.tar", max compression
+gzip compressed data, was "pycubes-0.4.2.tar", last modified: Sat May 11 13:32:52 2024, max compression
```

## Comparing `pyCubes-0.4.1.tar` & `pycubes-0.4.2.tar`

### file list

```diff
@@ -1,28 +1,26 @@
--rw-r--r--   0        0        0     1063 2021-12-09 06:31:48.382935 pyCubes-0.4.1/LICENSE
--rw-r--r--   0        0        0     2651 2021-12-09 06:31:48.382935 pyCubes-0.4.1/README.md
--rw-r--r--   0        0        0        0 2021-12-09 06:31:48.382935 pyCubes-0.4.1/cubes/__init__.py
--rw-r--r--   0        0        0      567 2021-12-09 06:31:48.382935 pyCubes-0.4.1/cubes/nbt.py
--rw-r--r--   0        0        0       98 2021-12-09 06:31:48.382935 pyCubes-0.4.1/cubes/net/__init__.py
--rw-r--r--   0        0        0     1623 2021-12-09 06:31:48.382935 pyCubes-0.4.1/cubes/net/connection.py
--rw-r--r--   0        0        0      798 2021-12-09 06:31:48.382935 pyCubes-0.4.1/cubes/net/serializers/__init__.py
--rw-r--r--   0        0        0      791 2021-12-09 06:31:48.382935 pyCubes-0.4.1/cubes/net/serializers/_abc.py
--rw-r--r--   0        0        0     7707 2021-12-09 06:31:48.382935 pyCubes-0.4.1/cubes/net/serializers/_entity_metadata.py
--rw-r--r--   0        0        0      724 2021-12-09 06:31:48.382935 pyCubes-0.4.1/cubes/net/serializers/_mixins.py
--rw-r--r--   0        0        0      880 2021-12-09 06:31:48.382935 pyCubes-0.4.1/cubes/net/serializers/_nbt.py
--rw-r--r--   0        0        0     4931 2021-12-09 06:31:48.382935 pyCubes-0.4.1/cubes/net/serializers/_particle.py
--rw-r--r--   0        0        0     1753 2021-12-09 06:31:48.382935 pyCubes-0.4.1/cubes/net/serializers/_position.py
--rw-r--r--   0        0        0     2351 2021-12-09 06:31:48.382935 pyCubes-0.4.1/cubes/net/serializers/_simple.py
--rw-r--r--   0        0        0     1360 2021-12-09 06:31:48.382935 pyCubes-0.4.1/cubes/net/serializers/_slot.py
--rw-r--r--   0        0        0     1140 2021-12-09 06:31:48.382935 pyCubes-0.4.1/cubes/net/serializers/_string.py
--rw-r--r--   0        0        0      655 2021-12-09 06:31:48.382935 pyCubes-0.4.1/cubes/net/serializers/_uuid.py
--rw-r--r--   0        0        0     1974 2021-12-09 06:31:48.382935 pyCubes-0.4.1/cubes/net/serializers/_var_length.py
--rw-r--r--   0        0        0     2858 2021-12-09 06:31:48.382935 pyCubes-0.4.1/cubes/net/server.py
--rw-r--r--   0        0        0      239 2021-12-09 06:31:48.382935 pyCubes-0.4.1/cubes/types_/__init__.py
--rw-r--r--   0        0        0      143 2021-12-09 06:31:48.382935 pyCubes-0.4.1/cubes/types_/_mixins.py
--rw-r--r--   0        0        0     1195 2021-12-09 06:31:48.382935 pyCubes-0.4.1/cubes/types_/entity.py
--rw-r--r--   0        0        0     5624 2021-12-09 06:31:48.382935 pyCubes-0.4.1/cubes/types_/particle.py
--rw-r--r--   0        0        0      697 2021-12-09 06:31:48.382935 pyCubes-0.4.1/cubes/types_/slot.py
--rw-r--r--   0        0        0      261 2021-12-09 06:31:48.382935 pyCubes-0.4.1/cubes/utils.py
--rw-r--r--   0        0        0     2014 2021-12-09 06:31:48.386936 pyCubes-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     3682 2021-12-09 06:32:01.560496 pyCubes-0.4.1/setup.py
--rw-r--r--   0        0        0     4139 2021-12-09 06:32:01.560894 pyCubes-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-01 07:14:50.092546 pycubes-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2629 2024-05-11 13:15:42.195371 pycubes-0.4.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 07:23:28.936879 pycubes-0.4.2/cubes/__init__.py
+-rw-r--r--   0        0        0      584 2024-05-11 13:15:42.195700 pycubes-0.4.2/cubes/nbt.py
+-rw-r--r--   0        0        0       80 2024-05-11 13:15:42.196005 pycubes-0.4.2/cubes/net/__init__.py
+-rw-r--r--   0        0        0     1455 2024-05-11 13:15:42.196324 pycubes-0.4.2/cubes/net/connection.py
+-rw-r--r--   0        0        0      107 2024-05-03 13:21:49.318781 pycubes-0.4.2/cubes/net/packetflow.py
+-rw-r--r--   0        0        0      662 2024-05-11 13:15:42.196639 pycubes-0.4.2/cubes/net/serializers/__init__.py
+-rw-r--r--   0        0        0      859 2024-04-30 07:23:28.937466 pycubes-0.4.2/cubes/net/serializers/_abc.py
+-rw-r--r--   0        0        0      738 2024-05-11 13:15:42.196984 pycubes-0.4.2/cubes/net/serializers/_mixins.py
+-rw-r--r--   0        0        0      880 2024-04-30 07:23:28.937838 pycubes-0.4.2/cubes/net/serializers/_nbt.py
+-rw-r--r--   0        0        0     1757 2024-05-11 13:15:42.197352 pycubes-0.4.2/cubes/net/serializers/_position.py
+-rw-r--r--   0        0        0     2351 2024-05-11 10:48:00.677048 pycubes-0.4.2/cubes/net/serializers/_simple.py
+-rw-r--r--   0        0        0     1140 2024-04-30 07:23:28.938392 pycubes-0.4.2/cubes/net/serializers/_string.py
+-rw-r--r--   0        0        0      655 2024-04-30 07:23:28.938487 pycubes-0.4.2/cubes/net/serializers/_uuid.py
+-rw-r--r--   0        0        0     1981 2024-05-11 13:15:42.197705 pycubes-0.4.2/cubes/net/serializers/_var_length.py
+-rw-r--r--   0        0        0     2858 2024-05-11 11:57:11.364963 pycubes-0.4.2/cubes/net/server.py
+-rw-r--r--   0        0        0      311 2024-05-11 13:15:42.198050 pycubes-0.4.2/cubes/utils.py
+-rw-r--r--   0        0        0     2613 2024-05-11 13:32:52.017339 pycubes-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-11 13:15:42.200032 pycubes-0.4.2/tests/__init__.py
+-rw-r--r--   0        0        0       88 2024-04-30 07:23:28.942056 pycubes-0.4.2/tests/conftest.py
+-rw-r--r--   0        0        0      452 2024-04-30 07:23:28.942212 pycubes-0.4.2/tests/data/test_data.snbt
+-rw-r--r--   0        0        0    12083 2024-05-11 13:15:42.200469 pycubes-0.4.2/tests/net/test_serializers.py
+-rw-r--r--   0        0        0     2051 2024-05-11 13:15:42.200788 pycubes-0.4.2/tests/net/test_server_and_conn.py
+-rw-r--r--   0        0        0      135 2024-05-11 13:15:42.201058 pycubes-0.4.2/tests/test_utils.py
+-rw-r--r--   0        0        0     4045 1970-01-01 00:00:00.000000 pycubes-0.4.2/PKG-INFO
```

### Comparing `pyCubes-0.4.1/LICENSE` & `pycubes-0.4.2/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Dmitry
+Copyright (c) 2021-2024 Dmitry
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pyCubes-0.4.1/README.md` & `pycubes-0.4.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,54 +3,56 @@
 <p align="center">
 <a href="https://pypi.org/project/pycubes"><img alt="PyPI" src="https://img.shields.io/pypi/v/pycubes"></a>
 <a href="https://pypi.org/project/pycubes"><img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/pycubes"></a>
 <a href="https://pypi.org/project/pycubes"><img alt="PyPI - License" src="https://img.shields.io/pypi/l/pyCubes"></a>
 <a href="https://pepy.tech/project/pycubes"><img alt="Downloads" src="https://pepy.tech/badge/pycubes/month"></a>
 </p>
 <p align="center">
-<a href="https://github.com/DavisDmitry/pyCubes/actions/workflows/test.yml"><img alt="Test" src="https://github.com/DavisDmitry/pyCubes/actions/workflows/test.yml/badge.svg"></a>
-<a href="https://github.com/DavisDmitry/pyCubes/actions/workflows/lint.yml"><img alt="Lint" src="https://github.com/DavisDmitry/pyCubes/actions/workflows/lint.yml/badge.svg"></a>
+<a href="https://github.com/DavisDmitry/pyCubes/actions/workflows/test.yml"><img alt="Test" src="https://github.com/DavisDmitry/pyCubes/actions/workflows/test.yml/badge.svg?branch=master"></a>
+<a href="https://github.com/DavisDmitry/pyCubes/actions/workflows/lint.yml"><img alt="Lint" src="https://github.com/DavisDmitry/pyCubes/actions/workflows/lint.yml/badge.svg?branch=master"></a>
 <a href="https://codecov.io/gh/DavisDmitry/pyCubes"><img alt="codecov" src="https://codecov.io/gh/DavisDmitry/pyCubes/branch/master/graph/badge.svg?token=Y18ZNYT4YS"></a>
 </p>
 <p align="center">
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 <a href="https://pycqa.github.io/isort"><img alt="Imports: isort" src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336"></a>
 </p>
 
 ---
+
 <p align="center">
 <a href="https://pycubes.dmitrydavis.xyz">Documentation</a> | 
 <a href="https://github.com/DavisDmitry/pyCubes/tree/master/examples">Examples</a> | 
 <a href="https://wiki.vg/Protocol">Protocol Specification</a>
 </p>
 
 ---
-pyCubes is a library for creating servers and clients for Minecraft Java Edition (1.14+).
+
+pyCubes is a library for creating servers and clients for Minecraft Java Edition.
 
 **❗ 0.x versions are not stable. The library API is subject to change.**
 
 ## Installation
 
 ```bash
 pip install pyCubes
 ```
 
 ## Features
 
-* Serializers for [Data types](https://wiki.vg/Data_types) (missing Chat, use String instead)
-* Connection
-* Low level server
-* NBT module (wrapper over the [nbtlib](https://github.com/vberlier/nbtlib))
-* `generate_uuid` utility (generates UUID by player_name for using in offline mode)
-* [AnyIO](https://github.com/agronholm/anyio) support (an asynchronous networking and concurrency library)
+- Serializers for some [Data types](https://wiki.vg/Data_types)
+- Connection
+- Low level server
+- NBT module (wrapper over the [nbtlib](https://github.com/vberlier/nbtlib))
+- `generate_uuid` utility (generates UUID by player_name for using in offline mode)
+- [AnyIO](https://github.com/agronholm/anyio) support (an asynchronous networking and concurrency library)
 
 ## TODO
 
-* [x] Serializer for all packets Data types
-* [ ] Packets descriptor
-* [ ] Implement compression
-* [ ] High level server application with event driven API
-* [ ] High level client application with event driven API
-* [ ] High level proxy application with event driven API
-* [ ] Chat API (chat messages constructor)
-* [ ] Commands API
-* [ ] Add API Reference to docs
+- [x] Serializers for Data types
+- [ ] Network packets
+- [ ] Implement compression
+- [ ] High level server application with event driven API
+- [ ] High level client application with event driven API
+- [ ] High level proxy application with event driven API
+- [ ] Chat API (chat messages constructor)
+- [ ] Commands API
+- [ ] Add API Reference to docs
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
                              ************ ppyyCCuubbeess ************
            _[_P_y_P_I_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _L_i_c_e_n_s_e_]_[_D_o_w_n_l_o_a_d_s_]
                              _[_T_e_s_t_]_[_L_i_n_t_]_[_c_o_d_e_c_o_v_]
                       _[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_I_m_p_o_r_t_s_:_ _i_s_o_r_t_]
 ---
                _D_o_c_u_m_e_n_t_a_t_i_o_n | _E_x_a_m_p_l_e_s | _P_r_o_t_o_c_o_l_ _S_p_e_c_i_f_i_c_a_t_i_o_n
 --- pyCubes is a library for creating servers and clients for Minecraft Java
-Edition (1.14+). **â 0.x versions are not stable. The library API is subject
-to change.** ## Installation ```bash pip install pyCubes ``` ## Features *
-Serializers for [Data types](https://wiki.vg/Data_types) (missing Chat, use
-String instead) * Connection * Low level server * NBT module (wrapper over the
-[nbtlib](https://github.com/vberlier/nbtlib)) * `generate_uuid` utility
-(generates UUID by player_name for using in offline mode) * [AnyIO](https://
-github.com/agronholm/anyio) support (an asynchronous networking and concurrency
-library) ## TODO * [x] Serializer for all packets Data types * [ ] Packets
-descriptor * [ ] Implement compression * [ ] High level server application with
-event driven API * [ ] High level client application with event driven API *
-[ ] High level proxy application with event driven API * [ ] Chat API (chat
-messages constructor) * [ ] Commands API * [ ] Add API Reference to docs
+Edition. **â 0.x versions are not stable. The library API is subject to
+change.** ## Installation ```bash pip install pyCubes ``` ## Features -
+Serializers for some [Data types](https://wiki.vg/Data_types) - Connection -
+Low level server - NBT module (wrapper over the [nbtlib](https://github.com/
+vberlier/nbtlib)) - `generate_uuid` utility (generates UUID by player_name for
+using in offline mode) - [AnyIO](https://github.com/agronholm/anyio) support
+(an asynchronous networking and concurrency library) ## TODO - [x] Serializers
+for Data types - [ ] Network packets - [ ] Implement compression - [ ] High
+level server application with event driven API - [ ] High level client
+application with event driven API - [ ] High level proxy application with event
+driven API - [ ] Chat API (chat messages constructor) - [ ] Commands API - [ ]
+Add API Reference to docs
```

### Comparing `pyCubes-0.4.1/cubes/nbt.py` & `pycubes-0.4.2/cubes/nbt.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,16 +4,17 @@
     From it you can use classes: `Byte`, `ByteArray`, `Compound`, `Double`, `End`,
     `Float`, `Int`, `IntArray`, `List`, `Long`, `LongArray`, `Short`, `String`
     and the function `schema`.
 
 Examples:
     >>> cubes.nbt.String('vberlier is cool!')
 """
+
 # pylint: disable=W0611
-from nbtlib import (
+from nbtlib import (  # type: ignore
     Byte,
     ByteArray,
     Compound,
     Double,
     End,
     Float,
     Int,
```

### Comparing `pyCubes-0.4.1/cubes/net/connection.py` & `pycubes-0.4.2/cubes/net/connection.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,43 @@
-import enum
 import io
+from typing import cast
 
 import anyio
 import anyio.abc
 
 from cubes.net import serializers
 
 
 class _LengthVarIntSerializer(serializers.VarIntSerializer):
     _MAX_BYTES = 3
     _RANGE = (1, 2097151)
 
 
-class ConnectionStatus(enum.IntEnum):
-    HANDSHAKE = 0
-    STATUS = 1
-    LOGIN = 2
-    PLAY = 3
-
-
 class Connection:
-    __slots__ = ("_stream", "_remote_address", "_local_address", "_status")
+    __slots__ = ("_stream", "_remote_address", "_local_address", "_state")
 
     def __init__(self, stream: anyio.abc.SocketStream):
         self._stream = stream
-        self._remote_address = stream.extra(anyio.abc.SocketAttribute.remote_address)
-        self._local_address = stream.extra(anyio.abc.SocketAttribute.local_address)
-        self._status = ConnectionStatus.HANDSHAKE
+        self._remote_address = cast(
+            anyio.abc.IPSockAddrType,
+            stream.extra(anyio.abc.SocketAttribute.remote_address),
+        )
+        self._local_address = cast(
+            anyio.abc.IPSockAddrType,
+            stream.extra(anyio.abc.SocketAttribute.local_address),
+        )
 
     @property
-    def status(self) -> ConnectionStatus:
-        return self._status
-
-    @property
-    def remote_address(self) -> tuple[str, int]:
+    def remote_address(self) -> anyio.abc.IPSockAddrType:
         return self._remote_address
 
     @property
-    def local_address(self) -> tuple[str, int]:
+    def local_address(self) -> anyio.abc.IPSockAddrType:
         return self._local_address
 
-    @status.setter
-    def status(self, value: ConnectionStatus):
-        self._status = value
-
     async def receive(self) -> io.BytesIO:
         length = await _LengthVarIntSerializer.from_stream(self._stream)
         return io.BytesIO(await self._stream.receive(length))
 
     async def send(self, *packets: io.BytesIO) -> None:
         buffer = io.BytesIO()
         for packet in packets:
```

### Comparing `pyCubes-0.4.1/cubes/net/serializers/__init__.py` & `pycubes-0.4.2/cubes/net/serializers/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-from cubes.net.serializers._entity_metadata import EntityMetadataSerializer
+from cubes.net.serializers._abc import AbstractSerializer
 from cubes.net.serializers._nbt import NBTSerializer
-from cubes.net.serializers._particle import ParticleSerializer
 from cubes.net.serializers._position import PositionSerializer
 from cubes.net.serializers._simple import (
     AngleSerializer,
     BooleanSerializer,
     ByteSerializer,
     DoubleSerializer,
     FloatSerializer,
     IntSerializer,
     LongSerializer,
     ShortSerializer,
     UnsignedByteSerializer,
     UnsignedShortSerializer,
 )
-from cubes.net.serializers._slot import SlotSerializer
 from cubes.net.serializers._string import IdentifierSerializer, StringSerializer
 from cubes.net.serializers._uuid import UUIDSerializer
 from cubes.net.serializers._var_length import VarIntSerializer, VarLongSerializer
```

### Comparing `pyCubes-0.4.1/cubes/net/serializers/_abc.py` & `pycubes-0.4.2/cubes/net/serializers/_abc.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,18 @@
     __slots__ = ("_value",)
 
     def __init__(self, value: T, validate: bool = True):
         if validate:
             self.validate(value)
         self._value = value
 
+    @property
+    def value(self) -> T:
+        return self._value
+
     @classmethod
     @abc.abstractmethod
     def validate(cls, value: T) -> None:
         """"""
 
     @abc.abstractmethod
     def serialize(self) -> bytes:
```

### Comparing `pyCubes-0.4.1/cubes/net/serializers/_mixins.py` & `pycubes-0.4.2/cubes/net/serializers/_mixins.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import io
 
 from cubes.net.serializers import _abc
 
 
 class StupidValidationMixin(_abc.AbstractSerializer[_abc.T]):
-    TYPE: _abc.T
+    _TYPE: type[_abc.T]
 
     @classmethod
     def validate(cls, value: _abc.T) -> None:
         cls._TYPE(value)
 
 
 class RangeValidationMixin(_abc.AbstractSerializer[_abc.T]):
-    TYPE: _abc.T
+    _TYPE: type[_abc.T]
     _RANGE: tuple[_abc.T, _abc.T]
 
     @classmethod
     def validate(cls, value: _abc.T) -> None:
         value = cls._TYPE(value)
         min_, max_ = cls._RANGE
         if value < min_ or value > max_:
```

### Comparing `pyCubes-0.4.1/cubes/net/serializers/_nbt.py` & `pycubes-0.4.2/cubes/net/serializers/_nbt.py`

 * *Files identical despite different names*

### Comparing `pyCubes-0.4.1/cubes/net/serializers/_position.py` & `pycubes-0.4.2/cubes/net/serializers/_position.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,18 +36,18 @@
                 self._to_twos_complement(y, 12),
             )
         )
         return struct.pack(">Q", value)
 
     @classmethod
     def deserialize(cls, data: bytes) -> tuple[int, int, int]:
-        data = struct.unpack(">Q", data)[0]
-        x = cls._from_twos_complement(data >> 38, 26)
-        z = cls._from_twos_complement(data >> 12 & 0x3FFFFFF, 26)
-        y = cls._from_twos_complement(data & 0xFFF, 12)
+        _data = struct.unpack(">Q", data)[0]
+        x = cls._from_twos_complement(_data >> 38, 26)
+        z = cls._from_twos_complement(_data >> 12 & 0x3FFFFFF, 26)
+        y = cls._from_twos_complement(_data & 0xFFF, 12)
         return x, y, z
 
     def to_buffer(self, buffer: io.BytesIO) -> None:
         buffer.write(self.serialize())
 
     @classmethod
     def from_buffer(cls, buffer: io.BytesIO) -> tuple[int, int, int]:
```

### Comparing `pyCubes-0.4.1/cubes/net/serializers/_simple.py` & `pycubes-0.4.2/cubes/net/serializers/_simple.py`

 * *Files identical despite different names*

### Comparing `pyCubes-0.4.1/cubes/net/serializers/_string.py` & `pycubes-0.4.2/cubes/net/serializers/_string.py`

 * *Files identical despite different names*

### Comparing `pyCubes-0.4.1/cubes/net/serializers/_uuid.py` & `pycubes-0.4.2/cubes/net/serializers/_uuid.py`

 * *Files identical despite different names*

### Comparing `pyCubes-0.4.1/cubes/net/serializers/_var_length.py` & `pycubes-0.4.2/cubes/net/serializers/_var_length.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             if not byte & 0x80:
                 break
         if result & (1 << (cls._BYTES_SHIFT - 1)):
             result -= 1 << cls._BYTES_SHIFT
         return result
 
     @classmethod
-    async def from_stream(cls, buffer: anyio.abc.ByteStream) -> int:
+    async def from_stream(cls, buffer: anyio.abc.ByteReceiveStream) -> int:
         result = 0
         for index in range(cls._MAX_BYTES):
             byte = ord(await buffer.receive(1))
             result |= (byte & 0x7F) << 7 * index
             if not byte & 0x80:
                 break
         if result & (1 << (cls._BYTES_SHIFT - 1)):
```

### Comparing `pyCubes-0.4.1/cubes/net/server.py` & `pycubes-0.4.2/cubes/net/server.py`

 * *Files identical despite different names*

### Comparing `pyCubes-0.4.1/pyproject.toml` & `pycubes-0.4.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,66 +1,118 @@
-[tool.poetry]
+[project]
 name = "pyCubes"
-version = "0.4.1"
+version = "0.4.2"
 description = "Library for creating servers and clients for Minecraft Java Edition"
-authors = ["Dmitry Davis <dmitrydavis@protonmail.com>"]
-license = "MIT"
+authors = [
+    { name = "DmitryDavis", email = "dmitrydavis@protonmail.com" },
+    { name = "Dmitry Davis", email = "dmitrydavis@protonmail.com" },
+]
+dependencies = [
+    "anyio>=4.3.0",
+    "nbtlib>=2.0.4",
+]
+requires-python = "<4.0,>=3.10"
 readme = "README.md"
-homepage = "https://github.com/DavisDmitry/pyCubes"
-documentation = "https://pycubes.dmitrydavis.xyz"
 classifiers = [
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Internet",
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Software Development :: Libraries :: Python Modules",
-    "Typing :: Typed"
+    "Typing :: Typed",
+]
+
+[project.license]
+text = "MIT"
+
+[project.urls]
+homepage = "https://github.com/DavisDmitry/pyCubes"
+documentation = "https://pycubes.dmitrydavis.xyz"
+
+[build-system]
+requires = [
+    "pdm-backend",
+]
+build-backend = "pdm.backend"
+
+[tool.pdm]
+distribution = true
+
+[tool.pdm.dev-dependencies]
+dev = [
+    "trio>=0.25.0",
+]
+linters = [
+    "black>=24.4.2",
+    "isort>=5.13.2",
+    "mypy>=1.10.0",
+    "pylint>=3.1.0",
+]
+tests = [
+    "pytest>=8.2.0",
+    "pytest-cov>=5.0.0",
+]
+docs = [
+    "mkdocs-material>=9.5.20",
+    "mkdocs-static-i18n>=1.2.2",
+    "pymdown-extensions>=10.8.1",
 ]
-packages = [{include="cubes"}]
 
-[tool.poetry.dependencies]
-python = "^3.10"
-anyio = "^3.4.0"
-nbtlib = "2.0.4"
-pydantic = "^1.8.2"
-mkdocs-material = {version = "^8.0.5", optional = true}
-mkdocs-static-i18n = {version = "^0.22", optional = true}
-pymdown-extensions = {version = "^9.1", optional = true}
-
-[tool.poetry.extras]
-docs = ["mkdocs-material", "mkdocs-static-i18n", "pymdown-extensions", "mkautodoc"]
-
-[tool.poetry.dev-dependencies]
-black = "^21.12b0"
-flake8 = "^4.0.1"
-flake8-annotations-complexity = "^0.0.6"
-flake8-annotations-coverage = "^0.0.5"
-flake8-bandit = "^2.1.2"
-flake8-bugbear = "^21.11.29"
-isort = "^5.9.3"
-pylint = "^2.12.2"
-pytest = "^6.2.5"
-pytest-cov = "^3.0.0"
-trio = "^0.19.0"
+[tool.pdm.scripts]
+_isort_format = "isort ."
+_black_format = "black ."
+_mypy = "mypy cubes tests"
+_pylint = "pylint cubes"
+_isort_lint = "isort --check --diff ."
+_black_lint = "black --check --diff ."
+test = "pytest --cov=cubes --cov-report=term-missing"
+docs-serve = "mkdocs serve"
+docs-build = "mkdocs build"
+docs-deploy = "mkdocs gh-deploy -m \"📝 Update docs\""
+
+[tool.pdm.scripts.format]
+composite = [
+    "_isort_format",
+    "_black_format",
+]
+
+[tool.pdm.scripts.lint]
+composite = [
+    "_mypy",
+    "_pylint",
+    "_isort_lint",
+    "_black_lint",
+]
+keep_going = true
+
+[tool.pdm.build]
+includes = [
+    "cubes",
+]
 
 [tool.black]
-target-version = ['py310']
+target-version = [
+    "py310",
+]
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 
 [tool.pylint.message_control]
-disable = ["C0112", "C0114", "C0115", "C0116"]
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+disable = [
+    "C0112",
+    "C0114",
+    "C0115",
+    "C0116",
+]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyCubes-0.4.1/PKG-INFO` & `pycubes-0.4.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,91 +1,89 @@
 Metadata-Version: 2.1
-Name: pycubes
-Version: 0.4.1
+Name: pyCubes
+Version: 0.4.2
 Summary: Library for creating servers and clients for Minecraft Java Edition
 Home-page: https://github.com/DavisDmitry/pyCubes
+Author-Email: DmitryDavis <dmitrydavis@protonmail.com>, Dmitry Davis <dmitrydavis@protonmail.com>
 License: MIT
-Author: Dmitry Davis
-Author-email: dmitrydavis@protonmail.com
-Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Provides-Extra: docs
-Requires-Dist: anyio (>=3.4.0,<4.0.0)
-Requires-Dist: mkdocs-material (>=8.0.5,<9.0.0); extra == "docs"
-Requires-Dist: mkdocs-static-i18n (>=0.22,<0.23); extra == "docs"
-Requires-Dist: nbtlib (==2.0.4)
-Requires-Dist: pydantic (>=1.8.2,<2.0.0)
-Requires-Dist: pymdown-extensions (>=9.1,<10.0); extra == "docs"
+Project-URL: Homepage, https://github.com/DavisDmitry/pyCubes
 Project-URL: Documentation, https://pycubes.dmitrydavis.xyz
+Requires-Python: <4.0,>=3.10
+Requires-Dist: anyio>=4.3.0
+Requires-Dist: nbtlib>=2.0.4
 Description-Content-Type: text/markdown
 
 <h1 align="center">pyCubes</h1>
 
 <p align="center">
 <a href="https://pypi.org/project/pycubes"><img alt="PyPI" src="https://img.shields.io/pypi/v/pycubes"></a>
 <a href="https://pypi.org/project/pycubes"><img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/pycubes"></a>
 <a href="https://pypi.org/project/pycubes"><img alt="PyPI - License" src="https://img.shields.io/pypi/l/pyCubes"></a>
 <a href="https://pepy.tech/project/pycubes"><img alt="Downloads" src="https://pepy.tech/badge/pycubes/month"></a>
 </p>
 <p align="center">
-<a href="https://github.com/DavisDmitry/pyCubes/actions/workflows/test.yml"><img alt="Test" src="https://github.com/DavisDmitry/pyCubes/actions/workflows/test.yml/badge.svg"></a>
-<a href="https://github.com/DavisDmitry/pyCubes/actions/workflows/lint.yml"><img alt="Lint" src="https://github.com/DavisDmitry/pyCubes/actions/workflows/lint.yml/badge.svg"></a>
+<a href="https://github.com/DavisDmitry/pyCubes/actions/workflows/test.yml"><img alt="Test" src="https://github.com/DavisDmitry/pyCubes/actions/workflows/test.yml/badge.svg?branch=master"></a>
+<a href="https://github.com/DavisDmitry/pyCubes/actions/workflows/lint.yml"><img alt="Lint" src="https://github.com/DavisDmitry/pyCubes/actions/workflows/lint.yml/badge.svg?branch=master"></a>
 <a href="https://codecov.io/gh/DavisDmitry/pyCubes"><img alt="codecov" src="https://codecov.io/gh/DavisDmitry/pyCubes/branch/master/graph/badge.svg?token=Y18ZNYT4YS"></a>
 </p>
 <p align="center">
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 <a href="https://pycqa.github.io/isort"><img alt="Imports: isort" src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336"></a>
 </p>
 
 ---
+
 <p align="center">
 <a href="https://pycubes.dmitrydavis.xyz">Documentation</a> | 
 <a href="https://github.com/DavisDmitry/pyCubes/tree/master/examples">Examples</a> | 
 <a href="https://wiki.vg/Protocol">Protocol Specification</a>
 </p>
 
 ---
-pyCubes is a library for creating servers and clients for Minecraft Java Edition (1.14+).
+
+pyCubes is a library for creating servers and clients for Minecraft Java Edition.
 
 **❗ 0.x versions are not stable. The library API is subject to change.**
 
 ## Installation
 
 ```bash
 pip install pyCubes
 ```
 
 ## Features
 
-* Serializers for [Data types](https://wiki.vg/Data_types) (missing Chat, use String instead)
-* Connection
-* Low level server
-* NBT module (wrapper over the [nbtlib](https://github.com/vberlier/nbtlib))
-* `generate_uuid` utility (generates UUID by player_name for using in offline mode)
-* [AnyIO](https://github.com/agronholm/anyio) support (an asynchronous networking and concurrency library)
+- Serializers for some [Data types](https://wiki.vg/Data_types)
+- Connection
+- Low level server
+- NBT module (wrapper over the [nbtlib](https://github.com/vberlier/nbtlib))
+- `generate_uuid` utility (generates UUID by player_name for using in offline mode)
+- [AnyIO](https://github.com/agronholm/anyio) support (an asynchronous networking and concurrency library)
 
 ## TODO
 
-* [x] Serializer for all packets Data types
-* [ ] Packets descriptor
-* [ ] Implement compression
-* [ ] High level server application with event driven API
-* [ ] High level client application with event driven API
-* [ ] High level proxy application with event driven API
-* [ ] Chat API (chat messages constructor)
-* [ ] Commands API
-* [ ] Add API Reference to docs
-
+- [x] Serializers for Data types
+- [ ] Network packets
+- [ ] Implement compression
+- [ ] High level server application with event driven API
+- [ ] High level client application with event driven API
+- [ ] High level proxy application with event driven API
+- [ ] Chat API (chat messages constructor)
+- [ ] Commands API
+- [ ] Add API Reference to docs
```

#### html2text {}

```diff
@@ -1,39 +1,39 @@
-Metadata-Version: 2.1 Name: pycubes Version: 0.4.1 Summary: Library for
+Metadata-Version: 2.1 Name: pyCubes Version: 0.4.2 Summary: Library for
 creating servers and clients for Minecraft Java Edition Home-page: https://
-github.com/DavisDmitry/pyCubes License: MIT Author: Dmitry Davis Author-email:
-dmitrydavis@protonmail.com Requires-Python: >=3.10,<4.0 Classifier: Intended
-Audience :: Developers Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3 :: Only Classifier: Programming Language :: Python :: 3.10 Classifier:
+github.com/DavisDmitry/pyCubes Author-Email: DmitryDavis
+protonmail.com>, Dmitry Davis
+protonmail.com> License: MIT Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators Classifier: License ::
+OSI Approved :: MIT License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier: Topic
 :: Internet Classifier: Topic :: Software Development Classifier: Topic ::
 Software Development :: Libraries Classifier: Topic :: Software Development ::
 Libraries :: Application Frameworks Classifier: Topic :: Software Development
-:: Libraries :: Python Modules Classifier: Typing :: Typed Provides-Extra: docs
-Requires-Dist: anyio (>=3.4.0,<4.0.0) Requires-Dist: mkdocs-material
-(>=8.0.5,<9.0.0); extra == "docs" Requires-Dist: mkdocs-static-i18n
-(>=0.22,<0.23); extra == "docs" Requires-Dist: nbtlib (==2.0.4) Requires-Dist:
-pydantic (>=1.8.2,<2.0.0) Requires-Dist: pymdown-extensions (>=9.1,<10.0);
-extra == "docs" Project-URL: Documentation, https://pycubes.dmitrydavis.xyz
-Description-Content-Type: text/markdown
+:: Libraries :: Python Modules Classifier: Typing :: Typed Project-URL:
+Homepage, https://github.com/DavisDmitry/pyCubes Project-URL: Documentation,
+https://pycubes.dmitrydavis.xyz Requires-Python: <4.0,>=3.10 Requires-Dist:
+anyio>=4.3.0 Requires-Dist: nbtlib>=2.0.4 Description-Content-Type: text/
+markdown
                              ************ ppyyCCuubbeess ************
            _[_P_y_P_I_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _L_i_c_e_n_s_e_]_[_D_o_w_n_l_o_a_d_s_]
                              _[_T_e_s_t_]_[_L_i_n_t_]_[_c_o_d_e_c_o_v_]
                       _[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_I_m_p_o_r_t_s_:_ _i_s_o_r_t_]
 ---
                _D_o_c_u_m_e_n_t_a_t_i_o_n | _E_x_a_m_p_l_e_s | _P_r_o_t_o_c_o_l_ _S_p_e_c_i_f_i_c_a_t_i_o_n
 --- pyCubes is a library for creating servers and clients for Minecraft Java
-Edition (1.14+). **â 0.x versions are not stable. The library API is subject
-to change.** ## Installation ```bash pip install pyCubes ``` ## Features *
-Serializers for [Data types](https://wiki.vg/Data_types) (missing Chat, use
-String instead) * Connection * Low level server * NBT module (wrapper over the
-[nbtlib](https://github.com/vberlier/nbtlib)) * `generate_uuid` utility
-(generates UUID by player_name for using in offline mode) * [AnyIO](https://
-github.com/agronholm/anyio) support (an asynchronous networking and concurrency
-library) ## TODO * [x] Serializer for all packets Data types * [ ] Packets
-descriptor * [ ] Implement compression * [ ] High level server application with
-event driven API * [ ] High level client application with event driven API *
-[ ] High level proxy application with event driven API * [ ] Chat API (chat
-messages constructor) * [ ] Commands API * [ ] Add API Reference to docs
+Edition. **â 0.x versions are not stable. The library API is subject to
+change.** ## Installation ```bash pip install pyCubes ``` ## Features -
+Serializers for some [Data types](https://wiki.vg/Data_types) - Connection -
+Low level server - NBT module (wrapper over the [nbtlib](https://github.com/
+vberlier/nbtlib)) - `generate_uuid` utility (generates UUID by player_name for
+using in offline mode) - [AnyIO](https://github.com/agronholm/anyio) support
+(an asynchronous networking and concurrency library) ## TODO - [x] Serializers
+for Data types - [ ] Network packets - [ ] Implement compression - [ ] High
+level server application with event driven API - [ ] High level client
+application with event driven API - [ ] High level proxy application with event
+driven API - [ ] Chat API (chat messages constructor) - [ ] Commands API - [ ]
+Add API Reference to docs
```

