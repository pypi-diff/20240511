# Comparing `tmp/pyckb-0.2.0.tar.gz` & `tmp/pyckb-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyckb-0.2.0.tar", last modified: Sun May  5 01:43:59 2024, max compression
+gzip compressed data, was "pyckb-0.2.1.tar", last modified: Sat May 11 01:13:14 2024, max compression
```

## Comparing `pyckb-0.2.0.tar` & `pyckb-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-05 01:43:59.690624 pyckb-0.2.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1065 2023-12-30 04:14:24.000000 pyckb-0.2.0/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4232 2024-05-05 01:43:59.686623 pyckb-0.2.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2722 2024-04-10 03:25:41.000000 pyckb-0.2.0/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-05 01:43:59.686623 pyckb-0.2.0/ckb/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      195 2024-04-29 09:12:52.000000 pyckb-0.2.0/ckb/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4637 2024-04-19 12:01:42.000000 pyckb-0.2.0/ckb/bech32m.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4149 2024-04-26 09:57:50.000000 pyckb-0.2.0/ckb/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17860 2024-05-05 01:35:59.000000 pyckb-0.2.0/ckb/core.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       30 2024-04-29 09:13:08.000000 pyckb-0.2.0/ckb/denomination.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1565 2024-05-02 03:14:12.000000 pyckb-0.2.0/ckb/ecdsa.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3773 2024-05-05 01:36:48.000000 pyckb-0.2.0/ckb/molecule.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2373 2024-04-23 08:43:17.000000 pyckb-0.2.0/ckb/rpc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4324 2024-04-30 05:58:44.000000 pyckb-0.2.0/ckb/secp256k1.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23980 2024-05-05 01:39:01.000000 pyckb-0.2.0/ckb/wallet.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-05 01:43:59.686623 pyckb-0.2.0/pyckb.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4232 2024-05-05 01:43:59.000000 pyckb-0.2.0/pyckb.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      398 2024-05-05 01:43:59.000000 pyckb-0.2.0/pyckb.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-05 01:43:59.000000 pyckb-0.2.0/pyckb.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-05-05 01:43:59.000000 pyckb-0.2.0/pyckb.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        4 2024-05-05 01:43:59.000000 pyckb-0.2.0/pyckb.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      370 2024-05-05 01:43:14.000000 pyckb-0.2.0/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-05 01:43:59.690624 pyckb-0.2.0/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-05 01:43:59.686623 pyckb-0.2.0/test/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2237 2024-05-05 01:31:03.000000 pyckb-0.2.0/test/test_core.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      586 2024-01-12 02:25:22.000000 pyckb-0.2.0/test/test_ecdsa.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1235 2024-05-05 01:28:02.000000 pyckb-0.2.0/test/test_rpc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1807 2024-04-29 09:17:31.000000 pyckb-0.2.0/test/test_wallet.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-11 01:13:14.142755 pyckb-0.2.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1065 2023-12-30 04:14:24.000000 pyckb-0.2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4232 2024-05-11 01:13:14.142755 pyckb-0.2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2722 2024-04-10 03:25:41.000000 pyckb-0.2.1/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-11 01:13:14.142755 pyckb-0.2.1/ckb/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      194 2024-05-10 14:37:32.000000 pyckb-0.2.1/ckb/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4991 2024-05-11 01:08:28.000000 pyckb-0.2.1/ckb/bech32.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4149 2024-04-26 09:57:50.000000 pyckb-0.2.1/ckb/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17744 2024-05-10 14:40:46.000000 pyckb-0.2.1/ckb/core.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       30 2024-04-29 09:13:08.000000 pyckb-0.2.1/ckb/denomination.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1565 2024-05-02 03:14:12.000000 pyckb-0.2.1/ckb/ecdsa.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3773 2024-05-05 01:36:48.000000 pyckb-0.2.1/ckb/molecule.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2373 2024-04-23 08:43:17.000000 pyckb-0.2.1/ckb/rpc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4464 2024-05-10 12:59:48.000000 pyckb-0.2.1/ckb/secp256k1.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23980 2024-05-05 01:39:01.000000 pyckb-0.2.1/ckb/wallet.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-11 01:13:14.142755 pyckb-0.2.1/pyckb.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4232 2024-05-11 01:13:14.000000 pyckb-0.2.1/pyckb.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      397 2024-05-11 01:13:14.000000 pyckb-0.2.1/pyckb.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-11 01:13:14.000000 pyckb-0.2.1/pyckb.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-05-11 01:13:14.000000 pyckb-0.2.1/pyckb.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        4 2024-05-11 01:13:14.000000 pyckb-0.2.1/pyckb.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      370 2024-05-11 01:12:43.000000 pyckb-0.2.1/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-11 01:13:14.142755 pyckb-0.2.1/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-11 01:13:14.142755 pyckb-0.2.1/test/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2237 2024-05-05 01:31:03.000000 pyckb-0.2.1/test/test_core.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      586 2024-01-12 02:25:22.000000 pyckb-0.2.1/test/test_ecdsa.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1235 2024-05-05 01:28:02.000000 pyckb-0.2.1/test/test_rpc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1807 2024-04-29 09:17:31.000000 pyckb-0.2.1/test/test_wallet.py
```

### Comparing `pyckb-0.2.0/LICENSE` & `pyckb-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyckb-0.2.0/PKG-INFO` & `pyckb-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyckb
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python SDK for CKB
 Author-email: Mohanson <mohanson@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Mohanson
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyckb-0.2.0/README.md` & `pyckb-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyckb-0.2.0/ckb/bech32m.py` & `pyckb-0.2.1/ckb/bech32.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,104 +18,106 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 # BIP-0173 https://github.com/bitcoin/bips/blob/master/bip-0173.mediawiki
 # BIP-0350 https://github.com/bitcoin/bips/blob/master/bip-0350.mediawiki
 # Derived from https://raw.githubusercontent.com/sipa/bech32/master/ref/python/segwit_addr.py
 #
