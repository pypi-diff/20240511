# Comparing `tmp/nbforager-0.2.1.tar.gz` & `tmp/nbforager-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbforager-0.2.1.tar", max compression
+gzip compressed data, was "nbforager-0.2.2.tar", max compression
```

## Comparing `nbforager-0.2.1.tar` & `nbforager-0.2.2.tar`

### file list

```diff
@@ -1,50 +1,51 @@
--rw-r--r--   0        0        0      398 2024-03-11 16:50:59.007930 nbforager-0.2.1/nbforager/__init__.py
--rw-r--r--   0        0        0      818 2024-01-30 07:34:52.504482 nbforager-0.2.1/nbforager/api/__init__.py
--rw-r--r--   0        0        0    26563 2024-03-29 17:37:40.555725 nbforager-0.2.1/nbforager/api/base_c.py
--rw-r--r--   0        0        0      449 2024-01-30 07:34:52.676932 nbforager-0.2.1/nbforager/api/base_ca.py
--rw-r--r--   0        0        0     1352 2024-01-30 07:34:52.683321 nbforager-0.2.1/nbforager/api/circuits.py
--rw-r--r--   0        0        0     5579 2024-01-30 07:41:55.226009 nbforager-0.2.1/nbforager/api/connector.py
--rw-r--r--   0        0        0      660 2024-01-30 07:34:52.803054 nbforager-0.2.1/nbforager/api/core.py
--rw-r--r--   0        0        0     7520 2024-01-30 07:34:52.378187 nbforager-0.2.1/nbforager/api/dcim.py
--rw-r--r--   0        0        0     5619 2024-01-30 07:34:52.760329 nbforager-0.2.1/nbforager/api/extended_get.py
--rw-r--r--   0        0        0     2930 2024-01-30 07:34:52.631714 nbforager-0.2.1/nbforager/api/extras.py
--rw-r--r--   0        0        0     5331 2024-01-30 07:34:52.738848 nbforager-0.2.1/nbforager/api/ip_addresses.py
--rw-r--r--   0        0        0     2921 2024-01-30 07:34:52.484280 nbforager-0.2.1/nbforager/api/ipam.py
--rw-r--r--   0        0        0      597 2024-01-30 07:34:52.246797 nbforager-0.2.1/nbforager/api/plugins_ca.py
--rw-r--r--   0        0        0      385 2024-01-30 07:34:52.146738 nbforager-0.2.1/nbforager/api/status.py
--rw-r--r--   0        0        0     1242 2024-01-30 07:34:52.724960 nbforager-0.2.1/nbforager/api/tenancy.py
--rw-r--r--   0        0        0     1117 2024-01-30 07:34:52.272019 nbforager-0.2.1/nbforager/api/users.py
--rw-r--r--   0        0        0     1289 2024-01-30 07:34:52.457666 nbforager-0.2.1/nbforager/api/virtualization.py
--rw-r--r--   0        0        0      782 2024-01-30 07:34:52.174355 nbforager-0.2.1/nbforager/api/wireless.py
--rw-r--r--   0        0        0      175 2024-03-11 16:50:59.013928 nbforager-0.2.1/nbforager/exceptions.py
--rw-r--r--   0        0        0       17 2023-12-17 11:33:45.934677 nbforager-0.2.1/nbforager/foragers/__init__.py
--rw-r--r--   0        0        0     1681 2024-03-11 16:50:59.016976 nbforager-0.2.1/nbforager/foragers/base_fa.py
--rw-r--r--   0        0        0     1493 2024-03-11 16:50:59.018978 nbforager-0.2.1/nbforager/foragers/circuits.py
--rw-r--r--   0        0        0     1032 2024-03-11 16:50:59.021977 nbforager-0.2.1/nbforager/foragers/core.py
--rw-r--r--   0        0        0     5942 2024-03-11 16:50:59.026980 nbforager-0.2.1/nbforager/foragers/dcim.py
--rw-r--r--   0        0        0     2664 2024-03-11 16:50:59.028981 nbforager-0.2.1/nbforager/foragers/extras.py
--rw-r--r--   0        0        0    13627 2024-03-29 13:34:02.623673 nbforager-0.2.1/nbforager/foragers/forager.py
--rw-r--r--   0        0        0     2707 2024-03-11 16:50:59.036975 nbforager-0.2.1/nbforager/foragers/ipam.py
--rw-r--r--   0        0        0      540 2023-12-02 15:48:47.753539 nbforager-0.2.1/nbforager/foragers/ipv4.py
--rw-r--r--   0        0        0     9992 2024-03-29 17:37:40.557728 nbforager-0.2.1/nbforager/foragers/joiner.py
--rw-r--r--   0        0        0     1506 2024-03-11 16:50:59.039978 nbforager-0.2.1/nbforager/foragers/tenancy.py
--rw-r--r--   0        0        0     1211 2024-03-11 16:50:59.042978 nbforager-0.2.1/nbforager/foragers/users.py
--rw-r--r--   0        0        0     1362 2024-03-11 16:50:59.045974 nbforager-0.2.1/nbforager/foragers/virtualization.py
--rw-r--r--   0        0        0     1122 2024-03-11 16:50:59.048977 nbforager-0.2.1/nbforager/foragers/wireless.py
--rw-r--r--   0        0        0    15087 2024-03-29 16:13:06.030840 nbforager-0.2.1/nbforager/helpers.py
--rw-r--r--   0        0        0      844 2023-11-17 09:14:13.531979 nbforager-0.2.1/nbforager/log.py
--rw-r--r--   0        0        0     4021 2023-10-28 18:13:26.862376 nbforager-0.2.1/nbforager/messages.py
--rw-r--r--   0        0        0     7220 2024-03-11 16:50:59.051976 nbforager-0.2.1/nbforager/nb_api.py
--rw-r--r--   0        0        0     4617 2024-03-29 17:37:40.561725 nbforager-0.2.1/nbforager/nb_cache.py
--rw-r--r--   0        0        0    16072 2024-03-29 17:37:40.564733 nbforager-0.2.1/nbforager/nb_forager.py
--rw-r--r--   0        0        0    11431 2024-03-29 17:37:40.567728 nbforager-0.2.1/nbforager/nb_tree.py
--rw-r--r--   0        0        0       15 2024-03-11 16:50:59.058023 nbforager-0.2.1/nbforager/parser/__init__.py
--rw-r--r--   0        0        0     5203 2024-03-11 16:52:28.983714 nbforager-0.2.1/nbforager/parser/nb_custom.py
--rw-r--r--   0        0        0     9849 2024-03-11 16:50:59.063027 nbforager-0.2.1/nbforager/parser/nb_parser.py
--rw-r--r--   0        0        0    27853 2024-03-29 17:37:40.570728 nbforager-0.2.1/nbforager/parser/nb_value.py
--rw-r--r--   0        0        0        0 2022-11-06 21:30:57.837000 nbforager-0.2.1/nbforager/py.typed
--rw-r--r--   0        0        0     9611 2024-03-11 16:50:59.068025 nbforager-0.2.1/nbforager/py_tree.py
--rw-r--r--   0        0        0     1750 2024-03-11 16:50:59.070023 nbforager-0.2.1/nbforager/types_.py
--rw-r--r--   0        0        0     3052 2024-03-29 17:37:40.573728 nbforager-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     7302 2024-03-11 16:50:58.968890 nbforager-0.2.1/README.rst
--rw-r--r--   0        0        0     8684 1970-01-01 00:00:00.000000 nbforager-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     9796 2023-10-28 18:13:26.831908 nbforager-0.2.2/LICENCE.txt
+-rw-r--r--   0        0        0      398 2024-03-11 16:50:59.007930 nbforager-0.2.2/nbforager/__init__.py
+-rw-r--r--   0        0        0      818 2024-01-30 07:34:52.504482 nbforager-0.2.2/nbforager/api/__init__.py
+-rw-r--r--   0        0        0    26757 2024-05-11 10:29:18.349446 nbforager-0.2.2/nbforager/api/base_c.py
+-rw-r--r--   0        0        0      449 2024-01-30 07:34:52.676932 nbforager-0.2.2/nbforager/api/base_ca.py
+-rw-r--r--   0        0        0     1352 2024-01-30 07:34:52.683321 nbforager-0.2.2/nbforager/api/circuits.py
+-rw-r--r--   0        0        0     5579 2024-01-30 07:41:55.226009 nbforager-0.2.2/nbforager/api/connector.py
+-rw-r--r--   0        0        0      660 2024-01-30 07:34:52.803054 nbforager-0.2.2/nbforager/api/core.py
+-rw-r--r--   0        0        0     7520 2024-01-30 07:34:52.378187 nbforager-0.2.2/nbforager/api/dcim.py
+-rw-r--r--   0        0        0     5619 2024-01-30 07:34:52.760329 nbforager-0.2.2/nbforager/api/extended_get.py
+-rw-r--r--   0        0        0     2930 2024-01-30 07:34:52.631714 nbforager-0.2.2/nbforager/api/extras.py
+-rw-r--r--   0        0        0     5331 2024-01-30 07:34:52.738848 nbforager-0.2.2/nbforager/api/ip_addresses.py
+-rw-r--r--   0        0        0     2921 2024-01-30 07:34:52.484280 nbforager-0.2.2/nbforager/api/ipam.py
+-rw-r--r--   0        0        0      597 2024-01-30 07:34:52.246797 nbforager-0.2.2/nbforager/api/plugins_ca.py
+-rw-r--r--   0        0        0      385 2024-01-30 07:34:52.146738 nbforager-0.2.2/nbforager/api/status.py
+-rw-r--r--   0        0        0     1242 2024-01-30 07:34:52.724960 nbforager-0.2.2/nbforager/api/tenancy.py
+-rw-r--r--   0        0        0     1117 2024-01-30 07:34:52.272019 nbforager-0.2.2/nbforager/api/users.py
+-rw-r--r--   0        0        0     1289 2024-01-30 07:34:52.457666 nbforager-0.2.2/nbforager/api/virtualization.py
+-rw-r--r--   0        0        0      782 2024-01-30 07:34:52.174355 nbforager-0.2.2/nbforager/api/wireless.py
+-rw-r--r--   0        0        0      175 2024-03-11 16:50:59.013928 nbforager-0.2.2/nbforager/exceptions.py
+-rw-r--r--   0        0        0       17 2023-12-17 11:33:45.934677 nbforager-0.2.2/nbforager/foragers/__init__.py
+-rw-r--r--   0        0        0     1681 2024-03-11 16:50:59.016976 nbforager-0.2.2/nbforager/foragers/base_fa.py
+-rw-r--r--   0        0        0     1493 2024-03-11 16:50:59.018978 nbforager-0.2.2/nbforager/foragers/circuits.py
+-rw-r--r--   0        0        0     1032 2024-03-11 16:50:59.021977 nbforager-0.2.2/nbforager/foragers/core.py
+-rw-r--r--   0        0        0     5942 2024-03-11 16:50:59.026980 nbforager-0.2.2/nbforager/foragers/dcim.py
+-rw-r--r--   0        0        0     2664 2024-03-11 16:50:59.028981 nbforager-0.2.2/nbforager/foragers/extras.py
+-rw-r--r--   0        0        0    13627 2024-03-29 13:34:02.623673 nbforager-0.2.2/nbforager/foragers/forager.py
+-rw-r--r--   0        0        0     2707 2024-03-11 16:50:59.036975 nbforager-0.2.2/nbforager/foragers/ipam.py
+-rw-r--r--   0        0        0      540 2023-12-02 15:48:47.753539 nbforager-0.2.2/nbforager/foragers/ipv4.py
+-rw-r--r--   0        0        0    12163 2024-05-11 12:55:22.629082 nbforager-0.2.2/nbforager/foragers/joiner.py
+-rw-r--r--   0        0        0     1506 2024-03-11 16:50:59.039978 nbforager-0.2.2/nbforager/foragers/tenancy.py
+-rw-r--r--   0        0        0     1211 2024-03-11 16:50:59.042978 nbforager-0.2.2/nbforager/foragers/users.py
+-rw-r--r--   0        0        0     1362 2024-03-11 16:50:59.045974 nbforager-0.2.2/nbforager/foragers/virtualization.py
+-rw-r--r--   0        0        0     1122 2024-03-11 16:50:59.048977 nbforager-0.2.2/nbforager/foragers/wireless.py
+-rw-r--r--   0        0        0    15087 2024-03-29 16:13:06.030840 nbforager-0.2.2/nbforager/helpers.py
+-rw-r--r--   0        0        0      844 2023-11-17 09:14:13.531979 nbforager-0.2.2/nbforager/log.py
+-rw-r--r--   0        0        0     4021 2023-10-28 18:13:26.862376 nbforager-0.2.2/nbforager/messages.py
+-rw-r--r--   0        0        0     7220 2024-03-11 16:50:59.051976 nbforager-0.2.2/nbforager/nb_api.py
+-rw-r--r--   0        0        0     4617 2024-03-29 17:37:40.561725 nbforager-0.2.2/nbforager/nb_cache.py
+-rw-r--r--   0        0        0    16330 2024-05-11 13:02:21.175179 nbforager-0.2.2/nbforager/nb_forager.py
+-rw-r--r--   0        0        0    11215 2024-05-11 12:23:19.621221 nbforager-0.2.2/nbforager/nb_tree.py
+-rw-r--r--   0        0        0       15 2024-03-11 16:50:59.058023 nbforager-0.2.2/nbforager/parser/__init__.py
+-rw-r--r--   0        0        0     5203 2024-03-11 16:52:28.983714 nbforager-0.2.2/nbforager/parser/nb_custom.py
+-rw-r--r--   0        0        0     9849 2024-03-11 16:50:59.063027 nbforager-0.2.2/nbforager/parser/nb_parser.py
+-rw-r--r--   0        0        0    27853 2024-03-29 17:37:40.570728 nbforager-0.2.2/nbforager/parser/nb_value.py
+-rw-r--r--   0        0        0        0 2022-11-06 21:30:57.837000 nbforager-0.2.2/nbforager/py.typed
+-rw-r--r--   0        0        0     9611 2024-03-11 16:50:59.068025 nbforager-0.2.2/nbforager/py_tree.py
+-rw-r--r--   0        0        0     1750 2024-03-11 16:50:59.070023 nbforager-0.2.2/nbforager/types_.py
+-rw-r--r--   0        0        0     3070 2024-05-11 09:32:37.108320 nbforager-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     7302 2024-03-11 16:50:58.968890 nbforager-0.2.2/README.rst
+-rw-r--r--   0        0        0     8735 1970-01-01 00:00:00.000000 nbforager-0.2.2/PKG-INFO
```

### Comparing `nbforager-0.2.1/nbforager/api/__init__.py` & `nbforager-0.2.2/nbforager/api/__init__.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/api/base_c.py` & `nbforager-0.2.2/nbforager/api/base_c.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         "slug",
         "display",
         "prefix",
         "address",
         "cid",
         "vid",
         "asn",
