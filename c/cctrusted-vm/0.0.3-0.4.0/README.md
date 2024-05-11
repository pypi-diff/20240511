# Comparing `tmp/cctrusted_vm-0.0.3.tar.gz` & `tmp/cctrusted_vm-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cctrusted_vm-0.0.3.tar", last modified: Wed Dec 27 07:49:10 2023, max compression
+gzip compressed data, was "cctrusted_vm-0.4.0.tar", last modified: Mon Apr  8 03:08:49 2024, max compression
```

## Comparing `cctrusted_vm-0.0.3.tar` & `cctrusted_vm-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 07:49:10.877832 cctrusted_vm-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2023-12-27 07:49:10.877832 cctrusted_vm-0.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 07:49:10.877832 cctrusted_vm-0.0.3/cctrusted_vm/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-12-27 07:48:49.000000 cctrusted_vm-0.0.3/cctrusted_vm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13583 2023-12-27 07:48:49.000000 cctrusted_vm-0.0.3/cctrusted_vm/cvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2023-12-27 07:48:49.000000 cctrusted_vm-0.0.3/cctrusted_vm/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2023-12-27 07:48:49.000000 cctrusted_vm-0.0.3/cctrusted_vm/tdx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 07:49:10.877832 cctrusted_vm-0.0.3/cctrusted_vm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2023-12-27 07:49:10.000000 cctrusted_vm-0.0.3/cctrusted_vm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      261 2023-12-27 07:49:10.000000 cctrusted_vm-0.0.3/cctrusted_vm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-27 07:49:10.000000 cctrusted_vm-0.0.3/cctrusted_vm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-27 07:49:10.000000 cctrusted_vm-0.0.3/cctrusted_vm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      785 2023-12-27 07:48:49.000000 cctrusted_vm-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-27 07:49:10.877832 cctrusted_vm-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 07:49:10.877832 cctrusted_vm-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2023-12-27 07:48:49.000000 cctrusted_vm-0.0.3/tests/test_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:08:49.366724 cctrusted_vm-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-08 03:08:49.366724 cctrusted_vm-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-08 03:08:42.000000 cctrusted_vm-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:08:49.366724 cctrusted_vm-0.4.0/cctrusted_vm/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-08 03:08:42.000000 cctrusted_vm-0.4.0/cctrusted_vm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19141 2024-04-08 03:08:42.000000 cctrusted_vm-0.4.0/cctrusted_vm/cvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-04-08 03:08:42.000000 cctrusted_vm-0.4.0/cctrusted_vm/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-08 03:08:42.000000 cctrusted_vm-0.4.0/cctrusted_vm/tdx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:08:49.366724 cctrusted_vm-0.4.0/cctrusted_vm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-08 03:08:49.000000 cctrusted_vm-0.4.0/cctrusted_vm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-08 03:08:49.000000 cctrusted_vm-0.4.0/cctrusted_vm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 03:08:49.000000 cctrusted_vm-0.4.0/cctrusted_vm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 03:08:49.000000 cctrusted_vm-0.4.0/cctrusted_vm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-08 03:08:49.000000 cctrusted_vm-0.4.0/cctrusted_vm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-08 03:08:42.000000 cctrusted_vm-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 03:08:49.366724 cctrusted_vm-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:08:49.366724 cctrusted_vm-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-08 03:08:42.000000 cctrusted_vm-0.4.0/tests/test_sdk.py
```

### Comparing `cctrusted_vm-0.0.3/cctrusted_vm/cvm.py` & `cctrusted_vm-0.4.0/cctrusted_vm/cvm.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,44 +8,37 @@
 """
 import base64
 import hashlib
 import os
 import logging
 import struct
 import fcntl
+import socket
 from abc import abstractmethod
-from cctrusted_base.imr import TdxRTMR,TcgIMR
-from cctrusted_base.quote import Quote
+from cctrusted_base.api import CCTrustedApi
+from cctrusted_base.imr import TcgIMR
+from cctrusted_base.ccreport import CcReport
 from cctrusted_base.tcg import TcgAlgorithmRegistry
 from cctrusted_base.tdx.common import TDX_VERSION_1_0, TDX_VERSION_1_5
-from cctrusted_base.tdx.quote import TdxQuoteReq10, TdxQuoteReq15
+from cctrusted_base.tdx.rtmr import TdxRTMR
+from cctrusted_base.tdx.quote import TdxQuoteReq10, TdxQuoteReq15, TdxQuote, TdxQuoteReq
 from cctrusted_base.tdx.report import TdxReportReq10, TdxReportReq15
 
 LOG = logging.getLogger(__name__)
 
 class ConfidentialVM:
 
-    TYPE_CC_NONE = -1
-    TYPE_CC_TDX = 0
-    TYPE_CC_SEV = 1
-    TYPE_CC_CCA = 2
-
-    TYPE_CC_STRING = {
-        TYPE_CC_TDX: "TDX",
-        TYPE_CC_SEV: "SEV",
-        TYPE_CC_CCA: "CCA"
-    }
-
     _inst = None
 
     def __init__(self, cctype):
         self._cc_type:int = cctype
         self._is_init:bool = False
         self._imrs:dict[int, TcgIMR] = {}
-        self._cc_event_log:bytes = None
+        self._boot_time_event_log:bytes = None
+        self._runtime_event_log = None
 
     @property
     def cc_type(self) -> int:
         """CC type like TYPE_CC_TDX, TYPE_CC_SEV etc."""
         return self._cc_type
 
     @property
@@ -64,20 +57,25 @@
     def imrs(self) -> list[TcgIMR]:
         """The array of integrated measurement registers (IMR)."""
         return self._imrs
 
     @property
     def cc_type_str(self):
         """the CC type string."""
-        return ConfidentialVM.TYPE_CC_STRING[self.cc_type]
+        return CCTrustedApi.cc_type_str[self.cc_type]
+
+    @property
+    def boot_time_event_log(self):
+        """boot time event log data blob."""
+        return self._boot_time_event_log
 
     @property
-    def cc_event_log(self):
-        """event log data blob."""
-        return self._cc_event_log
+    def runtime_event_log(self):
+        """runtime event log data blob"""
+        return self._runtime_event_log
 
     def init(self) -> bool:
         """Initialize the CC stub and environment.
 
         Returns:
             Success or not
         """
@@ -95,19 +93,19 @@
 
     @staticmethod
     def detect_cc_type():
         """Detect the type of current confidential VM"""
         # TODO: refine the justification
         for devpath in TdxVM.DEVICE_NODE_PATH.values():
             if os.path.exists(devpath):
-                return ConfidentialVM.TYPE_CC_TDX
-        return ConfidentialVM.TYPE_CC_NONE
+                return CCTrustedApi.TYPE_CC_TDX
+        return CCTrustedApi.TYPE_CC_NONE
 
     @abstractmethod
-    def process_cc_report(self) -> bool:
+    def process_cc_report(self, report_data=None) -> bool:
         """Process the confidential computing REPORT.
 
         Returns:
             Success or not.
         """
         raise NotImplementedError("Should be implemented by inherited class")
 
@@ -117,48 +115,53 @@
 
         Returns:
             Success or not.
         """
         raise NotImplementedError("Should be implemented by inherited class")
 
     @abstractmethod