-# Reference implementation for Bech32/Bech32m and segwit addresses.
+# Reference implementation for Bech32/bech32 and segwit addresses.
 
 import typing
 
 CHARSET = 'qpzry9x8gf2tvdw0s3jn54khce6mua7l'
-CONST = 0x2bc830a3
+CONST_0 = 1
+CONST_M = 0x2bc830a3
 
 
-def bech32m_polymod(data: bytearray) -> int:
+def bech32_polymod(data: bytearray) -> int:
     # Internal function that computes the Bech32 checksum.
     assert isinstance(data, bytearray)
     gen = [0x3b6a57b2, 0x26508e6d, 0x1ea119fa, 0x3d4233dd, 0x2a1462b3]
     chk = 1
     for val in data:
         top = chk >> 25
         chk = chk & 0x1ffffff
         chk = chk << 5 ^ val
         for i in range(5):
             chk ^= gen[i] if ((top >> i) & 1) else 0
     return chk
 
 
-def bech32m_hrp_expand(hrp: str) -> bytearray:
+def bech32_hrpconv(hrp: str) -> bytearray:
     # Expand the HRP into values for checksum computation.
     r = bytearray()
     r.extend([ord(x) >> 5 for x in hrp])
     r.append(0)
     r.extend([ord(x) & 31 for x in hrp])
     return r
 
 
-def bech32m_verify_checksum(hrp: str, data: bytearray) -> bool:
-    # Verify a checksum given HRP and converted data characters.
-    assert isinstance(data, bytearray)
-    return bech32m_polymod(bech32m_hrp_expand(hrp) + bytearray(data)) == CONST
-
-
-def bech32m_create_checksum(hrp: str, data: bytearray) -> bytearray:
-    # Compute the checksum values given HRP and data.
+def bech32_re_arrange_5(data: bytearray) -> bytearray:
+    # Re-arrange those bits into groups of 5, and pad with zeroes at the end if needed.
     assert isinstance(data, bytearray)
