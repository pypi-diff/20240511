# Comparing `tmp/cctrusted_base-0.0.3.tar.gz` & `tmp/cctrusted_base-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cctrusted_base-0.0.3.tar", last modified: Wed Dec 27 07:48:57 2023, max compression
+gzip compressed data, was "cctrusted_base-0.4.0.tar", last modified: Mon Apr  8 02:50:10 2024, max compression
```

## Comparing `cctrusted_base-0.0.3.tar` & `cctrusted_base-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 07:48:57.113995 cctrusted_base-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2023-12-27 07:48:57.113995 cctrusted_base-0.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 07:48:57.109995 cctrusted_base-0.0.3/cctrusted_base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 07:48:49.000000 cctrusted_base-0.0.3/cctrusted_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3712 2023-12-27 07:48:49.000000 cctrusted_base-0.0.3/cctrusted_base/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2023-12-27 07:48:49.000000 cctrusted_base-0.0.3/cctrusted_base/binaryblob.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2023-12-27 07:48:49.000000 cctrusted_base-0.0.3/cctrusted_base/ccel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8815 2023-12-27 07:48:49.000000 cctrusted_base-0.0.3/cctrusted_base/eventlog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2023-12-27 07:48:49.000000 cctrusted_base-0.0.3/cctrusted_base/imr.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2023-12-27 07:48:49.000000 cctrusted_base-0.0.3/cctrusted_base/quote.py
--rw-r--r--   0 runner    (1001) docker     (127)    12752 2023-12-27 07:48:49.000000 cctrusted_base-0.0.3/cctrusted_base/tcg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 07:48:57.113995 cctrusted_base-0.0.3/cctrusted_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2023-12-27 07:48:57.000000 cctrusted_base-0.0.3/cctrusted_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      362 2023-12-27 07:48:57.000000 cctrusted_base-0.0.3/cctrusted_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-27 07:48:57.000000 cctrusted_base-0.0.3/cctrusted_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-27 07:48:57.000000 cctrusted_base-0.0.3/cctrusted_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      791 2023-12-27 07:48:49.000000 cctrusted_base-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-27 07:48:57.113995 cctrusted_base-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:50:10.564227 cctrusted_base-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-08 02:50:10.564227 cctrusted_base-0.4.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:50:10.560227 cctrusted_base-0.4.0/cctrusted_base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 02:50:02.000000 cctrusted_base-0.4.0/cctrusted_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-08 02:50:02.000000 cctrusted_base-0.4.0/cctrusted_base/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-08 02:50:02.000000 cctrusted_base-0.4.0/cctrusted_base/binaryblob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-08 02:50:02.000000 cctrusted_base-0.4.0/cctrusted_base/ccel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-08 02:50:02.000000 cctrusted_base-0.4.0/cctrusted_base/ccreport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20578 2024-04-08 02:50:02.000000 cctrusted_base-0.4.0/cctrusted_base/eventlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-08 02:50:02.000000 cctrusted_base-0.4.0/cctrusted_base/imr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22419 2024-04-08 02:50:02.000000 cctrusted_base-0.4.0/cctrusted_base/tcg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19226 2024-04-08 02:50:02.000000 cctrusted_base-0.4.0/cctrusted_base/tcgcel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:50:10.564227 cctrusted_base-0.4.0/cctrusted_base/tdx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 02:50:02.000000 cctrusted_base-0.4.0/cctrusted_base/tdx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-08 02:50:02.000000 cctrusted_base-0.4.0/cctrusted_base/tdx/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41488 2024-04-08 02:50:02.000000 cctrusted_base-0.4.0/cctrusted_base/tdx/quote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9954 2024-04-08 02:50:02.000000 cctrusted_base-0.4.0/cctrusted_base/tdx/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-08 02:50:02.000000 cctrusted_base-0.4.0/cctrusted_base/tdx/rtmr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:50:10.564227 cctrusted_base-0.4.0/cctrusted_base/tpm/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-08 02:50:02.000000 cctrusted_base-0.4.0/cctrusted_base/tpm/pcr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-08 02:50:02.000000 cctrusted_base-0.4.0/cctrusted_base/tpm/quote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:50:10.564227 cctrusted_base-0.4.0/cctrusted_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-08 02:50:10.000000 cctrusted_base-0.4.0/cctrusted_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 02:50:10.000000 cctrusted_base-0.4.0/cctrusted_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 02:50:10.000000 cctrusted_base-0.4.0/cctrusted_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-08 02:50:10.000000 cctrusted_base-0.4.0/cctrusted_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-08 02:50:02.000000 cctrusted_base-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 02:50:10.564227 cctrusted_base-0.4.0/setup.cfg
```

### Comparing `cctrusted_base-0.0.3/PKG-INFO` & `cctrusted_base-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cctrusted_base
-Version: 0.0.3
+Version: 0.4.0
 Summary: CC Trusted API Base SDK
 Author-email: "Lu, Ken" <ken.lu@intel.com>, "Zhang, Wenhui" <wenhui.zhang@bytedance.com>
 License: Apache Software License
 Project-URL: Homepage, https://github.com/cc-api/cc-trusted-api
 Project-URL: Bug Tracker, https://github.com/cc-api/cc-trusted-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `cctrusted_base-0.0.3/cctrusted_base/api.py` & `cctrusted_base-0.4.0/cctrusted_base/api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,45 @@
 """
 The CC Trusted API
 """
