# Comparing `tmp/dynaddrmgr-0.5.5.tar.gz` & `tmp/dynaddrmgr-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynaddrmgr-0.5.5.tar", max compression
+gzip compressed data, was "dynaddrmgr-0.5.6.tar", max compression
```

## Comparing `dynaddrmgr-0.5.5.tar` & `dynaddrmgr-0.5.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1097 2023-08-03 16:44:32.784008 dynaddrmgr-0.5.5/LICENSE
--rw-r--r--   0        0        0     1606 2023-08-03 16:44:32.784008 dynaddrmgr-0.5.5/README.md
--rw-r--r--   0        0        0       59 2023-11-24 17:55:06.512780 dynaddrmgr-0.5.5/dynaddrmgr/__init__.py
--rw-r--r--   0        0        0     6645 2023-11-24 17:55:06.512780 dynaddrmgr-0.5.5/dynaddrmgr/app.py
--rw-r--r--   0        0        0     3885 2023-08-03 16:44:32.784008 dynaddrmgr-0.5.5/dynaddrmgr/dynhost.py
--rw-r--r--   0        0        0     2401 2023-08-03 16:44:32.784008 dynaddrmgr-0.5.5/dynaddrmgr/dynrules.py
--rw-r--r--   0        0        0     2189 2023-08-03 16:44:32.784008 dynaddrmgr-0.5.5/dynaddrmgr/dyntmpls.py
--rw-r--r--   0        0        0      655 2023-08-03 16:44:32.784008 dynaddrmgr-0.5.5/dynaddrmgr/foos.py
--rw-r--r--   0        0        0     5070 2023-08-03 16:44:32.784008 dynaddrmgr-0.5.5/dynaddrmgr/fwhdlr.py
--rw-r--r--   0        0        0      294 2023-08-03 16:44:32.784008 dynaddrmgr-0.5.5/dynaddrmgr/kinds.py
--rw-r--r--   0        0        0        0 2023-08-03 16:44:32.784008 dynaddrmgr-0.5.5/dynaddrmgr/py.typed
--rw-r--r--   0        0        0     3850 2023-08-03 16:44:32.784008 dynaddrmgr-0.5.5/dynaddrmgr/rule.py
--rw-r--r--   0        0        0     4371 2023-10-09 19:34:29.689162 dynaddrmgr-0.5.5/dynaddrmgr/tmplmgr.py
--rw-r--r--   0        0        0     8661 2023-08-03 16:44:32.784008 dynaddrmgr-0.5.5/dynaddrmgr/ufw.py
--rw-r--r--   0        0        0     1676 2023-11-24 17:55:06.516780 dynaddrmgr-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     2687 1970-01-01 00:00:00.000000 dynaddrmgr-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-01-18 20:13:38.224772 dynaddrmgr-0.5.6/LICENSE
+-rw-r--r--   0        0        0     1606 2023-03-02 18:15:54.777115 dynaddrmgr-0.5.6/README.md
+-rw-r--r--   0        0        0       59 2024-05-11 12:18:21.584811 dynaddrmgr-0.5.6/dynaddrmgr/__init__.py
+-rw-r--r--   0        0        0     6638 2024-05-10 19:50:00.750981 dynaddrmgr-0.5.6/dynaddrmgr/app.py
+-rw-r--r--   0        0        0     4113 2024-05-10 19:24:34.176184 dynaddrmgr-0.5.6/dynaddrmgr/dynhost.py
+-rw-r--r--   0        0        0     2556 2024-05-11 12:06:54.554678 dynaddrmgr-0.5.6/dynaddrmgr/dynrules.py
+-rw-r--r--   0        0        0     2203 2024-04-30 16:39:10.707909 dynaddrmgr-0.5.6/dynaddrmgr/dyntmpls.py
+-rw-r--r--   0        0        0      678 2024-04-30 16:39:10.707909 dynaddrmgr-0.5.6/dynaddrmgr/foos.py
+-rw-r--r--   0        0        0     5071 2024-04-30 16:39:10.707909 dynaddrmgr-0.5.6/dynaddrmgr/fwhdlr.py
+-rw-r--r--   0        0        0      294 2024-05-10 19:49:34.782457 dynaddrmgr-0.5.6/dynaddrmgr/kinds.py
+-rw-r--r--   0        0        0        0 2023-03-02 18:15:54.777115 dynaddrmgr-0.5.6/dynaddrmgr/py.typed
+-rw-r--r--   0        0        0     4028 2024-05-11 11:49:18.960778 dynaddrmgr-0.5.6/dynaddrmgr/rule.py
+-rw-r--r--   0        0        0     4372 2024-04-30 16:39:10.707909 dynaddrmgr-0.5.6/dynaddrmgr/tmplmgr.py
+-rw-r--r--   0        0        0     9637 2024-05-11 11:38:30.875344 dynaddrmgr-0.5.6/dynaddrmgr/ufw.py
+-rw-r--r--   0        0        0     1775 2024-05-11 12:18:21.584811 dynaddrmgr-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     2772 1970-01-01 00:00:00.000000 dynaddrmgr-0.5.6/PKG-INFO
```

### Comparing `dynaddrmgr-0.5.5/LICENSE` & `dynaddrmgr-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dynaddrmgr-0.5.5/README.md` & `dynaddrmgr-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `dynaddrmgr-0.5.5/dynaddrmgr/app.py` & `dynaddrmgr-0.5.6/dynaddrmgr/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 
 Classes:
     DynAddrMgr
 
 Misc variables:
     APPNM
 """
+
 import subprocess  # noqa: S404
 from typing import List, Tuple, Union
 
 from dns.exception import DNSException
 from nslookup import DNSresponse, Nslookup
 from wtforglib.ipaddress_foos import ipv6_to_netprefix, is_ipv6_address
 from wtforglib.kinds import StrAnyDict
 from wtforglib.scribe import Scribe
 
 APPNM = "dynaddrmgr"
 
 
-class FakedProcessResult(object):
+class FakedProcessResult:
     """Faked process result."""
 
     stdout: str
     stderr: str
     returncode: int
 
     def __init__(self, stdout: str = "", stderr: str = "", returncode: int = 0) -> None:
```