-    def get_quote(self, nonce: bytearray, data: bytearray, extraArgs) -> Quote:
-        """Get the quote for given nonce and data.
+    def get_cc_report(self, nonce: bytearray, data: bytearray, extraArgs) -> CcReport:
+        """Get the CcReport (i.e. quote) for given nonce and data.
 
-        The quote is signing of attestation data (IMR values or hashes of IMR
+        The CcReport is signing of attestation data (IMR values or hashes of IMR
         values), made by a trusted foundation (TPM) using a key trusted by the
         verifier.
 
         Different trusted foundation may use different quote format.
 
         Args:
             nonce (bytearray): against replay attacks.
             data (bytearray): user data
             extraArgs: for TPM, it will be given list of IMR/PCRs
 
         Returns:
-            The ``Quote`` object.
+            The ``CcReport`` object.
         """
         raise NotImplementedError("Should be implemented by inherited class")
 
     def dump(self):
         """Dump confidential VM information."""
         LOG.info("======================================")
         LOG.info("CVM type = %s", self.cc_type_str)
         LOG.info("CVM version = %s", self.version)
         LOG.info("======================================")
 
     @staticmethod
     def inst():
         """Singleton interface for the instance of CcLinuxStub"""
         if ConfidentialVM._inst is None:
+            obj = None
             cc_type = ConfidentialVM.detect_cc_type()
-            if cc_type is ConfidentialVM.TYPE_CC_TDX:
+            if cc_type is CCTrustedApi.TYPE_CC_TDX:
                 obj = TdxVM()
-            if obj.init():
+            else:
+                LOG.error("Unsupported confidential environment.")
+                return None
+
+            if obj is not None and obj.init():
                 ConfidentialVM._inst = obj
             else:
                 LOG.error("Fail to initialize the confidential VM.")
         return ConfidentialVM._inst
 
 class TdxVM(ConfidentialVM):
 
@@ -209,19 +212,22 @@
 
     # The length of the tdquote 4 pages
     TDX_QUOTE_LEN = 4 * 4096
 
     # ACPI table containing the event logs
     ACPI_TABLE_FILE = "/sys/firmware/acpi/tables/CCEL"
     ACPI_TABLE_DATA_FILE = "/sys/firmware/acpi/tables/data/CCEL"
+    IMA_DATA_FILE = "/sys/kernel/security/integrity/ima/ascii_runtime_measurements"
+    CFG_FILE_PATH = "/etc/tdx-attest.conf"
 
     def __init__(self):
-        ConfidentialVM.__init__(self, ConfidentialVM.TYPE_CC_TDX)
+        ConfidentialVM.__init__(self, CCTrustedApi.TYPE_CC_TDX)
         self._version:str = None
         self._tdreport = None
+        self._config:dict = self._load_config()
 
     @property
     def version(self):
         if self._version is None:
             for key, value in TdxVM.DEVICE_NODE_PATH.items():
                 if os.path.exists(value):
                     self._version = key
@@ -232,15 +238,43 @@
         return TcgAlgorithmRegistry.TPM_ALG_SHA384
 
     @property
     def tdreport(self):
         """TDREPORT structure"""
         return self._tdreport
 
-    def process_cc_report(self) -> bool:
+    def _load_config(self):
+        """Process TDX attest config file and fetch params within the config."""
+        tdx_config_dict = {}
+        if os.path.exists(TdxVM.CFG_FILE_PATH):
+            LOG.debug("Found TDX Config file at %s", TdxVM.CFG_FILE_PATH)
+            try:
+                with open(TdxVM.CFG_FILE_PATH, 'rb') as cfg_file:
+                    cfg_info = [line.rstrip() for line in cfg_file]
+                    for line in cfg_info:
+                        # remove spaces in each line
+                        # save all configs into tdx_config_dict
+                        line = line.decode("utf-8").replace(" ", "")
+                        param = line.partition("=")
+                        tdx_config_dict[param[0]] = param[2]
+            except(PermissionError, OSError):
+                LOG.error("Need root permission to open file %s for params.",
+                          TdxVM.CFG_FILE_PATH)
+                return None
+
+            # convert port param into integer and check its validity
+            if "port" in tdx_config_dict:
+                tdx_config_dict["port"] = int(tdx_config_dict["port"])
+                if tdx_config_dict["port"] < 0 or tdx_config_dict["port"] > 65535:
+                    LOG.debug("Invalid vsock port specified in the config.")
+                    del tdx_config_dict["port"]
+
+        return tdx_config_dict
+
+    def process_cc_report(self, report_data=None) -> bool:
         """Process the confidential computing REPORT."""
         dev_path = self.DEVICE_NODE_PATH[self.version]
         try:
             tdx_dev = os.open(dev_path, os.O_RDWR)
         except (PermissionError, IOError, OSError):
             LOG.error("Fail to open device node %s", dev_path)
             return False
@@ -249,15 +283,15 @@
 
         if self.version is TDX_VERSION_1_0:
             tdreport_req = TdxReportReq10()
         elif self.version is TDX_VERSION_1_5:
             tdreport_req = TdxReportReq15()
 
         # pylint: disable=E1111
-        reqbuf = tdreport_req.prepare_reqbuf()
+        reqbuf = tdreport_req.prepare_reqbuf(report_data)
         try:
             fcntl.ioctl(tdx_dev, self.IOCTL_GET_REPORT[self.version], reqbuf)
         except OSError:
             LOG.error("Fail to execute ioctl for file %s", dev_path)
             os.close(tdx_dev)
             return False
 
@@ -293,43 +327,63 @@
             False means error occurred in event log processing
 
         Raises:
             PermissionError: An error occurred when accessing CCEL files
         """
 
         # verify if CCEL files existed
-        if not os.path.exists(TdxVM.ACPI_TABLE_FILE):
-            LOG.error("Failed to find TDX CCEL table at %s", TdxVM.ACPI_TABLE_FILE)
-            return False
-
-        if not os.path.exists(TdxVM.ACPI_TABLE_DATA_FILE):
-            LOG.error("Failed to find TDX CCEL data file at %s", TdxVM.ACPI_TABLE_DATA_FILE)
+        if (not os.path.exists(TdxVM.ACPI_TABLE_FILE) or
+            not os.path.exists(TdxVM.ACPI_TABLE_DATA_FILE)):
+            LOG.error("Failed to find TDX CCEL table at %s or CCEL data file at %s",
+                      TdxVM.ACPI_TABLE_FILE, TdxVM.ACPI_TABLE_DATA_FILE)
             return False
 
         try:
             with open(TdxVM.ACPI_TABLE_FILE, "rb") as f:
                 ccel_data = f.read()
                 assert len(ccel_data) > 0 and ccel_data[0:4] == b'CCEL', \
                     "Invalid CCEL table"
         except (PermissionError, OSError):
             LOG.error("Need root permission to open file %s", TdxVM.ACPI_TABLE_FILE)
             return False
 
         try:
             with open(TdxVM.ACPI_TABLE_DATA_FILE, "rb") as f:
-                self._cc_event_log = f.read()
-                assert len(self._cc_event_log) > 0
+                self._boot_time_event_log = f.read()
+                assert len(self._boot_time_event_log) > 0
         except (PermissionError, OSError):
             LOG.error("Need root permission to open file %s", TdxVM.ACPI_TABLE_DATA_FILE)
             return False
+
+        # Check if the identifier 'ima_hash=sha384' exists on kernel cmdline
+        # If yes, suppose IMA over RTMR enabled in kernel (IMA over RTMR patch included in
+        # https://github.com/intel/tdx-tools/blob/tdx-1.5/build/common/patches-tdx-kernel-MVP-KERNEL-6.2.16-v5.0.tar.gz)
+        # If not, suppose IMA over RTMR not enabled in kernel
+        with open("/proc/cmdline", encoding="utf-8") as cmdfile:
+            cmdline = cmdfile.read().splitlines()
+            if "ima_hash=sha384" not in cmdline[0].split(" "):
+                return True
+
+        if not os.path.exists(TdxVM.IMA_DATA_FILE):
+            LOG.error("Failed to find IMA binary measurements at %s", TdxVM.IMA_DATA_FILE)
+            return True
+
+        try:
+            with open(TdxVM.IMA_DATA_FILE, "rb") as f:
+                self._runtime_event_log = f.read()
+                if len(self._runtime_event_log) == 0:
+                    LOG.info("Empty IMA measurement found at %s", TdxVM.IMA_DATA_FILE)
+        except (PermissionError, OSError):
+            LOG.error("Need root permission to open file %s", TdxVM.IMA_DATA_FILE)
+
         return True
 
 
-    def get_quote(self, nonce: bytearray, data: bytearray, extraArgs) -> Quote:
-        """Get quote.
+    def get_cc_report(self, nonce: bytearray, data: bytearray, extraArgs) -> CcReport:
+        """Get CcReport (i.e. TD Quote in the context of TDX).
 
         This depends on Quote Generation Service. Please reference "Whitepaper:
         Linux* Stacks for Intel® Trust Domain Extensions (4.3 Attestation)" for
         settings:
         https://www.intel.com/content/www/us/en/content-details/790888/whitepaper-linux-stacks-for-intel-trust-domain-extensions-1-5.html
 
         1. Set up the host: follow 4.3.1 ~ 4.3.4.
@@ -338,59 +392,125 @@
 
         Args:
         nonce (bytearray): against replay attacks.
         data (bytearray): user data
         extraArgs: for TPM, it will be given list of IMR/PCRs
 
         Returns:
-            The ``Quote`` object.
+            The ``CcReport`` object. Return None if it fails.
+
+        Raises:
+            binascii.Error when the parameter "nonce" or "data" is not base64 encoded.
         """
 
         # Prepare user defined data which could include nonce
         if nonce is not None:
-            nonce = base64.b64decode(nonce)
+            nonce = base64.b64decode(nonce, validate=True)
         if data is not None:
-            data = base64.b64decode(data)
+            data = base64.b64decode(data, validate=True)
         report_bytes = None
-        if self.tdreport is not None:
-            LOG.info("Using report data directly to generate quote")
-            report_bytes = self.tdreport.data
-        if report_bytes is None:
-            LOG.error("No existing report data")
-            if nonce is None and data is None:
-                LOG.info("No report data, generating default quote")
-            else:
-                LOG.info("Calculate report data by nonce and user data")
-                hash_algo = hashlib.sha512()
-                if nonce is not None:
-                    hash_algo.update(bytes(nonce))
-                if data is not None:
-                    hash_algo.update(bytes(data))
-                report_bytes = hash_algo.digest()
+        input_data = None
+        if nonce is None and data is None:
+            LOG.info("No report data, generating default quote")
+        else:
+            LOG.info("Calculate report data by nonce and user data")
+            hash_algo = hashlib.sha512()
+            if nonce is not None:
+                hash_algo.update(bytes(nonce))
+            if data is not None:
+                hash_algo.update(bytes(data))
+            input_data = hash_algo.digest()
+        self.process_cc_report(input_data)
+        report_bytes = self.tdreport.data
+
+        if self.version is TDX_VERSION_1_0:
+            quote_req = TdxQuoteReq10()
+        elif self.version is TDX_VERSION_1_5:
+            quote_req = TdxQuoteReq15()
+
+        # Check if appropriate qgs vsock port specified in TDX attest config
+        # If specified, use vsock to get quote and return TdxQuote object
+        td_report = None
+        if self._config and "port" in self._config:
+            LOG.info("Use vsock for TDX quote fetching.")
+            td_report = self._invoke_quote_fetching_on_vsock(
+                report_bytes, quote_req, self._config["port"])
+
+        # Check if quote fetching by vsock has been done successfully
+        # If yes, return result and skip following steps
+        if td_report:
+            return td_report
+
+        # Fetch quote through tdvmcall
+        LOG.info("Use tdvmcall for TDX quote fetching.")
+        # pylint: disable=E1111
+        req_buf = quote_req.prepare_reqbuf(report_bytes)
 
         # Open TDX guest device node
         dev_path = self.DEVICE_NODE_PATH[self.version]
         try:
             tdx_dev = os.open(dev_path, os.O_RDWR)
         except (PermissionError, IOError, OSError) as e:
             LOG.error("Fail to open device node %s: %s", dev_path, str(e))
             return None
         LOG.debug("Successful open device node %s", dev_path)
 
         # Run ioctl command to get TD Quote
-        if self.version is TDX_VERSION_1_0:
-            quote_req = TdxQuoteReq10()
-        elif self.version is TDX_VERSION_1_5:
-            quote_req = TdxQuoteReq15()
-        # pylint: disable=E1111
-        req_buf = quote_req.prepare_reqbuf(report_bytes)
         try:
             fcntl.ioctl(tdx_dev, self.IOCTL_GET_QUOTE[self.version], req_buf)
         except OSError as e:
             LOG.error("Fail to execute ioctl for file %s: %s", dev_path, str(e))
             os.close(tdx_dev)
             return None
         LOG.debug("Successful get Quote from %s.", dev_path)
         os.close(tdx_dev)
 
         # Get TD Quote from ioctl command output
         return quote_req.process_output(req_buf)
+
+    def _invoke_quote_fetching_on_vsock(
+        self,
+        report_bytes:bytes,
+        quote_req:TdxQuoteReq,
+        port:int=None
+        ) -> TdxQuote:
+        """Invoke TDX quote fetching through vsock.
+
+        Args:
+          report_bytes(bytes): report data included in quote request
+          quote_req(TdxQuoteReq): the TDX quote request instance to call QGS
+          port(integer): the port number of QGS vsock
+
+        Returns:
+          A TdxQuote object fetched through vsock
+        """
+        # Setup socket to connect qgs socket on host
+        try:
+            with socket.socket(socket.AF_VSOCK, socket.SOCK_STREAM, 0) as sock:
+                sock.settimeout(30)
+                sock.connect((socket.VMADDR_CID_HOST, port))
+
+                header_size = 4
+                # Generate p_blob_payload buffer
+                qgs_msg = quote_req.qgs_msg_quote_req(report_bytes)
+                msg_size = len(qgs_msg)
+                p_blob_payload = bytearray(msg_size.to_bytes(header_size, "big"))
+                p_blob_payload[header_size:] = qgs_msg[:msg_size]
+
+                # Send quote request
+                nsent = sock.send(p_blob_payload)
+                LOG.debug("Sent %d bytes for Quote request.", nsent)
+
+                # Receive quote response
+                header = sock.recv(header_size)
+                in_msg_size = 0
+                for i in range(header_size):
+                    in_msg_size = (in_msg_size << 8) + (header[i] & 0xFF)
+                qgs_resp = sock.recv(in_msg_size)
+                LOG.debug("Received %d bytes as Quote response", in_msg_size)
+
+                sock.close()
+        except socket.error as msg:
+            LOG.error("Socket Error: %s", msg)
+            return None
+        tdquote = quote_req.qgs_msg_quote_resp(qgs_resp)
+        return TdxQuote(tdquote)
```

### Comparing `cctrusted_vm-0.0.3/cctrusted_vm/sdk.py` & `cctrusted_vm-0.4.0/cctrusted_vm/sdk.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 The VMSDK implementation for ``CCTrusted`` API.
 """
 import logging
 
 # pylint: disable=unused-import
 from cctrusted_base.api import CCTrustedApi
 from cctrusted_base.imr import TcgIMR
-from cctrusted_base.quote import Quote
+from cctrusted_base.ccreport import CcReport
+from cctrusted_base.eventlog import EventLogs
 from cctrusted_base.eventlog import TcgEventLog
 from cctrusted_base.tcg import TcgAlgorithmRegistry
 from cctrusted_vm.cvm import ConfidentialVM
 
 
 LOG = logging.getLogger(__name__)
 
@@ -50,23 +51,23 @@
 
         Different trusted foundation may provide different count of measurement
         register. For example, Intel TDX TDREPORT provides the 4 measurement
         register by default. TPM provides 24 measurement (0~16 for SRTM and 17~24
         for DRTM).
 
         Beyond the real mesurement register, some SDK may extend virtual measurement
-        reigster for addtional trust chain like container, namespace, cluster in
+        reigster for additional trust chain like container, namespace, cluster in
         cloud native paradiagm.
 
         Returns:
             The count of measurement registers
         """
         return len(self._cvm.imrs)
 
-    def get_measurement(self, imr_select:[int, int]) -> TcgIMR:
+    def get_cc_measurement(self, imr_select:[int, int]) -> TcgIMR:
         """Get measurement register according to given selected index and algorithms
 
         Each trusted foundation in CC environment provides the multiple measurement
         registers, the count is update to ``get_measurement_count()``. And for each
         measurement register, it may provides multiple digest for different algorithms.
 
         Args:
@@ -82,43 +83,60 @@
         if imr_index not in self._cvm.imrs:
             LOG.error("Invalid select index for IMR.")
             return None
 
         if algo_id is None or algo_id is TcgAlgorithmRegistry.TPM_ALG_ERROR:
             algo_id = self._cvm.default_algo_id
 
-        return self._cvm.imrs[imr_index].digest(algo_id)
+        # Re-do the processing to fetch the latest measurements
+        self._cvm.process_cc_report()
 
-    def get_quote(self, nonce: bytearray, data: bytearray, extraArgs=None) -> Quote:
-        """Get the quote for given nonce and data.
+        return self._cvm.imrs[imr_index]
 
-        The quote is signing of attestation data (IMR values or hashes of IMR
+    def get_cc_report(
+        self,
+        nonce: bytearray = None,
+        data: bytearray = None,
+        extraArgs = None
+    ) -> CcReport:
+        """Get the CcReport (i.e. quote) for given nonce and data.
+
+        The CcReport is signing of attestation data (IMR values or hashes of IMR
         values), made by a trusted foundation (TPM) using a key trusted by the
         verifier.
 
         Different trusted foundation may use different quote format.
 
         Args:
             nonce (bytearray): against replay attacks.
             data (bytearray): user data
             extraArgs: for TPM, it will be given list of IMR/PCRs
 
         Returns:
-            The ``Quote`` object.
+            The ``CcReport`` object. Return None if it fails.
         """
-        return self._cvm.get_quote(nonce, data, extraArgs)
+        return self._cvm.get_cc_report(nonce, data, extraArgs)
 
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
+            Parsed event logs following TCG Spec.
         """
-        event_logs = TcgEventLog(self._cvm.cc_event_log)
+        # Re-do the processing to fetch the latest event logs
+        self._cvm.process_eventlog()
+
+        event_logs = EventLogs(self._cvm.boot_time_event_log, self._cvm.runtime_event_log,
+                               TcgEventLog.TCG_FORMAT_PCCLIENT)
+
         event_logs.select(start, count)
 
-        return event_logs
+        return event_logs.event_logs
```

### Comparing `cctrusted_vm-0.0.3/cctrusted_vm/tdx.py` & `cctrusted_vm-0.4.0/cctrusted_vm/tdx.py`

 * *Files identical despite different names*

### Comparing `cctrusted_vm-0.0.3/pyproject.toml` & `cctrusted_vm-0.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 [project]
 name = "cctrusted_vm"
-version = "0.0.3"
+version = "0.4.0"
 authors = [
   { name="Lu, Ken", email="ken.lu@intel.com" },
   { name="Zhang, Wenhui", email="wenhui.zhang@bytedance.com" },
 ]
 description = "CC Trusted API VM SDK"
 readme = "README.md"
 license = { text="Apache Software License" }
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: POSIX :: Linux",
 ]
 dependencies = [
+  "cctrusted_base",
+  "pytest",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/cc-api/cc-trusted-api"
 "Bug Tracker" = "https://github.com/cc-api/cc-trusted-api/issues"
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where=["."]
-include=["cctrusted_vm"]
+include=["cctrusted_vm*"]
```