+        "device_id",
     ]
     _init_params = [
         "host",
         "token",
         "scheme",
         "port",
         "verify",
@@ -68,39 +69,45 @@
         "sleep",
         "default_get",
         "loners",
     ]
     _reserved_keys: DLStr = {
         "ipam/": [
             # ipam aggregates, prefixes, ip_addresses
-            "ipv4",
-            "aggregate",
-            "super_prefix",
-            "sub_prefixes",
-            "ip_addresses",
+            "_ipv4",
+            "_aggregate",
+            "_super_prefix",
+            "_sub_prefixes",
+            "_ip_addresses",
             # evonetbox
             "overlapped",
             "warnings",
             "nbnets",
             "nbnets__subnets",
         ],
         "dcim/devices/": [
-            "interfaces",
-            "front_ports",
-            "rear_ports",
-            "console_ports",
-            "console_server_ports",
-            "power_ports",
-            "power_outlets",
-            "module_bays",
-            "device_bays",
-            "inventory_items",
+            "_interfaces",
+            "_front_ports",
+            "_rear_ports",
+            "_console_ports",
+            "_console_server_ports",
+            "_power_ports",
+            "_power_outlets",
+            "_module_bays",
+            "_device_bays",
+            "_inventory_items",
+        ],
+        "dcim/interfaces/": [
+            "_ip_addresses",
         ],
         "virtualization/virtual-machines/": [
-            "interfaces",
+            "_interfaces",
+        ],
+        "virtualization/interfaces/": [
+            "_ip_addresses",
         ],
     }
 
     def __init__(self, **kwargs):
         """Init BaseC.
 
         :param str host: Netbox host name.
```

### Comparing `nbforager-0.2.1/nbforager/api/circuits.py` & `nbforager-0.2.2/nbforager/api/circuits.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/api/connector.py` & `nbforager-0.2.2/nbforager/api/connector.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/api/core.py` & `nbforager-0.2.2/nbforager/api/core.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/api/dcim.py` & `nbforager-0.2.2/nbforager/api/dcim.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/api/extended_get.py` & `nbforager-0.2.2/nbforager/api/extended_get.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/api/extras.py` & `nbforager-0.2.2/nbforager/api/extras.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/api/ip_addresses.py` & `nbforager-0.2.2/nbforager/api/ip_addresses.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/api/ipam.py` & `nbforager-0.2.2/nbforager/api/ipam.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/api/plugins_ca.py` & `nbforager-0.2.2/nbforager/api/plugins_ca.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/api/tenancy.py` & `nbforager-0.2.2/nbforager/api/tenancy.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/api/users.py` & `nbforager-0.2.2/nbforager/api/users.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/api/virtualization.py` & `nbforager-0.2.2/nbforager/api/virtualization.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/api/wireless.py` & `nbforager-0.2.2/nbforager/api/wireless.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/foragers/base_fa.py` & `nbforager-0.2.2/nbforager/foragers/base_fa.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/foragers/circuits.py` & `nbforager-0.2.2/nbforager/foragers/circuits.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/foragers/core.py` & `nbforager-0.2.2/nbforager/foragers/core.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/foragers/dcim.py` & `nbforager-0.2.2/nbforager/foragers/dcim.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/foragers/extras.py` & `nbforager-0.2.2/nbforager/foragers/extras.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/foragers/forager.py` & `nbforager-0.2.2/nbforager/foragers/forager.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/foragers/ipam.py` & `nbforager-0.2.2/nbforager/foragers/ipam.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/foragers/ipv4.py` & `nbforager-0.2.2/nbforager/foragers/ipv4.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/foragers/joiner.py` & `nbforager-0.2.2/nbforager/foragers/joiner.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,215 +19,269 @@
 
     def __init__(self, tree: NbTree):
         """Init Joiner.
         :param NbTree tree: Contains Netbox that need to be updated similar to the WEB UI.
         """
         self.tree = tree
 
+    # noinspection PyProtectedMember
+    def init_extra_keys(self) -> None:
+        """Init extra keys to represent Netbox objects similar to the WEB UI.
+
+        :return: None. Update NbTree object.
+        """
+        for app, model in [
+            ("dcim", "devices"),
+            ("dcim", "interfaces"),
+            ("virtualization", "virtual_machines"),
+            ("virtualization", "interfaces"),
+        ]:
+            key = f"{app}/{model}/".replace("_", "-")
+            reserved_keys: LStr = BaseC._reserved_keys[key]  # pylint: disable=W0212
+            objects_d: DiDAny = getattr(getattr(self.tree, app), model)
+            for object_d in objects_d.values():
+                for _key in reserved_keys:
+                    object_d[_key] = {}
+
+        for model, key, strict in [
+            ("aggregates", "prefix", True),
+            ("prefixes", "prefix", True),
+            ("ip_addresses", "address", False),
+        ]:
+            objects: DiDAny = getattr(self.tree.ipam, model)
+            for data in objects.values():
+                nbv = NbValue(data=data)
+                family: int = nbv.family_value()
+                if family != 4:
+                    continue
+                snet = data[key]
+                data["_ipv4"] = IPv4(snet, strict=strict)
+                data["_aggregate"] = {}  # DAny
+                data["_super_prefix"] = {}  # DAny
+                data["_sub_prefixes"] = []  # LDAny
+                data["_ip_addresses"] = []  # LDAny
+
     def join_dcim_devices(self) -> None:
         """Create additional keys to represent dcim.devices similar to the WEB UI.
 
             In dcim.devices:
 