### Comparing `dynaddrmgr-0.5.5/dynaddrmgr/dynhost.py` & `dynaddrmgr-0.5.6/dynaddrmgr/dynhost.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,38 +8,42 @@
 from typing import List, Optional, Tuple, Union
 
 from wtforglib.kinds import StrAnyDict
 
 from dynaddrmgr.rule import FwRule
 
 EXAMPLES = """
-#   - name: dynpr.wtforg.net
-#     ipv4: true
-#     ipv6: true
-#     ports:
-#       tcp:
-#         - 22
-#         - 3306
-#         - 33060
-#         - 5432
+  - name: dynpr.wtforg.net
+    ipv4: true
+    ipv6: true
+    ports:
+      tcp:
+        - 22
+        - 3306
+        - 33060
+        - 5432
+      app:
+        - DNS
 """
 PortList = List[int]
+AppList = List[str]
 CfgPortList = List[Union[str, int]]
 
 
-class DynamicHost(object):
+class DynamicHost:
     """DynamicHost is a wrapper for the dynamic host."""
 
     name: str
     ipv4: bool
     ipv6: bool
     ipv6net: int
     _ports_both: PortList
     _ports_tcp: PortList
     _ports_udp: PortList
+    _apps: AppList
     _rules: List[FwRule]
     fw_handler: object
 
     def __init__(self, hinfo: StrAnyDict) -> None:
         """Initialize DynamicHost.
 
         Parameters
@@ -52,16 +56,17 @@
         self.ipv6 = hinfo["ipv6"]
         self.ipv6net = hinfo.get("ipv6net", 0)
         ports = hinfo["ports"]
         self._rules = []
         self._ports_both = self._init_both(ports.get("both"))
         self._ports_tcp = self._init_tcp(ports.get("tcp"))
         self._ports_udp = self._init_udp(ports.get("udp"))
+        self._apps = ports.get("app", [])
 
-    def rules(self, ips: Tuple[str, ...]) -> List[FwRule]:
+    def rules(self, ips: Tuple[str, ...]) -> List[FwRule]:  # noqa: C901,WPS210,WPS231
         """Get rules for dynamic host.
 
         Parameters
         ----------
         ips : Tuple[str, ...]
             List of ipaddress sources
 
