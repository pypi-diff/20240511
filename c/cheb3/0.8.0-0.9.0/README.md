# Comparing `tmp/cheb3-0.8.0.tar.gz` & `tmp/cheb3-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheb3-0.8.0.tar", last modified: Wed Oct 25 07:40:54 2023, max compression
+gzip compressed data, was "cheb3-0.9.0.tar", last modified: Sat Jan 27 14:43:08 2024, max compression
```

## Comparing `cheb3-0.8.0.tar` & `cheb3-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 07:40:54.787443 cheb3-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-10-25 07:40:43.000000 cheb3-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2023-10-25 07:40:54.787443 cheb3-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      882 2023-10-25 07:40:46.000000 cheb3-0.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 07:40:54.787443 cheb3-0.8.0/cheb3/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2023-10-25 07:40:43.000000 cheb3-0.8.0/cheb3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2023-10-25 07:40:43.000000 cheb3-0.8.0/cheb3/account.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2023-10-25 07:40:43.000000 cheb3-0.8.0/cheb3/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-10-25 07:40:43.000000 cheb3-0.8.0/cheb3/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     9799 2023-10-25 07:40:43.000000 cheb3-0.8.0/cheb3/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     9197 2023-10-25 07:40:43.000000 cheb3-0.8.0/cheb3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 07:40:54.787443 cheb3-0.8.0/cheb3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2023-10-25 07:40:54.000000 cheb3-0.8.0/cheb3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      284 2023-10-25 07:40:54.000000 cheb3-0.8.0/cheb3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-25 07:40:54.000000 cheb3-0.8.0/cheb3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-10-25 07:40:54.000000 cheb3-0.8.0/cheb3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-10-25 07:40:54.000000 cheb3-0.8.0/cheb3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      736 2023-10-25 07:40:43.000000 cheb3-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-25 07:40:54.787443 cheb3-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 14:43:08.870144 cheb3-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-01-27 14:43:01.000000 cheb3-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-01-27 14:43:08.870144 cheb3-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-01-27 14:43:02.000000 cheb3-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 14:43:08.870144 cheb3-0.9.0/cheb3/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-01-27 14:43:01.000000 cheb3-0.9.0/cheb3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-01-27 14:43:01.000000 cheb3-0.9.0/cheb3/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-01-27 14:43:01.000000 cheb3-0.9.0/cheb3/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-01-27 14:43:01.000000 cheb3-0.9.0/cheb3/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9799 2024-01-27 14:43:01.000000 cheb3-0.9.0/cheb3/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10120 2024-01-27 14:43:01.000000 cheb3-0.9.0/cheb3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 14:43:08.870144 cheb3-0.9.0/cheb3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-01-27 14:43:08.000000 cheb3-0.9.0/cheb3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-01-27 14:43:08.000000 cheb3-0.9.0/cheb3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-27 14:43:08.000000 cheb3-0.9.0/cheb3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-27 14:43:08.000000 cheb3-0.9.0/cheb3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-27 14:43:08.000000 cheb3-0.9.0/cheb3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-01-27 14:43:01.000000 cheb3-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-27 14:43:08.870144 cheb3-0.9.0/setup.cfg
```

### Comparing `cheb3-0.8.0/LICENSE` & `cheb3-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cheb3-0.8.0/PKG-INFO` & `cheb3-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheb3
-Version: 0.8.0
+Version: 0.9.0
 Summary: Web3 CTF tool based on web3.py
 Author-email: YanhuiJessica <y4nhv1@gmail.com>
 Project-URL: Homepage, https://github.com/YanhuiJessica/cheb3
 Project-URL: Documentation, https://cheb3.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/YanhuiJessica/cheb3
 Project-URL: Bug Reports, https://github.com/YanhuiJessica/cheb3/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cheb3-0.8.0/README.rst` & `cheb3-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `cheb3-0.8.0/cheb3/account.py` & `cheb3-0.9.0/cheb3/account.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,34 +43,39 @@
         eth_acct = cast(Account, PropertyCheckingFactory(cls.__name__, (cls,), {"w3": w3}))
         return eth_acct
 
     def get_balance(self) -> int:
         """Returns the balance of the account instance."""
         return self.w3.eth.get_balance(self.eth_acct.address)
 
