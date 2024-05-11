# Comparing `tmp/types-docker-7.0.0.20240507.tar.gz` & `tmp/types-docker-7.0.0.20240511.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-docker-7.0.0.20240507.tar", last modified: Tue May  7 02:25:17 2024, max compression
+gzip compressed data, was "types-docker-7.0.0.20240511.tar", last modified: Sat May 11 02:18:14 2024, max compression
```

## Comparing `types-docker-7.0.0.20240507.tar` & `types-docker-7.0.0.20240511.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:25:17.018967 types-docker-7.0.0.20240507/
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-07 02:25:15.000000 types-docker-7.0.0.20240507/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-07 02:25:15.000000 types-docker-7.0.0.20240507/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-07 02:25:17.018967 types-docker-7.0.0.20240507/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:25:17.006966 types-docker-7.0.0.20240507/docker-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-07 02:25:15.000000 types-docker-7.0.0.20240507/docker-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:25:17.010966 types-docker-7.0.0.20240507/docker-stubs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/api/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/api/build.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/api/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/api/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/api/container.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/api/daemon.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/api/exec_api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/api/image.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/api/network.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/api/plugin.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/api/secret.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/api/service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/api/swarm.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/api/volume.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/auth.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/constants.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:25:17.010966 types-docker-7.0.0.20240507/docker-stubs/context/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/context/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/context/api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/context/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/context/context.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:25:17.010966 types-docker-7.0.0.20240507/docker-stubs/credentials/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/credentials/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/credentials/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/credentials/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/credentials/store.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/credentials/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/errors.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:25:17.014967 types-docker-7.0.0.20240507/docker-stubs/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/models/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/models/configs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/models/containers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/models/images.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/models/networks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/models/nodes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/models/plugins.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/models/resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/models/secrets.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/models/services.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/models/swarm.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/models/volumes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:25:15.000000 types-docker-7.0.0.20240507/docker-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/tls.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:25:17.014967 types-docker-7.0.0.20240507/docker-stubs/transport/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/transport/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/transport/basehttpadapter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/transport/npipeconn.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/transport/npipesocket.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/transport/sshconn.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/transport/unixconn.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:25:17.014967 types-docker-7.0.0.20240507/docker-stubs/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/types/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/types/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/types/containers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/types/daemon.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/types/healthcheck.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/types/networks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/types/services.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/types/swarm.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:25:17.018967 types-docker-7.0.0.20240507/docker-stubs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/utils/build.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/utils/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/utils/decorators.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/utils/fnmatch.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/utils/json_stream.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/utils/ports.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/utils/proxy.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/utils/socket.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/utils/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 02:25:05.000000 types-docker-7.0.0.20240507/docker-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 02:25:17.018967 types-docker-7.0.0.20240507/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-07 02:25:15.000000 types-docker-7.0.0.20240507/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:25:17.018967 types-docker-7.0.0.20240507/types_docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-07 02:25:16.000000 types-docker-7.0.0.20240507/types_docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-07 02:25:16.000000 types-docker-7.0.0.20240507/types_docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 02:25:16.000000 types-docker-7.0.0.20240507/types_docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-07 02:25:16.000000 types-docker-7.0.0.20240507/types_docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 02:25:16.000000 types-docker-7.0.0.20240507/types_docker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:14.462194 types-docker-7.0.0.20240511/
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-11 02:18:13.000000 types-docker-7.0.0.20240511/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-11 02:18:13.000000 types-docker-7.0.0.20240511/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-11 02:18:14.462194 types-docker-7.0.0.20240511/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:14.454193 types-docker-7.0.0.20240511/docker-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-11 02:18:13.000000 types-docker-7.0.0.20240511/docker-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:14.454193 types-docker-7.0.0.20240511/docker-stubs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/api/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/api/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/api/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/api/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/api/container.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/api/daemon.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/api/exec_api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/api/image.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/api/network.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/api/plugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/api/secret.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/api/service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/api/swarm.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/api/volume.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/auth.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/constants.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:14.454193 types-docker-7.0.0.20240511/docker-stubs/context/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/context/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/context/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/context/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/context/context.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:14.454193 types-docker-7.0.0.20240511/docker-stubs/credentials/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/credentials/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/credentials/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/credentials/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/credentials/store.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/credentials/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/errors.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:14.458193 types-docker-7.0.0.20240511/docker-stubs/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/models/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/models/configs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/models/containers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/models/images.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/models/networks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/models/nodes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/models/plugins.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/models/resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/models/secrets.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/models/services.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/models/swarm.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/models/volumes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:13.000000 types-docker-7.0.0.20240511/docker-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/tls.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:14.458193 types-docker-7.0.0.20240511/docker-stubs/transport/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/transport/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/transport/basehttpadapter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/transport/npipeconn.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/transport/npipesocket.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/transport/sshconn.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/transport/unixconn.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:14.458193 types-docker-7.0.0.20240511/docker-stubs/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/types/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/types/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/types/containers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/types/daemon.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/types/healthcheck.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/types/networks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/types/services.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/types/swarm.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:14.458193 types-docker-7.0.0.20240511/docker-stubs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/utils/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/utils/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/utils/decorators.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/utils/fnmatch.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/utils/json_stream.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/utils/ports.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/utils/proxy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/utils/socket.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/utils/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 02:18:14.462194 types-docker-7.0.0.20240511/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-11 02:18:13.000000 types-docker-7.0.0.20240511/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:14.462194 types-docker-7.0.0.20240511/types_docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-11 02:18:14.000000 types-docker-7.0.0.20240511/types_docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-11 02:18:14.000000 types-docker-7.0.0.20240511/types_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 02:18:14.000000 types-docker-7.0.0.20240511/types_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-11 02:18:14.000000 types-docker-7.0.0.20240511/types_docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-11 02:18:14.000000 types-docker-7.0.0.20240511/types_docker.egg-info/top_level.txt
```

### Comparing `types-docker-7.0.0.20240507/CHANGELOG.md` & `types-docker-7.0.0.20240511/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 7.0.0.20240511 (2024-05-11)
+
+Add some types to Docker ContainerCollection parameters (#11857)
+
 ## 7.0.0.20240507 (2024-05-07)
 
 Add return type to Docker Container.stop (#11869)
 
 We can see at
 https://github.com/docker/docker-py/blob/b6464dbed92b14b2c61d5ee49805fce041a3e083/docker/models/containers.py#L452
 that this returns the return value of `self.client.api.stop`.
```

### Comparing `types-docker-7.0.0.20240507/PKG-INFO` & `types-docker-7.0.0.20240511/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-docker
-Version: 7.0.0.20240507
+Version: 7.0.0.20240511
 Summary: Typing stubs for docker
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docker.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-docker` aims to provide accurate annotations
 for `docker==7.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docker. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `727f3c4320d2af3af2f16695e24dd78e79b7c070` and was tested
-with mypy 1.10.0, pyright 1.1.361, and
+This package was generated from typeshed commit `7bfde5b676a19080f4496c618117b748e2a02628` and was tested
+with mypy 1.10.0, pyright 1.1.362, and
 pytype 2024.4.11.
```

### Comparing `types-docker-7.0.0.20240507/docker-stubs/api/build.pyi` & `types-docker-7.0.0.20240511/docker-stubs/api/build.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/api/client.pyi` & `types-docker-7.0.0.20240511/docker-stubs/api/client.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/api/container.pyi` & `types-docker-7.0.0.20240511/docker-stubs/api/container.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/api/daemon.pyi` & `types-docker-7.0.0.20240511/docker-stubs/api/daemon.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/api/exec_api.pyi` & `types-docker-7.0.0.20240511/docker-stubs/api/exec_api.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/api/image.pyi` & `types-docker-7.0.0.20240511/docker-stubs/api/image.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/api/network.pyi` & `types-docker-7.0.0.20240511/docker-stubs/api/network.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/api/plugin.pyi` & `types-docker-7.0.0.20240511/docker-stubs/api/plugin.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/api/service.pyi` & `types-docker-7.0.0.20240511/docker-stubs/api/service.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/api/swarm.pyi` & `types-docker-7.0.0.20240511/docker-stubs/api/swarm.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/api/volume.pyi` & `types-docker-7.0.0.20240511/docker-stubs/api/volume.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/auth.pyi` & `types-docker-7.0.0.20240511/docker-stubs/auth.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/client.pyi` & `types-docker-7.0.0.20240511/docker-stubs/client.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/constants.pyi` & `types-docker-7.0.0.20240511/docker-stubs/constants.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/context/api.pyi` & `types-docker-7.0.0.20240511/docker-stubs/context/api.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/context/context.pyi` & `types-docker-7.0.0.20240511/docker-stubs/context/context.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/errors.pyi` & `types-docker-7.0.0.20240511/docker-stubs/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/models/containers.pyi` & `types-docker-7.0.0.20240511/docker-stubs/models/containers.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -53,18 +53,24 @@
     def unpause(self): ...
     def update(self, **kwargs): ...
     def wait(self, **kwargs): ...
 
 class ContainerCollection(Collection[Container]):
     model: type[Container]
     def run(
-        self, image, command: Incomplete | None = None, stdout: bool = True, stderr: bool = False, remove: bool = False, **kwargs
+        self,
+        image: str,
+        command: str | list[str] | None = None,
+        stdout: bool = True,
+        stderr: bool = False,
+        remove: bool = False,
+        **kwargs,
     ): ...
-    def create(self, image, command: Incomplete | None = None, **kwargs): ...  # type:ignore[override]
-    def get(self, container_id): ...
+    def create(self, image: str, command: str | list[str] | None = None, **kwargs): ...  # type:ignore[override]
+    def get(self, container_id: str): ...
     def list(
         self,
         all: bool = False,
         before: Incomplete | None = None,
         filters: Incomplete | None = None,
         limit: int = -1,
         since: Incomplete | None = None,
```

### Comparing `types-docker-7.0.0.20240507/docker-stubs/models/images.pyi` & `types-docker-7.0.0.20240511/docker-stubs/models/images.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/models/networks.pyi` & `types-docker-7.0.0.20240511/docker-stubs/models/networks.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/models/plugins.pyi` & `types-docker-7.0.0.20240511/docker-stubs/models/plugins.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/models/resource.pyi` & `types-docker-7.0.0.20240511/docker-stubs/models/resource.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/models/services.pyi` & `types-docker-7.0.0.20240511/docker-stubs/models/services.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/models/swarm.pyi` & `types-docker-7.0.0.20240511/docker-stubs/models/swarm.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/models/volumes.pyi` & `types-docker-7.0.0.20240511/docker-stubs/models/volumes.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/transport/npipeconn.pyi` & `types-docker-7.0.0.20240511/docker-stubs/transport/npipeconn.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/transport/npipesocket.pyi` & `types-docker-7.0.0.20240511/docker-stubs/transport/npipesocket.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/transport/sshconn.pyi` & `types-docker-7.0.0.20240511/docker-stubs/transport/sshconn.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/transport/unixconn.pyi` & `types-docker-7.0.0.20240511/docker-stubs/transport/unixconn.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/types/__init__.pyi` & `types-docker-7.0.0.20240511/docker-stubs/types/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/types/containers.pyi` & `types-docker-7.0.0.20240511/docker-stubs/types/containers.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/types/healthcheck.pyi` & `types-docker-7.0.0.20240511/docker-stubs/types/healthcheck.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/types/networks.pyi` & `types-docker-7.0.0.20240511/docker-stubs/types/networks.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/types/services.pyi` & `types-docker-7.0.0.20240511/docker-stubs/types/services.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/types/swarm.pyi` & `types-docker-7.0.0.20240511/docker-stubs/types/swarm.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/utils/__init__.pyi` & `types-docker-7.0.0.20240511/docker-stubs/utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/utils/build.pyi` & `types-docker-7.0.0.20240511/docker-stubs/utils/build.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/utils/proxy.pyi` & `types-docker-7.0.0.20240511/docker-stubs/utils/proxy.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/utils/socket.pyi` & `types-docker-7.0.0.20240511/docker-stubs/utils/socket.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/docker-stubs/utils/utils.pyi` & `types-docker-7.0.0.20240511/docker-stubs/utils/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240507/setup.py` & `types-docker-7.0.0.20240511/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 This version of `types-docker` aims to provide accurate annotations
 for `docker==7.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docker. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `727f3c4320d2af3af2f16695e24dd78e79b7c070` and was tested
-with mypy 1.10.0, pyright 1.1.361, and
+This package was generated from typeshed commit `7bfde5b676a19080f4496c618117b748e2a02628` and was tested
+with mypy 1.10.0, pyright 1.1.362, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="7.0.0.20240507",
+      version="7.0.0.20240511",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docker.md",
```

### Comparing `types-docker-7.0.0.20240507/types_docker.egg-info/PKG-INFO` & `types-docker-7.0.0.20240511/types_docker.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-docker
-Version: 7.0.0.20240507
+Version: 7.0.0.20240511
 Summary: Typing stubs for docker
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docker.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-docker` aims to provide accurate annotations
 for `docker==7.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docker. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `727f3c4320d2af3af2f16695e24dd78e79b7c070` and was tested
-with mypy 1.10.0, pyright 1.1.361, and
+This package was generated from typeshed commit `7bfde5b676a19080f4496c618117b748e2a02628` and was tested
+with mypy 1.10.0, pyright 1.1.362, and
 pytype 2024.4.11.
```

### Comparing `types-docker-7.0.0.20240507/types_docker.egg-info/SOURCES.txt` & `types-docker-7.0.0.20240511/types_docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