-            - ``console_ports``
-            - ``console_server_ports``
-            - ``device_bays``
-            - ``front_ports``
-            - ``interfaces``
-            - ``inventory_items``
-            - ``module_bays``
-            - ``power_outlets``
-            - ``power_ports``
-            - ``rear_ports``
+            - ``_console_ports``
+            - ``_console_server_ports``
+            - ``_device_bays``
+            - ``_front_ports``
+            - ``_interfaces``
+            - ``_inventory_items``
+            - ``_module_bays``
+            - ``_power_outlets``
+            - ``_power_ports``
+            - ``_rear_ports``
+
+            In dcim.interfaces:
+
+            - ``_ip_addresses``
 
         :return: None. Update NbTree object.
         """
-        self._join_devices(app="dcim")
+        self._join_dcim_devices(app="dcim")
+        self._join_dcim_interfaces(app="dcim")
 
     def join_virtualization_virtual_machines(self) -> None:
         """Create additional keys to represent virtualization.virtual_machines.
 
-        Add interfaces in virtualization.virtual_machines.
+            In virtualization.virtual_machines:
+
+            - ``_interfaces``
+
+            In virtualization.interfaces:
+
+            - ``_ip_addresses``
 
         :return: None. Update NbTree object.
         """
-        self._join_devices(app="virtualization")
+        self._join_dcim_devices(app="virtualization")
+        self._join_dcim_interfaces(app="virtualization")
 
     # noinspection PyProtectedMember
-    def _join_devices(self, app: str) -> None:
+    def _join_dcim_devices(self, app: str) -> None:
         """Create additional keys to represent devices/VM similar to the WEB UI.
 
         :param app: Application name: "dcim", "virtualization"
 
         :return: None. Update NbTree object.
         """
         model = "devices"
         key = "dcim/devices/"
         if app == "virtualization":
             model = "virtual_machines"
             key = "virtualization/virtual-machines/"
-        models: LStr = BaseC._reserved_keys[key]  # pylint: disable=W0212
-
-        # init extra keys
+        reserved_keys: LStr = BaseC._reserved_keys[key]  # pylint: disable=W0212
         devices_d: DiDAny = getattr(getattr(self.tree, app), model)
-        for device in devices_d.values():
-            for model in models:
-                device[model] = {}
 
-        # set extra values
+        # set values
         key = "device"
         if app == "virtualization":
             key = "virtual_machine"
 
+        models = [s.lstrip("_") for s in reserved_keys]
         for model in models:
             ports_d: DiDAny = getattr(getattr(self.tree, app), model)
             ports: LDAny = list(ports_d.values())
 
             # sort by interface idx
             ports_lt = [(Intf(d["name"]), d) for d in ports]
             ports_lt.sort(key=itemgetter(0))
             ports = [dict(t[1]) for t in ports_lt]
 
-            for port in ports:
-                name = port["name"]
-                id_ = port[key]["id"]
-                device_: DAny = devices_d.get(id_, {})  # pylint: disable=E1101
-                if model in device_:
-                    device_[model][name] = port
+            for port_d in ports:
+                name = port_d["name"]
+                id_ = port_d[key]["id"]
+                device_d: DAny = devices_d.get(id_, {})  # pylint: disable=E1101
+                _key = f"_{model}"
+                if _key in device_d:
+                    device_d[_key][name] = port_d
+
+    def _join_dcim_interfaces(self, app: str) -> None:
+        """Create additional keys to represent dcim/interfaces with assigned ipam/ip-addresses.
+
+        :param app: Application name: "dcim", "virtualization"
+
+        :return: None. Update NbTree object.
+        """
+        model = "interfaces"
+        object_type = "virtualization.vminterface" if app == "virtualization" else "dcim.interface"
+        interfaces_d: DiDAny = getattr(getattr(self.tree, app), model)
+
+        app = "ipam"
+        model = "ip_addresses"
+        _key = f"_{model}"
+        addresses_d: DiDAny = getattr(getattr(self.tree, app), model)
+        addresses: LDAny = list(addresses_d.values())
+        addresses.sort(key=itemgetter("address"))
+
+        for address_d in addresses:
+            address = address_d["address"]
+            assigned_object_id = address_d["assigned_object_id"]
+            if not assigned_object_id:
+                continue
+            if address_d["assigned_object_type"] != object_type:
+                continue
+            interface_d: DAny = interfaces_d.get(assigned_object_id, {})  # pylint: disable=E1101
+            if _key in interface_d:
+                interface_d[_key][address] = address_d
 
     def join_ipam_ipv4(self) -> None:
         """Create additional keys to represent ipam similar to the WEB UI.
 
             Add new attributes in ipam.aggregate, ipam.prefixes, ipam.ip_addresses:
 