-    data = bech32m_hrp_expand(hrp) + data
-    pmod = bech32m_polymod(data + bytearray(6)) ^ CONST
-    return bytearray([(pmod >> 5 * (5 - i)) & 31 for i in range(6)])
+    acc = 0
+    bit = 0
+    ret = bytearray()
+    max_val = 0x1f
+    max_acc = 0xfff
+    for b in data:
+        acc = ((acc << 8) | b) & max_acc
+        bit += 8
+        for _ in range(bit // 5):
+            bit -= 5
+            ret.append((acc >> bit) & max_val)
+    if bit:
+        pad_bit = 5 - bit
+        ret.append((acc << pad_bit) & max_val)
+    return ret
 
 
-def bech32m_encode(hrp: str, data: bytearray) -> str:
-    # Compute a Bech32 string given HRP and data values.
-    assert isinstance(data, bytearray)
-    data = data + bech32m_create_checksum(hrp, data)
-    return hrp + '1' + ''.join([CHARSET[d] for d in data])
+def bech32_create_checksum(hrp: str, ver: int, data: bytearray):
+    hrpdata = bech32_hrpconv(hrp) + data
+    polymod = bech32_polymod(hrpdata + bytearray(6))
+    if ver == 0:
+        polymod = polymod ^ CONST_0
+    if ver >= 1:
+        polymod = polymod ^ CONST_M
+    return bytearray([(polymod >> 5 * (5 - i)) & 31 for i in range(6)])
+
+
+def bech32_verify_checksum(hrp: str, ver: int, data: bytearray):
+    if ver == 0:
+        return bech32_polymod(bech32_hrpconv(hrp) + bytearray(data)) == CONST_0
+    if ver >= 1:
+        return bech32_polymod(bech32_hrpconv(hrp) + bytearray(data)) == CONST_M
 
 
-def bech32m_decode(bech: str) -> typing.Tuple[str, bytearray]:
+def bech32_decode(ver: int, bech: str) -> typing.Tuple[str, bytearray]:
     # Validate a string, and determine HRP and data.
     for c in bech:
         assert ord(c) >= ord('!')
         assert ord(c) <= ord('~')
     bech = bech.lower()
     pos = bech.rfind('1')
     assert pos > 0
     assert pos + 6 < len(bech)
     for c in bech[pos+1:]:
         assert c in CHARSET
     hrp = bech[:pos]
     data = bytearray([CHARSET.find(x) for x in bech[pos+1:]])
-    assert bech32m_verify_checksum(hrp, data)
+    assert bech32_verify_checksum(hrp, ver, data)
     return hrp, data[:-6]
 
 
-def bech32m_re_arrange_5(data: bytearray) -> bytearray:
-    # Re-arrange those bits into groups of 5, and pad with zeroes at the end if needed.
-    assert isinstance(data, bytearray)
-    acc = 0
-    bit = 0
-    ret = bytearray()
-    max_val = 0x1f
-    max_acc = 0xfff
-    for b in data:
-        acc = ((acc << 8) | b) & max_acc
-        bit += 8
-        for _ in range(bit // 5):
-            bit -= 5
-            ret.append((acc >> bit) & max_val)
-    if bit:
-        pad_bit = 5 - bit
-        ret.append((acc << pad_bit) & max_val)
-    return ret
+def bech32_encode(hrp: str, ver: int, data: bytearray):
+    datasum = data + bech32_create_checksum(hrp, ver, data)
+    return hrp + '1' + ''.join([CHARSET[d] for d in datasum])
 
 
-def bech32m_re_arrange_8(data: bytearray) -> bytearray:
+def bech32_re_arrange_8(data: bytearray) -> bytearray:
     # Re-arrange those bits into groups of 8 bits. Any incomplete group at the end MUST be 4 bits or less, MUST be all
     # zeroes, and is discarded.
     assert isinstance(data, bytearray)
     acc = 0
     bit = 0
     ret = bytearray()
     max_val = 0xff
@@ -125,7 +127,22 @@
         acc = ((acc << 5) | b) & max_acc
         bit += 5
         for _ in range(bit // 8):
             bit -= 8
             ret.append((acc >> bit) & max_val)
     assert bit < 5
     return ret
+
+
+def decode(hrp: str, addr: str) -> bytearray:
+    # Decode a segwit address.
+    pre, data = bech32_decode(1, addr)
+    assert pre == hrp
+    return bech32_re_arrange_8(data)
+
+
+def encode(hrp: str, prog: bytearray) -> str:
+    # Encode a segwit address.
+    assert isinstance(prog, bytearray)
+    r = bech32_encode(hrp, 1, bech32_re_arrange_5(prog))
+    assert prog == decode(hrp, r)
+    return r
```

### Comparing `pyckb-0.2.0/ckb/config.py` & `pyckb-0.2.1/ckb/config.py`

 * *Files identical despite different names*

### Comparing `pyckb-0.2.0/ckb/core.py` & `pyckb-0.2.1/ckb/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import ckb.bech32m
+import ckb.bech32
 import ckb.config
 import ckb.ecdsa
 import ckb.molecule
 import ckb.secp256k1
 import hashlib
 import json
 
@@ -168,23 +168,19 @@
     # See: https://github.com/rev-chaos/ckb-address-demo/blob/master/ckb_addr_test.py
     payload = bytearray()
     payload.append(0x00)
     # Append secp256k1 code hash
     payload.extend(script.code_hash)
     payload.append(script.hash_type)
     payload.extend(script.args)
-    return ckb.bech32m.bech32m_encode(
-        ckb.config.current.hrp,
-        ckb.bech32m.bech32m_re_arrange_5(payload),
-    )
+    return ckb.bech32.encode(ckb.config.current.hrp, payload)
 
 
 def address_decode(addr: str) -> Script:
-    _, data = ckb.bech32m.bech32m_decode(addr)
-    payload = bytearray(ckb.bech32m.bech32m_re_arrange_8(data))
+    payload = ckb.bech32.decode(ckb.config.current.hrp, addr)
     assert payload[0] == 0
     code_hash = payload[1:33]
     hash_type = payload[33]
     args = payload[34:]
     return Script(code_hash, hash_type, args)
```

### Comparing `pyckb-0.2.0/ckb/ecdsa.py` & `pyckb-0.2.1/ckb/ecdsa.py`

 * *Files identical despite different names*

### Comparing `pyckb-0.2.0/ckb/molecule.py` & `pyckb-0.2.1/ckb/molecule.py`

 * *Files identical despite different names*

### Comparing `pyckb-0.2.0/ckb/rpc.py` & `pyckb-0.2.1/ckb/rpc.py`

 * *Files identical despite different names*

### Comparing `pyckb-0.2.0/ckb/secp256k1.py` & `pyckb-0.2.1/ckb/secp256k1.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+import typing
+Self = typing.Self
+
+
 class Fp:
     # Galois field. In mathematics, a finite field or Galois field is a field that contains a finite number of elements.
     # As with any field, a finite field is a set on which the operations of multiplication, addition, subtraction and
     # division are defined and satisfy certain basic rules.
     #
     # https://www.cs.miami.edu/home/burt/learning/Csc609.142/ecdsa-cert.pdf
     # Don Johnson, Alfred Menezes and Scott Vanstone, The Elliptic Curve Digital Signature Algorithm (ECDSA)
@@ -11,34 +15,34 @@
 
     def __init__(self, x: int):
         self.x = x % self.p
 
     def __repr__(self):
         return f'Fp(0x{self.x:064x})'
 
-    def __eq__(self, data):
+    def __eq__(self, data: Self):
         assert self.p == data.p
         return self.x == data.x
 
-    def __add__(self, data):
+    def __add__(self, data: Self):
         assert self.p == data.p
         return self.__class__((self.x + data.x) % self.p)
 
-    def __sub__(self, data):
+    def __sub__(self, data: Self):
         assert self.p == data.p
         return self.__class__((self.x - data.x) % self.p)
 
-    def __mul__(self, data):
+    def __mul__(self, data: Self):
         assert self.p == data.p
         return self.__class__((self.x * data.x) % self.p)
 
-    def __truediv__(self, data):
+    def __truediv__(self, data: Self):
         return self * data ** -1
 
-    def __pow__(self, data):
+    def __pow__(self, data: int):
         return self.__class__(pow(self.x, data, self.p))
 
     def __pos__(self):
         return self
 
     def __neg__(self):
         return self.__class__(self.p - self.x)
@@ -92,21 +96,21 @@
             assert y ** 2 == x ** 3 + A * x + B
         self.x = x
         self.y = y
 
     def __repr__(self):
         return f'Pt({self.x}, {self.y})'
 
-    def __eq__(self, data):
+    def __eq__(self, data: Self):
         return all([
             self.x == data.x,
             self.y == data.y,
         ])
 
-    def __add__(self, data):
+    def __add__(self, data: Self) -> Self:
         # https://www.cs.miami.edu/home/burt/learning/Csc609.142/ecdsa-cert.pdf
         # Don Johnson, Alfred Menezes and Scott Vanstone, The Elliptic Curve Digital Signature Algorithm (ECDSA)
         # 4.1 Elliptic Curves Over Fp
         if self.x == Fq(0) and self.y == Fq(0):
             return data
         if data.x == Fq(0) and data.y == Fq(0):
             return self
@@ -118,38 +122,38 @@
             s = (x1 * x1 + x1 * x1 + x1 * x1 + A) / (y1 + y1)
         else:
             s = (y2 - y1) / (x2 - x1)
         x3 = s * s - x1 - x2
         y3 = s * (x1 - x3) - y1
         return Pt(x3, y3)
 
-    def __sub__(self, data):
+    def __sub__(self, data: Self) -> Self:
         return self + data.__neg__()
 
-    def __mul__(self, k: Fr):
+    def __mul__(self, k: Fr) -> Self:
         # Point multiplication: Double-and-add
         # https://en.wikipedia.org/wiki/Elliptic_curve_point_multiplication
         n = k.x
         result = I
         addend = self
         while n:
             b = n & 1
             if b == 1:
                 result += addend
             addend = addend + addend
             n = n >> 1
         return result
 
-    def __truediv__(self, k):
+    def __truediv__(self, k: Fr) -> Self:
         return self.__mul__(k ** -1)
 
-    def __pos__(self):
+    def __pos__(self) -> Self:
         return self
 
-    def __neg__(self):
+    def __neg__(self) -> Self:
         return Pt(self.x, -self.y)
 
 
 # Identity element
 I = Pt(
     Fq(0),
     Fq(0),
```

### Comparing `pyckb-0.2.0/ckb/wallet.py` & `pyckb-0.2.1/ckb/wallet.py`

 * *Files identical despite different names*

### Comparing `pyckb-0.2.0/pyckb.egg-info/PKG-INFO` & `pyckb-0.2.1/pyckb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyckb
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python SDK for CKB
 Author-email: Mohanson <mohanson@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Mohanson
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyckb-0.2.0/test/test_core.py` & `pyckb-0.2.1/test/test_core.py`

 * *Files identical despite different names*

### Comparing `pyckb-0.2.0/test/test_ecdsa.py` & `pyckb-0.2.1/test/test_ecdsa.py`

 * *Files identical despite different names*

### Comparing `pyckb-0.2.0/test/test_rpc.py` & `pyckb-0.2.1/test/test_rpc.py`

 * *Files identical despite different names*

### Comparing `pyckb-0.2.0/test/test_wallet.py` & `pyckb-0.2.1/test/test_wallet.py`

 * *Files identical despite different names*

