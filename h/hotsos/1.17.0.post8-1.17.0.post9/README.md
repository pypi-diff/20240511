# Comparing `tmp/hotsos-1.17.0.post8.tar.gz` & `tmp/hotsos-1.17.0.post9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hotsos-1.17.0.post8.tar", last modified: Fri Apr  5 08:13:23 2024, max compression
+gzip compressed data, was "hotsos-1.17.0.post9.tar", last modified: Tue Apr  9 08:55:40 2024, max compression
```

## Comparing `hotsos-1.17.0.post8.tar` & `hotsos-1.17.0.post9.tar`

### file list

```diff
@@ -1,435 +1,435 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.137164 hotsos-1.17.0.post8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-05 08:13:23.137164 hotsos-1.17.0.post8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.073169 hotsos-1.17.0.post8/hotsos/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 08:13:13.000000 hotsos-1.17.0.post8/hotsos/.repo-info
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14992 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9479 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.077168 hotsos-1.17.0.post8/hotsos/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10727 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     9157 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.081168 hotsos-1.17.0.post8/hotsos/core/host_helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/host_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/host_helpers/apparmor.py
--rw-r--r--   0 runner    (1001) docker     (127)    41470 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/host_helpers/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/host_helpers/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/host_helpers/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/host_helpers/filestat.py
--rw-r--r--   0 runner    (1001) docker     (127)    13279 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/host_helpers/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    14431 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/host_helpers/packaging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/host_helpers/pebble.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/host_helpers/ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/host_helpers/sysctl.py
--rw-r--r--   0 runner    (1001) docker     (127)    15618 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/host_helpers/systemd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/host_helpers/uptime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.081168 hotsos-1.17.0.post8/hotsos/core/issues/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/issues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/issues/issue_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/issues/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.081168 hotsos-1.17.0.post8/hotsos/core/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.081168 hotsos-1.17.0.post8/hotsos/core/plugins/juju/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/juju/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/juju/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/juju/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.081168 hotsos-1.17.0.post8/hotsos/core/plugins/kernel/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/kernel/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/kernel/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.085168 hotsos-1.17.0.post8/hotsos/core/plugins/kernel/kernlog/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/kernel/kernlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14852 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/kernel/kernlog/calltrace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/kernel/kernlog/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/kernel/kernlog/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/kernel/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    20691 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/kernel/net.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/kernel/sysfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/kubernetes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.085168 hotsos-1.17.0.post8/hotsos/core/plugins/lxd/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/lxd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/lxd/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/maas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/mysql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.085168 hotsos-1.17.0.post8/hotsos/core/plugins/openstack/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/openstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8531 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/openstack/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    63860 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/openstack/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/openstack/neutron.py
--rw-r--r--   0 runner    (1001) docker     (127)    10628 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/openstack/nova.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/openstack/octavia.py
--rw-r--r--   0 runner    (1001) docker     (127)    19646 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/openstack/openstack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.085168 hotsos-1.17.0.post8/hotsos/core/plugins/openvswitch/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/openvswitch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/openvswitch/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/openvswitch/ovn.py
--rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/openvswitch/ovs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/pacemaker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.085168 hotsos-1.17.0.post8/hotsos/core/plugins/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/rabbitmq/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/rabbitmq/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/sosreport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.085168 hotsos-1.17.0.post8/hotsos/core/plugins/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/storage/bcache.py
--rw-r--r--   0 runner    (1001) docker     (127)    38502 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/storage/ceph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.089167 hotsos-1.17.0.post8/hotsos/core/plugins/system/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/system/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/system/system.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugins/vault.py
--rw-r--r--   0 runner    (1001) docker     (127)    15121 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/plugintools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/root_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.089167 hotsos-1.17.0.post8/hotsos/core/ycheck/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/ycheck/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.089167 hotsos-1.17.0.post8/hotsos/core/ycheck/engine/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/ycheck/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/ycheck/engine/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.089167 hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8817 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    17002 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/conclusions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/inputdef.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.089167 hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/requires/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/requires/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/requires/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/requires/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.093167 hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/requires/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/requires/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8661 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/requires/types/apt.py
--rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/requires/types/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/requires/types/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/requires/types/pebble.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/requires/types/property.py
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/requires/types/snap.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/requires/types/systemd.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/requires/types/varops.py
--rw-r--r--   0 runner    (1001) docker     (127)    15726 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/vardef.py
--rw-r--r--   0 runner    (1001) docker     (127)    16022 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/ycheck/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/core/ycheck/scenarios.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.025173 hotsos-1.17.0.post8/hotsos/defs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.025173 hotsos-1.17.0.post8/hotsos/defs/events/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.093167 hotsos-1.17.0.post8/hotsos/defs/events/openstack/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/events/openstack/apache.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/events/openstack/apparmor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/events/openstack/http-requests.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.093167 hotsos-1.17.0.post8/hotsos/defs/events/openstack/neutron/
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/events/openstack/neutron/agents.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/events/openstack/neutron/ml2-routers.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.093167 hotsos-1.17.0.post8/hotsos/defs/events/openstack/nova/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/events/openstack/nova/external-events.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.093167 hotsos-1.17.0.post8/hotsos/defs/events/openstack/nova/migrations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.093167 hotsos-1.17.0.post8/hotsos/defs/events/openstack/nova/migrations/live-migration/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/events/openstack/nova/migrations/live-migration/dst-pre-live-migration.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/events/openstack/nova/migrations/live-migration/src-migration.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/events/openstack/nova/migrations/live-migration/src-post-live-migration.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/events/openstack/nova/migrations/migrations.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/events/openstack/nova/nova-compute.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/events/openstack/octavia.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.025173 hotsos-1.17.0.post8/hotsos/defs/events/openvswitch/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.093167 hotsos-1.17.0.post8/hotsos/defs/events/openvswitch/ovn/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/events/openvswitch/ovn/errors-and-warnings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/events/openvswitch/ovn/ovn-central.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/events/openvswitch/ovn/ovn-controller.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.097167 hotsos-1.17.0.post8/hotsos/defs/events/openvswitch/ovs/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/events/openvswitch/ovs/bfd.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/events/openvswitch/ovs/datapath-checks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/events/openvswitch/ovs/errors-and-warnings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/events/openvswitch/ovs/ovs-vswitchd.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.025173 hotsos-1.17.0.post8/hotsos/defs/events/storage/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.025173 hotsos-1.17.0.post8/hotsos/defs/events/storage/ceph/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.097167 hotsos-1.17.0.post8/hotsos/defs/events/storage/ceph/mon/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/events/storage/ceph/mon/mon.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/events/storage/ceph/mon/monlogs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.097167 hotsos-1.17.0.post8/hotsos/defs/events/storage/ceph/osd/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/events/storage/ceph/osd/osd.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/events/storage/ceph/osd/osdlogs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.069169 hotsos-1.17.0.post8/hotsos/defs/scenarios/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.097167 hotsos-1.17.0.post8/hotsos/defs/scenarios/juju/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.097167 hotsos-1.17.0.post8/hotsos/defs/scenarios/juju/bugs/
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/juju/bugs/lp1812361.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/juju/bugs/lp1852502.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/juju/bugs/lp1858519.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/juju/bugs/lp1895040.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/juju/bugs/lp1910958.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/juju/bugs/lp1948906.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/juju/bugs/lp1983140.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/juju/bugs/lp1983506.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/juju/bugs/lp1996230.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/juju/charm_unit_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/juju/juju.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/juju/jujud_machine_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/juju/snap_channel.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.101167 hotsos-1.17.0.post8/hotsos/defs/scenarios/kernel/
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/kernel/amd_iommu_pt.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/kernel/disk_failure.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/kernel/kernlog_calltrace.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/kernel/memory.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.101167 hotsos-1.17.0.post8/hotsos/defs/scenarios/kernel/network/
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/kernel/network/misc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/kernel/network/netlink.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7336 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/kernel/network/tcp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/kernel/network/udp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/kernel/qla2xxx.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.101167 hotsos-1.17.0.post8/hotsos/defs/scenarios/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/kubernetes/kubernetes.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/kubernetes/system_cpufreq_mode.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.101167 hotsos-1.17.0.post8/hotsos/defs/scenarios/lxd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.101167 hotsos-1.17.0.post8/hotsos/defs/scenarios/lxd/bugs/
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/lxd/bugs/lp1807628.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/lxd/lxcfs_deadlock.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/lxd/snap_channel.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.101167 hotsos-1.17.0.post8/hotsos/defs/scenarios/maas/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/maas/maas_proxy_issue.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.101167 hotsos-1.17.0.post8/hotsos/defs/scenarios/mysql/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.101167 hotsos-1.17.0.post8/hotsos/defs/scenarios/mysql/bugs/
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/mysql/bugs/lp1959861.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/mysql/bugs/lp1971565.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/mysql/bugs/lp2039444.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/mysql/bugs/lp372017.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/mysql/mysql.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/mysql/mysql_connections.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.105166 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.065169 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/barbican/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.105166 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/barbican/bugs/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/barbican/bugs/lp1946787.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.065169 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/cinder/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.105166 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/cinder/bugs/
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/cinder/bugs/lp2004555.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/eol.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.065169 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/keystone/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.105166 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/keystone/bugs/
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/keystone/bugs/lp1896125.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.105166 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/masakari/
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/masakari/pacemaker_remote.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.105166 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/neutron/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.109166 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1794991.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1883089.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1896506.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1907686.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1927868.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1928031.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1929832.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1948466.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1960319.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1965297.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1979089.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1993628.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1996594.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/neutron/neutron_ovs_cleanup.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/neutron/oslo_privsep_errors.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/neutron/ovn_stale_db.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/neutron/ovndb_leader_bouncing.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.109166 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/nova/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.109166 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/nova/bugs/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp1761062.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp1860743.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp1888395.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp1904580.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp1944619.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp1967956.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp2004555.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp2012284.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/nova/config_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/nova/cpu_pinning.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/nova/service_mem_usage.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.109166 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/octavia/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.109166 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/octavia/bugs/
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/octavia/bugs/lp2029857.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/octavia/bugs/sb1896125.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/octavia/excessive_failovers.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/octavia/hm_port_health.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/openstack.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/openstack_apache2_certificates.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/openstack_charm_conflicts.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.109166 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/openstack_charms/
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/openstack_charms/nova_cc_ssh_known_hosts_fail.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/pkgs_from_mixed_releases_found.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/system_cpufreq_mode.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/systemd_masked_services.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.113166 hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.113166 hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/bugs/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/bugs/lp1839592.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/bugs/lp1978806.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/dpif_lost_packets.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/dpif_resubmit_actions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/openvswitch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.113166 hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/ovn/
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/ovn/bfd_flapping.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.113166 hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/ovn/bugs/
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1865127.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1917475.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_certs_logs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_services.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_certs_valid.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_chassis_certs_logs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_elections.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_upgrades.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/ovn/ovsdb_reconnect_errors.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/ovn/service_mem_usage.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/service_restarts.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.113166 hotsos-1.17.0.post8/hotsos/defs/scenarios/pacemaker/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.113166 hotsos-1.17.0.post8/hotsos/defs/scenarios/pacemaker/bugs/
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/pacemaker/bugs/lp1874719.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/pacemaker/pacemaker.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.117165 hotsos-1.17.0.post8/hotsos/defs/scenarios/rabbitmq/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.117165 hotsos-1.17.0.post8/hotsos/defs/scenarios/rabbitmq/bugs/
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/rabbitmq/bugs/lp1943937.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/rabbitmq/cluster_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/rabbitmq/cluster_logchecks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/rabbitmq/cluster_resources.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/rabbitmq/rabbitmq.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.117165 hotsos-1.17.0.post8/hotsos/defs/scenarios/sosreport/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/sosreport/plugin_timeouts.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.117165 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.117165 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/bcache/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/bcache/bcache.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/bcache/bdev.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/bcache/cacheset.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.069169 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.117165 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mgr/
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mgr/autoscaler_overlap_roots.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.121165 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/auth_insecure_global_id_reclaim_allowed.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/autoscaler_bug.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_size.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_spillover.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph-mon.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_address_overlap.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_cluster_health.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_versions_mismatch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/crushmap_bucket_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/empty_clog.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/eol.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/laggy_pgs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/large_omap_objects.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/meta_backend_mon.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_db_too_big.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_elections_flapping.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_flapping.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_maps_backlog_too_large.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_messenger_v2_protocol.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_heartbeats.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_ops.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_unusual_raw.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_imbalance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_overdose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/required_osd_release_mismatch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/rgw_frontend.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/ssds_using_bcache.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/unresponsive_mon_mgr.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.125165 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.125165 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1936136.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1959649.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1996010.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2013960.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2016845.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph-osd.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph_address_overlap.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/eol.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/filestore_to_bluestore_upgrade.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/juju_ceph_no_bcache_tuning.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/meta_backend_osd.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_flapping.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_latency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_slow_ops.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/pg_overdose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/ssd_osds_no_discard.yaml.disabled
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/system_cpufreq_mode.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.125165 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-rgw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.125165 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-rgw/bugs/
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-rgw/bugs/lp1974138.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-rgw/rgw_frontend_rgw.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.125165 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/common/
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/common/ceph_charm_conflicts.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/storage.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.125165 hotsos-1.17.0.post8/hotsos/defs/scenarios/system/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/system/system.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/system/unattended_upgrades.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.125165 hotsos-1.17.0.post8/hotsos/defs/scenarios/vault/
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/defs/scenarios/vault/snap_channel.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.125165 hotsos-1.17.0.post8/hotsos/plugin_extensions/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.125165 hotsos-1.17.0.post8/hotsos/plugin_extensions/juju/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/juju/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/juju/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.129164 hotsos-1.17.0.post8/hotsos/plugin_extensions/kernel/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/kernel/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.129164 hotsos-1.17.0.post8/hotsos/plugin_extensions/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/kubernetes/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.129164 hotsos-1.17.0.post8/hotsos/plugin_extensions/lxd/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/lxd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/lxd/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.129164 hotsos-1.17.0.post8/hotsos/plugin_extensions/maas/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/maas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/maas/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.129164 hotsos-1.17.0.post8/hotsos/plugin_extensions/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/mysql/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.129164 hotsos-1.17.0.post8/hotsos/plugin_extensions/openstack/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/openstack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.129164 hotsos-1.17.0.post8/hotsos/plugin_extensions/openstack/agent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/openstack/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14382 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/openstack/agent/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/openstack/agent/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/openstack/nova_external_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/openstack/service_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/openstack/service_network_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/openstack/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/openstack/vm_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.133164 hotsos-1.17.0.post8/hotsos/plugin_extensions/openvswitch/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/openvswitch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9596 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/openvswitch/event_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/openvswitch/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.133164 hotsos-1.17.0.post8/hotsos/plugin_extensions/pacemaker/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/pacemaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/pacemaker/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.133164 hotsos-1.17.0.post8/hotsos/plugin_extensions/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/rabbitmq/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.133164 hotsos-1.17.0.post8/hotsos/plugin_extensions/sosreport/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/sosreport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/sosreport/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.133164 hotsos-1.17.0.post8/hotsos/plugin_extensions/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/storage/bcache_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/storage/ceph_event_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/storage/ceph_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.133164 hotsos-1.17.0.post8/hotsos/plugin_extensions/system/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/system/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/system/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.133164 hotsos-1.17.0.post8/hotsos/plugin_extensions/vault/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/plugin_extensions/vault/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.133164 hotsos-1.17.0.post8/hotsos/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/templates/content_dict.html
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/templates/content_list.html
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/hotsos/templates/header.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:13:23.133164 hotsos-1.17.0.post8/hotsos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-05 08:13:23.000000 hotsos-1.17.0.post8/hotsos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16441 2024-04-05 08:13:23.000000 hotsos-1.17.0.post8/hotsos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 08:13:23.000000 hotsos-1.17.0.post8/hotsos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-05 08:13:23.000000 hotsos-1.17.0.post8/hotsos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-05 08:13:23.000000 hotsos-1.17.0.post8/hotsos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 08:13:23.000000 hotsos-1.17.0.post8/hotsos.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 08:13:23.137164 hotsos-1.17.0.post8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-05 08:13:07.000000 hotsos-1.17.0.post8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.850190 hotsos-1.17.0.post9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-09 08:55:40.850190 hotsos-1.17.0.post9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.798191 hotsos-1.17.0.post9/hotsos/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 08:55:31.000000 hotsos-1.17.0.post9/hotsos/.repo-info
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14992 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9479 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.798191 hotsos-1.17.0.post9/hotsos/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10727 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9157 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.802191 hotsos-1.17.0.post9/hotsos/core/host_helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/host_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/host_helpers/apparmor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41924 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/host_helpers/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/host_helpers/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/host_helpers/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/host_helpers/filestat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13279 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/host_helpers/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14431 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/host_helpers/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/host_helpers/pebble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/host_helpers/ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/host_helpers/sysctl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15618 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/host_helpers/systemd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/host_helpers/uptime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.802191 hotsos-1.17.0.post9/hotsos/core/issues/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/issues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/issues/issue_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/issues/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.802191 hotsos-1.17.0.post9/hotsos/core/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.802191 hotsos-1.17.0.post9/hotsos/core/plugins/juju/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/juju/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/juju/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/juju/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.806191 hotsos-1.17.0.post9/hotsos/core/plugins/kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/kernel/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/kernel/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.806191 hotsos-1.17.0.post9/hotsos/core/plugins/kernel/kernlog/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/kernel/kernlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14852 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/kernel/kernlog/calltrace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/kernel/kernlog/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/kernel/kernlog/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/kernel/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20691 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/kernel/net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/kernel/sysfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/kubernetes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.806191 hotsos-1.17.0.post9/hotsos/core/plugins/lxd/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/lxd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/lxd/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/maas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/mysql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.806191 hotsos-1.17.0.post9/hotsos/core/plugins/openstack/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/openstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8531 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/openstack/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63860 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/openstack/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/openstack/neutron.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10628 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/openstack/nova.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/openstack/octavia.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19646 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/openstack/openstack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.806191 hotsos-1.17.0.post9/hotsos/core/plugins/openvswitch/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/openvswitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/openvswitch/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/openvswitch/ovn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/openvswitch/ovs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/pacemaker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.806191 hotsos-1.17.0.post9/hotsos/core/plugins/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/rabbitmq/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/rabbitmq/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/sosreport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.810191 hotsos-1.17.0.post9/hotsos/core/plugins/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/storage/bcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38502 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/storage/ceph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.810191 hotsos-1.17.0.post9/hotsos/core/plugins/system/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/system/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/system/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugins/vault.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15121 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/plugintools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/root_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.810191 hotsos-1.17.0.post9/hotsos/core/ycheck/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/ycheck/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.810191 hotsos-1.17.0.post9/hotsos/core/ycheck/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/ycheck/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/ycheck/engine/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.810191 hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8817 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17002 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/conclusions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/inputdef.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.810191 hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/requires/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/requires/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/requires/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/requires/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.814191 hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/requires/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/requires/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8661 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/requires/types/apt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/requires/types/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/requires/types/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/requires/types/pebble.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/requires/types/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/requires/types/snap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/requires/types/systemd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/requires/types/varops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15726 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/vardef.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16022 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/ycheck/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/core/ycheck/scenarios.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.786191 hotsos-1.17.0.post9/hotsos/defs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.786191 hotsos-1.17.0.post9/hotsos/defs/events/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.814191 hotsos-1.17.0.post9/hotsos/defs/events/openstack/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/events/openstack/apache.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/events/openstack/apparmor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/events/openstack/http-requests.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.814191 hotsos-1.17.0.post9/hotsos/defs/events/openstack/neutron/
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/events/openstack/neutron/agents.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/events/openstack/neutron/ml2-routers.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.814191 hotsos-1.17.0.post9/hotsos/defs/events/openstack/nova/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/events/openstack/nova/external-events.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.814191 hotsos-1.17.0.post9/hotsos/defs/events/openstack/nova/migrations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.814191 hotsos-1.17.0.post9/hotsos/defs/events/openstack/nova/migrations/live-migration/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/events/openstack/nova/migrations/live-migration/dst-pre-live-migration.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/events/openstack/nova/migrations/live-migration/src-migration.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/events/openstack/nova/migrations/live-migration/src-post-live-migration.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/events/openstack/nova/migrations/migrations.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/events/openstack/nova/nova-compute.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/events/openstack/octavia.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.786191 hotsos-1.17.0.post9/hotsos/defs/events/openvswitch/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.814191 hotsos-1.17.0.post9/hotsos/defs/events/openvswitch/ovn/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/events/openvswitch/ovn/errors-and-warnings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/events/openvswitch/ovn/ovn-central.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/events/openvswitch/ovn/ovn-controller.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.814191 hotsos-1.17.0.post9/hotsos/defs/events/openvswitch/ovs/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/events/openvswitch/ovs/bfd.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/events/openvswitch/ovs/datapath-checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/events/openvswitch/ovs/errors-and-warnings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/events/openvswitch/ovs/ovs-vswitchd.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.786191 hotsos-1.17.0.post9/hotsos/defs/events/storage/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.786191 hotsos-1.17.0.post9/hotsos/defs/events/storage/ceph/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.818191 hotsos-1.17.0.post9/hotsos/defs/events/storage/ceph/mon/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/events/storage/ceph/mon/mon.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/events/storage/ceph/mon/monlogs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.818191 hotsos-1.17.0.post9/hotsos/defs/events/storage/ceph/osd/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/events/storage/ceph/osd/osd.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/events/storage/ceph/osd/osdlogs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.794191 hotsos-1.17.0.post9/hotsos/defs/scenarios/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.818191 hotsos-1.17.0.post9/hotsos/defs/scenarios/juju/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.818191 hotsos-1.17.0.post9/hotsos/defs/scenarios/juju/bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/juju/bugs/lp1812361.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/juju/bugs/lp1852502.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/juju/bugs/lp1858519.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/juju/bugs/lp1895040.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/juju/bugs/lp1910958.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/juju/bugs/lp1948906.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/juju/bugs/lp1983140.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/juju/bugs/lp1983506.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/juju/bugs/lp1996230.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/juju/charm_unit_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/juju/juju.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/juju/jujud_machine_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/juju/snap_channel.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.818191 hotsos-1.17.0.post9/hotsos/defs/scenarios/kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/kernel/amd_iommu_pt.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/kernel/disk_failure.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/kernel/kernlog_calltrace.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/kernel/memory.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.822191 hotsos-1.17.0.post9/hotsos/defs/scenarios/kernel/network/
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/kernel/network/misc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/kernel/network/netlink.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7336 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/kernel/network/tcp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/kernel/network/udp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/kernel/qla2xxx.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.822191 hotsos-1.17.0.post9/hotsos/defs/scenarios/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/kubernetes/kubernetes.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/kubernetes/system_cpufreq_mode.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.822191 hotsos-1.17.0.post9/hotsos/defs/scenarios/lxd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.822191 hotsos-1.17.0.post9/hotsos/defs/scenarios/lxd/bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/lxd/bugs/lp1807628.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/lxd/lxcfs_deadlock.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/lxd/snap_channel.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.822191 hotsos-1.17.0.post9/hotsos/defs/scenarios/maas/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/maas/maas_proxy_issue.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.822191 hotsos-1.17.0.post9/hotsos/defs/scenarios/mysql/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.822191 hotsos-1.17.0.post9/hotsos/defs/scenarios/mysql/bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/mysql/bugs/lp1959861.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/mysql/bugs/lp1971565.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/mysql/bugs/lp2039444.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/mysql/bugs/lp372017.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/mysql/mysql.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/mysql/mysql_connections.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.822191 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.790191 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/barbican/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.822191 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/barbican/bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/barbican/bugs/lp1946787.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.790191 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/cinder/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.822191 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/cinder/bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/cinder/bugs/lp2004555.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/eol.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.790191 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/keystone/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.822191 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/keystone/bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/keystone/bugs/lp1896125.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.822191 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/masakari/
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/masakari/pacemaker_remote.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.826191 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/neutron/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.826191 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/neutron/bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1794991.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1883089.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1896506.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1907686.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1927868.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1928031.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1929832.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1948466.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1960319.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1965297.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1979089.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1993628.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1996594.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/neutron/neutron_ovs_cleanup.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/neutron/oslo_privsep_errors.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/neutron/ovn_stale_db.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/neutron/ovndb_leader_bouncing.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.826191 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/nova/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.830191 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/nova/bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1761062.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1860743.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1888395.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1904580.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1944619.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1967956.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp2004555.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp2012284.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/nova/config_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/nova/cpu_pinning.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/nova/service_mem_usage.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.830191 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/octavia/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.830191 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/octavia/bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/octavia/bugs/lp2029857.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/octavia/bugs/sb1896125.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/octavia/excessive_failovers.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/octavia/hm_port_health.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/openstack.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/openstack_apache2_certificates.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/openstack_charm_conflicts.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.830191 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/openstack_charms/
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/openstack_charms/nova_cc_ssh_known_hosts_fail.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/pkgs_from_mixed_releases_found.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/system_cpufreq_mode.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/systemd_masked_services.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.830191 hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.830191 hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/bugs/lp1839592.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/bugs/lp1978806.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/dpif_lost_packets.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/dpif_resubmit_actions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/openvswitch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.830191 hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/ovn/
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/ovn/bfd_flapping.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.830191 hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/ovn/bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1865127.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1917475.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_certs_logs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_services.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_certs_valid.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_chassis_certs_logs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_elections.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_upgrades.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/ovn/ovsdb_reconnect_errors.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/ovn/service_mem_usage.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/service_restarts.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.830191 hotsos-1.17.0.post9/hotsos/defs/scenarios/pacemaker/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.834190 hotsos-1.17.0.post9/hotsos/defs/scenarios/pacemaker/bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/pacemaker/bugs/lp1874719.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/pacemaker/pacemaker.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.834190 hotsos-1.17.0.post9/hotsos/defs/scenarios/rabbitmq/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.834190 hotsos-1.17.0.post9/hotsos/defs/scenarios/rabbitmq/bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/rabbitmq/bugs/lp1943937.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/rabbitmq/cluster_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/rabbitmq/cluster_logchecks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/rabbitmq/cluster_resources.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/rabbitmq/rabbitmq.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.834190 hotsos-1.17.0.post9/hotsos/defs/scenarios/sosreport/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/sosreport/plugin_timeouts.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.834190 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.834190 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/bcache/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/bcache/bcache.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/bcache/bdev.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/bcache/cacheset.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.794191 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.834190 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mgr/
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mgr/autoscaler_overlap_roots.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.838190 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/auth_insecure_global_id_reclaim_allowed.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/autoscaler_bug.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_size.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_spillover.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph-mon.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_address_overlap.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_cluster_health.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_versions_mismatch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/crushmap_bucket_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/empty_clog.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/eol.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/laggy_pgs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/large_omap_objects.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/meta_backend_mon.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_db_too_big.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_elections_flapping.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_flapping.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_maps_backlog_too_large.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_messenger_v2_protocol.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_heartbeats.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_ops.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_unusual_raw.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_imbalance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_overdose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/required_osd_release_mismatch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/rgw_frontend.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ssds_using_bcache.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/unresponsive_mon_mgr.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.842190 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.842190 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1936136.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1959649.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1996010.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2013960.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2016845.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph-osd.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph_address_overlap.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/eol.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/filestore_to_bluestore_upgrade.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/juju_ceph_no_bcache_tuning.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/meta_backend_osd.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_flapping.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_latency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_slow_ops.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/pg_overdose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/ssd_osds_no_discard.yaml.disabled
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/system_cpufreq_mode.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.842190 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-rgw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.842190 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-rgw/bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-rgw/bugs/lp1974138.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-rgw/rgw_frontend_rgw.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.842190 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/common/ceph_charm_conflicts.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/storage.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.842190 hotsos-1.17.0.post9/hotsos/defs/scenarios/system/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/system/system.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/system/unattended_upgrades.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.842190 hotsos-1.17.0.post9/hotsos/defs/scenarios/vault/
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/defs/scenarios/vault/snap_channel.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.842190 hotsos-1.17.0.post9/hotsos/plugin_extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.842190 hotsos-1.17.0.post9/hotsos/plugin_extensions/juju/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/juju/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/juju/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.842190 hotsos-1.17.0.post9/hotsos/plugin_extensions/kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/kernel/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.842190 hotsos-1.17.0.post9/hotsos/plugin_extensions/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/kubernetes/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.842190 hotsos-1.17.0.post9/hotsos/plugin_extensions/lxd/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/lxd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/lxd/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.842190 hotsos-1.17.0.post9/hotsos/plugin_extensions/maas/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/maas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/maas/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.846190 hotsos-1.17.0.post9/hotsos/plugin_extensions/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/mysql/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.846190 hotsos-1.17.0.post9/hotsos/plugin_extensions/openstack/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/openstack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.846190 hotsos-1.17.0.post9/hotsos/plugin_extensions/openstack/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/openstack/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14382 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/openstack/agent/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/openstack/agent/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/openstack/nova_external_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/openstack/service_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/openstack/service_network_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/openstack/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/openstack/vm_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.846190 hotsos-1.17.0.post9/hotsos/plugin_extensions/openvswitch/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/openvswitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9596 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/openvswitch/event_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/openvswitch/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.846190 hotsos-1.17.0.post9/hotsos/plugin_extensions/pacemaker/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/pacemaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/pacemaker/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.846190 hotsos-1.17.0.post9/hotsos/plugin_extensions/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/rabbitmq/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.846190 hotsos-1.17.0.post9/hotsos/plugin_extensions/sosreport/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/sosreport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/sosreport/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.846190 hotsos-1.17.0.post9/hotsos/plugin_extensions/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/storage/bcache_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/storage/ceph_event_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/storage/ceph_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.850190 hotsos-1.17.0.post9/hotsos/plugin_extensions/system/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/system/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/system/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.850190 hotsos-1.17.0.post9/hotsos/plugin_extensions/vault/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/plugin_extensions/vault/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.850190 hotsos-1.17.0.post9/hotsos/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/templates/content_dict.html
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/templates/content_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/hotsos/templates/header.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:55:40.850190 hotsos-1.17.0.post9/hotsos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-09 08:55:40.000000 hotsos-1.17.0.post9/hotsos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16441 2024-04-09 08:55:40.000000 hotsos-1.17.0.post9/hotsos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 08:55:40.000000 hotsos-1.17.0.post9/hotsos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-09 08:55:40.000000 hotsos-1.17.0.post9/hotsos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-09 08:55:40.000000 hotsos-1.17.0.post9/hotsos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 08:55:40.000000 hotsos-1.17.0.post9/hotsos.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 08:55:40.850190 hotsos-1.17.0.post9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-09 08:55:25.000000 hotsos-1.17.0.post9/setup.py
```

### Comparing `hotsos-1.17.0.post8/LICENSE` & `hotsos-1.17.0.post9/LICENSE`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/PKG-INFO` & `hotsos-1.17.0.post9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hotsos
-Version: 1.17.0.post8
+Version: 1.17.0.post9
 Summary: Software analysis toolkit. Define checks in high-level language and leverage library to perform analysis of common Cloud applications.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: importlib-metadata; python_version >= "3.8"
 Requires-Dist: click
 Requires-Dist: cryptography
```