+import logging
 from abc import ABC, abstractmethod
 # pylint: disable=unused-import
 from cctrusted_base.imr import TcgIMR
-from cctrusted_base.quote import Quote
-from cctrusted_base.eventlog import TcgEventLog
+from cctrusted_base.eventlog import EventLogs
+from cctrusted_base.ccreport import CcReport
 from cctrusted_base.tcg import TcgAlgorithmRegistry
 
+LOG = logging.getLogger(__name__)
+
 class CCTrustedApi(ABC):
 
     """Abstract class for CC Trusted API.
 
     The inherited SDK class will implement the APIs.
     """
 
+    TYPE_CC_NONE = -1
+    TYPE_CC_TPM = 0
+    TYPE_CC_TDX = 1
+    TYPE_CC_SEV = 2
+    TYPE_CC_CCA = 3
+
+    TYPE_CC_STRING = {
+        TYPE_CC_TPM: "TPM",
+        TYPE_CC_TDX: "TDX",
+        TYPE_CC_SEV: "SEV",
+        TYPE_CC_CCA: "CCA"
+    }
+
+    @staticmethod
+    def cc_type_str(cc_type):
+        """the CC type string."""
+        return CCTrustedApi.TYPE_CC_STRING[cc_type]
+
     @abstractmethod
     def get_default_algorithms(self) -> TcgAlgorithmRegistry:
         """Get the default Digest algorithms supported by trusted foundation.
 
         Different trusted foundation may support different algorithms, for example
         the Intel TDX use SHA384, TPM uses SHA256.
 
@@ -45,15 +66,15 @@
 
         Returns:
             The count of measurement registers
         """
         raise NotImplementedError("Inherited SDK class should implement this.")
 
     @abstractmethod
-    def get_measurement(self, imr_select:[int, int]) -> TcgIMR:
+    def get_cc_measurement(self, imr_select:[int, int]) -> TcgIMR:
         """Get measurement register according to given selected index and algorithms
 
         Each trusted foundation in CC environment provides the multiple measurement
         registers, the count is update to ``get_measurement_count()``. And for each
         measurement register, it may provides multiple digest for different algorithms.
 
         Args:
@@ -62,15 +83,20 @@
 
         Returns:
             The object of TcgIMR
         """
         raise NotImplementedError("Inherited SDK class should implement this.")
 
     @abstractmethod
-    def get_quote(self, nonce: bytearray, data: bytearray, extraArgs=None) -> Quote:
+    def get_cc_report(
+        self,
+        nonce: bytearray = None,
+        data: bytearray = None,
+        extraArgs = None
+    ) -> CcReport:
         """Get the quote for given nonce and data.
 
         The quote is signing of attestation data (IMR values or hashes of IMR
         values), made by a trusted foundation (TPM) using a key trusted by the
         verifier.
 
         Different trusted foundation may use different quote format.
@@ -82,19 +108,46 @@
 
         Returns:
             The ``Quote`` object.
         """
         raise NotImplementedError("Inherited SDK class should implement this.")
 
     @abstractmethod