-            - ``ipv4`` IPv4 object, child of ciscoconfparse.IPv4Obj
-            - ``aggregate`` Aggregate data for ipam.prefixes and ipam.ip_addresses
-            - ``super_prefix`` Related parent prefix data for ipam.prefixes and ipam.ip_addresses
-            - ``sub_prefixes`` Related child prefixes data for ipam.prefixes and ipam.ip_addresses
-            - ``ip_addresses`` Related IP addresses data for ipam.aggregates and ipam.prefixes
+            - ``_ipv4`` IPv4 object, child of ciscoconfparse.IPv4Obj
+            - ``_aggregate`` Aggregate data for ipam.prefixes and ipam.ip_addresses
+            - ``_super_prefix`` Related parent prefix data for ipam.prefixes and ipam.ip_addresses
+            - ``_sub_prefixes`` Related child prefixes data for ipam.prefixes and ipam.ip_addresses
+            - ``_ip_addresses`` Related IP addresses data for ipam.aggregates and ipam.prefixes
 
         :return: None. Update NbTree object.
         """
-        self._init_ipam_keys()
         self._join_ipam_aggregates()
         self._join_ipam_prefixes()
         self._join_ipam_ip_addresses()
         self._join_update_sub_prefixes()
 
-    def _init_ipam_keys(self) -> None:
-        """Init extra keys that are required for aggregates, prefixes, ip_addresses."""
-        for model, key, strict in [
-            ("aggregates", "prefix", True),
-            ("prefixes", "prefix", True),
-            ("ip_addresses", "address", False),
-        ]:
-            objects: DiDAny = getattr(self.tree.ipam, model)
-            for data in objects.values():
-                nbv = NbValue(data=data)
-                family: int = nbv.family_value()
-                if family != 4:
-                    continue
-                snet = data[key]
-                data["ipv4"] = IPv4(snet, strict=strict)
-                data["aggregate"] = {}  # DAny
-                data["super_prefix"] = {}  # DAny
-                data["sub_prefixes"] = []  # LDAny
-                data["ip_addresses"] = []  # LDAny
-
     def _join_ipam_aggregates(self) -> None:
-        """Add prefixes to tree.ipam.aggregates.sub_prefixes."""
+        """Add prefixes to tree.ipam.aggregates._sub_prefixes."""
         aggregates: LDAny = self._get_aggregates_ip4()
         prefixes_d: DiLDAny = self._get_prefixes_ip4_d()
         for aggregate in aggregates:
             for depth, prefixes in prefixes_d.items():
                 for prefix in prefixes:
                     _aggregate = aggregate["prefix"]
                     _prefix = prefix["prefix"]
-                    if prefix["ipv4"] in aggregate["ipv4"]:
-                        prefix["aggregate"] = aggregate
+                    if prefix["_ipv4"] in aggregate["_ipv4"]:
+                        prefix["_aggregate"] = aggregate
                         if depth == 0:
-                            aggregate["sub_prefixes"].append(prefix)
+                            aggregate["_sub_prefixes"].append(prefix)
 
     def _join_ipam_ip_addresses(self) -> None:
-        """Add prefixes to tree.ipam.ip-addresses.super_prefix."""
+        """Add prefixes to tree.ipam.ip-addresses._super_prefix."""
         ip_addresses: LDAny = self._get_ip_addresses_ip4()
         prefixes_d: DiLDAny = self._get_prefixes_ip4_d()
         depths: LInt = list(prefixes_d)
         depths.reverse()
 
         added_addresses: LDAny = []
         for depth in depths:
             ip_addresses_ = ip_addresses.copy()
             prefixes: LDAny = prefixes_d.get(depth, [])
             for ip_address in ip_addresses_:
                 for prefix in prefixes:
-                    if ip_address["ipv4"] not in prefix["ipv4"]:
+                    if ip_address["_ipv4"] not in prefix["_ipv4"]:
                         continue
                     if ip_address in added_addresses:
                         continue
-                    ip_address["aggregate"] = prefix["aggregate"]
-                    ip_address["super_prefix"] = prefix
-                    prefix["ip_addresses"].append(ip_address)
+                    ip_address["_aggregate"] = prefix["_aggregate"]
+                    ip_address["_super_prefix"] = prefix
+                    prefix["_ip_addresses"].append(ip_address)
                     added_addresses.append(ip_address)
             ip_addresses = [d for d in ip_addresses if d not in added_addresses]
 
     def _join_ipam_prefixes(self) -> None:
-        """Add prefixes to tree.ipam.prefixes.sub_prefixes, super_prefix"""
+        """Add prefixes to tree.ipam.prefixes._sub_prefixes, _super_prefix"""
         super_prefixes = []
         prefixes_d: DiLDAny = self._get_prefixes_ip4_d()
         for depth, sub_prefixes in enumerate(prefixes_d.values()):
             if not depth:
                 super_prefixes = sub_prefixes
                 continue
             for super_prefix in super_prefixes:
-                if super_prefix["ipv4"].prefixlen == 32:
+                if super_prefix["_ipv4"].prefixlen == 32:
                     continue
                 for sub_prefix in sub_prefixes:
-                    if sub_prefix["ipv4"] in (super_prefix["ipv4"]):
-                        super_prefix["sub_prefixes"].append(sub_prefix)
-                        sub_prefix["super_prefix"] = super_prefix
+                    if sub_prefix["_ipv4"] in (super_prefix["_ipv4"]):
+                        super_prefix["_sub_prefixes"].append(sub_prefix)
+                        sub_prefix["_super_prefix"] = super_prefix
             super_prefixes = sub_prefixes
 
     def _join_update_sub_prefixes(self) -> None:
-        """Update sub_prefixes in ipam.aggregates and ipam.prefixes.
+        """Update _sub_prefixes in ipam.aggregates and ipam.prefixes.
 
         Remove duplicates, remove objects with improper depth, sort by IPv4.
         """
         aggregates = self._get_aggregates_ip4()
         for aggregate in aggregates:
-            sub_prefixes = vlist.no_dupl(aggregate["sub_prefixes"])
-            sub_prefixes = [d for d in sub_prefixes if not d["super_prefix"]]
-            aggregate["sub_prefixes"] = sorted(sub_prefixes, key=itemgetter("ipv4"))
+            sub_prefixes = vlist.no_dupl(aggregate["_sub_prefixes"])
+            sub_prefixes = [d for d in sub_prefixes if not d["_super_prefix"]]
+            aggregate["_sub_prefixes"] = sorted(sub_prefixes, key=itemgetter("_ipv4"))
 
         prefixes = self._get_prefixes_ip4()
         for prefix in prefixes:
-            sub_prefixes = vlist.no_dupl(prefix["sub_prefixes"])
-            prefix["sub_prefixes"] = sorted(sub_prefixes, key=itemgetter("ipv4"))
-            ip_addresses = vlist.no_dupl(prefix["ip_addresses"])
-            prefix["ip_addresses"] = sorted(ip_addresses, key=itemgetter("ipv4"))
+            sub_prefixes = vlist.no_dupl(prefix["_sub_prefixes"])
+            prefix["_sub_prefixes"] = sorted(sub_prefixes, key=itemgetter("_ipv4"))
+            ip_addresses = vlist.no_dupl(prefix["_ip_addresses"])
+            prefix["_ip_addresses"] = sorted(ip_addresses, key=itemgetter("_ipv4"))
 
     # ============================= helpers ==============================
 
     def _get_aggregates_ip4(self) -> LDAny:
         """Return ipam.aggregates family=4 sorted by IPv4."""
         aggregates: LDAny = list(self.tree.ipam.aggregates.values())
         aggregates = [d for d in aggregates if d["family"]["value"] == 4]