### Comparing `hotsos-1.17.0.post8/README.md` & `hotsos-1.17.0.post9/README.md`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/cli.py` & `hotsos-1.17.0.post9/hotsos/cli.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/client.py` & `hotsos-1.17.0.post9/hotsos/client.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/analytics.py` & `hotsos-1.17.0.post9/hotsos/core/analytics.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/config.py` & `hotsos-1.17.0.post9/hotsos/core/config.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/factory.py` & `hotsos-1.17.0.post9/hotsos/core/factory.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/host_helpers/__init__.py` & `hotsos-1.17.0.post9/hotsos/core/host_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/host_helpers/apparmor.py` & `hotsos-1.17.0.post9/hotsos/core/host_helpers/apparmor.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/host_helpers/cli.py` & `hotsos-1.17.0.post9/hotsos/core/host_helpers/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,19 @@
 
         return catch_exceptions_inner2
 
     return catch_exceptions_inner1
 
 
 class SourceNotFound(Exception):
-    pass
+    def __init__(self, path):
+        self.path = path
+
+    def __repr__(self):
+        return "source path '{}' not found".format(self.path)
 
 
 class CommandNotFound(Exception):
     def __init__(self, cmd, msg):
         self.msg = "command '{}' not found in catalog: '{}'".format(cmd, msg)
 
     def __str__(self):