@@ -75,14 +80,16 @@
             for ipaddr in ips:
                 for bport in self._ports_both:
                     self._rules.append(FwRule(bport, "", ipaddr, bang_comment))
                 for tport in self._ports_tcp:
                     self._rules.append(FwRule(tport, "tcp", ipaddr, bang_comment))
                 for uport in self._ports_udp:
                     self._rules.append(FwRule(uport, "udp", ipaddr, bang_comment))
+                for app in self._apps:
+                    self._rules.append(FwRule(app, "app", ipaddr, bang_comment))
         return self._rules
 
     def _init_both(self, ports: Optional[CfgPortList]) -> PortList:
         """Initialize both ports list.
 
         Parameters
         ----------
```

### Comparing `dynaddrmgr-0.5.5/dynaddrmgr/dynrules.py` & `dynaddrmgr-0.5.6/dynaddrmgr/dynrules.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 Misc variables:
 
     CONTEXT_SETTINGS
 """
 
 import sys
+import traceback
 import types
 from datetime import datetime
 from typing import AnyStr
 
 import click
 from click.core import Context
 from wtforglib.supers import requires_super_user
@@ -86,25 +87,30 @@
     test: bool,
     noop: bool,
     verbose: bool,
 ) -> int:
     """Main function for dynamic firewall rule manager."""
     if not test:
         requires_super_user("When --no-test  dynaddrmgr")
-    cfg = load_config_file(config, debug)
+    cfg = load_config_file(config, "dynaddrmgr", debug)
     fwtype = cfg.get("firewall_handler", "unspecified").lower()
     try:
         if fwtype == "ufw":
             app = UfwHandler(cfg, debug=debug, noop=noop, test=test, verbose=verbose)
         else:
             raise ValueError("firewall {0} is not supported".format(fwtype))
         rtn_val = app.manage_rules()
     except Exception as ex:
         rtn_val = 1
         print("{0} - {1}".format(datetime.now(), ex), file=sys.stderr)
+        if debug:
+            print("-" * 60)
+            traceback.print_exc(file=sys.stdout)
+            print("-" * 60)
+
     return rtn_val
 
 
 if __name__ == "__main__":  # pragma no cover
     sys.exit(main())
 
 # vim:ft=py noqa: E800
```

### Comparing `dynaddrmgr-0.5.5/dynaddrmgr/dyntmpls.py` & `dynaddrmgr-0.5.6/dynaddrmgr/dyntmpls.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     noop: bool,
     verbose: bool,
 ) -> int:
     """Main function for dynamic template manager."""
     if not test:
         requires_super_user("When --no-test  dynaddrmgr")
     app = TemplateManager(
-        load_config_file(config, debug),
+        load_config_file(config, "dynaddrmgr", debug),
         debug=debug,
         noop=noop,
         test=test,
         verbose=verbose,
     )
     try:
         rtn_val = app.manage_templates()
```

### Comparing `dynaddrmgr-0.5.5/dynaddrmgr/foos.py` & `dynaddrmgr-0.5.6/dynaddrmgr/foos.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 from pathlib import Path
 
 import click
 from wtforglib.files import load_yaml_file
 from wtforglib.kinds import StrAnyDict
 
 
-def load_config_file(config: str, debug: bool) -> StrAnyDict:
+def load_config_file(config: str, base: str, debug: bool) -> StrAnyDict:
     """Load the configuration file."""
     if not config:
-        config_path = Path.home() / ".config" / "dynaddrmgr.yaml"
+        config_path = Path.home() / ".config" / "{0}.yaml".format(base)
         if config_path.is_file():
             config = str(config_path)
         else:
-            config = "/etc/dynaddrmgr.yaml"
+            config = "/etc/{0}.yaml".format(base)
     if debug:
         click.echo("DEBUG: config file => {0}".format(config))
     return load_yaml_file(config, missing_ok=False)
```

### Comparing `dynaddrmgr-0.5.5/dynaddrmgr/fwhdlr.py` & `dynaddrmgr-0.5.6/dynaddrmgr/fwhdlr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Top level module for dynaddrmgr application.
 
 Classes:
     FakedProcessResult
     FirewallHandler
 """
+
 import tempfile
 from logging import Logger
 from pathlib import Path
 from typing import List, NoReturn
 
 from wtforglib.kinds import StrAnyDict
```

### Comparing `dynaddrmgr-0.5.5/dynaddrmgr/rule.py` & `dynaddrmgr-0.5.6/dynaddrmgr/rule.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,55 +16,63 @@
 
 from ipaddress import ip_address, ip_network
 from typing import Optional, Union
 
 from dynaddrmgr.kinds import IPSource
 
 
-class FwRule(object):
+class FwRule:
     """FwRule represents a firewall rule."""
 
     index: int
-    port: int
+    allow: Union[str, int]
     protocol: str
     ipaddr: IPSource
     comment: str
     status: int
 
     def __init__(  # noqa: WPS211
         self,
-        port: Union[str, int],
+        allow: Union[str, int],
         proto: str,
         ipaddr: str,
         comment: str,
         index: str = "-1",
     ) -> None:
         """Initialize FwRule.
 
         Parameters
         ----------
-        port : Union[str, int]
-            Port number
+        allow : Union[str, int]
+            Port number or app
         proto : str
-            Protocal
+            Protocol
         ipaddr : str
             IP address
         comment : str
             comment string
         index : str
             status index number
         """
-        self.port = int(port)
         self.protocol = proto
+        if proto == "app":
+            self.allow = allow
+        else:
+            self.allow = int(allow)
+
         self.ipaddr = self.ip_source(ipaddr)
         if comment.startswith("!!"):
             if proto:
-                comment = "{0}/{1}-{2} (dynaddrmgr)".format(port, proto, comment[2:])
+                comment = "{0}/{1}-{2} (dynaddrmgr)".format(
+                    allow,
+                    proto,
+                    comment[2:],
+                )
             else:
-                comment = "{0}-{1} (dynaddrmgr)".format(port, comment[2:])
+                comment = "{0}-{1} (dynaddrmgr)".format(allow, comment[2:])
         self.comment = comment
         self.index = int(index)
         self.status = 0
 
     def __str__(self) -> str:
         """Returns a string representation of this instance.
 
@@ -72,23 +80,23 @@
         -------
         str
             representation of this instance
         """
         if self.protocol:
             return "[%2s] %5s/%s %-40s # %s [%d]" % (  # noqa: WPS323
                 str(self.index),
-                str(self.port),
+                str(self.allow),
                 self.protocol,
                 str(self.ipaddr),
                 self.comment,
                 self.status,
             )
         return "[%2s] %5s %-45s # %s [%d]" % (  # noqa: WPS323
             str(self.index),
-            str(self.port),
+            str(self.allow),
             str(self.ipaddr),
             self.comment,
             self.status,
         )
 
     def __eq__(self, other: object) -> bool:
         """Compare FwRule objects.
@@ -109,15 +117,15 @@
             True if equal
         """
         if not isinstance(other, FwRule):
             # don't attempt to compare against unrelated types
             raise ValueError("Can only compare FwRule instances.")
         if self.ipaddr != other.ipaddr:
             return False
-        if self.port != other.port:
+        if self.allow != other.allow:
             return False
         if self.protocol != other.protocol:
             return False
         return self.comment == other.comment
 
     def ip_source(self, ipaddr: str) -> IPSource:
         """Convert string representation to IPSource object.