-        return sorted(aggregates, key=itemgetter("ipv4"))
+        return sorted(aggregates, key=itemgetter("_ipv4"))
 
     def _get_ip_addresses_ip4(self) -> LDAny:
         """Return ipam.ip_addresses family=4 sorted by IPv4."""
         ip_addresses: LDAny = list(self.tree.ipam.ip_addresses.values())
         ip_addresses = [d for d in ip_addresses if d["family"]["value"] == 4 and d["vrf"] is None]
-        return sorted(ip_addresses, key=itemgetter("ipv4"))
+        return sorted(ip_addresses, key=itemgetter("_ipv4"))
 
     def _get_prefixes_ip4(self) -> LDAny:
         """Return ipam.prefixes family=4 sorted by IPv4."""
         prefixes: LDAny = list(self.tree.ipam.prefixes.values())
         prefixes = [d for d in prefixes if d["family"]["value"] == 4 and d["vrf"] is None]
-        return sorted(prefixes, key=itemgetter("ipv4"))
+        return sorted(prefixes, key=itemgetter("_ipv4"))
 
     def _get_prefixes_ip4_d(self) -> DiLDAny:
         """Split prefixes by depth.
 
         :return: A dictionary of prefixes where the key represents the depth
             and the value represents a list of prefixes at that depth.
         """