@@ -235,15 +239,15 @@
         if args:
             self.path = self.path.format(*args)
 
         if kwargs:
             self.path = self.path.format(**kwargs)
 
         if not os.path.exists(self.path):
-            raise SourceNotFound()
+            raise SourceNotFound(self.path)
 
         if skip_load_contents:
             CmdOutput(None, self.path)
 
         # NOTE: any post-exec hooks must be aware that their input will be
         # defined by the following.
         if self.json_decode:
@@ -289,15 +293,15 @@
     @reset_command
     @run_post_exec_hooks
     @run_pre_exec_hooks
     def __call__(self, *args, **kwargs):
         # TODO: find a better way to handle this because path may still need
         # formatting.
         if not os.path.exists(self.original_path):
-            raise SourceNotFound()
+            raise SourceNotFound(self.original_path)
 
         if args:
             self.path = self.path.format(*args)
 
         if kwargs:
             self.path = self.path.format(**kwargs)
 
@@ -371,57 +375,101 @@
 
         if kwargs.get("date"):
             self.path = "{} --since {}".format(self.path, kwargs.get("date"))
         else:
             self.path = "{} --since {}".format(self.path, self.since_date)
 
 
-class OVSDPCTLFileCmd(FileCmd):
+class OVSAppCtlFileCmd(FileCmd):
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.register_hook("pre-exec", self.performat_sos_datapath)
+    def __call__(self, *args, **kwargs):
+        for key in ['flags', 'args']:
+            if key in kwargs:
+                kwargs[key] = '_{}'.format(kwargs[key])
+            else:
+                kwargs[key] = ''
+
+        if 'args' in kwargs and kwargs['command'].startswith('dpctl/'):
+            # e.g. this would be for dpctl datapath
+            kwargs['args'] = kwargs['args'].replace('@', '_')
 