```

### Comparing `dynaddrmgr-0.5.5/dynaddrmgr/tmplmgr.py` & `dynaddrmgr-0.5.6/dynaddrmgr/tmplmgr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Top level module for dynaddrmgr application.
 
 Classes:
     TemplateManager
 """
+
 from typing import Dict, List, Optional, Tuple
 
 from wtforglib.kinds import StrAnyDict
 from wtforglib.options import basic_options
 from wtforglib.tmplwrtr import TemplateWriter
 
 from dynaddrmgr.app import DynAddrMgr
```

### Comparing `dynaddrmgr-0.5.5/dynaddrmgr/ufw.py` & `dynaddrmgr-0.5.6/dynaddrmgr/ufw.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 
 Classes:
     UfwHandler
 
 Misc variables:
     TEST_STATUS
 """
+
 import re
 import tempfile
 from pathlib import Path
 from typing import List, Tuple
 
 from wtforglib.kinds import StrAnyDict
 
+from dynaddrmgr.app import WtfProcessResult
 from dynaddrmgr.fwhdlr import FirewallHandler
 from dynaddrmgr.rule import FwRule
 
 TEST_STATUS = """Status: active
 
      To                         Action      From
      --                         ------      ----
@@ -199,50 +201,96 @@
                     )
         for idx in sorted(indices, key=int, reverse=True):
             cmd_result = self._run_command((UFW, "--force", "delete", str(idx)))
             if cmd_result.returncode != 0:
                 errors += 1
         return errors
 
+    def _run_app_command(self, rule: FwRule) -> WtfProcessResult:
+        """Run app command.
+
+        Parameters
+        ----------
+        rule : FwRule
+            The rule to run
+
+        Returns
+        -------
+        WtfProcessResult
+            The result of the command
+        """
+        return self._run_command(
+            (
+                UFW,
+                "allow",
+                "from",
+                str(rule.ipaddr),
+                "to",
+                "any",
+                "app",
+                str(rule.allow),
+                "comment",
+                rule.comment,
+            ),
+        )
+
+    def _run_port_command(self, rule: FwRule) -> WtfProcessResult:
+        """Run port command.
+
+        Parameters
+        ----------
+        rule : FwRule
+            The rule to run
+
+        Returns
+        -------
+        WtfProcessResult
+            The result of the command
+        """
+        if rule.protocol:
+            return self._run_command(
+                (
+                    UFW,
+                    "allow",
+                    "from",
+                    str(rule.ipaddr),
+                    "to",
+                    "any",
+                    "port",
+                    str(rule.allow),
+                    "proto",
+                    rule.protocol,
+                    "comment",
+                    rule.comment,
+                ),
+            )
+        return self._run_command(
+            (
+                UFW,
+                "allow",
+                "from",
+                str(rule.ipaddr),
+                "to",
+                "any",
+                "port",
+                str(rule.allow),
+                "comment",
+                rule.comment,
+            ),
+        )
+
     def _add_unmatched_rules(self) -> int:
         """Add unmatched rules."""
         errors = 0
         for rule in self.new_rules:
             if rule.status:
                 continue  # skipping matched rules
             if rule.protocol:
                 # ufw allow from 174.24.93.102 to any port 33060 proto tcp
                 # comment '33060/tcp cosprings.teknofile.net'
-                cmd_result = self._run_command(
-                    (
-                        UFW,
-                        "allow",
-                        "from",
-                        str(rule.ipaddr),
-                        "to",
-                        "any",
-                        "port",
-                        str(rule.port),
-                        "proto",
-                        rule.protocol,
-                        "comment",
-                        rule.comment,
-                    ),
-                )
-            else:
-                cmd_result = self._run_command(
-                    (
-                        UFW,
-                        "allow",
-                        "from",
-                        str(rule.ipaddr),
-                        "to",
-                        "any",
-                        "port",
-                        str(rule.port),
-                        "comment",
-                        rule.comment,
-                    ),
-                )
+                if rule.protocol == "app":
+                    cmd_result = self._run_app_command(rule)
+                else:
+                    cmd_result = self._run_port_command(rule)
             if cmd_result.returncode != 0:
                 errors += 1
         return errors
```

### Comparing `dynaddrmgr-0.5.5/pyproject.toml` & `dynaddrmgr-0.5.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "dynaddrmgr"
 description = "Tools to manage actions based on dynamic host address changes."
-version = "0.5.5"
+version = "0.5.6"
 license = "MIT"
 
 authors = [
   "Quien Sabe <qs5779@mail.com>",
 ]
 
 readme = "README.md"
@@ -15,53 +15,58 @@
 keywords = []
 
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Topic :: Software Development :: Libraries :: Python Modules",
+  "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
+  "Typing :: Typed",
 ]
 
 [tool.poetry.scripts]
 dyntmplmgr = "dynaddrmgr.dyntmpls:main"
 dynfwrules = "dynaddrmgr.dynrules:main"
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<4.0"
-click = "^8.1.5"
+python = ">=3.9,<4.0"
+click = "^8.1.0"
 nslookup = "^1.7.0"
-wtforglib = ">= 0.8.3"
+wtforglib = "^0.8"
 jinja2 = "^3.1.2"
 dnspython = "^2.4.2"
 
+[tool.poetry.group.test]
+optional = true
+
 [tool.poetry.group.test.dependencies]
-mypy = "^1.7.0"
-wemake-python-styleguide = "^0.18"
-flake8-pytest-style = "^1.6"
+mypy = "^1.9"
+wemake-python-styleguide = "^0.19"
+flake8-pytest-style = ">=1.6,<3.0"
 doc8 = "^1.0"
-nitpick = ">=0.32,<0.35"
-safety = "^2.3"
-pytest = "^7.3"
-pytest-cov = "^4.0"
+nitpick = "^0.35"
+safety = ">=2.3,<4.0"
+pytest = ">=7.4,<9.0"
+pytest-cov = ">=4,<6"
 pytest-randomly = "^3.12"
-testfixtures = "^7.1.0"
-black = "^23.3.0"
-isort = { version = "<5.12.0", python = "<3.8" }
-requests-cache = ">=0.9,<1.2"
+testfixtures = ">=7.1,<9.0"
+black = ">=23.3,<25.0"
+isort = "^5.13"
+requests-cache = ">=0.9,<1.3"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 sphinx = ">=5.2,<8.0"
-sphinx-autodoc-typehints = "^1.23"
+sphinx-autodoc-typehints = ">=1.23,<3.0"
 m2r2 = "^0.3"
 tomli = "^2.0"
 
 
 [build-system]
 requires = ["poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dynaddrmgr-0.5.5/PKG-INFO` & `dynaddrmgr-0.5.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: dynaddrmgr
-Version: 0.5.5
+Version: 0.5.6
 Summary: Tools to manage actions based on dynamic host address changes.
 Home-page: https://github.com/wtfo-guru/dynaddrmgr
 License: MIT
 Author: Quien Sabe
 Author-email: qs5779@mail.com
-Requires-Python: >=3.8.1,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: click (>=8.1.5,<9.0.0)
+Classifier: Typing :: Typed
+Requires-Dist: click (>=8.1.0,<9.0.0)
 Requires-Dist: dnspython (>=2.4.2,<3.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: nslookup (>=1.7.0,<2.0.0)
-Requires-Dist: wtforglib (>=0.8.3)
+Requires-Dist: wtforglib (>=0.8,<0.9)
 Project-URL: Repository, https://github.com/wtfo-guru/dynaddrmgr
 Description-Content-Type: text/markdown
 
 # dynaddrmgr
 
 [![Build Status](https://github.com/wtfo-guru/dynaddrmgr/actions/workflows/test.yml/badge.svg)](https://github.com/wtfo-guru/dynaddrmgr/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/wtfo-guru/dynaddrmgr/branch/main/graph/badge.svg)](https://codecov.io/gh/wtfo-guru/dynaddrmgr)
```