```

### Comparing `nbforager-0.2.1/nbforager/foragers/tenancy.py` & `nbforager-0.2.2/nbforager/foragers/tenancy.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/foragers/users.py` & `nbforager-0.2.2/nbforager/foragers/users.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/foragers/virtualization.py` & `nbforager-0.2.2/nbforager/foragers/virtualization.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/foragers/wireless.py` & `nbforager-0.2.2/nbforager/foragers/wireless.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/helpers.py` & `nbforager-0.2.2/nbforager/helpers.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/log.py` & `nbforager-0.2.2/nbforager/log.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/messages.py` & `nbforager-0.2.2/nbforager/messages.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/nb_api.py` & `nbforager-0.2.2/nbforager/nb_api.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/nb_cache.py` & `nbforager-0.2.2/nbforager/nb_cache.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/nb_forager.py` & `nbforager-0.2.2/nbforager/nb_forager.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import logging
 from datetime import datetime
 from pathlib import Path
 
 import pynetbox
 from pynetbox.core.endpoint import Endpoint
 from vhelpers import vstr
+from copy import deepcopy
 
 from nbforager import nb_tree
 from nbforager.foragers.circuits import CircuitsAF
 from nbforager.foragers.core import CoreAF
 from nbforager.foragers.dcim import DcimAF
 from nbforager.foragers.extras import ExtrasAF
 from nbforager.foragers.ipam import IpamAF
@@ -284,49 +285,57 @@
         """Assemble Netbox objects in NbForager.tree within itself.
 
         The Netbox objects are represented as a multidimensional dictionary.
 
         :param dcim: True - Create additional keys to represent Netbox dcim objects.
             False - Only join objects that are present in the API response.
 
-            In dcim.devices:
+            In dcim.devices, virtualization.virtual_machines:
 
-            - ``console_ports``
-            - ``console_server_ports``
-            - ``device_bays``
-            - ``front_ports``
-            - ``interfaces``
-            - ``inventory_items``
-            - ``module_bays``
-            - ``power_outlets``
-            - ``power_ports``
-            - ``rear_ports``
+            - ``_console_ports``
+            - ``_console_server_ports``
+            - ``_device_bays``
+            - ``_front_ports``
+            - ``_interfaces``
+            - ``_inventory_items``
+            - ``_module_bays``
+            - ``_power_outlets``
+            - ``_power_ports``
+            - ``_rear_ports``
+
+            In dcim.interfaces, virtualization.interfaces:
+
+            - ``_ip_addresses``
 
         :param ipam: True - Create additional keys to represent Netbox ipam objects.
             False - Only join objects that are present in the API response.
 
             In ipam.aggregate, ipam.prefixes, ipam.ip_addresses:
 
-            - ``ipv4`` IPv4 object, child of ciscoconfparse.IPv4Obj
-            - ``aggregate`` Aggregate data for ipam.prefixes and ipam.ip_addresses
-            - ``super_prefix`` Related parent prefix data for ipam.prefixes and ipam.ip_addresses
-            - ``sub_prefixes`` Related child prefixes data for ipam.prefixes and ipam.ip_addresses
-            - ``ip_addresses`` Related IP addresses data for ipam.aggregates and ipam.prefixes
+            - ``_ipv4`` IPv4 object, child of ciscoconfparse.IPv4Obj
+            - ``_aggregate`` Aggregate data for ipam.prefixes and ipam.ip_addresses
+            - ``_super_prefix`` Related parent prefix data for ipam.prefixes and ipam.ip_addresses
+            - ``_sub_prefixes`` Related child prefixes data for ipam.prefixes and ipam.ip_addresses
+            - ``_ip_addresses`` Related IP addresses data for ipam.aggregates and ipam.prefixes
 
         :return: NbTree object with the joined Netbox objects.
 
         :rtype: NbTree
         """