-    def performat_sos_datapath(self, **kwargs):
-        if 'datapath' in kwargs:
-            datapath = kwargs['datapath'].replace('@', '_')
-            self.path = self.path.format(datapath=datapath)
+        kwargs['command'] = kwargs['command'].replace('/', '.')
+        try:
+            out = super().__call__(*args, **kwargs)
+        except SourceNotFound:
+            log.debug("%s: source not found: %s", self.__class__.__name__,
+                      self.path)
+            raise
+
+        return out
 
 
-class OVSOFCTLBinCmd(BinCmd):
+class OVSOFCtlCmdBase(object):
     OFPROTOCOL_VERSIONS = ['OpenFlow15', 'OpenFlow14', 'OpenFlow13',
                            'OpenFlow12', 'OpenFlow11', 'OpenFlow10']
 
+
+class OVSOFCtlBinCmd(OVSOFCtlCmdBase, BinCmd):
+
     def __call__(self, *args, **kwargs):
         """
-        First try without specifying protocol version then is error is raised
-        try with version.
+        First try without specifying protocol version. If error is raised
+        try with different versions until we get a result.
         """
         self.cmd = "ovs-ofctl {}".format(self.cmd)
         try:
             return super().__call__(*args, **kwargs)
         except CLIExecError:
-            log.debug("ofctl command with no protocol version failed")
+            log.debug("%s: command with no protocol version failed",
+                      self.__class__.__name__)
 
         # If the command raised an exception it will have been caught by the
         # catch_exceptions decorator and [] returned. We have no way of knowing
         # if that was the actual return or an exception was raised so we just
         # go ahead and retry with specific OF versions until we get a result.
         for ver in self.OFPROTOCOL_VERSIONS:
-            log.debug("trying ofctl command with protocol version %s", ver)
+            log.debug("%s: trying again with protocol version %s",
+                      self.__class__.__name__, ver)
             self.reset()
             self.cmd = "ovs-ofctl -O {} {}".format(ver, self.cmd)
             try:
                 return super().__call__(*args, **kwargs)
             except CLIExecError:
-                log.debug("ofctl command with protocol version %s failed", ver)
+                log.debug("%s: command with protocol version %s failed",
+                          self.__class__.__name__, ver)
 
         return CmdOutput([])
 
 
+class OVSOFCtlFileCmd(OVSOFCtlCmdBase, FileCmd):
+
+    def __call__(self, *args, **kwargs):
+        """
+        First try without specifying protocol version. If error is raised
+        try with different versions until we get a result.
+        """
+        try:
+            kwargs['ofversion'] = ''
+            return super().__call__(*args, **kwargs)
+        except SourceNotFound:
+            log.debug("%s: command with no protocol version failed",
+                      self.__class__.__name__)
+
+        for ver in self.OFPROTOCOL_VERSIONS:
+            log.debug("%s: trying again with protocol version %s",
+                      self.__class__.__name__, ver)
+            self.reset()
+            try:
+                kwargs['ofversion'] = '_-O_{}'.format(ver)
+                return super().__call__(*args, **kwargs)
+            except SourceNotFound:
+                if ver == self.OFPROTOCOL_VERSIONS[-1]:
+                    raise
+
+
 class DateBinCmd(BinCmd):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.register_hook("pre-exec", self.format_date_cmd)
 
     def format_date_cmd(self, **kwargs):
@@ -499,15 +547,15 @@
             self.register_hook('post-exec', self.cleanup)
             self.orig_path = None
             self.first_line_filter = first_line_filter
             self.last_line_filter = last_line_filter
 
     def format_json_contents(self, *args, **kwargs):  # pylint: disable=W0613
         if not os.path.exists(self.path):
-            raise SourceNotFound
+            raise SourceNotFound(self.path)
 
         with open(self.path) as f:
             lines = f.readlines()
 
         if self.first_line_filter:
             line_filter = self.first_line_filter
         else:
@@ -911,46 +959,25 @@
                         singleline=True),
                  FileCmd('sos_commands/openvswitch/ovs-vsctl_-t_5_get_'
                          '{table}_{record}_{column}', singleline=True)],
             'ovs_vsctl_list':
                 [BinCmd('ovs-vsctl list {table}'),
                  FileCmd('sos_commands/openvswitch/'
                          'ovs-vsctl_-t_5_list_{table}')],
-            'ovs_appctl_dpctl_show':
-                [BinCmd('ovs-appctl dpctl/show -s {datapath}'),
-                 OVSDPCTLFileCmd('sos_commands/openvswitch/'
-                                 'ovs-appctl_dpctl.show_-s_{datapath}')],
-            'ovs_appctl_dpctl_dump_conntrack':
-                [BinCmd('ovs-appctl dpctl/dump-conntrack -m {datapath}'),
-                 OVSDPCTLFileCmd(
-                            'sos_commands/openvswitch/'
-                            'ovs-appctl_dpctl.dump-conntrack_-m_{datapath}')],
-            'ovs_appctl_ofproto_list_tunnels':
-                [BinCmd('ovs-appctl ofproto/list-tunnels'),
-                 OVSDPCTLFileCmd('sos_commands/openvswitch/'
-                                 'ovs-appctl_ofproto.list-tunnels')],
             'ovs_vsctl_list_br':
                 [BinCmd('ovs-vsctl list-br'),
                  FileCmd('sos_commands/openvswitch/ovs-vsctl_-t_5_list-br')],
