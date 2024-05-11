# Comparing `tmp/fim-utils-1.6.4.tar.gz` & `tmp/fim-utils-1.7.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fim-utils-1.6.4.tar", last modified: Tue Feb 27 14:29:18 2024, max compression
+gzip compressed data, was "fim-utils-1.7.0b1.tar", last modified: Sat May 11 02:54:36 2024, max compression
```

## Comparing `fim-utils-1.6.4.tar` & `fim-utils-1.7.0b1.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0     1955 2024-01-04 15:38:10.582923 fim-utils-1.6.4/.gitignore
--rw-r--r--   0        0        0     1071 2024-01-04 15:38:10.583073 fim-utils-1.6.4/LICENSE
--rw-r--r--   0        0        0      201 2024-01-04 15:38:10.583205 fim-utils-1.6.4/MANIFEST.in
--rw-r--r--   0        0        0     8509 2024-02-27 14:27:42.901797 fim-utils-1.6.4/README.md
--rw-r--r--   0        0        0      156 2024-02-27 14:25:15.584629 fim-utils-1.6.4/fimutil/__init__.py
--rw-r--r--   0        0        0        2 2024-01-04 15:38:10.583760 fim-utils-1.6.4/fimutil/al2s/__init__.py
--rw-r--r--   0        0        0       70 2024-02-27 14:27:42.901969 fim-utils-1.6.4/fimutil/al2s/al2s.conf.template
--rw-r--r--   0        0        0    12377 2024-02-27 14:27:42.902156 fim-utils-1.6.4/fimutil/al2s/al2s_api.py
--rw-r--r--   0        0        0     9603 2024-02-27 14:27:42.903191 fim-utils-1.6.4/fimutil/al2s/arm.py
--rw-r--r--   0        0        0      667 2024-01-04 15:38:10.584096 fim-utils-1.6.4/fimutil/al2s/cloud_cfg.py
--rw-r--r--   0        0        0        2 2024-01-04 15:38:10.584401 fim-utils-1.6.4/fimutil/netam/__init__.py
--rw-r--r--   0        0        0    21038 2024-01-04 15:38:10.584514 fim-utils-1.6.4/fimutil/netam/arm.py
--rw-r--r--   0        0        0     4247 2024-01-04 15:38:10.584715 fim-utils-1.6.4/fimutil/netam/nso.py
--rw-r--r--   0        0        0     3439 2024-01-04 15:38:10.584875 fim-utils-1.6.4/fimutil/netam/sr_pce.py
--rw-r--r--   0        0        0        2 2024-01-04 15:38:10.585206 fim-utils-1.6.4/fimutil/ralph/__init__.py
--rw-r--r--   0        0        0     3456 2024-01-04 15:38:10.585371 fim-utils-1.6.4/fimutil/ralph/asset.py
--rw-r--r--   0        0        0     2454 2024-01-04 15:38:10.585509 fim-utils-1.6.4/fimutil/ralph/dp_switch.py
--rw-r--r--   0        0        0     3991 2024-01-04 15:38:10.585652 fim-utils-1.6.4/fimutil/ralph/ethernetport.py
--rw-r--r--   0        0        0    22915 2024-01-04 15:56:37.608185 fim-utils-1.6.4/fimutil/ralph/fim_helper.py
--rw-r--r--   0        0        0     2574 2024-01-04 15:38:10.586028 fim-utils-1.6.4/fimutil/ralph/fpga.py
--rw-r--r--   0        0        0     2088 2024-02-27 14:24:50.635061 fim-utils-1.6.4/fimutil/ralph/gpu.py
--rw-r--r--   0        0        0     3307 2024-01-04 15:38:10.586277 fim-utils-1.6.4/fimutil/ralph/model.py
--rw-r--r--   0        0        0     1725 2024-01-04 15:38:10.586428 fim-utils-1.6.4/fimutil/ralph/nvme.py
--rw-r--r--   0        0        0     1384 2024-01-04 15:38:10.586557 fim-utils-1.6.4/fimutil/ralph/ralph_uri.py
--rw-r--r--   0        0        0     7294 2024-01-04 15:56:37.608454 fim-utils-1.6.4/fimutil/ralph/site.py
--rw-r--r--   0        0        0      885 2024-01-04 15:38:10.586904 fim-utils-1.6.4/fimutil/ralph/storage.py
--rw-r--r--   0        0        0    11128 2024-01-29 15:14:04.727793 fim-utils-1.6.4/fimutil/ralph/worker_node.py
--rw-r--r--   0        0        0        0 2024-01-04 15:38:10.587417 fim-utils-1.6.4/fimutil/utilities/__init__.py
--rw-r--r--   0        0        0     6216 2024-01-04 15:56:37.608653 fim-utils-1.6.4/fimutil/utilities/generate_instance_flavors.py
--rw-r--r--   0        0        0     1363 2024-02-27 14:27:42.903349 fim-utils-1.6.4/fimutil/utilities/scan_al2s.py
--rw-r--r--   0        0        0     1877 2024-01-04 15:38:10.588111 fim-utils-1.6.4/fimutil/utilities/scan_net.py
--rw-r--r--   0        0        0     5625 2024-01-04 15:38:10.588590 fim-utils-1.6.4/fimutil/utilities/scan_site.py
--rw-r--r--   0        0        0     2121 2024-01-04 15:38:10.588804 fim-utils-1.6.4/fimutil/utilities/scan_worker.py
--rw-r--r--   0        0        0     1030 2024-02-27 14:25:50.882866 fim-utils-1.6.4/pyproject.toml
--rw-r--r--   0        0        0      984 2024-01-04 15:38:10.589207 fim-utils-1.6.4/setup.py
--rw-r--r--   0        0        0     1513 2024-02-27 14:27:42.903591 fim-utils-1.6.4/test/al2s_test.py
--rw-r--r--   0        0        0     1114 2024-01-04 15:38:10.589872 fim-utils-1.6.4/test/netam_test.py
--rw-r--r--   0        0        0      326 2024-01-04 15:38:10.590054 fim-utils-1.6.4/test/ralph_test.py
--rw-r--r--   0        0        0     9231 1970-01-01 00:00:00.000000 fim-utils-1.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1955 2024-01-04 15:38:10.582923 fim-utils-1.7.0b1/.gitignore
+-rw-r--r--   0        0        0     1071 2024-01-04 15:38:10.583073 fim-utils-1.7.0b1/LICENSE
+-rw-r--r--   0        0        0      201 2024-01-04 15:38:10.583205 fim-utils-1.7.0b1/MANIFEST.in
+-rw-r--r--   0        0        0     8671 2024-05-11 02:27:13.133092 fim-utils-1.7.0b1/README.md
+-rw-r--r--   0        0        0      158 2024-05-11 02:47:18.942023 fim-utils-1.7.0b1/fimutil/__init__.py
+-rw-r--r--   0        0        0        2 2024-01-04 15:38:10.583760 fim-utils-1.7.0b1/fimutil/al2s/__init__.py
+-rw-r--r--   0        0        0       70 2024-02-27 14:27:42.901969 fim-utils-1.7.0b1/fimutil/al2s/al2s.conf.template
+-rw-r--r--   0        0        0    12377 2024-02-27 14:27:42.902156 fim-utils-1.7.0b1/fimutil/al2s/al2s_api.py
+-rw-r--r--   0        0        0     9603 2024-02-27 14:27:42.903191 fim-utils-1.7.0b1/fimutil/al2s/arm.py
+-rw-r--r--   0        0        0      667 2024-01-04 15:38:10.584096 fim-utils-1.7.0b1/fimutil/al2s/cloud_cfg.py
+-rw-r--r--   0        0        0        2 2024-01-04 15:38:10.584401 fim-utils-1.7.0b1/fimutil/netam/__init__.py
+-rw-r--r--   0        0        0    21817 2024-05-10 08:58:33.558511 fim-utils-1.7.0b1/fimutil/netam/arm.py
+-rw-r--r--   0        0        0     4247 2024-01-04 15:38:10.584715 fim-utils-1.7.0b1/fimutil/netam/nso.py
+-rw-r--r--   0        0        0     3439 2024-01-04 15:38:10.584875 fim-utils-1.7.0b1/fimutil/netam/sr_pce.py
+-rw-r--r--   0        0        0        2 2024-01-04 15:38:10.585206 fim-utils-1.7.0b1/fimutil/ralph/__init__.py
+-rw-r--r--   0        0        0     3478 2024-05-10 17:29:54.447929 fim-utils-1.7.0b1/fimutil/ralph/asset.py
+-rw-r--r--   0        0        0     2454 2024-01-04 15:38:10.585509 fim-utils-1.7.0b1/fimutil/ralph/dp_switch.py
+-rw-r--r--   0        0        0     3991 2024-01-04 15:38:10.585652 fim-utils-1.7.0b1/fimutil/ralph/ethernetport.py
+-rw-r--r--   0        0        0    25789 2024-05-11 02:02:54.660722 fim-utils-1.7.0b1/fimutil/ralph/fim_helper.py
+-rw-r--r--   0        0        0     2574 2024-01-04 15:38:10.586028 fim-utils-1.7.0b1/fimutil/ralph/fpga.py
+-rw-r--r--   0        0        0     2088 2024-02-27 14:24:50.635061 fim-utils-1.7.0b1/fimutil/ralph/gpu.py
+-rw-r--r--   0        0        0     3307 2024-01-04 15:38:10.586277 fim-utils-1.7.0b1/fimutil/ralph/model.py
+-rw-r--r--   0        0        0     1725 2024-01-04 15:38:10.586428 fim-utils-1.7.0b1/fimutil/ralph/nvme.py
+-rw-r--r--   0        0        0     1998 2024-05-10 21:42:05.649139 fim-utils-1.7.0b1/fimutil/ralph/p4_switch.py
+-rw-r--r--   0        0        0     1384 2024-01-04 15:38:10.586557 fim-utils-1.7.0b1/fimutil/ralph/ralph_uri.py
+-rw-r--r--   0        0        0     8381 2024-05-10 20:05:45.369295 fim-utils-1.7.0b1/fimutil/ralph/site.py
+-rw-r--r--   0        0        0      885 2024-01-04 15:38:10.586904 fim-utils-1.7.0b1/fimutil/ralph/storage.py
+-rw-r--r--   0        0        0    11349 2024-05-11 02:27:13.139125 fim-utils-1.7.0b1/fimutil/ralph/worker_node.py
+-rw-r--r--   0        0        0        0 2024-01-04 15:38:10.587417 fim-utils-1.7.0b1/fimutil/utilities/__init__.py
+-rw-r--r--   0        0        0     6216 2024-01-04 15:56:37.608653 fim-utils-1.7.0b1/fimutil/utilities/generate_instance_flavors.py
+-rw-r--r--   0        0        0     1363 2024-02-27 14:27:42.903349 fim-utils-1.7.0b1/fimutil/utilities/scan_al2s.py
+-rw-r--r--   0        0        0     1877 2024-01-04 15:38:10.588111 fim-utils-1.7.0b1/fimutil/utilities/scan_net.py
+-rw-r--r--   0        0        0     5625 2024-01-04 15:38:10.588590 fim-utils-1.7.0b1/fimutil/utilities/scan_site.py
+-rw-r--r--   0        0        0     2121 2024-01-04 15:38:10.588804 fim-utils-1.7.0b1/fimutil/utilities/scan_worker.py
+-rw-r--r--   0        0        0     1032 2024-05-10 20:47:11.260720 fim-utils-1.7.0b1/pyproject.toml
+-rw-r--r--   0        0        0      984 2024-01-04 15:38:10.589207 fim-utils-1.7.0b1/setup.py
+-rw-r--r--   0        0        0     1513 2024-02-27 14:27:42.903591 fim-utils-1.7.0b1/test/al2s_test.py
+-rw-r--r--   0        0        0     1114 2024-01-04 15:38:10.589872 fim-utils-1.7.0b1/test/netam_test.py
+-rw-r--r--   0        0        0      326 2024-01-04 15:38:10.590054 fim-utils-1.7.0b1/test/ralph_test.py
+-rw-r--r--   0        0        0     9397 1970-01-01 00:00:00.000000 fim-utils-1.7.0b1/PKG-INFO
```

### Comparing `fim-utils-1.6.4/.gitignore` & `fim-utils-1.7.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `fim-utils-1.6.4/LICENSE` & `fim-utils-1.7.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `fim-utils-1.6.4/README.md` & `fim-utils-1.7.0b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 
 The config file (by default `.scan-config.json` allows to statically override certain scanned details:
 - Allows for site to say it is using some other site's DP switch
 
 The general format example of the file is as follows (SITE1, SITE2 are all-caps site names):
 ```
 {
+  "ram_offset": 24
   "SITE1": {
     "dpswitch": {
       "URL": <URL of SITE2's dp switch in Ralph>,
       "Site": "SITE2"
     },
     "ptp": true,
     "storage": {
@@ -113,14 +114,15 @@
       }
     },
     "mac_offset": "f2:ab"
     "connected_ports": [ "HundredGigE0/0/0/15" ]
   }
 }
 ```
+`ram_offset` specifies an offset to subtract from the actual RAM value. This is adjustment needed to for RAM allocated to NOVA on the workers.
 `mac_offset` intended to be used with OpenStack sites to aid unique MAC generation for vNICs. Note
 that the first octet of mac_offset must be [even](https://github.com/openstack/neutron-lib/blob/cf494c8be10b36daf238fa12cf7c615656e6640d/neutron_lib/api/validators/__init__.py#L40).
 
 `connected_ports` are only effective for generating JSON files (do not affect ARMs) which are then used to put other ports
 (not include uplinks and facility ports) into admin DOWN state.
 
 `cpu_allocation_ratio` intended to be used when enabling over subscription for a site.
```

### Comparing `fim-utils-1.6.4/fimutil/al2s/al2s_api.py` & `fim-utils-1.7.0b1/fimutil/al2s/al2s_api.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.6.4/fimutil/al2s/arm.py` & `fim-utils-1.7.0b1/fimutil/al2s/arm.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.6.4/fimutil/al2s/cloud_cfg.py` & `fim-utils-1.7.0b1/fimutil/al2s/cloud_cfg.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.6.4/fimutil/netam/arm.py` & `fim-utils-1.7.0b1/fimutil/netam/arm.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,21 @@
                 continue
             ifaces = self.nso.interfaces(dev_name)
             isis_ifaces = self.nso.isis_interfaces(dev_name)
             if ifaces:
                 if isis_ifaces is None:
                     raise NetAmArmError(f"Device '{dev_name}' has no active isis interface - fix that or consider '--skip-device device-name'")
                 for iface in list(ifaces):
+                    # get loopback addresses
+                    if iface['name'] == 'Loopback0':
+                        if 'ietf-ip:ipv4' in iface:
+                            dev['loopback_ipv4'] = iface['ietf-ip:ipv4']['address'][0]['ip']
+                        if 'ietf-ip:ipv6' in iface:
+                            dev['loopback_ipv6'] = iface['ietf-ip:ipv6']['address'][0]['ip']
+                        continue
                     # skip if not an isis l2 p2p interfaces
                     is_isis_iface = False
                     for isis_iface in isis_ifaces:
                         if iface['name'] == isis_iface['name']:
                             is_isis_iface = True
                     # only keep interfaces in up status and of "*GigE0/1/2*" pattern
                     if iface['admin-status'] == 'up' and re.search('GigE\d/\d/\d|Bundle-Ether\d+', iface['name']):
@@ -135,14 +142,16 @@
                 if 'l2_vlan_range' in site_info:
                     l2_ns_labs = f.Labels.update(l2_ns_labs, vlan_range=site_info['l2_vlan_range'].split(','))
                 ipv4_ns_labs = f.Labels()
                 if 'ipv4_net' in site_info:
                     ipv4_ns_labs = f.Labels.update(ipv4_ns_labs, ipv4_subnet=site_info['ipv4_net'])
                 if 'ipv4_vlan_range' in site_info:
                     ipv4_ns_labs = f.Labels.update(ipv4_ns_labs, vlan_range=site_info['ipv4_vlan_range'].split(','))
+                if 'loopback_ipv4' in node:
+                    ipv4_ns_labs = f.Labels.update(ipv4_ns_labs, ipv4=node['loopback_ipv4'])
                 ipv4_ns = switch.add_network_service(name=switch.name + '-ipv4-ns', layer=f.Layer.L3,
                                                      labels=ipv4_ns_labs,
                                                      node_id=switch.node_id + '-ipv4-ns', nstype=f.ServiceType.FABNetv4)
                 ipv4ext_ns_labs = f.Labels()
                 if 'ipv4_public_net' in site_info:
                     ipv4ext_ns_labs = f.Labels.update(ipv4ext_ns_labs, ipv4_subnet=site_info['ipv4_public_net'])
                 if 'ipv4_vlan_range' in site_info:
@@ -152,14 +161,16 @@
                                                      node_id=switch.node_id + '-ipv4ext-ns', nstype=f.ServiceType.FABNetv4Ext)
 
                 ipv6_ns_labs = f.Labels()
                 if 'ipv6_net' in site_info:
                     ipv6_ns_labs = f.Labels.update(ipv6_ns_labs, ipv6_subnet=site_info['ipv6_net'])
                 if 'ipv6_vlan_range' in site_info:
                     ipv6_ns_labs = f.Labels.update(ipv6_ns_labs, vlan_range=site_info['ipv6_vlan_range'].split(','))
+                if 'loopback_ipv6' in node:
+                    ipv6_ns_labs = f.Labels.update(ipv6_ns_labs, ipv6=node['loopback_ipv6'])
                 ipv6_ns = switch.add_network_service(name=switch.name + '-ipv6-ns', layer=f.Layer.L3,
                                                      labels=ipv6_ns_labs,
                                                      node_id=switch.node_id + '-ipv6-ns', nstype=f.ServiceType.FABNetv6)
                 ipv6ext_ns_labs = f.Labels()
                 if 'ipv6_net' in site_info:
                     ipv6ext_ns_labs = f.Labels.update(ipv6ext_ns_labs, ipv6_subnet=site_info['ipv6_net'])
                 if 'ipv6_vlan_range' in site_info:
@@ -178,14 +189,16 @@
             # add L2 NetworkService
             l2_ns = switch.add_network_service(name=switch.name + '-ns', layer=f.Layer.L2, labels=l2_ns_labs,
                                                node_id=switch.node_id + '-ns', nstype=f.ServiceType.MPLS)
             # add ports
             if 'interfaces' in node:
                 for port in node['interfaces']:
                     port_name = port['name']
+                    if 'phys-address' not in port:
+                        continue
                     port_mac = port['phys-address']
                     port_nid = f"port+{node_name}:{port_name}"
                     speed_gbps = int(int(port['speed']) / 1000000000)
                     # add capabilities
                     port_caps = f.Capacities(bw=speed_gbps)
                     # add labels (vlan ??)
                     port_labs = f.Labels(local_name=port_name, mac=port_mac)
```

### Comparing `fim-utils-1.6.4/fimutil/netam/nso.py` & `fim-utils-1.7.0b1/fimutil/netam/nso.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.6.4/fimutil/netam/sr_pce.py` & `fim-utils-1.7.0b1/fimutil/netam/sr_pce.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.6.4/fimutil/ralph/asset.py` & `fim-utils-1.7.0b1/fimutil/ralph/asset.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     EthernetCardPF = auto()
     EthernetCardVF = auto()
     Model = auto()
     Storage = auto()
     DPSwitch = auto()
     Abstract = auto()
     FPGA = auto()
+    P4Switch = auto()
 
     def __str__(self):
         return self.name
 
 
 class RalphAsset(ABC):
     """
```

### Comparing `fim-utils-1.6.4/fimutil/ralph/dp_switch.py` & `fim-utils-1.7.0b1/fimutil/ralph/dp_switch.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.6.4/fimutil/ralph/ethernetport.py` & `fim-utils-1.7.0b1/fimutil/ralph/ethernetport.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.6.4/fimutil/ralph/fim_helper.py` & `fim-utils-1.7.0b1/fimutil/ralph/fim_helper.py`

 * *Files 9% similar despite different names*

```diff
@@ -493,14 +493,80 @@
                                  stitch_node=True)
         topo.add_link(name='l' + str(link_idx),
                       node_id=sp.node_id + '-DAC',
                       ltype=LinkType.Patch,
                       interfaces=[sp, v])
         link_idx += 1
 
+    # create p4 switch with interfaces and links back to dataplane switch ports
+    logging.debug('Adding p4 switch')
+    if site.p4_switch is None:
+        logging.info(f'P4 Switch was not detected/catalogued')
+        return topo
+
+    # this prefers an IP address, but uses S/N if IP is None (like in GENI racks)
+    logging.info(f'Adding P4 switch {site.name}')
+
+    p4_name = p4_switch_name_id(real_switch_site.lower(),
+                                site.p4_switch.fields['IP'] if site.p4_switch.fields['IP'] else site.p4_switch.fields['SN'])
+
+    p4 = topo.add_node(name=p4_name[0],
+                       node_id=p4_name[1],
+                       site=site.name, ntype=NodeType.Switch, stitch_node=True)
+
+    p4_service_type = ServiceType.MPLS
+    p4_ns = p4.add_network_service(name=p4.name + '-ns', node_id=p4.node_id + '-ns',
+                                   nstype=p4_service_type, stitch_node=False)
+
+    dp_to_p4_ports = []
+
+    for c in site.p4_switch.components.values():
+        speed, unit = __parse_speed_spec(c.fields['Speed'])
+        speed = __normalize_units(speed, unit, 'G')
+        speed_int = int(speed)
+        capacities = Capacities(bw=speed_int)
+
+        description = c.fields['Description']
+        if "management" in description:
+            port_name = "mgmt"
+        else:
+            # Use regular expression to find the value after "Port"
+            match = re.search(r'Port (\d+)', description)
+            if not match:
+                logging.warning(f"Port could not be determined from Description for component: {c}")
+                continue
+            port_name = match.group(1)
+
+        labels = Labels(local_name=f'p{port_name}')
+        if c.fields['MAC']:
+            labels.mac = c.fields['MAC']
+
+        connection = c.fields['Connection']
+
+        match2 = re.search(r'port\s+(\S+)', connection, re.IGNORECASE)
+        if not match2:
+            logging.warning(f"Data Plane port could not be determined from Connection for component: {c}")
+            continue
+
+        # Build dp_to_p4_ports here
+        dp_to_p4_ports.append(match2.group(1))
+
+        p4_ns.add_interface(name=f'p{port_name}', node_id=p4_name[1] + f'-int{port_name}' if p4_name[1] else None,
+                            itype=InterfaceType.DedicatedPort,
+                            labels=labels, capacities=capacities)
+
+    # add dp switch ports that link to P4 switch ports (note they are not stitch nodes!!)
+    for d, p4idx in zip(dp_to_p4_ports, range(1, 8 + 1)):
+        sp = dp_ns.add_interface(name=d, itype=InterfaceType.TrunkPort,
+                                 node_id=dp_port_id(dp.name, d), stitch_node=False)
+        topo.add_link(name='l' + str(link_idx), ltype=LinkType.Patch,
+                           interfaces=[p4.interfaces[f'p{p4idx}'], sp],
+                           node_id=sp.node_id + '-DAC')
+        link_idx += 1
+
     return topo
 
 
 if __name__ == "__main__":
     logging.basicConfig(level=logging.INFO)
     print(__parse_speed_spec('10 Gbps'))
     print(__parse_speed_spec('10G'))
```

### Comparing `fim-utils-1.6.4/fimutil/ralph/fpga.py` & `fim-utils-1.7.0b1/fimutil/ralph/fpga.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.6.4/fimutil/ralph/gpu.py` & `fim-utils-1.7.0b1/fimutil/ralph/gpu.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.6.4/fimutil/ralph/model.py` & `fim-utils-1.7.0b1/fimutil/ralph/model.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.6.4/fimutil/ralph/nvme.py` & `fim-utils-1.7.0b1/fimutil/ralph/nvme.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.6.4/fimutil/ralph/ralph_uri.py` & `fim-utils-1.7.0b1/fimutil/ralph/ralph_uri.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.6.4/fimutil/ralph/site.py` & `fim-utils-1.7.0b1/fimutil/ralph/site.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 from abc import ABC
 from urllib.parse import urlencode
 import pyjq
 from typing import Dict
 import json
 
+from fimutil.ralph.p4_switch import P4Switch
 from fimutil.ralph.ralph_uri import RalphURI
 from fimutil.ralph.worker_node import WorkerNode
 from fimutil.ralph.storage import Storage
 from fimutil.ralph.dp_switch import DPSwitch
 
 
 class Site:
@@ -19,14 +20,15 @@
     def __init__(self, *, site_name: str, ralph: RalphURI, config: Dict = None, domain: str = '.fabric-testbed.net'):
         """
         Site name can be upper or lower case
         """
         self.workers = list()
         self.storage = None
         self.dp_switch = None
+        self.p4_switch = None
         self.ptp = False
         self.name = site_name
         self.domain = domain
         self.ralph = ralph
         self.config = config
 
     def catalog(self):
@@ -60,14 +62,26 @@
             if not dp_switch_url:
                 raise ValueError
             self.dp_switch = DPSwitch(uri=dp_switch_url, ralph=self.ralph)
             self.dp_switch.parse()
         except ValueError:
             logging.warning('Unable to find a dataplane switch in site, continuing')
 
+        try:
+            logging.info(f'Searching for P4 switch URL')
+            query = {'hostname': f'{self.name.lower()}-p4-sw' + self.domain}
+            results = self.ralph.get_json_object(self.ralph.base_uri + 'data-center-assets/?' +
+                                                 urlencode(query))
+            p4_switch_url = pyjq.one('[ .results[0].url ]', results)[0]
+            logging.info(f'Identified P4 switch {p4_switch_url=}')
+            self.p4_switch = P4Switch(uri=p4_switch_url, ralph=self.ralph)
+            self.p4_switch.parse()
+        except ValueError:
+            logging.warning('Unable to find a p4 switch in site, continuing')
+
         query = {'hostname': f'{self.name.lower()}-time' + self.domain}
         results = self.ralph.get_json_object(self.ralph.base_uri + 'data-center-assets/?' +
                                              urlencode(query))
 
         if self.config and self.config.get(self.name) and self.config.get(self.name).get('ptp'):
             ptp_override = self.config.get(self.name).get('ptp')
             if not isinstance(ptp_override, bool):
@@ -130,24 +144,33 @@
 
     def __str__(self):
         assets = list()
         if self.storage:
             assets.append(str(self.storage))
         if self.dp_switch:
             assets.append(str(self.dp_switch))
+        if self.p4_switch:
+            assets.append(str(self.p4_switch))
         for w in self.workers:
             assets.append(str(w))
         return '\n'.join(assets)
 
     def to_json(self):
         ret = dict()
         if self.storage:
             ret["Storage"] = self.storage.fields.copy()
         if self.dp_switch:
             ret["DataPlane"] = self.dp_switch.fields.copy()
+        if self.p4_switch:
+            ret["P4"] = self.p4_switch.fields.copy()
+            p4_dp_ports = self.p4_switch.get_dp_ports()
+            p4_dp_ports = list(set(p4_dp_ports))
+            p4_dp_ports.sort()
+            ret["P4"]["Connected_ports"] = p4_dp_ports
+
         # collect port information from all workers
         dp_ports = list()
         for w in self.workers:
             dp_ports.extend(w.get_dp_ports())
         # see if any extra ports are mentioned in the config file
         if self.config and self.config.get(self.name) and self.config.get(self.name).get('connected_ports'):
             dp_ports.extend(self.config.get(self.name).get('connected_ports'))
@@ -155,8 +178,8 @@
         dp_ports = list(set(dp_ports))
         dp_ports.sort()
         ret["DataPlane"]["Connected_ports"] = dp_ports
         n = list()
         for w in self.workers:
             n.append(w.to_json())
         ret["Nodes"] = n
-        return ret
+        return ret
```

### Comparing `fim-utils-1.6.4/fimutil/ralph/storage.py` & `fim-utils-1.7.0b1/fimutil/ralph/storage.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.6.4/fimutil/ralph/worker_node.py` & `fim-utils-1.7.0b1/fimutil/ralph/worker_node.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,14 +94,20 @@
         ram = int(custom_fields_dict.get('usable_memory', '0'))//1024
         if ram > 0:
             self.model.fields['RAM'] = f'{ram}G'
         disk = custom_fields_dict.get('usable_disk')
         if disk:
             self.model.fields['Disk'] = f'{disk}G'
 
+        if self.config and self.config.get('ram_offset'):
+            ram_offset = self.config.get('ram_offset')
+            ram -= ram_offset
+            if ram > 0:
+                self.model.fields['RAM'] = f'{ram}G'
+
         # override from config if present
         if self.config and self.config.get(self.site) and self.config.get(self.site).get('workers') and \
             self.config.get(self.site).get('workers').get(self.fields['Name']):
             worker_override = self.config.get(self.site).get('workers').get(self.fields['Name'])
             self.model.fields['RAM'] = worker_override.get('RAM', self.model.fields['RAM'])
             self.model.fields['CPU'] = worker_override.get('CPU', self.model.fields['CPU'])
             self.model.fields['Core'] = worker_override.get('Core', self.model.fields['Core'])
```

### Comparing `fim-utils-1.6.4/fimutil/utilities/generate_instance_flavors.py` & `fim-utils-1.7.0b1/fimutil/utilities/generate_instance_flavors.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.6.4/fimutil/utilities/scan_al2s.py` & `fim-utils-1.7.0b1/fimutil/utilities/scan_al2s.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.6.4/fimutil/utilities/scan_net.py` & `fim-utils-1.7.0b1/fimutil/utilities/scan_net.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.6.4/fimutil/utilities/scan_site.py` & `fim-utils-1.7.0b1/fimutil/utilities/scan_site.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.6.4/fimutil/utilities/scan_worker.py` & `fim-utils-1.7.0b1/fimutil/utilities/scan_worker.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.6.4/pyproject.toml` & `fim-utils-1.7.0b1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License",
 		"Programming Language :: Python :: 3",
 		"Operating System :: OS Independent"]
 dynamic = ["version", "description"]
 requires-python = '>=3.9'
 dependencies = [
-	"fabric_fim >= 1.6.2",
+	"fabric_fim >= 1.7.0b1",
     "pyjq == 2.6.0",
 	"jsonpath_ng == 1.5.3",
 	]
 
 [tool.flit.module]
 name = "fimutil"
```

### Comparing `fim-utils-1.6.4/setup.py` & `fim-utils-1.7.0b1/setup.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.6.4/test/al2s_test.py` & `fim-utils-1.7.0b1/test/al2s_test.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.6.4/test/netam_test.py` & `fim-utils-1.7.0b1/test/netam_test.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.6.4/PKG-INFO` & `fim-utils-1.7.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: fim-utils
-Version: 1.6.4
+Version: 1.7.0b1
 Summary: This is a package of Information Model utilitied for FABRIC
 Author-email: Ilya Baldin <ibaldin@renci.org>, Xi Yang <xiyang@es.net>, Hussamuddin Nasir <nasir@netlab.uky.edu>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Dist: fabric_fim >= 1.6.2
+Requires-Dist: fabric_fim >= 1.7.0b1
 Requires-Dist: pyjq == 2.6.0
 Requires-Dist: jsonpath_ng == 1.5.3
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: flit ; extra == "test"
 Project-URL: Home, https://github.com/fabric-testbed/information-model-utils
 Provides-Extra: test
 
@@ -108,14 +108,15 @@
 
 The config file (by default `.scan-config.json` allows to statically override certain scanned details:
 - Allows for site to say it is using some other site's DP switch
 
 The general format example of the file is as follows (SITE1, SITE2 are all-caps site names):
 ```
 {
+  "ram_offset": 24
   "SITE1": {
     "dpswitch": {
       "URL": <URL of SITE2's dp switch in Ralph>,
       "Site": "SITE2"
     },
     "ptp": true,
     "storage": {
@@ -131,14 +132,15 @@
       }
     },
     "mac_offset": "f2:ab"
     "connected_ports": [ "HundredGigE0/0/0/15" ]
   }
 }
 ```
+`ram_offset` specifies an offset to subtract from the actual RAM value. This is adjustment needed to for RAM allocated to NOVA on the workers.
 `mac_offset` intended to be used with OpenStack sites to aid unique MAC generation for vNICs. Note
 that the first octet of mac_offset must be [even](https://github.com/openstack/neutron-lib/blob/cf494c8be10b36daf238fa12cf7c615656e6640d/neutron_lib/api/validators/__init__.py#L40).
 
 `connected_ports` are only effective for generating JSON files (do not affect ARMs) which are then used to put other ports
 (not include uplinks and facility ports) into admin DOWN state.
 
 `cpu_allocation_ratio` intended to be used when enabling over subscription for a site.
```