-        tree: NbTree = nb_tree.join_tree(self.root)
+        tree: NbTree = deepcopy(self.root)
+        if dcim or ipam:
+            Joiner(tree).init_extra_keys()
+
+        tree = nb_tree.join_tree(tree)
         nb_tree.insert_tree(src=tree, dst=self.tree)
-        joiner = Joiner(tree=self.tree)
+
         if dcim:
-            joiner.join_dcim_devices()
+            Joiner(self.tree).join_dcim_devices()
         if ipam:
-            joiner.join_ipam_ipv4()
+            Joiner(self.tree).join_ipam_ipv4()
 
     def read_cache(self) -> None:
         """Read cached data from a pickle file.
 
         Save data to the NbForager.root and NbForager.status.
 
         :return: None. Update self object.
```

### Comparing `nbforager-0.2.1/nbforager/nb_tree.py` & `nbforager-0.2.2/nbforager/nb_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,22 +283,14 @@
             continue
 
         if not data:
             urls_.append(url)
     return urls_
 
 
-def delete_branches(tree: NbTree) -> NbTree:
-    """Delete data in multidimensional dictionaries."""
-
-def restore_branches(tree: NbTree) -> NbTree:
-    """Restore data in multidimensional dictionaries."""
-
-
-
 # ============================= helpers ==============================
 
 
 def _get_child(child: DAny, tree: NbTree) -> DAny:
     """Search child Netbox object in the model data to insert (replace) it in the parent.
 
     :param child: Netbox object that require dependency update.
```

### Comparing `nbforager-0.2.1/nbforager/parser/nb_custom.py` & `nbforager-0.2.2/nbforager/parser/nb_custom.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/parser/nb_parser.py` & `nbforager-0.2.2/nbforager/parser/nb_parser.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/parser/nb_value.py` & `nbforager-0.2.2/nbforager/parser/nb_value.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/py_tree.py` & `nbforager-0.2.2/nbforager/py_tree.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/nbforager/types_.py` & `nbforager-0.2.2/nbforager/types_.py`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/pyproject.toml` & `nbforager-0.2.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nbforager"
-version = "0.2.1"
+version = "0.2.2"
 description = "Python package designed to assist in working with the Netbox REST API. The filter parameters are identical to those in the Web UI filter form. It replaces brief data with full information, and Netbox objects are represented as a recursive multidimensional dictionary."
 authors = ["Vladimirs Prusakovs <vladimir.prusakovs@gmail.com>"]
 readme = "README.rst"
 license = "Apache-2.0"
 homepage = "https://github.com/vladimirs-git/nbforager"
 repository = "https://github.com/vladimirs-git/nbforager"
 keywords = ["netbox"]
@@ -24,14 +24,15 @@
 requests = "^2"
 tomli = "2.0.1"
 vhelpers = "^0.1"
 tabulate = "^0.9.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.6.1"
+poetry = "1.8.3"
 pygments = "^2.16.1"
 pylint = "^3.0.1"
 pytest = "^7.4.2"
 pytest-cov = "^4.1.0"
 pytest-mock = "^3.12.0"
 readthedocs-sphinx-search = "^0.3.1"
 requests-mock = "^1.11.0"
@@ -50,15 +51,15 @@
 nbforager = ["py.typed"]
 
 [tool.poetry.extras]
 test = ["pytest"]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/vladimirs-git/nbforager/issues"
-"Download URL" = "https://github.com/vladimirs-git/nbforager/archive/refs/tags/0.2.1.tar.gz"
+"Download URL" = "https://github.com/vladimirs-git/nbforager/archive/refs/tags/0.2.2.tar.gz"
 
 [tool.pylint]
 max-line-length = 100
 disable = "fixme"
 
 #[tool.pylint.message_control]
 #enable = ["too-many-public-methods"]
```

### Comparing `nbforager-0.2.1/README.rst` & `nbforager-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `nbforager-0.2.1/PKG-INFO` & `nbforager-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbforager
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python package designed to assist in working with the Netbox REST API. The filter parameters are identical to those in the Web UI filter form. It replaces brief data with full information, and Netbox objects are represented as a recursive multidimensional dictionary.
 Home-page: https://github.com/vladimirs-git/nbforager
 License: Apache-2.0
 Keywords: netbox
 Author: Vladimirs Prusakovs
 Author-email: vladimir.prusakovs@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -13,25 +13,26 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: test
 Requires-Dist: ciscoconfparse (>=1.9,<2.0)
 Requires-Dist: netports (>=0.12.1,<0.13.0)
 Requires-Dist: pydantic (>=2,<3)
 Requires-Dist: pynetbox (>=7.3.3,<8.0.0)
 Requires-Dist: requests (>=2,<3)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tomli (==2.0.1)
 Requires-Dist: vhelpers (>=0.1,<0.2)
 Project-URL: Bug Tracker, https://github.com/vladimirs-git/nbforager/issues
-Project-URL: Download URL, https://github.com/vladimirs-git/nbforager/archive/refs/tags/0.2.1.tar.gz
+Project-URL: Download URL, https://github.com/vladimirs-git/nbforager/archive/refs/tags/0.2.2.tar.gz
 Project-URL: Repository, https://github.com/vladimirs-git/nbforager
 Description-Content-Type: text/x-rst
 
 nbforager
 =========
```