-    def call(self, to: HexStr, data: HexStr = "0x") -> HexBytes:
+    def call(self, to: HexStr, data: HexStr = "0x", **kwargs) -> HexBytes:
         """Interact with a smart contract without creating a new
         transaction on the blockchain.
 
         :param to: The address of the contract.
         :type to: HexStr
         :param data: The transaction data, defaults to `0x`.
         :type data: HexStr
 
+        Keyword Args:
+            state_override (dict): Specify the state override set.
+                View `Geth documentation <https://geth.ethereum.org/docs/interacting-with-geth/rpc/ns-eth#eth-call>`_ for more details.
+
         :rtype: ~hexbytes.main.HexBytes
         """
 
         to = Web3.to_checksum_address(to)
 
         return self.w3.eth.call(
             {
                 "to": to,
                 "from": self.address,
                 "data": data,
-            }
+            },
+            state_override=kwargs.get("state_override", None),
         )
 
     def send_transaction(self, to: Union[HexStr, None], value: int = 0, data: HexStr = "0x", **kwargs) -> TxReceipt:
         """Transfer ETH or interact with a smart contract.
 
         :param to: The address of the receiver.
         :type to: Union[HexStr, None]
```

### Comparing `cheb3-0.8.0/cheb3/connection.py` & `cheb3-0.9.0/cheb3/connection.py`

 * *Files identical despite different names*

### Comparing `cheb3-0.8.0/cheb3/contract.py` & `cheb3-0.9.0/cheb3/contract.py`

 * *Files identical despite different names*

### Comparing `cheb3-0.8.0/cheb3/utils.py` & `cheb3-0.9.0/cheb3/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os
+import json
 from typing import List, Tuple, Dict, Union, Any, Iterable
 from hexbytes import HexBytes
 from itertools import accumulate
 
 from web3 import Web3
 from web3.exceptions import MismatchedABI
 from eth_typing import HexStr
@@ -11,14 +13,36 @@
 from solcx import compile_source, set_solc_version
 from solcx.install import install_solc
 from solcx.exceptions import SolcNotInstalled
 
 from cheb3.constants import TYPE_ALIAS
 
 
+def load_compiled(contract_file: str, contract_name: str = None, base_path: str = "out/") -> Tuple[Dict, str]:
+    """Loads compiled contracts from the project.
+
+    :param contract_file: The name of the contract file.
+    :type contract_file: str
+    :param contract_name: Specifies the contract to be loaded. Defaults
+        to the contract filename without suffix.
+    :type contract_name: str
+    :param base_path: Use the given path as the root of the source tree
+        to load the compiled output. Defaults to "out/".
+    :type base_path: str
+
+    :return: ABI and bytecode of the required contract.
+    :rtype: Tuple[Dict, str]
+    """
+
+    contract_name = contract_name or os.path.splitext(contract_file)[0]
+    with open(os.path.join(base_path, contract_file, f"{contract_name}.json"), "r") as f:
+        compiled = json.load(f)
+        return (compiled["abi"], compiled["bytecode"]["object"])
+
+
 def compile_file(
     contract_file: str,
     contract_names: Union[str, List[str]] = None,
     solc_version: str = None,
     base_path: str = None,
 ) -> Dict[str, Tuple[Dict, str]]:
     """Compile the Solidity source in the given file.
@@ -193,15 +217,15 @@
             sig += f"{types[i]},"
         return (sig[:-1], types)
 
     ret = dfs(signature[signature.find("(") + 1: -1])
     signature = signature[: signature.find("(") + 1] + ret[0] + ")"
     types = ret[1]
     if len(types) != len(args):
-        raise MismatchedABI("Thypee supplied parameters do not match the signatrue.")
+        raise MismatchedABI("Supplied parameters do not match the signature.")
 
     selector = Web3.solidity_keccak(["string"], [signature])[:4]
 
     parameters = eth_abi.encode(types, args)
     return f"0x{(selector + parameters).hex()}"
```

### Comparing `cheb3-0.8.0/cheb3.egg-info/PKG-INFO` & `cheb3-0.9.0/cheb3.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheb3
-Version: 0.8.0
+Version: 0.9.0
 Summary: Web3 CTF tool based on web3.py
 Author-email: YanhuiJessica <y4nhv1@gmail.com>
 Project-URL: Homepage, https://github.com/YanhuiJessica/cheb3
 Project-URL: Documentation, https://cheb3.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/YanhuiJessica/cheb3
 Project-URL: Bug Reports, https://github.com/YanhuiJessica/cheb3/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cheb3-0.8.0/pyproject.toml` & `cheb3-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cheb3"
-version = "0.8.0"
+version = "0.9.0"
 authors = [{name = "YanhuiJessica",email = "y4nhv1@gmail.com"}]
 description = "Web3 CTF tool based on web3.py"
 readme = "README.rst"
 requires-python = ">=3.8"
 dependencies = [
   "web3>=6.10.0",
   "py-solc-x",
```