-            'ovs_ofctl_show':
-                [OVSOFCTLBinCmd('show {bridge}'),
-                 FileCmd('sos_commands/openvswitch/'
-                         'ovs-ofctl_-O_OpenFlow15_show_{bridge}'),
-                 FileCmd('sos_commands/openvswitch/'
-                         'ovs-ofctl_-O_OpenFlow14_show_{bridge}'),
-                 FileCmd('sos_commands/openvswitch/'
-                         'ovs-ofctl_-O_OpenFlow13_show_{bridge}'),
-                 FileCmd('sos_commands/openvswitch/'
-                         'ovs-ofctl_-O_OpenFlow12_show_{bridge}'),
-                 FileCmd('sos_commands/openvswitch/'
-                         'ovs-ofctl_-O_OpenFlow11_show_{bridge}'),
-                 FileCmd('sos_commands/openvswitch/'
-                         'ovs-ofctl_-O_OpenFlow10_show_{bridge}'),
-                 FileCmd('sos_commands/openvswitch/'
-                         'ovs-ofctl_show_{bridge}')],
+            'ovs_appctl':
+                [BinCmd('ovs-appctl {command} {flags} {args}'),
+                 OVSAppCtlFileCmd('sos_commands/openvswitch/ovs-appctl_'
+                                  '{command}{flags}{args}')],
+            'ovs_ofctl':
+                [OVSOFCtlBinCmd('{command} {args}'),
+                 OVSOFCtlFileCmd('sos_commands/openvswitch/'
+                                 'ovs-ofctl{ofversion}_{command}_{args}')],
             'pacemaker_crm_status':
                 [BinCmd('crm status'),
                  FileCmd('sos_commands/pacemaker/crm_status')],
             'pebble_services':
                 [BinCmd('pebble services'),
                  # This is how operator charms run it
                  BinCmd('/charm/bin/pebble services'),
```

### Comparing `hotsos-1.17.0.post8/hotsos/core/host_helpers/common.py` & `hotsos-1.17.0.post9/hotsos/core/host_helpers/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/host_helpers/config.py` & `hotsos-1.17.0.post9/hotsos/core/host_helpers/config.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/host_helpers/filestat.py` & `hotsos-1.17.0.post9/hotsos/core/host_helpers/filestat.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/host_helpers/network.py` & `hotsos-1.17.0.post9/hotsos/core/host_helpers/network.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/host_helpers/packaging.py` & `hotsos-1.17.0.post9/hotsos/core/host_helpers/packaging.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/host_helpers/pebble.py` & `hotsos-1.17.0.post9/hotsos/core/host_helpers/pebble.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/host_helpers/ssl.py` & `hotsos-1.17.0.post9/hotsos/core/host_helpers/ssl.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/host_helpers/sysctl.py` & `hotsos-1.17.0.post9/hotsos/core/host_helpers/sysctl.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/host_helpers/systemd.py` & `hotsos-1.17.0.post9/hotsos/core/host_helpers/systemd.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/host_helpers/uptime.py` & `hotsos-1.17.0.post9/hotsos/core/host_helpers/uptime.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/issues/issue_types.py` & `hotsos-1.17.0.post9/hotsos/core/issues/issue_types.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/issues/utils.py` & `hotsos-1.17.0.post9/hotsos/core/issues/utils.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/log.py` & `hotsos-1.17.0.post9/hotsos/core/log.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/plugins/juju/common.py` & `hotsos-1.17.0.post9/hotsos/core/plugins/juju/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/plugins/juju/resources.py` & `hotsos-1.17.0.post9/hotsos/core/plugins/juju/resources.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/plugins/kernel/common.py` & `hotsos-1.17.0.post9/hotsos/core/plugins/kernel/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/plugins/kernel/config.py` & `hotsos-1.17.0.post9/hotsos/core/plugins/kernel/config.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/plugins/kernel/kernlog/calltrace.py` & `hotsos-1.17.0.post9/hotsos/core/plugins/kernel/kernlog/calltrace.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/plugins/kernel/kernlog/common.py` & `hotsos-1.17.0.post9/hotsos/core/plugins/kernel/kernlog/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/plugins/kernel/kernlog/events.py` & `hotsos-1.17.0.post9/hotsos/core/plugins/kernel/kernlog/events.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/plugins/kernel/memory.py` & `hotsos-1.17.0.post9/hotsos/core/plugins/kernel/memory.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/plugins/kernel/net.py` & `hotsos-1.17.0.post9/hotsos/core/plugins/kernel/net.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/plugins/kernel/sysfs.py` & `hotsos-1.17.0.post9/hotsos/core/plugins/kernel/sysfs.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/plugins/kubernetes.py` & `hotsos-1.17.0.post9/hotsos/core/plugins/kubernetes.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/plugins/lxd/common.py` & `hotsos-1.17.0.post9/hotsos/core/plugins/lxd/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/plugins/maas.py` & `hotsos-1.17.0.post9/hotsos/core/plugins/maas.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/plugins/mysql.py` & `hotsos-1.17.0.post9/hotsos/core/plugins/mysql.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/plugins/openstack/common.py` & `hotsos-1.17.0.post9/hotsos/core/plugins/openstack/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/plugins/openstack/exceptions.py` & `hotsos-1.17.0.post9/hotsos/core/plugins/openstack/exceptions.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/plugins/openstack/neutron.py` & `hotsos-1.17.0.post9/hotsos/core/plugins/openstack/neutron.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/plugins/openstack/nova.py` & `hotsos-1.17.0.post9/hotsos/core/plugins/openstack/nova.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/plugins/openstack/octavia.py` & `hotsos-1.17.0.post9/hotsos/core/plugins/openstack/octavia.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/plugins/openstack/openstack.py` & `hotsos-1.17.0.post9/hotsos/core/plugins/openstack/openstack.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/plugins/openvswitch/common.py` & `hotsos-1.17.0.post9/hotsos/core/plugins/openvswitch/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/plugins/openvswitch/ovn.py` & `hotsos-1.17.0.post9/hotsos/core/plugins/openvswitch/ovn.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/plugins/openvswitch/ovs.py` & `hotsos-1.17.0.post9/hotsos/core/plugins/openvswitch/ovs.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,15 +78,16 @@
         return OVSDBTable(table)
 
 
 class OVSDPLookups(object):
 
     def __init__(self):
         cli = CLIHelper()
-        out = cli.ovs_appctl_dpctl_show(datapath='system@ovs-system')
+        out = cli.ovs_appctl(command='dpctl/show', flags='-s',
+                             args='system@ovs-system')
         cexpr = re.compile(r'\s*lookups: hit:(\S+) missed:(\S+) lost:(\S+)')
         self.fields = {'hit': 0, 'missed': 0, 'lost': 0}
         for line in out:
             ret = re.match(cexpr, line)
             if ret:
                 self.fields['hit'] = int(ret.group(1))
                 self.fields['missed'] = int(ret.group(2))
@@ -103,15 +104,15 @@
         self.name = name
         self.cli = CLIHelper()
         self.nethelper = nethelper
 
     @cached_property
     def ports(self):
         ports = []
-        for line in self.cli.ovs_ofctl_show(bridge=self.name):
+        for line in self.cli.ovs_ofctl(command='show', args=self.name):
             ret = re.compile(r'^\s+\d+\((\S+)\):\s+').match(line)
             if ret:
                 name = ret.group(1)
                 port = self.nethelper.get_interface_with_name(name)
                 if not port:
                     port = name
 
@@ -146,15 +147,15 @@
                 tunnel_info[proto] = {'local': local_addr}
 
         nethelp = HostNetworkingHelper()
         with CLIHelperFile() as cli:
             s = FileSearcher()
             expr = r'.+ \(([a-z]+): ([a-f\d\.:]+)->([a-f\d\.:]+), .+'
             s.add(SearchDef(expr, tag='all'),
-                  cli.ovs_appctl_ofproto_list_tunnels())
+                  cli.ovs_appctl(command='ofproto/list-tunnels'))
             results = s.run()
             for r in results.find_by_tag('all'):
                 proto = r.get(1)
                 if proto not in tunnel_info:
                     tunnel_info[proto] = {}
 
                 if 'remotes' not in tunnel_info[proto]:
```

### Comparing `hotsos-1.17.0.post8/hotsos/core/plugins/pacemaker.py` & `hotsos-1.17.0.post9/hotsos/core/plugins/pacemaker.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/plugins/rabbitmq/common.py` & `hotsos-1.17.0.post9/hotsos/core/plugins/rabbitmq/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/plugins/rabbitmq/report.py` & `hotsos-1.17.0.post9/hotsos/core/plugins/rabbitmq/report.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/plugins/sosreport.py` & `hotsos-1.17.0.post9/hotsos/core/plugins/sosreport.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/plugins/storage/bcache.py` & `hotsos-1.17.0.post9/hotsos/core/plugins/storage/bcache.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/plugins/storage/ceph.py` & `hotsos-1.17.0.post9/hotsos/core/plugins/storage/ceph.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/plugins/system/system.py` & `hotsos-1.17.0.post9/hotsos/core/plugins/system/system.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/plugins/vault.py` & `hotsos-1.17.0.post9/hotsos/core/plugins/vault.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/plugintools.py` & `hotsos-1.17.0.post9/hotsos/core/plugintools.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/root_manager.py` & `hotsos-1.17.0.post9/hotsos/core/root_manager.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/search.py` & `hotsos-1.17.0.post9/hotsos/core/search.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/utils.py` & `hotsos-1.17.0.post9/hotsos/core/utils.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/ycheck/engine/common.py` & `hotsos-1.17.0.post9/hotsos/core/ycheck/engine/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/checks.py` & `hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/checks.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/common.py` & `hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/conclusions.py` & `hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/conclusions.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/inputdef.py` & `hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/inputdef.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/requires/common.py` & `hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/requires/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/requires/requires.py` & `hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/requires/requires.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/requires/types/apt.py` & `hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/requires/types/apt.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/requires/types/config.py` & `hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/requires/types/config.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/requires/types/path.py` & `hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/requires/types/path.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/requires/types/pebble.py` & `hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/requires/types/pebble.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/requires/types/property.py` & `hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/requires/types/property.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/requires/types/snap.py` & `hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/requires/types/snap.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/requires/types/systemd.py` & `hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/requires/types/systemd.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/requires/types/varops.py` & `hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/requires/types/varops.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/search.py` & `hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/search.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/ycheck/engine/properties/vardef.py` & `hotsos-1.17.0.post9/hotsos/core/ycheck/engine/properties/vardef.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/ycheck/events.py` & `hotsos-1.17.0.post9/hotsos/core/ycheck/events.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/core/ycheck/scenarios.py` & `hotsos-1.17.0.post9/hotsos/core/ycheck/scenarios.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/events/openstack/apparmor.yaml` & `hotsos-1.17.0.post9/hotsos/defs/events/openstack/apparmor.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/events/openstack/neutron/agents.yaml` & `hotsos-1.17.0.post9/hotsos/defs/events/openstack/neutron/agents.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/events/openstack/nova/external-events.yaml` & `hotsos-1.17.0.post9/hotsos/defs/events/openstack/nova/external-events.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/events/openstack/octavia.yaml` & `hotsos-1.17.0.post9/hotsos/defs/events/openstack/octavia.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/events/openvswitch/ovn/errors-and-warnings.yaml` & `hotsos-1.17.0.post9/hotsos/defs/events/openvswitch/ovn/errors-and-warnings.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/events/openvswitch/ovn/ovn-central.yaml` & `hotsos-1.17.0.post9/hotsos/defs/events/openvswitch/ovn/ovn-central.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/events/openvswitch/ovn/ovn-controller.yaml` & `hotsos-1.17.0.post9/hotsos/defs/events/openvswitch/ovn/ovn-controller.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/events/openvswitch/ovs/datapath-checks.yaml` & `hotsos-1.17.0.post9/hotsos/defs/events/openvswitch/ovs/datapath-checks.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 input:
-  command: ovs_appctl_dpctl_show
+  command: ovs_appctl
   options:
     kwargs:
-      datapath: 'system@ovs-system'
+      command: dpctl/show
+      flags: '-s'
+      args: 'system@ovs-system'
 port-stats:
   start: '\s+port \d+: (\S+)'
   body: '\s+([RT]X) \S+:(\d+) \S+:(\d+) \S+:(\d+) \S+:(\d+) \S+:(\d+)'
 deferred-action-limit-reached:
   input:
     path: 'var/log/kern.log'
   # NOTE: the kern.log timestamp pattern is of the form
```

### Comparing `hotsos-1.17.0.post8/hotsos/defs/events/openvswitch/ovs/ovs-vswitchd.yaml` & `hotsos-1.17.0.post9/hotsos/defs/events/openvswitch/ovs/ovs-vswitchd.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/events/storage/ceph/mon/monlogs.yaml` & `hotsos-1.17.0.post9/hotsos/defs/events/storage/ceph/mon/monlogs.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/events/storage/ceph/osd/osdlogs.yaml` & `hotsos-1.17.0.post9/hotsos/defs/events/storage/ceph/osd/osdlogs.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/juju/bugs/lp1812361.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/juju/bugs/lp1812361.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/juju/bugs/lp1852502.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/juju/bugs/lp1852502.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/juju/bugs/lp1858519.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/juju/bugs/lp1858519.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/juju/bugs/lp1895040.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/juju/bugs/lp1895040.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/juju/bugs/lp1910958.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/juju/bugs/lp1910958.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/juju/bugs/lp1948906.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/juju/bugs/lp1948906.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/juju/bugs/lp1996230.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/juju/bugs/lp1996230.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/juju/charm_unit_checks.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/juju/charm_unit_checks.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/juju/snap_channel.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/juju/snap_channel.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/kernel/amd_iommu_pt.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/kernel/amd_iommu_pt.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/kernel/disk_failure.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/kernel/disk_failure.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/kernel/kernlog_calltrace.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/kernel/kernlog_calltrace.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/kernel/memory.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/kernel/memory.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/kernel/network/misc.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/kernel/network/misc.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/kernel/network/netlink.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/kernel/network/netlink.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/kernel/network/tcp.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/kernel/network/tcp.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/kernel/network/udp.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/kernel/network/udp.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/kernel/qla2xxx.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/kernel/qla2xxx.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/kubernetes/system_cpufreq_mode.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/kubernetes/system_cpufreq_mode.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/lxd/bugs/lp1807628.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/lxd/bugs/lp1807628.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/lxd/lxcfs_deadlock.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/lxd/lxcfs_deadlock.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/lxd/snap_channel.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/lxd/snap_channel.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/maas/maas_proxy_issue.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/maas/maas_proxy_issue.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/mysql/bugs/lp1959861.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/mysql/bugs/lp1959861.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/mysql/bugs/lp1971565.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/mysql/bugs/lp1971565.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/mysql/bugs/lp2039444.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/mysql/bugs/lp2039444.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/mysql/mysql_connections.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/mysql/mysql_connections.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/barbican/bugs/lp1946787.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/barbican/bugs/lp1946787.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/cinder/bugs/lp2004555.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/cinder/bugs/lp2004555.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/eol.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/eol.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/keystone/bugs/lp1896125.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/keystone/bugs/lp1896125.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/masakari/pacemaker_remote.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/masakari/pacemaker_remote.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1794991.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1794991.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1896506.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1896506.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1907686.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1907686.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1927868.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1927868.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1948466.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1948466.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1960319.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1960319.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1979089.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1979089.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1993628.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1993628.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1996594.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1996594.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/neutron/neutron_ovs_cleanup.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/neutron/neutron_ovs_cleanup.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/neutron/oslo_privsep_errors.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/neutron/oslo_privsep_errors.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/neutron/ovn_stale_db.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/neutron/ovn_stale_db.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/neutron/ovndb_leader_bouncing.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/neutron/ovndb_leader_bouncing.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp1761062.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1761062.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp1860743.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1860743.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp1888395.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1888395.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp1904580.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1904580.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp1967956.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1967956.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp2004555.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp2004555.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp2012284.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp2012284.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/nova/config_checks.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/nova/config_checks.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/nova/cpu_pinning.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/nova/cpu_pinning.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/nova/service_mem_usage.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/nova/service_mem_usage.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/octavia/bugs/lp2029857.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/octavia/bugs/lp2029857.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/octavia/bugs/sb1896125.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/octavia/bugs/sb1896125.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/octavia/excessive_failovers.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/octavia/excessive_failovers.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/octavia/hm_port_health.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/octavia/hm_port_health.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/openstack_apache2_certificates.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/openstack_apache2_certificates.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/openstack_charm_conflicts.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/openstack_charm_conflicts.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/openstack_charms/nova_cc_ssh_known_hosts_fail.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/openstack_charms/nova_cc_ssh_known_hosts_fail.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/system_cpufreq_mode.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/system_cpufreq_mode.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openstack/systemd_masked_services.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openstack/systemd_masked_services.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/bugs/lp1839592.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/bugs/lp1839592.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/bugs/lp1978806.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/bugs/lp1978806.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 input:
-  command: ovs_appctl_dpctl_dump_conntrack
+  command: ovs_appctl
   options:
     kwargs:
-      datapath: 'system@ovs-system'
+      command: dpctl/dump-conntrack
+      flags: '-m'
+      args: 'system@ovs-system'
 checks:
   # NOTE: we don't extract any info from the following searches so they define the smallest group possible so as to minimise saved data.
   ovs_using_geneve:
     input:
-      command: ovs_appctl_ofproto_list_tunnels
+      command: ovs_appctl
+      options:
+        kwargs:
+          command: ofproto/list-tunnels
     search: '.+ \((g)eneve:'
   ovs_using_vxlan:
     input:
-      command: ovs_appctl_ofproto_list_tunnels
+      command: ovs_appctl
+      options:
+        kwargs:
+          command: ofproto/list-tunnels
     search: '.+ \((v)xlan:'
   geneve_is_tracked:
     search: '^(u)dp,.+,sport=6081,'
   vxlan_is_tracked:
     search: '^(u)dp,.+,sport=4789,'
 conclusions:
   ovs_ct_tunnels:
```

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/dpif_lost_packets.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/dpif_lost_packets.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/dpif_resubmit_actions.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/dpif_resubmit_actions.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/ovn/bfd_flapping.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/ovn/bfd_flapping.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1865127.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1865127.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_certs_logs.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_certs_logs.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_services.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_services.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_certs_valid.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_certs_valid.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_chassis_certs_logs.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_chassis_certs_logs.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_elections.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_elections.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_upgrades.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_upgrades.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/ovn/ovsdb_reconnect_errors.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/ovn/ovsdb_reconnect_errors.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/ovn/service_mem_usage.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/ovn/service_mem_usage.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/openvswitch/service_restarts.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/openvswitch/service_restarts.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/pacemaker/bugs/lp1874719.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/pacemaker/bugs/lp1874719.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/rabbitmq/bugs/lp1943937.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/rabbitmq/bugs/lp1943937.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/rabbitmq/cluster_config.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/rabbitmq/cluster_config.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/rabbitmq/cluster_logchecks.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/rabbitmq/cluster_logchecks.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/rabbitmq/cluster_resources.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/rabbitmq/cluster_resources.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/sosreport/plugin_timeouts.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/sosreport/plugin_timeouts.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/bcache/bdev.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/bcache/bdev.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/bcache/cacheset.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/bcache/cacheset.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mgr/autoscaler_overlap_roots.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mgr/autoscaler_overlap_roots.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/auth_insecure_global_id_reclaim_allowed.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/auth_insecure_global_id_reclaim_allowed.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/autoscaler_bug.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/autoscaler_bug.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_size.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_size.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_spillover.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_spillover.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph-mon.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph-mon.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_address_overlap.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_address_overlap.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_cluster_health.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_cluster_health.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_versions_mismatch.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_versions_mismatch.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/crushmap_bucket_checks.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/crushmap_bucket_checks.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/empty_clog.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/empty_clog.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/eol.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/eol.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/laggy_pgs.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/laggy_pgs.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/large_omap_objects.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/large_omap_objects.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/meta_backend_mon.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/meta_backend_mon.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_db_too_big.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_db_too_big.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_elections_flapping.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_elections_flapping.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_flapping.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_flapping.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_maps_backlog_too_large.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_maps_backlog_too_large.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_messenger_v2_protocol.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_messenger_v2_protocol.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_heartbeats.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_heartbeats.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_ops.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_ops.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_unusual_raw.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_unusual_raw.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_imbalance.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_imbalance.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_overdose.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_overdose.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/required_osd_release_mismatch.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/required_osd_release_mismatch.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/rgw_frontend.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/rgw_frontend.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/ssds_using_bcache.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ssds_using_bcache.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/unresponsive_mon_mgr.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/unresponsive_mon_mgr.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1936136.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1936136.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1959649.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1959649.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1996010.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1996010.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2013960.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2013960.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2016845.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2016845.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph_address_overlap.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph_address_overlap.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/eol.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/eol.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/filestore_to_bluestore_upgrade.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/filestore_to_bluestore_upgrade.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/juju_ceph_no_bcache_tuning.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/juju_ceph_no_bcache_tuning.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/meta_backend_osd.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/meta_backend_osd.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_flapping.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_flapping.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_latency.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_latency.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_slow_ops.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_slow_ops.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/pg_overdose.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/pg_overdose.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/ssd_osds_no_discard.yaml.disabled` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/ssd_osds_no_discard.yaml.disabled`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/system_cpufreq_mode.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/system_cpufreq_mode.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-rgw/bugs/lp1974138.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-rgw/bugs/lp1974138.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/ceph-rgw/rgw_frontend_rgw.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/ceph-rgw/rgw_frontend_rgw.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/storage/ceph/common/ceph_charm_conflicts.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/storage/ceph/common/ceph_charm_conflicts.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/defs/scenarios/vault/snap_channel.yaml` & `hotsos-1.17.0.post9/hotsos/defs/scenarios/vault/snap_channel.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/plugin_extensions/juju/summary.py` & `hotsos-1.17.0.post9/hotsos/plugin_extensions/juju/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/plugin_extensions/kernel/summary.py` & `hotsos-1.17.0.post9/hotsos/plugin_extensions/kernel/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/plugin_extensions/kubernetes/summary.py` & `hotsos-1.17.0.post9/hotsos/plugin_extensions/kubernetes/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/plugin_extensions/lxd/summary.py` & `hotsos-1.17.0.post9/hotsos/plugin_extensions/lxd/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/plugin_extensions/openstack/agent/events.py` & `hotsos-1.17.0.post9/hotsos/plugin_extensions/openstack/agent/events.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/plugin_extensions/openstack/agent/exceptions.py` & `hotsos-1.17.0.post9/hotsos/plugin_extensions/openstack/agent/exceptions.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/plugin_extensions/openstack/nova_external_events.py` & `hotsos-1.17.0.post9/hotsos/plugin_extensions/openstack/nova_external_events.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/plugin_extensions/openstack/service_features.py` & `hotsos-1.17.0.post9/hotsos/plugin_extensions/openstack/service_features.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/plugin_extensions/openstack/service_network_checks.py` & `hotsos-1.17.0.post9/hotsos/plugin_extensions/openstack/service_network_checks.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/plugin_extensions/openstack/summary.py` & `hotsos-1.17.0.post9/hotsos/plugin_extensions/openstack/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/plugin_extensions/openstack/vm_info.py` & `hotsos-1.17.0.post9/hotsos/plugin_extensions/openstack/vm_info.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/plugin_extensions/openvswitch/event_checks.py` & `hotsos-1.17.0.post9/hotsos/plugin_extensions/openvswitch/event_checks.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/plugin_extensions/openvswitch/summary.py` & `hotsos-1.17.0.post9/hotsos/plugin_extensions/openvswitch/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/plugin_extensions/pacemaker/summary.py` & `hotsos-1.17.0.post9/hotsos/plugin_extensions/pacemaker/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/plugin_extensions/rabbitmq/summary.py` & `hotsos-1.17.0.post9/hotsos/plugin_extensions/rabbitmq/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/plugin_extensions/storage/bcache_summary.py` & `hotsos-1.17.0.post9/hotsos/plugin_extensions/storage/bcache_summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/plugin_extensions/storage/ceph_event_checks.py` & `hotsos-1.17.0.post9/hotsos/plugin_extensions/storage/ceph_event_checks.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/plugin_extensions/storage/ceph_summary.py` & `hotsos-1.17.0.post9/hotsos/plugin_extensions/storage/ceph_summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/plugin_extensions/system/checks.py` & `hotsos-1.17.0.post9/hotsos/plugin_extensions/system/checks.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/plugin_extensions/system/summary.py` & `hotsos-1.17.0.post9/hotsos/plugin_extensions/system/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos/templates/header.html` & `hotsos-1.17.0.post9/hotsos/templates/header.html`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/hotsos.egg-info/PKG-INFO` & `hotsos-1.17.0.post9/hotsos.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hotsos
-Version: 1.17.0.post8
+Version: 1.17.0.post9
 Summary: Software analysis toolkit. Define checks in high-level language and leverage library to perform analysis of common Cloud applications.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: importlib-metadata; python_version >= "3.8"
 Requires-Dist: click
 Requires-Dist: cryptography
```

### Comparing `hotsos-1.17.0.post8/hotsos.egg-info/SOURCES.txt` & `hotsos-1.17.0.post9/hotsos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hotsos-1.17.0.post8/pyproject.toml` & `hotsos-1.17.0.post9/pyproject.toml`

 * *Files identical despite different names*