-    def get_eventlog(self, start:int = None, count:int = None) -> TcgEventLog:
+    def get_cc_eventlog(self, start:int = None, count:int = None) -> list:
         """Get eventlog for given index and count.
 
         TCG log in Eventlog. Verify to spoof events in the TCG log, hence defeating
         remotely-attested measured-boot.
         To measure the full CC runtime environment, the eventlog may include addtional
         OS type and cloud native type event beyond the measured-boot.
 
+        Args:
+            start(int): the first index of event log to fetch
+            count(int): the number of event logs to fetch
+
         Returns:
-            ``TcgEventLog`` object.
+            list of parsed event logs following TCG spec.
         """
         raise NotImplementedError("Inherited SDK class should implement this.")
+
+    @staticmethod
+    def replay_cc_eventlog(event_logs:list) -> dict:
+        """Replay event logs based on data provided.
+
+        TCG event logs can be replayed against IMR measurements to prove the integrity of
+        the event logs.
+
+        Args:
+            event_logs(list): the list of parsed event logs to replay
+
+        Returns:
+            A dictionary containing the replay result displayed by IMR index and hash algorithm.
+            Layer 1 key of the dict is the IMR index, the value is another dict which using the
+            hash algorithm as the key and the replayed measurement as value.
+            Sample value:
+                { 0: { 12: <measurement_replayed> } }
+        """
+        if event_logs is None or len(event_logs) == 0:
+            LOG.info("No event log provided to replay.")
+            return {}
+
+        return EventLogs.replay(event_logs)
```

### Comparing `cctrusted_base-0.0.3/cctrusted_base/binaryblob.py` & `cctrusted_base-0.4.0/cctrusted_base/binaryblob.py`

 * *Files identical despite different names*

### Comparing `cctrusted_base-0.0.3/cctrusted_base/ccel.py` & `cctrusted_base-0.4.0/cctrusted_base/ccel.py`

 * *Files identical despite different names*

### Comparing `cctrusted_base-0.0.3/cctrusted_base/imr.py` & `cctrusted_base-0.4.0/cctrusted_base/imr.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Integrity Measurement Register packages.
 """
 
 from abc import ABC, abstractmethod
-from cctrusted_base.tcg import TcgDigest, TcgAlgorithmRegistry
+from cctrusted_base.tcg import TcgDigest
 
 class TcgIMR(ABC):
     """Common Integrated Measurement Register class."""
 
     _INVALID_IMR_INDEX = -1
 
     def __init__(self, index, default_alg_id, default_digest_hash):
@@ -52,25 +52,7 @@
         """Check whether IMR is valid or not.
 
         Returns:
             whether IMR is valid or not.
         """
         return self._index != TcgIMR._INVALID_IMR_INDEX and \
             self._index <= self.max_index
-
-class TdxRTMR(TcgIMR):
-    """RTMR class defined for Intel TDX."""
-
-    @property
-    def max_index(self):
-        return 3
-
-    def __init__(self, index, digest_hash):
-        super().__init__(index, TcgAlgorithmRegistry.TPM_ALG_SHA384,
-                        digest_hash)
-
-class TpmPCR(TcgIMR):
-    """PCR class defined for TPM"""
-
-    @property
-    def max_index(self):
-        return 23
```

### Comparing `cctrusted_base-0.0.3/cctrusted_base.egg-info/PKG-INFO` & `cctrusted_base-0.4.0/cctrusted_base.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cctrusted_base
-Version: 0.0.3
+Version: 0.4.0
 Summary: CC Trusted API Base SDK
 Author-email: "Lu, Ken" <ken.lu@intel.com>, "Zhang, Wenhui" <wenhui.zhang@bytedance.com>
 License: Apache Software License
 Project-URL: Homepage, https://github.com/cc-api/cc-trusted-api
 Project-URL: Bug Tracker, https://github.com/cc-api/cc-trusted-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `cctrusted_base-0.0.3/pyproject.toml` & `cctrusted_base-0.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cctrusted_base"
-version = "0.0.3"
+version = "0.4.0"
 authors = [
   { name="Lu, Ken", email="ken.lu@intel.com" },
   { name="Zhang, Wenhui", email="wenhui.zhang@bytedance.com" },
 ]
 description = "CC Trusted API Base SDK"
 readme = "README.md"
 license = { text="Apache Software License" }
@@ -23,8 +23,8 @@
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where=["."]
-include=["cctrusted_base"]
+include=["cctrusted_base*"]
```

