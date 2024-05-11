# Comparing `tmp/skypilot_nightly-1.0.0.dev20240509.tar.gz` & `tmp/skypilot_nightly-1.0.0.dev20240510.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skypilot_nightly-1.0.0.dev20240509.tar", last modified: Thu May  9 10:38:33 2024, max compression
+gzip compressed data, was "skypilot_nightly-1.0.0.dev20240510.tar", last modified: Fri May 10 10:38:15 2024, max compression
```

## Comparing `skypilot_nightly-1.0.0.dev20240509.tar` & `skypilot_nightly-1.0.0.dev20240510.tar`

### file list

```diff
@@ -1,339 +1,339 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.853181 skypilot_nightly-1.0.0.dev20240509/
--rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-05-09 10:38:33.853181 skypilot_nightly-1.0.0.dev20240509/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12079 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 10:38:33.853181 skypilot_nightly-1.0.0.dev20240509/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    12055 2024-05-09 10:38:29.000000 skypilot_nightly-1.0.0.dev20240509/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.785180 skypilot_nightly-1.0.0.dev20240509/sky/
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-05-09 10:38:33.000000 skypilot_nightly-1.0.0.dev20240509/sky/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.789180 skypilot_nightly-1.0.0.dev20240509/sky/adaptors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/adaptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/adaptors/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/adaptors/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/adaptors/cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/adaptors/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/adaptors/cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/adaptors/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/adaptors/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/adaptors/ibm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/adaptors/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/adaptors/oci.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/adaptors/runpod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/adaptors/vsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    21408 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.789180 skypilot_nightly-1.0.0.dev20240509/sky/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)   125396 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/backends/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   230261 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/backends/cloud_vm_ray_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/backends/docker_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16741 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/backends/local_docker_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.789180 skypilot_nightly-1.0.0.dev20240509/sky/backends/monkey_patches/
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/backends/monkey_patches/monkey_patch_ray_up.py
--rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/backends/wheel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.789180 skypilot_nightly-1.0.0.dev20240509/sky/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/benchmark/benchmark_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    26446 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/benchmark/benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/check.py
--rw-r--r--   0 runner    (1001) docker     (127)   190684 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/cloud_stores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.793180 skypilot_nightly-1.0.0.dev20240509/sky/clouds/
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44608 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    31006 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)    31745 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/cloud_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    12036 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)    12647 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/fluidstack.py
--rw-r--r--   0 runner    (1001) docker     (127)    48019 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)    21044 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/ibm.py
--rw-r--r--   0 runner    (1001) docker     (127)    20122 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12157 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    25299 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/oci.py
--rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/paperspace.py
--rw-r--r--   0 runner    (1001) docker     (127)    11166 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/runpod.py
--rw-r--r--   0 runner    (1001) docker     (127)    15546 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.797180 skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12550 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/aws_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/azure_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    26837 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/cudo_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.797180 skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/data_fetchers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/data_fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py
--rw-r--r--   0 runner    (1001) docker     (127)    22243 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    21462 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/fluidstack_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    24120 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/gcp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/ibm_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/kubernetes_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/lambda_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/oci_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/paperspace_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/runpod_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/scp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/vsphere_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.797180 skypilot_nightly-1.0.0.dev20240509/sky/clouds/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/utils/gcp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/utils/lambda_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/utils/oci_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/utils/scp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/clouds/vsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    33633 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/dag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.801180 skypilot_nightly-1.0.0.dev20240509/sky/data/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/data/data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)    21664 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/data/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/data/mounting_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   118872 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/data/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/data/storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    24917 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)    28681 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/global_user_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.801180 skypilot_nightly-1.0.0.dev20240509/sky/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/jobs/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    26607 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/jobs/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    13430 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/jobs/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.801180 skypilot_nightly-1.0.0.dev20240509/sky/jobs/dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/jobs/dashboard/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.801180 skypilot_nightly-1.0.0.dev20240509/sky/jobs/dashboard/static/
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/jobs/dashboard/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.801180 skypilot_nightly-1.0.0.dev20240509/sky/jobs/dashboard/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/jobs/dashboard/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    25556 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/jobs/recovery_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    23041 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/jobs/state.py
--rw-r--r--   0 runner    (1001) docker     (127)    33067 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/jobs/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    54188 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.805180 skypilot_nightly-1.0.0.dev20240509/sky/provision/
--rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.805180 skypilot_nightly-1.0.0.dev20240509/sky/provision/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22092 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/aws/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    36307 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/aws/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.805180 skypilot_nightly-1.0.0.dev20240509/sky/provision/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/azure/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     9339 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.805180 skypilot_nightly-1.0.0.dev20240509/sky/provision/cudo/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/cudo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/cudo/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/cudo/cudo_machine_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/cudo/cudo_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/cudo/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    16758 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/docker_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.805180 skypilot_nightly-1.0.0.dev20240509/sky/provision/fluidstack/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/fluidstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/fluidstack/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/fluidstack/fluidstack_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14974 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/fluidstack/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.809180 skypilot_nightly-1.0.0.dev20240509/sky/provision/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32964 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/gcp/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    24215 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/gcp/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    59069 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/gcp/instance_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22186 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/instance_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.809180 skypilot_nightly-1.0.0.dev20240509/sky/provision/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22684 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/kubernetes/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    32919 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/kubernetes/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.809180 skypilot_nightly-1.0.0.dev20240509/sky/provision/kubernetes/manifests/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/kubernetes/manifests/smarter-device-manager-configmap.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/kubernetes/manifests/smarter-device-manager-daemonset.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/kubernetes/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     9384 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/kubernetes/network_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    61188 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/kubernetes/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/metadata_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.809180 skypilot_nightly-1.0.0.dev20240509/sky/provision/paperspace/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/paperspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/paperspace/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/paperspace/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/paperspace/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/paperspace/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25103 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/provisioner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.809180 skypilot_nightly-1.0.0.dev20240509/sky/provision/runpod/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/runpod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/runpod/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/runpod/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/runpod/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.813180 skypilot_nightly-1.0.0.dev20240509/sky/provision/vsphere/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/vsphere/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.813180 skypilot_nightly-1.0.0.dev20240509/sky/provision/vsphere/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/vsphere/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/vsphere/common/cls_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14096 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/vsphere/common/cls_api_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/vsphere/common/custom_script.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/vsphere/common/id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/vsphere/common/metadata_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/vsphere/common/service_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/vsphere/common/service_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/vsphere/common/ssl_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/vsphere/common/vapiconnect.py
--rw-r--r--   0 runner    (1001) docker     (127)    17877 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/vsphere/common/vim_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/vsphere/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    24488 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/vsphere/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    15151 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/provision/vsphere/vsphere_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    65346 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.817180 skypilot_nightly-1.0.0.dev20240509/sky/serve/
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30136 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/serve/autoscalers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/serve/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/serve/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    28522 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/serve/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/serve/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/serve/load_balancing_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)    56630 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/serve/replica_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18830 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/serve/serve_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    37183 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/serve/serve_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/serve/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    13803 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/serve/service_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.817180 skypilot_nightly-1.0.0.dev20240509/sky/setup_files/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/setup_files/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12055 2024-05-09 10:38:29.000000 skypilot_nightly-1.0.0.dev20240509/sky/setup_files/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/sky_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.821180 skypilot_nightly-1.0.0.dev20240509/sky/skylet/
--rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/attempt_skylet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/autostop_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9977 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    11759 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    35198 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/job_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    18824 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/log_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/log_lib.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.821180 skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.821180 skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/azure/azure-config-template.json
--rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/azure/azure-vm-template.json
--rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/azure/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    19215 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/azure/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    16355 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/command_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.821180 skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38280 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/ibm/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/ibm/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    34630 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/ibm/vpc_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.821180 skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/lambda_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/lambda_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13971 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/lambda_cloud/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.821180 skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/oci/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20492 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/oci/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    17202 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/oci/query_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/oci/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.825180 skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/scp/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/scp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/scp/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    22411 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/scp/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.825180 skypilot_nightly-1.0.0.dev20240509/sky/skylet/ray_patches/
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/ray_patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/ray_patches/autoscaler.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/ray_patches/cli.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/ray_patches/command_runner.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/ray_patches/log_monitor.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/ray_patches/updater.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/ray_patches/worker.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/skylet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skylet/subprocess_daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/skypilot_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/status_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    47130 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.829180 skypilot_nightly-1.0.0.dev20240509/sky/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/templates/aws-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     9037 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/templates/azure-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/templates/cudo-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/templates/fluidstack-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/templates/gcp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/templates/ibm-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/templates/jobs-controller.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/templates/kubernetes-ingress.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/templates/kubernetes-loadbalancer.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/templates/kubernetes-port-forward-proxy-command.sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)    13943 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/templates/kubernetes-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/templates/kubernetes-ssh-jump.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/templates/lambda-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/templates/local-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/templates/oci-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/templates/paperspace-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/templates/runpod-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/templates/scp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/templates/sky-serve-controller.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/templates/vsphere-ray.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.829180 skypilot_nightly-1.0.0.dev20240509/sky/usage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/usage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/usage/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    17601 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/usage/usage_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.833180 skypilot_nightly-1.0.0.dev20240509/sky/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/utils/accelerator_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.833180 skypilot_nightly-1.0.0.dev20240509/sky/utils/cli_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/utils/cli_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/utils/cli_utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/utils/cluster_yaml_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22168 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/utils/command_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/utils/command_runner.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    23848 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    34359 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/utils/controller_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/utils/dag_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/utils/env_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.837180 skypilot_nightly-1.0.0.dev20240509/sky/utils/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/utils/kubernetes/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9759 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/utils/kubernetes/create_cluster.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      927 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/utils/kubernetes/delete_cluster.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/utils/kubernetes/generate_kind_config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4422 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/utils/kubernetes/generate_static_kubeconfig.sh
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/utils/kubernetes/gpu_labeler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/utils/kubernetes_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/utils/resources_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/utils/rich_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22543 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/utils/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/utils/subprocess_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/utils/timeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/utils/ux_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/sky/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.841180 skypilot_nightly-1.0.0.dev20240509/skypilot_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-05-09 10:38:33.000000 skypilot_nightly-1.0.0.dev20240509/skypilot_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9353 2024-05-09 10:38:33.000000 skypilot_nightly-1.0.0.dev20240509/skypilot_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 10:38:33.000000 skypilot_nightly-1.0.0.dev20240509/skypilot_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-09 10:38:33.000000 skypilot_nightly-1.0.0.dev20240509/skypilot_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-09 10:38:33.000000 skypilot_nightly-1.0.0.dev20240509/skypilot_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-09 10:38:33.000000 skypilot_nightly-1.0.0.dev20240509/skypilot_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:38:33.841180 skypilot_nightly-1.0.0.dev20240509/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/tests/test_global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17529 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/tests/test_jobs_and_serve.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/tests/test_list_accelerators.py
--rw-r--r--   0 runner    (1001) docker     (127)    27759 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/tests/test_optimizer_dryruns.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/tests/test_optimizer_random_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/tests/test_serve_autoscaler.py
--rw-r--r--   0 runner    (1001) docker     (127)   215682 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/tests/test_smoke.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/tests/test_wheels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-09 10:38:25.000000 skypilot_nightly-1.0.0.dev20240509/tests/test_yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.943324 skypilot_nightly-1.0.0.dev20240510/
+-rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-05-10 10:38:10.000000 skypilot_nightly-1.0.0.dev20240510/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-05-10 10:38:15.943324 skypilot_nightly-1.0.0.dev20240510/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12079 2024-05-10 10:38:10.000000 skypilot_nightly-1.0.0.dev20240510/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 10:38:15.943324 skypilot_nightly-1.0.0.dev20240510/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    12055 2024-05-10 10:38:13.000000 skypilot_nightly-1.0.0.dev20240510/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.887323 skypilot_nightly-1.0.0.dev20240510/sky/
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-05-10 10:38:15.000000 skypilot_nightly-1.0.0.dev20240510/sky/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.887323 skypilot_nightly-1.0.0.dev20240510/sky/adaptors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/adaptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/adaptors/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/adaptors/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/adaptors/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/adaptors/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/adaptors/cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/adaptors/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/adaptors/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/adaptors/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/adaptors/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/adaptors/oci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/adaptors/runpod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/adaptors/vsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21408 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.891323 skypilot_nightly-1.0.0.dev20240510/sky/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)   125420 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/backends/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   230261 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/backends/cloud_vm_ray_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/backends/docker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16741 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/backends/local_docker_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.891323 skypilot_nightly-1.0.0.dev20240510/sky/backends/monkey_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/backends/monkey_patches/monkey_patch_ray_up.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/backends/wheel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.891323 skypilot_nightly-1.0.0.dev20240510/sky/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/benchmark/benchmark_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26446 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/benchmark/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)   190684 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/cloud_stores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.895323 skypilot_nightly-1.0.0.dev20240510/sky/clouds/
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44608 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31006 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31817 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/cloud_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12036 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12647 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/fluidstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48019 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21044 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20409 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12157 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25299 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/oci.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/paperspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11166 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/runpod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15546 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.895323 skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12550 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/aws_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/azure_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26837 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/cudo_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.899323 skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/data_fetchers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/data_fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22243 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21462 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/fluidstack_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24120 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/gcp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/ibm_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/kubernetes_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/lambda_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/oci_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/paperspace_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/runpod_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/scp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/vsphere_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.899323 skypilot_nightly-1.0.0.dev20240510/sky/clouds/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/utils/gcp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/utils/lambda_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/utils/oci_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/utils/scp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/clouds/vsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34233 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/dag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.899323 skypilot_nightly-1.0.0.dev20240510/sky/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/data/data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21664 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/data/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/data/mounting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   118872 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/data/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/data/storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25107 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28681 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/global_user_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.903324 skypilot_nightly-1.0.0.dev20240510/sky/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/jobs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26607 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/jobs/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13430 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/jobs/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.903324 skypilot_nightly-1.0.0.dev20240510/sky/jobs/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/jobs/dashboard/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.903324 skypilot_nightly-1.0.0.dev20240510/sky/jobs/dashboard/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/jobs/dashboard/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.903324 skypilot_nightly-1.0.0.dev20240510/sky/jobs/dashboard/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/jobs/dashboard/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    25556 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/jobs/recovery_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23041 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/jobs/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33067 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/jobs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54188 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.903324 skypilot_nightly-1.0.0.dev20240510/sky/provision/
+-rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.903324 skypilot_nightly-1.0.0.dev20240510/sky/provision/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22092 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/aws/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36307 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/aws/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.903324 skypilot_nightly-1.0.0.dev20240510/sky/provision/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/azure/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9339 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.903324 skypilot_nightly-1.0.0.dev20240510/sky/provision/cudo/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/cudo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/cudo/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/cudo/cudo_machine_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/cudo/cudo_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/cudo/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16758 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/docker_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.907323 skypilot_nightly-1.0.0.dev20240510/sky/provision/fluidstack/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/fluidstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/fluidstack/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/fluidstack/fluidstack_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14974 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/fluidstack/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.907323 skypilot_nightly-1.0.0.dev20240510/sky/provision/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32964 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/gcp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24215 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/gcp/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59069 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/gcp/instance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22186 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/instance_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.907323 skypilot_nightly-1.0.0.dev20240510/sky/provision/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22684 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/kubernetes/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32919 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/kubernetes/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.907323 skypilot_nightly-1.0.0.dev20240510/sky/provision/kubernetes/manifests/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/kubernetes/manifests/smarter-device-manager-configmap.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/kubernetes/manifests/smarter-device-manager-daemonset.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/kubernetes/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9384 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/kubernetes/network_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61255 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/kubernetes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/metadata_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.907323 skypilot_nightly-1.0.0.dev20240510/sky/provision/paperspace/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/paperspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/paperspace/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/paperspace/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/paperspace/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/paperspace/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25103 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/provisioner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.911324 skypilot_nightly-1.0.0.dev20240510/sky/provision/runpod/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/runpod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/runpod/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/runpod/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/runpod/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.911324 skypilot_nightly-1.0.0.dev20240510/sky/provision/vsphere/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/vsphere/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.911324 skypilot_nightly-1.0.0.dev20240510/sky/provision/vsphere/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/vsphere/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/vsphere/common/cls_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14096 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/vsphere/common/cls_api_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/vsphere/common/custom_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/vsphere/common/id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/vsphere/common/metadata_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/vsphere/common/service_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/vsphere/common/service_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/vsphere/common/ssl_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/vsphere/common/vapiconnect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17877 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/vsphere/common/vim_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/vsphere/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24488 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/vsphere/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15151 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/provision/vsphere/vsphere_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65346 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.915324 skypilot_nightly-1.0.0.dev20240510/sky/serve/
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30136 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/serve/autoscalers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/serve/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/serve/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28522 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/serve/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/serve/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/serve/load_balancing_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56630 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/serve/replica_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18830 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/serve/serve_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37183 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/serve/serve_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/serve/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13803 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/serve/service_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.915324 skypilot_nightly-1.0.0.dev20240510/sky/setup_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/setup_files/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12055 2024-05-10 10:38:13.000000 skypilot_nightly-1.0.0.dev20240510/sky/setup_files/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/sky_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.915324 skypilot_nightly-1.0.0.dev20240510/sky/skylet/
+-rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/attempt_skylet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/autostop_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9977 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11759 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35198 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/job_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18824 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/log_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/log_lib.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.915324 skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.915324 skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/azure/azure-config-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/azure/azure-vm-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/azure/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19215 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/azure/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16355 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/command_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.919324 skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38280 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/ibm/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/ibm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34630 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/ibm/vpc_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.919324 skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/lambda_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/lambda_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13971 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/lambda_cloud/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.919324 skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/oci/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20492 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/oci/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17202 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/oci/query_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/oci/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.919324 skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/scp/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/scp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/scp/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22411 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/scp/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.919324 skypilot_nightly-1.0.0.dev20240510/sky/skylet/ray_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/ray_patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/ray_patches/autoscaler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/ray_patches/cli.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/ray_patches/command_runner.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/ray_patches/log_monitor.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/ray_patches/updater.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/ray_patches/worker.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/skylet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skylet/subprocess_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/skypilot_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/status_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47130 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.923324 skypilot_nightly-1.0.0.dev20240510/sky/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/templates/aws-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     9037 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/templates/azure-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/templates/cudo-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/templates/fluidstack-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/templates/gcp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/templates/ibm-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/templates/jobs-controller.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/templates/kubernetes-ingress.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/templates/kubernetes-loadbalancer.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/templates/kubernetes-port-forward-proxy-command.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)    13943 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/templates/kubernetes-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/templates/kubernetes-ssh-jump.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/templates/lambda-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/templates/local-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/templates/oci-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/templates/paperspace-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/templates/runpod-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/templates/scp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/templates/sky-serve-controller.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/templates/vsphere-ray.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.923324 skypilot_nightly-1.0.0.dev20240510/sky/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/usage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/usage/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17601 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/usage/usage_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.927324 skypilot_nightly-1.0.0.dev20240510/sky/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/utils/accelerator_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.927324 skypilot_nightly-1.0.0.dev20240510/sky/utils/cli_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/utils/cli_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/utils/cli_utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/utils/cluster_yaml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22168 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/utils/command_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/utils/command_runner.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    23848 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34359 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/utils/controller_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/utils/dag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/utils/env_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.927324 skypilot_nightly-1.0.0.dev20240510/sky/utils/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/utils/kubernetes/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9759 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/utils/kubernetes/create_cluster.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      927 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/utils/kubernetes/delete_cluster.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/utils/kubernetes/generate_kind_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4422 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/utils/kubernetes/generate_static_kubeconfig.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/utils/kubernetes/gpu_labeler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/utils/kubernetes_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/utils/resources_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/utils/rich_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22737 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/utils/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/utils/subprocess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/utils/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/utils/ux_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/sky/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.931324 skypilot_nightly-1.0.0.dev20240510/skypilot_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-05-10 10:38:15.000000 skypilot_nightly-1.0.0.dev20240510/skypilot_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9353 2024-05-10 10:38:15.000000 skypilot_nightly-1.0.0.dev20240510/skypilot_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 10:38:15.000000 skypilot_nightly-1.0.0.dev20240510/skypilot_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-10 10:38:15.000000 skypilot_nightly-1.0.0.dev20240510/skypilot_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-10 10:38:15.000000 skypilot_nightly-1.0.0.dev20240510/skypilot_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-10 10:38:15.000000 skypilot_nightly-1.0.0.dev20240510/skypilot_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:38:15.931324 skypilot_nightly-1.0.0.dev20240510/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/tests/test_global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17529 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/tests/test_jobs_and_serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/tests/test_list_accelerators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27759 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/tests/test_optimizer_dryruns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/tests/test_optimizer_random_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/tests/test_serve_autoscaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)   215682 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/tests/test_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/tests/test_wheels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-10 10:38:11.000000 skypilot_nightly-1.0.0.dev20240510/tests/test_yaml_parser.py
```

### Comparing `skypilot_nightly-1.0.0.dev20240509/LICENSE` & `skypilot_nightly-1.0.0.dev20240510/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/MANIFEST.in` & `skypilot_nightly-1.0.0.dev20240510/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/PKG-INFO` & `skypilot_nightly-1.0.0.dev20240510/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20240509
+Version: 1.0.0.dev20240510
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

### Comparing `skypilot_nightly-1.0.0.dev20240509/README.md` & `skypilot_nightly-1.0.0.dev20240510/README.md`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/pyproject.toml` & `skypilot_nightly-1.0.0.dev20240510/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/setup.py` & `skypilot_nightly-1.0.0.dev20240510/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/__init__.py` & `skypilot_nightly-1.0.0.dev20240510/sky/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """The SkyPilot package."""
 import os
 import subprocess
 from typing import Optional
 import urllib.request
 
 # Replaced with the current commit when building the wheels.
-_SKYPILOT_COMMIT_SHA = '07da93b3c3b87e53d0ebd7e033c9ce24992151fe'
+_SKYPILOT_COMMIT_SHA = '4683c46edb5e1b5dcadb1ef143e6baedc145fcd4'
 
 
 def _get_git_commit():
     if 'SKYPILOT_COMMIT_SHA' not in _SKYPILOT_COMMIT_SHA:
         # This is a release build, so we don't need to get the commit hash from
         # git, as it's already been set.
         return _SKYPILOT_COMMIT_SHA
@@ -31,15 +31,15 @@
             commit_hash += '-dirty'
         return commit_hash
     except Exception:  # pylint: disable=broad-except
         return _SKYPILOT_COMMIT_SHA
 
 
 __commit__ = _get_git_commit()
-__version__ = '1.0.0.dev20240509'
+__version__ = '1.0.0.dev20240510'
 __root_dir__ = os.path.dirname(os.path.abspath(__file__))
 
 
 # ---------------------- Proxy Configuration ---------------------- #
 def _set_http_proxy_env_vars() -> None:
     urllib_proxies = dict(urllib.request.getproxies())
```

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/adaptors/aws.py` & `skypilot_nightly-1.0.0.dev20240510/sky/adaptors/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/adaptors/azure.py` & `skypilot_nightly-1.0.0.dev20240510/sky/adaptors/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/adaptors/cloudflare.py` & `skypilot_nightly-1.0.0.dev20240510/sky/adaptors/cloudflare.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/adaptors/common.py` & `skypilot_nightly-1.0.0.dev20240510/sky/adaptors/common.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/adaptors/gcp.py` & `skypilot_nightly-1.0.0.dev20240510/sky/adaptors/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/adaptors/ibm.py` & `skypilot_nightly-1.0.0.dev20240510/sky/adaptors/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/adaptors/kubernetes.py` & `skypilot_nightly-1.0.0.dev20240510/sky/adaptors/kubernetes.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/adaptors/oci.py` & `skypilot_nightly-1.0.0.dev20240510/sky/adaptors/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/adaptors/vsphere.py` & `skypilot_nightly-1.0.0.dev20240510/sky/adaptors/vsphere.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/authentication.py` & `skypilot_nightly-1.0.0.dev20240510/sky/authentication.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/backends/__init__.py` & `skypilot_nightly-1.0.0.dev20240510/sky/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/backends/backend.py` & `skypilot_nightly-1.0.0.dev20240510/sky/backends/backend.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/backends/backend_utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/backends/backend_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2113,5726 +2113,5727 @@
 00008400: 6c6f 7564 7320 3d20 5b5d 0a20 2020 2072  louds = [].    r
 00008410: 656d 6f74 655f 6964 656e 7469 7479 203d  emote_identity =
 00008420: 2073 6b79 7069 6c6f 745f 636f 6e66 6967   skypilot_config
 00008430: 2e67 6574 5f6e 6573 7465 6428 0a20 2020  .get_nested(.   
 00008440: 2020 2020 2028 7374 7228 636c 6f75 6429       (str(cloud)
 00008450: 2e6c 6f77 6572 2829 2c20 2772 656d 6f74  .lower(), 'remot
 00008460: 655f 6964 656e 7469 7479 2729 2c0a 2020  e_identity'),.  
-00008470: 2020 2020 2020 7363 6865 6d61 732e 5245        schemas.RE
-00008480: 4d4f 5445 5f49 4445 4e54 4954 595f 4445  MOTE_IDENTITY_DE
-00008490: 4641 554c 5429 0a20 2020 2069 6620 7265  FAULT).    if re
-000084a0: 6d6f 7465 5f69 6465 6e74 6974 7920 6973  mote_identity is
-000084b0: 206e 6f74 204e 6f6e 6520 616e 6420 6e6f   not None and no
-000084c0: 7420 6973 696e 7374 616e 6365 2872 656d  t isinstance(rem
-000084d0: 6f74 655f 6964 656e 7469 7479 2c20 7374  ote_identity, st
-000084e0: 7229 3a0a 2020 2020 2020 2020 666f 7220  r):.        for 
-000084f0: 7072 6f66 696c 6520 696e 2072 656d 6f74  profile in remot
-00008500: 655f 6964 656e 7469 7479 3a0a 2020 2020  e_identity:.    
-00008510: 2020 2020 2020 2020 6966 2066 6e6d 6174          if fnmat
-00008520: 6368 2e66 6e6d 6174 6368 6361 7365 2863  ch.fnmatchcase(c
-00008530: 6c75 7374 6572 5f6e 616d 652c 206c 6973  luster_name, lis
-00008540: 7428 7072 6f66 696c 652e 6b65 7973 2829  t(profile.keys()
-00008550: 295b 305d 293a 0a20 2020 2020 2020 2020  )[0]):.         
-00008560: 2020 2020 2020 2072 656d 6f74 655f 6964         remote_id
-00008570: 656e 7469 7479 203d 206c 6973 7428 7072  entity = list(pr
-00008580: 6f66 696c 652e 7661 6c75 6573 2829 295b  ofile.values())[
-00008590: 305d 0a20 2020 2020 2020 2020 2020 2020  0].             
-000085a0: 2020 2062 7265 616b 0a20 2020 2069 6620     break.    if 
-000085b0: 7265 6d6f 7465 5f69 6465 6e74 6974 7920  remote_identity 
-000085c0: 213d 2073 6368 656d 6173 2e52 656d 6f74  != schemas.Remot
-000085d0: 6549 6465 6e74 6974 794f 7074 696f 6e73  eIdentityOptions
-000085e0: 2e4c 4f43 414c 5f43 5245 4445 4e54 4941  .LOCAL_CREDENTIA
-000085f0: 4c53 2e76 616c 7565 3a0a 2020 2020 2020  LS.value:.      
-00008600: 2020 6966 206e 6f74 2063 6c6f 7564 2e73    if not cloud.s
-00008610: 7570 706f 7274 735f 7365 7276 6963 655f  upports_service_
-00008620: 6163 636f 756e 745f 6f6e 5f72 656d 6f74  account_on_remot
-00008630: 6528 293a 0a20 2020 2020 2020 2020 2020  e():.           
-00008640: 2072 6169 7365 2065 7863 6570 7469 6f6e   raise exception
-00008650: 732e 496e 7661 6c69 6443 6c6f 7564 436f  s.InvalidCloudCo
-00008660: 6e66 6967 7328 0a20 2020 2020 2020 2020  nfigs(.         
-00008670: 2020 2020 2020 2027 7265 6d6f 7465 5f69         'remote_i
-00008680: 6465 6e74 6974 793a 2053 4552 5649 4345  dentity: SERVICE
-00008690: 5f41 4343 4f55 4e54 2069 7320 7370 6563  _ACCOUNT is spec
-000086a0: 6966 6965 6420 696e 2027 0a20 2020 2020  ified in '.     
-000086b0: 2020 2020 2020 2020 2020 2066 277b 736b             f'{sk
-000086c0: 7970 696c 6f74 5f63 6f6e 6669 672e 6c6f  ypilot_config.lo
-000086d0: 6164 6564 5f63 6f6e 6669 675f 7061 7468  aded_config_path
-000086e0: 2172 7d20 666f 7220 7b63 6c6f 7564 7d2c  !r} for {cloud},
-000086f0: 2062 7574 2069 7420 270a 2020 2020 2020   but it '.      
-00008700: 2020 2020 2020 2020 2020 2769 7320 6e6f            'is no
-00008710: 7420 7375 7070 6f72 7465 6420 6279 2074  t supported by t
-00008720: 6869 7320 636c 6f75 642e 2052 656d 6f76  his cloud. Remov
-00008730: 6520 7468 6520 636f 6e66 6967 206f 7220  e the config or 
-00008740: 7365 743a 2027 0a20 2020 2020 2020 2020  set: '.         
-00008750: 2020 2020 2020 2027 6072 656d 6f74 655f         '`remote_
-00008760: 6964 656e 7469 7479 3a20 4c4f 4341 4c5f  identity: LOCAL_
-00008770: 4352 4544 454e 5449 414c 5360 2e27 290a  CREDENTIALS`.').
-00008780: 2020 2020 2020 2020 6578 636c 7564 6564          excluded
-00008790: 5f63 6c6f 7564 7320 3d20 5b63 6c6f 7564  _clouds = [cloud
-000087a0: 5d0a 2020 2020 6372 6564 656e 7469 616c  ].    credential
-000087b0: 7320 3d20 736b 795f 6368 6563 6b2e 6765  s = sky_check.ge
-000087c0: 745f 636c 6f75 645f 6372 6564 656e 7469  t_cloud_credenti
-000087d0: 616c 5f66 696c 655f 6d6f 756e 7473 2865  al_file_mounts(e
-000087e0: 7863 6c75 6465 645f 636c 6f75 6473 290a  xcluded_clouds).
-000087f0: 0a20 2020 2061 7574 685f 636f 6e66 6967  .    auth_config
-00008800: 203d 207b 2773 7368 5f70 7269 7661 7465   = {'ssh_private
-00008810: 5f6b 6579 273a 2061 7574 682e 5052 4956  _key': auth.PRIV
-00008820: 4154 455f 5353 485f 4b45 595f 5041 5448  ATE_SSH_KEY_PATH
-00008830: 7d0a 2020 2020 7265 6769 6f6e 5f6e 616d  }.    region_nam
-00008840: 6520 3d20 7265 736f 7572 6365 735f 7661  e = resources_va
-00008850: 7273 2e67 6574 2827 7265 6769 6f6e 2729  rs.get('region')
-00008860: 0a0a 2020 2020 7961 6d6c 5f70 6174 6820  ..    yaml_path 
-00008870: 3d20 5f67 6574 5f79 616d 6c5f 7061 7468  = _get_yaml_path
-00008880: 5f66 726f 6d5f 636c 7573 7465 725f 6e61  _from_cluster_na
-00008890: 6d65 2863 6c75 7374 6572 5f6e 616d 6529  me(cluster_name)
-000088a0: 0a0a 2020 2020 2320 5265 7472 6965 7665  ..    # Retrieve
-000088b0: 2074 6865 2073 7368 5f70 726f 7879 5f63   the ssh_proxy_c
-000088c0: 6f6d 6d61 6e64 2066 6f72 2074 6865 2067  ommand for the g
-000088d0: 6976 656e 2063 6c6f 7564 202f 2072 6567  iven cloud / reg
-000088e0: 696f 6e2e 0a20 2020 2073 7368 5f70 726f  ion..    ssh_pro
-000088f0: 7879 5f63 6f6d 6d61 6e64 5f63 6f6e 6669  xy_command_confi
-00008900: 6720 3d20 736b 7970 696c 6f74 5f63 6f6e  g = skypilot_con
-00008910: 6669 672e 6765 745f 6e65 7374 6564 280a  fig.get_nested(.
-00008920: 2020 2020 2020 2020 2873 7472 2863 6c6f          (str(clo
-00008930: 7564 292e 6c6f 7765 7228 292c 2027 7373  ud).lower(), 'ss
-00008940: 685f 7072 6f78 795f 636f 6d6d 616e 6427  h_proxy_command'
-00008950: 292c 204e 6f6e 6529 0a20 2020 2069 6620  ), None).    if 
-00008960: 2869 7369 6e73 7461 6e63 6528 7373 685f  (isinstance(ssh_
-00008970: 7072 6f78 795f 636f 6d6d 616e 645f 636f  proxy_command_co
-00008980: 6e66 6967 2c20 7374 7229 206f 720a 2020  nfig, str) or.  
-00008990: 2020 2020 2020 2020 2020 7373 685f 7072            ssh_pr
-000089a0: 6f78 795f 636f 6d6d 616e 645f 636f 6e66  oxy_command_conf
-000089b0: 6967 2069 7320 4e6f 6e65 293a 0a20 2020  ig is None):.   
-000089c0: 2020 2020 2073 7368 5f70 726f 7879 5f63       ssh_proxy_c
-000089d0: 6f6d 6d61 6e64 203d 2073 7368 5f70 726f  ommand = ssh_pro
-000089e0: 7879 5f63 6f6d 6d61 6e64 5f63 6f6e 6669  xy_command_confi
-000089f0: 670a 2020 2020 656c 7365 3a0a 2020 2020  g.    else:.    
-00008a00: 2020 2020 2320 7373 685f 7072 6f78 795f      # ssh_proxy_
-00008a10: 636f 6d6d 616e 645f 636f 6e66 6967 3a20  command_config: 
-00008a20: 4469 6374 5b73 7472 2c20 7374 725d 2c20  Dict[str, str], 
-00008a30: 7265 6769 6f6e 5f6e 616d 6520 2d3e 2063  region_name -> c
-00008a40: 6f6d 6d61 6e64 0a20 2020 2020 2020 2023  ommand.        #
-00008a50: 2054 6869 7320 7479 7065 2063 6865 636b   This type check
-00008a60: 2069 7320 646f 6e65 2062 7920 736b 7970   is done by skyp
-00008a70: 696c 6f74 5f63 6f6e 6669 6720 6174 2063  ilot_config at c
-00008a80: 6f6e 6669 6720 6c6f 6164 2074 696d 652e  onfig load time.
-00008a90: 0a0a 2020 2020 2020 2020 2320 5468 6572  ..        # Ther
-00008aa0: 6520 6172 6520 7477 6f20 6361 7365 733a  e are two cases:
-00008ab0: 0a20 2020 2020 2020 2069 6620 6b65 6570  .        if keep
-00008ac0: 5f6c 6175 6e63 685f 6669 656c 6473 5f69  _launch_fields_i
-00008ad0: 6e5f 6578 6973 7469 6e67 5f63 6f6e 6669  n_existing_confi
-00008ae0: 673a 0a20 2020 2020 2020 2020 2020 2023  g:.            #
-00008af0: 2028 3129 2057 6527 7265 2072 652d 7072   (1) We're re-pr
-00008b00: 6f76 6973 696f 6e69 6e67 2061 6e20 6578  ovisioning an ex
-00008b10: 6973 7469 6e67 2063 6c75 7374 6572 2e0a  isting cluster..
-00008b20: 2020 2020 2020 2020 2020 2020 230a 2020              #.  
-00008b30: 2020 2020 2020 2020 2020 2320 5765 2075            # We u
-00008b40: 7365 204e 6f6e 6520 666f 7220 7373 685f  se None for ssh_
-00008b50: 7072 6f78 795f 636f 6d6d 616e 642c 2077  proxy_command, w
-00008b60: 6869 6368 2077 696c 6c20 6265 2072 6573  hich will be res
-00008b70: 746f 7265 6420 746f 2074 6865 0a20 2020  tored to the.   
-00008b80: 2020 2020 2020 2020 2023 2063 6c75 7374           # clust
-00008b90: 6572 2773 206f 7269 6769 6e61 6c20 7661  er's original va
-00008ba0: 6c75 6520 6c61 7465 7220 6279 205f 7265  lue later by _re
-00008bb0: 706c 6163 655f 7961 6d6c 5f64 6963 7473  place_yaml_dicts
-00008bc0: 2829 2e0a 2020 2020 2020 2020 2020 2020  ()..            
-00008bd0: 7373 685f 7072 6f78 795f 636f 6d6d 616e  ssh_proxy_comman
-00008be0: 6420 3d20 4e6f 6e65 0a20 2020 2020 2020  d = None.       
-00008bf0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00008c00: 2020 2023 2028 3229 2057 6527 7265 206c     # (2) We're l
-00008c10: 6175 6e63 6869 6e67 2061 206e 6577 2063  aunching a new c
-00008c20: 6c75 7374 6572 2e0a 2020 2020 2020 2020  luster..        
-00008c30: 2020 2020 230a 2020 2020 2020 2020 2020      #.          
-00008c40: 2020 2320 5265 736f 7572 6365 732e 6765    # Resources.ge
-00008c50: 745f 7661 6c69 645f 7265 6769 6f6e 735f  t_valid_regions_
-00008c60: 666f 725f 6c61 756e 6368 6162 6c65 2829  for_launchable()
-00008c70: 2072 6573 7065 6374 7320 7468 6520 6b65   respects the ke
-00008c80: 7973 2028 7265 6769 6f6e 7329 0a20 2020  ys (regions).   
-00008c90: 2020 2020 2020 2020 2023 2069 6e20 7373           # in ss
-00008ca0: 685f 7072 6f78 795f 636f 6d6d 616e 6420  h_proxy_command 
-00008cb0: 696e 2073 6b79 7069 6c6f 745f 636f 6e66  in skypilot_conf
-00008cc0: 6967 2e20 536f 2068 6572 6520 7765 2061  ig. So here we a
-00008cd0: 6464 2061 6e20 6173 7365 7274 2e0a 2020  dd an assert..  
-00008ce0: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-00008cf0: 2072 6567 696f 6e5f 6e61 6d65 2069 6e20   region_name in 
-00008d00: 7373 685f 7072 6f78 795f 636f 6d6d 616e  ssh_proxy_comman
-00008d10: 645f 636f 6e66 6967 2c20 280a 2020 2020  d_config, (.    
-00008d20: 2020 2020 2020 2020 2020 2020 7265 6769              regi
-00008d30: 6f6e 5f6e 616d 652c 2073 7368 5f70 726f  on_name, ssh_pro
-00008d40: 7879 5f63 6f6d 6d61 6e64 5f63 6f6e 6669  xy_command_confi
-00008d50: 6729 0a20 2020 2020 2020 2020 2020 2073  g).            s
-00008d60: 7368 5f70 726f 7879 5f63 6f6d 6d61 6e64  sh_proxy_command
-00008d70: 203d 2073 7368 5f70 726f 7879 5f63 6f6d   = ssh_proxy_com
-00008d80: 6d61 6e64 5f63 6f6e 6669 675b 7265 6769  mand_config[regi
-00008d90: 6f6e 5f6e 616d 655d 0a20 2020 206c 6f67  on_name].    log
-00008da0: 6765 722e 6465 6275 6728 6627 5573 696e  ger.debug(f'Usin
-00008db0: 6720 7373 685f 7072 6f78 795f 636f 6d6d  g ssh_proxy_comm
-00008dc0: 616e 643a 207b 7373 685f 7072 6f78 795f  and: {ssh_proxy_
-00008dd0: 636f 6d6d 616e 6421 727d 2729 0a0a 2020  command!r}')..  
-00008de0: 2020 2320 5573 6572 2d73 7570 706c 6965    # User-supplie
-00008df0: 6420 676c 6f62 616c 2069 6e73 7461 6e63  d global instanc
-00008e00: 6520 7461 6773 2066 726f 6d20 7e2f 2e73  e tags from ~/.s
-00008e10: 6b79 2f63 6f6e 6669 672e 7961 6d6c 2e0a  ky/config.yaml..
-00008e20: 2020 2020 6c61 6265 6c73 203d 2073 6b79      labels = sky
-00008e30: 7069 6c6f 745f 636f 6e66 6967 2e67 6574  pilot_config.get
-00008e40: 5f6e 6573 7465 6428 2873 7472 2863 6c6f  _nested((str(clo
-00008e50: 7564 292e 6c6f 7765 7228 292c 2027 6c61  ud).lower(), 'la
-00008e60: 6265 6c73 2729 2c20 7b7d 290a 2020 2020  bels'), {}).    
-00008e70: 2320 4465 7072 6563 6174 6564 3a20 696e  # Deprecated: in
-00008e80: 7374 616e 6365 5f74 6167 7320 6861 7665  stance_tags have
-00008e90: 2062 6565 6e20 7265 706c 6163 6564 2062   been replaced b
-00008ea0: 7920 6c61 6265 6c73 2e20 466f 7220 6261  y labels. For ba
-00008eb0: 636b 7761 7264 0a20 2020 2023 2063 6f6d  ckward.    # com
-00008ec0: 7061 7469 6269 6c69 7479 2c20 7765 2073  patibility, we s
-00008ed0: 7570 706f 7274 2074 6865 6d20 616e 6420  upport them and 
-00008ee0: 7468 6520 7363 6865 6d61 2061 6c6c 6f77  the schema allow
-00008ef0: 7320 7468 656d 206f 6e6c 7920 6966 0a20  s them only if. 
-00008f00: 2020 2023 2060 6c61 6265 6c73 6020 6172     # `labels` ar
-00008f10: 6520 6e6f 7420 7370 6563 6966 6965 642e  e not specified.
-00008f20: 2054 6869 7320 7368 6f75 6c64 2062 6520   This should be 
-00008f30: 7265 6d6f 7665 6420 6166 7465 7220 302e  removed after 0.
-00008f40: 372e 302e 0a20 2020 206c 6162 656c 7320  7.0..    labels 
-00008f50: 3d20 736b 7970 696c 6f74 5f63 6f6e 6669  = skypilot_confi
-00008f60: 672e 6765 745f 6e65 7374 6564 2828 7374  g.get_nested((st
-00008f70: 7228 636c 6f75 6429 2e6c 6f77 6572 2829  r(cloud).lower()
-00008f80: 2c20 2769 6e73 7461 6e63 655f 7461 6773  , 'instance_tags
-00008f90: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-00008fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008fb0: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
-00008fc0: 6c73 290a 2020 2020 2320 6c61 6265 6c73  ls).    # labels
-00008fd0: 2069 7320 6120 6469 6374 2c20 7768 6963   is a dict, whic
-00008fe0: 6820 6973 2067 7561 7261 6e74 6565 6420  h is guaranteed 
-00008ff0: 6279 2074 6865 2074 7970 6520 6368 6563  by the type chec
-00009000: 6b20 696e 0a20 2020 2023 2073 6368 656d  k in.    # schem
-00009010: 6173 2e70 790a 2020 2020 6173 7365 7274  as.py.    assert
-00009020: 2069 7369 6e73 7461 6e63 6528 6c61 6265   isinstance(labe
-00009030: 6c73 2c20 6469 6374 292c 206c 6162 656c  ls, dict), label
-00009040: 730a 0a20 2020 2023 2047 6574 206c 6162  s..    # Get lab
-00009050: 656c 7320 6672 6f6d 2072 6573 6f75 7263  els from resourc
-00009060: 6573 2061 6e64 206f 7665 7272 6964 6520  es and override 
-00009070: 6672 6f6d 2074 6865 206c 6162 656c 7320  from the labels 
-00009080: 746f 5f70 726f 7669 7369 6f6e 2e0a 2020  to_provision..  
-00009090: 2020 6966 2074 6f5f 7072 6f76 6973 696f    if to_provisio
-000090a0: 6e2e 6c61 6265 6c73 3a0a 2020 2020 2020  n.labels:.      
-000090b0: 2020 6c61 6265 6c73 2e75 7064 6174 6528    labels.update(
-000090c0: 746f 5f70 726f 7669 7369 6f6e 2e6c 6162  to_provision.lab
-000090d0: 656c 7329 0a0a 2020 2020 2320 4475 6d70  els)..    # Dump
-000090e0: 2074 6865 2052 6179 2070 6f72 7473 2074   the Ray ports t
-000090f0: 6f20 6120 6669 6c65 2066 6f72 2052 6179  o a file for Ray
-00009100: 206a 6f62 2073 7562 6d69 7373 696f 6e0a   job submission.
-00009110: 2020 2020 6475 6d70 5f70 6f72 745f 636f      dump_port_co
-00009120: 6d6d 616e 6420 3d20 280a 2020 2020 2020  mmand = (.      
-00009130: 2020 6627 7b63 6f6e 7374 616e 7473 2e53    f'{constants.S
-00009140: 4b59 5f50 5954 484f 4e5f 434d 447d 202d  KY_PYTHON_CMD} -
-00009150: 6320 5c27 696d 706f 7274 206a 736f 6e2c  c \'import json,
-00009160: 206f 733b 206a 736f 6e2e 6475 6d70 287b   os; json.dump({
-00009170: 636f 6e73 7461 6e74 732e 534b 595f 5245  constants.SKY_RE
-00009180: 4d4f 5445 5f52 4159 5f50 4f52 545f 4449  MOTE_RAY_PORT_DI
-00009190: 4354 5f53 5452 7d2c 2027 0a20 2020 2020  CT_STR}, '.     
-000091a0: 2020 2066 276f 7065 6e28 6f73 2e70 6174     f'open(os.pat
-000091b0: 682e 6578 7061 6e64 7573 6572 2822 7b63  h.expanduser("{c
-000091c0: 6f6e 7374 616e 7473 2e53 4b59 5f52 454d  onstants.SKY_REM
-000091d0: 4f54 455f 5241 595f 504f 5254 5f46 494c  OTE_RAY_PORT_FIL
-000091e0: 457d 2229 2c20 2277 222c 2065 6e63 6f64  E}"), "w", encod
-000091f0: 696e 673d 2275 7466 2d38 2229 295c 2727  ing="utf-8"))\''
-00009200: 0a20 2020 2029 0a0a 2020 2020 2320 5573  .    )..    # Us
-00009210: 6520 6120 746d 7020 6669 6c65 2070 6174  e a tmp file pat
-00009220: 6820 746f 2061 766f 6964 2069 6e63 6f6d  h to avoid incom
-00009230: 706c 6574 6520 5941 4d4c 2066 696c 6520  plete YAML file 
-00009240: 6265 696e 6720 7265 2d75 7365 6420 696e  being re-used in
-00009250: 2074 6865 0a20 2020 2023 2066 7574 7572   the.    # futur
-00009260: 652e 0a20 2020 2074 6d70 5f79 616d 6c5f  e..    tmp_yaml_
-00009270: 7061 7468 203d 2079 616d 6c5f 7061 7468  path = yaml_path
-00009280: 202b 2027 2e74 6d70 270a 2020 2020 636f   + '.tmp'.    co
-00009290: 6d6d 6f6e 5f75 7469 6c73 2e66 696c 6c5f  mmon_utils.fill_
-000092a0: 7465 6d70 6c61 7465 280a 2020 2020 2020  template(.      
-000092b0: 2020 636c 7573 7465 725f 636f 6e66 6967    cluster_config
-000092c0: 5f74 656d 706c 6174 652c 0a20 2020 2020  _template,.     
-000092d0: 2020 2064 6963 7428 0a20 2020 2020 2020     dict(.       
-000092e0: 2020 2020 2072 6573 6f75 7263 6573 5f76       resources_v
-000092f0: 6172 732c 0a20 2020 2020 2020 2020 2020  ars,.           
-00009300: 202a 2a7b 0a20 2020 2020 2020 2020 2020   **{.           
-00009310: 2020 2020 2027 636c 7573 7465 725f 6e61       'cluster_na
-00009320: 6d65 5f6f 6e5f 636c 6f75 6427 3a20 636c  me_on_cloud': cl
+00008470: 2020 2020 2020 7363 6865 6d61 732e 6765        schemas.ge
+00008480: 745f 6465 6661 756c 745f 7265 6d6f 7465  t_default_remote
+00008490: 5f69 6465 6e74 6974 7928 7374 7228 636c  _identity(str(cl
+000084a0: 6f75 6429 2e6c 6f77 6572 2829 2929 0a20  oud).lower())). 
+000084b0: 2020 2069 6620 7265 6d6f 7465 5f69 6465     if remote_ide
+000084c0: 6e74 6974 7920 6973 206e 6f74 204e 6f6e  ntity is not Non
+000084d0: 6520 616e 6420 6e6f 7420 6973 696e 7374  e and not isinst
+000084e0: 616e 6365 2872 656d 6f74 655f 6964 656e  ance(remote_iden
+000084f0: 7469 7479 2c20 7374 7229 3a0a 2020 2020  tity, str):.    
+00008500: 2020 2020 666f 7220 7072 6f66 696c 6520      for profile 
+00008510: 696e 2072 656d 6f74 655f 6964 656e 7469  in remote_identi
+00008520: 7479 3a0a 2020 2020 2020 2020 2020 2020  ty:.            
+00008530: 6966 2066 6e6d 6174 6368 2e66 6e6d 6174  if fnmatch.fnmat
+00008540: 6368 6361 7365 2863 6c75 7374 6572 5f6e  chcase(cluster_n
+00008550: 616d 652c 206c 6973 7428 7072 6f66 696c  ame, list(profil
+00008560: 652e 6b65 7973 2829 295b 305d 293a 0a20  e.keys())[0]):. 
+00008570: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00008580: 656d 6f74 655f 6964 656e 7469 7479 203d  emote_identity =
+00008590: 206c 6973 7428 7072 6f66 696c 652e 7661   list(profile.va
+000085a0: 6c75 6573 2829 295b 305d 0a20 2020 2020  lues())[0].     
+000085b0: 2020 2020 2020 2020 2020 2062 7265 616b             break
+000085c0: 0a20 2020 2069 6620 7265 6d6f 7465 5f69  .    if remote_i
+000085d0: 6465 6e74 6974 7920 213d 2073 6368 656d  dentity != schem
+000085e0: 6173 2e52 656d 6f74 6549 6465 6e74 6974  as.RemoteIdentit
+000085f0: 794f 7074 696f 6e73 2e4c 4f43 414c 5f43  yOptions.LOCAL_C
+00008600: 5245 4445 4e54 4941 4c53 2e76 616c 7565  REDENTIALS.value
+00008610: 3a0a 2020 2020 2020 2020 6966 206e 6f74  :.        if not
+00008620: 2063 6c6f 7564 2e73 7570 706f 7274 735f   cloud.supports_
+00008630: 7365 7276 6963 655f 6163 636f 756e 745f  service_account_
+00008640: 6f6e 5f72 656d 6f74 6528 293a 0a20 2020  on_remote():.   
+00008650: 2020 2020 2020 2020 2072 6169 7365 2065           raise e
+00008660: 7863 6570 7469 6f6e 732e 496e 7661 6c69  xceptions.Invali
+00008670: 6443 6c6f 7564 436f 6e66 6967 7328 0a20  dCloudConfigs(. 
+00008680: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00008690: 7265 6d6f 7465 5f69 6465 6e74 6974 793a  remote_identity:
+000086a0: 2053 4552 5649 4345 5f41 4343 4f55 4e54   SERVICE_ACCOUNT
+000086b0: 2069 7320 7370 6563 6966 6965 6420 696e   is specified in
+000086c0: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
+000086d0: 2020 2066 277b 736b 7970 696c 6f74 5f63     f'{skypilot_c
+000086e0: 6f6e 6669 672e 6c6f 6164 6564 5f63 6f6e  onfig.loaded_con
+000086f0: 6669 675f 7061 7468 2172 7d20 666f 7220  fig_path!r} for 
+00008700: 7b63 6c6f 7564 7d2c 2062 7574 2069 7420  {cloud}, but it 
+00008710: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+00008720: 2020 2769 7320 6e6f 7420 7375 7070 6f72    'is not suppor
+00008730: 7465 6420 6279 2074 6869 7320 636c 6f75  ted by this clou
+00008740: 642e 2052 656d 6f76 6520 7468 6520 636f  d. Remove the co
+00008750: 6e66 6967 206f 7220 7365 743a 2027 0a20  nfig or set: '. 
+00008760: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00008770: 6072 656d 6f74 655f 6964 656e 7469 7479  `remote_identity
+00008780: 3a20 4c4f 4341 4c5f 4352 4544 454e 5449  : LOCAL_CREDENTI
+00008790: 414c 5360 2e27 290a 2020 2020 2020 2020  ALS`.').        
+000087a0: 6578 636c 7564 6564 5f63 6c6f 7564 7320  excluded_clouds 
+000087b0: 3d20 5b63 6c6f 7564 5d0a 2020 2020 6372  = [cloud].    cr
+000087c0: 6564 656e 7469 616c 7320 3d20 736b 795f  edentials = sky_
+000087d0: 6368 6563 6b2e 6765 745f 636c 6f75 645f  check.get_cloud_
+000087e0: 6372 6564 656e 7469 616c 5f66 696c 655f  credential_file_
+000087f0: 6d6f 756e 7473 2865 7863 6c75 6465 645f  mounts(excluded_
+00008800: 636c 6f75 6473 290a 0a20 2020 2061 7574  clouds)..    aut
+00008810: 685f 636f 6e66 6967 203d 207b 2773 7368  h_config = {'ssh
+00008820: 5f70 7269 7661 7465 5f6b 6579 273a 2061  _private_key': a
+00008830: 7574 682e 5052 4956 4154 455f 5353 485f  uth.PRIVATE_SSH_
+00008840: 4b45 595f 5041 5448 7d0a 2020 2020 7265  KEY_PATH}.    re
+00008850: 6769 6f6e 5f6e 616d 6520 3d20 7265 736f  gion_name = reso
+00008860: 7572 6365 735f 7661 7273 2e67 6574 2827  urces_vars.get('
+00008870: 7265 6769 6f6e 2729 0a0a 2020 2020 7961  region')..    ya
+00008880: 6d6c 5f70 6174 6820 3d20 5f67 6574 5f79  ml_path = _get_y
+00008890: 616d 6c5f 7061 7468 5f66 726f 6d5f 636c  aml_path_from_cl
+000088a0: 7573 7465 725f 6e61 6d65 2863 6c75 7374  uster_name(clust
+000088b0: 6572 5f6e 616d 6529 0a0a 2020 2020 2320  er_name)..    # 
+000088c0: 5265 7472 6965 7665 2074 6865 2073 7368  Retrieve the ssh
+000088d0: 5f70 726f 7879 5f63 6f6d 6d61 6e64 2066  _proxy_command f
+000088e0: 6f72 2074 6865 2067 6976 656e 2063 6c6f  or the given clo
+000088f0: 7564 202f 2072 6567 696f 6e2e 0a20 2020  ud / region..   
+00008900: 2073 7368 5f70 726f 7879 5f63 6f6d 6d61   ssh_proxy_comma
+00008910: 6e64 5f63 6f6e 6669 6720 3d20 736b 7970  nd_config = skyp
+00008920: 696c 6f74 5f63 6f6e 6669 672e 6765 745f  ilot_config.get_
+00008930: 6e65 7374 6564 280a 2020 2020 2020 2020  nested(.        
+00008940: 2873 7472 2863 6c6f 7564 292e 6c6f 7765  (str(cloud).lowe
+00008950: 7228 292c 2027 7373 685f 7072 6f78 795f  r(), 'ssh_proxy_
+00008960: 636f 6d6d 616e 6427 292c 204e 6f6e 6529  command'), None)
+00008970: 0a20 2020 2069 6620 2869 7369 6e73 7461  .    if (isinsta
+00008980: 6e63 6528 7373 685f 7072 6f78 795f 636f  nce(ssh_proxy_co
+00008990: 6d6d 616e 645f 636f 6e66 6967 2c20 7374  mmand_config, st
+000089a0: 7229 206f 720a 2020 2020 2020 2020 2020  r) or.          
+000089b0: 2020 7373 685f 7072 6f78 795f 636f 6d6d    ssh_proxy_comm
+000089c0: 616e 645f 636f 6e66 6967 2069 7320 4e6f  and_config is No
+000089d0: 6e65 293a 0a20 2020 2020 2020 2073 7368  ne):.        ssh
+000089e0: 5f70 726f 7879 5f63 6f6d 6d61 6e64 203d  _proxy_command =
+000089f0: 2073 7368 5f70 726f 7879 5f63 6f6d 6d61   ssh_proxy_comma
+00008a00: 6e64 5f63 6f6e 6669 670a 2020 2020 656c  nd_config.    el
+00008a10: 7365 3a0a 2020 2020 2020 2020 2320 7373  se:.        # ss
+00008a20: 685f 7072 6f78 795f 636f 6d6d 616e 645f  h_proxy_command_
+00008a30: 636f 6e66 6967 3a20 4469 6374 5b73 7472  config: Dict[str
+00008a40: 2c20 7374 725d 2c20 7265 6769 6f6e 5f6e  , str], region_n
+00008a50: 616d 6520 2d3e 2063 6f6d 6d61 6e64 0a20  ame -> command. 
+00008a60: 2020 2020 2020 2023 2054 6869 7320 7479         # This ty
+00008a70: 7065 2063 6865 636b 2069 7320 646f 6e65  pe check is done
+00008a80: 2062 7920 736b 7970 696c 6f74 5f63 6f6e   by skypilot_con
+00008a90: 6669 6720 6174 2063 6f6e 6669 6720 6c6f  fig at config lo
+00008aa0: 6164 2074 696d 652e 0a0a 2020 2020 2020  ad time...      
+00008ab0: 2020 2320 5468 6572 6520 6172 6520 7477    # There are tw
+00008ac0: 6f20 6361 7365 733a 0a20 2020 2020 2020  o cases:.       
+00008ad0: 2069 6620 6b65 6570 5f6c 6175 6e63 685f   if keep_launch_
+00008ae0: 6669 656c 6473 5f69 6e5f 6578 6973 7469  fields_in_existi
+00008af0: 6e67 5f63 6f6e 6669 673a 0a20 2020 2020  ng_config:.     
+00008b00: 2020 2020 2020 2023 2028 3129 2057 6527         # (1) We'
+00008b10: 7265 2072 652d 7072 6f76 6973 696f 6e69  re re-provisioni
+00008b20: 6e67 2061 6e20 6578 6973 7469 6e67 2063  ng an existing c
+00008b30: 6c75 7374 6572 2e0a 2020 2020 2020 2020  luster..        
+00008b40: 2020 2020 230a 2020 2020 2020 2020 2020      #.          
+00008b50: 2020 2320 5765 2075 7365 204e 6f6e 6520    # We use None 
+00008b60: 666f 7220 7373 685f 7072 6f78 795f 636f  for ssh_proxy_co
+00008b70: 6d6d 616e 642c 2077 6869 6368 2077 696c  mmand, which wil
+00008b80: 6c20 6265 2072 6573 746f 7265 6420 746f  l be restored to
+00008b90: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
+00008ba0: 2023 2063 6c75 7374 6572 2773 206f 7269   # cluster's ori
+00008bb0: 6769 6e61 6c20 7661 6c75 6520 6c61 7465  ginal value late
+00008bc0: 7220 6279 205f 7265 706c 6163 655f 7961  r by _replace_ya
+00008bd0: 6d6c 5f64 6963 7473 2829 2e0a 2020 2020  ml_dicts()..    
+00008be0: 2020 2020 2020 2020 7373 685f 7072 6f78          ssh_prox
+00008bf0: 795f 636f 6d6d 616e 6420 3d20 4e6f 6e65  y_command = None
+00008c00: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00008c10: 2020 2020 2020 2020 2020 2023 2028 3229             # (2)
+00008c20: 2057 6527 7265 206c 6175 6e63 6869 6e67   We're launching
+00008c30: 2061 206e 6577 2063 6c75 7374 6572 2e0a   a new cluster..
+00008c40: 2020 2020 2020 2020 2020 2020 230a 2020              #.  
+00008c50: 2020 2020 2020 2020 2020 2320 5265 736f            # Reso
+00008c60: 7572 6365 732e 6765 745f 7661 6c69 645f  urces.get_valid_
+00008c70: 7265 6769 6f6e 735f 666f 725f 6c61 756e  regions_for_laun
+00008c80: 6368 6162 6c65 2829 2072 6573 7065 6374  chable() respect
+00008c90: 7320 7468 6520 6b65 7973 2028 7265 6769  s the keys (regi
+00008ca0: 6f6e 7329 0a20 2020 2020 2020 2020 2020  ons).           
+00008cb0: 2023 2069 6e20 7373 685f 7072 6f78 795f   # in ssh_proxy_
+00008cc0: 636f 6d6d 616e 6420 696e 2073 6b79 7069  command in skypi
+00008cd0: 6c6f 745f 636f 6e66 6967 2e20 536f 2068  lot_config. So h
+00008ce0: 6572 6520 7765 2061 6464 2061 6e20 6173  ere we add an as
+00008cf0: 7365 7274 2e0a 2020 2020 2020 2020 2020  sert..          
+00008d00: 2020 6173 7365 7274 2072 6567 696f 6e5f    assert region_
+00008d10: 6e61 6d65 2069 6e20 7373 685f 7072 6f78  name in ssh_prox
+00008d20: 795f 636f 6d6d 616e 645f 636f 6e66 6967  y_command_config
+00008d30: 2c20 280a 2020 2020 2020 2020 2020 2020  , (.            
+00008d40: 2020 2020 7265 6769 6f6e 5f6e 616d 652c      region_name,
+00008d50: 2073 7368 5f70 726f 7879 5f63 6f6d 6d61   ssh_proxy_comma
+00008d60: 6e64 5f63 6f6e 6669 6729 0a20 2020 2020  nd_config).     
+00008d70: 2020 2020 2020 2073 7368 5f70 726f 7879         ssh_proxy
+00008d80: 5f63 6f6d 6d61 6e64 203d 2073 7368 5f70  _command = ssh_p
+00008d90: 726f 7879 5f63 6f6d 6d61 6e64 5f63 6f6e  roxy_command_con
+00008da0: 6669 675b 7265 6769 6f6e 5f6e 616d 655d  fig[region_name]
+00008db0: 0a20 2020 206c 6f67 6765 722e 6465 6275  .    logger.debu
+00008dc0: 6728 6627 5573 696e 6720 7373 685f 7072  g(f'Using ssh_pr
+00008dd0: 6f78 795f 636f 6d6d 616e 643a 207b 7373  oxy_command: {ss
+00008de0: 685f 7072 6f78 795f 636f 6d6d 616e 6421  h_proxy_command!
+00008df0: 727d 2729 0a0a 2020 2020 2320 5573 6572  r}')..    # User
+00008e00: 2d73 7570 706c 6965 6420 676c 6f62 616c  -supplied global
+00008e10: 2069 6e73 7461 6e63 6520 7461 6773 2066   instance tags f
+00008e20: 726f 6d20 7e2f 2e73 6b79 2f63 6f6e 6669  rom ~/.sky/confi
+00008e30: 672e 7961 6d6c 2e0a 2020 2020 6c61 6265  g.yaml..    labe
+00008e40: 6c73 203d 2073 6b79 7069 6c6f 745f 636f  ls = skypilot_co
+00008e50: 6e66 6967 2e67 6574 5f6e 6573 7465 6428  nfig.get_nested(
+00008e60: 2873 7472 2863 6c6f 7564 292e 6c6f 7765  (str(cloud).lowe
+00008e70: 7228 292c 2027 6c61 6265 6c73 2729 2c20  r(), 'labels'), 
+00008e80: 7b7d 290a 2020 2020 2320 4465 7072 6563  {}).    # Deprec
+00008e90: 6174 6564 3a20 696e 7374 616e 6365 5f74  ated: instance_t
+00008ea0: 6167 7320 6861 7665 2062 6565 6e20 7265  ags have been re
+00008eb0: 706c 6163 6564 2062 7920 6c61 6265 6c73  placed by labels
+00008ec0: 2e20 466f 7220 6261 636b 7761 7264 0a20  . For backward. 
+00008ed0: 2020 2023 2063 6f6d 7061 7469 6269 6c69     # compatibili
+00008ee0: 7479 2c20 7765 2073 7570 706f 7274 2074  ty, we support t
+00008ef0: 6865 6d20 616e 6420 7468 6520 7363 6865  hem and the sche
+00008f00: 6d61 2061 6c6c 6f77 7320 7468 656d 206f  ma allows them o
+00008f10: 6e6c 7920 6966 0a20 2020 2023 2060 6c61  nly if.    # `la
+00008f20: 6265 6c73 6020 6172 6520 6e6f 7420 7370  bels` are not sp
+00008f30: 6563 6966 6965 642e 2054 6869 7320 7368  ecified. This sh
+00008f40: 6f75 6c64 2062 6520 7265 6d6f 7665 6420  ould be removed 
+00008f50: 6166 7465 7220 302e 372e 302e 0a20 2020  after 0.7.0..   
+00008f60: 206c 6162 656c 7320 3d20 736b 7970 696c   labels = skypil
+00008f70: 6f74 5f63 6f6e 6669 672e 6765 745f 6e65  ot_config.get_ne
+00008f80: 7374 6564 2828 7374 7228 636c 6f75 6429  sted((str(cloud)
+00008f90: 2e6c 6f77 6572 2829 2c20 2769 6e73 7461  .lower(), 'insta
+00008fa0: 6e63 655f 7461 6773 2729 2c0a 2020 2020  nce_tags'),.    
+00008fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008fd0: 2020 2020 6c61 6265 6c73 290a 2020 2020      labels).    
+00008fe0: 2320 6c61 6265 6c73 2069 7320 6120 6469  # labels is a di
+00008ff0: 6374 2c20 7768 6963 6820 6973 2067 7561  ct, which is gua
+00009000: 7261 6e74 6565 6420 6279 2074 6865 2074  ranteed by the t
+00009010: 7970 6520 6368 6563 6b20 696e 0a20 2020  ype check in.   
+00009020: 2023 2073 6368 656d 6173 2e70 790a 2020   # schemas.py.  
+00009030: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
+00009040: 6e63 6528 6c61 6265 6c73 2c20 6469 6374  nce(labels, dict
+00009050: 292c 206c 6162 656c 730a 0a20 2020 2023  ), labels..    #
+00009060: 2047 6574 206c 6162 656c 7320 6672 6f6d   Get labels from
+00009070: 2072 6573 6f75 7263 6573 2061 6e64 206f   resources and o
+00009080: 7665 7272 6964 6520 6672 6f6d 2074 6865  verride from the
+00009090: 206c 6162 656c 7320 746f 5f70 726f 7669   labels to_provi
+000090a0: 7369 6f6e 2e0a 2020 2020 6966 2074 6f5f  sion..    if to_
+000090b0: 7072 6f76 6973 696f 6e2e 6c61 6265 6c73  provision.labels
+000090c0: 3a0a 2020 2020 2020 2020 6c61 6265 6c73  :.        labels
+000090d0: 2e75 7064 6174 6528 746f 5f70 726f 7669  .update(to_provi
+000090e0: 7369 6f6e 2e6c 6162 656c 7329 0a0a 2020  sion.labels)..  
+000090f0: 2020 2320 4475 6d70 2074 6865 2052 6179    # Dump the Ray
+00009100: 2070 6f72 7473 2074 6f20 6120 6669 6c65   ports to a file
+00009110: 2066 6f72 2052 6179 206a 6f62 2073 7562   for Ray job sub
+00009120: 6d69 7373 696f 6e0a 2020 2020 6475 6d70  mission.    dump
+00009130: 5f70 6f72 745f 636f 6d6d 616e 6420 3d20  _port_command = 
+00009140: 280a 2020 2020 2020 2020 6627 7b63 6f6e  (.        f'{con
+00009150: 7374 616e 7473 2e53 4b59 5f50 5954 484f  stants.SKY_PYTHO
+00009160: 4e5f 434d 447d 202d 6320 5c27 696d 706f  N_CMD} -c \'impo
+00009170: 7274 206a 736f 6e2c 206f 733b 206a 736f  rt json, os; jso
+00009180: 6e2e 6475 6d70 287b 636f 6e73 7461 6e74  n.dump({constant
+00009190: 732e 534b 595f 5245 4d4f 5445 5f52 4159  s.SKY_REMOTE_RAY
+000091a0: 5f50 4f52 545f 4449 4354 5f53 5452 7d2c  _PORT_DICT_STR},
+000091b0: 2027 0a20 2020 2020 2020 2066 276f 7065   '.        f'ope
+000091c0: 6e28 6f73 2e70 6174 682e 6578 7061 6e64  n(os.path.expand
+000091d0: 7573 6572 2822 7b63 6f6e 7374 616e 7473  user("{constants
+000091e0: 2e53 4b59 5f52 454d 4f54 455f 5241 595f  .SKY_REMOTE_RAY_
+000091f0: 504f 5254 5f46 494c 457d 2229 2c20 2277  PORT_FILE}"), "w
+00009200: 222c 2065 6e63 6f64 696e 673d 2275 7466  ", encoding="utf
+00009210: 2d38 2229 295c 2727 0a20 2020 2029 0a0a  -8"))\''.    )..
+00009220: 2020 2020 2320 5573 6520 6120 746d 7020      # Use a tmp 
+00009230: 6669 6c65 2070 6174 6820 746f 2061 766f  file path to avo
+00009240: 6964 2069 6e63 6f6d 706c 6574 6520 5941  id incomplete YA
+00009250: 4d4c 2066 696c 6520 6265 696e 6720 7265  ML file being re
+00009260: 2d75 7365 6420 696e 2074 6865 0a20 2020  -used in the.   
+00009270: 2023 2066 7574 7572 652e 0a20 2020 2074   # future..    t
+00009280: 6d70 5f79 616d 6c5f 7061 7468 203d 2079  mp_yaml_path = y
+00009290: 616d 6c5f 7061 7468 202b 2027 2e74 6d70  aml_path + '.tmp
+000092a0: 270a 2020 2020 636f 6d6d 6f6e 5f75 7469  '.    common_uti
+000092b0: 6c73 2e66 696c 6c5f 7465 6d70 6c61 7465  ls.fill_template
+000092c0: 280a 2020 2020 2020 2020 636c 7573 7465  (.        cluste
+000092d0: 725f 636f 6e66 6967 5f74 656d 706c 6174  r_config_templat
+000092e0: 652c 0a20 2020 2020 2020 2064 6963 7428  e,.        dict(
+000092f0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00009300: 6f75 7263 6573 5f76 6172 732c 0a20 2020  ources_vars,.   
+00009310: 2020 2020 2020 2020 202a 2a7b 0a20 2020           **{.   
+00009320: 2020 2020 2020 2020 2020 2020 2027 636c               'cl
 00009330: 7573 7465 725f 6e61 6d65 5f6f 6e5f 636c  uster_name_on_cl
-00009340: 6f75 642c 0a20 2020 2020 2020 2020 2020  oud,.           
-00009350: 2020 2020 2027 6e75 6d5f 6e6f 6465 7327       'num_nodes'
-00009360: 3a20 6e75 6d5f 6e6f 6465 732c 0a20 2020  : num_nodes,.   
-00009370: 2020 2020 2020 2020 2020 2020 2027 6469               'di
-00009380: 736b 5f73 697a 6527 3a20 746f 5f70 726f  sk_size': to_pro
-00009390: 7669 7369 6f6e 2e64 6973 6b5f 7369 7a65  vision.disk_size
-000093a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000093b0: 2020 2320 4966 2074 6865 2063 7572 7265    # If the curre
-000093c0: 6e74 2063 6f64 6520 6973 2072 756e 2062  nt code is run b
-000093d0: 7920 636f 6e74 726f 6c6c 6572 2c20 7072  y controller, pr
-000093e0: 6f70 6167 6174 6520 7468 6520 7265 616c  opagate the real
-000093f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009400: 2023 2063 616c 6c69 6e67 2075 7365 7220   # calling user 
-00009410: 7768 6963 6820 7368 6f75 6c64 2776 6520  which should've 
-00009420: 6265 656e 2070 6173 7365 6420 696e 2061  been passed in a
-00009430: 7320 7468 650a 2020 2020 2020 2020 2020  s the.          
-00009440: 2020 2020 2020 2320 534b 5950 494c 4f54        # SKYPILOT
-00009450: 5f55 5345 5220 656e 7620 7661 7220 2873  _USER env var (s
-00009460: 6565 0a20 2020 2020 2020 2020 2020 2020  ee.             
-00009470: 2020 2023 2063 6f6e 7472 6f6c 6c65 725f     # controller_
-00009480: 7574 696c 732e 7368 6172 6564 5f63 6f6e  utils.shared_con
-00009490: 7472 6f6c 6c65 725f 7661 7273 5f74 6f5f  troller_vars_to_
-000094a0: 6669 6c6c 2829 2e0a 2020 2020 2020 2020  fill()..        
-000094b0: 2020 2020 2020 2020 2775 7365 7227 3a20          'user': 
-000094c0: 636f 6d6d 6f6e 5f75 7469 6c73 2e67 6574  common_utils.get
-000094d0: 5f63 6c65 616e 6564 5f75 7365 726e 616d  _cleaned_usernam
-000094e0: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-000094f0: 2020 2020 2020 206f 732e 656e 7669 726f         os.enviro
-00009500: 6e2e 6765 7428 636f 6e73 7461 6e74 732e  n.get(constants.
-00009510: 5553 4552 5f45 4e56 5f56 4152 2c20 2727  USER_ENV_VAR, ''
-00009520: 2929 2c0a 0a20 2020 2020 2020 2020 2020  )),..           
-00009530: 2020 2020 2023 204e 6574 776f 726b 696e       # Networkin
-00009540: 6720 636f 6e66 6967 730a 2020 2020 2020  g configs.      
-00009550: 2020 2020 2020 2020 2020 2775 7365 5f69            'use_i
-00009560: 6e74 6572 6e61 6c5f 6970 7327 3a20 736b  nternal_ips': sk
-00009570: 7970 696c 6f74 5f63 6f6e 6669 672e 6765  ypilot_config.ge
-00009580: 745f 6e65 7374 6564 280a 2020 2020 2020  t_nested(.      
-00009590: 2020 2020 2020 2020 2020 2020 2020 2873                (s
-000095a0: 7472 2863 6c6f 7564 292e 6c6f 7765 7228  tr(cloud).lower(
-000095b0: 292c 2027 7573 655f 696e 7465 726e 616c  ), 'use_internal
-000095c0: 5f69 7073 2729 2c20 4661 6c73 6529 2c0a  _ips'), False),.
-000095d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095e0: 2773 7368 5f70 726f 7879 5f63 6f6d 6d61  'ssh_proxy_comma
-000095f0: 6e64 273a 2073 7368 5f70 726f 7879 5f63  nd': ssh_proxy_c
-00009600: 6f6d 6d61 6e64 2c0a 2020 2020 2020 2020  ommand,.        
-00009610: 2020 2020 2020 2020 2776 7063 5f6e 616d          'vpc_nam
-00009620: 6527 3a20 736b 7970 696c 6f74 5f63 6f6e  e': skypilot_con
-00009630: 6669 672e 6765 745f 6e65 7374 6564 280a  fig.get_nested(.
-00009640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009650: 2020 2020 2873 7472 2863 6c6f 7564 292e      (str(cloud).
-00009660: 6c6f 7765 7228 292c 2027 7670 635f 6e61  lower(), 'vpc_na
-00009670: 6d65 2729 2c20 4e6f 6e65 292c 0a0a 2020  me'), None),..  
-00009680: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00009690: 5573 6572 2d73 7570 706c 6965 6420 6c61  User-supplied la
-000096a0: 6265 6c73 2e0a 2020 2020 2020 2020 2020  bels..          
-000096b0: 2020 2020 2020 276c 6162 656c 7327 3a20        'labels': 
-000096c0: 6c61 6265 6c73 2c0a 2020 2020 2020 2020  labels,.        
-000096d0: 2020 2020 2020 2020 2320 5573 6572 2d73          # User-s
-000096e0: 7570 706c 6965 6420 7265 6d6f 7465 5f69  upplied remote_i
-000096f0: 6465 6e74 6974 790a 2020 2020 2020 2020  dentity.        
-00009700: 2020 2020 2020 2020 2772 656d 6f74 655f          'remote_
-00009710: 6964 656e 7469 7479 273a 2072 656d 6f74  identity': remot
-00009720: 655f 6964 656e 7469 7479 2c0a 2020 2020  e_identity,.    
-00009730: 2020 2020 2020 2020 2020 2020 2320 5468              # Th
-00009740: 6520 7265 7365 7276 6174 696f 6e20 706f  e reservation po
-00009750: 6f6c 7320 7468 6174 2073 7065 6369 6669  ols that specifi
-00009760: 6564 2062 7920 7468 6520 7573 6572 2e20  ed by the user. 
-00009770: 5468 6973 2069 730a 2020 2020 2020 2020  This is.        
-00009780: 2020 2020 2020 2020 2320 6375 7272 656e          # curren
-00009790: 746c 7920 6f6e 6c79 2075 7365 6420 6279  tly only used by
-000097a0: 2047 4350 2e0a 2020 2020 2020 2020 2020   GCP..          
-000097b0: 2020 2020 2020 2773 7065 6369 6669 635f        'specific_
-000097c0: 7265 7365 7276 6174 696f 6e73 273a 2073  reservations': s
+00009340: 6f75 6427 3a20 636c 7573 7465 725f 6e61  oud': cluster_na
+00009350: 6d65 5f6f 6e5f 636c 6f75 642c 0a20 2020  me_on_cloud,.   
+00009360: 2020 2020 2020 2020 2020 2020 2027 6e75               'nu
+00009370: 6d5f 6e6f 6465 7327 3a20 6e75 6d5f 6e6f  m_nodes': num_no
+00009380: 6465 732c 0a20 2020 2020 2020 2020 2020  des,.           
+00009390: 2020 2020 2027 6469 736b 5f73 697a 6527       'disk_size'
+000093a0: 3a20 746f 5f70 726f 7669 7369 6f6e 2e64  : to_provision.d
+000093b0: 6973 6b5f 7369 7a65 2c0a 2020 2020 2020  isk_size,.      
+000093c0: 2020 2020 2020 2020 2020 2320 4966 2074            # If t
+000093d0: 6865 2063 7572 7265 6e74 2063 6f64 6520  he current code 
+000093e0: 6973 2072 756e 2062 7920 636f 6e74 726f  is run by contro
+000093f0: 6c6c 6572 2c20 7072 6f70 6167 6174 6520  ller, propagate 
+00009400: 7468 6520 7265 616c 0a20 2020 2020 2020  the real.       
+00009410: 2020 2020 2020 2020 2023 2063 616c 6c69           # calli
+00009420: 6e67 2075 7365 7220 7768 6963 6820 7368  ng user which sh
+00009430: 6f75 6c64 2776 6520 6265 656e 2070 6173  ould've been pas
+00009440: 7365 6420 696e 2061 7320 7468 650a 2020  sed in as the.  
+00009450: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00009460: 534b 5950 494c 4f54 5f55 5345 5220 656e  SKYPILOT_USER en
+00009470: 7620 7661 7220 2873 6565 0a20 2020 2020  v var (see.     
+00009480: 2020 2020 2020 2020 2020 2023 2063 6f6e             # con
+00009490: 7472 6f6c 6c65 725f 7574 696c 732e 7368  troller_utils.sh
+000094a0: 6172 6564 5f63 6f6e 7472 6f6c 6c65 725f  ared_controller_
+000094b0: 7661 7273 5f74 6f5f 6669 6c6c 2829 2e0a  vars_to_fill()..
+000094c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000094d0: 2775 7365 7227 3a20 636f 6d6d 6f6e 5f75  'user': common_u
+000094e0: 7469 6c73 2e67 6574 5f63 6c65 616e 6564  tils.get_cleaned
+000094f0: 5f75 7365 726e 616d 6528 0a20 2020 2020  _username(.     
+00009500: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00009510: 732e 656e 7669 726f 6e2e 6765 7428 636f  s.environ.get(co
+00009520: 6e73 7461 6e74 732e 5553 4552 5f45 4e56  nstants.USER_ENV
+00009530: 5f56 4152 2c20 2727 2929 2c0a 0a20 2020  _VAR, '')),..   
+00009540: 2020 2020 2020 2020 2020 2020 2023 204e               # N
+00009550: 6574 776f 726b 696e 6720 636f 6e66 6967  etworking config
+00009560: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00009570: 2020 2775 7365 5f69 6e74 6572 6e61 6c5f    'use_internal_
+00009580: 6970 7327 3a20 736b 7970 696c 6f74 5f63  ips': skypilot_c
+00009590: 6f6e 6669 672e 6765 745f 6e65 7374 6564  onfig.get_nested
+000095a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000095b0: 2020 2020 2020 2873 7472 2863 6c6f 7564        (str(cloud
+000095c0: 292e 6c6f 7765 7228 292c 2027 7573 655f  ).lower(), 'use_
+000095d0: 696e 7465 726e 616c 5f69 7073 2729 2c20  internal_ips'), 
+000095e0: 4661 6c73 6529 2c0a 2020 2020 2020 2020  False),.        
+000095f0: 2020 2020 2020 2020 2773 7368 5f70 726f          'ssh_pro
+00009600: 7879 5f63 6f6d 6d61 6e64 273a 2073 7368  xy_command': ssh
+00009610: 5f70 726f 7879 5f63 6f6d 6d61 6e64 2c0a  _proxy_command,.
+00009620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009630: 2776 7063 5f6e 616d 6527 3a20 736b 7970  'vpc_name': skyp
+00009640: 696c 6f74 5f63 6f6e 6669 672e 6765 745f  ilot_config.get_
+00009650: 6e65 7374 6564 280a 2020 2020 2020 2020  nested(.        
+00009660: 2020 2020 2020 2020 2020 2020 2873 7472              (str
+00009670: 2863 6c6f 7564 292e 6c6f 7765 7228 292c  (cloud).lower(),
+00009680: 2027 7670 635f 6e61 6d65 2729 2c20 4e6f   'vpc_name'), No
+00009690: 6e65 292c 0a0a 2020 2020 2020 2020 2020  ne),..          
+000096a0: 2020 2020 2020 2320 5573 6572 2d73 7570        # User-sup
+000096b0: 706c 6965 6420 6c61 6265 6c73 2e0a 2020  plied labels..  
+000096c0: 2020 2020 2020 2020 2020 2020 2020 276c                'l
+000096d0: 6162 656c 7327 3a20 6c61 6265 6c73 2c0a  abels': labels,.
+000096e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096f0: 2320 5573 6572 2d73 7570 706c 6965 6420  # User-supplied 
+00009700: 7265 6d6f 7465 5f69 6465 6e74 6974 790a  remote_identity.
+00009710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009720: 2772 656d 6f74 655f 6964 656e 7469 7479  'remote_identity
+00009730: 273a 2072 656d 6f74 655f 6964 656e 7469  ': remote_identi
+00009740: 7479 2c0a 2020 2020 2020 2020 2020 2020  ty,.            
+00009750: 2020 2020 2320 5468 6520 7265 7365 7276      # The reserv
+00009760: 6174 696f 6e20 706f 6f6c 7320 7468 6174  ation pools that
+00009770: 2073 7065 6369 6669 6564 2062 7920 7468   specified by th
+00009780: 6520 7573 6572 2e20 5468 6973 2069 730a  e user. This is.
+00009790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000097a0: 2320 6375 7272 656e 746c 7920 6f6e 6c79  # currently only
+000097b0: 2075 7365 6420 6279 2047 4350 2e0a 2020   used by GCP..  
+000097c0: 2020 2020 2020 2020 2020 2020 2020 2773                's
 000097d0: 7065 6369 6669 635f 7265 7365 7276 6174  pecific_reservat
-000097e0: 696f 6e73 2c0a 0a20 2020 2020 2020 2020  ions,..         
-000097f0: 2020 2020 2020 2023 2043 6f6e 6461 2073         # Conda s
-00009800: 6574 7570 0a20 2020 2020 2020 2020 2020  etup.           
-00009810: 2020 2020 2027 636f 6e64 615f 696e 7374       'conda_inst
-00009820: 616c 6c61 7469 6f6e 5f63 6f6d 6d61 6e64  allation_command
-00009830: 7327 3a0a 2020 2020 2020 2020 2020 2020  s':.            
-00009840: 2020 2020 2020 2020 636f 6e73 7461 6e74          constant
-00009850: 732e 434f 4e44 415f 494e 5354 414c 4c41  s.CONDA_INSTALLA
-00009860: 5449 4f4e 5f43 4f4d 4d41 4e44 532c 0a20  TION_COMMANDS,. 
-00009870: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00009880: 2057 6520 7368 6f75 6c64 206e 6f74 2075   We should not u
-00009890: 7365 2060 2e66 6f72 6d61 7460 2c20 6173  se `.format`, as
-000098a0: 2069 7420 636f 6e74 6169 6e73 2027 7b7d   it contains '{}
-000098b0: 2720 6173 2074 6865 2062 6173 680a 2020  ' as the bash.  
-000098c0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-000098d0: 7379 6e74 6178 2e0a 2020 2020 2020 2020  syntax..        
-000098e0: 2020 2020 2020 2020 2772 6179 5f73 6b79          'ray_sky
-000098f0: 7069 6c6f 745f 696e 7374 616c 6c61 7469  pilot_installati
-00009900: 6f6e 5f63 6f6d 6d61 6e64 7327 3a0a 2020  on_commands':.  
-00009910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009920: 2020 2863 6f6e 7374 616e 7473 2e52 4159    (constants.RAY
-00009930: 5f53 4b59 5049 4c4f 545f 494e 5354 414c  _SKYPILOT_INSTAL
-00009940: 4c41 5449 4f4e 5f43 4f4d 4d41 4e44 532e  LATION_COMMANDS.
-00009950: 7265 706c 6163 6528 0a20 2020 2020 2020  replace(.       
-00009960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009970: 2027 7b73 6b79 5f77 6865 656c 5f68 6173   '{sky_wheel_has
-00009980: 687d 272c 0a20 2020 2020 2020 2020 2020  h}',.           
-00009990: 2020 2020 2020 2020 2020 2020 2077 6865               whe
-000099a0: 656c 5f68 6173 6829 2e72 6570 6c61 6365  el_hash).replace
-000099b0: 2827 7b63 6c6f 7564 7d27 2c0a 2020 2020  ('{cloud}',.    
-000099c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099e0: 2020 2020 2020 2020 7374 7228 636c 6f75          str(clou
-000099f0: 6429 2e6c 6f77 6572 2829 2929 2c0a 0a20  d).lower())),.. 
-00009a00: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00009a10: 2050 6f72 7420 6f66 2052 6179 2028 4743   Port of Ray (GC
-00009a20: 5320 7365 7276 6572 292e 0a20 2020 2020  S server)..     
-00009a30: 2020 2020 2020 2020 2020 2023 2052 6179             # Ray
-00009a40: 2773 2064 6566 6175 6c74 2070 6f72 7420  's default port 
-00009a50: 3633 3739 2069 7320 636f 6e66 6c69 6374  6379 is conflict
-00009a60: 6564 2077 6974 6820 5265 6469 732e 0a20  ed with Redis.. 
-00009a70: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00009a80: 7261 795f 706f 7274 273a 2063 6f6e 7374  ray_port': const
-00009a90: 616e 7473 2e53 4b59 5f52 454d 4f54 455f  ants.SKY_REMOTE_
-00009aa0: 5241 595f 504f 5254 2c0a 2020 2020 2020  RAY_PORT,.      
-00009ab0: 2020 2020 2020 2020 2020 2772 6179 5f64            'ray_d
-00009ac0: 6173 6862 6f61 7264 5f70 6f72 7427 3a20  ashboard_port': 
-00009ad0: 636f 6e73 7461 6e74 732e 534b 595f 5245  constants.SKY_RE
-00009ae0: 4d4f 5445 5f52 4159 5f44 4153 4842 4f41  MOTE_RAY_DASHBOA
-00009af0: 5244 5f50 4f52 542c 0a20 2020 2020 2020  RD_PORT,.       
-00009b00: 2020 2020 2020 2020 2027 7261 795f 7465           'ray_te
-00009b10: 6d70 5f64 6972 273a 2063 6f6e 7374 616e  mp_dir': constan
-00009b20: 7473 2e53 4b59 5f52 454d 4f54 455f 5241  ts.SKY_REMOTE_RA
-00009b30: 595f 5445 4d50 4449 522c 0a20 2020 2020  Y_TEMPDIR,.     
-00009b40: 2020 2020 2020 2020 2020 2027 6475 6d70             'dump
-00009b50: 5f70 6f72 745f 636f 6d6d 616e 6427 3a20  _port_command': 
-00009b60: 6475 6d70 5f70 6f72 745f 636f 6d6d 616e  dump_port_comman
-00009b70: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-00009b80: 2020 2023 2053 6b79 2d69 6e74 6572 6e61     # Sky-interna
-00009b90: 6c20 636f 6e73 7461 6e74 732e 0a20 2020  l constants..   
-00009ba0: 2020 2020 2020 2020 2020 2020 2027 736b               'sk
-00009bb0: 795f 7261 795f 636d 6427 3a20 636f 6e73  y_ray_cmd': cons
-00009bc0: 7461 6e74 732e 534b 595f 5241 595f 434d  tants.SKY_RAY_CM
-00009bd0: 442c 0a20 2020 2020 2020 2020 2020 2020  D,.             
-00009be0: 2020 2027 736b 795f 7069 705f 636d 6427     'sky_pip_cmd'
-00009bf0: 3a20 636f 6e73 7461 6e74 732e 534b 595f  : constants.SKY_
-00009c00: 5049 505f 434d 442c 0a20 2020 2020 2020  PIP_CMD,.       
-00009c10: 2020 2020 2020 2020 2027 7261 795f 7665           'ray_ve
-00009c20: 7273 696f 6e27 3a20 636f 6e73 7461 6e74  rsion': constant
-00009c30: 732e 534b 595f 5245 4d4f 5445 5f52 4159  s.SKY_REMOTE_RAY
-00009c40: 5f56 4552 5349 4f4e 2c0a 2020 2020 2020  _VERSION,.      
-00009c50: 2020 2020 2020 2020 2020 2320 436f 6d6d            # Comm
-00009c60: 616e 6420 666f 7220 7761 6974 696e 6720  and for waiting 
-00009c70: 7261 7920 636c 7573 7465 7220 746f 2062  ray cluster to b
-00009c80: 6520 7265 6164 7920 6f6e 2068 6561 642e  e ready on head.
-00009c90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009ca0: 2027 7261 795f 6865 6164 5f77 6169 745f   'ray_head_wait_
-00009cb0: 696e 6974 6961 6c69 7a65 645f 636f 6d6d  initialized_comm
-00009cc0: 616e 6427 3a0a 2020 2020 2020 2020 2020  and':.          
-00009cd0: 2020 2020 2020 2020 2020 696e 7374 616e            instan
-00009ce0: 6365 5f73 6574 7570 2e52 4159 5f48 4541  ce_setup.RAY_HEA
-00009cf0: 445f 5741 4954 5f49 4e49 5449 414c 495a  D_WAIT_INITIALIZ
-00009d00: 4544 5f43 4f4d 4d41 4e44 2c0a 0a20 2020  ED_COMMAND,..   
-00009d10: 2020 2020 2020 2020 2020 2020 2023 2043               # C
-00009d20: 6c6f 7564 2063 7265 6465 6e74 6961 6c73  loud credentials
-00009d30: 2066 6f72 2063 6c6f 7564 2073 746f 7261   for cloud stora
-00009d40: 6765 2e0a 2020 2020 2020 2020 2020 2020  ge..            
-00009d50: 2020 2020 2763 7265 6465 6e74 6961 6c73      'credentials
-00009d60: 273a 2063 7265 6465 6e74 6961 6c73 2c0a  ': credentials,.
-00009d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d80: 2320 536b 7920 7265 6d6f 7465 2075 7469  # Sky remote uti
-00009d90: 6c73 2e0a 2020 2020 2020 2020 2020 2020  ls..            
-00009da0: 2020 2020 2773 6b79 5f72 656d 6f74 655f      'sky_remote_
-00009db0: 7061 7468 273a 2053 4b59 5f52 454d 4f54  path': SKY_REMOT
-00009dc0: 455f 5041 5448 2c0a 2020 2020 2020 2020  E_PATH,.        
-00009dd0: 2020 2020 2020 2020 2773 6b79 5f6c 6f63          'sky_loc
-00009de0: 616c 5f70 6174 6827 3a20 7374 7228 6c6f  al_path': str(lo
-00009df0: 6361 6c5f 7768 6565 6c5f 7061 7468 292c  cal_wheel_path),
-00009e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009e10: 2023 2041 6464 2079 616d 6c20 6669 6c65   # Add yaml file
-00009e20: 2070 6174 6820 746f 2074 6865 2074 656d   path to the tem
-00009e30: 706c 6174 6520 7661 7269 6162 6c65 732e  plate variables.
-00009e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009e50: 2027 736b 795f 7261 795f 7961 6d6c 5f72   'sky_ray_yaml_r
-00009e60: 656d 6f74 655f 7061 7468 273a 0a20 2020  emote_path':.   
-00009e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e80: 2063 6c75 7374 6572 5f79 616d 6c5f 7574   cluster_yaml_ut
-00009e90: 696c 732e 534b 595f 434c 5553 5445 525f  ils.SKY_CLUSTER_
-00009ea0: 5941 4d4c 5f52 454d 4f54 455f 5041 5448  YAML_REMOTE_PATH
-00009eb0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00009ec0: 2020 2773 6b79 5f72 6179 5f79 616d 6c5f    'sky_ray_yaml_
-00009ed0: 6c6f 6361 6c5f 7061 7468 273a 2074 6d70  local_path': tmp
-00009ee0: 5f79 616d 6c5f 7061 7468 2c0a 2020 2020  _yaml_path,.    
-00009ef0: 2020 2020 2020 2020 2020 2020 2773 6b79              'sky
-00009f00: 5f76 6572 7369 6f6e 273a 2073 7472 2876  _version': str(v
-00009f10: 6572 7369 6f6e 2e70 6172 7365 2873 6b79  ersion.parse(sky
-00009f20: 2e5f 5f76 6572 7369 6f6e 5f5f 2929 2c0a  .__version__)),.
-00009f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f40: 2773 6b79 5f77 6865 656c 5f68 6173 6827  'sky_wheel_hash'
-00009f50: 3a20 7768 6565 6c5f 6861 7368 2c0a 2020  : wheel_hash,.  
-00009f60: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00009f70: 4175 7468 656e 7469 6361 7469 6f6e 2028  Authentication (
-00009f80: 6f70 7469 6f6e 616c 292e 0a20 2020 2020  optional)..     
-00009f90: 2020 2020 2020 2020 2020 202a 2a61 7574             **aut
-00009fa0: 685f 636f 6e66 6967 2c0a 2020 2020 2020  h_config,.      
-00009fb0: 2020 2020 2020 7d29 2c0a 2020 2020 2020        }),.      
-00009fc0: 2020 6f75 7470 7574 5f70 6174 683d 746d    output_path=tm
-00009fd0: 705f 7961 6d6c 5f70 6174 6829 0a20 2020  p_yaml_path).   
-00009fe0: 2063 6f6e 6669 675f 6469 6374 5b27 636c   config_dict['cl
-00009ff0: 7573 7465 725f 6e61 6d65 275d 203d 2063  uster_name'] = c
-0000a000: 6c75 7374 6572 5f6e 616d 650a 2020 2020  luster_name.    
-0000a010: 636f 6e66 6967 5f64 6963 745b 2772 6179  config_dict['ray
-0000a020: 275d 203d 2079 616d 6c5f 7061 7468 0a20  '] = yaml_path. 
-0000a030: 2020 2069 6620 6472 7972 756e 3a0a 2020     if dryrun:.  
-0000a040: 2020 2020 2020 2320 4966 2064 7279 7275        # If dryru
-0000a050: 6e2c 2072 6574 7572 6e20 7468 6520 756e  n, return the un
-0000a060: 6669 6e69 7368 6564 2074 6d70 2079 616d  finished tmp yam
-0000a070: 6c20 7061 7468 2e0a 2020 2020 2020 2020  l path..        
-0000a080: 636f 6e66 6967 5f64 6963 745b 2772 6179  config_dict['ray
-0000a090: 275d 203d 2074 6d70 5f79 616d 6c5f 7061  '] = tmp_yaml_pa
-0000a0a0: 7468 0a20 2020 2020 2020 2072 6574 7572  th.        retur
-0000a0b0: 6e20 636f 6e66 6967 5f64 6963 740a 2020  n config_dict.  
-0000a0c0: 2020 5f61 6464 5f61 7574 685f 746f 5f63    _add_auth_to_c
-0000a0d0: 6c75 7374 6572 5f63 6f6e 6669 6728 636c  luster_config(cl
-0000a0e0: 6f75 642c 2074 6d70 5f79 616d 6c5f 7061  oud, tmp_yaml_pa
-0000a0f0: 7468 290a 0a20 2020 2023 2041 6464 206b  th)..    # Add k
-0000a100: 7562 6572 6e65 7465 7320 636f 6e66 6967  ubernetes config
-0000a110: 2066 6965 6c64 7320 6672 6f6d 207e 2f2e   fields from ~/.
-0000a120: 736b 792f 636f 6e66 6967 0a20 2020 2069  sky/config.    i
-0000a130: 6620 6973 696e 7374 616e 6365 2863 6c6f  f isinstance(clo
-0000a140: 7564 2c20 636c 6f75 6473 2e4b 7562 6572  ud, clouds.Kuber
-0000a150: 6e65 7465 7329 3a0a 2020 2020 2020 2020  netes):.        
-0000a160: 6b75 6265 726e 6574 6573 5f75 7469 6c73  kubernetes_utils
-0000a170: 2e63 6f6d 6269 6e65 5f70 6f64 5f63 6f6e  .combine_pod_con
-0000a180: 6669 675f 6669 656c 6473 2874 6d70 5f79  fig_fields(tmp_y
-0000a190: 616d 6c5f 7061 7468 290a 2020 2020 2020  aml_path).      
-0000a1a0: 2020 6b75 6265 726e 6574 6573 5f75 7469    kubernetes_uti
-0000a1b0: 6c73 2e63 6f6d 6269 6e65 5f6d 6574 6164  ls.combine_metad
-0000a1c0: 6174 615f 6669 656c 6473 2874 6d70 5f79  ata_fields(tmp_y
-0000a1d0: 616d 6c5f 7061 7468 290a 0a20 2020 2023  aml_path)..    #
-0000a1e0: 2052 6573 746f 7265 2074 6865 206f 6c64   Restore the old
-0000a1f0: 2079 616d 6c20 636f 6e74 656e 7420 666f   yaml content fo
-0000a200: 7220 6261 636b 7761 7264 2063 6f6d 7061  r backward compa
-0000a210: 7469 6269 6c69 7479 2e0a 2020 2020 6966  tibility..    if
-0000a220: 206f 732e 7061 7468 2e65 7869 7374 7328   os.path.exists(
-0000a230: 7961 6d6c 5f70 6174 6829 2061 6e64 206b  yaml_path) and k
-0000a240: 6565 705f 6c61 756e 6368 5f66 6965 6c64  eep_launch_field
-0000a250: 735f 696e 5f65 7869 7374 696e 675f 636f  s_in_existing_co
-0000a260: 6e66 6967 3a0a 2020 2020 2020 2020 7769  nfig:.        wi
-0000a270: 7468 206f 7065 6e28 7961 6d6c 5f70 6174  th open(yaml_pat
-0000a280: 682c 2027 7227 2c20 656e 636f 6469 6e67  h, 'r', encoding
-0000a290: 3d27 7574 662d 3827 2920 6173 2066 3a0a  ='utf-8') as f:.
-0000a2a0: 2020 2020 2020 2020 2020 2020 6f6c 645f              old_
-0000a2b0: 7961 6d6c 5f63 6f6e 7465 6e74 203d 2066  yaml_content = f
-0000a2c0: 2e72 6561 6428 290a 2020 2020 2020 2020  .read().        
-0000a2d0: 7769 7468 206f 7065 6e28 746d 705f 7961  with open(tmp_ya
-0000a2e0: 6d6c 5f70 6174 682c 2027 7227 2c20 656e  ml_path, 'r', en
-0000a2f0: 636f 6469 6e67 3d27 7574 662d 3827 2920  coding='utf-8') 
-0000a300: 6173 2066 3a0a 2020 2020 2020 2020 2020  as f:.          
-0000a310: 2020 6e65 775f 7961 6d6c 5f63 6f6e 7465    new_yaml_conte
-0000a320: 6e74 203d 2066 2e72 6561 6428 290a 2020  nt = f.read().  
-0000a330: 2020 2020 2020 7265 7374 6f72 6564 5f79        restored_y
-0000a340: 616d 6c5f 636f 6e74 656e 7420 3d20 5f72  aml_content = _r
-0000a350: 6570 6c61 6365 5f79 616d 6c5f 6469 6374  eplace_yaml_dict
-0000a360: 7328 0a20 2020 2020 2020 2020 2020 206e  s(.            n
-0000a370: 6577 5f79 616d 6c5f 636f 6e74 656e 742c  ew_yaml_content,
-0000a380: 206f 6c64 5f79 616d 6c5f 636f 6e74 656e   old_yaml_conten
-0000a390: 742c 0a20 2020 2020 2020 2020 2020 205f  t,.            _
-0000a3a0: 5241 595f 5941 4d4c 5f4b 4559 535f 544f  RAY_YAML_KEYS_TO
-0000a3b0: 5f52 4553 544f 5245 5f46 4f52 5f42 4143  _RESTORE_FOR_BAC
-0000a3c0: 4b5f 434f 4d50 4154 4942 494c 4954 592c  K_COMPATIBILITY,
-0000a3d0: 0a20 2020 2020 2020 2020 2020 205f 5241  .            _RA
-0000a3e0: 595f 5941 4d4c 5f4b 4559 535f 544f 5f52  Y_YAML_KEYS_TO_R
-0000a3f0: 4553 544f 5245 5f45 5843 4550 5449 4f4e  ESTORE_EXCEPTION
-0000a400: 5329 0a20 2020 2020 2020 2077 6974 6820  S).        with 
-0000a410: 6f70 656e 2874 6d70 5f79 616d 6c5f 7061  open(tmp_yaml_pa
-0000a420: 7468 2c20 2777 272c 2065 6e63 6f64 696e  th, 'w', encodin
-0000a430: 673d 2775 7466 2d38 2729 2061 7320 663a  g='utf-8') as f:
-0000a440: 0a20 2020 2020 2020 2020 2020 2066 2e77  .            f.w
-0000a450: 7269 7465 2872 6573 746f 7265 645f 7961  rite(restored_ya
-0000a460: 6d6c 5f63 6f6e 7465 6e74 290a 0a20 2020  ml_content)..   
-0000a470: 2063 6f6e 6669 675f 6469 6374 5b27 636c   config_dict['cl
-0000a480: 7573 7465 725f 6e61 6d65 5f6f 6e5f 636c  uster_name_on_cl
-0000a490: 6f75 6427 5d20 3d20 636c 7573 7465 725f  oud'] = cluster_
-0000a4a0: 6e61 6d65 5f6f 6e5f 636c 6f75 640a 0a20  name_on_cloud.. 
-0000a4b0: 2020 2023 204f 7074 696d 697a 6174 696f     # Optimizatio
-0000a4c0: 6e3a 2063 6f70 7920 7468 6520 636f 6e74  n: copy the cont
-0000a4d0: 656e 7473 206f 6620 736f 7572 6365 2066  ents of source f
-0000a4e0: 696c 6573 2069 6e20 6669 6c65 5f6d 6f75  iles in file_mou
-0000a4f0: 6e74 7320 746f 2061 0a20 2020 2023 2073  nts to a.    # s
-0000a500: 7065 6369 616c 2064 6972 2c20 616e 6420  pecial dir, and 
-0000a510: 7570 6c6f 6164 2074 6861 7420 6173 2074  upload that as t
-0000a520: 6865 206f 6e6c 7920 6669 6c65 5f6d 6f75  he only file_mou
-0000a530: 6e74 2069 6e73 7465 6164 2e20 4465 6c61  nt instead. Dela
-0000a540: 790a 2020 2020 2320 6361 6c6c 696e 6720  y.    # calling 
-0000a550: 7468 6973 206f 7074 696d 697a 6174 696f  this optimizatio
-0000a560: 6e20 756e 7469 6c20 6e6f 772c 2077 6865  n until now, whe
-0000a570: 6e20 616c 6c20 736f 7572 6365 2066 696c  n all source fil
-0000a580: 6573 2068 6176 6520 6265 656e 0a20 2020  es have been.   
-0000a590: 2023 2077 7269 7474 656e 2061 6e64 2074   # written and t
-0000a5a0: 6865 6972 2063 6f6e 7465 6e74 7320 6669  heir contents fi
-0000a5b0: 6e61 6c69 7a65 642e 0a20 2020 2023 0a20  nalized..    #. 
-0000a5c0: 2020 2023 204e 6f74 6520 7468 6174 2074     # Note that t
-0000a5d0: 6865 2072 6179 2079 616d 6c20 6669 6c65  he ray yaml file
-0000a5e0: 2077 696c 6c20 6265 2063 6f70 6965 6420   will be copied 
-0000a5f0: 696e 746f 2074 6861 7420 7370 6563 6961  into that specia
-0000a600: 6c20 6469 7220 2869 2e65 2e2c 0a20 2020  l dir (i.e.,.   
-0000a610: 2023 2075 706c 6f61 6465 6420 6173 2070   # uploaded as p
-0000a620: 6172 7420 6f66 2074 6865 2066 696c 655f  art of the file_
-0000a630: 6d6f 756e 7473 292c 2073 6f20 7468 6520  mounts), so the 
-0000a640: 7265 7374 6f72 6520 666f 7220 6261 636b  restore for back
-0000a650: 7761 7264 0a20 2020 2023 2063 6f6d 7061  ward.    # compa
-0000a660: 7469 6269 6c69 7479 2073 686f 756c 6420  tibility should 
-0000a670: 676f 2062 6566 6f72 6520 7468 6973 2063  go before this c
-0000a680: 616c 6c2e 0a20 2020 205f 6f70 7469 6d69  all..    _optimi
-0000a690: 7a65 5f66 696c 655f 6d6f 756e 7473 2874  ze_file_mounts(t
-0000a6a0: 6d70 5f79 616d 6c5f 7061 7468 290a 0a20  mp_yaml_path).. 
-0000a6b0: 2020 2023 2052 656e 616d 6520 7468 6520     # Rename the 
-0000a6c0: 746d 7020 6669 6c65 2074 6f20 7468 6520  tmp file to the 
-0000a6d0: 6669 6e61 6c20 5941 4d4c 2070 6174 682e  final YAML path.
-0000a6e0: 0a20 2020 206f 732e 7265 6e61 6d65 2874  .    os.rename(t
-0000a6f0: 6d70 5f79 616d 6c5f 7061 7468 2c20 7961  mp_yaml_path, ya
-0000a700: 6d6c 5f70 6174 6829 0a20 2020 2075 7361  ml_path).    usa
-0000a710: 6765 5f6c 6962 2e6d 6573 7361 6765 732e  ge_lib.messages.
-0000a720: 7573 6167 652e 7570 6461 7465 5f72 6179  usage.update_ray
-0000a730: 5f79 616d 6c28 7961 6d6c 5f70 6174 6829  _yaml(yaml_path)
-0000a740: 0a20 2020 2072 6574 7572 6e20 636f 6e66  .    return conf
-0000a750: 6967 5f64 6963 740a 0a0a 6465 6620 5f61  ig_dict...def _a
-0000a760: 6464 5f61 7574 685f 746f 5f63 6c75 7374  dd_auth_to_clust
-0000a770: 6572 5f63 6f6e 6669 6728 636c 6f75 643a  er_config(cloud:
-0000a780: 2063 6c6f 7564 732e 436c 6f75 642c 2063   clouds.Cloud, c
-0000a790: 6c75 7374 6572 5f63 6f6e 6669 675f 6669  luster_config_fi
-0000a7a0: 6c65 3a20 7374 7229 3a0a 2020 2020 2222  le: str):.    ""
-0000a7b0: 2241 6464 7320 5353 4820 6b65 7920 696e  "Adds SSH key in
-0000a7c0: 666f 2074 6f20 7468 6520 636c 7573 7465  fo to the cluste
-0000a7d0: 7220 636f 6e66 6967 2e0a 0a20 2020 2054  r config...    T
-0000a7e0: 6869 7320 6675 6e63 7469 6f6e 2773 206f  his function's o
-0000a7f0: 7574 7075 7420 7265 6d6f 7665 7320 636f  utput removes co
-0000a800: 6d6d 656e 7473 2069 6e63 6c75 6465 6420  mments included 
-0000a810: 696e 2074 6865 206a 696e 6a61 3220 7465  in the jinja2 te
-0000a820: 6d70 6c61 7465 2e0a 2020 2020 2222 220a  mplate..    """.
-0000a830: 2020 2020 636f 6e66 6967 203d 2063 6f6d      config = com
-0000a840: 6d6f 6e5f 7574 696c 732e 7265 6164 5f79  mon_utils.read_y
-0000a850: 616d 6c28 636c 7573 7465 725f 636f 6e66  aml(cluster_conf
-0000a860: 6967 5f66 696c 6529 0a20 2020 2023 2043  ig_file).    # C
-0000a870: 6865 636b 2074 6865 2061 7661 696c 6162  heck the availab
-0000a880: 696c 6974 7920 6f66 2074 6865 2063 6c6f  ility of the clo
-0000a890: 7564 2074 7970 652e 0a20 2020 2069 6620  ud type..    if 
-0000a8a0: 6973 696e 7374 616e 6365 2863 6c6f 7564  isinstance(cloud
-0000a8b0: 2c20 2863 6c6f 7564 732e 4157 532c 2063  , (clouds.AWS, c
-0000a8c0: 6c6f 7564 732e 4f43 492c 2063 6c6f 7564  louds.OCI, cloud
-0000a8d0: 732e 5343 502c 2063 6c6f 7564 732e 5673  s.SCP, clouds.Vs
-0000a8e0: 7068 6572 652c 0a20 2020 2020 2020 2020  phere,.         
-0000a8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a900: 2063 6c6f 7564 732e 4375 646f 2c20 636c   clouds.Cudo, cl
-0000a910: 6f75 6473 2e50 6170 6572 7370 6163 6529  ouds.Paperspace)
-0000a920: 293a 0a20 2020 2020 2020 2063 6f6e 6669  ):.        confi
-0000a930: 6720 3d20 6175 7468 2e63 6f6e 6669 6775  g = auth.configu
-0000a940: 7265 5f73 7368 5f69 6e66 6f28 636f 6e66  re_ssh_info(conf
-0000a950: 6967 290a 2020 2020 656c 6966 2069 7369  ig).    elif isi
-0000a960: 6e73 7461 6e63 6528 636c 6f75 642c 2063  nstance(cloud, c
-0000a970: 6c6f 7564 732e 4743 5029 3a0a 2020 2020  louds.GCP):.    
-0000a980: 2020 2020 636f 6e66 6967 203d 2061 7574      config = aut
-0000a990: 682e 7365 7475 705f 6763 705f 6175 7468  h.setup_gcp_auth
-0000a9a0: 656e 7469 6361 7469 6f6e 2863 6f6e 6669  entication(confi
-0000a9b0: 6729 0a20 2020 2065 6c69 6620 6973 696e  g).    elif isin
-0000a9c0: 7374 616e 6365 2863 6c6f 7564 2c20 636c  stance(cloud, cl
-0000a9d0: 6f75 6473 2e41 7a75 7265 293a 0a20 2020  ouds.Azure):.   
-0000a9e0: 2020 2020 2063 6f6e 6669 6720 3d20 6175       config = au
-0000a9f0: 7468 2e73 6574 7570 5f61 7a75 7265 5f61  th.setup_azure_a
-0000aa00: 7574 6865 6e74 6963 6174 696f 6e28 636f  uthentication(co
-0000aa10: 6e66 6967 290a 2020 2020 656c 6966 2069  nfig).    elif i
-0000aa20: 7369 6e73 7461 6e63 6528 636c 6f75 642c  sinstance(cloud,
-0000aa30: 2063 6c6f 7564 732e 4c61 6d62 6461 293a   clouds.Lambda):
-0000aa40: 0a20 2020 2020 2020 2063 6f6e 6669 6720  .        config 
-0000aa50: 3d20 6175 7468 2e73 6574 7570 5f6c 616d  = auth.setup_lam
-0000aa60: 6264 615f 6175 7468 656e 7469 6361 7469  bda_authenticati
-0000aa70: 6f6e 2863 6f6e 6669 6729 0a20 2020 2065  on(config).    e
-0000aa80: 6c69 6620 6973 696e 7374 616e 6365 2863  lif isinstance(c
-0000aa90: 6c6f 7564 2c20 636c 6f75 6473 2e4b 7562  loud, clouds.Kub
-0000aaa0: 6572 6e65 7465 7329 3a0a 2020 2020 2020  ernetes):.      
-0000aab0: 2020 636f 6e66 6967 203d 2061 7574 682e    config = auth.
-0000aac0: 7365 7475 705f 6b75 6265 726e 6574 6573  setup_kubernetes
-0000aad0: 5f61 7574 6865 6e74 6963 6174 696f 6e28  _authentication(
-0000aae0: 636f 6e66 6967 290a 2020 2020 656c 6966  config).    elif
-0000aaf0: 2069 7369 6e73 7461 6e63 6528 636c 6f75   isinstance(clou
-0000ab00: 642c 2063 6c6f 7564 732e 4942 4d29 3a0a  d, clouds.IBM):.
-0000ab10: 2020 2020 2020 2020 636f 6e66 6967 203d          config =
-0000ab20: 2061 7574 682e 7365 7475 705f 6962 6d5f   auth.setup_ibm_
-0000ab30: 6175 7468 656e 7469 6361 7469 6f6e 2863  authentication(c
-0000ab40: 6f6e 6669 6729 0a20 2020 2065 6c69 6620  onfig).    elif 
-0000ab50: 6973 696e 7374 616e 6365 2863 6c6f 7564  isinstance(cloud
-0000ab60: 2c20 636c 6f75 6473 2e52 756e 506f 6429  , clouds.RunPod)
-0000ab70: 3a0a 2020 2020 2020 2020 636f 6e66 6967  :.        config
-0000ab80: 203d 2061 7574 682e 7365 7475 705f 7275   = auth.setup_ru
-0000ab90: 6e70 6f64 5f61 7574 6865 6e74 6963 6174  npod_authenticat
-0000aba0: 696f 6e28 636f 6e66 6967 290a 2020 2020  ion(config).    
-0000abb0: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
-0000abc0: 636c 6f75 642c 2063 6c6f 7564 732e 466c  cloud, clouds.Fl
-0000abd0: 7569 6473 7461 636b 293a 0a20 2020 2020  uidstack):.     
-0000abe0: 2020 2063 6f6e 6669 6720 3d20 6175 7468     config = auth
-0000abf0: 2e73 6574 7570 5f66 6c75 6964 7374 6163  .setup_fluidstac
-0000ac00: 6b5f 6175 7468 656e 7469 6361 7469 6f6e  k_authentication
-0000ac10: 2863 6f6e 6669 6729 0a20 2020 2065 6c73  (config).    els
-0000ac20: 653a 0a20 2020 2020 2020 2061 7373 6572  e:.        asser
-0000ac30: 7420 4661 6c73 652c 2063 6c6f 7564 0a20  t False, cloud. 
-0000ac40: 2020 2063 6f6d 6d6f 6e5f 7574 696c 732e     common_utils.
-0000ac50: 6475 6d70 5f79 616d 6c28 636c 7573 7465  dump_yaml(cluste
-0000ac60: 725f 636f 6e66 6967 5f66 696c 652c 2063  r_config_file, c
-0000ac70: 6f6e 6669 6729 0a0a 0a64 6566 2067 6574  onfig)...def get
-0000ac80: 5f72 756e 5f74 696d 6573 7461 6d70 2829  _run_timestamp()
-0000ac90: 202d 3e20 7374 723a 0a20 2020 2072 6574   -> str:.    ret
-0000aca0: 7572 6e20 2773 6b79 2d27 202b 2064 6174  urn 'sky-' + dat
-0000acb0: 6574 696d 652e 6e6f 7728 292e 7374 7266  etime.now().strf
-0000acc0: 7469 6d65 2827 2559 2d25 6d2d 2564 2d25  time('%Y-%m-%d-%
-0000acd0: 482d 254d 2d25 532d 2566 2729 0a0a 0a64  H-%M-%S-%f')...d
-0000ace0: 6566 2067 6574 5f74 696d 6573 7461 6d70  ef get_timestamp
-0000acf0: 5f66 726f 6d5f 7275 6e5f 7469 6d65 7374  _from_run_timest
-0000ad00: 616d 7028 7275 6e5f 7469 6d65 7374 616d  amp(run_timestam
-0000ad10: 703a 2073 7472 2920 2d3e 2066 6c6f 6174  p: str) -> float
-0000ad20: 3a0a 2020 2020 7265 7475 726e 2064 6174  :.    return dat
-0000ad30: 6574 696d 652e 7374 7270 7469 6d65 280a  etime.strptime(.
-0000ad40: 2020 2020 2020 2020 7275 6e5f 7469 6d65          run_time
-0000ad50: 7374 616d 702e 7061 7274 6974 696f 6e28  stamp.partition(
-0000ad60: 272d 2729 5b32 5d2c 2027 2559 2d25 6d2d  '-')[2], '%Y-%m-
-0000ad70: 2564 2d25 482d 254d 2d25 532d 2566 2729  %d-%H-%M-%S-%f')
-0000ad80: 2e74 696d 6573 7461 6d70 2829 0a0a 0a64  .timestamp()...d
-0000ad90: 6566 205f 636f 756e 745f 6865 616c 7468  ef _count_health
-0000ada0: 795f 6e6f 6465 735f 6672 6f6d 5f72 6179  y_nodes_from_ray
-0000adb0: 286f 7574 7075 743a 2073 7472 2c0a 2020  (output: str,.  
-0000adc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000add0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ade0: 6973 5f6c 6f63 616c 5f63 6c6f 7564 3a20  is_local_cloud: 
-0000adf0: 626f 6f6c 203d 2046 616c 7365 0a20 2020  bool = False.   
-0000ae00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae10: 2020 2020 2020 2020 2020 2020 2020 2920                ) 
-0000ae20: 2d3e 2054 7570 6c65 5b69 6e74 2c20 696e  -> Tuple[int, in
-0000ae30: 745d 3a0a 2020 2020 2222 2243 6f75 6e74  t]:.    """Count
-0000ae40: 2074 6865 206e 756d 6265 7220 6f66 2068   the number of h
-0000ae50: 6561 6c74 6879 206e 6f64 6573 2066 726f  ealthy nodes fro
-0000ae60: 6d20 7468 6520 6f75 7470 7574 206f 6620  m the output of 
-0000ae70: 6072 6179 2073 7461 7475 7360 2e22 2222  `ray status`."""
-0000ae80: 0a0a 2020 2020 6465 6620 6765 745f 7265  ..    def get_re
-0000ae90: 6164 795f 6e6f 6465 735f 636f 756e 7473  ady_nodes_counts
-0000aea0: 2870 6174 7465 726e 2c20 6f75 7470 7574  (pattern, output
-0000aeb0: 293a 0a20 2020 2020 2020 2072 6573 756c  ):.        resul
-0000aec0: 7420 3d20 7061 7474 6572 6e2e 6669 6e64  t = pattern.find
-0000aed0: 616c 6c28 6f75 7470 7574 290a 2020 2020  all(output).    
-0000aee0: 2020 2020 6966 206e 6f74 2072 6573 756c      if not resul
-0000aef0: 743a 0a20 2020 2020 2020 2020 2020 2072  t:.            r
-0000af00: 6574 7572 6e20 300a 2020 2020 2020 2020  eturn 0.        
-0000af10: 6173 7365 7274 206c 656e 2872 6573 756c  assert len(resul
-0000af20: 7429 203d 3d20 312c 2072 6573 756c 740a  t) == 1, result.
-0000af30: 2020 2020 2020 2020 7265 7475 726e 2069          return i
-0000af40: 6e74 2872 6573 756c 745b 305d 290a 0a20  nt(result[0]).. 
-0000af50: 2020 2023 2043 6865 636b 2069 6620 7468     # Check if th
-0000af60: 6520 7261 7920 636c 7573 7465 7220 6973  e ray cluster is
-0000af70: 2073 7461 7274 6564 2077 6974 6820 7261   started with ra
-0000af80: 7920 6175 746f 7363 616c 6572 2e20 496e  y autoscaler. In
-0000af90: 206e 6577 0a20 2020 2023 2070 726f 7669   new.    # provi
-0000afa0: 7369 6f6e 6572 2028 2331 3730 3229 2061  sioner (#1702) a
-0000afb0: 6e64 206c 6f63 616c 206d 6f64 652c 2077  nd local mode, w
-0000afc0: 6520 7374 6172 7465 6420 7468 6520 7261  e started the ra
-0000afd0: 7920 636c 7573 7465 7220 7769 7468 6f75  y cluster withou
-0000afe0: 7420 7261 790a 2020 2020 2320 6175 746f  t ray.    # auto
-0000aff0: 7363 616c 6572 2e0a 2020 2020 2320 4966  scaler..    # If
-0000b000: 2072 6179 2063 6c75 7374 6572 2069 7320   ray cluster is 
-0000b010: 7374 6172 7465 6420 7769 7468 2072 6179  started with ray
-0000b020: 2061 7574 6f73 6361 6c65 722c 2074 6865   autoscaler, the
-0000b030: 206f 7574 7075 7420 7769 6c6c 2062 653a   output will be:
-0000b040: 0a20 2020 2023 2020 3120 7261 792e 6865  .    #  1 ray.he
-0000b050: 6164 2e64 6566 6175 6c74 0a20 2020 2023  ad.default.    #
-0000b060: 2020 2e2e 2e0a 2020 2020 2320 544f 444f    ....    # TODO
-0000b070: 287a 6877 7529 3a20 6f6e 6365 2077 6520  (zhwu): once we 
-0000b080: 6465 7072 6563 6174 6520 7468 6520 6f6c  deprecate the ol
-0000b090: 6420 7072 6f76 6973 696f 6e65 722c 2077  d provisioner, w
-0000b0a0: 6520 6361 6e20 7265 6d6f 7665 2074 6869  e can remove thi
-0000b0b0: 730a 2020 2020 2320 6368 6563 6b2e 0a20  s.    # check.. 
-0000b0c0: 2020 2072 6179 5f61 7574 6f73 6361 6c65     ray_autoscale
-0000b0d0: 725f 6865 6164 203d 2067 6574 5f72 6561  r_head = get_rea
-0000b0e0: 6479 5f6e 6f64 6573 5f63 6f75 6e74 7328  dy_nodes_counts(
-0000b0f0: 5f4c 4155 4e43 4845 445f 4845 4144 5f50  _LAUNCHED_HEAD_P
-0000b100: 4154 5445 524e 2c20 6f75 7470 7574 290a  ATTERN, output).
-0000b110: 2020 2020 6973 5f6c 6f63 616c 5f72 6179      is_local_ray
-0000b120: 5f63 6c75 7374 6572 203d 2072 6179 5f61  _cluster = ray_a
-0000b130: 7574 6f73 6361 6c65 725f 6865 6164 203d  utoscaler_head =
-0000b140: 3d20 300a 0a20 2020 2069 6620 6973 5f6c  = 0..    if is_l
-0000b150: 6f63 616c 5f72 6179 5f63 6c75 7374 6572  ocal_ray_cluster
-0000b160: 206f 7220 6973 5f6c 6f63 616c 5f63 6c6f   or is_local_clo
-0000b170: 7564 3a0a 2020 2020 2020 2020 2320 5261  ud:.        # Ra
-0000b180: 7920 636c 7573 7465 7220 6973 206c 6175  y cluster is lau
-0000b190: 6e63 6865 6420 7769 7468 206e 6577 2070  nched with new p
-0000b1a0: 726f 7669 7369 6f6e 6572 0a20 2020 2020  rovisioner.     
-0000b1b0: 2020 2023 2046 6f72 206e 6577 2070 726f     # For new pro
-0000b1c0: 7669 7369 6f6e 6572 2061 6e64 206c 6f63  visioner and loc
-0000b1d0: 616c 206d 6f64 652c 2074 6865 206f 7574  al mode, the out
-0000b1e0: 7075 7420 7769 6c6c 2062 653a 0a20 2020  put will be:.   
-0000b1f0: 2020 2020 2023 2020 3120 6e6f 6465 5f78       #  1 node_x
-0000b200: 7878 780a 2020 2020 2020 2020 2320 2031  xxx.        #  1
-0000b210: 206e 6f64 655f 7878 7878 0a20 2020 2020   node_xxxx.     
-0000b220: 2020 2072 6561 6479 5f68 6561 6420 3d20     ready_head = 
-0000b230: 300a 2020 2020 2020 2020 7265 6164 795f  0.        ready_
-0000b240: 776f 726b 6572 7320 3d20 5f4c 4155 4e43  workers = _LAUNC
-0000b250: 4845 445f 4c4f 4341 4c5f 574f 524b 4552  HED_LOCAL_WORKER
-0000b260: 5f50 4154 5445 524e 2e66 696e 6461 6c6c  _PATTERN.findall
-0000b270: 286f 7574 7075 7429 0a20 2020 2020 2020  (output).       
-0000b280: 2072 6561 6479 5f77 6f72 6b65 7273 203d   ready_workers =
-0000b290: 206c 656e 2872 6561 6479 5f77 6f72 6b65   len(ready_worke
-0000b2a0: 7273 290a 2020 2020 2020 2020 6966 2069  rs).        if i
-0000b2b0: 735f 6c6f 6361 6c5f 7261 795f 636c 7573  s_local_ray_clus
-0000b2c0: 7465 723a 0a20 2020 2020 2020 2020 2020  ter:.           
-0000b2d0: 2072 6561 6479 5f68 6561 6420 3d20 310a   ready_head = 1.
-0000b2e0: 2020 2020 2020 2020 2020 2020 7265 6164              read
-0000b2f0: 795f 776f 726b 6572 7320 2d3d 2031 0a20  y_workers -= 1. 
-0000b300: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-0000b310: 6164 795f 6865 6164 2c20 7265 6164 795f  ady_head, ready_
-0000b320: 776f 726b 6572 730a 0a20 2020 2023 2043  workers..    # C
-0000b330: 6f75 6e74 206e 756d 6265 7220 6f66 206e  ount number of n
-0000b340: 6f64 6573 2062 7920 7061 7273 696e 6720  odes by parsing 
-0000b350: 7468 6520 6f75 7470 7574 206f 6620 6072  the output of `r
-0000b360: 6179 2073 7461 7475 7360 2e20 5468 6520  ay status`. The 
-0000b370: 6f75 7470 7574 0a20 2020 2023 206c 6f6f  output.    # loo
-0000b380: 6b73 206c 696b 653a 0a20 2020 2023 2020  ks like:.    #  
-0000b390: 2031 2072 6179 2e68 6561 642e 6465 6661   1 ray.head.defa
-0000b3a0: 756c 740a 2020 2020 2320 2020 3220 7261  ult.    #   2 ra
-0000b3b0: 792e 776f 726b 6572 2e64 6566 6175 6c74  y.worker.default
-0000b3c0: 0a20 2020 2072 6561 6479 5f68 6561 6420  .    ready_head 
-0000b3d0: 3d20 7261 795f 6175 746f 7363 616c 6572  = ray_autoscaler
-0000b3e0: 5f68 6561 640a 2020 2020 7265 6164 795f  _head.    ready_
-0000b3f0: 776f 726b 6572 7320 3d20 6765 745f 7265  workers = get_re
-0000b400: 6164 795f 6e6f 6465 735f 636f 756e 7473  ady_nodes_counts
-0000b410: 285f 4c41 554e 4348 4544 5f57 4f52 4b45  (_LAUNCHED_WORKE
-0000b420: 525f 5041 5454 4552 4e2c 206f 7574 7075  R_PATTERN, outpu
-0000b430: 7429 0a20 2020 2072 6561 6479 5f72 6573  t).    ready_res
-0000b440: 6572 7665 645f 776f 726b 6572 7320 3d20  erved_workers = 
-0000b450: 6765 745f 7265 6164 795f 6e6f 6465 735f  get_ready_nodes_
-0000b460: 636f 756e 7473 280a 2020 2020 2020 2020  counts(.        
-0000b470: 5f4c 4155 4e43 4845 445f 5245 5345 5256  _LAUNCHED_RESERV
-0000b480: 4544 5f57 4f52 4b45 525f 5041 5454 4552  ED_WORKER_PATTER
-0000b490: 4e2c 206f 7574 7075 7429 0a20 2020 2072  N, output).    r
-0000b4a0: 6561 6479 5f77 6f72 6b65 7273 202b 3d20  eady_workers += 
-0000b4b0: 7265 6164 795f 7265 7365 7276 6564 5f77  ready_reserved_w
-0000b4c0: 6f72 6b65 7273 0a20 2020 2061 7373 6572  orkers.    asser
-0000b4d0: 7420 7265 6164 795f 6865 6164 203c 3d20  t ready_head <= 
-0000b4e0: 312c 2066 2723 6865 6164 206e 6f64 6520  1, f'#head node 
-0000b4f0: 7368 6f75 6c64 2062 6520 3c3d 3120 2847  should be <=1 (G
-0000b500: 6f74 207b 7265 6164 795f 6865 6164 7d29  ot {ready_head})
-0000b510: 2e27 0a20 2020 2072 6574 7572 6e20 7265  .'.    return re
-0000b520: 6164 795f 6865 6164 2c20 7265 6164 795f  ady_head, ready_
-0000b530: 776f 726b 6572 730a 0a0a 6465 6620 6765  workers...def ge
-0000b540: 745f 646f 636b 6572 5f75 7365 7228 6970  t_docker_user(ip
-0000b550: 3a20 7374 722c 2063 6c75 7374 6572 5f63  : str, cluster_c
-0000b560: 6f6e 6669 675f 6669 6c65 3a20 7374 7229  onfig_file: str)
-0000b570: 202d 3e20 7374 723a 0a20 2020 2022 2222   -> str:.    """
-0000b580: 4669 6e64 2064 6f63 6b65 7220 636f 6e74  Find docker cont
-0000b590: 6169 6e65 7220 7573 6572 6e61 6d65 2e22  ainer username."
-0000b5a0: 2222 0a20 2020 2073 7368 5f63 7265 6465  "".    ssh_crede
-0000b5b0: 6e74 6961 6c73 203d 2073 7368 5f63 7265  ntials = ssh_cre
-0000b5c0: 6465 6e74 6961 6c5f 6672 6f6d 5f79 616d  dential_from_yam
-0000b5d0: 6c28 636c 7573 7465 725f 636f 6e66 6967  l(cluster_config
-0000b5e0: 5f66 696c 6529 0a20 2020 2072 756e 6e65  _file).    runne
-0000b5f0: 7220 3d20 636f 6d6d 616e 645f 7275 6e6e  r = command_runn
-0000b600: 6572 2e53 5348 436f 6d6d 616e 6452 756e  er.SSHCommandRun
-0000b610: 6e65 7228 6e6f 6465 3d28 6970 2c20 3232  ner(node=(ip, 22
-0000b620: 292c 202a 2a73 7368 5f63 7265 6465 6e74  ), **ssh_credent
-0000b630: 6961 6c73 290a 2020 2020 636f 6e74 6169  ials).    contai
-0000b640: 6e65 725f 6e61 6d65 203d 2063 6f6e 7374  ner_name = const
-0000b650: 616e 7473 2e44 4546 4155 4c54 5f44 4f43  ants.DEFAULT_DOC
-0000b660: 4b45 525f 434f 4e54 4149 4e45 525f 4e41  KER_CONTAINER_NA
-0000b670: 4d45 0a20 2020 2077 686f 616d 695f 7265  ME.    whoami_re
-0000b680: 7475 726e 636f 6465 2c20 7768 6f61 6d69  turncode, whoami
-0000b690: 5f73 7464 6f75 742c 2077 686f 616d 695f  _stdout, whoami_
-0000b6a0: 7374 6465 7272 203d 2072 756e 6e65 722e  stderr = runner.
-0000b6b0: 7275 6e28 0a20 2020 2020 2020 2066 2773  run(.        f's
-0000b6c0: 7564 6f20 646f 636b 6572 2065 7865 6320  udo docker exec 
-0000b6d0: 7b63 6f6e 7461 696e 6572 5f6e 616d 657d  {container_name}
-0000b6e0: 2077 686f 616d 6927 2c0a 2020 2020 2020   whoami',.      
-0000b6f0: 2020 7374 7265 616d 5f6c 6f67 733d 4661    stream_logs=Fa
-0000b700: 6c73 652c 0a20 2020 2020 2020 2072 6571  lse,.        req
-0000b710: 7569 7265 5f6f 7574 7075 7473 3d54 7275  uire_outputs=Tru
-0000b720: 6529 0a20 2020 2061 7373 6572 7420 7768  e).    assert wh
-0000b730: 6f61 6d69 5f72 6574 7572 6e63 6f64 6520  oami_returncode 
-0000b740: 3d3d 2030 2c20 280a 2020 2020 2020 2020  == 0, (.        
-0000b750: 6627 4661 696c 6564 2074 6f20 6765 7420  f'Failed to get 
-0000b760: 646f 636b 6572 2063 6f6e 7461 696e 6572  docker container
-0000b770: 2075 7365 722e 2052 6574 7572 6e20 270a   user. Return '.
-0000b780: 2020 2020 2020 2020 6627 636f 6465 3a20          f'code: 
-0000b790: 7b77 686f 616d 695f 7265 7475 726e 636f  {whoami_returnco
-0000b7a0: 6465 7d2c 2045 7272 6f72 3a20 7b77 686f  de}, Error: {who
-0000b7b0: 616d 695f 7374 6465 7272 7d27 290a 2020  ami_stderr}').  
-0000b7c0: 2020 646f 636b 6572 5f75 7365 7220 3d20    docker_user = 
-0000b7d0: 7768 6f61 6d69 5f73 7464 6f75 742e 7374  whoami_stdout.st
-0000b7e0: 7269 7028 290a 2020 2020 6c6f 6767 6572  rip().    logger
-0000b7f0: 2e64 6562 7567 2866 2744 6f63 6b65 7220  .debug(f'Docker 
-0000b800: 636f 6e74 6169 6e65 7220 7573 6572 3a20  container user: 
-0000b810: 7b64 6f63 6b65 725f 7573 6572 7d27 290a  {docker_user}').
-0000b820: 2020 2020 7265 7475 726e 2064 6f63 6b65      return docke
-0000b830: 725f 7573 6572 0a0a 0a40 7469 6d65 6c69  r_user...@timeli
-0000b840: 6e65 2e65 7665 6e74 0a64 6566 2077 6169  ne.event.def wai
-0000b850: 745f 756e 7469 6c5f 7261 795f 636c 7573  t_until_ray_clus
-0000b860: 7465 725f 7265 6164 7928 0a20 2020 2063  ter_ready(.    c
-0000b870: 6c75 7374 6572 5f63 6f6e 6669 675f 6669  luster_config_fi
-0000b880: 6c65 3a20 7374 722c 0a20 2020 206e 756d  le: str,.    num
-0000b890: 5f6e 6f64 6573 3a20 696e 742c 0a20 2020  _nodes: int,.   
-0000b8a0: 206c 6f67 5f70 6174 683a 2073 7472 2c0a   log_path: str,.
-0000b8b0: 2020 2020 6973 5f6c 6f63 616c 5f63 6c6f      is_local_clo
-0000b8c0: 7564 3a20 626f 6f6c 203d 2046 616c 7365  ud: bool = False
-0000b8d0: 2c0a 2020 2020 6e6f 6465 735f 6c61 756e  ,.    nodes_laun
-0000b8e0: 6368 696e 675f 7072 6f67 7265 7373 5f74  ching_progress_t
-0000b8f0: 696d 656f 7574 3a20 4f70 7469 6f6e 616c  imeout: Optional
-0000b900: 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a 2920  [int] = None,.) 
-0000b910: 2d3e 2054 7570 6c65 5b62 6f6f 6c2c 204f  -> Tuple[bool, O
-0000b920: 7074 696f 6e61 6c5b 7374 725d 5d3a 0a20  ptional[str]]:. 
-0000b930: 2020 2022 2222 5761 6974 2075 6e74 696c     """Wait until
-0000b940: 2074 6865 2072 6179 2063 6c75 7374 6572   the ray cluster
-0000b950: 2069 7320 7365 7420 7570 206f 6e20 564d   is set up on VM
-0000b960: 7320 6f72 2069 6e20 636f 6e74 6169 6e65  s or in containe
-0000b970: 7273 2e0a 0a20 2020 2052 6574 7572 6e73  rs...    Returns
-0000b980: 3a20 2077 6865 7468 6572 2074 6865 2065  :  whether the e
-0000b990: 6e74 6972 6520 7261 7920 636c 7573 7465  ntire ray cluste
-0000b9a0: 7220 6973 2072 6561 6479 2c20 616e 6420  r is ready, and 
-0000b9b0: 646f 636b 6572 2075 7365 726e 616d 650a  docker username.
-0000b9c0: 2020 2020 6966 206c 6175 6e63 6865 6420      if launched 
-0000b9d0: 7769 7468 2064 6f63 6b65 722e 0a20 2020  with docker..   
-0000b9e0: 2022 2222 0a20 2020 2023 204d 616e 7561   """.    # Manua
-0000b9f0: 6c6c 7920 6665 7463 6869 6e67 2068 6561  lly fetching hea
-0000ba00: 6420 6970 2069 6e73 7465 6164 206f 6620  d ip instead of 
-0000ba10: 7573 696e 6720 6072 6179 2065 7865 6360  using `ray exec`
-0000ba20: 2074 6f20 6176 6f69 6420 7468 6520 6275   to avoid the bu
-0000ba30: 670a 2020 2020 2320 7468 6174 2060 7261  g.    # that `ra
-0000ba40: 7920 6578 6563 6020 6661 696c 7320 746f  y exec` fails to
-0000ba50: 2063 6f6e 6e65 6374 2074 6f20 7468 6520   connect to the 
-0000ba60: 6865 6164 206e 6f64 6520 6166 7465 7220  head node after 
-0000ba70: 736f 6d65 2077 6f72 6b65 7273 0a20 2020  some workers.   
-0000ba80: 2023 206c 6175 6e63 6865 6420 6573 7065   # launched espe
-0000ba90: 6369 616c 6c79 2066 6f72 2041 7a75 7265  cially for Azure
-0000baa0: 2e0a 2020 2020 7472 793a 0a20 2020 2020  ..    try:.     
-0000bab0: 2020 2068 6561 645f 6970 203d 205f 7175     head_ip = _qu
-0000bac0: 6572 795f 6865 6164 5f69 705f 7769 7468  ery_head_ip_with
-0000bad0: 5f72 6574 7269 6573 280a 2020 2020 2020  _retries(.      
-0000bae0: 2020 2020 2020 636c 7573 7465 725f 636f        cluster_co
-0000baf0: 6e66 6967 5f66 696c 652c 206d 6178 5f61  nfig_file, max_a
-0000bb00: 7474 656d 7074 733d 5741 4954 5f48 4541  ttempts=WAIT_HEA
-0000bb10: 445f 4e4f 4445 5f49 505f 4d41 585f 4154  D_NODE_IP_MAX_AT
-0000bb20: 5445 4d50 5453 290a 2020 2020 6578 6365  TEMPTS).    exce
-0000bb30: 7074 2065 7863 6570 7469 6f6e 732e 4665  pt exceptions.Fe
-0000bb40: 7463 6843 6c75 7374 6572 496e 666f 4572  tchClusterInfoEr
-0000bb50: 726f 7220 6173 2065 3a0a 2020 2020 2020  ror as e:.      
-0000bb60: 2020 6c6f 6767 6572 2e65 7272 6f72 2863    logger.error(c
-0000bb70: 6f6d 6d6f 6e5f 7574 696c 732e 666f 726d  ommon_utils.form
-0000bb80: 6174 5f65 7863 6570 7469 6f6e 2865 2929  at_exception(e))
-0000bb90: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000bba0: 4661 6c73 652c 204e 6f6e 6520 2023 2066  False, None  # f
-0000bbb0: 6169 6c65 640a 0a20 2020 2063 6f6e 6669  ailed..    confi
-0000bbc0: 6720 3d20 636f 6d6d 6f6e 5f75 7469 6c73  g = common_utils
-0000bbd0: 2e72 6561 645f 7961 6d6c 2863 6c75 7374  .read_yaml(clust
-0000bbe0: 6572 5f63 6f6e 6669 675f 6669 6c65 290a  er_config_file).
-0000bbf0: 0a20 2020 2064 6f63 6b65 725f 7573 6572  .    docker_user
-0000bc00: 203d 204e 6f6e 650a 2020 2020 6966 2027   = None.    if '
-0000bc10: 646f 636b 6572 2720 696e 2063 6f6e 6669  docker' in confi
-0000bc20: 673a 0a20 2020 2020 2020 2064 6f63 6b65  g:.        docke
-0000bc30: 725f 7573 6572 203d 2067 6574 5f64 6f63  r_user = get_doc
-0000bc40: 6b65 725f 7573 6572 2868 6561 645f 6970  ker_user(head_ip
-0000bc50: 2c20 636c 7573 7465 725f 636f 6e66 6967  , cluster_config
-0000bc60: 5f66 696c 6529 0a0a 2020 2020 6966 206e  _file)..    if n
-0000bc70: 756d 5f6e 6f64 6573 203c 3d20 313a 0a20  um_nodes <= 1:. 
-0000bc80: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-0000bc90: 7565 2c20 646f 636b 6572 5f75 7365 720a  ue, docker_user.
-0000bca0: 0a20 2020 2073 7368 5f63 7265 6465 6e74  .    ssh_credent
-0000bcb0: 6961 6c73 203d 2073 7368 5f63 7265 6465  ials = ssh_crede
-0000bcc0: 6e74 6961 6c5f 6672 6f6d 5f79 616d 6c28  ntial_from_yaml(
-0000bcd0: 636c 7573 7465 725f 636f 6e66 6967 5f66  cluster_config_f
-0000bce0: 696c 652c 2064 6f63 6b65 725f 7573 6572  ile, docker_user
-0000bcf0: 290a 2020 2020 6c61 7374 5f6e 6f64 6573  ).    last_nodes
-0000bd00: 5f73 6f5f 6661 7220 3d20 300a 2020 2020  _so_far = 0.    
-0000bd10: 7374 6172 7420 3d20 7469 6d65 2e74 696d  start = time.tim
-0000bd20: 6528 290a 2020 2020 7275 6e6e 6572 203d  e().    runner =
-0000bd30: 2063 6f6d 6d61 6e64 5f72 756e 6e65 722e   command_runner.
-0000bd40: 5353 4843 6f6d 6d61 6e64 5275 6e6e 6572  SSHCommandRunner
-0000bd50: 286e 6f64 653d 2868 6561 645f 6970 2c20  (node=(head_ip, 
-0000bd60: 3232 292c 0a20 2020 2020 2020 2020 2020  22),.           
-0000bd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000097e0: 696f 6e73 273a 2073 7065 6369 6669 635f  ions': specific_
+000097f0: 7265 7365 7276 6174 696f 6e73 2c0a 0a20  reservations,.. 
+00009800: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00009810: 2043 6f6e 6461 2073 6574 7570 0a20 2020   Conda setup.   
+00009820: 2020 2020 2020 2020 2020 2020 2027 636f               'co
+00009830: 6e64 615f 696e 7374 616c 6c61 7469 6f6e  nda_installation
+00009840: 5f63 6f6d 6d61 6e64 7327 3a0a 2020 2020  _commands':.    
+00009850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009860: 636f 6e73 7461 6e74 732e 434f 4e44 415f  constants.CONDA_
+00009870: 494e 5354 414c 4c41 5449 4f4e 5f43 4f4d  INSTALLATION_COM
+00009880: 4d41 4e44 532c 0a20 2020 2020 2020 2020  MANDS,.         
+00009890: 2020 2020 2020 2023 2057 6520 7368 6f75         # We shou
+000098a0: 6c64 206e 6f74 2075 7365 2060 2e66 6f72  ld not use `.for
+000098b0: 6d61 7460 2c20 6173 2069 7420 636f 6e74  mat`, as it cont
+000098c0: 6169 6e73 2027 7b7d 2720 6173 2074 6865  ains '{}' as the
+000098d0: 2062 6173 680a 2020 2020 2020 2020 2020   bash.          
+000098e0: 2020 2020 2020 2320 7379 6e74 6178 2e0a        # syntax..
+000098f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009900: 2772 6179 5f73 6b79 7069 6c6f 745f 696e  'ray_skypilot_in
+00009910: 7374 616c 6c61 7469 6f6e 5f63 6f6d 6d61  stallation_comma
+00009920: 6e64 7327 3a0a 2020 2020 2020 2020 2020  nds':.          
+00009930: 2020 2020 2020 2020 2020 2863 6f6e 7374            (const
+00009940: 616e 7473 2e52 4159 5f53 4b59 5049 4c4f  ants.RAY_SKYPILO
+00009950: 545f 494e 5354 414c 4c41 5449 4f4e 5f43  T_INSTALLATION_C
+00009960: 4f4d 4d41 4e44 532e 7265 706c 6163 6528  OMMANDS.replace(
+00009970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009980: 2020 2020 2020 2020 2027 7b73 6b79 5f77           '{sky_w
+00009990: 6865 656c 5f68 6173 687d 272c 0a20 2020  heel_hash}',.   
+000099a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000099b0: 2020 2020 2077 6865 656c 5f68 6173 6829       wheel_hash)
+000099c0: 2e72 6570 6c61 6365 2827 7b63 6c6f 7564  .replace('{cloud
+000099d0: 7d27 2c0a 2020 2020 2020 2020 2020 2020  }',.            
+000099e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000099f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a00: 7374 7228 636c 6f75 6429 2e6c 6f77 6572  str(cloud).lower
+00009a10: 2829 2929 2c0a 0a20 2020 2020 2020 2020  ())),..         
+00009a20: 2020 2020 2020 2023 2050 6f72 7420 6f66         # Port of
+00009a30: 2052 6179 2028 4743 5320 7365 7276 6572   Ray (GCS server
+00009a40: 292e 0a20 2020 2020 2020 2020 2020 2020  )..             
+00009a50: 2020 2023 2052 6179 2773 2064 6566 6175     # Ray's defau
+00009a60: 6c74 2070 6f72 7420 3633 3739 2069 7320  lt port 6379 is 
+00009a70: 636f 6e66 6c69 6374 6564 2077 6974 6820  conflicted with 
+00009a80: 5265 6469 732e 0a20 2020 2020 2020 2020  Redis..         
+00009a90: 2020 2020 2020 2027 7261 795f 706f 7274         'ray_port
+00009aa0: 273a 2063 6f6e 7374 616e 7473 2e53 4b59  ': constants.SKY
+00009ab0: 5f52 454d 4f54 455f 5241 595f 504f 5254  _REMOTE_RAY_PORT
+00009ac0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00009ad0: 2020 2772 6179 5f64 6173 6862 6f61 7264    'ray_dashboard
+00009ae0: 5f70 6f72 7427 3a20 636f 6e73 7461 6e74  _port': constant
+00009af0: 732e 534b 595f 5245 4d4f 5445 5f52 4159  s.SKY_REMOTE_RAY
+00009b00: 5f44 4153 4842 4f41 5244 5f50 4f52 542c  _DASHBOARD_PORT,
+00009b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009b20: 2027 7261 795f 7465 6d70 5f64 6972 273a   'ray_temp_dir':
+00009b30: 2063 6f6e 7374 616e 7473 2e53 4b59 5f52   constants.SKY_R
+00009b40: 454d 4f54 455f 5241 595f 5445 4d50 4449  EMOTE_RAY_TEMPDI
+00009b50: 522c 0a20 2020 2020 2020 2020 2020 2020  R,.             
+00009b60: 2020 2027 6475 6d70 5f70 6f72 745f 636f     'dump_port_co
+00009b70: 6d6d 616e 6427 3a20 6475 6d70 5f70 6f72  mmand': dump_por
+00009b80: 745f 636f 6d6d 616e 642c 0a20 2020 2020  t_command,.     
+00009b90: 2020 2020 2020 2020 2020 2023 2053 6b79             # Sky
+00009ba0: 2d69 6e74 6572 6e61 6c20 636f 6e73 7461  -internal consta
+00009bb0: 6e74 732e 0a20 2020 2020 2020 2020 2020  nts..           
+00009bc0: 2020 2020 2027 736b 795f 7261 795f 636d       'sky_ray_cm
+00009bd0: 6427 3a20 636f 6e73 7461 6e74 732e 534b  d': constants.SK
+00009be0: 595f 5241 595f 434d 442c 0a20 2020 2020  Y_RAY_CMD,.     
+00009bf0: 2020 2020 2020 2020 2020 2027 736b 795f             'sky_
+00009c00: 7069 705f 636d 6427 3a20 636f 6e73 7461  pip_cmd': consta
+00009c10: 6e74 732e 534b 595f 5049 505f 434d 442c  nts.SKY_PIP_CMD,
+00009c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009c30: 2027 7261 795f 7665 7273 696f 6e27 3a20   'ray_version': 
+00009c40: 636f 6e73 7461 6e74 732e 534b 595f 5245  constants.SKY_RE
+00009c50: 4d4f 5445 5f52 4159 5f56 4552 5349 4f4e  MOTE_RAY_VERSION
+00009c60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00009c70: 2020 2320 436f 6d6d 616e 6420 666f 7220    # Command for 
+00009c80: 7761 6974 696e 6720 7261 7920 636c 7573  waiting ray clus
+00009c90: 7465 7220 746f 2062 6520 7265 6164 7920  ter to be ready 
+00009ca0: 6f6e 2068 6561 642e 0a20 2020 2020 2020  on head..       
+00009cb0: 2020 2020 2020 2020 2027 7261 795f 6865           'ray_he
+00009cc0: 6164 5f77 6169 745f 696e 6974 6961 6c69  ad_wait_initiali
+00009cd0: 7a65 645f 636f 6d6d 616e 6427 3a0a 2020  zed_command':.  
+00009ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009cf0: 2020 696e 7374 616e 6365 5f73 6574 7570    instance_setup
+00009d00: 2e52 4159 5f48 4541 445f 5741 4954 5f49  .RAY_HEAD_WAIT_I
+00009d10: 4e49 5449 414c 495a 4544 5f43 4f4d 4d41  NITIALIZED_COMMA
+00009d20: 4e44 2c0a 0a20 2020 2020 2020 2020 2020  ND,..           
+00009d30: 2020 2020 2023 2043 6c6f 7564 2063 7265       # Cloud cre
+00009d40: 6465 6e74 6961 6c73 2066 6f72 2063 6c6f  dentials for clo
+00009d50: 7564 2073 746f 7261 6765 2e0a 2020 2020  ud storage..    
+00009d60: 2020 2020 2020 2020 2020 2020 2763 7265              'cre
+00009d70: 6465 6e74 6961 6c73 273a 2063 7265 6465  dentials': crede
+00009d80: 6e74 6961 6c73 2c0a 2020 2020 2020 2020  ntials,.        
+00009d90: 2020 2020 2020 2020 2320 536b 7920 7265          # Sky re
+00009da0: 6d6f 7465 2075 7469 6c73 2e0a 2020 2020  mote utils..    
+00009db0: 2020 2020 2020 2020 2020 2020 2773 6b79              'sky
+00009dc0: 5f72 656d 6f74 655f 7061 7468 273a 2053  _remote_path': S
+00009dd0: 4b59 5f52 454d 4f54 455f 5041 5448 2c0a  KY_REMOTE_PATH,.
+00009de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009df0: 2773 6b79 5f6c 6f63 616c 5f70 6174 6827  'sky_local_path'
+00009e00: 3a20 7374 7228 6c6f 6361 6c5f 7768 6565  : str(local_whee
+00009e10: 6c5f 7061 7468 292c 0a20 2020 2020 2020  l_path),.       
+00009e20: 2020 2020 2020 2020 2023 2041 6464 2079           # Add y
+00009e30: 616d 6c20 6669 6c65 2070 6174 6820 746f  aml file path to
+00009e40: 2074 6865 2074 656d 706c 6174 6520 7661   the template va
+00009e50: 7269 6162 6c65 732e 0a20 2020 2020 2020  riables..       
+00009e60: 2020 2020 2020 2020 2027 736b 795f 7261           'sky_ra
+00009e70: 795f 7961 6d6c 5f72 656d 6f74 655f 7061  y_yaml_remote_pa
+00009e80: 7468 273a 0a20 2020 2020 2020 2020 2020  th':.           
+00009e90: 2020 2020 2020 2020 2063 6c75 7374 6572           cluster
+00009ea0: 5f79 616d 6c5f 7574 696c 732e 534b 595f  _yaml_utils.SKY_
+00009eb0: 434c 5553 5445 525f 5941 4d4c 5f52 454d  CLUSTER_YAML_REM
+00009ec0: 4f54 455f 5041 5448 2c0a 2020 2020 2020  OTE_PATH,.      
+00009ed0: 2020 2020 2020 2020 2020 2773 6b79 5f72            'sky_r
+00009ee0: 6179 5f79 616d 6c5f 6c6f 6361 6c5f 7061  ay_yaml_local_pa
+00009ef0: 7468 273a 2074 6d70 5f79 616d 6c5f 7061  th': tmp_yaml_pa
+00009f00: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
+00009f10: 2020 2020 2773 6b79 5f76 6572 7369 6f6e      'sky_version
+00009f20: 273a 2073 7472 2876 6572 7369 6f6e 2e70  ': str(version.p
+00009f30: 6172 7365 2873 6b79 2e5f 5f76 6572 7369  arse(sky.__versi
+00009f40: 6f6e 5f5f 2929 2c0a 2020 2020 2020 2020  on__)),.        
+00009f50: 2020 2020 2020 2020 2773 6b79 5f77 6865          'sky_whe
+00009f60: 656c 5f68 6173 6827 3a20 7768 6565 6c5f  el_hash': wheel_
+00009f70: 6861 7368 2c0a 2020 2020 2020 2020 2020  hash,.          
+00009f80: 2020 2020 2020 2320 4175 7468 656e 7469        # Authenti
+00009f90: 6361 7469 6f6e 2028 6f70 7469 6f6e 616c  cation (optional
+00009fa0: 292e 0a20 2020 2020 2020 2020 2020 2020  )..             
+00009fb0: 2020 202a 2a61 7574 685f 636f 6e66 6967     **auth_config
+00009fc0: 2c0a 2020 2020 2020 2020 2020 2020 7d29  ,.            })
+00009fd0: 2c0a 2020 2020 2020 2020 6f75 7470 7574  ,.        output
+00009fe0: 5f70 6174 683d 746d 705f 7961 6d6c 5f70  _path=tmp_yaml_p
+00009ff0: 6174 6829 0a20 2020 2063 6f6e 6669 675f  ath).    config_
+0000a000: 6469 6374 5b27 636c 7573 7465 725f 6e61  dict['cluster_na
+0000a010: 6d65 275d 203d 2063 6c75 7374 6572 5f6e  me'] = cluster_n
+0000a020: 616d 650a 2020 2020 636f 6e66 6967 5f64  ame.    config_d
+0000a030: 6963 745b 2772 6179 275d 203d 2079 616d  ict['ray'] = yam
+0000a040: 6c5f 7061 7468 0a20 2020 2069 6620 6472  l_path.    if dr
+0000a050: 7972 756e 3a0a 2020 2020 2020 2020 2320  yrun:.        # 
+0000a060: 4966 2064 7279 7275 6e2c 2072 6574 7572  If dryrun, retur
+0000a070: 6e20 7468 6520 756e 6669 6e69 7368 6564  n the unfinished
+0000a080: 2074 6d70 2079 616d 6c20 7061 7468 2e0a   tmp yaml path..
+0000a090: 2020 2020 2020 2020 636f 6e66 6967 5f64          config_d
+0000a0a0: 6963 745b 2772 6179 275d 203d 2074 6d70  ict['ray'] = tmp
+0000a0b0: 5f79 616d 6c5f 7061 7468 0a20 2020 2020  _yaml_path.     
+0000a0c0: 2020 2072 6574 7572 6e20 636f 6e66 6967     return config
+0000a0d0: 5f64 6963 740a 2020 2020 5f61 6464 5f61  _dict.    _add_a
+0000a0e0: 7574 685f 746f 5f63 6c75 7374 6572 5f63  uth_to_cluster_c
+0000a0f0: 6f6e 6669 6728 636c 6f75 642c 2074 6d70  onfig(cloud, tmp
+0000a100: 5f79 616d 6c5f 7061 7468 290a 0a20 2020  _yaml_path)..   
+0000a110: 2023 2041 6464 206b 7562 6572 6e65 7465   # Add kubernete
+0000a120: 7320 636f 6e66 6967 2066 6965 6c64 7320  s config fields 
+0000a130: 6672 6f6d 207e 2f2e 736b 792f 636f 6e66  from ~/.sky/conf
+0000a140: 6967 0a20 2020 2069 6620 6973 696e 7374  ig.    if isinst
+0000a150: 616e 6365 2863 6c6f 7564 2c20 636c 6f75  ance(cloud, clou
+0000a160: 6473 2e4b 7562 6572 6e65 7465 7329 3a0a  ds.Kubernetes):.
+0000a170: 2020 2020 2020 2020 6b75 6265 726e 6574          kubernet
+0000a180: 6573 5f75 7469 6c73 2e63 6f6d 6269 6e65  es_utils.combine
+0000a190: 5f70 6f64 5f63 6f6e 6669 675f 6669 656c  _pod_config_fiel
+0000a1a0: 6473 2874 6d70 5f79 616d 6c5f 7061 7468  ds(tmp_yaml_path
+0000a1b0: 290a 2020 2020 2020 2020 6b75 6265 726e  ).        kubern
+0000a1c0: 6574 6573 5f75 7469 6c73 2e63 6f6d 6269  etes_utils.combi
+0000a1d0: 6e65 5f6d 6574 6164 6174 615f 6669 656c  ne_metadata_fiel
+0000a1e0: 6473 2874 6d70 5f79 616d 6c5f 7061 7468  ds(tmp_yaml_path
+0000a1f0: 290a 0a20 2020 2023 2052 6573 746f 7265  )..    # Restore
+0000a200: 2074 6865 206f 6c64 2079 616d 6c20 636f   the old yaml co
+0000a210: 6e74 656e 7420 666f 7220 6261 636b 7761  ntent for backwa
+0000a220: 7264 2063 6f6d 7061 7469 6269 6c69 7479  rd compatibility
+0000a230: 2e0a 2020 2020 6966 206f 732e 7061 7468  ..    if os.path
+0000a240: 2e65 7869 7374 7328 7961 6d6c 5f70 6174  .exists(yaml_pat
+0000a250: 6829 2061 6e64 206b 6565 705f 6c61 756e  h) and keep_laun
+0000a260: 6368 5f66 6965 6c64 735f 696e 5f65 7869  ch_fields_in_exi
+0000a270: 7374 696e 675f 636f 6e66 6967 3a0a 2020  sting_config:.  
+0000a280: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
+0000a290: 7961 6d6c 5f70 6174 682c 2027 7227 2c20  yaml_path, 'r', 
+0000a2a0: 656e 636f 6469 6e67 3d27 7574 662d 3827  encoding='utf-8'
+0000a2b0: 2920 6173 2066 3a0a 2020 2020 2020 2020  ) as f:.        
+0000a2c0: 2020 2020 6f6c 645f 7961 6d6c 5f63 6f6e      old_yaml_con
+0000a2d0: 7465 6e74 203d 2066 2e72 6561 6428 290a  tent = f.read().
+0000a2e0: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
+0000a2f0: 6e28 746d 705f 7961 6d6c 5f70 6174 682c  n(tmp_yaml_path,
+0000a300: 2027 7227 2c20 656e 636f 6469 6e67 3d27   'r', encoding='
+0000a310: 7574 662d 3827 2920 6173 2066 3a0a 2020  utf-8') as f:.  
+0000a320: 2020 2020 2020 2020 2020 6e65 775f 7961            new_ya
+0000a330: 6d6c 5f63 6f6e 7465 6e74 203d 2066 2e72  ml_content = f.r
+0000a340: 6561 6428 290a 2020 2020 2020 2020 7265  ead().        re
+0000a350: 7374 6f72 6564 5f79 616d 6c5f 636f 6e74  stored_yaml_cont
+0000a360: 656e 7420 3d20 5f72 6570 6c61 6365 5f79  ent = _replace_y
+0000a370: 616d 6c5f 6469 6374 7328 0a20 2020 2020  aml_dicts(.     
+0000a380: 2020 2020 2020 206e 6577 5f79 616d 6c5f         new_yaml_
+0000a390: 636f 6e74 656e 742c 206f 6c64 5f79 616d  content, old_yam
+0000a3a0: 6c5f 636f 6e74 656e 742c 0a20 2020 2020  l_content,.     
+0000a3b0: 2020 2020 2020 205f 5241 595f 5941 4d4c         _RAY_YAML
+0000a3c0: 5f4b 4559 535f 544f 5f52 4553 544f 5245  _KEYS_TO_RESTORE
+0000a3d0: 5f46 4f52 5f42 4143 4b5f 434f 4d50 4154  _FOR_BACK_COMPAT
+0000a3e0: 4942 494c 4954 592c 0a20 2020 2020 2020  IBILITY,.       
+0000a3f0: 2020 2020 205f 5241 595f 5941 4d4c 5f4b       _RAY_YAML_K
+0000a400: 4559 535f 544f 5f52 4553 544f 5245 5f45  EYS_TO_RESTORE_E
+0000a410: 5843 4550 5449 4f4e 5329 0a20 2020 2020  XCEPTIONS).     
+0000a420: 2020 2077 6974 6820 6f70 656e 2874 6d70     with open(tmp
+0000a430: 5f79 616d 6c5f 7061 7468 2c20 2777 272c  _yaml_path, 'w',
+0000a440: 2065 6e63 6f64 696e 673d 2775 7466 2d38   encoding='utf-8
+0000a450: 2729 2061 7320 663a 0a20 2020 2020 2020  ') as f:.       
+0000a460: 2020 2020 2066 2e77 7269 7465 2872 6573       f.write(res
+0000a470: 746f 7265 645f 7961 6d6c 5f63 6f6e 7465  tored_yaml_conte
+0000a480: 6e74 290a 0a20 2020 2063 6f6e 6669 675f  nt)..    config_
+0000a490: 6469 6374 5b27 636c 7573 7465 725f 6e61  dict['cluster_na
+0000a4a0: 6d65 5f6f 6e5f 636c 6f75 6427 5d20 3d20  me_on_cloud'] = 
+0000a4b0: 636c 7573 7465 725f 6e61 6d65 5f6f 6e5f  cluster_name_on_
+0000a4c0: 636c 6f75 640a 0a20 2020 2023 204f 7074  cloud..    # Opt
+0000a4d0: 696d 697a 6174 696f 6e3a 2063 6f70 7920  imization: copy 
+0000a4e0: 7468 6520 636f 6e74 656e 7473 206f 6620  the contents of 
+0000a4f0: 736f 7572 6365 2066 696c 6573 2069 6e20  source files in 
+0000a500: 6669 6c65 5f6d 6f75 6e74 7320 746f 2061  file_mounts to a
+0000a510: 0a20 2020 2023 2073 7065 6369 616c 2064  .    # special d
+0000a520: 6972 2c20 616e 6420 7570 6c6f 6164 2074  ir, and upload t
+0000a530: 6861 7420 6173 2074 6865 206f 6e6c 7920  hat as the only 
+0000a540: 6669 6c65 5f6d 6f75 6e74 2069 6e73 7465  file_mount inste
+0000a550: 6164 2e20 4465 6c61 790a 2020 2020 2320  ad. Delay.    # 
+0000a560: 6361 6c6c 696e 6720 7468 6973 206f 7074  calling this opt
+0000a570: 696d 697a 6174 696f 6e20 756e 7469 6c20  imization until 
+0000a580: 6e6f 772c 2077 6865 6e20 616c 6c20 736f  now, when all so
+0000a590: 7572 6365 2066 696c 6573 2068 6176 6520  urce files have 
+0000a5a0: 6265 656e 0a20 2020 2023 2077 7269 7474  been.    # writt
+0000a5b0: 656e 2061 6e64 2074 6865 6972 2063 6f6e  en and their con
+0000a5c0: 7465 6e74 7320 6669 6e61 6c69 7a65 642e  tents finalized.
+0000a5d0: 0a20 2020 2023 0a20 2020 2023 204e 6f74  .    #.    # Not
+0000a5e0: 6520 7468 6174 2074 6865 2072 6179 2079  e that the ray y
+0000a5f0: 616d 6c20 6669 6c65 2077 696c 6c20 6265  aml file will be
+0000a600: 2063 6f70 6965 6420 696e 746f 2074 6861   copied into tha
+0000a610: 7420 7370 6563 6961 6c20 6469 7220 2869  t special dir (i
+0000a620: 2e65 2e2c 0a20 2020 2023 2075 706c 6f61  .e.,.    # uploa
+0000a630: 6465 6420 6173 2070 6172 7420 6f66 2074  ded as part of t
+0000a640: 6865 2066 696c 655f 6d6f 756e 7473 292c  he file_mounts),
+0000a650: 2073 6f20 7468 6520 7265 7374 6f72 6520   so the restore 
+0000a660: 666f 7220 6261 636b 7761 7264 0a20 2020  for backward.   
+0000a670: 2023 2063 6f6d 7061 7469 6269 6c69 7479   # compatibility
+0000a680: 2073 686f 756c 6420 676f 2062 6566 6f72   should go befor
+0000a690: 6520 7468 6973 2063 616c 6c2e 0a20 2020  e this call..   
+0000a6a0: 205f 6f70 7469 6d69 7a65 5f66 696c 655f   _optimize_file_
+0000a6b0: 6d6f 756e 7473 2874 6d70 5f79 616d 6c5f  mounts(tmp_yaml_
+0000a6c0: 7061 7468 290a 0a20 2020 2023 2052 656e  path)..    # Ren
+0000a6d0: 616d 6520 7468 6520 746d 7020 6669 6c65  ame the tmp file
+0000a6e0: 2074 6f20 7468 6520 6669 6e61 6c20 5941   to the final YA
+0000a6f0: 4d4c 2070 6174 682e 0a20 2020 206f 732e  ML path..    os.
+0000a700: 7265 6e61 6d65 2874 6d70 5f79 616d 6c5f  rename(tmp_yaml_
+0000a710: 7061 7468 2c20 7961 6d6c 5f70 6174 6829  path, yaml_path)
+0000a720: 0a20 2020 2075 7361 6765 5f6c 6962 2e6d  .    usage_lib.m
+0000a730: 6573 7361 6765 732e 7573 6167 652e 7570  essages.usage.up
+0000a740: 6461 7465 5f72 6179 5f79 616d 6c28 7961  date_ray_yaml(ya
+0000a750: 6d6c 5f70 6174 6829 0a20 2020 2072 6574  ml_path).    ret
+0000a760: 7572 6e20 636f 6e66 6967 5f64 6963 740a  urn config_dict.
+0000a770: 0a0a 6465 6620 5f61 6464 5f61 7574 685f  ..def _add_auth_
+0000a780: 746f 5f63 6c75 7374 6572 5f63 6f6e 6669  to_cluster_confi
+0000a790: 6728 636c 6f75 643a 2063 6c6f 7564 732e  g(cloud: clouds.
+0000a7a0: 436c 6f75 642c 2063 6c75 7374 6572 5f63  Cloud, cluster_c
+0000a7b0: 6f6e 6669 675f 6669 6c65 3a20 7374 7229  onfig_file: str)
+0000a7c0: 3a0a 2020 2020 2222 2241 6464 7320 5353  :.    """Adds SS
+0000a7d0: 4820 6b65 7920 696e 666f 2074 6f20 7468  H key info to th
+0000a7e0: 6520 636c 7573 7465 7220 636f 6e66 6967  e cluster config
+0000a7f0: 2e0a 0a20 2020 2054 6869 7320 6675 6e63  ...    This func
+0000a800: 7469 6f6e 2773 206f 7574 7075 7420 7265  tion's output re
+0000a810: 6d6f 7665 7320 636f 6d6d 656e 7473 2069  moves comments i
+0000a820: 6e63 6c75 6465 6420 696e 2074 6865 206a  ncluded in the j
+0000a830: 696e 6a61 3220 7465 6d70 6c61 7465 2e0a  inja2 template..
+0000a840: 2020 2020 2222 220a 2020 2020 636f 6e66      """.    conf
+0000a850: 6967 203d 2063 6f6d 6d6f 6e5f 7574 696c  ig = common_util
+0000a860: 732e 7265 6164 5f79 616d 6c28 636c 7573  s.read_yaml(clus
+0000a870: 7465 725f 636f 6e66 6967 5f66 696c 6529  ter_config_file)
+0000a880: 0a20 2020 2023 2043 6865 636b 2074 6865  .    # Check the
+0000a890: 2061 7661 696c 6162 696c 6974 7920 6f66   availability of
+0000a8a0: 2074 6865 2063 6c6f 7564 2074 7970 652e   the cloud type.
+0000a8b0: 0a20 2020 2069 6620 6973 696e 7374 616e  .    if isinstan
+0000a8c0: 6365 2863 6c6f 7564 2c20 2863 6c6f 7564  ce(cloud, (cloud
+0000a8d0: 732e 4157 532c 2063 6c6f 7564 732e 4f43  s.AWS, clouds.OC
+0000a8e0: 492c 2063 6c6f 7564 732e 5343 502c 2063  I, clouds.SCP, c
+0000a8f0: 6c6f 7564 732e 5673 7068 6572 652c 0a20  louds.Vsphere,. 
+0000a900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a910: 2020 2020 2020 2020 2063 6c6f 7564 732e           clouds.
+0000a920: 4375 646f 2c20 636c 6f75 6473 2e50 6170  Cudo, clouds.Pap
+0000a930: 6572 7370 6163 6529 293a 0a20 2020 2020  erspace)):.     
+0000a940: 2020 2063 6f6e 6669 6720 3d20 6175 7468     config = auth
+0000a950: 2e63 6f6e 6669 6775 7265 5f73 7368 5f69  .configure_ssh_i
+0000a960: 6e66 6f28 636f 6e66 6967 290a 2020 2020  nfo(config).    
+0000a970: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
+0000a980: 636c 6f75 642c 2063 6c6f 7564 732e 4743  cloud, clouds.GC
+0000a990: 5029 3a0a 2020 2020 2020 2020 636f 6e66  P):.        conf
+0000a9a0: 6967 203d 2061 7574 682e 7365 7475 705f  ig = auth.setup_
+0000a9b0: 6763 705f 6175 7468 656e 7469 6361 7469  gcp_authenticati
+0000a9c0: 6f6e 2863 6f6e 6669 6729 0a20 2020 2065  on(config).    e
+0000a9d0: 6c69 6620 6973 696e 7374 616e 6365 2863  lif isinstance(c
+0000a9e0: 6c6f 7564 2c20 636c 6f75 6473 2e41 7a75  loud, clouds.Azu
+0000a9f0: 7265 293a 0a20 2020 2020 2020 2063 6f6e  re):.        con
+0000aa00: 6669 6720 3d20 6175 7468 2e73 6574 7570  fig = auth.setup
+0000aa10: 5f61 7a75 7265 5f61 7574 6865 6e74 6963  _azure_authentic
+0000aa20: 6174 696f 6e28 636f 6e66 6967 290a 2020  ation(config).  
+0000aa30: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
+0000aa40: 6528 636c 6f75 642c 2063 6c6f 7564 732e  e(cloud, clouds.
+0000aa50: 4c61 6d62 6461 293a 0a20 2020 2020 2020  Lambda):.       
+0000aa60: 2063 6f6e 6669 6720 3d20 6175 7468 2e73   config = auth.s
+0000aa70: 6574 7570 5f6c 616d 6264 615f 6175 7468  etup_lambda_auth
+0000aa80: 656e 7469 6361 7469 6f6e 2863 6f6e 6669  entication(confi
+0000aa90: 6729 0a20 2020 2065 6c69 6620 6973 696e  g).    elif isin
+0000aaa0: 7374 616e 6365 2863 6c6f 7564 2c20 636c  stance(cloud, cl
+0000aab0: 6f75 6473 2e4b 7562 6572 6e65 7465 7329  ouds.Kubernetes)
+0000aac0: 3a0a 2020 2020 2020 2020 636f 6e66 6967  :.        config
+0000aad0: 203d 2061 7574 682e 7365 7475 705f 6b75   = auth.setup_ku
+0000aae0: 6265 726e 6574 6573 5f61 7574 6865 6e74  bernetes_authent
+0000aaf0: 6963 6174 696f 6e28 636f 6e66 6967 290a  ication(config).
+0000ab00: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
+0000ab10: 6e63 6528 636c 6f75 642c 2063 6c6f 7564  nce(cloud, cloud
+0000ab20: 732e 4942 4d29 3a0a 2020 2020 2020 2020  s.IBM):.        
+0000ab30: 636f 6e66 6967 203d 2061 7574 682e 7365  config = auth.se
+0000ab40: 7475 705f 6962 6d5f 6175 7468 656e 7469  tup_ibm_authenti
+0000ab50: 6361 7469 6f6e 2863 6f6e 6669 6729 0a20  cation(config). 
+0000ab60: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
+0000ab70: 6365 2863 6c6f 7564 2c20 636c 6f75 6473  ce(cloud, clouds
+0000ab80: 2e52 756e 506f 6429 3a0a 2020 2020 2020  .RunPod):.      
+0000ab90: 2020 636f 6e66 6967 203d 2061 7574 682e    config = auth.
+0000aba0: 7365 7475 705f 7275 6e70 6f64 5f61 7574  setup_runpod_aut
+0000abb0: 6865 6e74 6963 6174 696f 6e28 636f 6e66  hentication(conf
+0000abc0: 6967 290a 2020 2020 656c 6966 2069 7369  ig).    elif isi
+0000abd0: 6e73 7461 6e63 6528 636c 6f75 642c 2063  nstance(cloud, c
+0000abe0: 6c6f 7564 732e 466c 7569 6473 7461 636b  louds.Fluidstack
+0000abf0: 293a 0a20 2020 2020 2020 2063 6f6e 6669  ):.        confi
+0000ac00: 6720 3d20 6175 7468 2e73 6574 7570 5f66  g = auth.setup_f
+0000ac10: 6c75 6964 7374 6163 6b5f 6175 7468 656e  luidstack_authen
+0000ac20: 7469 6361 7469 6f6e 2863 6f6e 6669 6729  tication(config)
+0000ac30: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+0000ac40: 2020 2061 7373 6572 7420 4661 6c73 652c     assert False,
+0000ac50: 2063 6c6f 7564 0a20 2020 2063 6f6d 6d6f   cloud.    commo
+0000ac60: 6e5f 7574 696c 732e 6475 6d70 5f79 616d  n_utils.dump_yam
+0000ac70: 6c28 636c 7573 7465 725f 636f 6e66 6967  l(cluster_config
+0000ac80: 5f66 696c 652c 2063 6f6e 6669 6729 0a0a  _file, config)..
+0000ac90: 0a64 6566 2067 6574 5f72 756e 5f74 696d  .def get_run_tim
+0000aca0: 6573 7461 6d70 2829 202d 3e20 7374 723a  estamp() -> str:
+0000acb0: 0a20 2020 2072 6574 7572 6e20 2773 6b79  .    return 'sky
+0000acc0: 2d27 202b 2064 6174 6574 696d 652e 6e6f  -' + datetime.no
+0000acd0: 7728 292e 7374 7266 7469 6d65 2827 2559  w().strftime('%Y
+0000ace0: 2d25 6d2d 2564 2d25 482d 254d 2d25 532d  -%m-%d-%H-%M-%S-
+0000acf0: 2566 2729 0a0a 0a64 6566 2067 6574 5f74  %f')...def get_t
+0000ad00: 696d 6573 7461 6d70 5f66 726f 6d5f 7275  imestamp_from_ru
+0000ad10: 6e5f 7469 6d65 7374 616d 7028 7275 6e5f  n_timestamp(run_
+0000ad20: 7469 6d65 7374 616d 703a 2073 7472 2920  timestamp: str) 
+0000ad30: 2d3e 2066 6c6f 6174 3a0a 2020 2020 7265  -> float:.    re
+0000ad40: 7475 726e 2064 6174 6574 696d 652e 7374  turn datetime.st
+0000ad50: 7270 7469 6d65 280a 2020 2020 2020 2020  rptime(.        
+0000ad60: 7275 6e5f 7469 6d65 7374 616d 702e 7061  run_timestamp.pa
+0000ad70: 7274 6974 696f 6e28 272d 2729 5b32 5d2c  rtition('-')[2],
+0000ad80: 2027 2559 2d25 6d2d 2564 2d25 482d 254d   '%Y-%m-%d-%H-%M
+0000ad90: 2d25 532d 2566 2729 2e74 696d 6573 7461  -%S-%f').timesta
+0000ada0: 6d70 2829 0a0a 0a64 6566 205f 636f 756e  mp()...def _coun
+0000adb0: 745f 6865 616c 7468 795f 6e6f 6465 735f  t_healthy_nodes_
+0000adc0: 6672 6f6d 5f72 6179 286f 7574 7075 743a  from_ray(output:
+0000add0: 2073 7472 2c0a 2020 2020 2020 2020 2020   str,.          
+0000ade0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000adf0: 2020 2020 2020 2020 6973 5f6c 6f63 616c          is_local
+0000ae00: 5f63 6c6f 7564 3a20 626f 6f6c 203d 2046  _cloud: bool = F
+0000ae10: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
+0000ae20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae30: 2020 2020 2020 2920 2d3e 2054 7570 6c65        ) -> Tuple
+0000ae40: 5b69 6e74 2c20 696e 745d 3a0a 2020 2020  [int, int]:.    
+0000ae50: 2222 2243 6f75 6e74 2074 6865 206e 756d  """Count the num
+0000ae60: 6265 7220 6f66 2068 6561 6c74 6879 206e  ber of healthy n
+0000ae70: 6f64 6573 2066 726f 6d20 7468 6520 6f75  odes from the ou
+0000ae80: 7470 7574 206f 6620 6072 6179 2073 7461  tput of `ray sta
+0000ae90: 7475 7360 2e22 2222 0a0a 2020 2020 6465  tus`."""..    de
+0000aea0: 6620 6765 745f 7265 6164 795f 6e6f 6465  f get_ready_node
+0000aeb0: 735f 636f 756e 7473 2870 6174 7465 726e  s_counts(pattern
+0000aec0: 2c20 6f75 7470 7574 293a 0a20 2020 2020  , output):.     
+0000aed0: 2020 2072 6573 756c 7420 3d20 7061 7474     result = patt
+0000aee0: 6572 6e2e 6669 6e64 616c 6c28 6f75 7470  ern.findall(outp
+0000aef0: 7574 290a 2020 2020 2020 2020 6966 206e  ut).        if n
+0000af00: 6f74 2072 6573 756c 743a 0a20 2020 2020  ot result:.     
+0000af10: 2020 2020 2020 2072 6574 7572 6e20 300a         return 0.
+0000af20: 2020 2020 2020 2020 6173 7365 7274 206c          assert l
+0000af30: 656e 2872 6573 756c 7429 203d 3d20 312c  en(result) == 1,
+0000af40: 2072 6573 756c 740a 2020 2020 2020 2020   result.        
+0000af50: 7265 7475 726e 2069 6e74 2872 6573 756c  return int(resul
+0000af60: 745b 305d 290a 0a20 2020 2023 2043 6865  t[0])..    # Che
+0000af70: 636b 2069 6620 7468 6520 7261 7920 636c  ck if the ray cl
+0000af80: 7573 7465 7220 6973 2073 7461 7274 6564  uster is started
+0000af90: 2077 6974 6820 7261 7920 6175 746f 7363   with ray autosc
+0000afa0: 616c 6572 2e20 496e 206e 6577 0a20 2020  aler. In new.   
+0000afb0: 2023 2070 726f 7669 7369 6f6e 6572 2028   # provisioner (
+0000afc0: 2331 3730 3229 2061 6e64 206c 6f63 616c  #1702) and local
+0000afd0: 206d 6f64 652c 2077 6520 7374 6172 7465   mode, we starte
+0000afe0: 6420 7468 6520 7261 7920 636c 7573 7465  d the ray cluste
+0000aff0: 7220 7769 7468 6f75 7420 7261 790a 2020  r without ray.  
+0000b000: 2020 2320 6175 746f 7363 616c 6572 2e0a    # autoscaler..
+0000b010: 2020 2020 2320 4966 2072 6179 2063 6c75      # If ray clu
+0000b020: 7374 6572 2069 7320 7374 6172 7465 6420  ster is started 
+0000b030: 7769 7468 2072 6179 2061 7574 6f73 6361  with ray autosca
+0000b040: 6c65 722c 2074 6865 206f 7574 7075 7420  ler, the output 
+0000b050: 7769 6c6c 2062 653a 0a20 2020 2023 2020  will be:.    #  
+0000b060: 3120 7261 792e 6865 6164 2e64 6566 6175  1 ray.head.defau
+0000b070: 6c74 0a20 2020 2023 2020 2e2e 2e0a 2020  lt.    #  ....  
+0000b080: 2020 2320 544f 444f 287a 6877 7529 3a20    # TODO(zhwu): 
+0000b090: 6f6e 6365 2077 6520 6465 7072 6563 6174  once we deprecat
+0000b0a0: 6520 7468 6520 6f6c 6420 7072 6f76 6973  e the old provis
+0000b0b0: 696f 6e65 722c 2077 6520 6361 6e20 7265  ioner, we can re
+0000b0c0: 6d6f 7665 2074 6869 730a 2020 2020 2320  move this.    # 
+0000b0d0: 6368 6563 6b2e 0a20 2020 2072 6179 5f61  check..    ray_a
+0000b0e0: 7574 6f73 6361 6c65 725f 6865 6164 203d  utoscaler_head =
+0000b0f0: 2067 6574 5f72 6561 6479 5f6e 6f64 6573   get_ready_nodes
+0000b100: 5f63 6f75 6e74 7328 5f4c 4155 4e43 4845  _counts(_LAUNCHE
+0000b110: 445f 4845 4144 5f50 4154 5445 524e 2c20  D_HEAD_PATTERN, 
+0000b120: 6f75 7470 7574 290a 2020 2020 6973 5f6c  output).    is_l
+0000b130: 6f63 616c 5f72 6179 5f63 6c75 7374 6572  ocal_ray_cluster
+0000b140: 203d 2072 6179 5f61 7574 6f73 6361 6c65   = ray_autoscale
+0000b150: 725f 6865 6164 203d 3d20 300a 0a20 2020  r_head == 0..   
+0000b160: 2069 6620 6973 5f6c 6f63 616c 5f72 6179   if is_local_ray
+0000b170: 5f63 6c75 7374 6572 206f 7220 6973 5f6c  _cluster or is_l
+0000b180: 6f63 616c 5f63 6c6f 7564 3a0a 2020 2020  ocal_cloud:.    
+0000b190: 2020 2020 2320 5261 7920 636c 7573 7465      # Ray cluste
+0000b1a0: 7220 6973 206c 6175 6e63 6865 6420 7769  r is launched wi
+0000b1b0: 7468 206e 6577 2070 726f 7669 7369 6f6e  th new provision
+0000b1c0: 6572 0a20 2020 2020 2020 2023 2046 6f72  er.        # For
+0000b1d0: 206e 6577 2070 726f 7669 7369 6f6e 6572   new provisioner
+0000b1e0: 2061 6e64 206c 6f63 616c 206d 6f64 652c   and local mode,
+0000b1f0: 2074 6865 206f 7574 7075 7420 7769 6c6c   the output will
+0000b200: 2062 653a 0a20 2020 2020 2020 2023 2020   be:.        #  
+0000b210: 3120 6e6f 6465 5f78 7878 780a 2020 2020  1 node_xxxx.    
+0000b220: 2020 2020 2320 2031 206e 6f64 655f 7878      #  1 node_xx
+0000b230: 7878 0a20 2020 2020 2020 2072 6561 6479  xx.        ready
+0000b240: 5f68 6561 6420 3d20 300a 2020 2020 2020  _head = 0.      
+0000b250: 2020 7265 6164 795f 776f 726b 6572 7320    ready_workers 
+0000b260: 3d20 5f4c 4155 4e43 4845 445f 4c4f 4341  = _LAUNCHED_LOCA
+0000b270: 4c5f 574f 524b 4552 5f50 4154 5445 524e  L_WORKER_PATTERN
+0000b280: 2e66 696e 6461 6c6c 286f 7574 7075 7429  .findall(output)
+0000b290: 0a20 2020 2020 2020 2072 6561 6479 5f77  .        ready_w
+0000b2a0: 6f72 6b65 7273 203d 206c 656e 2872 6561  orkers = len(rea
+0000b2b0: 6479 5f77 6f72 6b65 7273 290a 2020 2020  dy_workers).    
+0000b2c0: 2020 2020 6966 2069 735f 6c6f 6361 6c5f      if is_local_
+0000b2d0: 7261 795f 636c 7573 7465 723a 0a20 2020  ray_cluster:.   
+0000b2e0: 2020 2020 2020 2020 2072 6561 6479 5f68           ready_h
+0000b2f0: 6561 6420 3d20 310a 2020 2020 2020 2020  ead = 1.        
+0000b300: 2020 2020 7265 6164 795f 776f 726b 6572      ready_worker
+0000b310: 7320 2d3d 2031 0a20 2020 2020 2020 2072  s -= 1.        r
+0000b320: 6574 7572 6e20 7265 6164 795f 6865 6164  eturn ready_head
+0000b330: 2c20 7265 6164 795f 776f 726b 6572 730a  , ready_workers.
+0000b340: 0a20 2020 2023 2043 6f75 6e74 206e 756d  .    # Count num
+0000b350: 6265 7220 6f66 206e 6f64 6573 2062 7920  ber of nodes by 
+0000b360: 7061 7273 696e 6720 7468 6520 6f75 7470  parsing the outp
+0000b370: 7574 206f 6620 6072 6179 2073 7461 7475  ut of `ray statu
+0000b380: 7360 2e20 5468 6520 6f75 7470 7574 0a20  s`. The output. 
+0000b390: 2020 2023 206c 6f6f 6b73 206c 696b 653a     # looks like:
+0000b3a0: 0a20 2020 2023 2020 2031 2072 6179 2e68  .    #   1 ray.h
+0000b3b0: 6561 642e 6465 6661 756c 740a 2020 2020  ead.default.    
+0000b3c0: 2320 2020 3220 7261 792e 776f 726b 6572  #   2 ray.worker
+0000b3d0: 2e64 6566 6175 6c74 0a20 2020 2072 6561  .default.    rea
+0000b3e0: 6479 5f68 6561 6420 3d20 7261 795f 6175  dy_head = ray_au
+0000b3f0: 746f 7363 616c 6572 5f68 6561 640a 2020  toscaler_head.  
+0000b400: 2020 7265 6164 795f 776f 726b 6572 7320    ready_workers 
+0000b410: 3d20 6765 745f 7265 6164 795f 6e6f 6465  = get_ready_node
+0000b420: 735f 636f 756e 7473 285f 4c41 554e 4348  s_counts(_LAUNCH
+0000b430: 4544 5f57 4f52 4b45 525f 5041 5454 4552  ED_WORKER_PATTER
+0000b440: 4e2c 206f 7574 7075 7429 0a20 2020 2072  N, output).    r
+0000b450: 6561 6479 5f72 6573 6572 7665 645f 776f  eady_reserved_wo
+0000b460: 726b 6572 7320 3d20 6765 745f 7265 6164  rkers = get_read
+0000b470: 795f 6e6f 6465 735f 636f 756e 7473 280a  y_nodes_counts(.
+0000b480: 2020 2020 2020 2020 5f4c 4155 4e43 4845          _LAUNCHE
+0000b490: 445f 5245 5345 5256 4544 5f57 4f52 4b45  D_RESERVED_WORKE
+0000b4a0: 525f 5041 5454 4552 4e2c 206f 7574 7075  R_PATTERN, outpu
+0000b4b0: 7429 0a20 2020 2072 6561 6479 5f77 6f72  t).    ready_wor
+0000b4c0: 6b65 7273 202b 3d20 7265 6164 795f 7265  kers += ready_re
+0000b4d0: 7365 7276 6564 5f77 6f72 6b65 7273 0a20  served_workers. 
+0000b4e0: 2020 2061 7373 6572 7420 7265 6164 795f     assert ready_
+0000b4f0: 6865 6164 203c 3d20 312c 2066 2723 6865  head <= 1, f'#he
+0000b500: 6164 206e 6f64 6520 7368 6f75 6c64 2062  ad node should b
+0000b510: 6520 3c3d 3120 2847 6f74 207b 7265 6164  e <=1 (Got {read
+0000b520: 795f 6865 6164 7d29 2e27 0a20 2020 2072  y_head}).'.    r
+0000b530: 6574 7572 6e20 7265 6164 795f 6865 6164  eturn ready_head
+0000b540: 2c20 7265 6164 795f 776f 726b 6572 730a  , ready_workers.
+0000b550: 0a0a 6465 6620 6765 745f 646f 636b 6572  ..def get_docker
+0000b560: 5f75 7365 7228 6970 3a20 7374 722c 2063  _user(ip: str, c
+0000b570: 6c75 7374 6572 5f63 6f6e 6669 675f 6669  luster_config_fi
+0000b580: 6c65 3a20 7374 7229 202d 3e20 7374 723a  le: str) -> str:
+0000b590: 0a20 2020 2022 2222 4669 6e64 2064 6f63  .    """Find doc
+0000b5a0: 6b65 7220 636f 6e74 6169 6e65 7220 7573  ker container us
+0000b5b0: 6572 6e61 6d65 2e22 2222 0a20 2020 2073  ername.""".    s
+0000b5c0: 7368 5f63 7265 6465 6e74 6961 6c73 203d  sh_credentials =
+0000b5d0: 2073 7368 5f63 7265 6465 6e74 6961 6c5f   ssh_credential_
+0000b5e0: 6672 6f6d 5f79 616d 6c28 636c 7573 7465  from_yaml(cluste
+0000b5f0: 725f 636f 6e66 6967 5f66 696c 6529 0a20  r_config_file). 
+0000b600: 2020 2072 756e 6e65 7220 3d20 636f 6d6d     runner = comm
+0000b610: 616e 645f 7275 6e6e 6572 2e53 5348 436f  and_runner.SSHCo
+0000b620: 6d6d 616e 6452 756e 6e65 7228 6e6f 6465  mmandRunner(node
+0000b630: 3d28 6970 2c20 3232 292c 202a 2a73 7368  =(ip, 22), **ssh
+0000b640: 5f63 7265 6465 6e74 6961 6c73 290a 2020  _credentials).  
+0000b650: 2020 636f 6e74 6169 6e65 725f 6e61 6d65    container_name
+0000b660: 203d 2063 6f6e 7374 616e 7473 2e44 4546   = constants.DEF
+0000b670: 4155 4c54 5f44 4f43 4b45 525f 434f 4e54  AULT_DOCKER_CONT
+0000b680: 4149 4e45 525f 4e41 4d45 0a20 2020 2077  AINER_NAME.    w
+0000b690: 686f 616d 695f 7265 7475 726e 636f 6465  hoami_returncode
+0000b6a0: 2c20 7768 6f61 6d69 5f73 7464 6f75 742c  , whoami_stdout,
+0000b6b0: 2077 686f 616d 695f 7374 6465 7272 203d   whoami_stderr =
+0000b6c0: 2072 756e 6e65 722e 7275 6e28 0a20 2020   runner.run(.   
+0000b6d0: 2020 2020 2066 2773 7564 6f20 646f 636b       f'sudo dock
+0000b6e0: 6572 2065 7865 6320 7b63 6f6e 7461 696e  er exec {contain
+0000b6f0: 6572 5f6e 616d 657d 2077 686f 616d 6927  er_name} whoami'
+0000b700: 2c0a 2020 2020 2020 2020 7374 7265 616d  ,.        stream
+0000b710: 5f6c 6f67 733d 4661 6c73 652c 0a20 2020  _logs=False,.   
+0000b720: 2020 2020 2072 6571 7569 7265 5f6f 7574       require_out
+0000b730: 7075 7473 3d54 7275 6529 0a20 2020 2061  puts=True).    a
+0000b740: 7373 6572 7420 7768 6f61 6d69 5f72 6574  ssert whoami_ret
+0000b750: 7572 6e63 6f64 6520 3d3d 2030 2c20 280a  urncode == 0, (.
+0000b760: 2020 2020 2020 2020 6627 4661 696c 6564          f'Failed
+0000b770: 2074 6f20 6765 7420 646f 636b 6572 2063   to get docker c
+0000b780: 6f6e 7461 696e 6572 2075 7365 722e 2052  ontainer user. R
+0000b790: 6574 7572 6e20 270a 2020 2020 2020 2020  eturn '.        
+0000b7a0: 6627 636f 6465 3a20 7b77 686f 616d 695f  f'code: {whoami_
+0000b7b0: 7265 7475 726e 636f 6465 7d2c 2045 7272  returncode}, Err
+0000b7c0: 6f72 3a20 7b77 686f 616d 695f 7374 6465  or: {whoami_stde
+0000b7d0: 7272 7d27 290a 2020 2020 646f 636b 6572  rr}').    docker
+0000b7e0: 5f75 7365 7220 3d20 7768 6f61 6d69 5f73  _user = whoami_s
+0000b7f0: 7464 6f75 742e 7374 7269 7028 290a 2020  tdout.strip().  
+0000b800: 2020 6c6f 6767 6572 2e64 6562 7567 2866    logger.debug(f
+0000b810: 2744 6f63 6b65 7220 636f 6e74 6169 6e65  'Docker containe
+0000b820: 7220 7573 6572 3a20 7b64 6f63 6b65 725f  r user: {docker_
+0000b830: 7573 6572 7d27 290a 2020 2020 7265 7475  user}').    retu
+0000b840: 726e 2064 6f63 6b65 725f 7573 6572 0a0a  rn docker_user..
+0000b850: 0a40 7469 6d65 6c69 6e65 2e65 7665 6e74  .@timeline.event
+0000b860: 0a64 6566 2077 6169 745f 756e 7469 6c5f  .def wait_until_
+0000b870: 7261 795f 636c 7573 7465 725f 7265 6164  ray_cluster_read
+0000b880: 7928 0a20 2020 2063 6c75 7374 6572 5f63  y(.    cluster_c
+0000b890: 6f6e 6669 675f 6669 6c65 3a20 7374 722c  onfig_file: str,
+0000b8a0: 0a20 2020 206e 756d 5f6e 6f64 6573 3a20  .    num_nodes: 
+0000b8b0: 696e 742c 0a20 2020 206c 6f67 5f70 6174  int,.    log_pat
+0000b8c0: 683a 2073 7472 2c0a 2020 2020 6973 5f6c  h: str,.    is_l
+0000b8d0: 6f63 616c 5f63 6c6f 7564 3a20 626f 6f6c  ocal_cloud: bool
+0000b8e0: 203d 2046 616c 7365 2c0a 2020 2020 6e6f   = False,.    no
+0000b8f0: 6465 735f 6c61 756e 6368 696e 675f 7072  des_launching_pr
+0000b900: 6f67 7265 7373 5f74 696d 656f 7574 3a20  ogress_timeout: 
+0000b910: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+0000b920: 4e6f 6e65 2c0a 2920 2d3e 2054 7570 6c65  None,.) -> Tuple
+0000b930: 5b62 6f6f 6c2c 204f 7074 696f 6e61 6c5b  [bool, Optional[
+0000b940: 7374 725d 5d3a 0a20 2020 2022 2222 5761  str]]:.    """Wa
+0000b950: 6974 2075 6e74 696c 2074 6865 2072 6179  it until the ray
+0000b960: 2063 6c75 7374 6572 2069 7320 7365 7420   cluster is set 
+0000b970: 7570 206f 6e20 564d 7320 6f72 2069 6e20  up on VMs or in 
+0000b980: 636f 6e74 6169 6e65 7273 2e0a 0a20 2020  containers...   
+0000b990: 2052 6574 7572 6e73 3a20 2077 6865 7468   Returns:  wheth
+0000b9a0: 6572 2074 6865 2065 6e74 6972 6520 7261  er the entire ra
+0000b9b0: 7920 636c 7573 7465 7220 6973 2072 6561  y cluster is rea
+0000b9c0: 6479 2c20 616e 6420 646f 636b 6572 2075  dy, and docker u
+0000b9d0: 7365 726e 616d 650a 2020 2020 6966 206c  sername.    if l
+0000b9e0: 6175 6e63 6865 6420 7769 7468 2064 6f63  aunched with doc
+0000b9f0: 6b65 722e 0a20 2020 2022 2222 0a20 2020  ker..    """.   
+0000ba00: 2023 204d 616e 7561 6c6c 7920 6665 7463   # Manually fetc
+0000ba10: 6869 6e67 2068 6561 6420 6970 2069 6e73  hing head ip ins
+0000ba20: 7465 6164 206f 6620 7573 696e 6720 6072  tead of using `r
+0000ba30: 6179 2065 7865 6360 2074 6f20 6176 6f69  ay exec` to avoi
+0000ba40: 6420 7468 6520 6275 670a 2020 2020 2320  d the bug.    # 
+0000ba50: 7468 6174 2060 7261 7920 6578 6563 6020  that `ray exec` 
+0000ba60: 6661 696c 7320 746f 2063 6f6e 6e65 6374  fails to connect
+0000ba70: 2074 6f20 7468 6520 6865 6164 206e 6f64   to the head nod
+0000ba80: 6520 6166 7465 7220 736f 6d65 2077 6f72  e after some wor
+0000ba90: 6b65 7273 0a20 2020 2023 206c 6175 6e63  kers.    # launc
+0000baa0: 6865 6420 6573 7065 6369 616c 6c79 2066  hed especially f
+0000bab0: 6f72 2041 7a75 7265 2e0a 2020 2020 7472  or Azure..    tr
+0000bac0: 793a 0a20 2020 2020 2020 2068 6561 645f  y:.        head_
+0000bad0: 6970 203d 205f 7175 6572 795f 6865 6164  ip = _query_head
+0000bae0: 5f69 705f 7769 7468 5f72 6574 7269 6573  _ip_with_retries
+0000baf0: 280a 2020 2020 2020 2020 2020 2020 636c  (.            cl
+0000bb00: 7573 7465 725f 636f 6e66 6967 5f66 696c  uster_config_fil
+0000bb10: 652c 206d 6178 5f61 7474 656d 7074 733d  e, max_attempts=
+0000bb20: 5741 4954 5f48 4541 445f 4e4f 4445 5f49  WAIT_HEAD_NODE_I
+0000bb30: 505f 4d41 585f 4154 5445 4d50 5453 290a  P_MAX_ATTEMPTS).
+0000bb40: 2020 2020 6578 6365 7074 2065 7863 6570      except excep
+0000bb50: 7469 6f6e 732e 4665 7463 6843 6c75 7374  tions.FetchClust
+0000bb60: 6572 496e 666f 4572 726f 7220 6173 2065  erInfoError as e
+0000bb70: 3a0a 2020 2020 2020 2020 6c6f 6767 6572  :.        logger
+0000bb80: 2e65 7272 6f72 2863 6f6d 6d6f 6e5f 7574  .error(common_ut
+0000bb90: 696c 732e 666f 726d 6174 5f65 7863 6570  ils.format_excep
+0000bba0: 7469 6f6e 2865 2929 0a20 2020 2020 2020  tion(e)).       
+0000bbb0: 2072 6574 7572 6e20 4661 6c73 652c 204e   return False, N
+0000bbc0: 6f6e 6520 2023 2066 6169 6c65 640a 0a20  one  # failed.. 
+0000bbd0: 2020 2063 6f6e 6669 6720 3d20 636f 6d6d     config = comm
+0000bbe0: 6f6e 5f75 7469 6c73 2e72 6561 645f 7961  on_utils.read_ya
+0000bbf0: 6d6c 2863 6c75 7374 6572 5f63 6f6e 6669  ml(cluster_confi
+0000bc00: 675f 6669 6c65 290a 0a20 2020 2064 6f63  g_file)..    doc
+0000bc10: 6b65 725f 7573 6572 203d 204e 6f6e 650a  ker_user = None.
+0000bc20: 2020 2020 6966 2027 646f 636b 6572 2720      if 'docker' 
+0000bc30: 696e 2063 6f6e 6669 673a 0a20 2020 2020  in config:.     
+0000bc40: 2020 2064 6f63 6b65 725f 7573 6572 203d     docker_user =
+0000bc50: 2067 6574 5f64 6f63 6b65 725f 7573 6572   get_docker_user
+0000bc60: 2868 6561 645f 6970 2c20 636c 7573 7465  (head_ip, cluste
+0000bc70: 725f 636f 6e66 6967 5f66 696c 6529 0a0a  r_config_file)..
+0000bc80: 2020 2020 6966 206e 756d 5f6e 6f64 6573      if num_nodes
+0000bc90: 203c 3d20 313a 0a20 2020 2020 2020 2072   <= 1:.        r
+0000bca0: 6574 7572 6e20 5472 7565 2c20 646f 636b  eturn True, dock
+0000bcb0: 6572 5f75 7365 720a 0a20 2020 2073 7368  er_user..    ssh
+0000bcc0: 5f63 7265 6465 6e74 6961 6c73 203d 2073  _credentials = s
+0000bcd0: 7368 5f63 7265 6465 6e74 6961 6c5f 6672  sh_credential_fr
+0000bce0: 6f6d 5f79 616d 6c28 636c 7573 7465 725f  om_yaml(cluster_
+0000bcf0: 636f 6e66 6967 5f66 696c 652c 2064 6f63  config_file, doc
+0000bd00: 6b65 725f 7573 6572 290a 2020 2020 6c61  ker_user).    la
+0000bd10: 7374 5f6e 6f64 6573 5f73 6f5f 6661 7220  st_nodes_so_far 
+0000bd20: 3d20 300a 2020 2020 7374 6172 7420 3d20  = 0.    start = 
+0000bd30: 7469 6d65 2e74 696d 6528 290a 2020 2020  time.time().    
+0000bd40: 7275 6e6e 6572 203d 2063 6f6d 6d61 6e64  runner = command
+0000bd50: 5f72 756e 6e65 722e 5353 4843 6f6d 6d61  _runner.SSHComma
+0000bd60: 6e64 5275 6e6e 6572 286e 6f64 653d 2868  ndRunner(node=(h
+0000bd70: 6561 645f 6970 2c20 3232 292c 0a20 2020  ead_ip, 22),.   
 0000bd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd90: 2020 2a2a 7373 685f 6372 6564 656e 7469    **ssh_credenti
-0000bda0: 616c 7329 0a20 2020 2077 6974 6820 7269  als).    with ri
-0000bdb0: 6368 5f75 7469 6c73 2e73 6166 655f 7374  ch_utils.safe_st
-0000bdc0: 6174 7573 280a 2020 2020 2020 2020 2020  atus(.          
-0000bdd0: 2020 275b 626f 6c64 2063 7961 6e5d 5761    '[bold cyan]Wa
-0000bde0: 6974 696e 6720 666f 7220 776f 726b 6572  iting for worker
-0000bdf0: 732e 2e2e 2729 2061 7320 776f 726b 6572  s...') as worker
-0000be00: 5f73 7461 7475 733a 0a20 2020 2020 2020  _status:.       
-0000be10: 2077 6869 6c65 2054 7275 653a 0a20 2020   while True:.   
-0000be20: 2020 2020 2020 2020 2072 632c 206f 7574           rc, out
-0000be30: 7075 742c 2073 7464 6572 7220 3d20 7275  put, stderr = ru
-0000be40: 6e6e 6572 2e72 756e 280a 2020 2020 2020  nner.run(.      
-0000be50: 2020 2020 2020 2020 2020 696e 7374 616e            instan
-0000be60: 6365 5f73 6574 7570 2e52 4159 5f53 5441  ce_setup.RAY_STA
-0000be70: 5455 535f 5749 5448 5f53 4b59 5f52 4159  TUS_WITH_SKY_RAY
-0000be80: 5f50 4f52 545f 434f 4d4d 414e 442c 0a20  _PORT_COMMAND,. 
-0000be90: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0000bea0: 6f67 5f70 6174 683d 6c6f 675f 7061 7468  og_path=log_path
-0000beb0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000bec0: 2020 7374 7265 616d 5f6c 6f67 733d 4661    stream_logs=Fa
-0000bed0: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
-0000bee0: 2020 2020 2072 6571 7569 7265 5f6f 7574       require_out
-0000bef0: 7075 7473 3d54 7275 652c 0a20 2020 2020  puts=True,.     
-0000bf00: 2020 2020 2020 2020 2020 2073 6570 6172             separ
-0000bf10: 6174 655f 7374 6465 7272 3d54 7275 6529  ate_stderr=True)
-0000bf20: 0a20 2020 2020 2020 2020 2020 2073 7562  .            sub
-0000bf30: 7072 6f63 6573 735f 7574 696c 732e 6861  process_utils.ha
-0000bf40: 6e64 6c65 5f72 6574 7572 6e63 6f64 6528  ndle_returncode(
-0000bf50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bf60: 2072 632c 2069 6e73 7461 6e63 655f 7365   rc, instance_se
-0000bf70: 7475 702e 5241 595f 5354 4154 5553 5f57  tup.RAY_STATUS_W
-0000bf80: 4954 485f 534b 595f 5241 595f 504f 5254  ITH_SKY_RAY_PORT
-0000bf90: 5f43 4f4d 4d41 4e44 2c0a 2020 2020 2020  _COMMAND,.      
-0000bfa0: 2020 2020 2020 2020 2020 2746 6169 6c65            'Faile
-0000bfb0: 6420 746f 2072 756e 2072 6179 2073 7461  d to run ray sta
-0000bfc0: 7475 7320 6f6e 2068 6561 6420 6e6f 6465  tus on head node
-0000bfd0: 2e27 2c20 7374 6465 7272 290a 2020 2020  .', stderr).    
-0000bfe0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-0000bff0: 6562 7567 286f 7574 7075 7429 0a0a 2020  ebug(output)..  
-0000c000: 2020 2020 2020 2020 2020 7265 6164 795f            ready_
-0000c010: 6865 6164 2c20 7265 6164 795f 776f 726b  head, ready_work
-0000c020: 6572 7320 3d20 5f63 6f75 6e74 5f68 6561  ers = _count_hea
-0000c030: 6c74 6879 5f6e 6f64 6573 5f66 726f 6d5f  lthy_nodes_from_
-0000c040: 7261 7928 0a20 2020 2020 2020 2020 2020  ray(.           
-0000c050: 2020 2020 206f 7574 7075 742c 2069 735f       output, is_
-0000c060: 6c6f 6361 6c5f 636c 6f75 643d 6973 5f6c  local_cloud=is_l
-0000c070: 6f63 616c 5f63 6c6f 7564 290a 0a20 2020  ocal_cloud)..   
-0000c080: 2020 2020 2020 2020 2077 6f72 6b65 725f           worker_
-0000c090: 7374 6174 7573 2e75 7064 6174 6528 275b  status.update('[
-0000c0a0: 626f 6c64 2063 7961 6e5d 270a 2020 2020  bold cyan]'.    
-0000c0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0c0: 2020 2020 2020 2020 2020 2020 2066 277b               f'{
-0000c0d0: 7265 6164 795f 776f 726b 6572 737d 206f  ready_workers} o
-0000c0e0: 7574 206f 6620 7b6e 756d 5f6e 6f64 6573  ut of {num_nodes
-0000c0f0: 202d 2031 7d20 270a 2020 2020 2020 2020   - 1} '.        
-0000c100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c110: 2020 2020 2020 2020 2027 776f 726b 6572           'worker
-0000c120: 7320 7265 6164 7927 290a 0a20 2020 2020  s ready')..     
-0000c130: 2020 2020 2020 2023 2049 6e20 7468 6520         # In the 
-0000c140: 6c6f 6361 6c20 6361 7365 2c20 7265 6164  local case, read
-0000c150: 795f 6865 6164 3d30 2061 6e64 2072 6561  y_head=0 and rea
-0000c160: 6479 5f77 6f72 6b65 7273 3d6e 756d 5f6e  dy_workers=num_n
-0000c170: 6f64 6573 2e20 5468 6973 0a20 2020 2020  odes. This.     
-0000c180: 2020 2020 2020 2023 2069 7320 6265 6361         # is beca
-0000c190: 7573 6520 7468 6572 6520 6973 206e 6f20  use there is no 
-0000c1a0: 6d61 7463 6869 6e67 2072 6567 6578 2066  matching regex f
-0000c1b0: 6f72 205f 4c41 554e 4348 4544 5f48 4541  or _LAUNCHED_HEA
-0000c1c0: 445f 5041 5454 4552 4e2e 0a20 2020 2020  D_PATTERN..     
-0000c1d0: 2020 2020 2020 2069 6620 7265 6164 795f         if ready_
-0000c1e0: 6865 6164 202b 2072 6561 6479 5f77 6f72  head + ready_wor
-0000c1f0: 6b65 7273 203d 3d20 6e75 6d5f 6e6f 6465  kers == num_node
-0000c200: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-0000c210: 2020 2023 2041 6c6c 206e 6f64 6573 2061     # All nodes a
-0000c220: 7265 2075 702e 0a20 2020 2020 2020 2020  re up..         
-0000c230: 2020 2020 2020 2062 7265 616b 0a0a 2020         break..  
-0000c240: 2020 2020 2020 2020 2020 2320 5065 6e64            # Pend
-0000c250: 696e 6720 776f 726b 6572 7320 7468 6174  ing workers that
-0000c260: 2068 6176 6520 6265 656e 206c 6175 6e63   have been launc
-0000c270: 6865 6420 6279 2072 6179 2075 702e 0a20  hed by ray up.. 
-0000c280: 2020 2020 2020 2020 2020 2066 6f75 6e64             found
-0000c290: 5f69 7073 203d 205f 4c41 554e 4348 494e  _ips = _LAUNCHIN
-0000c2a0: 475f 4950 5f50 4154 5445 524e 2e66 696e  G_IP_PATTERN.fin
-0000c2b0: 6461 6c6c 286f 7574 7075 7429 0a20 2020  dall(output).   
-0000c2c0: 2020 2020 2020 2020 2070 656e 6469 6e67           pending
-0000c2d0: 5f77 6f72 6b65 7273 203d 206c 656e 2866  _workers = len(f
-0000c2e0: 6f75 6e64 5f69 7073 290a 0a20 2020 2020  ound_ips)..     
-0000c2f0: 2020 2020 2020 2023 2054 4f44 4f28 7a68         # TODO(zh
-0000c300: 7775 293a 2048 616e 646c 6520 7468 6520  wu): Handle the 
-0000c310: 6361 7365 2077 6865 7265 2074 6865 2066  case where the f
-0000c320: 6f6c 6c6f 7769 6e67 206f 6363 7572 732c  ollowing occurs,
-0000c330: 2077 6865 7265 2072 6179 0a20 2020 2020   where ray.     
-0000c340: 2020 2020 2020 2023 2063 6c75 7374 6572         # cluster
-0000c350: 2069 7320 6e6f 7420 636f 7272 6563 746c   is not correctl
-0000c360: 7920 7374 6172 7465 6420 6f6e 2074 6865  y started on the
-0000c370: 2063 6c75 7374 6572 2e0a 2020 2020 2020   cluster..      
-0000c380: 2020 2020 2020 2320 5065 6e64 696e 673a        # Pending:
-0000c390: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
-0000c3a0: 3137 322e 3331 2e39 2e31 3231 3a20 7261  172.31.9.121: ra
-0000c3b0: 792e 776f 726b 6572 2e64 6566 6175 6c74  y.worker.default
-0000c3c0: 2c20 756e 696e 6974 6961 6c69 7a65 640a  , uninitialized.
-0000c3d0: 2020 2020 2020 2020 2020 2020 6e6f 6465              node
-0000c3e0: 735f 736f 5f66 6172 203d 2072 6561 6479  s_so_far = ready
-0000c3f0: 5f68 6561 6420 2b20 7265 6164 795f 776f  _head + ready_wo
-0000c400: 726b 6572 7320 2b20 7065 6e64 696e 675f  rkers + pending_
-0000c410: 776f 726b 6572 730a 0a20 2020 2020 2020  workers..       
-0000c420: 2020 2020 2023 2043 6865 636b 2074 6865       # Check the
-0000c430: 206e 756d 6265 7220 6f66 206e 6f64 6573   number of nodes
-0000c440: 2074 6861 7420 6172 6520 6665 7463 6865   that are fetche
-0000c450: 642e 2054 696d 656f 7574 2069 6620 6e6f  d. Timeout if no
-0000c460: 206e 6577 0a20 2020 2020 2020 2020 2020   new.           
-0000c470: 2023 206e 6f64 6573 2066 6574 6368 6564   # nodes fetched
-0000c480: 2069 6e20 6120 7768 696c 6520 286e 6f64   in a while (nod
-0000c490: 6573 5f6c 6175 6e63 6869 6e67 5f70 726f  es_launching_pro
-0000c4a0: 6772 6573 735f 7469 6d65 6f75 7429 2c0a  gress_timeout),.
-0000c4b0: 2020 2020 2020 2020 2020 2020 2320 7468              # th
-0000c4c0: 6f75 6768 206e 756d 6265 7220 6f66 206e  ough number of n
-0000c4d0: 6f64 6573 5f73 6f5f 6661 7220 6973 2073  odes_so_far is s
-0000c4e0: 7469 6c6c 206e 6f74 2061 7320 6578 7065  till not as expe
-0000c4f0: 6374 6564 2e0a 2020 2020 2020 2020 2020  cted..          
-0000c500: 2020 6966 206e 6f64 6573 5f73 6f5f 6661    if nodes_so_fa
-0000c510: 7220 3e20 6c61 7374 5f6e 6f64 6573 5f73  r > last_nodes_s
-0000c520: 6f5f 6661 723a 0a20 2020 2020 2020 2020  o_far:.         
-0000c530: 2020 2020 2020 2023 2052 6573 6574 2074         # Reset t
-0000c540: 6865 2073 7461 7274 2074 696d 6520 6966  he start time if
-0000c550: 2074 6865 206e 756d 6265 7220 6f66 206c   the number of l
-0000c560: 6175 6e63 6869 6e67 206e 6f64 6573 0a20  aunching nodes. 
-0000c570: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000c580: 2063 6861 6e67 6573 2c20 692e 652e 206e   changes, i.e. n
-0000c590: 6577 206e 6f64 6573 2061 7265 206c 6175  ew nodes are lau
-0000c5a0: 6e63 6865 642e 0a20 2020 2020 2020 2020  nched..         
-0000c5b0: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-0000c5c0: 6275 6728 2752 6573 6574 2073 7461 7274  bug('Reset start
-0000c5d0: 2074 696d 652c 2061 7320 6e65 7720 6e6f   time, as new no
-0000c5e0: 6465 7320 6172 6520 6c61 756e 6368 6564  des are launched
-0000c5f0: 2e20 270a 2020 2020 2020 2020 2020 2020  . '.            
-0000c600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c610: 2066 2728 7b6c 6173 745f 6e6f 6465 735f   f'({last_nodes_
-0000c620: 736f 5f66 6172 7d20 2d3e 207b 6e6f 6465  so_far} -> {node
-0000c630: 735f 736f 5f66 6172 7d29 2729 0a20 2020  s_so_far})').   
-0000c640: 2020 2020 2020 2020 2020 2020 2073 7461               sta
-0000c650: 7274 203d 2074 696d 652e 7469 6d65 2829  rt = time.time()
-0000c660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c670: 206c 6173 745f 6e6f 6465 735f 736f 5f66   last_nodes_so_f
-0000c680: 6172 203d 206e 6f64 6573 5f73 6f5f 6661  ar = nodes_so_fa
-0000c690: 720a 2020 2020 2020 2020 2020 2020 656c  r.            el
-0000c6a0: 6966 2028 6e6f 6465 735f 6c61 756e 6368  if (nodes_launch
-0000c6b0: 696e 675f 7072 6f67 7265 7373 5f74 696d  ing_progress_tim
-0000c6c0: 656f 7574 2069 7320 6e6f 7420 4e6f 6e65  eout is not None
-0000c6d0: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
-0000c6e0: 2020 2020 2020 2074 696d 652e 7469 6d65         time.time
-0000c6f0: 2829 202d 2073 7461 7274 203e 206e 6f64  () - start > nod
-0000c700: 6573 5f6c 6175 6e63 6869 6e67 5f70 726f  es_launching_pro
-0000c710: 6772 6573 735f 7469 6d65 6f75 7420 616e  gress_timeout an
-0000c720: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-0000c730: 2020 2020 6e6f 6465 735f 736f 5f66 6172      nodes_so_far
-0000c740: 2021 3d20 6e75 6d5f 6e6f 6465 7329 3a0a   != num_nodes):.
-0000c750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c760: 6c6f 6767 6572 2e65 7272 6f72 280a 2020  logger.error(.  
-0000c770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c780: 2020 2754 696d 6564 206f 7574 3a20 7761    'Timed out: wa
-0000c790: 6974 6564 2066 6f72 206d 6f72 6520 7468  ited for more th
-0000c7a0: 616e 2027 0a20 2020 2020 2020 2020 2020  an '.           
-0000c7b0: 2020 2020 2020 2020 2066 277b 6e6f 6465           f'{node
-0000c7c0: 735f 6c61 756e 6368 696e 675f 7072 6f67  s_launching_prog
-0000c7d0: 7265 7373 5f74 696d 656f 7574 7d20 7365  ress_timeout} se
-0000c7e0: 636f 6e64 7320 666f 7220 6e65 7720 270a  conds for new '.
-0000c7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c800: 2020 2020 2777 6f72 6b65 7273 2074 6f20      'workers to 
-0000c810: 6265 2070 726f 7669 7369 6f6e 6564 2c20  be provisioned, 
-0000c820: 6275 7420 6e6f 2070 726f 6772 6573 732e  but no progress.
-0000c830: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
-0000c840: 2020 2072 6574 7572 6e20 4661 6c73 652c     return False,
-0000c850: 204e 6f6e 6520 2023 2066 6169 6c65 640a   None  # failed.
-0000c860: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000c870: 2728 6e6f 2070 656e 6469 6e67 206e 6f64  '(no pending nod
-0000c880: 6573 2927 2069 6e20 6f75 7470 7574 2061  es)' in output a
-0000c890: 6e64 2027 286e 6f20 6661 696c 7572 6573  nd '(no failures
-0000c8a0: 2927 2069 6e20 6f75 7470 7574 3a0a 2020  )' in output:.  
-0000c8b0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000c8c0: 4275 6720 696e 2072 6179 2061 7574 6f73  Bug in ray autos
-0000c8d0: 6361 6c65 723a 2065 2e67 2e2c 206f 6e20  caler: e.g., on 
-0000c8e0: 4743 502c 2069 6620 7265 7175 6573 7469  GCP, if requesti
-0000c8f0: 6e67 2032 206e 6f64 6573 0a20 2020 2020  ng 2 nodes.     
-0000c900: 2020 2020 2020 2020 2020 2023 2074 6861             # tha
-0000c910: 7420 4743 5020 6361 6e20 7361 7469 7366  t GCP can satisf
-0000c920: 7920 6f6e 6c79 2062 7920 6861 6c66 2c20  y only by half, 
-0000c930: 7468 6520 776f 726b 6572 206e 6f64 6520  the worker node 
-0000c940: 776f 756c 6420 6265 0a20 2020 2020 2020  would be.       
-0000c950: 2020 2020 2020 2020 2023 2066 6f72 676f           # forgo
-0000c960: 7474 656e 2e20 5468 6520 636f 7272 6563  tten. The correc
-0000c970: 7420 6265 6861 7669 6f72 2073 686f 756c  t behavior shoul
-0000c980: 6420 6265 2066 6f72 2069 7420 746f 2065  d be for it to e
-0000c990: 7272 6f72 206f 7574 2e0a 2020 2020 2020  rror out..      
-0000c9a0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-0000c9b0: 2e65 7272 6f72 280a 2020 2020 2020 2020  .error(.        
-0000c9c0: 2020 2020 2020 2020 2020 2020 2746 6169              'Fai
-0000c9d0: 6c65 6420 746f 206c 6175 6e63 6820 6d75  led to launch mu
-0000c9e0: 6c74 6970 6c65 206e 6f64 6573 206f 6e20  ltiple nodes on 
-0000c9f0: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-0000ca00: 2020 2020 2020 2747 4350 2064 7565 2074        'GCP due t
-0000ca10: 6f20 6120 6e6f 6e64 6574 6572 6d69 6e69  o a nondetermini
-0000ca20: 7374 6963 2062 7567 2069 6e20 7261 7920  stic bug in ray 
-0000ca30: 6175 746f 7363 616c 6572 2e27 290a 2020  autoscaler.').  
-0000ca40: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000ca50: 7475 726e 2046 616c 7365 2c20 4e6f 6e65  turn False, None
-0000ca60: 2020 2320 6661 696c 6564 0a20 2020 2020    # failed.     
-0000ca70: 2020 2020 2020 2074 696d 652e 736c 6565         time.slee
-0000ca80: 7028 3130 290a 2020 2020 7265 7475 726e  p(10).    return
-0000ca90: 2054 7275 652c 2064 6f63 6b65 725f 7573   True, docker_us
-0000caa0: 6572 2020 2320 7375 6363 6573 730a 0a0a  er  # success...
-0000cab0: 6465 6620 7373 685f 6372 6564 656e 7469  def ssh_credenti
-0000cac0: 616c 5f66 726f 6d5f 7961 6d6c 280a 2020  al_from_yaml(.  
-0000cad0: 2020 636c 7573 7465 725f 7961 6d6c 3a20    cluster_yaml: 
-0000cae0: 7374 722c 0a20 2020 2064 6f63 6b65 725f  str,.    docker_
-0000caf0: 7573 6572 3a20 4f70 7469 6f6e 616c 5b73  user: Optional[s
-0000cb00: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
-0000cb10: 7373 685f 7573 6572 3a20 4f70 7469 6f6e  ssh_user: Option
-0000cb20: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
-0000cb30: 2920 2d3e 2044 6963 745b 7374 722c 2041  ) -> Dict[str, A
-0000cb40: 6e79 5d3a 0a20 2020 2022 2222 5265 7475  ny]:.    """Retu
-0000cb50: 726e 7320 7373 685f 7573 6572 2c20 7373  rns ssh_user, ss
-0000cb60: 685f 7072 6976 6174 655f 6b65 7920 616e  h_private_key an
-0000cb70: 6420 7373 685f 636f 6e74 726f 6c20 6e61  d ssh_control na
-0000cb80: 6d65 2e0a 0a20 2020 2041 7267 733a 0a20  me...    Args:. 
-0000cb90: 2020 2020 2020 2063 6c75 7374 6572 5f79         cluster_y
-0000cba0: 616d 6c3a 2070 6174 6820 746f 2074 6865  aml: path to the
-0000cbb0: 2063 6c75 7374 6572 2079 616d 6c2e 0a20   cluster yaml.. 
-0000cbc0: 2020 2020 2020 2064 6f63 6b65 725f 7573         docker_us
-0000cbd0: 6572 3a20 7768 656e 2075 7369 6e67 2063  er: when using c
-0000cbe0: 7573 746f 6d20 646f 636b 6572 2069 6d61  ustom docker ima
-0000cbf0: 6765 2c20 7573 6520 7468 6973 2075 7365  ge, use this use
-0000cc00: 7220 746f 2073 7368 2069 6e74 6f0a 2020  r to ssh into.  
-0000cc10: 2020 2020 2020 2020 2020 7468 6520 646f            the do
-0000cc20: 636b 6572 2063 6f6e 7461 696e 6572 2e0a  cker container..
-0000cc30: 2020 2020 2020 2020 7373 685f 7573 6572          ssh_user
-0000cc40: 3a20 6f76 6572 7269 6465 2074 6865 2073  : override the s
-0000cc50: 7368 5f75 7365 7220 696e 2074 6865 2063  sh_user in the c
-0000cc60: 6c75 7374 6572 2079 616d 6c2e 0a20 2020  luster yaml..   
-0000cc70: 2022 2222 0a20 2020 2063 6f6e 6669 6720   """.    config 
-0000cc80: 3d20 636f 6d6d 6f6e 5f75 7469 6c73 2e72  = common_utils.r
-0000cc90: 6561 645f 7961 6d6c 2863 6c75 7374 6572  ead_yaml(cluster
-0000cca0: 5f79 616d 6c29 0a20 2020 2061 7574 685f  _yaml).    auth_
-0000ccb0: 7365 6374 696f 6e20 3d20 636f 6e66 6967  section = config
-0000ccc0: 5b27 6175 7468 275d 0a20 2020 2069 6620  ['auth'].    if 
-0000ccd0: 7373 685f 7573 6572 2069 7320 4e6f 6e65  ssh_user is None
-0000cce0: 3a0a 2020 2020 2020 2020 7373 685f 7573  :.        ssh_us
-0000ccf0: 6572 203d 2061 7574 685f 7365 6374 696f  er = auth_sectio
-0000cd00: 6e5b 2773 7368 5f75 7365 7227 5d2e 7374  n['ssh_user'].st
-0000cd10: 7269 7028 290a 2020 2020 7373 685f 7072  rip().    ssh_pr
-0000cd20: 6976 6174 655f 6b65 7920 3d20 6175 7468  ivate_key = auth
-0000cd30: 5f73 6563 7469 6f6e 2e67 6574 2827 7373  _section.get('ss
-0000cd40: 685f 7072 6976 6174 655f 6b65 7927 290a  h_private_key').
-0000cd50: 2020 2020 7373 685f 636f 6e74 726f 6c5f      ssh_control_
-0000cd60: 6e61 6d65 203d 2063 6f6e 6669 672e 6765  name = config.ge
-0000cd70: 7428 2763 6c75 7374 6572 5f6e 616d 6527  t('cluster_name'
-0000cd80: 2c20 275f 5f64 6566 6175 6c74 5f5f 2729  , '__default__')
-0000cd90: 0a20 2020 2073 7368 5f70 726f 7879 5f63  .    ssh_proxy_c
-0000cda0: 6f6d 6d61 6e64 203d 2061 7574 685f 7365  ommand = auth_se
-0000cdb0: 6374 696f 6e2e 6765 7428 2773 7368 5f70  ction.get('ssh_p
-0000cdc0: 726f 7879 5f63 6f6d 6d61 6e64 2729 0a20  roxy_command'). 
-0000cdd0: 2020 2063 7265 6465 6e74 6961 6c73 203d     credentials =
-0000cde0: 207b 0a20 2020 2020 2020 2027 7373 685f   {.        'ssh_
-0000cdf0: 7573 6572 273a 2073 7368 5f75 7365 722c  user': ssh_user,
-0000ce00: 0a20 2020 2020 2020 2027 7373 685f 7072  .        'ssh_pr
-0000ce10: 6976 6174 655f 6b65 7927 3a20 7373 685f  ivate_key': ssh_
-0000ce20: 7072 6976 6174 655f 6b65 792c 0a20 2020  private_key,.   
-0000ce30: 2020 2020 2027 7373 685f 636f 6e74 726f       'ssh_contro
-0000ce40: 6c5f 6e61 6d65 273a 2073 7368 5f63 6f6e  l_name': ssh_con
-0000ce50: 7472 6f6c 5f6e 616d 652c 0a20 2020 2020  trol_name,.     
-0000ce60: 2020 2027 7373 685f 7072 6f78 795f 636f     'ssh_proxy_co
-0000ce70: 6d6d 616e 6427 3a20 7373 685f 7072 6f78  mmand': ssh_prox
-0000ce80: 795f 636f 6d6d 616e 642c 0a20 2020 207d  y_command,.    }
-0000ce90: 0a20 2020 2069 6620 646f 636b 6572 5f75  .    if docker_u
-0000cea0: 7365 7220 6973 206e 6f74 204e 6f6e 653a  ser is not None:
-0000ceb0: 0a20 2020 2020 2020 2063 7265 6465 6e74  .        credent
-0000cec0: 6961 6c73 5b27 646f 636b 6572 5f75 7365  ials['docker_use
-0000ced0: 7227 5d20 3d20 646f 636b 6572 5f75 7365  r'] = docker_use
-0000cee0: 720a 2020 2020 7373 685f 7072 6f76 6964  r.    ssh_provid
-0000cef0: 6572 5f6d 6f64 756c 6520 3d20 636f 6e66  er_module = conf
-0000cf00: 6967 5b27 7072 6f76 6964 6572 275d 5b27  ig['provider']['
-0000cf10: 6d6f 6475 6c65 275d 0a20 2020 2023 2049  module'].    # I
-0000cf20: 6620 7765 2061 7265 2072 756e 6e69 6e67  f we are running
-0000cf30: 2073 7368 2063 6f6d 6d61 6e64 206f 6e20   ssh command on 
-0000cf40: 6b75 6265 726e 6574 6573 206e 6f64 652e  kubernetes node.
-0000cf50: 0a20 2020 2069 6620 276b 7562 6572 6e65  .    if 'kuberne
-0000cf60: 7465 7327 2069 6e20 7373 685f 7072 6f76  tes' in ssh_prov
-0000cf70: 6964 6572 5f6d 6f64 756c 653a 0a20 2020  ider_module:.   
-0000cf80: 2020 2020 2063 7265 6465 6e74 6961 6c73       credentials
-0000cf90: 5b27 6469 7361 626c 655f 636f 6e74 726f  ['disable_contro
-0000cfa0: 6c5f 6d61 7374 6572 275d 203d 2054 7275  l_master'] = Tru
-0000cfb0: 650a 2020 2020 7265 7475 726e 2063 7265  e.    return cre
-0000cfc0: 6465 6e74 6961 6c73 0a0a 0a64 6566 2070  dentials...def p
-0000cfd0: 6172 616c 6c65 6c5f 6461 7461 5f74 7261  arallel_data_tra
-0000cfe0: 6e73 6665 725f 746f 5f6e 6f64 6573 280a  nsfer_to_nodes(.
-0000cff0: 2020 2020 7275 6e6e 6572 733a 204c 6973      runners: Lis
-0000d000: 745b 636f 6d6d 616e 645f 7275 6e6e 6572  t[command_runner
-0000d010: 2e43 6f6d 6d61 6e64 5275 6e6e 6572 5d2c  .CommandRunner],
-0000d020: 0a20 2020 2073 6f75 7263 653a 204f 7074  .    source: Opt
-0000d030: 696f 6e61 6c5b 7374 725d 2c0a 2020 2020  ional[str],.    
-0000d040: 7461 7267 6574 3a20 7374 722c 0a20 2020  target: str,.   
-0000d050: 2063 6d64 3a20 4f70 7469 6f6e 616c 5b73   cmd: Optional[s
-0000d060: 7472 5d2c 0a20 2020 2072 756e 5f72 7379  tr],.    run_rsy
-0000d070: 6e63 3a20 626f 6f6c 2c0a 2020 2020 2a2c  nc: bool,.    *,
-0000d080: 0a20 2020 2061 6374 696f 6e5f 6d65 7373  .    action_mess
-0000d090: 6167 653a 2073 7472 2c0a 2020 2020 2320  age: str,.    # 
-0000d0a0: 4164 7661 6e63 6564 206f 7074 696f 6e73  Advanced options
-0000d0b0: 2e0a 2020 2020 6c6f 675f 7061 7468 3a20  ..    log_path: 
-0000d0c0: 7374 7220 3d20 6f73 2e64 6576 6e75 6c6c  str = os.devnull
-0000d0d0: 2c0a 2020 2020 7374 7265 616d 5f6c 6f67  ,.    stream_log
-0000d0e0: 733a 2062 6f6f 6c20 3d20 4661 6c73 652c  s: bool = False,
-0000d0f0: 0a20 2020 2073 6f75 7263 655f 6261 7368  .    source_bash
-0000d100: 7263 3a20 626f 6f6c 203d 2046 616c 7365  rc: bool = False
-0000d110: 2c0a 293a 0a20 2020 2022 2222 5275 6e73  ,.):.    """Runs
-0000d120: 2061 2063 6f6d 6d61 6e64 206f 6e20 616c   a command on al
-0000d130: 6c20 6e6f 6465 7320 616e 6420 6f70 7469  l nodes and opti
-0000d140: 6f6e 616c 6c79 2072 756e 7320 7273 796e  onally runs rsyn
-0000d150: 6320 6672 6f6d 2073 7263 2d3e 6473 742e  c from src->dst.
-0000d160: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
-0000d170: 2020 2020 7275 6e6e 6572 733a 2041 206c      runners: A l
-0000d180: 6973 7420 6f66 2043 6f6d 6d61 6e64 5275  ist of CommandRu
-0000d190: 6e6e 6572 206f 626a 6563 7473 2074 6861  nner objects tha
-0000d1a0: 7420 7265 7072 6573 656e 7420 6d75 6c74  t represent mult
-0000d1b0: 6970 6c65 206e 6f64 6573 2e0a 2020 2020  iple nodes..    
-0000d1c0: 2020 2020 736f 7572 6365 3a20 4f70 7469      source: Opti
-0000d1d0: 6f6e 616c 5b73 7472 5d3b 2053 6f75 7263  onal[str]; Sourc
-0000d1e0: 6520 666f 7220 7273 796e 6320 6f6e 206c  e for rsync on l
-0000d1f0: 6f63 616c 206e 6f64 650a 2020 2020 2020  ocal node.      
-0000d200: 2020 7461 7267 6574 3a20 7374 723b 2044    target: str; D
-0000d210: 6573 7469 6e61 7469 6f6e 206f 6e20 7265  estination on re
-0000d220: 6d6f 7465 206e 6f64 6520 666f 7220 7273  mote node for rs
-0000d230: 796e 630a 2020 2020 2020 2020 636d 643a  ync.        cmd:
-0000d240: 2073 7472 3b20 436f 6d6d 616e 6420 746f   str; Command to
-0000d250: 2062 6520 6578 6563 7574 6564 206f 6e20   be executed on 
-0000d260: 616c 6c20 6e6f 6465 730a 2020 2020 2020  all nodes.      
-0000d270: 2020 6163 7469 6f6e 5f6d 6573 7361 6765    action_message
-0000d280: 3a20 7374 723b 204d 6573 7361 6765 2074  : str; Message t
-0000d290: 6f20 6265 2070 7269 6e74 6564 2077 6869  o be printed whi
-0000d2a0: 6c65 2074 6865 2063 6f6d 6d61 6e64 2072  le the command r
-0000d2b0: 756e 730a 2020 2020 2020 2020 6c6f 675f  uns.        log_
-0000d2c0: 7061 7468 3a20 7374 723b 2050 6174 6820  path: str; Path 
-0000d2d0: 746f 2074 6865 206c 6f67 2066 696c 650a  to the log file.
-0000d2e0: 2020 2020 2020 2020 7374 7265 616d 5f6c          stream_l
-0000d2f0: 6f67 733a 2062 6f6f 6c3b 2057 6865 7468  ogs: bool; Wheth
-0000d300: 6572 2074 6f20 7374 7265 616d 206c 6f67  er to stream log
-0000d310: 7320 746f 2073 7464 6f75 740a 2020 2020  s to stdout.    
-0000d320: 2020 2020 736f 7572 6365 5f62 6173 6872      source_bashr
-0000d330: 633a 2062 6f6f 6c3b 2053 6f75 7263 6520  c: bool; Source 
-0000d340: 6261 7368 7263 2062 6566 6f72 6520 7275  bashrc before ru
-0000d350: 6e6e 696e 6720 7468 6520 636f 6d6d 616e  nning the comman
-0000d360: 642e 0a20 2020 2022 2222 0a20 2020 2066  d..    """.    f
-0000d370: 6f72 6520 3d20 636f 6c6f 7261 6d61 2e46  ore = colorama.F
-0000d380: 6f72 650a 2020 2020 7374 796c 6520 3d20  ore.    style = 
-0000d390: 636f 6c6f 7261 6d61 2e53 7479 6c65 0a0a  colorama.Style..
-0000d3a0: 2020 2020 6f72 6967 696e 5f73 6f75 7263      origin_sourc
-0000d3b0: 6520 3d20 736f 7572 6365 0a0a 2020 2020  e = source..    
-0000d3c0: 6465 6620 5f73 796e 635f 6e6f 6465 2872  def _sync_node(r
-0000d3d0: 756e 6e65 723a 2027 636f 6d6d 616e 645f  unner: 'command_
-0000d3e0: 7275 6e6e 6572 2e43 6f6d 6d61 6e64 5275  runner.CommandRu
-0000d3f0: 6e6e 6572 2729 202d 3e20 4e6f 6e65 3a0a  nner') -> None:.
-0000d400: 2020 2020 2020 2020 6966 2063 6d64 2069          if cmd i
-0000d410: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000d420: 2020 2020 2020 2020 7263 2c20 7374 646f          rc, stdo
-0000d430: 7574 2c20 7374 6465 7272 203d 2072 756e  ut, stderr = run
-0000d440: 6e65 722e 7275 6e28 636d 642c 0a20 2020  ner.run(cmd,.   
-0000d450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d470: 2020 2020 2020 2020 206c 6f67 5f70 6174           log_pat
-0000d480: 683d 6c6f 675f 7061 7468 2c0a 2020 2020  h=log_path,.    
-0000d490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4b0: 2020 2020 2020 2020 7374 7265 616d 5f6c          stream_l
-0000d4c0: 6f67 733d 7374 7265 616d 5f6c 6f67 732c  ogs=stream_logs,
-0000d4d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4f0: 2020 2020 2020 2020 2020 2020 2072 6571               req
-0000d500: 7569 7265 5f6f 7574 7075 7473 3d54 7275  uire_outputs=Tru
-0000d510: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0000d520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d530: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000d540: 6f75 7263 655f 6261 7368 7263 3d73 6f75  ource_bashrc=sou
-0000d550: 7263 655f 6261 7368 7263 290a 2020 2020  rce_bashrc).    
-0000d560: 2020 2020 2020 2020 6572 725f 6d73 6720          err_msg 
-0000d570: 3d20 2827 4661 696c 6564 2074 6f20 7275  = ('Failed to ru
-0000d580: 6e20 636f 6d6d 616e 6420 6265 666f 7265  n command before
-0000d590: 2072 7379 6e63 2027 0a20 2020 2020 2020   rsync '.       
-0000d5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5b0: 6627 7b6f 7269 6769 6e5f 736f 7572 6365  f'{origin_source
-0000d5c0: 7d20 2d3e 207b 7461 7267 6574 7d2e 2027  } -> {target}. '
-0000d5d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d5e0: 2020 2020 2020 2020 2745 6e73 7572 6520          'Ensure 
-0000d5f0: 7468 6174 2074 6865 206e 6574 776f 726b  that the network
-0000d600: 2069 7320 7374 6162 6c65 2c20 7468 656e   is stable, then
-0000d610: 2072 6574 7279 2e20 270a 2020 2020 2020   retry. '.      
-0000d620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d630: 2066 277b 636d 647d 2729 0a20 2020 2020   f'{cmd}').     
-0000d640: 2020 2020 2020 2069 6620 6c6f 675f 7061         if log_pa
-0000d650: 7468 2021 3d20 6f73 2e64 6576 6e75 6c6c  th != os.devnull
-0000d660: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000d670: 2020 6572 725f 6d73 6720 2b3d 2066 2720    err_msg += f' 
-0000d680: 5365 6520 6c6f 6773 2069 6e20 7b6c 6f67  See logs in {log
-0000d690: 5f70 6174 687d 270a 2020 2020 2020 2020  _path}'.        
-0000d6a0: 2020 2020 7375 6270 726f 6365 7373 5f75      subprocess_u
-0000d6b0: 7469 6c73 2e68 616e 646c 655f 7265 7475  tils.handle_retu
-0000d6c0: 726e 636f 6465 2872 632c 0a20 2020 2020  rncode(rc,.     
-0000d6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6f0: 2020 2020 2020 2020 2020 636d 642c 0a20            cmd,. 
+0000bd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bda0: 2020 2020 2020 2020 2020 2a2a 7373 685f            **ssh_
+0000bdb0: 6372 6564 656e 7469 616c 7329 0a20 2020  credentials).   
+0000bdc0: 2077 6974 6820 7269 6368 5f75 7469 6c73   with rich_utils
+0000bdd0: 2e73 6166 655f 7374 6174 7573 280a 2020  .safe_status(.  
+0000bde0: 2020 2020 2020 2020 2020 275b 626f 6c64            '[bold
+0000bdf0: 2063 7961 6e5d 5761 6974 696e 6720 666f   cyan]Waiting fo
+0000be00: 7220 776f 726b 6572 732e 2e2e 2729 2061  r workers...') a
+0000be10: 7320 776f 726b 6572 5f73 7461 7475 733a  s worker_status:
+0000be20: 0a20 2020 2020 2020 2077 6869 6c65 2054  .        while T
+0000be30: 7275 653a 0a20 2020 2020 2020 2020 2020  rue:.           
+0000be40: 2072 632c 206f 7574 7075 742c 2073 7464   rc, output, std
+0000be50: 6572 7220 3d20 7275 6e6e 6572 2e72 756e  err = runner.run
+0000be60: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000be70: 2020 696e 7374 616e 6365 5f73 6574 7570    instance_setup
+0000be80: 2e52 4159 5f53 5441 5455 535f 5749 5448  .RAY_STATUS_WITH
+0000be90: 5f53 4b59 5f52 4159 5f50 4f52 545f 434f  _SKY_RAY_PORT_CO
+0000bea0: 4d4d 414e 442c 0a20 2020 2020 2020 2020  MMAND,.         
+0000beb0: 2020 2020 2020 206c 6f67 5f70 6174 683d         log_path=
+0000bec0: 6c6f 675f 7061 7468 2c0a 2020 2020 2020  log_path,.      
+0000bed0: 2020 2020 2020 2020 2020 7374 7265 616d            stream
+0000bee0: 5f6c 6f67 733d 4661 6c73 652c 0a20 2020  _logs=False,.   
+0000bef0: 2020 2020 2020 2020 2020 2020 2072 6571               req
+0000bf00: 7569 7265 5f6f 7574 7075 7473 3d54 7275  uire_outputs=Tru
+0000bf10: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0000bf20: 2020 2073 6570 6172 6174 655f 7374 6465     separate_stde
+0000bf30: 7272 3d54 7275 6529 0a20 2020 2020 2020  rr=True).       
+0000bf40: 2020 2020 2073 7562 7072 6f63 6573 735f       subprocess_
+0000bf50: 7574 696c 732e 6861 6e64 6c65 5f72 6574  utils.handle_ret
+0000bf60: 7572 6e63 6f64 6528 0a20 2020 2020 2020  urncode(.       
+0000bf70: 2020 2020 2020 2020 2072 632c 2069 6e73           rc, ins
+0000bf80: 7461 6e63 655f 7365 7475 702e 5241 595f  tance_setup.RAY_
+0000bf90: 5354 4154 5553 5f57 4954 485f 534b 595f  STATUS_WITH_SKY_
+0000bfa0: 5241 595f 504f 5254 5f43 4f4d 4d41 4e44  RAY_PORT_COMMAND
+0000bfb0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000bfc0: 2020 2746 6169 6c65 6420 746f 2072 756e    'Failed to run
+0000bfd0: 2072 6179 2073 7461 7475 7320 6f6e 2068   ray status on h
+0000bfe0: 6561 6420 6e6f 6465 2e27 2c20 7374 6465  ead node.', stde
+0000bff0: 7272 290a 2020 2020 2020 2020 2020 2020  rr).            
+0000c000: 6c6f 6767 6572 2e64 6562 7567 286f 7574  logger.debug(out
+0000c010: 7075 7429 0a0a 2020 2020 2020 2020 2020  put)..          
+0000c020: 2020 7265 6164 795f 6865 6164 2c20 7265    ready_head, re
+0000c030: 6164 795f 776f 726b 6572 7320 3d20 5f63  ady_workers = _c
+0000c040: 6f75 6e74 5f68 6561 6c74 6879 5f6e 6f64  ount_healthy_nod
+0000c050: 6573 5f66 726f 6d5f 7261 7928 0a20 2020  es_from_ray(.   
+0000c060: 2020 2020 2020 2020 2020 2020 206f 7574               out
+0000c070: 7075 742c 2069 735f 6c6f 6361 6c5f 636c  put, is_local_cl
+0000c080: 6f75 643d 6973 5f6c 6f63 616c 5f63 6c6f  oud=is_local_clo
+0000c090: 7564 290a 0a20 2020 2020 2020 2020 2020  ud)..           
+0000c0a0: 2077 6f72 6b65 725f 7374 6174 7573 2e75   worker_status.u
+0000c0b0: 7064 6174 6528 275b 626f 6c64 2063 7961  pdate('[bold cya
+0000c0c0: 6e5d 270a 2020 2020 2020 2020 2020 2020  n]'.            
+0000c0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c0e0: 2020 2020 2066 277b 7265 6164 795f 776f       f'{ready_wo
+0000c0f0: 726b 6572 737d 206f 7574 206f 6620 7b6e  rkers} out of {n
+0000c100: 756d 5f6e 6f64 6573 202d 2031 7d20 270a  um_nodes - 1} '.
+0000c110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c130: 2027 776f 726b 6572 7320 7265 6164 7927   'workers ready'
+0000c140: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
+0000c150: 2049 6e20 7468 6520 6c6f 6361 6c20 6361   In the local ca
+0000c160: 7365 2c20 7265 6164 795f 6865 6164 3d30  se, ready_head=0
+0000c170: 2061 6e64 2072 6561 6479 5f77 6f72 6b65   and ready_worke
+0000c180: 7273 3d6e 756d 5f6e 6f64 6573 2e20 5468  rs=num_nodes. Th
+0000c190: 6973 0a20 2020 2020 2020 2020 2020 2023  is.            #
+0000c1a0: 2069 7320 6265 6361 7573 6520 7468 6572   is because ther
+0000c1b0: 6520 6973 206e 6f20 6d61 7463 6869 6e67  e is no matching
+0000c1c0: 2072 6567 6578 2066 6f72 205f 4c41 554e   regex for _LAUN
+0000c1d0: 4348 4544 5f48 4541 445f 5041 5454 4552  CHED_HEAD_PATTER
+0000c1e0: 4e2e 0a20 2020 2020 2020 2020 2020 2069  N..            i
+0000c1f0: 6620 7265 6164 795f 6865 6164 202b 2072  f ready_head + r
+0000c200: 6561 6479 5f77 6f72 6b65 7273 203d 3d20  eady_workers == 
+0000c210: 6e75 6d5f 6e6f 6465 733a 0a20 2020 2020  num_nodes:.     
+0000c220: 2020 2020 2020 2020 2020 2023 2041 6c6c             # All
+0000c230: 206e 6f64 6573 2061 7265 2075 702e 0a20   nodes are up.. 
+0000c240: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+0000c250: 7265 616b 0a0a 2020 2020 2020 2020 2020  reak..          
+0000c260: 2020 2320 5065 6e64 696e 6720 776f 726b    # Pending work
+0000c270: 6572 7320 7468 6174 2068 6176 6520 6265  ers that have be
+0000c280: 656e 206c 6175 6e63 6865 6420 6279 2072  en launched by r
+0000c290: 6179 2075 702e 0a20 2020 2020 2020 2020  ay up..         
+0000c2a0: 2020 2066 6f75 6e64 5f69 7073 203d 205f     found_ips = _
+0000c2b0: 4c41 554e 4348 494e 475f 4950 5f50 4154  LAUNCHING_IP_PAT
+0000c2c0: 5445 524e 2e66 696e 6461 6c6c 286f 7574  TERN.findall(out
+0000c2d0: 7075 7429 0a20 2020 2020 2020 2020 2020  put).           
+0000c2e0: 2070 656e 6469 6e67 5f77 6f72 6b65 7273   pending_workers
+0000c2f0: 203d 206c 656e 2866 6f75 6e64 5f69 7073   = len(found_ips
+0000c300: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
+0000c310: 2054 4f44 4f28 7a68 7775 293a 2048 616e   TODO(zhwu): Han
+0000c320: 646c 6520 7468 6520 6361 7365 2077 6865  dle the case whe
+0000c330: 7265 2074 6865 2066 6f6c 6c6f 7769 6e67  re the following
+0000c340: 206f 6363 7572 732c 2077 6865 7265 2072   occurs, where r
+0000c350: 6179 0a20 2020 2020 2020 2020 2020 2023  ay.            #
+0000c360: 2063 6c75 7374 6572 2069 7320 6e6f 7420   cluster is not 
+0000c370: 636f 7272 6563 746c 7920 7374 6172 7465  correctly starte
+0000c380: 6420 6f6e 2074 6865 2063 6c75 7374 6572  d on the cluster
+0000c390: 2e0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0000c3a0: 5065 6e64 696e 673a 0a20 2020 2020 2020  Pending:.       
+0000c3b0: 2020 2020 2023 2020 3137 322e 3331 2e39       #  172.31.9
+0000c3c0: 2e31 3231 3a20 7261 792e 776f 726b 6572  .121: ray.worker
+0000c3d0: 2e64 6566 6175 6c74 2c20 756e 696e 6974  .default, uninit
+0000c3e0: 6961 6c69 7a65 640a 2020 2020 2020 2020  ialized.        
+0000c3f0: 2020 2020 6e6f 6465 735f 736f 5f66 6172      nodes_so_far
+0000c400: 203d 2072 6561 6479 5f68 6561 6420 2b20   = ready_head + 
+0000c410: 7265 6164 795f 776f 726b 6572 7320 2b20  ready_workers + 
+0000c420: 7065 6e64 696e 675f 776f 726b 6572 730a  pending_workers.
+0000c430: 0a20 2020 2020 2020 2020 2020 2023 2043  .            # C
+0000c440: 6865 636b 2074 6865 206e 756d 6265 7220  heck the number 
+0000c450: 6f66 206e 6f64 6573 2074 6861 7420 6172  of nodes that ar
+0000c460: 6520 6665 7463 6865 642e 2054 696d 656f  e fetched. Timeo
+0000c470: 7574 2069 6620 6e6f 206e 6577 0a20 2020  ut if no new.   
+0000c480: 2020 2020 2020 2020 2023 206e 6f64 6573           # nodes
+0000c490: 2066 6574 6368 6564 2069 6e20 6120 7768   fetched in a wh
+0000c4a0: 696c 6520 286e 6f64 6573 5f6c 6175 6e63  ile (nodes_launc
+0000c4b0: 6869 6e67 5f70 726f 6772 6573 735f 7469  hing_progress_ti
+0000c4c0: 6d65 6f75 7429 2c0a 2020 2020 2020 2020  meout),.        
+0000c4d0: 2020 2020 2320 7468 6f75 6768 206e 756d      # though num
+0000c4e0: 6265 7220 6f66 206e 6f64 6573 5f73 6f5f  ber of nodes_so_
+0000c4f0: 6661 7220 6973 2073 7469 6c6c 206e 6f74  far is still not
+0000c500: 2061 7320 6578 7065 6374 6564 2e0a 2020   as expected..  
+0000c510: 2020 2020 2020 2020 2020 6966 206e 6f64            if nod
+0000c520: 6573 5f73 6f5f 6661 7220 3e20 6c61 7374  es_so_far > last
+0000c530: 5f6e 6f64 6573 5f73 6f5f 6661 723a 0a20  _nodes_so_far:. 
+0000c540: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000c550: 2052 6573 6574 2074 6865 2073 7461 7274   Reset the start
+0000c560: 2074 696d 6520 6966 2074 6865 206e 756d   time if the num
+0000c570: 6265 7220 6f66 206c 6175 6e63 6869 6e67  ber of launching
+0000c580: 206e 6f64 6573 0a20 2020 2020 2020 2020   nodes.         
+0000c590: 2020 2020 2020 2023 2063 6861 6e67 6573         # changes
+0000c5a0: 2c20 692e 652e 206e 6577 206e 6f64 6573  , i.e. new nodes
+0000c5b0: 2061 7265 206c 6175 6e63 6865 642e 0a20   are launched.. 
+0000c5c0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0000c5d0: 6f67 6765 722e 6465 6275 6728 2752 6573  ogger.debug('Res
+0000c5e0: 6574 2073 7461 7274 2074 696d 652c 2061  et start time, a
+0000c5f0: 7320 6e65 7720 6e6f 6465 7320 6172 6520  s new nodes are 
+0000c600: 6c61 756e 6368 6564 2e20 270a 2020 2020  launched. '.    
+0000c610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c620: 2020 2020 2020 2020 2066 2728 7b6c 6173           f'({las
+0000c630: 745f 6e6f 6465 735f 736f 5f66 6172 7d20  t_nodes_so_far} 
+0000c640: 2d3e 207b 6e6f 6465 735f 736f 5f66 6172  -> {nodes_so_far
+0000c650: 7d29 2729 0a20 2020 2020 2020 2020 2020  })').           
+0000c660: 2020 2020 2073 7461 7274 203d 2074 696d       start = tim
+0000c670: 652e 7469 6d65 2829 0a20 2020 2020 2020  e.time().       
+0000c680: 2020 2020 2020 2020 206c 6173 745f 6e6f           last_no
+0000c690: 6465 735f 736f 5f66 6172 203d 206e 6f64  des_so_far = nod
+0000c6a0: 6573 5f73 6f5f 6661 720a 2020 2020 2020  es_so_far.      
+0000c6b0: 2020 2020 2020 656c 6966 2028 6e6f 6465        elif (node
+0000c6c0: 735f 6c61 756e 6368 696e 675f 7072 6f67  s_launching_prog
+0000c6d0: 7265 7373 5f74 696d 656f 7574 2069 7320  ress_timeout is 
+0000c6e0: 6e6f 7420 4e6f 6e65 2061 6e64 0a20 2020  not None and.   
+0000c6f0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000c700: 696d 652e 7469 6d65 2829 202d 2073 7461  ime.time() - sta
+0000c710: 7274 203e 206e 6f64 6573 5f6c 6175 6e63  rt > nodes_launc
+0000c720: 6869 6e67 5f70 726f 6772 6573 735f 7469  hing_progress_ti
+0000c730: 6d65 6f75 7420 616e 640a 2020 2020 2020  meout and.      
+0000c740: 2020 2020 2020 2020 2020 2020 6e6f 6465              node
+0000c750: 735f 736f 5f66 6172 2021 3d20 6e75 6d5f  s_so_far != num_
+0000c760: 6e6f 6465 7329 3a0a 2020 2020 2020 2020  nodes):.        
+0000c770: 2020 2020 2020 2020 6c6f 6767 6572 2e65          logger.e
+0000c780: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+0000c790: 2020 2020 2020 2020 2020 2754 696d 6564            'Timed
+0000c7a0: 206f 7574 3a20 7761 6974 6564 2066 6f72   out: waited for
+0000c7b0: 206d 6f72 6520 7468 616e 2027 0a20 2020   more than '.   
+0000c7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c7d0: 2066 277b 6e6f 6465 735f 6c61 756e 6368   f'{nodes_launch
+0000c7e0: 696e 675f 7072 6f67 7265 7373 5f74 696d  ing_progress_tim
+0000c7f0: 656f 7574 7d20 7365 636f 6e64 7320 666f  eout} seconds fo
+0000c800: 7220 6e65 7720 270a 2020 2020 2020 2020  r new '.        
+0000c810: 2020 2020 2020 2020 2020 2020 2777 6f72              'wor
+0000c820: 6b65 7273 2074 6f20 6265 2070 726f 7669  kers to be provi
+0000c830: 7369 6f6e 6564 2c20 6275 7420 6e6f 2070  sioned, but no p
+0000c840: 726f 6772 6573 732e 2729 0a20 2020 2020  rogress.').     
+0000c850: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000c860: 6e20 4661 6c73 652c 204e 6f6e 6520 2023  n False, None  #
+0000c870: 2066 6169 6c65 640a 0a20 2020 2020 2020   failed..       
+0000c880: 2020 2020 2069 6620 2728 6e6f 2070 656e       if '(no pen
+0000c890: 6469 6e67 206e 6f64 6573 2927 2069 6e20  ding nodes)' in 
+0000c8a0: 6f75 7470 7574 2061 6e64 2027 286e 6f20  output and '(no 
+0000c8b0: 6661 696c 7572 6573 2927 2069 6e20 6f75  failures)' in ou
+0000c8c0: 7470 7574 3a0a 2020 2020 2020 2020 2020  tput:.          
+0000c8d0: 2020 2020 2020 2320 4275 6720 696e 2072        # Bug in r
+0000c8e0: 6179 2061 7574 6f73 6361 6c65 723a 2065  ay autoscaler: e
+0000c8f0: 2e67 2e2c 206f 6e20 4743 502c 2069 6620  .g., on GCP, if 
+0000c900: 7265 7175 6573 7469 6e67 2032 206e 6f64  requesting 2 nod
+0000c910: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
+0000c920: 2020 2023 2074 6861 7420 4743 5020 6361     # that GCP ca
+0000c930: 6e20 7361 7469 7366 7920 6f6e 6c79 2062  n satisfy only b
+0000c940: 7920 6861 6c66 2c20 7468 6520 776f 726b  y half, the work
+0000c950: 6572 206e 6f64 6520 776f 756c 6420 6265  er node would be
+0000c960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c970: 2023 2066 6f72 676f 7474 656e 2e20 5468   # forgotten. Th
+0000c980: 6520 636f 7272 6563 7420 6265 6861 7669  e correct behavi
+0000c990: 6f72 2073 686f 756c 6420 6265 2066 6f72  or should be for
+0000c9a0: 2069 7420 746f 2065 7272 6f72 206f 7574   it to error out
+0000c9b0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000c9c0: 2020 6c6f 6767 6572 2e65 7272 6f72 280a    logger.error(.
+0000c9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c9e0: 2020 2020 2746 6169 6c65 6420 746f 206c      'Failed to l
+0000c9f0: 6175 6e63 6820 6d75 6c74 6970 6c65 206e  aunch multiple n
+0000ca00: 6f64 6573 206f 6e20 270a 2020 2020 2020  odes on '.      
+0000ca10: 2020 2020 2020 2020 2020 2020 2020 2747                'G
+0000ca20: 4350 2064 7565 2074 6f20 6120 6e6f 6e64  CP due to a nond
+0000ca30: 6574 6572 6d69 6e69 7374 6963 2062 7567  eterministic bug
+0000ca40: 2069 6e20 7261 7920 6175 746f 7363 616c   in ray autoscal
+0000ca50: 6572 2e27 290a 2020 2020 2020 2020 2020  er.').          
+0000ca60: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+0000ca70: 7365 2c20 4e6f 6e65 2020 2320 6661 696c  se, None  # fail
+0000ca80: 6564 0a20 2020 2020 2020 2020 2020 2074  ed.            t
+0000ca90: 696d 652e 736c 6565 7028 3130 290a 2020  ime.sleep(10).  
+0000caa0: 2020 7265 7475 726e 2054 7275 652c 2064    return True, d
+0000cab0: 6f63 6b65 725f 7573 6572 2020 2320 7375  ocker_user  # su
+0000cac0: 6363 6573 730a 0a0a 6465 6620 7373 685f  ccess...def ssh_
+0000cad0: 6372 6564 656e 7469 616c 5f66 726f 6d5f  credential_from_
+0000cae0: 7961 6d6c 280a 2020 2020 636c 7573 7465  yaml(.    cluste
+0000caf0: 725f 7961 6d6c 3a20 7374 722c 0a20 2020  r_yaml: str,.   
+0000cb00: 2064 6f63 6b65 725f 7573 6572 3a20 4f70   docker_user: Op
+0000cb10: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+0000cb20: 6e65 2c0a 2020 2020 7373 685f 7573 6572  ne,.    ssh_user
+0000cb30: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+0000cb40: 3d20 4e6f 6e65 2c0a 2920 2d3e 2044 6963  = None,.) -> Dic
+0000cb50: 745b 7374 722c 2041 6e79 5d3a 0a20 2020  t[str, Any]:.   
+0000cb60: 2022 2222 5265 7475 726e 7320 7373 685f   """Returns ssh_
+0000cb70: 7573 6572 2c20 7373 685f 7072 6976 6174  user, ssh_privat
+0000cb80: 655f 6b65 7920 616e 6420 7373 685f 636f  e_key and ssh_co
+0000cb90: 6e74 726f 6c20 6e61 6d65 2e0a 0a20 2020  ntrol name...   
+0000cba0: 2041 7267 733a 0a20 2020 2020 2020 2063   Args:.        c
+0000cbb0: 6c75 7374 6572 5f79 616d 6c3a 2070 6174  luster_yaml: pat
+0000cbc0: 6820 746f 2074 6865 2063 6c75 7374 6572  h to the cluster
+0000cbd0: 2079 616d 6c2e 0a20 2020 2020 2020 2064   yaml..        d
+0000cbe0: 6f63 6b65 725f 7573 6572 3a20 7768 656e  ocker_user: when
+0000cbf0: 2075 7369 6e67 2063 7573 746f 6d20 646f   using custom do
+0000cc00: 636b 6572 2069 6d61 6765 2c20 7573 6520  cker image, use 
+0000cc10: 7468 6973 2075 7365 7220 746f 2073 7368  this user to ssh
+0000cc20: 2069 6e74 6f0a 2020 2020 2020 2020 2020   into.          
+0000cc30: 2020 7468 6520 646f 636b 6572 2063 6f6e    the docker con
+0000cc40: 7461 696e 6572 2e0a 2020 2020 2020 2020  tainer..        
+0000cc50: 7373 685f 7573 6572 3a20 6f76 6572 7269  ssh_user: overri
+0000cc60: 6465 2074 6865 2073 7368 5f75 7365 7220  de the ssh_user 
+0000cc70: 696e 2074 6865 2063 6c75 7374 6572 2079  in the cluster y
+0000cc80: 616d 6c2e 0a20 2020 2022 2222 0a20 2020  aml..    """.   
+0000cc90: 2063 6f6e 6669 6720 3d20 636f 6d6d 6f6e   config = common
+0000cca0: 5f75 7469 6c73 2e72 6561 645f 7961 6d6c  _utils.read_yaml
+0000ccb0: 2863 6c75 7374 6572 5f79 616d 6c29 0a20  (cluster_yaml). 
+0000ccc0: 2020 2061 7574 685f 7365 6374 696f 6e20     auth_section 
+0000ccd0: 3d20 636f 6e66 6967 5b27 6175 7468 275d  = config['auth']
+0000cce0: 0a20 2020 2069 6620 7373 685f 7573 6572  .    if ssh_user
+0000ccf0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+0000cd00: 2020 7373 685f 7573 6572 203d 2061 7574    ssh_user = aut
+0000cd10: 685f 7365 6374 696f 6e5b 2773 7368 5f75  h_section['ssh_u
+0000cd20: 7365 7227 5d2e 7374 7269 7028 290a 2020  ser'].strip().  
+0000cd30: 2020 7373 685f 7072 6976 6174 655f 6b65    ssh_private_ke
+0000cd40: 7920 3d20 6175 7468 5f73 6563 7469 6f6e  y = auth_section
+0000cd50: 2e67 6574 2827 7373 685f 7072 6976 6174  .get('ssh_privat
+0000cd60: 655f 6b65 7927 290a 2020 2020 7373 685f  e_key').    ssh_
+0000cd70: 636f 6e74 726f 6c5f 6e61 6d65 203d 2063  control_name = c
+0000cd80: 6f6e 6669 672e 6765 7428 2763 6c75 7374  onfig.get('clust
+0000cd90: 6572 5f6e 616d 6527 2c20 275f 5f64 6566  er_name', '__def
+0000cda0: 6175 6c74 5f5f 2729 0a20 2020 2073 7368  ault__').    ssh
+0000cdb0: 5f70 726f 7879 5f63 6f6d 6d61 6e64 203d  _proxy_command =
+0000cdc0: 2061 7574 685f 7365 6374 696f 6e2e 6765   auth_section.ge
+0000cdd0: 7428 2773 7368 5f70 726f 7879 5f63 6f6d  t('ssh_proxy_com
+0000cde0: 6d61 6e64 2729 0a20 2020 2063 7265 6465  mand').    crede
+0000cdf0: 6e74 6961 6c73 203d 207b 0a20 2020 2020  ntials = {.     
+0000ce00: 2020 2027 7373 685f 7573 6572 273a 2073     'ssh_user': s
+0000ce10: 7368 5f75 7365 722c 0a20 2020 2020 2020  sh_user,.       
+0000ce20: 2027 7373 685f 7072 6976 6174 655f 6b65   'ssh_private_ke
+0000ce30: 7927 3a20 7373 685f 7072 6976 6174 655f  y': ssh_private_
+0000ce40: 6b65 792c 0a20 2020 2020 2020 2027 7373  key,.        'ss
+0000ce50: 685f 636f 6e74 726f 6c5f 6e61 6d65 273a  h_control_name':
+0000ce60: 2073 7368 5f63 6f6e 7472 6f6c 5f6e 616d   ssh_control_nam
+0000ce70: 652c 0a20 2020 2020 2020 2027 7373 685f  e,.        'ssh_
+0000ce80: 7072 6f78 795f 636f 6d6d 616e 6427 3a20  proxy_command': 
+0000ce90: 7373 685f 7072 6f78 795f 636f 6d6d 616e  ssh_proxy_comman
+0000cea0: 642c 0a20 2020 207d 0a20 2020 2069 6620  d,.    }.    if 
+0000ceb0: 646f 636b 6572 5f75 7365 7220 6973 206e  docker_user is n
+0000cec0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0000ced0: 2063 7265 6465 6e74 6961 6c73 5b27 646f   credentials['do
+0000cee0: 636b 6572 5f75 7365 7227 5d20 3d20 646f  cker_user'] = do
+0000cef0: 636b 6572 5f75 7365 720a 2020 2020 7373  cker_user.    ss
+0000cf00: 685f 7072 6f76 6964 6572 5f6d 6f64 756c  h_provider_modul
+0000cf10: 6520 3d20 636f 6e66 6967 5b27 7072 6f76  e = config['prov
+0000cf20: 6964 6572 275d 5b27 6d6f 6475 6c65 275d  ider']['module']
+0000cf30: 0a20 2020 2023 2049 6620 7765 2061 7265  .    # If we are
+0000cf40: 2072 756e 6e69 6e67 2073 7368 2063 6f6d   running ssh com
+0000cf50: 6d61 6e64 206f 6e20 6b75 6265 726e 6574  mand on kubernet
+0000cf60: 6573 206e 6f64 652e 0a20 2020 2069 6620  es node..    if 
+0000cf70: 276b 7562 6572 6e65 7465 7327 2069 6e20  'kubernetes' in 
+0000cf80: 7373 685f 7072 6f76 6964 6572 5f6d 6f64  ssh_provider_mod
+0000cf90: 756c 653a 0a20 2020 2020 2020 2063 7265  ule:.        cre
+0000cfa0: 6465 6e74 6961 6c73 5b27 6469 7361 626c  dentials['disabl
+0000cfb0: 655f 636f 6e74 726f 6c5f 6d61 7374 6572  e_control_master
+0000cfc0: 275d 203d 2054 7275 650a 2020 2020 7265  '] = True.    re
+0000cfd0: 7475 726e 2063 7265 6465 6e74 6961 6c73  turn credentials
+0000cfe0: 0a0a 0a64 6566 2070 6172 616c 6c65 6c5f  ...def parallel_
+0000cff0: 6461 7461 5f74 7261 6e73 6665 725f 746f  data_transfer_to
+0000d000: 5f6e 6f64 6573 280a 2020 2020 7275 6e6e  _nodes(.    runn
+0000d010: 6572 733a 204c 6973 745b 636f 6d6d 616e  ers: List[comman
+0000d020: 645f 7275 6e6e 6572 2e43 6f6d 6d61 6e64  d_runner.Command
+0000d030: 5275 6e6e 6572 5d2c 0a20 2020 2073 6f75  Runner],.    sou
+0000d040: 7263 653a 204f 7074 696f 6e61 6c5b 7374  rce: Optional[st
+0000d050: 725d 2c0a 2020 2020 7461 7267 6574 3a20  r],.    target: 
+0000d060: 7374 722c 0a20 2020 2063 6d64 3a20 4f70  str,.    cmd: Op
+0000d070: 7469 6f6e 616c 5b73 7472 5d2c 0a20 2020  tional[str],.   
+0000d080: 2072 756e 5f72 7379 6e63 3a20 626f 6f6c   run_rsync: bool
+0000d090: 2c0a 2020 2020 2a2c 0a20 2020 2061 6374  ,.    *,.    act
+0000d0a0: 696f 6e5f 6d65 7373 6167 653a 2073 7472  ion_message: str
+0000d0b0: 2c0a 2020 2020 2320 4164 7661 6e63 6564  ,.    # Advanced
+0000d0c0: 206f 7074 696f 6e73 2e0a 2020 2020 6c6f   options..    lo
+0000d0d0: 675f 7061 7468 3a20 7374 7220 3d20 6f73  g_path: str = os
+0000d0e0: 2e64 6576 6e75 6c6c 2c0a 2020 2020 7374  .devnull,.    st
+0000d0f0: 7265 616d 5f6c 6f67 733a 2062 6f6f 6c20  ream_logs: bool 
+0000d100: 3d20 4661 6c73 652c 0a20 2020 2073 6f75  = False,.    sou
+0000d110: 7263 655f 6261 7368 7263 3a20 626f 6f6c  rce_bashrc: bool
+0000d120: 203d 2046 616c 7365 2c0a 293a 0a20 2020   = False,.):.   
+0000d130: 2022 2222 5275 6e73 2061 2063 6f6d 6d61   """Runs a comma
+0000d140: 6e64 206f 6e20 616c 6c20 6e6f 6465 7320  nd on all nodes 
+0000d150: 616e 6420 6f70 7469 6f6e 616c 6c79 2072  and optionally r
+0000d160: 756e 7320 7273 796e 6320 6672 6f6d 2073  uns rsync from s
+0000d170: 7263 2d3e 6473 742e 0a0a 2020 2020 4172  rc->dst...    Ar
+0000d180: 6773 3a0a 2020 2020 2020 2020 7275 6e6e  gs:.        runn
+0000d190: 6572 733a 2041 206c 6973 7420 6f66 2043  ers: A list of C
+0000d1a0: 6f6d 6d61 6e64 5275 6e6e 6572 206f 626a  ommandRunner obj
+0000d1b0: 6563 7473 2074 6861 7420 7265 7072 6573  ects that repres
+0000d1c0: 656e 7420 6d75 6c74 6970 6c65 206e 6f64  ent multiple nod
+0000d1d0: 6573 2e0a 2020 2020 2020 2020 736f 7572  es..        sour
+0000d1e0: 6365 3a20 4f70 7469 6f6e 616c 5b73 7472  ce: Optional[str
+0000d1f0: 5d3b 2053 6f75 7263 6520 666f 7220 7273  ]; Source for rs
+0000d200: 796e 6320 6f6e 206c 6f63 616c 206e 6f64  ync on local nod
+0000d210: 650a 2020 2020 2020 2020 7461 7267 6574  e.        target
+0000d220: 3a20 7374 723b 2044 6573 7469 6e61 7469  : str; Destinati
+0000d230: 6f6e 206f 6e20 7265 6d6f 7465 206e 6f64  on on remote nod
+0000d240: 6520 666f 7220 7273 796e 630a 2020 2020  e for rsync.    
+0000d250: 2020 2020 636d 643a 2073 7472 3b20 436f      cmd: str; Co
+0000d260: 6d6d 616e 6420 746f 2062 6520 6578 6563  mmand to be exec
+0000d270: 7574 6564 206f 6e20 616c 6c20 6e6f 6465  uted on all node
+0000d280: 730a 2020 2020 2020 2020 6163 7469 6f6e  s.        action
+0000d290: 5f6d 6573 7361 6765 3a20 7374 723b 204d  _message: str; M
+0000d2a0: 6573 7361 6765 2074 6f20 6265 2070 7269  essage to be pri
+0000d2b0: 6e74 6564 2077 6869 6c65 2074 6865 2063  nted while the c
+0000d2c0: 6f6d 6d61 6e64 2072 756e 730a 2020 2020  ommand runs.    
+0000d2d0: 2020 2020 6c6f 675f 7061 7468 3a20 7374      log_path: st
+0000d2e0: 723b 2050 6174 6820 746f 2074 6865 206c  r; Path to the l
+0000d2f0: 6f67 2066 696c 650a 2020 2020 2020 2020  og file.        
+0000d300: 7374 7265 616d 5f6c 6f67 733a 2062 6f6f  stream_logs: boo
+0000d310: 6c3b 2057 6865 7468 6572 2074 6f20 7374  l; Whether to st
+0000d320: 7265 616d 206c 6f67 7320 746f 2073 7464  ream logs to std
+0000d330: 6f75 740a 2020 2020 2020 2020 736f 7572  out.        sour
+0000d340: 6365 5f62 6173 6872 633a 2062 6f6f 6c3b  ce_bashrc: bool;
+0000d350: 2053 6f75 7263 6520 6261 7368 7263 2062   Source bashrc b
+0000d360: 6566 6f72 6520 7275 6e6e 696e 6720 7468  efore running th
+0000d370: 6520 636f 6d6d 616e 642e 0a20 2020 2022  e command..    "
+0000d380: 2222 0a20 2020 2066 6f72 6520 3d20 636f  "".    fore = co
+0000d390: 6c6f 7261 6d61 2e46 6f72 650a 2020 2020  lorama.Fore.    
+0000d3a0: 7374 796c 6520 3d20 636f 6c6f 7261 6d61  style = colorama
+0000d3b0: 2e53 7479 6c65 0a0a 2020 2020 6f72 6967  .Style..    orig
+0000d3c0: 696e 5f73 6f75 7263 6520 3d20 736f 7572  in_source = sour
+0000d3d0: 6365 0a0a 2020 2020 6465 6620 5f73 796e  ce..    def _syn
+0000d3e0: 635f 6e6f 6465 2872 756e 6e65 723a 2027  c_node(runner: '
+0000d3f0: 636f 6d6d 616e 645f 7275 6e6e 6572 2e43  command_runner.C
+0000d400: 6f6d 6d61 6e64 5275 6e6e 6572 2729 202d  ommandRunner') -
+0000d410: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+0000d420: 6966 2063 6d64 2069 7320 6e6f 7420 4e6f  if cmd is not No
+0000d430: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000d440: 7263 2c20 7374 646f 7574 2c20 7374 6465  rc, stdout, stde
+0000d450: 7272 203d 2072 756e 6e65 722e 7275 6e28  rr = runner.run(
+0000d460: 636d 642c 0a20 2020 2020 2020 2020 2020  cmd,.           
+0000d470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d490: 206c 6f67 5f70 6174 683d 6c6f 675f 7061   log_path=log_pa
+0000d4a0: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
+0000d4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d4d0: 7374 7265 616d 5f6c 6f67 733d 7374 7265  stream_logs=stre
+0000d4e0: 616d 5f6c 6f67 732c 0a20 2020 2020 2020  am_logs,.       
+0000d4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d510: 2020 2020 2072 6571 7569 7265 5f6f 7574       require_out
+0000d520: 7075 7473 3d54 7275 652c 0a20 2020 2020  puts=True,.     
+0000d530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d550: 2020 2020 2020 2073 6f75 7263 655f 6261         source_ba
+0000d560: 7368 7263 3d73 6f75 7263 655f 6261 7368  shrc=source_bash
+0000d570: 7263 290a 2020 2020 2020 2020 2020 2020  rc).            
+0000d580: 6572 725f 6d73 6720 3d20 2827 4661 696c  err_msg = ('Fail
+0000d590: 6564 2074 6f20 7275 6e20 636f 6d6d 616e  ed to run comman
+0000d5a0: 6420 6265 666f 7265 2072 7379 6e63 2027  d before rsync '
+0000d5b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d5c0: 2020 2020 2020 2020 6627 7b6f 7269 6769          f'{origi
+0000d5d0: 6e5f 736f 7572 6365 7d20 2d3e 207b 7461  n_source} -> {ta
+0000d5e0: 7267 6574 7d2e 2027 0a20 2020 2020 2020  rget}. '.       
+0000d5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d600: 2745 6e73 7572 6520 7468 6174 2074 6865  'Ensure that the
+0000d610: 206e 6574 776f 726b 2069 7320 7374 6162   network is stab
+0000d620: 6c65 2c20 7468 656e 2072 6574 7279 2e20  le, then retry. 
+0000d630: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+0000d640: 2020 2020 2020 2020 2066 277b 636d 647d           f'{cmd}
+0000d650: 2729 0a20 2020 2020 2020 2020 2020 2069  ').            i
+0000d660: 6620 6c6f 675f 7061 7468 2021 3d20 6f73  f log_path != os
+0000d670: 2e64 6576 6e75 6c6c 3a0a 2020 2020 2020  .devnull:.      
+0000d680: 2020 2020 2020 2020 2020 6572 725f 6d73            err_ms
+0000d690: 6720 2b3d 2066 2720 5365 6520 6c6f 6773  g += f' See logs
+0000d6a0: 2069 6e20 7b6c 6f67 5f70 6174 687d 270a   in {log_path}'.
+0000d6b0: 2020 2020 2020 2020 2020 2020 7375 6270              subp
+0000d6c0: 726f 6365 7373 5f75 7469 6c73 2e68 616e  rocess_utils.han
+0000d6d0: 646c 655f 7265 7475 726e 636f 6465 2872  dle_returncode(r
+0000d6e0: 632c 0a20 2020 2020 2020 2020 2020 2020  c,.             
+0000d6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000d700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d720: 2020 2020 2020 2020 2020 2020 2020 6572                er
-0000d730: 725f 6d73 672c 0a20 2020 2020 2020 2020  r_msg,.         
-0000d740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d710: 2020 636d 642c 0a20 2020 2020 2020 2020    cmd,.         
+0000d720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d740: 2020 2020 2020 6572 725f 6d73 672c 0a20        err_msg,. 
 0000d750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d760: 2020 2020 2020 7374 6465 7272 3d73 7464        stderr=std
-0000d770: 6f75 7420 2b20 7374 6465 7272 290a 0a20  out + stderr).. 
-0000d780: 2020 2020 2020 2069 6620 7275 6e5f 7273         if run_rs
-0000d790: 796e 633a 0a20 2020 2020 2020 2020 2020  ync:.           
-0000d7a0: 2061 7373 6572 7420 736f 7572 6365 2069   assert source i
-0000d7b0: 7320 6e6f 7420 4e6f 6e65 0a20 2020 2020  s not None.     
-0000d7c0: 2020 2020 2020 2023 2054 4f44 4f28 7a68         # TODO(zh
-0000d7d0: 7775 293a 204f 7074 696d 697a 6520 666f  wu): Optimize fo
-0000d7e0: 7220 6c61 7267 6520 616d 6f75 6e74 206f  r large amount o
-0000d7f0: 6620 6669 6c65 732e 0a20 2020 2020 2020  f files..       
-0000d800: 2020 2020 2023 207a 6970 202f 2074 7261       # zip / tra
-0000d810: 6e73 6665 7220 2f20 756e 7a69 700a 2020  nsfer / unzip.  
-0000d820: 2020 2020 2020 2020 2020 7275 6e6e 6572            runner
-0000d830: 2e72 7379 6e63 280a 2020 2020 2020 2020  .rsync(.        
-0000d840: 2020 2020 2020 2020 736f 7572 6365 3d73          source=s
-0000d850: 6f75 7263 652c 0a20 2020 2020 2020 2020  ource,.         
-0000d860: 2020 2020 2020 2074 6172 6765 743d 7461         target=ta
-0000d870: 7267 6574 2c0a 2020 2020 2020 2020 2020  rget,.          
-0000d880: 2020 2020 2020 7570 3d54 7275 652c 0a20        up=True,. 
-0000d890: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0000d8a0: 6f67 5f70 6174 683d 6c6f 675f 7061 7468  og_path=log_path
-0000d8b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000d8c0: 2020 7374 7265 616d 5f6c 6f67 733d 7374    stream_logs=st
-0000d8d0: 7265 616d 5f6c 6f67 732c 0a20 2020 2020  ream_logs,.     
-0000d8e0: 2020 2020 2020 2029 0a0a 2020 2020 6e75         )..    nu
-0000d8f0: 6d5f 6e6f 6465 7320 3d20 6c65 6e28 7275  m_nodes = len(ru
-0000d900: 6e6e 6572 7329 0a20 2020 2070 6c75 7261  nners).    plura
-0000d910: 6c20 3d20 2773 2720 6966 206e 756d 5f6e  l = 's' if num_n
-0000d920: 6f64 6573 203e 2031 2065 6c73 6520 2727  odes > 1 else ''
-0000d930: 0a20 2020 206d 6573 7361 6765 203d 2028  .    message = (
-0000d940: 6627 7b66 6f72 652e 4359 414e 7d7b 6163  f'{fore.CYAN}{ac
-0000d950: 7469 6f6e 5f6d 6573 7361 6765 7d20 2874  tion_message} (t
-0000d960: 6f20 7b6e 756d 5f6e 6f64 6573 7d20 6e6f  o {num_nodes} no
-0000d970: 6465 7b70 6c75 7261 6c7d 2927 0a20 2020  de{plural})'.   
-0000d980: 2020 2020 2020 2020 2020 2020 6627 3a20              f': 
-0000d990: 7b73 7479 6c65 2e42 5249 4748 547d 7b6f  {style.BRIGHT}{o
-0000d9a0: 7269 6769 6e5f 736f 7572 6365 7d7b 7374  rigin_source}{st
-0000d9b0: 796c 652e 5245 5345 545f 414c 4c7d 202d  yle.RESET_ALL} -
-0000d9c0: 3e20 270a 2020 2020 2020 2020 2020 2020  > '.            
-0000d9d0: 2020 2066 277b 7374 796c 652e 4252 4947     f'{style.BRIG
-0000d9e0: 4854 7d7b 7461 7267 6574 7d7b 7374 796c  HT}{target}{styl
-0000d9f0: 652e 5245 5345 545f 414c 4c7d 2729 0a20  e.RESET_ALL}'). 
-0000da00: 2020 206c 6f67 6765 722e 696e 666f 286d     logger.info(m
-0000da10: 6573 7361 6765 290a 2020 2020 7769 7468  essage).    with
-0000da20: 2072 6963 685f 7574 696c 732e 7361 6665   rich_utils.safe
-0000da30: 5f73 7461 7475 7328 6627 5b62 6f6c 6420  _status(f'[bold 
-0000da40: 6379 616e 5d7b 6163 7469 6f6e 5f6d 6573  cyan]{action_mes
-0000da50: 7361 6765 7d5b 2f5d 2729 3a0a 2020 2020  sage}[/]'):.    
-0000da60: 2020 2020 7375 6270 726f 6365 7373 5f75      subprocess_u
-0000da70: 7469 6c73 2e72 756e 5f69 6e5f 7061 7261  tils.run_in_para
-0000da80: 6c6c 656c 285f 7379 6e63 5f6e 6f64 652c  llel(_sync_node,
-0000da90: 2072 756e 6e65 7273 290a 0a0a 6465 6620   runners)...def 
-0000daa0: 6368 6563 6b5f 6c6f 6361 6c5f 6770 7573  check_local_gpus
-0000dab0: 2829 202d 3e20 626f 6f6c 3a0a 2020 2020  () -> bool:.    
-0000dac0: 2222 2243 6865 636b 7320 6966 2047 5055  """Checks if GPU
-0000dad0: 7320 6172 6520 6176 6169 6c61 626c 6520  s are available 
-0000dae0: 6c6f 6361 6c6c 792e 0a0a 2020 2020 5265  locally...    Re
-0000daf0: 7475 726e 7320 7768 6574 6865 7220 4750  turns whether GP
-0000db00: 5573 2061 7265 2061 7661 696c 6162 6c65  Us are available
-0000db10: 206f 6e20 7468 6520 6c6f 6361 6c20 6d61   on the local ma
-0000db20: 6368 696e 6520 6279 2063 6865 636b 696e  chine by checkin
-0000db30: 670a 2020 2020 6966 206e 7669 6469 612d  g.    if nvidia-
-0000db40: 736d 6920 6973 2069 6e73 7461 6c6c 6564  smi is installed
-0000db50: 2061 6e64 2072 6574 7572 6e73 207a 6572   and returns zer
-0000db60: 6f20 7265 7475 726e 2063 6f64 652e 0a0a  o return code...
-0000db70: 2020 2020 5265 7475 726e 7320 5472 7565      Returns True
-0000db80: 2069 6620 6e76 6964 6961 2d73 6d69 2069   if nvidia-smi i
-0000db90: 7320 696e 7374 616c 6c65 6420 616e 6420  s installed and 
-0000dba0: 7265 7475 726e 7320 7a65 726f 2072 6574  returns zero ret
-0000dbb0: 7572 6e20 636f 6465 2c0a 2020 2020 4661  urn code,.    Fa
-0000dbc0: 6c73 6520 6966 206e 6f74 2e0a 2020 2020  lse if not..    
-0000dbd0: 2222 220a 2020 2020 6973 5f66 756e 6374  """.    is_funct
-0000dbe0: 696f 6e61 6c20 3d20 4661 6c73 650a 2020  ional = False.  
-0000dbf0: 2020 696e 7374 616c 6c61 7469 6f6e 5f63    installation_c
-0000dc00: 6865 636b 203d 2073 7562 7072 6f63 6573  heck = subproces
-0000dc10: 732e 7275 6e28 5b27 7768 6963 6827 2c20  s.run(['which', 
-0000dc20: 276e 7669 6469 612d 736d 6927 5d2c 0a20  'nvidia-smi'],. 
-0000dc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc50: 2020 2020 2020 2073 7464 6f75 743d 7375         stdout=su
-0000dc60: 6270 726f 6365 7373 2e44 4556 4e55 4c4c  bprocess.DEVNULL
-0000dc70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000dc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc90: 2020 2020 2020 2020 2020 7374 6465 7272            stderr
-0000dca0: 3d73 7562 7072 6f63 6573 732e 4445 564e  =subprocess.DEVN
-0000dcb0: 554c 4c2c 0a20 2020 2020 2020 2020 2020  ULL,.           
-0000dcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dcd0: 2020 2020 2020 2020 2020 2020 2063 6865               che
-0000dce0: 636b 3d46 616c 7365 290a 2020 2020 6973  ck=False).    is
-0000dcf0: 5f69 6e73 7461 6c6c 6564 203d 2069 6e73  _installed = ins
-0000dd00: 7461 6c6c 6174 696f 6e5f 6368 6563 6b2e  tallation_check.
-0000dd10: 7265 7475 726e 636f 6465 203d 3d20 300a  returncode == 0.
-0000dd20: 2020 2020 6966 2069 735f 696e 7374 616c      if is_instal
-0000dd30: 6c65 643a 0a20 2020 2020 2020 2065 7865  led:.        exe
-0000dd40: 6375 7469 6f6e 5f63 6865 636b 203d 2073  cution_check = s
-0000dd50: 7562 7072 6f63 6573 732e 7275 6e28 5b27  ubprocess.run(['
-0000dd60: 6e76 6964 6961 2d73 6d69 275d 2c0a 2020  nvidia-smi'],.  
-0000dd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd90: 2020 2020 2020 2073 7464 6f75 743d 7375         stdout=su
-0000dda0: 6270 726f 6365 7373 2e44 4556 4e55 4c4c  bprocess.DEVNULL
-0000ddb0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000ddc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ddd0: 2020 2020 2020 2020 2020 2073 7464 6572             stder
-0000dde0: 723d 7375 6270 726f 6365 7373 2e44 4556  r=subprocess.DEV
-0000ddf0: 4e55 4c4c 2c0a 2020 2020 2020 2020 2020  NULL,.          
-0000de00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de10: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000de20: 6865 636b 3d46 616c 7365 290a 2020 2020  heck=False).    
-0000de30: 2020 2020 6973 5f66 756e 6374 696f 6e61      is_functiona
-0000de40: 6c20 3d20 6578 6563 7574 696f 6e5f 6368  l = execution_ch
-0000de50: 6563 6b2e 7265 7475 726e 636f 6465 203d  eck.returncode =
-0000de60: 3d20 300a 2020 2020 7265 7475 726e 2069  = 0.    return i
-0000de70: 735f 6675 6e63 7469 6f6e 616c 0a0a 0a64  s_functional...d
-0000de80: 6566 2067 656e 6572 6174 655f 636c 7573  ef generate_clus
-0000de90: 7465 725f 6e61 6d65 2829 3a0a 2020 2020  ter_name():.    
-0000dea0: 2320 544f 444f 3a20 6368 616e 6765 2074  # TODO: change t
-0000deb0: 6869 7320 4944 2066 6f72 6d61 7474 696e  his ID formattin
-0000dec0: 6720 746f 2073 6f6d 6574 6869 6e67 206d  g to something m
-0000ded0: 6f72 6520 706c 6561 7361 6e74 2e0a 2020  ore pleasant..  
-0000dee0: 2020 2320 5573 6572 206e 616d 6520 6973    # User name is
-0000def0: 2068 656c 7066 756c 2069 6e20 6e6f 6e2d   helpful in non-
-0000df00: 6973 6f6c 6174 6564 2061 6363 6f75 6e74  isolated account
-0000df10: 732c 2065 2e67 2e2c 2047 4350 2c20 417a  s, e.g., GCP, Az
-0000df20: 7572 652e 0a20 2020 2072 6574 7572 6e20  ure..    return 
-0000df30: 6627 736b 792d 7b75 7569 642e 7575 6964  f'sky-{uuid.uuid
-0000df40: 3428 292e 6865 785b 3a34 5d7d 2d7b 636f  4().hex[:4]}-{co
-0000df50: 6d6d 6f6e 5f75 7469 6c73 2e67 6574 5f63  mmon_utils.get_c
-0000df60: 6c65 616e 6564 5f75 7365 726e 616d 6528  leaned_username(
-0000df70: 297d 270a 0a0a 6465 6620 5f71 7565 7279  )}'...def _query
-0000df80: 5f68 6561 645f 6970 5f77 6974 685f 7265  _head_ip_with_re
-0000df90: 7472 6965 7328 636c 7573 7465 725f 7961  tries(cluster_ya
-0000dfa0: 6d6c 3a20 7374 722c 0a20 2020 2020 2020  ml: str,.       
-0000dfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dfc0: 2020 2020 2020 2020 206d 6178 5f61 7474           max_att
-0000dfd0: 656d 7074 733a 2069 6e74 203d 2031 2920  empts: int = 1) 
-0000dfe0: 2d3e 2073 7472 3a0a 2020 2020 2222 2252  -> str:.    """R
-0000dff0: 6574 7572 6e73 2074 6865 2049 5020 6f66  eturns the IP of
-0000e000: 2074 6865 2068 6561 6420 6e6f 6465 2062   the head node b
-0000e010: 7920 7175 6572 7969 6e67 2074 6865 2063  y querying the c
-0000e020: 6c6f 7564 2e0a 0a20 2020 2052 6169 7365  loud...    Raise
-0000e030: 733a 0a20 2020 2020 2065 7863 6570 7469  s:.      excepti
-0000e040: 6f6e 732e 4665 7463 6843 6c75 7374 6572  ons.FetchCluster
-0000e050: 496e 666f 4572 726f 723a 2069 6620 7765  InfoError: if we
-0000e060: 2066 6169 6c65 6420 746f 2067 6574 2074   failed to get t
-0000e070: 6865 2068 6561 6420 4950 2e0a 2020 2020  he head IP..    
-0000e080: 2222 220a 2020 2020 6261 636b 6f66 6620  """.    backoff 
-0000e090: 3d20 636f 6d6d 6f6e 5f75 7469 6c73 2e42  = common_utils.B
-0000e0a0: 6163 6b6f 6666 2869 6e69 7469 616c 5f62  ackoff(initial_b
-0000e0b0: 6163 6b6f 6666 3d35 2c20 6d61 785f 6261  ackoff=5, max_ba
-0000e0c0: 636b 6f66 665f 6661 6374 6f72 3d35 290a  ckoff_factor=5).
-0000e0d0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-0000e0e0: 6765 286d 6178 5f61 7474 656d 7074 7329  ge(max_attempts)
-0000e0f0: 3a0a 2020 2020 2020 2020 7472 793a 0a20  :.        try:. 
-0000e100: 2020 2020 2020 2020 2020 2066 756c 6c5f             full_
-0000e110: 636c 7573 7465 725f 7961 6d6c 203d 2073  cluster_yaml = s
-0000e120: 7472 2870 6174 686c 6962 2e50 6174 6828  tr(pathlib.Path(
-0000e130: 636c 7573 7465 725f 7961 6d6c 292e 6578  cluster_yaml).ex
-0000e140: 7061 6e64 7573 6572 2829 290a 2020 2020  panduser()).    
-0000e150: 2020 2020 2020 2020 6f75 7420 3d20 7375          out = su
-0000e160: 6270 726f 6365 7373 5f75 7469 6c73 2e72  bprocess_utils.r
-0000e170: 756e 280a 2020 2020 2020 2020 2020 2020  un(.            
-0000e180: 2020 2020 6627 7261 7920 6765 742d 6865      f'ray get-he
-0000e190: 6164 2d69 7020 7b66 756c 6c5f 636c 7573  ad-ip {full_clus
-0000e1a0: 7465 725f 7961 6d6c 2172 7d27 2c0a 2020  ter_yaml!r}',.  
-0000e1b0: 2020 2020 2020 2020 2020 2020 2020 7374                st
-0000e1c0: 646f 7574 3d73 7562 7072 6f63 6573 732e  dout=subprocess.
-0000e1d0: 5049 5045 2c0a 2020 2020 2020 2020 2020  PIPE,.          
-0000e1e0: 2020 2020 2020 7374 6465 7272 3d73 7562        stderr=sub
-0000e1f0: 7072 6f63 6573 732e 4445 564e 554c 4c29  process.DEVNULL)
-0000e200: 2e73 7464 6f75 742e 6465 636f 6465 2829  .stdout.decode()
-0000e210: 2e73 7472 6970 2829 0a20 2020 2020 2020  .strip().       
-0000e220: 2020 2020 2068 6561 645f 6970 5f6c 6973       head_ip_lis
-0000e230: 7420 3d20 7265 2e66 696e 6461 6c6c 2849  t = re.findall(I
-0000e240: 505f 4144 4452 5f52 4547 4558 2c20 6f75  P_ADDR_REGEX, ou
-0000e250: 7429 0a20 2020 2020 2020 2020 2020 2069  t).            i
-0000e260: 6620 6c65 6e28 6865 6164 5f69 705f 6c69  f len(head_ip_li
-0000e270: 7374 2920 3e20 313a 0a20 2020 2020 2020  st) > 1:.       
-0000e280: 2020 2020 2020 2020 2023 2054 6869 7320           # This 
-0000e290: 636f 756c 6420 6265 2074 7269 6767 6572  could be trigger
-0000e2a0: 6564 2069 6620 652e 672e 2c20 736f 6d65  ed if e.g., some
-0000e2b0: 206c 6f67 6769 6e67 2069 7320 6164 6465   logging is adde
-0000e2c0: 6420 696e 0a20 2020 2020 2020 2020 2020  d in.           
-0000e2d0: 2020 2020 2023 2073 6b79 7069 6c6f 745f       # skypilot_
-0000e2e0: 636f 6e66 6967 2c20 6120 6d6f 6475 6c65  config, a module
-0000e2f0: 2074 6861 7420 6861 7320 736f 6d65 2063   that has some c
-0000e300: 6f64 6520 6578 6563 7574 6564 0a20 2020  ode executed.   
-0000e310: 2020 2020 2020 2020 2020 2020 2023 2077               # w
-0000e320: 6865 6e65 7665 7220 6073 6b79 6020 6973  henever `sky` is
-0000e330: 2069 6d70 6f72 7465 642e 0a20 2020 2020   imported..     
-0000e340: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-0000e350: 722e 7761 726e 696e 6728 0a20 2020 2020  r.warning(.     
-0000e360: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0000e370: 4465 7465 6374 6564 206d 6f72 6520 7468  Detected more th
-0000e380: 616e 2031 2049 5020 6672 6f6d 2074 6865  an 1 IP from the
-0000e390: 206f 7574 7075 7420 6f66 2027 0a20 2020   output of '.   
-0000e3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e3b0: 2027 7468 6520 6072 6179 2067 6574 2d68   'the `ray get-h
-0000e3c0: 6561 642d 6970 6020 636f 6d6d 616e 642e  ead-ip` command.
-0000e3d0: 2054 6869 7320 636f 756c 6420 270a 2020   This could '.  
-0000e3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e3f0: 2020 2768 6170 7065 6e20 6966 2074 6865    'happen if the
-0000e400: 7265 2069 7320 6578 7472 6120 6f75 7470  re is extra outp
-0000e410: 7574 2066 726f 6d20 6974 2c20 270a 2020  ut from it, '.  
-0000e420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e430: 2020 2777 6869 6368 2073 686f 756c 6420    'which should 
-0000e440: 6265 2069 6e73 7065 6374 6564 2062 656c  be inspected bel
-0000e450: 6f77 2e5c 6e50 726f 6365 6564 696e 6720  ow.\nProceeding 
-0000e460: 7769 7468 2027 0a20 2020 2020 2020 2020  with '.         
-0000e470: 2020 2020 2020 2020 2020 2066 2774 6865             f'the
-0000e480: 206c 6173 7420 6465 7465 6374 6564 2049   last detected I
-0000e490: 5020 287b 6865 6164 5f69 705f 6c69 7374  P ({head_ip_list
-0000e4a0: 5b2d 315d 7d29 2061 7320 6865 6164 2049  [-1]}) as head I
-0000e4b0: 502e 270a 2020 2020 2020 2020 2020 2020  P.'.            
-0000e4c0: 2020 2020 2020 2020 6627 5c6e 3d3d 204f          f'\n== O
-0000e4d0: 7574 7075 7420 3d3d 5c6e 7b6f 7574 7d27  utput ==\n{out}'
-0000e4e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e4f0: 2020 2020 2066 275c 6e3d 3d20 4f75 7470       f'\n== Outp
-0000e500: 7574 2065 6e64 7320 3d3d 2729 0a20 2020  ut ends ==').   
-0000e510: 2020 2020 2020 2020 2020 2020 2068 6561               hea
-0000e520: 645f 6970 5f6c 6973 7420 3d20 6865 6164  d_ip_list = head
-0000e530: 5f69 705f 6c69 7374 5b2d 313a 5d0a 2020  _ip_list[-1:].  
-0000e540: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-0000e550: 2031 203d 3d20 6c65 6e28 6865 6164 5f69   1 == len(head_i
-0000e560: 705f 6c69 7374 292c 2028 6f75 742c 2068  p_list), (out, h
-0000e570: 6561 645f 6970 5f6c 6973 7429 0a20 2020  ead_ip_list).   
-0000e580: 2020 2020 2020 2020 2068 6561 645f 6970           head_ip
-0000e590: 203d 2068 6561 645f 6970 5f6c 6973 745b   = head_ip_list[
-0000e5a0: 305d 0a20 2020 2020 2020 2020 2020 2062  0].            b
-0000e5b0: 7265 616b 0a20 2020 2020 2020 2065 7863  reak.        exc
-0000e5c0: 6570 7420 7375 6270 726f 6365 7373 2e43  ept subprocess.C
-0000e5d0: 616c 6c65 6450 726f 6365 7373 4572 726f  alledProcessErro
-0000e5e0: 7220 6173 2065 3a0a 2020 2020 2020 2020  r as e:.        
-0000e5f0: 2020 2020 6966 2069 203d 3d20 6d61 785f      if i == max_
-0000e600: 6174 7465 6d70 7473 202d 2031 3a0a 2020  attempts - 1:.  
-0000e610: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-0000e620: 6973 6520 6578 6365 7074 696f 6e73 2e46  ise exceptions.F
-0000e630: 6574 6368 436c 7573 7465 7249 6e66 6f45  etchClusterInfoE
-0000e640: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
-0000e650: 2020 2020 2020 2020 2020 7265 6173 6f6e            reason
-0000e660: 3d65 7863 6570 7469 6f6e 732e 4665 7463  =exceptions.Fetc
-0000e670: 6843 6c75 7374 6572 496e 666f 4572 726f  hClusterInfoErro
-0000e680: 722e 5265 6173 6f6e 2e48 4541 4429 2066  r.Reason.HEAD) f
-0000e690: 726f 6d20 650a 2020 2020 2020 2020 2020  rom e.          
-0000e6a0: 2020 2320 5265 7472 7920 6966 2074 6865    # Retry if the
-0000e6b0: 2063 6c75 7374 6572 2069 7320 6e6f 7420   cluster is not 
-0000e6c0: 7570 2079 6574 2e0a 2020 2020 2020 2020  up yet..        
-0000e6d0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-0000e6e0: 2827 5265 7472 7969 6e67 2074 6f20 6765  ('Retrying to ge
-0000e6f0: 7420 6865 6164 2069 702e 2729 0a20 2020  t head ip.').   
-0000e700: 2020 2020 2020 2020 2074 696d 652e 736c           time.sl
-0000e710: 6565 7028 6261 636b 6f66 662e 6375 7272  eep(backoff.curr
-0000e720: 656e 745f 6261 636b 6f66 6628 2929 0a20  ent_backoff()). 
-0000e730: 2020 2072 6574 7572 6e20 6865 6164 5f69     return head_i
-0000e740: 700a 0a0a 4074 696d 656c 696e 652e 6576  p...@timeline.ev
-0000e750: 656e 740a 6465 6620 6765 745f 6e6f 6465  ent.def get_node
-0000e760: 5f69 7073 2863 6c75 7374 6572 5f79 616d  _ips(cluster_yam
-0000e770: 6c3a 2073 7472 2c0a 2020 2020 2020 2020  l: str,.        
-0000e780: 2020 2020 2020 2020 2065 7870 6563 7465           expecte
-0000e790: 645f 6e75 6d5f 6e6f 6465 733a 2069 6e74  d_num_nodes: int
-0000e7a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000e7b0: 2020 2068 6561 645f 6970 5f6d 6178 5f61     head_ip_max_a
-0000e7c0: 7474 656d 7074 733a 2069 6e74 203d 2031  ttempts: int = 1
-0000e7d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000e7e0: 2020 2077 6f72 6b65 725f 6970 5f6d 6178     worker_ip_max
-0000e7f0: 5f61 7474 656d 7074 733a 2069 6e74 203d  _attempts: int =
-0000e800: 2031 2c0a 2020 2020 2020 2020 2020 2020   1,.            
-0000e810: 2020 2020 2067 6574 5f69 6e74 6572 6e61       get_interna
-0000e820: 6c5f 6970 733a 2062 6f6f 6c20 3d20 4661  l_ips: bool = Fa
-0000e830: 6c73 6529 202d 3e20 4c69 7374 5b73 7472  lse) -> List[str
-0000e840: 5d3a 0a20 2020 2022 2222 5265 7475 726e  ]:.    """Return
-0000e850: 7320 7468 6520 4950 7320 6f66 2061 6c6c  s the IPs of all
-0000e860: 206e 6f64 6573 2069 6e20 7468 6520 636c   nodes in the cl
-0000e870: 7573 7465 722c 2077 6974 6820 6865 6164  uster, with head
-0000e880: 206e 6f64 6520 6174 2066 726f 6e74 2e0a   node at front..
-0000e890: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-0000e8a0: 2020 2063 6c75 7374 6572 5f79 616d 6c3a     cluster_yaml:
-0000e8b0: 2050 6174 6820 746f 2074 6865 2063 6c75   Path to the clu
-0000e8c0: 7374 6572 2079 616d 6c2e 0a20 2020 2020  ster yaml..     
-0000e8d0: 2020 2065 7870 6563 7465 645f 6e75 6d5f     expected_num_
-0000e8e0: 6e6f 6465 733a 2045 7870 6563 7465 6420  nodes: Expected 
-0000e8f0: 6e75 6d62 6572 206f 6620 6e6f 6465 7320  number of nodes 
-0000e900: 696e 2074 6865 2063 6c75 7374 6572 2e0a  in the cluster..
-0000e910: 2020 2020 2020 2020 6865 6164 5f69 705f          head_ip_
-0000e920: 6d61 785f 6174 7465 6d70 7473 3a20 4d61  max_attempts: Ma
-0000e930: 7820 6174 7465 6d70 7473 2074 6f20 6765  x attempts to ge
-0000e940: 7420 6865 6164 2069 702e 0a20 2020 2020  t head ip..     
-0000e950: 2020 2077 6f72 6b65 725f 6970 5f6d 6178     worker_ip_max
-0000e960: 5f61 7474 656d 7074 733a 204d 6178 2061  _attempts: Max a
-0000e970: 7474 656d 7074 7320 746f 2067 6574 2077  ttempts to get w
-0000e980: 6f72 6b65 7220 6970 732e 0a20 2020 2020  orker ips..     
-0000e990: 2020 2067 6574 5f69 6e74 6572 6e61 6c5f     get_internal_
-0000e9a0: 6970 733a 2057 6865 7468 6572 2074 6f20  ips: Whether to 
-0000e9b0: 6765 7420 696e 7465 726e 616c 2049 5073  get internal IPs
-0000e9c0: 2e20 5768 656e 2046 616c 7365 2c20 6974  . When False, it
-0000e9d0: 2069 7320 7374 696c 6c0a 2020 2020 2020   is still.      
-0000e9e0: 2020 2020 2020 706f 7373 6962 6c65 2074        possible t
-0000e9f0: 6f20 6765 7420 696e 7465 726e 616c 2049  o get internal I
-0000ea00: 5073 2069 6620 7468 6520 636c 7573 7465  Ps if the cluste
-0000ea10: 7220 646f 6573 206e 6f74 2068 6176 6520  r does not have 
-0000ea20: 6578 7465 726e 616c 0a20 2020 2020 2020  external.       
-0000ea30: 2020 2020 2049 5073 2e0a 0a20 2020 2052       IPs...    R
-0000ea40: 6169 7365 733a 0a20 2020 2020 2020 2065  aises:.        e
-0000ea50: 7863 6570 7469 6f6e 732e 4665 7463 6843  xceptions.FetchC
-0000ea60: 6c75 7374 6572 496e 666f 4572 726f 723a  lusterInfoError:
-0000ea70: 2069 6620 7765 2066 6169 6c65 6420 746f   if we failed to
-0000ea80: 2067 6574 2074 6865 2049 5073 2e20 652e   get the IPs. e.
-0000ea90: 7265 6173 6f6e 2069 730a 2020 2020 2020  reason is.      
-0000eaa0: 2020 2020 2020 4845 4144 206f 7220 574f        HEAD or WO
-0000eab0: 524b 4552 2e0a 2020 2020 2222 220a 2020  RKER..    """.  
-0000eac0: 2020 7261 795f 636f 6e66 6967 203d 2063    ray_config = c
-0000ead0: 6f6d 6d6f 6e5f 7574 696c 732e 7265 6164  ommon_utils.read
-0000eae0: 5f79 616d 6c28 636c 7573 7465 725f 7961  _yaml(cluster_ya
-0000eaf0: 6d6c 290a 2020 2020 2320 5573 6520 7468  ml).    # Use th
-0000eb00: 6520 6e65 7720 7072 6f76 6973 696f 6e65  e new provisione
-0000eb10: 7220 666f 7220 4157 532e 0a20 2020 2070  r for AWS..    p
-0000eb20: 726f 7669 6465 725f 6e61 6d65 203d 2063  rovider_name = c
-0000eb30: 6c75 7374 6572 5f79 616d 6c5f 7574 696c  luster_yaml_util
-0000eb40: 732e 6765 745f 7072 6f76 6964 6572 5f6e  s.get_provider_n
-0000eb50: 616d 6528 7261 795f 636f 6e66 6967 290a  ame(ray_config).
-0000eb60: 2020 2020 636c 6f75 6420 3d20 636c 6f75      cloud = clou
-0000eb70: 645f 7265 6769 7374 7279 2e43 4c4f 5544  d_registry.CLOUD
-0000eb80: 5f52 4547 4953 5452 592e 6672 6f6d 5f73  _REGISTRY.from_s
-0000eb90: 7472 2870 726f 7669 6465 725f 6e61 6d65  tr(provider_name
-0000eba0: 290a 2020 2020 6173 7365 7274 2063 6c6f  ).    assert clo
-0000ebb0: 7564 2069 7320 6e6f 7420 4e6f 6e65 2c20  ud is not None, 
-0000ebc0: 7072 6f76 6964 6572 5f6e 616d 650a 0a20  provider_name.. 
-0000ebd0: 2020 2069 6620 636c 6f75 642e 5052 4f56     if cloud.PROV
-0000ebe0: 4953 494f 4e45 525f 5645 5253 494f 4e20  ISIONER_VERSION 
-0000ebf0: 3e3d 2063 6c6f 7564 732e 5072 6f76 6973  >= clouds.Provis
-0000ec00: 696f 6e65 7256 6572 7369 6f6e 2e53 4b59  ionerVersion.SKY
-0000ec10: 5049 4c4f 543a 0a20 2020 2020 2020 2074  PILOT:.        t
-0000ec20: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-0000ec30: 6d65 7461 6461 7461 203d 2070 726f 7669  metadata = provi
-0000ec40: 7369 6f6e 5f6c 6962 2e67 6574 5f63 6c75  sion_lib.get_clu
-0000ec50: 7374 6572 5f69 6e66 6f28 0a20 2020 2020  ster_info(.     
-0000ec60: 2020 2020 2020 2020 2020 2070 726f 7669             provi
-0000ec70: 6465 725f 6e61 6d65 2c20 7261 795f 636f  der_name, ray_co
-0000ec80: 6e66 6967 5b27 7072 6f76 6964 6572 275d  nfig['provider']
-0000ec90: 2e67 6574 2827 7265 6769 6f6e 2729 2c0a  .get('region'),.
-0000eca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ecb0: 7261 795f 636f 6e66 6967 5b27 636c 7573  ray_config['clus
-0000ecc0: 7465 725f 6e61 6d65 275d 2c20 7261 795f  ter_name'], ray_
-0000ecd0: 636f 6e66 6967 5b27 7072 6f76 6964 6572  config['provider
-0000ece0: 275d 290a 2020 2020 2020 2020 6578 6365  ']).        exce
-0000ecf0: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-0000ed00: 653a 2020 2320 7079 6c69 6e74 3a20 6469  e:  # pylint: di
-0000ed10: 7361 626c 653d 6272 6f61 642d 6578 6365  sable=broad-exce
-0000ed20: 7074 0a20 2020 2020 2020 2020 2020 2023  pt.            #
-0000ed30: 2054 6869 7320 636f 756c 6420 6861 7070   This could happ
-0000ed40: 656e 2077 6865 6e20 7468 6520 564d 2069  en when the VM i
-0000ed50: 7320 6e6f 7420 6675 6c6c 7920 6c61 756e  s not fully laun
-0000ed60: 6368 6564 2c20 616e 6420 6120 7573 6572  ched, and a user
-0000ed70: 0a20 2020 2020 2020 2020 2020 2023 2069  .            # i
-0000ed80: 7320 7472 7969 6e67 2074 6f20 7465 726d  s trying to term
-0000ed90: 696e 6174 6520 6974 2077 6974 6820 6073  inate it with `s
-0000eda0: 6b79 2064 6f77 6e60 2e0a 2020 2020 2020  ky down`..      
-0000edb0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-0000edc0: 7567 280a 2020 2020 2020 2020 2020 2020  ug(.            
-0000edd0: 2020 2020 2746 6169 6c65 6420 746f 2067      'Failed to g
-0000ede0: 6574 2063 6c75 7374 6572 2069 6e66 6f20  et cluster info 
-0000edf0: 666f 7220 270a 2020 2020 2020 2020 2020  for '.          
-0000ee00: 2020 2020 2020 6627 7b72 6179 5f63 6f6e        f'{ray_con
-0000ee10: 6669 675b 2263 6c75 7374 6572 5f6e 616d  fig["cluster_nam
-0000ee20: 6522 5d7d 2066 726f 6d20 7468 6520 6e65  e"]} from the ne
-0000ee30: 7720 7072 6f76 6973 696f 6e65 7220 270a  w provisioner '.
-0000ee40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee50: 6627 7769 7468 207b 636f 6d6d 6f6e 5f75  f'with {common_u
-0000ee60: 7469 6c73 2e66 6f72 6d61 745f 6578 6365  tils.format_exce
-0000ee70: 7074 696f 6e28 6529 7d2e 2729 0a20 2020  ption(e)}.').   
-0000ee80: 2020 2020 2020 2020 2072 6169 7365 2065           raise e
-0000ee90: 7863 6570 7469 6f6e 732e 4665 7463 6843  xceptions.FetchC
-0000eea0: 6c75 7374 6572 496e 666f 4572 726f 7228  lusterInfoError(
-0000eeb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000eec0: 2065 7863 6570 7469 6f6e 732e 4665 7463   exceptions.Fetc
-0000eed0: 6843 6c75 7374 6572 496e 666f 4572 726f  hClusterInfoErro
-0000eee0: 722e 5265 6173 6f6e 2e48 4541 4429 2066  r.Reason.HEAD) f
-0000eef0: 726f 6d20 650a 2020 2020 2020 2020 6966  rom e.        if
-0000ef00: 206c 656e 286d 6574 6164 6174 612e 696e   len(metadata.in
-0000ef10: 7374 616e 6365 7329 203c 2065 7870 6563  stances) < expec
-0000ef20: 7465 645f 6e75 6d5f 6e6f 6465 733a 0a20  ted_num_nodes:. 
-0000ef30: 2020 2020 2020 2020 2020 2023 2053 696d             # Sim
-0000ef40: 756c 6174 6520 7468 6520 6578 6365 7074  ulate the except
-0000ef50: 696f 6e20 7768 656e 2052 6179 2068 6561  ion when Ray hea
-0000ef60: 6420 6e6f 6465 2069 7320 6e6f 7420 7570  d node is not up
-0000ef70: 2e0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
-0000ef80: 6973 6520 6578 6365 7074 696f 6e73 2e46  ise exceptions.F
-0000ef90: 6574 6368 436c 7573 7465 7249 6e66 6f45  etchClusterInfoE
-0000efa0: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
-0000efb0: 2020 2020 2020 6578 6365 7074 696f 6e73        exceptions
-0000efc0: 2e46 6574 6368 436c 7573 7465 7249 6e66  .FetchClusterInf
-0000efd0: 6f45 7272 6f72 2e52 6561 736f 6e2e 4845  oError.Reason.HE
-0000efe0: 4144 290a 2020 2020 2020 2020 7265 7475  AD).        retu
-0000eff0: 726e 206d 6574 6164 6174 612e 6765 745f  rn metadata.get_
-0000f000: 6665 6173 6962 6c65 5f69 7073 2867 6574  feasible_ips(get
-0000f010: 5f69 6e74 6572 6e61 6c5f 6970 7329 0a0a  _internal_ips)..
-0000f020: 2020 2020 6966 2067 6574 5f69 6e74 6572      if get_inter
-0000f030: 6e61 6c5f 6970 733a 0a20 2020 2020 2020  nal_ips:.       
-0000f040: 2077 6974 6820 7465 6d70 6669 6c65 2e4e   with tempfile.N
-0000f050: 616d 6564 5465 6d70 6f72 6172 7946 696c  amedTemporaryFil
-0000f060: 6528 6d6f 6465 3d27 7727 2c20 6465 6c65  e(mode='w', dele
-0000f070: 7465 3d46 616c 7365 2920 6173 2066 3a0a  te=False) as f:.
-0000f080: 2020 2020 2020 2020 2020 2020 7261 795f              ray_
-0000f090: 636f 6e66 6967 5b27 7072 6f76 6964 6572  config['provider
-0000f0a0: 275d 5b27 7573 655f 696e 7465 726e 616c  ']['use_internal
-0000f0b0: 5f69 7073 275d 203d 2054 7275 650a 2020  _ips'] = True.  
-0000f0c0: 2020 2020 2020 2020 2020 7961 6d6c 2e64            yaml.d
-0000f0d0: 756d 7028 7261 795f 636f 6e66 6967 2c20  ump(ray_config, 
-0000f0e0: 6629 0a20 2020 2020 2020 2020 2020 2063  f).            c
-0000f0f0: 6c75 7374 6572 5f79 616d 6c20 3d20 662e  luster_yaml = f.
-0000f100: 6e61 6d65 0a0a 2020 2020 2320 4368 6563  name..    # Chec
-0000f110: 6b20 7468 6520 6e65 7477 6f72 6b20 636f  k the network co
-0000f120: 6e6e 6563 7469 6f6e 2066 6972 7374 2074  nnection first t
-0000f130: 6f20 6176 6f69 6420 6c6f 6e67 2068 616e  o avoid long han
-0000f140: 6769 6e67 2074 696d 6520 666f 720a 2020  ging time for.  
-0000f150: 2020 2320 7261 7920 6765 742d 6865 6164    # ray get-head
-0000f160: 2d69 7020 6265 6c6f 772c 2069 6620 6120  -ip below, if a 
-0000f170: 6c6f 6e67 2d6c 6173 7469 6e67 206e 6574  long-lasting net
-0000f180: 776f 726b 2063 6f6e 6e65 6374 696f 6e20  work connection 
-0000f190: 6661 696c 7572 650a 2020 2020 2320 6861  failure.    # ha
-0000f1a0: 7070 656e 732e 0a20 2020 2063 6865 636b  ppens..    check
-0000f1b0: 5f6e 6574 776f 726b 5f63 6f6e 6e65 6374  _network_connect
-0000f1c0: 696f 6e28 290a 2020 2020 6865 6164 5f69  ion().    head_i
-0000f1d0: 7020 3d20 5f71 7565 7279 5f68 6561 645f  p = _query_head_
-0000f1e0: 6970 5f77 6974 685f 7265 7472 6965 7328  ip_with_retries(
-0000f1f0: 636c 7573 7465 725f 7961 6d6c 2c0a 2020  cluster_yaml,.  
-0000f200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f220: 2020 2020 2020 2020 6d61 785f 6174 7465          max_atte
-0000f230: 6d70 7473 3d68 6561 645f 6970 5f6d 6178  mpts=head_ip_max
-0000f240: 5f61 7474 656d 7074 7329 0a20 2020 2068  _attempts).    h
-0000f250: 6561 645f 6970 5f6c 6973 7420 3d20 5b68  ead_ip_list = [h
-0000f260: 6561 645f 6970 5d0a 2020 2020 6966 2065  ead_ip].    if e
-0000f270: 7870 6563 7465 645f 6e75 6d5f 6e6f 6465  xpected_num_node
-0000f280: 7320 3e20 313a 0a20 2020 2020 2020 2062  s > 1:.        b
-0000f290: 6163 6b6f 6666 203d 2063 6f6d 6d6f 6e5f  ackoff = common_
-0000f2a0: 7574 696c 732e 4261 636b 6f66 6628 696e  utils.Backoff(in
-0000f2b0: 6974 6961 6c5f 6261 636b 6f66 663d 352c  itial_backoff=5,
-0000f2c0: 206d 6178 5f62 6163 6b6f 6666 5f66 6163   max_backoff_fac
-0000f2d0: 746f 723d 3529 0a0a 2020 2020 2020 2020  tor=5)..        
-0000f2e0: 666f 7220 7265 7472 795f 636e 7420 696e  for retry_cnt in
-0000f2f0: 2072 616e 6765 2877 6f72 6b65 725f 6970   range(worker_ip
-0000f300: 5f6d 6178 5f61 7474 656d 7074 7329 3a0a  _max_attempts):.
-0000f310: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-0000f320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f330: 2066 756c 6c5f 636c 7573 7465 725f 7961   full_cluster_ya
-0000f340: 6d6c 203d 2073 7472 2870 6174 686c 6962  ml = str(pathlib
-0000f350: 2e50 6174 6828 636c 7573 7465 725f 7961  .Path(cluster_ya
-0000f360: 6d6c 292e 6578 7061 6e64 7573 6572 2829  ml).expanduser()
-0000f370: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000f380: 2020 7072 6f63 203d 2073 7562 7072 6f63    proc = subproc
-0000f390: 6573 735f 7574 696c 732e 7275 6e28 0a20  ess_utils.run(. 
-0000f3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f3b0: 2020 2066 2772 6179 2067 6574 2d77 6f72     f'ray get-wor
-0000f3c0: 6b65 722d 6970 7320 7b66 756c 6c5f 636c  ker-ips {full_cl
-0000f3d0: 7573 7465 725f 7961 6d6c 2172 7d27 2c0a  uster_yaml!r}',.
-0000f3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f3f0: 2020 2020 7374 646f 7574 3d73 7562 7072      stdout=subpr
-0000f400: 6f63 6573 732e 5049 5045 2c0a 2020 2020  ocess.PIPE,.    
-0000f410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f420: 7374 6465 7272 3d73 7562 7072 6f63 6573  stderr=subproces
-0000f430: 732e 5049 5045 290a 2020 2020 2020 2020  s.PIPE).        
-0000f440: 2020 2020 2020 2020 6f75 7420 3d20 7072          out = pr
-0000f450: 6f63 2e73 7464 6f75 742e 6465 636f 6465  oc.stdout.decode
-0000f460: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-0000f470: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
-0000f480: 2020 2020 2065 7863 6570 7420 7375 6270       except subp
-0000f490: 726f 6365 7373 2e43 616c 6c65 6450 726f  rocess.CalledPro
-0000f4a0: 6365 7373 4572 726f 7220 6173 2065 3a0a  cessError as e:.
-0000f4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f4c0: 6966 2072 6574 7279 5f63 6e74 203d 3d20  if retry_cnt == 
-0000f4d0: 776f 726b 6572 5f69 705f 6d61 785f 6174  worker_ip_max_at
-0000f4e0: 7465 6d70 7473 202d 2031 3a0a 2020 2020  tempts - 1:.    
-0000f4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f500: 7261 6973 6520 6578 6365 7074 696f 6e73  raise exceptions
-0000f510: 2e46 6574 6368 436c 7573 7465 7249 6e66  .FetchClusterInf
-0000f520: 6f45 7272 6f72 280a 2020 2020 2020 2020  oError(.        
-0000f530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f540: 6578 6365 7074 696f 6e73 2e46 6574 6368  exceptions.Fetch
-0000f550: 436c 7573 7465 7249 6e66 6f45 7272 6f72  ClusterInfoError
-0000f560: 2e52 6561 736f 6e2e 574f 524b 4552 2920  .Reason.WORKER) 
-0000f570: 6672 6f6d 2065 0a20 2020 2020 2020 2020  from e.         
-0000f580: 2020 2020 2020 2023 2052 6574 7279 2069         # Retry i
-0000f590: 6620 7468 6520 7373 6820 6973 206e 6f74  f the ssh is not
-0000f5a0: 2072 6561 6479 2066 6f72 2074 6865 2077   ready for the w
-0000f5b0: 6f72 6b65 7273 2079 6574 2e0a 2020 2020  orkers yet..    
-0000f5c0: 2020 2020 2020 2020 2020 2020 6261 636b              back
-0000f5d0: 6f66 665f 7469 6d65 203d 2062 6163 6b6f  off_time = backo
-0000f5e0: 6666 2e63 7572 7265 6e74 5f62 6163 6b6f  ff.current_backo
-0000f5f0: 6666 2829 0a20 2020 2020 2020 2020 2020  ff().           
-0000f600: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-0000f610: 6728 2752 6574 7279 696e 6720 746f 2067  g('Retrying to g
-0000f620: 6574 2077 6f72 6b65 7220 6970 2027 0a20  et worker ip '. 
-0000f630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f640: 2020 2020 2020 2020 2020 2020 6627 5b7b              f'[{
-0000f650: 7265 7472 795f 636e 747d 2f7b 776f 726b  retry_cnt}/{work
-0000f660: 6572 5f69 705f 6d61 785f 6174 7465 6d70  er_ip_max_attemp
-0000f670: 7473 7d5d 2069 6e20 270a 2020 2020 2020  ts}] in '.      
-0000f680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f690: 2020 2020 2020 2066 277b 6261 636b 6f66         f'{backof
-0000f6a0: 665f 7469 6d65 7d20 7365 636f 6e64 732e  f_time} seconds.
-0000f6b0: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
-0000f6c0: 2020 2074 696d 652e 736c 6565 7028 6261     time.sleep(ba
-0000f6d0: 636b 6f66 665f 7469 6d65 290a 2020 2020  ckoff_time).    
-0000f6e0: 2020 2020 776f 726b 6572 5f69 7073 203d      worker_ips =
-0000f6f0: 2072 652e 6669 6e64 616c 6c28 4950 5f41   re.findall(IP_A
-0000f700: 4444 525f 5245 4745 582c 206f 7574 290a  DDR_REGEX, out).
-0000f710: 2020 2020 2020 2020 6966 206c 656e 2877          if len(w
-0000f720: 6f72 6b65 725f 6970 7329 2021 3d20 6578  orker_ips) != ex
-0000f730: 7065 6374 6564 5f6e 756d 5f6e 6f64 6573  pected_num_nodes
-0000f740: 202d 2031 3a0a 2020 2020 2020 2020 2020   - 1:.          
-0000f750: 2020 6e20 3d20 6578 7065 6374 6564 5f6e    n = expected_n
-0000f760: 756d 5f6e 6f64 6573 202d 2031 0a20 2020  um_nodes - 1.   
-0000f770: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
-0000f780: 776f 726b 6572 5f69 7073 2920 3e20 6e3a  worker_ips) > n:
-0000f790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f7a0: 2023 2054 6869 7320 636f 756c 6420 6265   # This could be
-0000f7b0: 2074 7269 6767 6572 6564 2069 6620 652e   triggered if e.
-0000f7c0: 672e 2c20 736f 6d65 206c 6f67 6769 6e67  g., some logging
-0000f7d0: 2069 7320 6164 6465 6420 696e 0a20 2020   is added in.   
-0000f7e0: 2020 2020 2020 2020 2020 2020 2023 2073               # s
-0000f7f0: 6b79 7069 6c6f 745f 636f 6e66 6967 2c20  kypilot_config, 
-0000f800: 6120 6d6f 6475 6c65 2074 6861 7420 6861  a module that ha
-0000f810: 7320 736f 6d65 2063 6f64 6520 6578 6563  s some code exec
-0000f820: 7574 6564 2077 6865 6e65 7665 720a 2020  uted whenever.  
-0000f830: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000f840: 6073 6b79 6020 6973 2069 6d70 6f72 7465  `sky` is importe
-0000f850: 642e 0a20 2020 2020 2020 2020 2020 2020  d..             
-0000f860: 2020 206c 6f67 6765 722e 7761 726e 696e     logger.warnin
-0000f870: 6728 0a20 2020 2020 2020 2020 2020 2020  g(.             
-0000f880: 2020 2020 2020 2066 2745 7870 6563 7465         f'Expecte
-0000f890: 6420 7b6e 7d20 776f 726b 6572 2049 5028  d {n} worker IP(
-0000f8a0: 7329 3b20 666f 756e 6420 270a 2020 2020  s); found '.    
-0000f8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f8c0: 6627 7b6c 656e 2877 6f72 6b65 725f 6970  f'{len(worker_ip
-0000f8d0: 7329 7d3a 207b 776f 726b 6572 5f69 7073  s)}: {worker_ips
-0000f8e0: 7d27 0a20 2020 2020 2020 2020 2020 2020  }'.             
-0000f8f0: 2020 2020 2020 2027 5c6e 5468 6973 2063         '\nThis c
-0000f900: 6f75 6c64 2068 6170 7065 6e20 6966 2074  ould happen if t
-0000f910: 6865 7265 2069 7320 6578 7472 6120 6f75  here is extra ou
-0000f920: 7470 7574 2066 726f 6d20 270a 2020 2020  tput from '.    
-0000f930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f940: 2760 7261 7920 6765 742d 776f 726b 6572  '`ray get-worker
-0000f950: 2d69 7073 602c 2077 6869 6368 2073 686f  -ips`, which sho
-0000f960: 756c 6420 6265 2069 6e73 7065 6374 6564  uld be inspected
-0000f970: 2062 656c 6f77 2e27 0a20 2020 2020 2020   below.'.       
-0000f980: 2020 2020 2020 2020 2020 2020 2066 275c               f'\
-0000f990: 6e3d 3d20 4f75 7470 7574 203d 3d5c 6e7b  n== Output ==\n{
-0000f9a0: 6f75 747d 270a 2020 2020 2020 2020 2020  out}'.          
-0000f9b0: 2020 2020 2020 2020 2020 6627 5c6e 3d3d            f'\n==
-0000f9c0: 204f 7574 7075 7420 656e 6473 203d 3d27   Output ends =='
-0000f9d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000f9e0: 2020 6c6f 6767 6572 2e77 6172 6e69 6e67    logger.warning
-0000f9f0: 2866 275c 6e50 726f 6365 6564 696e 6720  (f'\nProceeding 
-0000fa00: 7769 7468 2074 6865 206c 6173 7420 7b6e  with the last {n
-0000fa10: 7d20 270a 2020 2020 2020 2020 2020 2020  } '.            
-0000fa20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa30: 2020 2066 2764 6574 6563 7465 6420 4950     f'detected IP
-0000fa40: 2873 293a 207b 776f 726b 6572 5f69 7073  (s): {worker_ips
-0000fa50: 5b2d 6e3a 5d7d 2e27 290a 2020 2020 2020  [-n:]}.').      
-0000fa60: 2020 2020 2020 2020 2020 776f 726b 6572            worker
-0000fa70: 5f69 7073 203d 2077 6f72 6b65 725f 6970  _ips = worker_ip
-0000fa80: 735b 2d6e 3a5d 0a20 2020 2020 2020 2020  s[-n:].         
-0000fa90: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000faa0: 2020 2020 2020 2020 2072 6169 7365 2065           raise e
-0000fab0: 7863 6570 7469 6f6e 732e 4665 7463 6843  xceptions.FetchC
-0000fac0: 6c75 7374 6572 496e 666f 4572 726f 7228  lusterInfoError(
-0000fad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fae0: 2020 2020 2065 7863 6570 7469 6f6e 732e       exceptions.
-0000faf0: 4665 7463 6843 6c75 7374 6572 496e 666f  FetchClusterInfo
-0000fb00: 4572 726f 722e 5265 6173 6f6e 2e57 4f52  Error.Reason.WOR
-0000fb10: 4b45 5229 0a20 2020 2065 6c73 653a 0a20  KER).    else:. 
-0000fb20: 2020 2020 2020 2077 6f72 6b65 725f 6970         worker_ip
-0000fb30: 7320 3d20 5b5d 0a20 2020 2072 6574 7572  s = [].    retur
-0000fb40: 6e20 6865 6164 5f69 705f 6c69 7374 202b  n head_ip_list +
-0000fb50: 2077 6f72 6b65 725f 6970 730a 0a0a 6465   worker_ips...de
-0000fb60: 6620 6368 6563 6b5f 6e65 7477 6f72 6b5f  f check_network_
-0000fb70: 636f 6e6e 6563 7469 6f6e 2829 3a0a 2020  connection():.  
-0000fb80: 2020 2320 546f 6c65 7261 7465 2033 2072    # Tolerate 3 r
-0000fb90: 6574 7269 6573 2061 7320 6974 2069 7320  etries as it is 
-0000fba0: 6f62 7365 7276 6564 2074 6861 7420 636f  observed that co
-0000fbb0: 6e6e 6563 7469 6f6e 7320 6361 6e20 6661  nnections can fa
-0000fbc0: 696c 2e0a 2020 2020 6164 6170 7465 7220  il..    adapter 
-0000fbd0: 3d20 6164 6170 7465 7273 2e48 5454 5041  = adapters.HTTPA
-0000fbe0: 6461 7074 6572 286d 6178 5f72 6574 7269  dapter(max_retri
-0000fbf0: 6573 3d72 6574 7279 5f6c 6962 2e52 6574  es=retry_lib.Ret
-0000fc00: 7279 2874 6f74 616c 3d33 2929 0a20 2020  ry(total=3)).   
-0000fc10: 2068 7474 7020 3d20 7265 7175 6573 7473   http = requests
-0000fc20: 2e53 6573 7369 6f6e 2829 0a20 2020 2068  .Session().    h
-0000fc30: 7474 702e 6d6f 756e 7428 2768 7474 7073  ttp.mount('https
-0000fc40: 3a2f 2f27 2c20 6164 6170 7465 7229 0a20  ://', adapter). 
-0000fc50: 2020 2068 7474 702e 6d6f 756e 7428 2768     http.mount('h
-0000fc60: 7474 703a 2f2f 272c 2061 6461 7074 6572  ttp://', adapter
-0000fc70: 290a 2020 2020 666f 7220 692c 2069 7020  ).    for i, ip 
-0000fc80: 696e 2065 6e75 6d65 7261 7465 285f 5445  in enumerate(_TE
-0000fc90: 5354 5f49 505f 4c49 5354 293a 0a20 2020  ST_IP_LIST):.   
-0000fca0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-0000fcb0: 2020 2020 2020 6874 7470 2e68 6561 6428        http.head(
-0000fcc0: 6970 2c20 7469 6d65 6f75 743d 3329 0a20  ip, timeout=3). 
-0000fcd0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000fce0: 6e0a 2020 2020 2020 2020 6578 6365 7074  n.        except
-0000fcf0: 2028 7265 7175 6573 7473 2e54 696d 656f   (requests.Timeo
-0000fd00: 7574 2c20 7265 7175 6573 7473 2e65 7863  ut, requests.exc
-0000fd10: 6570 7469 6f6e 732e 436f 6e6e 6563 7469  eptions.Connecti
-0000fd20: 6f6e 4572 726f 7229 2061 7320 653a 0a20  onError) as e:. 
-0000fd30: 2020 2020 2020 2020 2020 2069 6620 6920             if i 
-0000fd40: 3d3d 206c 656e 285f 5445 5354 5f49 505f  == len(_TEST_IP_
-0000fd50: 4c49 5354 2920 2d20 313a 0a20 2020 2020  LIST) - 1:.     
-0000fd60: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0000fd70: 2065 7863 6570 7469 6f6e 732e 4e65 7477   exceptions.Netw
-0000fd80: 6f72 6b45 7272 6f72 2827 436f 756c 6420  orkError('Could 
-0000fd90: 6e6f 7420 7265 6672 6573 6820 7468 6520  not refresh the 
-0000fda0: 636c 7573 7465 722e 2027 0a20 2020 2020  cluster. '.     
-0000fdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fdd0: 2020 2020 2020 2020 2027 4e65 7477 6f72           'Networ
-0000fde0: 6b20 7365 656d 7320 646f 776e 2e27 2920  k seems down.') 
-0000fdf0: 6672 6f6d 2065 0a0a 0a64 6566 2063 6865  from e...def che
-0000fe00: 636b 5f6f 776e 6572 5f69 6465 6e74 6974  ck_owner_identit
-0000fe10: 7928 636c 7573 7465 725f 6e61 6d65 3a20  y(cluster_name: 
-0000fe20: 7374 7229 202d 3e20 4e6f 6e65 3a0a 2020  str) -> None:.  
-0000fe30: 2020 2222 2243 6865 636b 2069 6620 6375    """Check if cu
-0000fe40: 7272 656e 7420 7573 6572 2069 7320 7468  rrent user is th
-0000fe50: 6520 7361 6d65 2061 7320 7468 6520 7573  e same as the us
-0000fe60: 6572 2077 686f 2063 7265 6174 6564 2074  er who created t
-0000fe70: 6865 2063 6c75 7374 6572 2e0a 0a20 2020  he cluster...   
-0000fe80: 2052 6169 7365 733a 0a20 2020 2020 2020   Raises:.       
-0000fe90: 2065 7863 6570 7469 6f6e 732e 436c 7573   exceptions.Clus
-0000fea0: 7465 724f 776e 6572 4964 656e 7469 7479  terOwnerIdentity
-0000feb0: 4d69 736d 6174 6368 4572 726f 723a 2069  MismatchError: i
-0000fec0: 6620 7468 6520 6375 7272 656e 7420 7573  f the current us
-0000fed0: 6572 2069 730a 2020 2020 2020 2020 2020  er is.          
-0000fee0: 6e6f 7420 7468 6520 7361 6d65 2061 7320  not the same as 
-0000fef0: 7468 6520 7573 6572 2077 686f 2063 7265  the user who cre
-0000ff00: 6174 6564 2074 6865 2063 6c75 7374 6572  ated the cluster
-0000ff10: 2e0a 2020 2020 2020 2020 6578 6365 7074  ..        except
-0000ff20: 696f 6e73 2e43 6c6f 7564 5573 6572 4964  ions.CloudUserId
-0000ff30: 656e 7469 7479 4572 726f 723a 2069 6620  entityError: if 
-0000ff40: 7765 2066 6169 6c20 746f 2067 6574 2074  we fail to get t
-0000ff50: 6865 2063 7572 7265 6e74 2075 7365 720a  he current user.
-0000ff60: 2020 2020 2020 2020 2020 6964 656e 7469            identi
-0000ff70: 7479 2e0a 2020 2020 2222 220a 2020 2020  ty..    """.    
-0000ff80: 6966 2065 6e76 5f6f 7074 696f 6e73 2e4f  if env_options.O
-0000ff90: 7074 696f 6e73 2e53 4b49 505f 434c 4f55  ptions.SKIP_CLOU
-0000ffa0: 445f 4944 454e 5449 5459 5f43 4845 434b  D_IDENTITY_CHECK
-0000ffb0: 2e67 6574 2829 3a0a 2020 2020 2020 2020  .get():.        
-0000ffc0: 7265 7475 726e 0a20 2020 2072 6563 6f72  return.    recor
-0000ffd0: 6420 3d20 676c 6f62 616c 5f75 7365 725f  d = global_user_
-0000ffe0: 7374 6174 652e 6765 745f 636c 7573 7465  state.get_cluste
-0000fff0: 725f 6672 6f6d 5f6e 616d 6528 636c 7573  r_from_name(clus
-00010000: 7465 725f 6e61 6d65 290a 2020 2020 6966  ter_name).    if
-00010010: 2072 6563 6f72 6420 6973 204e 6f6e 653a   record is None:
-00010020: 0a20 2020 2020 2020 2072 6574 7572 6e0a  .        return.
-00010030: 2020 2020 6861 6e64 6c65 203d 2072 6563      handle = rec
-00010040: 6f72 645b 2768 616e 646c 6527 5d0a 2020  ord['handle'].  
-00010050: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
-00010060: 6e63 6528 6861 6e64 6c65 2c20 6261 636b  nce(handle, back
-00010070: 656e 6473 2e43 6c6f 7564 566d 5261 7952  ends.CloudVmRayR
-00010080: 6573 6f75 7263 6548 616e 646c 6529 3a0a  esourceHandle):.
-00010090: 2020 2020 2020 2020 7265 7475 726e 0a0a          return..
-000100a0: 2020 2020 636c 6f75 6420 3d20 6861 6e64      cloud = hand
-000100b0: 6c65 2e6c 6175 6e63 6865 645f 7265 736f  le.launched_reso
-000100c0: 7572 6365 732e 636c 6f75 640a 2020 2020  urces.cloud.    
-000100d0: 6375 7272 656e 745f 7573 6572 5f69 6465  current_user_ide
-000100e0: 6e74 6974 7920 3d20 636c 6f75 642e 6765  ntity = cloud.ge
-000100f0: 745f 6375 7272 656e 745f 7573 6572 5f69  t_current_user_i
-00010100: 6465 6e74 6974 7928 290a 2020 2020 6f77  dentity().    ow
-00010110: 6e65 725f 6964 656e 7469 7479 203d 2072  ner_identity = r
-00010120: 6563 6f72 645b 276f 776e 6572 275d 0a20  ecord['owner']. 
-00010130: 2020 2069 6620 6375 7272 656e 745f 7573     if current_us
-00010140: 6572 5f69 6465 6e74 6974 7920 6973 204e  er_identity is N
-00010150: 6f6e 653a 0a20 2020 2020 2020 2023 2053  one:.        # S
-00010160: 6b69 7020 7468 6520 6368 6563 6b20 6966  kip the check if
-00010170: 2074 6865 2063 6c6f 7564 2064 6f65 7320   the cloud does 
-00010180: 6e6f 7420 7375 7070 6f72 7420 7573 6572  not support user
-00010190: 2069 6465 6e74 6974 792e 0a20 2020 2020   identity..     
-000101a0: 2020 2072 6574 7572 6e0a 2020 2020 2320     return.    # 
-000101b0: 5468 6520 7573 6572 2069 6465 6e74 6974  The user identit
-000101c0: 7920 6361 6e20 6265 204e 6f6e 652c 2069  y can be None, i
-000101d0: 6620 7468 6520 636c 7573 7465 7220 6973  f the cluster is
-000101e0: 2063 7265 6174 6564 2062 7920 616e 206f   created by an o
-000101f0: 6c64 6572 0a20 2020 2023 2076 6572 7369  lder.    # versi
-00010200: 6f6e 206f 6620 536b 7950 696c 6f74 2e20  on of SkyPilot. 
-00010210: 496e 2074 6861 7420 6361 7365 2c20 7765  In that case, we
-00010220: 2073 6574 2074 6865 2075 7365 7220 6964   set the user id
-00010230: 656e 7469 7479 2074 6f20 7468 650a 2020  entity to the.  
-00010240: 2020 2320 6375 7272 656e 7420 6f6e 652e    # current one.
-00010250: 0a20 2020 2023 204e 4f54 453a 2061 2075  .    # NOTE: a u
-00010260: 7365 7220 7768 6f20 7570 6772 6164 6573  ser who upgrades
-00010270: 2053 6b79 5069 6c6f 7420 616e 6420 7377   SkyPilot and sw
-00010280: 6974 6368 6573 2074 6f20 6120 6e65 7720  itches to a new 
-00010290: 636c 6f75 6420 6964 656e 7469 7479 0a20  cloud identity. 
-000102a0: 2020 2023 2069 6d6d 6564 6961 7465 6c79     # immediately
-000102b0: 2077 6974 686f 7574 2060 736b 7920 7374   without `sky st
-000102c0: 6174 7573 202d 2d72 6566 7265 7368 6020  atus --refresh` 
-000102d0: 6669 7273 742c 2077 696c 6c20 6361 7573  first, will caus
-000102e0: 6520 6120 6c65 616b 6167 650a 2020 2020  e a leakage.    
-000102f0: 2320 6f66 2074 6865 2065 7869 7374 696e  # of the existin
-00010300: 6720 636c 7573 7465 722e 2057 6520 6465  g cluster. We de
-00010310: 656d 2074 6869 7320 616e 2061 6363 6570  em this an accep
-00010320: 7461 626c 6520 7472 6164 656f 6666 206d  table tradeoff m
-00010330: 6169 6e6c 790a 2020 2020 2320 6265 6361  ainly.    # beca
-00010340: 7573 6520 6d75 6c74 692d 6964 656e 7469  use multi-identi
-00010350: 7479 2069 7320 6e6f 7420 636f 6d6d 6f6e  ty is not common
-00010360: 2028 6174 206c 6561 7374 2061 7420 7468   (at least at th
-00010370: 6520 6d6f 6d65 6e74 292e 0a20 2020 2069  e moment)..    i
-00010380: 6620 6f77 6e65 725f 6964 656e 7469 7479  f owner_identity
-00010390: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-000103a0: 2020 676c 6f62 616c 5f75 7365 725f 7374    global_user_st
-000103b0: 6174 652e 7365 745f 6f77 6e65 725f 6964  ate.set_owner_id
-000103c0: 656e 7469 7479 5f66 6f72 5f63 6c75 7374  entity_for_clust
-000103d0: 6572 280a 2020 2020 2020 2020 2020 2020  er(.            
-000103e0: 636c 7573 7465 725f 6e61 6d65 2c20 6375  cluster_name, cu
-000103f0: 7272 656e 745f 7573 6572 5f69 6465 6e74  rrent_user_ident
-00010400: 6974 7929 0a20 2020 2065 6c73 653a 0a20  ity).    else:. 
-00010410: 2020 2020 2020 2061 7373 6572 7420 6973         assert is
-00010420: 696e 7374 616e 6365 286f 776e 6572 5f69  instance(owner_i
-00010430: 6465 6e74 6974 792c 206c 6973 7429 0a20  dentity, list). 
-00010440: 2020 2020 2020 2023 2049 7420 6973 204f         # It is O
-00010450: 4b20 6966 2074 6865 206f 776e 6572 2069  K if the owner i
-00010460: 6465 6e74 6974 7920 6973 2073 686f 7274  dentity is short
-00010470: 6572 2c20 7768 6963 6820 7769 6c6c 2068  er, which will h
-00010480: 6170 7065 6e20 7768 656e 0a20 2020 2020  appen when.     
-00010490: 2020 2023 2074 6865 2063 6c75 7374 6572     # the cluster
-000104a0: 2069 7320 6c61 756e 6368 6564 2062 6566   is launched bef
-000104b0: 6f72 6520 2331 3830 382e 2049 6e20 7468  ore #1808. In th
-000104c0: 6174 2063 6173 652c 2077 6520 6f6e 6c79  at case, we only
-000104d0: 2063 6865 636b 0a20 2020 2020 2020 2023   check.        #
-000104e0: 2074 6865 2073 616d 6520 6c65 6e67 7468   the same length
-000104f0: 2028 7a69 7020 7769 6c6c 2073 746f 7020   (zip will stop 
-00010500: 6174 2074 6865 2073 686f 7274 6572 206f  at the shorter o
-00010510: 6e65 292e 0a20 2020 2020 2020 2066 6f72  ne)..        for
-00010520: 2069 2c20 286f 776e 6572 2c0a 2020 2020   i, (owner,.    
-00010530: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00010540: 656e 7429 2069 6e20 656e 756d 6572 6174  ent) in enumerat
-00010550: 6528 7a69 7028 6f77 6e65 725f 6964 656e  e(zip(owner_iden
-00010560: 7469 7479 2c0a 2020 2020 2020 2020 2020  tity,.          
-00010570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d770: 2020 2020 2020 2020 2020 2020 2020 7374                st
+0000d780: 6465 7272 3d73 7464 6f75 7420 2b20 7374  derr=stdout + st
+0000d790: 6465 7272 290a 0a20 2020 2020 2020 2069  derr)..        i
+0000d7a0: 6620 7275 6e5f 7273 796e 633a 0a20 2020  f run_rsync:.   
+0000d7b0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+0000d7c0: 736f 7572 6365 2069 7320 6e6f 7420 4e6f  source is not No
+0000d7d0: 6e65 0a20 2020 2020 2020 2020 2020 2023  ne.            #
+0000d7e0: 2054 4f44 4f28 7a68 7775 293a 204f 7074   TODO(zhwu): Opt
+0000d7f0: 696d 697a 6520 666f 7220 6c61 7267 6520  imize for large 
+0000d800: 616d 6f75 6e74 206f 6620 6669 6c65 732e  amount of files.
+0000d810: 0a20 2020 2020 2020 2020 2020 2023 207a  .            # z
+0000d820: 6970 202f 2074 7261 6e73 6665 7220 2f20  ip / transfer / 
+0000d830: 756e 7a69 700a 2020 2020 2020 2020 2020  unzip.          
+0000d840: 2020 7275 6e6e 6572 2e72 7379 6e63 280a    runner.rsync(.
+0000d850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d860: 736f 7572 6365 3d73 6f75 7263 652c 0a20  source=source,. 
+0000d870: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000d880: 6172 6765 743d 7461 7267 6574 2c0a 2020  arget=target,.  
+0000d890: 2020 2020 2020 2020 2020 2020 2020 7570                up
+0000d8a0: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
+0000d8b0: 2020 2020 2020 206c 6f67 5f70 6174 683d         log_path=
+0000d8c0: 6c6f 675f 7061 7468 2c0a 2020 2020 2020  log_path,.      
+0000d8d0: 2020 2020 2020 2020 2020 7374 7265 616d            stream
+0000d8e0: 5f6c 6f67 733d 7374 7265 616d 5f6c 6f67  _logs=stream_log
+0000d8f0: 732c 0a20 2020 2020 2020 2020 2020 2029  s,.            )
+0000d900: 0a0a 2020 2020 6e75 6d5f 6e6f 6465 7320  ..    num_nodes 
+0000d910: 3d20 6c65 6e28 7275 6e6e 6572 7329 0a20  = len(runners). 
+0000d920: 2020 2070 6c75 7261 6c20 3d20 2773 2720     plural = 's' 
+0000d930: 6966 206e 756d 5f6e 6f64 6573 203e 2031  if num_nodes > 1
+0000d940: 2065 6c73 6520 2727 0a20 2020 206d 6573   else ''.    mes
+0000d950: 7361 6765 203d 2028 6627 7b66 6f72 652e  sage = (f'{fore.
+0000d960: 4359 414e 7d7b 6163 7469 6f6e 5f6d 6573  CYAN}{action_mes
+0000d970: 7361 6765 7d20 2874 6f20 7b6e 756d 5f6e  sage} (to {num_n
+0000d980: 6f64 6573 7d20 6e6f 6465 7b70 6c75 7261  odes} node{plura
+0000d990: 6c7d 2927 0a20 2020 2020 2020 2020 2020  l})'.           
+0000d9a0: 2020 2020 6627 3a20 7b73 7479 6c65 2e42      f': {style.B
+0000d9b0: 5249 4748 547d 7b6f 7269 6769 6e5f 736f  RIGHT}{origin_so
+0000d9c0: 7572 6365 7d7b 7374 796c 652e 5245 5345  urce}{style.RESE
+0000d9d0: 545f 414c 4c7d 202d 3e20 270a 2020 2020  T_ALL} -> '.    
+0000d9e0: 2020 2020 2020 2020 2020 2066 277b 7374             f'{st
+0000d9f0: 796c 652e 4252 4947 4854 7d7b 7461 7267  yle.BRIGHT}{targ
+0000da00: 6574 7d7b 7374 796c 652e 5245 5345 545f  et}{style.RESET_
+0000da10: 414c 4c7d 2729 0a20 2020 206c 6f67 6765  ALL}').    logge
+0000da20: 722e 696e 666f 286d 6573 7361 6765 290a  r.info(message).
+0000da30: 2020 2020 7769 7468 2072 6963 685f 7574      with rich_ut
+0000da40: 696c 732e 7361 6665 5f73 7461 7475 7328  ils.safe_status(
+0000da50: 6627 5b62 6f6c 6420 6379 616e 5d7b 6163  f'[bold cyan]{ac
+0000da60: 7469 6f6e 5f6d 6573 7361 6765 7d5b 2f5d  tion_message}[/]
+0000da70: 2729 3a0a 2020 2020 2020 2020 7375 6270  '):.        subp
+0000da80: 726f 6365 7373 5f75 7469 6c73 2e72 756e  rocess_utils.run
+0000da90: 5f69 6e5f 7061 7261 6c6c 656c 285f 7379  _in_parallel(_sy
+0000daa0: 6e63 5f6e 6f64 652c 2072 756e 6e65 7273  nc_node, runners
+0000dab0: 290a 0a0a 6465 6620 6368 6563 6b5f 6c6f  )...def check_lo
+0000dac0: 6361 6c5f 6770 7573 2829 202d 3e20 626f  cal_gpus() -> bo
+0000dad0: 6f6c 3a0a 2020 2020 2222 2243 6865 636b  ol:.    """Check
+0000dae0: 7320 6966 2047 5055 7320 6172 6520 6176  s if GPUs are av
+0000daf0: 6169 6c61 626c 6520 6c6f 6361 6c6c 792e  ailable locally.
+0000db00: 0a0a 2020 2020 5265 7475 726e 7320 7768  ..    Returns wh
+0000db10: 6574 6865 7220 4750 5573 2061 7265 2061  ether GPUs are a
+0000db20: 7661 696c 6162 6c65 206f 6e20 7468 6520  vailable on the 
+0000db30: 6c6f 6361 6c20 6d61 6368 696e 6520 6279  local machine by
+0000db40: 2063 6865 636b 696e 670a 2020 2020 6966   checking.    if
+0000db50: 206e 7669 6469 612d 736d 6920 6973 2069   nvidia-smi is i
+0000db60: 6e73 7461 6c6c 6564 2061 6e64 2072 6574  nstalled and ret
+0000db70: 7572 6e73 207a 6572 6f20 7265 7475 726e  urns zero return
+0000db80: 2063 6f64 652e 0a0a 2020 2020 5265 7475   code...    Retu
+0000db90: 726e 7320 5472 7565 2069 6620 6e76 6964  rns True if nvid
+0000dba0: 6961 2d73 6d69 2069 7320 696e 7374 616c  ia-smi is instal
+0000dbb0: 6c65 6420 616e 6420 7265 7475 726e 7320  led and returns 
+0000dbc0: 7a65 726f 2072 6574 7572 6e20 636f 6465  zero return code
+0000dbd0: 2c0a 2020 2020 4661 6c73 6520 6966 206e  ,.    False if n
+0000dbe0: 6f74 2e0a 2020 2020 2222 220a 2020 2020  ot..    """.    
+0000dbf0: 6973 5f66 756e 6374 696f 6e61 6c20 3d20  is_functional = 
+0000dc00: 4661 6c73 650a 2020 2020 696e 7374 616c  False.    instal
+0000dc10: 6c61 7469 6f6e 5f63 6865 636b 203d 2073  lation_check = s
+0000dc20: 7562 7072 6f63 6573 732e 7275 6e28 5b27  ubprocess.run(['
+0000dc30: 7768 6963 6827 2c20 276e 7669 6469 612d  which', 'nvidia-
+0000dc40: 736d 6927 5d2c 0a20 2020 2020 2020 2020  smi'],.         
+0000dc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc60: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000dc70: 7464 6f75 743d 7375 6270 726f 6365 7373  tdout=subprocess
+0000dc80: 2e44 4556 4e55 4c4c 2c0a 2020 2020 2020  .DEVNULL,.      
+0000dc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dcb0: 2020 7374 6465 7272 3d73 7562 7072 6f63    stderr=subproc
+0000dcc0: 6573 732e 4445 564e 554c 4c2c 0a20 2020  ess.DEVNULL,.   
+0000dcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dcf0: 2020 2020 2063 6865 636b 3d46 616c 7365       check=False
+0000dd00: 290a 2020 2020 6973 5f69 6e73 7461 6c6c  ).    is_install
+0000dd10: 6564 203d 2069 6e73 7461 6c6c 6174 696f  ed = installatio
+0000dd20: 6e5f 6368 6563 6b2e 7265 7475 726e 636f  n_check.returnco
+0000dd30: 6465 203d 3d20 300a 2020 2020 6966 2069  de == 0.    if i
+0000dd40: 735f 696e 7374 616c 6c65 643a 0a20 2020  s_installed:.   
+0000dd50: 2020 2020 2065 7865 6375 7469 6f6e 5f63       execution_c
+0000dd60: 6865 636b 203d 2073 7562 7072 6f63 6573  heck = subproces
+0000dd70: 732e 7275 6e28 5b27 6e76 6964 6961 2d73  s.run(['nvidia-s
+0000dd80: 6d69 275d 2c0a 2020 2020 2020 2020 2020  mi'],.          
+0000dd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dda0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000ddb0: 7464 6f75 743d 7375 6270 726f 6365 7373  tdout=subprocess
+0000ddc0: 2e44 4556 4e55 4c4c 2c0a 2020 2020 2020  .DEVNULL,.      
+0000ddd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ddf0: 2020 2073 7464 6572 723d 7375 6270 726f     stderr=subpro
+0000de00: 6365 7373 2e44 4556 4e55 4c4c 2c0a 2020  cess.DEVNULL,.  
+0000de10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de30: 2020 2020 2020 2063 6865 636b 3d46 616c         check=Fal
+0000de40: 7365 290a 2020 2020 2020 2020 6973 5f66  se).        is_f
+0000de50: 756e 6374 696f 6e61 6c20 3d20 6578 6563  unctional = exec
+0000de60: 7574 696f 6e5f 6368 6563 6b2e 7265 7475  ution_check.retu
+0000de70: 726e 636f 6465 203d 3d20 300a 2020 2020  rncode == 0.    
+0000de80: 7265 7475 726e 2069 735f 6675 6e63 7469  return is_functi
+0000de90: 6f6e 616c 0a0a 0a64 6566 2067 656e 6572  onal...def gener
+0000dea0: 6174 655f 636c 7573 7465 725f 6e61 6d65  ate_cluster_name
+0000deb0: 2829 3a0a 2020 2020 2320 544f 444f 3a20  ():.    # TODO: 
+0000dec0: 6368 616e 6765 2074 6869 7320 4944 2066  change this ID f
+0000ded0: 6f72 6d61 7474 696e 6720 746f 2073 6f6d  ormatting to som
+0000dee0: 6574 6869 6e67 206d 6f72 6520 706c 6561  ething more plea
+0000def0: 7361 6e74 2e0a 2020 2020 2320 5573 6572  sant..    # User
+0000df00: 206e 616d 6520 6973 2068 656c 7066 756c   name is helpful
+0000df10: 2069 6e20 6e6f 6e2d 6973 6f6c 6174 6564   in non-isolated
+0000df20: 2061 6363 6f75 6e74 732c 2065 2e67 2e2c   accounts, e.g.,
+0000df30: 2047 4350 2c20 417a 7572 652e 0a20 2020   GCP, Azure..   
+0000df40: 2072 6574 7572 6e20 6627 736b 792d 7b75   return f'sky-{u
+0000df50: 7569 642e 7575 6964 3428 292e 6865 785b  uid.uuid4().hex[
+0000df60: 3a34 5d7d 2d7b 636f 6d6d 6f6e 5f75 7469  :4]}-{common_uti
+0000df70: 6c73 2e67 6574 5f63 6c65 616e 6564 5f75  ls.get_cleaned_u
+0000df80: 7365 726e 616d 6528 297d 270a 0a0a 6465  sername()}'...de
+0000df90: 6620 5f71 7565 7279 5f68 6561 645f 6970  f _query_head_ip
+0000dfa0: 5f77 6974 685f 7265 7472 6965 7328 636c  _with_retries(cl
+0000dfb0: 7573 7465 725f 7961 6d6c 3a20 7374 722c  uster_yaml: str,
+0000dfc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dfe0: 206d 6178 5f61 7474 656d 7074 733a 2069   max_attempts: i
+0000dff0: 6e74 203d 2031 2920 2d3e 2073 7472 3a0a  nt = 1) -> str:.
+0000e000: 2020 2020 2222 2252 6574 7572 6e73 2074      """Returns t
+0000e010: 6865 2049 5020 6f66 2074 6865 2068 6561  he IP of the hea
+0000e020: 6420 6e6f 6465 2062 7920 7175 6572 7969  d node by queryi
+0000e030: 6e67 2074 6865 2063 6c6f 7564 2e0a 0a20  ng the cloud... 
+0000e040: 2020 2052 6169 7365 733a 0a20 2020 2020     Raises:.     
+0000e050: 2065 7863 6570 7469 6f6e 732e 4665 7463   exceptions.Fetc
+0000e060: 6843 6c75 7374 6572 496e 666f 4572 726f  hClusterInfoErro
+0000e070: 723a 2069 6620 7765 2066 6169 6c65 6420  r: if we failed 
+0000e080: 746f 2067 6574 2074 6865 2068 6561 6420  to get the head 
+0000e090: 4950 2e0a 2020 2020 2222 220a 2020 2020  IP..    """.    
+0000e0a0: 6261 636b 6f66 6620 3d20 636f 6d6d 6f6e  backoff = common
+0000e0b0: 5f75 7469 6c73 2e42 6163 6b6f 6666 2869  _utils.Backoff(i
+0000e0c0: 6e69 7469 616c 5f62 6163 6b6f 6666 3d35  nitial_backoff=5
+0000e0d0: 2c20 6d61 785f 6261 636b 6f66 665f 6661  , max_backoff_fa
+0000e0e0: 6374 6f72 3d35 290a 2020 2020 666f 7220  ctor=5).    for 
+0000e0f0: 6920 696e 2072 616e 6765 286d 6178 5f61  i in range(max_a
+0000e100: 7474 656d 7074 7329 3a0a 2020 2020 2020  ttempts):.      
+0000e110: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+0000e120: 2020 2066 756c 6c5f 636c 7573 7465 725f     full_cluster_
+0000e130: 7961 6d6c 203d 2073 7472 2870 6174 686c  yaml = str(pathl
+0000e140: 6962 2e50 6174 6828 636c 7573 7465 725f  ib.Path(cluster_
+0000e150: 7961 6d6c 292e 6578 7061 6e64 7573 6572  yaml).expanduser
+0000e160: 2829 290a 2020 2020 2020 2020 2020 2020  ()).            
+0000e170: 6f75 7420 3d20 7375 6270 726f 6365 7373  out = subprocess
+0000e180: 5f75 7469 6c73 2e72 756e 280a 2020 2020  _utils.run(.    
+0000e190: 2020 2020 2020 2020 2020 2020 6627 7261              f'ra
+0000e1a0: 7920 6765 742d 6865 6164 2d69 7020 7b66  y get-head-ip {f
+0000e1b0: 756c 6c5f 636c 7573 7465 725f 7961 6d6c  ull_cluster_yaml
+0000e1c0: 2172 7d27 2c0a 2020 2020 2020 2020 2020  !r}',.          
+0000e1d0: 2020 2020 2020 7374 646f 7574 3d73 7562        stdout=sub
+0000e1e0: 7072 6f63 6573 732e 5049 5045 2c0a 2020  process.PIPE,.  
+0000e1f0: 2020 2020 2020 2020 2020 2020 2020 7374                st
+0000e200: 6465 7272 3d73 7562 7072 6f63 6573 732e  derr=subprocess.
+0000e210: 4445 564e 554c 4c29 2e73 7464 6f75 742e  DEVNULL).stdout.
+0000e220: 6465 636f 6465 2829 2e73 7472 6970 2829  decode().strip()
+0000e230: 0a20 2020 2020 2020 2020 2020 2068 6561  .            hea
+0000e240: 645f 6970 5f6c 6973 7420 3d20 7265 2e66  d_ip_list = re.f
+0000e250: 696e 6461 6c6c 2849 505f 4144 4452 5f52  indall(IP_ADDR_R
+0000e260: 4547 4558 2c20 6f75 7429 0a20 2020 2020  EGEX, out).     
+0000e270: 2020 2020 2020 2069 6620 6c65 6e28 6865         if len(he
+0000e280: 6164 5f69 705f 6c69 7374 2920 3e20 313a  ad_ip_list) > 1:
+0000e290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e2a0: 2023 2054 6869 7320 636f 756c 6420 6265   # This could be
+0000e2b0: 2074 7269 6767 6572 6564 2069 6620 652e   triggered if e.
+0000e2c0: 672e 2c20 736f 6d65 206c 6f67 6769 6e67  g., some logging
+0000e2d0: 2069 7320 6164 6465 6420 696e 0a20 2020   is added in.   
+0000e2e0: 2020 2020 2020 2020 2020 2020 2023 2073               # s
+0000e2f0: 6b79 7069 6c6f 745f 636f 6e66 6967 2c20  kypilot_config, 
+0000e300: 6120 6d6f 6475 6c65 2074 6861 7420 6861  a module that ha
+0000e310: 7320 736f 6d65 2063 6f64 6520 6578 6563  s some code exec
+0000e320: 7574 6564 0a20 2020 2020 2020 2020 2020  uted.           
+0000e330: 2020 2020 2023 2077 6865 6e65 7665 7220       # whenever 
+0000e340: 6073 6b79 6020 6973 2069 6d70 6f72 7465  `sky` is importe
+0000e350: 642e 0a20 2020 2020 2020 2020 2020 2020  d..             
+0000e360: 2020 206c 6f67 6765 722e 7761 726e 696e     logger.warnin
+0000e370: 6728 0a20 2020 2020 2020 2020 2020 2020  g(.             
+0000e380: 2020 2020 2020 2027 4465 7465 6374 6564         'Detected
+0000e390: 206d 6f72 6520 7468 616e 2031 2049 5020   more than 1 IP 
+0000e3a0: 6672 6f6d 2074 6865 206f 7574 7075 7420  from the output 
+0000e3b0: 6f66 2027 0a20 2020 2020 2020 2020 2020  of '.           
+0000e3c0: 2020 2020 2020 2020 2027 7468 6520 6072           'the `r
+0000e3d0: 6179 2067 6574 2d68 6561 642d 6970 6020  ay get-head-ip` 
+0000e3e0: 636f 6d6d 616e 642e 2054 6869 7320 636f  command. This co
+0000e3f0: 756c 6420 270a 2020 2020 2020 2020 2020  uld '.          
+0000e400: 2020 2020 2020 2020 2020 2768 6170 7065            'happe
+0000e410: 6e20 6966 2074 6865 7265 2069 7320 6578  n if there is ex
+0000e420: 7472 6120 6f75 7470 7574 2066 726f 6d20  tra output from 
+0000e430: 6974 2c20 270a 2020 2020 2020 2020 2020  it, '.          
+0000e440: 2020 2020 2020 2020 2020 2777 6869 6368            'which
+0000e450: 2073 686f 756c 6420 6265 2069 6e73 7065   should be inspe
+0000e460: 6374 6564 2062 656c 6f77 2e5c 6e50 726f  cted below.\nPro
+0000e470: 6365 6564 696e 6720 7769 7468 2027 0a20  ceeding with '. 
+0000e480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e490: 2020 2066 2774 6865 206c 6173 7420 6465     f'the last de
+0000e4a0: 7465 6374 6564 2049 5020 287b 6865 6164  tected IP ({head
+0000e4b0: 5f69 705f 6c69 7374 5b2d 315d 7d29 2061  _ip_list[-1]}) a
+0000e4c0: 7320 6865 6164 2049 502e 270a 2020 2020  s head IP.'.    
+0000e4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4e0: 6627 5c6e 3d3d 204f 7574 7075 7420 3d3d  f'\n== Output ==
+0000e4f0: 5c6e 7b6f 7574 7d27 0a20 2020 2020 2020  \n{out}'.       
+0000e500: 2020 2020 2020 2020 2020 2020 2066 275c               f'\
+0000e510: 6e3d 3d20 4f75 7470 7574 2065 6e64 7320  n== Output ends 
+0000e520: 3d3d 2729 0a20 2020 2020 2020 2020 2020  ==').           
+0000e530: 2020 2020 2068 6561 645f 6970 5f6c 6973       head_ip_lis
+0000e540: 7420 3d20 6865 6164 5f69 705f 6c69 7374  t = head_ip_list
+0000e550: 5b2d 313a 5d0a 2020 2020 2020 2020 2020  [-1:].          
+0000e560: 2020 6173 7365 7274 2031 203d 3d20 6c65    assert 1 == le
+0000e570: 6e28 6865 6164 5f69 705f 6c69 7374 292c  n(head_ip_list),
+0000e580: 2028 6f75 742c 2068 6561 645f 6970 5f6c   (out, head_ip_l
+0000e590: 6973 7429 0a20 2020 2020 2020 2020 2020  ist).           
+0000e5a0: 2068 6561 645f 6970 203d 2068 6561 645f   head_ip = head_
+0000e5b0: 6970 5f6c 6973 745b 305d 0a20 2020 2020  ip_list[0].     
+0000e5c0: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
+0000e5d0: 2020 2020 2065 7863 6570 7420 7375 6270       except subp
+0000e5e0: 726f 6365 7373 2e43 616c 6c65 6450 726f  rocess.CalledPro
+0000e5f0: 6365 7373 4572 726f 7220 6173 2065 3a0a  cessError as e:.
+0000e600: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+0000e610: 203d 3d20 6d61 785f 6174 7465 6d70 7473   == max_attempts
+0000e620: 202d 2031 3a0a 2020 2020 2020 2020 2020   - 1:.          
+0000e630: 2020 2020 2020 7261 6973 6520 6578 6365        raise exce
+0000e640: 7074 696f 6e73 2e46 6574 6368 436c 7573  ptions.FetchClus
+0000e650: 7465 7249 6e66 6f45 7272 6f72 280a 2020  terInfoError(.  
+0000e660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e670: 2020 7265 6173 6f6e 3d65 7863 6570 7469    reason=excepti
+0000e680: 6f6e 732e 4665 7463 6843 6c75 7374 6572  ons.FetchCluster
+0000e690: 496e 666f 4572 726f 722e 5265 6173 6f6e  InfoError.Reason
+0000e6a0: 2e48 4541 4429 2066 726f 6d20 650a 2020  .HEAD) from e.  
+0000e6b0: 2020 2020 2020 2020 2020 2320 5265 7472            # Retr
+0000e6c0: 7920 6966 2074 6865 2063 6c75 7374 6572  y if the cluster
+0000e6d0: 2069 7320 6e6f 7420 7570 2079 6574 2e0a   is not up yet..
+0000e6e0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+0000e6f0: 6572 2e64 6562 7567 2827 5265 7472 7969  er.debug('Retryi
+0000e700: 6e67 2074 6f20 6765 7420 6865 6164 2069  ng to get head i
+0000e710: 702e 2729 0a20 2020 2020 2020 2020 2020  p.').           
+0000e720: 2074 696d 652e 736c 6565 7028 6261 636b   time.sleep(back
+0000e730: 6f66 662e 6375 7272 656e 745f 6261 636b  off.current_back
+0000e740: 6f66 6628 2929 0a20 2020 2072 6574 7572  off()).    retur
+0000e750: 6e20 6865 6164 5f69 700a 0a0a 4074 696d  n head_ip...@tim
+0000e760: 656c 696e 652e 6576 656e 740a 6465 6620  eline.event.def 
+0000e770: 6765 745f 6e6f 6465 5f69 7073 2863 6c75  get_node_ips(clu
+0000e780: 7374 6572 5f79 616d 6c3a 2073 7472 2c0a  ster_yaml: str,.
+0000e790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e7a0: 2065 7870 6563 7465 645f 6e75 6d5f 6e6f   expected_num_no
+0000e7b0: 6465 733a 2069 6e74 2c0a 2020 2020 2020  des: int,.      
+0000e7c0: 2020 2020 2020 2020 2020 2068 6561 645f             head_
+0000e7d0: 6970 5f6d 6178 5f61 7474 656d 7074 733a  ip_max_attempts:
+0000e7e0: 2069 6e74 203d 2031 2c0a 2020 2020 2020   int = 1,.      
+0000e7f0: 2020 2020 2020 2020 2020 2077 6f72 6b65             worke
+0000e800: 725f 6970 5f6d 6178 5f61 7474 656d 7074  r_ip_max_attempt
+0000e810: 733a 2069 6e74 203d 2031 2c0a 2020 2020  s: int = 1,.    
+0000e820: 2020 2020 2020 2020 2020 2020 2067 6574               get
+0000e830: 5f69 6e74 6572 6e61 6c5f 6970 733a 2062  _internal_ips: b
+0000e840: 6f6f 6c20 3d20 4661 6c73 6529 202d 3e20  ool = False) -> 
+0000e850: 4c69 7374 5b73 7472 5d3a 0a20 2020 2022  List[str]:.    "
+0000e860: 2222 5265 7475 726e 7320 7468 6520 4950  ""Returns the IP
+0000e870: 7320 6f66 2061 6c6c 206e 6f64 6573 2069  s of all nodes i
+0000e880: 6e20 7468 6520 636c 7573 7465 722c 2077  n the cluster, w
+0000e890: 6974 6820 6865 6164 206e 6f64 6520 6174  ith head node at
+0000e8a0: 2066 726f 6e74 2e0a 0a20 2020 2041 7267   front...    Arg
+0000e8b0: 733a 0a20 2020 2020 2020 2063 6c75 7374  s:.        clust
+0000e8c0: 6572 5f79 616d 6c3a 2050 6174 6820 746f  er_yaml: Path to
+0000e8d0: 2074 6865 2063 6c75 7374 6572 2079 616d   the cluster yam
+0000e8e0: 6c2e 0a20 2020 2020 2020 2065 7870 6563  l..        expec
+0000e8f0: 7465 645f 6e75 6d5f 6e6f 6465 733a 2045  ted_num_nodes: E
+0000e900: 7870 6563 7465 6420 6e75 6d62 6572 206f  xpected number o
+0000e910: 6620 6e6f 6465 7320 696e 2074 6865 2063  f nodes in the c
+0000e920: 6c75 7374 6572 2e0a 2020 2020 2020 2020  luster..        
+0000e930: 6865 6164 5f69 705f 6d61 785f 6174 7465  head_ip_max_atte
+0000e940: 6d70 7473 3a20 4d61 7820 6174 7465 6d70  mpts: Max attemp
+0000e950: 7473 2074 6f20 6765 7420 6865 6164 2069  ts to get head i
+0000e960: 702e 0a20 2020 2020 2020 2077 6f72 6b65  p..        worke
+0000e970: 725f 6970 5f6d 6178 5f61 7474 656d 7074  r_ip_max_attempt
+0000e980: 733a 204d 6178 2061 7474 656d 7074 7320  s: Max attempts 
+0000e990: 746f 2067 6574 2077 6f72 6b65 7220 6970  to get worker ip
+0000e9a0: 732e 0a20 2020 2020 2020 2067 6574 5f69  s..        get_i
+0000e9b0: 6e74 6572 6e61 6c5f 6970 733a 2057 6865  nternal_ips: Whe
+0000e9c0: 7468 6572 2074 6f20 6765 7420 696e 7465  ther to get inte
+0000e9d0: 726e 616c 2049 5073 2e20 5768 656e 2046  rnal IPs. When F
+0000e9e0: 616c 7365 2c20 6974 2069 7320 7374 696c  alse, it is stil
+0000e9f0: 6c0a 2020 2020 2020 2020 2020 2020 706f  l.            po
+0000ea00: 7373 6962 6c65 2074 6f20 6765 7420 696e  ssible to get in
+0000ea10: 7465 726e 616c 2049 5073 2069 6620 7468  ternal IPs if th
+0000ea20: 6520 636c 7573 7465 7220 646f 6573 206e  e cluster does n
+0000ea30: 6f74 2068 6176 6520 6578 7465 726e 616c  ot have external
+0000ea40: 0a20 2020 2020 2020 2020 2020 2049 5073  .            IPs
+0000ea50: 2e0a 0a20 2020 2052 6169 7365 733a 0a20  ...    Raises:. 
+0000ea60: 2020 2020 2020 2065 7863 6570 7469 6f6e         exception
+0000ea70: 732e 4665 7463 6843 6c75 7374 6572 496e  s.FetchClusterIn
+0000ea80: 666f 4572 726f 723a 2069 6620 7765 2066  foError: if we f
+0000ea90: 6169 6c65 6420 746f 2067 6574 2074 6865  ailed to get the
+0000eaa0: 2049 5073 2e20 652e 7265 6173 6f6e 2069   IPs. e.reason i
+0000eab0: 730a 2020 2020 2020 2020 2020 2020 4845  s.            HE
+0000eac0: 4144 206f 7220 574f 524b 4552 2e0a 2020  AD or WORKER..  
+0000ead0: 2020 2222 220a 2020 2020 7261 795f 636f    """.    ray_co
+0000eae0: 6e66 6967 203d 2063 6f6d 6d6f 6e5f 7574  nfig = common_ut
+0000eaf0: 696c 732e 7265 6164 5f79 616d 6c28 636c  ils.read_yaml(cl
+0000eb00: 7573 7465 725f 7961 6d6c 290a 2020 2020  uster_yaml).    
+0000eb10: 2320 5573 6520 7468 6520 6e65 7720 7072  # Use the new pr
+0000eb20: 6f76 6973 696f 6e65 7220 666f 7220 4157  ovisioner for AW
+0000eb30: 532e 0a20 2020 2070 726f 7669 6465 725f  S..    provider_
+0000eb40: 6e61 6d65 203d 2063 6c75 7374 6572 5f79  name = cluster_y
+0000eb50: 616d 6c5f 7574 696c 732e 6765 745f 7072  aml_utils.get_pr
+0000eb60: 6f76 6964 6572 5f6e 616d 6528 7261 795f  ovider_name(ray_
+0000eb70: 636f 6e66 6967 290a 2020 2020 636c 6f75  config).    clou
+0000eb80: 6420 3d20 636c 6f75 645f 7265 6769 7374  d = cloud_regist
+0000eb90: 7279 2e43 4c4f 5544 5f52 4547 4953 5452  ry.CLOUD_REGISTR
+0000eba0: 592e 6672 6f6d 5f73 7472 2870 726f 7669  Y.from_str(provi
+0000ebb0: 6465 725f 6e61 6d65 290a 2020 2020 6173  der_name).    as
+0000ebc0: 7365 7274 2063 6c6f 7564 2069 7320 6e6f  sert cloud is no
+0000ebd0: 7420 4e6f 6e65 2c20 7072 6f76 6964 6572  t None, provider
+0000ebe0: 5f6e 616d 650a 0a20 2020 2069 6620 636c  _name..    if cl
+0000ebf0: 6f75 642e 5052 4f56 4953 494f 4e45 525f  oud.PROVISIONER_
+0000ec00: 5645 5253 494f 4e20 3e3d 2063 6c6f 7564  VERSION >= cloud
+0000ec10: 732e 5072 6f76 6973 696f 6e65 7256 6572  s.ProvisionerVer
+0000ec20: 7369 6f6e 2e53 4b59 5049 4c4f 543a 0a20  sion.SKYPILOT:. 
+0000ec30: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+0000ec40: 2020 2020 2020 2020 6d65 7461 6461 7461          metadata
+0000ec50: 203d 2070 726f 7669 7369 6f6e 5f6c 6962   = provision_lib
+0000ec60: 2e67 6574 5f63 6c75 7374 6572 5f69 6e66  .get_cluster_inf
+0000ec70: 6f28 0a20 2020 2020 2020 2020 2020 2020  o(.             
+0000ec80: 2020 2070 726f 7669 6465 725f 6e61 6d65     provider_name
+0000ec90: 2c20 7261 795f 636f 6e66 6967 5b27 7072  , ray_config['pr
+0000eca0: 6f76 6964 6572 275d 2e67 6574 2827 7265  ovider'].get('re
+0000ecb0: 6769 6f6e 2729 2c0a 2020 2020 2020 2020  gion'),.        
+0000ecc0: 2020 2020 2020 2020 7261 795f 636f 6e66          ray_conf
+0000ecd0: 6967 5b27 636c 7573 7465 725f 6e61 6d65  ig['cluster_name
+0000ece0: 275d 2c20 7261 795f 636f 6e66 6967 5b27  '], ray_config['
+0000ecf0: 7072 6f76 6964 6572 275d 290a 2020 2020  provider']).    
+0000ed00: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
+0000ed10: 7469 6f6e 2061 7320 653a 2020 2320 7079  tion as e:  # py
+0000ed20: 6c69 6e74 3a20 6469 7361 626c 653d 6272  lint: disable=br
+0000ed30: 6f61 642d 6578 6365 7074 0a20 2020 2020  oad-except.     
+0000ed40: 2020 2020 2020 2023 2054 6869 7320 636f         # This co
+0000ed50: 756c 6420 6861 7070 656e 2077 6865 6e20  uld happen when 
+0000ed60: 7468 6520 564d 2069 7320 6e6f 7420 6675  the VM is not fu
+0000ed70: 6c6c 7920 6c61 756e 6368 6564 2c20 616e  lly launched, an
+0000ed80: 6420 6120 7573 6572 0a20 2020 2020 2020  d a user.       
+0000ed90: 2020 2020 2023 2069 7320 7472 7969 6e67       # is trying
+0000eda0: 2074 6f20 7465 726d 696e 6174 6520 6974   to terminate it
+0000edb0: 2077 6974 6820 6073 6b79 2064 6f77 6e60   with `sky down`
+0000edc0: 2e0a 2020 2020 2020 2020 2020 2020 6c6f  ..            lo
+0000edd0: 6767 6572 2e64 6562 7567 280a 2020 2020  gger.debug(.    
+0000ede0: 2020 2020 2020 2020 2020 2020 2746 6169              'Fai
+0000edf0: 6c65 6420 746f 2067 6574 2063 6c75 7374  led to get clust
+0000ee00: 6572 2069 6e66 6f20 666f 7220 270a 2020  er info for '.  
+0000ee10: 2020 2020 2020 2020 2020 2020 2020 6627                f'
+0000ee20: 7b72 6179 5f63 6f6e 6669 675b 2263 6c75  {ray_config["clu
+0000ee30: 7374 6572 5f6e 616d 6522 5d7d 2066 726f  ster_name"]} fro
+0000ee40: 6d20 7468 6520 6e65 7720 7072 6f76 6973  m the new provis
+0000ee50: 696f 6e65 7220 270a 2020 2020 2020 2020  ioner '.        
+0000ee60: 2020 2020 2020 2020 6627 7769 7468 207b          f'with {
+0000ee70: 636f 6d6d 6f6e 5f75 7469 6c73 2e66 6f72  common_utils.for
+0000ee80: 6d61 745f 6578 6365 7074 696f 6e28 6529  mat_exception(e)
+0000ee90: 7d2e 2729 0a20 2020 2020 2020 2020 2020  }.').           
+0000eea0: 2072 6169 7365 2065 7863 6570 7469 6f6e   raise exception
+0000eeb0: 732e 4665 7463 6843 6c75 7374 6572 496e  s.FetchClusterIn
+0000eec0: 666f 4572 726f 7228 0a20 2020 2020 2020  foError(.       
+0000eed0: 2020 2020 2020 2020 2065 7863 6570 7469           excepti
+0000eee0: 6f6e 732e 4665 7463 6843 6c75 7374 6572  ons.FetchCluster
+0000eef0: 496e 666f 4572 726f 722e 5265 6173 6f6e  InfoError.Reason
+0000ef00: 2e48 4541 4429 2066 726f 6d20 650a 2020  .HEAD) from e.  
+0000ef10: 2020 2020 2020 6966 206c 656e 286d 6574        if len(met
+0000ef20: 6164 6174 612e 696e 7374 616e 6365 7329  adata.instances)
+0000ef30: 203c 2065 7870 6563 7465 645f 6e75 6d5f   < expected_num_
+0000ef40: 6e6f 6465 733a 0a20 2020 2020 2020 2020  nodes:.         
+0000ef50: 2020 2023 2053 696d 756c 6174 6520 7468     # Simulate th
+0000ef60: 6520 6578 6365 7074 696f 6e20 7768 656e  e exception when
+0000ef70: 2052 6179 2068 6561 6420 6e6f 6465 2069   Ray head node i
+0000ef80: 7320 6e6f 7420 7570 2e0a 2020 2020 2020  s not up..      
+0000ef90: 2020 2020 2020 7261 6973 6520 6578 6365        raise exce
+0000efa0: 7074 696f 6e73 2e46 6574 6368 436c 7573  ptions.FetchClus
+0000efb0: 7465 7249 6e66 6f45 7272 6f72 280a 2020  terInfoError(.  
+0000efc0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+0000efd0: 6365 7074 696f 6e73 2e46 6574 6368 436c  ceptions.FetchCl
+0000efe0: 7573 7465 7249 6e66 6f45 7272 6f72 2e52  usterInfoError.R
+0000eff0: 6561 736f 6e2e 4845 4144 290a 2020 2020  eason.HEAD).    
+0000f000: 2020 2020 7265 7475 726e 206d 6574 6164      return metad
+0000f010: 6174 612e 6765 745f 6665 6173 6962 6c65  ata.get_feasible
+0000f020: 5f69 7073 2867 6574 5f69 6e74 6572 6e61  _ips(get_interna
+0000f030: 6c5f 6970 7329 0a0a 2020 2020 6966 2067  l_ips)..    if g
+0000f040: 6574 5f69 6e74 6572 6e61 6c5f 6970 733a  et_internal_ips:
+0000f050: 0a20 2020 2020 2020 2077 6974 6820 7465  .        with te
+0000f060: 6d70 6669 6c65 2e4e 616d 6564 5465 6d70  mpfile.NamedTemp
+0000f070: 6f72 6172 7946 696c 6528 6d6f 6465 3d27  oraryFile(mode='
+0000f080: 7727 2c20 6465 6c65 7465 3d46 616c 7365  w', delete=False
+0000f090: 2920 6173 2066 3a0a 2020 2020 2020 2020  ) as f:.        
+0000f0a0: 2020 2020 7261 795f 636f 6e66 6967 5b27      ray_config['
+0000f0b0: 7072 6f76 6964 6572 275d 5b27 7573 655f  provider']['use_
+0000f0c0: 696e 7465 726e 616c 5f69 7073 275d 203d  internal_ips'] =
+0000f0d0: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
+0000f0e0: 2020 7961 6d6c 2e64 756d 7028 7261 795f    yaml.dump(ray_
+0000f0f0: 636f 6e66 6967 2c20 6629 0a20 2020 2020  config, f).     
+0000f100: 2020 2020 2020 2063 6c75 7374 6572 5f79         cluster_y
+0000f110: 616d 6c20 3d20 662e 6e61 6d65 0a0a 2020  aml = f.name..  
+0000f120: 2020 2320 4368 6563 6b20 7468 6520 6e65    # Check the ne
+0000f130: 7477 6f72 6b20 636f 6e6e 6563 7469 6f6e  twork connection
+0000f140: 2066 6972 7374 2074 6f20 6176 6f69 6420   first to avoid 
+0000f150: 6c6f 6e67 2068 616e 6769 6e67 2074 696d  long hanging tim
+0000f160: 6520 666f 720a 2020 2020 2320 7261 7920  e for.    # ray 
+0000f170: 6765 742d 6865 6164 2d69 7020 6265 6c6f  get-head-ip belo
+0000f180: 772c 2069 6620 6120 6c6f 6e67 2d6c 6173  w, if a long-las
+0000f190: 7469 6e67 206e 6574 776f 726b 2063 6f6e  ting network con
+0000f1a0: 6e65 6374 696f 6e20 6661 696c 7572 650a  nection failure.
+0000f1b0: 2020 2020 2320 6861 7070 656e 732e 0a20      # happens.. 
+0000f1c0: 2020 2063 6865 636b 5f6e 6574 776f 726b     check_network
+0000f1d0: 5f63 6f6e 6e65 6374 696f 6e28 290a 2020  _connection().  
+0000f1e0: 2020 6865 6164 5f69 7020 3d20 5f71 7565    head_ip = _que
+0000f1f0: 7279 5f68 6561 645f 6970 5f77 6974 685f  ry_head_ip_with_
+0000f200: 7265 7472 6965 7328 636c 7573 7465 725f  retries(cluster_
+0000f210: 7961 6d6c 2c0a 2020 2020 2020 2020 2020  yaml,.          
+0000f220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f240: 6d61 785f 6174 7465 6d70 7473 3d68 6561  max_attempts=hea
+0000f250: 645f 6970 5f6d 6178 5f61 7474 656d 7074  d_ip_max_attempt
+0000f260: 7329 0a20 2020 2068 6561 645f 6970 5f6c  s).    head_ip_l
+0000f270: 6973 7420 3d20 5b68 6561 645f 6970 5d0a  ist = [head_ip].
+0000f280: 2020 2020 6966 2065 7870 6563 7465 645f      if expected_
+0000f290: 6e75 6d5f 6e6f 6465 7320 3e20 313a 0a20  num_nodes > 1:. 
+0000f2a0: 2020 2020 2020 2062 6163 6b6f 6666 203d         backoff =
+0000f2b0: 2063 6f6d 6d6f 6e5f 7574 696c 732e 4261   common_utils.Ba
+0000f2c0: 636b 6f66 6628 696e 6974 6961 6c5f 6261  ckoff(initial_ba
+0000f2d0: 636b 6f66 663d 352c 206d 6178 5f62 6163  ckoff=5, max_bac
+0000f2e0: 6b6f 6666 5f66 6163 746f 723d 3529 0a0a  koff_factor=5)..
+0000f2f0: 2020 2020 2020 2020 666f 7220 7265 7472          for retr
+0000f300: 795f 636e 7420 696e 2072 616e 6765 2877  y_cnt in range(w
+0000f310: 6f72 6b65 725f 6970 5f6d 6178 5f61 7474  orker_ip_max_att
+0000f320: 656d 7074 7329 3a0a 2020 2020 2020 2020  empts):.        
+0000f330: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+0000f340: 2020 2020 2020 2020 2066 756c 6c5f 636c           full_cl
+0000f350: 7573 7465 725f 7961 6d6c 203d 2073 7472  uster_yaml = str
+0000f360: 2870 6174 686c 6962 2e50 6174 6828 636c  (pathlib.Path(cl
+0000f370: 7573 7465 725f 7961 6d6c 292e 6578 7061  uster_yaml).expa
+0000f380: 6e64 7573 6572 2829 290a 2020 2020 2020  nduser()).      
+0000f390: 2020 2020 2020 2020 2020 7072 6f63 203d            proc =
+0000f3a0: 2073 7562 7072 6f63 6573 735f 7574 696c   subprocess_util
+0000f3b0: 732e 7275 6e28 0a20 2020 2020 2020 2020  s.run(.         
+0000f3c0: 2020 2020 2020 2020 2020 2066 2772 6179             f'ray
+0000f3d0: 2067 6574 2d77 6f72 6b65 722d 6970 7320   get-worker-ips 
+0000f3e0: 7b66 756c 6c5f 636c 7573 7465 725f 7961  {full_cluster_ya
+0000f3f0: 6d6c 2172 7d27 2c0a 2020 2020 2020 2020  ml!r}',.        
+0000f400: 2020 2020 2020 2020 2020 2020 7374 646f              stdo
+0000f410: 7574 3d73 7562 7072 6f63 6573 732e 5049  ut=subprocess.PI
+0000f420: 5045 2c0a 2020 2020 2020 2020 2020 2020  PE,.            
+0000f430: 2020 2020 2020 2020 7374 6465 7272 3d73          stderr=s
+0000f440: 7562 7072 6f63 6573 732e 5049 5045 290a  ubprocess.PIPE).
+0000f450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f460: 6f75 7420 3d20 7072 6f63 2e73 7464 6f75  out = proc.stdou
+0000f470: 742e 6465 636f 6465 2829 0a20 2020 2020  t.decode().     
+0000f480: 2020 2020 2020 2020 2020 2062 7265 616b             break
+0000f490: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
+0000f4a0: 6570 7420 7375 6270 726f 6365 7373 2e43  ept subprocess.C
+0000f4b0: 616c 6c65 6450 726f 6365 7373 4572 726f  alledProcessErro
+0000f4c0: 7220 6173 2065 3a0a 2020 2020 2020 2020  r as e:.        
+0000f4d0: 2020 2020 2020 2020 6966 2072 6574 7279          if retry
+0000f4e0: 5f63 6e74 203d 3d20 776f 726b 6572 5f69  _cnt == worker_i
+0000f4f0: 705f 6d61 785f 6174 7465 6d70 7473 202d  p_max_attempts -
+0000f500: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
+0000f510: 2020 2020 2020 2020 7261 6973 6520 6578          raise ex
+0000f520: 6365 7074 696f 6e73 2e46 6574 6368 436c  ceptions.FetchCl
+0000f530: 7573 7465 7249 6e66 6f45 7272 6f72 280a  usterInfoError(.
+0000f540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f550: 2020 2020 2020 2020 6578 6365 7074 696f          exceptio
+0000f560: 6e73 2e46 6574 6368 436c 7573 7465 7249  ns.FetchClusterI
+0000f570: 6e66 6f45 7272 6f72 2e52 6561 736f 6e2e  nfoError.Reason.
+0000f580: 574f 524b 4552 2920 6672 6f6d 2065 0a20  WORKER) from e. 
+0000f590: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000f5a0: 2052 6574 7279 2069 6620 7468 6520 7373   Retry if the ss
+0000f5b0: 6820 6973 206e 6f74 2072 6561 6479 2066  h is not ready f
+0000f5c0: 6f72 2074 6865 2077 6f72 6b65 7273 2079  or the workers y
+0000f5d0: 6574 2e0a 2020 2020 2020 2020 2020 2020  et..            
+0000f5e0: 2020 2020 6261 636b 6f66 665f 7469 6d65      backoff_time
+0000f5f0: 203d 2062 6163 6b6f 6666 2e63 7572 7265   = backoff.curre
+0000f600: 6e74 5f62 6163 6b6f 6666 2829 0a20 2020  nt_backoff().   
+0000f610: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+0000f620: 6765 722e 6465 6275 6728 2752 6574 7279  ger.debug('Retry
+0000f630: 696e 6720 746f 2067 6574 2077 6f72 6b65  ing to get worke
+0000f640: 7220 6970 2027 0a20 2020 2020 2020 2020  r ip '.         
+0000f650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f660: 2020 2020 6627 5b7b 7265 7472 795f 636e      f'[{retry_cn
+0000f670: 747d 2f7b 776f 726b 6572 5f69 705f 6d61  t}/{worker_ip_ma
+0000f680: 785f 6174 7465 6d70 7473 7d5d 2069 6e20  x_attempts}] in 
+0000f690: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+0000f6a0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000f6b0: 277b 6261 636b 6f66 665f 7469 6d65 7d20  '{backoff_time} 
+0000f6c0: 7365 636f 6e64 732e 2729 0a20 2020 2020  seconds.').     
+0000f6d0: 2020 2020 2020 2020 2020 2074 696d 652e             time.
+0000f6e0: 736c 6565 7028 6261 636b 6f66 665f 7469  sleep(backoff_ti
+0000f6f0: 6d65 290a 2020 2020 2020 2020 776f 726b  me).        work
+0000f700: 6572 5f69 7073 203d 2072 652e 6669 6e64  er_ips = re.find
+0000f710: 616c 6c28 4950 5f41 4444 525f 5245 4745  all(IP_ADDR_REGE
+0000f720: 582c 206f 7574 290a 2020 2020 2020 2020  X, out).        
+0000f730: 6966 206c 656e 2877 6f72 6b65 725f 6970  if len(worker_ip
+0000f740: 7329 2021 3d20 6578 7065 6374 6564 5f6e  s) != expected_n
+0000f750: 756d 5f6e 6f64 6573 202d 2031 3a0a 2020  um_nodes - 1:.  
+0000f760: 2020 2020 2020 2020 2020 6e20 3d20 6578            n = ex
+0000f770: 7065 6374 6564 5f6e 756d 5f6e 6f64 6573  pected_num_nodes
+0000f780: 202d 2031 0a20 2020 2020 2020 2020 2020   - 1.           
+0000f790: 2069 6620 6c65 6e28 776f 726b 6572 5f69   if len(worker_i
+0000f7a0: 7073 2920 3e20 6e3a 0a20 2020 2020 2020  ps) > n:.       
+0000f7b0: 2020 2020 2020 2020 2023 2054 6869 7320           # This 
+0000f7c0: 636f 756c 6420 6265 2074 7269 6767 6572  could be trigger
+0000f7d0: 6564 2069 6620 652e 672e 2c20 736f 6d65  ed if e.g., some
+0000f7e0: 206c 6f67 6769 6e67 2069 7320 6164 6465   logging is adde
+0000f7f0: 6420 696e 0a20 2020 2020 2020 2020 2020  d in.           
+0000f800: 2020 2020 2023 2073 6b79 7069 6c6f 745f       # skypilot_
+0000f810: 636f 6e66 6967 2c20 6120 6d6f 6475 6c65  config, a module
+0000f820: 2074 6861 7420 6861 7320 736f 6d65 2063   that has some c
+0000f830: 6f64 6520 6578 6563 7574 6564 2077 6865  ode executed whe
+0000f840: 6e65 7665 720a 2020 2020 2020 2020 2020  never.          
+0000f850: 2020 2020 2020 2320 6073 6b79 6020 6973        # `sky` is
+0000f860: 2069 6d70 6f72 7465 642e 0a20 2020 2020   imported..     
+0000f870: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+0000f880: 722e 7761 726e 696e 6728 0a20 2020 2020  r.warning(.     
+0000f890: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000f8a0: 2745 7870 6563 7465 6420 7b6e 7d20 776f  'Expected {n} wo
+0000f8b0: 726b 6572 2049 5028 7329 3b20 666f 756e  rker IP(s); foun
+0000f8c0: 6420 270a 2020 2020 2020 2020 2020 2020  d '.            
+0000f8d0: 2020 2020 2020 2020 6627 7b6c 656e 2877          f'{len(w
+0000f8e0: 6f72 6b65 725f 6970 7329 7d3a 207b 776f  orker_ips)}: {wo
+0000f8f0: 726b 6572 5f69 7073 7d27 0a20 2020 2020  rker_ips}'.     
+0000f900: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0000f910: 5c6e 5468 6973 2063 6f75 6c64 2068 6170  \nThis could hap
+0000f920: 7065 6e20 6966 2074 6865 7265 2069 7320  pen if there is 
+0000f930: 6578 7472 6120 6f75 7470 7574 2066 726f  extra output fro
+0000f940: 6d20 270a 2020 2020 2020 2020 2020 2020  m '.            
+0000f950: 2020 2020 2020 2020 2760 7261 7920 6765          '`ray ge
+0000f960: 742d 776f 726b 6572 2d69 7073 602c 2077  t-worker-ips`, w
+0000f970: 6869 6368 2073 686f 756c 6420 6265 2069  hich should be i
+0000f980: 6e73 7065 6374 6564 2062 656c 6f77 2e27  nspected below.'
+0000f990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f9a0: 2020 2020 2066 275c 6e3d 3d20 4f75 7470       f'\n== Outp
+0000f9b0: 7574 203d 3d5c 6e7b 6f75 747d 270a 2020  ut ==\n{out}'.  
+0000f9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f9d0: 2020 6627 5c6e 3d3d 204f 7574 7075 7420    f'\n== Output 
+0000f9e0: 656e 6473 203d 3d27 290a 2020 2020 2020  ends ==').      
+0000f9f0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+0000fa00: 2e77 6172 6e69 6e67 2866 275c 6e50 726f  .warning(f'\nPro
+0000fa10: 6365 6564 696e 6720 7769 7468 2074 6865  ceeding with the
+0000fa20: 206c 6173 7420 7b6e 7d20 270a 2020 2020   last {n} '.    
+0000fa30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa40: 2020 2020 2020 2020 2020 2066 2764 6574             f'det
+0000fa50: 6563 7465 6420 4950 2873 293a 207b 776f  ected IP(s): {wo
+0000fa60: 726b 6572 5f69 7073 5b2d 6e3a 5d7d 2e27  rker_ips[-n:]}.'
+0000fa70: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000fa80: 2020 776f 726b 6572 5f69 7073 203d 2077    worker_ips = w
+0000fa90: 6f72 6b65 725f 6970 735b 2d6e 3a5d 0a20  orker_ips[-n:]. 
+0000faa0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000fab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fac0: 2072 6169 7365 2065 7863 6570 7469 6f6e   raise exception
+0000fad0: 732e 4665 7463 6843 6c75 7374 6572 496e  s.FetchClusterIn
+0000fae0: 666f 4572 726f 7228 0a20 2020 2020 2020  foError(.       
+0000faf0: 2020 2020 2020 2020 2020 2020 2065 7863               exc
+0000fb00: 6570 7469 6f6e 732e 4665 7463 6843 6c75  eptions.FetchClu
+0000fb10: 7374 6572 496e 666f 4572 726f 722e 5265  sterInfoError.Re
+0000fb20: 6173 6f6e 2e57 4f52 4b45 5229 0a20 2020  ason.WORKER).   
+0000fb30: 2065 6c73 653a 0a20 2020 2020 2020 2077   else:.        w
+0000fb40: 6f72 6b65 725f 6970 7320 3d20 5b5d 0a20  orker_ips = []. 
+0000fb50: 2020 2072 6574 7572 6e20 6865 6164 5f69     return head_i
+0000fb60: 705f 6c69 7374 202b 2077 6f72 6b65 725f  p_list + worker_
+0000fb70: 6970 730a 0a0a 6465 6620 6368 6563 6b5f  ips...def check_
+0000fb80: 6e65 7477 6f72 6b5f 636f 6e6e 6563 7469  network_connecti
+0000fb90: 6f6e 2829 3a0a 2020 2020 2320 546f 6c65  on():.    # Tole
+0000fba0: 7261 7465 2033 2072 6574 7269 6573 2061  rate 3 retries a
+0000fbb0: 7320 6974 2069 7320 6f62 7365 7276 6564  s it is observed
+0000fbc0: 2074 6861 7420 636f 6e6e 6563 7469 6f6e   that connection
+0000fbd0: 7320 6361 6e20 6661 696c 2e0a 2020 2020  s can fail..    
+0000fbe0: 6164 6170 7465 7220 3d20 6164 6170 7465  adapter = adapte
+0000fbf0: 7273 2e48 5454 5041 6461 7074 6572 286d  rs.HTTPAdapter(m
+0000fc00: 6178 5f72 6574 7269 6573 3d72 6574 7279  ax_retries=retry
+0000fc10: 5f6c 6962 2e52 6574 7279 2874 6f74 616c  _lib.Retry(total
+0000fc20: 3d33 2929 0a20 2020 2068 7474 7020 3d20  =3)).    http = 
+0000fc30: 7265 7175 6573 7473 2e53 6573 7369 6f6e  requests.Session
+0000fc40: 2829 0a20 2020 2068 7474 702e 6d6f 756e  ().    http.moun
+0000fc50: 7428 2768 7474 7073 3a2f 2f27 2c20 6164  t('https://', ad
+0000fc60: 6170 7465 7229 0a20 2020 2068 7474 702e  apter).    http.
+0000fc70: 6d6f 756e 7428 2768 7474 703a 2f2f 272c  mount('http://',
+0000fc80: 2061 6461 7074 6572 290a 2020 2020 666f   adapter).    fo
+0000fc90: 7220 692c 2069 7020 696e 2065 6e75 6d65  r i, ip in enume
+0000fca0: 7261 7465 285f 5445 5354 5f49 505f 4c49  rate(_TEST_IP_LI
+0000fcb0: 5354 293a 0a20 2020 2020 2020 2074 7279  ST):.        try
+0000fcc0: 3a0a 2020 2020 2020 2020 2020 2020 6874  :.            ht
+0000fcd0: 7470 2e68 6561 6428 6970 2c20 7469 6d65  tp.head(ip, time
+0000fce0: 6f75 743d 3329 0a20 2020 2020 2020 2020  out=3).         
+0000fcf0: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+0000fd00: 2020 6578 6365 7074 2028 7265 7175 6573    except (reques
+0000fd10: 7473 2e54 696d 656f 7574 2c20 7265 7175  ts.Timeout, requ
+0000fd20: 6573 7473 2e65 7863 6570 7469 6f6e 732e  ests.exceptions.
+0000fd30: 436f 6e6e 6563 7469 6f6e 4572 726f 7229  ConnectionError)
+0000fd40: 2061 7320 653a 0a20 2020 2020 2020 2020   as e:.         
+0000fd50: 2020 2069 6620 6920 3d3d 206c 656e 285f     if i == len(_
+0000fd60: 5445 5354 5f49 505f 4c49 5354 2920 2d20  TEST_IP_LIST) - 
+0000fd70: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
+0000fd80: 2020 2072 6169 7365 2065 7863 6570 7469     raise excepti
+0000fd90: 6f6e 732e 4e65 7477 6f72 6b45 7272 6f72  ons.NetworkError
+0000fda0: 2827 436f 756c 6420 6e6f 7420 7265 6672  ('Could not refr
+0000fdb0: 6573 6820 7468 6520 636c 7573 7465 722e  esh the cluster.
+0000fdc0: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
+0000fdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fdf0: 2027 4e65 7477 6f72 6b20 7365 656d 7320   'Network seems 
+0000fe00: 646f 776e 2e27 2920 6672 6f6d 2065 0a0a  down.') from e..
+0000fe10: 0a64 6566 2063 6865 636b 5f6f 776e 6572  .def check_owner
+0000fe20: 5f69 6465 6e74 6974 7928 636c 7573 7465  _identity(cluste
+0000fe30: 725f 6e61 6d65 3a20 7374 7229 202d 3e20  r_name: str) -> 
+0000fe40: 4e6f 6e65 3a0a 2020 2020 2222 2243 6865  None:.    """Che
+0000fe50: 636b 2069 6620 6375 7272 656e 7420 7573  ck if current us
+0000fe60: 6572 2069 7320 7468 6520 7361 6d65 2061  er is the same a
+0000fe70: 7320 7468 6520 7573 6572 2077 686f 2063  s the user who c
+0000fe80: 7265 6174 6564 2074 6865 2063 6c75 7374  reated the clust
+0000fe90: 6572 2e0a 0a20 2020 2052 6169 7365 733a  er...    Raises:
+0000fea0: 0a20 2020 2020 2020 2065 7863 6570 7469  .        excepti
+0000feb0: 6f6e 732e 436c 7573 7465 724f 776e 6572  ons.ClusterOwner
+0000fec0: 4964 656e 7469 7479 4d69 736d 6174 6368  IdentityMismatch
+0000fed0: 4572 726f 723a 2069 6620 7468 6520 6375  Error: if the cu
+0000fee0: 7272 656e 7420 7573 6572 2069 730a 2020  rrent user is.  
+0000fef0: 2020 2020 2020 2020 6e6f 7420 7468 6520          not the 
+0000ff00: 7361 6d65 2061 7320 7468 6520 7573 6572  same as the user
+0000ff10: 2077 686f 2063 7265 6174 6564 2074 6865   who created the
+0000ff20: 2063 6c75 7374 6572 2e0a 2020 2020 2020   cluster..      
+0000ff30: 2020 6578 6365 7074 696f 6e73 2e43 6c6f    exceptions.Clo
+0000ff40: 7564 5573 6572 4964 656e 7469 7479 4572  udUserIdentityEr
+0000ff50: 726f 723a 2069 6620 7765 2066 6169 6c20  ror: if we fail 
+0000ff60: 746f 2067 6574 2074 6865 2063 7572 7265  to get the curre
+0000ff70: 6e74 2075 7365 720a 2020 2020 2020 2020  nt user.        
+0000ff80: 2020 6964 656e 7469 7479 2e0a 2020 2020    identity..    
+0000ff90: 2222 220a 2020 2020 6966 2065 6e76 5f6f  """.    if env_o
+0000ffa0: 7074 696f 6e73 2e4f 7074 696f 6e73 2e53  ptions.Options.S
+0000ffb0: 4b49 505f 434c 4f55 445f 4944 454e 5449  KIP_CLOUD_IDENTI
+0000ffc0: 5459 5f43 4845 434b 2e67 6574 2829 3a0a  TY_CHECK.get():.
+0000ffd0: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+0000ffe0: 2020 2072 6563 6f72 6420 3d20 676c 6f62     record = glob
+0000fff0: 616c 5f75 7365 725f 7374 6174 652e 6765  al_user_state.ge
+00010000: 745f 636c 7573 7465 725f 6672 6f6d 5f6e  t_cluster_from_n
+00010010: 616d 6528 636c 7573 7465 725f 6e61 6d65  ame(cluster_name
+00010020: 290a 2020 2020 6966 2072 6563 6f72 6420  ).    if record 
+00010030: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00010040: 2072 6574 7572 6e0a 2020 2020 6861 6e64   return.    hand
+00010050: 6c65 203d 2072 6563 6f72 645b 2768 616e  le = record['han
+00010060: 646c 6527 5d0a 2020 2020 6966 206e 6f74  dle'].    if not
+00010070: 2069 7369 6e73 7461 6e63 6528 6861 6e64   isinstance(hand
+00010080: 6c65 2c20 6261 636b 656e 6473 2e43 6c6f  le, backends.Clo
+00010090: 7564 566d 5261 7952 6573 6f75 7263 6548  udVmRayResourceH
+000100a0: 616e 646c 6529 3a0a 2020 2020 2020 2020  andle):.        
+000100b0: 7265 7475 726e 0a0a 2020 2020 636c 6f75  return..    clou
+000100c0: 6420 3d20 6861 6e64 6c65 2e6c 6175 6e63  d = handle.launc
+000100d0: 6865 645f 7265 736f 7572 6365 732e 636c  hed_resources.cl
+000100e0: 6f75 640a 2020 2020 6375 7272 656e 745f  oud.    current_
+000100f0: 7573 6572 5f69 6465 6e74 6974 7920 3d20  user_identity = 
+00010100: 636c 6f75 642e 6765 745f 6375 7272 656e  cloud.get_curren
+00010110: 745f 7573 6572 5f69 6465 6e74 6974 7928  t_user_identity(
+00010120: 290a 2020 2020 6f77 6e65 725f 6964 656e  ).    owner_iden
+00010130: 7469 7479 203d 2072 6563 6f72 645b 276f  tity = record['o
+00010140: 776e 6572 275d 0a20 2020 2069 6620 6375  wner'].    if cu
+00010150: 7272 656e 745f 7573 6572 5f69 6465 6e74  rrent_user_ident
+00010160: 6974 7920 6973 204e 6f6e 653a 0a20 2020  ity is None:.   
+00010170: 2020 2020 2023 2053 6b69 7020 7468 6520       # Skip the 
+00010180: 6368 6563 6b20 6966 2074 6865 2063 6c6f  check if the clo
+00010190: 7564 2064 6f65 7320 6e6f 7420 7375 7070  ud does not supp
+000101a0: 6f72 7420 7573 6572 2069 6465 6e74 6974  ort user identit
+000101b0: 792e 0a20 2020 2020 2020 2072 6574 7572  y..        retur
+000101c0: 6e0a 2020 2020 2320 5468 6520 7573 6572  n.    # The user
+000101d0: 2069 6465 6e74 6974 7920 6361 6e20 6265   identity can be
+000101e0: 204e 6f6e 652c 2069 6620 7468 6520 636c   None, if the cl
+000101f0: 7573 7465 7220 6973 2063 7265 6174 6564  uster is created
+00010200: 2062 7920 616e 206f 6c64 6572 0a20 2020   by an older.   
+00010210: 2023 2076 6572 7369 6f6e 206f 6620 536b   # version of Sk
+00010220: 7950 696c 6f74 2e20 496e 2074 6861 7420  yPilot. In that 
+00010230: 6361 7365 2c20 7765 2073 6574 2074 6865  case, we set the
+00010240: 2075 7365 7220 6964 656e 7469 7479 2074   user identity t
+00010250: 6f20 7468 650a 2020 2020 2320 6375 7272  o the.    # curr
+00010260: 656e 7420 6f6e 652e 0a20 2020 2023 204e  ent one..    # N
+00010270: 4f54 453a 2061 2075 7365 7220 7768 6f20  OTE: a user who 
+00010280: 7570 6772 6164 6573 2053 6b79 5069 6c6f  upgrades SkyPilo
+00010290: 7420 616e 6420 7377 6974 6368 6573 2074  t and switches t
+000102a0: 6f20 6120 6e65 7720 636c 6f75 6420 6964  o a new cloud id
+000102b0: 656e 7469 7479 0a20 2020 2023 2069 6d6d  entity.    # imm
+000102c0: 6564 6961 7465 6c79 2077 6974 686f 7574  ediately without
+000102d0: 2060 736b 7920 7374 6174 7573 202d 2d72   `sky status --r
+000102e0: 6566 7265 7368 6020 6669 7273 742c 2077  efresh` first, w
+000102f0: 696c 6c20 6361 7573 6520 6120 6c65 616b  ill cause a leak
+00010300: 6167 650a 2020 2020 2320 6f66 2074 6865  age.    # of the
+00010310: 2065 7869 7374 696e 6720 636c 7573 7465   existing cluste
+00010320: 722e 2057 6520 6465 656d 2074 6869 7320  r. We deem this 
+00010330: 616e 2061 6363 6570 7461 626c 6520 7472  an acceptable tr
+00010340: 6164 656f 6666 206d 6169 6e6c 790a 2020  adeoff mainly.  
+00010350: 2020 2320 6265 6361 7573 6520 6d75 6c74    # because mult
+00010360: 692d 6964 656e 7469 7479 2069 7320 6e6f  i-identity is no
+00010370: 7420 636f 6d6d 6f6e 2028 6174 206c 6561  t common (at lea
+00010380: 7374 2061 7420 7468 6520 6d6f 6d65 6e74  st at the moment
+00010390: 292e 0a20 2020 2069 6620 6f77 6e65 725f  )..    if owner_
+000103a0: 6964 656e 7469 7479 2069 7320 4e6f 6e65  identity is None
+000103b0: 3a0a 2020 2020 2020 2020 676c 6f62 616c  :.        global
+000103c0: 5f75 7365 725f 7374 6174 652e 7365 745f  _user_state.set_
+000103d0: 6f77 6e65 725f 6964 656e 7469 7479 5f66  owner_identity_f
+000103e0: 6f72 5f63 6c75 7374 6572 280a 2020 2020  or_cluster(.    
+000103f0: 2020 2020 2020 2020 636c 7573 7465 725f          cluster_
+00010400: 6e61 6d65 2c20 6375 7272 656e 745f 7573  name, current_us
+00010410: 6572 5f69 6465 6e74 6974 7929 0a20 2020  er_identity).   
+00010420: 2065 6c73 653a 0a20 2020 2020 2020 2061   else:.        a
+00010430: 7373 6572 7420 6973 696e 7374 616e 6365  ssert isinstance
+00010440: 286f 776e 6572 5f69 6465 6e74 6974 792c  (owner_identity,
+00010450: 206c 6973 7429 0a20 2020 2020 2020 2023   list).        #
+00010460: 2049 7420 6973 204f 4b20 6966 2074 6865   It is OK if the
+00010470: 206f 776e 6572 2069 6465 6e74 6974 7920   owner identity 
+00010480: 6973 2073 686f 7274 6572 2c20 7768 6963  is shorter, whic
+00010490: 6820 7769 6c6c 2068 6170 7065 6e20 7768  h will happen wh
+000104a0: 656e 0a20 2020 2020 2020 2023 2074 6865  en.        # the
+000104b0: 2063 6c75 7374 6572 2069 7320 6c61 756e   cluster is laun
+000104c0: 6368 6564 2062 6566 6f72 6520 2331 3830  ched before #180
+000104d0: 382e 2049 6e20 7468 6174 2063 6173 652c  8. In that case,
+000104e0: 2077 6520 6f6e 6c79 2063 6865 636b 0a20   we only check. 
+000104f0: 2020 2020 2020 2023 2074 6865 2073 616d         # the sam
+00010500: 6520 6c65 6e67 7468 2028 7a69 7020 7769  e length (zip wi
+00010510: 6c6c 2073 746f 7020 6174 2074 6865 2073  ll stop at the s
+00010520: 686f 7274 6572 206f 6e65 292e 0a20 2020  horter one)..   
+00010530: 2020 2020 2066 6f72 2069 2c20 286f 776e       for i, (own
+00010540: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
+00010550: 2020 2020 6375 7272 656e 7429 2069 6e20      current) in 
+00010560: 656e 756d 6572 6174 6528 7a69 7028 6f77  enumerate(zip(ow
+00010570: 6e65 725f 6964 656e 7469 7479 2c0a 2020  ner_identity,.  
 00010580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010590: 6375 7272 656e 745f 7573 6572 5f69 6465  current_user_ide
-000105a0: 6e74 6974 7929 293a 0a20 2020 2020 2020  ntity)):.       
-000105b0: 2020 2020 2023 2043 6c65 616e 2075 7020       # Clean up 
-000105c0: 7468 6520 6f77 6e65 7220 6964 656e 7469  the owner identi
-000105d0: 7479 2066 6f72 2074 6865 2062 6163 6b73  ty for the backs
-000105e0: 6c61 7368 2061 6e64 206e 6577 6c69 6e65  lash and newline
-000105f0: 732c 2063 6175 7365 640a 2020 2020 2020  s, caused.      
-00010600: 2020 2020 2020 2320 6279 2074 6865 2063        # by the c
-00010610: 6c6f 7564 2043 4c49 206f 7574 7075 742c  loud CLI output,
-00010620: 2065 2e67 2e20 6763 6c6f 7564 2e0a 2020   e.g. gcloud..  
-00010630: 2020 2020 2020 2020 2020 6f77 6e65 7220            owner 
-00010640: 3d20 6f77 6e65 722e 7265 706c 6163 6528  = owner.replace(
-00010650: 275c 6e27 2c20 2727 292e 7265 706c 6163  '\n', '').replac
-00010660: 6528 275c 5c27 2c20 2727 290a 2020 2020  e('\\', '').    
-00010670: 2020 2020 2020 2020 6966 206f 776e 6572          if owner
-00010680: 203d 3d20 6375 7272 656e 743a 0a20 2020   == current:.   
-00010690: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000106a0: 6920 213d 2030 3a0a 2020 2020 2020 2020  i != 0:.        
-000106b0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-000106c0: 6572 2e77 6172 6e69 6e67 280a 2020 2020  er.warning(.    
-000106d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106e0: 2020 2020 6627 5468 6520 636c 7573 7465      f'The cluste
-000106f0: 7220 7761 7320 6f77 6e65 6420 6279 207b  r was owned by {
-00010700: 6f77 6e65 725f 6964 656e 7469 7479 7d2c  owner_identity},
-00010710: 2062 7574 2027 0a20 2020 2020 2020 2020   but '.         
-00010720: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00010730: 2761 206e 6577 2069 6465 6e74 6974 7920  'a new identity 
-00010740: 7b63 7572 7265 6e74 5f75 7365 725f 6964  {current_user_id
-00010750: 656e 7469 7479 7d20 6973 2061 6374 6976  entity} is activ
-00010760: 6174 6564 2e20 5765 2073 7469 6c6c 2027  ated. We still '
-00010770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010780: 2020 2020 2020 2020 2027 616c 6c6f 7720           'allow 
-00010790: 7468 6520 6f70 6572 6174 696f 6e20 6173  the operation as
-000107a0: 2074 6865 2074 776f 2069 6465 6e74 6974   the two identit
-000107b0: 6965 7320 6172 6520 6c69 6b65 6c79 2074  ies are likely t
-000107c0: 6f20 6861 7665 2027 0a20 2020 2020 2020  o have '.       
-000107d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107e0: 2027 7468 6520 7361 6d65 2061 6363 6573   'the same acces
-000107f0: 7320 746f 2074 6865 2063 6c75 7374 6572  s to the cluster
-00010800: 2e20 506c 6561 7365 2062 6520 6177 6172  . Please be awar
-00010810: 6520 7468 6174 2074 6869 7320 6361 6e20  e that this can 
-00010820: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-00010830: 2020 2020 2020 2020 2020 2763 6175 7365            'cause
-00010840: 2075 6e65 7870 6563 7465 6420 636c 7573   unexpected clus
-00010850: 7465 7220 6c65 616b 6167 6520 6966 2074  ter leakage if t
-00010860: 6865 2074 776f 2069 6465 6e74 6974 6965  he two identitie
-00010870: 7320 6172 6520 6e6f 7420 270a 2020 2020  s are not '.    
-00010880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010890: 2020 2020 2761 6374 7561 6c6c 7920 6571      'actually eq
-000108a0: 7569 7661 6c65 6e74 2028 652e 672e 2c20  uivalent (e.g., 
-000108b0: 6265 6c6f 6e67 2074 6f20 7468 6520 7361  belong to the sa
-000108c0: 6d65 2070 6572 736f 6e29 2e27 0a20 2020  me person).'.   
-000108d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108e0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-000108f0: 2020 2069 6620 6920 213d 2030 206f 7220     if i != 0 or 
-00010900: 6c65 6e28 6f77 6e65 725f 6964 656e 7469  len(owner_identi
-00010910: 7479 2920 213d 206c 656e 2863 7572 7265  ty) != len(curre
-00010920: 6e74 5f75 7365 725f 6964 656e 7469 7479  nt_user_identity
-00010930: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00010940: 2020 2020 2020 2023 2057 6520 7570 6461         # We upda
-00010950: 7465 2074 6865 206f 776e 6572 206f 6620  te the owner of 
-00010960: 6120 636c 7573 7465 722c 2077 6865 6e3a  a cluster, when:
-00010970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010980: 2020 2020 2023 2031 2e20 5468 6520 7374       # 1. The st
-00010990: 7269 6374 6573 7420 6964 656e 7474 7920  rictest identty 
-000109a0: 2869 2e65 2e20 7468 6520 6669 7273 7420  (i.e. the first 
-000109b0: 6f6e 6529 2064 6f65 7320 6e6f 740a 2020  one) does not.  
-000109c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109d0: 2020 2320 6d61 7463 682c 2062 7574 2074    # match, but t
-000109e0: 6865 206c 6174 7465 7220 6f6e 6573 206d  he latter ones m
-000109f0: 6174 6368 2e0a 2020 2020 2020 2020 2020  atch..          
-00010a00: 2020 2020 2020 2020 2020 2320 322e 2054            # 2. T
-00010a10: 6865 206c 656e 6774 6820 6f66 2074 6865  he length of the
-00010a20: 2074 776f 2069 6465 6e74 6974 6965 7320   two identities 
-00010a30: 6172 6520 6469 6666 6572 656e 742c 2077  are different, w
-00010a40: 6869 6368 0a20 2020 2020 2020 2020 2020  hich.           
-00010a50: 2020 2020 2020 2020 2023 2077 696c 6c20           # will 
-00010a60: 6f6e 6c79 2068 6170 7065 6e20 7768 656e  only happen when
-00010a70: 2074 6865 2063 6c75 7374 6572 2069 7320   the cluster is 
-00010a80: 6c61 756e 6368 6564 2062 6566 6f72 6520  launched before 
-00010a90: 2331 3830 382e 0a20 2020 2020 2020 2020  #1808..         
-00010aa0: 2020 2020 2020 2020 2020 2023 2055 7064             # Upd
-00010ab0: 6174 6520 7468 6520 7573 6572 2069 6465  ate the user ide
-00010ac0: 6e74 6974 7920 746f 2061 766f 6964 2073  ntity to avoid s
-00010ad0: 686f 7769 6e67 2074 6865 2077 6172 6e69  howing the warni
-00010ae0: 6e67 2061 626f 7665 0a20 2020 2020 2020  ng above.       
-00010af0: 2020 2020 2020 2020 2020 2020 2023 2061               # a
-00010b00: 6761 696e 2e0a 2020 2020 2020 2020 2020  gain..          
-00010b10: 2020 2020 2020 2020 2020 676c 6f62 616c            global
-00010b20: 5f75 7365 725f 7374 6174 652e 7365 745f  _user_state.set_
-00010b30: 6f77 6e65 725f 6964 656e 7469 7479 5f66  owner_identity_f
-00010b40: 6f72 5f63 6c75 7374 6572 280a 2020 2020  or_cluster(.    
-00010b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b60: 2020 2020 636c 7573 7465 725f 6e61 6d65      cluster_name
-00010b70: 2c20 6375 7272 656e 745f 7573 6572 5f69  , current_user_i
-00010b80: 6465 6e74 6974 7929 0a20 2020 2020 2020  dentity).       
-00010b90: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00010ba0: 2023 2054 6865 2075 7365 7220 6964 656e   # The user iden
-00010bb0: 7469 7479 206d 6174 6368 6573 2e0a 2020  tity matches..  
-00010bc0: 2020 2020 2020 7769 7468 2075 785f 7574        with ux_ut
-00010bd0: 696c 732e 7072 696e 745f 6578 6365 7074  ils.print_except
-00010be0: 696f 6e5f 6e6f 5f74 7261 6365 6261 636b  ion_no_traceback
-00010bf0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00010c00: 7261 6973 6520 6578 6365 7074 696f 6e73  raise exceptions
-00010c10: 2e43 6c75 7374 6572 4f77 6e65 7249 6465  .ClusterOwnerIde
-00010c20: 6e74 6974 794d 6973 6d61 7463 6845 7272  ntityMismatchErr
-00010c30: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
-00010c40: 2020 2020 6627 7b63 6c75 7374 6572 5f6e      f'{cluster_n
-00010c50: 616d 6521 727d 2028 7b63 6c6f 7564 7d29  ame!r} ({cloud})
-00010c60: 2069 7320 6f77 6e65 6420 6279 2061 6363   is owned by acc
-00010c70: 6f75 6e74 2027 0a20 2020 2020 2020 2020  ount '.         
-00010c80: 2020 2020 2020 2066 277b 6f77 6e65 725f         f'{owner_
-00010c90: 6964 656e 7469 7479 2172 7d2c 2062 7574  identity!r}, but
-00010ca0: 2074 6865 2061 6374 6976 6174 6564 2061   the activated a
-00010cb0: 6363 6f75 6e74 2027 0a20 2020 2020 2020  ccount '.       
-00010cc0: 2020 2020 2020 2020 2066 2769 7320 7b63           f'is {c
-00010cd0: 7572 7265 6e74 5f75 7365 725f 6964 656e  urrent_user_iden
-00010ce0: 7469 7479 2172 7d2e 2729 0a0a 0a64 6566  tity!r}.')...def
-00010cf0: 2074 6167 5f66 696c 7465 725f 666f 725f   tag_filter_for_
-00010d00: 636c 7573 7465 7228 636c 7573 7465 725f  cluster(cluster_
-00010d10: 6e61 6d65 3a20 7374 7229 202d 3e20 4469  name: str) -> Di
-00010d20: 6374 5b73 7472 2c20 7374 725d 3a0a 2020  ct[str, str]:.  
-00010d30: 2020 2222 2252 6574 7572 6e73 2061 2074    """Returns a t
-00010d40: 6167 2066 696c 7465 7220 666f 7220 7468  ag filter for th
-00010d50: 6520 636c 7573 7465 722e 2222 220a 2020  e cluster.""".  
-00010d60: 2020 7265 7475 726e 207b 0a20 2020 2020    return {.     
-00010d70: 2020 2027 7261 792d 636c 7573 7465 722d     'ray-cluster-
-00010d80: 6e61 6d65 273a 2063 6c75 7374 6572 5f6e  name': cluster_n
-00010d90: 616d 652c 0a20 2020 207d 0a0a 0a64 6566  ame,.    }...def
-00010da0: 205f 7175 6572 795f 636c 7573 7465 725f   _query_cluster_
-00010db0: 7374 6174 7573 5f76 6961 5f63 6c6f 7564  status_via_cloud
-00010dc0: 5f61 7069 280a 2020 2020 6861 6e64 6c65  _api(.    handle
-00010dd0: 3a20 2763 6c6f 7564 5f76 6d5f 7261 795f  : 'cloud_vm_ray_
-00010de0: 6261 636b 656e 642e 436c 6f75 6456 6d52  backend.CloudVmR
-00010df0: 6179 5265 736f 7572 6365 4861 6e64 6c65  ayResourceHandle
-00010e00: 270a 2920 2d3e 204c 6973 745b 7374 6174  '.) -> List[stat
-00010e10: 7573 5f6c 6962 2e43 6c75 7374 6572 5374  us_lib.ClusterSt
-00010e20: 6174 7573 5d3a 0a20 2020 2022 2222 5265  atus]:.    """Re
-00010e30: 7475 726e 7320 7468 6520 7374 6174 7573  turns the status
-00010e40: 206f 6620 7468 6520 636c 7573 7465 722e   of the cluster.
-00010e50: 0a0a 2020 2020 5261 6973 6573 3a0a 2020  ..    Raises:.  
-00010e60: 2020 2020 2020 6578 6365 7074 696f 6e73        exceptions
-00010e70: 2e43 6c75 7374 6572 5374 6174 7573 4665  .ClusterStatusFe
-00010e80: 7463 6869 6e67 4572 726f 723a 2074 6865  tchingError: the
-00010e90: 2063 6c75 7374 6572 2073 7461 7475 7320   cluster status 
-00010ea0: 6361 6e6e 6f74 2062 650a 2020 2020 2020  cannot be.      
-00010eb0: 2020 2020 6665 7463 6865 6420 6672 6f6d      fetched from
-00010ec0: 2074 6865 2063 6c6f 7564 2070 726f 7669   the cloud provi
-00010ed0: 6465 722e 0a20 2020 2022 2222 0a20 2020  der..    """.   
-00010ee0: 2063 6c75 7374 6572 5f6e 616d 655f 6f6e   cluster_name_on
-00010ef0: 5f63 6c6f 7564 203d 2068 616e 646c 652e  _cloud = handle.
-00010f00: 636c 7573 7465 725f 6e61 6d65 5f6f 6e5f  cluster_name_on_
-00010f10: 636c 6f75 640a 2020 2020 636c 7573 7465  cloud.    cluste
-00010f20: 725f 6e61 6d65 5f69 6e5f 6869 6e74 203d  r_name_in_hint =
-00010f30: 2063 6f6d 6d6f 6e5f 7574 696c 732e 636c   common_utils.cl
-00010f40: 7573 7465 725f 6e61 6d65 5f69 6e5f 6869  uster_name_in_hi
-00010f50: 6e74 280a 2020 2020 2020 2020 6861 6e64  nt(.        hand
-00010f60: 6c65 2e63 6c75 7374 6572 5f6e 616d 652c  le.cluster_name,
-00010f70: 2063 6c75 7374 6572 5f6e 616d 655f 6f6e   cluster_name_on
-00010f80: 5f63 6c6f 7564 290a 2020 2020 2320 5573  _cloud).    # Us
-00010f90: 6520 7265 6769 6f6e 2061 6e64 207a 6f6e  e region and zon
-00010fa0: 6520 6672 6f6d 2074 6865 2063 6c75 7374  e from the clust
-00010fb0: 6572 2063 6f6e 6669 672c 2069 6e73 7465  er config, inste
-00010fc0: 6164 206f 6620 7468 650a 2020 2020 2320  ad of the.    # 
-00010fd0: 6861 6e64 6c65 2e6c 6175 6e63 6865 645f  handle.launched_
-00010fe0: 7265 736f 7572 6365 732c 2062 6563 6175  resources, becau
-00010ff0: 7365 2074 6865 206c 6174 7465 7220 6d61  se the latter ma
-00011000: 7920 6e6f 7420 6265 2073 6574 0a20 2020  y not be set.   
-00011010: 2023 2063 6f72 7265 6374 6c79 2079 6574   # correctly yet
-00011020: 2e0a 2020 2020 7261 795f 636f 6e66 6967  ..    ray_config
-00011030: 203d 2063 6f6d 6d6f 6e5f 7574 696c 732e   = common_utils.
-00011040: 7265 6164 5f79 616d 6c28 6861 6e64 6c65  read_yaml(handle
-00011050: 2e63 6c75 7374 6572 5f79 616d 6c29 0a20  .cluster_yaml). 
-00011060: 2020 2070 726f 7669 6465 725f 636f 6e66     provider_conf
-00011070: 6967 203d 2072 6179 5f63 6f6e 6669 675b  ig = ray_config[
-00011080: 2770 726f 7669 6465 7227 5d0a 0a20 2020  'provider']..   
-00011090: 2023 2051 7565 7279 2074 6865 2063 6c6f   # Query the clo
-000110a0: 7564 2070 726f 7669 6465 722e 0a20 2020  ud provider..   
-000110b0: 2023 2054 4f44 4f28 7375 7175 6172 6b29   # TODO(suquark)
-000110c0: 3a20 6d6f 7665 2069 6d70 6c65 6d65 6e74  : move implement
-000110d0: 6174 696f 6e73 206f 6620 6d6f 7265 2063  ations of more c
-000110e0: 6c6f 7564 7320 6865 7265 0a20 2020 2063  louds here.    c
-000110f0: 6c6f 7564 203d 2068 616e 646c 652e 6c61  loud = handle.la
-00011100: 756e 6368 6564 5f72 6573 6f75 7263 6573  unched_resources
-00011110: 2e63 6c6f 7564 0a20 2020 2061 7373 6572  .cloud.    asser
-00011120: 7420 636c 6f75 6420 6973 206e 6f74 204e  t cloud is not N
-00011130: 6f6e 652c 2068 616e 646c 650a 2020 2020  one, handle.    
-00011140: 6966 2063 6c6f 7564 2e53 5441 5455 535f  if cloud.STATUS_
-00011150: 5645 5253 494f 4e20 3e3d 2063 6c6f 7564  VERSION >= cloud
-00011160: 732e 5374 6174 7573 5665 7273 696f 6e2e  s.StatusVersion.
-00011170: 534b 5950 494c 4f54 3a0a 2020 2020 2020  SKYPILOT:.      
-00011180: 2020 636c 6f75 645f 6e61 6d65 203d 2072    cloud_name = r
-00011190: 6570 7228 6861 6e64 6c65 2e6c 6175 6e63  epr(handle.launc
-000111a0: 6865 645f 7265 736f 7572 6365 732e 636c  hed_resources.cl
-000111b0: 6f75 6429 0a20 2020 2020 2020 2074 7279  oud).        try
-000111c0: 3a0a 2020 2020 2020 2020 2020 2020 6e6f  :.            no
-000111d0: 6465 5f73 7461 7475 735f 6469 6374 203d  de_status_dict =
-000111e0: 2070 726f 7669 7369 6f6e 5f6c 6962 2e71   provision_lib.q
-000111f0: 7565 7279 5f69 6e73 7461 6e63 6573 280a  uery_instances(.
-00011200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011210: 636c 6f75 645f 6e61 6d65 2c20 636c 7573  cloud_name, clus
-00011220: 7465 725f 6e61 6d65 5f6f 6e5f 636c 6f75  ter_name_on_clou
-00011230: 642c 2070 726f 7669 6465 725f 636f 6e66  d, provider_conf
-00011240: 6967 290a 2020 2020 2020 2020 2020 2020  ig).            
-00011250: 6c6f 6767 6572 2e64 6562 7567 2866 2751  logger.debug(f'Q
-00011260: 7565 7279 696e 6720 7b63 6c6f 7564 5f6e  uerying {cloud_n
-00011270: 616d 657d 2063 6c75 7374 6572 2027 0a20  ame} cluster '. 
-00011280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011290: 2020 2020 2020 2020 6627 7b63 6c75 7374          f'{clust
-000112a0: 6572 5f6e 616d 655f 696e 5f68 696e 747d  er_name_in_hint}
-000112b0: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
-000112c0: 2020 2020 2020 2020 2020 2020 6627 7374              f'st
-000112d0: 6174 7573 3a5c 6e7b 7070 7269 6e74 2e70  atus:\n{pprint.p
-000112e0: 666f 726d 6174 286e 6f64 655f 7374 6174  format(node_stat
-000112f0: 7573 5f64 6963 7429 7d27 290a 2020 2020  us_dict)}').    
-00011300: 2020 2020 2020 2020 6e6f 6465 5f73 7461          node_sta
-00011310: 7475 7365 7320 3d20 6c69 7374 286e 6f64  tuses = list(nod
-00011320: 655f 7374 6174 7573 5f64 6963 742e 7661  e_status_dict.va
-00011330: 6c75 6573 2829 290a 2020 2020 2020 2020  lues()).        
-00011340: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-00011350: 2061 7320 653a 2020 2320 7079 6c69 6e74   as e:  # pylint
-00011360: 3a20 6469 7361 626c 653d 6272 6f61 642d  : disable=broad-
-00011370: 6578 6365 7074 0a20 2020 2020 2020 2020  except.         
-00011380: 2020 2077 6974 6820 7578 5f75 7469 6c73     with ux_utils
-00011390: 2e70 7269 6e74 5f65 7863 6570 7469 6f6e  .print_exception
-000113a0: 5f6e 6f5f 7472 6163 6562 6163 6b28 293a  _no_traceback():
-000113b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000113c0: 2072 6169 7365 2065 7863 6570 7469 6f6e   raise exception
-000113d0: 732e 436c 7573 7465 7253 7461 7475 7346  s.ClusterStatusF
-000113e0: 6574 6368 696e 6745 7272 6f72 280a 2020  etchingError(.  
-000113f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011400: 2020 6627 4661 696c 6564 2074 6f20 7175    f'Failed to qu
-00011410: 6572 7920 7b63 6c6f 7564 5f6e 616d 657d  ery {cloud_name}
-00011420: 2063 6c75 7374 6572 2027 0a20 2020 2020   cluster '.     
-00011430: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00011440: 277b 636c 7573 7465 725f 6e61 6d65 5f69  '{cluster_name_i
-00011450: 6e5f 6869 6e74 7d20 270a 2020 2020 2020  n_hint} '.      
-00011460: 2020 2020 2020 2020 2020 2020 2020 6627                f'
-00011470: 7374 6174 7573 3a20 7b63 6f6d 6d6f 6e5f  status: {common_
-00011480: 7574 696c 732e 666f 726d 6174 5f65 7863  utils.format_exc
-00011490: 6570 7469 6f6e 2865 2c20 7573 655f 6272  eption(e, use_br
-000114a0: 6163 6b65 743d 5472 7565 297d 270a 2020  acket=True)}'.  
-000114b0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-000114c0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000114d0: 2020 7265 6769 6f6e 203d 2070 726f 7669    region = provi
-000114e0: 6465 725f 636f 6e66 6967 2e67 6574 2827  der_config.get('
-000114f0: 7265 6769 6f6e 2729 206f 7220 7072 6f76  region') or prov
-00011500: 6964 6572 5f63 6f6e 6669 672e 6765 7428  ider_config.get(
-00011510: 0a20 2020 2020 2020 2020 2020 2027 6c6f  .            'lo
-00011520: 6361 7469 6f6e 2729 0a20 2020 2020 2020  cation').       
-00011530: 207a 6f6e 6520 3d20 7261 795f 636f 6e66   zone = ray_conf
-00011540: 6967 5b27 7072 6f76 6964 6572 275d 2e67  ig['provider'].g
-00011550: 6574 2827 6176 6169 6c61 6269 6c69 7479  et('availability
-00011560: 5f7a 6f6e 6527 290a 2020 2020 2020 2020  _zone').        
-00011570: 6e6f 6465 5f73 7461 7475 7365 7320 3d20  node_statuses = 
-00011580: 636c 6f75 642e 7175 6572 795f 7374 6174  cloud.query_stat
-00011590: 7573 280a 2020 2020 2020 2020 2020 2020  us(.            
-000115a0: 636c 7573 7465 725f 6e61 6d65 5f6f 6e5f  cluster_name_on_
-000115b0: 636c 6f75 642c 0a20 2020 2020 2020 2020  cloud,.         
-000115c0: 2020 2074 6167 5f66 696c 7465 725f 666f     tag_filter_fo
-000115d0: 725f 636c 7573 7465 7228 636c 7573 7465  r_cluster(cluste
-000115e0: 725f 6e61 6d65 5f6f 6e5f 636c 6f75 6429  r_name_on_cloud)
-000115f0: 2c20 7265 6769 6f6e 2c20 7a6f 6e65 290a  , region, zone).
-00011600: 2020 2020 7265 7475 726e 206e 6f64 655f      return node_
-00011610: 7374 6174 7573 6573 0a0a 0a64 6566 2063  statuses...def c
-00011620: 6865 636b 5f63 616e 5f63 6c6f 6e65 5f64  heck_can_clone_d
-00011630: 6973 6b5f 616e 645f 6f76 6572 7269 6465  isk_and_override
-00011640: 5f74 6173 6b28 0a20 2020 2063 6c75 7374  _task(.    clust
-00011650: 6572 5f6e 616d 653a 2073 7472 2c20 7461  er_name: str, ta
-00011660: 7267 6574 5f63 6c75 7374 6572 5f6e 616d  rget_cluster_nam
-00011670: 653a 204f 7074 696f 6e61 6c5b 7374 725d  e: Optional[str]
-00011680: 2c20 7461 736b 3a20 2774 6173 6b5f 6c69  , task: 'task_li
-00011690: 622e 5461 736b 270a 2920 2d3e 2054 7570  b.Task'.) -> Tup
-000116a0: 6c65 5b27 7461 736b 5f6c 6962 2e54 6173  le['task_lib.Tas
-000116b0: 6b27 2c20 2763 6c6f 7564 5f76 6d5f 7261  k', 'cloud_vm_ra
-000116c0: 795f 6261 636b 656e 642e 436c 6f75 6456  y_backend.CloudV
-000116d0: 6d52 6179 5265 736f 7572 6365 4861 6e64  mRayResourceHand
-000116e0: 6c65 275d 3a0a 2020 2020 2222 2243 6865  le']:.    """Che
-000116f0: 636b 2069 6620 7468 6520 7461 736b 2069  ck if the task i
-00011700: 7320 636f 6d70 6174 6962 6c65 2074 6f20  s compatible to 
-00011710: 636c 6f6e 6520 6469 736b 2066 726f 6d20  clone disk from 
-00011720: 7468 6520 736f 7572 6365 2063 6c75 7374  the source clust
-00011730: 6572 2e0a 0a20 2020 2041 7267 733a 0a20  er...    Args:. 
-00011740: 2020 2020 2020 2063 6c75 7374 6572 5f6e         cluster_n
-00011750: 616d 653a 2054 6865 206e 616d 6520 6f66  ame: The name of
-00011760: 2074 6865 2063 6c75 7374 6572 2074 6f20   the cluster to 
-00011770: 636c 6f6e 6520 6469 736b 2066 726f 6d2e  clone disk from.
-00011780: 0a20 2020 2020 2020 2074 6172 6765 745f  .        target_
-00011790: 636c 7573 7465 725f 6e61 6d65 3a20 5468  cluster_name: Th
-000117a0: 6520 6e61 6d65 206f 6620 7468 6520 7461  e name of the ta
-000117b0: 7267 6574 2063 6c75 7374 6572 2e0a 2020  rget cluster..  
-000117c0: 2020 2020 2020 7461 736b 3a20 5468 6520        task: The 
-000117d0: 7461 736b 2074 6f20 6368 6563 6b2e 0a0a  task to check...
-000117e0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-000117f0: 2020 2020 2054 6865 2074 6173 6b20 746f       The task to
-00011800: 2075 7365 2061 6e64 2074 6865 2072 6573   use and the res
-00011810: 6f75 7263 6520 6861 6e64 6c65 206f 6620  ource handle of 
-00011820: 7468 6520 736f 7572 6365 2063 6c75 7374  the source clust
-00011830: 6572 2e0a 0a20 2020 2052 6169 7365 733a  er...    Raises:
-00011840: 0a20 2020 2020 2020 2056 616c 7565 4572  .        ValueEr
-00011850: 726f 723a 2049 6620 7468 6520 736f 7572  ror: If the sour
-00011860: 6365 2063 6c75 7374 6572 2064 6f65 7320  ce cluster does 
-00011870: 6e6f 7420 6578 6973 742e 0a20 2020 2020  not exist..     
-00011880: 2020 2065 7863 6570 7469 6f6e 732e 4e6f     exceptions.No
-00011890: 7453 7570 706f 7274 6564 4572 726f 723a  tSupportedError:
-000118a0: 2049 6620 7468 6520 736f 7572 6365 2063   If the source c
-000118b0: 6c75 7374 6572 2069 7320 6e6f 7420 7661  luster is not va
-000118c0: 6c69 6420 6f72 2074 6865 0a20 2020 2020  lid or the.     
-000118d0: 2020 2020 2020 2074 6173 6b20 6973 206e         task is n
-000118e0: 6f74 2063 6f6d 7061 7469 626c 6520 746f  ot compatible to
-000118f0: 2063 6c6f 6e65 2064 6973 6b20 6672 6f6d   clone disk from
-00011900: 2074 6865 2073 6f75 7263 6520 636c 7573   the source clus
-00011910: 7465 722e 0a20 2020 2022 2222 0a20 2020  ter..    """.   
-00011920: 2073 6f75 7263 655f 636c 7573 7465 725f   source_cluster_
-00011930: 7374 6174 7573 2c20 6861 6e64 6c65 203d  status, handle =
-00011940: 2072 6566 7265 7368 5f63 6c75 7374 6572   refresh_cluster
-00011950: 5f73 7461 7475 735f 6861 6e64 6c65 2863  _status_handle(c
-00011960: 6c75 7374 6572 5f6e 616d 6529 0a20 2020  luster_name).   
-00011970: 2069 6620 736f 7572 6365 5f63 6c75 7374   if source_clust
-00011980: 6572 5f73 7461 7475 7320 6973 204e 6f6e  er_status is Non
-00011990: 653a 0a20 2020 2020 2020 2077 6974 6820  e:.        with 
-000119a0: 7578 5f75 7469 6c73 2e70 7269 6e74 5f65  ux_utils.print_e
-000119b0: 7863 6570 7469 6f6e 5f6e 6f5f 7472 6163  xception_no_trac
-000119c0: 6562 6163 6b28 293a 0a20 2020 2020 2020  eback():.       
-000119d0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-000119e0: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
-000119f0: 2020 2020 2020 2066 2743 616e 6e6f 7420         f'Cannot 
-00011a00: 6669 6e64 2063 6c75 7374 6572 207b 636c  find cluster {cl
-00011a10: 7573 7465 725f 6e61 6d65 2172 7d20 746f  uster_name!r} to
-00011a20: 2063 6c6f 6e65 2064 6973 6b20 6672 6f6d   clone disk from
-00011a30: 2e27 290a 0a20 2020 2069 6620 6e6f 7420  .')..    if not 
-00011a40: 6973 696e 7374 616e 6365 2868 616e 646c  isinstance(handl
-00011a50: 652c 2062 6163 6b65 6e64 732e 436c 6f75  e, backends.Clou
-00011a60: 6456 6d52 6179 5265 736f 7572 6365 4861  dVmRayResourceHa
-00011a70: 6e64 6c65 293a 0a20 2020 2020 2020 2077  ndle):.        w
-00011a80: 6974 6820 7578 5f75 7469 6c73 2e70 7269  ith ux_utils.pri
-00011a90: 6e74 5f65 7863 6570 7469 6f6e 5f6e 6f5f  nt_exception_no_
-00011aa0: 7472 6163 6562 6163 6b28 293a 0a20 2020  traceback():.   
-00011ab0: 2020 2020 2020 2020 2072 6169 7365 2065           raise e
-00011ac0: 7863 6570 7469 6f6e 732e 4e6f 7453 7570  xceptions.NotSup
-00011ad0: 706f 7274 6564 4572 726f 7228 0a20 2020  portedError(.   
-00011ae0: 2020 2020 2020 2020 2020 2020 2066 2743               f'C
-00011af0: 616e 6e6f 7420 636c 6f6e 6520 6469 736b  annot clone disk
-00011b00: 2066 726f 6d20 6120 6e6f 6e2d 636c 6f75   from a non-clou
-00011b10: 6420 636c 7573 7465 7220 7b63 6c75 7374  d cluster {clust
-00011b20: 6572 5f6e 616d 6521 727d 2e27 290a 0a20  er_name!r}.').. 
-00011b30: 2020 2069 6620 736f 7572 6365 5f63 6c75     if source_clu
-00011b40: 7374 6572 5f73 7461 7475 7320 213d 2073  ster_status != s
-00011b50: 7461 7475 735f 6c69 622e 436c 7573 7465  tatus_lib.Cluste
-00011b60: 7253 7461 7475 732e 5354 4f50 5045 443a  rStatus.STOPPED:
-00011b70: 0a20 2020 2020 2020 2077 6974 6820 7578  .        with ux
-00011b80: 5f75 7469 6c73 2e70 7269 6e74 5f65 7863  _utils.print_exc
-00011b90: 6570 7469 6f6e 5f6e 6f5f 7472 6163 6562  eption_no_traceb
-00011ba0: 6163 6b28 293a 0a20 2020 2020 2020 2020  ack():.         
-00011bb0: 2020 2072 6169 7365 2065 7863 6570 7469     raise excepti
-00011bc0: 6f6e 732e 4e6f 7453 7570 706f 7274 6564  ons.NotSupported
-00011bd0: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
-00011be0: 2020 2020 2020 2066 2743 616e 6e6f 7420         f'Cannot 
-00011bf0: 636c 6f6e 6520 6469 736b 2066 726f 6d20  clone disk from 
-00011c00: 636c 7573 7465 7220 7b63 6c75 7374 6572  cluster {cluster
-00011c10: 5f6e 616d 6521 727d 2027 0a20 2020 2020  _name!r} '.     
-00011c20: 2020 2020 2020 2020 2020 2066 2728 7b73             f'({s
-00011c30: 6f75 7263 655f 636c 7573 7465 725f 7374  ource_cluster_st
-00011c40: 6174 7573 2172 7d29 2e20 506c 6561 7365  atus!r}). Please
-00011c50: 2073 746f 7020 7468 6520 270a 2020 2020   stop the '.    
-00011c60: 2020 2020 2020 2020 2020 2020 6627 636c              f'cl
-00011c70: 7573 7465 7220 6669 7273 743a 2073 6b79  uster first: sky
-00011c80: 2073 746f 7020 7b63 6c75 7374 6572 5f6e   stop {cluster_n
-00011c90: 616d 657d 2729 0a0a 2020 2020 6966 2074  ame}')..    if t
-00011ca0: 6172 6765 745f 636c 7573 7465 725f 6e61  arget_cluster_na
-00011cb0: 6d65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  me is not None:.
-00011cc0: 2020 2020 2020 2020 7461 7267 6574 5f63          target_c
-00011cd0: 6c75 7374 6572 5f73 7461 7475 732c 205f  luster_status, _
-00011ce0: 203d 2072 6566 7265 7368 5f63 6c75 7374   = refresh_clust
-00011cf0: 6572 5f73 7461 7475 735f 6861 6e64 6c65  er_status_handle
-00011d00: 280a 2020 2020 2020 2020 2020 2020 7461  (.            ta
-00011d10: 7267 6574 5f63 6c75 7374 6572 5f6e 616d  rget_cluster_nam
-00011d20: 6529 0a20 2020 2020 2020 2069 6620 7461  e).        if ta
-00011d30: 7267 6574 5f63 6c75 7374 6572 5f73 7461  rget_cluster_sta
-00011d40: 7475 7320 6973 206e 6f74 204e 6f6e 653a  tus is not None:
-00011d50: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
-00011d60: 6820 7578 5f75 7469 6c73 2e70 7269 6e74  h ux_utils.print
-00011d70: 5f65 7863 6570 7469 6f6e 5f6e 6f5f 7472  _exception_no_tr
-00011d80: 6163 6562 6163 6b28 293a 0a20 2020 2020  aceback():.     
-00011d90: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00011da0: 2065 7863 6570 7469 6f6e 732e 4e6f 7453   exceptions.NotS
-00011db0: 7570 706f 7274 6564 4572 726f 7228 0a20  upportedError(. 
-00011dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011dd0: 2020 2066 2754 6865 2074 6172 6765 7420     f'The target 
-00011de0: 636c 7573 7465 7220 7b74 6172 6765 745f  cluster {target_
-00011df0: 636c 7573 7465 725f 6e61 6d65 2172 7d20  cluster_name!r} 
-00011e00: 616c 7265 6164 7920 6578 6973 7473 2e20  already exists. 
-00011e10: 436c 6f6e 696e 6720 270a 2020 2020 2020  Cloning '.      
-00011e20: 2020 2020 2020 2020 2020 2020 2020 2764                'd
-00011e30: 6973 6b20 6973 206f 6e6c 7920 7375 7070  isk is only supp
-00011e40: 6f72 7465 6420 7768 656e 2063 7265 6174  orted when creat
-00011e50: 696e 6720 6120 6e65 7720 636c 7573 7465  ing a new cluste
-00011e60: 722e 2054 6f20 6669 783a 2073 7065 6369  r. To fix: speci
-00011e70: 6679 2027 0a20 2020 2020 2020 2020 2020  fy '.           
-00011e80: 2020 2020 2020 2020 2027 6120 6e65 7720           'a new 
-00011e90: 7461 7267 6574 2063 6c75 7374 6572 206e  target cluster n
-00011ea0: 616d 652e 2729 0a0a 2020 2020 6e65 775f  ame.')..    new_
-00011eb0: 7461 736b 5f72 6573 6f75 7263 6573 203d  task_resources =
-00011ec0: 205b 5d0a 2020 2020 6f72 6967 696e 616c   [].    original
-00011ed0: 5f63 6c6f 7564 203d 2068 616e 646c 652e  _cloud = handle.
-00011ee0: 6c61 756e 6368 6564 5f72 6573 6f75 7263  launched_resourc
-00011ef0: 6573 2e63 6c6f 7564 0a20 2020 206f 7269  es.cloud.    ori
-00011f00: 6769 6e61 6c5f 636c 6f75 642e 6368 6563  ginal_cloud.chec
-00011f10: 6b5f 6665 6174 7572 6573 5f61 7265 5f73  k_features_are_s
-00011f20: 7570 706f 7274 6564 280a 2020 2020 2020  upported(.      
-00011f30: 2020 6861 6e64 6c65 2e6c 6175 6e63 6865    handle.launche
-00011f40: 645f 7265 736f 7572 6365 732c 0a20 2020  d_resources,.   
-00011f50: 2020 2020 207b 636c 6f75 6473 2e43 6c6f       {clouds.Clo
-00011f60: 7564 496d 706c 656d 656e 7461 7469 6f6e  udImplementation
-00011f70: 4665 6174 7572 6573 2e43 4c4f 4e45 5f44  Features.CLONE_D
-00011f80: 4953 4b5f 4652 4f4d 5f43 4c55 5354 4552  ISK_FROM_CLUSTER
-00011f90: 7d29 0a0a 2020 2020 6173 7365 7274 206f  })..    assert o
-00011fa0: 7269 6769 6e61 6c5f 636c 6f75 6420 6973  riginal_cloud is
-00011fb0: 206e 6f74 204e 6f6e 652c 2068 616e 646c   not None, handl
-00011fc0: 652e 6c61 756e 6368 6564 5f72 6573 6f75  e.launched_resou
-00011fd0: 7263 6573 0a20 2020 2068 6173 5f6f 7665  rces.    has_ove
-00011fe0: 7272 6964 6520 3d20 4661 6c73 650a 2020  rride = False.  
-00011ff0: 2020 6861 735f 6469 736b 5f73 697a 655f    has_disk_size_
-00012000: 6d65 7420 3d20 4661 6c73 650a 2020 2020  met = False.    
-00012010: 6861 735f 636c 6f75 645f 6d65 7420 3d20  has_cloud_met = 
-00012020: 4661 6c73 650a 2020 2020 666f 7220 7461  False.    for ta
-00012030: 736b 5f72 6573 6f75 7263 6573 2069 6e20  sk_resources in 
-00012040: 7461 736b 2e72 6573 6f75 7263 6573 3a0a  task.resources:.
-00012050: 2020 2020 2020 2020 6966 2068 616e 646c          if handl
-00012060: 652e 6c61 756e 6368 6564 5f72 6573 6f75  e.launched_resou
-00012070: 7263 6573 2e64 6973 6b5f 7369 7a65 203e  rces.disk_size >
-00012080: 2074 6173 6b5f 7265 736f 7572 6365 732e   task_resources.
-00012090: 6469 736b 5f73 697a 653a 0a20 2020 2020  disk_size:.     
-000120a0: 2020 2020 2020 2023 2054 6865 2074 6172         # The tar
-000120b0: 6765 7420 636c 7573 7465 7227 7320 6469  get cluster's di
-000120c0: 736b 2073 686f 756c 6420 6265 2061 7420  sk should be at 
-000120d0: 6c65 6173 7420 6173 206c 6172 6765 2061  least as large a
-000120e0: 7320 7468 6520 736f 7572 6365 2e0a 2020  s the source..  
-000120f0: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-00012100: 7565 0a20 2020 2020 2020 2068 6173 5f64  ue.        has_d
-00012110: 6973 6b5f 7369 7a65 5f6d 6574 203d 2054  isk_size_met = T
-00012120: 7275 650a 2020 2020 2020 2020 6966 2074  rue.        if t
-00012130: 6173 6b5f 7265 736f 7572 6365 732e 636c  ask_resources.cl
-00012140: 6f75 6420 6973 206e 6f74 204e 6f6e 6520  oud is not None 
-00012150: 616e 6420 6e6f 7420 6f72 6967 696e 616c  and not original
-00012160: 5f63 6c6f 7564 2e69 735f 7361 6d65 5f63  _cloud.is_same_c
-00012170: 6c6f 7564 280a 2020 2020 2020 2020 2020  loud(.          
-00012180: 2020 2020 2020 7461 736b 5f72 6573 6f75        task_resou
-00012190: 7263 6573 2e63 6c6f 7564 293a 0a20 2020  rces.cloud):.   
-000121a0: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-000121b0: 650a 2020 2020 2020 2020 6861 735f 636c  e.        has_cl
-000121c0: 6f75 645f 6d65 7420 3d20 5472 7565 0a0a  oud_met = True..
-000121d0: 2020 2020 2020 2020 6f76 6572 7269 6465          override
-000121e0: 5f70 6172 616d 203d 207b 7d0a 2020 2020  _param = {}.    
-000121f0: 2020 2020 6966 2074 6173 6b5f 7265 736f      if task_reso
-00012200: 7572 6365 732e 636c 6f75 6420 6973 204e  urces.cloud is N
-00012210: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00012220: 206f 7665 7272 6964 655f 7061 7261 6d5b   override_param[
-00012230: 2763 6c6f 7564 275d 203d 206f 7269 6769  'cloud'] = origi
-00012240: 6e61 6c5f 636c 6f75 640a 2020 2020 2020  nal_cloud.      
-00012250: 2020 6966 2074 6173 6b5f 7265 736f 7572    if task_resour
-00012260: 6365 732e 7265 6769 6f6e 2069 7320 4e6f  ces.region is No
-00012270: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00012280: 6f76 6572 7269 6465 5f70 6172 616d 5b27  override_param['
-00012290: 7265 6769 6f6e 275d 203d 2068 616e 646c  region'] = handl
-000122a0: 652e 6c61 756e 6368 6564 5f72 6573 6f75  e.launched_resou
-000122b0: 7263 6573 2e72 6567 696f 6e0a 0a20 2020  rces.region..   
-000122c0: 2020 2020 2069 6620 6f76 6572 7269 6465       if override
-000122d0: 5f70 6172 616d 3a0a 2020 2020 2020 2020  _param:.        
-000122e0: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
-000122f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012300: 2066 274e 6f20 636c 6f75 642f 7265 6769   f'No cloud/regi
-00012310: 6f6e 2073 7065 6369 6669 6564 2066 6f72  on specified for
-00012320: 2074 6865 2074 6173 6b20 7b74 6173 6b5f   the task {task_
-00012330: 7265 736f 7572 6365 737d 2e20 5573 696e  resources}. Usin
-00012340: 6720 7468 6520 7361 6d65 2072 6567 696f  g the same regio
-00012350: 6e20 270a 2020 2020 2020 2020 2020 2020  n '.            
-00012360: 2020 2020 6627 6173 2073 6f75 7263 6520      f'as source 
-00012370: 636c 7573 7465 7220 7b63 6c75 7374 6572  cluster {cluster
-00012380: 5f6e 616d 6521 727d 3a20 270a 2020 2020  _name!r}: '.    
-00012390: 2020 2020 2020 2020 2020 2020 6627 7b68              f'{h
-000123a0: 616e 646c 652e 6c61 756e 6368 6564 5f72  andle.launched_r
-000123b0: 6573 6f75 7263 6573 2e63 6c6f 7564 7d27  esources.cloud}'
-000123c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000123d0: 2066 2728 7b68 616e 646c 652e 6c61 756e   f'({handle.laun
-000123e0: 6368 6564 5f72 6573 6f75 7263 6573 2e72  ched_resources.r
-000123f0: 6567 696f 6e7d 292e 2729 0a20 2020 2020  egion}).').     
-00012400: 2020 2020 2020 2068 6173 5f6f 7665 7272         has_overr
-00012410: 6964 6520 3d20 5472 7565 0a20 2020 2020  ide = True.     
-00012420: 2020 2074 6173 6b5f 7265 736f 7572 6365     task_resource
-00012430: 7320 3d20 7461 736b 5f72 6573 6f75 7263  s = task_resourc
-00012440: 6573 2e63 6f70 7928 2a2a 6f76 6572 7269  es.copy(**overri
-00012450: 6465 5f70 6172 616d 290a 2020 2020 2020  de_param).      
-00012460: 2020 6e65 775f 7461 736b 5f72 6573 6f75    new_task_resou
-00012470: 7263 6573 2e61 7070 656e 6428 7461 736b  rces.append(task
-00012480: 5f72 6573 6f75 7263 6573 290a 0a20 2020  _resources)..   
-00012490: 2069 6620 6e6f 7420 6e65 775f 7461 736b   if not new_task
-000124a0: 5f72 6573 6f75 7263 6573 3a0a 2020 2020  _resources:.    
-000124b0: 2020 2020 6966 206e 6f74 2068 6173 5f64      if not has_d
-000124c0: 6973 6b5f 7369 7a65 5f6d 6574 3a0a 2020  isk_size_met:.  
-000124d0: 2020 2020 2020 2020 2020 7769 7468 2075            with u
-000124e0: 785f 7574 696c 732e 7072 696e 745f 6578  x_utils.print_ex
-000124f0: 6365 7074 696f 6e5f 6e6f 5f74 7261 6365  ception_no_trace
-00012500: 6261 636b 2829 3a0a 2020 2020 2020 2020  back():.        
-00012510: 2020 2020 2020 2020 7461 7267 6574 5f63          target_c
-00012520: 6c75 7374 6572 5f6e 616d 655f 7374 7220  luster_name_str 
-00012530: 3d20 6627 207b 7461 7267 6574 5f63 6c75  = f' {target_clu
-00012540: 7374 6572 5f6e 616d 6521 727d 270a 2020  ster_name!r}'.  
-00012550: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00012560: 2074 6172 6765 745f 636c 7573 7465 725f   target_cluster_
-00012570: 6e61 6d65 2069 7320 4e6f 6e65 3a0a 2020  name is None:.  
-00012580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012590: 2020 7461 7267 6574 5f63 6c75 7374 6572    target_cluster
-000125a0: 5f6e 616d 655f 7374 7220 3d20 2727 0a20  _name_str = ''. 
-000125b0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000125c0: 6169 7365 2065 7863 6570 7469 6f6e 732e  aise exceptions.
-000125d0: 4e6f 7453 7570 706f 7274 6564 4572 726f  NotSupportedErro
-000125e0: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-000125f0: 2020 2020 2020 2066 2754 6865 2074 6172         f'The tar
-00012600: 6765 7420 636c 7573 7465 727b 7461 7267  get cluster{targ
-00012610: 6574 5f63 6c75 7374 6572 5f6e 616d 655f  et_cluster_name_
-00012620: 7374 727d 2073 686f 756c 6420 6861 7665  str} should have
-00012630: 2061 2064 6973 6b20 7369 7a65 2027 0a20   a disk size '. 
-00012640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012650: 2020 2066 276f 6620 6174 206c 6561 7374     f'of at least
-00012660: 207b 6861 6e64 6c65 2e6c 6175 6e63 6865   {handle.launche
-00012670: 645f 7265 736f 7572 6365 732e 6469 736b  d_resources.disk
-00012680: 5f73 697a 657d 2047 4220 746f 2063 6c6f  _size} GB to clo
-00012690: 6e65 2074 6865 2027 0a20 2020 2020 2020  ne the '.       
-000126a0: 2020 2020 2020 2020 2020 2020 2066 2764               f'd
-000126b0: 6973 6b20 6672 6f6d 207b 636c 7573 7465  isk from {cluste
-000126c0: 725f 6e61 6d65 2172 7d2e 2729 0a20 2020  r_name!r}.').   
-000126d0: 2020 2020 2069 6620 6e6f 7420 6861 735f       if not has_
-000126e0: 636c 6f75 645f 6d65 743a 0a20 2020 2020  cloud_met:.     
-000126f0: 2020 2020 2020 2074 6173 6b5f 7265 736f         task_reso
-00012700: 7572 6365 735f 636c 6f75 645f 7374 7220  urces_cloud_str 
-00012710: 3d20 275b 2720 2b20 272c 272e 6a6f 696e  = '[' + ','.join
-00012720: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00012730: 2020 5b66 277b 7265 732e 636c 6f75 647d    [f'{res.cloud}
-00012740: 2720 666f 7220 7265 7320 696e 2074 6173  ' for res in tas
-00012750: 6b2e 7265 736f 7572 6365 735d 2920 2b20  k.resources]) + 
-00012760: 275d 270a 2020 2020 2020 2020 2020 2020  ']'.            
-00012770: 7461 736b 5f72 6573 6f75 7263 6573 5f73  task_resources_s
-00012780: 7472 203d 2027 5b27 202b 2027 2c27 2e6a  tr = '[' + ','.j
-00012790: 6f69 6e28 0a20 2020 2020 2020 2020 2020  oin(.           
-000127a0: 2020 2020 205b 6627 7b72 6573 7d27 2066       [f'{res}' f
-000127b0: 6f72 2072 6573 2069 6e20 7461 736b 2e72  or res in task.r
-000127c0: 6573 6f75 7263 6573 5d29 202b 2027 5d27  esources]) + ']'
-000127d0: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
-000127e0: 6820 7578 5f75 7469 6c73 2e70 7269 6e74  h ux_utils.print
-000127f0: 5f65 7863 6570 7469 6f6e 5f6e 6f5f 7472  _exception_no_tr
-00012800: 6163 6562 6163 6b28 293a 0a20 2020 2020  aceback():.     
-00012810: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00012820: 2056 616c 7565 4572 726f 7228 0a20 2020   ValueError(.   
-00012830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012840: 2066 2743 616e 6e6f 7420 636c 6f6e 6520   f'Cannot clone 
-00012850: 6469 736b 2061 6372 6f73 7320 636c 6f75  disk across clou
-00012860: 6420 6672 6f6d 207b 6f72 6967 696e 616c  d from {original
-00012870: 5f63 6c6f 7564 7d20 746f 2027 0a20 2020  _cloud} to '.   
-00012880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012890: 2066 277b 7461 736b 5f72 6573 6f75 7263   f'{task_resourc
-000128a0: 6573 5f63 6c6f 7564 5f73 7472 7d20 666f  es_cloud_str} fo
-000128b0: 7220 7265 736f 7572 6365 7320 7b74 6173  r resources {tas
-000128c0: 6b5f 7265 736f 7572 6365 735f 7374 727d  k_resources_str}
-000128d0: 2e27 0a20 2020 2020 2020 2020 2020 2020  .'.             
-000128e0: 2020 2029 0a20 2020 2020 2020 2061 7373     ).        ass
-000128f0: 6572 7420 4661 6c73 652c 2027 5368 6f75  ert False, 'Shou
-00012900: 6c64 206e 6f74 2072 6561 6368 2068 6572  ld not reach her
-00012910: 652e 270a 2020 2020 2320 7365 7420 7468  e.'.    # set th
-00012920: 6520 6e65 775f 7461 736b 5f72 6573 6f75  e new_task_resou
-00012930: 7263 6573 2074 6f20 6265 2074 6865 2073  rces to be the s
-00012940: 616d 6520 7479 7065 2028 6c69 7374 206f  ame type (list o
-00012950: 7220 7365 7429 2061 7320 7468 650a 2020  r set) as the.  
-00012960: 2020 2320 6f72 6967 696e 616c 2074 6173    # original tas
-00012970: 6b2e 7265 736f 7572 6365 730a 2020 2020  k.resources.    
-00012980: 6966 2068 6173 5f6f 7665 7272 6964 653a  if has_override:
-00012990: 0a20 2020 2020 2020 2074 6173 6b2e 7365  .        task.se
-000129a0: 745f 7265 736f 7572 6365 7328 7479 7065  t_resources(type
-000129b0: 2874 6173 6b2e 7265 736f 7572 6365 7329  (task.resources)
-000129c0: 286e 6577 5f74 6173 6b5f 7265 736f 7572  (new_task_resour
-000129d0: 6365 7329 290a 2020 2020 2020 2020 2320  ces)).        # 
-000129e0: 5265 7365 7420 7468 6520 6265 7374 5f72  Reset the best_r
-000129f0: 6573 6f75 7263 6573 2074 6f20 7472 6967  esources to trig
-00012a00: 6572 2072 652d 6f70 7469 6d69 7a61 7469  er re-optimizati
-00012a10: 6f6e 0a20 2020 2020 2020 2023 206c 6174  on.        # lat
-00012a20: 6572 2c20 736f 2074 6861 7420 7468 6520  er, so that the 
-00012a30: 6e65 7720 7461 736b 5f72 6573 6f75 7263  new task_resourc
-00012a40: 6573 2077 696c 6c20 6265 2075 7365 642e  es will be used.
-00012a50: 0a20 2020 2020 2020 2074 6173 6b2e 6265  .        task.be
-00012a60: 7374 5f72 6573 6f75 7263 6573 203d 204e  st_resources = N
-00012a70: 6f6e 650a 2020 2020 7265 7475 726e 2074  one.    return t
-00012a80: 6173 6b2c 2068 616e 646c 650a 0a0a 6465  ask, handle...de
-00012a90: 6620 5f75 7064 6174 655f 636c 7573 7465  f _update_cluste
-00012aa0: 725f 7374 6174 7573 5f6e 6f5f 6c6f 636b  r_status_no_lock
-00012ab0: 280a 2020 2020 2020 2020 636c 7573 7465  (.        cluste
-00012ac0: 725f 6e61 6d65 3a20 7374 7229 202d 3e20  r_name: str) -> 
-00012ad0: 4f70 7469 6f6e 616c 5b44 6963 745b 7374  Optional[Dict[st
-00012ae0: 722c 2041 6e79 5d5d 3a0a 2020 2020 2222  r, Any]]:.    ""
-00012af0: 2255 7064 6174 6573 2074 6865 2073 7461  "Updates the sta
-00012b00: 7475 7320 6f66 2074 6865 2063 6c75 7374  tus of the clust
-00012b10: 6572 2e0a 0a20 2020 2052 6169 7365 733a  er...    Raises:
-00012b20: 0a20 2020 2020 2020 2065 7863 6570 7469  .        excepti
-00012b30: 6f6e 732e 436c 7573 7465 7253 7461 7475  ons.ClusterStatu
-00012b40: 7346 6574 6368 696e 6745 7272 6f72 3a20  sFetchingError: 
-00012b50: 7468 6520 636c 7573 7465 7220 7374 6174  the cluster stat
-00012b60: 7573 2063 616e 6e6f 7420 6265 0a20 2020  us cannot be.   
-00012b70: 2020 2020 2020 2066 6574 6368 6564 2066         fetched f
-00012b80: 726f 6d20 7468 6520 636c 6f75 6420 7072  rom the cloud pr
-00012b90: 6f76 6964 6572 2e0a 2020 2020 2222 220a  ovider..    """.
-00012ba0: 2020 2020 7265 636f 7264 203d 2067 6c6f      record = glo
-00012bb0: 6261 6c5f 7573 6572 5f73 7461 7465 2e67  bal_user_state.g
-00012bc0: 6574 5f63 6c75 7374 6572 5f66 726f 6d5f  et_cluster_from_
-00012bd0: 6e61 6d65 2863 6c75 7374 6572 5f6e 616d  name(cluster_nam
-00012be0: 6529 0a20 2020 2069 6620 7265 636f 7264  e).    if record
-00012bf0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00012c00: 2020 7265 7475 726e 204e 6f6e 650a 2020    return None.  
-00012c10: 2020 6861 6e64 6c65 203d 2072 6563 6f72    handle = recor
-00012c20: 645b 2768 616e 646c 6527 5d0a 2020 2020  d['handle'].    
-00012c30: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
-00012c40: 6528 6861 6e64 6c65 2c20 6261 636b 656e  e(handle, backen
-00012c50: 6473 2e43 6c6f 7564 566d 5261 7952 6573  ds.CloudVmRayRes
-00012c60: 6f75 7263 6548 616e 646c 6529 3a0a 2020  ourceHandle):.  
-00012c70: 2020 2020 2020 7265 7475 726e 2072 6563        return rec
-00012c80: 6f72 640a 2020 2020 636c 7573 7465 725f  ord.    cluster_
-00012c90: 6e61 6d65 203d 2068 616e 646c 652e 636c  name = handle.cl
-00012ca0: 7573 7465 725f 6e61 6d65 0a0a 2020 2020  uster_name..    
-00012cb0: 6e6f 6465 5f73 7461 7475 7365 7320 3d20  node_statuses = 
-00012cc0: 5f71 7565 7279 5f63 6c75 7374 6572 5f73  _query_cluster_s
-00012cd0: 7461 7475 735f 7669 615f 636c 6f75 645f  tatus_via_cloud_
-00012ce0: 6170 6928 6861 6e64 6c65 290a 0a20 2020  api(handle)..   
-00012cf0: 2061 6c6c 5f6e 6f64 6573 5f75 7020 3d20   all_nodes_up = 
-00012d00: 2861 6c6c 280a 2020 2020 2020 2020 7374  (all(.        st
-00012d10: 6174 7573 203d 3d20 7374 6174 7573 5f6c  atus == status_l
-00012d20: 6962 2e43 6c75 7374 6572 5374 6174 7573  ib.ClusterStatus
-00012d30: 2e55 5020 666f 7220 7374 6174 7573 2069  .UP for status i
-00012d40: 6e20 6e6f 6465 5f73 7461 7475 7365 7329  n node_statuses)
-00012d50: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
-00012d60: 2020 2020 2020 2020 206c 656e 286e 6f64           len(nod
-00012d70: 655f 7374 6174 7573 6573 2920 3d3d 2068  e_statuses) == h
-00012d80: 616e 646c 652e 6c61 756e 6368 6564 5f6e  andle.launched_n
-00012d90: 6f64 6573 290a 0a20 2020 2064 6566 2072  odes)..    def r
-00012da0: 756e 5f72 6179 5f73 7461 7475 735f 746f  un_ray_status_to
-00012db0: 5f63 6865 636b 5f72 6179 5f63 6c75 7374  _check_ray_clust
-00012dc0: 6572 5f68 6561 6c74 6879 2829 202d 3e20  er_healthy() -> 
-00012dd0: 626f 6f6c 3a0a 2020 2020 2020 2020 7472  bool:.        tr
-00012de0: 793a 0a20 2020 2020 2020 2020 2020 2023  y:.            #
-00012df0: 204e 4f54 453a 2066 6574 6368 696e 6720   NOTE: fetching 
-00012e00: 7468 6520 4950 7320 6973 2076 6572 7920  the IPs is very 
-00012e10: 736c 6f77 2061 7320 6974 2063 616c 6c73  slow as it calls
-00012e20: 2069 6e74 6f0a 2020 2020 2020 2020 2020   into.          
-00012e30: 2020 2320 6072 6179 2067 6574 2068 6561    # `ray get hea
-00012e40: 642d 6970 2f77 6f72 6b65 722d 6970 7360  d-ip/worker-ips`
-00012e50: 2e20 5573 696e 6720 6361 6368 6564 2049  . Using cached I
-00012e60: 5073 2069 7320 7361 6665 2062 6563 6175  Ps is safe becau
-00012e70: 7365 0a20 2020 2020 2020 2020 2020 2023  se.            #
-00012e80: 2069 6e20 7468 6520 776f 7273 7420 6361   in the worst ca
-00012e90: 7365 2077 6520 7469 6d65 206f 7574 2069  se we time out i
-00012ea0: 6e20 7468 6520 6072 6179 2073 7461 7475  n the `ray statu
-00012eb0: 7360 2053 5348 2063 6f6d 6d61 6e64 0a20  s` SSH command. 
-00012ec0: 2020 2020 2020 2020 2020 2023 2062 656c             # bel
-00012ed0: 6f77 2e0a 2020 2020 2020 2020 2020 2020  ow..            
-00012ee0: 7275 6e6e 6572 7320 3d20 6861 6e64 6c65  runners = handle
-00012ef0: 2e67 6574 5f63 6f6d 6d61 6e64 5f72 756e  .get_command_run
-00012f00: 6e65 7273 2866 6f72 6365 5f63 6163 6865  ners(force_cache
-00012f10: 643d 5472 7565 290a 2020 2020 2020 2020  d=True).        
-00012f20: 2020 2020 2320 5468 6973 2068 6170 7065      # This happe
-00012f30: 6e73 2077 6865 6e20 7573 6572 2069 6e74  ns when user int
-00012f40: 6572 7275 7074 2074 6865 2060 736b 7920  errupt the `sky 
-00012f50: 6c61 756e 6368 6020 7072 6f63 6573 7320  launch` process 
-00012f60: 6265 666f 7265 0a20 2020 2020 2020 2020  before.         
-00012f70: 2020 2023 2074 6865 2066 6972 7374 2074     # the first t
-00012f80: 696d 6520 7265 736f 7572 6365 7320 6861  ime resources ha
-00012f90: 6e64 6c65 2069 7320 7772 6974 7465 6e20  ndle is written 
-00012fa0: 6261 636b 2074 6f20 6c6f 6361 6c20 6461  back to local da
-00012fb0: 7461 6261 7365 2e0a 2020 2020 2020 2020  tabase..        
-00012fc0: 2020 2020 2320 5468 6973 2069 7320 6865      # This is he
-00012fd0: 6c70 6675 6c20 7768 656e 2075 7365 7220  lpful when user 
-00012fe0: 696e 7465 7272 7570 7420 6166 7465 7220  interrupt after 
-00012ff0: 7468 6520 7072 6f76 6973 696f 6e20 6973  the provision is
-00013000: 2064 6f6e 650a 2020 2020 2020 2020 2020   done.          
-00013010: 2020 2320 616e 6420 6265 666f 7265 2074    # and before t
-00013020: 6865 2073 6b79 6c65 7420 6973 2072 6573  he skylet is res
-00013030: 7461 7274 6564 2e20 4166 7465 7220 2332  tarted. After #2
-00013040: 3330 3420 6973 206d 6572 6765 642c 2074  304 is merged, t
-00013050: 6869 730a 2020 2020 2020 2020 2020 2020  his.            
-00013060: 2320 6865 6c70 7320 6b65 6570 2074 6865  # helps keep the
-00013070: 2063 6c75 7374 6572 2073 7461 7475 7320   cluster status 
-00013080: 746f 2049 4e49 5420 6166 7465 7220 6073  to INIT after `s
-00013090: 6b79 2073 7461 7475 7320 2d72 602c 2073  ky status -r`, s
-000130a0: 6f0a 2020 2020 2020 2020 2020 2020 2320  o.            # 
-000130b0: 7573 6572 2077 696c 6c20 6265 206e 6f74  user will be not
-000130c0: 6966 6965 6420 7468 6174 2061 6e79 2061  ified that any a
-000130d0: 7574 6f20 7374 6f70 2f64 6f77 6e20 6d69  uto stop/down mi
-000130e0: 6768 7420 6e6f 7420 6265 0a20 2020 2020  ght not be.     
-000130f0: 2020 2020 2020 2023 2074 7269 6767 6572         # trigger
-00013100: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
-00013110: 6966 206e 6f74 2072 756e 6e65 7273 3a0a  if not runners:.
-00013120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013130: 6c6f 6767 6572 2e64 6562 7567 2866 2752  logger.debug(f'R
-00013140: 6566 7265 7368 696e 6720 7374 6174 7573  efreshing status
-00013150: 2028 7b63 6c75 7374 6572 5f6e 616d 6521   ({cluster_name!
-00013160: 727d 293a 204e 6f20 6361 6368 6564 2027  r}): No cached '
-00013170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013180: 2020 2020 2020 2020 2020 2020 2020 6627                f'
-00013190: 4950 7320 666f 756e 642e 2048 616e 646c  IPs found. Handl
-000131a0: 653a 207b 6861 6e64 6c65 7d27 290a 2020  e: {handle}').  
-000131b0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-000131c0: 6973 6520 6578 6365 7074 696f 6e73 2e46  ise exceptions.F
-000131d0: 6574 6368 436c 7573 7465 7249 6e66 6f45  etchClusterInfoE
-000131e0: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
-000131f0: 2020 2020 2020 2020 2020 7265 6173 6f6e            reason
-00013200: 3d65 7863 6570 7469 6f6e 732e 4665 7463  =exceptions.Fetc
-00013210: 6843 6c75 7374 6572 496e 666f 4572 726f  hClusterInfoErro
-00013220: 722e 5265 6173 6f6e 2e48 4541 4429 0a20  r.Reason.HEAD). 
-00013230: 2020 2020 2020 2020 2020 2068 6561 645f             head_
-00013240: 7275 6e6e 6572 203d 2072 756e 6e65 7273  runner = runners
-00013250: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
-00013260: 7263 2c20 6f75 7470 7574 2c20 7374 6465  rc, output, stde
-00013270: 7272 203d 2068 6561 645f 7275 6e6e 6572  rr = head_runner
-00013280: 2e72 756e 280a 2020 2020 2020 2020 2020  .run(.          
-00013290: 2020 2020 2020 696e 7374 616e 6365 5f73        instance_s
-000132a0: 6574 7570 2e52 4159 5f53 5441 5455 535f  etup.RAY_STATUS_
-000132b0: 5749 5448 5f53 4b59 5f52 4159 5f50 4f52  WITH_SKY_RAY_POR
-000132c0: 545f 434f 4d4d 414e 442c 0a20 2020 2020  T_COMMAND,.     
-000132d0: 2020 2020 2020 2020 2020 2073 7472 6561             strea
-000132e0: 6d5f 6c6f 6773 3d46 616c 7365 2c0a 2020  m_logs=False,.  
-000132f0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00013300: 7175 6972 655f 6f75 7470 7574 733d 5472  quire_outputs=Tr
-00013310: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00013320: 2020 2020 7365 7061 7261 7465 5f73 7464      separate_std
-00013330: 6572 723d 5472 7565 290a 2020 2020 2020  err=True).      
-00013340: 2020 2020 2020 6966 2072 633a 0a20 2020        if rc:.   
-00013350: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-00013360: 7365 2052 756e 7469 6d65 4572 726f 7228  se RuntimeError(
-00013370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013380: 2020 2020 2066 2752 6566 7265 7368 696e       f'Refreshin
-00013390: 6720 7374 6174 7573 2028 7b63 6c75 7374  g status ({clust
-000133a0: 6572 5f6e 616d 6521 727d 293a 2046 6169  er_name!r}): Fai
-000133b0: 6c65 6420 746f 2063 6865 636b 2027 0a20  led to check '. 
-000133c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133d0: 2020 2066 2772 6179 2063 6c75 7374 6572     f'ray cluster
-000133e0: 5c27 7320 6865 616c 7468 696e 6573 7320  \'s healthiness 
-000133f0: 7769 7468 2027 0a20 2020 2020 2020 2020  with '.         
-00013400: 2020 2020 2020 2020 2020 2066 277b 696e             f'{in
-00013410: 7374 616e 6365 5f73 6574 7570 2e52 4159  stance_setup.RAY
-00013420: 5f53 5441 5455 535f 5749 5448 5f53 4b59  _STATUS_WITH_SKY
-00013430: 5f52 4159 5f50 4f52 545f 434f 4d4d 414e  _RAY_PORT_COMMAN
-00013440: 447d 2e5c 6e27 0a20 2020 2020 2020 2020  D}.\n'.         
-00013450: 2020 2020 2020 2020 2020 2066 272d 2d20             f'-- 
-00013460: 7374 646f 7574 202d 2d5c 6e7b 6f75 7470  stdout --\n{outp
-00013470: 7574 7d5c 6e2d 2d20 7374 6465 7272 202d  ut}\n-- stderr -
-00013480: 2d5c 6e7b 7374 6465 7272 7d27 290a 0a20  -\n{stderr}').. 
-00013490: 2020 2020 2020 2020 2020 2072 6561 6479             ready
-000134a0: 5f68 6561 642c 2072 6561 6479 5f77 6f72  _head, ready_wor
-000134b0: 6b65 7273 203d 205f 636f 756e 745f 6865  kers = _count_he
-000134c0: 616c 7468 795f 6e6f 6465 735f 6672 6f6d  althy_nodes_from
-000134d0: 5f72 6179 286f 7574 7075 7429 0a20 2020  _ray(output).   
-000134e0: 2020 2020 2020 2020 2074 6f74 616c 5f6e           total_n
-000134f0: 6f64 6573 203d 2068 616e 646c 652e 6c61  odes = handle.la
-00013500: 756e 6368 6564 5f6e 6f64 6573 202a 2068  unched_nodes * h
-00013510: 616e 646c 652e 6e75 6d5f 6970 735f 7065  andle.num_ips_pe
-00013520: 725f 6e6f 6465 0a20 2020 2020 2020 2020  r_node.         
-00013530: 2020 2069 6620 7265 6164 795f 6865 6164     if ready_head
-00013540: 202b 2072 6561 6479 5f77 6f72 6b65 7273   + ready_workers
-00013550: 203d 3d20 746f 7461 6c5f 6e6f 6465 733a   == total_nodes:
-00013560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013570: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
-00013580: 2020 2020 2020 2020 2072 6169 7365 2052           raise R
-00013590: 756e 7469 6d65 4572 726f 7228 0a20 2020  untimeError(.   
-000135a0: 2020 2020 2020 2020 2020 2020 2066 2752               f'R
-000135b0: 6566 7265 7368 696e 6720 7374 6174 7573  efreshing status
-000135c0: 2028 7b63 6c75 7374 6572 5f6e 616d 6521   ({cluster_name!
-000135d0: 727d 293a 2072 6179 2073 7461 7475 7320  r}): ray status 
-000135e0: 6e6f 7420 7368 6f77 696e 6720 270a 2020  not showing '.  
-000135f0: 2020 2020 2020 2020 2020 2020 2020 6627                f'
-00013600: 616c 6c20 6e6f 6465 7320 287b 7265 6164  all nodes ({read
-00013610: 795f 6865 6164 202b 2072 6561 6479 5f77  y_head + ready_w
-00013620: 6f72 6b65 7273 7d2f 270a 2020 2020 2020  orkers}/'.      
-00013630: 2020 2020 2020 2020 2020 6627 7b74 6f74            f'{tot
-00013640: 616c 5f6e 6f64 6573 7d29 3b20 6f75 7470  al_nodes}); outp
-00013650: 7574 3a20 7b6f 7574 7075 747d 3b20 7374  ut: {output}; st
-00013660: 6465 7272 3a20 7b73 7464 6572 727d 2729  derr: {stderr}')
-00013670: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-00013680: 6578 6365 7074 696f 6e73 2e46 6574 6368  exceptions.Fetch
-00013690: 436c 7573 7465 7249 6e66 6f45 7272 6f72  ClusterInfoError
-000136a0: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
-000136b0: 6767 6572 2e64 6562 7567 280a 2020 2020  gger.debug(.    
-000136c0: 2020 2020 2020 2020 2020 2020 6627 5265              f'Re
-000136d0: 6672 6573 6869 6e67 2073 7461 7475 7320  freshing status 
-000136e0: 287b 636c 7573 7465 725f 6e61 6d65 2172  ({cluster_name!r
-000136f0: 7d29 2066 6169 6c65 6420 746f 2067 6574  }) failed to get
-00013700: 2049 5073 2e27 290a 2020 2020 2020 2020   IPs.').        
-00013710: 6578 6365 7074 2052 756e 7469 6d65 4572  except RuntimeEr
-00013720: 726f 7220 6173 2065 3a0a 2020 2020 2020  ror as e:.      
-00013730: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-00013740: 7567 2873 7472 2865 2929 0a20 2020 2020  ug(str(e)).     
-00013750: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-00013760: 696f 6e20 6173 2065 3a20 2023 2070 796c  ion as e:  # pyl
-00013770: 696e 743a 2064 6973 6162 6c65 3d62 726f  int: disable=bro
-00013780: 6164 2d65 7863 6570 740a 2020 2020 2020  ad-except.      
-00013790: 2020 2020 2020 2320 5468 6973 2063 616e        # This can
-000137a0: 2062 6520 7261 6973 6564 2062 7920 6065   be raised by `e
-000137b0: 7874 6572 6e61 6c5f 7373 685f 706f 7274  xternal_ssh_port
-000137c0: 7328 2960 2c20 6475 6520 746f 2074 6865  s()`, due to the
-000137d0: 0a20 2020 2020 2020 2020 2020 2023 2075  .            # u
-000137e0: 6e64 6572 6c79 696e 6720 6361 6c6c 2074  nderlying call t
-000137f0: 6f20 6b75 6265 726e 6574 6573 2041 5049  o kubernetes API
-00013800: 2e0a 2020 2020 2020 2020 2020 2020 6c6f  ..            lo
-00013810: 6767 6572 2e64 6562 7567 280a 2020 2020  gger.debug(.    
-00013820: 2020 2020 2020 2020 2020 2020 6627 5265              f'Re
-00013830: 6672 6573 6869 6e67 2073 7461 7475 7320  freshing status 
-00013840: 287b 636c 7573 7465 725f 6e61 6d65 2172  ({cluster_name!r
-00013850: 7d29 2066 6169 6c65 643a 2027 0a20 2020  }) failed: '.   
-00013860: 2020 2020 2020 2020 2020 2020 2066 277b               f'{
-00013870: 636f 6d6d 6f6e 5f75 7469 6c73 2e66 6f72  common_utils.for
-00013880: 6d61 745f 6578 6365 7074 696f 6e28 652c  mat_exception(e,
-00013890: 2075 7365 5f62 7261 636b 6574 3d54 7275   use_bracket=Tru
-000138a0: 6529 7d27 290a 2020 2020 2020 2020 7265  e)}').        re
-000138b0: 7475 726e 2046 616c 7365 0a0a 2020 2020  turn False..    
-000138c0: 2320 4465 7465 726d 696e 696e 6720 6966  # Determining if
-000138d0: 2074 6865 2063 6c75 7374 6572 2069 7320   the cluster is 
-000138e0: 6865 616c 7468 7920 2855 5029 3a0a 2020  healthy (UP):.  
-000138f0: 2020 230a 2020 2020 2320 466f 7220 6e6f    #.    # For no
-00013900: 6e2d 7370 6f74 2063 6c75 7374 6572 733a  n-spot clusters:
-00013910: 2049 6620 7261 7920 7374 6174 7573 2073   If ray status s
-00013920: 686f 7773 2061 6c6c 206e 6f64 6573 2061  hows all nodes a
-00013930: 7265 2068 6561 6c74 6879 2c20 6974 2069  re healthy, it i
-00013940: 730a 2020 2020 2320 7361 6665 2074 6f20  s.    # safe to 
-00013950: 7365 7420 7468 6520 7374 6174 7573 2074  set the status t
-00013960: 6f20 5550 2061 7320 7374 6172 7469 6e67  o UP as starting
-00013970: 2072 6179 2069 7320 7468 6520 6669 6e61   ray is the fina
-00013980: 6c20 7374 6570 206f 6620 736b 790a 2020  l step of sky.  
-00013990: 2020 2320 6c61 756e 6368 2e20 4275 7420    # launch. But 
-000139a0: 7765 2066 6f75 6e64 2074 6861 7420 7261  we found that ra
-000139b0: 7920 7374 6174 7573 2069 7320 7761 7920  y status is way 
-000139c0: 746f 6f20 736c 6f77 2028 7365 6520 4e4f  too slow (see NO
-000139d0: 5445 2062 656c 6f77 2920 736f 0a20 2020  TE below) so.   
-000139e0: 2023 2077 6520 616c 7761 7973 2071 7565   # we always que
-000139f0: 7279 2074 6865 2063 6c6f 7564 2070 726f  ry the cloud pro
-00013a00: 7669 6465 7220 6669 7273 7420 7768 6963  vider first whic
-00013a10: 6820 6973 2066 6173 7465 722e 0a20 2020  h is faster..   
-00013a20: 2023 0a20 2020 2023 2046 6f72 2073 706f   #.    # For spo
-00013a30: 7420 636c 7573 7465 7273 3a20 7468 6520  t clusters: the 
-00013a40: 6162 6f76 6520 6361 6e20 6265 2075 6e73  above can be uns
-00013a50: 6166 6520 6265 6361 7573 6520 7468 6520  afe because the 
-00013a60: 5261 7920 636c 7573 7465 7220 6d61 790a  Ray cluster may.
-00013a70: 2020 2020 2320 7265 6d61 696e 2068 6561      # remain hea
-00013a80: 6c74 6879 2066 6f72 2061 2077 6869 6c65  lthy for a while
-00013a90: 2062 6566 6f72 6520 7468 6520 636c 6f75   before the clou
-00013aa0: 6420 636f 6d70 6c65 7465 6c79 2070 7265  d completely pre
-00013ab0: 656d 7074 7320 7468 6520 564d 732e 0a20  empts the VMs.. 
-00013ac0: 2020 2023 2057 6520 6861 7665 206d 6974     # We have mit
-00013ad0: 6967 6174 6564 2074 6869 7320 6279 2061  igated this by a
-00013ae0: 6761 696e 2066 6972 7374 2071 7565 7279  gain first query
-00013af0: 696e 6720 7468 6520 564d 2073 7461 7465  ing the VM state
-00013b00: 2066 726f 6d20 7468 6520 636c 6f75 640a   from the cloud.
-00013b10: 2020 2020 2320 7072 6f76 6964 6572 2e0a      # provider..
-00013b20: 2020 2020 6966 2061 6c6c 5f6e 6f64 6573      if all_nodes
-00013b30: 5f75 7020 616e 6420 7275 6e5f 7261 795f  _up and run_ray_
-00013b40: 7374 6174 7573 5f74 6f5f 6368 6563 6b5f  status_to_check_
-00013b50: 7261 795f 636c 7573 7465 725f 6865 616c  ray_cluster_heal
-00013b60: 7468 7928 293a 0a20 2020 2020 2020 2023  thy():.        #
-00013b70: 204e 4f54 453a 2061 6c6c 5f6e 6f64 6573   NOTE: all_nodes
-00013b80: 5f75 7020 6361 6c63 756c 6174 696f 6e20  _up calculation 
-00013b90: 6973 2066 6173 7420 6475 6520 746f 2063  is fast due to c
-00013ba0: 616c 6c69 6e67 2063 6c6f 7564 2043 4c49  alling cloud CLI
-00013bb0: 3b0a 2020 2020 2020 2020 2320 7275 6e5f  ;.        # run_
-00013bc0: 7261 795f 7374 6174 7573 5f74 6f5f 6368  ray_status_to_ch
-00013bd0: 6563 6b5f 616c 6c5f 6e6f 6465 735f 7570  eck_all_nodes_up
-00013be0: 2829 2069 7320 736c 6f77 2064 7565 2074  () is slow due t
-00013bf0: 6f20 6361 6c6c 696e 6720 6072 6179 2067  o calling `ray g
-00013c00: 6574 0a20 2020 2020 2020 2023 2068 6561  et.        # hea
-00013c10: 642d 6970 2f77 6f72 6b65 722d 6970 7360  d-ip/worker-ips`
-00013c20: 2e0a 2020 2020 2020 2020 7265 636f 7264  ..        record
-00013c30: 5b27 7374 6174 7573 275d 203d 2073 7461  ['status'] = sta
-00013c40: 7475 735f 6c69 622e 436c 7573 7465 7253  tus_lib.ClusterS
-00013c50: 7461 7475 732e 5550 0a20 2020 2020 2020  tatus.UP.       
-00013c60: 2067 6c6f 6261 6c5f 7573 6572 5f73 7461   global_user_sta
-00013c70: 7465 2e61 6464 5f6f 725f 7570 6461 7465  te.add_or_update
-00013c80: 5f63 6c75 7374 6572 2863 6c75 7374 6572  _cluster(cluster
-00013c90: 5f6e 616d 652c 0a20 2020 2020 2020 2020  _name,.         
-00013ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105a0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+000105b0: 7573 6572 5f69 6465 6e74 6974 7929 293a  user_identity)):
+000105c0: 0a20 2020 2020 2020 2020 2020 2023 2043  .            # C
+000105d0: 6c65 616e 2075 7020 7468 6520 6f77 6e65  lean up the owne
+000105e0: 7220 6964 656e 7469 7479 2066 6f72 2074  r identity for t
+000105f0: 6865 2062 6163 6b73 6c61 7368 2061 6e64  he backslash and
+00010600: 206e 6577 6c69 6e65 732c 2063 6175 7365   newlines, cause
+00010610: 640a 2020 2020 2020 2020 2020 2020 2320  d.            # 
+00010620: 6279 2074 6865 2063 6c6f 7564 2043 4c49  by the cloud CLI
+00010630: 206f 7574 7075 742c 2065 2e67 2e20 6763   output, e.g. gc
+00010640: 6c6f 7564 2e0a 2020 2020 2020 2020 2020  loud..          
+00010650: 2020 6f77 6e65 7220 3d20 6f77 6e65 722e    owner = owner.
+00010660: 7265 706c 6163 6528 275c 6e27 2c20 2727  replace('\n', ''
+00010670: 292e 7265 706c 6163 6528 275c 5c27 2c20  ).replace('\\', 
+00010680: 2727 290a 2020 2020 2020 2020 2020 2020  '').            
+00010690: 6966 206f 776e 6572 203d 3d20 6375 7272  if owner == curr
+000106a0: 656e 743a 0a20 2020 2020 2020 2020 2020  ent:.           
+000106b0: 2020 2020 2069 6620 6920 213d 2030 3a0a       if i != 0:.
+000106c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000106d0: 2020 2020 6c6f 6767 6572 2e77 6172 6e69      logger.warni
+000106e0: 6e67 280a 2020 2020 2020 2020 2020 2020  ng(.            
+000106f0: 2020 2020 2020 2020 2020 2020 6627 5468              f'Th
+00010700: 6520 636c 7573 7465 7220 7761 7320 6f77  e cluster was ow
+00010710: 6e65 6420 6279 207b 6f77 6e65 725f 6964  ned by {owner_id
+00010720: 656e 7469 7479 7d2c 2062 7574 2027 0a20  entity}, but '. 
+00010730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010740: 2020 2020 2020 2066 2761 206e 6577 2069         f'a new i
+00010750: 6465 6e74 6974 7920 7b63 7572 7265 6e74  dentity {current
+00010760: 5f75 7365 725f 6964 656e 7469 7479 7d20  _user_identity} 
+00010770: 6973 2061 6374 6976 6174 6564 2e20 5765  is activated. We
+00010780: 2073 7469 6c6c 2027 0a20 2020 2020 2020   still '.       
+00010790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000107a0: 2027 616c 6c6f 7720 7468 6520 6f70 6572   'allow the oper
+000107b0: 6174 696f 6e20 6173 2074 6865 2074 776f  ation as the two
+000107c0: 2069 6465 6e74 6974 6965 7320 6172 6520   identities are 
+000107d0: 6c69 6b65 6c79 2074 6f20 6861 7665 2027  likely to have '
+000107e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000107f0: 2020 2020 2020 2020 2027 7468 6520 7361           'the sa
+00010800: 6d65 2061 6363 6573 7320 746f 2074 6865  me access to the
+00010810: 2063 6c75 7374 6572 2e20 506c 6561 7365   cluster. Please
+00010820: 2062 6520 6177 6172 6520 7468 6174 2074   be aware that t
+00010830: 6869 7320 6361 6e20 270a 2020 2020 2020  his can '.      
+00010840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010850: 2020 2763 6175 7365 2075 6e65 7870 6563    'cause unexpec
+00010860: 7465 6420 636c 7573 7465 7220 6c65 616b  ted cluster leak
+00010870: 6167 6520 6966 2074 6865 2074 776f 2069  age if the two i
+00010880: 6465 6e74 6974 6965 7320 6172 6520 6e6f  dentities are no
+00010890: 7420 270a 2020 2020 2020 2020 2020 2020  t '.            
+000108a0: 2020 2020 2020 2020 2020 2020 2761 6374              'act
+000108b0: 7561 6c6c 7920 6571 7569 7661 6c65 6e74  ually equivalent
+000108c0: 2028 652e 672e 2c20 6265 6c6f 6e67 2074   (e.g., belong t
+000108d0: 6f20 7468 6520 7361 6d65 2070 6572 736f  o the same perso
+000108e0: 6e29 2e27 0a20 2020 2020 2020 2020 2020  n).'.           
+000108f0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00010900: 2020 2020 2020 2020 2020 2069 6620 6920             if i 
+00010910: 213d 2030 206f 7220 6c65 6e28 6f77 6e65  != 0 or len(owne
+00010920: 725f 6964 656e 7469 7479 2920 213d 206c  r_identity) != l
+00010930: 656e 2863 7572 7265 6e74 5f75 7365 725f  en(current_user_
+00010940: 6964 656e 7469 7479 293a 0a20 2020 2020  identity):.     
+00010950: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00010960: 2057 6520 7570 6461 7465 2074 6865 206f   We update the o
+00010970: 776e 6572 206f 6620 6120 636c 7573 7465  wner of a cluste
+00010980: 722c 2077 6865 6e3a 0a20 2020 2020 2020  r, when:.       
+00010990: 2020 2020 2020 2020 2020 2020 2023 2031               # 1
+000109a0: 2e20 5468 6520 7374 7269 6374 6573 7420  . The strictest 
+000109b0: 6964 656e 7474 7920 2869 2e65 2e20 7468  identty (i.e. th
+000109c0: 6520 6669 7273 7420 6f6e 6529 2064 6f65  e first one) doe
+000109d0: 7320 6e6f 740a 2020 2020 2020 2020 2020  s not.          
+000109e0: 2020 2020 2020 2020 2020 2320 6d61 7463            # matc
+000109f0: 682c 2062 7574 2074 6865 206c 6174 7465  h, but the latte
+00010a00: 7220 6f6e 6573 206d 6174 6368 2e0a 2020  r ones match..  
+00010a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a20: 2020 2320 322e 2054 6865 206c 656e 6774    # 2. The lengt
+00010a30: 6820 6f66 2074 6865 2074 776f 2069 6465  h of the two ide
+00010a40: 6e74 6974 6965 7320 6172 6520 6469 6666  ntities are diff
+00010a50: 6572 656e 742c 2077 6869 6368 0a20 2020  erent, which.   
+00010a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a70: 2023 2077 696c 6c20 6f6e 6c79 2068 6170   # will only hap
+00010a80: 7065 6e20 7768 656e 2074 6865 2063 6c75  pen when the clu
+00010a90: 7374 6572 2069 7320 6c61 756e 6368 6564  ster is launched
+00010aa0: 2062 6566 6f72 6520 2331 3830 382e 0a20   before #1808.. 
+00010ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ac0: 2020 2023 2055 7064 6174 6520 7468 6520     # Update the 
+00010ad0: 7573 6572 2069 6465 6e74 6974 7920 746f  user identity to
+00010ae0: 2061 766f 6964 2073 686f 7769 6e67 2074   avoid showing t
+00010af0: 6865 2077 6172 6e69 6e67 2061 626f 7665  he warning above
+00010b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010b10: 2020 2020 2023 2061 6761 696e 2e0a 2020       # again..  
+00010b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b30: 2020 676c 6f62 616c 5f75 7365 725f 7374    global_user_st
+00010b40: 6174 652e 7365 745f 6f77 6e65 725f 6964  ate.set_owner_id
+00010b50: 656e 7469 7479 5f66 6f72 5f63 6c75 7374  entity_for_clust
+00010b60: 6572 280a 2020 2020 2020 2020 2020 2020  er(.            
+00010b70: 2020 2020 2020 2020 2020 2020 636c 7573              clus
+00010b80: 7465 725f 6e61 6d65 2c20 6375 7272 656e  ter_name, curren
+00010b90: 745f 7573 6572 5f69 6465 6e74 6974 7929  t_user_identity)
+00010ba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010bb0: 2072 6574 7572 6e20 2023 2054 6865 2075   return  # The u
+00010bc0: 7365 7220 6964 656e 7469 7479 206d 6174  ser identity mat
+00010bd0: 6368 6573 2e0a 2020 2020 2020 2020 7769  ches..        wi
+00010be0: 7468 2075 785f 7574 696c 732e 7072 696e  th ux_utils.prin
+00010bf0: 745f 6578 6365 7074 696f 6e5f 6e6f 5f74  t_exception_no_t
+00010c00: 7261 6365 6261 636b 2829 3a0a 2020 2020  raceback():.    
+00010c10: 2020 2020 2020 2020 7261 6973 6520 6578          raise ex
+00010c20: 6365 7074 696f 6e73 2e43 6c75 7374 6572  ceptions.Cluster
+00010c30: 4f77 6e65 7249 6465 6e74 6974 794d 6973  OwnerIdentityMis
+00010c40: 6d61 7463 6845 7272 6f72 280a 2020 2020  matchError(.    
+00010c50: 2020 2020 2020 2020 2020 2020 6627 7b63              f'{c
+00010c60: 6c75 7374 6572 5f6e 616d 6521 727d 2028  luster_name!r} (
+00010c70: 7b63 6c6f 7564 7d29 2069 7320 6f77 6e65  {cloud}) is owne
+00010c80: 6420 6279 2061 6363 6f75 6e74 2027 0a20  d by account '. 
+00010c90: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00010ca0: 277b 6f77 6e65 725f 6964 656e 7469 7479  '{owner_identity
+00010cb0: 2172 7d2c 2062 7574 2074 6865 2061 6374  !r}, but the act
+00010cc0: 6976 6174 6564 2061 6363 6f75 6e74 2027  ivated account '
+00010cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010ce0: 2066 2769 7320 7b63 7572 7265 6e74 5f75   f'is {current_u
+00010cf0: 7365 725f 6964 656e 7469 7479 2172 7d2e  ser_identity!r}.
+00010d00: 2729 0a0a 0a64 6566 2074 6167 5f66 696c  ')...def tag_fil
+00010d10: 7465 725f 666f 725f 636c 7573 7465 7228  ter_for_cluster(
+00010d20: 636c 7573 7465 725f 6e61 6d65 3a20 7374  cluster_name: st
+00010d30: 7229 202d 3e20 4469 6374 5b73 7472 2c20  r) -> Dict[str, 
+00010d40: 7374 725d 3a0a 2020 2020 2222 2252 6574  str]:.    """Ret
+00010d50: 7572 6e73 2061 2074 6167 2066 696c 7465  urns a tag filte
+00010d60: 7220 666f 7220 7468 6520 636c 7573 7465  r for the cluste
+00010d70: 722e 2222 220a 2020 2020 7265 7475 726e  r.""".    return
+00010d80: 207b 0a20 2020 2020 2020 2027 7261 792d   {.        'ray-
+00010d90: 636c 7573 7465 722d 6e61 6d65 273a 2063  cluster-name': c
+00010da0: 6c75 7374 6572 5f6e 616d 652c 0a20 2020  luster_name,.   
+00010db0: 207d 0a0a 0a64 6566 205f 7175 6572 795f   }...def _query_
+00010dc0: 636c 7573 7465 725f 7374 6174 7573 5f76  cluster_status_v
+00010dd0: 6961 5f63 6c6f 7564 5f61 7069 280a 2020  ia_cloud_api(.  
+00010de0: 2020 6861 6e64 6c65 3a20 2763 6c6f 7564    handle: 'cloud
+00010df0: 5f76 6d5f 7261 795f 6261 636b 656e 642e  _vm_ray_backend.
+00010e00: 436c 6f75 6456 6d52 6179 5265 736f 7572  CloudVmRayResour
+00010e10: 6365 4861 6e64 6c65 270a 2920 2d3e 204c  ceHandle'.) -> L
+00010e20: 6973 745b 7374 6174 7573 5f6c 6962 2e43  ist[status_lib.C
+00010e30: 6c75 7374 6572 5374 6174 7573 5d3a 0a20  lusterStatus]:. 
+00010e40: 2020 2022 2222 5265 7475 726e 7320 7468     """Returns th
+00010e50: 6520 7374 6174 7573 206f 6620 7468 6520  e status of the 
+00010e60: 636c 7573 7465 722e 0a0a 2020 2020 5261  cluster...    Ra
+00010e70: 6973 6573 3a0a 2020 2020 2020 2020 6578  ises:.        ex
+00010e80: 6365 7074 696f 6e73 2e43 6c75 7374 6572  ceptions.Cluster
+00010e90: 5374 6174 7573 4665 7463 6869 6e67 4572  StatusFetchingEr
+00010ea0: 726f 723a 2074 6865 2063 6c75 7374 6572  ror: the cluster
+00010eb0: 2073 7461 7475 7320 6361 6e6e 6f74 2062   status cannot b
+00010ec0: 650a 2020 2020 2020 2020 2020 6665 7463  e.          fetc
+00010ed0: 6865 6420 6672 6f6d 2074 6865 2063 6c6f  hed from the clo
+00010ee0: 7564 2070 726f 7669 6465 722e 0a20 2020  ud provider..   
+00010ef0: 2022 2222 0a20 2020 2063 6c75 7374 6572   """.    cluster
+00010f00: 5f6e 616d 655f 6f6e 5f63 6c6f 7564 203d  _name_on_cloud =
+00010f10: 2068 616e 646c 652e 636c 7573 7465 725f   handle.cluster_
+00010f20: 6e61 6d65 5f6f 6e5f 636c 6f75 640a 2020  name_on_cloud.  
+00010f30: 2020 636c 7573 7465 725f 6e61 6d65 5f69    cluster_name_i
+00010f40: 6e5f 6869 6e74 203d 2063 6f6d 6d6f 6e5f  n_hint = common_
+00010f50: 7574 696c 732e 636c 7573 7465 725f 6e61  utils.cluster_na
+00010f60: 6d65 5f69 6e5f 6869 6e74 280a 2020 2020  me_in_hint(.    
+00010f70: 2020 2020 6861 6e64 6c65 2e63 6c75 7374      handle.clust
+00010f80: 6572 5f6e 616d 652c 2063 6c75 7374 6572  er_name, cluster
+00010f90: 5f6e 616d 655f 6f6e 5f63 6c6f 7564 290a  _name_on_cloud).
+00010fa0: 2020 2020 2320 5573 6520 7265 6769 6f6e      # Use region
+00010fb0: 2061 6e64 207a 6f6e 6520 6672 6f6d 2074   and zone from t
+00010fc0: 6865 2063 6c75 7374 6572 2063 6f6e 6669  he cluster confi
+00010fd0: 672c 2069 6e73 7465 6164 206f 6620 7468  g, instead of th
+00010fe0: 650a 2020 2020 2320 6861 6e64 6c65 2e6c  e.    # handle.l
+00010ff0: 6175 6e63 6865 645f 7265 736f 7572 6365  aunched_resource
+00011000: 732c 2062 6563 6175 7365 2074 6865 206c  s, because the l
+00011010: 6174 7465 7220 6d61 7920 6e6f 7420 6265  atter may not be
+00011020: 2073 6574 0a20 2020 2023 2063 6f72 7265   set.    # corre
+00011030: 6374 6c79 2079 6574 2e0a 2020 2020 7261  ctly yet..    ra
+00011040: 795f 636f 6e66 6967 203d 2063 6f6d 6d6f  y_config = commo
+00011050: 6e5f 7574 696c 732e 7265 6164 5f79 616d  n_utils.read_yam
+00011060: 6c28 6861 6e64 6c65 2e63 6c75 7374 6572  l(handle.cluster
+00011070: 5f79 616d 6c29 0a20 2020 2070 726f 7669  _yaml).    provi
+00011080: 6465 725f 636f 6e66 6967 203d 2072 6179  der_config = ray
+00011090: 5f63 6f6e 6669 675b 2770 726f 7669 6465  _config['provide
+000110a0: 7227 5d0a 0a20 2020 2023 2051 7565 7279  r']..    # Query
+000110b0: 2074 6865 2063 6c6f 7564 2070 726f 7669   the cloud provi
+000110c0: 6465 722e 0a20 2020 2023 2054 4f44 4f28  der..    # TODO(
+000110d0: 7375 7175 6172 6b29 3a20 6d6f 7665 2069  suquark): move i
+000110e0: 6d70 6c65 6d65 6e74 6174 696f 6e73 206f  mplementations o
+000110f0: 6620 6d6f 7265 2063 6c6f 7564 7320 6865  f more clouds he
+00011100: 7265 0a20 2020 2063 6c6f 7564 203d 2068  re.    cloud = h
+00011110: 616e 646c 652e 6c61 756e 6368 6564 5f72  andle.launched_r
+00011120: 6573 6f75 7263 6573 2e63 6c6f 7564 0a20  esources.cloud. 
+00011130: 2020 2061 7373 6572 7420 636c 6f75 6420     assert cloud 
+00011140: 6973 206e 6f74 204e 6f6e 652c 2068 616e  is not None, han
+00011150: 646c 650a 2020 2020 6966 2063 6c6f 7564  dle.    if cloud
+00011160: 2e53 5441 5455 535f 5645 5253 494f 4e20  .STATUS_VERSION 
+00011170: 3e3d 2063 6c6f 7564 732e 5374 6174 7573  >= clouds.Status
+00011180: 5665 7273 696f 6e2e 534b 5950 494c 4f54  Version.SKYPILOT
+00011190: 3a0a 2020 2020 2020 2020 636c 6f75 645f  :.        cloud_
+000111a0: 6e61 6d65 203d 2072 6570 7228 6861 6e64  name = repr(hand
+000111b0: 6c65 2e6c 6175 6e63 6865 645f 7265 736f  le.launched_reso
+000111c0: 7572 6365 732e 636c 6f75 6429 0a20 2020  urces.cloud).   
+000111d0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+000111e0: 2020 2020 2020 6e6f 6465 5f73 7461 7475        node_statu
+000111f0: 735f 6469 6374 203d 2070 726f 7669 7369  s_dict = provisi
+00011200: 6f6e 5f6c 6962 2e71 7565 7279 5f69 6e73  on_lib.query_ins
+00011210: 7461 6e63 6573 280a 2020 2020 2020 2020  tances(.        
+00011220: 2020 2020 2020 2020 636c 6f75 645f 6e61          cloud_na
+00011230: 6d65 2c20 636c 7573 7465 725f 6e61 6d65  me, cluster_name
+00011240: 5f6f 6e5f 636c 6f75 642c 2070 726f 7669  _on_cloud, provi
+00011250: 6465 725f 636f 6e66 6967 290a 2020 2020  der_config).    
+00011260: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+00011270: 6562 7567 2866 2751 7565 7279 696e 6720  ebug(f'Querying 
+00011280: 7b63 6c6f 7564 5f6e 616d 657d 2063 6c75  {cloud_name} clu
+00011290: 7374 6572 2027 0a20 2020 2020 2020 2020  ster '.         
+000112a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112b0: 6627 7b63 6c75 7374 6572 5f6e 616d 655f  f'{cluster_name_
+000112c0: 696e 5f68 696e 747d 2027 0a20 2020 2020  in_hint} '.     
+000112d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112e0: 2020 2020 6627 7374 6174 7573 3a5c 6e7b      f'status:\n{
+000112f0: 7070 7269 6e74 2e70 666f 726d 6174 286e  pprint.pformat(n
+00011300: 6f64 655f 7374 6174 7573 5f64 6963 7429  ode_status_dict)
+00011310: 7d27 290a 2020 2020 2020 2020 2020 2020  }').            
+00011320: 6e6f 6465 5f73 7461 7475 7365 7320 3d20  node_statuses = 
+00011330: 6c69 7374 286e 6f64 655f 7374 6174 7573  list(node_status
+00011340: 5f64 6963 742e 7661 6c75 6573 2829 290a  _dict.values()).
+00011350: 2020 2020 2020 2020 6578 6365 7074 2045          except E
+00011360: 7863 6570 7469 6f6e 2061 7320 653a 2020  xception as e:  
+00011370: 2320 7079 6c69 6e74 3a20 6469 7361 626c  # pylint: disabl
+00011380: 653d 6272 6f61 642d 6578 6365 7074 0a20  e=broad-except. 
+00011390: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+000113a0: 7578 5f75 7469 6c73 2e70 7269 6e74 5f65  ux_utils.print_e
+000113b0: 7863 6570 7469 6f6e 5f6e 6f5f 7472 6163  xception_no_trac
+000113c0: 6562 6163 6b28 293a 0a20 2020 2020 2020  eback():.       
+000113d0: 2020 2020 2020 2020 2072 6169 7365 2065           raise e
+000113e0: 7863 6570 7469 6f6e 732e 436c 7573 7465  xceptions.Cluste
+000113f0: 7253 7461 7475 7346 6574 6368 696e 6745  rStatusFetchingE
+00011400: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+00011410: 2020 2020 2020 2020 2020 6627 4661 696c            f'Fail
+00011420: 6564 2074 6f20 7175 6572 7920 7b63 6c6f  ed to query {clo
+00011430: 7564 5f6e 616d 657d 2063 6c75 7374 6572  ud_name} cluster
+00011440: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
+00011450: 2020 2020 2020 2066 277b 636c 7573 7465         f'{cluste
+00011460: 725f 6e61 6d65 5f69 6e5f 6869 6e74 7d20  r_name_in_hint} 
+00011470: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+00011480: 2020 2020 2020 6627 7374 6174 7573 3a20        f'status: 
+00011490: 7b63 6f6d 6d6f 6e5f 7574 696c 732e 666f  {common_utils.fo
+000114a0: 726d 6174 5f65 7863 6570 7469 6f6e 2865  rmat_exception(e
+000114b0: 2c20 7573 655f 6272 6163 6b65 743d 5472  , use_bracket=Tr
+000114c0: 7565 297d 270a 2020 2020 2020 2020 2020  ue)}'.          
+000114d0: 2020 2020 2020 290a 2020 2020 656c 7365        ).    else
+000114e0: 3a0a 2020 2020 2020 2020 7265 6769 6f6e  :.        region
+000114f0: 203d 2070 726f 7669 6465 725f 636f 6e66   = provider_conf
+00011500: 6967 2e67 6574 2827 7265 6769 6f6e 2729  ig.get('region')
+00011510: 206f 7220 7072 6f76 6964 6572 5f63 6f6e   or provider_con
+00011520: 6669 672e 6765 7428 0a20 2020 2020 2020  fig.get(.       
+00011530: 2020 2020 2027 6c6f 6361 7469 6f6e 2729       'location')
+00011540: 0a20 2020 2020 2020 207a 6f6e 6520 3d20  .        zone = 
+00011550: 7261 795f 636f 6e66 6967 5b27 7072 6f76  ray_config['prov
+00011560: 6964 6572 275d 2e67 6574 2827 6176 6169  ider'].get('avai
+00011570: 6c61 6269 6c69 7479 5f7a 6f6e 6527 290a  lability_zone').
+00011580: 2020 2020 2020 2020 6e6f 6465 5f73 7461          node_sta
+00011590: 7475 7365 7320 3d20 636c 6f75 642e 7175  tuses = cloud.qu
+000115a0: 6572 795f 7374 6174 7573 280a 2020 2020  ery_status(.    
+000115b0: 2020 2020 2020 2020 636c 7573 7465 725f          cluster_
+000115c0: 6e61 6d65 5f6f 6e5f 636c 6f75 642c 0a20  name_on_cloud,. 
+000115d0: 2020 2020 2020 2020 2020 2074 6167 5f66             tag_f
+000115e0: 696c 7465 725f 666f 725f 636c 7573 7465  ilter_for_cluste
+000115f0: 7228 636c 7573 7465 725f 6e61 6d65 5f6f  r(cluster_name_o
+00011600: 6e5f 636c 6f75 6429 2c20 7265 6769 6f6e  n_cloud), region
+00011610: 2c20 7a6f 6e65 290a 2020 2020 7265 7475  , zone).    retu
+00011620: 726e 206e 6f64 655f 7374 6174 7573 6573  rn node_statuses
+00011630: 0a0a 0a64 6566 2063 6865 636b 5f63 616e  ...def check_can
+00011640: 5f63 6c6f 6e65 5f64 6973 6b5f 616e 645f  _clone_disk_and_
+00011650: 6f76 6572 7269 6465 5f74 6173 6b28 0a20  override_task(. 
+00011660: 2020 2063 6c75 7374 6572 5f6e 616d 653a     cluster_name:
+00011670: 2073 7472 2c20 7461 7267 6574 5f63 6c75   str, target_clu
+00011680: 7374 6572 5f6e 616d 653a 204f 7074 696f  ster_name: Optio
+00011690: 6e61 6c5b 7374 725d 2c20 7461 736b 3a20  nal[str], task: 
+000116a0: 2774 6173 6b5f 6c69 622e 5461 736b 270a  'task_lib.Task'.
+000116b0: 2920 2d3e 2054 7570 6c65 5b27 7461 736b  ) -> Tuple['task
+000116c0: 5f6c 6962 2e54 6173 6b27 2c20 2763 6c6f  _lib.Task', 'clo
+000116d0: 7564 5f76 6d5f 7261 795f 6261 636b 656e  ud_vm_ray_backen
+000116e0: 642e 436c 6f75 6456 6d52 6179 5265 736f  d.CloudVmRayReso
+000116f0: 7572 6365 4861 6e64 6c65 275d 3a0a 2020  urceHandle']:.  
+00011700: 2020 2222 2243 6865 636b 2069 6620 7468    """Check if th
+00011710: 6520 7461 736b 2069 7320 636f 6d70 6174  e task is compat
+00011720: 6962 6c65 2074 6f20 636c 6f6e 6520 6469  ible to clone di
+00011730: 736b 2066 726f 6d20 7468 6520 736f 7572  sk from the sour
+00011740: 6365 2063 6c75 7374 6572 2e0a 0a20 2020  ce cluster...   
+00011750: 2041 7267 733a 0a20 2020 2020 2020 2063   Args:.        c
+00011760: 6c75 7374 6572 5f6e 616d 653a 2054 6865  luster_name: The
+00011770: 206e 616d 6520 6f66 2074 6865 2063 6c75   name of the clu
+00011780: 7374 6572 2074 6f20 636c 6f6e 6520 6469  ster to clone di
+00011790: 736b 2066 726f 6d2e 0a20 2020 2020 2020  sk from..       
+000117a0: 2074 6172 6765 745f 636c 7573 7465 725f   target_cluster_
+000117b0: 6e61 6d65 3a20 5468 6520 6e61 6d65 206f  name: The name o
+000117c0: 6620 7468 6520 7461 7267 6574 2063 6c75  f the target clu
+000117d0: 7374 6572 2e0a 2020 2020 2020 2020 7461  ster..        ta
+000117e0: 736b 3a20 5468 6520 7461 736b 2074 6f20  sk: The task to 
+000117f0: 6368 6563 6b2e 0a0a 2020 2020 5265 7475  check...    Retu
+00011800: 726e 733a 0a20 2020 2020 2020 2054 6865  rns:.        The
+00011810: 2074 6173 6b20 746f 2075 7365 2061 6e64   task to use and
+00011820: 2074 6865 2072 6573 6f75 7263 6520 6861   the resource ha
+00011830: 6e64 6c65 206f 6620 7468 6520 736f 7572  ndle of the sour
+00011840: 6365 2063 6c75 7374 6572 2e0a 0a20 2020  ce cluster...   
+00011850: 2052 6169 7365 733a 0a20 2020 2020 2020   Raises:.       
+00011860: 2056 616c 7565 4572 726f 723a 2049 6620   ValueError: If 
+00011870: 7468 6520 736f 7572 6365 2063 6c75 7374  the source clust
+00011880: 6572 2064 6f65 7320 6e6f 7420 6578 6973  er does not exis
+00011890: 742e 0a20 2020 2020 2020 2065 7863 6570  t..        excep
+000118a0: 7469 6f6e 732e 4e6f 7453 7570 706f 7274  tions.NotSupport
+000118b0: 6564 4572 726f 723a 2049 6620 7468 6520  edError: If the 
+000118c0: 736f 7572 6365 2063 6c75 7374 6572 2069  source cluster i
+000118d0: 7320 6e6f 7420 7661 6c69 6420 6f72 2074  s not valid or t
+000118e0: 6865 0a20 2020 2020 2020 2020 2020 2074  he.            t
+000118f0: 6173 6b20 6973 206e 6f74 2063 6f6d 7061  ask is not compa
+00011900: 7469 626c 6520 746f 2063 6c6f 6e65 2064  tible to clone d
+00011910: 6973 6b20 6672 6f6d 2074 6865 2073 6f75  isk from the sou
+00011920: 7263 6520 636c 7573 7465 722e 0a20 2020  rce cluster..   
+00011930: 2022 2222 0a20 2020 2073 6f75 7263 655f   """.    source_
+00011940: 636c 7573 7465 725f 7374 6174 7573 2c20  cluster_status, 
+00011950: 6861 6e64 6c65 203d 2072 6566 7265 7368  handle = refresh
+00011960: 5f63 6c75 7374 6572 5f73 7461 7475 735f  _cluster_status_
+00011970: 6861 6e64 6c65 2863 6c75 7374 6572 5f6e  handle(cluster_n
+00011980: 616d 6529 0a20 2020 2069 6620 736f 7572  ame).    if sour
+00011990: 6365 5f63 6c75 7374 6572 5f73 7461 7475  ce_cluster_statu
+000119a0: 7320 6973 204e 6f6e 653a 0a20 2020 2020  s is None:.     
+000119b0: 2020 2077 6974 6820 7578 5f75 7469 6c73     with ux_utils
+000119c0: 2e70 7269 6e74 5f65 7863 6570 7469 6f6e  .print_exception
+000119d0: 5f6e 6f5f 7472 6163 6562 6163 6b28 293a  _no_traceback():
+000119e0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+000119f0: 7365 2056 616c 7565 4572 726f 7228 0a20  se ValueError(. 
+00011a00: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00011a10: 2743 616e 6e6f 7420 6669 6e64 2063 6c75  'Cannot find clu
+00011a20: 7374 6572 207b 636c 7573 7465 725f 6e61  ster {cluster_na
+00011a30: 6d65 2172 7d20 746f 2063 6c6f 6e65 2064  me!r} to clone d
+00011a40: 6973 6b20 6672 6f6d 2e27 290a 0a20 2020  isk from.')..   
+00011a50: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
+00011a60: 6365 2868 616e 646c 652c 2062 6163 6b65  ce(handle, backe
+00011a70: 6e64 732e 436c 6f75 6456 6d52 6179 5265  nds.CloudVmRayRe
+00011a80: 736f 7572 6365 4861 6e64 6c65 293a 0a20  sourceHandle):. 
+00011a90: 2020 2020 2020 2077 6974 6820 7578 5f75         with ux_u
+00011aa0: 7469 6c73 2e70 7269 6e74 5f65 7863 6570  tils.print_excep
+00011ab0: 7469 6f6e 5f6e 6f5f 7472 6163 6562 6163  tion_no_tracebac
+00011ac0: 6b28 293a 0a20 2020 2020 2020 2020 2020  k():.           
+00011ad0: 2072 6169 7365 2065 7863 6570 7469 6f6e   raise exception
+00011ae0: 732e 4e6f 7453 7570 706f 7274 6564 4572  s.NotSupportedEr
+00011af0: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
+00011b00: 2020 2020 2066 2743 616e 6e6f 7420 636c       f'Cannot cl
+00011b10: 6f6e 6520 6469 736b 2066 726f 6d20 6120  one disk from a 
+00011b20: 6e6f 6e2d 636c 6f75 6420 636c 7573 7465  non-cloud cluste
+00011b30: 7220 7b63 6c75 7374 6572 5f6e 616d 6521  r {cluster_name!
+00011b40: 727d 2e27 290a 0a20 2020 2069 6620 736f  r}.')..    if so
+00011b50: 7572 6365 5f63 6c75 7374 6572 5f73 7461  urce_cluster_sta
+00011b60: 7475 7320 213d 2073 7461 7475 735f 6c69  tus != status_li
+00011b70: 622e 436c 7573 7465 7253 7461 7475 732e  b.ClusterStatus.
+00011b80: 5354 4f50 5045 443a 0a20 2020 2020 2020  STOPPED:.       
+00011b90: 2077 6974 6820 7578 5f75 7469 6c73 2e70   with ux_utils.p
+00011ba0: 7269 6e74 5f65 7863 6570 7469 6f6e 5f6e  rint_exception_n
+00011bb0: 6f5f 7472 6163 6562 6163 6b28 293a 0a20  o_traceback():. 
+00011bc0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00011bd0: 2065 7863 6570 7469 6f6e 732e 4e6f 7453   exceptions.NotS
+00011be0: 7570 706f 7274 6564 4572 726f 7228 0a20  upportedError(. 
+00011bf0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00011c00: 2743 616e 6e6f 7420 636c 6f6e 6520 6469  'Cannot clone di
+00011c10: 736b 2066 726f 6d20 636c 7573 7465 7220  sk from cluster 
+00011c20: 7b63 6c75 7374 6572 5f6e 616d 6521 727d  {cluster_name!r}
+00011c30: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
+00011c40: 2020 2066 2728 7b73 6f75 7263 655f 636c     f'({source_cl
+00011c50: 7573 7465 725f 7374 6174 7573 2172 7d29  uster_status!r})
+00011c60: 2e20 506c 6561 7365 2073 746f 7020 7468  . Please stop th
+00011c70: 6520 270a 2020 2020 2020 2020 2020 2020  e '.            
+00011c80: 2020 2020 6627 636c 7573 7465 7220 6669      f'cluster fi
+00011c90: 7273 743a 2073 6b79 2073 746f 7020 7b63  rst: sky stop {c
+00011ca0: 6c75 7374 6572 5f6e 616d 657d 2729 0a0a  luster_name}')..
+00011cb0: 2020 2020 6966 2074 6172 6765 745f 636c      if target_cl
+00011cc0: 7573 7465 725f 6e61 6d65 2069 7320 6e6f  uster_name is no
+00011cd0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00011ce0: 7461 7267 6574 5f63 6c75 7374 6572 5f73  target_cluster_s
+00011cf0: 7461 7475 732c 205f 203d 2072 6566 7265  tatus, _ = refre
+00011d00: 7368 5f63 6c75 7374 6572 5f73 7461 7475  sh_cluster_statu
+00011d10: 735f 6861 6e64 6c65 280a 2020 2020 2020  s_handle(.      
+00011d20: 2020 2020 2020 7461 7267 6574 5f63 6c75        target_clu
+00011d30: 7374 6572 5f6e 616d 6529 0a20 2020 2020  ster_name).     
+00011d40: 2020 2069 6620 7461 7267 6574 5f63 6c75     if target_clu
+00011d50: 7374 6572 5f73 7461 7475 7320 6973 206e  ster_status is n
+00011d60: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00011d70: 2020 2020 2077 6974 6820 7578 5f75 7469       with ux_uti
+00011d80: 6c73 2e70 7269 6e74 5f65 7863 6570 7469  ls.print_excepti
+00011d90: 6f6e 5f6e 6f5f 7472 6163 6562 6163 6b28  on_no_traceback(
+00011da0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00011db0: 2020 2072 6169 7365 2065 7863 6570 7469     raise excepti
+00011dc0: 6f6e 732e 4e6f 7453 7570 706f 7274 6564  ons.NotSupported
+00011dd0: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
+00011de0: 2020 2020 2020 2020 2020 2066 2754 6865             f'The
+00011df0: 2074 6172 6765 7420 636c 7573 7465 7220   target cluster 
+00011e00: 7b74 6172 6765 745f 636c 7573 7465 725f  {target_cluster_
+00011e10: 6e61 6d65 2172 7d20 616c 7265 6164 7920  name!r} already 
+00011e20: 6578 6973 7473 2e20 436c 6f6e 696e 6720  exists. Cloning 
+00011e30: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+00011e40: 2020 2020 2020 2764 6973 6b20 6973 206f        'disk is o
+00011e50: 6e6c 7920 7375 7070 6f72 7465 6420 7768  nly supported wh
+00011e60: 656e 2063 7265 6174 696e 6720 6120 6e65  en creating a ne
+00011e70: 7720 636c 7573 7465 722e 2054 6f20 6669  w cluster. To fi
+00011e80: 783a 2073 7065 6369 6679 2027 0a20 2020  x: specify '.   
+00011e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ea0: 2027 6120 6e65 7720 7461 7267 6574 2063   'a new target c
+00011eb0: 6c75 7374 6572 206e 616d 652e 2729 0a0a  luster name.')..
+00011ec0: 2020 2020 6e65 775f 7461 736b 5f72 6573      new_task_res
+00011ed0: 6f75 7263 6573 203d 205b 5d0a 2020 2020  ources = [].    
+00011ee0: 6f72 6967 696e 616c 5f63 6c6f 7564 203d  original_cloud =
+00011ef0: 2068 616e 646c 652e 6c61 756e 6368 6564   handle.launched
+00011f00: 5f72 6573 6f75 7263 6573 2e63 6c6f 7564  _resources.cloud
+00011f10: 0a20 2020 206f 7269 6769 6e61 6c5f 636c  .    original_cl
+00011f20: 6f75 642e 6368 6563 6b5f 6665 6174 7572  oud.check_featur
+00011f30: 6573 5f61 7265 5f73 7570 706f 7274 6564  es_are_supported
+00011f40: 280a 2020 2020 2020 2020 6861 6e64 6c65  (.        handle
+00011f50: 2e6c 6175 6e63 6865 645f 7265 736f 7572  .launched_resour
+00011f60: 6365 732c 0a20 2020 2020 2020 207b 636c  ces,.        {cl
+00011f70: 6f75 6473 2e43 6c6f 7564 496d 706c 656d  ouds.CloudImplem
+00011f80: 656e 7461 7469 6f6e 4665 6174 7572 6573  entationFeatures
+00011f90: 2e43 4c4f 4e45 5f44 4953 4b5f 4652 4f4d  .CLONE_DISK_FROM
+00011fa0: 5f43 4c55 5354 4552 7d29 0a0a 2020 2020  _CLUSTER})..    
+00011fb0: 6173 7365 7274 206f 7269 6769 6e61 6c5f  assert original_
+00011fc0: 636c 6f75 6420 6973 206e 6f74 204e 6f6e  cloud is not Non
+00011fd0: 652c 2068 616e 646c 652e 6c61 756e 6368  e, handle.launch
+00011fe0: 6564 5f72 6573 6f75 7263 6573 0a20 2020  ed_resources.   
+00011ff0: 2068 6173 5f6f 7665 7272 6964 6520 3d20   has_override = 
+00012000: 4661 6c73 650a 2020 2020 6861 735f 6469  False.    has_di
+00012010: 736b 5f73 697a 655f 6d65 7420 3d20 4661  sk_size_met = Fa
+00012020: 6c73 650a 2020 2020 6861 735f 636c 6f75  lse.    has_clou
+00012030: 645f 6d65 7420 3d20 4661 6c73 650a 2020  d_met = False.  
+00012040: 2020 666f 7220 7461 736b 5f72 6573 6f75    for task_resou
+00012050: 7263 6573 2069 6e20 7461 736b 2e72 6573  rces in task.res
+00012060: 6f75 7263 6573 3a0a 2020 2020 2020 2020  ources:.        
+00012070: 6966 2068 616e 646c 652e 6c61 756e 6368  if handle.launch
+00012080: 6564 5f72 6573 6f75 7263 6573 2e64 6973  ed_resources.dis
+00012090: 6b5f 7369 7a65 203e 2074 6173 6b5f 7265  k_size > task_re
+000120a0: 736f 7572 6365 732e 6469 736b 5f73 697a  sources.disk_siz
+000120b0: 653a 0a20 2020 2020 2020 2020 2020 2023  e:.            #
+000120c0: 2054 6865 2074 6172 6765 7420 636c 7573   The target clus
+000120d0: 7465 7227 7320 6469 736b 2073 686f 756c  ter's disk shoul
+000120e0: 6420 6265 2061 7420 6c65 6173 7420 6173  d be at least as
+000120f0: 206c 6172 6765 2061 7320 7468 6520 736f   large as the so
+00012100: 7572 6365 2e0a 2020 2020 2020 2020 2020  urce..          
+00012110: 2020 636f 6e74 696e 7565 0a20 2020 2020    continue.     
+00012120: 2020 2068 6173 5f64 6973 6b5f 7369 7a65     has_disk_size
+00012130: 5f6d 6574 203d 2054 7275 650a 2020 2020  _met = True.    
+00012140: 2020 2020 6966 2074 6173 6b5f 7265 736f      if task_reso
+00012150: 7572 6365 732e 636c 6f75 6420 6973 206e  urces.cloud is n
+00012160: 6f74 204e 6f6e 6520 616e 6420 6e6f 7420  ot None and not 
+00012170: 6f72 6967 696e 616c 5f63 6c6f 7564 2e69  original_cloud.i
+00012180: 735f 7361 6d65 5f63 6c6f 7564 280a 2020  s_same_cloud(.  
+00012190: 2020 2020 2020 2020 2020 2020 2020 7461                ta
+000121a0: 736b 5f72 6573 6f75 7263 6573 2e63 6c6f  sk_resources.clo
+000121b0: 7564 293a 0a20 2020 2020 2020 2020 2020  ud):.           
+000121c0: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
+000121d0: 2020 6861 735f 636c 6f75 645f 6d65 7420    has_cloud_met 
+000121e0: 3d20 5472 7565 0a0a 2020 2020 2020 2020  = True..        
+000121f0: 6f76 6572 7269 6465 5f70 6172 616d 203d  override_param =
+00012200: 207b 7d0a 2020 2020 2020 2020 6966 2074   {}.        if t
+00012210: 6173 6b5f 7265 736f 7572 6365 732e 636c  ask_resources.cl
+00012220: 6f75 6420 6973 204e 6f6e 653a 0a20 2020  oud is None:.   
+00012230: 2020 2020 2020 2020 206f 7665 7272 6964           overrid
+00012240: 655f 7061 7261 6d5b 2763 6c6f 7564 275d  e_param['cloud']
+00012250: 203d 206f 7269 6769 6e61 6c5f 636c 6f75   = original_clou
+00012260: 640a 2020 2020 2020 2020 6966 2074 6173  d.        if tas
+00012270: 6b5f 7265 736f 7572 6365 732e 7265 6769  k_resources.regi
+00012280: 6f6e 2069 7320 4e6f 6e65 3a0a 2020 2020  on is None:.    
+00012290: 2020 2020 2020 2020 6f76 6572 7269 6465          override
+000122a0: 5f70 6172 616d 5b27 7265 6769 6f6e 275d  _param['region']
+000122b0: 203d 2068 616e 646c 652e 6c61 756e 6368   = handle.launch
+000122c0: 6564 5f72 6573 6f75 7263 6573 2e72 6567  ed_resources.reg
+000122d0: 696f 6e0a 0a20 2020 2020 2020 2069 6620  ion..        if 
+000122e0: 6f76 6572 7269 6465 5f70 6172 616d 3a0a  override_param:.
+000122f0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+00012300: 6572 2e69 6e66 6f28 0a20 2020 2020 2020  er.info(.       
+00012310: 2020 2020 2020 2020 2066 274e 6f20 636c           f'No cl
+00012320: 6f75 642f 7265 6769 6f6e 2073 7065 6369  oud/region speci
+00012330: 6669 6564 2066 6f72 2074 6865 2074 6173  fied for the tas
+00012340: 6b20 7b74 6173 6b5f 7265 736f 7572 6365  k {task_resource
+00012350: 737d 2e20 5573 696e 6720 7468 6520 7361  s}. Using the sa
+00012360: 6d65 2072 6567 696f 6e20 270a 2020 2020  me region '.    
+00012370: 2020 2020 2020 2020 2020 2020 6627 6173              f'as
+00012380: 2073 6f75 7263 6520 636c 7573 7465 7220   source cluster 
+00012390: 7b63 6c75 7374 6572 5f6e 616d 6521 727d  {cluster_name!r}
+000123a0: 3a20 270a 2020 2020 2020 2020 2020 2020  : '.            
+000123b0: 2020 2020 6627 7b68 616e 646c 652e 6c61      f'{handle.la
+000123c0: 756e 6368 6564 5f72 6573 6f75 7263 6573  unched_resources
+000123d0: 2e63 6c6f 7564 7d27 0a20 2020 2020 2020  .cloud}'.       
+000123e0: 2020 2020 2020 2020 2066 2728 7b68 616e           f'({han
+000123f0: 646c 652e 6c61 756e 6368 6564 5f72 6573  dle.launched_res
+00012400: 6f75 7263 6573 2e72 6567 696f 6e7d 292e  ources.region}).
+00012410: 2729 0a20 2020 2020 2020 2020 2020 2068  ').            h
+00012420: 6173 5f6f 7665 7272 6964 6520 3d20 5472  as_override = Tr
+00012430: 7565 0a20 2020 2020 2020 2074 6173 6b5f  ue.        task_
+00012440: 7265 736f 7572 6365 7320 3d20 7461 736b  resources = task
+00012450: 5f72 6573 6f75 7263 6573 2e63 6f70 7928  _resources.copy(
+00012460: 2a2a 6f76 6572 7269 6465 5f70 6172 616d  **override_param
+00012470: 290a 2020 2020 2020 2020 6e65 775f 7461  ).        new_ta
+00012480: 736b 5f72 6573 6f75 7263 6573 2e61 7070  sk_resources.app
+00012490: 656e 6428 7461 736b 5f72 6573 6f75 7263  end(task_resourc
+000124a0: 6573 290a 0a20 2020 2069 6620 6e6f 7420  es)..    if not 
+000124b0: 6e65 775f 7461 736b 5f72 6573 6f75 7263  new_task_resourc
+000124c0: 6573 3a0a 2020 2020 2020 2020 6966 206e  es:.        if n
+000124d0: 6f74 2068 6173 5f64 6973 6b5f 7369 7a65  ot has_disk_size
+000124e0: 5f6d 6574 3a0a 2020 2020 2020 2020 2020  _met:.          
+000124f0: 2020 7769 7468 2075 785f 7574 696c 732e    with ux_utils.
+00012500: 7072 696e 745f 6578 6365 7074 696f 6e5f  print_exception_
+00012510: 6e6f 5f74 7261 6365 6261 636b 2829 3a0a  no_traceback():.
+00012520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012530: 7461 7267 6574 5f63 6c75 7374 6572 5f6e  target_cluster_n
+00012540: 616d 655f 7374 7220 3d20 6627 207b 7461  ame_str = f' {ta
+00012550: 7267 6574 5f63 6c75 7374 6572 5f6e 616d  rget_cluster_nam
+00012560: 6521 727d 270a 2020 2020 2020 2020 2020  e!r}'.          
+00012570: 2020 2020 2020 6966 2074 6172 6765 745f        if target_
+00012580: 636c 7573 7465 725f 6e61 6d65 2069 7320  cluster_name is 
+00012590: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000125a0: 2020 2020 2020 2020 2020 7461 7267 6574            target
+000125b0: 5f63 6c75 7374 6572 5f6e 616d 655f 7374  _cluster_name_st
+000125c0: 7220 3d20 2727 0a20 2020 2020 2020 2020  r = ''.         
+000125d0: 2020 2020 2020 2072 6169 7365 2065 7863         raise exc
+000125e0: 6570 7469 6f6e 732e 4e6f 7453 7570 706f  eptions.NotSuppo
+000125f0: 7274 6564 4572 726f 7228 0a20 2020 2020  rtedError(.     
+00012600: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00012610: 2754 6865 2074 6172 6765 7420 636c 7573  'The target clus
+00012620: 7465 727b 7461 7267 6574 5f63 6c75 7374  ter{target_clust
+00012630: 6572 5f6e 616d 655f 7374 727d 2073 686f  er_name_str} sho
+00012640: 756c 6420 6861 7665 2061 2064 6973 6b20  uld have a disk 
+00012650: 7369 7a65 2027 0a20 2020 2020 2020 2020  size '.         
+00012660: 2020 2020 2020 2020 2020 2066 276f 6620             f'of 
+00012670: 6174 206c 6561 7374 207b 6861 6e64 6c65  at least {handle
+00012680: 2e6c 6175 6e63 6865 645f 7265 736f 7572  .launched_resour
+00012690: 6365 732e 6469 736b 5f73 697a 657d 2047  ces.disk_size} G
+000126a0: 4220 746f 2063 6c6f 6e65 2074 6865 2027  B to clone the '
+000126b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000126c0: 2020 2020 2066 2764 6973 6b20 6672 6f6d       f'disk from
+000126d0: 207b 636c 7573 7465 725f 6e61 6d65 2172   {cluster_name!r
+000126e0: 7d2e 2729 0a20 2020 2020 2020 2069 6620  }.').        if 
+000126f0: 6e6f 7420 6861 735f 636c 6f75 645f 6d65  not has_cloud_me
+00012700: 743a 0a20 2020 2020 2020 2020 2020 2074  t:.            t
+00012710: 6173 6b5f 7265 736f 7572 6365 735f 636c  ask_resources_cl
+00012720: 6f75 645f 7374 7220 3d20 275b 2720 2b20  oud_str = '[' + 
+00012730: 272c 272e 6a6f 696e 280a 2020 2020 2020  ','.join(.      
+00012740: 2020 2020 2020 2020 2020 5b66 277b 7265            [f'{re
+00012750: 732e 636c 6f75 647d 2720 666f 7220 7265  s.cloud}' for re
+00012760: 7320 696e 2074 6173 6b2e 7265 736f 7572  s in task.resour
+00012770: 6365 735d 2920 2b20 275d 270a 2020 2020  ces]) + ']'.    
+00012780: 2020 2020 2020 2020 7461 736b 5f72 6573          task_res
+00012790: 6f75 7263 6573 5f73 7472 203d 2027 5b27  ources_str = '['
+000127a0: 202b 2027 2c27 2e6a 6f69 6e28 0a20 2020   + ','.join(.   
+000127b0: 2020 2020 2020 2020 2020 2020 205b 6627               [f'
+000127c0: 7b72 6573 7d27 2066 6f72 2072 6573 2069  {res}' for res i
+000127d0: 6e20 7461 736b 2e72 6573 6f75 7263 6573  n task.resources
+000127e0: 5d29 202b 2027 5d27 0a20 2020 2020 2020  ]) + ']'.       
+000127f0: 2020 2020 2077 6974 6820 7578 5f75 7469       with ux_uti
+00012800: 6c73 2e70 7269 6e74 5f65 7863 6570 7469  ls.print_excepti
+00012810: 6f6e 5f6e 6f5f 7472 6163 6562 6163 6b28  on_no_traceback(
+00012820: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00012830: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00012840: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
+00012850: 2020 2020 2020 2020 2066 2743 616e 6e6f           f'Canno
+00012860: 7420 636c 6f6e 6520 6469 736b 2061 6372  t clone disk acr
+00012870: 6f73 7320 636c 6f75 6420 6672 6f6d 207b  oss cloud from {
+00012880: 6f72 6967 696e 616c 5f63 6c6f 7564 7d20  original_cloud} 
+00012890: 746f 2027 0a20 2020 2020 2020 2020 2020  to '.           
+000128a0: 2020 2020 2020 2020 2066 277b 7461 736b           f'{task
+000128b0: 5f72 6573 6f75 7263 6573 5f63 6c6f 7564  _resources_cloud
+000128c0: 5f73 7472 7d20 666f 7220 7265 736f 7572  _str} for resour
+000128d0: 6365 7320 7b74 6173 6b5f 7265 736f 7572  ces {task_resour
+000128e0: 6365 735f 7374 727d 2e27 0a20 2020 2020  ces_str}.'.     
+000128f0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00012900: 2020 2020 2061 7373 6572 7420 4661 6c73       assert Fals
+00012910: 652c 2027 5368 6f75 6c64 206e 6f74 2072  e, 'Should not r
+00012920: 6561 6368 2068 6572 652e 270a 2020 2020  each here.'.    
+00012930: 2320 7365 7420 7468 6520 6e65 775f 7461  # set the new_ta
+00012940: 736b 5f72 6573 6f75 7263 6573 2074 6f20  sk_resources to 
+00012950: 6265 2074 6865 2073 616d 6520 7479 7065  be the same type
+00012960: 2028 6c69 7374 206f 7220 7365 7429 2061   (list or set) a
+00012970: 7320 7468 650a 2020 2020 2320 6f72 6967  s the.    # orig
+00012980: 696e 616c 2074 6173 6b2e 7265 736f 7572  inal task.resour
+00012990: 6365 730a 2020 2020 6966 2068 6173 5f6f  ces.    if has_o
+000129a0: 7665 7272 6964 653a 0a20 2020 2020 2020  verride:.       
+000129b0: 2074 6173 6b2e 7365 745f 7265 736f 7572   task.set_resour
+000129c0: 6365 7328 7479 7065 2874 6173 6b2e 7265  ces(type(task.re
+000129d0: 736f 7572 6365 7329 286e 6577 5f74 6173  sources)(new_tas
+000129e0: 6b5f 7265 736f 7572 6365 7329 290a 2020  k_resources)).  
+000129f0: 2020 2020 2020 2320 5265 7365 7420 7468        # Reset th
+00012a00: 6520 6265 7374 5f72 6573 6f75 7263 6573  e best_resources
+00012a10: 2074 6f20 7472 6967 6572 2072 652d 6f70   to triger re-op
+00012a20: 7469 6d69 7a61 7469 6f6e 0a20 2020 2020  timization.     
+00012a30: 2020 2023 206c 6174 6572 2c20 736f 2074     # later, so t
+00012a40: 6861 7420 7468 6520 6e65 7720 7461 736b  hat the new task
+00012a50: 5f72 6573 6f75 7263 6573 2077 696c 6c20  _resources will 
+00012a60: 6265 2075 7365 642e 0a20 2020 2020 2020  be used..       
+00012a70: 2074 6173 6b2e 6265 7374 5f72 6573 6f75   task.best_resou
+00012a80: 7263 6573 203d 204e 6f6e 650a 2020 2020  rces = None.    
+00012a90: 7265 7475 726e 2074 6173 6b2c 2068 616e  return task, han
+00012aa0: 646c 650a 0a0a 6465 6620 5f75 7064 6174  dle...def _updat
+00012ab0: 655f 636c 7573 7465 725f 7374 6174 7573  e_cluster_status
+00012ac0: 5f6e 6f5f 6c6f 636b 280a 2020 2020 2020  _no_lock(.      
+00012ad0: 2020 636c 7573 7465 725f 6e61 6d65 3a20    cluster_name: 
+00012ae0: 7374 7229 202d 3e20 4f70 7469 6f6e 616c  str) -> Optional
+00012af0: 5b44 6963 745b 7374 722c 2041 6e79 5d5d  [Dict[str, Any]]
+00012b00: 3a0a 2020 2020 2222 2255 7064 6174 6573  :.    """Updates
+00012b10: 2074 6865 2073 7461 7475 7320 6f66 2074   the status of t
+00012b20: 6865 2063 6c75 7374 6572 2e0a 0a20 2020  he cluster...   
+00012b30: 2052 6169 7365 733a 0a20 2020 2020 2020   Raises:.       
+00012b40: 2065 7863 6570 7469 6f6e 732e 436c 7573   exceptions.Clus
+00012b50: 7465 7253 7461 7475 7346 6574 6368 696e  terStatusFetchin
+00012b60: 6745 7272 6f72 3a20 7468 6520 636c 7573  gError: the clus
+00012b70: 7465 7220 7374 6174 7573 2063 616e 6e6f  ter status canno
+00012b80: 7420 6265 0a20 2020 2020 2020 2020 2066  t be.          f
+00012b90: 6574 6368 6564 2066 726f 6d20 7468 6520  etched from the 
+00012ba0: 636c 6f75 6420 7072 6f76 6964 6572 2e0a  cloud provider..
+00012bb0: 2020 2020 2222 220a 2020 2020 7265 636f      """.    reco
+00012bc0: 7264 203d 2067 6c6f 6261 6c5f 7573 6572  rd = global_user
+00012bd0: 5f73 7461 7465 2e67 6574 5f63 6c75 7374  _state.get_clust
+00012be0: 6572 5f66 726f 6d5f 6e61 6d65 2863 6c75  er_from_name(clu
+00012bf0: 7374 6572 5f6e 616d 6529 0a20 2020 2069  ster_name).    i
+00012c00: 6620 7265 636f 7264 2069 7320 4e6f 6e65  f record is None
+00012c10: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00012c20: 204e 6f6e 650a 2020 2020 6861 6e64 6c65   None.    handle
+00012c30: 203d 2072 6563 6f72 645b 2768 616e 646c   = record['handl
+00012c40: 6527 5d0a 2020 2020 6966 206e 6f74 2069  e'].    if not i
+00012c50: 7369 6e73 7461 6e63 6528 6861 6e64 6c65  sinstance(handle
+00012c60: 2c20 6261 636b 656e 6473 2e43 6c6f 7564  , backends.Cloud
+00012c70: 566d 5261 7952 6573 6f75 7263 6548 616e  VmRayResourceHan
+00012c80: 646c 6529 3a0a 2020 2020 2020 2020 7265  dle):.        re
+00012c90: 7475 726e 2072 6563 6f72 640a 2020 2020  turn record.    
+00012ca0: 636c 7573 7465 725f 6e61 6d65 203d 2068  cluster_name = h
+00012cb0: 616e 646c 652e 636c 7573 7465 725f 6e61  andle.cluster_na
+00012cc0: 6d65 0a0a 2020 2020 6e6f 6465 5f73 7461  me..    node_sta
+00012cd0: 7475 7365 7320 3d20 5f71 7565 7279 5f63  tuses = _query_c
+00012ce0: 6c75 7374 6572 5f73 7461 7475 735f 7669  luster_status_vi
+00012cf0: 615f 636c 6f75 645f 6170 6928 6861 6e64  a_cloud_api(hand
+00012d00: 6c65 290a 0a20 2020 2061 6c6c 5f6e 6f64  le)..    all_nod
+00012d10: 6573 5f75 7020 3d20 2861 6c6c 280a 2020  es_up = (all(.  
+00012d20: 2020 2020 2020 7374 6174 7573 203d 3d20        status == 
+00012d30: 7374 6174 7573 5f6c 6962 2e43 6c75 7374  status_lib.Clust
+00012d40: 6572 5374 6174 7573 2e55 5020 666f 7220  erStatus.UP for 
+00012d50: 7374 6174 7573 2069 6e20 6e6f 6465 5f73  status in node_s
+00012d60: 7461 7475 7365 7329 2061 6e64 0a20 2020  tatuses) and.   
+00012d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d80: 206c 656e 286e 6f64 655f 7374 6174 7573   len(node_status
+00012d90: 6573 2920 3d3d 2068 616e 646c 652e 6c61  es) == handle.la
+00012da0: 756e 6368 6564 5f6e 6f64 6573 290a 0a20  unched_nodes).. 
+00012db0: 2020 2064 6566 2072 756e 5f72 6179 5f73     def run_ray_s
+00012dc0: 7461 7475 735f 746f 5f63 6865 636b 5f72  tatus_to_check_r
+00012dd0: 6179 5f63 6c75 7374 6572 5f68 6561 6c74  ay_cluster_healt
+00012de0: 6879 2829 202d 3e20 626f 6f6c 3a0a 2020  hy() -> bool:.  
+00012df0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+00012e00: 2020 2020 2020 2023 204e 4f54 453a 2066         # NOTE: f
+00012e10: 6574 6368 696e 6720 7468 6520 4950 7320  etching the IPs 
+00012e20: 6973 2076 6572 7920 736c 6f77 2061 7320  is very slow as 
+00012e30: 6974 2063 616c 6c73 2069 6e74 6f0a 2020  it calls into.  
+00012e40: 2020 2020 2020 2020 2020 2320 6072 6179            # `ray
+00012e50: 2067 6574 2068 6561 642d 6970 2f77 6f72   get head-ip/wor
+00012e60: 6b65 722d 6970 7360 2e20 5573 696e 6720  ker-ips`. Using 
+00012e70: 6361 6368 6564 2049 5073 2069 7320 7361  cached IPs is sa
+00012e80: 6665 2062 6563 6175 7365 0a20 2020 2020  fe because.     
+00012e90: 2020 2020 2020 2023 2069 6e20 7468 6520         # in the 
+00012ea0: 776f 7273 7420 6361 7365 2077 6520 7469  worst case we ti
+00012eb0: 6d65 206f 7574 2069 6e20 7468 6520 6072  me out in the `r
+00012ec0: 6179 2073 7461 7475 7360 2053 5348 2063  ay status` SSH c
+00012ed0: 6f6d 6d61 6e64 0a20 2020 2020 2020 2020  ommand.         
+00012ee0: 2020 2023 2062 656c 6f77 2e0a 2020 2020     # below..    
+00012ef0: 2020 2020 2020 2020 7275 6e6e 6572 7320          runners 
+00012f00: 3d20 6861 6e64 6c65 2e67 6574 5f63 6f6d  = handle.get_com
+00012f10: 6d61 6e64 5f72 756e 6e65 7273 2866 6f72  mand_runners(for
+00012f20: 6365 5f63 6163 6865 643d 5472 7565 290a  ce_cached=True).
+00012f30: 2020 2020 2020 2020 2020 2020 2320 5468              # Th
+00012f40: 6973 2068 6170 7065 6e73 2077 6865 6e20  is happens when 
+00012f50: 7573 6572 2069 6e74 6572 7275 7074 2074  user interrupt t
+00012f60: 6865 2060 736b 7920 6c61 756e 6368 6020  he `sky launch` 
+00012f70: 7072 6f63 6573 7320 6265 666f 7265 0a20  process before. 
+00012f80: 2020 2020 2020 2020 2020 2023 2074 6865             # the
+00012f90: 2066 6972 7374 2074 696d 6520 7265 736f   first time reso
+00012fa0: 7572 6365 7320 6861 6e64 6c65 2069 7320  urces handle is 
+00012fb0: 7772 6974 7465 6e20 6261 636b 2074 6f20  written back to 
+00012fc0: 6c6f 6361 6c20 6461 7461 6261 7365 2e0a  local database..
+00012fd0: 2020 2020 2020 2020 2020 2020 2320 5468              # Th
+00012fe0: 6973 2069 7320 6865 6c70 6675 6c20 7768  is is helpful wh
+00012ff0: 656e 2075 7365 7220 696e 7465 7272 7570  en user interrup
+00013000: 7420 6166 7465 7220 7468 6520 7072 6f76  t after the prov
+00013010: 6973 696f 6e20 6973 2064 6f6e 650a 2020  ision is done.  
+00013020: 2020 2020 2020 2020 2020 2320 616e 6420            # and 
+00013030: 6265 666f 7265 2074 6865 2073 6b79 6c65  before the skyle
+00013040: 7420 6973 2072 6573 7461 7274 6564 2e20  t is restarted. 
+00013050: 4166 7465 7220 2332 3330 3420 6973 206d  After #2304 is m
+00013060: 6572 6765 642c 2074 6869 730a 2020 2020  erged, this.    
+00013070: 2020 2020 2020 2020 2320 6865 6c70 7320          # helps 
+00013080: 6b65 6570 2074 6865 2063 6c75 7374 6572  keep the cluster
+00013090: 2073 7461 7475 7320 746f 2049 4e49 5420   status to INIT 
+000130a0: 6166 7465 7220 6073 6b79 2073 7461 7475  after `sky statu
+000130b0: 7320 2d72 602c 2073 6f0a 2020 2020 2020  s -r`, so.      
+000130c0: 2020 2020 2020 2320 7573 6572 2077 696c        # user wil
+000130d0: 6c20 6265 206e 6f74 6966 6965 6420 7468  l be notified th
+000130e0: 6174 2061 6e79 2061 7574 6f20 7374 6f70  at any auto stop
+000130f0: 2f64 6f77 6e20 6d69 6768 7420 6e6f 7420  /down might not 
+00013100: 6265 0a20 2020 2020 2020 2020 2020 2023  be.            #
+00013110: 2074 7269 6767 6572 6564 2e0a 2020 2020   triggered..    
+00013120: 2020 2020 2020 2020 6966 206e 6f74 2072          if not r
+00013130: 756e 6e65 7273 3a0a 2020 2020 2020 2020  unners:.        
+00013140: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+00013150: 6562 7567 2866 2752 6566 7265 7368 696e  ebug(f'Refreshin
+00013160: 6720 7374 6174 7573 2028 7b63 6c75 7374  g status ({clust
+00013170: 6572 5f6e 616d 6521 727d 293a 204e 6f20  er_name!r}): No 
+00013180: 6361 6368 6564 2027 0a20 2020 2020 2020  cached '.       
+00013190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000131a0: 2020 2020 2020 6627 4950 7320 666f 756e        f'IPs foun
+000131b0: 642e 2048 616e 646c 653a 207b 6861 6e64  d. Handle: {hand
+000131c0: 6c65 7d27 290a 2020 2020 2020 2020 2020  le}').          
+000131d0: 2020 2020 2020 7261 6973 6520 6578 6365        raise exce
+000131e0: 7074 696f 6e73 2e46 6574 6368 436c 7573  ptions.FetchClus
+000131f0: 7465 7249 6e66 6f45 7272 6f72 280a 2020  terInfoError(.  
+00013200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013210: 2020 7265 6173 6f6e 3d65 7863 6570 7469    reason=excepti
+00013220: 6f6e 732e 4665 7463 6843 6c75 7374 6572  ons.FetchCluster
+00013230: 496e 666f 4572 726f 722e 5265 6173 6f6e  InfoError.Reason
+00013240: 2e48 4541 4429 0a20 2020 2020 2020 2020  .HEAD).         
+00013250: 2020 2068 6561 645f 7275 6e6e 6572 203d     head_runner =
+00013260: 2072 756e 6e65 7273 5b30 5d0a 2020 2020   runners[0].    
+00013270: 2020 2020 2020 2020 7263 2c20 6f75 7470          rc, outp
+00013280: 7574 2c20 7374 6465 7272 203d 2068 6561  ut, stderr = hea
+00013290: 645f 7275 6e6e 6572 2e72 756e 280a 2020  d_runner.run(.  
+000132a0: 2020 2020 2020 2020 2020 2020 2020 696e                in
+000132b0: 7374 616e 6365 5f73 6574 7570 2e52 4159  stance_setup.RAY
+000132c0: 5f53 5441 5455 535f 5749 5448 5f53 4b59  _STATUS_WITH_SKY
+000132d0: 5f52 4159 5f50 4f52 545f 434f 4d4d 414e  _RAY_PORT_COMMAN
+000132e0: 442c 0a20 2020 2020 2020 2020 2020 2020  D,.             
+000132f0: 2020 2073 7472 6561 6d5f 6c6f 6773 3d46     stream_logs=F
+00013300: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
+00013310: 2020 2020 2020 7265 7175 6972 655f 6f75        require_ou
+00013320: 7470 7574 733d 5472 7565 2c0a 2020 2020  tputs=True,.    
+00013330: 2020 2020 2020 2020 2020 2020 7365 7061              sepa
+00013340: 7261 7465 5f73 7464 6572 723d 5472 7565  rate_stderr=True
+00013350: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00013360: 2072 633a 0a20 2020 2020 2020 2020 2020   rc:.           
+00013370: 2020 2020 2072 6169 7365 2052 756e 7469       raise Runti
+00013380: 6d65 4572 726f 7228 0a20 2020 2020 2020  meError(.       
+00013390: 2020 2020 2020 2020 2020 2020 2066 2752               f'R
+000133a0: 6566 7265 7368 696e 6720 7374 6174 7573  efreshing status
+000133b0: 2028 7b63 6c75 7374 6572 5f6e 616d 6521   ({cluster_name!
+000133c0: 727d 293a 2046 6169 6c65 6420 746f 2063  r}): Failed to c
+000133d0: 6865 636b 2027 0a20 2020 2020 2020 2020  heck '.         
+000133e0: 2020 2020 2020 2020 2020 2066 2772 6179             f'ray
+000133f0: 2063 6c75 7374 6572 5c27 7320 6865 616c   cluster\'s heal
+00013400: 7468 696e 6573 7320 7769 7468 2027 0a20  thiness with '. 
+00013410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013420: 2020 2066 277b 696e 7374 616e 6365 5f73     f'{instance_s
+00013430: 6574 7570 2e52 4159 5f53 5441 5455 535f  etup.RAY_STATUS_
+00013440: 5749 5448 5f53 4b59 5f52 4159 5f50 4f52  WITH_SKY_RAY_POR
+00013450: 545f 434f 4d4d 414e 447d 2e5c 6e27 0a20  T_COMMAND}.\n'. 
+00013460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013470: 2020 2066 272d 2d20 7374 646f 7574 202d     f'-- stdout -
+00013480: 2d5c 6e7b 6f75 7470 7574 7d5c 6e2d 2d20  -\n{output}\n-- 
+00013490: 7374 6465 7272 202d 2d5c 6e7b 7374 6465  stderr --\n{stde
+000134a0: 7272 7d27 290a 0a20 2020 2020 2020 2020  rr}')..         
+000134b0: 2020 2072 6561 6479 5f68 6561 642c 2072     ready_head, r
+000134c0: 6561 6479 5f77 6f72 6b65 7273 203d 205f  eady_workers = _
+000134d0: 636f 756e 745f 6865 616c 7468 795f 6e6f  count_healthy_no
+000134e0: 6465 735f 6672 6f6d 5f72 6179 286f 7574  des_from_ray(out
+000134f0: 7075 7429 0a20 2020 2020 2020 2020 2020  put).           
+00013500: 2074 6f74 616c 5f6e 6f64 6573 203d 2068   total_nodes = h
+00013510: 616e 646c 652e 6c61 756e 6368 6564 5f6e  andle.launched_n
+00013520: 6f64 6573 202a 2068 616e 646c 652e 6e75  odes * handle.nu
+00013530: 6d5f 6970 735f 7065 725f 6e6f 6465 0a20  m_ips_per_node. 
+00013540: 2020 2020 2020 2020 2020 2069 6620 7265             if re
+00013550: 6164 795f 6865 6164 202b 2072 6561 6479  ady_head + ready
+00013560: 5f77 6f72 6b65 7273 203d 3d20 746f 7461  _workers == tota
+00013570: 6c5f 6e6f 6465 733a 0a20 2020 2020 2020  l_nodes:.       
+00013580: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00013590: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
+000135a0: 2072 6169 7365 2052 756e 7469 6d65 4572   raise RuntimeEr
+000135b0: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
+000135c0: 2020 2020 2066 2752 6566 7265 7368 696e       f'Refreshin
+000135d0: 6720 7374 6174 7573 2028 7b63 6c75 7374  g status ({clust
+000135e0: 6572 5f6e 616d 6521 727d 293a 2072 6179  er_name!r}): ray
+000135f0: 2073 7461 7475 7320 6e6f 7420 7368 6f77   status not show
+00013600: 696e 6720 270a 2020 2020 2020 2020 2020  ing '.          
+00013610: 2020 2020 2020 6627 616c 6c20 6e6f 6465        f'all node
+00013620: 7320 287b 7265 6164 795f 6865 6164 202b  s ({ready_head +
+00013630: 2072 6561 6479 5f77 6f72 6b65 7273 7d2f   ready_workers}/
+00013640: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+00013650: 2020 6627 7b74 6f74 616c 5f6e 6f64 6573    f'{total_nodes
+00013660: 7d29 3b20 6f75 7470 7574 3a20 7b6f 7574  }); output: {out
+00013670: 7075 747d 3b20 7374 6465 7272 3a20 7b73  put}; stderr: {s
+00013680: 7464 6572 727d 2729 0a20 2020 2020 2020  tderr}').       
+00013690: 2065 7863 6570 7420 6578 6365 7074 696f   except exceptio
+000136a0: 6e73 2e46 6574 6368 436c 7573 7465 7249  ns.FetchClusterI
+000136b0: 6e66 6f45 7272 6f72 3a0a 2020 2020 2020  nfoError:.      
+000136c0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+000136d0: 7567 280a 2020 2020 2020 2020 2020 2020  ug(.            
+000136e0: 2020 2020 6627 5265 6672 6573 6869 6e67      f'Refreshing
+000136f0: 2073 7461 7475 7320 287b 636c 7573 7465   status ({cluste
+00013700: 725f 6e61 6d65 2172 7d29 2066 6169 6c65  r_name!r}) faile
+00013710: 6420 746f 2067 6574 2049 5073 2e27 290a  d to get IPs.').
+00013720: 2020 2020 2020 2020 6578 6365 7074 2052          except R
+00013730: 756e 7469 6d65 4572 726f 7220 6173 2065  untimeError as e
+00013740: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
+00013750: 6767 6572 2e64 6562 7567 2873 7472 2865  gger.debug(str(e
+00013760: 2929 0a20 2020 2020 2020 2065 7863 6570  )).        excep
+00013770: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+00013780: 3a20 2023 2070 796c 696e 743a 2064 6973  :  # pylint: dis
+00013790: 6162 6c65 3d62 726f 6164 2d65 7863 6570  able=broad-excep
+000137a0: 740a 2020 2020 2020 2020 2020 2020 2320  t.            # 
+000137b0: 5468 6973 2063 616e 2062 6520 7261 6973  This can be rais
+000137c0: 6564 2062 7920 6065 7874 6572 6e61 6c5f  ed by `external_
+000137d0: 7373 685f 706f 7274 7328 2960 2c20 6475  ssh_ports()`, du
+000137e0: 6520 746f 2074 6865 0a20 2020 2020 2020  e to the.       
+000137f0: 2020 2020 2023 2075 6e64 6572 6c79 696e       # underlyin
+00013800: 6720 6361 6c6c 2074 6f20 6b75 6265 726e  g call to kubern
+00013810: 6574 6573 2041 5049 2e0a 2020 2020 2020  etes API..      
+00013820: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+00013830: 7567 280a 2020 2020 2020 2020 2020 2020  ug(.            
+00013840: 2020 2020 6627 5265 6672 6573 6869 6e67      f'Refreshing
+00013850: 2073 7461 7475 7320 287b 636c 7573 7465   status ({cluste
+00013860: 725f 6e61 6d65 2172 7d29 2066 6169 6c65  r_name!r}) faile
+00013870: 643a 2027 0a20 2020 2020 2020 2020 2020  d: '.           
+00013880: 2020 2020 2066 277b 636f 6d6d 6f6e 5f75       f'{common_u
+00013890: 7469 6c73 2e66 6f72 6d61 745f 6578 6365  tils.format_exce
+000138a0: 7074 696f 6e28 652c 2075 7365 5f62 7261  ption(e, use_bra
+000138b0: 636b 6574 3d54 7275 6529 7d27 290a 2020  cket=True)}').  
+000138c0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+000138d0: 7365 0a0a 2020 2020 2320 4465 7465 726d  se..    # Determ
+000138e0: 696e 696e 6720 6966 2074 6865 2063 6c75  ining if the clu
+000138f0: 7374 6572 2069 7320 6865 616c 7468 7920  ster is healthy 
+00013900: 2855 5029 3a0a 2020 2020 230a 2020 2020  (UP):.    #.    
+00013910: 2320 466f 7220 6e6f 6e2d 7370 6f74 2063  # For non-spot c
+00013920: 6c75 7374 6572 733a 2049 6620 7261 7920  lusters: If ray 
+00013930: 7374 6174 7573 2073 686f 7773 2061 6c6c  status shows all
+00013940: 206e 6f64 6573 2061 7265 2068 6561 6c74   nodes are healt
+00013950: 6879 2c20 6974 2069 730a 2020 2020 2320  hy, it is.    # 
+00013960: 7361 6665 2074 6f20 7365 7420 7468 6520  safe to set the 
+00013970: 7374 6174 7573 2074 6f20 5550 2061 7320  status to UP as 
+00013980: 7374 6172 7469 6e67 2072 6179 2069 7320  starting ray is 
+00013990: 7468 6520 6669 6e61 6c20 7374 6570 206f  the final step o
+000139a0: 6620 736b 790a 2020 2020 2320 6c61 756e  f sky.    # laun
+000139b0: 6368 2e20 4275 7420 7765 2066 6f75 6e64  ch. But we found
+000139c0: 2074 6861 7420 7261 7920 7374 6174 7573   that ray status
+000139d0: 2069 7320 7761 7920 746f 6f20 736c 6f77   is way too slow
+000139e0: 2028 7365 6520 4e4f 5445 2062 656c 6f77   (see NOTE below
+000139f0: 2920 736f 0a20 2020 2023 2077 6520 616c  ) so.    # we al
+00013a00: 7761 7973 2071 7565 7279 2074 6865 2063  ways query the c
+00013a10: 6c6f 7564 2070 726f 7669 6465 7220 6669  loud provider fi
+00013a20: 7273 7420 7768 6963 6820 6973 2066 6173  rst which is fas
+00013a30: 7465 722e 0a20 2020 2023 0a20 2020 2023  ter..    #.    #
+00013a40: 2046 6f72 2073 706f 7420 636c 7573 7465   For spot cluste
+00013a50: 7273 3a20 7468 6520 6162 6f76 6520 6361  rs: the above ca
+00013a60: 6e20 6265 2075 6e73 6166 6520 6265 6361  n be unsafe beca
+00013a70: 7573 6520 7468 6520 5261 7920 636c 7573  use the Ray clus
+00013a80: 7465 7220 6d61 790a 2020 2020 2320 7265  ter may.    # re
+00013a90: 6d61 696e 2068 6561 6c74 6879 2066 6f72  main healthy for
+00013aa0: 2061 2077 6869 6c65 2062 6566 6f72 6520   a while before 
+00013ab0: 7468 6520 636c 6f75 6420 636f 6d70 6c65  the cloud comple
+00013ac0: 7465 6c79 2070 7265 656d 7074 7320 7468  tely preempts th
+00013ad0: 6520 564d 732e 0a20 2020 2023 2057 6520  e VMs..    # We 
+00013ae0: 6861 7665 206d 6974 6967 6174 6564 2074  have mitigated t
+00013af0: 6869 7320 6279 2061 6761 696e 2066 6972  his by again fir
+00013b00: 7374 2071 7565 7279 696e 6720 7468 6520  st querying the 
+00013b10: 564d 2073 7461 7465 2066 726f 6d20 7468  VM state from th
+00013b20: 6520 636c 6f75 640a 2020 2020 2320 7072  e cloud.    # pr
+00013b30: 6f76 6964 6572 2e0a 2020 2020 6966 2061  ovider..    if a
+00013b40: 6c6c 5f6e 6f64 6573 5f75 7020 616e 6420  ll_nodes_up and 
+00013b50: 7275 6e5f 7261 795f 7374 6174 7573 5f74  run_ray_status_t
+00013b60: 6f5f 6368 6563 6b5f 7261 795f 636c 7573  o_check_ray_clus
+00013b70: 7465 725f 6865 616c 7468 7928 293a 0a20  ter_healthy():. 
+00013b80: 2020 2020 2020 2023 204e 4f54 453a 2061         # NOTE: a
+00013b90: 6c6c 5f6e 6f64 6573 5f75 7020 6361 6c63  ll_nodes_up calc
+00013ba0: 756c 6174 696f 6e20 6973 2066 6173 7420  ulation is fast 
+00013bb0: 6475 6520 746f 2063 616c 6c69 6e67 2063  due to calling c
+00013bc0: 6c6f 7564 2043 4c49 3b0a 2020 2020 2020  loud CLI;.      
+00013bd0: 2020 2320 7275 6e5f 7261 795f 7374 6174    # run_ray_stat
+00013be0: 7573 5f74 6f5f 6368 6563 6b5f 616c 6c5f  us_to_check_all_
+00013bf0: 6e6f 6465 735f 7570 2829 2069 7320 736c  nodes_up() is sl
+00013c00: 6f77 2064 7565 2074 6f20 6361 6c6c 696e  ow due to callin
+00013c10: 6720 6072 6179 2067 6574 0a20 2020 2020  g `ray get.     
+00013c20: 2020 2023 2068 6561 642d 6970 2f77 6f72     # head-ip/wor
+00013c30: 6b65 722d 6970 7360 2e0a 2020 2020 2020  ker-ips`..      
+00013c40: 2020 7265 636f 7264 5b27 7374 6174 7573    record['status
+00013c50: 275d 203d 2073 7461 7475 735f 6c69 622e  '] = status_lib.
+00013c60: 436c 7573 7465 7253 7461 7475 732e 5550  ClusterStatus.UP
+00013c70: 0a20 2020 2020 2020 2067 6c6f 6261 6c5f  .        global_
+00013c80: 7573 6572 5f73 7461 7465 2e61 6464 5f6f  user_state.add_o
+00013c90: 725f 7570 6461 7465 5f63 6c75 7374 6572  r_update_cluster
+00013ca0: 2863 6c75 7374 6572 5f6e 616d 652c 0a20  (cluster_name,. 
 00013cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013cc0: 2020 2020 2020 2068 616e 646c 652c 0a20         handle,. 
-00013cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013cf0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00013d00: 6571 7565 7374 6564 5f72 6573 6f75 7263  equested_resourc
-00013d10: 6573 3d4e 6f6e 652c 0a20 2020 2020 2020  es=None,.       
-00013d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d40: 2020 2020 2020 2020 2072 6561 6479 3d54           ready=T
-00013d50: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-00013d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013cd0: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+00013ce0: 616e 646c 652c 0a20 2020 2020 2020 2020  andle,.         
+00013cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d10: 2020 2020 2020 2072 6571 7565 7374 6564         requested
+00013d20: 5f72 6573 6f75 7263 6573 3d4e 6f6e 652c  _resources=None,
+00013d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d60: 2072 6561 6479 3d54 7275 652c 0a20 2020   ready=True,.   
 00013d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d80: 2020 2020 2069 735f 6c61 756e 6368 3d46       is_launch=F
-00013d90: 616c 7365 290a 2020 2020 2020 2020 7265  alse).        re
-00013da0: 7475 726e 2072 6563 6f72 640a 0a20 2020  turn record..   
-00013db0: 2023 2041 6c6c 2063 6173 6573 2062 656c   # All cases bel
-00013dc0: 6f77 2061 7265 2074 7261 6e73 6974 696f  ow are transitio
-00013dd0: 6e69 6e67 2074 6865 2063 6c75 7374 6572  ning the cluster
-00013de0: 2074 6f20 6e6f 6e2d 5550 2073 7461 7465   to non-UP state
-00013df0: 732e 0a20 2020 2069 6620 6c65 6e28 6e6f  s..    if len(no
-00013e00: 6465 5f73 7461 7475 7365 7329 203e 2068  de_statuses) > h
-00013e10: 616e 646c 652e 6c61 756e 6368 6564 5f6e  andle.launched_n
-00013e20: 6f64 6573 3a0a 2020 2020 2020 2020 2320  odes:.        # 
-00013e30: 556e 6578 7065 6374 6564 3a20 696e 2074  Unexpected: in t
-00013e40: 6865 2071 7565 7269 6564 2072 6567 696f  he queried regio
-00013e50: 6e20 6d6f 7265 2074 6861 6e20 3120 636c  n more than 1 cl
-00013e60: 7573 7465 7220 7769 7468 2074 6865 2073  uster with the s
-00013e70: 616d 650a 2020 2020 2020 2020 2320 636f  ame.        # co
-00013e80: 6e73 7472 7563 7465 6420 6e61 6d65 2074  nstructed name t
-00013e90: 6167 2072 6574 7572 6e65 642e 2054 6869  ag returned. Thi
-00013ea0: 7320 7769 6c6c 2074 7970 6963 616c 6c79  s will typically
-00013eb0: 206e 6f74 2068 6170 7065 6e20 756e 6c65   not happen unle
-00013ec0: 7373 0a20 2020 2020 2020 2023 2075 7365  ss.        # use
-00013ed0: 7273 206d 616e 7561 6c6c 7920 6372 6561  rs manually crea
-00013ee0: 7465 2061 2063 6c75 7374 6572 2077 6974  te a cluster wit
-00013ef0: 6820 7468 6174 2063 6f6e 7374 7275 6374  h that construct
-00013f00: 6564 206e 616d 6520 6f72 2074 6865 7265  ed name or there
-00013f10: 0a20 2020 2020 2020 2023 2077 6173 2061  .        # was a
-00013f20: 2072 6573 6f75 7263 6520 6c65 616b 2063   resource leak c
-00013f30: 6175 7365 6420 6279 2064 6966 6665 7265  aused by differe
-00013f40: 6e74 206c 6175 6e63 6820 6861 7368 2062  nt launch hash b
-00013f50: 6566 6f72 6520 2331 3637 310a 2020 2020  efore #1671.    
-00013f60: 2020 2020 2320 7761 7320 6d65 7267 6564      # was merged
-00013f70: 2e0a 2020 2020 2020 2020 230a 2020 2020  ..        #.    
-00013f80: 2020 2020 2320 2854 6563 686e 6963 616c      # (Technical
-00013f90: 6c79 2073 7065 616b 696e 672c 2065 7665  ly speaking, eve
-00013fa0: 6e20 6966 2072 6574 7572 6e65 6420 6e75  n if returned nu
-00013fb0: 6d20 6e6f 6465 7320 3c3d 206e 756d 0a20  m nodes <= num. 
-00013fc0: 2020 2020 2020 2023 2068 616e 646c 652e         # handle.
-00013fd0: 6c61 756e 6368 6564 5f6e 6f64 6573 292c  launched_nodes),
-00013fe0: 206e 6f74 2069 6e63 6c75 6469 6e67 2074   not including t
-00013ff0: 6865 206c 6175 6e63 6820 6861 7368 2063  he launch hash c
-00014000: 6f75 6c64 206d 6561 6e20 7468 650a 2020  ould mean the.  
-00014010: 2020 2020 2020 2320 7265 7475 726e 6564        # returned
-00014020: 206e 6f64 6573 2063 6f6e 7461 696e 2073   nodes contain s
-00014030: 6f6d 6520 6e6f 6465 7320 7468 6174 2064  ome nodes that d
-00014040: 6f20 6e6f 7420 6265 6c6f 6e67 2074 6f20  o not belong to 
-00014050: 7468 6520 6c6f 6769 6361 6c0a 2020 2020  the logical.    
-00014060: 2020 2020 2320 736b 7970 696c 6f74 2063      # skypilot c
-00014070: 6c75 7374 6572 2e20 446f 6573 6e27 7420  luster. Doesn't 
-00014080: 7365 656d 2074 6f20 6265 2061 2067 6f6f  seem to be a goo
-00014090: 6420 7761 7920 746f 2068 616e 646c 6520  d way to handle 
-000140a0: 7468 6973 2066 6f72 0a20 2020 2020 2020  this for.       
-000140b0: 2023 206e 6f77 3f29 0a20 2020 2020 2020   # now?).       
-000140c0: 2023 0a20 2020 2020 2020 2023 2057 6520   #.        # We 
-000140d0: 6861 7665 206e 6f74 2065 7870 6572 6965  have not experie
-000140e0: 6e63 6564 2074 6865 2061 626f 7665 3b20  nced the above; 
-000140f0: 6164 6469 6e67 2061 7320 6120 7361 6665  adding as a safe
-00014100: 6775 6172 642e 0a20 2020 2020 2020 2023  guard..        #
-00014110: 0a20 2020 2020 2020 2023 2053 696e 6365  .        # Since
-00014120: 2077 6520 6661 696c 6564 2074 6f20 7265   we failed to re
-00014130: 6672 6573 682c 2072 6169 7365 2074 6865  fresh, raise the
-00014140: 2073 7461 7475 7320 6665 7463 6869 6e67   status fetching
-00014150: 2065 7272 6f72 2e0a 2020 2020 2020 2020   error..        
-00014160: 7769 7468 2075 785f 7574 696c 732e 7072  with ux_utils.pr
-00014170: 696e 745f 6578 6365 7074 696f 6e5f 6e6f  int_exception_no
-00014180: 5f74 7261 6365 6261 636b 2829 3a0a 2020  _traceback():.  
-00014190: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000141a0: 6578 6365 7074 696f 6e73 2e43 6c75 7374  exceptions.Clust
-000141b0: 6572 5374 6174 7573 4665 7463 6869 6e67  erStatusFetching
-000141c0: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
-000141d0: 2020 2020 2020 2066 2746 6f75 6e64 207b         f'Found {
-000141e0: 6c65 6e28 6e6f 6465 5f73 7461 7475 7365  len(node_statuse
-000141f0: 7329 7d20 6e6f 6465 2873 2920 7769 7468  s)} node(s) with
-00014200: 2074 6865 2073 616d 6520 636c 7573 7465   the same cluste
-00014210: 7220 6e61 6d65 270a 2020 2020 2020 2020  r name'.        
-00014220: 2020 2020 2020 2020 6627 2074 6167 2069          f' tag i
-00014230: 6e20 7468 6520 636c 6f75 6420 7072 6f76  n the cloud prov
-00014240: 6964 6572 2066 6f72 2063 6c75 7374 6572  ider for cluster
-00014250: 207b 636c 7573 7465 725f 6e61 6d65 2172   {cluster_name!r
-00014260: 7d2c 2027 0a20 2020 2020 2020 2020 2020  }, '.           
-00014270: 2020 2020 2066 2777 6869 6368 2073 686f       f'which sho
-00014280: 756c 6420 6861 7665 207b 6861 6e64 6c65  uld have {handle
-00014290: 2e6c 6175 6e63 6865 645f 6e6f 6465 737d  .launched_nodes}
-000142a0: 206e 6f64 6573 2e20 5468 6973 2027 0a20   nodes. This '. 
-000142b0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000142c0: 276e 6f72 6d61 6c6c 7920 7368 6f75 6c64  'normally should
-000142d0: 206e 6f74 2068 6170 7065 6e2e 207b 636f   not happen. {co
-000142e0: 6c6f 7261 6d61 2e46 6f72 652e 5245 447d  lorama.Fore.RED}
-000142f0: 506c 6561 7365 2063 6865 636b 2027 0a20  Please check '. 
-00014300: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00014310: 7468 6520 636c 6f75 6420 636f 6e73 6f6c  the cloud consol
-00014320: 6520 616e 6420 6669 7820 616e 7920 706f  e and fix any po
-00014330: 7373 6962 6c65 2072 6573 6f75 7263 6573  ssible resources
-00014340: 206c 6561 6b61 6765 2027 0a20 2020 2020   leakage '.     
-00014350: 2020 2020 2020 2020 2020 2027 2865 2e67             '(e.g
-00014360: 2e2c 2069 6620 7468 6572 6520 6172 6520  ., if there are 
-00014370: 616e 7920 7374 6f70 7065 6420 6e6f 6465  any stopped node
-00014380: 7320 616e 6420 7468 6579 2064 6f20 6e6f  s and they do no
-00014390: 7420 6861 7665 2027 0a20 2020 2020 2020  t have '.       
-000143a0: 2020 2020 2020 2020 2027 6461 7461 206f           'data o
-000143b0: 7220 6172 6520 756e 6865 616c 7468 792c  r are unhealthy,
-000143c0: 2074 6572 6d69 6e61 7465 2074 6865 6d29   terminate them)
-000143d0: 2e27 0a20 2020 2020 2020 2020 2020 2020  .'.             
-000143e0: 2020 2066 277b 636f 6c6f 7261 6d61 2e53     f'{colorama.S
-000143f0: 7479 6c65 2e52 4553 4554 5f41 4c4c 7d27  tyle.RESET_ALL}'
-00014400: 290a 2020 2020 6173 7365 7274 206c 656e  ).    assert len
-00014410: 286e 6f64 655f 7374 6174 7573 6573 2920  (node_statuses) 
-00014420: 3c3d 2068 616e 646c 652e 6c61 756e 6368  <= handle.launch
-00014430: 6564 5f6e 6f64 6573 0a0a 2020 2020 2320  ed_nodes..    # 
-00014440: 4966 2074 6865 206e 6f64 655f 7374 6174  If the node_stat
-00014450: 7573 6573 2069 7320 656d 7074 792c 2061  uses is empty, a
-00014460: 6c6c 2074 6865 206e 6f64 6573 2061 7265  ll the nodes are
-00014470: 2074 6572 6d69 6e61 7465 642e 2057 6520   terminated. We 
-00014480: 6361 6e0a 2020 2020 2320 7361 6665 6c79  can.    # safely
-00014490: 2073 6574 2074 6865 2063 6c75 7374 6572   set the cluster
-000144a0: 2073 7461 7475 7320 746f 2054 4552 4d49   status to TERMI
-000144b0: 4e41 5445 442e 2054 6869 7320 6861 6e64  NATED. This hand
-000144c0: 6c65 7320 7468 6520 6564 6765 2063 6173  les the edge cas
-000144d0: 650a 2020 2020 2320 7768 6572 6520 7468  e.    # where th
-000144e0: 6520 636c 7573 7465 7220 6973 2074 6572  e cluster is ter
-000144f0: 6d69 6e61 7465 6420 6279 2074 6865 2075  minated by the u
-00014500: 7365 7220 6d61 6e75 616c 6c79 2074 6872  ser manually thr
-00014510: 6f75 6768 2074 6865 2055 492e 0a20 2020  ough the UI..   
-00014520: 2074 6f5f 7465 726d 696e 6174 6520 3d20   to_terminate = 
-00014530: 6e6f 7420 6e6f 6465 5f73 7461 7475 7365  not node_statuse
-00014540: 730a 0a20 2020 2023 2041 2063 6c75 7374  s..    # A clust
-00014550: 6572 2069 7320 636f 6e73 6964 6572 6564  er is considered
-00014560: 2022 6162 6e6f 726d 616c 222c 2069 6620   "abnormal", if 
-00014570: 6e6f 7420 616c 6c20 6e6f 6465 7320 6172  not all nodes ar
-00014580: 6520 5445 524d 494e 4154 4544 206f 720a  e TERMINATED or.
-00014590: 2020 2020 2320 6e6f 7420 616c 6c20 6e6f      # not all no
-000145a0: 6465 7320 6172 6520 5354 4f50 5045 442e  des are STOPPED.
-000145b0: 2057 6520 6368 6563 6b20 7468 6174 2077   We check that w
-000145c0: 6974 6820 7468 6520 666f 6c6c 6f77 696e  ith the followin
-000145d0: 6720 6c6f 6769 633a 0a20 2020 2023 2020  g logic:.    #  
-000145e0: 202a 204e 6f74 2061 6c6c 206e 6f64 6573   * Not all nodes
-000145f0: 2061 7265 2074 6572 6d69 6e61 7465 6420   are terminated 
-00014600: 616e 6420 7468 6572 6527 7320 6174 206c  and there's at l
-00014610: 6561 7374 206f 6e65 206e 6f64 650a 2020  east one node.  
-00014620: 2020 2320 2020 2020 7465 726d 696e 6174    #     terminat
-00014630: 6564 3b20 6f72 0a20 2020 2023 2020 202a  ed; or.    #   *
-00014640: 2041 6e79 206f 6620 7468 6520 6e6f 6e2d   Any of the non-
-00014650: 5445 524d 494e 4154 4544 206e 6f64 6573  TERMINATED nodes
-00014660: 2069 7320 696e 2061 206e 6f6e 2d53 544f   is in a non-STO
-00014670: 5050 4544 2073 7461 7475 732e 0a20 2020  PPED status..   
-00014680: 2023 0a20 2020 2023 2054 6869 7320 696e   #.    # This in
-00014690: 636c 7564 6573 2074 6865 7365 2073 7065  cludes these spe
-000146a0: 6369 616c 2063 6173 6573 3a0a 2020 2020  cial cases:.    
-000146b0: 2320 2020 2a20 416c 6c20 7374 6f70 7065  #   * All stoppe
-000146c0: 6420 6172 6520 636f 6e73 6964 6572 6564  d are considered
-000146d0: 206e 6f72 6d61 6c20 616e 6420 7769 6c6c   normal and will
-000146e0: 2062 6520 636c 6561 6e65 6420 7570 2061   be cleaned up a
-000146f0: 7420 7468 6520 656e 640a 2020 2020 2320  t the end.    # 
-00014700: 2020 2020 6f66 2074 6865 2066 756e 6374      of the funct
-00014710: 696f 6e2e 0a20 2020 2023 2020 202a 2053  ion..    #   * S
-00014720: 6f6d 6520 6f66 2074 6865 206e 6f64 6573  ome of the nodes
-00014730: 2055 5020 7368 6f75 6c64 2062 6520 636f   UP should be co
-00014740: 6e73 6964 6572 6564 2061 626e 6f72 6d61  nsidered abnorma
-00014750: 6c2c 2062 6563 6175 7365 2074 6865 2072  l, because the r
-00014760: 6179 0a20 2020 2023 2020 2020 2063 6c75  ay.    #     clu
-00014770: 7374 6572 2069 7320 7072 6f62 6162 6c79  ster is probably
-00014780: 2064 6f77 6e2e 0a20 2020 2023 2020 202a   down..    #   *
-00014790: 2054 6865 2063 6c75 7374 6572 2069 7320   The cluster is 
-000147a0: 7061 7274 6961 6c6c 7920 7465 726d 696e  partially termin
-000147b0: 6174 6564 206f 7220 7374 6f70 7065 6420  ated or stopped 
-000147c0: 7368 6f75 6c64 2062 6520 636f 6e73 6964  should be consid
-000147d0: 6572 6564 0a20 2020 2023 2020 2020 2061  ered.    #     a
-000147e0: 626e 6f72 6d61 6c2e 0a20 2020 2023 0a20  bnormal..    #. 
-000147f0: 2020 2023 2041 6e20 6162 6e6f 726d 616c     # An abnormal
-00014800: 2063 6c75 7374 6572 2077 696c 6c20 7472   cluster will tr
-00014810: 616e 7369 7469 6f6e 2074 6f20 494e 4954  ansition to INIT
-00014820: 2061 6e64 2068 6176 6520 616e 7920 6175   and have any au
-00014830: 746f 7374 6f70 2073 6574 7469 6e67 0a20  tostop setting. 
-00014840: 2020 2023 2072 6573 6574 2028 756e 6c65     # reset (unle
-00014850: 7373 2069 7427 7320 6175 746f 7374 6f70  ss it's autostop
-00014860: 7069 6e67 2f61 7574 6f64 6f77 6e69 6e67  ping/autodowning
-00014870: 292e 0a20 2020 2069 735f 6162 6e6f 726d  )..    is_abnorm
-00014880: 616c 203d 2028 2830 203c 206c 656e 286e  al = ((0 < len(n
-00014890: 6f64 655f 7374 6174 7573 6573 2920 3c20  ode_statuses) < 
-000148a0: 6861 6e64 6c65 2e6c 6175 6e63 6865 645f  handle.launched_
-000148b0: 6e6f 6465 7329 206f 7220 616e 7928 0a20  nodes) or any(. 
-000148c0: 2020 2020 2020 2073 7461 7475 7320 213d         status !=
-000148d0: 2073 7461 7475 735f 6c69 622e 436c 7573   status_lib.Clus
-000148e0: 7465 7253 7461 7475 732e 5354 4f50 5045  terStatus.STOPPE
-000148f0: 4420 666f 7220 7374 6174 7573 2069 6e20  D for status in 
-00014900: 6e6f 6465 5f73 7461 7475 7365 7329 290a  node_statuses)).
-00014910: 2020 2020 6966 2069 735f 6162 6e6f 726d      if is_abnorm
-00014920: 616c 3a0a 2020 2020 2020 2020 6c6f 6767  al:.        logg
-00014930: 6572 2e64 6562 7567 2827 5468 6520 636c  er.debug('The cl
-00014940: 7573 7465 7220 6973 2061 626e 6f72 6d61  uster is abnorma
-00014950: 6c2e 2053 6574 7469 6e67 2074 6f20 494e  l. Setting to IN
-00014960: 4954 2073 7461 7475 732e 2027 0a20 2020  IT status. '.   
-00014970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014980: 2020 6627 6e6f 6465 5f73 7461 7475 7365    f'node_statuse
-00014990: 733a 207b 6e6f 6465 5f73 7461 7475 7365  s: {node_statuse
-000149a0: 737d 2729 0a20 2020 2020 2020 2062 6163  s}').        bac
-000149b0: 6b65 6e64 203d 2067 6574 5f62 6163 6b65  kend = get_backe
-000149c0: 6e64 5f66 726f 6d5f 6861 6e64 6c65 2868  nd_from_handle(h
-000149d0: 616e 646c 6529 0a20 2020 2020 2020 2069  andle).        i
-000149e0: 6620 6973 696e 7374 616e 6365 2862 6163  f isinstance(bac
-000149f0: 6b65 6e64 2c0a 2020 2020 2020 2020 2020  kend,.          
-00014a00: 2020 2020 2020 2020 2020 2020 6261 636b              back
-00014a10: 656e 6473 2e43 6c6f 7564 566d 5261 7942  ends.CloudVmRayB
-00014a20: 6163 6b65 6e64 2920 616e 6420 7265 636f  ackend) and reco
-00014a30: 7264 5b27 6175 746f 7374 6f70 275d 203e  rd['autostop'] >
-00014a40: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-00014a50: 2069 6620 6e6f 7420 6261 636b 656e 642e   if not backend.
-00014a60: 6973 5f64 6566 696e 6974 656c 795f 6175  is_definitely_au
-00014a70: 746f 7374 6f70 7069 6e67 2868 616e 646c  tostopping(handl
-00014a80: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00014a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d90: 2020 2020 2020 2020 2020 2020 2069 735f               is_
+00013da0: 6c61 756e 6368 3d46 616c 7365 290a 2020  launch=False).  
+00013db0: 2020 2020 2020 7265 7475 726e 2072 6563        return rec
+00013dc0: 6f72 640a 0a20 2020 2023 2041 6c6c 2063  ord..    # All c
+00013dd0: 6173 6573 2062 656c 6f77 2061 7265 2074  ases below are t
+00013de0: 7261 6e73 6974 696f 6e69 6e67 2074 6865  ransitioning the
+00013df0: 2063 6c75 7374 6572 2074 6f20 6e6f 6e2d   cluster to non-
+00013e00: 5550 2073 7461 7465 732e 0a20 2020 2069  UP states..    i
+00013e10: 6620 6c65 6e28 6e6f 6465 5f73 7461 7475  f len(node_statu
+00013e20: 7365 7329 203e 2068 616e 646c 652e 6c61  ses) > handle.la
+00013e30: 756e 6368 6564 5f6e 6f64 6573 3a0a 2020  unched_nodes:.  
+00013e40: 2020 2020 2020 2320 556e 6578 7065 6374        # Unexpect
+00013e50: 6564 3a20 696e 2074 6865 2071 7565 7269  ed: in the queri
+00013e60: 6564 2072 6567 696f 6e20 6d6f 7265 2074  ed region more t
+00013e70: 6861 6e20 3120 636c 7573 7465 7220 7769  han 1 cluster wi
+00013e80: 7468 2074 6865 2073 616d 650a 2020 2020  th the same.    
+00013e90: 2020 2020 2320 636f 6e73 7472 7563 7465      # constructe
+00013ea0: 6420 6e61 6d65 2074 6167 2072 6574 7572  d name tag retur
+00013eb0: 6e65 642e 2054 6869 7320 7769 6c6c 2074  ned. This will t
+00013ec0: 7970 6963 616c 6c79 206e 6f74 2068 6170  ypically not hap
+00013ed0: 7065 6e20 756e 6c65 7373 0a20 2020 2020  pen unless.     
+00013ee0: 2020 2023 2075 7365 7273 206d 616e 7561     # users manua
+00013ef0: 6c6c 7920 6372 6561 7465 2061 2063 6c75  lly create a clu
+00013f00: 7374 6572 2077 6974 6820 7468 6174 2063  ster with that c
+00013f10: 6f6e 7374 7275 6374 6564 206e 616d 6520  onstructed name 
+00013f20: 6f72 2074 6865 7265 0a20 2020 2020 2020  or there.       
+00013f30: 2023 2077 6173 2061 2072 6573 6f75 7263   # was a resourc
+00013f40: 6520 6c65 616b 2063 6175 7365 6420 6279  e leak caused by
+00013f50: 2064 6966 6665 7265 6e74 206c 6175 6e63   different launc
+00013f60: 6820 6861 7368 2062 6566 6f72 6520 2331  h hash before #1
+00013f70: 3637 310a 2020 2020 2020 2020 2320 7761  671.        # wa
+00013f80: 7320 6d65 7267 6564 2e0a 2020 2020 2020  s merged..      
+00013f90: 2020 230a 2020 2020 2020 2020 2320 2854    #.        # (T
+00013fa0: 6563 686e 6963 616c 6c79 2073 7065 616b  echnically speak
+00013fb0: 696e 672c 2065 7665 6e20 6966 2072 6574  ing, even if ret
+00013fc0: 7572 6e65 6420 6e75 6d20 6e6f 6465 7320  urned num nodes 
+00013fd0: 3c3d 206e 756d 0a20 2020 2020 2020 2023  <= num.        #
+00013fe0: 2068 616e 646c 652e 6c61 756e 6368 6564   handle.launched
+00013ff0: 5f6e 6f64 6573 292c 206e 6f74 2069 6e63  _nodes), not inc
+00014000: 6c75 6469 6e67 2074 6865 206c 6175 6e63  luding the launc
+00014010: 6820 6861 7368 2063 6f75 6c64 206d 6561  h hash could mea
+00014020: 6e20 7468 650a 2020 2020 2020 2020 2320  n the.        # 
+00014030: 7265 7475 726e 6564 206e 6f64 6573 2063  returned nodes c
+00014040: 6f6e 7461 696e 2073 6f6d 6520 6e6f 6465  ontain some node
+00014050: 7320 7468 6174 2064 6f20 6e6f 7420 6265  s that do not be
+00014060: 6c6f 6e67 2074 6f20 7468 6520 6c6f 6769  long to the logi
+00014070: 6361 6c0a 2020 2020 2020 2020 2320 736b  cal.        # sk
+00014080: 7970 696c 6f74 2063 6c75 7374 6572 2e20  ypilot cluster. 
+00014090: 446f 6573 6e27 7420 7365 656d 2074 6f20  Doesn't seem to 
+000140a0: 6265 2061 2067 6f6f 6420 7761 7920 746f  be a good way to
+000140b0: 2068 616e 646c 6520 7468 6973 2066 6f72   handle this for
+000140c0: 0a20 2020 2020 2020 2023 206e 6f77 3f29  .        # now?)
+000140d0: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
+000140e0: 2020 2023 2057 6520 6861 7665 206e 6f74     # We have not
+000140f0: 2065 7870 6572 6965 6e63 6564 2074 6865   experienced the
+00014100: 2061 626f 7665 3b20 6164 6469 6e67 2061   above; adding a
+00014110: 7320 6120 7361 6665 6775 6172 642e 0a20  s a safeguard.. 
+00014120: 2020 2020 2020 2023 0a20 2020 2020 2020         #.       
+00014130: 2023 2053 696e 6365 2077 6520 6661 696c   # Since we fail
+00014140: 6564 2074 6f20 7265 6672 6573 682c 2072  ed to refresh, r
+00014150: 6169 7365 2074 6865 2073 7461 7475 7320  aise the status 
+00014160: 6665 7463 6869 6e67 2065 7272 6f72 2e0a  fetching error..
+00014170: 2020 2020 2020 2020 7769 7468 2075 785f          with ux_
+00014180: 7574 696c 732e 7072 696e 745f 6578 6365  utils.print_exce
+00014190: 7074 696f 6e5f 6e6f 5f74 7261 6365 6261  ption_no_traceba
+000141a0: 636b 2829 3a0a 2020 2020 2020 2020 2020  ck():.          
+000141b0: 2020 7261 6973 6520 6578 6365 7074 696f    raise exceptio
+000141c0: 6e73 2e43 6c75 7374 6572 5374 6174 7573  ns.ClusterStatus
+000141d0: 4665 7463 6869 6e67 4572 726f 7228 0a20  FetchingError(. 
+000141e0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000141f0: 2746 6f75 6e64 207b 6c65 6e28 6e6f 6465  'Found {len(node
+00014200: 5f73 7461 7475 7365 7329 7d20 6e6f 6465  _statuses)} node
+00014210: 2873 2920 7769 7468 2074 6865 2073 616d  (s) with the sam
+00014220: 6520 636c 7573 7465 7220 6e61 6d65 270a  e cluster name'.
+00014230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014240: 6627 2074 6167 2069 6e20 7468 6520 636c  f' tag in the cl
+00014250: 6f75 6420 7072 6f76 6964 6572 2066 6f72  oud provider for
+00014260: 2063 6c75 7374 6572 207b 636c 7573 7465   cluster {cluste
+00014270: 725f 6e61 6d65 2172 7d2c 2027 0a20 2020  r_name!r}, '.   
+00014280: 2020 2020 2020 2020 2020 2020 2066 2777               f'w
+00014290: 6869 6368 2073 686f 756c 6420 6861 7665  hich should have
+000142a0: 207b 6861 6e64 6c65 2e6c 6175 6e63 6865   {handle.launche
+000142b0: 645f 6e6f 6465 737d 206e 6f64 6573 2e20  d_nodes} nodes. 
+000142c0: 5468 6973 2027 0a20 2020 2020 2020 2020  This '.         
+000142d0: 2020 2020 2020 2066 276e 6f72 6d61 6c6c         f'normall
+000142e0: 7920 7368 6f75 6c64 206e 6f74 2068 6170  y should not hap
+000142f0: 7065 6e2e 207b 636f 6c6f 7261 6d61 2e46  pen. {colorama.F
+00014300: 6f72 652e 5245 447d 506c 6561 7365 2063  ore.RED}Please c
+00014310: 6865 636b 2027 0a20 2020 2020 2020 2020  heck '.         
+00014320: 2020 2020 2020 2027 7468 6520 636c 6f75         'the clou
+00014330: 6420 636f 6e73 6f6c 6520 616e 6420 6669  d console and fi
+00014340: 7820 616e 7920 706f 7373 6962 6c65 2072  x any possible r
+00014350: 6573 6f75 7263 6573 206c 6561 6b61 6765  esources leakage
+00014360: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
+00014370: 2020 2027 2865 2e67 2e2c 2069 6620 7468     '(e.g., if th
+00014380: 6572 6520 6172 6520 616e 7920 7374 6f70  ere are any stop
+00014390: 7065 6420 6e6f 6465 7320 616e 6420 7468  ped nodes and th
+000143a0: 6579 2064 6f20 6e6f 7420 6861 7665 2027  ey do not have '
+000143b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000143c0: 2027 6461 7461 206f 7220 6172 6520 756e   'data or are un
+000143d0: 6865 616c 7468 792c 2074 6572 6d69 6e61  healthy, termina
+000143e0: 7465 2074 6865 6d29 2e27 0a20 2020 2020  te them).'.     
+000143f0: 2020 2020 2020 2020 2020 2066 277b 636f             f'{co
+00014400: 6c6f 7261 6d61 2e53 7479 6c65 2e52 4553  lorama.Style.RES
+00014410: 4554 5f41 4c4c 7d27 290a 2020 2020 6173  ET_ALL}').    as
+00014420: 7365 7274 206c 656e 286e 6f64 655f 7374  sert len(node_st
+00014430: 6174 7573 6573 2920 3c3d 2068 616e 646c  atuses) <= handl
+00014440: 652e 6c61 756e 6368 6564 5f6e 6f64 6573  e.launched_nodes
+00014450: 0a0a 2020 2020 2320 4966 2074 6865 206e  ..    # If the n
+00014460: 6f64 655f 7374 6174 7573 6573 2069 7320  ode_statuses is 
+00014470: 656d 7074 792c 2061 6c6c 2074 6865 206e  empty, all the n
+00014480: 6f64 6573 2061 7265 2074 6572 6d69 6e61  odes are termina
+00014490: 7465 642e 2057 6520 6361 6e0a 2020 2020  ted. We can.    
+000144a0: 2320 7361 6665 6c79 2073 6574 2074 6865  # safely set the
+000144b0: 2063 6c75 7374 6572 2073 7461 7475 7320   cluster status 
+000144c0: 746f 2054 4552 4d49 4e41 5445 442e 2054  to TERMINATED. T
+000144d0: 6869 7320 6861 6e64 6c65 7320 7468 6520  his handles the 
+000144e0: 6564 6765 2063 6173 650a 2020 2020 2320  edge case.    # 
+000144f0: 7768 6572 6520 7468 6520 636c 7573 7465  where the cluste
+00014500: 7220 6973 2074 6572 6d69 6e61 7465 6420  r is terminated 
+00014510: 6279 2074 6865 2075 7365 7220 6d61 6e75  by the user manu
+00014520: 616c 6c79 2074 6872 6f75 6768 2074 6865  ally through the
+00014530: 2055 492e 0a20 2020 2074 6f5f 7465 726d   UI..    to_term
+00014540: 696e 6174 6520 3d20 6e6f 7420 6e6f 6465  inate = not node
+00014550: 5f73 7461 7475 7365 730a 0a20 2020 2023  _statuses..    #
+00014560: 2041 2063 6c75 7374 6572 2069 7320 636f   A cluster is co
+00014570: 6e73 6964 6572 6564 2022 6162 6e6f 726d  nsidered "abnorm
+00014580: 616c 222c 2069 6620 6e6f 7420 616c 6c20  al", if not all 
+00014590: 6e6f 6465 7320 6172 6520 5445 524d 494e  nodes are TERMIN
+000145a0: 4154 4544 206f 720a 2020 2020 2320 6e6f  ATED or.    # no
+000145b0: 7420 616c 6c20 6e6f 6465 7320 6172 6520  t all nodes are 
+000145c0: 5354 4f50 5045 442e 2057 6520 6368 6563  STOPPED. We chec
+000145d0: 6b20 7468 6174 2077 6974 6820 7468 6520  k that with the 
+000145e0: 666f 6c6c 6f77 696e 6720 6c6f 6769 633a  following logic:
+000145f0: 0a20 2020 2023 2020 202a 204e 6f74 2061  .    #   * Not a
+00014600: 6c6c 206e 6f64 6573 2061 7265 2074 6572  ll nodes are ter
+00014610: 6d69 6e61 7465 6420 616e 6420 7468 6572  minated and ther
+00014620: 6527 7320 6174 206c 6561 7374 206f 6e65  e's at least one
+00014630: 206e 6f64 650a 2020 2020 2320 2020 2020   node.    #     
+00014640: 7465 726d 696e 6174 6564 3b20 6f72 0a20  terminated; or. 
+00014650: 2020 2023 2020 202a 2041 6e79 206f 6620     #   * Any of 
+00014660: 7468 6520 6e6f 6e2d 5445 524d 494e 4154  the non-TERMINAT
+00014670: 4544 206e 6f64 6573 2069 7320 696e 2061  ED nodes is in a
+00014680: 206e 6f6e 2d53 544f 5050 4544 2073 7461   non-STOPPED sta
+00014690: 7475 732e 0a20 2020 2023 0a20 2020 2023  tus..    #.    #
+000146a0: 2054 6869 7320 696e 636c 7564 6573 2074   This includes t
+000146b0: 6865 7365 2073 7065 6369 616c 2063 6173  hese special cas
+000146c0: 6573 3a0a 2020 2020 2320 2020 2a20 416c  es:.    #   * Al
+000146d0: 6c20 7374 6f70 7065 6420 6172 6520 636f  l stopped are co
+000146e0: 6e73 6964 6572 6564 206e 6f72 6d61 6c20  nsidered normal 
+000146f0: 616e 6420 7769 6c6c 2062 6520 636c 6561  and will be clea
+00014700: 6e65 6420 7570 2061 7420 7468 6520 656e  ned up at the en
+00014710: 640a 2020 2020 2320 2020 2020 6f66 2074  d.    #     of t
+00014720: 6865 2066 756e 6374 696f 6e2e 0a20 2020  he function..   
+00014730: 2023 2020 202a 2053 6f6d 6520 6f66 2074   #   * Some of t
+00014740: 6865 206e 6f64 6573 2055 5020 7368 6f75  he nodes UP shou
+00014750: 6c64 2062 6520 636f 6e73 6964 6572 6564  ld be considered
+00014760: 2061 626e 6f72 6d61 6c2c 2062 6563 6175   abnormal, becau
+00014770: 7365 2074 6865 2072 6179 0a20 2020 2023  se the ray.    #
+00014780: 2020 2020 2063 6c75 7374 6572 2069 7320       cluster is 
+00014790: 7072 6f62 6162 6c79 2064 6f77 6e2e 0a20  probably down.. 
+000147a0: 2020 2023 2020 202a 2054 6865 2063 6c75     #   * The clu
+000147b0: 7374 6572 2069 7320 7061 7274 6961 6c6c  ster is partiall
+000147c0: 7920 7465 726d 696e 6174 6564 206f 7220  y terminated or 
+000147d0: 7374 6f70 7065 6420 7368 6f75 6c64 2062  stopped should b
+000147e0: 6520 636f 6e73 6964 6572 6564 0a20 2020  e considered.   
+000147f0: 2023 2020 2020 2061 626e 6f72 6d61 6c2e   #     abnormal.
+00014800: 0a20 2020 2023 0a20 2020 2023 2041 6e20  .    #.    # An 
+00014810: 6162 6e6f 726d 616c 2063 6c75 7374 6572  abnormal cluster
+00014820: 2077 696c 6c20 7472 616e 7369 7469 6f6e   will transition
+00014830: 2074 6f20 494e 4954 2061 6e64 2068 6176   to INIT and hav
+00014840: 6520 616e 7920 6175 746f 7374 6f70 2073  e any autostop s
+00014850: 6574 7469 6e67 0a20 2020 2023 2072 6573  etting.    # res
+00014860: 6574 2028 756e 6c65 7373 2069 7427 7320  et (unless it's 
+00014870: 6175 746f 7374 6f70 7069 6e67 2f61 7574  autostopping/aut
+00014880: 6f64 6f77 6e69 6e67 292e 0a20 2020 2069  odowning)..    i
+00014890: 735f 6162 6e6f 726d 616c 203d 2028 2830  s_abnormal = ((0
+000148a0: 203c 206c 656e 286e 6f64 655f 7374 6174   < len(node_stat
+000148b0: 7573 6573 2920 3c20 6861 6e64 6c65 2e6c  uses) < handle.l
+000148c0: 6175 6e63 6865 645f 6e6f 6465 7329 206f  aunched_nodes) o
+000148d0: 7220 616e 7928 0a20 2020 2020 2020 2073  r any(.        s
+000148e0: 7461 7475 7320 213d 2073 7461 7475 735f  tatus != status_
+000148f0: 6c69 622e 436c 7573 7465 7253 7461 7475  lib.ClusterStatu
+00014900: 732e 5354 4f50 5045 4420 666f 7220 7374  s.STOPPED for st
+00014910: 6174 7573 2069 6e20 6e6f 6465 5f73 7461  atus in node_sta
+00014920: 7475 7365 7329 290a 2020 2020 6966 2069  tuses)).    if i
+00014930: 735f 6162 6e6f 726d 616c 3a0a 2020 2020  s_abnormal:.    
+00014940: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+00014950: 2827 5468 6520 636c 7573 7465 7220 6973  ('The cluster is
+00014960: 2061 626e 6f72 6d61 6c2e 2053 6574 7469   abnormal. Setti
+00014970: 6e67 2074 6f20 494e 4954 2073 7461 7475  ng to INIT statu
+00014980: 732e 2027 0a20 2020 2020 2020 2020 2020  s. '.           
+00014990: 2020 2020 2020 2020 2020 6627 6e6f 6465            f'node
+000149a0: 5f73 7461 7475 7365 733a 207b 6e6f 6465  _statuses: {node
+000149b0: 5f73 7461 7475 7365 737d 2729 0a20 2020  _statuses}').   
+000149c0: 2020 2020 2062 6163 6b65 6e64 203d 2067       backend = g
+000149d0: 6574 5f62 6163 6b65 6e64 5f66 726f 6d5f  et_backend_from_
+000149e0: 6861 6e64 6c65 2868 616e 646c 6529 0a20  handle(handle). 
+000149f0: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00014a00: 616e 6365 2862 6163 6b65 6e64 2c0a 2020  ance(backend,.  
+00014a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014a20: 2020 2020 6261 636b 656e 6473 2e43 6c6f      backends.Clo
+00014a30: 7564 566d 5261 7942 6163 6b65 6e64 2920  udVmRayBackend) 
+00014a40: 616e 6420 7265 636f 7264 5b27 6175 746f  and record['auto
+00014a50: 7374 6f70 275d 203e 3d20 303a 0a20 2020  stop'] >= 0:.   
+00014a60: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00014a70: 6261 636b 656e 642e 6973 5f64 6566 696e  backend.is_defin
+00014a80: 6974 656c 795f 6175 746f 7374 6f70 7069  itely_autostoppi
+00014a90: 6e67 2868 616e 646c 652c 0a20 2020 2020  ng(handle,.     
 00014aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ab0: 2020 2020 2020 2020 2073 7472 6561 6d5f           stream_
-00014ac0: 6c6f 6773 3d46 616c 7365 293a 0a20 2020  logs=False):.   
-00014ad0: 2020 2020 2020 2020 2020 2020 2023 2046               # F
-00014ae0: 7269 656e 646c 7920 6869 6e74 2e0a 2020  riendly hint..  
-00014af0: 2020 2020 2020 2020 2020 2020 2020 6175                au
-00014b00: 746f 7374 6f70 203d 2072 6563 6f72 645b  tostop = record[
-00014b10: 2761 7574 6f73 746f 7027 5d0a 2020 2020  'autostop'].    
-00014b20: 2020 2020 2020 2020 2020 2020 6d61 7962              mayb
-00014b30: 655f 646f 776e 5f73 7472 203d 2027 202d  e_down_str = ' -
-00014b40: 2d64 6f77 6e27 2069 6620 7265 636f 7264  -down' if record
-00014b50: 5b27 746f 5f64 6f77 6e27 5d20 656c 7365  ['to_down'] else
-00014b60: 2027 270a 2020 2020 2020 2020 2020 2020   ''.            
-00014b70: 2020 2020 6e6f 756e 203d 2027 6175 746f      noun = 'auto
-00014b80: 646f 776e 2720 6966 2072 6563 6f72 645b  down' if record[
-00014b90: 2774 6f5f 646f 776e 275d 2065 6c73 6520  'to_down'] else 
-00014ba0: 2761 7574 6f73 746f 7027 0a0a 2020 2020  'autostop'..    
-00014bb0: 2020 2020 2020 2020 2020 2020 2320 5265              # Re
-00014bc0: 7365 7420 7468 6520 6175 746f 7374 6f70  set the autostop
-00014bd0: 7069 6e67 2061 7320 7468 6520 636c 7573  ping as the clus
-00014be0: 7465 7220 6973 2061 626e 6f72 6d61 6c2c  ter is abnormal,
-00014bf0: 2061 6e64 206d 6179 0a20 2020 2020 2020   and may.       
-00014c00: 2020 2020 2020 2020 2023 206e 6f74 2063           # not c
-00014c10: 6f72 7265 6374 6c79 2061 7574 6f73 746f  orrectly autosto
-00014c20: 702e 2052 6573 6574 7469 6e67 2074 6865  p. Resetting the
-00014c30: 2061 7574 6f73 746f 7020 7769 6c6c 206c   autostop will l
-00014c40: 6574 0a20 2020 2020 2020 2020 2020 2020  et.             
-00014c50: 2020 2023 2074 6865 2075 7365 7220 6b6e     # the user kn
-00014c60: 6f77 2074 6861 7420 7468 6520 6175 746f  ow that the auto
-00014c70: 7374 6f70 206d 6179 206e 6f74 2068 6170  stop may not hap
-00014c80: 7065 6e20 746f 2061 766f 6964 0a20 2020  pen to avoid.   
-00014c90: 2020 2020 2020 2020 2020 2020 2023 206c               # l
-00014ca0: 6561 6b61 6765 7320 6672 6f6d 2074 6865  eakages from the
-00014cb0: 2061 7373 756d 7074 696f 6e20 7468 6174   assumption that
-00014cc0: 2074 6865 2063 6c75 7374 6572 2077 696c   the cluster wil
-00014cd0: 6c20 6175 746f 7374 6f70 2e0a 2020 2020  l autostop..    
-00014ce0: 2020 2020 2020 2020 2020 2020 7375 6363              succ
-00014cf0: 6573 7320 3d20 5472 7565 0a20 2020 2020  ess = True.     
-00014d00: 2020 2020 2020 2020 2020 2072 6573 6574             reset
-00014d10: 5f6c 6f63 616c 5f61 7574 6f73 746f 7020  _local_autostop 
-00014d20: 3d20 5472 7565 0a20 2020 2020 2020 2020  = True.         
-00014d30: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-00014d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d50: 6261 636b 656e 642e 7365 745f 6175 746f  backend.set_auto
-00014d60: 7374 6f70 2868 616e 646c 652c 202d 312c  stop(handle, -1,
-00014d70: 2073 7472 6561 6d5f 6c6f 6773 3d46 616c   stream_logs=Fal
-00014d80: 7365 290a 2020 2020 2020 2020 2020 2020  se).            
-00014d90: 2020 2020 6578 6365 7074 2065 7863 6570      except excep
-00014da0: 7469 6f6e 732e 436f 6d6d 616e 6445 7272  tions.CommandErr
-00014db0: 6f72 2061 7320 653a 0a20 2020 2020 2020  or as e:.       
-00014dc0: 2020 2020 2020 2020 2020 2020 2073 7563               suc
-00014dd0: 6365 7373 203d 2046 616c 7365 0a20 2020  cess = False.   
-00014de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014df0: 2069 6620 652e 7265 7475 726e 636f 6465   if e.returncode
-00014e00: 203d 3d20 3235 353a 0a20 2020 2020 2020   == 255:.       
-00014e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014e20: 206c 6f67 6765 722e 6465 6275 6728 6627   logger.debug(f'
-00014e30: 5468 6520 636c 7573 7465 7220 6973 206c  The cluster is l
-00014e40: 696b 656c 7920 7b6e 6f75 6e7d 6564 2e27  ikely {noun}ed.'
-00014e50: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00014e60: 2020 2020 2020 2020 2020 7265 7365 745f            reset_
-00014e70: 6c6f 6361 6c5f 6175 746f 7374 6f70 203d  local_autostop =
-00014e80: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
-00014e90: 2020 2020 2020 2065 7863 6570 7420 2845         except (E
-00014ea0: 7863 6570 7469 6f6e 2c20 5379 7374 656d  xception, System
-00014eb0: 4578 6974 2920 6173 2065 3a20 2023 2070  Exit) as e:  # p
-00014ec0: 796c 696e 743a 2064 6973 6162 6c65 3d62  ylint: disable=b
-00014ed0: 726f 6164 2d65 7863 6570 740a 2020 2020  road-except.    
-00014ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ef0: 7375 6363 6573 7320 3d20 4661 6c73 650a  success = False.
-00014f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f10: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-00014f20: 2866 2746 6169 6c65 6420 746f 2072 6573  (f'Failed to res
-00014f30: 6574 2061 7574 6f73 746f 702e 2044 7565  et autostop. Due
-00014f40: 2074 6f20 270a 2020 2020 2020 2020 2020   to '.          
-00014f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f60: 2020 2020 2020 2066 277b 636f 6d6d 6f6e         f'{common
-00014f70: 5f75 7469 6c73 2e66 6f72 6d61 745f 6578  _utils.format_ex
-00014f80: 6365 7074 696f 6e28 6529 7d27 290a 2020  ception(e)}').  
-00014f90: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00014fa0: 2072 6573 6574 5f6c 6f63 616c 5f61 7574   reset_local_aut
-00014fb0: 6f73 746f 703a 0a20 2020 2020 2020 2020  ostop:.         
-00014fc0: 2020 2020 2020 2020 2020 2067 6c6f 6261             globa
-00014fd0: 6c5f 7573 6572 5f73 7461 7465 2e73 6574  l_user_state.set
-00014fe0: 5f63 6c75 7374 6572 5f61 7574 6f73 746f  _cluster_autosto
-00014ff0: 705f 7661 6c75 6528 0a20 2020 2020 2020  p_value(.       
-00015000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015010: 2068 616e 646c 652e 636c 7573 7465 725f   handle.cluster_
-00015020: 6e61 6d65 2c20 2d31 2c20 746f 5f64 6f77  name, -1, to_dow
-00015030: 6e3d 4661 6c73 6529 0a0a 2020 2020 2020  n=False)..      
-00015040: 2020 2020 2020 2020 2020 6966 2073 7563            if suc
-00015050: 6365 7373 3a0a 2020 2020 2020 2020 2020  cess:.          
-00015060: 2020 2020 2020 2020 2020 6f70 6572 6174            operat
-00015070: 696f 6e5f 7374 7220 3d20 2866 2743 616e  ion_str = (f'Can
-00015080: 6365 6c65 6420 7b6e 6f75 6e7d 206f 6e20  celed {noun} on 
-00015090: 7468 6520 636c 7573 7465 7220 270a 2020  the cluster '.  
-000150a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000150b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000150c0: 2020 2066 277b 636c 7573 7465 725f 6e61     f'{cluster_na
-000150d0: 6d65 2172 7d27 290a 2020 2020 2020 2020  me!r}').        
-000150e0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00014ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ad0: 2073 7472 6561 6d5f 6c6f 6773 3d46 616c   stream_logs=Fal
+00014ae0: 7365 293a 0a20 2020 2020 2020 2020 2020  se):.           
+00014af0: 2020 2020 2023 2046 7269 656e 646c 7920       # Friendly 
+00014b00: 6869 6e74 2e0a 2020 2020 2020 2020 2020  hint..          
+00014b10: 2020 2020 2020 6175 746f 7374 6f70 203d        autostop =
+00014b20: 2072 6563 6f72 645b 2761 7574 6f73 746f   record['autosto
+00014b30: 7027 5d0a 2020 2020 2020 2020 2020 2020  p'].            
+00014b40: 2020 2020 6d61 7962 655f 646f 776e 5f73      maybe_down_s
+00014b50: 7472 203d 2027 202d 2d64 6f77 6e27 2069  tr = ' --down' i
+00014b60: 6620 7265 636f 7264 5b27 746f 5f64 6f77  f record['to_dow
+00014b70: 6e27 5d20 656c 7365 2027 270a 2020 2020  n'] else ''.    
+00014b80: 2020 2020 2020 2020 2020 2020 6e6f 756e              noun
+00014b90: 203d 2027 6175 746f 646f 776e 2720 6966   = 'autodown' if
+00014ba0: 2072 6563 6f72 645b 2774 6f5f 646f 776e   record['to_down
+00014bb0: 275d 2065 6c73 6520 2761 7574 6f73 746f  '] else 'autosto
+00014bc0: 7027 0a0a 2020 2020 2020 2020 2020 2020  p'..            
+00014bd0: 2020 2020 2320 5265 7365 7420 7468 6520      # Reset the 
+00014be0: 6175 746f 7374 6f70 7069 6e67 2061 7320  autostopping as 
+00014bf0: 7468 6520 636c 7573 7465 7220 6973 2061  the cluster is a
+00014c00: 626e 6f72 6d61 6c2c 2061 6e64 206d 6179  bnormal, and may
+00014c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014c20: 2023 206e 6f74 2063 6f72 7265 6374 6c79   # not correctly
+00014c30: 2061 7574 6f73 746f 702e 2052 6573 6574   autostop. Reset
+00014c40: 7469 6e67 2074 6865 2061 7574 6f73 746f  ting the autosto
+00014c50: 7020 7769 6c6c 206c 6574 0a20 2020 2020  p will let.     
+00014c60: 2020 2020 2020 2020 2020 2023 2074 6865             # the
+00014c70: 2075 7365 7220 6b6e 6f77 2074 6861 7420   user know that 
+00014c80: 7468 6520 6175 746f 7374 6f70 206d 6179  the autostop may
+00014c90: 206e 6f74 2068 6170 7065 6e20 746f 2061   not happen to a
+00014ca0: 766f 6964 0a20 2020 2020 2020 2020 2020  void.           
+00014cb0: 2020 2020 2023 206c 6561 6b61 6765 7320       # leakages 
+00014cc0: 6672 6f6d 2074 6865 2061 7373 756d 7074  from the assumpt
+00014cd0: 696f 6e20 7468 6174 2074 6865 2063 6c75  ion that the clu
+00014ce0: 7374 6572 2077 696c 6c20 6175 746f 7374  ster will autost
+00014cf0: 6f70 2e0a 2020 2020 2020 2020 2020 2020  op..            
+00014d00: 2020 2020 7375 6363 6573 7320 3d20 5472      success = Tr
+00014d10: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
+00014d20: 2020 2072 6573 6574 5f6c 6f63 616c 5f61     reset_local_a
+00014d30: 7574 6f73 746f 7020 3d20 5472 7565 0a20  utostop = True. 
+00014d40: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00014d50: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00014d60: 2020 2020 2020 2020 6261 636b 656e 642e          backend.
+00014d70: 7365 745f 6175 746f 7374 6f70 2868 616e  set_autostop(han
+00014d80: 646c 652c 202d 312c 2073 7472 6561 6d5f  dle, -1, stream_
+00014d90: 6c6f 6773 3d46 616c 7365 290a 2020 2020  logs=False).    
+00014da0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00014db0: 7074 2065 7863 6570 7469 6f6e 732e 436f  pt exceptions.Co
+00014dc0: 6d6d 616e 6445 7272 6f72 2061 7320 653a  mmandError as e:
+00014dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014de0: 2020 2020 2073 7563 6365 7373 203d 2046       success = F
+00014df0: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
+00014e00: 2020 2020 2020 2020 2069 6620 652e 7265           if e.re
+00014e10: 7475 726e 636f 6465 203d 3d20 3235 353a  turncode == 255:
+00014e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014e30: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+00014e40: 6465 6275 6728 6627 5468 6520 636c 7573  debug(f'The clus
+00014e50: 7465 7220 6973 206c 696b 656c 7920 7b6e  ter is likely {n
+00014e60: 6f75 6e7d 6564 2e27 290a 2020 2020 2020  oun}ed.').      
+00014e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e80: 2020 7265 7365 745f 6c6f 6361 6c5f 6175    reset_local_au
+00014e90: 746f 7374 6f70 203d 2046 616c 7365 0a20  tostop = False. 
+00014ea0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00014eb0: 7863 6570 7420 2845 7863 6570 7469 6f6e  xcept (Exception
+00014ec0: 2c20 5379 7374 656d 4578 6974 2920 6173  , SystemExit) as
+00014ed0: 2065 3a20 2023 2070 796c 696e 743a 2064   e:  # pylint: d
+00014ee0: 6973 6162 6c65 3d62 726f 6164 2d65 7863  isable=broad-exc
+00014ef0: 6570 740a 2020 2020 2020 2020 2020 2020  ept.            
+00014f00: 2020 2020 2020 2020 7375 6363 6573 7320          success 
+00014f10: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
+00014f20: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+00014f30: 6572 2e64 6562 7567 2866 2746 6169 6c65  er.debug(f'Faile
+00014f40: 6420 746f 2072 6573 6574 2061 7574 6f73  d to reset autos
+00014f50: 746f 702e 2044 7565 2074 6f20 270a 2020  top. Due to '.  
+00014f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f70: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00014f80: 277b 636f 6d6d 6f6e 5f75 7469 6c73 2e66  '{common_utils.f
+00014f90: 6f72 6d61 745f 6578 6365 7074 696f 6e28  ormat_exception(
+00014fa0: 6529 7d27 290a 2020 2020 2020 2020 2020  e)}').          
+00014fb0: 2020 2020 2020 6966 2072 6573 6574 5f6c        if reset_l
+00014fc0: 6f63 616c 5f61 7574 6f73 746f 703a 0a20  ocal_autostop:. 
+00014fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014fe0: 2020 2067 6c6f 6261 6c5f 7573 6572 5f73     global_user_s
+00014ff0: 7461 7465 2e73 6574 5f63 6c75 7374 6572  tate.set_cluster
+00015000: 5f61 7574 6f73 746f 705f 7661 6c75 6528  _autostop_value(
+00015010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015020: 2020 2020 2020 2020 2068 616e 646c 652e           handle.
+00015030: 636c 7573 7465 725f 6e61 6d65 2c20 2d31  cluster_name, -1
+00015040: 2c20 746f 5f64 6f77 6e3d 4661 6c73 6529  , to_down=False)
+00015050: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015060: 2020 6966 2073 7563 6365 7373 3a0a 2020    if success:.  
+00015070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015080: 2020 6f70 6572 6174 696f 6e5f 7374 7220    operation_str 
+00015090: 3d20 2866 2743 616e 6365 6c65 6420 7b6e  = (f'Canceled {n
+000150a0: 6f75 6e7d 206f 6e20 7468 6520 636c 7573  oun} on the clus
+000150b0: 7465 7220 270a 2020 2020 2020 2020 2020  ter '.          
+000150c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000150d0: 2020 2020 2020 2020 2020 2066 277b 636c             f'{cl
+000150e0: 7573 7465 725f 6e61 6d65 2172 7d27 290a  uster_name!r}').
 000150f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015100: 2020 6f70 6572 6174 696f 6e5f 7374 7220    operation_str 
-00015110: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-00015120: 2020 2020 2020 2020 2020 2020 6627 4174              f'At
-00015130: 7465 6d70 7465 6420 746f 2063 616e 6365  tempted to cance
-00015140: 6c20 7b6e 6f75 6e7d 206f 6e20 7468 6520  l {noun} on the 
-00015150: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-00015160: 2020 2020 2020 2020 2020 6627 636c 7573            f'clus
-00015170: 7465 7220 7b63 6c75 7374 6572 5f6e 616d  ter {cluster_nam
-00015180: 6521 727d 2077 6974 6820 6265 7374 2065  e!r} with best e
-00015190: 6666 6f72 7427 290a 2020 2020 2020 2020  ffort').        
-000151a0: 2020 2020 2020 2020 7965 6c6c 6f77 203d          yellow =
-000151b0: 2063 6f6c 6f72 616d 612e 466f 7265 2e59   colorama.Fore.Y
-000151c0: 454c 4c4f 570a 2020 2020 2020 2020 2020  ELLOW.          
-000151d0: 2020 2020 2020 6272 6967 6874 203d 2063        bright = c
-000151e0: 6f6c 6f72 616d 612e 5374 796c 652e 4252  olorama.Style.BR
-000151f0: 4947 4854 0a20 2020 2020 2020 2020 2020  IGHT.           
-00015200: 2020 2020 2072 6573 6574 203d 2063 6f6c       reset = col
-00015210: 6f72 616d 612e 5374 796c 652e 5245 5345  orama.Style.RESE
-00015220: 545f 414c 4c0a 2020 2020 2020 2020 2020  T_ALL.          
-00015230: 2020 2020 2020 7578 5f75 7469 6c73 2e63        ux_utils.c
-00015240: 6f6e 736f 6c65 5f6e 6577 6c69 6e65 2829  onsole_newline()
-00015250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015260: 206c 6f67 6765 722e 7761 726e 696e 6728   logger.warning(
-00015270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015280: 2020 2020 2066 277b 7965 6c6c 6f77 7d7b       f'{yellow}{
-00015290: 6f70 6572 6174 696f 6e5f 7374 727d 2c20  operation_str}, 
-000152a0: 7369 6e63 6520 6974 2069 7320 666f 756e  since it is foun
-000152b0: 6420 746f 2062 6520 696e 2061 6e20 270a  d to be in an '.
-000152c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000152d0: 2020 2020 6627 6162 6e6f 726d 616c 2073      f'abnormal s
-000152e0: 7461 7465 2e20 546f 2066 6978 2c20 7472  tate. To fix, tr
-000152f0: 7920 7275 6e6e 696e 673a 207b 7265 7365  y running: {rese
-00015300: 747d 7b62 7269 6768 747d 736b 7920 270a  t}{bright}sky '.
-00015310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015320: 2020 2020 6627 7374 6172 7420 2d66 202d      f'start -f -
-00015330: 6920 7b61 7574 6f73 746f 707d 7b6d 6179  i {autostop}{may
-00015340: 6265 5f64 6f77 6e5f 7374 727d 207b 636c  be_down_str} {cl
-00015350: 7573 7465 725f 6e61 6d65 7d27 0a20 2020  uster_name}'.   
-00015360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015370: 2066 277b 7265 7365 747d 2729 0a20 2020   f'{reset}').   
-00015380: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00015390: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-000153a0: 785f 7574 696c 732e 636f 6e73 6f6c 655f  x_utils.console_
-000153b0: 6e65 776c 696e 6528 290a 2020 2020 2020  newline().      
-000153c0: 2020 2020 2020 2020 2020 6f70 6572 6174            operat
-000153d0: 696f 6e5f 7374 7220 3d20 2761 7574 6f64  ion_str = 'autod
-000153e0: 6f77 6e69 6e67 2720 6966 2072 6563 6f72  owning' if recor
-000153f0: 645b 0a20 2020 2020 2020 2020 2020 2020  d[.             
-00015400: 2020 2020 2020 2027 746f 5f64 6f77 6e27         'to_down'
-00015410: 5d20 656c 7365 2027 6175 746f 7374 6f70  ] else 'autostop
-00015420: 7069 6e67 270a 2020 2020 2020 2020 2020  ping'.          
-00015430: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
-00015440: 6f28 0a20 2020 2020 2020 2020 2020 2020  o(.             
-00015450: 2020 2020 2020 2066 2743 6c75 7374 6572         f'Cluster
-00015460: 207b 636c 7573 7465 725f 6e61 6d65 2172   {cluster_name!r
-00015470: 7d20 6973 207b 6f70 6572 6174 696f 6e5f  } is {operation_
-00015480: 7374 727d 2e20 5365 7474 696e 6720 746f  str}. Setting to
-00015490: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
-000154a0: 2020 2020 2020 2027 494e 4954 2073 7461         'INIT sta
-000154b0: 7475 733b 2074 7279 2072 6566 7265 7368  tus; try refresh
-000154c0: 2061 6761 696e 2069 6e20 6120 7768 696c   again in a whil
-000154d0: 652e 2729 0a0a 2020 2020 2020 2020 2320  e.')..        # 
-000154e0: 4966 2074 6865 2075 7365 7220 7374 6172  If the user star
-000154f0: 7473 2070 6172 7420 6f66 2061 2053 544f  ts part of a STO
-00015500: 5050 4544 2063 6c75 7374 6572 2c20 7765  PPED cluster, we
-00015510: 2073 7469 6c6c 206e 6565 6420 6120 7374   still need a st
-00015520: 6174 7573 0a20 2020 2020 2020 2023 2074  atus.        # t
-00015530: 6f20 7265 7072 6573 656e 7420 7468 6520  o represent the 
-00015540: 6162 6e6f 726d 616c 2073 7461 7475 732e  abnormal status.
-00015550: 2046 6f72 2073 706f 7420 636c 7573 7465   For spot cluste
-00015560: 722c 2069 7420 6361 6e20 616c 736f 0a20  r, it can also. 
-00015570: 2020 2020 2020 2023 2072 6570 7265 7365         # represe
-00015580: 6e74 2074 6861 7420 7468 6520 636c 7573  nt that the clus
-00015590: 7465 7220 6973 2070 6172 7469 616c 6c79  ter is partially
-000155a0: 2070 7265 656d 7074 6564 2e0a 2020 2020   preempted..    
-000155b0: 2020 2020 2320 544f 444f 287a 6877 7529      # TODO(zhwu)
-000155c0: 3a20 7468 6520 6465 6669 6e69 7469 6f6e  : the definition
-000155d0: 206f 6620 494e 4954 2073 686f 756c 6420   of INIT should 
-000155e0: 6265 2061 7564 6974 6564 2f63 6861 6e67  be audited/chang
-000155f0: 6564 2e0a 2020 2020 2020 2020 2320 4164  ed..        # Ad
-00015600: 6469 6e67 2061 206e 6577 2073 7461 7475  ding a new statu
-00015610: 7320 554e 4845 414c 5448 5920 666f 7220  s UNHEALTHY for 
-00015620: 6162 6e6f 726d 616c 2073 7461 7475 7320  abnormal status 
-00015630: 6361 6e20 6265 2061 2063 686f 6963 652e  can be a choice.
-00015640: 0a20 2020 2020 2020 2067 6c6f 6261 6c5f  .        global_
-00015650: 7573 6572 5f73 7461 7465 2e61 6464 5f6f  user_state.add_o
-00015660: 725f 7570 6461 7465 5f63 6c75 7374 6572  r_update_cluster
-00015670: 2863 6c75 7374 6572 5f6e 616d 652c 0a20  (cluster_name,. 
-00015680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000156a0: 2020 2020 2020 2020 2020 2020 2020 2068                 h
-000156b0: 616e 646c 652c 0a20 2020 2020 2020 2020  andle,.         
-000156c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015100: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00015110: 2020 2020 2020 2020 2020 6f70 6572 6174            operat
+00015120: 696f 6e5f 7374 7220 3d20 280a 2020 2020  ion_str = (.    
+00015130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015140: 2020 2020 6627 4174 7465 6d70 7465 6420      f'Attempted 
+00015150: 746f 2063 616e 6365 6c20 7b6e 6f75 6e7d  to cancel {noun}
+00015160: 206f 6e20 7468 6520 270a 2020 2020 2020   on the '.      
+00015170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015180: 2020 6627 636c 7573 7465 7220 7b63 6c75    f'cluster {clu
+00015190: 7374 6572 5f6e 616d 6521 727d 2077 6974  ster_name!r} wit
+000151a0: 6820 6265 7374 2065 6666 6f72 7427 290a  h best effort').
+000151b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000151c0: 7965 6c6c 6f77 203d 2063 6f6c 6f72 616d  yellow = coloram
+000151d0: 612e 466f 7265 2e59 454c 4c4f 570a 2020  a.Fore.YELLOW.  
+000151e0: 2020 2020 2020 2020 2020 2020 2020 6272                br
+000151f0: 6967 6874 203d 2063 6f6c 6f72 616d 612e  ight = colorama.
+00015200: 5374 796c 652e 4252 4947 4854 0a20 2020  Style.BRIGHT.   
+00015210: 2020 2020 2020 2020 2020 2020 2072 6573               res
+00015220: 6574 203d 2063 6f6c 6f72 616d 612e 5374  et = colorama.St
+00015230: 796c 652e 5245 5345 545f 414c 4c0a 2020  yle.RESET_ALL.  
+00015240: 2020 2020 2020 2020 2020 2020 2020 7578                ux
+00015250: 5f75 7469 6c73 2e63 6f6e 736f 6c65 5f6e  _utils.console_n
+00015260: 6577 6c69 6e65 2829 0a20 2020 2020 2020  ewline().       
+00015270: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+00015280: 7761 726e 696e 6728 0a20 2020 2020 2020  warning(.       
+00015290: 2020 2020 2020 2020 2020 2020 2066 277b               f'{
+000152a0: 7965 6c6c 6f77 7d7b 6f70 6572 6174 696f  yellow}{operatio
+000152b0: 6e5f 7374 727d 2c20 7369 6e63 6520 6974  n_str}, since it
+000152c0: 2069 7320 666f 756e 6420 746f 2062 6520   is found to be 
+000152d0: 696e 2061 6e20 270a 2020 2020 2020 2020  in an '.        
+000152e0: 2020 2020 2020 2020 2020 2020 6627 6162              f'ab
+000152f0: 6e6f 726d 616c 2073 7461 7465 2e20 546f  normal state. To
+00015300: 2066 6978 2c20 7472 7920 7275 6e6e 696e   fix, try runnin
+00015310: 673a 207b 7265 7365 747d 7b62 7269 6768  g: {reset}{brigh
+00015320: 747d 736b 7920 270a 2020 2020 2020 2020  t}sky '.        
+00015330: 2020 2020 2020 2020 2020 2020 6627 7374              f'st
+00015340: 6172 7420 2d66 202d 6920 7b61 7574 6f73  art -f -i {autos
+00015350: 746f 707d 7b6d 6179 6265 5f64 6f77 6e5f  top}{maybe_down_
+00015360: 7374 727d 207b 636c 7573 7465 725f 6e61  str} {cluster_na
+00015370: 6d65 7d27 0a20 2020 2020 2020 2020 2020  me}'.           
+00015380: 2020 2020 2020 2020 2066 277b 7265 7365           f'{rese
+00015390: 747d 2729 0a20 2020 2020 2020 2020 2020  t}').           
+000153a0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000153b0: 2020 2020 2020 2075 785f 7574 696c 732e         ux_utils.
+000153c0: 636f 6e73 6f6c 655f 6e65 776c 696e 6528  console_newline(
+000153d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000153e0: 2020 6f70 6572 6174 696f 6e5f 7374 7220    operation_str 
+000153f0: 3d20 2761 7574 6f64 6f77 6e69 6e67 2720  = 'autodowning' 
+00015400: 6966 2072 6563 6f72 645b 0a20 2020 2020  if record[.     
+00015410: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00015420: 746f 5f64 6f77 6e27 5d20 656c 7365 2027  to_down'] else '
+00015430: 6175 746f 7374 6f70 7069 6e67 270a 2020  autostopping'.  
+00015440: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00015450: 6767 6572 2e69 6e66 6f28 0a20 2020 2020  gger.info(.     
+00015460: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00015470: 2743 6c75 7374 6572 207b 636c 7573 7465  'Cluster {cluste
+00015480: 725f 6e61 6d65 2172 7d20 6973 207b 6f70  r_name!r} is {op
+00015490: 6572 6174 696f 6e5f 7374 727d 2e20 5365  eration_str}. Se
+000154a0: 7474 696e 6720 746f 2027 0a20 2020 2020  tting to '.     
+000154b0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+000154c0: 494e 4954 2073 7461 7475 733b 2074 7279  INIT status; try
+000154d0: 2072 6566 7265 7368 2061 6761 696e 2069   refresh again i
+000154e0: 6e20 6120 7768 696c 652e 2729 0a0a 2020  n a while.')..  
+000154f0: 2020 2020 2020 2320 4966 2074 6865 2075        # If the u
+00015500: 7365 7220 7374 6172 7473 2070 6172 7420  ser starts part 
+00015510: 6f66 2061 2053 544f 5050 4544 2063 6c75  of a STOPPED clu
+00015520: 7374 6572 2c20 7765 2073 7469 6c6c 206e  ster, we still n
+00015530: 6565 6420 6120 7374 6174 7573 0a20 2020  eed a status.   
+00015540: 2020 2020 2023 2074 6f20 7265 7072 6573       # to repres
+00015550: 656e 7420 7468 6520 6162 6e6f 726d 616c  ent the abnormal
+00015560: 2073 7461 7475 732e 2046 6f72 2073 706f   status. For spo
+00015570: 7420 636c 7573 7465 722c 2069 7420 6361  t cluster, it ca
+00015580: 6e20 616c 736f 0a20 2020 2020 2020 2023  n also.        #
+00015590: 2072 6570 7265 7365 6e74 2074 6861 7420   represent that 
+000155a0: 7468 6520 636c 7573 7465 7220 6973 2070  the cluster is p
+000155b0: 6172 7469 616c 6c79 2070 7265 656d 7074  artially preempt
+000155c0: 6564 2e0a 2020 2020 2020 2020 2320 544f  ed..        # TO
+000155d0: 444f 287a 6877 7529 3a20 7468 6520 6465  DO(zhwu): the de
+000155e0: 6669 6e69 7469 6f6e 206f 6620 494e 4954  finition of INIT
+000155f0: 2073 686f 756c 6420 6265 2061 7564 6974   should be audit
+00015600: 6564 2f63 6861 6e67 6564 2e0a 2020 2020  ed/changed..    
+00015610: 2020 2020 2320 4164 6469 6e67 2061 206e      # Adding a n
+00015620: 6577 2073 7461 7475 7320 554e 4845 414c  ew status UNHEAL
+00015630: 5448 5920 666f 7220 6162 6e6f 726d 616c  THY for abnormal
+00015640: 2073 7461 7475 7320 6361 6e20 6265 2061   status can be a
+00015650: 2063 686f 6963 652e 0a20 2020 2020 2020   choice..       
+00015660: 2067 6c6f 6261 6c5f 7573 6572 5f73 7461   global_user_sta
+00015670: 7465 2e61 6464 5f6f 725f 7570 6461 7465  te.add_or_update
+00015680: 5f63 6c75 7374 6572 2863 6c75 7374 6572  _cluster(cluster
+00015690: 5f6e 616d 652c 0a20 2020 2020 2020 2020  _name,.         
+000156a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000156b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000156c0: 2020 2020 2020 2068 616e 646c 652c 0a20         handle,. 
 000156d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000156e0: 2020 2020 2020 2072 6571 7565 7374 6564         requested
-000156f0: 5f72 6573 6f75 7263 6573 3d4e 6f6e 652c  _resources=None,
-00015700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000156e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000156f0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00015700: 6571 7565 7374 6564 5f72 6573 6f75 7263  equested_resourc
+00015710: 6573 3d4e 6f6e 652c 0a20 2020 2020 2020  es=None,.       
 00015720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015730: 2072 6561 6479 3d46 616c 7365 2c0a 2020   ready=False,.  
-00015740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015760: 2020 2020 2020 2020 2020 2020 2020 6973                is
-00015770: 5f6c 6175 6e63 683d 4661 6c73 6529 0a20  _launch=False). 
-00015780: 2020 2020 2020 2072 6574 7572 6e20 676c         return gl
-00015790: 6f62 616c 5f75 7365 725f 7374 6174 652e  obal_user_state.
-000157a0: 6765 745f 636c 7573 7465 725f 6672 6f6d  get_cluster_from
-000157b0: 5f6e 616d 6528 636c 7573 7465 725f 6e61  _name(cluster_na
-000157c0: 6d65 290a 2020 2020 2320 4e6f 7720 6973  me).    # Now is
-000157d0: 5f61 626e 6f72 6d61 6c20 6973 2046 616c  _abnormal is Fal
-000157e0: 7365 3a20 6569 7468 6572 206e 6f64 655f  se: either node_
-000157f0: 7374 6174 7573 6573 2069 7320 656d 7074  statuses is empt
-00015800: 7920 6f72 2061 6c6c 206e 6f64 6573 2061  y or all nodes a
-00015810: 7265 0a20 2020 2023 2053 544f 5050 4544  re.    # STOPPED
-00015820: 2e0a 2020 2020 6261 636b 656e 6420 3d20  ..    backend = 
-00015830: 6261 636b 656e 6473 2e43 6c6f 7564 566d  backends.CloudVm
-00015840: 5261 7942 6163 6b65 6e64 2829 0a20 2020  RayBackend().   
-00015850: 2062 6163 6b65 6e64 2e70 6f73 745f 7465   backend.post_te
-00015860: 6172 646f 776e 5f63 6c65 616e 7570 2868  ardown_cleanup(h
-00015870: 616e 646c 652c 2074 6572 6d69 6e61 7465  andle, terminate
-00015880: 3d74 6f5f 7465 726d 696e 6174 652c 2070  =to_terminate, p
-00015890: 7572 6765 3d46 616c 7365 290a 2020 2020  urge=False).    
-000158a0: 7265 7475 726e 2067 6c6f 6261 6c5f 7573  return global_us
-000158b0: 6572 5f73 7461 7465 2e67 6574 5f63 6c75  er_state.get_clu
-000158c0: 7374 6572 5f66 726f 6d5f 6e61 6d65 2863  ster_from_name(c
-000158d0: 6c75 7374 6572 5f6e 616d 6529 0a0a 0a64  luster_name)...d
-000158e0: 6566 205f 7570 6461 7465 5f63 6c75 7374  ef _update_clust
-000158f0: 6572 5f73 7461 7475 7328 0a20 2020 2063  er_status(.    c
-00015900: 6c75 7374 6572 5f6e 616d 653a 2073 7472  luster_name: str
-00015910: 2c0a 2020 2020 6163 7175 6972 655f 7065  ,.    acquire_pe
-00015920: 725f 636c 7573 7465 725f 7374 6174 7573  r_cluster_status
-00015930: 5f6c 6f63 6b3a 2062 6f6f 6c2c 0a20 2020  _lock: bool,.   
-00015940: 2063 6c75 7374 6572 5f73 7461 7475 735f   cluster_status_
-00015950: 6c6f 636b 5f74 696d 656f 7574 3a20 696e  lock_timeout: in
-00015960: 7420 3d20 434c 5553 5445 525f 5354 4154  t = CLUSTER_STAT
-00015970: 5553 5f4c 4f43 4b5f 5449 4d45 4f55 545f  US_LOCK_TIMEOUT_
-00015980: 5345 434f 4e44 530a 2920 2d3e 204f 7074  SECONDS.) -> Opt
-00015990: 696f 6e61 6c5b 4469 6374 5b73 7472 2c20  ional[Dict[str, 
-000159a0: 416e 795d 5d3a 0a20 2020 2022 2222 5570  Any]]:.    """Up
-000159b0: 6461 7465 2074 6865 2063 6c75 7374 6572  date the cluster
-000159c0: 2073 7461 7475 732e 0a0a 2020 2020 5468   status...    Th
-000159d0: 6520 636c 7573 7465 7220 7374 6174 7573  e cluster status
-000159e0: 2069 7320 7570 6461 7465 6420 6279 2063   is updated by c
-000159f0: 6865 636b 696e 6720 7261 7920 636c 7573  hecking ray clus
-00015a00: 7465 7220 616e 6420 7265 616c 2073 7461  ter and real sta
-00015a10: 7475 7320 6672 6f6d 0a20 2020 2063 6c6f  tus from.    clo
-00015a20: 7564 2e0a 0a20 2020 2054 6865 2066 756e  ud...    The fun
-00015a30: 6374 696f 6e20 7769 6c6c 2075 7064 6174  ction will updat
-00015a40: 6520 7468 6520 6361 6368 6564 2063 6c75  e the cached clu
-00015a50: 7374 6572 2073 7461 7475 7320 696e 2074  ster status in t
-00015a60: 6865 2067 6c6f 6261 6c20 7374 6174 652e  he global state.
-00015a70: 2046 6f72 0a20 2020 2074 6865 2064 6573   For.    the des
-00015a80: 6967 6e20 6f66 2074 6865 2063 6c75 7374  ign of the clust
-00015a90: 6572 2073 7461 7475 7320 616e 6420 7472  er status and tr
-00015aa0: 616e 7369 7469 6f6e 2c20 706c 6561 7365  ansition, please
-00015ab0: 2072 6566 6572 2074 6f20 7468 650a 2020   refer to the.  
-00015ac0: 2020 736b 792f 6465 7369 676e 5f64 6f63    sky/design_doc
-00015ad0: 732f 636c 7573 7465 725f 7374 6174 7573  s/cluster_status
-00015ae0: 2e6d 640a 0a20 2020 2041 7267 733a 0a20  .md..    Args:. 
-00015af0: 2020 2020 2020 2063 6c75 7374 6572 5f6e         cluster_n
-00015b00: 616d 653a 2054 6865 206e 616d 6520 6f66  ame: The name of
-00015b10: 2074 6865 2063 6c75 7374 6572 2e0a 2020   the cluster..  
-00015b20: 2020 2020 2020 6163 7175 6972 655f 7065        acquire_pe
-00015b30: 725f 636c 7573 7465 725f 7374 6174 7573  r_cluster_status
-00015b40: 5f6c 6f63 6b3a 2057 6865 7468 6572 2074  _lock: Whether t
-00015b50: 6f20 6163 7175 6972 6520 7468 6520 7065  o acquire the pe
-00015b60: 722d 636c 7573 7465 7220 6c6f 636b 0a20  r-cluster lock. 
-00015b70: 2020 2020 2020 2020 2062 6566 6f72 6520           before 
-00015b80: 7570 6461 7469 6e67 2074 6865 2073 7461  updating the sta
-00015b90: 7475 732e 0a20 2020 2020 2020 2063 6c75  tus..        clu
-00015ba0: 7374 6572 5f73 7461 7475 735f 6c6f 636b  ster_status_lock
-00015bb0: 5f74 696d 656f 7574 3a20 5468 6520 7469  _timeout: The ti
-00015bc0: 6d65 6f75 7420 746f 2061 6371 7569 7265  meout to acquire
-00015bd0: 2074 6865 2070 6572 2d63 6c75 7374 6572   the per-cluster
-00015be0: 0a20 2020 2020 2020 2020 206c 6f63 6b2e  .          lock.
-00015bf0: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
-00015c00: 2020 2020 2020 2049 6620 7468 6520 636c         If the cl
-00015c10: 7573 7465 7220 6973 2074 6572 6d69 6e61  uster is termina
-00015c20: 7465 6420 6f72 2064 6f65 7320 6e6f 7420  ted or does not 
-00015c30: 6578 6973 742c 2072 6574 7572 6e20 4e6f  exist, return No
-00015c40: 6e65 2e20 4f74 6865 7277 6973 650a 2020  ne. Otherwise.  
-00015c50: 2020 2020 2020 7265 7475 726e 7320 7468        returns th
-00015c60: 6520 696e 7075 7420 7265 636f 7264 2077  e input record w
-00015c70: 6974 6820 7374 6174 7573 2061 6e64 2068  ith status and h
-00015c80: 616e 646c 6520 706f 7465 6e74 6961 6c6c  andle potentiall
-00015c90: 7920 7570 6461 7465 642e 0a0a 2020 2020  y updated...    
-00015ca0: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
-00015cb0: 6578 6365 7074 696f 6e73 2e43 6c75 7374  exceptions.Clust
-00015cc0: 6572 4f77 6e65 7249 6465 6e74 6974 794d  erOwnerIdentityM
-00015cd0: 6973 6d61 7463 6845 7272 6f72 3a20 6966  ismatchError: if
-00015ce0: 2074 6865 2063 7572 7265 6e74 2075 7365   the current use
-00015cf0: 7220 6973 0a20 2020 2020 2020 2020 206e  r is.          n
-00015d00: 6f74 2074 6865 2073 616d 6520 6173 2074  ot the same as t
-00015d10: 6865 2075 7365 7220 7768 6f20 6372 6561  he user who crea
-00015d20: 7465 6420 7468 6520 636c 7573 7465 722e  ted the cluster.
-00015d30: 0a20 2020 2020 2020 2065 7863 6570 7469  .        excepti
-00015d40: 6f6e 732e 436c 6f75 6455 7365 7249 6465  ons.CloudUserIde
-00015d50: 6e74 6974 7945 7272 6f72 3a20 6966 2077  ntityError: if w
-00015d60: 6520 6661 696c 2074 6f20 6765 7420 7468  e fail to get th
-00015d70: 6520 6375 7272 656e 7420 7573 6572 0a20  e current user. 
-00015d80: 2020 2020 2020 2020 2069 6465 6e74 6974           identit
-00015d90: 792e 0a20 2020 2020 2020 2065 7863 6570  y..        excep
-00015da0: 7469 6f6e 732e 436c 7573 7465 7253 7461  tions.ClusterSta
-00015db0: 7475 7346 6574 6368 696e 6745 7272 6f72  tusFetchingError
-00015dc0: 3a20 7468 6520 636c 7573 7465 7220 7374  : the cluster st
-00015dd0: 6174 7573 2063 616e 6e6f 7420 6265 0a20  atus cannot be. 
-00015de0: 2020 2020 2020 2020 2066 6574 6368 6564           fetched
-00015df0: 2066 726f 6d20 7468 6520 636c 6f75 6420   from the cloud 
-00015e00: 7072 6f76 6964 6572 206f 7220 7468 6572  provider or ther
-00015e10: 6520 6172 6520 6c65 616b 6564 206e 6f64  e are leaked nod
-00015e20: 6573 2063 6175 7369 6e67 0a20 2020 2020  es causing.     
-00015e30: 2020 2020 2074 6865 206e 6f64 6520 6e75       the node nu
-00015e40: 6d62 6572 206c 6172 6765 7220 7468 616e  mber larger than
-00015e50: 2065 7870 6563 7465 642e 0a20 2020 2022   expected..    "
-00015e60: 2222 0a20 2020 2069 6620 6e6f 7420 6163  "".    if not ac
-00015e70: 7175 6972 655f 7065 725f 636c 7573 7465  quire_per_cluste
-00015e80: 725f 7374 6174 7573 5f6c 6f63 6b3a 0a20  r_status_lock:. 
-00015e90: 2020 2020 2020 2072 6574 7572 6e20 5f75         return _u
-00015ea0: 7064 6174 655f 636c 7573 7465 725f 7374  pdate_cluster_st
-00015eb0: 6174 7573 5f6e 6f5f 6c6f 636b 2863 6c75  atus_no_lock(clu
-00015ec0: 7374 6572 5f6e 616d 6529 0a0a 2020 2020  ster_name)..    
-00015ed0: 7472 793a 0a20 2020 2020 2020 2077 6974  try:.        wit
-00015ee0: 6820 6669 6c65 6c6f 636b 2e46 696c 654c  h filelock.FileL
-00015ef0: 6f63 6b28 434c 5553 5445 525f 5354 4154  ock(CLUSTER_STAT
-00015f00: 5553 5f4c 4f43 4b5f 5041 5448 2e66 6f72  US_LOCK_PATH.for
-00015f10: 6d61 7428 636c 7573 7465 725f 6e61 6d65  mat(cluster_name
-00015f20: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00015f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015f40: 2020 7469 6d65 6f75 743d 636c 7573 7465    timeout=cluste
-00015f50: 725f 7374 6174 7573 5f6c 6f63 6b5f 7469  r_status_lock_ti
-00015f60: 6d65 6f75 7429 3a0a 2020 2020 2020 2020  meout):.        
-00015f70: 2020 2020 7265 7475 726e 205f 7570 6461      return _upda
-00015f80: 7465 5f63 6c75 7374 6572 5f73 7461 7475  te_cluster_statu
-00015f90: 735f 6e6f 5f6c 6f63 6b28 636c 7573 7465  s_no_lock(cluste
-00015fa0: 725f 6e61 6d65 290a 2020 2020 6578 6365  r_name).    exce
-00015fb0: 7074 2066 696c 656c 6f63 6b2e 5469 6d65  pt filelock.Time
-00015fc0: 6f75 743a 0a20 2020 2020 2020 206c 6f67  out:.        log
-00015fd0: 6765 722e 6465 6275 6728 2752 6566 7265  ger.debug('Refre
-00015fe0: 7368 696e 6720 7374 6174 7573 3a20 4661  shing status: Fa
-00015ff0: 696c 6564 2067 6574 2074 6865 206c 6f63  iled get the loc
-00016000: 6b20 666f 7220 636c 7573 7465 7220 270a  k for cluster '.
-00016010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016020: 2020 2020 2066 277b 636c 7573 7465 725f       f'{cluster_
-00016030: 6e61 6d65 2172 7d2e 2055 7369 6e67 2074  name!r}. Using t
-00016040: 6865 2063 6163 6865 6420 7374 6174 7573  he cached status
-00016050: 2e27 290a 2020 2020 2020 2020 7265 636f  .').        reco
-00016060: 7264 203d 2067 6c6f 6261 6c5f 7573 6572  rd = global_user
-00016070: 5f73 7461 7465 2e67 6574 5f63 6c75 7374  _state.get_clust
-00016080: 6572 5f66 726f 6d5f 6e61 6d65 2863 6c75  er_from_name(clu
-00016090: 7374 6572 5f6e 616d 6529 0a20 2020 2020  ster_name).     
-000160a0: 2020 2072 6574 7572 6e20 7265 636f 7264     return record
-000160b0: 0a0a 0a64 6566 2072 6566 7265 7368 5f63  ...def refresh_c
-000160c0: 6c75 7374 6572 5f72 6563 6f72 6428 0a20  luster_record(. 
-000160d0: 2020 2063 6c75 7374 6572 5f6e 616d 653a     cluster_name:
-000160e0: 2073 7472 2c0a 2020 2020 2a2c 0a20 2020   str,.    *,.   
-000160f0: 2066 6f72 6365 5f72 6566 7265 7368 5f73   force_refresh_s
-00016100: 7461 7475 7365 733a 204f 7074 696f 6e61  tatuses: Optiona
-00016110: 6c5b 5365 745b 7374 6174 7573 5f6c 6962  l[Set[status_lib
-00016120: 2e43 6c75 7374 6572 5374 6174 7573 5d5d  .ClusterStatus]]
-00016130: 203d 204e 6f6e 652c 0a20 2020 2061 6371   = None,.    acq
-00016140: 7569 7265 5f70 6572 5f63 6c75 7374 6572  uire_per_cluster
-00016150: 5f73 7461 7475 735f 6c6f 636b 3a20 626f  _status_lock: bo
-00016160: 6f6c 203d 2054 7275 652c 0a20 2020 2063  ol = True,.    c
-00016170: 6c75 7374 6572 5f73 7461 7475 735f 6c6f  luster_status_lo
-00016180: 636b 5f74 696d 656f 7574 3a20 696e 7420  ck_timeout: int 
-00016190: 3d20 434c 5553 5445 525f 5354 4154 5553  = CLUSTER_STATUS
-000161a0: 5f4c 4f43 4b5f 5449 4d45 4f55 545f 5345  _LOCK_TIMEOUT_SE
-000161b0: 434f 4e44 530a 2920 2d3e 204f 7074 696f  CONDS.) -> Optio
-000161c0: 6e61 6c5b 4469 6374 5b73 7472 2c20 416e  nal[Dict[str, An
-000161d0: 795d 5d3a 0a20 2020 2022 2222 5265 6672  y]]:.    """Refr
-000161e0: 6573 6820 7468 6520 636c 7573 7465 722c  esh the cluster,
-000161f0: 2061 6e64 2072 6574 7572 6e20 7468 6520   and return the 
-00016200: 706f 7373 6962 6c79 2075 7064 6174 6564  possibly updated
-00016210: 2072 6563 6f72 642e 0a0a 2020 2020 5468   record...    Th
-00016220: 6973 2066 756e 6374 696f 6e20 7769 6c6c  is function will
-00016230: 2061 6c73 6f20 6368 6563 6b20 7468 6520   also check the 
-00016240: 6f77 6e65 7220 6964 656e 7469 7479 206f  owner identity o
-00016250: 6620 7468 6520 636c 7573 7465 722c 2061  f the cluster, a
-00016260: 6e64 2072 6169 7365 0a20 2020 2065 7863  nd raise.    exc
-00016270: 6570 7469 6f6e 7320 6966 2074 6865 2063  eptions if the c
-00016280: 7572 7265 6e74 2075 7365 7220 6973 206e  urrent user is n
-00016290: 6f74 2074 6865 2073 616d 6520 6173 2074  ot the same as t
-000162a0: 6865 2075 7365 7220 7768 6f20 6372 6561  he user who crea
-000162b0: 7465 6420 7468 650a 2020 2020 636c 7573  ted the.    clus
-000162c0: 7465 722e 0a0a 2020 2020 4172 6773 3a0a  ter...    Args:.
-000162d0: 2020 2020 2020 2020 636c 7573 7465 725f          cluster_
-000162e0: 6e61 6d65 3a20 5468 6520 6e61 6d65 206f  name: The name o
-000162f0: 6620 7468 6520 636c 7573 7465 722e 0a20  f the cluster.. 
-00016300: 2020 2020 2020 2066 6f72 6365 5f72 6566         force_ref
-00016310: 7265 7368 5f73 7461 7475 7365 733a 2069  resh_statuses: i
-00016320: 6620 7370 6563 6966 6965 642c 2072 6566  f specified, ref
-00016330: 7265 7368 2074 6865 2063 6c75 7374 6572  resh the cluster
-00016340: 2069 6620 6974 2068 6173 206f 6e65 206f   if it has one o
-00016350: 660a 2020 2020 2020 2020 2020 7468 6520  f.          the 
-00016360: 7370 6563 6966 6965 6420 7374 6174 7573  specified status
-00016370: 6573 2e20 4164 6469 7469 6f6e 616c 6c79  es. Additionally
-00016380: 2c20 636c 7573 7465 7273 2073 6174 6973  , clusters satis
-00016390: 6679 696e 6720 7468 650a 2020 2020 2020  fying the.      
-000163a0: 2020 2020 666f 6c6c 6f77 696e 6720 636f      following co
-000163b0: 6e64 6974 696f 6e73 2077 696c 6c20 616c  nditions will al
-000163c0: 7761 7973 2062 6520 7265 6672 6573 6865  ways be refreshe
-000163d0: 6420 6e6f 206d 6174 7465 7220 7468 650a  d no matter the.
-000163e0: 2020 2020 2020 2020 2020 6172 6775 6d65            argume
-000163f0: 6e74 2069 7320 7370 6563 6966 6965 6420  nt is specified 
-00016400: 6f72 206e 6f74 3a0a 2020 2020 2020 2020  or not:.        
-00016410: 2020 2020 312e 2069 7320 6120 7370 6f74      1. is a spot
-00016420: 2063 6c75 7374 6572 2c20 6f72 0a20 2020   cluster, or.   
-00016430: 2020 2020 2020 2020 2032 2e20 6973 2061           2. is a
-00016440: 206e 6f6e 2d73 706f 7420 636c 7573 7465   non-spot cluste
-00016450: 722c 2069 7320 6e6f 7420 5354 4f50 5045  r, is not STOPPE
-00016460: 442c 2061 6e64 2061 7574 6f73 746f 7020  D, and autostop 
-00016470: 6973 2073 6574 2e0a 2020 2020 2020 2020  is set..        
-00016480: 6163 7175 6972 655f 7065 725f 636c 7573  acquire_per_clus
-00016490: 7465 725f 7374 6174 7573 5f6c 6f63 6b3a  ter_status_lock:
-000164a0: 2057 6865 7468 6572 2074 6f20 6163 7175   Whether to acqu
-000164b0: 6972 6520 7468 6520 7065 722d 636c 7573  ire the per-clus
-000164c0: 7465 7220 6c6f 636b 0a20 2020 2020 2020  ter lock.       
-000164d0: 2020 2062 6566 6f72 6520 7570 6461 7469     before updati
-000164e0: 6e67 2074 6865 2073 7461 7475 732e 0a20  ng the status.. 
-000164f0: 2020 2020 2020 2063 6c75 7374 6572 5f73         cluster_s
-00016500: 7461 7475 735f 6c6f 636b 5f74 696d 656f  tatus_lock_timeo
-00016510: 7574 3a20 5468 6520 7469 6d65 6f75 7420  ut: The timeout 
-00016520: 746f 2061 6371 7569 7265 2074 6865 2070  to acquire the p
-00016530: 6572 2d63 6c75 7374 6572 0a20 2020 2020  er-cluster.     
-00016540: 2020 2020 206c 6f63 6b2e 2049 6620 7469       lock. If ti
-00016550: 6d65 6f75 742c 2074 6865 2066 756e 6374  meout, the funct
-00016560: 696f 6e20 7769 6c6c 2075 7365 2074 6865  ion will use the
-00016570: 2063 6163 6865 6420 7374 6174 7573 2e0a   cached status..
-00016580: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
-00016590: 2020 2020 2020 4966 2074 6865 2063 6c75        If the clu
-000165a0: 7374 6572 2069 7320 7465 726d 696e 6174  ster is terminat
-000165b0: 6564 206f 7220 646f 6573 206e 6f74 2065  ed or does not e
-000165c0: 7869 7374 2c20 7265 7475 726e 204e 6f6e  xist, return Non
-000165d0: 652e 0a20 2020 2020 2020 204f 7468 6572  e..        Other
-000165e0: 7769 7365 2072 6574 7572 6e73 2074 6865  wise returns the
-000165f0: 2063 6c75 7374 6572 2072 6563 6f72 642e   cluster record.
-00016600: 0a0a 2020 2020 5261 6973 6573 3a0a 2020  ..    Raises:.  
-00016610: 2020 2020 2020 6578 6365 7074 696f 6e73        exceptions
-00016620: 2e43 6c75 7374 6572 4f77 6e65 7249 6465  .ClusterOwnerIde
-00016630: 6e74 6974 794d 6973 6d61 7463 6845 7272  ntityMismatchErr
-00016640: 6f72 3a20 6966 2074 6865 2063 7572 7265  or: if the curre
-00016650: 6e74 2075 7365 7220 6973 0a20 2020 2020  nt user is.     
-00016660: 2020 2020 206e 6f74 2074 6865 2073 616d       not the sam
-00016670: 6520 6173 2074 6865 2075 7365 7220 7768  e as the user wh
-00016680: 6f20 6372 6561 7465 6420 7468 6520 636c  o created the cl
-00016690: 7573 7465 722e 0a20 2020 2020 2020 2065  uster..        e
-000166a0: 7863 6570 7469 6f6e 732e 436c 6f75 6455  xceptions.CloudU
-000166b0: 7365 7249 6465 6e74 6974 7945 7272 6f72  serIdentityError
-000166c0: 3a20 6966 2077 6520 6661 696c 2074 6f20  : if we fail to 
-000166d0: 6765 7420 7468 6520 6375 7272 656e 7420  get the current 
-000166e0: 7573 6572 0a20 2020 2020 2020 2020 2069  user.          i
-000166f0: 6465 6e74 6974 792e 0a20 2020 2020 2020  dentity..       
-00016700: 2065 7863 6570 7469 6f6e 732e 436c 7573   exceptions.Clus
-00016710: 7465 7253 7461 7475 7346 6574 6368 696e  terStatusFetchin
-00016720: 6745 7272 6f72 3a20 7468 6520 636c 7573  gError: the clus
-00016730: 7465 7220 7374 6174 7573 2063 616e 6e6f  ter status canno
-00016740: 7420 6265 0a20 2020 2020 2020 2020 2066  t be.          f
-00016750: 6574 6368 6564 2066 726f 6d20 7468 6520  etched from the 
-00016760: 636c 6f75 6420 7072 6f76 6964 6572 206f  cloud provider o
-00016770: 7220 7468 6572 6520 6172 6520 6c65 616b  r there are leak
-00016780: 6564 206e 6f64 6573 2063 6175 7369 6e67  ed nodes causing
-00016790: 0a20 2020 2020 2020 2020 2074 6865 206e  .          the n
-000167a0: 6f64 6520 6e75 6d62 6572 206c 6172 6765  ode number large
-000167b0: 7220 7468 616e 2065 7870 6563 7465 642e  r than expected.
-000167c0: 0a20 2020 2022 2222 0a0a 2020 2020 7265  .    """..    re
-000167d0: 636f 7264 203d 2067 6c6f 6261 6c5f 7573  cord = global_us
-000167e0: 6572 5f73 7461 7465 2e67 6574 5f63 6c75  er_state.get_clu
-000167f0: 7374 6572 5f66 726f 6d5f 6e61 6d65 2863  ster_from_name(c
-00016800: 6c75 7374 6572 5f6e 616d 6529 0a20 2020  luster_name).   
-00016810: 2069 6620 7265 636f 7264 2069 7320 4e6f   if record is No
-00016820: 6e65 3a0a 2020 2020 2020 2020 7265 7475  ne:.        retu
-00016830: 726e 204e 6f6e 650a 2020 2020 6368 6563  rn None.    chec
-00016840: 6b5f 6f77 6e65 725f 6964 656e 7469 7479  k_owner_identity
-00016850: 2863 6c75 7374 6572 5f6e 616d 6529 0a0a  (cluster_name)..
-00016860: 2020 2020 6861 6e64 6c65 203d 2072 6563      handle = rec
-00016870: 6f72 645b 2768 616e 646c 6527 5d0a 2020  ord['handle'].  
-00016880: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00016890: 6861 6e64 6c65 2c20 6261 636b 656e 6473  handle, backends
-000168a0: 2e43 6c6f 7564 566d 5261 7952 6573 6f75  .CloudVmRayResou
-000168b0: 7263 6548 616e 646c 6529 3a0a 2020 2020  rceHandle):.    
-000168c0: 2020 2020 7573 655f 7370 6f74 203d 2068      use_spot = h
-000168d0: 616e 646c 652e 6c61 756e 6368 6564 5f72  andle.launched_r
-000168e0: 6573 6f75 7263 6573 2e75 7365 5f73 706f  esources.use_spo
-000168f0: 740a 2020 2020 2020 2020 6861 735f 6175  t.        has_au
-00016900: 746f 7374 6f70 203d 2028 7265 636f 7264  tostop = (record
-00016910: 5b27 7374 6174 7573 275d 2021 3d20 7374  ['status'] != st
-00016920: 6174 7573 5f6c 6962 2e43 6c75 7374 6572  atus_lib.Cluster
-00016930: 5374 6174 7573 2e53 544f 5050 4544 2061  Status.STOPPED a
-00016940: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
-00016950: 2020 2020 2020 2020 2020 2072 6563 6f72             recor
-00016960: 645b 2761 7574 6f73 746f 7027 5d20 3e3d  d['autostop'] >=
-00016970: 2030 290a 2020 2020 2020 2020 666f 7263   0).        forc
-00016980: 655f 7265 6672 6573 685f 666f 725f 636c  e_refresh_for_cl
-00016990: 7573 7465 7220 3d20 2866 6f72 6365 5f72  uster = (force_r
-000169a0: 6566 7265 7368 5f73 7461 7475 7365 7320  efresh_statuses 
-000169b0: 6973 206e 6f74 204e 6f6e 6520 616e 640a  is not None and.
-000169c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000169d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000169e0: 2020 2020 2072 6563 6f72 645b 2773 7461       record['sta
-000169f0: 7475 7327 5d20 696e 2066 6f72 6365 5f72  tus'] in force_r
-00016a00: 6566 7265 7368 5f73 7461 7475 7365 7329  efresh_statuses)
-00016a10: 0a20 2020 2020 2020 2069 6620 666f 7263  .        if forc
-00016a20: 655f 7265 6672 6573 685f 666f 725f 636c  e_refresh_for_cl
-00016a30: 7573 7465 7220 6f72 2068 6173 5f61 7574  uster or has_aut
-00016a40: 6f73 746f 7020 6f72 2075 7365 5f73 706f  ostop or use_spo
-00016a50: 743a 0a20 2020 2020 2020 2020 2020 2072  t:.            r
-00016a60: 6563 6f72 6420 3d20 5f75 7064 6174 655f  ecord = _update_
-00016a70: 636c 7573 7465 725f 7374 6174 7573 280a  cluster_status(.
-00016a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a90: 636c 7573 7465 725f 6e61 6d65 2c0a 2020  cluster_name,.  
-00016aa0: 2020 2020 2020 2020 2020 2020 2020 6163                ac
-00016ab0: 7175 6972 655f 7065 725f 636c 7573 7465  quire_per_cluste
-00016ac0: 725f 7374 6174 7573 5f6c 6f63 6b3d 6163  r_status_lock=ac
-00016ad0: 7175 6972 655f 7065 725f 636c 7573 7465  quire_per_cluste
-00016ae0: 725f 7374 6174 7573 5f6c 6f63 6b2c 0a20  r_status_lock,. 
-00016af0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00016b00: 6c75 7374 6572 5f73 7461 7475 735f 6c6f  luster_status_lo
-00016b10: 636b 5f74 696d 656f 7574 3d63 6c75 7374  ck_timeout=clust
-00016b20: 6572 5f73 7461 7475 735f 6c6f 636b 5f74  er_status_lock_t
-00016b30: 696d 656f 7574 290a 2020 2020 7265 7475  imeout).    retu
-00016b40: 726e 2072 6563 6f72 640a 0a0a 4074 696d  rn record...@tim
-00016b50: 656c 696e 652e 6576 656e 740a 6465 6620  eline.event.def 
-00016b60: 7265 6672 6573 685f 636c 7573 7465 725f  refresh_cluster_
-00016b70: 7374 6174 7573 5f68 616e 646c 6528 0a20  status_handle(. 
-00016b80: 2020 2063 6c75 7374 6572 5f6e 616d 653a     cluster_name:
-00016b90: 2073 7472 2c0a 2020 2020 2a2c 0a20 2020   str,.    *,.   
-00016ba0: 2066 6f72 6365 5f72 6566 7265 7368 5f73   force_refresh_s
-00016bb0: 7461 7475 7365 733a 204f 7074 696f 6e61  tatuses: Optiona
-00016bc0: 6c5b 5365 745b 7374 6174 7573 5f6c 6962  l[Set[status_lib
-00016bd0: 2e43 6c75 7374 6572 5374 6174 7573 5d5d  .ClusterStatus]]
-00016be0: 203d 204e 6f6e 652c 0a20 2020 2061 6371   = None,.    acq
-00016bf0: 7569 7265 5f70 6572 5f63 6c75 7374 6572  uire_per_cluster
-00016c00: 5f73 7461 7475 735f 6c6f 636b 3a20 626f  _status_lock: bo
-00016c10: 6f6c 203d 2054 7275 652c 0a20 2020 2063  ol = True,.    c
-00016c20: 6c75 7374 6572 5f73 7461 7475 735f 6c6f  luster_status_lo
-00016c30: 636b 5f74 696d 656f 7574 3a20 696e 7420  ck_timeout: int 
-00016c40: 3d20 434c 5553 5445 525f 5354 4154 5553  = CLUSTER_STATUS
-00016c50: 5f4c 4f43 4b5f 5449 4d45 4f55 545f 5345  _LOCK_TIMEOUT_SE
-00016c60: 434f 4e44 530a 2920 2d3e 2054 7570 6c65  CONDS.) -> Tuple
-00016c70: 5b4f 7074 696f 6e61 6c5b 7374 6174 7573  [Optional[status
-00016c80: 5f6c 6962 2e43 6c75 7374 6572 5374 6174  _lib.ClusterStat
-00016c90: 7573 5d2c 0a20 2020 2020 2020 2020 2020  us],.           
-00016ca0: 4f70 7469 6f6e 616c 5b62 6163 6b65 6e64  Optional[backend
-00016cb0: 732e 5265 736f 7572 6365 4861 6e64 6c65  s.ResourceHandle
-00016cc0: 5d5d 3a0a 2020 2020 2222 2252 6566 7265  ]]:.    """Refre
-00016cd0: 7368 2074 6865 2063 6c75 7374 6572 2c20  sh the cluster, 
-00016ce0: 616e 6420 7265 7475 726e 2074 6865 2070  and return the p
-00016cf0: 6f73 7369 626c 7920 7570 6461 7465 6420  ossibly updated 
-00016d00: 7374 6174 7573 2061 6e64 2068 616e 646c  status and handl
-00016d10: 652e 0a0a 2020 2020 5468 6973 2069 7320  e...    This is 
-00016d20: 6120 7772 6170 7065 7220 6f66 2072 6566  a wrapper of ref
-00016d30: 7265 7368 5f63 6c75 7374 6572 5f72 6563  resh_cluster_rec
-00016d40: 6f72 642c 2077 6869 6368 2072 6574 7572  ord, which retur
-00016d50: 6e73 2074 6865 2073 7461 7475 7320 616e  ns the status an
-00016d60: 640a 2020 2020 6861 6e64 6c65 206f 6620  d.    handle of 
-00016d70: 7468 6520 636c 7573 7465 722e 0a20 2020  the cluster..   
-00016d80: 2050 6c65 6173 6520 7265 6665 7220 746f   Please refer to
-00016d90: 2074 6865 2064 6f63 7374 7269 6e67 206f   the docstring o
-00016da0: 6620 7265 6672 6573 685f 636c 7573 7465  f refresh_cluste
-00016db0: 725f 7265 636f 7264 2066 6f72 2074 6865  r_record for the
-00016dc0: 2064 6574 6169 6c73 2e0a 2020 2020 2222   details..    ""
-00016dd0: 220a 2020 2020 7265 636f 7264 203d 2072  ".    record = r
-00016de0: 6566 7265 7368 5f63 6c75 7374 6572 5f72  efresh_cluster_r
-00016df0: 6563 6f72 6428 0a20 2020 2020 2020 2063  ecord(.        c
-00016e00: 6c75 7374 6572 5f6e 616d 652c 0a20 2020  luster_name,.   
-00016e10: 2020 2020 2066 6f72 6365 5f72 6566 7265       force_refre
-00016e20: 7368 5f73 7461 7475 7365 733d 666f 7263  sh_statuses=forc
-00016e30: 655f 7265 6672 6573 685f 7374 6174 7573  e_refresh_status
-00016e40: 6573 2c0a 2020 2020 2020 2020 6163 7175  es,.        acqu
-00016e50: 6972 655f 7065 725f 636c 7573 7465 725f  ire_per_cluster_
-00016e60: 7374 6174 7573 5f6c 6f63 6b3d 6163 7175  status_lock=acqu
-00016e70: 6972 655f 7065 725f 636c 7573 7465 725f  ire_per_cluster_
-00016e80: 7374 6174 7573 5f6c 6f63 6b2c 0a20 2020  status_lock,.   
-00016e90: 2020 2020 2063 6c75 7374 6572 5f73 7461       cluster_sta
-00016ea0: 7475 735f 6c6f 636b 5f74 696d 656f 7574  tus_lock_timeout
-00016eb0: 3d63 6c75 7374 6572 5f73 7461 7475 735f  =cluster_status_
-00016ec0: 6c6f 636b 5f74 696d 656f 7574 290a 2020  lock_timeout).  
-00016ed0: 2020 6966 2072 6563 6f72 6420 6973 204e    if record is N
-00016ee0: 6f6e 653a 0a20 2020 2020 2020 2072 6574  one:.        ret
-00016ef0: 7572 6e20 4e6f 6e65 2c20 4e6f 6e65 0a20  urn None, None. 
-00016f00: 2020 2072 6574 7572 6e20 7265 636f 7264     return record
-00016f10: 5b27 7374 6174 7573 275d 2c20 7265 636f  ['status'], reco
-00016f20: 7264 5b27 6861 6e64 6c65 275d 0a0a 0a23  rd['handle']...#
-00016f30: 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   ===============
-00016f40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00016f50: 3d3d 3d3d 3d3d 0a0a 0a40 7479 7069 6e67  ======...@typing
-00016f60: 2e6f 7665 726c 6f61 640a 6465 6620 6368  .overload.def ch
-00016f70: 6563 6b5f 636c 7573 7465 725f 6176 6169  eck_cluster_avai
-00016f80: 6c61 626c 6528 0a20 2020 2063 6c75 7374  lable(.    clust
-00016f90: 6572 5f6e 616d 653a 2073 7472 2c0a 2020  er_name: str,.  
-00016fa0: 2020 2a2c 0a20 2020 206f 7065 7261 7469    *,.    operati
-00016fb0: 6f6e 3a20 7374 722c 0a20 2020 2063 6865  on: str,.    che
-00016fc0: 636b 5f63 6c6f 7564 5f76 6d5f 7261 795f  ck_cloud_vm_ray_
-00016fd0: 6261 636b 656e 643a 204c 6974 6572 616c  backend: Literal
-00016fe0: 5b54 7275 655d 203d 2054 7275 652c 0a20  [True] = True,. 
-00016ff0: 2020 2064 7279 7275 6e3a 2062 6f6f 6c20     dryrun: bool 
-00017000: 3d20 2e2e 2e2c 0a29 202d 3e20 2763 6c6f  = ...,.) -> 'clo
-00017010: 7564 5f76 6d5f 7261 795f 6261 636b 656e  ud_vm_ray_backen
-00017020: 642e 436c 6f75 6456 6d52 6179 5265 736f  d.CloudVmRayReso
-00017030: 7572 6365 4861 6e64 6c65 273a 0a20 2020  urceHandle':.   
-00017040: 202e 2e2e 0a0a 0a40 7479 7069 6e67 2e6f   ......@typing.o
-00017050: 7665 726c 6f61 640a 6465 6620 6368 6563  verload.def chec
-00017060: 6b5f 636c 7573 7465 725f 6176 6169 6c61  k_cluster_availa
-00017070: 626c 6528 0a20 2020 2063 6c75 7374 6572  ble(.    cluster
-00017080: 5f6e 616d 653a 2073 7472 2c0a 2020 2020  _name: str,.    
-00017090: 2a2c 0a20 2020 206f 7065 7261 7469 6f6e  *,.    operation
-000170a0: 3a20 7374 722c 0a20 2020 2063 6865 636b  : str,.    check
-000170b0: 5f63 6c6f 7564 5f76 6d5f 7261 795f 6261  _cloud_vm_ray_ba
-000170c0: 636b 656e 643a 204c 6974 6572 616c 5b46  ckend: Literal[F
-000170d0: 616c 7365 5d2c 0a20 2020 2064 7279 7275  alse],.    dryru
-000170e0: 6e3a 2062 6f6f 6c20 3d20 2e2e 2e2c 0a29  n: bool = ...,.)
-000170f0: 202d 3e20 6261 636b 656e 6473 2e52 6573   -> backends.Res
-00017100: 6f75 7263 6548 616e 646c 653a 0a20 2020  ourceHandle:.   
-00017110: 202e 2e2e 0a0a 0a64 6566 2063 6865 636b   ......def check
-00017120: 5f63 6c75 7374 6572 5f61 7661 696c 6162  _cluster_availab
-00017130: 6c65 280a 2020 2020 636c 7573 7465 725f  le(.    cluster_
-00017140: 6e61 6d65 3a20 7374 722c 0a20 2020 202a  name: str,.    *
-00017150: 2c0a 2020 2020 6f70 6572 6174 696f 6e3a  ,.    operation:
-00017160: 2073 7472 2c0a 2020 2020 6368 6563 6b5f   str,.    check_
-00017170: 636c 6f75 645f 766d 5f72 6179 5f62 6163  cloud_vm_ray_bac
-00017180: 6b65 6e64 3a20 626f 6f6c 203d 2054 7275  kend: bool = Tru
-00017190: 652c 0a20 2020 2064 7279 7275 6e3a 2062  e,.    dryrun: b
-000171a0: 6f6f 6c20 3d20 4661 6c73 652c 0a29 202d  ool = False,.) -
-000171b0: 3e20 6261 636b 656e 6473 2e52 6573 6f75  > backends.Resou
-000171c0: 7263 6548 616e 646c 653a 0a20 2020 2022  rceHandle:.    "
-000171d0: 2222 4368 6563 6b20 6966 2074 6865 2063  ""Check if the c
-000171e0: 6c75 7374 6572 2069 7320 6176 6169 6c61  luster is availa
-000171f0: 626c 652e 0a0a 2020 2020 5261 6973 6573  ble...    Raises
-00017200: 3a0a 2020 2020 2020 2020 5661 6c75 6545  :.        ValueE
-00017210: 7272 6f72 3a20 6966 2074 6865 2063 6c75  rror: if the clu
-00017220: 7374 6572 2064 6f65 7320 6e6f 7420 6578  ster does not ex
-00017230: 6973 742e 0a20 2020 2020 2020 2065 7863  ist..        exc
-00017240: 6570 7469 6f6e 732e 436c 7573 7465 724e  eptions.ClusterN
-00017250: 6f74 5570 4572 726f 723a 2069 6620 7468  otUpError: if th
-00017260: 6520 636c 7573 7465 7220 6973 206e 6f74  e cluster is not
-00017270: 2055 502e 0a20 2020 2020 2020 2065 7863   UP..        exc
-00017280: 6570 7469 6f6e 732e 4e6f 7453 7570 706f  eptions.NotSuppo
-00017290: 7274 6564 4572 726f 723a 2069 6620 7468  rtedError: if th
-000172a0: 6520 636c 7573 7465 7220 6973 206e 6f74  e cluster is not
-000172b0: 2062 6173 6564 206f 6e0a 2020 2020 2020   based on.      
-000172c0: 2020 2020 436c 6f75 6456 6d52 6179 4261      CloudVmRayBa
-000172d0: 636b 656e 642e 0a20 2020 2020 2020 2065  ckend..        e
-000172e0: 7863 6570 7469 6f6e 732e 436c 7573 7465  xceptions.Cluste
-000172f0: 724f 776e 6572 4964 656e 7469 7479 4d69  rOwnerIdentityMi
-00017300: 736d 6174 6368 4572 726f 723a 2069 6620  smatchError: if 
-00017310: 7468 6520 6375 7272 656e 7420 7573 6572  the current user
-00017320: 2069 730a 2020 2020 2020 2020 2020 6e6f   is.          no
-00017330: 7420 7468 6520 7361 6d65 2061 7320 7468  t the same as th
-00017340: 6520 7573 6572 2077 686f 2063 7265 6174  e user who creat
-00017350: 6564 2074 6865 2063 6c75 7374 6572 2e0a  ed the cluster..
-00017360: 2020 2020 2020 2020 6578 6365 7074 696f          exceptio
-00017370: 6e73 2e43 6c6f 7564 5573 6572 4964 656e  ns.CloudUserIden
-00017380: 7469 7479 4572 726f 723a 2069 6620 7765  tityError: if we
-00017390: 2066 6169 6c20 746f 2067 6574 2074 6865   fail to get the
-000173a0: 2063 7572 7265 6e74 2075 7365 720a 2020   current user.  
-000173b0: 2020 2020 2020 2020 6964 656e 7469 7479          identity
-000173c0: 2e0a 2020 2020 2222 220a 2020 2020 7265  ..    """.    re
-000173d0: 636f 7264 203d 2067 6c6f 6261 6c5f 7573  cord = global_us
-000173e0: 6572 5f73 7461 7465 2e67 6574 5f63 6c75  er_state.get_clu
-000173f0: 7374 6572 5f66 726f 6d5f 6e61 6d65 2863  ster_from_name(c
-00017400: 6c75 7374 6572 5f6e 616d 6529 0a20 2020  luster_name).   
-00017410: 2069 6620 6472 7972 756e 3a0a 2020 2020   if dryrun:.    
-00017420: 2020 2020 6173 7365 7274 2072 6563 6f72      assert recor
-00017430: 6420 6973 206e 6f74 204e 6f6e 652c 2063  d is not None, c
-00017440: 6c75 7374 6572 5f6e 616d 650a 2020 2020  luster_name.    
-00017450: 2020 2020 7265 7475 726e 2072 6563 6f72      return recor
-00017460: 645b 2768 616e 646c 6527 5d0a 0a20 2020  d['handle']..   
-00017470: 2070 7265 7669 6f75 735f 636c 7573 7465   previous_cluste
-00017480: 725f 7374 6174 7573 203d 204e 6f6e 650a  r_status = None.
-00017490: 2020 2020 6966 2072 6563 6f72 6420 6973      if record is
-000174a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000174b0: 2020 2070 7265 7669 6f75 735f 636c 7573     previous_clus
-000174c0: 7465 725f 7374 6174 7573 203d 2072 6563  ter_status = rec
-000174d0: 6f72 645b 2773 7461 7475 7327 5d0a 0a20  ord['status'].. 
-000174e0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-000174f0: 636c 7573 7465 725f 7374 6174 7573 2c20  cluster_status, 
-00017500: 6861 6e64 6c65 203d 2072 6566 7265 7368  handle = refresh
-00017510: 5f63 6c75 7374 6572 5f73 7461 7475 735f  _cluster_status_
-00017520: 6861 6e64 6c65 2863 6c75 7374 6572 5f6e  handle(cluster_n
-00017530: 616d 6529 0a20 2020 2065 7863 6570 7420  ame).    except 
-00017540: 6578 6365 7074 696f 6e73 2e43 6c75 7374  exceptions.Clust
-00017550: 6572 5374 6174 7573 4665 7463 6869 6e67  erStatusFetching
-00017560: 4572 726f 7220 6173 2065 3a0a 2020 2020  Error as e:.    
-00017570: 2020 2020 2320 4661 696c 6564 2074 6f20      # Failed to 
-00017580: 7265 6672 6573 6820 7468 6520 636c 7573  refresh the clus
-00017590: 7465 7220 7374 6174 7573 2069 7320 6e6f  ter status is no
-000175a0: 7420 6661 7461 6c20 6572 726f 7220 6173  t fatal error as
-000175b0: 2074 6865 2063 616c 6c65 7273 0a20 2020   the callers.   
-000175c0: 2020 2020 2023 2063 616e 2073 7469 6c6c       # can still
-000175d0: 2062 6520 646f 6e65 2062 7920 6f6e 6c79   be done by only
-000175e0: 2075 7369 6e67 2073 7368 2c20 6275 7420   using ssh, but 
-000175f0: 7468 6520 7373 6820 6361 6e20 6861 6e67  the ssh can hang
-00017600: 2069 6620 7468 650a 2020 2020 2020 2020   if the.        
-00017610: 2320 636c 7573 7465 7220 6973 206e 6f74  # cluster is not
-00017620: 2075 7020 2865 2e67 2e2c 2061 7574 6f73   up (e.g., autos
-00017630: 746f 7070 6564 292e 0a0a 2020 2020 2020  topped)...      
-00017640: 2020 2320 5765 2064 6f20 6e6f 7420 6361    # We do not ca
-00017650: 7463 6820 7468 6520 6578 6365 7074 696f  tch the exceptio
-00017660: 6e20 666f 7220 636c 6f75 6420 6964 656e  n for cloud iden
-00017670: 7469 7479 2063 6865 636b 696e 6720 666f  tity checking fo
-00017680: 7220 6e6f 772c 2069 6e0a 2020 2020 2020  r now, in.      
-00017690: 2020 2320 6f72 6465 7220 746f 2064 6973    # order to dis
-000176a0: 6162 6c65 2061 6c6c 206f 7065 7261 7469  able all operati
-000176b0: 6f6e 7320 6f6e 2063 6c75 7374 6572 7320  ons on clusters 
-000176c0: 6372 6561 7465 6420 6279 2061 6e6f 7468  created by anoth
-000176d0: 6572 2075 7365 720a 2020 2020 2020 2020  er user.        
-000176e0: 2320 6964 656e 7469 7479 2e20 2054 6861  # identity.  Tha
-000176f0: 7420 7769 6c6c 206d 616b 6520 7468 6520  t will make the 
-00017700: 6465 7369 676e 2073 696d 706c 6572 2061  design simpler a
-00017710: 6e64 2065 6173 6965 7220 746f 0a20 2020  nd easier to.   
-00017720: 2020 2020 2023 2075 6e64 6572 7374 616e       # understan
-00017730: 642c 2062 7574 2069 7420 6d69 6768 7420  d, but it might 
-00017740: 6265 2075 7365 6675 6c20 746f 2061 6c6c  be useful to all
-00017750: 6f77 2074 6865 2075 7365 7220 746f 2075  ow the user to u
-00017760: 7365 0a20 2020 2020 2020 2023 206f 7065  se.        # ope
-00017770: 7261 7469 6f6e 7320 7468 6174 206f 6e6c  rations that onl
-00017780: 7920 696e 766f 6c76 6520 7373 6820 2865  y involve ssh (e
-00017790: 2e67 2e2c 2073 6b79 2065 7865 632c 2073  .g., sky exec, s
-000177a0: 6b79 206c 6f67 732c 2065 7463 2920 6576  ky logs, etc) ev
-000177b0: 656e 0a20 2020 2020 2020 2023 2069 6620  en.        # if 
-000177c0: 7468 6520 7573 6572 2069 7320 6e6f 7420  the user is not 
-000177d0: 7468 6520 6f77 6e65 7220 6f66 2074 6865  the owner of the
-000177e0: 2063 6c75 7374 6572 2e0a 2020 2020 2020   cluster..      
-000177f0: 2020 7578 5f75 7469 6c73 2e63 6f6e 736f    ux_utils.conso
-00017800: 6c65 5f6e 6577 6c69 6e65 2829 0a20 2020  le_newline().   
-00017810: 2020 2020 206c 6f67 6765 722e 7761 726e       logger.warn
-00017820: 696e 6728 0a20 2020 2020 2020 2020 2020  ing(.           
-00017830: 2066 2746 6169 6c65 6420 746f 2072 6566   f'Failed to ref
-00017840: 7265 7368 2074 6865 2073 7461 7475 7320  resh the status 
-00017850: 666f 7220 636c 7573 7465 7220 7b63 6c75  for cluster {clu
-00017860: 7374 6572 5f6e 616d 6521 727d 2e20 4974  ster_name!r}. It
-00017870: 2069 7320 270a 2020 2020 2020 2020 2020   is '.          
-00017880: 2020 6627 6e6f 7420 6661 7461 6c2c 2062    f'not fatal, b
-00017890: 7574 207b 6f70 6572 6174 696f 6e7d 206d  ut {operation} m
-000178a0: 6967 6874 2068 616e 6720 6966 2074 6865  ight hang if the
-000178b0: 2063 6c75 7374 6572 2069 7320 6e6f 7420   cluster is not 
-000178c0: 7570 2e5c 6e27 0a20 2020 2020 2020 2020  up.\n'.         
-000178d0: 2020 2066 2744 6574 6169 6c65 6420 7265     f'Detailed re
-000178e0: 6173 6f6e 3a20 7b65 7d27 290a 2020 2020  ason: {e}').    
-000178f0: 2020 2020 6966 2072 6563 6f72 6420 6973      if record is
-00017900: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00017910: 2020 2063 6c75 7374 6572 5f73 7461 7475     cluster_statu
-00017920: 732c 2068 616e 646c 6520 3d20 4e6f 6e65  s, handle = None
-00017930: 2c20 4e6f 6e65 0a20 2020 2020 2020 2065  , None.        e
-00017940: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00017950: 2063 6c75 7374 6572 5f73 7461 7475 732c   cluster_status,
-00017960: 2068 616e 646c 6520 3d20 7265 636f 7264   handle = record
-00017970: 5b27 7374 6174 7573 275d 2c20 7265 636f  ['status'], reco
-00017980: 7264 5b27 6861 6e64 6c65 275d 0a0a 2020  rd['handle']..  
-00017990: 2020 6272 6967 6874 203d 2063 6f6c 6f72    bright = color
-000179a0: 616d 612e 5374 796c 652e 4252 4947 4854  ama.Style.BRIGHT
-000179b0: 0a20 2020 2072 6573 6574 203d 2063 6f6c  .    reset = col
-000179c0: 6f72 616d 612e 5374 796c 652e 5245 5345  orama.Style.RESE
-000179d0: 545f 414c 4c0a 2020 2020 6966 2068 616e  T_ALL.    if han
-000179e0: 646c 6520 6973 204e 6f6e 653a 0a20 2020  dle is None:.   
-000179f0: 2020 2020 2069 6620 7072 6576 696f 7573       if previous
-00017a00: 5f63 6c75 7374 6572 5f73 7461 7475 7320  _cluster_status 
-00017a10: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00017a20: 2020 2020 2065 7272 6f72 5f6d 7367 203d       error_msg =
-00017a30: 2066 2743 6c75 7374 6572 207b 636c 7573   f'Cluster {clus
-00017a40: 7465 725f 6e61 6d65 2172 7d20 646f 6573  ter_name!r} does
-00017a50: 206e 6f74 2065 7869 7374 2e27 0a20 2020   not exist.'.   
-00017a60: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00017a70: 2020 2020 2020 2065 7272 6f72 5f6d 7367         error_msg
-00017a80: 203d 2028 6627 436c 7573 7465 7220 7b63   = (f'Cluster {c
-00017a90: 6c75 7374 6572 5f6e 616d 6521 727d 206e  luster_name!r} n
-00017aa0: 6f74 2066 6f75 6e64 206f 6e20 7468 6520  ot found on the 
-00017ab0: 636c 6f75 6420 270a 2020 2020 2020 2020  cloud '.        
-00017ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ad0: 2027 7072 6f76 6964 6572 2e27 290a 2020   'provider.').  
-00017ae0: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-00017af0: 2072 6563 6f72 6420 6973 206e 6f74 204e   record is not N
-00017b00: 6f6e 652c 2070 7265 7669 6f75 735f 636c  one, previous_cl
-00017b10: 7573 7465 725f 7374 6174 7573 0a20 2020  uster_status.   
-00017b20: 2020 2020 2020 2020 2061 6374 696f 6e73           actions
-00017b30: 203d 205b 5d0a 2020 2020 2020 2020 2020   = [].          
-00017b40: 2020 6966 2072 6563 6f72 645b 2768 616e    if record['han
-00017b50: 646c 6527 5d2e 6c61 756e 6368 6564 5f72  dle'].launched_r
-00017b60: 6573 6f75 7263 6573 2e75 7365 5f73 706f  esources.use_spo
-00017b70: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-00017b80: 2020 2061 6374 696f 6e73 2e61 7070 656e     actions.appen
-00017b90: 6428 2770 7265 656d 7074 6564 2729 0a20  d('preempted'). 
-00017ba0: 2020 2020 2020 2020 2020 2069 6620 7265             if re
-00017bb0: 636f 7264 5b27 6175 746f 7374 6f70 275d  cord['autostop']
-00017bc0: 203e 2030 2061 6e64 2072 6563 6f72 645b   > 0 and record[
-00017bd0: 2774 6f5f 646f 776e 275d 3a0a 2020 2020  'to_down']:.    
-00017be0: 2020 2020 2020 2020 2020 2020 6163 7469              acti
-00017bf0: 6f6e 732e 6170 7065 6e64 2827 6175 746f  ons.append('auto
-00017c00: 646f 776e 6564 2729 0a20 2020 2020 2020  downed').       
-00017c10: 2020 2020 2061 6374 696f 6e73 2e61 7070       actions.app
-00017c20: 656e 6428 276d 616e 7561 6c6c 7920 7465  end('manually te
-00017c30: 726d 696e 6174 6564 2069 6e20 636f 6e73  rminated in cons
-00017c40: 6f6c 6527 290a 2020 2020 2020 2020 2020  ole').          
-00017c50: 2020 6966 206c 656e 2861 6374 696f 6e73    if len(actions
-00017c60: 2920 3e20 313a 0a20 2020 2020 2020 2020  ) > 1:.         
-00017c70: 2020 2020 2020 2061 6374 696f 6e73 5b2d         actions[-
-00017c80: 315d 203d 2027 6f72 2027 202b 2061 6374  1] = 'or ' + act
-00017c90: 696f 6e73 5b2d 315d 0a20 2020 2020 2020  ions[-1].       
-00017ca0: 2020 2020 2061 6374 696f 6e73 5f73 7472       actions_str
-00017cb0: 203d 2027 2c20 272e 6a6f 696e 2861 6374   = ', '.join(act
-00017cc0: 696f 6e73 290a 2020 2020 2020 2020 2020  ions).          
-00017cd0: 2020 6d65 7373 6167 6520 3d20 6627 2049    message = f' I
-00017ce0: 7420 7761 7320 6c69 6b65 6c79 207b 6163  t was likely {ac
-00017cf0: 7469 6f6e 735f 7374 727d 2e27 0a20 2020  tions_str}.'.   
-00017d00: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
-00017d10: 6163 7469 6f6e 7329 203e 2031 3a0a 2020  actions) > 1:.  
-00017d20: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-00017d30: 7373 6167 6520 3d20 6d65 7373 6167 652e  ssage = message.
-00017d40: 7265 706c 6163 6528 276c 696b 656c 7927  replace('likely'
-00017d50: 2c20 2765 6974 6865 7227 290a 2020 2020  , 'either').    
-00017d60: 2020 2020 2020 2020 6572 726f 725f 6d73          error_ms
-00017d70: 6720 2b3d 206d 6573 7361 6765 0a0a 2020  g += message..  
-00017d80: 2020 2020 2020 7769 7468 2075 785f 7574        with ux_ut
-00017d90: 696c 732e 7072 696e 745f 6578 6365 7074  ils.print_except
-00017da0: 696f 6e5f 6e6f 5f74 7261 6365 6261 636b  ion_no_traceback
-00017db0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00017dc0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00017dd0: 2866 277b 636f 6c6f 7261 6d61 2e46 6f72  (f'{colorama.For
-00017de0: 652e 5945 4c4c 4f57 7d7b 6572 726f 725f  e.YELLOW}{error_
-00017df0: 6d73 677d 7b72 6573 6574 7d27 290a 2020  msg}{reset}').  
-00017e00: 2020 6173 7365 7274 2063 6c75 7374 6572    assert cluster
-00017e10: 5f73 7461 7475 7320 6973 206e 6f74 204e  _status is not N
-00017e20: 6f6e 652c 2027 6861 6e64 6c65 2069 7320  one, 'handle is 
-00017e30: 6e6f 7420 4e6f 6e65 2062 7574 2073 7461  not None but sta
-00017e40: 7475 7320 6973 204e 6f6e 6527 0a20 2020  tus is None'.   
-00017e50: 2062 6163 6b65 6e64 203d 2067 6574 5f62   backend = get_b
-00017e60: 6163 6b65 6e64 5f66 726f 6d5f 6861 6e64  ackend_from_hand
-00017e70: 6c65 2868 616e 646c 6529 0a20 2020 2069  le(handle).    i
-00017e80: 6620 6368 6563 6b5f 636c 6f75 645f 766d  f check_cloud_vm
-00017e90: 5f72 6179 5f62 6163 6b65 6e64 2061 6e64  _ray_backend and
-00017ea0: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
-00017eb0: 0a20 2020 2020 2020 2020 2020 2062 6163  .            bac
-00017ec0: 6b65 6e64 2c20 6261 636b 656e 6473 2e43  kend, backends.C
-00017ed0: 6c6f 7564 566d 5261 7942 6163 6b65 6e64  loudVmRayBackend
-00017ee0: 293a 0a20 2020 2020 2020 2077 6974 6820  ):.        with 
-00017ef0: 7578 5f75 7469 6c73 2e70 7269 6e74 5f65  ux_utils.print_e
-00017f00: 7863 6570 7469 6f6e 5f6e 6f5f 7472 6163  xception_no_trac
-00017f10: 6562 6163 6b28 293a 0a20 2020 2020 2020  eback():.       
-00017f20: 2020 2020 2072 6169 7365 2065 7863 6570       raise excep
-00017f30: 7469 6f6e 732e 4e6f 7453 7570 706f 7274  tions.NotSupport
-00017f40: 6564 4572 726f 7228 0a20 2020 2020 2020  edError(.       
-00017f50: 2020 2020 2020 2020 2066 277b 636f 6c6f           f'{colo
-00017f60: 7261 6d61 2e46 6f72 652e 5945 4c4c 4f57  rama.Fore.YELLOW
-00017f70: 7d7b 6f70 6572 6174 696f 6e2e 6361 7069  }{operation.capi
-00017f80: 7461 6c69 7a65 2829 7d3a 2073 6b69 7070  talize()}: skipp
-00017f90: 6564 2066 6f72 2027 0a20 2020 2020 2020  ed for '.       
-00017fa0: 2020 2020 2020 2020 2066 2763 6c75 7374           f'clust
-00017fb0: 6572 207b 636c 7573 7465 725f 6e61 6d65  er {cluster_name
-00017fc0: 2172 7d2e 2049 7420 6973 206f 6e6c 7920  !r}. It is only 
-00017fd0: 7375 7070 6f72 7465 6420 6279 2062 6163  supported by bac
-00017fe0: 6b65 6e64 3a20 270a 2020 2020 2020 2020  kend: '.        
-00017ff0: 2020 2020 2020 2020 6627 7b62 6163 6b65          f'{backe
-00018000: 6e64 732e 436c 6f75 6456 6d52 6179 4261  nds.CloudVmRayBa
-00018010: 636b 656e 642e 4e41 4d45 7d2e 270a 2020  ckend.NAME}.'.  
-00018020: 2020 2020 2020 2020 2020 2020 2020 6627                f'
-00018030: 7b72 6573 6574 7d27 290a 2020 2020 6966  {reset}').    if
-00018040: 2063 6c75 7374 6572 5f73 7461 7475 7320   cluster_status 
-00018050: 213d 2073 7461 7475 735f 6c69 622e 436c  != status_lib.Cl
-00018060: 7573 7465 7253 7461 7475 732e 5550 3a0a  usterStatus.UP:.
-00018070: 2020 2020 2020 2020 7769 7468 2075 785f          with ux_
-00018080: 7574 696c 732e 7072 696e 745f 6578 6365  utils.print_exce
-00018090: 7074 696f 6e5f 6e6f 5f74 7261 6365 6261  ption_no_traceba
-000180a0: 636b 2829 3a0a 2020 2020 2020 2020 2020  ck():.          
-000180b0: 2020 6869 6e74 5f66 6f72 5f69 6e69 7420    hint_for_init 
-000180c0: 3d20 2727 0a20 2020 2020 2020 2020 2020  = ''.           
-000180d0: 2069 6620 636c 7573 7465 725f 7374 6174   if cluster_stat
-000180e0: 7573 203d 3d20 7374 6174 7573 5f6c 6962  us == status_lib
-000180f0: 2e43 6c75 7374 6572 5374 6174 7573 2e49  .ClusterStatus.I
-00018100: 4e49 543a 0a20 2020 2020 2020 2020 2020  NIT:.           
-00018110: 2020 2020 2068 696e 745f 666f 725f 696e       hint_for_in
-00018120: 6974 203d 2028 0a20 2020 2020 2020 2020  it = (.         
-00018130: 2020 2020 2020 2020 2020 2066 277b 7265             f'{re
-00018140: 7365 747d 2057 6169 7420 666f 7220 6120  set} Wait for a 
-00018150: 6c61 756e 6368 2074 6f20 6669 6e69 7368  launch to finish
-00018160: 2c20 6f72 2075 7365 2074 6869 7320 636f  , or use this co
-00018170: 6d6d 616e 6420 270a 2020 2020 2020 2020  mmand '.        
-00018180: 2020 2020 2020 2020 2020 2020 6627 746f              f'to
-00018190: 2074 7279 2074 6f20 7472 616e 7369 7469   try to transiti
-000181a0: 6f6e 2074 6865 2063 6c75 7374 6572 2074  on the cluster t
-000181b0: 6f20 5550 3a20 7b62 7269 6768 747d 736b  o UP: {bright}sk
-000181c0: 7920 270a 2020 2020 2020 2020 2020 2020  y '.            
-000181d0: 2020 2020 2020 2020 6627 7374 6172 7420          f'start 
-000181e0: 7b63 6c75 7374 6572 5f6e 616d 657d 7b72  {cluster_name}{r
-000181f0: 6573 6574 7d27 290a 2020 2020 2020 2020  eset}').        
-00018200: 2020 2020 7261 6973 6520 6578 6365 7074      raise except
-00018210: 696f 6e73 2e43 6c75 7374 6572 4e6f 7455  ions.ClusterNotU
-00018220: 7045 7272 6f72 280a 2020 2020 2020 2020  pError(.        
-00018230: 2020 2020 2020 2020 6627 7b63 6f6c 6f72          f'{color
-00018240: 616d 612e 466f 7265 2e59 454c 4c4f 577d  ama.Fore.YELLOW}
-00018250: 7b6f 7065 7261 7469 6f6e 2e63 6170 6974  {operation.capit
-00018260: 616c 697a 6528 297d 3a20 736b 6970 7065  alize()}: skippe
-00018270: 6420 666f 7220 270a 2020 2020 2020 2020  d for '.        
-00018280: 2020 2020 2020 2020 6627 636c 7573 7465          f'cluste
-00018290: 7220 7b63 6c75 7374 6572 5f6e 616d 6521  r {cluster_name!
-000182a0: 727d 2028 7374 6174 7573 3a20 7b63 6c75  r} (status: {clu
-000182b0: 7374 6572 5f73 7461 7475 732e 7661 6c75  ster_status.valu
-000182c0: 657d 292e 2027 0a20 2020 2020 2020 2020  e}). '.         
-000182d0: 2020 2020 2020 2027 4974 2069 7320 6f6e         'It is on
-000182e0: 6c79 2061 6c6c 6f77 6564 2066 6f72 2027  ly allowed for '
-000182f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018300: 2066 277b 7374 6174 7573 5f6c 6962 2e43   f'{status_lib.C
-00018310: 6c75 7374 6572 5374 6174 7573 2e55 502e  lusterStatus.UP.
-00018320: 7661 6c75 657d 2063 6c75 7374 6572 732e  value} clusters.
-00018330: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-00018340: 2020 6627 7b68 696e 745f 666f 725f 696e    f'{hint_for_in
-00018350: 6974 7d27 0a20 2020 2020 2020 2020 2020  it}'.           
-00018360: 2020 2020 2066 277b 7265 7365 747d 272c       f'{reset}',
-00018370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018380: 2063 6c75 7374 6572 5f73 7461 7475 733d   cluster_status=
-00018390: 636c 7573 7465 725f 7374 6174 7573 2c0a  cluster_status,.
-000183a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000183b0: 6861 6e64 6c65 3d68 616e 646c 6529 0a0a  handle=handle)..
-000183c0: 2020 2020 6966 2068 616e 646c 652e 6865      if handle.he
-000183d0: 6164 5f69 7020 6973 204e 6f6e 653a 0a20  ad_ip is None:. 
-000183e0: 2020 2020 2020 2077 6974 6820 7578 5f75         with ux_u
-000183f0: 7469 6c73 2e70 7269 6e74 5f65 7863 6570  tils.print_excep
-00018400: 7469 6f6e 5f6e 6f5f 7472 6163 6562 6163  tion_no_tracebac
-00018410: 6b28 293a 0a20 2020 2020 2020 2020 2020  k():.           
-00018420: 2072 6169 7365 2065 7863 6570 7469 6f6e   raise exception
-00018430: 732e 436c 7573 7465 724e 6f74 5570 4572  s.ClusterNotUpEr
-00018440: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
-00018450: 2020 2020 2066 2743 6c75 7374 6572 207b       f'Cluster {
-00018460: 636c 7573 7465 725f 6e61 6d65 2172 7d20  cluster_name!r} 
-00018470: 6861 7320 6265 656e 2073 746f 7070 6564  has been stopped
-00018480: 206f 7220 6e6f 7420 7072 6f70 6572 6c79   or not properly
-00018490: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
-000184a0: 2020 2027 7365 7420 7570 2e20 506c 6561     'set up. Plea
-000184b0: 7365 2072 652d 6c61 756e 6368 2069 7420  se re-launch it 
-000184c0: 7769 7468 2060 736b 7920 7374 6172 7460  with `sky start`
-000184d0: 2e27 2c0a 2020 2020 2020 2020 2020 2020  .',.            
-000184e0: 2020 2020 636c 7573 7465 725f 7374 6174      cluster_stat
-000184f0: 7573 3d63 6c75 7374 6572 5f73 7461 7475  us=cluster_statu
-00018500: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-00018510: 2020 2068 616e 646c 653d 6861 6e64 6c65     handle=handle
-00018520: 290a 2020 2020 7265 7475 726e 2068 616e  ).    return han
-00018530: 646c 650a 0a0a 2320 544f 444f 2874 6961  dle...# TODO(tia
-00018540: 6e29 3a20 5265 6661 6374 6f72 2074 6f20  n): Refactor to 
-00018550: 636f 6e74 726f 6c6c 6572 5f75 7469 6c73  controller_utils
-00018560: 2e20 4375 7272 656e 7420 626c 6f63 6b65  . Current blocke
-00018570: 723a 2063 6972 6375 6c61 7220 696d 706f  r: circular impo
-00018580: 7274 2e0a 6465 6620 6973 5f63 6f6e 7472  rt..def is_contr
-00018590: 6f6c 6c65 725f 6163 6365 7373 6962 6c65  oller_accessible
-000185a0: 280a 2020 2020 636f 6e74 726f 6c6c 6572  (.    controller
-000185b0: 3a20 636f 6e74 726f 6c6c 6572 5f75 7469  : controller_uti
-000185c0: 6c73 2e43 6f6e 7472 6f6c 6c65 7273 2c0a  ls.Controllers,.
-000185d0: 2020 2020 7374 6f70 7065 645f 6d65 7373      stopped_mess
-000185e0: 6167 653a 2073 7472 2c0a 2020 2020 6e6f  age: str,.    no
-000185f0: 6e5f 6578 6973 7465 6e74 5f6d 6573 7361  n_existent_messa
-00018600: 6765 3a20 4f70 7469 6f6e 616c 5b73 7472  ge: Optional[str
-00018610: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 6578  ] = None,.    ex
-00018620: 6974 5f69 665f 6e6f 745f 6163 6365 7373  it_if_not_access
-00018630: 6962 6c65 3a20 626f 6f6c 203d 2046 616c  ible: bool = Fal
-00018640: 7365 2c0a 2920 2d3e 2027 6261 636b 656e  se,.) -> 'backen
-00018650: 6473 2e43 6c6f 7564 566d 5261 7952 6573  ds.CloudVmRayRes
-00018660: 6f75 7263 6548 616e 646c 6527 3a0a 2020  ourceHandle':.  
-00018670: 2020 2222 2243 6865 636b 2069 6620 7468    """Check if th
-00018680: 6520 6a6f 6273 2f73 6572 7665 2063 6f6e  e jobs/serve con
-00018690: 7472 6f6c 6c65 7220 6973 2075 702e 0a0a  troller is up...
-000186a0: 2020 2020 5468 6520 636f 6e74 726f 6c6c      The controll
-000186b0: 6572 2069 7320 6163 6365 7373 6962 6c65  er is accessible
-000186c0: 2077 6865 6e20 6974 2069 7320 696e 2055   when it is in U
-000186d0: 5020 6f72 2049 4e49 5420 7374 6174 652c  P or INIT state,
-000186e0: 2061 6e64 2074 6865 2073 7368 0a20 2020   and the ssh.   
-000186f0: 2063 6f6e 6e65 6374 696f 6e20 6973 2073   connection is s
-00018700: 7563 6365 7373 6675 6c2e 0a0a 2020 2020  uccessful...    
-00018710: 4974 2063 616e 2062 6520 7573 6564 2074  It can be used t
-00018720: 6f20 6368 6563 6b20 6966 2074 6865 2063  o check if the c
-00018730: 6f6e 7472 6f6c 6c65 7220 6973 2061 6363  ontroller is acc
-00018740: 6573 7369 626c 6520 2873 696e 6365 2074  essible (since t
-00018750: 6865 2061 7574 6f73 746f 700a 2020 2020  he autostop.    
-00018760: 6973 2073 6574 2066 6f72 2074 6865 2063  is set for the c
-00018770: 6f6e 7472 6f6c 6c65 7229 2062 6566 6f72  ontroller) befor
-00018780: 6520 7468 6520 6a6f 6273 2f73 6572 7665  e the jobs/serve
-00018790: 2063 6f6d 6d61 6e64 7320 696e 7465 7261   commands intera
-000187a0: 6374 2077 6974 6820 7468 650a 2020 2020  ct with the.    
-000187b0: 636f 6e74 726f 6c6c 6572 2e0a 0a20 2020  controller...   
-000187c0: 2043 6c75 7374 6572 4e6f 7455 7045 7272   ClusterNotUpErr
-000187d0: 6f72 2077 696c 6c20 6265 2072 6169 7365  or will be raise
-000187e0: 6420 7768 656e 6576 6572 2074 6865 2063  d whenever the c
-000187f0: 6f6e 7472 6f6c 6c65 7220 6361 6e6e 6f74  ontroller cannot
-00018800: 2062 6520 6163 6365 7373 6564 2e0a 0a20   be accessed... 
-00018810: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00018820: 2074 7970 653a 2054 7970 6520 6f66 2074   type: Type of t
-00018830: 6865 2063 6f6e 7472 6f6c 6c65 722e 0a20  he controller.. 
-00018840: 2020 2020 2020 2073 746f 7070 6564 5f6d         stopped_m
-00018850: 6573 7361 6765 3a20 4d65 7373 6167 6520  essage: Message 
-00018860: 746f 2070 7269 6e74 2069 6620 7468 6520  to print if the 
-00018870: 636f 6e74 726f 6c6c 6572 2069 7320 5354  controller is ST
-00018880: 4f50 5045 442e 0a20 2020 2020 2020 206e  OPPED..        n
-00018890: 6f6e 5f65 7869 7374 656e 745f 6d65 7373  on_existent_mess
-000188a0: 6167 653a 204d 6573 7361 6765 2074 6f20  age: Message to 
-000188b0: 7368 6f77 2069 6620 7468 6520 636f 6e74  show if the cont
-000188c0: 726f 6c6c 6572 2064 6f65 7320 6e6f 7420  roller does not 
-000188d0: 6578 6973 742e 0a20 2020 2020 2020 2065  exist..        e
-000188e0: 7869 745f 6966 5f6e 6f74 5f61 6363 6573  xit_if_not_acces
-000188f0: 7369 626c 653a 2057 6865 7468 6572 2074  sible: Whether t
-00018900: 6f20 6578 6974 2064 6972 6563 746c 7920  o exit directly 
-00018910: 6966 2074 6865 2063 6f6e 7472 6f6c 6c65  if the controlle
-00018920: 7220 6973 206e 6f74 0a20 2020 2020 2020  r is not.       
-00018930: 2020 2061 6363 6573 7369 626c 652e 2049     accessible. I
-00018940: 6620 4661 6c73 652c 2074 6865 2066 756e  f False, the fun
-00018950: 6374 696f 6e20 7769 6c6c 2072 6169 7365  ction will raise
-00018960: 2043 6c75 7374 6572 4e6f 7455 7045 7272   ClusterNotUpErr
-00018970: 6f72 2e0a 0a20 2020 2052 6574 7572 6e73  or...    Returns
-00018980: 3a0a 2020 2020 2020 2020 6861 6e64 6c65  :.        handle
-00018990: 3a20 5468 6520 5265 736f 7572 6365 4861  : The ResourceHa
-000189a0: 6e64 6c65 206f 6620 7468 6520 636f 6e74  ndle of the cont
-000189b0: 726f 6c6c 6572 2e0a 0a20 2020 2052 6169  roller...    Rai
-000189c0: 7365 733a 0a20 2020 2020 2020 2065 7863  ses:.        exc
-000189d0: 6570 7469 6f6e 732e 436c 7573 7465 724f  eptions.ClusterO
-000189e0: 776e 6572 4964 656e 7469 7479 4d69 736d  wnerIdentityMism
-000189f0: 6174 6368 4572 726f 723a 2069 6620 7468  atchError: if th
-00018a00: 6520 6375 7272 656e 7420 7573 6572 2069  e current user i
-00018a10: 7320 6e6f 740a 2020 2020 2020 2020 2020  s not.          
-00018a20: 7468 6520 7361 6d65 2061 7320 7468 6520  the same as the 
-00018a30: 7573 6572 2077 686f 2063 7265 6174 6564  user who created
-00018a40: 2074 6865 2063 6c75 7374 6572 2e0a 2020   the cluster..  
-00018a50: 2020 2020 2020 6578 6365 7074 696f 6e73        exceptions
-00018a60: 2e43 6c6f 7564 5573 6572 4964 656e 7469  .CloudUserIdenti
-00018a70: 7479 4572 726f 723a 2069 6620 7765 2066  tyError: if we f
-00018a80: 6169 6c20 746f 2067 6574 2074 6865 2063  ail to get the c
-00018a90: 7572 7265 6e74 2075 7365 720a 2020 2020  urrent user.    
-00018aa0: 2020 2020 2020 6964 656e 7469 7479 2e0a        identity..
-00018ab0: 2020 2020 2020 2020 6578 6365 7074 696f          exceptio
-00018ac0: 6e73 2e43 6c75 7374 6572 4e6f 7455 7045  ns.ClusterNotUpE
-00018ad0: 7272 6f72 3a20 6966 2074 6865 2063 6f6e  rror: if the con
-00018ae0: 7472 6f6c 6c65 7220 6973 206e 6f74 2061  troller is not a
-00018af0: 6363 6573 7369 626c 652c 206f 720a 2020  ccessible, or.  
-00018b00: 2020 2020 2020 2020 6661 696c 6564 2074          failed t
-00018b10: 6f20 6265 2063 6f6e 6e65 6374 6564 2e0a  o be connected..
-00018b20: 2020 2020 2222 220a 2020 2020 6966 206e      """.    if n
-00018b30: 6f6e 5f65 7869 7374 656e 745f 6d65 7373  on_existent_mess
-00018b40: 6167 6520 6973 204e 6f6e 653a 0a20 2020  age is None:.   
-00018b50: 2020 2020 206e 6f6e 5f65 7869 7374 656e       non_existen
-00018b60: 745f 6d65 7373 6167 6520 3d20 636f 6e74  t_message = cont
-00018b70: 726f 6c6c 6572 2e76 616c 7565 2e64 6566  roller.value.def
-00018b80: 6175 6c74 5f68 696e 745f 6966 5f6e 6f6e  ault_hint_if_non
-00018b90: 5f65 7869 7374 656e 740a 2020 2020 636c  _existent.    cl
-00018ba0: 7573 7465 725f 6e61 6d65 203d 2063 6f6e  uster_name = con
-00018bb0: 7472 6f6c 6c65 722e 7661 6c75 652e 636c  troller.value.cl
-00018bc0: 7573 7465 725f 6e61 6d65 0a20 2020 206e  uster_name.    n
-00018bd0: 6565 645f 636f 6e6e 6563 7469 6f6e 5f63  eed_connection_c
-00018be0: 6865 636b 203d 2046 616c 7365 0a20 2020  heck = False.   
-00018bf0: 2063 6f6e 7472 6f6c 6c65 725f 7374 6174   controller_stat
-00018c00: 7573 2c20 6861 6e64 6c65 203d 204e 6f6e  us, handle = Non
-00018c10: 652c 204e 6f6e 650a 2020 2020 7472 793a  e, None.    try:
-00018c20: 0a20 2020 2020 2020 2023 2053 6574 2066  .        # Set f
-00018c30: 6f72 6365 5f72 6566 7265 7368 5f73 7461  orce_refresh_sta
-00018c40: 7475 7365 733d 5b49 4e49 545d 2074 6f20  tuses=[INIT] to 
-00018c50: 6d61 6b65 2073 7572 6520 7468 6520 7265  make sure the re
-00018c60: 6672 6573 6820 6861 7070 656e 730a 2020  fresh happens.  
-00018c70: 2020 2020 2020 2320 7768 656e 2074 6865        # when the
-00018c80: 2063 6f6e 7472 6f6c 6c65 7220 6973 2049   controller is I
-00018c90: 4e49 542f 5550 2028 7472 6967 6765 7265  NIT/UP (triggere
-00018ca0: 6420 696e 2074 6865 7365 2073 7461 7475  d in these statu
-00018cb0: 7365 7320 6173 2074 6865 0a20 2020 2020  ses as the.     
-00018cc0: 2020 2023 2061 7574 6f73 746f 7020 6973     # autostop is
-00018cd0: 2061 6c77 6179 7320 7365 7420 666f 7220   always set for 
-00018ce0: 7468 6520 636f 6e74 726f 6c6c 6572 292e  the controller).
-00018cf0: 2054 6865 2063 6f6e 7472 6f6c 6c65 7220   The controller 
-00018d00: 6361 6e20 6265 2069 6e0a 2020 2020 2020  can be in.      
-00018d10: 2020 2320 666f 6c6c 6f77 696e 6720 6361    # following ca
-00018d20: 7365 733a 0a20 2020 2020 2020 2023 202a  ses:.        # *
-00018d30: 2028 5550 2c20 6175 746f 7374 6f70 2073   (UP, autostop s
-00018d40: 6574 293a 2069 7420 7769 6c6c 2062 6520  et): it will be 
-00018d50: 7265 6672 6573 6865 6420 7769 7468 6f75  refreshed withou
-00018d60: 7420 666f 7263 655f 7265 6672 6573 6820  t force_refresh 
-00018d70: 7365 742e 0a20 2020 2020 2020 2023 202a  set..        # *
-00018d80: 2028 5550 2c20 6e6f 2061 7574 6f73 746f   (UP, no autosto
-00018d90: 7029 3a20 7665 7279 2072 6172 6520 2861  p): very rare (a
-00018da0: 2075 7365 7220 6374 726c 2d63 2077 6865   user ctrl-c whe
-00018db0: 6e20 7468 6520 636f 6e74 726f 6c6c 6572  n the controller
-00018dc0: 2069 730a 2020 2020 2020 2020 2320 2020   is.        #   
-00018dd0: 6c61 756e 6368 696e 6729 2c20 646f 6573  launching), does
-00018de0: 206e 6f74 206d 6174 7465 7220 6966 2072   not matter if r
-00018df0: 6566 7265 7368 206f 7220 6e6f 742c 2073  efresh or not, s
-00018e00: 696e 6365 206e 6f20 6175 746f 7374 6f70  ince no autostop
-00018e10: 2e20 5765 0a20 2020 2020 2020 2023 2020  . We.        #  
-00018e20: 2064 6f6e 2774 2069 6e63 6c75 6465 2055   don't include U
-00018e30: 5020 696e 2066 6f72 6365 5f72 6566 7265  P in force_refre
-00018e40: 7368 5f73 7461 7475 7365 7320 746f 2061  sh_statuses to a
-00018e50: 766f 6964 206f 7665 7268 6561 6473 2e0a  void overheads..
-00018e60: 2020 2020 2020 2020 2320 2a20 2849 4e49          # * (INI
-00018e70: 542c 2061 7574 6f73 746f 7020 7365 7429  T, autostop set)
-00018e80: 0a20 2020 2020 2020 2023 202a 2028 494e  .        # * (IN
-00018e90: 4954 2c20 6e6f 2061 7574 6f73 746f 7029  IT, no autostop)
-00018ea0: 3a20 7665 7279 2072 6172 6520 285f 7570  : very rare (_up
-00018eb0: 6461 7465 5f63 6c75 7374 6572 5f73 7461  date_cluster_sta
-00018ec0: 7475 735f 6e6f 5f6c 6f63 6b20 6d61 790a  tus_no_lock may.
-00018ed0: 2020 2020 2020 2020 2320 2020 7265 7365          #   rese
-00018ee0: 7420 6c6f 6361 6c20 6175 746f 7374 6f70  t local autostop
-00018ef0: 2063 6f6e 6669 6729 2c20 6275 7420 666f   config), but fo
-00018f00: 7263 655f 7265 6672 6573 6820 7769 6c6c  rce_refresh will
-00018f10: 206d 616b 6520 7375 7265 0a20 2020 2020   make sure.     
-00018f20: 2020 2023 2020 2073 7461 7475 7320 6973     #   status is
-00018f30: 2072 6566 7265 7368 6564 2e0a 2020 2020   refreshed..    
-00018f40: 2020 2020 230a 2020 2020 2020 2020 2320      #.        # 
-00018f50: 5765 2061 766f 6964 7320 756e 6e65 6365  We avoids unnece
-00018f60: 7373 6172 7920 636f 7374 6c79 2072 6566  ssary costly ref
-00018f70: 7265 7368 2077 6865 6e20 7468 6520 636f  resh when the co
-00018f80: 6e74 726f 6c6c 6572 2069 7320 616c 7265  ntroller is alre
-00018f90: 6164 790a 2020 2020 2020 2020 2320 5354  ady.        # ST
-00018fa0: 4f50 5045 442e 2054 6869 7320 6f70 7469  OPPED. This opti
-00018fb0: 6d69 7a61 7469 6f6e 2069 7320 6261 7365  mization is base
-00018fc0: 6420 6f6e 2074 6865 2061 7373 756d 7074  d on the assumpt
-00018fd0: 696f 6e20 7468 6174 2074 6865 2075 7365  ion that the use
-00018fe0: 720a 2020 2020 2020 2020 2320 7769 6c6c  r.        # will
-00018ff0: 206e 6f74 2073 7461 7274 2074 6865 2063   not start the c
-00019000: 6f6e 7472 6f6c 6c65 7220 6d61 6e75 616c  ontroller manual
-00019010: 6c79 2066 726f 6d20 7468 6520 636c 6f75  ly from the clou
-00019020: 6420 636f 6e73 6f6c 652e 0a20 2020 2020  d console..     
-00019030: 2020 2023 0a20 2020 2020 2020 2023 2054     #.        # T
-00019040: 6865 2061 6371 7569 7265 5f6c 6f63 6b5f  he acquire_lock_
-00019050: 7469 6d65 6f75 7420 6973 2073 6574 2074  timeout is set t
-00019060: 6f20 3020 746f 2061 766f 6964 2068 616e  o 0 to avoid han
-00019070: 6769 6e67 2074 6865 2063 6f6d 6d61 6e64  ging the command
-00019080: 2077 6865 6e0a 2020 2020 2020 2020 2320   when.        # 
-00019090: 6d75 6c74 6970 6c65 206a 6f62 732e 6c61  multiple jobs.la
-000190a0: 756e 6368 2063 6f6d 6d61 6e64 7320 6172  unch commands ar
-000190b0: 6520 7275 6e6e 696e 6720 6174 2074 6865  e running at the
-000190c0: 2073 616d 6520 7469 6d65 2e20 4f75 7220   same time. Our 
-000190d0: 6c61 7465 720a 2020 2020 2020 2020 2320  later.        # 
-000190e0: 636f 6465 2077 696c 6c20 6368 6563 6b20  code will check 
-000190f0: 6966 2074 6865 2063 6f6e 7472 6f6c 6c65  if the controlle
-00019100: 7220 6973 2061 6363 6573 7369 626c 6520  r is accessible 
-00019110: 6279 2064 6972 6563 746c 7920 6368 6563  by directly chec
-00019120: 6b69 6e67 0a20 2020 2020 2020 2023 2074  king.        # t
-00019130: 6865 2073 7368 2063 6f6e 6e65 6374 696f  he ssh connectio
-00019140: 6e20 746f 2074 6865 2063 6f6e 7472 6f6c  n to the control
-00019150: 6c65 722c 2069 6620 6974 2066 6169 6c73  ler, if it fails
-00019160: 2074 6f20 6765 7420 6163 6375 7261 7465   to get accurate
-00019170: 0a20 2020 2020 2020 2023 2073 7461 7475  .        # statu
-00019180: 7320 6f66 2074 6865 2063 6f6e 7472 6f6c  s of the control
-00019190: 6c65 722e 0a20 2020 2020 2020 2063 6f6e  ler..        con
-000191a0: 7472 6f6c 6c65 725f 7374 6174 7573 2c20  troller_status, 
-000191b0: 6861 6e64 6c65 203d 2072 6566 7265 7368  handle = refresh
-000191c0: 5f63 6c75 7374 6572 5f73 7461 7475 735f  _cluster_status_
-000191d0: 6861 6e64 6c65 280a 2020 2020 2020 2020  handle(.        
-000191e0: 2020 2020 636c 7573 7465 725f 6e61 6d65      cluster_name
-000191f0: 2c0a 2020 2020 2020 2020 2020 2020 666f  ,.            fo
-00019200: 7263 655f 7265 6672 6573 685f 7374 6174  rce_refresh_stat
-00019210: 7573 6573 3d5b 7374 6174 7573 5f6c 6962  uses=[status_lib
-00019220: 2e43 6c75 7374 6572 5374 6174 7573 2e49  .ClusterStatus.I
-00019230: 4e49 545d 2c0a 2020 2020 2020 2020 2020  NIT],.          
-00019240: 2020 636c 7573 7465 725f 7374 6174 7573    cluster_status
-00019250: 5f6c 6f63 6b5f 7469 6d65 6f75 743d 3029  _lock_timeout=0)
-00019260: 0a20 2020 2065 7863 6570 7420 6578 6365  .    except exce
-00019270: 7074 696f 6e73 2e43 6c75 7374 6572 5374  ptions.ClusterSt
-00019280: 6174 7573 4665 7463 6869 6e67 4572 726f  atusFetchingErro
-00019290: 7220 6173 2065 3a0a 2020 2020 2020 2020  r as e:.        
-000192a0: 2320 5765 2064 6f20 6e6f 7420 6361 7463  # We do not catc
-000192b0: 6820 7468 6520 6578 6365 7074 696f 6e73  h the exceptions
-000192c0: 2072 656c 6174 6564 2074 6f20 7468 6520   related to the 
-000192d0: 636c 7573 7465 7220 6f77 6e65 7220 6964  cluster owner id
-000192e0: 656e 7469 7479 0a20 2020 2020 2020 2023  entity.        #
-000192f0: 206d 6973 6d61 7463 682c 2070 6c65 6173   mismatch, pleas
-00019300: 6520 7265 6665 7220 746f 2074 6865 2063  e refer to the c
-00019310: 6f6d 6d65 6e74 2069 6e0a 2020 2020 2020  omment in.      
-00019320: 2020 2320 6062 6163 6b65 6e64 5f75 7469    # `backend_uti
-00019330: 6c73 2e63 6865 636b 5f63 6c75 7374 6572  ls.check_cluster
-00019340: 5f61 7661 696c 6162 6c65 602e 0a20 2020  _available`..   
-00019350: 2020 2020 2063 6f6e 7472 6f6c 6c65 725f       controller_
-00019360: 6e61 6d65 203d 2063 6f6e 7472 6f6c 6c65  name = controlle
-00019370: 722e 7661 6c75 652e 6e61 6d65 2e72 6570  r.value.name.rep
-00019380: 6c61 6365 2827 2063 6f6e 7472 6f6c 6c65  lace(' controlle
-00019390: 7227 2c20 2727 290a 2020 2020 2020 2020  r', '').        
-000193a0: 6c6f 6767 6572 2e77 6172 6e69 6e67 280a  logger.warning(.
-000193b0: 2020 2020 2020 2020 2020 2020 2746 6169              'Fai
-000193c0: 6c65 6420 746f 2067 6574 2074 6865 2073  led to get the s
-000193d0: 7461 7475 7320 6f66 2074 6865 2063 6f6e  tatus of the con
-000193e0: 7472 6f6c 6c65 722e 2049 7420 6973 206e  troller. It is n
-000193f0: 6f74 2027 0a20 2020 2020 2020 2020 2020  ot '.           
-00019400: 2066 2766 6174 616c 2c20 6275 7420 7b63   f'fatal, but {c
-00019410: 6f6e 7472 6f6c 6c65 725f 6e61 6d65 7d20  ontroller_name} 
-00019420: 636f 6d6d 616e 6473 2f63 616c 6c73 206d  commands/calls m
-00019430: 6179 2068 616e 6720 6f72 2072 6574 7572  ay hang or retur
-00019440: 6e20 270a 2020 2020 2020 2020 2020 2020  n '.            
-00019450: 2773 7461 6c65 2069 6e66 6f72 6d61 7469  'stale informati
-00019460: 6f6e 2c20 7768 656e 2074 6865 2063 6f6e  on, when the con
-00019470: 7472 6f6c 6c65 7220 6973 206e 6f74 2075  troller is not u
-00019480: 702e 5c6e 270a 2020 2020 2020 2020 2020  p.\n'.          
-00019490: 2020 6627 2020 4465 7461 696c 733a 207b    f'  Details: {
-000194a0: 636f 6d6d 6f6e 5f75 7469 6c73 2e66 6f72  common_utils.for
-000194b0: 6d61 745f 6578 6365 7074 696f 6e28 652c  mat_exception(e,
-000194c0: 2075 7365 5f62 7261 636b 6574 3d54 7275   use_bracket=Tru
-000194d0: 6529 7d27 290a 2020 2020 2020 2020 7265  e)}').        re
-000194e0: 636f 7264 203d 2067 6c6f 6261 6c5f 7573  cord = global_us
-000194f0: 6572 5f73 7461 7465 2e67 6574 5f63 6c75  er_state.get_clu
-00019500: 7374 6572 5f66 726f 6d5f 6e61 6d65 2863  ster_from_name(c
-00019510: 6c75 7374 6572 5f6e 616d 6529 0a20 2020  luster_name).   
-00019520: 2020 2020 2069 6620 7265 636f 7264 2069       if record i
-00019530: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00019540: 2020 2020 2020 2020 636f 6e74 726f 6c6c          controll
-00019550: 6572 5f73 7461 7475 732c 2068 616e 646c  er_status, handl
-00019560: 6520 3d20 7265 636f 7264 5b27 7374 6174  e = record['stat
-00019570: 7573 275d 2c20 7265 636f 7264 5b27 6861  us'], record['ha
-00019580: 6e64 6c65 275d 0a20 2020 2020 2020 2020  ndle'].         
-00019590: 2020 2023 2057 6520 6368 6563 6b20 7468     # We check th
-000195a0: 6520 636f 6e6e 6563 7469 6f6e 2065 7665  e connection eve
-000195b0: 6e20 6966 2074 6865 2063 6c75 7374 6572  n if the cluster
-000195c0: 2068 6173 2061 2063 6163 6865 6420 7374   has a cached st
-000195d0: 6174 7573 2055 500a 2020 2020 2020 2020  atus UP.        
-000195e0: 2020 2020 2320 746f 206d 616b 6520 7375      # to make su
-000195f0: 7265 2074 6865 2063 6f6e 7472 6f6c 6c65  re the controlle
-00019600: 7220 6973 2061 6374 7561 6c6c 7920 6163  r is actually ac
-00019610: 6365 7373 6962 6c65 2c20 6173 2074 6865  cessible, as the
-00019620: 2063 6163 6865 640a 2020 2020 2020 2020   cached.        
-00019630: 2020 2020 2320 7374 6174 7573 206d 6967      # status mig
-00019640: 6874 2062 6520 7374 616c 652e 0a20 2020  ht be stale..   
-00019650: 2020 2020 2020 2020 206e 6565 645f 636f           need_co
-00019660: 6e6e 6563 7469 6f6e 5f63 6865 636b 203d  nnection_check =
-00019670: 2054 7275 650a 0a20 2020 2065 7272 6f72   True..    error
-00019680: 5f6d 7367 203d 204e 6f6e 650a 2020 2020  _msg = None.    
-00019690: 6966 2063 6f6e 7472 6f6c 6c65 725f 7374  if controller_st
-000196a0: 6174 7573 203d 3d20 7374 6174 7573 5f6c  atus == status_l
-000196b0: 6962 2e43 6c75 7374 6572 5374 6174 7573  ib.ClusterStatus
-000196c0: 2e53 544f 5050 4544 3a0a 2020 2020 2020  .STOPPED:.      
-000196d0: 2020 6572 726f 725f 6d73 6720 3d20 7374    error_msg = st
-000196e0: 6f70 7065 645f 6d65 7373 6167 650a 2020  opped_message.  
-000196f0: 2020 656c 6966 2063 6f6e 7472 6f6c 6c65    elif controlle
-00019700: 725f 7374 6174 7573 2069 7320 4e6f 6e65  r_status is None
-00019710: 206f 7220 6861 6e64 6c65 2069 7320 4e6f   or handle is No
-00019720: 6e65 206f 7220 6861 6e64 6c65 2e68 6561  ne or handle.hea
-00019730: 645f 6970 2069 7320 4e6f 6e65 3a0a 2020  d_ip is None:.  
-00019740: 2020 2020 2020 2320 5765 2063 6865 636b        # We check
-00019750: 2074 6865 2063 6f6e 7472 6f6c 6c65 7220   the controller 
-00019760: 6973 2053 544f 5050 4544 2062 6566 6f72  is STOPPED befor
-00019770: 6520 7468 6520 6368 6563 6b20 666f 7220  e the check for 
-00019780: 6861 6e64 6c65 2e68 6561 645f 6970 0a20  handle.head_ip. 
-00019790: 2020 2020 2020 2023 204e 6f6e 6520 6265         # None be
-000197a0: 6361 7573 6520 7768 656e 2074 6865 2063  cause when the c
-000197b0: 6f6e 7472 6f6c 6c65 7220 6973 2053 544f  ontroller is STO
-000197c0: 5050 4544 2c20 6861 6e64 6c65 2e68 6561  PPED, handle.hea
-000197d0: 645f 6970 2063 616e 2061 6c73 6f0a 2020  d_ip can also.  
-000197e0: 2020 2020 2020 2320 6265 204e 6f6e 652c        # be None,
-000197f0: 2062 7574 2077 6520 6f6e 6c79 2077 616e   but we only wan
-00019800: 7420 746f 2063 6174 6368 2074 6865 2063  t to catch the c
-00019810: 6173 6520 7768 656e 2074 6865 2063 6f6e  ase when the con
-00019820: 7472 6f6c 6c65 7220 6973 0a20 2020 2020  troller is.     
-00019830: 2020 2023 2062 6569 6e67 2070 726f 7669     # being provi
-00019840: 7369 6f6e 6564 2061 7420 7468 6520 6669  sioned at the fi
-00019850: 7273 7420 7469 6d65 2061 6e64 2068 6176  rst time and hav
-00019860: 6520 6e6f 2068 6561 645f 6970 2e0a 2020  e no head_ip..  
-00019870: 2020 2020 2020 6572 726f 725f 6d73 6720        error_msg 
-00019880: 3d20 6e6f 6e5f 6578 6973 7465 6e74 5f6d  = non_existent_m
-00019890: 6573 7361 6765 0a20 2020 2065 6c69 6620  essage.    elif 
-000198a0: 2863 6f6e 7472 6f6c 6c65 725f 7374 6174  (controller_stat
-000198b0: 7573 203d 3d20 7374 6174 7573 5f6c 6962  us == status_lib
-000198c0: 2e43 6c75 7374 6572 5374 6174 7573 2e49  .ClusterStatus.I
-000198d0: 4e49 5420 6f72 0a20 2020 2020 2020 2020  NIT or.         
-000198e0: 206e 6565 645f 636f 6e6e 6563 7469 6f6e   need_connection
-000198f0: 5f63 6865 636b 293a 0a20 2020 2020 2020  _check):.       
-00019900: 2023 2043 6865 636b 2073 7368 2063 6f6e   # Check ssh con
-00019910: 6e65 6374 696f 6e20 6966 2028 3129 2063  nection if (1) c
-00019920: 6f6e 7472 6f6c 6c65 7220 6973 2069 6e20  ontroller is in 
-00019930: 494e 4954 2073 7461 7465 2c20 6f72 2028  INIT state, or (
-00019940: 3229 2077 6520 6661 696c 6564 2074 6f20  2) we failed to 
-00019950: 6665 7463 6820 7468 650a 2020 2020 2020  fetch the.      
-00019960: 2020 2320 7374 6174 7573 2c20 626f 7468    # status, both
-00019970: 206f 6620 7768 6963 6820 6361 6e20 6861   of which can ha
-00019980: 7070 656e 2077 6865 6e20 636f 6e74 726f  ppen when contro
-00019990: 6c6c 6572 2773 2073 7461 7475 7320 6c6f  ller's status lo
-000199a0: 636b 2069 7320 6865 6c64 2062 7920 616e  ck is held by an
-000199b0: 6f74 6865 7220 6073 6b79 206a 6f62 7320  other `sky jobs 
-000199c0: 6c61 756e 6368 6020 6f72 0a20 2020 2020  launch` or.     
-000199d0: 2020 2023 2060 736b 7920 7365 7276 6520     # `sky serve 
-000199e0: 7570 602e 2049 6620 7765 2068 6176 65c2  up`. If we have.
-000199f0: a063 6f6e 7472 6f6c 6c65 7227 7320 6865  .controller's he
-00019a00: 6164 5f69 7020 6176 6169 6c61 626c 6520  ad_ip available 
-00019a10: 616e 6420 6974 2069 7320 7373 682d 7265  and it is ssh-re
-00019a20: 6163 6861 626c 652c 0a20 2020 2020 2020  achable,.       
-00019a30: 2023 2077 6520 6361 6e20 616c 6c6f 7720   # we can allow 
-00019a40: 6163 6365 7373 2074 6f20 7468 6520 636f  access to the co
-00019a50: 6e74 726f 6c6c 6572 2e0a 2020 2020 2020  ntroller..      
-00019a60: 2020 7373 685f 6372 6564 656e 7469 616c    ssh_credential
-00019a70: 7320 3d20 7373 685f 6372 6564 656e 7469  s = ssh_credenti
-00019a80: 616c 5f66 726f 6d5f 7961 6d6c 2868 616e  al_from_yaml(han
-00019a90: 646c 652e 636c 7573 7465 725f 7961 6d6c  dle.cluster_yaml
-00019aa0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00019ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015740: 2020 2020 2020 2020 2072 6561 6479 3d46           ready=F
+00015750: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
+00015760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015780: 2020 2020 2020 6973 5f6c 6175 6e63 683d        is_launch=
+00015790: 4661 6c73 6529 0a20 2020 2020 2020 2072  False).        r
+000157a0: 6574 7572 6e20 676c 6f62 616c 5f75 7365  eturn global_use
+000157b0: 725f 7374 6174 652e 6765 745f 636c 7573  r_state.get_clus
+000157c0: 7465 725f 6672 6f6d 5f6e 616d 6528 636c  ter_from_name(cl
+000157d0: 7573 7465 725f 6e61 6d65 290a 2020 2020  uster_name).    
+000157e0: 2320 4e6f 7720 6973 5f61 626e 6f72 6d61  # Now is_abnorma
+000157f0: 6c20 6973 2046 616c 7365 3a20 6569 7468  l is False: eith
+00015800: 6572 206e 6f64 655f 7374 6174 7573 6573  er node_statuses
+00015810: 2069 7320 656d 7074 7920 6f72 2061 6c6c   is empty or all
+00015820: 206e 6f64 6573 2061 7265 0a20 2020 2023   nodes are.    #
+00015830: 2053 544f 5050 4544 2e0a 2020 2020 6261   STOPPED..    ba
+00015840: 636b 656e 6420 3d20 6261 636b 656e 6473  ckend = backends
+00015850: 2e43 6c6f 7564 566d 5261 7942 6163 6b65  .CloudVmRayBacke
+00015860: 6e64 2829 0a20 2020 2062 6163 6b65 6e64  nd().    backend
+00015870: 2e70 6f73 745f 7465 6172 646f 776e 5f63  .post_teardown_c
+00015880: 6c65 616e 7570 2868 616e 646c 652c 2074  leanup(handle, t
+00015890: 6572 6d69 6e61 7465 3d74 6f5f 7465 726d  erminate=to_term
+000158a0: 696e 6174 652c 2070 7572 6765 3d46 616c  inate, purge=Fal
+000158b0: 7365 290a 2020 2020 7265 7475 726e 2067  se).    return g
+000158c0: 6c6f 6261 6c5f 7573 6572 5f73 7461 7465  lobal_user_state
+000158d0: 2e67 6574 5f63 6c75 7374 6572 5f66 726f  .get_cluster_fro
+000158e0: 6d5f 6e61 6d65 2863 6c75 7374 6572 5f6e  m_name(cluster_n
+000158f0: 616d 6529 0a0a 0a64 6566 205f 7570 6461  ame)...def _upda
+00015900: 7465 5f63 6c75 7374 6572 5f73 7461 7475  te_cluster_statu
+00015910: 7328 0a20 2020 2063 6c75 7374 6572 5f6e  s(.    cluster_n
+00015920: 616d 653a 2073 7472 2c0a 2020 2020 6163  ame: str,.    ac
+00015930: 7175 6972 655f 7065 725f 636c 7573 7465  quire_per_cluste
+00015940: 725f 7374 6174 7573 5f6c 6f63 6b3a 2062  r_status_lock: b
+00015950: 6f6f 6c2c 0a20 2020 2063 6c75 7374 6572  ool,.    cluster
+00015960: 5f73 7461 7475 735f 6c6f 636b 5f74 696d  _status_lock_tim
+00015970: 656f 7574 3a20 696e 7420 3d20 434c 5553  eout: int = CLUS
+00015980: 5445 525f 5354 4154 5553 5f4c 4f43 4b5f  TER_STATUS_LOCK_
+00015990: 5449 4d45 4f55 545f 5345 434f 4e44 530a  TIMEOUT_SECONDS.
+000159a0: 2920 2d3e 204f 7074 696f 6e61 6c5b 4469  ) -> Optional[Di
+000159b0: 6374 5b73 7472 2c20 416e 795d 5d3a 0a20  ct[str, Any]]:. 
+000159c0: 2020 2022 2222 5570 6461 7465 2074 6865     """Update the
+000159d0: 2063 6c75 7374 6572 2073 7461 7475 732e   cluster status.
+000159e0: 0a0a 2020 2020 5468 6520 636c 7573 7465  ..    The cluste
+000159f0: 7220 7374 6174 7573 2069 7320 7570 6461  r status is upda
+00015a00: 7465 6420 6279 2063 6865 636b 696e 6720  ted by checking 
+00015a10: 7261 7920 636c 7573 7465 7220 616e 6420  ray cluster and 
+00015a20: 7265 616c 2073 7461 7475 7320 6672 6f6d  real status from
+00015a30: 0a20 2020 2063 6c6f 7564 2e0a 0a20 2020  .    cloud...   
+00015a40: 2054 6865 2066 756e 6374 696f 6e20 7769   The function wi
+00015a50: 6c6c 2075 7064 6174 6520 7468 6520 6361  ll update the ca
+00015a60: 6368 6564 2063 6c75 7374 6572 2073 7461  ched cluster sta
+00015a70: 7475 7320 696e 2074 6865 2067 6c6f 6261  tus in the globa
+00015a80: 6c20 7374 6174 652e 2046 6f72 0a20 2020  l state. For.   
+00015a90: 2074 6865 2064 6573 6967 6e20 6f66 2074   the design of t
+00015aa0: 6865 2063 6c75 7374 6572 2073 7461 7475  he cluster statu
+00015ab0: 7320 616e 6420 7472 616e 7369 7469 6f6e  s and transition
+00015ac0: 2c20 706c 6561 7365 2072 6566 6572 2074  , please refer t
+00015ad0: 6f20 7468 650a 2020 2020 736b 792f 6465  o the.    sky/de
+00015ae0: 7369 676e 5f64 6f63 732f 636c 7573 7465  sign_docs/cluste
+00015af0: 725f 7374 6174 7573 2e6d 640a 0a20 2020  r_status.md..   
+00015b00: 2041 7267 733a 0a20 2020 2020 2020 2063   Args:.        c
+00015b10: 6c75 7374 6572 5f6e 616d 653a 2054 6865  luster_name: The
+00015b20: 206e 616d 6520 6f66 2074 6865 2063 6c75   name of the clu
+00015b30: 7374 6572 2e0a 2020 2020 2020 2020 6163  ster..        ac
+00015b40: 7175 6972 655f 7065 725f 636c 7573 7465  quire_per_cluste
+00015b50: 725f 7374 6174 7573 5f6c 6f63 6b3a 2057  r_status_lock: W
+00015b60: 6865 7468 6572 2074 6f20 6163 7175 6972  hether to acquir
+00015b70: 6520 7468 6520 7065 722d 636c 7573 7465  e the per-cluste
+00015b80: 7220 6c6f 636b 0a20 2020 2020 2020 2020  r lock.         
+00015b90: 2062 6566 6f72 6520 7570 6461 7469 6e67   before updating
+00015ba0: 2074 6865 2073 7461 7475 732e 0a20 2020   the status..   
+00015bb0: 2020 2020 2063 6c75 7374 6572 5f73 7461       cluster_sta
+00015bc0: 7475 735f 6c6f 636b 5f74 696d 656f 7574  tus_lock_timeout
+00015bd0: 3a20 5468 6520 7469 6d65 6f75 7420 746f  : The timeout to
+00015be0: 2061 6371 7569 7265 2074 6865 2070 6572   acquire the per
+00015bf0: 2d63 6c75 7374 6572 0a20 2020 2020 2020  -cluster.       
+00015c00: 2020 206c 6f63 6b2e 0a0a 2020 2020 5265     lock...    Re
+00015c10: 7475 726e 733a 0a20 2020 2020 2020 2049  turns:.        I
+00015c20: 6620 7468 6520 636c 7573 7465 7220 6973  f the cluster is
+00015c30: 2074 6572 6d69 6e61 7465 6420 6f72 2064   terminated or d
+00015c40: 6f65 7320 6e6f 7420 6578 6973 742c 2072  oes not exist, r
+00015c50: 6574 7572 6e20 4e6f 6e65 2e20 4f74 6865  eturn None. Othe
+00015c60: 7277 6973 650a 2020 2020 2020 2020 7265  rwise.        re
+00015c70: 7475 726e 7320 7468 6520 696e 7075 7420  turns the input 
+00015c80: 7265 636f 7264 2077 6974 6820 7374 6174  record with stat
+00015c90: 7573 2061 6e64 2068 616e 646c 6520 706f  us and handle po
+00015ca0: 7465 6e74 6961 6c6c 7920 7570 6461 7465  tentially update
+00015cb0: 642e 0a0a 2020 2020 5261 6973 6573 3a0a  d...    Raises:.
+00015cc0: 2020 2020 2020 2020 6578 6365 7074 696f          exceptio
+00015cd0: 6e73 2e43 6c75 7374 6572 4f77 6e65 7249  ns.ClusterOwnerI
+00015ce0: 6465 6e74 6974 794d 6973 6d61 7463 6845  dentityMismatchE
+00015cf0: 7272 6f72 3a20 6966 2074 6865 2063 7572  rror: if the cur
+00015d00: 7265 6e74 2075 7365 7220 6973 0a20 2020  rent user is.   
+00015d10: 2020 2020 2020 206e 6f74 2074 6865 2073         not the s
+00015d20: 616d 6520 6173 2074 6865 2075 7365 7220  ame as the user 
+00015d30: 7768 6f20 6372 6561 7465 6420 7468 6520  who created the 
+00015d40: 636c 7573 7465 722e 0a20 2020 2020 2020  cluster..       
+00015d50: 2065 7863 6570 7469 6f6e 732e 436c 6f75   exceptions.Clou
+00015d60: 6455 7365 7249 6465 6e74 6974 7945 7272  dUserIdentityErr
+00015d70: 6f72 3a20 6966 2077 6520 6661 696c 2074  or: if we fail t
+00015d80: 6f20 6765 7420 7468 6520 6375 7272 656e  o get the curren
+00015d90: 7420 7573 6572 0a20 2020 2020 2020 2020  t user.         
+00015da0: 2069 6465 6e74 6974 792e 0a20 2020 2020   identity..     
+00015db0: 2020 2065 7863 6570 7469 6f6e 732e 436c     exceptions.Cl
+00015dc0: 7573 7465 7253 7461 7475 7346 6574 6368  usterStatusFetch
+00015dd0: 696e 6745 7272 6f72 3a20 7468 6520 636c  ingError: the cl
+00015de0: 7573 7465 7220 7374 6174 7573 2063 616e  uster status can
+00015df0: 6e6f 7420 6265 0a20 2020 2020 2020 2020  not be.         
+00015e00: 2066 6574 6368 6564 2066 726f 6d20 7468   fetched from th
+00015e10: 6520 636c 6f75 6420 7072 6f76 6964 6572  e cloud provider
+00015e20: 206f 7220 7468 6572 6520 6172 6520 6c65   or there are le
+00015e30: 616b 6564 206e 6f64 6573 2063 6175 7369  aked nodes causi
+00015e40: 6e67 0a20 2020 2020 2020 2020 2074 6865  ng.          the
+00015e50: 206e 6f64 6520 6e75 6d62 6572 206c 6172   node number lar
+00015e60: 6765 7220 7468 616e 2065 7870 6563 7465  ger than expecte
+00015e70: 642e 0a20 2020 2022 2222 0a20 2020 2069  d..    """.    i
+00015e80: 6620 6e6f 7420 6163 7175 6972 655f 7065  f not acquire_pe
+00015e90: 725f 636c 7573 7465 725f 7374 6174 7573  r_cluster_status
+00015ea0: 5f6c 6f63 6b3a 0a20 2020 2020 2020 2072  _lock:.        r
+00015eb0: 6574 7572 6e20 5f75 7064 6174 655f 636c  eturn _update_cl
+00015ec0: 7573 7465 725f 7374 6174 7573 5f6e 6f5f  uster_status_no_
+00015ed0: 6c6f 636b 2863 6c75 7374 6572 5f6e 616d  lock(cluster_nam
+00015ee0: 6529 0a0a 2020 2020 7472 793a 0a20 2020  e)..    try:.   
+00015ef0: 2020 2020 2077 6974 6820 6669 6c65 6c6f       with filelo
+00015f00: 636b 2e46 696c 654c 6f63 6b28 434c 5553  ck.FileLock(CLUS
+00015f10: 5445 525f 5354 4154 5553 5f4c 4f43 4b5f  TER_STATUS_LOCK_
+00015f20: 5041 5448 2e66 6f72 6d61 7428 636c 7573  PATH.format(clus
+00015f30: 7465 725f 6e61 6d65 292c 0a20 2020 2020  ter_name),.     
+00015f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015f50: 2020 2020 2020 2020 2020 7469 6d65 6f75            timeou
+00015f60: 743d 636c 7573 7465 725f 7374 6174 7573  t=cluster_status
+00015f70: 5f6c 6f63 6b5f 7469 6d65 6f75 7429 3a0a  _lock_timeout):.
+00015f80: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00015f90: 726e 205f 7570 6461 7465 5f63 6c75 7374  rn _update_clust
+00015fa0: 6572 5f73 7461 7475 735f 6e6f 5f6c 6f63  er_status_no_loc
+00015fb0: 6b28 636c 7573 7465 725f 6e61 6d65 290a  k(cluster_name).
+00015fc0: 2020 2020 6578 6365 7074 2066 696c 656c      except filel
+00015fd0: 6f63 6b2e 5469 6d65 6f75 743a 0a20 2020  ock.Timeout:.   
+00015fe0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+00015ff0: 6728 2752 6566 7265 7368 696e 6720 7374  g('Refreshing st
+00016000: 6174 7573 3a20 4661 696c 6564 2067 6574  atus: Failed get
+00016010: 2074 6865 206c 6f63 6b20 666f 7220 636c   the lock for cl
+00016020: 7573 7465 7220 270a 2020 2020 2020 2020  uster '.        
+00016030: 2020 2020 2020 2020 2020 2020 2066 277b               f'{
+00016040: 636c 7573 7465 725f 6e61 6d65 2172 7d2e  cluster_name!r}.
+00016050: 2055 7369 6e67 2074 6865 2063 6163 6865   Using the cache
+00016060: 6420 7374 6174 7573 2e27 290a 2020 2020  d status.').    
+00016070: 2020 2020 7265 636f 7264 203d 2067 6c6f      record = glo
+00016080: 6261 6c5f 7573 6572 5f73 7461 7465 2e67  bal_user_state.g
+00016090: 6574 5f63 6c75 7374 6572 5f66 726f 6d5f  et_cluster_from_
+000160a0: 6e61 6d65 2863 6c75 7374 6572 5f6e 616d  name(cluster_nam
+000160b0: 6529 0a20 2020 2020 2020 2072 6574 7572  e).        retur
+000160c0: 6e20 7265 636f 7264 0a0a 0a64 6566 2072  n record...def r
+000160d0: 6566 7265 7368 5f63 6c75 7374 6572 5f72  efresh_cluster_r
+000160e0: 6563 6f72 6428 0a20 2020 2063 6c75 7374  ecord(.    clust
+000160f0: 6572 5f6e 616d 653a 2073 7472 2c0a 2020  er_name: str,.  
+00016100: 2020 2a2c 0a20 2020 2066 6f72 6365 5f72    *,.    force_r
+00016110: 6566 7265 7368 5f73 7461 7475 7365 733a  efresh_statuses:
+00016120: 204f 7074 696f 6e61 6c5b 5365 745b 7374   Optional[Set[st
+00016130: 6174 7573 5f6c 6962 2e43 6c75 7374 6572  atus_lib.Cluster
+00016140: 5374 6174 7573 5d5d 203d 204e 6f6e 652c  Status]] = None,
+00016150: 0a20 2020 2061 6371 7569 7265 5f70 6572  .    acquire_per
+00016160: 5f63 6c75 7374 6572 5f73 7461 7475 735f  _cluster_status_
+00016170: 6c6f 636b 3a20 626f 6f6c 203d 2054 7275  lock: bool = Tru
+00016180: 652c 0a20 2020 2063 6c75 7374 6572 5f73  e,.    cluster_s
+00016190: 7461 7475 735f 6c6f 636b 5f74 696d 656f  tatus_lock_timeo
+000161a0: 7574 3a20 696e 7420 3d20 434c 5553 5445  ut: int = CLUSTE
+000161b0: 525f 5354 4154 5553 5f4c 4f43 4b5f 5449  R_STATUS_LOCK_TI
+000161c0: 4d45 4f55 545f 5345 434f 4e44 530a 2920  MEOUT_SECONDS.) 
+000161d0: 2d3e 204f 7074 696f 6e61 6c5b 4469 6374  -> Optional[Dict
+000161e0: 5b73 7472 2c20 416e 795d 5d3a 0a20 2020  [str, Any]]:.   
+000161f0: 2022 2222 5265 6672 6573 6820 7468 6520   """Refresh the 
+00016200: 636c 7573 7465 722c 2061 6e64 2072 6574  cluster, and ret
+00016210: 7572 6e20 7468 6520 706f 7373 6962 6c79  urn the possibly
+00016220: 2075 7064 6174 6564 2072 6563 6f72 642e   updated record.
+00016230: 0a0a 2020 2020 5468 6973 2066 756e 6374  ..    This funct
+00016240: 696f 6e20 7769 6c6c 2061 6c73 6f20 6368  ion will also ch
+00016250: 6563 6b20 7468 6520 6f77 6e65 7220 6964  eck the owner id
+00016260: 656e 7469 7479 206f 6620 7468 6520 636c  entity of the cl
+00016270: 7573 7465 722c 2061 6e64 2072 6169 7365  uster, and raise
+00016280: 0a20 2020 2065 7863 6570 7469 6f6e 7320  .    exceptions 
+00016290: 6966 2074 6865 2063 7572 7265 6e74 2075  if the current u
+000162a0: 7365 7220 6973 206e 6f74 2074 6865 2073  ser is not the s
+000162b0: 616d 6520 6173 2074 6865 2075 7365 7220  ame as the user 
+000162c0: 7768 6f20 6372 6561 7465 6420 7468 650a  who created the.
+000162d0: 2020 2020 636c 7573 7465 722e 0a0a 2020      cluster...  
+000162e0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+000162f0: 636c 7573 7465 725f 6e61 6d65 3a20 5468  cluster_name: Th
+00016300: 6520 6e61 6d65 206f 6620 7468 6520 636c  e name of the cl
+00016310: 7573 7465 722e 0a20 2020 2020 2020 2066  uster..        f
+00016320: 6f72 6365 5f72 6566 7265 7368 5f73 7461  orce_refresh_sta
+00016330: 7475 7365 733a 2069 6620 7370 6563 6966  tuses: if specif
+00016340: 6965 642c 2072 6566 7265 7368 2074 6865  ied, refresh the
+00016350: 2063 6c75 7374 6572 2069 6620 6974 2068   cluster if it h
+00016360: 6173 206f 6e65 206f 660a 2020 2020 2020  as one of.      
+00016370: 2020 2020 7468 6520 7370 6563 6966 6965      the specifie
+00016380: 6420 7374 6174 7573 6573 2e20 4164 6469  d statuses. Addi
+00016390: 7469 6f6e 616c 6c79 2c20 636c 7573 7465  tionally, cluste
+000163a0: 7273 2073 6174 6973 6679 696e 6720 7468  rs satisfying th
+000163b0: 650a 2020 2020 2020 2020 2020 666f 6c6c  e.          foll
+000163c0: 6f77 696e 6720 636f 6e64 6974 696f 6e73  owing conditions
+000163d0: 2077 696c 6c20 616c 7761 7973 2062 6520   will always be 
+000163e0: 7265 6672 6573 6865 6420 6e6f 206d 6174  refreshed no mat
+000163f0: 7465 7220 7468 650a 2020 2020 2020 2020  ter the.        
+00016400: 2020 6172 6775 6d65 6e74 2069 7320 7370    argument is sp
+00016410: 6563 6966 6965 6420 6f72 206e 6f74 3a0a  ecified or not:.
+00016420: 2020 2020 2020 2020 2020 2020 312e 2069              1. i
+00016430: 7320 6120 7370 6f74 2063 6c75 7374 6572  s a spot cluster
+00016440: 2c20 6f72 0a20 2020 2020 2020 2020 2020  , or.           
+00016450: 2032 2e20 6973 2061 206e 6f6e 2d73 706f   2. is a non-spo
+00016460: 7420 636c 7573 7465 722c 2069 7320 6e6f  t cluster, is no
+00016470: 7420 5354 4f50 5045 442c 2061 6e64 2061  t STOPPED, and a
+00016480: 7574 6f73 746f 7020 6973 2073 6574 2e0a  utostop is set..
+00016490: 2020 2020 2020 2020 6163 7175 6972 655f          acquire_
+000164a0: 7065 725f 636c 7573 7465 725f 7374 6174  per_cluster_stat
+000164b0: 7573 5f6c 6f63 6b3a 2057 6865 7468 6572  us_lock: Whether
+000164c0: 2074 6f20 6163 7175 6972 6520 7468 6520   to acquire the 
+000164d0: 7065 722d 636c 7573 7465 7220 6c6f 636b  per-cluster lock
+000164e0: 0a20 2020 2020 2020 2020 2062 6566 6f72  .          befor
+000164f0: 6520 7570 6461 7469 6e67 2074 6865 2073  e updating the s
+00016500: 7461 7475 732e 0a20 2020 2020 2020 2063  tatus..        c
+00016510: 6c75 7374 6572 5f73 7461 7475 735f 6c6f  luster_status_lo
+00016520: 636b 5f74 696d 656f 7574 3a20 5468 6520  ck_timeout: The 
+00016530: 7469 6d65 6f75 7420 746f 2061 6371 7569  timeout to acqui
+00016540: 7265 2074 6865 2070 6572 2d63 6c75 7374  re the per-clust
+00016550: 6572 0a20 2020 2020 2020 2020 206c 6f63  er.          loc
+00016560: 6b2e 2049 6620 7469 6d65 6f75 742c 2074  k. If timeout, t
+00016570: 6865 2066 756e 6374 696f 6e20 7769 6c6c  he function will
+00016580: 2075 7365 2074 6865 2063 6163 6865 6420   use the cached 
+00016590: 7374 6174 7573 2e0a 0a20 2020 2052 6574  status...    Ret
+000165a0: 7572 6e73 3a0a 2020 2020 2020 2020 4966  urns:.        If
+000165b0: 2074 6865 2063 6c75 7374 6572 2069 7320   the cluster is 
+000165c0: 7465 726d 696e 6174 6564 206f 7220 646f  terminated or do
+000165d0: 6573 206e 6f74 2065 7869 7374 2c20 7265  es not exist, re
+000165e0: 7475 726e 204e 6f6e 652e 0a20 2020 2020  turn None..     
+000165f0: 2020 204f 7468 6572 7769 7365 2072 6574     Otherwise ret
+00016600: 7572 6e73 2074 6865 2063 6c75 7374 6572  urns the cluster
+00016610: 2072 6563 6f72 642e 0a0a 2020 2020 5261   record...    Ra
+00016620: 6973 6573 3a0a 2020 2020 2020 2020 6578  ises:.        ex
+00016630: 6365 7074 696f 6e73 2e43 6c75 7374 6572  ceptions.Cluster
+00016640: 4f77 6e65 7249 6465 6e74 6974 794d 6973  OwnerIdentityMis
+00016650: 6d61 7463 6845 7272 6f72 3a20 6966 2074  matchError: if t
+00016660: 6865 2063 7572 7265 6e74 2075 7365 7220  he current user 
+00016670: 6973 0a20 2020 2020 2020 2020 206e 6f74  is.          not
+00016680: 2074 6865 2073 616d 6520 6173 2074 6865   the same as the
+00016690: 2075 7365 7220 7768 6f20 6372 6561 7465   user who create
+000166a0: 6420 7468 6520 636c 7573 7465 722e 0a20  d the cluster.. 
+000166b0: 2020 2020 2020 2065 7863 6570 7469 6f6e         exception
+000166c0: 732e 436c 6f75 6455 7365 7249 6465 6e74  s.CloudUserIdent
+000166d0: 6974 7945 7272 6f72 3a20 6966 2077 6520  ityError: if we 
+000166e0: 6661 696c 2074 6f20 6765 7420 7468 6520  fail to get the 
+000166f0: 6375 7272 656e 7420 7573 6572 0a20 2020  current user.   
+00016700: 2020 2020 2020 2069 6465 6e74 6974 792e         identity.
+00016710: 0a20 2020 2020 2020 2065 7863 6570 7469  .        excepti
+00016720: 6f6e 732e 436c 7573 7465 7253 7461 7475  ons.ClusterStatu
+00016730: 7346 6574 6368 696e 6745 7272 6f72 3a20  sFetchingError: 
+00016740: 7468 6520 636c 7573 7465 7220 7374 6174  the cluster stat
+00016750: 7573 2063 616e 6e6f 7420 6265 0a20 2020  us cannot be.   
+00016760: 2020 2020 2020 2066 6574 6368 6564 2066         fetched f
+00016770: 726f 6d20 7468 6520 636c 6f75 6420 7072  rom the cloud pr
+00016780: 6f76 6964 6572 206f 7220 7468 6572 6520  ovider or there 
+00016790: 6172 6520 6c65 616b 6564 206e 6f64 6573  are leaked nodes
+000167a0: 2063 6175 7369 6e67 0a20 2020 2020 2020   causing.       
+000167b0: 2020 2074 6865 206e 6f64 6520 6e75 6d62     the node numb
+000167c0: 6572 206c 6172 6765 7220 7468 616e 2065  er larger than e
+000167d0: 7870 6563 7465 642e 0a20 2020 2022 2222  xpected..    """
+000167e0: 0a0a 2020 2020 7265 636f 7264 203d 2067  ..    record = g
+000167f0: 6c6f 6261 6c5f 7573 6572 5f73 7461 7465  lobal_user_state
+00016800: 2e67 6574 5f63 6c75 7374 6572 5f66 726f  .get_cluster_fro
+00016810: 6d5f 6e61 6d65 2863 6c75 7374 6572 5f6e  m_name(cluster_n
+00016820: 616d 6529 0a20 2020 2069 6620 7265 636f  ame).    if reco
+00016830: 7264 2069 7320 4e6f 6e65 3a0a 2020 2020  rd is None:.    
+00016840: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
+00016850: 2020 2020 6368 6563 6b5f 6f77 6e65 725f      check_owner_
+00016860: 6964 656e 7469 7479 2863 6c75 7374 6572  identity(cluster
+00016870: 5f6e 616d 6529 0a0a 2020 2020 6861 6e64  _name)..    hand
+00016880: 6c65 203d 2072 6563 6f72 645b 2768 616e  le = record['han
+00016890: 646c 6527 5d0a 2020 2020 6966 2069 7369  dle'].    if isi
+000168a0: 6e73 7461 6e63 6528 6861 6e64 6c65 2c20  nstance(handle, 
+000168b0: 6261 636b 656e 6473 2e43 6c6f 7564 566d  backends.CloudVm
+000168c0: 5261 7952 6573 6f75 7263 6548 616e 646c  RayResourceHandl
+000168d0: 6529 3a0a 2020 2020 2020 2020 7573 655f  e):.        use_
+000168e0: 7370 6f74 203d 2068 616e 646c 652e 6c61  spot = handle.la
+000168f0: 756e 6368 6564 5f72 6573 6f75 7263 6573  unched_resources
+00016900: 2e75 7365 5f73 706f 740a 2020 2020 2020  .use_spot.      
+00016910: 2020 6861 735f 6175 746f 7374 6f70 203d    has_autostop =
+00016920: 2028 7265 636f 7264 5b27 7374 6174 7573   (record['status
+00016930: 275d 2021 3d20 7374 6174 7573 5f6c 6962  '] != status_lib
+00016940: 2e43 6c75 7374 6572 5374 6174 7573 2e53  .ClusterStatus.S
+00016950: 544f 5050 4544 2061 6e64 0a20 2020 2020  TOPPED and.     
+00016960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016970: 2020 2072 6563 6f72 645b 2761 7574 6f73     record['autos
+00016980: 746f 7027 5d20 3e3d 2030 290a 2020 2020  top'] >= 0).    
+00016990: 2020 2020 666f 7263 655f 7265 6672 6573      force_refres
+000169a0: 685f 666f 725f 636c 7573 7465 7220 3d20  h_for_cluster = 
+000169b0: 2866 6f72 6365 5f72 6566 7265 7368 5f73  (force_refresh_s
+000169c0: 7461 7475 7365 7320 6973 206e 6f74 204e  tatuses is not N
+000169d0: 6f6e 6520 616e 640a 2020 2020 2020 2020  one and.        
+000169e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000169f0: 2020 2020 2020 2020 2020 2020 2072 6563               rec
+00016a00: 6f72 645b 2773 7461 7475 7327 5d20 696e  ord['status'] in
+00016a10: 2066 6f72 6365 5f72 6566 7265 7368 5f73   force_refresh_s
+00016a20: 7461 7475 7365 7329 0a20 2020 2020 2020  tatuses).       
+00016a30: 2069 6620 666f 7263 655f 7265 6672 6573   if force_refres
+00016a40: 685f 666f 725f 636c 7573 7465 7220 6f72  h_for_cluster or
+00016a50: 2068 6173 5f61 7574 6f73 746f 7020 6f72   has_autostop or
+00016a60: 2075 7365 5f73 706f 743a 0a20 2020 2020   use_spot:.     
+00016a70: 2020 2020 2020 2072 6563 6f72 6420 3d20         record = 
+00016a80: 5f75 7064 6174 655f 636c 7573 7465 725f  _update_cluster_
+00016a90: 7374 6174 7573 280a 2020 2020 2020 2020  status(.        
+00016aa0: 2020 2020 2020 2020 636c 7573 7465 725f          cluster_
+00016ab0: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
+00016ac0: 2020 2020 2020 6163 7175 6972 655f 7065        acquire_pe
+00016ad0: 725f 636c 7573 7465 725f 7374 6174 7573  r_cluster_status
+00016ae0: 5f6c 6f63 6b3d 6163 7175 6972 655f 7065  _lock=acquire_pe
+00016af0: 725f 636c 7573 7465 725f 7374 6174 7573  r_cluster_status
+00016b00: 5f6c 6f63 6b2c 0a20 2020 2020 2020 2020  _lock,.         
+00016b10: 2020 2020 2020 2063 6c75 7374 6572 5f73         cluster_s
+00016b20: 7461 7475 735f 6c6f 636b 5f74 696d 656f  tatus_lock_timeo
+00016b30: 7574 3d63 6c75 7374 6572 5f73 7461 7475  ut=cluster_statu
+00016b40: 735f 6c6f 636b 5f74 696d 656f 7574 290a  s_lock_timeout).
+00016b50: 2020 2020 7265 7475 726e 2072 6563 6f72      return recor
+00016b60: 640a 0a0a 4074 696d 656c 696e 652e 6576  d...@timeline.ev
+00016b70: 656e 740a 6465 6620 7265 6672 6573 685f  ent.def refresh_
+00016b80: 636c 7573 7465 725f 7374 6174 7573 5f68  cluster_status_h
+00016b90: 616e 646c 6528 0a20 2020 2063 6c75 7374  andle(.    clust
+00016ba0: 6572 5f6e 616d 653a 2073 7472 2c0a 2020  er_name: str,.  
+00016bb0: 2020 2a2c 0a20 2020 2066 6f72 6365 5f72    *,.    force_r
+00016bc0: 6566 7265 7368 5f73 7461 7475 7365 733a  efresh_statuses:
+00016bd0: 204f 7074 696f 6e61 6c5b 5365 745b 7374   Optional[Set[st
+00016be0: 6174 7573 5f6c 6962 2e43 6c75 7374 6572  atus_lib.Cluster
+00016bf0: 5374 6174 7573 5d5d 203d 204e 6f6e 652c  Status]] = None,
+00016c00: 0a20 2020 2061 6371 7569 7265 5f70 6572  .    acquire_per
+00016c10: 5f63 6c75 7374 6572 5f73 7461 7475 735f  _cluster_status_
+00016c20: 6c6f 636b 3a20 626f 6f6c 203d 2054 7275  lock: bool = Tru
+00016c30: 652c 0a20 2020 2063 6c75 7374 6572 5f73  e,.    cluster_s
+00016c40: 7461 7475 735f 6c6f 636b 5f74 696d 656f  tatus_lock_timeo
+00016c50: 7574 3a20 696e 7420 3d20 434c 5553 5445  ut: int = CLUSTE
+00016c60: 525f 5354 4154 5553 5f4c 4f43 4b5f 5449  R_STATUS_LOCK_TI
+00016c70: 4d45 4f55 545f 5345 434f 4e44 530a 2920  MEOUT_SECONDS.) 
+00016c80: 2d3e 2054 7570 6c65 5b4f 7074 696f 6e61  -> Tuple[Optiona
+00016c90: 6c5b 7374 6174 7573 5f6c 6962 2e43 6c75  l[status_lib.Clu
+00016ca0: 7374 6572 5374 6174 7573 5d2c 0a20 2020  sterStatus],.   
+00016cb0: 2020 2020 2020 2020 4f70 7469 6f6e 616c          Optional
+00016cc0: 5b62 6163 6b65 6e64 732e 5265 736f 7572  [backends.Resour
+00016cd0: 6365 4861 6e64 6c65 5d5d 3a0a 2020 2020  ceHandle]]:.    
+00016ce0: 2222 2252 6566 7265 7368 2074 6865 2063  """Refresh the c
+00016cf0: 6c75 7374 6572 2c20 616e 6420 7265 7475  luster, and retu
+00016d00: 726e 2074 6865 2070 6f73 7369 626c 7920  rn the possibly 
+00016d10: 7570 6461 7465 6420 7374 6174 7573 2061  updated status a
+00016d20: 6e64 2068 616e 646c 652e 0a0a 2020 2020  nd handle...    
+00016d30: 5468 6973 2069 7320 6120 7772 6170 7065  This is a wrappe
+00016d40: 7220 6f66 2072 6566 7265 7368 5f63 6c75  r of refresh_clu
+00016d50: 7374 6572 5f72 6563 6f72 642c 2077 6869  ster_record, whi
+00016d60: 6368 2072 6574 7572 6e73 2074 6865 2073  ch returns the s
+00016d70: 7461 7475 7320 616e 640a 2020 2020 6861  tatus and.    ha
+00016d80: 6e64 6c65 206f 6620 7468 6520 636c 7573  ndle of the clus
+00016d90: 7465 722e 0a20 2020 2050 6c65 6173 6520  ter..    Please 
+00016da0: 7265 6665 7220 746f 2074 6865 2064 6f63  refer to the doc
+00016db0: 7374 7269 6e67 206f 6620 7265 6672 6573  string of refres
+00016dc0: 685f 636c 7573 7465 725f 7265 636f 7264  h_cluster_record
+00016dd0: 2066 6f72 2074 6865 2064 6574 6169 6c73   for the details
+00016de0: 2e0a 2020 2020 2222 220a 2020 2020 7265  ..    """.    re
+00016df0: 636f 7264 203d 2072 6566 7265 7368 5f63  cord = refresh_c
+00016e00: 6c75 7374 6572 5f72 6563 6f72 6428 0a20  luster_record(. 
+00016e10: 2020 2020 2020 2063 6c75 7374 6572 5f6e         cluster_n
+00016e20: 616d 652c 0a20 2020 2020 2020 2066 6f72  ame,.        for
+00016e30: 6365 5f72 6566 7265 7368 5f73 7461 7475  ce_refresh_statu
+00016e40: 7365 733d 666f 7263 655f 7265 6672 6573  ses=force_refres
+00016e50: 685f 7374 6174 7573 6573 2c0a 2020 2020  h_statuses,.    
+00016e60: 2020 2020 6163 7175 6972 655f 7065 725f      acquire_per_
+00016e70: 636c 7573 7465 725f 7374 6174 7573 5f6c  cluster_status_l
+00016e80: 6f63 6b3d 6163 7175 6972 655f 7065 725f  ock=acquire_per_
+00016e90: 636c 7573 7465 725f 7374 6174 7573 5f6c  cluster_status_l
+00016ea0: 6f63 6b2c 0a20 2020 2020 2020 2063 6c75  ock,.        clu
+00016eb0: 7374 6572 5f73 7461 7475 735f 6c6f 636b  ster_status_lock
+00016ec0: 5f74 696d 656f 7574 3d63 6c75 7374 6572  _timeout=cluster
+00016ed0: 5f73 7461 7475 735f 6c6f 636b 5f74 696d  _status_lock_tim
+00016ee0: 656f 7574 290a 2020 2020 6966 2072 6563  eout).    if rec
+00016ef0: 6f72 6420 6973 204e 6f6e 653a 0a20 2020  ord is None:.   
+00016f00: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+00016f10: 2c20 4e6f 6e65 0a20 2020 2072 6574 7572  , None.    retur
+00016f20: 6e20 7265 636f 7264 5b27 7374 6174 7573  n record['status
+00016f30: 275d 2c20 7265 636f 7264 5b27 6861 6e64  '], record['hand
+00016f40: 6c65 275d 0a0a 0a23 203d 3d3d 3d3d 3d3d  le']...# =======
+00016f50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00016f60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a  ==============..
+00016f70: 0a40 7479 7069 6e67 2e6f 7665 726c 6f61  .@typing.overloa
+00016f80: 640a 6465 6620 6368 6563 6b5f 636c 7573  d.def check_clus
+00016f90: 7465 725f 6176 6169 6c61 626c 6528 0a20  ter_available(. 
+00016fa0: 2020 2063 6c75 7374 6572 5f6e 616d 653a     cluster_name:
+00016fb0: 2073 7472 2c0a 2020 2020 2a2c 0a20 2020   str,.    *,.   
+00016fc0: 206f 7065 7261 7469 6f6e 3a20 7374 722c   operation: str,
+00016fd0: 0a20 2020 2063 6865 636b 5f63 6c6f 7564  .    check_cloud
+00016fe0: 5f76 6d5f 7261 795f 6261 636b 656e 643a  _vm_ray_backend:
+00016ff0: 204c 6974 6572 616c 5b54 7275 655d 203d   Literal[True] =
+00017000: 2054 7275 652c 0a20 2020 2064 7279 7275   True,.    dryru
+00017010: 6e3a 2062 6f6f 6c20 3d20 2e2e 2e2c 0a29  n: bool = ...,.)
+00017020: 202d 3e20 2763 6c6f 7564 5f76 6d5f 7261   -> 'cloud_vm_ra
+00017030: 795f 6261 636b 656e 642e 436c 6f75 6456  y_backend.CloudV
+00017040: 6d52 6179 5265 736f 7572 6365 4861 6e64  mRayResourceHand
+00017050: 6c65 273a 0a20 2020 202e 2e2e 0a0a 0a40  le':.    ......@
+00017060: 7479 7069 6e67 2e6f 7665 726c 6f61 640a  typing.overload.
+00017070: 6465 6620 6368 6563 6b5f 636c 7573 7465  def check_cluste
+00017080: 725f 6176 6169 6c61 626c 6528 0a20 2020  r_available(.   
+00017090: 2063 6c75 7374 6572 5f6e 616d 653a 2073   cluster_name: s
+000170a0: 7472 2c0a 2020 2020 2a2c 0a20 2020 206f  tr,.    *,.    o
+000170b0: 7065 7261 7469 6f6e 3a20 7374 722c 0a20  peration: str,. 
+000170c0: 2020 2063 6865 636b 5f63 6c6f 7564 5f76     check_cloud_v
+000170d0: 6d5f 7261 795f 6261 636b 656e 643a 204c  m_ray_backend: L
+000170e0: 6974 6572 616c 5b46 616c 7365 5d2c 0a20  iteral[False],. 
+000170f0: 2020 2064 7279 7275 6e3a 2062 6f6f 6c20     dryrun: bool 
+00017100: 3d20 2e2e 2e2c 0a29 202d 3e20 6261 636b  = ...,.) -> back
+00017110: 656e 6473 2e52 6573 6f75 7263 6548 616e  ends.ResourceHan
+00017120: 646c 653a 0a20 2020 202e 2e2e 0a0a 0a64  dle:.    ......d
+00017130: 6566 2063 6865 636b 5f63 6c75 7374 6572  ef check_cluster
+00017140: 5f61 7661 696c 6162 6c65 280a 2020 2020  _available(.    
+00017150: 636c 7573 7465 725f 6e61 6d65 3a20 7374  cluster_name: st
+00017160: 722c 0a20 2020 202a 2c0a 2020 2020 6f70  r,.    *,.    op
+00017170: 6572 6174 696f 6e3a 2073 7472 2c0a 2020  eration: str,.  
+00017180: 2020 6368 6563 6b5f 636c 6f75 645f 766d    check_cloud_vm
+00017190: 5f72 6179 5f62 6163 6b65 6e64 3a20 626f  _ray_backend: bo
+000171a0: 6f6c 203d 2054 7275 652c 0a20 2020 2064  ol = True,.    d
+000171b0: 7279 7275 6e3a 2062 6f6f 6c20 3d20 4661  ryrun: bool = Fa
+000171c0: 6c73 652c 0a29 202d 3e20 6261 636b 656e  lse,.) -> backen
+000171d0: 6473 2e52 6573 6f75 7263 6548 616e 646c  ds.ResourceHandl
+000171e0: 653a 0a20 2020 2022 2222 4368 6563 6b20  e:.    """Check 
+000171f0: 6966 2074 6865 2063 6c75 7374 6572 2069  if the cluster i
+00017200: 7320 6176 6169 6c61 626c 652e 0a0a 2020  s available...  
+00017210: 2020 5261 6973 6573 3a0a 2020 2020 2020    Raises:.      
+00017220: 2020 5661 6c75 6545 7272 6f72 3a20 6966    ValueError: if
+00017230: 2074 6865 2063 6c75 7374 6572 2064 6f65   the cluster doe
+00017240: 7320 6e6f 7420 6578 6973 742e 0a20 2020  s not exist..   
+00017250: 2020 2020 2065 7863 6570 7469 6f6e 732e       exceptions.
+00017260: 436c 7573 7465 724e 6f74 5570 4572 726f  ClusterNotUpErro
+00017270: 723a 2069 6620 7468 6520 636c 7573 7465  r: if the cluste
+00017280: 7220 6973 206e 6f74 2055 502e 0a20 2020  r is not UP..   
+00017290: 2020 2020 2065 7863 6570 7469 6f6e 732e       exceptions.
+000172a0: 4e6f 7453 7570 706f 7274 6564 4572 726f  NotSupportedErro
+000172b0: 723a 2069 6620 7468 6520 636c 7573 7465  r: if the cluste
+000172c0: 7220 6973 206e 6f74 2062 6173 6564 206f  r is not based o
+000172d0: 6e0a 2020 2020 2020 2020 2020 436c 6f75  n.          Clou
+000172e0: 6456 6d52 6179 4261 636b 656e 642e 0a20  dVmRayBackend.. 
+000172f0: 2020 2020 2020 2065 7863 6570 7469 6f6e         exception
+00017300: 732e 436c 7573 7465 724f 776e 6572 4964  s.ClusterOwnerId
+00017310: 656e 7469 7479 4d69 736d 6174 6368 4572  entityMismatchEr
+00017320: 726f 723a 2069 6620 7468 6520 6375 7272  ror: if the curr
+00017330: 656e 7420 7573 6572 2069 730a 2020 2020  ent user is.    
+00017340: 2020 2020 2020 6e6f 7420 7468 6520 7361        not the sa
+00017350: 6d65 2061 7320 7468 6520 7573 6572 2077  me as the user w
+00017360: 686f 2063 7265 6174 6564 2074 6865 2063  ho created the c
+00017370: 6c75 7374 6572 2e0a 2020 2020 2020 2020  luster..        
+00017380: 6578 6365 7074 696f 6e73 2e43 6c6f 7564  exceptions.Cloud
+00017390: 5573 6572 4964 656e 7469 7479 4572 726f  UserIdentityErro
+000173a0: 723a 2069 6620 7765 2066 6169 6c20 746f  r: if we fail to
+000173b0: 2067 6574 2074 6865 2063 7572 7265 6e74   get the current
+000173c0: 2075 7365 720a 2020 2020 2020 2020 2020   user.          
+000173d0: 6964 656e 7469 7479 2e0a 2020 2020 2222  identity..    ""
+000173e0: 220a 2020 2020 7265 636f 7264 203d 2067  ".    record = g
+000173f0: 6c6f 6261 6c5f 7573 6572 5f73 7461 7465  lobal_user_state
+00017400: 2e67 6574 5f63 6c75 7374 6572 5f66 726f  .get_cluster_fro
+00017410: 6d5f 6e61 6d65 2863 6c75 7374 6572 5f6e  m_name(cluster_n
+00017420: 616d 6529 0a20 2020 2069 6620 6472 7972  ame).    if dryr
+00017430: 756e 3a0a 2020 2020 2020 2020 6173 7365  un:.        asse
+00017440: 7274 2072 6563 6f72 6420 6973 206e 6f74  rt record is not
+00017450: 204e 6f6e 652c 2063 6c75 7374 6572 5f6e   None, cluster_n
+00017460: 616d 650a 2020 2020 2020 2020 7265 7475  ame.        retu
+00017470: 726e 2072 6563 6f72 645b 2768 616e 646c  rn record['handl
+00017480: 6527 5d0a 0a20 2020 2070 7265 7669 6f75  e']..    previou
+00017490: 735f 636c 7573 7465 725f 7374 6174 7573  s_cluster_status
+000174a0: 203d 204e 6f6e 650a 2020 2020 6966 2072   = None.    if r
+000174b0: 6563 6f72 6420 6973 206e 6f74 204e 6f6e  ecord is not Non
+000174c0: 653a 0a20 2020 2020 2020 2070 7265 7669  e:.        previ
+000174d0: 6f75 735f 636c 7573 7465 725f 7374 6174  ous_cluster_stat
+000174e0: 7573 203d 2072 6563 6f72 645b 2773 7461  us = record['sta
+000174f0: 7475 7327 5d0a 0a20 2020 2074 7279 3a0a  tus']..    try:.
+00017500: 2020 2020 2020 2020 636c 7573 7465 725f          cluster_
+00017510: 7374 6174 7573 2c20 6861 6e64 6c65 203d  status, handle =
+00017520: 2072 6566 7265 7368 5f63 6c75 7374 6572   refresh_cluster
+00017530: 5f73 7461 7475 735f 6861 6e64 6c65 2863  _status_handle(c
+00017540: 6c75 7374 6572 5f6e 616d 6529 0a20 2020  luster_name).   
+00017550: 2065 7863 6570 7420 6578 6365 7074 696f   except exceptio
+00017560: 6e73 2e43 6c75 7374 6572 5374 6174 7573  ns.ClusterStatus
+00017570: 4665 7463 6869 6e67 4572 726f 7220 6173  FetchingError as
+00017580: 2065 3a0a 2020 2020 2020 2020 2320 4661   e:.        # Fa
+00017590: 696c 6564 2074 6f20 7265 6672 6573 6820  iled to refresh 
+000175a0: 7468 6520 636c 7573 7465 7220 7374 6174  the cluster stat
+000175b0: 7573 2069 7320 6e6f 7420 6661 7461 6c20  us is not fatal 
+000175c0: 6572 726f 7220 6173 2074 6865 2063 616c  error as the cal
+000175d0: 6c65 7273 0a20 2020 2020 2020 2023 2063  lers.        # c
+000175e0: 616e 2073 7469 6c6c 2062 6520 646f 6e65  an still be done
+000175f0: 2062 7920 6f6e 6c79 2075 7369 6e67 2073   by only using s
+00017600: 7368 2c20 6275 7420 7468 6520 7373 6820  sh, but the ssh 
+00017610: 6361 6e20 6861 6e67 2069 6620 7468 650a  can hang if the.
+00017620: 2020 2020 2020 2020 2320 636c 7573 7465          # cluste
+00017630: 7220 6973 206e 6f74 2075 7020 2865 2e67  r is not up (e.g
+00017640: 2e2c 2061 7574 6f73 746f 7070 6564 292e  ., autostopped).
+00017650: 0a0a 2020 2020 2020 2020 2320 5765 2064  ..        # We d
+00017660: 6f20 6e6f 7420 6361 7463 6820 7468 6520  o not catch the 
+00017670: 6578 6365 7074 696f 6e20 666f 7220 636c  exception for cl
+00017680: 6f75 6420 6964 656e 7469 7479 2063 6865  oud identity che
+00017690: 636b 696e 6720 666f 7220 6e6f 772c 2069  cking for now, i
+000176a0: 6e0a 2020 2020 2020 2020 2320 6f72 6465  n.        # orde
+000176b0: 7220 746f 2064 6973 6162 6c65 2061 6c6c  r to disable all
+000176c0: 206f 7065 7261 7469 6f6e 7320 6f6e 2063   operations on c
+000176d0: 6c75 7374 6572 7320 6372 6561 7465 6420  lusters created 
+000176e0: 6279 2061 6e6f 7468 6572 2075 7365 720a  by another user.
+000176f0: 2020 2020 2020 2020 2320 6964 656e 7469          # identi
+00017700: 7479 2e20 2054 6861 7420 7769 6c6c 206d  ty.  That will m
+00017710: 616b 6520 7468 6520 6465 7369 676e 2073  ake the design s
+00017720: 696d 706c 6572 2061 6e64 2065 6173 6965  impler and easie
+00017730: 7220 746f 0a20 2020 2020 2020 2023 2075  r to.        # u
+00017740: 6e64 6572 7374 616e 642c 2062 7574 2069  nderstand, but i
+00017750: 7420 6d69 6768 7420 6265 2075 7365 6675  t might be usefu
+00017760: 6c20 746f 2061 6c6c 6f77 2074 6865 2075  l to allow the u
+00017770: 7365 7220 746f 2075 7365 0a20 2020 2020  ser to use.     
+00017780: 2020 2023 206f 7065 7261 7469 6f6e 7320     # operations 
+00017790: 7468 6174 206f 6e6c 7920 696e 766f 6c76  that only involv
+000177a0: 6520 7373 6820 2865 2e67 2e2c 2073 6b79  e ssh (e.g., sky
+000177b0: 2065 7865 632c 2073 6b79 206c 6f67 732c   exec, sky logs,
+000177c0: 2065 7463 2920 6576 656e 0a20 2020 2020   etc) even.     
+000177d0: 2020 2023 2069 6620 7468 6520 7573 6572     # if the user
+000177e0: 2069 7320 6e6f 7420 7468 6520 6f77 6e65   is not the owne
+000177f0: 7220 6f66 2074 6865 2063 6c75 7374 6572  r of the cluster
+00017800: 2e0a 2020 2020 2020 2020 7578 5f75 7469  ..        ux_uti
+00017810: 6c73 2e63 6f6e 736f 6c65 5f6e 6577 6c69  ls.console_newli
+00017820: 6e65 2829 0a20 2020 2020 2020 206c 6f67  ne().        log
+00017830: 6765 722e 7761 726e 696e 6728 0a20 2020  ger.warning(.   
+00017840: 2020 2020 2020 2020 2066 2746 6169 6c65           f'Faile
+00017850: 6420 746f 2072 6566 7265 7368 2074 6865  d to refresh the
+00017860: 2073 7461 7475 7320 666f 7220 636c 7573   status for clus
+00017870: 7465 7220 7b63 6c75 7374 6572 5f6e 616d  ter {cluster_nam
+00017880: 6521 727d 2e20 4974 2069 7320 270a 2020  e!r}. It is '.  
+00017890: 2020 2020 2020 2020 2020 6627 6e6f 7420            f'not 
+000178a0: 6661 7461 6c2c 2062 7574 207b 6f70 6572  fatal, but {oper
+000178b0: 6174 696f 6e7d 206d 6967 6874 2068 616e  ation} might han
+000178c0: 6720 6966 2074 6865 2063 6c75 7374 6572  g if the cluster
+000178d0: 2069 7320 6e6f 7420 7570 2e5c 6e27 0a20   is not up.\n'. 
+000178e0: 2020 2020 2020 2020 2020 2066 2744 6574             f'Det
+000178f0: 6169 6c65 6420 7265 6173 6f6e 3a20 7b65  ailed reason: {e
+00017900: 7d27 290a 2020 2020 2020 2020 6966 2072  }').        if r
+00017910: 6563 6f72 6420 6973 204e 6f6e 653a 0a20  ecord is None:. 
+00017920: 2020 2020 2020 2020 2020 2063 6c75 7374             clust
+00017930: 6572 5f73 7461 7475 732c 2068 616e 646c  er_status, handl
+00017940: 6520 3d20 4e6f 6e65 2c20 4e6f 6e65 0a20  e = None, None. 
+00017950: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00017960: 2020 2020 2020 2020 2063 6c75 7374 6572           cluster
+00017970: 5f73 7461 7475 732c 2068 616e 646c 6520  _status, handle 
+00017980: 3d20 7265 636f 7264 5b27 7374 6174 7573  = record['status
+00017990: 275d 2c20 7265 636f 7264 5b27 6861 6e64  '], record['hand
+000179a0: 6c65 275d 0a0a 2020 2020 6272 6967 6874  le']..    bright
+000179b0: 203d 2063 6f6c 6f72 616d 612e 5374 796c   = colorama.Styl
+000179c0: 652e 4252 4947 4854 0a20 2020 2072 6573  e.BRIGHT.    res
+000179d0: 6574 203d 2063 6f6c 6f72 616d 612e 5374  et = colorama.St
+000179e0: 796c 652e 5245 5345 545f 414c 4c0a 2020  yle.RESET_ALL.  
+000179f0: 2020 6966 2068 616e 646c 6520 6973 204e    if handle is N
+00017a00: 6f6e 653a 0a20 2020 2020 2020 2069 6620  one:.        if 
+00017a10: 7072 6576 696f 7573 5f63 6c75 7374 6572  previous_cluster
+00017a20: 5f73 7461 7475 7320 6973 204e 6f6e 653a  _status is None:
+00017a30: 0a20 2020 2020 2020 2020 2020 2065 7272  .            err
+00017a40: 6f72 5f6d 7367 203d 2066 2743 6c75 7374  or_msg = f'Clust
+00017a50: 6572 207b 636c 7573 7465 725f 6e61 6d65  er {cluster_name
+00017a60: 2172 7d20 646f 6573 206e 6f74 2065 7869  !r} does not exi
+00017a70: 7374 2e27 0a20 2020 2020 2020 2065 6c73  st.'.        els
+00017a80: 653a 0a20 2020 2020 2020 2020 2020 2065  e:.            e
+00017a90: 7272 6f72 5f6d 7367 203d 2028 6627 436c  rror_msg = (f'Cl
+00017aa0: 7573 7465 7220 7b63 6c75 7374 6572 5f6e  uster {cluster_n
+00017ab0: 616d 6521 727d 206e 6f74 2066 6f75 6e64  ame!r} not found
+00017ac0: 206f 6e20 7468 6520 636c 6f75 6420 270a   on the cloud '.
+00017ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ae0: 2020 2020 2020 2020 2027 7072 6f76 6964           'provid
+00017af0: 6572 2e27 290a 2020 2020 2020 2020 2020  er.').          
+00017b00: 2020 6173 7365 7274 2072 6563 6f72 6420    assert record 
+00017b10: 6973 206e 6f74 204e 6f6e 652c 2070 7265  is not None, pre
+00017b20: 7669 6f75 735f 636c 7573 7465 725f 7374  vious_cluster_st
+00017b30: 6174 7573 0a20 2020 2020 2020 2020 2020  atus.           
+00017b40: 2061 6374 696f 6e73 203d 205b 5d0a 2020   actions = [].  
+00017b50: 2020 2020 2020 2020 2020 6966 2072 6563            if rec
+00017b60: 6f72 645b 2768 616e 646c 6527 5d2e 6c61  ord['handle'].la
+00017b70: 756e 6368 6564 5f72 6573 6f75 7263 6573  unched_resources
+00017b80: 2e75 7365 5f73 706f 743a 0a20 2020 2020  .use_spot:.     
+00017b90: 2020 2020 2020 2020 2020 2061 6374 696f             actio
+00017ba0: 6e73 2e61 7070 656e 6428 2770 7265 656d  ns.append('preem
+00017bb0: 7074 6564 2729 0a20 2020 2020 2020 2020  pted').         
+00017bc0: 2020 2069 6620 7265 636f 7264 5b27 6175     if record['au
+00017bd0: 746f 7374 6f70 275d 203e 2030 2061 6e64  tostop'] > 0 and
+00017be0: 2072 6563 6f72 645b 2774 6f5f 646f 776e   record['to_down
+00017bf0: 275d 3a0a 2020 2020 2020 2020 2020 2020  ']:.            
+00017c00: 2020 2020 6163 7469 6f6e 732e 6170 7065      actions.appe
+00017c10: 6e64 2827 6175 746f 646f 776e 6564 2729  nd('autodowned')
+00017c20: 0a20 2020 2020 2020 2020 2020 2061 6374  .            act
+00017c30: 696f 6e73 2e61 7070 656e 6428 276d 616e  ions.append('man
+00017c40: 7561 6c6c 7920 7465 726d 696e 6174 6564  ually terminated
+00017c50: 2069 6e20 636f 6e73 6f6c 6527 290a 2020   in console').  
+00017c60: 2020 2020 2020 2020 2020 6966 206c 656e            if len
+00017c70: 2861 6374 696f 6e73 2920 3e20 313a 0a20  (actions) > 1:. 
+00017c80: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00017c90: 6374 696f 6e73 5b2d 315d 203d 2027 6f72  ctions[-1] = 'or
+00017ca0: 2027 202b 2061 6374 696f 6e73 5b2d 315d   ' + actions[-1]
+00017cb0: 0a20 2020 2020 2020 2020 2020 2061 6374  .            act
+00017cc0: 696f 6e73 5f73 7472 203d 2027 2c20 272e  ions_str = ', '.
+00017cd0: 6a6f 696e 2861 6374 696f 6e73 290a 2020  join(actions).  
+00017ce0: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
+00017cf0: 6520 3d20 6627 2049 7420 7761 7320 6c69  e = f' It was li
+00017d00: 6b65 6c79 207b 6163 7469 6f6e 735f 7374  kely {actions_st
+00017d10: 727d 2e27 0a20 2020 2020 2020 2020 2020  r}.'.           
+00017d20: 2069 6620 6c65 6e28 6163 7469 6f6e 7329   if len(actions)
+00017d30: 203e 2031 3a0a 2020 2020 2020 2020 2020   > 1:.          
+00017d40: 2020 2020 2020 6d65 7373 6167 6520 3d20        message = 
+00017d50: 6d65 7373 6167 652e 7265 706c 6163 6528  message.replace(
+00017d60: 276c 696b 656c 7927 2c20 2765 6974 6865  'likely', 'eithe
+00017d70: 7227 290a 2020 2020 2020 2020 2020 2020  r').            
+00017d80: 6572 726f 725f 6d73 6720 2b3d 206d 6573  error_msg += mes
+00017d90: 7361 6765 0a0a 2020 2020 2020 2020 7769  sage..        wi
+00017da0: 7468 2075 785f 7574 696c 732e 7072 696e  th ux_utils.prin
+00017db0: 745f 6578 6365 7074 696f 6e5f 6e6f 5f74  t_exception_no_t
+00017dc0: 7261 6365 6261 636b 2829 3a0a 2020 2020  raceback():.    
+00017dd0: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00017de0: 6c75 6545 7272 6f72 2866 277b 636f 6c6f  lueError(f'{colo
+00017df0: 7261 6d61 2e46 6f72 652e 5945 4c4c 4f57  rama.Fore.YELLOW
+00017e00: 7d7b 6572 726f 725f 6d73 677d 7b72 6573  }{error_msg}{res
+00017e10: 6574 7d27 290a 2020 2020 6173 7365 7274  et}').    assert
+00017e20: 2063 6c75 7374 6572 5f73 7461 7475 7320   cluster_status 
+00017e30: 6973 206e 6f74 204e 6f6e 652c 2027 6861  is not None, 'ha
+00017e40: 6e64 6c65 2069 7320 6e6f 7420 4e6f 6e65  ndle is not None
+00017e50: 2062 7574 2073 7461 7475 7320 6973 204e   but status is N
+00017e60: 6f6e 6527 0a20 2020 2062 6163 6b65 6e64  one'.    backend
+00017e70: 203d 2067 6574 5f62 6163 6b65 6e64 5f66   = get_backend_f
+00017e80: 726f 6d5f 6861 6e64 6c65 2868 616e 646c  rom_handle(handl
+00017e90: 6529 0a20 2020 2069 6620 6368 6563 6b5f  e).    if check_
+00017ea0: 636c 6f75 645f 766d 5f72 6179 5f62 6163  cloud_vm_ray_bac
+00017eb0: 6b65 6e64 2061 6e64 206e 6f74 2069 7369  kend and not isi
+00017ec0: 6e73 7461 6e63 6528 0a20 2020 2020 2020  nstance(.       
+00017ed0: 2020 2020 2062 6163 6b65 6e64 2c20 6261       backend, ba
+00017ee0: 636b 656e 6473 2e43 6c6f 7564 566d 5261  ckends.CloudVmRa
+00017ef0: 7942 6163 6b65 6e64 293a 0a20 2020 2020  yBackend):.     
+00017f00: 2020 2077 6974 6820 7578 5f75 7469 6c73     with ux_utils
+00017f10: 2e70 7269 6e74 5f65 7863 6570 7469 6f6e  .print_exception
+00017f20: 5f6e 6f5f 7472 6163 6562 6163 6b28 293a  _no_traceback():
+00017f30: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00017f40: 7365 2065 7863 6570 7469 6f6e 732e 4e6f  se exceptions.No
+00017f50: 7453 7570 706f 7274 6564 4572 726f 7228  tSupportedError(
+00017f60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017f70: 2066 277b 636f 6c6f 7261 6d61 2e46 6f72   f'{colorama.For
+00017f80: 652e 5945 4c4c 4f57 7d7b 6f70 6572 6174  e.YELLOW}{operat
+00017f90: 696f 6e2e 6361 7069 7461 6c69 7a65 2829  ion.capitalize()
+00017fa0: 7d3a 2073 6b69 7070 6564 2066 6f72 2027  }: skipped for '
+00017fb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017fc0: 2066 2763 6c75 7374 6572 207b 636c 7573   f'cluster {clus
+00017fd0: 7465 725f 6e61 6d65 2172 7d2e 2049 7420  ter_name!r}. It 
+00017fe0: 6973 206f 6e6c 7920 7375 7070 6f72 7465  is only supporte
+00017ff0: 6420 6279 2062 6163 6b65 6e64 3a20 270a  d by backend: '.
+00018000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018010: 6627 7b62 6163 6b65 6e64 732e 436c 6f75  f'{backends.Clou
+00018020: 6456 6d52 6179 4261 636b 656e 642e 4e41  dVmRayBackend.NA
+00018030: 4d45 7d2e 270a 2020 2020 2020 2020 2020  ME}.'.          
+00018040: 2020 2020 2020 6627 7b72 6573 6574 7d27        f'{reset}'
+00018050: 290a 2020 2020 6966 2063 6c75 7374 6572  ).    if cluster
+00018060: 5f73 7461 7475 7320 213d 2073 7461 7475  _status != statu
+00018070: 735f 6c69 622e 436c 7573 7465 7253 7461  s_lib.ClusterSta
+00018080: 7475 732e 5550 3a0a 2020 2020 2020 2020  tus.UP:.        
+00018090: 7769 7468 2075 785f 7574 696c 732e 7072  with ux_utils.pr
+000180a0: 696e 745f 6578 6365 7074 696f 6e5f 6e6f  int_exception_no
+000180b0: 5f74 7261 6365 6261 636b 2829 3a0a 2020  _traceback():.  
+000180c0: 2020 2020 2020 2020 2020 6869 6e74 5f66            hint_f
+000180d0: 6f72 5f69 6e69 7420 3d20 2727 0a20 2020  or_init = ''.   
+000180e0: 2020 2020 2020 2020 2069 6620 636c 7573           if clus
+000180f0: 7465 725f 7374 6174 7573 203d 3d20 7374  ter_status == st
+00018100: 6174 7573 5f6c 6962 2e43 6c75 7374 6572  atus_lib.Cluster
+00018110: 5374 6174 7573 2e49 4e49 543a 0a20 2020  Status.INIT:.   
+00018120: 2020 2020 2020 2020 2020 2020 2068 696e               hin
+00018130: 745f 666f 725f 696e 6974 203d 2028 0a20  t_for_init = (. 
+00018140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018150: 2020 2066 277b 7265 7365 747d 2057 6169     f'{reset} Wai
+00018160: 7420 666f 7220 6120 6c61 756e 6368 2074  t for a launch t
+00018170: 6f20 6669 6e69 7368 2c20 6f72 2075 7365  o finish, or use
+00018180: 2074 6869 7320 636f 6d6d 616e 6420 270a   this command '.
+00018190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000181a0: 2020 2020 6627 746f 2074 7279 2074 6f20      f'to try to 
+000181b0: 7472 616e 7369 7469 6f6e 2074 6865 2063  transition the c
+000181c0: 6c75 7374 6572 2074 6f20 5550 3a20 7b62  luster to UP: {b
+000181d0: 7269 6768 747d 736b 7920 270a 2020 2020  right}sky '.    
+000181e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000181f0: 6627 7374 6172 7420 7b63 6c75 7374 6572  f'start {cluster
+00018200: 5f6e 616d 657d 7b72 6573 6574 7d27 290a  _name}{reset}').
+00018210: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00018220: 6520 6578 6365 7074 696f 6e73 2e43 6c75  e exceptions.Clu
+00018230: 7374 6572 4e6f 7455 7045 7272 6f72 280a  sterNotUpError(.
+00018240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018250: 6627 7b63 6f6c 6f72 616d 612e 466f 7265  f'{colorama.Fore
+00018260: 2e59 454c 4c4f 577d 7b6f 7065 7261 7469  .YELLOW}{operati
+00018270: 6f6e 2e63 6170 6974 616c 697a 6528 297d  on.capitalize()}
+00018280: 3a20 736b 6970 7065 6420 666f 7220 270a  : skipped for '.
+00018290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000182a0: 6627 636c 7573 7465 7220 7b63 6c75 7374  f'cluster {clust
+000182b0: 6572 5f6e 616d 6521 727d 2028 7374 6174  er_name!r} (stat
+000182c0: 7573 3a20 7b63 6c75 7374 6572 5f73 7461  us: {cluster_sta
+000182d0: 7475 732e 7661 6c75 657d 292e 2027 0a20  tus.value}). '. 
+000182e0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+000182f0: 4974 2069 7320 6f6e 6c79 2061 6c6c 6f77  It is only allow
+00018300: 6564 2066 6f72 2027 0a20 2020 2020 2020  ed for '.       
+00018310: 2020 2020 2020 2020 2066 277b 7374 6174           f'{stat
+00018320: 7573 5f6c 6962 2e43 6c75 7374 6572 5374  us_lib.ClusterSt
+00018330: 6174 7573 2e55 502e 7661 6c75 657d 2063  atus.UP.value} c
+00018340: 6c75 7374 6572 732e 270a 2020 2020 2020  lusters.'.      
+00018350: 2020 2020 2020 2020 2020 6627 7b68 696e            f'{hin
+00018360: 745f 666f 725f 696e 6974 7d27 0a20 2020  t_for_init}'.   
+00018370: 2020 2020 2020 2020 2020 2020 2066 277b               f'{
+00018380: 7265 7365 747d 272c 0a20 2020 2020 2020  reset}',.       
+00018390: 2020 2020 2020 2020 2063 6c75 7374 6572           cluster
+000183a0: 5f73 7461 7475 733d 636c 7573 7465 725f  _status=cluster_
+000183b0: 7374 6174 7573 2c0a 2020 2020 2020 2020  status,.        
+000183c0: 2020 2020 2020 2020 6861 6e64 6c65 3d68          handle=h
+000183d0: 616e 646c 6529 0a0a 2020 2020 6966 2068  andle)..    if h
+000183e0: 616e 646c 652e 6865 6164 5f69 7020 6973  andle.head_ip is
+000183f0: 204e 6f6e 653a 0a20 2020 2020 2020 2077   None:.        w
+00018400: 6974 6820 7578 5f75 7469 6c73 2e70 7269  ith ux_utils.pri
+00018410: 6e74 5f65 7863 6570 7469 6f6e 5f6e 6f5f  nt_exception_no_
+00018420: 7472 6163 6562 6163 6b28 293a 0a20 2020  traceback():.   
+00018430: 2020 2020 2020 2020 2072 6169 7365 2065           raise e
+00018440: 7863 6570 7469 6f6e 732e 436c 7573 7465  xceptions.Cluste
+00018450: 724e 6f74 5570 4572 726f 7228 0a20 2020  rNotUpError(.   
+00018460: 2020 2020 2020 2020 2020 2020 2066 2743               f'C
+00018470: 6c75 7374 6572 207b 636c 7573 7465 725f  luster {cluster_
+00018480: 6e61 6d65 2172 7d20 6861 7320 6265 656e  name!r} has been
+00018490: 2073 746f 7070 6564 206f 7220 6e6f 7420   stopped or not 
+000184a0: 7072 6f70 6572 6c79 2027 0a20 2020 2020  properly '.     
+000184b0: 2020 2020 2020 2020 2020 2027 7365 7420             'set 
+000184c0: 7570 2e20 506c 6561 7365 2072 652d 6c61  up. Please re-la
+000184d0: 756e 6368 2069 7420 7769 7468 2060 736b  unch it with `sk
+000184e0: 7920 7374 6172 7460 2e27 2c0a 2020 2020  y start`.',.    
+000184f0: 2020 2020 2020 2020 2020 2020 636c 7573              clus
+00018500: 7465 725f 7374 6174 7573 3d63 6c75 7374  ter_status=clust
+00018510: 6572 5f73 7461 7475 732c 0a20 2020 2020  er_status,.     
+00018520: 2020 2020 2020 2020 2020 2068 616e 646c             handl
+00018530: 653d 6861 6e64 6c65 290a 2020 2020 7265  e=handle).    re
+00018540: 7475 726e 2068 616e 646c 650a 0a0a 2320  turn handle...# 
+00018550: 544f 444f 2874 6961 6e29 3a20 5265 6661  TODO(tian): Refa
+00018560: 6374 6f72 2074 6f20 636f 6e74 726f 6c6c  ctor to controll
+00018570: 6572 5f75 7469 6c73 2e20 4375 7272 656e  er_utils. Curren
+00018580: 7420 626c 6f63 6b65 723a 2063 6972 6375  t blocker: circu
+00018590: 6c61 7220 696d 706f 7274 2e0a 6465 6620  lar import..def 
+000185a0: 6973 5f63 6f6e 7472 6f6c 6c65 725f 6163  is_controller_ac
+000185b0: 6365 7373 6962 6c65 280a 2020 2020 636f  cessible(.    co
+000185c0: 6e74 726f 6c6c 6572 3a20 636f 6e74 726f  ntroller: contro
+000185d0: 6c6c 6572 5f75 7469 6c73 2e43 6f6e 7472  ller_utils.Contr
+000185e0: 6f6c 6c65 7273 2c0a 2020 2020 7374 6f70  ollers,.    stop
+000185f0: 7065 645f 6d65 7373 6167 653a 2073 7472  ped_message: str
+00018600: 2c0a 2020 2020 6e6f 6e5f 6578 6973 7465  ,.    non_existe
+00018610: 6e74 5f6d 6573 7361 6765 3a20 4f70 7469  nt_message: Opti
+00018620: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00018630: 2c0a 2020 2020 6578 6974 5f69 665f 6e6f  ,.    exit_if_no
+00018640: 745f 6163 6365 7373 6962 6c65 3a20 626f  t_accessible: bo
+00018650: 6f6c 203d 2046 616c 7365 2c0a 2920 2d3e  ol = False,.) ->
+00018660: 2027 6261 636b 656e 6473 2e43 6c6f 7564   'backends.Cloud
+00018670: 566d 5261 7952 6573 6f75 7263 6548 616e  VmRayResourceHan
+00018680: 646c 6527 3a0a 2020 2020 2222 2243 6865  dle':.    """Che
+00018690: 636b 2069 6620 7468 6520 6a6f 6273 2f73  ck if the jobs/s
+000186a0: 6572 7665 2063 6f6e 7472 6f6c 6c65 7220  erve controller 
+000186b0: 6973 2075 702e 0a0a 2020 2020 5468 6520  is up...    The 
+000186c0: 636f 6e74 726f 6c6c 6572 2069 7320 6163  controller is ac
+000186d0: 6365 7373 6962 6c65 2077 6865 6e20 6974  cessible when it
+000186e0: 2069 7320 696e 2055 5020 6f72 2049 4e49   is in UP or INI
+000186f0: 5420 7374 6174 652c 2061 6e64 2074 6865  T state, and the
+00018700: 2073 7368 0a20 2020 2063 6f6e 6e65 6374   ssh.    connect
+00018710: 696f 6e20 6973 2073 7563 6365 7373 6675  ion is successfu
+00018720: 6c2e 0a0a 2020 2020 4974 2063 616e 2062  l...    It can b
+00018730: 6520 7573 6564 2074 6f20 6368 6563 6b20  e used to check 
+00018740: 6966 2074 6865 2063 6f6e 7472 6f6c 6c65  if the controlle
+00018750: 7220 6973 2061 6363 6573 7369 626c 6520  r is accessible 
+00018760: 2873 696e 6365 2074 6865 2061 7574 6f73  (since the autos
+00018770: 746f 700a 2020 2020 6973 2073 6574 2066  top.    is set f
+00018780: 6f72 2074 6865 2063 6f6e 7472 6f6c 6c65  or the controlle
+00018790: 7229 2062 6566 6f72 6520 7468 6520 6a6f  r) before the jo
+000187a0: 6273 2f73 6572 7665 2063 6f6d 6d61 6e64  bs/serve command
+000187b0: 7320 696e 7465 7261 6374 2077 6974 6820  s interact with 
+000187c0: 7468 650a 2020 2020 636f 6e74 726f 6c6c  the.    controll
+000187d0: 6572 2e0a 0a20 2020 2043 6c75 7374 6572  er...    Cluster
+000187e0: 4e6f 7455 7045 7272 6f72 2077 696c 6c20  NotUpError will 
+000187f0: 6265 2072 6169 7365 6420 7768 656e 6576  be raised whenev
+00018800: 6572 2074 6865 2063 6f6e 7472 6f6c 6c65  er the controlle
+00018810: 7220 6361 6e6e 6f74 2062 6520 6163 6365  r cannot be acce
+00018820: 7373 6564 2e0a 0a20 2020 2041 7267 733a  ssed...    Args:
+00018830: 0a20 2020 2020 2020 2074 7970 653a 2054  .        type: T
+00018840: 7970 6520 6f66 2074 6865 2063 6f6e 7472  ype of the contr
+00018850: 6f6c 6c65 722e 0a20 2020 2020 2020 2073  oller..        s
+00018860: 746f 7070 6564 5f6d 6573 7361 6765 3a20  topped_message: 
+00018870: 4d65 7373 6167 6520 746f 2070 7269 6e74  Message to print
+00018880: 2069 6620 7468 6520 636f 6e74 726f 6c6c   if the controll
+00018890: 6572 2069 7320 5354 4f50 5045 442e 0a20  er is STOPPED.. 
+000188a0: 2020 2020 2020 206e 6f6e 5f65 7869 7374         non_exist
+000188b0: 656e 745f 6d65 7373 6167 653a 204d 6573  ent_message: Mes
+000188c0: 7361 6765 2074 6f20 7368 6f77 2069 6620  sage to show if 
+000188d0: 7468 6520 636f 6e74 726f 6c6c 6572 2064  the controller d
+000188e0: 6f65 7320 6e6f 7420 6578 6973 742e 0a20  oes not exist.. 
+000188f0: 2020 2020 2020 2065 7869 745f 6966 5f6e         exit_if_n
+00018900: 6f74 5f61 6363 6573 7369 626c 653a 2057  ot_accessible: W
+00018910: 6865 7468 6572 2074 6f20 6578 6974 2064  hether to exit d
+00018920: 6972 6563 746c 7920 6966 2074 6865 2063  irectly if the c
+00018930: 6f6e 7472 6f6c 6c65 7220 6973 206e 6f74  ontroller is not
+00018940: 0a20 2020 2020 2020 2020 2061 6363 6573  .          acces
+00018950: 7369 626c 652e 2049 6620 4661 6c73 652c  sible. If False,
+00018960: 2074 6865 2066 756e 6374 696f 6e20 7769   the function wi
+00018970: 6c6c 2072 6169 7365 2043 6c75 7374 6572  ll raise Cluster
+00018980: 4e6f 7455 7045 7272 6f72 2e0a 0a20 2020  NotUpError...   
+00018990: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+000189a0: 2020 6861 6e64 6c65 3a20 5468 6520 5265    handle: The Re
+000189b0: 736f 7572 6365 4861 6e64 6c65 206f 6620  sourceHandle of 
+000189c0: 7468 6520 636f 6e74 726f 6c6c 6572 2e0a  the controller..
+000189d0: 0a20 2020 2052 6169 7365 733a 0a20 2020  .    Raises:.   
+000189e0: 2020 2020 2065 7863 6570 7469 6f6e 732e       exceptions.
+000189f0: 436c 7573 7465 724f 776e 6572 4964 656e  ClusterOwnerIden
+00018a00: 7469 7479 4d69 736d 6174 6368 4572 726f  tityMismatchErro
+00018a10: 723a 2069 6620 7468 6520 6375 7272 656e  r: if the curren
+00018a20: 7420 7573 6572 2069 7320 6e6f 740a 2020  t user is not.  
+00018a30: 2020 2020 2020 2020 7468 6520 7361 6d65          the same
+00018a40: 2061 7320 7468 6520 7573 6572 2077 686f   as the user who
+00018a50: 2063 7265 6174 6564 2074 6865 2063 6c75   created the clu
+00018a60: 7374 6572 2e0a 2020 2020 2020 2020 6578  ster..        ex
+00018a70: 6365 7074 696f 6e73 2e43 6c6f 7564 5573  ceptions.CloudUs
+00018a80: 6572 4964 656e 7469 7479 4572 726f 723a  erIdentityError:
+00018a90: 2069 6620 7765 2066 6169 6c20 746f 2067   if we fail to g
+00018aa0: 6574 2074 6865 2063 7572 7265 6e74 2075  et the current u
+00018ab0: 7365 720a 2020 2020 2020 2020 2020 6964  ser.          id
+00018ac0: 656e 7469 7479 2e0a 2020 2020 2020 2020  entity..        
+00018ad0: 6578 6365 7074 696f 6e73 2e43 6c75 7374  exceptions.Clust
+00018ae0: 6572 4e6f 7455 7045 7272 6f72 3a20 6966  erNotUpError: if
+00018af0: 2074 6865 2063 6f6e 7472 6f6c 6c65 7220   the controller 
+00018b00: 6973 206e 6f74 2061 6363 6573 7369 626c  is not accessibl
+00018b10: 652c 206f 720a 2020 2020 2020 2020 2020  e, or.          
+00018b20: 6661 696c 6564 2074 6f20 6265 2063 6f6e  failed to be con
+00018b30: 6e65 6374 6564 2e0a 2020 2020 2222 220a  nected..    """.
+00018b40: 2020 2020 6966 206e 6f6e 5f65 7869 7374      if non_exist
+00018b50: 656e 745f 6d65 7373 6167 6520 6973 204e  ent_message is N
+00018b60: 6f6e 653a 0a20 2020 2020 2020 206e 6f6e  one:.        non
+00018b70: 5f65 7869 7374 656e 745f 6d65 7373 6167  _existent_messag
+00018b80: 6520 3d20 636f 6e74 726f 6c6c 6572 2e76  e = controller.v
+00018b90: 616c 7565 2e64 6566 6175 6c74 5f68 696e  alue.default_hin
+00018ba0: 745f 6966 5f6e 6f6e 5f65 7869 7374 656e  t_if_non_existen
+00018bb0: 740a 2020 2020 636c 7573 7465 725f 6e61  t.    cluster_na
+00018bc0: 6d65 203d 2063 6f6e 7472 6f6c 6c65 722e  me = controller.
+00018bd0: 7661 6c75 652e 636c 7573 7465 725f 6e61  value.cluster_na
+00018be0: 6d65 0a20 2020 206e 6565 645f 636f 6e6e  me.    need_conn
+00018bf0: 6563 7469 6f6e 5f63 6865 636b 203d 2046  ection_check = F
+00018c00: 616c 7365 0a20 2020 2063 6f6e 7472 6f6c  alse.    control
+00018c10: 6c65 725f 7374 6174 7573 2c20 6861 6e64  ler_status, hand
+00018c20: 6c65 203d 204e 6f6e 652c 204e 6f6e 650a  le = None, None.
+00018c30: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00018c40: 2023 2053 6574 2066 6f72 6365 5f72 6566   # Set force_ref
+00018c50: 7265 7368 5f73 7461 7475 7365 733d 5b49  resh_statuses=[I
+00018c60: 4e49 545d 2074 6f20 6d61 6b65 2073 7572  NIT] to make sur
+00018c70: 6520 7468 6520 7265 6672 6573 6820 6861  e the refresh ha
+00018c80: 7070 656e 730a 2020 2020 2020 2020 2320  ppens.        # 
+00018c90: 7768 656e 2074 6865 2063 6f6e 7472 6f6c  when the control
+00018ca0: 6c65 7220 6973 2049 4e49 542f 5550 2028  ler is INIT/UP (
+00018cb0: 7472 6967 6765 7265 6420 696e 2074 6865  triggered in the
+00018cc0: 7365 2073 7461 7475 7365 7320 6173 2074  se statuses as t
+00018cd0: 6865 0a20 2020 2020 2020 2023 2061 7574  he.        # aut
+00018ce0: 6f73 746f 7020 6973 2061 6c77 6179 7320  ostop is always 
+00018cf0: 7365 7420 666f 7220 7468 6520 636f 6e74  set for the cont
+00018d00: 726f 6c6c 6572 292e 2054 6865 2063 6f6e  roller). The con
+00018d10: 7472 6f6c 6c65 7220 6361 6e20 6265 2069  troller can be i
+00018d20: 6e0a 2020 2020 2020 2020 2320 666f 6c6c  n.        # foll
+00018d30: 6f77 696e 6720 6361 7365 733a 0a20 2020  owing cases:.   
+00018d40: 2020 2020 2023 202a 2028 5550 2c20 6175       # * (UP, au
+00018d50: 746f 7374 6f70 2073 6574 293a 2069 7420  tostop set): it 
+00018d60: 7769 6c6c 2062 6520 7265 6672 6573 6865  will be refreshe
+00018d70: 6420 7769 7468 6f75 7420 666f 7263 655f  d without force_
+00018d80: 7265 6672 6573 6820 7365 742e 0a20 2020  refresh set..   
+00018d90: 2020 2020 2023 202a 2028 5550 2c20 6e6f       # * (UP, no
+00018da0: 2061 7574 6f73 746f 7029 3a20 7665 7279   autostop): very
+00018db0: 2072 6172 6520 2861 2075 7365 7220 6374   rare (a user ct
+00018dc0: 726c 2d63 2077 6865 6e20 7468 6520 636f  rl-c when the co
+00018dd0: 6e74 726f 6c6c 6572 2069 730a 2020 2020  ntroller is.    
+00018de0: 2020 2020 2320 2020 6c61 756e 6368 696e      #   launchin
+00018df0: 6729 2c20 646f 6573 206e 6f74 206d 6174  g), does not mat
+00018e00: 7465 7220 6966 2072 6566 7265 7368 206f  ter if refresh o
+00018e10: 7220 6e6f 742c 2073 696e 6365 206e 6f20  r not, since no 
+00018e20: 6175 746f 7374 6f70 2e20 5765 0a20 2020  autostop. We.   
+00018e30: 2020 2020 2023 2020 2064 6f6e 2774 2069       #   don't i
+00018e40: 6e63 6c75 6465 2055 5020 696e 2066 6f72  nclude UP in for
+00018e50: 6365 5f72 6566 7265 7368 5f73 7461 7475  ce_refresh_statu
+00018e60: 7365 7320 746f 2061 766f 6964 206f 7665  ses to avoid ove
+00018e70: 7268 6561 6473 2e0a 2020 2020 2020 2020  rheads..        
+00018e80: 2320 2a20 2849 4e49 542c 2061 7574 6f73  # * (INIT, autos
+00018e90: 746f 7020 7365 7429 0a20 2020 2020 2020  top set).       
+00018ea0: 2023 202a 2028 494e 4954 2c20 6e6f 2061   # * (INIT, no a
+00018eb0: 7574 6f73 746f 7029 3a20 7665 7279 2072  utostop): very r
+00018ec0: 6172 6520 285f 7570 6461 7465 5f63 6c75  are (_update_clu
+00018ed0: 7374 6572 5f73 7461 7475 735f 6e6f 5f6c  ster_status_no_l
+00018ee0: 6f63 6b20 6d61 790a 2020 2020 2020 2020  ock may.        
+00018ef0: 2320 2020 7265 7365 7420 6c6f 6361 6c20  #   reset local 
+00018f00: 6175 746f 7374 6f70 2063 6f6e 6669 6729  autostop config)
+00018f10: 2c20 6275 7420 666f 7263 655f 7265 6672  , but force_refr
+00018f20: 6573 6820 7769 6c6c 206d 616b 6520 7375  esh will make su
+00018f30: 7265 0a20 2020 2020 2020 2023 2020 2073  re.        #   s
+00018f40: 7461 7475 7320 6973 2072 6566 7265 7368  tatus is refresh
+00018f50: 6564 2e0a 2020 2020 2020 2020 230a 2020  ed..        #.  
+00018f60: 2020 2020 2020 2320 5765 2061 766f 6964        # We avoid
+00018f70: 7320 756e 6e65 6365 7373 6172 7920 636f  s unnecessary co
+00018f80: 7374 6c79 2072 6566 7265 7368 2077 6865  stly refresh whe
+00018f90: 6e20 7468 6520 636f 6e74 726f 6c6c 6572  n the controller
+00018fa0: 2069 7320 616c 7265 6164 790a 2020 2020   is already.    
+00018fb0: 2020 2020 2320 5354 4f50 5045 442e 2054      # STOPPED. T
+00018fc0: 6869 7320 6f70 7469 6d69 7a61 7469 6f6e  his optimization
+00018fd0: 2069 7320 6261 7365 6420 6f6e 2074 6865   is based on the
+00018fe0: 2061 7373 756d 7074 696f 6e20 7468 6174   assumption that
+00018ff0: 2074 6865 2075 7365 720a 2020 2020 2020   the user.      
+00019000: 2020 2320 7769 6c6c 206e 6f74 2073 7461    # will not sta
+00019010: 7274 2074 6865 2063 6f6e 7472 6f6c 6c65  rt the controlle
+00019020: 7220 6d61 6e75 616c 6c79 2066 726f 6d20  r manually from 
+00019030: 7468 6520 636c 6f75 6420 636f 6e73 6f6c  the cloud consol
+00019040: 652e 0a20 2020 2020 2020 2023 0a20 2020  e..        #.   
+00019050: 2020 2020 2023 2054 6865 2061 6371 7569       # The acqui
+00019060: 7265 5f6c 6f63 6b5f 7469 6d65 6f75 7420  re_lock_timeout 
+00019070: 6973 2073 6574 2074 6f20 3020 746f 2061  is set to 0 to a
+00019080: 766f 6964 2068 616e 6769 6e67 2074 6865  void hanging the
+00019090: 2063 6f6d 6d61 6e64 2077 6865 6e0a 2020   command when.  
+000190a0: 2020 2020 2020 2320 6d75 6c74 6970 6c65        # multiple
+000190b0: 206a 6f62 732e 6c61 756e 6368 2063 6f6d   jobs.launch com
+000190c0: 6d61 6e64 7320 6172 6520 7275 6e6e 696e  mands are runnin
+000190d0: 6720 6174 2074 6865 2073 616d 6520 7469  g at the same ti
+000190e0: 6d65 2e20 4f75 7220 6c61 7465 720a 2020  me. Our later.  
+000190f0: 2020 2020 2020 2320 636f 6465 2077 696c        # code wil
+00019100: 6c20 6368 6563 6b20 6966 2074 6865 2063  l check if the c
+00019110: 6f6e 7472 6f6c 6c65 7220 6973 2061 6363  ontroller is acc
+00019120: 6573 7369 626c 6520 6279 2064 6972 6563  essible by direc
+00019130: 746c 7920 6368 6563 6b69 6e67 0a20 2020  tly checking.   
+00019140: 2020 2020 2023 2074 6865 2073 7368 2063       # the ssh c
+00019150: 6f6e 6e65 6374 696f 6e20 746f 2074 6865  onnection to the
+00019160: 2063 6f6e 7472 6f6c 6c65 722c 2069 6620   controller, if 
+00019170: 6974 2066 6169 6c73 2074 6f20 6765 7420  it fails to get 
+00019180: 6163 6375 7261 7465 0a20 2020 2020 2020  accurate.       
+00019190: 2023 2073 7461 7475 7320 6f66 2074 6865   # status of the
+000191a0: 2063 6f6e 7472 6f6c 6c65 722e 0a20 2020   controller..   
+000191b0: 2020 2020 2063 6f6e 7472 6f6c 6c65 725f       controller_
+000191c0: 7374 6174 7573 2c20 6861 6e64 6c65 203d  status, handle =
+000191d0: 2072 6566 7265 7368 5f63 6c75 7374 6572   refresh_cluster
+000191e0: 5f73 7461 7475 735f 6861 6e64 6c65 280a  _status_handle(.
+000191f0: 2020 2020 2020 2020 2020 2020 636c 7573              clus
+00019200: 7465 725f 6e61 6d65 2c0a 2020 2020 2020  ter_name,.      
+00019210: 2020 2020 2020 666f 7263 655f 7265 6672        force_refr
+00019220: 6573 685f 7374 6174 7573 6573 3d5b 7374  esh_statuses=[st
+00019230: 6174 7573 5f6c 6962 2e43 6c75 7374 6572  atus_lib.Cluster
+00019240: 5374 6174 7573 2e49 4e49 545d 2c0a 2020  Status.INIT],.  
+00019250: 2020 2020 2020 2020 2020 636c 7573 7465            cluste
+00019260: 725f 7374 6174 7573 5f6c 6f63 6b5f 7469  r_status_lock_ti
+00019270: 6d65 6f75 743d 3029 0a20 2020 2065 7863  meout=0).    exc
+00019280: 6570 7420 6578 6365 7074 696f 6e73 2e43  ept exceptions.C
+00019290: 6c75 7374 6572 5374 6174 7573 4665 7463  lusterStatusFetc
+000192a0: 6869 6e67 4572 726f 7220 6173 2065 3a0a  hingError as e:.
+000192b0: 2020 2020 2020 2020 2320 5765 2064 6f20          # We do 
+000192c0: 6e6f 7420 6361 7463 6820 7468 6520 6578  not catch the ex
+000192d0: 6365 7074 696f 6e73 2072 656c 6174 6564  ceptions related
+000192e0: 2074 6f20 7468 6520 636c 7573 7465 7220   to the cluster 
+000192f0: 6f77 6e65 7220 6964 656e 7469 7479 0a20  owner identity. 
+00019300: 2020 2020 2020 2023 206d 6973 6d61 7463         # mismatc
+00019310: 682c 2070 6c65 6173 6520 7265 6665 7220  h, please refer 
+00019320: 746f 2074 6865 2063 6f6d 6d65 6e74 2069  to the comment i
+00019330: 6e0a 2020 2020 2020 2020 2320 6062 6163  n.        # `bac
+00019340: 6b65 6e64 5f75 7469 6c73 2e63 6865 636b  kend_utils.check
+00019350: 5f63 6c75 7374 6572 5f61 7661 696c 6162  _cluster_availab
+00019360: 6c65 602e 0a20 2020 2020 2020 2063 6f6e  le`..        con
+00019370: 7472 6f6c 6c65 725f 6e61 6d65 203d 2063  troller_name = c
+00019380: 6f6e 7472 6f6c 6c65 722e 7661 6c75 652e  ontroller.value.
+00019390: 6e61 6d65 2e72 6570 6c61 6365 2827 2063  name.replace(' c
+000193a0: 6f6e 7472 6f6c 6c65 7227 2c20 2727 290a  ontroller', '').
+000193b0: 2020 2020 2020 2020 6c6f 6767 6572 2e77          logger.w
+000193c0: 6172 6e69 6e67 280a 2020 2020 2020 2020  arning(.        
+000193d0: 2020 2020 2746 6169 6c65 6420 746f 2067      'Failed to g
+000193e0: 6574 2074 6865 2073 7461 7475 7320 6f66  et the status of
+000193f0: 2074 6865 2063 6f6e 7472 6f6c 6c65 722e   the controller.
+00019400: 2049 7420 6973 206e 6f74 2027 0a20 2020   It is not '.   
+00019410: 2020 2020 2020 2020 2066 2766 6174 616c           f'fatal
+00019420: 2c20 6275 7420 7b63 6f6e 7472 6f6c 6c65  , but {controlle
+00019430: 725f 6e61 6d65 7d20 636f 6d6d 616e 6473  r_name} commands
+00019440: 2f63 616c 6c73 206d 6179 2068 616e 6720  /calls may hang 
+00019450: 6f72 2072 6574 7572 6e20 270a 2020 2020  or return '.    
+00019460: 2020 2020 2020 2020 2773 7461 6c65 2069          'stale i
+00019470: 6e66 6f72 6d61 7469 6f6e 2c20 7768 656e  nformation, when
+00019480: 2074 6865 2063 6f6e 7472 6f6c 6c65 7220   the controller 
+00019490: 6973 206e 6f74 2075 702e 5c6e 270a 2020  is not up.\n'.  
+000194a0: 2020 2020 2020 2020 2020 6627 2020 4465            f'  De
+000194b0: 7461 696c 733a 207b 636f 6d6d 6f6e 5f75  tails: {common_u
+000194c0: 7469 6c73 2e66 6f72 6d61 745f 6578 6365  tils.format_exce
+000194d0: 7074 696f 6e28 652c 2075 7365 5f62 7261  ption(e, use_bra
+000194e0: 636b 6574 3d54 7275 6529 7d27 290a 2020  cket=True)}').  
+000194f0: 2020 2020 2020 7265 636f 7264 203d 2067        record = g
+00019500: 6c6f 6261 6c5f 7573 6572 5f73 7461 7465  lobal_user_state
+00019510: 2e67 6574 5f63 6c75 7374 6572 5f66 726f  .get_cluster_fro
+00019520: 6d5f 6e61 6d65 2863 6c75 7374 6572 5f6e  m_name(cluster_n
+00019530: 616d 6529 0a20 2020 2020 2020 2069 6620  ame).        if 
+00019540: 7265 636f 7264 2069 7320 6e6f 7420 4e6f  record is not No
+00019550: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00019560: 636f 6e74 726f 6c6c 6572 5f73 7461 7475  controller_statu
+00019570: 732c 2068 616e 646c 6520 3d20 7265 636f  s, handle = reco
+00019580: 7264 5b27 7374 6174 7573 275d 2c20 7265  rd['status'], re
+00019590: 636f 7264 5b27 6861 6e64 6c65 275d 0a20  cord['handle']. 
+000195a0: 2020 2020 2020 2020 2020 2023 2057 6520             # We 
+000195b0: 6368 6563 6b20 7468 6520 636f 6e6e 6563  check the connec
+000195c0: 7469 6f6e 2065 7665 6e20 6966 2074 6865  tion even if the
+000195d0: 2063 6c75 7374 6572 2068 6173 2061 2063   cluster has a c
+000195e0: 6163 6865 6420 7374 6174 7573 2055 500a  ached status UP.
+000195f0: 2020 2020 2020 2020 2020 2020 2320 746f              # to
+00019600: 206d 616b 6520 7375 7265 2074 6865 2063   make sure the c
+00019610: 6f6e 7472 6f6c 6c65 7220 6973 2061 6374  ontroller is act
+00019620: 7561 6c6c 7920 6163 6365 7373 6962 6c65  ually accessible
+00019630: 2c20 6173 2074 6865 2063 6163 6865 640a  , as the cached.
+00019640: 2020 2020 2020 2020 2020 2020 2320 7374              # st
+00019650: 6174 7573 206d 6967 6874 2062 6520 7374  atus might be st
+00019660: 616c 652e 0a20 2020 2020 2020 2020 2020  ale..           
+00019670: 206e 6565 645f 636f 6e6e 6563 7469 6f6e   need_connection
+00019680: 5f63 6865 636b 203d 2054 7275 650a 0a20  _check = True.. 
+00019690: 2020 2065 7272 6f72 5f6d 7367 203d 204e     error_msg = N
+000196a0: 6f6e 650a 2020 2020 6966 2063 6f6e 7472  one.    if contr
+000196b0: 6f6c 6c65 725f 7374 6174 7573 203d 3d20  oller_status == 
+000196c0: 7374 6174 7573 5f6c 6962 2e43 6c75 7374  status_lib.Clust
+000196d0: 6572 5374 6174 7573 2e53 544f 5050 4544  erStatus.STOPPED
+000196e0: 3a0a 2020 2020 2020 2020 6572 726f 725f  :.        error_
+000196f0: 6d73 6720 3d20 7374 6f70 7065 645f 6d65  msg = stopped_me
+00019700: 7373 6167 650a 2020 2020 656c 6966 2063  ssage.    elif c
+00019710: 6f6e 7472 6f6c 6c65 725f 7374 6174 7573  ontroller_status
+00019720: 2069 7320 4e6f 6e65 206f 7220 6861 6e64   is None or hand
+00019730: 6c65 2069 7320 4e6f 6e65 206f 7220 6861  le is None or ha
+00019740: 6e64 6c65 2e68 6561 645f 6970 2069 7320  ndle.head_ip is 
+00019750: 4e6f 6e65 3a0a 2020 2020 2020 2020 2320  None:.        # 
+00019760: 5765 2063 6865 636b 2074 6865 2063 6f6e  We check the con
+00019770: 7472 6f6c 6c65 7220 6973 2053 544f 5050  troller is STOPP
+00019780: 4544 2062 6566 6f72 6520 7468 6520 6368  ED before the ch
+00019790: 6563 6b20 666f 7220 6861 6e64 6c65 2e68  eck for handle.h
+000197a0: 6561 645f 6970 0a20 2020 2020 2020 2023  ead_ip.        #
+000197b0: 204e 6f6e 6520 6265 6361 7573 6520 7768   None because wh
+000197c0: 656e 2074 6865 2063 6f6e 7472 6f6c 6c65  en the controlle
+000197d0: 7220 6973 2053 544f 5050 4544 2c20 6861  r is STOPPED, ha
+000197e0: 6e64 6c65 2e68 6561 645f 6970 2063 616e  ndle.head_ip can
+000197f0: 2061 6c73 6f0a 2020 2020 2020 2020 2320   also.        # 
+00019800: 6265 204e 6f6e 652c 2062 7574 2077 6520  be None, but we 
+00019810: 6f6e 6c79 2077 616e 7420 746f 2063 6174  only want to cat
+00019820: 6368 2074 6865 2063 6173 6520 7768 656e  ch the case when
+00019830: 2074 6865 2063 6f6e 7472 6f6c 6c65 7220   the controller 
+00019840: 6973 0a20 2020 2020 2020 2023 2062 6569  is.        # bei
+00019850: 6e67 2070 726f 7669 7369 6f6e 6564 2061  ng provisioned a
+00019860: 7420 7468 6520 6669 7273 7420 7469 6d65  t the first time
+00019870: 2061 6e64 2068 6176 6520 6e6f 2068 6561   and have no hea
+00019880: 645f 6970 2e0a 2020 2020 2020 2020 6572  d_ip..        er
+00019890: 726f 725f 6d73 6720 3d20 6e6f 6e5f 6578  ror_msg = non_ex
+000198a0: 6973 7465 6e74 5f6d 6573 7361 6765 0a20  istent_message. 
+000198b0: 2020 2065 6c69 6620 2863 6f6e 7472 6f6c     elif (control
+000198c0: 6c65 725f 7374 6174 7573 203d 3d20 7374  ler_status == st
+000198d0: 6174 7573 5f6c 6962 2e43 6c75 7374 6572  atus_lib.Cluster
+000198e0: 5374 6174 7573 2e49 4e49 5420 6f72 0a20  Status.INIT or. 
+000198f0: 2020 2020 2020 2020 206e 6565 645f 636f           need_co
+00019900: 6e6e 6563 7469 6f6e 5f63 6865 636b 293a  nnection_check):
+00019910: 0a20 2020 2020 2020 2023 2043 6865 636b  .        # Check
+00019920: 2073 7368 2063 6f6e 6e65 6374 696f 6e20   ssh connection 
+00019930: 6966 2028 3129 2063 6f6e 7472 6f6c 6c65  if (1) controlle
+00019940: 7220 6973 2069 6e20 494e 4954 2073 7461  r is in INIT sta
+00019950: 7465 2c20 6f72 2028 3229 2077 6520 6661  te, or (2) we fa
+00019960: 696c 6564 2074 6f20 6665 7463 6820 7468  iled to fetch th
+00019970: 650a 2020 2020 2020 2020 2320 7374 6174  e.        # stat
+00019980: 7573 2c20 626f 7468 206f 6620 7768 6963  us, both of whic
+00019990: 6820 6361 6e20 6861 7070 656e 2077 6865  h can happen whe
+000199a0: 6e20 636f 6e74 726f 6c6c 6572 2773 2073  n controller's s
+000199b0: 7461 7475 7320 6c6f 636b 2069 7320 6865  tatus lock is he
+000199c0: 6c64 2062 7920 616e 6f74 6865 7220 6073  ld by another `s
+000199d0: 6b79 206a 6f62 7320 6c61 756e 6368 6020  ky jobs launch` 
+000199e0: 6f72 0a20 2020 2020 2020 2023 2060 736b  or.        # `sk
+000199f0: 7920 7365 7276 6520 7570 602e 2049 6620  y serve up`. If 
+00019a00: 7765 2068 6176 65c2 a063 6f6e 7472 6f6c  we have..control
+00019a10: 6c65 7227 7320 6865 6164 5f69 7020 6176  ler's head_ip av
+00019a20: 6169 6c61 626c 6520 616e 6420 6974 2069  ailable and it i
+00019a30: 7320 7373 682d 7265 6163 6861 626c 652c  s ssh-reachable,
+00019a40: 0a20 2020 2020 2020 2023 2077 6520 6361  .        # we ca
+00019a50: 6e20 616c 6c6f 7720 6163 6365 7373 2074  n allow access t
+00019a60: 6f20 7468 6520 636f 6e74 726f 6c6c 6572  o the controller
+00019a70: 2e0a 2020 2020 2020 2020 7373 685f 6372  ..        ssh_cr
+00019a80: 6564 656e 7469 616c 7320 3d20 7373 685f  edentials = ssh_
+00019a90: 6372 6564 656e 7469 616c 5f66 726f 6d5f  credential_from_
+00019aa0: 7961 6d6c 2868 616e 646c 652e 636c 7573  yaml(handle.clus
+00019ab0: 7465 725f 7961 6d6c 2c0a 2020 2020 2020  ter_yaml,.      
 00019ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019ad0: 2020 2020 2068 616e 646c 652e 646f 636b       handle.dock
-00019ae0: 6572 5f75 7365 722c 0a20 2020 2020 2020  er_user,.       
-00019af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019b10: 2020 2020 2020 2020 2020 2020 6861 6e64              hand
-00019b20: 6c65 2e73 7368 5f75 7365 7229 0a0a 2020  le.ssh_user)..  
-00019b30: 2020 2020 2020 7275 6e6e 6572 203d 2063        runner = c
-00019b40: 6f6d 6d61 6e64 5f72 756e 6e65 722e 5353  ommand_runner.SS
-00019b50: 4843 6f6d 6d61 6e64 5275 6e6e 6572 286e  HCommandRunner(n
-00019b60: 6f64 653d 2868 616e 646c 652e 6865 6164  ode=(handle.head
-00019b70: 5f69 702c 0a20 2020 2020 2020 2020 2020  _ip,.           
-00019b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019ae0: 2020 2020 2020 2020 2020 2020 2068 616e               han
+00019af0: 646c 652e 646f 636b 6572 5f75 7365 722c  dle.docker_user,
+00019b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b30: 2020 2020 6861 6e64 6c65 2e73 7368 5f75      handle.ssh_u
+00019b40: 7365 7229 0a0a 2020 2020 2020 2020 7275  ser)..        ru
+00019b50: 6e6e 6572 203d 2063 6f6d 6d61 6e64 5f72  nner = command_r
+00019b60: 756e 6e65 722e 5353 4843 6f6d 6d61 6e64  unner.SSHCommand
+00019b70: 5275 6e6e 6572 286e 6f64 653d 2868 616e  Runner(node=(han
+00019b80: 646c 652e 6865 6164 5f69 702c 0a20 2020  dle.head_ip,.   
 00019b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019ba0: 2020 2020 2020 2020 2020 2020 6861 6e64              hand
-00019bb0: 6c65 2e68 6561 645f 7373 685f 706f 7274  le.head_ssh_port
-00019bc0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00019bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019bc0: 2020 2020 6861 6e64 6c65 2e68 6561 645f      handle.head_
+00019bd0: 7373 685f 706f 7274 292c 0a20 2020 2020  ssh_port),.     
 00019be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019bf0: 2020 2020 2a2a 7373 685f 6372 6564 656e      **ssh_creden
-00019c00: 7469 616c 7329 0a20 2020 2020 2020 2069  tials).        i
-00019c10: 6620 6e6f 7420 7275 6e6e 6572 2e63 6865  f not runner.che
-00019c20: 636b 5f63 6f6e 6e65 6374 696f 6e28 293a  ck_connection():
-00019c30: 0a20 2020 2020 2020 2020 2020 2065 7272  .            err
-00019c40: 6f72 5f6d 7367 203d 2063 6f6e 7472 6f6c  or_msg = control
-00019c50: 6c65 722e 7661 6c75 652e 636f 6e6e 6563  ler.value.connec
-00019c60: 7469 6f6e 5f65 7272 6f72 5f68 696e 740a  tion_error_hint.
-00019c70: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00019c80: 2020 6173 7365 7274 2063 6f6e 7472 6f6c    assert control
-00019c90: 6c65 725f 7374 6174 7573 203d 3d20 7374  ler_status == st
-00019ca0: 6174 7573 5f6c 6962 2e43 6c75 7374 6572  atus_lib.Cluster
-00019cb0: 5374 6174 7573 2e55 502c 2068 616e 646c  Status.UP, handl
-00019cc0: 650a 0a20 2020 2069 6620 6572 726f 725f  e..    if error_
-00019cd0: 6d73 6720 6973 206e 6f74 204e 6f6e 653a  msg is not None:
-00019ce0: 0a20 2020 2020 2020 2069 6620 6578 6974  .        if exit
-00019cf0: 5f69 665f 6e6f 745f 6163 6365 7373 6962  _if_not_accessib
-00019d00: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
-00019d10: 736b 795f 6c6f 6767 696e 672e 7072 696e  sky_logging.prin
-00019d20: 7428 6572 726f 725f 6d73 6729 0a20 2020  t(error_msg).   
-00019d30: 2020 2020 2020 2020 2073 7973 2e65 7869           sys.exi
-00019d40: 7428 3129 0a20 2020 2020 2020 2077 6974  t(1).        wit
-00019d50: 6820 7578 5f75 7469 6c73 2e70 7269 6e74  h ux_utils.print
-00019d60: 5f65 7863 6570 7469 6f6e 5f6e 6f5f 7472  _exception_no_tr
-00019d70: 6163 6562 6163 6b28 293a 0a20 2020 2020  aceback():.     
-00019d80: 2020 2020 2020 2072 6169 7365 2065 7863         raise exc
-00019d90: 6570 7469 6f6e 732e 436c 7573 7465 724e  eptions.ClusterN
-00019da0: 6f74 5570 4572 726f 7228 6572 726f 725f  otUpError(error_
-00019db0: 6d73 672c 0a20 2020 2020 2020 2020 2020  msg,.           
-00019dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019c00: 2020 2020 2020 2020 2020 2020 2a2a 7373              **ss
+00019c10: 685f 6372 6564 656e 7469 616c 7329 0a20  h_credentials). 
+00019c20: 2020 2020 2020 2069 6620 6e6f 7420 7275         if not ru
+00019c30: 6e6e 6572 2e63 6865 636b 5f63 6f6e 6e65  nner.check_conne
+00019c40: 6374 696f 6e28 293a 0a20 2020 2020 2020  ction():.       
+00019c50: 2020 2020 2065 7272 6f72 5f6d 7367 203d       error_msg =
+00019c60: 2063 6f6e 7472 6f6c 6c65 722e 7661 6c75   controller.valu
+00019c70: 652e 636f 6e6e 6563 7469 6f6e 5f65 7272  e.connection_err
+00019c80: 6f72 5f68 696e 740a 2020 2020 656c 7365  or_hint.    else
+00019c90: 3a0a 2020 2020 2020 2020 6173 7365 7274  :.        assert
+00019ca0: 2063 6f6e 7472 6f6c 6c65 725f 7374 6174   controller_stat
+00019cb0: 7573 203d 3d20 7374 6174 7573 5f6c 6962  us == status_lib
+00019cc0: 2e43 6c75 7374 6572 5374 6174 7573 2e55  .ClusterStatus.U
+00019cd0: 502c 2068 616e 646c 650a 0a20 2020 2069  P, handle..    i
+00019ce0: 6620 6572 726f 725f 6d73 6720 6973 206e  f error_msg is n
+00019cf0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00019d00: 2069 6620 6578 6974 5f69 665f 6e6f 745f   if exit_if_not_
+00019d10: 6163 6365 7373 6962 6c65 3a0a 2020 2020  accessible:.    
+00019d20: 2020 2020 2020 2020 736b 795f 6c6f 6767          sky_logg
+00019d30: 696e 672e 7072 696e 7428 6572 726f 725f  ing.print(error_
+00019d40: 6d73 6729 0a20 2020 2020 2020 2020 2020  msg).           
+00019d50: 2073 7973 2e65 7869 7428 3129 0a20 2020   sys.exit(1).   
+00019d60: 2020 2020 2077 6974 6820 7578 5f75 7469       with ux_uti
+00019d70: 6c73 2e70 7269 6e74 5f65 7863 6570 7469  ls.print_excepti
+00019d80: 6f6e 5f6e 6f5f 7472 6163 6562 6163 6b28  on_no_traceback(
+00019d90: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+00019da0: 6169 7365 2065 7863 6570 7469 6f6e 732e  aise exceptions.
+00019db0: 436c 7573 7465 724e 6f74 5570 4572 726f  ClusterNotUpErro
+00019dc0: 7228 6572 726f 725f 6d73 672c 0a20 2020  r(error_msg,.   
 00019dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019de0: 2020 2020 636c 7573 7465 725f 7374 6174      cluster_stat
-00019df0: 7573 3d63 6f6e 7472 6f6c 6c65 725f 7374  us=controller_st
-00019e00: 6174 7573 2c0a 2020 2020 2020 2020 2020  atus,.          
-00019e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019df0: 2020 2020 2020 2020 2020 2020 636c 7573              clus
+00019e00: 7465 725f 7374 6174 7573 3d63 6f6e 7472  ter_status=contr
+00019e10: 6f6c 6c65 725f 7374 6174 7573 2c0a 2020  oller_status,.  
 00019e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019e30: 2020 2020 2068 616e 646c 653d 6861 6e64       handle=hand
-00019e40: 6c65 290a 2020 2020 6173 7365 7274 2068  le).    assert h
-00019e50: 616e 646c 6520 6973 206e 6f74 204e 6f6e  andle is not Non
-00019e60: 6520 616e 6420 6861 6e64 6c65 2e68 6561  e and handle.hea
-00019e70: 645f 6970 2069 7320 6e6f 7420 4e6f 6e65  d_ip is not None
-00019e80: 2c20 280a 2020 2020 2020 2020 6861 6e64  , (.        hand
-00019e90: 6c65 2c20 636f 6e74 726f 6c6c 6572 5f73  le, controller_s
-00019ea0: 7461 7475 7329 0a20 2020 2072 6574 7572  tatus).    retur
-00019eb0: 6e20 6861 6e64 6c65 0a0a 0a63 6c61 7373  n handle...class
-00019ec0: 2043 6c6f 7564 4669 6c74 6572 2865 6e75   CloudFilter(enu
-00019ed0: 6d2e 456e 756d 293a 0a20 2020 2023 2046  m.Enum):.    # F
-00019ee0: 696c 7465 7220 666f 7220 616c 6c20 7479  ilter for all ty
-00019ef0: 7065 7320 6f66 2063 6c6f 7564 732e 0a20  pes of clouds.. 
-00019f00: 2020 2041 4c4c 203d 2027 616c 6c27 0a20     ALL = 'all'. 
-00019f10: 2020 2023 2046 696c 7465 7220 666f 7220     # Filter for 
-00019f20: 536b 7927 7320 6d61 696e 2063 6c6f 7564  Sky's main cloud
-00019f30: 7320 2861 7773 2c20 6763 702c 2061 7a75  s (aws, gcp, azu
-00019f40: 7265 2c20 646f 636b 6572 292e 0a20 2020  re, docker)..   
-00019f50: 2043 4c4f 5544 535f 414e 445f 444f 434b   CLOUDS_AND_DOCK
-00019f60: 4552 203d 2027 636c 6f75 6473 2d61 6e64  ER = 'clouds-and
-00019f70: 2d64 6f63 6b65 7227 0a20 2020 2023 2046  -docker'.    # F
-00019f80: 696c 7465 7220 666f 7220 6f6e 6c79 206c  ilter for only l
-00019f90: 6f63 616c 2063 6c6f 7564 732e 0a20 2020  ocal clouds..   
-00019fa0: 204c 4f43 414c 203d 2027 6c6f 6361 6c27   LOCAL = 'local'
-00019fb0: 0a0a 0a64 6566 2067 6574 5f63 6c75 7374  ...def get_clust
-00019fc0: 6572 7328 0a20 2020 2069 6e63 6c75 6465  ers(.    include
-00019fd0: 5f63 6f6e 7472 6f6c 6c65 723a 2062 6f6f  _controller: boo
-00019fe0: 6c2c 0a20 2020 2072 6566 7265 7368 3a20  l,.    refresh: 
-00019ff0: 626f 6f6c 2c0a 2020 2020 636c 7573 7465  bool,.    cluste
-0001a000: 725f 6e61 6d65 733a 204f 7074 696f 6e61  r_names: Optiona
-0001a010: 6c5b 556e 696f 6e5b 7374 722c 204c 6973  l[Union[str, Lis
-0001a020: 745b 7374 725d 5d5d 203d 204e 6f6e 652c  t[str]]] = None,
-0001a030: 0a29 202d 3e20 4c69 7374 5b44 6963 745b  .) -> List[Dict[
-0001a040: 7374 722c 2041 6e79 5d5d 3a0a 2020 2020  str, Any]]:.    
-0001a050: 2222 2252 6574 7572 6e73 2061 206c 6973  """Returns a lis
-0001a060: 7420 6f66 2063 6163 6865 6420 6f72 206f  t of cached or o
-0001a070: 7074 696f 6e61 6c6c 7920 7265 6672 6573  ptionally refres
-0001a080: 6865 6420 636c 7573 7465 7220 7265 636f  hed cluster reco
-0001a090: 7264 732e 0a0a 2020 2020 436f 6d62 7320  rds...    Combs 
-0001a0a0: 7468 726f 7567 6820 7468 6520 6461 7461  through the data
-0001a0b0: 6261 7365 2028 696e 207e 2f2e 736b 792f  base (in ~/.sky/
-0001a0c0: 7374 6174 652e 6462 2920 746f 2067 6574  state.db) to get
-0001a0d0: 2061 206c 6973 7420 6f66 2072 6563 6f72   a list of recor
-0001a0e0: 6473 0a20 2020 2063 6f72 7265 7370 6f6e  ds.    correspon
-0001a0f0: 6469 6e67 2074 6f20 6c61 756e 6368 6564  ding to launched
-0001a100: 2063 6c75 7374 6572 7320 2866 696c 7465   clusters (filte
-0001a110: 7265 6420 6279 2060 636c 7573 7465 725f  red by `cluster_
-0001a120: 6e61 6d65 7360 2069 6620 6974 2069 730a  names` if it is.
-0001a130: 2020 2020 7370 6563 6966 6965 6429 2e20      specified). 
-0001a140: 5468 6520 7265 6672 6573 6820 666c 6167  The refresh flag
-0001a150: 2063 616e 2062 6520 7573 6564 2074 6f20   can be used to 
-0001a160: 666f 7263 6520 6120 7265 6672 6573 6820  force a refresh 
-0001a170: 6f66 2074 6865 2073 7461 7475 730a 2020  of the status.  
-0001a180: 2020 6f66 2074 6865 2063 6c75 7374 6572    of the cluster
-0001a190: 732e 0a0a 2020 2020 4172 6773 3a0a 2020  s...    Args:.  
-0001a1a0: 2020 2020 2020 696e 636c 7564 655f 636f        include_co
-0001a1b0: 6e74 726f 6c6c 6572 3a20 5768 6574 6865  ntroller: Whethe
-0001a1c0: 7220 746f 2069 6e63 6c75 6465 2063 6f6e  r to include con
-0001a1d0: 7472 6f6c 6c65 7273 2c20 652e 672e 206a  trollers, e.g. j
-0001a1e0: 6f62 7320 636f 6e74 726f 6c6c 6572 0a20  obs controller. 
-0001a1f0: 2020 2020 2020 2020 2020 206f 7220 736b             or sk
-0001a200: 7920 7365 7276 6520 636f 6e74 726f 6c6c  y serve controll
-0001a210: 6572 2e0a 2020 2020 2020 2020 7265 6672  er..        refr
-0001a220: 6573 683a 2057 6865 7468 6572 2074 6f20  esh: Whether to 
-0001a230: 7265 6672 6573 6820 7468 6520 7374 6174  refresh the stat
-0001a240: 7573 206f 6620 7468 6520 636c 7573 7465  us of the cluste
-0001a250: 7273 2e20 2852 6566 7265 7368 696e 6720  rs. (Refreshing 
-0001a260: 7769 6c6c 0a20 2020 2020 2020 2020 2020  will.           
-0001a270: 2073 6574 2074 6865 2073 7461 7475 7320   set the status 
-0001a280: 746f 2053 544f 5050 4544 2069 6620 7468  to STOPPED if th
-0001a290: 6520 636c 7573 7465 7220 6361 6e6e 6f74  e cluster cannot
-0001a2a0: 2062 6520 7069 6e67 6564 2e29 0a20 2020   be pinged.).   
-0001a2b0: 2020 2020 2063 6c6f 7564 5f66 696c 7465       cloud_filte
-0001a2c0: 723a 2053 6574 7320 7768 6963 6820 636c  r: Sets which cl
-0001a2d0: 6f75 6473 2074 6f20 6669 6c65 7220 7468  ouds to filer th
-0001a2e0: 726f 7567 6820 6672 6f6d 2074 6865 2067  rough from the g
-0001a2f0: 6c6f 6261 6c20 7573 6572 0a20 2020 2020  lobal user.     
-0001a300: 2020 2020 2020 2073 7461 7465 2e20 5375         state. Su
-0001a310: 7070 6f72 7473 2074 6872 6565 2076 616c  pports three val
-0001a320: 7565 732c 2027 616c 6c27 2066 6f72 2061  ues, 'all' for a
-0001a330: 6c6c 2063 6c6f 7564 732c 2027 7075 626c  ll clouds, 'publ
-0001a340: 6963 2720 666f 720a 2020 2020 2020 2020  ic' for.        
-0001a350: 2020 2020 7075 626c 6963 2063 6c6f 7564      public cloud
-0001a360: 7320 6f6e 6c79 2c20 616e 6420 276c 6f63  s only, and 'loc
-0001a370: 616c 2720 666f 7220 6f6e 6c79 206c 6f63  al' for only loc
-0001a380: 616c 2063 6c6f 7564 732e 0a20 2020 2020  al clouds..     
-0001a390: 2020 2063 6c75 7374 6572 5f6e 616d 6573     cluster_names
-0001a3a0: 3a20 4966 2070 726f 7669 6465 642c 206f  : If provided, o
-0001a3b0: 6e6c 7920 7265 7475 726e 2072 6563 6f72  nly return recor
-0001a3c0: 6473 2066 6f72 2074 6865 2067 6976 656e  ds for the given
-0001a3d0: 2063 6c75 7374 6572 0a20 2020 2020 2020   cluster.       
-0001a3e0: 2020 2020 206e 616d 6573 2e0a 0a20 2020       names...   
-0001a3f0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-0001a400: 2020 4120 6c69 7374 206f 6620 636c 7573    A list of clus
-0001a410: 7465 7220 7265 636f 7264 732e 2049 6620  ter records. If 
-0001a420: 7468 6520 636c 7573 7465 7220 646f 6573  the cluster does
-0001a430: 206e 6f74 2065 7869 7374 206f 7220 6861   not exist or ha
-0001a440: 7320 6265 656e 0a20 2020 2020 2020 2074  s been.        t
-0001a450: 6572 6d69 6e61 7465 642c 2074 6865 2072  erminated, the r
-0001a460: 6563 6f72 6420 7769 6c6c 2062 6520 6f6d  ecord will be om
-0001a470: 6974 7465 6420 6672 6f6d 2074 6865 2072  itted from the r
-0001a480: 6574 7572 6e65 6420 6c69 7374 2e0a 2020  eturned list..  
-0001a490: 2020 2222 220a 2020 2020 7265 636f 7264    """.    record
-0001a4a0: 7320 3d20 676c 6f62 616c 5f75 7365 725f  s = global_user_
-0001a4b0: 7374 6174 652e 6765 745f 636c 7573 7465  state.get_cluste
-0001a4c0: 7273 2829 0a0a 2020 2020 6966 206e 6f74  rs()..    if not
-0001a4d0: 2069 6e63 6c75 6465 5f63 6f6e 7472 6f6c   include_control
-0001a4e0: 6c65 723a 0a20 2020 2020 2020 2072 6563  ler:.        rec
-0001a4f0: 6f72 6473 203d 205b 0a20 2020 2020 2020  ords = [.       
-0001a500: 2020 2020 2072 6563 6f72 6420 666f 7220       record for 
-0001a510: 7265 636f 7264 2069 6e20 7265 636f 7264  record in record
-0001a520: 730a 2020 2020 2020 2020 2020 2020 6966  s.            if
-0001a530: 2063 6f6e 7472 6f6c 6c65 725f 7574 696c   controller_util
-0001a540: 732e 436f 6e74 726f 6c6c 6572 732e 6672  s.Controllers.fr
-0001a550: 6f6d 5f6e 616d 6528 7265 636f 7264 5b27  om_name(record['
-0001a560: 6e61 6d65 275d 2920 6973 204e 6f6e 650a  name']) is None.
-0001a570: 2020 2020 2020 2020 5d0a 0a20 2020 2079          ]..    y
-0001a580: 656c 6c6f 7720 3d20 636f 6c6f 7261 6d61  ellow = colorama
-0001a590: 2e46 6f72 652e 5945 4c4c 4f57 0a20 2020  .Fore.YELLOW.   
-0001a5a0: 2062 7269 6768 7420 3d20 636f 6c6f 7261   bright = colora
-0001a5b0: 6d61 2e53 7479 6c65 2e42 5249 4748 540a  ma.Style.BRIGHT.
-0001a5c0: 2020 2020 7265 7365 7420 3d20 636f 6c6f      reset = colo
-0001a5d0: 7261 6d61 2e53 7479 6c65 2e52 4553 4554  rama.Style.RESET
-0001a5e0: 5f41 4c4c 0a0a 2020 2020 6966 2063 6c75  _ALL..    if clu
-0001a5f0: 7374 6572 5f6e 616d 6573 2069 7320 6e6f  ster_names is no
-0001a600: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0001a610: 6966 2069 7369 6e73 7461 6e63 6528 636c  if isinstance(cl
-0001a620: 7573 7465 725f 6e61 6d65 732c 2073 7472  uster_names, str
-0001a630: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
-0001a640: 6c75 7374 6572 5f6e 616d 6573 203d 205b  luster_names = [
-0001a650: 636c 7573 7465 725f 6e61 6d65 735d 0a20  cluster_names]. 
-0001a660: 2020 2020 2020 206e 6577 5f72 6563 6f72         new_recor
-0001a670: 6473 203d 205b 5d0a 2020 2020 2020 2020  ds = [].        
-0001a680: 6e6f 745f 6578 6973 745f 636c 7573 7465  not_exist_cluste
-0001a690: 725f 6e61 6d65 7320 3d20 5b5d 0a20 2020  r_names = [].   
-0001a6a0: 2020 2020 2066 6f72 2063 6c75 7374 6572       for cluster
-0001a6b0: 5f6e 616d 6520 696e 2063 6c75 7374 6572  _name in cluster
-0001a6c0: 5f6e 616d 6573 3a0a 2020 2020 2020 2020  _names:.        
-0001a6d0: 2020 2020 666f 7220 7265 636f 7264 2069      for record i
-0001a6e0: 6e20 7265 636f 7264 733a 0a20 2020 2020  n records:.     
-0001a6f0: 2020 2020 2020 2020 2020 2069 6620 7265             if re
-0001a700: 636f 7264 5b27 6e61 6d65 275d 203d 3d20  cord['name'] == 
-0001a710: 636c 7573 7465 725f 6e61 6d65 3a0a 2020  cluster_name:.  
-0001a720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a730: 2020 6e65 775f 7265 636f 7264 732e 6170    new_records.ap
-0001a740: 7065 6e64 2872 6563 6f72 6429 0a20 2020  pend(record).   
-0001a750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a760: 2062 7265 616b 0a20 2020 2020 2020 2020   break.         
-0001a770: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0001a780: 2020 2020 2020 2020 206e 6f74 5f65 7869           not_exi
-0001a790: 7374 5f63 6c75 7374 6572 5f6e 616d 6573  st_cluster_names
-0001a7a0: 2e61 7070 656e 6428 636c 7573 7465 725f  .append(cluster_
-0001a7b0: 6e61 6d65 290a 2020 2020 2020 2020 6966  name).        if
-0001a7c0: 206e 6f74 5f65 7869 7374 5f63 6c75 7374   not_exist_clust
-0001a7d0: 6572 5f6e 616d 6573 3a0a 2020 2020 2020  er_names:.      
-0001a7e0: 2020 2020 2020 636c 7573 7465 7273 5f73        clusters_s
-0001a7f0: 7472 203d 2027 2c20 272e 6a6f 696e 286e  tr = ', '.join(n
-0001a800: 6f74 5f65 7869 7374 5f63 6c75 7374 6572  ot_exist_cluster
-0001a810: 5f6e 616d 6573 290a 2020 2020 2020 2020  _names).        
-0001a820: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
-0001a830: 6627 436c 7573 7465 7228 7329 206e 6f74  f'Cluster(s) not
-0001a840: 2066 6f75 6e64 3a20 7b62 7269 6768 747d   found: {bright}
-0001a850: 7b63 6c75 7374 6572 735f 7374 727d 7b72  {clusters_str}{r
-0001a860: 6573 6574 7d2e 2729 0a20 2020 2020 2020  eset}.').       
-0001a870: 2072 6563 6f72 6473 203d 206e 6577 5f72   records = new_r
-0001a880: 6563 6f72 6473 0a0a 2020 2020 6966 206e  ecords..    if n
-0001a890: 6f74 2072 6566 7265 7368 3a0a 2020 2020  ot refresh:.    
-0001a8a0: 2020 2020 7265 7475 726e 2072 6563 6f72      return recor
-0001a8b0: 6473 0a0a 2020 2020 706c 7572 616c 203d  ds..    plural =
-0001a8c0: 2027 7327 2069 6620 6c65 6e28 7265 636f   's' if len(reco
-0001a8d0: 7264 7329 203e 2031 2065 6c73 6520 2727  rds) > 1 else ''
-0001a8e0: 0a20 2020 2070 726f 6772 6573 7320 3d20  .    progress = 
-0001a8f0: 7269 6368 5f70 726f 6772 6573 732e 5072  rich_progress.Pr
-0001a900: 6f67 7265 7373 2874 7261 6e73 6965 6e74  ogress(transient
-0001a910: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
-0001a920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a930: 2020 2020 2020 2020 2020 2020 2072 6564               red
-0001a940: 6972 6563 745f 7374 646f 7574 3d46 616c  irect_stdout=Fal
-0001a950: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-0001a960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a970: 2020 2020 2020 2020 2020 7265 6469 7265            redire
-0001a980: 6374 5f73 7464 6572 723d 4661 6c73 6529  ct_stderr=False)
-0001a990: 0a20 2020 2074 6173 6b20 3d20 7072 6f67  .    task = prog
-0001a9a0: 7265 7373 2e61 6464 5f74 6173 6b28 0a20  ress.add_task(. 
-0001a9b0: 2020 2020 2020 2066 275b 626f 6c64 2063         f'[bold c
-0001a9c0: 7961 6e5d 5265 6672 6573 6869 6e67 2073  yan]Refreshing s
-0001a9d0: 7461 7475 7320 666f 7220 7b6c 656e 2872  tatus for {len(r
-0001a9e0: 6563 6f72 6473 297d 2063 6c75 7374 6572  ecords)} cluster
-0001a9f0: 7b70 6c75 7261 6c7d 5b2f 5d27 2c0a 2020  {plural}[/]',.  
-0001aa00: 2020 2020 2020 746f 7461 6c3d 6c65 6e28        total=len(
-0001aa10: 7265 636f 7264 7329 290a 0a20 2020 2064  records))..    d
-0001aa20: 6566 205f 7265 6672 6573 685f 636c 7573  ef _refresh_clus
-0001aa30: 7465 7228 636c 7573 7465 725f 6e61 6d65  ter(cluster_name
-0001aa40: 293a 0a20 2020 2020 2020 2074 7279 3a0a  ):.        try:.
-0001aa50: 2020 2020 2020 2020 2020 2020 7265 636f              reco
-0001aa60: 7264 203d 2072 6566 7265 7368 5f63 6c75  rd = refresh_clu
-0001aa70: 7374 6572 5f72 6563 6f72 6428 0a20 2020  ster_record(.   
-0001aa80: 2020 2020 2020 2020 2020 2020 2063 6c75               clu
-0001aa90: 7374 6572 5f6e 616d 652c 0a20 2020 2020  ster_name,.     
-0001aaa0: 2020 2020 2020 2020 2020 2066 6f72 6365             force
-0001aab0: 5f72 6566 7265 7368 5f73 7461 7475 7365  _refresh_statuse
-0001aac0: 733d 7365 7428 7374 6174 7573 5f6c 6962  s=set(status_lib
-0001aad0: 2e43 6c75 7374 6572 5374 6174 7573 292c  .ClusterStatus),
-0001aae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001aaf0: 2061 6371 7569 7265 5f70 6572 5f63 6c75   acquire_per_clu
-0001ab00: 7374 6572 5f73 7461 7475 735f 6c6f 636b  ster_status_lock
-0001ab10: 3d54 7275 6529 0a20 2020 2020 2020 2065  =True).        e
-0001ab20: 7863 6570 7420 2865 7863 6570 7469 6f6e  xcept (exception
-0001ab30: 732e 436c 7573 7465 7253 7461 7475 7346  s.ClusterStatusF
-0001ab40: 6574 6368 696e 6745 7272 6f72 2c0a 2020  etchingError,.  
-0001ab50: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-0001ab60: 6365 7074 696f 6e73 2e43 6c6f 7564 5573  ceptions.CloudUs
-0001ab70: 6572 4964 656e 7469 7479 4572 726f 722c  erIdentityError,
-0001ab80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001ab90: 2065 7863 6570 7469 6f6e 732e 436c 7573   exceptions.Clus
-0001aba0: 7465 724f 776e 6572 4964 656e 7469 7479  terOwnerIdentity
-0001abb0: 4d69 736d 6174 6368 4572 726f 7229 2061  MismatchError) a
-0001abc0: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
-0001abd0: 2023 2044 6f20 6e6f 7420 6661 696c 2074   # Do not fail t
-0001abe0: 6865 2065 6e74 6972 6520 7265 6672 6573  he entire refres
-0001abf0: 6820 7072 6f63 6573 732e 2054 6865 2063  h process. The c
-0001ac00: 616c 6c65 7220 7769 6c6c 0a20 2020 2020  aller will.     
-0001ac10: 2020 2020 2020 2023 2068 616e 646c 6520         # handle 
-0001ac20: 7468 6520 2755 4e4b 4e4f 574e 2720 7374  the 'UNKNOWN' st
-0001ac30: 6174 7573 2c20 616e 6420 636f 6c6c 6563  atus, and collec
-0001ac40: 7420 7468 6520 6572 726f 7273 2069 6e74  t the errors int
-0001ac50: 6f0a 2020 2020 2020 2020 2020 2020 2320  o.            # 
-0001ac60: 6120 7461 626c 652e 0a20 2020 2020 2020  a table..       
-0001ac70: 2020 2020 2072 6563 6f72 6420 3d20 7b27       record = {'
-0001ac80: 7374 6174 7573 273a 2027 554e 4b4e 4f57  status': 'UNKNOW
-0001ac90: 4e27 2c20 2765 7272 6f72 273a 2065 7d0a  N', 'error': e}.
-0001aca0: 2020 2020 2020 2020 7072 6f67 7265 7373          progress
-0001acb0: 2e75 7064 6174 6528 7461 736b 2c20 6164  .update(task, ad
-0001acc0: 7661 6e63 653d 3129 0a20 2020 2020 2020  vance=1).       
-0001acd0: 2072 6574 7572 6e20 7265 636f 7264 0a0a   return record..
-0001ace0: 2020 2020 636c 7573 7465 725f 6e61 6d65      cluster_name
-0001acf0: 7320 3d20 5b72 6563 6f72 645b 276e 616d  s = [record['nam
-0001ad00: 6527 5d20 666f 7220 7265 636f 7264 2069  e'] for record i
-0001ad10: 6e20 7265 636f 7264 735d 0a20 2020 2077  n records].    w
-0001ad20: 6974 6820 7072 6f67 7265 7373 3a0a 2020  ith progress:.  
-0001ad30: 2020 2020 2020 7570 6461 7465 645f 7265        updated_re
-0001ad40: 636f 7264 7320 3d20 7375 6270 726f 6365  cords = subproce
-0001ad50: 7373 5f75 7469 6c73 2e72 756e 5f69 6e5f  ss_utils.run_in_
-0001ad60: 7061 7261 6c6c 656c 280a 2020 2020 2020  parallel(.      
-0001ad70: 2020 2020 2020 5f72 6566 7265 7368 5f63        _refresh_c
-0001ad80: 6c75 7374 6572 2c20 636c 7573 7465 725f  luster, cluster_
-0001ad90: 6e61 6d65 7329 0a0a 2020 2020 2320 5368  names)..    # Sh
-0001ada0: 6f77 2069 6e66 6f72 6d61 7469 6f6e 2066  ow information f
-0001adb0: 6f72 2072 656d 6f76 6564 2063 6c75 7374  or removed clust
-0001adc0: 6572 732e 0a20 2020 206b 6570 745f 7265  ers..    kept_re
-0001add0: 636f 7264 7320 3d20 5b5d 0a20 2020 2061  cords = [].    a
-0001ade0: 7574 6f64 6f77 6e5f 636c 7573 7465 7273  utodown_clusters
-0001adf0: 2c20 7265 6d61 696e 696e 675f 636c 7573  , remaining_clus
-0001ae00: 7465 7273 2c20 6661 696c 6564 5f63 6c75  ters, failed_clu
-0001ae10: 7374 6572 7320 3d20 5b5d 2c20 5b5d 2c20  sters = [], [], 
-0001ae20: 5b5d 0a20 2020 2066 6f72 2069 2c20 7265  [].    for i, re
-0001ae30: 636f 7264 2069 6e20 656e 756d 6572 6174  cord in enumerat
-0001ae40: 6528 7265 636f 7264 7329 3a0a 2020 2020  e(records):.    
-0001ae50: 2020 2020 6966 2075 7064 6174 6564 5f72      if updated_r
-0001ae60: 6563 6f72 6473 5b69 5d20 6973 204e 6f6e  ecords[i] is Non
-0001ae70: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
-0001ae80: 6620 7265 636f 7264 5b27 746f 5f64 6f77  f record['to_dow
-0001ae90: 6e27 5d3a 0a20 2020 2020 2020 2020 2020  n']:.           
-0001aea0: 2020 2020 2061 7574 6f64 6f77 6e5f 636c       autodown_cl
-0001aeb0: 7573 7465 7273 2e61 7070 656e 6428 636c  usters.append(cl
-0001aec0: 7573 7465 725f 6e61 6d65 735b 695d 290a  uster_names[i]).
-0001aed0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0001aee0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001aef0: 2020 7265 6d61 696e 696e 675f 636c 7573    remaining_clus
-0001af00: 7465 7273 2e61 7070 656e 6428 636c 7573  ters.append(clus
-0001af10: 7465 725f 6e61 6d65 735b 695d 290a 2020  ter_names[i]).  
-0001af20: 2020 2020 2020 656c 6966 2075 7064 6174        elif updat
-0001af30: 6564 5f72 6563 6f72 6473 5b69 5d5b 2773  ed_records[i]['s
-0001af40: 7461 7475 7327 5d20 3d3d 2027 554e 4b4e  tatus'] == 'UNKN
-0001af50: 4f57 4e27 3a0a 2020 2020 2020 2020 2020  OWN':.          
-0001af60: 2020 6661 696c 6564 5f63 6c75 7374 6572    failed_cluster
-0001af70: 732e 6170 7065 6e64 280a 2020 2020 2020  s.append(.      
-0001af80: 2020 2020 2020 2020 2020 2863 6c75 7374            (clust
-0001af90: 6572 5f6e 616d 6573 5b69 5d2c 2075 7064  er_names[i], upd
-0001afa0: 6174 6564 5f72 6563 6f72 6473 5b69 5d5b  ated_records[i][
-0001afb0: 2765 7272 6f72 275d 2929 0a20 2020 2020  'error'])).     
-0001afc0: 2020 2020 2020 2023 204b 6565 7020 7468         # Keep th
-0001afd0: 6520 6f72 6967 696e 616c 2072 6563 6f72  e original recor
-0001afe0: 6420 6966 2074 6865 2073 7461 7475 7320  d if the status 
-0001aff0: 6973 2075 6e6b 6e6f 776e 2c0a 2020 2020  is unknown,.    
-0001b000: 2020 2020 2020 2020 2320 736f 2074 6861          # so tha
-0001b010: 7420 7468 6520 7573 6572 2063 616e 2073  t the user can s
-0001b020: 7469 6c6c 2073 6565 2074 6865 2063 6c75  till see the clu
-0001b030: 7374 6572 2e0a 2020 2020 2020 2020 2020  ster..          
-0001b040: 2020 6b65 7074 5f72 6563 6f72 6473 2e61    kept_records.a
-0001b050: 7070 656e 6428 7265 636f 7264 290a 2020  ppend(record).  
-0001b060: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0001b070: 2020 2020 2020 2020 6b65 7074 5f72 6563          kept_rec
-0001b080: 6f72 6473 2e61 7070 656e 6428 7570 6461  ords.append(upda
-0001b090: 7465 645f 7265 636f 7264 735b 695d 290a  ted_records[i]).
-0001b0a0: 0a20 2020 2069 6620 6175 746f 646f 776e  .    if autodown
-0001b0b0: 5f63 6c75 7374 6572 733a 0a20 2020 2020  _clusters:.     
-0001b0c0: 2020 2070 6c75 7261 6c20 3d20 2773 2720     plural = 's' 
-0001b0d0: 6966 206c 656e 2861 7574 6f64 6f77 6e5f  if len(autodown_
-0001b0e0: 636c 7573 7465 7273 2920 3e20 3120 656c  clusters) > 1 el
-0001b0f0: 7365 2027 270a 2020 2020 2020 2020 636c  se ''.        cl
-0001b100: 7573 7465 725f 7374 7220 3d20 272c 2027  uster_str = ', '
-0001b110: 2e6a 6f69 6e28 6175 746f 646f 776e 5f63  .join(autodown_c
-0001b120: 6c75 7374 6572 7329 0a20 2020 2020 2020  lusters).       
-0001b130: 206c 6f67 6765 722e 696e 666f 2866 2741   logger.info(f'A
-0001b140: 7574 6f64 6f77 6e65 6420 636c 7573 7465  utodowned cluste
-0001b150: 727b 706c 7572 616c 7d3a 2027 0a20 2020  r{plural}: '.   
-0001b160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b170: 2066 277b 6272 6967 6874 7d7b 636c 7573   f'{bright}{clus
-0001b180: 7465 725f 7374 727d 7b72 6573 6574 7d27  ter_str}{reset}'
-0001b190: 290a 2020 2020 6966 2072 656d 6169 6e69  ).    if remaini
-0001b1a0: 6e67 5f63 6c75 7374 6572 733a 0a20 2020  ng_clusters:.   
-0001b1b0: 2020 2020 2070 6c75 7261 6c20 3d20 2773       plural = 's
-0001b1c0: 2720 6966 206c 656e 2872 656d 6169 6e69  ' if len(remaini
-0001b1d0: 6e67 5f63 6c75 7374 6572 7329 203e 2031  ng_clusters) > 1
-0001b1e0: 2065 6c73 6520 2727 0a20 2020 2020 2020   else ''.       
-0001b1f0: 2063 6c75 7374 6572 5f73 7472 203d 2027   cluster_str = '
-0001b200: 2c20 272e 6a6f 696e 286e 616d 6520 666f  , '.join(name fo
-0001b210: 7220 6e61 6d65 2069 6e20 7265 6d61 696e  r name in remain
-0001b220: 696e 675f 636c 7573 7465 7273 290a 2020  ing_clusters).  
-0001b230: 2020 2020 2020 6c6f 6767 6572 2e77 6172        logger.war
-0001b240: 6e69 6e67 2866 277b 7965 6c6c 6f77 7d43  ning(f'{yellow}C
-0001b250: 6c75 7374 6572 7b70 6c75 7261 6c7d 2074  luster{plural} t
-0001b260: 6572 6d69 6e61 7465 6420 6f6e 2027 0a20  erminated on '. 
-0001b270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b280: 2020 2020 2020 6627 7468 6520 636c 6f75        f'the clou
-0001b290: 643a 207b 7265 7365 747d 7b62 7269 6768  d: {reset}{brigh
-0001b2a0: 747d 7b63 6c75 7374 6572 5f73 7472 7d7b  t}{cluster_str}{
-0001b2b0: 7265 7365 747d 2729 0a0a 2020 2020 6966  reset}')..    if
-0001b2c0: 2066 6169 6c65 645f 636c 7573 7465 7273   failed_clusters
-0001b2d0: 3a0a 2020 2020 2020 2020 706c 7572 616c  :.        plural
-0001b2e0: 203d 2027 7327 2069 6620 6c65 6e28 6661   = 's' if len(fa
-0001b2f0: 696c 6564 5f63 6c75 7374 6572 7329 203e  iled_clusters) >
-0001b300: 2031 2065 6c73 6520 2727 0a20 2020 2020   1 else ''.     
-0001b310: 2020 206c 6f67 6765 722e 7761 726e 696e     logger.warnin
-0001b320: 6728 6627 7b79 656c 6c6f 777d 4661 696c  g(f'{yellow}Fail
-0001b330: 6564 2074 6f20 7265 6672 6573 6820 7374  ed to refresh st
-0001b340: 6174 7573 2066 6f72 2027 0a20 2020 2020  atus for '.     
-0001b350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b360: 2020 6627 7b6c 656e 2866 6169 6c65 645f    f'{len(failed_
-0001b370: 636c 7573 7465 7273 297d 2063 6c75 7374  clusters)} clust
-0001b380: 6572 7b70 6c75 7261 6c7d 3a7b 7265 7365  er{plural}:{rese
-0001b390: 747d 2729 0a20 2020 2020 2020 2066 6f72  t}').        for
-0001b3a0: 2063 6c75 7374 6572 5f6e 616d 652c 2065   cluster_name, e
-0001b3b0: 2069 6e20 6661 696c 6564 5f63 6c75 7374   in failed_clust
-0001b3c0: 6572 733a 0a20 2020 2020 2020 2020 2020  ers:.           
-0001b3d0: 206c 6f67 6765 722e 7761 726e 696e 6728   logger.warning(
-0001b3e0: 6627 2020 7b62 7269 6768 747d 7b63 6c75  f'  {bright}{clu
-0001b3f0: 7374 6572 5f6e 616d 657d 7b72 6573 6574  ster_name}{reset
-0001b400: 7d3a 207b 657d 2729 0a20 2020 2072 6574  }: {e}').    ret
-0001b410: 7572 6e20 6b65 7074 5f72 6563 6f72 6473  urn kept_records
-0001b420: 0a0a 0a40 7479 7069 6e67 2e6f 7665 726c  ...@typing.overl
-0001b430: 6f61 640a 6465 6620 6765 745f 6261 636b  oad.def get_back
-0001b440: 656e 645f 6672 6f6d 5f68 616e 646c 6528  end_from_handle(
-0001b450: 0a20 2020 2068 616e 646c 653a 2027 636c  .    handle: 'cl
-0001b460: 6f75 645f 766d 5f72 6179 5f62 6163 6b65  oud_vm_ray_backe
-0001b470: 6e64 2e43 6c6f 7564 566d 5261 7952 6573  nd.CloudVmRayRes
-0001b480: 6f75 7263 6548 616e 646c 6527 0a29 202d  ourceHandle'.) -
-0001b490: 3e20 2763 6c6f 7564 5f76 6d5f 7261 795f  > 'cloud_vm_ray_
-0001b4a0: 6261 636b 656e 642e 436c 6f75 6456 6d52  backend.CloudVmR
-0001b4b0: 6179 4261 636b 656e 6427 3a0a 2020 2020  ayBackend':.    
-0001b4c0: 2e2e 2e0a 0a0a 4074 7970 696e 672e 6f76  ......@typing.ov
-0001b4d0: 6572 6c6f 6164 0a64 6566 2067 6574 5f62  erload.def get_b
-0001b4e0: 6163 6b65 6e64 5f66 726f 6d5f 6861 6e64  ackend_from_hand
-0001b4f0: 6c65 280a 2020 2020 6861 6e64 6c65 3a20  le(.    handle: 
-0001b500: 276c 6f63 616c 5f64 6f63 6b65 725f 6261  'local_docker_ba
-0001b510: 636b 656e 642e 4c6f 6361 6c44 6f63 6b65  ckend.LocalDocke
-0001b520: 7252 6573 6f75 7263 6548 616e 646c 6527  rResourceHandle'
-0001b530: 0a29 202d 3e20 276c 6f63 616c 5f64 6f63  .) -> 'local_doc
-0001b540: 6b65 725f 6261 636b 656e 642e 4c6f 6361  ker_backend.Loca
-0001b550: 6c44 6f63 6b65 7242 6163 6b65 6e64 273a  lDockerBackend':
-0001b560: 0a20 2020 202e 2e2e 0a0a 0a40 7479 7069  .    ......@typi
-0001b570: 6e67 2e6f 7665 726c 6f61 640a 6465 6620  ng.overload.def 
-0001b580: 6765 745f 6261 636b 656e 645f 6672 6f6d  get_backend_from
-0001b590: 5f68 616e 646c 6528 0a20 2020 2020 2020  _handle(.       
-0001b5a0: 2068 616e 646c 653a 2062 6163 6b65 6e64   handle: backend
-0001b5b0: 732e 5265 736f 7572 6365 4861 6e64 6c65  s.ResourceHandle
-0001b5c0: 2920 2d3e 2062 6163 6b65 6e64 732e 4261  ) -> backends.Ba
-0001b5d0: 636b 656e 643a 0a20 2020 202e 2e2e 0a0a  ckend:.    .....
-0001b5e0: 0a64 6566 2067 6574 5f62 6163 6b65 6e64  .def get_backend
-0001b5f0: 5f66 726f 6d5f 6861 6e64 6c65 280a 2020  _from_handle(.  
-0001b600: 2020 2020 2020 6861 6e64 6c65 3a20 6261        handle: ba
-0001b610: 636b 656e 6473 2e52 6573 6f75 7263 6548  ckends.ResourceH
-0001b620: 616e 646c 6529 202d 3e20 6261 636b 656e  andle) -> backen
-0001b630: 6473 2e42 6163 6b65 6e64 3a0a 2020 2020  ds.Backend:.    
-0001b640: 2222 2247 6574 7320 6120 4261 636b 656e  """Gets a Backen
-0001b650: 6420 6f62 6a65 6374 2063 6f72 7265 7370  d object corresp
-0001b660: 6f6e 6469 6e67 2074 6f20 6120 6861 6e64  onding to a hand
-0001b670: 6c65 2e0a 0a20 2020 2049 6e73 7065 6374  le...    Inspect
-0001b680: 7320 6861 6e64 6c65 2074 7970 6520 746f  s handle type to
-0001b690: 2069 6e66 6572 2074 6865 2062 6163 6b65   infer the backe
-0001b6a0: 6e64 2075 7365 6420 666f 7220 7468 6520  nd used for the 
-0001b6b0: 7265 736f 7572 6365 2e0a 2020 2020 2222  resource..    ""
-0001b6c0: 220a 2020 2020 6261 636b 656e 643a 2062  ".    backend: b
-0001b6d0: 6163 6b65 6e64 732e 4261 636b 656e 640a  ackends.Backend.
-0001b6e0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-0001b6f0: 6528 6861 6e64 6c65 2c20 6261 636b 656e  e(handle, backen
-0001b700: 6473 2e43 6c6f 7564 566d 5261 7952 6573  ds.CloudVmRayRes
-0001b710: 6f75 7263 6548 616e 646c 6529 3a0a 2020  ourceHandle):.  
-0001b720: 2020 2020 2020 6261 636b 656e 6420 3d20        backend = 
-0001b730: 6261 636b 656e 6473 2e43 6c6f 7564 566d  backends.CloudVm
-0001b740: 5261 7942 6163 6b65 6e64 2829 0a20 2020  RayBackend().   
-0001b750: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
-0001b760: 2868 616e 646c 652c 2062 6163 6b65 6e64  (handle, backend
-0001b770: 732e 4c6f 6361 6c44 6f63 6b65 7252 6573  s.LocalDockerRes
-0001b780: 6f75 7263 6548 616e 646c 6529 3a0a 2020  ourceHandle):.  
-0001b790: 2020 2020 2020 6261 636b 656e 6420 3d20        backend = 
-0001b7a0: 6261 636b 656e 6473 2e4c 6f63 616c 446f  backends.LocalDo
-0001b7b0: 636b 6572 4261 636b 656e 6428 290a 2020  ckerBackend().  
-0001b7c0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0001b7d0: 7261 6973 6520 4e6f 7449 6d70 6c65 6d65  raise NotImpleme
-0001b7e0: 6e74 6564 4572 726f 7228 0a20 2020 2020  ntedError(.     
-0001b7f0: 2020 2020 2020 2066 2748 616e 646c 6520         f'Handle 
-0001b800: 7479 7065 207b 7479 7065 2868 616e 646c  type {type(handl
-0001b810: 6529 7d20 6973 206e 6f74 2073 7570 706f  e)} is not suppo
-0001b820: 7274 6564 2079 6574 2e27 290a 2020 2020  rted yet.').    
-0001b830: 7265 7475 726e 2062 6163 6b65 6e64 0a0a  return backend..
-0001b840: 0a64 6566 2067 6574 5f74 6173 6b5f 6465  .def get_task_de
-0001b850: 6d61 6e64 735f 6469 6374 2874 6173 6b3a  mands_dict(task:
-0001b860: 2027 7461 736b 5f6c 6962 2e54 6173 6b27   'task_lib.Task'
-0001b870: 2920 2d3e 2044 6963 745b 7374 722c 2066  ) -> Dict[str, f
-0001b880: 6c6f 6174 5d3a 0a20 2020 2022 2222 5265  loat]:.    """Re
-0001b890: 7475 726e 7320 7468 6520 7265 736f 7572  turns the resour
-0001b8a0: 6365 7320 6469 6374 206f 6620 7468 6520  ces dict of the 
-0001b8b0: 7461 736b 2e0a 0a20 2020 2052 6574 7572  task...    Retur
-0001b8c0: 6e73 3a0a 2020 2020 2020 2020 4120 6469  ns:.        A di
-0001b8d0: 6374 206f 6620 7468 6520 7265 736f 7572  ct of the resour
-0001b8e0: 6365 7320 6f66 2074 6865 2074 6173 6b2e  ces of the task.
-0001b8f0: 2054 6865 206b 6579 7320 6172 6520 7468   The keys are th
-0001b900: 6520 7265 736f 7572 6365 206e 616d 6573  e resource names
-0001b910: 0a20 2020 2020 2020 2061 6e64 2074 6865  .        and the
-0001b920: 2076 616c 7565 7320 6172 6520 7468 6520   values are the 
-0001b930: 6e75 6d62 6572 206f 6620 7468 6520 7265  number of the re
-0001b940: 736f 7572 6365 732e 2049 7420 616c 7761  sources. It alwa
-0001b950: 7973 2063 6f6e 7461 696e 730a 2020 2020  ys contains.    
-0001b960: 2020 2020 7468 6520 4350 5520 7265 736f      the CPU reso
-0001b970: 7572 6365 2028 746f 2063 6f6e 7472 6f6c  urce (to control
-0001b980: 2074 6865 206d 6178 696d 756d 206e 756d   the maximum num
-0001b990: 6265 7220 6f66 2074 6173 6b73 292c 2061  ber of tasks), a
-0001b9a0: 6e64 0a20 2020 2020 2020 206f 7074 696f  nd.        optio
-0001b9b0: 6e61 6c6c 7920 6163 6365 6c65 7261 746f  nally accelerato
-0001b9c0: 7220 6465 6d61 6e64 732e 0a20 2020 2022  r demands..    "
-0001b9d0: 2222 0a20 2020 2023 2054 4f44 4f3a 2043  "".    # TODO: C
-0001b9e0: 7573 746f 6d20 4350 5520 616e 6420 6f74  ustom CPU and ot
-0001b9f0: 6865 7220 6d65 6d6f 7279 2072 6573 6f75  her memory resou
-0001ba00: 7263 6573 2061 7265 206e 6f74 2073 7570  rces are not sup
-0001ba10: 706f 7274 6564 2079 6574 2e0a 2020 2020  ported yet..    
-0001ba20: 2320 466f 7220 736b 7920 6a6f 6273 2f73  # For sky jobs/s
-0001ba30: 6572 7665 2063 6f6e 7472 6f6c 6c65 7220  erve controller 
-0001ba40: 7461 736b 2c20 7765 2073 6574 2074 6865  task, we set the
-0001ba50: 2043 5055 2072 6573 6f75 7263 6520 746f   CPU resource to
-0001ba60: 2061 2073 6d61 6c6c 6572 0a20 2020 2023   a smaller.    #
-0001ba70: 2076 616c 7565 2074 6f20 7375 7070 6f72   value to suppor
-0001ba80: 7420 6120 6c61 7267 6572 206e 756d 6265  t a larger numbe
-0001ba90: 7220 6f66 206d 616e 6167 6564 206a 6f62  r of managed job
-0001baa0: 7320 616e 6420 7365 7276 6963 6573 2e0a  s and services..
-0001bab0: 2020 2020 7265 736f 7572 6365 735f 6469      resources_di
-0001bac0: 6374 203d 207b 0a20 2020 2020 2020 2027  ct = {.        '
-0001bad0: 4350 5527 3a20 2863 6f6e 7374 616e 7473  CPU': (constants
-0001bae0: 2e43 4f4e 5452 4f4c 4c45 525f 5052 4f43  .CONTROLLER_PROC
-0001baf0: 4553 535f 4350 555f 4445 4d41 4e44 0a20  ESS_CPU_DEMAND. 
-0001bb00: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001bb10: 6620 7461 736b 2e69 735f 636f 6e74 726f  f task.is_contro
-0001bb20: 6c6c 6572 5f74 6173 6b28 2920 656c 7365  ller_task() else
-0001bb30: 2044 4546 4155 4c54 5f54 4153 4b5f 4350   DEFAULT_TASK_CP
-0001bb40: 555f 4445 4d41 4e44 290a 2020 2020 7d0a  U_DEMAND).    }.
-0001bb50: 2020 2020 6966 2074 6173 6b2e 6265 7374      if task.best
-0001bb60: 5f72 6573 6f75 7263 6573 2069 7320 6e6f  _resources is no
-0001bb70: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0001bb80: 7265 736f 7572 6365 7320 3d20 7461 736b  resources = task
-0001bb90: 2e62 6573 745f 7265 736f 7572 6365 730a  .best_resources.
-0001bba0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0001bbb0: 2020 2320 5461 736b 206d 6179 2028 652e    # Task may (e.
-0001bbc0: 672e 2c20 736b 7920 6c61 756e 6368 2920  g., sky launch) 
-0001bbd0: 6f72 206d 6179 206e 6f74 2028 652e 672e  or may not (e.g.
-0001bbe0: 2c20 736b 7920 6578 6563 2920 6861 7665  , sky exec) have
-0001bbf0: 2075 6e64 6572 676f 6e65 0a20 2020 2020   undergone.     
-0001bc00: 2020 2023 2073 6b79 2e6f 7074 696d 697a     # sky.optimiz
-0001bc10: 6528 292c 2073 6f20 6265 7374 5f72 6573  e(), so best_res
-0001bc20: 6f75 7263 6573 206d 6179 2062 6520 4e6f  ources may be No
-0001bc30: 6e65 2e0a 2020 2020 2020 2020 6173 7365  ne..        asse
-0001bc40: 7274 206c 656e 2874 6173 6b2e 7265 736f  rt len(task.reso
-0001bc50: 7572 6365 7329 203d 3d20 312c 2074 6173  urces) == 1, tas
-0001bc60: 6b2e 7265 736f 7572 6365 730a 2020 2020  k.resources.    
-0001bc70: 2020 2020 7265 736f 7572 6365 7320 3d20      resources = 
-0001bc80: 6c69 7374 2874 6173 6b2e 7265 736f 7572  list(task.resour
-0001bc90: 6365 7329 5b30 5d0a 2020 2020 6966 2072  ces)[0].    if r
-0001bca0: 6573 6f75 7263 6573 2069 7320 6e6f 7420  esources is not 
-0001bcb0: 4e6f 6e65 2061 6e64 2072 6573 6f75 7263  None and resourc
-0001bcc0: 6573 2e61 6363 656c 6572 6174 6f72 7320  es.accelerators 
-0001bcd0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0001bce0: 2020 2020 2072 6573 6f75 7263 6573 5f64       resources_d
-0001bcf0: 6963 742e 7570 6461 7465 2872 6573 6f75  ict.update(resou
-0001bd00: 7263 6573 2e61 6363 656c 6572 6174 6f72  rces.accelerator
-0001bd10: 7329 0a20 2020 2072 6574 7572 6e20 7265  s).    return re
-0001bd20: 736f 7572 6365 735f 6469 6374 0a0a 0a64  sources_dict...d
-0001bd30: 6566 2067 6574 5f74 6173 6b5f 7265 736f  ef get_task_reso
-0001bd40: 7572 6365 735f 7374 7228 7461 736b 3a20  urces_str(task: 
-0001bd50: 2774 6173 6b5f 6c69 622e 5461 736b 272c  'task_lib.Task',
-0001bd60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001bd70: 2020 2020 2020 2020 2020 2020 6973 5f6d              is_m
-0001bd80: 616e 6167 6564 5f6a 6f62 3a20 626f 6f6c  anaged_job: bool
-0001bd90: 203d 2046 616c 7365 2920 2d3e 2073 7472   = False) -> str
-0001bda0: 3a0a 2020 2020 2222 2252 6574 7572 6e73  :.    """Returns
-0001bdb0: 2074 6865 2072 6573 6f75 7263 6573 2073   the resources s
-0001bdc0: 7472 696e 6720 6f66 2074 6865 2074 6173  tring of the tas
-0001bdd0: 6b2e 0a0a 2020 2020 5468 6520 7265 736f  k...    The reso
-0001bde0: 7572 6365 7320 7374 7269 6e67 2069 7320  urces string is 
-0001bdf0: 6f6e 6c79 2075 7365 6420 6173 2061 2064  only used as a d
-0001be00: 6973 706c 6179 2070 7572 706f 7365 2c20  isplay purpose, 
-0001be10: 736f 2077 6520 6f6e 6c79 2073 686f 770a  so we only show.
-0001be20: 2020 2020 7468 6520 6163 6365 6c65 7261      the accelera
-0001be30: 746f 7220 6465 6d61 6e64 7320 2869 6620  tor demands (if 
-0001be40: 616e 7929 2e20 4f74 6865 7277 6973 652c  any). Otherwise,
-0001be50: 2074 6865 2043 5055 2064 656d 616e 6420   the CPU demand 
-0001be60: 6973 2073 686f 776e 2e0a 2020 2020 2222  is shown..    ""
-0001be70: 220a 2020 2020 7370 6f74 5f73 7472 203d  ".    spot_str =
-0001be80: 2027 270a 2020 2020 7461 736b 5f63 7075   ''.    task_cpu
-0001be90: 5f64 656d 616e 6420 3d20 2873 7472 2863  _demand = (str(c
-0001bea0: 6f6e 7374 616e 7473 2e43 4f4e 5452 4f4c  onstants.CONTROL
-0001beb0: 4c45 525f 5052 4f43 4553 535f 4350 555f  LER_PROCESS_CPU_
-0001bec0: 4445 4d41 4e44 290a 2020 2020 2020 2020  DEMAND).        
-0001bed0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001bee0: 6620 7461 736b 2e69 735f 636f 6e74 726f  f task.is_contro
-0001bef0: 6c6c 6572 5f74 6173 6b28 2920 656c 7365  ller_task() else
-0001bf00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001bf10: 2020 2020 2020 2020 7374 7228 4445 4641          str(DEFA
-0001bf20: 554c 545f 5441 534b 5f43 5055 5f44 454d  ULT_TASK_CPU_DEM
-0001bf30: 414e 4429 290a 2020 2020 6966 2074 6173  AND)).    if tas
-0001bf40: 6b2e 6265 7374 5f72 6573 6f75 7263 6573  k.best_resources
-0001bf50: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0001bf60: 2020 2020 2020 6163 6365 6c65 7261 746f        accelerato
-0001bf70: 725f 6469 6374 203d 2074 6173 6b2e 6265  r_dict = task.be
-0001bf80: 7374 5f72 6573 6f75 7263 6573 2e61 6363  st_resources.acc
-0001bf90: 656c 6572 6174 6f72 730a 2020 2020 2020  elerators.      
-0001bfa0: 2020 6966 2069 735f 6d61 6e61 6765 645f    if is_managed_
-0001bfb0: 6a6f 623a 0a20 2020 2020 2020 2020 2020  job:.           
-0001bfc0: 2069 6620 7461 736b 2e62 6573 745f 7265   if task.best_re
-0001bfd0: 736f 7572 6365 732e 7573 655f 7370 6f74  sources.use_spot
-0001bfe0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001bff0: 2020 7370 6f74 5f73 7472 203d 2027 5b53    spot_str = '[S
-0001c000: 706f 745d 270a 2020 2020 2020 2020 2020  pot]'.          
-0001c010: 2020 7461 736b 5f63 7075 5f64 656d 616e    task_cpu_deman
-0001c020: 6420 3d20 7461 736b 2e62 6573 745f 7265  d = task.best_re
-0001c030: 736f 7572 6365 732e 6370 7573 0a20 2020  sources.cpus.   
-0001c040: 2020 2020 2069 6620 6163 6365 6c65 7261       if accelera
-0001c050: 746f 725f 6469 6374 2069 7320 4e6f 6e65  tor_dict is None
-0001c060: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0001c070: 736f 7572 6365 735f 7374 7220 3d20 6627  sources_str = f'
-0001c080: 4350 553a 7b74 6173 6b5f 6370 755f 6465  CPU:{task_cpu_de
-0001c090: 6d61 6e64 7d27 0a20 2020 2020 2020 2065  mand}'.        e
-0001c0a0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0001c0b0: 2072 6573 6f75 7263 6573 5f73 7472 203d   resources_str =
-0001c0c0: 2027 2c20 272e 6a6f 696e 280a 2020 2020   ', '.join(.    
-0001c0d0: 2020 2020 2020 2020 2020 2020 6627 7b6b              f'{k
-0001c0e0: 7d3a 7b76 7d27 2066 6f72 206b 2c20 7620  }:{v}' for k, v 
-0001c0f0: 696e 2061 6363 656c 6572 6174 6f72 5f64  in accelerator_d
-0001c100: 6963 742e 6974 656d 7328 2929 0a20 2020  ict.items()).   
-0001c110: 2065 6c73 653a 0a20 2020 2020 2020 2072   else:.        r
-0001c120: 6573 6f75 7263 655f 6163 6365 6c65 7261  esource_accelera
-0001c130: 746f 7273 203d 205b 5d0a 2020 2020 2020  tors = [].      
-0001c140: 2020 6d69 6e5f 6370 7573 203d 2066 6c6f    min_cpus = flo
-0001c150: 6174 2827 696e 6627 290a 2020 2020 2020  at('inf').      
-0001c160: 2020 7370 6f74 5f74 7970 653a 2053 6574    spot_type: Set
-0001c170: 5b73 7472 5d20 3d20 7365 7428 290a 2020  [str] = set().  
-0001c180: 2020 2020 2020 666f 7220 7265 736f 7572        for resour
-0001c190: 6365 2069 6e20 7461 736b 2e72 6573 6f75  ce in task.resou
-0001c1a0: 7263 6573 3a0a 2020 2020 2020 2020 2020  rces:.          
-0001c1b0: 2020 7461 736b 5f63 7075 5f64 656d 616e    task_cpu_deman
-0001c1c0: 6420 3d20 2731 2b27 0a20 2020 2020 2020  d = '1+'.       
-0001c1d0: 2020 2020 2069 6620 7265 736f 7572 6365       if resource
-0001c1e0: 2e63 7075 7320 6973 206e 6f74 204e 6f6e  .cpus is not Non
-0001c1f0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0001c200: 2020 2074 6173 6b5f 6370 755f 6465 6d61     task_cpu_dema
-0001c210: 6e64 203d 2072 6573 6f75 7263 652e 6370  nd = resource.cp
-0001c220: 7573 0a20 2020 2020 2020 2020 2020 206d  us.            m
-0001c230: 696e 5f63 7075 7320 3d20 6d69 6e28 6d69  in_cpus = min(mi
-0001c240: 6e5f 6370 7573 2c20 666c 6f61 7428 7461  n_cpus, float(ta
-0001c250: 736b 5f63 7075 5f64 656d 616e 642e 7374  sk_cpu_demand.st
-0001c260: 7269 7028 272b 2027 2929 290a 2020 2020  rip('+ '))).    
-0001c270: 2020 2020 2020 2020 6966 2072 6573 6f75          if resou
-0001c280: 7263 652e 7573 655f 7370 6f74 3a0a 2020  rce.use_spot:.  
-0001c290: 2020 2020 2020 2020 2020 2020 2020 7370                sp
-0001c2a0: 6f74 5f74 7970 652e 6164 6428 2753 706f  ot_type.add('Spo
-0001c2b0: 7427 290a 2020 2020 2020 2020 2020 2020  t').            
-0001c2c0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0001c2d0: 2020 2020 2020 7370 6f74 5f74 7970 652e        spot_type.
-0001c2e0: 6164 6428 274f 6e2d 6465 6d61 6e64 2729  add('On-demand')
-0001c2f0: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-0001c300: 2072 6573 6f75 7263 652e 6163 6365 6c65   resource.accele
-0001c310: 7261 746f 7273 2069 7320 4e6f 6e65 3a0a  rators is None:.
-0001c320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c330: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
-0001c340: 2020 2020 2066 6f72 206b 2c20 7620 696e       for k, v in
-0001c350: 2072 6573 6f75 7263 652e 6163 6365 6c65   resource.accele
-0001c360: 7261 746f 7273 2e69 7465 6d73 2829 3a0a  rators.items():.
-0001c370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c380: 7265 736f 7572 6365 5f61 6363 656c 6572  resource_acceler
-0001c390: 6174 6f72 732e 6170 7065 6e64 2866 277b  ators.append(f'{
-0001c3a0: 6b7d 3a7b 767d 2729 0a0a 2020 2020 2020  k}:{v}')..      
-0001c3b0: 2020 6966 2069 735f 6d61 6e61 6765 645f    if is_managed_
-0001c3c0: 6a6f 623a 0a20 2020 2020 2020 2020 2020  job:.           
-0001c3d0: 2069 6620 6c65 6e28 7461 736b 2e72 6573   if len(task.res
-0001c3e0: 6f75 7263 6573 2920 3e20 313a 0a20 2020  ources) > 1:.   
-0001c3f0: 2020 2020 2020 2020 2020 2020 2074 6173               tas
-0001c400: 6b5f 6370 755f 6465 6d61 6e64 203d 2066  k_cpu_demand = f
-0001c410: 277b 6d69 6e5f 6370 7573 7d2b 270a 2020  '{min_cpus}+'.  
-0001c420: 2020 2020 2020 2020 2020 6966 2027 5370            if 'Sp
-0001c430: 6f74 2720 696e 2073 706f 745f 7479 7065  ot' in spot_type
-0001c440: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001c450: 2020 7370 6f74 5f73 7472 203d 2027 7c27    spot_str = '|'
-0001c460: 2e6a 6f69 6e28 736f 7274 6564 2873 706f  .join(sorted(spo
-0001c470: 745f 7479 7065 2929 0a20 2020 2020 2020  t_type)).       
-0001c480: 2020 2020 2020 2020 2073 706f 745f 7374           spot_st
-0001c490: 7220 3d20 6627 5b7b 7370 6f74 5f73 7472  r = f'[{spot_str
-0001c4a0: 7d5d 270a 2020 2020 2020 2020 6966 2072  }]'.        if r
-0001c4b0: 6573 6f75 7263 655f 6163 6365 6c65 7261  esource_accelera
-0001c4c0: 746f 7273 3a0a 2020 2020 2020 2020 2020  tors:.          
-0001c4d0: 2020 7265 736f 7572 6365 735f 7374 7220    resources_str 
-0001c4e0: 3d20 272c 2027 2e6a 6f69 6e28 7365 7428  = ', '.join(set(
-0001c4f0: 7265 736f 7572 6365 5f61 6363 656c 6572  resource_acceler
-0001c500: 6174 6f72 7329 290a 2020 2020 2020 2020  ators)).        
-0001c510: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0001c520: 2020 7265 736f 7572 6365 735f 7374 7220    resources_str 
-0001c530: 3d20 6627 4350 553a 7b74 6173 6b5f 6370  = f'CPU:{task_cp
-0001c540: 755f 6465 6d61 6e64 7d27 0a20 2020 2072  u_demand}'.    r
-0001c550: 6573 6f75 7263 6573 5f73 7472 203d 2066  esources_str = f
-0001c560: 277b 7461 736b 2e6e 756d 5f6e 6f64 6573  '{task.num_nodes
-0001c570: 7d78 5b7b 7265 736f 7572 6365 735f 7374  }x[{resources_st
-0001c580: 727d 5d7b 7370 6f74 5f73 7472 7d27 0a20  r}]{spot_str}'. 
-0001c590: 2020 2072 6574 7572 6e20 7265 736f 7572     return resour
-0001c5a0: 6365 735f 7374 720a 0a0a 2320 4861 6e64  ces_str...# Hand
-0001c5b0: 6c65 2063 7472 6c2d 630a 6465 6620 696e  le ctrl-c.def in
-0001c5c0: 7465 7272 7570 745f 6861 6e64 6c65 7228  terrupt_handler(
-0001c5d0: 7369 676e 756d 2c20 6672 616d 6529 3a0a  signum, frame):.
-0001c5e0: 2020 2020 6465 6c20 7369 676e 756d 2c20      del signum, 
-0001c5f0: 6672 616d 650a 2020 2020 7375 6270 726f  frame.    subpro
-0001c600: 6365 7373 5f75 7469 6c73 2e6b 696c 6c5f  cess_utils.kill_
-0001c610: 6368 696c 6472 656e 5f70 726f 6365 7373  children_process
-0001c620: 6573 2829 0a20 2020 2023 2041 766f 6964  es().    # Avoid
-0001c630: 2075 7369 6e67 206c 6f67 6765 7220 6865   using logger he
-0001c640: 7265 2c20 6173 2069 7420 7769 6c6c 2070  re, as it will p
-0001c650: 7269 6e74 2074 6865 2073 7461 636b 2074  rint the stack t
-0001c660: 7261 6365 2066 6f72 2062 726f 6b65 6e0a  race for broken.
-0001c670: 2020 2020 2320 7069 7065 2c20 7768 656e      # pipe, when
-0001c680: 2074 6865 206f 7574 7075 7420 6973 2070   the output is p
-0001c690: 6970 6564 2074 6f20 616e 6f74 6865 7220  iped to another 
-0001c6a0: 7072 6f67 7261 6d2e 0a20 2020 2070 7269  program..    pri
-0001c6b0: 6e74 2866 277b 636f 6c6f 7261 6d61 2e53  nt(f'{colorama.S
-0001c6c0: 7479 6c65 2e44 494d 7d54 6970 3a20 5468  tyle.DIM}Tip: Th
-0001c6d0: 6520 6a6f 6220 7769 6c6c 206b 6565 7020  e job will keep 
-0001c6e0: 270a 2020 2020 2020 2020 2020 6627 7275  '.          f'ru
-0001c6f0: 6e6e 696e 6720 6166 7465 7220 4374 726c  nning after Ctrl
-0001c700: 2d43 2e7b 636f 6c6f 7261 6d61 2e53 7479  -C.{colorama.Sty
-0001c710: 6c65 2e52 4553 4554 5f41 4c4c 7d27 290a  le.RESET_ALL}').
-0001c720: 2020 2020 7769 7468 2075 785f 7574 696c      with ux_util
-0001c730: 732e 7072 696e 745f 6578 6365 7074 696f  s.print_exceptio
-0001c740: 6e5f 6e6f 5f74 7261 6365 6261 636b 2829  n_no_traceback()
-0001c750: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
-0001c760: 4b65 7962 6f61 7264 496e 7465 7272 7570  KeyboardInterrup
-0001c770: 7428 6578 6365 7074 696f 6e73 2e4b 4559  t(exceptions.KEY
-0001c780: 424f 4152 445f 494e 5445 5252 5550 545f  BOARD_INTERRUPT_
-0001c790: 434f 4445 290a 0a0a 2320 4861 6e64 6c65  CODE)...# Handle
-0001c7a0: 2063 7472 6c2d 7a0a 6465 6620 7374 6f70   ctrl-z.def stop
-0001c7b0: 5f68 616e 646c 6572 2873 6967 6e75 6d2c  _handler(signum,
-0001c7c0: 2066 7261 6d65 293a 0a20 2020 2064 656c   frame):.    del
-0001c7d0: 2073 6967 6e75 6d2c 2066 7261 6d65 0a20   signum, frame. 
-0001c7e0: 2020 2073 7562 7072 6f63 6573 735f 7574     subprocess_ut
-0001c7f0: 696c 732e 6b69 6c6c 5f63 6869 6c64 7265  ils.kill_childre
-0001c800: 6e5f 7072 6f63 6573 7365 7328 290a 2020  n_processes().  
-0001c810: 2020 2320 4176 6f69 6420 7573 696e 6720    # Avoid using 
-0001c820: 6c6f 6767 6572 2068 6572 652c 2061 7320  logger here, as 
-0001c830: 6974 2077 696c 6c20 7072 696e 7420 7468  it will print th
-0001c840: 6520 7374 6163 6b20 7472 6163 6520 666f  e stack trace fo
-0001c850: 7220 6272 6f6b 656e 0a20 2020 2023 2070  r broken.    # p
-0001c860: 6970 652c 2077 6865 6e20 7468 6520 6f75  ipe, when the ou
-0001c870: 7470 7574 2069 7320 7069 7065 6420 746f  tput is piped to
-0001c880: 2061 6e6f 7468 6572 2070 726f 6772 616d   another program
-0001c890: 2e0a 2020 2020 7072 696e 7428 6627 7b63  ..    print(f'{c
-0001c8a0: 6f6c 6f72 616d 612e 5374 796c 652e 4449  olorama.Style.DI
-0001c8b0: 4d7d 5469 703a 2054 6865 206a 6f62 2077  M}Tip: The job w
-0001c8c0: 696c 6c20 6b65 6570 2027 0a20 2020 2020  ill keep '.     
-0001c8d0: 2020 2020 2066 2772 756e 6e69 6e67 2061       f'running a
-0001c8e0: 6674 6572 2043 7472 6c2d 5a2e 7b63 6f6c  fter Ctrl-Z.{col
-0001c8f0: 6f72 616d 612e 5374 796c 652e 5245 5345  orama.Style.RESE
-0001c900: 545f 414c 4c7d 2729 0a20 2020 2077 6974  T_ALL}').    wit
-0001c910: 6820 7578 5f75 7469 6c73 2e70 7269 6e74  h ux_utils.print
-0001c920: 5f65 7863 6570 7469 6f6e 5f6e 6f5f 7472  _exception_no_tr
-0001c930: 6163 6562 6163 6b28 293a 0a20 2020 2020  aceback():.     
-0001c940: 2020 2072 6169 7365 204b 6579 626f 6172     raise Keyboar
-0001c950: 6449 6e74 6572 7275 7074 2865 7863 6570  dInterrupt(excep
-0001c960: 7469 6f6e 732e 5349 4754 5354 505f 434f  tions.SIGTSTP_CO
-0001c970: 4445 290a 0a0a 6465 6620 7275 6e5f 636f  DE)...def run_co
-0001c980: 6d6d 616e 645f 616e 645f 6861 6e64 6c65  mmand_and_handle
-0001c990: 5f73 7368 5f66 6169 6c75 7265 2872 756e  _ssh_failure(run
-0001c9a0: 6e65 723a 2063 6f6d 6d61 6e64 5f72 756e  ner: command_run
-0001c9b0: 6e65 722e 5353 4843 6f6d 6d61 6e64 5275  ner.SSHCommandRu
-0001c9c0: 6e6e 6572 2c0a 2020 2020 2020 2020 2020  nner,.          
-0001c9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c9e0: 2020 2020 2020 2020 2020 2020 2063 6f6d               com
-0001c9f0: 6d61 6e64 3a20 7374 722c 0a20 2020 2020  mand: str,.     
-0001ca00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ca10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ca20: 2020 6661 696c 7572 655f 6d65 7373 6167    failure_messag
-0001ca30: 653a 2073 7472 2920 2d3e 2073 7472 3a0a  e: str) -> str:.
-0001ca40: 2020 2020 2222 2252 756e 7320 636f 6d6d      """Runs comm
-0001ca50: 616e 6420 7265 6d6f 7465 6c79 2061 6e64  and remotely and
-0001ca60: 2072 6574 7572 6e73 206f 7574 7075 7420   returns output 
-0001ca70: 7769 7468 2070 726f 7065 7220 6572 726f  with proper erro
-0001ca80: 7220 6861 6e64 6c69 6e67 2e22 2222 0a20  r handling.""". 
-0001ca90: 2020 2072 632c 2073 7464 6f75 742c 2073     rc, stdout, s
-0001caa0: 7464 6572 7220 3d20 7275 6e6e 6572 2e72  tderr = runner.r
-0001cab0: 756e 2863 6f6d 6d61 6e64 2c0a 2020 2020  un(command,.    
-0001cac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cae0: 7265 7175 6972 655f 6f75 7470 7574 733d  require_outputs=
-0001caf0: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-0001cb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cb10: 2020 2020 2020 2020 2020 7374 7265 616d            stream
-0001cb20: 5f6c 6f67 733d 4661 6c73 6529 0a20 2020  _logs=False).   
-0001cb30: 2069 6620 7263 203d 3d20 3235 353a 0a20   if rc == 255:. 
-0001cb40: 2020 2020 2020 2023 2053 5348 2066 6169         # SSH fai
-0001cb50: 6c65 640a 2020 2020 2020 2020 7261 6973  led.        rais
-0001cb60: 6520 5275 6e74 696d 6545 7272 6f72 280a  e RuntimeError(.
-0001cb70: 2020 2020 2020 2020 2020 2020 6627 5353              f'SS
-0001cb80: 4820 7769 7468 2075 7365 7220 7b72 756e  H with user {run
-0001cb90: 6e65 722e 7373 685f 7573 6572 7d20 616e  ner.ssh_user} an
-0001cba0: 6420 6b65 7920 7b72 756e 6e65 722e 7373  d key {runner.ss
-0001cbb0: 685f 7072 6976 6174 655f 6b65 797d 2027  h_private_key} '
-0001cbc0: 0a20 2020 2020 2020 2020 2020 2066 2774  .            f't
-0001cbd0: 6f20 7b72 756e 6e65 722e 6970 7d20 6661  o {runner.ip} fa
-0001cbe0: 696c 6564 2e20 5468 6973 2069 7320 6d6f  iled. This is mo
-0001cbf0: 7374 206c 696b 656c 7920 6475 6520 746f  st likely due to
-0001cc00: 2069 6e63 6f72 7265 6374 2027 0a20 2020   incorrect '.   
-0001cc10: 2020 2020 2020 2020 2027 6372 6564 656e           'creden
-0001cc20: 7469 616c 7320 6f72 2069 6e63 6f72 7265  tials or incorre
-0001cc30: 6374 2070 6572 6d69 7373 696f 6e73 2066  ct permissions f
-0001cc40: 6f72 2074 6865 206b 6579 2066 696c 652e  or the key file.
-0001cc50: 2043 6865 636b 2027 0a20 2020 2020 2020   Check '.       
-0001cc60: 2020 2020 2027 796f 7572 2063 7265 6465       'your crede
-0001cc70: 6e74 6961 6c73 2061 6e64 2074 7279 2061  ntials and try a
-0001cc80: 6761 696e 2e27 290a 2020 2020 7375 6270  gain.').    subp
-0001cc90: 726f 6365 7373 5f75 7469 6c73 2e68 616e  rocess_utils.han
-0001cca0: 646c 655f 7265 7475 726e 636f 6465 2872  dle_returncode(r
-0001ccb0: 632c 0a20 2020 2020 2020 2020 2020 2020  c,.             
-0001ccc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ccd0: 2020 2020 2020 2020 2020 636f 6d6d 616e            comman
-0001cce0: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-0001ccf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cd00: 2020 2020 2020 2020 2020 6661 696c 7572            failur
-0001cd10: 655f 6d65 7373 6167 652c 0a20 2020 2020  e_message,.     
-0001cd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cd40: 2020 7374 6465 7272 3d73 7464 6572 7229    stderr=stderr)
-0001cd50: 0a20 2020 2072 6574 7572 6e20 7374 646f  .    return stdo
-0001cd60: 7574 0a0a 0a64 6566 2063 6865 636b 5f72  ut...def check_r
-0001cd70: 7379 6e63 5f69 6e73 7461 6c6c 6564 2829  sync_installed()
-0001cd80: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2222   -> None:.    ""
-0001cd90: 2243 6865 636b 7320 6966 2072 7379 6e63  "Checks if rsync
-0001cda0: 2069 7320 696e 7374 616c 6c65 642e 0a0a   is installed...
-0001cdb0: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
-0001cdc0: 2020 2020 5275 6e74 696d 6545 7272 6f72      RuntimeError
-0001cdd0: 3a20 6966 2072 7379 6e63 2069 7320 6e6f  : if rsync is no
-0001cde0: 7420 696e 7374 616c 6c65 6420 696e 2074  t installed in t
-0001cdf0: 6865 206d 6163 6869 6e65 2e0a 2020 2020  he machine..    
-0001ce00: 2222 220a 2020 2020 7472 793a 0a20 2020  """.    try:.   
-0001ce10: 2020 2020 2073 7562 7072 6f63 6573 732e       subprocess.
-0001ce20: 7275 6e28 2772 7379 6e63 202d 2d76 6572  run('rsync --ver
-0001ce30: 7369 6f6e 272c 0a20 2020 2020 2020 2020  sion',.         
-0001ce40: 2020 2020 2020 2020 2020 2020 2020 7368                sh
-0001ce50: 656c 6c3d 5472 7565 2c0a 2020 2020 2020  ell=True,.      
-0001ce60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ce70: 2063 6865 636b 3d54 7275 652c 0a20 2020   check=True,.   
-0001ce80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ce90: 2020 2020 7374 646f 7574 3d73 7562 7072      stdout=subpr
-0001cea0: 6f63 6573 732e 5049 5045 2c0a 2020 2020  ocess.PIPE,.    
-0001ceb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cec0: 2020 2073 7464 6572 723d 7375 6270 726f     stderr=subpro
-0001ced0: 6365 7373 2e50 4950 4529 0a20 2020 2065  cess.PIPE).    e
-0001cee0: 7863 6570 7420 7375 6270 726f 6365 7373  xcept subprocess
-0001cef0: 2e43 616c 6c65 6450 726f 6365 7373 4572  .CalledProcessEr
-0001cf00: 726f 723a 0a20 2020 2020 2020 2077 6974  ror:.        wit
-0001cf10: 6820 7578 5f75 7469 6c73 2e70 7269 6e74  h ux_utils.print
-0001cf20: 5f65 7863 6570 7469 6f6e 5f6e 6f5f 7472  _exception_no_tr
-0001cf30: 6163 6562 6163 6b28 293a 0a20 2020 2020  aceback():.     
-0001cf40: 2020 2020 2020 2072 6169 7365 2052 756e         raise Run
-0001cf50: 7469 6d65 4572 726f 7228 0a20 2020 2020  timeError(.     
-0001cf60: 2020 2020 2020 2020 2020 2027 6072 7379             '`rsy
-0001cf70: 6e63 6020 6973 2072 6571 7569 7265 6420  nc` is required 
-0001cf80: 666f 7220 7072 6f76 6973 696f 6e69 6e67  for provisioning
-0001cf90: 2061 6e64 270a 2020 2020 2020 2020 2020   and'.          
-0001cfa0: 2020 2020 2020 2720 6974 2069 7320 6e6f        ' it is no
-0001cfb0: 7420 696e 7374 616c 6c65 642e 2046 6f72  t installed. For
-0001cfc0: 2044 6562 6961 6e2f 5562 756e 7475 2073   Debian/Ubuntu s
-0001cfd0: 7973 7465 6d2c 2027 0a20 2020 2020 2020  ystem, '.       
-0001cfe0: 2020 2020 2020 2020 2027 696e 7374 616c           'instal
-0001cff0: 6c20 6974 2077 6974 683a 5c6e 270a 2020  l it with:\n'.  
-0001d000: 2020 2020 2020 2020 2020 2020 2020 2720                ' 
-0001d010: 2024 2073 7564 6f20 6170 7420 696e 7374   $ sudo apt inst
-0001d020: 616c 6c20 7273 796e 6327 2920 6672 6f6d  all rsync') from
-0001d030: 204e 6f6e 650a 0a0a 6465 6620 6368 6563   None...def chec
-0001d040: 6b5f 7374 616c 655f 7275 6e74 696d 655f  k_stale_runtime_
-0001d050: 6f6e 5f72 656d 6f74 6528 7265 7475 726e  on_remote(return
-0001d060: 636f 6465 3a20 696e 742c 2073 7464 6572  code: int, stder
-0001d070: 723a 2073 7472 2c0a 2020 2020 2020 2020  r: str,.        
-0001d080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d090: 2020 2020 2020 2020 2020 636c 7573 7465            cluste
-0001d0a0: 725f 6e61 6d65 3a20 7374 7229 202d 3e20  r_name: str) -> 
-0001d0b0: 4e6f 6e65 3a0a 2020 2020 2222 2252 6169  None:.    """Rai
-0001d0c0: 7365 7320 5275 6e74 696d 6545 7272 6f72  ses RuntimeError
-0001d0d0: 2069 6620 7265 6d6f 7465 2053 6b79 5069   if remote SkyPi
-0001d0e0: 6c6f 7420 7275 6e74 696d 6520 6e65 6564  lot runtime need
-0001d0f0: 7320 746f 2062 6520 7570 6461 7465 642e  s to be updated.
-0001d100: 0a0a 2020 2020 5765 2064 6574 6563 7420  ..    We detect 
-0001d110: 7468 6973 2062 7920 7061 7273 696e 6720  this by parsing 
-0001d120: 6365 7274 6169 6e20 6261 636b 7761 7264  certain backward
-0001d130: 2d69 6e63 6f6d 7061 7469 626c 6520 6572  -incompatible er
-0001d140: 726f 7220 6d65 7373 6167 6573 2066 726f  ror messages fro
-0001d150: 6d0a 2020 2020 6073 7464 6572 7260 2e20  m.    `stderr`. 
-0001d160: 5479 7069 6361 6c6c 7920 6475 6520 746f  Typically due to
-0001d170: 2074 6865 206c 6f63 616c 2063 6c69 656e   the local clien
-0001d180: 7420 7665 7273 696f 6e20 6a75 7374 2067  t version just g
-0001d190: 6f74 2075 7064 6174 6564 2c20 616e 640a  ot updated, and.
-0001d1a0: 2020 2020 7468 6520 7265 6d6f 7465 2072      the remote r
-0001d1b0: 756e 7469 6d65 2069 7320 616e 206f 6c64  untime is an old
-0001d1c0: 6572 2076 6572 7369 6f6e 2e0a 2020 2020  er version..    
-0001d1d0: 2222 220a 2020 2020 7061 7474 6572 6e20  """.    pattern 
-0001d1e0: 3d20 7265 2e63 6f6d 7069 6c65 2872 2741  = re.compile(r'A
-0001d1f0: 7474 7269 6275 7465 4572 726f 723a 206d  ttributeError: m
-0001d200: 6f64 756c 6520 5c27 736b 795c 2e28 2e2a  odule \'sky\.(.*
-0001d210: 295c 2720 6861 7320 6e6f 2027 0a20 2020  )\' has no '.   
-0001d220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d230: 2020 2020 2020 7227 6174 7472 6962 7574        r'attribut
-0001d240: 6520 5c27 282e 2a29 5c27 2729 0a20 2020  e \'(.*)\'').   
-0001d250: 2069 6620 7265 7475 726e 636f 6465 2021   if returncode !
-0001d260: 3d20 303a 0a20 2020 2020 2020 2061 7474  = 0:.        att
-0001d270: 7269 6275 7465 5f65 7272 6f72 203d 2072  ribute_error = r
-0001d280: 652e 6669 6e64 616c 6c28 7061 7474 6572  e.findall(patter
-0001d290: 6e2c 2073 7464 6572 7229 0a20 2020 2020  n, stderr).     
-0001d2a0: 2020 2069 6620 6174 7472 6962 7574 655f     if attribute_
-0001d2b0: 6572 726f 723a 0a20 2020 2020 2020 2020  error:.         
-0001d2c0: 2020 2077 6974 6820 7578 5f75 7469 6c73     with ux_utils
-0001d2d0: 2e70 7269 6e74 5f65 7863 6570 7469 6f6e  .print_exception
-0001d2e0: 5f6e 6f5f 7472 6163 6562 6163 6b28 293a  _no_traceback():
-0001d2f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001d300: 2072 6169 7365 2052 756e 7469 6d65 4572   raise RuntimeEr
-0001d310: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
-0001d320: 2020 2020 2020 2020 2066 277b 636f 6c6f           f'{colo
-0001d330: 7261 6d61 2e46 6f72 652e 5245 447d 536b  rama.Fore.RED}Sk
-0001d340: 7950 696c 6f74 2072 756e 7469 6d65 206e  yPilot runtime n
-0001d350: 6565 6473 2074 6f20 6265 2075 7064 6174  eeds to be updat
-0001d360: 6564 2027 0a20 2020 2020 2020 2020 2020  ed '.           
-0001d370: 2020 2020 2020 2020 2027 6f6e 2074 6865           'on the
-0001d380: 2072 656d 6f74 6520 636c 7573 7465 722e   remote cluster.
-0001d390: 2054 6f20 7570 6461 7465 2c20 7275 6e20   To update, run 
-0001d3a0: 2865 7869 7374 696e 6720 6a6f 6273 2061  (existing jobs a
-0001d3b0: 7265 2027 0a20 2020 2020 2020 2020 2020  re '.           
-0001d3c0: 2020 2020 2020 2020 2066 276e 6f74 2069           f'not i
-0001d3d0: 6e74 6572 7275 7074 6564 293a 207b 636f  nterrupted): {co
-0001d3e0: 6c6f 7261 6d61 2e53 7479 6c65 2e42 5249  lorama.Style.BRI
-0001d3f0: 4748 547d 736b 7920 7374 6172 7420 2d66  GHT}sky start -f
-0001d400: 202d 7920 270a 2020 2020 2020 2020 2020   -y '.          
-0001d410: 2020 2020 2020 2020 2020 6627 7b63 6c75            f'{clu
-0001d420: 7374 6572 5f6e 616d 657d 7b63 6f6c 6f72  ster_name}{color
-0001d430: 616d 612e 5374 796c 652e 5245 5345 545f  ama.Style.RESET_
-0001d440: 414c 4c7d 270a 2020 2020 2020 2020 2020  ALL}'.          
-0001d450: 2020 2020 2020 2020 2020 6627 5c6e 2d2d            f'\n--
-0001d460: 2d20 4465 7461 696c 7320 2d2d 2d5c 6e7b  - Details ---\n{
-0001d470: 7374 6465 7272 2e73 7472 6970 2829 7d5c  stderr.strip()}\
-0001d480: 6e27 290a 0a0a 6465 6620 6765 745f 656e  n')...def get_en
-0001d490: 6470 6f69 6e74 7328 636c 7573 7465 723a  dpoints(cluster:
-0001d4a0: 2073 7472 2c0a 2020 2020 2020 2020 2020   str,.          
-0001d4b0: 2020 2020 2020 2020 706f 7274 3a20 4f70          port: Op
-0001d4c0: 7469 6f6e 616c 5b55 6e69 6f6e 5b69 6e74  tional[Union[int
-0001d4d0: 2c20 7374 725d 5d20 3d20 4e6f 6e65 2c0a  , str]] = None,.
-0001d4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d4f0: 2020 736b 6970 5f73 7461 7475 735f 6368    skip_status_ch
-0001d500: 6563 6b3a 2062 6f6f 6c20 3d20 4661 6c73  eck: bool = Fals
-0001d510: 6529 202d 3e20 4469 6374 5b69 6e74 2c20  e) -> Dict[int, 
-0001d520: 7374 725d 3a0a 2020 2020 2222 2247 6574  str]:.    """Get
-0001d530: 7320 7468 6520 656e 6470 6f69 6e74 2066  s the endpoint f
-0001d540: 6f72 2061 2067 6976 656e 2063 6c75 7374  or a given clust
-0001d550: 6572 2061 6e64 2070 6f72 7420 6e75 6d62  er and port numb
-0001d560: 6572 2028 656e 6470 6f69 6e74 292e 0a0a  er (endpoint)...
-0001d570: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-0001d580: 2020 636c 7573 7465 723a 2054 6865 206e    cluster: The n
-0001d590: 616d 6520 6f66 2074 6865 2063 6c75 7374  ame of the clust
-0001d5a0: 6572 2e0a 2020 2020 2020 2020 706f 7274  er..        port
-0001d5b0: 3a20 5468 6520 706f 7274 206e 756d 6265  : The port numbe
-0001d5c0: 7220 746f 2067 6574 2074 6865 2065 6e64  r to get the end
-0001d5d0: 706f 696e 7420 666f 722e 2049 6620 4e6f  point for. If No
-0001d5e0: 6e65 2c20 656e 6470 6f69 6e74 730a 2020  ne, endpoints.  
-0001d5f0: 2020 2020 2020 2020 2020 666f 7220 616c            for al
-0001d600: 6c20 706f 7274 7320 6172 6520 7265 7475  l ports are retu
-0001d610: 726e 6564 2e0a 2020 2020 2020 2020 736b  rned..        sk
-0001d620: 6970 5f73 7461 7475 735f 6368 6563 6b3a  ip_status_check:
-0001d630: 2057 6865 7468 6572 2074 6f20 736b 6970   Whether to skip
-0001d640: 2074 6865 2073 7461 7475 7320 6368 6563   the status chec
-0001d650: 6b20 666f 7220 7468 6520 636c 7573 7465  k for the cluste
-0001d660: 722e 0a20 2020 2020 2020 2020 2020 2054  r..            T
-0001d670: 6869 7320 6973 2075 7365 6675 6c20 7768  his is useful wh
-0001d680: 656e 2074 6865 2063 6c75 7374 6572 2069  en the cluster i
-0001d690: 7320 6b6e 6f77 6e20 746f 2062 6520 696e  s known to be in
-0001d6a0: 2061 2049 4e49 5420 7374 6174 650a 2020   a INIT state.  
-0001d6b0: 2020 2020 2020 2020 2020 616e 6420 7468            and th
-0001d6c0: 6520 6361 6c6c 6572 2077 616e 7473 2074  e caller wants t
-0001d6d0: 6f20 7175 6572 7920 7468 6520 656e 6470  o query the endp
-0001d6e0: 6f69 6e74 732e 2055 7365 6420 6279 2073  oints. Used by s
-0001d6f0: 6572 7665 0a20 2020 2020 2020 2020 2020  erve.           
-0001d700: 2063 6f6e 7472 6f6c 6c65 7220 746f 2071   controller to q
-0001d710: 7565 7279 2065 6e64 706f 696e 7473 2064  uery endpoints d
-0001d720: 7572 696e 6720 636c 7573 7465 7220 6c61  uring cluster la
-0001d730: 756e 6368 2077 6865 6e20 6d75 6c74 6970  unch when multip
-0001d740: 6c65 0a20 2020 2020 2020 2020 2020 2073  le.            s
-0001d750: 6572 7669 6365 7320 6d61 7920 6265 2067  ervices may be g
-0001d760: 6574 7469 6e67 206c 6175 6e63 6865 6420  etting launched 
-0001d770: 696e 2070 6172 616c 6c65 6c20 2861 6e64  in parallel (and
-0001d780: 2061 7320 6120 7265 7375 6c74 2c0a 2020   as a result,.  
-0001d790: 2020 2020 2020 2020 2020 7468 6520 636f            the co
-0001d7a0: 6e74 726f 6c6c 6572 206d 6179 2062 6520  ntroller may be 
-0001d7b0: 696e 2049 4e49 5420 7374 6174 7573 2064  in INIT status d
-0001d7c0: 7565 2074 6f20 6120 636f 6e63 7572 7265  ue to a concurre
-0001d7d0: 6e74 206c 6175 6e63 6829 2e0a 0a20 2020  nt launch)...   
-0001d7e0: 2052 6574 7572 6e73 3a20 4120 6469 6374   Returns: A dict
-0001d7f0: 696f 6e61 7279 206f 6620 706f 7274 206e  ionary of port n
-0001d800: 756d 6265 7273 2074 6f20 656e 6470 6f69  umbers to endpoi
-0001d810: 6e74 732e 2049 6620 656e 6470 6f69 6e74  nts. If endpoint
-0001d820: 2069 7320 4e6f 6e65 2c0a 2020 2020 2020   is None,.      
-0001d830: 2020 7468 6520 6469 6374 696f 6e61 7279    the dictionary
-0001d840: 2077 696c 6c20 636f 6e74 6169 6e20 616c   will contain al
-0001d850: 6c20 706f 7274 733a 656e 6470 6f69 6e74  l ports:endpoint
-0001d860: 7320 6578 706f 7365 6420 6f6e 2074 6865  s exposed on the
-0001d870: 2063 6c75 7374 6572 2e0a 2020 2020 2020   cluster..      
-0001d880: 2020 4966 2074 6865 2065 6e64 706f 696e    If the endpoin
-0001d890: 7420 6973 206e 6f74 2065 7870 6f73 6564  t is not exposed
-0001d8a0: 2079 6574 2028 652e 672e 2c20 6475 7269   yet (e.g., duri
-0001d8b0: 6e67 2063 6c75 7374 6572 206c 6175 6e63  ng cluster launc
-0001d8c0: 6820 6f72 0a20 2020 2020 2020 2077 6169  h or.        wai
-0001d8d0: 7469 6e67 2066 6f72 2063 6c6f 7564 2070  ting for cloud p
-0001d8e0: 726f 7669 6465 7220 746f 2065 7870 6f73  rovider to expos
-0001d8f0: 6520 7468 6520 656e 6470 6f69 6e74 292c  e the endpoint),
-0001d900: 2061 6e20 656d 7074 7920 6469 6374 696f   an empty dictio
-0001d910: 6e61 7279 0a20 2020 2020 2020 2069 7320  nary.        is 
-0001d920: 7265 7475 726e 6564 2e0a 0a20 2020 2052  returned...    R
-0001d930: 6169 7365 733a 0a20 2020 2020 2020 2056  aises:.        V
-0001d940: 616c 7565 4572 726f 723a 2069 6620 7468  alueError: if th
-0001d950: 6520 706f 7274 2069 7320 696e 7661 6c69  e port is invali
-0001d960: 6420 6f72 2074 6865 2063 6c6f 7564 2070  d or the cloud p
-0001d970: 726f 7669 6465 7220 646f 6573 206e 6f74  rovider does not
-0001d980: 0a20 2020 2020 2020 2020 2020 2073 7570  .            sup
-0001d990: 706f 7274 2071 7565 7279 696e 6720 656e  port querying en
-0001d9a0: 6470 6f69 6e74 732e 0a20 2020 2020 2020  dpoints..       
-0001d9b0: 2065 7863 6570 7469 6f6e 732e 436c 7573   exceptions.Clus
-0001d9c0: 7465 724e 6f74 5570 4572 726f 723a 2069  terNotUpError: i
-0001d9d0: 6620 7468 6520 636c 7573 7465 7220 6973  f the cluster is
-0001d9e0: 206e 6f74 2069 6e20 5550 2073 7461 7475   not in UP statu
-0001d9f0: 732e 0a20 2020 2022 2222 0a20 2020 2023  s..    """.    #
-0001da00: 2043 6173 7420 656e 6470 6f69 6e74 2074   Cast endpoint t
-0001da10: 6f20 696e 7420 6966 2069 7420 6973 206e  o int if it is n
-0001da20: 6f74 204e 6f6e 650a 2020 2020 6966 2070  ot None.    if p
-0001da30: 6f72 7420 6973 206e 6f74 204e 6f6e 653a  ort is not None:
-0001da40: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
-0001da50: 2020 2020 2020 2020 2020 706f 7274 203d            port =
-0001da60: 2069 6e74 2870 6f72 7429 0a20 2020 2020   int(port).     
-0001da70: 2020 2065 7863 6570 7420 5661 6c75 6545     except ValueE
-0001da80: 7272 6f72 3a0a 2020 2020 2020 2020 2020  rror:.          
-0001da90: 2020 7769 7468 2075 785f 7574 696c 732e    with ux_utils.
-0001daa0: 7072 696e 745f 6578 6365 7074 696f 6e5f  print_exception_
-0001dab0: 6e6f 5f74 7261 6365 6261 636b 2829 3a0a  no_traceback():.
-0001dac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dad0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-0001dae0: 2866 2749 6e76 616c 6964 2065 6e64 706f  (f'Invalid endpo
-0001daf0: 696e 7420 7b70 6f72 7421 727d 2e27 2920  int {port!r}.') 
-0001db00: 6672 6f6d 204e 6f6e 650a 2020 2020 636c  from None.    cl
-0001db10: 7573 7465 725f 7265 636f 7264 7320 3d20  uster_records = 
-0001db20: 6765 745f 636c 7573 7465 7273 2869 6e63  get_clusters(inc
-0001db30: 6c75 6465 5f63 6f6e 7472 6f6c 6c65 723d  lude_controller=
-0001db40: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-0001db50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001db60: 2020 2020 2020 2020 2072 6566 7265 7368           refresh
-0001db70: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
-0001db80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001db90: 2020 2020 2020 2020 2020 2063 6c75 7374             clust
-0001dba0: 6572 5f6e 616d 6573 3d5b 636c 7573 7465  er_names=[cluste
-0001dbb0: 725d 290a 2020 2020 636c 7573 7465 725f  r]).    cluster_
-0001dbc0: 7265 636f 7264 203d 2063 6c75 7374 6572  record = cluster
-0001dbd0: 5f72 6563 6f72 6473 5b30 5d0a 2020 2020  _records[0].    
-0001dbe0: 6966 2028 6e6f 7420 736b 6970 5f73 7461  if (not skip_sta
-0001dbf0: 7475 735f 6368 6563 6b20 616e 640a 2020  tus_check and.  
-0001dc00: 2020 2020 2020 2020 2020 636c 7573 7465            cluste
-0001dc10: 725f 7265 636f 7264 5b27 7374 6174 7573  r_record['status
-0001dc20: 275d 2021 3d20 7374 6174 7573 5f6c 6962  '] != status_lib
-0001dc30: 2e43 6c75 7374 6572 5374 6174 7573 2e55  .ClusterStatus.U
-0001dc40: 5029 3a0a 2020 2020 2020 2020 7769 7468  P):.        with
-0001dc50: 2075 785f 7574 696c 732e 7072 696e 745f   ux_utils.print_
-0001dc60: 6578 6365 7074 696f 6e5f 6e6f 5f74 7261  exception_no_tra
-0001dc70: 6365 6261 636b 2829 3a0a 2020 2020 2020  ceback():.      
-0001dc80: 2020 2020 2020 7261 6973 6520 6578 6365        raise exce
-0001dc90: 7074 696f 6e73 2e43 6c75 7374 6572 4e6f  ptions.ClusterNo
-0001dca0: 7455 7045 7272 6f72 280a 2020 2020 2020  tUpError(.      
-0001dcb0: 2020 2020 2020 2020 2020 6627 436c 7573            f'Clus
-0001dcc0: 7465 7220 7b63 6c75 7374 6572 5f72 6563  ter {cluster_rec
-0001dcd0: 6f72 645b 226e 616d 6522 5d21 727d 2027  ord["name"]!r} '
-0001dce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001dcf0: 2027 6973 206e 6f74 2069 6e20 5550 2073   'is not in UP s
-0001dd00: 7461 7475 732e 272c 2063 6c75 7374 6572  tatus.', cluster
-0001dd10: 5f72 6563 6f72 645b 2773 7461 7475 7327  _record['status'
-0001dd20: 5d29 0a20 2020 2068 616e 646c 6520 3d20  ]).    handle = 
-0001dd30: 636c 7573 7465 725f 7265 636f 7264 5b27  cluster_record['
-0001dd40: 6861 6e64 6c65 275d 0a20 2020 2069 6620  handle'].    if 
-0001dd50: 6e6f 7420 6973 696e 7374 616e 6365 2868  not isinstance(h
-0001dd60: 616e 646c 652c 2062 6163 6b65 6e64 732e  andle, backends.
-0001dd70: 436c 6f75 6456 6d52 6179 5265 736f 7572  CloudVmRayResour
-0001dd80: 6365 4861 6e64 6c65 293a 0a20 2020 2020  ceHandle):.     
-0001dd90: 2020 2077 6974 6820 7578 5f75 7469 6c73     with ux_utils
-0001dda0: 2e70 7269 6e74 5f65 7863 6570 7469 6f6e  .print_exception
-0001ddb0: 5f6e 6f5f 7472 6163 6562 6163 6b28 293a  _no_traceback():
-0001ddc0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0001ddd0: 7365 2056 616c 7565 4572 726f 7228 2751  se ValueError('Q
-0001dde0: 7565 7279 696e 6720 4950 2061 6464 7265  uerying IP addre
-0001ddf0: 7373 2069 7320 6e6f 7420 7375 7070 6f72  ss is not suppor
-0001de00: 7465 6420 270a 2020 2020 2020 2020 2020  ted '.          
-0001de10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001de20: 2020 2066 2766 6f72 2063 6c75 7374 6572     f'for cluster
-0001de30: 207b 636c 7573 7465 7221 727d 2077 6974   {cluster!r} wit
-0001de40: 6820 6261 636b 656e 6420 270a 2020 2020  h backend '.    
-0001de50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001de60: 2020 2020 2020 2020 2066 277b 6765 745f           f'{get_
-0001de70: 6261 636b 656e 645f 6672 6f6d 5f68 616e  backend_from_han
-0001de80: 646c 6528 6861 6e64 6c65 292e 4e41 4d45  dle(handle).NAME
-0001de90: 7d2e 2729 0a0a 2020 2020 6c61 756e 6368  }.')..    launch
-0001dea0: 6564 5f72 6573 6f75 7263 6573 203d 2068  ed_resources = h
-0001deb0: 616e 646c 652e 6c61 756e 6368 6564 5f72  andle.launched_r
-0001dec0: 6573 6f75 7263 6573 0a20 2020 2063 6c6f  esources.    clo
-0001ded0: 7564 203d 206c 6175 6e63 6865 645f 7265  ud = launched_re
-0001dee0: 736f 7572 6365 732e 636c 6f75 640a 2020  sources.cloud.  
-0001def0: 2020 7472 793a 0a20 2020 2020 2020 2063    try:.        c
-0001df00: 6c6f 7564 2e63 6865 636b 5f66 6561 7475  loud.check_featu
-0001df10: 7265 735f 6172 655f 7375 7070 6f72 7465  res_are_supporte
-0001df20: 6428 0a20 2020 2020 2020 2020 2020 206c  d(.            l
-0001df30: 6175 6e63 6865 645f 7265 736f 7572 6365  aunched_resource
-0001df40: 732c 207b 636c 6f75 6473 2e43 6c6f 7564  s, {clouds.Cloud
-0001df50: 496d 706c 656d 656e 7461 7469 6f6e 4665  ImplementationFe
-0001df60: 6174 7572 6573 2e4f 5045 4e5f 504f 5254  atures.OPEN_PORT
-0001df70: 537d 290a 2020 2020 6578 6365 7074 2065  S}).    except e
-0001df80: 7863 6570 7469 6f6e 732e 4e6f 7453 7570  xceptions.NotSup
-0001df90: 706f 7274 6564 4572 726f 723a 0a20 2020  portedError:.   
-0001dfa0: 2020 2020 2077 6974 6820 7578 5f75 7469       with ux_uti
-0001dfb0: 6c73 2e70 7269 6e74 5f65 7863 6570 7469  ls.print_excepti
-0001dfc0: 6f6e 5f6e 6f5f 7472 6163 6562 6163 6b28  on_no_traceback(
-0001dfd0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-0001dfe0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-0001dff0: 2751 7565 7279 696e 6720 656e 6470 6f69  'Querying endpoi
-0001e000: 6e74 7320 6973 206e 6f74 2073 7570 706f  nts is not suppo
-0001e010: 7274 6564 2027 0a20 2020 2020 2020 2020  rted '.         
-0001e020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e030: 2020 2020 6627 666f 7220 636c 7573 7465      f'for cluste
-0001e040: 7220 7b63 6c75 7374 6572 2172 7d20 6f6e  r {cluster!r} on
-0001e050: 207b 636c 6f75 647d 2e27 2920 6672 6f6d   {cloud}.') from
-0001e060: 204e 6f6e 650a 0a20 2020 2063 6f6e 6669   None..    confi
-0001e070: 6720 3d20 636f 6d6d 6f6e 5f75 7469 6c73  g = common_utils
-0001e080: 2e72 6561 645f 7961 6d6c 2868 616e 646c  .read_yaml(handl
-0001e090: 652e 636c 7573 7465 725f 7961 6d6c 290a  e.cluster_yaml).
-0001e0a0: 2020 2020 706f 7274 5f64 6574 6169 6c73      port_details
-0001e0b0: 203d 2070 726f 7669 7369 6f6e 5f6c 6962   = provision_lib
-0001e0c0: 2e71 7565 7279 5f70 6f72 7473 2872 6570  .query_ports(rep
-0001e0d0: 7228 636c 6f75 6429 2c0a 2020 2020 2020  r(cloud),.      
-0001e0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e100: 2020 2020 2020 2068 616e 646c 652e 636c         handle.cl
-0001e110: 7573 7465 725f 6e61 6d65 5f6f 6e5f 636c  uster_name_on_cl
-0001e120: 6f75 642c 0a20 2020 2020 2020 2020 2020  oud,.           
-0001e130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019e40: 2020 2020 2020 2020 2020 2020 2068 616e               han
+00019e50: 646c 653d 6861 6e64 6c65 290a 2020 2020  dle=handle).    
+00019e60: 6173 7365 7274 2068 616e 646c 6520 6973  assert handle is
+00019e70: 206e 6f74 204e 6f6e 6520 616e 6420 6861   not None and ha
+00019e80: 6e64 6c65 2e68 6561 645f 6970 2069 7320  ndle.head_ip is 
+00019e90: 6e6f 7420 4e6f 6e65 2c20 280a 2020 2020  not None, (.    
+00019ea0: 2020 2020 6861 6e64 6c65 2c20 636f 6e74      handle, cont
+00019eb0: 726f 6c6c 6572 5f73 7461 7475 7329 0a20  roller_status). 
+00019ec0: 2020 2072 6574 7572 6e20 6861 6e64 6c65     return handle
+00019ed0: 0a0a 0a63 6c61 7373 2043 6c6f 7564 4669  ...class CloudFi
+00019ee0: 6c74 6572 2865 6e75 6d2e 456e 756d 293a  lter(enum.Enum):
+00019ef0: 0a20 2020 2023 2046 696c 7465 7220 666f  .    # Filter fo
+00019f00: 7220 616c 6c20 7479 7065 7320 6f66 2063  r all types of c
+00019f10: 6c6f 7564 732e 0a20 2020 2041 4c4c 203d  louds..    ALL =
+00019f20: 2027 616c 6c27 0a20 2020 2023 2046 696c   'all'.    # Fil
+00019f30: 7465 7220 666f 7220 536b 7927 7320 6d61  ter for Sky's ma
+00019f40: 696e 2063 6c6f 7564 7320 2861 7773 2c20  in clouds (aws, 
+00019f50: 6763 702c 2061 7a75 7265 2c20 646f 636b  gcp, azure, dock
+00019f60: 6572 292e 0a20 2020 2043 4c4f 5544 535f  er)..    CLOUDS_
+00019f70: 414e 445f 444f 434b 4552 203d 2027 636c  AND_DOCKER = 'cl
+00019f80: 6f75 6473 2d61 6e64 2d64 6f63 6b65 7227  ouds-and-docker'
+00019f90: 0a20 2020 2023 2046 696c 7465 7220 666f  .    # Filter fo
+00019fa0: 7220 6f6e 6c79 206c 6f63 616c 2063 6c6f  r only local clo
+00019fb0: 7564 732e 0a20 2020 204c 4f43 414c 203d  uds..    LOCAL =
+00019fc0: 2027 6c6f 6361 6c27 0a0a 0a64 6566 2067   'local'...def g
+00019fd0: 6574 5f63 6c75 7374 6572 7328 0a20 2020  et_clusters(.   
+00019fe0: 2069 6e63 6c75 6465 5f63 6f6e 7472 6f6c   include_control
+00019ff0: 6c65 723a 2062 6f6f 6c2c 0a20 2020 2072  ler: bool,.    r
+0001a000: 6566 7265 7368 3a20 626f 6f6c 2c0a 2020  efresh: bool,.  
+0001a010: 2020 636c 7573 7465 725f 6e61 6d65 733a    cluster_names:
+0001a020: 204f 7074 696f 6e61 6c5b 556e 696f 6e5b   Optional[Union[
+0001a030: 7374 722c 204c 6973 745b 7374 725d 5d5d  str, List[str]]]
+0001a040: 203d 204e 6f6e 652c 0a29 202d 3e20 4c69   = None,.) -> Li
+0001a050: 7374 5b44 6963 745b 7374 722c 2041 6e79  st[Dict[str, Any
+0001a060: 5d5d 3a0a 2020 2020 2222 2252 6574 7572  ]]:.    """Retur
+0001a070: 6e73 2061 206c 6973 7420 6f66 2063 6163  ns a list of cac
+0001a080: 6865 6420 6f72 206f 7074 696f 6e61 6c6c  hed or optionall
+0001a090: 7920 7265 6672 6573 6865 6420 636c 7573  y refreshed clus
+0001a0a0: 7465 7220 7265 636f 7264 732e 0a0a 2020  ter records...  
+0001a0b0: 2020 436f 6d62 7320 7468 726f 7567 6820    Combs through 
+0001a0c0: 7468 6520 6461 7461 6261 7365 2028 696e  the database (in
+0001a0d0: 207e 2f2e 736b 792f 7374 6174 652e 6462   ~/.sky/state.db
+0001a0e0: 2920 746f 2067 6574 2061 206c 6973 7420  ) to get a list 
+0001a0f0: 6f66 2072 6563 6f72 6473 0a20 2020 2063  of records.    c
+0001a100: 6f72 7265 7370 6f6e 6469 6e67 2074 6f20  orresponding to 
+0001a110: 6c61 756e 6368 6564 2063 6c75 7374 6572  launched cluster
+0001a120: 7320 2866 696c 7465 7265 6420 6279 2060  s (filtered by `
+0001a130: 636c 7573 7465 725f 6e61 6d65 7360 2069  cluster_names` i
+0001a140: 6620 6974 2069 730a 2020 2020 7370 6563  f it is.    spec
+0001a150: 6966 6965 6429 2e20 5468 6520 7265 6672  ified). The refr
+0001a160: 6573 6820 666c 6167 2063 616e 2062 6520  esh flag can be 
+0001a170: 7573 6564 2074 6f20 666f 7263 6520 6120  used to force a 
+0001a180: 7265 6672 6573 6820 6f66 2074 6865 2073  refresh of the s
+0001a190: 7461 7475 730a 2020 2020 6f66 2074 6865  tatus.    of the
+0001a1a0: 2063 6c75 7374 6572 732e 0a0a 2020 2020   clusters...    
+0001a1b0: 4172 6773 3a0a 2020 2020 2020 2020 696e  Args:.        in
+0001a1c0: 636c 7564 655f 636f 6e74 726f 6c6c 6572  clude_controller
+0001a1d0: 3a20 5768 6574 6865 7220 746f 2069 6e63  : Whether to inc
+0001a1e0: 6c75 6465 2063 6f6e 7472 6f6c 6c65 7273  lude controllers
+0001a1f0: 2c20 652e 672e 206a 6f62 7320 636f 6e74  , e.g. jobs cont
+0001a200: 726f 6c6c 6572 0a20 2020 2020 2020 2020  roller.         
+0001a210: 2020 206f 7220 736b 7920 7365 7276 6520     or sky serve 
+0001a220: 636f 6e74 726f 6c6c 6572 2e0a 2020 2020  controller..    
+0001a230: 2020 2020 7265 6672 6573 683a 2057 6865      refresh: Whe
+0001a240: 7468 6572 2074 6f20 7265 6672 6573 6820  ther to refresh 
+0001a250: 7468 6520 7374 6174 7573 206f 6620 7468  the status of th
+0001a260: 6520 636c 7573 7465 7273 2e20 2852 6566  e clusters. (Ref
+0001a270: 7265 7368 696e 6720 7769 6c6c 0a20 2020  reshing will.   
+0001a280: 2020 2020 2020 2020 2073 6574 2074 6865           set the
+0001a290: 2073 7461 7475 7320 746f 2053 544f 5050   status to STOPP
+0001a2a0: 4544 2069 6620 7468 6520 636c 7573 7465  ED if the cluste
+0001a2b0: 7220 6361 6e6e 6f74 2062 6520 7069 6e67  r cannot be ping
+0001a2c0: 6564 2e29 0a20 2020 2020 2020 2063 6c6f  ed.).        clo
+0001a2d0: 7564 5f66 696c 7465 723a 2053 6574 7320  ud_filter: Sets 
+0001a2e0: 7768 6963 6820 636c 6f75 6473 2074 6f20  which clouds to 
+0001a2f0: 6669 6c65 7220 7468 726f 7567 6820 6672  filer through fr
+0001a300: 6f6d 2074 6865 2067 6c6f 6261 6c20 7573  om the global us
+0001a310: 6572 0a20 2020 2020 2020 2020 2020 2073  er.            s
+0001a320: 7461 7465 2e20 5375 7070 6f72 7473 2074  tate. Supports t
+0001a330: 6872 6565 2076 616c 7565 732c 2027 616c  hree values, 'al
+0001a340: 6c27 2066 6f72 2061 6c6c 2063 6c6f 7564  l' for all cloud
+0001a350: 732c 2027 7075 626c 6963 2720 666f 720a  s, 'public' for.
+0001a360: 2020 2020 2020 2020 2020 2020 7075 626c              publ
+0001a370: 6963 2063 6c6f 7564 7320 6f6e 6c79 2c20  ic clouds only, 
+0001a380: 616e 6420 276c 6f63 616c 2720 666f 7220  and 'local' for 
+0001a390: 6f6e 6c79 206c 6f63 616c 2063 6c6f 7564  only local cloud
+0001a3a0: 732e 0a20 2020 2020 2020 2063 6c75 7374  s..        clust
+0001a3b0: 6572 5f6e 616d 6573 3a20 4966 2070 726f  er_names: If pro
+0001a3c0: 7669 6465 642c 206f 6e6c 7920 7265 7475  vided, only retu
+0001a3d0: 726e 2072 6563 6f72 6473 2066 6f72 2074  rn records for t
+0001a3e0: 6865 2067 6976 656e 2063 6c75 7374 6572  he given cluster
+0001a3f0: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
+0001a400: 6573 2e0a 0a20 2020 2052 6574 7572 6e73  es...    Returns
+0001a410: 3a0a 2020 2020 2020 2020 4120 6c69 7374  :.        A list
+0001a420: 206f 6620 636c 7573 7465 7220 7265 636f   of cluster reco
+0001a430: 7264 732e 2049 6620 7468 6520 636c 7573  rds. If the clus
+0001a440: 7465 7220 646f 6573 206e 6f74 2065 7869  ter does not exi
+0001a450: 7374 206f 7220 6861 7320 6265 656e 0a20  st or has been. 
+0001a460: 2020 2020 2020 2074 6572 6d69 6e61 7465         terminate
+0001a470: 642c 2074 6865 2072 6563 6f72 6420 7769  d, the record wi
+0001a480: 6c6c 2062 6520 6f6d 6974 7465 6420 6672  ll be omitted fr
+0001a490: 6f6d 2074 6865 2072 6574 7572 6e65 6420  om the returned 
+0001a4a0: 6c69 7374 2e0a 2020 2020 2222 220a 2020  list..    """.  
+0001a4b0: 2020 7265 636f 7264 7320 3d20 676c 6f62    records = glob
+0001a4c0: 616c 5f75 7365 725f 7374 6174 652e 6765  al_user_state.ge
+0001a4d0: 745f 636c 7573 7465 7273 2829 0a0a 2020  t_clusters()..  
+0001a4e0: 2020 6966 206e 6f74 2069 6e63 6c75 6465    if not include
+0001a4f0: 5f63 6f6e 7472 6f6c 6c65 723a 0a20 2020  _controller:.   
+0001a500: 2020 2020 2072 6563 6f72 6473 203d 205b       records = [
+0001a510: 0a20 2020 2020 2020 2020 2020 2072 6563  .            rec
+0001a520: 6f72 6420 666f 7220 7265 636f 7264 2069  ord for record i
+0001a530: 6e20 7265 636f 7264 730a 2020 2020 2020  n records.      
+0001a540: 2020 2020 2020 6966 2063 6f6e 7472 6f6c        if control
+0001a550: 6c65 725f 7574 696c 732e 436f 6e74 726f  ler_utils.Contro
+0001a560: 6c6c 6572 732e 6672 6f6d 5f6e 616d 6528  llers.from_name(
+0001a570: 7265 636f 7264 5b27 6e61 6d65 275d 2920  record['name']) 
+0001a580: 6973 204e 6f6e 650a 2020 2020 2020 2020  is None.        
+0001a590: 5d0a 0a20 2020 2079 656c 6c6f 7720 3d20  ]..    yellow = 
+0001a5a0: 636f 6c6f 7261 6d61 2e46 6f72 652e 5945  colorama.Fore.YE
+0001a5b0: 4c4c 4f57 0a20 2020 2062 7269 6768 7420  LLOW.    bright 
+0001a5c0: 3d20 636f 6c6f 7261 6d61 2e53 7479 6c65  = colorama.Style
+0001a5d0: 2e42 5249 4748 540a 2020 2020 7265 7365  .BRIGHT.    rese
+0001a5e0: 7420 3d20 636f 6c6f 7261 6d61 2e53 7479  t = colorama.Sty
+0001a5f0: 6c65 2e52 4553 4554 5f41 4c4c 0a0a 2020  le.RESET_ALL..  
+0001a600: 2020 6966 2063 6c75 7374 6572 5f6e 616d    if cluster_nam
+0001a610: 6573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  es is not None:.
+0001a620: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+0001a630: 7461 6e63 6528 636c 7573 7465 725f 6e61  tance(cluster_na
+0001a640: 6d65 732c 2073 7472 293a 0a20 2020 2020  mes, str):.     
+0001a650: 2020 2020 2020 2063 6c75 7374 6572 5f6e         cluster_n
+0001a660: 616d 6573 203d 205b 636c 7573 7465 725f  ames = [cluster_
+0001a670: 6e61 6d65 735d 0a20 2020 2020 2020 206e  names].        n
+0001a680: 6577 5f72 6563 6f72 6473 203d 205b 5d0a  ew_records = [].
+0001a690: 2020 2020 2020 2020 6e6f 745f 6578 6973          not_exis
+0001a6a0: 745f 636c 7573 7465 725f 6e61 6d65 7320  t_cluster_names 
+0001a6b0: 3d20 5b5d 0a20 2020 2020 2020 2066 6f72  = [].        for
+0001a6c0: 2063 6c75 7374 6572 5f6e 616d 6520 696e   cluster_name in
+0001a6d0: 2063 6c75 7374 6572 5f6e 616d 6573 3a0a   cluster_names:.
+0001a6e0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0001a6f0: 7265 636f 7264 2069 6e20 7265 636f 7264  record in record
+0001a700: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+0001a710: 2020 2069 6620 7265 636f 7264 5b27 6e61     if record['na
+0001a720: 6d65 275d 203d 3d20 636c 7573 7465 725f  me'] == cluster_
+0001a730: 6e61 6d65 3a0a 2020 2020 2020 2020 2020  name:.          
+0001a740: 2020 2020 2020 2020 2020 6e65 775f 7265            new_re
+0001a750: 636f 7264 732e 6170 7065 6e64 2872 6563  cords.append(rec
+0001a760: 6f72 6429 0a20 2020 2020 2020 2020 2020  ord).           
+0001a770: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
+0001a780: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0001a790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a7a0: 206e 6f74 5f65 7869 7374 5f63 6c75 7374   not_exist_clust
+0001a7b0: 6572 5f6e 616d 6573 2e61 7070 656e 6428  er_names.append(
+0001a7c0: 636c 7573 7465 725f 6e61 6d65 290a 2020  cluster_name).  
+0001a7d0: 2020 2020 2020 6966 206e 6f74 5f65 7869        if not_exi
+0001a7e0: 7374 5f63 6c75 7374 6572 5f6e 616d 6573  st_cluster_names
+0001a7f0: 3a0a 2020 2020 2020 2020 2020 2020 636c  :.            cl
+0001a800: 7573 7465 7273 5f73 7472 203d 2027 2c20  usters_str = ', 
+0001a810: 272e 6a6f 696e 286e 6f74 5f65 7869 7374  '.join(not_exist
+0001a820: 5f63 6c75 7374 6572 5f6e 616d 6573 290a  _cluster_names).
+0001a830: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+0001a840: 6572 2e69 6e66 6f28 6627 436c 7573 7465  er.info(f'Cluste
+0001a850: 7228 7329 206e 6f74 2066 6f75 6e64 3a20  r(s) not found: 
+0001a860: 7b62 7269 6768 747d 7b63 6c75 7374 6572  {bright}{cluster
+0001a870: 735f 7374 727d 7b72 6573 6574 7d2e 2729  s_str}{reset}.')
+0001a880: 0a20 2020 2020 2020 2072 6563 6f72 6473  .        records
+0001a890: 203d 206e 6577 5f72 6563 6f72 6473 0a0a   = new_records..
+0001a8a0: 2020 2020 6966 206e 6f74 2072 6566 7265      if not refre
+0001a8b0: 7368 3a0a 2020 2020 2020 2020 7265 7475  sh:.        retu
+0001a8c0: 726e 2072 6563 6f72 6473 0a0a 2020 2020  rn records..    
+0001a8d0: 706c 7572 616c 203d 2027 7327 2069 6620  plural = 's' if 
+0001a8e0: 6c65 6e28 7265 636f 7264 7329 203e 2031  len(records) > 1
+0001a8f0: 2065 6c73 6520 2727 0a20 2020 2070 726f   else ''.    pro
+0001a900: 6772 6573 7320 3d20 7269 6368 5f70 726f  gress = rich_pro
+0001a910: 6772 6573 732e 5072 6f67 7265 7373 2874  gress.Progress(t
+0001a920: 7261 6e73 6965 6e74 3d54 7275 652c 0a20  ransient=True,. 
+0001a930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a950: 2020 2020 2072 6564 6972 6563 745f 7374       redirect_st
+0001a960: 646f 7574 3d46 616c 7365 2c0a 2020 2020  dout=False,.    
+0001a970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a990: 2020 7265 6469 7265 6374 5f73 7464 6572    redirect_stder
+0001a9a0: 723d 4661 6c73 6529 0a20 2020 2074 6173  r=False).    tas
+0001a9b0: 6b20 3d20 7072 6f67 7265 7373 2e61 6464  k = progress.add
+0001a9c0: 5f74 6173 6b28 0a20 2020 2020 2020 2066  _task(.        f
+0001a9d0: 275b 626f 6c64 2063 7961 6e5d 5265 6672  '[bold cyan]Refr
+0001a9e0: 6573 6869 6e67 2073 7461 7475 7320 666f  eshing status fo
+0001a9f0: 7220 7b6c 656e 2872 6563 6f72 6473 297d  r {len(records)}
+0001aa00: 2063 6c75 7374 6572 7b70 6c75 7261 6c7d   cluster{plural}
+0001aa10: 5b2f 5d27 2c0a 2020 2020 2020 2020 746f  [/]',.        to
+0001aa20: 7461 6c3d 6c65 6e28 7265 636f 7264 7329  tal=len(records)
+0001aa30: 290a 0a20 2020 2064 6566 205f 7265 6672  )..    def _refr
+0001aa40: 6573 685f 636c 7573 7465 7228 636c 7573  esh_cluster(clus
+0001aa50: 7465 725f 6e61 6d65 293a 0a20 2020 2020  ter_name):.     
+0001aa60: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+0001aa70: 2020 2020 7265 636f 7264 203d 2072 6566      record = ref
+0001aa80: 7265 7368 5f63 6c75 7374 6572 5f72 6563  resh_cluster_rec
+0001aa90: 6f72 6428 0a20 2020 2020 2020 2020 2020  ord(.           
+0001aaa0: 2020 2020 2063 6c75 7374 6572 5f6e 616d       cluster_nam
+0001aab0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0001aac0: 2020 2066 6f72 6365 5f72 6566 7265 7368     force_refresh
+0001aad0: 5f73 7461 7475 7365 733d 7365 7428 7374  _statuses=set(st
+0001aae0: 6174 7573 5f6c 6962 2e43 6c75 7374 6572  atus_lib.Cluster
+0001aaf0: 5374 6174 7573 292c 0a20 2020 2020 2020  Status),.       
+0001ab00: 2020 2020 2020 2020 2061 6371 7569 7265           acquire
+0001ab10: 5f70 6572 5f63 6c75 7374 6572 5f73 7461  _per_cluster_sta
+0001ab20: 7475 735f 6c6f 636b 3d54 7275 6529 0a20  tus_lock=True). 
+0001ab30: 2020 2020 2020 2065 7863 6570 7420 2865         except (e
+0001ab40: 7863 6570 7469 6f6e 732e 436c 7573 7465  xceptions.Cluste
+0001ab50: 7253 7461 7475 7346 6574 6368 696e 6745  rStatusFetchingE
+0001ab60: 7272 6f72 2c0a 2020 2020 2020 2020 2020  rror,.          
+0001ab70: 2020 2020 2020 6578 6365 7074 696f 6e73        exceptions
+0001ab80: 2e43 6c6f 7564 5573 6572 4964 656e 7469  .CloudUserIdenti
+0001ab90: 7479 4572 726f 722c 0a20 2020 2020 2020  tyError,.       
+0001aba0: 2020 2020 2020 2020 2065 7863 6570 7469           excepti
+0001abb0: 6f6e 732e 436c 7573 7465 724f 776e 6572  ons.ClusterOwner
+0001abc0: 4964 656e 7469 7479 4d69 736d 6174 6368  IdentityMismatch
+0001abd0: 4572 726f 7229 2061 7320 653a 0a20 2020  Error) as e:.   
+0001abe0: 2020 2020 2020 2020 2023 2044 6f20 6e6f           # Do no
+0001abf0: 7420 6661 696c 2074 6865 2065 6e74 6972  t fail the entir
+0001ac00: 6520 7265 6672 6573 6820 7072 6f63 6573  e refresh proces
+0001ac10: 732e 2054 6865 2063 616c 6c65 7220 7769  s. The caller wi
+0001ac20: 6c6c 0a20 2020 2020 2020 2020 2020 2023  ll.            #
+0001ac30: 2068 616e 646c 6520 7468 6520 2755 4e4b   handle the 'UNK
+0001ac40: 4e4f 574e 2720 7374 6174 7573 2c20 616e  NOWN' status, an
+0001ac50: 6420 636f 6c6c 6563 7420 7468 6520 6572  d collect the er
+0001ac60: 726f 7273 2069 6e74 6f0a 2020 2020 2020  rors into.      
+0001ac70: 2020 2020 2020 2320 6120 7461 626c 652e        # a table.
+0001ac80: 0a20 2020 2020 2020 2020 2020 2072 6563  .            rec
+0001ac90: 6f72 6420 3d20 7b27 7374 6174 7573 273a  ord = {'status':
+0001aca0: 2027 554e 4b4e 4f57 4e27 2c20 2765 7272   'UNKNOWN', 'err
+0001acb0: 6f72 273a 2065 7d0a 2020 2020 2020 2020  or': e}.        
+0001acc0: 7072 6f67 7265 7373 2e75 7064 6174 6528  progress.update(
+0001acd0: 7461 736b 2c20 6164 7661 6e63 653d 3129  task, advance=1)
+0001ace0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001acf0: 7265 636f 7264 0a0a 2020 2020 636c 7573  record..    clus
+0001ad00: 7465 725f 6e61 6d65 7320 3d20 5b72 6563  ter_names = [rec
+0001ad10: 6f72 645b 276e 616d 6527 5d20 666f 7220  ord['name'] for 
+0001ad20: 7265 636f 7264 2069 6e20 7265 636f 7264  record in record
+0001ad30: 735d 0a20 2020 2077 6974 6820 7072 6f67  s].    with prog
+0001ad40: 7265 7373 3a0a 2020 2020 2020 2020 7570  ress:.        up
+0001ad50: 6461 7465 645f 7265 636f 7264 7320 3d20  dated_records = 
+0001ad60: 7375 6270 726f 6365 7373 5f75 7469 6c73  subprocess_utils
+0001ad70: 2e72 756e 5f69 6e5f 7061 7261 6c6c 656c  .run_in_parallel
+0001ad80: 280a 2020 2020 2020 2020 2020 2020 5f72  (.            _r
+0001ad90: 6566 7265 7368 5f63 6c75 7374 6572 2c20  efresh_cluster, 
+0001ada0: 636c 7573 7465 725f 6e61 6d65 7329 0a0a  cluster_names)..
+0001adb0: 2020 2020 2320 5368 6f77 2069 6e66 6f72      # Show infor
+0001adc0: 6d61 7469 6f6e 2066 6f72 2072 656d 6f76  mation for remov
+0001add0: 6564 2063 6c75 7374 6572 732e 0a20 2020  ed clusters..   
+0001ade0: 206b 6570 745f 7265 636f 7264 7320 3d20   kept_records = 
+0001adf0: 5b5d 0a20 2020 2061 7574 6f64 6f77 6e5f  [].    autodown_
+0001ae00: 636c 7573 7465 7273 2c20 7265 6d61 696e  clusters, remain
+0001ae10: 696e 675f 636c 7573 7465 7273 2c20 6661  ing_clusters, fa
+0001ae20: 696c 6564 5f63 6c75 7374 6572 7320 3d20  iled_clusters = 
+0001ae30: 5b5d 2c20 5b5d 2c20 5b5d 0a20 2020 2066  [], [], [].    f
+0001ae40: 6f72 2069 2c20 7265 636f 7264 2069 6e20  or i, record in 
+0001ae50: 656e 756d 6572 6174 6528 7265 636f 7264  enumerate(record
+0001ae60: 7329 3a0a 2020 2020 2020 2020 6966 2075  s):.        if u
+0001ae70: 7064 6174 6564 5f72 6563 6f72 6473 5b69  pdated_records[i
+0001ae80: 5d20 6973 204e 6f6e 653a 0a20 2020 2020  ] is None:.     
+0001ae90: 2020 2020 2020 2069 6620 7265 636f 7264         if record
+0001aea0: 5b27 746f 5f64 6f77 6e27 5d3a 0a20 2020  ['to_down']:.   
+0001aeb0: 2020 2020 2020 2020 2020 2020 2061 7574               aut
+0001aec0: 6f64 6f77 6e5f 636c 7573 7465 7273 2e61  odown_clusters.a
+0001aed0: 7070 656e 6428 636c 7573 7465 725f 6e61  ppend(cluster_na
+0001aee0: 6d65 735b 695d 290a 2020 2020 2020 2020  mes[i]).        
+0001aef0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0001af00: 2020 2020 2020 2020 2020 7265 6d61 696e            remain
+0001af10: 696e 675f 636c 7573 7465 7273 2e61 7070  ing_clusters.app
+0001af20: 656e 6428 636c 7573 7465 725f 6e61 6d65  end(cluster_name
+0001af30: 735b 695d 290a 2020 2020 2020 2020 656c  s[i]).        el
+0001af40: 6966 2075 7064 6174 6564 5f72 6563 6f72  if updated_recor
+0001af50: 6473 5b69 5d5b 2773 7461 7475 7327 5d20  ds[i]['status'] 
+0001af60: 3d3d 2027 554e 4b4e 4f57 4e27 3a0a 2020  == 'UNKNOWN':.  
+0001af70: 2020 2020 2020 2020 2020 6661 696c 6564            failed
+0001af80: 5f63 6c75 7374 6572 732e 6170 7065 6e64  _clusters.append
+0001af90: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0001afa0: 2020 2863 6c75 7374 6572 5f6e 616d 6573    (cluster_names
+0001afb0: 5b69 5d2c 2075 7064 6174 6564 5f72 6563  [i], updated_rec
+0001afc0: 6f72 6473 5b69 5d5b 2765 7272 6f72 275d  ords[i]['error']
+0001afd0: 2929 0a20 2020 2020 2020 2020 2020 2023  )).            #
+0001afe0: 204b 6565 7020 7468 6520 6f72 6967 696e   Keep the origin
+0001aff0: 616c 2072 6563 6f72 6420 6966 2074 6865  al record if the
+0001b000: 2073 7461 7475 7320 6973 2075 6e6b 6e6f   status is unkno
+0001b010: 776e 2c0a 2020 2020 2020 2020 2020 2020  wn,.            
+0001b020: 2320 736f 2074 6861 7420 7468 6520 7573  # so that the us
+0001b030: 6572 2063 616e 2073 7469 6c6c 2073 6565  er can still see
+0001b040: 2074 6865 2063 6c75 7374 6572 2e0a 2020   the cluster..  
+0001b050: 2020 2020 2020 2020 2020 6b65 7074 5f72            kept_r
+0001b060: 6563 6f72 6473 2e61 7070 656e 6428 7265  ecords.append(re
+0001b070: 636f 7264 290a 2020 2020 2020 2020 656c  cord).        el
+0001b080: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0001b090: 6b65 7074 5f72 6563 6f72 6473 2e61 7070  kept_records.app
+0001b0a0: 656e 6428 7570 6461 7465 645f 7265 636f  end(updated_reco
+0001b0b0: 7264 735b 695d 290a 0a20 2020 2069 6620  rds[i])..    if 
+0001b0c0: 6175 746f 646f 776e 5f63 6c75 7374 6572  autodown_cluster
+0001b0d0: 733a 0a20 2020 2020 2020 2070 6c75 7261  s:.        plura
+0001b0e0: 6c20 3d20 2773 2720 6966 206c 656e 2861  l = 's' if len(a
+0001b0f0: 7574 6f64 6f77 6e5f 636c 7573 7465 7273  utodown_clusters
+0001b100: 2920 3e20 3120 656c 7365 2027 270a 2020  ) > 1 else ''.  
+0001b110: 2020 2020 2020 636c 7573 7465 725f 7374        cluster_st
+0001b120: 7220 3d20 272c 2027 2e6a 6f69 6e28 6175  r = ', '.join(au
+0001b130: 746f 646f 776e 5f63 6c75 7374 6572 7329  todown_clusters)
+0001b140: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+0001b150: 696e 666f 2866 2741 7574 6f64 6f77 6e65  info(f'Autodowne
+0001b160: 6420 636c 7573 7465 727b 706c 7572 616c  d cluster{plural
+0001b170: 7d3a 2027 0a20 2020 2020 2020 2020 2020  }: '.           
+0001b180: 2020 2020 2020 2020 2066 277b 6272 6967           f'{brig
+0001b190: 6874 7d7b 636c 7573 7465 725f 7374 727d  ht}{cluster_str}
+0001b1a0: 7b72 6573 6574 7d27 290a 2020 2020 6966  {reset}').    if
+0001b1b0: 2072 656d 6169 6e69 6e67 5f63 6c75 7374   remaining_clust
+0001b1c0: 6572 733a 0a20 2020 2020 2020 2070 6c75  ers:.        plu
+0001b1d0: 7261 6c20 3d20 2773 2720 6966 206c 656e  ral = 's' if len
+0001b1e0: 2872 656d 6169 6e69 6e67 5f63 6c75 7374  (remaining_clust
+0001b1f0: 6572 7329 203e 2031 2065 6c73 6520 2727  ers) > 1 else ''
+0001b200: 0a20 2020 2020 2020 2063 6c75 7374 6572  .        cluster
+0001b210: 5f73 7472 203d 2027 2c20 272e 6a6f 696e  _str = ', '.join
+0001b220: 286e 616d 6520 666f 7220 6e61 6d65 2069  (name for name i
+0001b230: 6e20 7265 6d61 696e 696e 675f 636c 7573  n remaining_clus
+0001b240: 7465 7273 290a 2020 2020 2020 2020 6c6f  ters).        lo
+0001b250: 6767 6572 2e77 6172 6e69 6e67 2866 277b  gger.warning(f'{
+0001b260: 7965 6c6c 6f77 7d43 6c75 7374 6572 7b70  yellow}Cluster{p
+0001b270: 6c75 7261 6c7d 2074 6572 6d69 6e61 7465  lural} terminate
+0001b280: 6420 6f6e 2027 0a20 2020 2020 2020 2020  d on '.         
+0001b290: 2020 2020 2020 2020 2020 2020 2020 6627                f'
+0001b2a0: 7468 6520 636c 6f75 643a 207b 7265 7365  the cloud: {rese
+0001b2b0: 747d 7b62 7269 6768 747d 7b63 6c75 7374  t}{bright}{clust
+0001b2c0: 6572 5f73 7472 7d7b 7265 7365 747d 2729  er_str}{reset}')
+0001b2d0: 0a0a 2020 2020 6966 2066 6169 6c65 645f  ..    if failed_
+0001b2e0: 636c 7573 7465 7273 3a0a 2020 2020 2020  clusters:.      
+0001b2f0: 2020 706c 7572 616c 203d 2027 7327 2069    plural = 's' i
+0001b300: 6620 6c65 6e28 6661 696c 6564 5f63 6c75  f len(failed_clu
+0001b310: 7374 6572 7329 203e 2031 2065 6c73 6520  sters) > 1 else 
+0001b320: 2727 0a20 2020 2020 2020 206c 6f67 6765  ''.        logge
+0001b330: 722e 7761 726e 696e 6728 6627 7b79 656c  r.warning(f'{yel
+0001b340: 6c6f 777d 4661 696c 6564 2074 6f20 7265  low}Failed to re
+0001b350: 6672 6573 6820 7374 6174 7573 2066 6f72  fresh status for
+0001b360: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
+0001b370: 2020 2020 2020 2020 2020 6627 7b6c 656e            f'{len
+0001b380: 2866 6169 6c65 645f 636c 7573 7465 7273  (failed_clusters
+0001b390: 297d 2063 6c75 7374 6572 7b70 6c75 7261  )} cluster{plura
+0001b3a0: 6c7d 3a7b 7265 7365 747d 2729 0a20 2020  l}:{reset}').   
+0001b3b0: 2020 2020 2066 6f72 2063 6c75 7374 6572       for cluster
+0001b3c0: 5f6e 616d 652c 2065 2069 6e20 6661 696c  _name, e in fail
+0001b3d0: 6564 5f63 6c75 7374 6572 733a 0a20 2020  ed_clusters:.   
+0001b3e0: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+0001b3f0: 7761 726e 696e 6728 6627 2020 7b62 7269  warning(f'  {bri
+0001b400: 6768 747d 7b63 6c75 7374 6572 5f6e 616d  ght}{cluster_nam
+0001b410: 657d 7b72 6573 6574 7d3a 207b 657d 2729  e}{reset}: {e}')
+0001b420: 0a20 2020 2072 6574 7572 6e20 6b65 7074  .    return kept
+0001b430: 5f72 6563 6f72 6473 0a0a 0a40 7479 7069  _records...@typi
+0001b440: 6e67 2e6f 7665 726c 6f61 640a 6465 6620  ng.overload.def 
+0001b450: 6765 745f 6261 636b 656e 645f 6672 6f6d  get_backend_from
+0001b460: 5f68 616e 646c 6528 0a20 2020 2068 616e  _handle(.    han
+0001b470: 646c 653a 2027 636c 6f75 645f 766d 5f72  dle: 'cloud_vm_r
+0001b480: 6179 5f62 6163 6b65 6e64 2e43 6c6f 7564  ay_backend.Cloud
+0001b490: 566d 5261 7952 6573 6f75 7263 6548 616e  VmRayResourceHan
+0001b4a0: 646c 6527 0a29 202d 3e20 2763 6c6f 7564  dle'.) -> 'cloud
+0001b4b0: 5f76 6d5f 7261 795f 6261 636b 656e 642e  _vm_ray_backend.
+0001b4c0: 436c 6f75 6456 6d52 6179 4261 636b 656e  CloudVmRayBacken
+0001b4d0: 6427 3a0a 2020 2020 2e2e 2e0a 0a0a 4074  d':.    ......@t
+0001b4e0: 7970 696e 672e 6f76 6572 6c6f 6164 0a64  yping.overload.d
+0001b4f0: 6566 2067 6574 5f62 6163 6b65 6e64 5f66  ef get_backend_f
+0001b500: 726f 6d5f 6861 6e64 6c65 280a 2020 2020  rom_handle(.    
+0001b510: 6861 6e64 6c65 3a20 276c 6f63 616c 5f64  handle: 'local_d
+0001b520: 6f63 6b65 725f 6261 636b 656e 642e 4c6f  ocker_backend.Lo
+0001b530: 6361 6c44 6f63 6b65 7252 6573 6f75 7263  calDockerResourc
+0001b540: 6548 616e 646c 6527 0a29 202d 3e20 276c  eHandle'.) -> 'l
+0001b550: 6f63 616c 5f64 6f63 6b65 725f 6261 636b  ocal_docker_back
+0001b560: 656e 642e 4c6f 6361 6c44 6f63 6b65 7242  end.LocalDockerB
+0001b570: 6163 6b65 6e64 273a 0a20 2020 202e 2e2e  ackend':.    ...
+0001b580: 0a0a 0a40 7479 7069 6e67 2e6f 7665 726c  ...@typing.overl
+0001b590: 6f61 640a 6465 6620 6765 745f 6261 636b  oad.def get_back
+0001b5a0: 656e 645f 6672 6f6d 5f68 616e 646c 6528  end_from_handle(
+0001b5b0: 0a20 2020 2020 2020 2068 616e 646c 653a  .        handle:
+0001b5c0: 2062 6163 6b65 6e64 732e 5265 736f 7572   backends.Resour
+0001b5d0: 6365 4861 6e64 6c65 2920 2d3e 2062 6163  ceHandle) -> bac
+0001b5e0: 6b65 6e64 732e 4261 636b 656e 643a 0a20  kends.Backend:. 
+0001b5f0: 2020 202e 2e2e 0a0a 0a64 6566 2067 6574     ......def get
+0001b600: 5f62 6163 6b65 6e64 5f66 726f 6d5f 6861  _backend_from_ha
+0001b610: 6e64 6c65 280a 2020 2020 2020 2020 6861  ndle(.        ha
+0001b620: 6e64 6c65 3a20 6261 636b 656e 6473 2e52  ndle: backends.R
+0001b630: 6573 6f75 7263 6548 616e 646c 6529 202d  esourceHandle) -
+0001b640: 3e20 6261 636b 656e 6473 2e42 6163 6b65  > backends.Backe
+0001b650: 6e64 3a0a 2020 2020 2222 2247 6574 7320  nd:.    """Gets 
+0001b660: 6120 4261 636b 656e 6420 6f62 6a65 6374  a Backend object
+0001b670: 2063 6f72 7265 7370 6f6e 6469 6e67 2074   corresponding t
+0001b680: 6f20 6120 6861 6e64 6c65 2e0a 0a20 2020  o a handle...   
+0001b690: 2049 6e73 7065 6374 7320 6861 6e64 6c65   Inspects handle
+0001b6a0: 2074 7970 6520 746f 2069 6e66 6572 2074   type to infer t
+0001b6b0: 6865 2062 6163 6b65 6e64 2075 7365 6420  he backend used 
+0001b6c0: 666f 7220 7468 6520 7265 736f 7572 6365  for the resource
+0001b6d0: 2e0a 2020 2020 2222 220a 2020 2020 6261  ..    """.    ba
+0001b6e0: 636b 656e 643a 2062 6163 6b65 6e64 732e  ckend: backends.
+0001b6f0: 4261 636b 656e 640a 2020 2020 6966 2069  Backend.    if i
+0001b700: 7369 6e73 7461 6e63 6528 6861 6e64 6c65  sinstance(handle
+0001b710: 2c20 6261 636b 656e 6473 2e43 6c6f 7564  , backends.Cloud
+0001b720: 566d 5261 7952 6573 6f75 7263 6548 616e  VmRayResourceHan
+0001b730: 646c 6529 3a0a 2020 2020 2020 2020 6261  dle):.        ba
+0001b740: 636b 656e 6420 3d20 6261 636b 656e 6473  ckend = backends
+0001b750: 2e43 6c6f 7564 566d 5261 7942 6163 6b65  .CloudVmRayBacke
+0001b760: 6e64 2829 0a20 2020 2065 6c69 6620 6973  nd().    elif is
+0001b770: 696e 7374 616e 6365 2868 616e 646c 652c  instance(handle,
+0001b780: 2062 6163 6b65 6e64 732e 4c6f 6361 6c44   backends.LocalD
+0001b790: 6f63 6b65 7252 6573 6f75 7263 6548 616e  ockerResourceHan
+0001b7a0: 646c 6529 3a0a 2020 2020 2020 2020 6261  dle):.        ba
+0001b7b0: 636b 656e 6420 3d20 6261 636b 656e 6473  ckend = backends
+0001b7c0: 2e4c 6f63 616c 446f 636b 6572 4261 636b  .LocalDockerBack
+0001b7d0: 656e 6428 290a 2020 2020 656c 7365 3a0a  end().    else:.
+0001b7e0: 2020 2020 2020 2020 7261 6973 6520 4e6f          raise No
+0001b7f0: 7449 6d70 6c65 6d65 6e74 6564 4572 726f  tImplementedErro
+0001b800: 7228 0a20 2020 2020 2020 2020 2020 2066  r(.            f
+0001b810: 2748 616e 646c 6520 7479 7065 207b 7479  'Handle type {ty
+0001b820: 7065 2868 616e 646c 6529 7d20 6973 206e  pe(handle)} is n
+0001b830: 6f74 2073 7570 706f 7274 6564 2079 6574  ot supported yet
+0001b840: 2e27 290a 2020 2020 7265 7475 726e 2062  .').    return b
+0001b850: 6163 6b65 6e64 0a0a 0a64 6566 2067 6574  ackend...def get
+0001b860: 5f74 6173 6b5f 6465 6d61 6e64 735f 6469  _task_demands_di
+0001b870: 6374 2874 6173 6b3a 2027 7461 736b 5f6c  ct(task: 'task_l
+0001b880: 6962 2e54 6173 6b27 2920 2d3e 2044 6963  ib.Task') -> Dic
+0001b890: 745b 7374 722c 2066 6c6f 6174 5d3a 0a20  t[str, float]:. 
+0001b8a0: 2020 2022 2222 5265 7475 726e 7320 7468     """Returns th
+0001b8b0: 6520 7265 736f 7572 6365 7320 6469 6374  e resources dict
+0001b8c0: 206f 6620 7468 6520 7461 736b 2e0a 0a20   of the task... 
+0001b8d0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+0001b8e0: 2020 2020 4120 6469 6374 206f 6620 7468      A dict of th
+0001b8f0: 6520 7265 736f 7572 6365 7320 6f66 2074  e resources of t
+0001b900: 6865 2074 6173 6b2e 2054 6865 206b 6579  he task. The key
+0001b910: 7320 6172 6520 7468 6520 7265 736f 7572  s are the resour
+0001b920: 6365 206e 616d 6573 0a20 2020 2020 2020  ce names.       
+0001b930: 2061 6e64 2074 6865 2076 616c 7565 7320   and the values 
+0001b940: 6172 6520 7468 6520 6e75 6d62 6572 206f  are the number o
+0001b950: 6620 7468 6520 7265 736f 7572 6365 732e  f the resources.
+0001b960: 2049 7420 616c 7761 7973 2063 6f6e 7461   It always conta
+0001b970: 696e 730a 2020 2020 2020 2020 7468 6520  ins.        the 
+0001b980: 4350 5520 7265 736f 7572 6365 2028 746f  CPU resource (to
+0001b990: 2063 6f6e 7472 6f6c 2074 6865 206d 6178   control the max
+0001b9a0: 696d 756d 206e 756d 6265 7220 6f66 2074  imum number of t
+0001b9b0: 6173 6b73 292c 2061 6e64 0a20 2020 2020  asks), and.     
+0001b9c0: 2020 206f 7074 696f 6e61 6c6c 7920 6163     optionally ac
+0001b9d0: 6365 6c65 7261 746f 7220 6465 6d61 6e64  celerator demand
+0001b9e0: 732e 0a20 2020 2022 2222 0a20 2020 2023  s..    """.    #
+0001b9f0: 2054 4f44 4f3a 2043 7573 746f 6d20 4350   TODO: Custom CP
+0001ba00: 5520 616e 6420 6f74 6865 7220 6d65 6d6f  U and other memo
+0001ba10: 7279 2072 6573 6f75 7263 6573 2061 7265  ry resources are
+0001ba20: 206e 6f74 2073 7570 706f 7274 6564 2079   not supported y
+0001ba30: 6574 2e0a 2020 2020 2320 466f 7220 736b  et..    # For sk
+0001ba40: 7920 6a6f 6273 2f73 6572 7665 2063 6f6e  y jobs/serve con
+0001ba50: 7472 6f6c 6c65 7220 7461 736b 2c20 7765  troller task, we
+0001ba60: 2073 6574 2074 6865 2043 5055 2072 6573   set the CPU res
+0001ba70: 6f75 7263 6520 746f 2061 2073 6d61 6c6c  ource to a small
+0001ba80: 6572 0a20 2020 2023 2076 616c 7565 2074  er.    # value t
+0001ba90: 6f20 7375 7070 6f72 7420 6120 6c61 7267  o support a larg
+0001baa0: 6572 206e 756d 6265 7220 6f66 206d 616e  er number of man
+0001bab0: 6167 6564 206a 6f62 7320 616e 6420 7365  aged jobs and se
+0001bac0: 7276 6963 6573 2e0a 2020 2020 7265 736f  rvices..    reso
+0001bad0: 7572 6365 735f 6469 6374 203d 207b 0a20  urces_dict = {. 
+0001bae0: 2020 2020 2020 2027 4350 5527 3a20 2863         'CPU': (c
+0001baf0: 6f6e 7374 616e 7473 2e43 4f4e 5452 4f4c  onstants.CONTROL
+0001bb00: 4c45 525f 5052 4f43 4553 535f 4350 555f  LER_PROCESS_CPU_
+0001bb10: 4445 4d41 4e44 0a20 2020 2020 2020 2020  DEMAND.         
+0001bb20: 2020 2020 2020 2069 6620 7461 736b 2e69         if task.i
+0001bb30: 735f 636f 6e74 726f 6c6c 6572 5f74 6173  s_controller_tas
+0001bb40: 6b28 2920 656c 7365 2044 4546 4155 4c54  k() else DEFAULT
+0001bb50: 5f54 4153 4b5f 4350 555f 4445 4d41 4e44  _TASK_CPU_DEMAND
+0001bb60: 290a 2020 2020 7d0a 2020 2020 6966 2074  ).    }.    if t
+0001bb70: 6173 6b2e 6265 7374 5f72 6573 6f75 7263  ask.best_resourc
+0001bb80: 6573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  es is not None:.
+0001bb90: 2020 2020 2020 2020 7265 736f 7572 6365          resource
+0001bba0: 7320 3d20 7461 736b 2e62 6573 745f 7265  s = task.best_re
+0001bbb0: 736f 7572 6365 730a 2020 2020 656c 7365  sources.    else
+0001bbc0: 3a0a 2020 2020 2020 2020 2320 5461 736b  :.        # Task
+0001bbd0: 206d 6179 2028 652e 672e 2c20 736b 7920   may (e.g., sky 
+0001bbe0: 6c61 756e 6368 2920 6f72 206d 6179 206e  launch) or may n
+0001bbf0: 6f74 2028 652e 672e 2c20 736b 7920 6578  ot (e.g., sky ex
+0001bc00: 6563 2920 6861 7665 2075 6e64 6572 676f  ec) have undergo
+0001bc10: 6e65 0a20 2020 2020 2020 2023 2073 6b79  ne.        # sky
+0001bc20: 2e6f 7074 696d 697a 6528 292c 2073 6f20  .optimize(), so 
+0001bc30: 6265 7374 5f72 6573 6f75 7263 6573 206d  best_resources m
+0001bc40: 6179 2062 6520 4e6f 6e65 2e0a 2020 2020  ay be None..    
+0001bc50: 2020 2020 6173 7365 7274 206c 656e 2874      assert len(t
+0001bc60: 6173 6b2e 7265 736f 7572 6365 7329 203d  ask.resources) =
+0001bc70: 3d20 312c 2074 6173 6b2e 7265 736f 7572  = 1, task.resour
+0001bc80: 6365 730a 2020 2020 2020 2020 7265 736f  ces.        reso
+0001bc90: 7572 6365 7320 3d20 6c69 7374 2874 6173  urces = list(tas
+0001bca0: 6b2e 7265 736f 7572 6365 7329 5b30 5d0a  k.resources)[0].
+0001bcb0: 2020 2020 6966 2072 6573 6f75 7263 6573      if resources
+0001bcc0: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
+0001bcd0: 2072 6573 6f75 7263 6573 2e61 6363 656c   resources.accel
+0001bce0: 6572 6174 6f72 7320 6973 206e 6f74 204e  erators is not N
+0001bcf0: 6f6e 653a 0a20 2020 2020 2020 2072 6573  one:.        res
+0001bd00: 6f75 7263 6573 5f64 6963 742e 7570 6461  ources_dict.upda
+0001bd10: 7465 2872 6573 6f75 7263 6573 2e61 6363  te(resources.acc
+0001bd20: 656c 6572 6174 6f72 7329 0a20 2020 2072  elerators).    r
+0001bd30: 6574 7572 6e20 7265 736f 7572 6365 735f  eturn resources_
+0001bd40: 6469 6374 0a0a 0a64 6566 2067 6574 5f74  dict...def get_t
+0001bd50: 6173 6b5f 7265 736f 7572 6365 735f 7374  ask_resources_st
+0001bd60: 7228 7461 736b 3a20 2774 6173 6b5f 6c69  r(task: 'task_li
+0001bd70: 622e 5461 736b 272c 0a20 2020 2020 2020  b.Task',.       
+0001bd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bd90: 2020 2020 6973 5f6d 616e 6167 6564 5f6a      is_managed_j
+0001bda0: 6f62 3a20 626f 6f6c 203d 2046 616c 7365  ob: bool = False
+0001bdb0: 2920 2d3e 2073 7472 3a0a 2020 2020 2222  ) -> str:.    ""
+0001bdc0: 2252 6574 7572 6e73 2074 6865 2072 6573  "Returns the res
+0001bdd0: 6f75 7263 6573 2073 7472 696e 6720 6f66  ources string of
+0001bde0: 2074 6865 2074 6173 6b2e 0a0a 2020 2020   the task...    
+0001bdf0: 5468 6520 7265 736f 7572 6365 7320 7374  The resources st
+0001be00: 7269 6e67 2069 7320 6f6e 6c79 2075 7365  ring is only use
+0001be10: 6420 6173 2061 2064 6973 706c 6179 2070  d as a display p
+0001be20: 7572 706f 7365 2c20 736f 2077 6520 6f6e  urpose, so we on
+0001be30: 6c79 2073 686f 770a 2020 2020 7468 6520  ly show.    the 
+0001be40: 6163 6365 6c65 7261 746f 7220 6465 6d61  accelerator dema
+0001be50: 6e64 7320 2869 6620 616e 7929 2e20 4f74  nds (if any). Ot
+0001be60: 6865 7277 6973 652c 2074 6865 2043 5055  herwise, the CPU
+0001be70: 2064 656d 616e 6420 6973 2073 686f 776e   demand is shown
+0001be80: 2e0a 2020 2020 2222 220a 2020 2020 7370  ..    """.    sp
+0001be90: 6f74 5f73 7472 203d 2027 270a 2020 2020  ot_str = ''.    
+0001bea0: 7461 736b 5f63 7075 5f64 656d 616e 6420  task_cpu_demand 
+0001beb0: 3d20 2873 7472 2863 6f6e 7374 616e 7473  = (str(constants
+0001bec0: 2e43 4f4e 5452 4f4c 4c45 525f 5052 4f43  .CONTROLLER_PROC
+0001bed0: 4553 535f 4350 555f 4445 4d41 4e44 290a  ESS_CPU_DEMAND).
+0001bee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bef0: 2020 2020 2020 2069 6620 7461 736b 2e69         if task.i
+0001bf00: 735f 636f 6e74 726f 6c6c 6572 5f74 6173  s_controller_tas
+0001bf10: 6b28 2920 656c 7365 0a20 2020 2020 2020  k() else.       
+0001bf20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bf30: 7374 7228 4445 4641 554c 545f 5441 534b  str(DEFAULT_TASK
+0001bf40: 5f43 5055 5f44 454d 414e 4429 290a 2020  _CPU_DEMAND)).  
+0001bf50: 2020 6966 2074 6173 6b2e 6265 7374 5f72    if task.best_r
+0001bf60: 6573 6f75 7263 6573 2069 7320 6e6f 7420  esources is not 
+0001bf70: 4e6f 6e65 3a0a 2020 2020 2020 2020 6163  None:.        ac
+0001bf80: 6365 6c65 7261 746f 725f 6469 6374 203d  celerator_dict =
+0001bf90: 2074 6173 6b2e 6265 7374 5f72 6573 6f75   task.best_resou
+0001bfa0: 7263 6573 2e61 6363 656c 6572 6174 6f72  rces.accelerator
+0001bfb0: 730a 2020 2020 2020 2020 6966 2069 735f  s.        if is_
+0001bfc0: 6d61 6e61 6765 645f 6a6f 623a 0a20 2020  managed_job:.   
+0001bfd0: 2020 2020 2020 2020 2069 6620 7461 736b           if task
+0001bfe0: 2e62 6573 745f 7265 736f 7572 6365 732e  .best_resources.
+0001bff0: 7573 655f 7370 6f74 3a0a 2020 2020 2020  use_spot:.      
+0001c000: 2020 2020 2020 2020 2020 7370 6f74 5f73            spot_s
+0001c010: 7472 203d 2027 5b53 706f 745d 270a 2020  tr = '[Spot]'.  
+0001c020: 2020 2020 2020 2020 2020 7461 736b 5f63            task_c
+0001c030: 7075 5f64 656d 616e 6420 3d20 7461 736b  pu_demand = task
+0001c040: 2e62 6573 745f 7265 736f 7572 6365 732e  .best_resources.
+0001c050: 6370 7573 0a20 2020 2020 2020 2069 6620  cpus.        if 
+0001c060: 6163 6365 6c65 7261 746f 725f 6469 6374  accelerator_dict
+0001c070: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+0001c080: 2020 2020 2020 7265 736f 7572 6365 735f        resources_
+0001c090: 7374 7220 3d20 6627 4350 553a 7b74 6173  str = f'CPU:{tas
+0001c0a0: 6b5f 6370 755f 6465 6d61 6e64 7d27 0a20  k_cpu_demand}'. 
+0001c0b0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0001c0c0: 2020 2020 2020 2020 2072 6573 6f75 7263           resourc
+0001c0d0: 6573 5f73 7472 203d 2027 2c20 272e 6a6f  es_str = ', '.jo
+0001c0e0: 696e 280a 2020 2020 2020 2020 2020 2020  in(.            
+0001c0f0: 2020 2020 6627 7b6b 7d3a 7b76 7d27 2066      f'{k}:{v}' f
+0001c100: 6f72 206b 2c20 7620 696e 2061 6363 656c  or k, v in accel
+0001c110: 6572 6174 6f72 5f64 6963 742e 6974 656d  erator_dict.item
+0001c120: 7328 2929 0a20 2020 2065 6c73 653a 0a20  s()).    else:. 
+0001c130: 2020 2020 2020 2072 6573 6f75 7263 655f         resource_
+0001c140: 6163 6365 6c65 7261 746f 7273 203d 205b  accelerators = [
+0001c150: 5d0a 2020 2020 2020 2020 6d69 6e5f 6370  ].        min_cp
+0001c160: 7573 203d 2066 6c6f 6174 2827 696e 6627  us = float('inf'
+0001c170: 290a 2020 2020 2020 2020 7370 6f74 5f74  ).        spot_t
+0001c180: 7970 653a 2053 6574 5b73 7472 5d20 3d20  ype: Set[str] = 
+0001c190: 7365 7428 290a 2020 2020 2020 2020 666f  set().        fo
+0001c1a0: 7220 7265 736f 7572 6365 2069 6e20 7461  r resource in ta
+0001c1b0: 736b 2e72 6573 6f75 7263 6573 3a0a 2020  sk.resources:.  
+0001c1c0: 2020 2020 2020 2020 2020 7461 736b 5f63            task_c
+0001c1d0: 7075 5f64 656d 616e 6420 3d20 2731 2b27  pu_demand = '1+'
+0001c1e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0001c1f0: 7265 736f 7572 6365 2e63 7075 7320 6973  resource.cpus is
+0001c200: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0001c210: 2020 2020 2020 2020 2020 2074 6173 6b5f             task_
+0001c220: 6370 755f 6465 6d61 6e64 203d 2072 6573  cpu_demand = res
+0001c230: 6f75 7263 652e 6370 7573 0a20 2020 2020  ource.cpus.     
+0001c240: 2020 2020 2020 206d 696e 5f63 7075 7320         min_cpus 
+0001c250: 3d20 6d69 6e28 6d69 6e5f 6370 7573 2c20  = min(min_cpus, 
+0001c260: 666c 6f61 7428 7461 736b 5f63 7075 5f64  float(task_cpu_d
+0001c270: 656d 616e 642e 7374 7269 7028 272b 2027  emand.strip('+ '
+0001c280: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
+0001c290: 6966 2072 6573 6f75 7263 652e 7573 655f  if resource.use_
+0001c2a0: 7370 6f74 3a0a 2020 2020 2020 2020 2020  spot:.          
+0001c2b0: 2020 2020 2020 7370 6f74 5f74 7970 652e        spot_type.
+0001c2c0: 6164 6428 2753 706f 7427 290a 2020 2020  add('Spot').    
+0001c2d0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0001c2e0: 2020 2020 2020 2020 2020 2020 2020 7370                sp
+0001c2f0: 6f74 5f74 7970 652e 6164 6428 274f 6e2d  ot_type.add('On-
+0001c300: 6465 6d61 6e64 2729 0a0a 2020 2020 2020  demand')..      
+0001c310: 2020 2020 2020 6966 2072 6573 6f75 7263        if resourc
+0001c320: 652e 6163 6365 6c65 7261 746f 7273 2069  e.accelerators i
+0001c330: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+0001c340: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+0001c350: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0001c360: 206b 2c20 7620 696e 2072 6573 6f75 7263   k, v in resourc
+0001c370: 652e 6163 6365 6c65 7261 746f 7273 2e69  e.accelerators.i
+0001c380: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
+0001c390: 2020 2020 2020 2020 7265 736f 7572 6365          resource
+0001c3a0: 5f61 6363 656c 6572 6174 6f72 732e 6170  _accelerators.ap
+0001c3b0: 7065 6e64 2866 277b 6b7d 3a7b 767d 2729  pend(f'{k}:{v}')
+0001c3c0: 0a0a 2020 2020 2020 2020 6966 2069 735f  ..        if is_
+0001c3d0: 6d61 6e61 6765 645f 6a6f 623a 0a20 2020  managed_job:.   
+0001c3e0: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
+0001c3f0: 7461 736b 2e72 6573 6f75 7263 6573 2920  task.resources) 
+0001c400: 3e20 313a 0a20 2020 2020 2020 2020 2020  > 1:.           
+0001c410: 2020 2020 2074 6173 6b5f 6370 755f 6465       task_cpu_de
+0001c420: 6d61 6e64 203d 2066 277b 6d69 6e5f 6370  mand = f'{min_cp
+0001c430: 7573 7d2b 270a 2020 2020 2020 2020 2020  us}+'.          
+0001c440: 2020 6966 2027 5370 6f74 2720 696e 2073    if 'Spot' in s
+0001c450: 706f 745f 7479 7065 3a0a 2020 2020 2020  pot_type:.      
+0001c460: 2020 2020 2020 2020 2020 7370 6f74 5f73            spot_s
+0001c470: 7472 203d 2027 7c27 2e6a 6f69 6e28 736f  tr = '|'.join(so
+0001c480: 7274 6564 2873 706f 745f 7479 7065 2929  rted(spot_type))
+0001c490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c4a0: 2073 706f 745f 7374 7220 3d20 6627 5b7b   spot_str = f'[{
+0001c4b0: 7370 6f74 5f73 7472 7d5d 270a 2020 2020  spot_str}]'.    
+0001c4c0: 2020 2020 6966 2072 6573 6f75 7263 655f      if resource_
+0001c4d0: 6163 6365 6c65 7261 746f 7273 3a0a 2020  accelerators:.  
+0001c4e0: 2020 2020 2020 2020 2020 7265 736f 7572            resour
+0001c4f0: 6365 735f 7374 7220 3d20 272c 2027 2e6a  ces_str = ', '.j
+0001c500: 6f69 6e28 7365 7428 7265 736f 7572 6365  oin(set(resource
+0001c510: 5f61 6363 656c 6572 6174 6f72 7329 290a  _accelerators)).
+0001c520: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0001c530: 2020 2020 2020 2020 2020 7265 736f 7572            resour
+0001c540: 6365 735f 7374 7220 3d20 6627 4350 553a  ces_str = f'CPU:
+0001c550: 7b74 6173 6b5f 6370 755f 6465 6d61 6e64  {task_cpu_demand
+0001c560: 7d27 0a20 2020 2072 6573 6f75 7263 6573  }'.    resources
+0001c570: 5f73 7472 203d 2066 277b 7461 736b 2e6e  _str = f'{task.n
+0001c580: 756d 5f6e 6f64 6573 7d78 5b7b 7265 736f  um_nodes}x[{reso
+0001c590: 7572 6365 735f 7374 727d 5d7b 7370 6f74  urces_str}]{spot
+0001c5a0: 5f73 7472 7d27 0a20 2020 2072 6574 7572  _str}'.    retur
+0001c5b0: 6e20 7265 736f 7572 6365 735f 7374 720a  n resources_str.
+0001c5c0: 0a0a 2320 4861 6e64 6c65 2063 7472 6c2d  ..# Handle ctrl-
+0001c5d0: 630a 6465 6620 696e 7465 7272 7570 745f  c.def interrupt_
+0001c5e0: 6861 6e64 6c65 7228 7369 676e 756d 2c20  handler(signum, 
+0001c5f0: 6672 616d 6529 3a0a 2020 2020 6465 6c20  frame):.    del 
+0001c600: 7369 676e 756d 2c20 6672 616d 650a 2020  signum, frame.  
+0001c610: 2020 7375 6270 726f 6365 7373 5f75 7469    subprocess_uti
+0001c620: 6c73 2e6b 696c 6c5f 6368 696c 6472 656e  ls.kill_children
+0001c630: 5f70 726f 6365 7373 6573 2829 0a20 2020  _processes().   
+0001c640: 2023 2041 766f 6964 2075 7369 6e67 206c   # Avoid using l
+0001c650: 6f67 6765 7220 6865 7265 2c20 6173 2069  ogger here, as i
+0001c660: 7420 7769 6c6c 2070 7269 6e74 2074 6865  t will print the
+0001c670: 2073 7461 636b 2074 7261 6365 2066 6f72   stack trace for
+0001c680: 2062 726f 6b65 6e0a 2020 2020 2320 7069   broken.    # pi
+0001c690: 7065 2c20 7768 656e 2074 6865 206f 7574  pe, when the out
+0001c6a0: 7075 7420 6973 2070 6970 6564 2074 6f20  put is piped to 
+0001c6b0: 616e 6f74 6865 7220 7072 6f67 7261 6d2e  another program.
+0001c6c0: 0a20 2020 2070 7269 6e74 2866 277b 636f  .    print(f'{co
+0001c6d0: 6c6f 7261 6d61 2e53 7479 6c65 2e44 494d  lorama.Style.DIM
+0001c6e0: 7d54 6970 3a20 5468 6520 6a6f 6220 7769  }Tip: The job wi
+0001c6f0: 6c6c 206b 6565 7020 270a 2020 2020 2020  ll keep '.      
+0001c700: 2020 2020 6627 7275 6e6e 696e 6720 6166      f'running af
+0001c710: 7465 7220 4374 726c 2d43 2e7b 636f 6c6f  ter Ctrl-C.{colo
+0001c720: 7261 6d61 2e53 7479 6c65 2e52 4553 4554  rama.Style.RESET
+0001c730: 5f41 4c4c 7d27 290a 2020 2020 7769 7468  _ALL}').    with
+0001c740: 2075 785f 7574 696c 732e 7072 696e 745f   ux_utils.print_
+0001c750: 6578 6365 7074 696f 6e5f 6e6f 5f74 7261  exception_no_tra
+0001c760: 6365 6261 636b 2829 3a0a 2020 2020 2020  ceback():.      
+0001c770: 2020 7261 6973 6520 4b65 7962 6f61 7264    raise Keyboard
+0001c780: 496e 7465 7272 7570 7428 6578 6365 7074  Interrupt(except
+0001c790: 696f 6e73 2e4b 4559 424f 4152 445f 494e  ions.KEYBOARD_IN
+0001c7a0: 5445 5252 5550 545f 434f 4445 290a 0a0a  TERRUPT_CODE)...
+0001c7b0: 2320 4861 6e64 6c65 2063 7472 6c2d 7a0a  # Handle ctrl-z.
+0001c7c0: 6465 6620 7374 6f70 5f68 616e 646c 6572  def stop_handler
+0001c7d0: 2873 6967 6e75 6d2c 2066 7261 6d65 293a  (signum, frame):
+0001c7e0: 0a20 2020 2064 656c 2073 6967 6e75 6d2c  .    del signum,
+0001c7f0: 2066 7261 6d65 0a20 2020 2073 7562 7072   frame.    subpr
+0001c800: 6f63 6573 735f 7574 696c 732e 6b69 6c6c  ocess_utils.kill
+0001c810: 5f63 6869 6c64 7265 6e5f 7072 6f63 6573  _children_proces
+0001c820: 7365 7328 290a 2020 2020 2320 4176 6f69  ses().    # Avoi
+0001c830: 6420 7573 696e 6720 6c6f 6767 6572 2068  d using logger h
+0001c840: 6572 652c 2061 7320 6974 2077 696c 6c20  ere, as it will 
+0001c850: 7072 696e 7420 7468 6520 7374 6163 6b20  print the stack 
+0001c860: 7472 6163 6520 666f 7220 6272 6f6b 656e  trace for broken
+0001c870: 0a20 2020 2023 2070 6970 652c 2077 6865  .    # pipe, whe
+0001c880: 6e20 7468 6520 6f75 7470 7574 2069 7320  n the output is 
+0001c890: 7069 7065 6420 746f 2061 6e6f 7468 6572  piped to another
+0001c8a0: 2070 726f 6772 616d 2e0a 2020 2020 7072   program..    pr
+0001c8b0: 696e 7428 6627 7b63 6f6c 6f72 616d 612e  int(f'{colorama.
+0001c8c0: 5374 796c 652e 4449 4d7d 5469 703a 2054  Style.DIM}Tip: T
+0001c8d0: 6865 206a 6f62 2077 696c 6c20 6b65 6570  he job will keep
+0001c8e0: 2027 0a20 2020 2020 2020 2020 2066 2772   '.          f'r
+0001c8f0: 756e 6e69 6e67 2061 6674 6572 2043 7472  unning after Ctr
+0001c900: 6c2d 5a2e 7b63 6f6c 6f72 616d 612e 5374  l-Z.{colorama.St
+0001c910: 796c 652e 5245 5345 545f 414c 4c7d 2729  yle.RESET_ALL}')
+0001c920: 0a20 2020 2077 6974 6820 7578 5f75 7469  .    with ux_uti
+0001c930: 6c73 2e70 7269 6e74 5f65 7863 6570 7469  ls.print_excepti
+0001c940: 6f6e 5f6e 6f5f 7472 6163 6562 6163 6b28  on_no_traceback(
+0001c950: 293a 0a20 2020 2020 2020 2072 6169 7365  ):.        raise
+0001c960: 204b 6579 626f 6172 6449 6e74 6572 7275   KeyboardInterru
+0001c970: 7074 2865 7863 6570 7469 6f6e 732e 5349  pt(exceptions.SI
+0001c980: 4754 5354 505f 434f 4445 290a 0a0a 6465  GTSTP_CODE)...de
+0001c990: 6620 7275 6e5f 636f 6d6d 616e 645f 616e  f run_command_an
+0001c9a0: 645f 6861 6e64 6c65 5f73 7368 5f66 6169  d_handle_ssh_fai
+0001c9b0: 6c75 7265 2872 756e 6e65 723a 2063 6f6d  lure(runner: com
+0001c9c0: 6d61 6e64 5f72 756e 6e65 722e 5353 4843  mand_runner.SSHC
+0001c9d0: 6f6d 6d61 6e64 5275 6e6e 6572 2c0a 2020  ommandRunner,.  
+0001c9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ca00: 2020 2020 2063 6f6d 6d61 6e64 3a20 7374       command: st
+0001ca10: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+0001ca20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ca30: 2020 2020 2020 2020 2020 6661 696c 7572            failur
+0001ca40: 655f 6d65 7373 6167 653a 2073 7472 2920  e_message: str) 
+0001ca50: 2d3e 2073 7472 3a0a 2020 2020 2222 2252  -> str:.    """R
+0001ca60: 756e 7320 636f 6d6d 616e 6420 7265 6d6f  uns command remo
+0001ca70: 7465 6c79 2061 6e64 2072 6574 7572 6e73  tely and returns
+0001ca80: 206f 7574 7075 7420 7769 7468 2070 726f   output with pro
+0001ca90: 7065 7220 6572 726f 7220 6861 6e64 6c69  per error handli
+0001caa0: 6e67 2e22 2222 0a20 2020 2072 632c 2073  ng.""".    rc, s
+0001cab0: 7464 6f75 742c 2073 7464 6572 7220 3d20  tdout, stderr = 
+0001cac0: 7275 6e6e 6572 2e72 756e 2863 6f6d 6d61  runner.run(comma
+0001cad0: 6e64 2c0a 2020 2020 2020 2020 2020 2020  nd,.            
+0001cae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001caf0: 2020 2020 2020 2020 7265 7175 6972 655f          require_
+0001cb00: 6f75 7470 7574 733d 5472 7565 2c0a 2020  outputs=True,.  
+0001cb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cb30: 2020 7374 7265 616d 5f6c 6f67 733d 4661    stream_logs=Fa
+0001cb40: 6c73 6529 0a20 2020 2069 6620 7263 203d  lse).    if rc =
+0001cb50: 3d20 3235 353a 0a20 2020 2020 2020 2023  = 255:.        #
+0001cb60: 2053 5348 2066 6169 6c65 640a 2020 2020   SSH failed.    
+0001cb70: 2020 2020 7261 6973 6520 5275 6e74 696d      raise Runtim
+0001cb80: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
+0001cb90: 2020 2020 6627 5353 4820 7769 7468 2075      f'SSH with u
+0001cba0: 7365 7220 7b72 756e 6e65 722e 7373 685f  ser {runner.ssh_
+0001cbb0: 7573 6572 7d20 616e 6420 6b65 7920 7b72  user} and key {r
+0001cbc0: 756e 6e65 722e 7373 685f 7072 6976 6174  unner.ssh_privat
+0001cbd0: 655f 6b65 797d 2027 0a20 2020 2020 2020  e_key} '.       
+0001cbe0: 2020 2020 2066 2774 6f20 7b72 756e 6e65       f'to {runne
+0001cbf0: 722e 6970 7d20 6661 696c 6564 2e20 5468  r.ip} failed. Th
+0001cc00: 6973 2069 7320 6d6f 7374 206c 696b 656c  is is most likel
+0001cc10: 7920 6475 6520 746f 2069 6e63 6f72 7265  y due to incorre
+0001cc20: 6374 2027 0a20 2020 2020 2020 2020 2020  ct '.           
+0001cc30: 2027 6372 6564 656e 7469 616c 7320 6f72   'credentials or
+0001cc40: 2069 6e63 6f72 7265 6374 2070 6572 6d69   incorrect permi
+0001cc50: 7373 696f 6e73 2066 6f72 2074 6865 206b  ssions for the k
+0001cc60: 6579 2066 696c 652e 2043 6865 636b 2027  ey file. Check '
+0001cc70: 0a20 2020 2020 2020 2020 2020 2027 796f  .            'yo
+0001cc80: 7572 2063 7265 6465 6e74 6961 6c73 2061  ur credentials a
+0001cc90: 6e64 2074 7279 2061 6761 696e 2e27 290a  nd try again.').
+0001cca0: 2020 2020 7375 6270 726f 6365 7373 5f75      subprocess_u
+0001ccb0: 7469 6c73 2e68 616e 646c 655f 7265 7475  tils.handle_retu
+0001ccc0: 726e 636f 6465 2872 632c 0a20 2020 2020  rncode(rc,.     
+0001ccd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ccf0: 2020 636f 6d6d 616e 642c 0a20 2020 2020    command,.     
+0001cd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cd20: 2020 6661 696c 7572 655f 6d65 7373 6167    failure_messag
+0001cd30: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0001cd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cd50: 2020 2020 2020 2020 2020 7374 6465 7272            stderr
+0001cd60: 3d73 7464 6572 7229 0a20 2020 2072 6574  =stderr).    ret
+0001cd70: 7572 6e20 7374 646f 7574 0a0a 0a64 6566  urn stdout...def
+0001cd80: 2063 6865 636b 5f72 7379 6e63 5f69 6e73   check_rsync_ins
+0001cd90: 7461 6c6c 6564 2829 202d 3e20 4e6f 6e65  talled() -> None
+0001cda0: 3a0a 2020 2020 2222 2243 6865 636b 7320  :.    """Checks 
+0001cdb0: 6966 2072 7379 6e63 2069 7320 696e 7374  if rsync is inst
+0001cdc0: 616c 6c65 642e 0a0a 2020 2020 5261 6973  alled...    Rais
+0001cdd0: 6573 3a0a 2020 2020 2020 2020 5275 6e74  es:.        Runt
+0001cde0: 696d 6545 7272 6f72 3a20 6966 2072 7379  imeError: if rsy
+0001cdf0: 6e63 2069 7320 6e6f 7420 696e 7374 616c  nc is not instal
+0001ce00: 6c65 6420 696e 2074 6865 206d 6163 6869  led in the machi
+0001ce10: 6e65 2e0a 2020 2020 2222 220a 2020 2020  ne..    """.    
+0001ce20: 7472 793a 0a20 2020 2020 2020 2073 7562  try:.        sub
+0001ce30: 7072 6f63 6573 732e 7275 6e28 2772 7379  process.run('rsy
+0001ce40: 6e63 202d 2d76 6572 7369 6f6e 272c 0a20  nc --version',. 
+0001ce50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ce60: 2020 2020 2020 7368 656c 6c3d 5472 7565        shell=True
+0001ce70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001ce80: 2020 2020 2020 2020 2063 6865 636b 3d54           check=T
+0001ce90: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+0001cea0: 2020 2020 2020 2020 2020 2020 7374 646f              stdo
+0001ceb0: 7574 3d73 7562 7072 6f63 6573 732e 5049  ut=subprocess.PI
+0001cec0: 5045 2c0a 2020 2020 2020 2020 2020 2020  PE,.            
+0001ced0: 2020 2020 2020 2020 2020 2073 7464 6572             stder
+0001cee0: 723d 7375 6270 726f 6365 7373 2e50 4950  r=subprocess.PIP
+0001cef0: 4529 0a20 2020 2065 7863 6570 7420 7375  E).    except su
+0001cf00: 6270 726f 6365 7373 2e43 616c 6c65 6450  bprocess.CalledP
+0001cf10: 726f 6365 7373 4572 726f 723a 0a20 2020  rocessError:.   
+0001cf20: 2020 2020 2077 6974 6820 7578 5f75 7469       with ux_uti
+0001cf30: 6c73 2e70 7269 6e74 5f65 7863 6570 7469  ls.print_excepti
+0001cf40: 6f6e 5f6e 6f5f 7472 6163 6562 6163 6b28  on_no_traceback(
+0001cf50: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+0001cf60: 6169 7365 2052 756e 7469 6d65 4572 726f  aise RuntimeErro
+0001cf70: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+0001cf80: 2020 2027 6072 7379 6e63 6020 6973 2072     '`rsync` is r
+0001cf90: 6571 7569 7265 6420 666f 7220 7072 6f76  equired for prov
+0001cfa0: 6973 696f 6e69 6e67 2061 6e64 270a 2020  isioning and'.  
+0001cfb0: 2020 2020 2020 2020 2020 2020 2020 2720                ' 
+0001cfc0: 6974 2069 7320 6e6f 7420 696e 7374 616c  it is not instal
+0001cfd0: 6c65 642e 2046 6f72 2044 6562 6961 6e2f  led. For Debian/
+0001cfe0: 5562 756e 7475 2073 7973 7465 6d2c 2027  Ubuntu system, '
+0001cff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001d000: 2027 696e 7374 616c 6c20 6974 2077 6974   'install it wit
+0001d010: 683a 5c6e 270a 2020 2020 2020 2020 2020  h:\n'.          
+0001d020: 2020 2020 2020 2720 2024 2073 7564 6f20        '  $ sudo 
+0001d030: 6170 7420 696e 7374 616c 6c20 7273 796e  apt install rsyn
+0001d040: 6327 2920 6672 6f6d 204e 6f6e 650a 0a0a  c') from None...
+0001d050: 6465 6620 6368 6563 6b5f 7374 616c 655f  def check_stale_
+0001d060: 7275 6e74 696d 655f 6f6e 5f72 656d 6f74  runtime_on_remot
+0001d070: 6528 7265 7475 726e 636f 6465 3a20 696e  e(returncode: in
+0001d080: 742c 2073 7464 6572 723a 2073 7472 2c0a  t, stderr: str,.
+0001d090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d0b0: 2020 636c 7573 7465 725f 6e61 6d65 3a20    cluster_name: 
+0001d0c0: 7374 7229 202d 3e20 4e6f 6e65 3a0a 2020  str) -> None:.  
+0001d0d0: 2020 2222 2252 6169 7365 7320 5275 6e74    """Raises Runt
+0001d0e0: 696d 6545 7272 6f72 2069 6620 7265 6d6f  imeError if remo
+0001d0f0: 7465 2053 6b79 5069 6c6f 7420 7275 6e74  te SkyPilot runt
+0001d100: 696d 6520 6e65 6564 7320 746f 2062 6520  ime needs to be 
+0001d110: 7570 6461 7465 642e 0a0a 2020 2020 5765  updated...    We
+0001d120: 2064 6574 6563 7420 7468 6973 2062 7920   detect this by 
+0001d130: 7061 7273 696e 6720 6365 7274 6169 6e20  parsing certain 
+0001d140: 6261 636b 7761 7264 2d69 6e63 6f6d 7061  backward-incompa
+0001d150: 7469 626c 6520 6572 726f 7220 6d65 7373  tible error mess
+0001d160: 6167 6573 2066 726f 6d0a 2020 2020 6073  ages from.    `s
+0001d170: 7464 6572 7260 2e20 5479 7069 6361 6c6c  tderr`. Typicall
+0001d180: 7920 6475 6520 746f 2074 6865 206c 6f63  y due to the loc
+0001d190: 616c 2063 6c69 656e 7420 7665 7273 696f  al client versio
+0001d1a0: 6e20 6a75 7374 2067 6f74 2075 7064 6174  n just got updat
+0001d1b0: 6564 2c20 616e 640a 2020 2020 7468 6520  ed, and.    the 
+0001d1c0: 7265 6d6f 7465 2072 756e 7469 6d65 2069  remote runtime i
+0001d1d0: 7320 616e 206f 6c64 6572 2076 6572 7369  s an older versi
+0001d1e0: 6f6e 2e0a 2020 2020 2222 220a 2020 2020  on..    """.    
+0001d1f0: 7061 7474 6572 6e20 3d20 7265 2e63 6f6d  pattern = re.com
+0001d200: 7069 6c65 2872 2741 7474 7269 6275 7465  pile(r'Attribute
+0001d210: 4572 726f 723a 206d 6f64 756c 6520 5c27  Error: module \'
+0001d220: 736b 795c 2e28 2e2a 295c 2720 6861 7320  sky\.(.*)\' has 
+0001d230: 6e6f 2027 0a20 2020 2020 2020 2020 2020  no '.           
+0001d240: 2020 2020 2020 2020 2020 2020 2020 7227                r'
+0001d250: 6174 7472 6962 7574 6520 5c27 282e 2a29  attribute \'(.*)
+0001d260: 5c27 2729 0a20 2020 2069 6620 7265 7475  \'').    if retu
+0001d270: 726e 636f 6465 2021 3d20 303a 0a20 2020  rncode != 0:.   
+0001d280: 2020 2020 2061 7474 7269 6275 7465 5f65       attribute_e
+0001d290: 7272 6f72 203d 2072 652e 6669 6e64 616c  rror = re.findal
+0001d2a0: 6c28 7061 7474 6572 6e2c 2073 7464 6572  l(pattern, stder
+0001d2b0: 7229 0a20 2020 2020 2020 2069 6620 6174  r).        if at
+0001d2c0: 7472 6962 7574 655f 6572 726f 723a 0a20  tribute_error:. 
+0001d2d0: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+0001d2e0: 7578 5f75 7469 6c73 2e70 7269 6e74 5f65  ux_utils.print_e
+0001d2f0: 7863 6570 7469 6f6e 5f6e 6f5f 7472 6163  xception_no_trac
+0001d300: 6562 6163 6b28 293a 0a20 2020 2020 2020  eback():.       
+0001d310: 2020 2020 2020 2020 2072 6169 7365 2052           raise R
+0001d320: 756e 7469 6d65 4572 726f 7228 0a20 2020  untimeError(.   
+0001d330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d340: 2066 277b 636f 6c6f 7261 6d61 2e46 6f72   f'{colorama.For
+0001d350: 652e 5245 447d 536b 7950 696c 6f74 2072  e.RED}SkyPilot r
+0001d360: 756e 7469 6d65 206e 6565 6473 2074 6f20  untime needs to 
+0001d370: 6265 2075 7064 6174 6564 2027 0a20 2020  be updated '.   
+0001d380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d390: 2027 6f6e 2074 6865 2072 656d 6f74 6520   'on the remote 
+0001d3a0: 636c 7573 7465 722e 2054 6f20 7570 6461  cluster. To upda
+0001d3b0: 7465 2c20 7275 6e20 2865 7869 7374 696e  te, run (existin
+0001d3c0: 6720 6a6f 6273 2061 7265 2027 0a20 2020  g jobs are '.   
+0001d3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d3e0: 2066 276e 6f74 2069 6e74 6572 7275 7074   f'not interrupt
+0001d3f0: 6564 293a 207b 636f 6c6f 7261 6d61 2e53  ed): {colorama.S
+0001d400: 7479 6c65 2e42 5249 4748 547d 736b 7920  tyle.BRIGHT}sky 
+0001d410: 7374 6172 7420 2d66 202d 7920 270a 2020  start -f -y '.  
+0001d420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d430: 2020 6627 7b63 6c75 7374 6572 5f6e 616d    f'{cluster_nam
+0001d440: 657d 7b63 6f6c 6f72 616d 612e 5374 796c  e}{colorama.Styl
+0001d450: 652e 5245 5345 545f 414c 4c7d 270a 2020  e.RESET_ALL}'.  
+0001d460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d470: 2020 6627 5c6e 2d2d 2d20 4465 7461 696c    f'\n--- Detail
+0001d480: 7320 2d2d 2d5c 6e7b 7374 6465 7272 2e73  s ---\n{stderr.s
+0001d490: 7472 6970 2829 7d5c 6e27 290a 0a0a 6465  trip()}\n')...de
+0001d4a0: 6620 6765 745f 656e 6470 6f69 6e74 7328  f get_endpoints(
+0001d4b0: 636c 7573 7465 723a 2073 7472 2c0a 2020  cluster: str,.  
+0001d4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d4d0: 706f 7274 3a20 4f70 7469 6f6e 616c 5b55  port: Optional[U
+0001d4e0: 6e69 6f6e 5b69 6e74 2c20 7374 725d 5d20  nion[int, str]] 
+0001d4f0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0001d500: 2020 2020 2020 2020 2020 736b 6970 5f73            skip_s
+0001d510: 7461 7475 735f 6368 6563 6b3a 2062 6f6f  tatus_check: boo
+0001d520: 6c20 3d20 4661 6c73 6529 202d 3e20 4469  l = False) -> Di
+0001d530: 6374 5b69 6e74 2c20 7374 725d 3a0a 2020  ct[int, str]:.  
+0001d540: 2020 2222 2247 6574 7320 7468 6520 656e    """Gets the en
+0001d550: 6470 6f69 6e74 2066 6f72 2061 2067 6976  dpoint for a giv
+0001d560: 656e 2063 6c75 7374 6572 2061 6e64 2070  en cluster and p
+0001d570: 6f72 7420 6e75 6d62 6572 2028 656e 6470  ort number (endp
+0001d580: 6f69 6e74 292e 0a0a 2020 2020 4172 6773  oint)...    Args
+0001d590: 3a0a 2020 2020 2020 2020 636c 7573 7465  :.        cluste
+0001d5a0: 723a 2054 6865 206e 616d 6520 6f66 2074  r: The name of t
+0001d5b0: 6865 2063 6c75 7374 6572 2e0a 2020 2020  he cluster..    
+0001d5c0: 2020 2020 706f 7274 3a20 5468 6520 706f      port: The po
+0001d5d0: 7274 206e 756d 6265 7220 746f 2067 6574  rt number to get
+0001d5e0: 2074 6865 2065 6e64 706f 696e 7420 666f   the endpoint fo
+0001d5f0: 722e 2049 6620 4e6f 6e65 2c20 656e 6470  r. If None, endp
+0001d600: 6f69 6e74 730a 2020 2020 2020 2020 2020  oints.          
+0001d610: 2020 666f 7220 616c 6c20 706f 7274 7320    for all ports 
+0001d620: 6172 6520 7265 7475 726e 6564 2e0a 2020  are returned..  
+0001d630: 2020 2020 2020 736b 6970 5f73 7461 7475        skip_statu
+0001d640: 735f 6368 6563 6b3a 2057 6865 7468 6572  s_check: Whether
+0001d650: 2074 6f20 736b 6970 2074 6865 2073 7461   to skip the sta
+0001d660: 7475 7320 6368 6563 6b20 666f 7220 7468  tus check for th
+0001d670: 6520 636c 7573 7465 722e 0a20 2020 2020  e cluster..     
+0001d680: 2020 2020 2020 2054 6869 7320 6973 2075         This is u
+0001d690: 7365 6675 6c20 7768 656e 2074 6865 2063  seful when the c
+0001d6a0: 6c75 7374 6572 2069 7320 6b6e 6f77 6e20  luster is known 
+0001d6b0: 746f 2062 6520 696e 2061 2049 4e49 5420  to be in a INIT 
+0001d6c0: 7374 6174 650a 2020 2020 2020 2020 2020  state.          
+0001d6d0: 2020 616e 6420 7468 6520 6361 6c6c 6572    and the caller
+0001d6e0: 2077 616e 7473 2074 6f20 7175 6572 7920   wants to query 
+0001d6f0: 7468 6520 656e 6470 6f69 6e74 732e 2055  the endpoints. U
+0001d700: 7365 6420 6279 2073 6572 7665 0a20 2020  sed by serve.   
+0001d710: 2020 2020 2020 2020 2063 6f6e 7472 6f6c           control
+0001d720: 6c65 7220 746f 2071 7565 7279 2065 6e64  ler to query end
+0001d730: 706f 696e 7473 2064 7572 696e 6720 636c  points during cl
+0001d740: 7573 7465 7220 6c61 756e 6368 2077 6865  uster launch whe
+0001d750: 6e20 6d75 6c74 6970 6c65 0a20 2020 2020  n multiple.     
+0001d760: 2020 2020 2020 2073 6572 7669 6365 7320         services 
+0001d770: 6d61 7920 6265 2067 6574 7469 6e67 206c  may be getting l
+0001d780: 6175 6e63 6865 6420 696e 2070 6172 616c  aunched in paral
+0001d790: 6c65 6c20 2861 6e64 2061 7320 6120 7265  lel (and as a re
+0001d7a0: 7375 6c74 2c0a 2020 2020 2020 2020 2020  sult,.          
+0001d7b0: 2020 7468 6520 636f 6e74 726f 6c6c 6572    the controller
+0001d7c0: 206d 6179 2062 6520 696e 2049 4e49 5420   may be in INIT 
+0001d7d0: 7374 6174 7573 2064 7565 2074 6f20 6120  status due to a 
+0001d7e0: 636f 6e63 7572 7265 6e74 206c 6175 6e63  concurrent launc
+0001d7f0: 6829 2e0a 0a20 2020 2052 6574 7572 6e73  h)...    Returns
+0001d800: 3a20 4120 6469 6374 696f 6e61 7279 206f  : A dictionary o
+0001d810: 6620 706f 7274 206e 756d 6265 7273 2074  f port numbers t
+0001d820: 6f20 656e 6470 6f69 6e74 732e 2049 6620  o endpoints. If 
+0001d830: 656e 6470 6f69 6e74 2069 7320 4e6f 6e65  endpoint is None
+0001d840: 2c0a 2020 2020 2020 2020 7468 6520 6469  ,.        the di
+0001d850: 6374 696f 6e61 7279 2077 696c 6c20 636f  ctionary will co
+0001d860: 6e74 6169 6e20 616c 6c20 706f 7274 733a  ntain all ports:
+0001d870: 656e 6470 6f69 6e74 7320 6578 706f 7365  endpoints expose
+0001d880: 6420 6f6e 2074 6865 2063 6c75 7374 6572  d on the cluster
+0001d890: 2e0a 2020 2020 2020 2020 4966 2074 6865  ..        If the
+0001d8a0: 2065 6e64 706f 696e 7420 6973 206e 6f74   endpoint is not
+0001d8b0: 2065 7870 6f73 6564 2079 6574 2028 652e   exposed yet (e.
+0001d8c0: 672e 2c20 6475 7269 6e67 2063 6c75 7374  g., during clust
+0001d8d0: 6572 206c 6175 6e63 6820 6f72 0a20 2020  er launch or.   
+0001d8e0: 2020 2020 2077 6169 7469 6e67 2066 6f72       waiting for
+0001d8f0: 2063 6c6f 7564 2070 726f 7669 6465 7220   cloud provider 
+0001d900: 746f 2065 7870 6f73 6520 7468 6520 656e  to expose the en
+0001d910: 6470 6f69 6e74 292c 2061 6e20 656d 7074  dpoint), an empt
+0001d920: 7920 6469 6374 696f 6e61 7279 0a20 2020  y dictionary.   
+0001d930: 2020 2020 2069 7320 7265 7475 726e 6564       is returned
+0001d940: 2e0a 0a20 2020 2052 6169 7365 733a 0a20  ...    Raises:. 
+0001d950: 2020 2020 2020 2056 616c 7565 4572 726f         ValueErro
+0001d960: 723a 2069 6620 7468 6520 706f 7274 2069  r: if the port i
+0001d970: 7320 696e 7661 6c69 6420 6f72 2074 6865  s invalid or the
+0001d980: 2063 6c6f 7564 2070 726f 7669 6465 7220   cloud provider 
+0001d990: 646f 6573 206e 6f74 0a20 2020 2020 2020  does not.       
+0001d9a0: 2020 2020 2073 7570 706f 7274 2071 7565       support que
+0001d9b0: 7279 696e 6720 656e 6470 6f69 6e74 732e  rying endpoints.
+0001d9c0: 0a20 2020 2020 2020 2065 7863 6570 7469  .        excepti
+0001d9d0: 6f6e 732e 436c 7573 7465 724e 6f74 5570  ons.ClusterNotUp
+0001d9e0: 4572 726f 723a 2069 6620 7468 6520 636c  Error: if the cl
+0001d9f0: 7573 7465 7220 6973 206e 6f74 2069 6e20  uster is not in 
+0001da00: 5550 2073 7461 7475 732e 0a20 2020 2022  UP status..    "
+0001da10: 2222 0a20 2020 2023 2043 6173 7420 656e  "".    # Cast en
+0001da20: 6470 6f69 6e74 2074 6f20 696e 7420 6966  dpoint to int if
+0001da30: 2069 7420 6973 206e 6f74 204e 6f6e 650a   it is not None.
+0001da40: 2020 2020 6966 2070 6f72 7420 6973 206e      if port is n
+0001da50: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0001da60: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+0001da70: 2020 706f 7274 203d 2069 6e74 2870 6f72    port = int(por
+0001da80: 7429 0a20 2020 2020 2020 2065 7863 6570  t).        excep
+0001da90: 7420 5661 6c75 6545 7272 6f72 3a0a 2020  t ValueError:.  
+0001daa0: 2020 2020 2020 2020 2020 7769 7468 2075            with u
+0001dab0: 785f 7574 696c 732e 7072 696e 745f 6578  x_utils.print_ex
+0001dac0: 6365 7074 696f 6e5f 6e6f 5f74 7261 6365  ception_no_trace
+0001dad0: 6261 636b 2829 3a0a 2020 2020 2020 2020  back():.        
+0001dae0: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+0001daf0: 6c75 6545 7272 6f72 2866 2749 6e76 616c  lueError(f'Inval
+0001db00: 6964 2065 6e64 706f 696e 7420 7b70 6f72  id endpoint {por
+0001db10: 7421 727d 2e27 2920 6672 6f6d 204e 6f6e  t!r}.') from Non
+0001db20: 650a 2020 2020 636c 7573 7465 725f 7265  e.    cluster_re
+0001db30: 636f 7264 7320 3d20 6765 745f 636c 7573  cords = get_clus
+0001db40: 7465 7273 2869 6e63 6c75 6465 5f63 6f6e  ters(include_con
+0001db50: 7472 6f6c 6c65 723d 5472 7565 2c0a 2020  troller=True,.  
+0001db60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001db70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001db80: 2072 6566 7265 7368 3d46 616c 7365 2c0a   refresh=False,.
+0001db90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dbb0: 2020 2063 6c75 7374 6572 5f6e 616d 6573     cluster_names
+0001dbc0: 3d5b 636c 7573 7465 725d 290a 2020 2020  =[cluster]).    
+0001dbd0: 636c 7573 7465 725f 7265 636f 7264 203d  cluster_record =
+0001dbe0: 2063 6c75 7374 6572 5f72 6563 6f72 6473   cluster_records
+0001dbf0: 5b30 5d0a 2020 2020 6966 2028 6e6f 7420  [0].    if (not 
+0001dc00: 736b 6970 5f73 7461 7475 735f 6368 6563  skip_status_chec
+0001dc10: 6b20 616e 640a 2020 2020 2020 2020 2020  k and.          
+0001dc20: 2020 636c 7573 7465 725f 7265 636f 7264    cluster_record
+0001dc30: 5b27 7374 6174 7573 275d 2021 3d20 7374  ['status'] != st
+0001dc40: 6174 7573 5f6c 6962 2e43 6c75 7374 6572  atus_lib.Cluster
+0001dc50: 5374 6174 7573 2e55 5029 3a0a 2020 2020  Status.UP):.    
+0001dc60: 2020 2020 7769 7468 2075 785f 7574 696c      with ux_util
+0001dc70: 732e 7072 696e 745f 6578 6365 7074 696f  s.print_exceptio
+0001dc80: 6e5f 6e6f 5f74 7261 6365 6261 636b 2829  n_no_traceback()
+0001dc90: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+0001dca0: 6973 6520 6578 6365 7074 696f 6e73 2e43  ise exceptions.C
+0001dcb0: 6c75 7374 6572 4e6f 7455 7045 7272 6f72  lusterNotUpError
+0001dcc0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0001dcd0: 2020 6627 436c 7573 7465 7220 7b63 6c75    f'Cluster {clu
+0001dce0: 7374 6572 5f72 6563 6f72 645b 226e 616d  ster_record["nam
+0001dcf0: 6522 5d21 727d 2027 0a20 2020 2020 2020  e"]!r} '.       
+0001dd00: 2020 2020 2020 2020 2027 6973 206e 6f74           'is not
+0001dd10: 2069 6e20 5550 2073 7461 7475 732e 272c   in UP status.',
+0001dd20: 2063 6c75 7374 6572 5f72 6563 6f72 645b   cluster_record[
+0001dd30: 2773 7461 7475 7327 5d29 0a20 2020 2068  'status']).    h
+0001dd40: 616e 646c 6520 3d20 636c 7573 7465 725f  andle = cluster_
+0001dd50: 7265 636f 7264 5b27 6861 6e64 6c65 275d  record['handle']
+0001dd60: 0a20 2020 2069 6620 6e6f 7420 6973 696e  .    if not isin
+0001dd70: 7374 616e 6365 2868 616e 646c 652c 2062  stance(handle, b
+0001dd80: 6163 6b65 6e64 732e 436c 6f75 6456 6d52  ackends.CloudVmR
+0001dd90: 6179 5265 736f 7572 6365 4861 6e64 6c65  ayResourceHandle
+0001dda0: 293a 0a20 2020 2020 2020 2077 6974 6820  ):.        with 
+0001ddb0: 7578 5f75 7469 6c73 2e70 7269 6e74 5f65  ux_utils.print_e
+0001ddc0: 7863 6570 7469 6f6e 5f6e 6f5f 7472 6163  xception_no_trac
+0001ddd0: 6562 6163 6b28 293a 0a20 2020 2020 2020  eback():.       
+0001dde0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+0001ddf0: 4572 726f 7228 2751 7565 7279 696e 6720  Error('Querying 
+0001de00: 4950 2061 6464 7265 7373 2069 7320 6e6f  IP address is no
+0001de10: 7420 7375 7070 6f72 7465 6420 270a 2020  t supported '.  
+0001de20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001de30: 2020 2020 2020 2020 2020 2066 2766 6f72             f'for
+0001de40: 2063 6c75 7374 6572 207b 636c 7573 7465   cluster {cluste
+0001de50: 7221 727d 2077 6974 6820 6261 636b 656e  r!r} with backen
+0001de60: 6420 270a 2020 2020 2020 2020 2020 2020  d '.            
+0001de70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001de80: 2066 277b 6765 745f 6261 636b 656e 645f   f'{get_backend_
+0001de90: 6672 6f6d 5f68 616e 646c 6528 6861 6e64  from_handle(hand
+0001dea0: 6c65 292e 4e41 4d45 7d2e 2729 0a0a 2020  le).NAME}.')..  
+0001deb0: 2020 6c61 756e 6368 6564 5f72 6573 6f75    launched_resou
+0001dec0: 7263 6573 203d 2068 616e 646c 652e 6c61  rces = handle.la
+0001ded0: 756e 6368 6564 5f72 6573 6f75 7263 6573  unched_resources
+0001dee0: 0a20 2020 2063 6c6f 7564 203d 206c 6175  .    cloud = lau
+0001def0: 6e63 6865 645f 7265 736f 7572 6365 732e  nched_resources.
+0001df00: 636c 6f75 640a 2020 2020 7472 793a 0a20  cloud.    try:. 
+0001df10: 2020 2020 2020 2063 6c6f 7564 2e63 6865         cloud.che
+0001df20: 636b 5f66 6561 7475 7265 735f 6172 655f  ck_features_are_
+0001df30: 7375 7070 6f72 7465 6428 0a20 2020 2020  supported(.     
+0001df40: 2020 2020 2020 206c 6175 6e63 6865 645f         launched_
+0001df50: 7265 736f 7572 6365 732c 207b 636c 6f75  resources, {clou
+0001df60: 6473 2e43 6c6f 7564 496d 706c 656d 656e  ds.CloudImplemen
+0001df70: 7461 7469 6f6e 4665 6174 7572 6573 2e4f  tationFeatures.O
+0001df80: 5045 4e5f 504f 5254 537d 290a 2020 2020  PEN_PORTS}).    
+0001df90: 6578 6365 7074 2065 7863 6570 7469 6f6e  except exception
+0001dfa0: 732e 4e6f 7453 7570 706f 7274 6564 4572  s.NotSupportedEr
+0001dfb0: 726f 723a 0a20 2020 2020 2020 2077 6974  ror:.        wit
+0001dfc0: 6820 7578 5f75 7469 6c73 2e70 7269 6e74  h ux_utils.print
+0001dfd0: 5f65 7863 6570 7469 6f6e 5f6e 6f5f 7472  _exception_no_tr
+0001dfe0: 6163 6562 6163 6b28 293a 0a20 2020 2020  aceback():.     
+0001dff0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+0001e000: 7565 4572 726f 7228 2751 7565 7279 696e  ueError('Queryin
+0001e010: 6720 656e 6470 6f69 6e74 7320 6973 206e  g endpoints is n
+0001e020: 6f74 2073 7570 706f 7274 6564 2027 0a20  ot supported '. 
+0001e030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e040: 2020 2020 2020 2020 2020 2020 6627 666f              f'fo
+0001e050: 7220 636c 7573 7465 7220 7b63 6c75 7374  r cluster {clust
+0001e060: 6572 2172 7d20 6f6e 207b 636c 6f75 647d  er!r} on {cloud}
+0001e070: 2e27 2920 6672 6f6d 204e 6f6e 650a 0a20  .') from None.. 
+0001e080: 2020 2063 6f6e 6669 6720 3d20 636f 6d6d     config = comm
+0001e090: 6f6e 5f75 7469 6c73 2e72 6561 645f 7961  on_utils.read_ya
+0001e0a0: 6d6c 2868 616e 646c 652e 636c 7573 7465  ml(handle.cluste
+0001e0b0: 725f 7961 6d6c 290a 2020 2020 706f 7274  r_yaml).    port
+0001e0c0: 5f64 6574 6169 6c73 203d 2070 726f 7669  _details = provi
+0001e0d0: 7369 6f6e 5f6c 6962 2e71 7565 7279 5f70  sion_lib.query_p
+0001e0e0: 6f72 7473 2872 6570 7228 636c 6f75 6429  orts(repr(cloud)
+0001e0f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001e100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e110: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+0001e120: 616e 646c 652e 636c 7573 7465 725f 6e61  andle.cluster_na
+0001e130: 6d65 5f6f 6e5f 636c 6f75 642c 0a20 2020  me_on_cloud,.   
 0001e140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e150: 2020 6861 6e64 6c65 2e6c 6175 6e63 6865    handle.launche
-0001e160: 645f 7265 736f 7572 6365 732e 706f 7274  d_resources.port
-0001e170: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-0001e180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e160: 2020 2020 2020 2020 2020 6861 6e64 6c65            handle
+0001e170: 2e6c 6175 6e63 6865 645f 7265 736f 7572  .launched_resour
+0001e180: 6365 732e 706f 7274 732c 0a20 2020 2020  ces.ports,.     
 0001e190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e1a0: 6865 6164 5f69 703d 6861 6e64 6c65 2e68  head_ip=handle.h
-0001e1b0: 6561 645f 6970 2c0a 2020 2020 2020 2020  ead_ip,.        
-0001e1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e1b0: 2020 2020 2020 2020 6865 6164 5f69 703d          head_ip=
+0001e1c0: 6861 6e64 6c65 2e68 6561 645f 6970 2c0a  handle.head_ip,.
 0001e1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e1e0: 2020 2020 2070 726f 7669 6465 725f 636f       provider_co
-0001e1f0: 6e66 6967 3d63 6f6e 6669 675b 2770 726f  nfig=config['pro
-0001e200: 7669 6465 7227 5d29 0a0a 2020 2020 2320  vider'])..    # 
-0001e210: 5661 6c69 6461 7469 6f6e 2062 6566 6f72  Validation befor
-0001e220: 6520 7265 7475 726e 696e 6720 7468 6520  e returning the 
-0001e230: 656e 6470 6f69 6e74 730a 2020 2020 6966  endpoints.    if
-0001e240: 2070 6f72 7420 6973 206e 6f74 204e 6f6e   port is not Non
-0001e250: 653a 0a20 2020 2020 2020 2023 2049 6620  e:.        # If 
-0001e260: 7468 6520 7265 7175 6573 7465 6420 656e  the requested en
-0001e270: 6470 6f69 6e74 2077 6173 206e 6f74 2074  dpoint was not t
-0001e280: 6f20 6265 2065 7870 6f73 6564 0a20 2020  o be exposed.   
-0001e290: 2020 2020 2070 6f72 745f 7365 7420 3d20       port_set = 
-0001e2a0: 7265 736f 7572 6365 735f 7574 696c 732e  resources_utils.
-0001e2b0: 706f 7274 5f72 616e 6765 735f 746f 5f73  port_ranges_to_s
-0001e2c0: 6574 280a 2020 2020 2020 2020 2020 2020  et(.            
-0001e2d0: 6861 6e64 6c65 2e6c 6175 6e63 6865 645f  handle.launched_
-0001e2e0: 7265 736f 7572 6365 732e 706f 7274 7329  resources.ports)
-0001e2f0: 0a20 2020 2020 2020 2069 6620 706f 7274  .        if port
-0001e300: 206e 6f74 2069 6e20 706f 7274 5f73 6574   not in port_set
-0001e310: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
-0001e320: 6767 6572 2e77 6172 6e69 6e67 2866 2750  gger.warning(f'P
-0001e330: 6f72 7420 7b70 6f72 747d 2069 7320 6e6f  ort {port} is no
-0001e340: 7420 6578 706f 7365 6420 6f6e 2027 0a20  t exposed on '. 
-0001e350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e360: 2020 2020 2020 2020 2020 6627 636c 7573            f'clus
-0001e370: 7465 7220 7b63 6c75 7374 6572 2172 7d2e  ter {cluster!r}.
-0001e380: 2729 0a20 2020 2020 2020 2020 2020 2072  ').            r
-0001e390: 6574 7572 6e20 7b7d 0a20 2020 2020 2020  eturn {}.       
-0001e3a0: 2023 2049 6620 7468 6520 7573 6572 2072   # If the user r
-0001e3b0: 6571 7565 7374 6564 2061 2073 7065 6369  equested a speci
-0001e3c0: 6669 6320 706f 7274 2065 6e64 706f 696e  fic port endpoin
-0001e3d0: 742c 2063 6865 636b 2069 6620 6974 2069  t, check if it i
-0001e3e0: 7320 6578 706f 7365 640a 2020 2020 2020  s exposed.      
-0001e3f0: 2020 6966 2070 6f72 7420 6e6f 7420 696e    if port not in
-0001e400: 2070 6f72 745f 6465 7461 696c 733a 0a20   port_details:. 
-0001e410: 2020 2020 2020 2020 2020 2065 7272 6f72             error
-0001e420: 5f6d 7367 203d 2028 6627 506f 7274 207b  _msg = (f'Port {
-0001e430: 706f 7274 7d20 6e6f 7420 6578 706f 7365  port} not expose
-0001e440: 6420 7965 742e 2027 0a20 2020 2020 2020  d yet. '.       
-0001e450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e460: 2020 6627 7b5f 454e 4450 4f49 4e54 535f    f'{_ENDPOINTS_
-0001e470: 5245 5452 595f 4d45 5353 4147 457d 2027  RETRY_MESSAGE} '
-0001e480: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-0001e490: 2068 616e 646c 652e 6c61 756e 6368 6564   handle.launched
-0001e4a0: 5f72 6573 6f75 7263 6573 2e63 6c6f 7564  _resources.cloud
-0001e4b0: 2e69 735f 7361 6d65 5f63 6c6f 7564 280a  .is_same_cloud(.
-0001e4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e4d0: 2020 2020 636c 6f75 6473 2e4b 7562 6572      clouds.Kuber
-0001e4e0: 6e65 7465 7328 2929 3a0a 2020 2020 2020  netes()):.      
-0001e4f0: 2020 2020 2020 2020 2020 2320 4164 6420            # Add 
-0001e500: 4b75 6265 726e 6574 6573 2073 7065 6369  Kubernetes speci
-0001e510: 6669 6320 6465 6275 6767 696e 6720 696e  fic debugging in
-0001e520: 666f 0a20 2020 2020 2020 2020 2020 2020  fo.             
-0001e530: 2020 2065 7272 6f72 5f6d 7367 202b 3d20     error_msg += 
-0001e540: 286b 7562 6572 6e65 7465 735f 7574 696c  (kubernetes_util
-0001e550: 732e 6765 745f 656e 6470 6f69 6e74 5f64  s.get_endpoint_d
-0001e560: 6562 7567 5f6d 6573 7361 6765 2829 290a  ebug_message()).
-0001e570: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-0001e580: 6572 2e77 6172 6e69 6e67 2865 7272 6f72  er.warning(error
-0001e590: 5f6d 7367 290a 2020 2020 2020 2020 2020  _msg).          
-0001e5a0: 2020 7265 7475 726e 207b 7d0a 2020 2020    return {}.    
-0001e5b0: 2020 2020 7265 7475 726e 207b 706f 7274      return {port
-0001e5c0: 3a20 706f 7274 5f64 6574 6169 6c73 5b70  : port_details[p
-0001e5d0: 6f72 745d 5b30 5d2e 7572 6c28 297d 0a20  ort][0].url()}. 
-0001e5e0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0001e5f0: 2069 6620 6e6f 7420 706f 7274 5f64 6574   if not port_det
-0001e600: 6169 6c73 3a0a 2020 2020 2020 2020 2020  ails:.          
-0001e610: 2020 2320 4966 2063 6c75 7374 6572 2068    # If cluster h
-0001e620: 6164 206e 6f20 706f 7274 7320 746f 2062  ad no ports to b
-0001e630: 6520 6578 706f 7365 640a 2020 2020 2020  e exposed.      
-0001e640: 2020 2020 2020 6966 2068 616e 646c 652e        if handle.
-0001e650: 6c61 756e 6368 6564 5f72 6573 6f75 7263  launched_resourc
-0001e660: 6573 2e70 6f72 7473 2069 7320 4e6f 6e65  es.ports is None
-0001e670: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001e680: 2020 6c6f 6767 6572 2e77 6172 6e69 6e67    logger.warning
-0001e690: 2866 2743 6c75 7374 6572 207b 636c 7573  (f'Cluster {clus
-0001e6a0: 7465 7221 727d 2064 6f65 7320 6e6f 7420  ter!r} does not 
-0001e6b0: 6861 7665 2061 6e79 2027 0a20 2020 2020  have any '.     
-0001e6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e6d0: 2020 2020 2020 2020 2020 2770 6f72 7473            'ports
-0001e6e0: 2074 6f20 6265 2065 7870 6f73 6564 2e27   to be exposed.'
-0001e6f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001e700: 2020 7265 7475 726e 207b 7d0a 2020 2020    return {}.    
-0001e710: 2020 2020 2020 2020 2320 456c 7365 2070          # Else p
-0001e720: 6f72 7473 2068 6176 6520 6e6f 7420 6265  orts have not be
-0001e730: 656e 2065 7870 6f73 6564 2065 7665 6e20  en exposed even 
-0001e740: 7468 6f75 6768 2074 6865 7920 6578 6973  though they exis
-0001e750: 742e 0a20 2020 2020 2020 2020 2020 2023  t..            #
-0001e760: 2049 6e20 7468 6973 2063 6173 652c 2061   In this case, a
-0001e770: 736b 2074 6865 2075 7365 7220 746f 2072  sk the user to r
-0001e780: 6574 7279 2e0a 2020 2020 2020 2020 2020  etry..          
-0001e790: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0001e7a0: 2020 2020 2020 2020 6572 726f 725f 6d73          error_ms
-0001e7b0: 6720 3d20 2866 274e 6f20 656e 6470 6f69  g = (f'No endpoi
-0001e7c0: 6e74 7320 6578 706f 7365 6420 7965 742e  nts exposed yet.
-0001e7d0: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
-0001e7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e7f0: 6627 7b5f 454e 4450 4f49 4e54 535f 5245  f'{_ENDPOINTS_RE
-0001e800: 5452 595f 4d45 5353 4147 457d 2027 290a  TRY_MESSAGE} ').
-0001e810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e820: 6966 2068 616e 646c 652e 6c61 756e 6368  if handle.launch
-0001e830: 6564 5f72 6573 6f75 7263 6573 2e63 6c6f  ed_resources.clo
-0001e840: 7564 2e69 735f 7361 6d65 5f63 6c6f 7564  ud.is_same_cloud
-0001e850: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0001e860: 2020 2020 2020 2020 2020 636c 6f75 6473            clouds
-0001e870: 2e4b 7562 6572 6e65 7465 7328 2929 3a0a  .Kubernetes()):.
-0001e880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e890: 2020 2020 2320 4164 6420 4b75 6265 726e      # Add Kubern
-0001e8a0: 6574 6573 2073 7065 6369 6669 6320 6465  etes specific de
-0001e8b0: 6275 6767 696e 6720 696e 666f 0a20 2020  bugging info.   
-0001e8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e8d0: 2065 7272 6f72 5f6d 7367 202b 3d20 5c0a   error_msg += \.
-0001e8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e8f0: 2020 2020 2020 2020 6b75 6265 726e 6574          kubernet
-0001e900: 6573 5f75 7469 6c73 2e67 6574 5f65 6e64  es_utils.get_end
-0001e910: 706f 696e 745f 6465 6275 675f 6d65 7373  point_debug_mess
-0001e920: 6167 6528 290a 2020 2020 2020 2020 2020  age().          
-0001e930: 2020 2020 2020 6c6f 6767 6572 2e77 6172        logger.war
-0001e940: 6e69 6e67 2865 7272 6f72 5f6d 7367 290a  ning(error_msg).
-0001e950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e960: 7265 7475 726e 207b 7d0a 2020 2020 2020  return {}.      
-0001e970: 2020 7265 7475 726e 207b 0a20 2020 2020    return {.     
-0001e980: 2020 2020 2020 2070 6f72 745f 6e75 6d3a         port_num:
-0001e990: 2075 726c 735b 305d 2e75 726c 2829 2066   urls[0].url() f
-0001e9a0: 6f72 2070 6f72 745f 6e75 6d2c 2075 726c  or port_num, url
-0001e9b0: 7320 696e 2070 6f72 745f 6465 7461 696c  s in port_detail
-0001e9c0: 732e 6974 656d 7328 290a 2020 2020 2020  s.items().      
-0001e9d0: 2020 7d0a                                  }.
+0001e1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e1f0: 2020 2020 2020 2020 2020 2020 2070 726f               pro
+0001e200: 7669 6465 725f 636f 6e66 6967 3d63 6f6e  vider_config=con
+0001e210: 6669 675b 2770 726f 7669 6465 7227 5d29  fig['provider'])
+0001e220: 0a0a 2020 2020 2320 5661 6c69 6461 7469  ..    # Validati
+0001e230: 6f6e 2062 6566 6f72 6520 7265 7475 726e  on before return
+0001e240: 696e 6720 7468 6520 656e 6470 6f69 6e74  ing the endpoint
+0001e250: 730a 2020 2020 6966 2070 6f72 7420 6973  s.    if port is
+0001e260: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0001e270: 2020 2023 2049 6620 7468 6520 7265 7175     # If the requ
+0001e280: 6573 7465 6420 656e 6470 6f69 6e74 2077  ested endpoint w
+0001e290: 6173 206e 6f74 2074 6f20 6265 2065 7870  as not to be exp
+0001e2a0: 6f73 6564 0a20 2020 2020 2020 2070 6f72  osed.        por
+0001e2b0: 745f 7365 7420 3d20 7265 736f 7572 6365  t_set = resource
+0001e2c0: 735f 7574 696c 732e 706f 7274 5f72 616e  s_utils.port_ran
+0001e2d0: 6765 735f 746f 5f73 6574 280a 2020 2020  ges_to_set(.    
+0001e2e0: 2020 2020 2020 2020 6861 6e64 6c65 2e6c          handle.l
+0001e2f0: 6175 6e63 6865 645f 7265 736f 7572 6365  aunched_resource
+0001e300: 732e 706f 7274 7329 0a20 2020 2020 2020  s.ports).       
+0001e310: 2069 6620 706f 7274 206e 6f74 2069 6e20   if port not in 
+0001e320: 706f 7274 5f73 6574 3a0a 2020 2020 2020  port_set:.      
+0001e330: 2020 2020 2020 6c6f 6767 6572 2e77 6172        logger.war
+0001e340: 6e69 6e67 2866 2750 6f72 7420 7b70 6f72  ning(f'Port {por
+0001e350: 747d 2069 7320 6e6f 7420 6578 706f 7365  t} is not expose
+0001e360: 6420 6f6e 2027 0a20 2020 2020 2020 2020  d on '.         
+0001e370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e380: 2020 6627 636c 7573 7465 7220 7b63 6c75    f'cluster {clu
+0001e390: 7374 6572 2172 7d2e 2729 0a20 2020 2020  ster!r}.').     
+0001e3a0: 2020 2020 2020 2072 6574 7572 6e20 7b7d         return {}
+0001e3b0: 0a20 2020 2020 2020 2023 2049 6620 7468  .        # If th
+0001e3c0: 6520 7573 6572 2072 6571 7565 7374 6564  e user requested
+0001e3d0: 2061 2073 7065 6369 6669 6320 706f 7274   a specific port
+0001e3e0: 2065 6e64 706f 696e 742c 2063 6865 636b   endpoint, check
+0001e3f0: 2069 6620 6974 2069 7320 6578 706f 7365   if it is expose
+0001e400: 640a 2020 2020 2020 2020 6966 2070 6f72  d.        if por
+0001e410: 7420 6e6f 7420 696e 2070 6f72 745f 6465  t not in port_de
+0001e420: 7461 696c 733a 0a20 2020 2020 2020 2020  tails:.         
+0001e430: 2020 2065 7272 6f72 5f6d 7367 203d 2028     error_msg = (
+0001e440: 6627 506f 7274 207b 706f 7274 7d20 6e6f  f'Port {port} no
+0001e450: 7420 6578 706f 7365 6420 7965 742e 2027  t exposed yet. '
+0001e460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e470: 2020 2020 2020 2020 2020 6627 7b5f 454e            f'{_EN
+0001e480: 4450 4f49 4e54 535f 5245 5452 595f 4d45  DPOINTS_RETRY_ME
+0001e490: 5353 4147 457d 2027 290a 2020 2020 2020  SSAGE} ').      
+0001e4a0: 2020 2020 2020 6966 2068 616e 646c 652e        if handle.
+0001e4b0: 6c61 756e 6368 6564 5f72 6573 6f75 7263  launched_resourc
+0001e4c0: 6573 2e63 6c6f 7564 2e69 735f 7361 6d65  es.cloud.is_same
+0001e4d0: 5f63 6c6f 7564 280a 2020 2020 2020 2020  _cloud(.        
+0001e4e0: 2020 2020 2020 2020 2020 2020 636c 6f75              clou
+0001e4f0: 6473 2e4b 7562 6572 6e65 7465 7328 2929  ds.Kubernetes())
+0001e500: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001e510: 2020 2320 4164 6420 4b75 6265 726e 6574    # Add Kubernet
+0001e520: 6573 2073 7065 6369 6669 6320 6465 6275  es specific debu
+0001e530: 6767 696e 6720 696e 666f 0a20 2020 2020  gging info.     
+0001e540: 2020 2020 2020 2020 2020 2065 7272 6f72             error
+0001e550: 5f6d 7367 202b 3d20 286b 7562 6572 6e65  _msg += (kuberne
+0001e560: 7465 735f 7574 696c 732e 6765 745f 656e  tes_utils.get_en
+0001e570: 6470 6f69 6e74 5f64 6562 7567 5f6d 6573  dpoint_debug_mes
+0001e580: 7361 6765 2829 290a 2020 2020 2020 2020  sage()).        
+0001e590: 2020 2020 6c6f 6767 6572 2e77 6172 6e69      logger.warni
+0001e5a0: 6e67 2865 7272 6f72 5f6d 7367 290a 2020  ng(error_msg).  
+0001e5b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0001e5c0: 207b 7d0a 2020 2020 2020 2020 7265 7475   {}.        retu
+0001e5d0: 726e 207b 706f 7274 3a20 706f 7274 5f64  rn {port: port_d
+0001e5e0: 6574 6169 6c73 5b70 6f72 745d 5b30 5d2e  etails[port][0].
+0001e5f0: 7572 6c28 297d 0a20 2020 2065 6c73 653a  url()}.    else:
+0001e600: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+0001e610: 706f 7274 5f64 6574 6169 6c73 3a0a 2020  port_details:.  
+0001e620: 2020 2020 2020 2020 2020 2320 4966 2063            # If c
+0001e630: 6c75 7374 6572 2068 6164 206e 6f20 706f  luster had no po
+0001e640: 7274 7320 746f 2062 6520 6578 706f 7365  rts to be expose
+0001e650: 640a 2020 2020 2020 2020 2020 2020 6966  d.            if
+0001e660: 2068 616e 646c 652e 6c61 756e 6368 6564   handle.launched
+0001e670: 5f72 6573 6f75 7263 6573 2e70 6f72 7473  _resources.ports
+0001e680: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+0001e690: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+0001e6a0: 2e77 6172 6e69 6e67 2866 2743 6c75 7374  .warning(f'Clust
+0001e6b0: 6572 207b 636c 7573 7465 7221 727d 2064  er {cluster!r} d
+0001e6c0: 6f65 7320 6e6f 7420 6861 7665 2061 6e79  oes not have any
+0001e6d0: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
+0001e6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e6f0: 2020 2770 6f72 7473 2074 6f20 6265 2065    'ports to be e
+0001e700: 7870 6f73 6564 2e27 290a 2020 2020 2020  xposed.').      
+0001e710: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0001e720: 207b 7d0a 2020 2020 2020 2020 2020 2020   {}.            
+0001e730: 2320 456c 7365 2070 6f72 7473 2068 6176  # Else ports hav
+0001e740: 6520 6e6f 7420 6265 656e 2065 7870 6f73  e not been expos
+0001e750: 6564 2065 7665 6e20 7468 6f75 6768 2074  ed even though t
+0001e760: 6865 7920 6578 6973 742e 0a20 2020 2020  hey exist..     
+0001e770: 2020 2020 2020 2023 2049 6e20 7468 6973         # In this
+0001e780: 2063 6173 652c 2061 736b 2074 6865 2075   case, ask the u
+0001e790: 7365 7220 746f 2072 6574 7279 2e0a 2020  ser to retry..  
+0001e7a0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+0001e7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e7c0: 6572 726f 725f 6d73 6720 3d20 2866 274e  error_msg = (f'N
+0001e7d0: 6f20 656e 6470 6f69 6e74 7320 6578 706f  o endpoints expo
+0001e7e0: 7365 6420 7965 742e 2027 0a20 2020 2020  sed yet. '.     
+0001e7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e800: 2020 2020 2020 2020 6627 7b5f 454e 4450          f'{_ENDP
+0001e810: 4f49 4e54 535f 5245 5452 595f 4d45 5353  OINTS_RETRY_MESS
+0001e820: 4147 457d 2027 290a 2020 2020 2020 2020  AGE} ').        
+0001e830: 2020 2020 2020 2020 6966 2068 616e 646c          if handl
+0001e840: 652e 6c61 756e 6368 6564 5f72 6573 6f75  e.launched_resou
+0001e850: 7263 6573 2e63 6c6f 7564 2e69 735f 7361  rces.cloud.is_sa
+0001e860: 6d65 5f63 6c6f 7564 280a 2020 2020 2020  me_cloud(.      
+0001e870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e880: 2020 636c 6f75 6473 2e4b 7562 6572 6e65    clouds.Kuberne
+0001e890: 7465 7328 2929 3a0a 2020 2020 2020 2020  tes()):.        
+0001e8a0: 2020 2020 2020 2020 2020 2020 2320 4164              # Ad
+0001e8b0: 6420 4b75 6265 726e 6574 6573 2073 7065  d Kubernetes spe
+0001e8c0: 6369 6669 6320 6465 6275 6767 696e 6720  cific debugging 
+0001e8d0: 696e 666f 0a20 2020 2020 2020 2020 2020  info.           
+0001e8e0: 2020 2020 2020 2020 2065 7272 6f72 5f6d           error_m
+0001e8f0: 7367 202b 3d20 5c0a 2020 2020 2020 2020  sg += \.        
+0001e900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e910: 6b75 6265 726e 6574 6573 5f75 7469 6c73  kubernetes_utils
+0001e920: 2e67 6574 5f65 6e64 706f 696e 745f 6465  .get_endpoint_de
+0001e930: 6275 675f 6d65 7373 6167 6528 290a 2020  bug_message().  
+0001e940: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+0001e950: 6767 6572 2e77 6172 6e69 6e67 2865 7272  gger.warning(err
+0001e960: 6f72 5f6d 7367 290a 2020 2020 2020 2020  or_msg).        
+0001e970: 2020 2020 2020 2020 7265 7475 726e 207b          return {
+0001e980: 7d0a 2020 2020 2020 2020 7265 7475 726e  }.        return
+0001e990: 207b 0a20 2020 2020 2020 2020 2020 2070   {.            p
+0001e9a0: 6f72 745f 6e75 6d3a 2075 726c 735b 305d  ort_num: urls[0]
+0001e9b0: 2e75 726c 2829 2066 6f72 2070 6f72 745f  .url() for port_
+0001e9c0: 6e75 6d2c 2075 726c 7320 696e 2070 6f72  num, urls in por
+0001e9d0: 745f 6465 7461 696c 732e 6974 656d 7328  t_details.items(
+0001e9e0: 290a 2020 2020 2020 2020 7d0a            ).        }.
```

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/backends/cloud_vm_ray_backend.py` & `skypilot_nightly-1.0.0.dev20240510/sky/backends/cloud_vm_ray_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/backends/docker_utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/backends/docker_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/backends/local_docker_backend.py` & `skypilot_nightly-1.0.0.dev20240510/sky/backends/local_docker_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/backends/monkey_patches/monkey_patch_ray_up.py` & `skypilot_nightly-1.0.0.dev20240510/sky/backends/monkey_patches/monkey_patch_ray_up.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/backends/wheel_utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/backends/wheel_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/benchmark/benchmark_state.py` & `skypilot_nightly-1.0.0.dev20240510/sky/benchmark/benchmark_state.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/benchmark/benchmark_utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/check.py` & `skypilot_nightly-1.0.0.dev20240510/sky/check.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/cli.py` & `skypilot_nightly-1.0.0.dev20240510/sky/cli.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/cloud_stores.py` & `skypilot_nightly-1.0.0.dev20240510/sky/cloud_stores.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/__init__.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/aws.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/azure.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/cloud.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/cloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     IMAGE_ID = 'image_id'
     DOCKER_IMAGE = 'docker_image'
     SPOT_INSTANCE = 'spot_instance'
     CUSTOM_DISK_TIER = 'custom_disk_tier'
     OPEN_PORTS = 'open_ports'
     STORAGE_MOUNTING = 'storage_mounting'
     HOST_CONTROLLERS = 'host_controllers'  # Can run jobs/serve controllers
+    AUTO_TERMINATE = 'auto_terminate'  # Pod/VM can stop or down itself
 
 
 class Region(collections.namedtuple('Region', ['name'])):
     """A region."""
     name: str
     zones: Optional[List['Zone']] = None
```

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/cloud_registry.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/cloud_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/cudo.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/cudo.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/fluidstack.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/fluidstack.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/gcp.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/ibm.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/kubernetes.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/kubernetes.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,16 +93,20 @@
     def _unsupported_features_for_resources(
         cls, resources: 'resources_lib.Resources'
     ) -> Dict[clouds.CloudImplementationFeatures, str]:
         unsupported_features = cls._CLOUD_UNSUPPORTED_FEATURES
         is_exec_auth, message = kubernetes_utils.is_kubeconfig_exec_auth()
         if is_exec_auth:
             assert isinstance(message, str), message
+            # Controllers cannot spin up new pods with exec auth.
             unsupported_features[
                 clouds.CloudImplementationFeatures.HOST_CONTROLLERS] = message
+            # Pod does not have permissions to terminate itself with exec auth.
+            unsupported_features[
+                clouds.CloudImplementationFeatures.AUTO_TERMINATE] = message
         return unsupported_features
 
     @classmethod
     def regions(cls) -> List[clouds.Region]:
         return cls._regions
 
     @classmethod
@@ -266,15 +270,16 @@
         if acc_count > 0 and acc_type is not None:
             k8s_acc_label_key, k8s_acc_label_value = \
                 kubernetes_utils.get_gpu_label_key_value(acc_type)
 
         port_mode = network_utils.get_port_mode(None)
 
         remote_identity = skypilot_config.get_nested(
-            ('kubernetes', 'remote_identity'), schemas.REMOTE_IDENTITY_DEFAULT)
+            ('kubernetes', 'remote_identity'),
+            schemas.get_default_remote_identity('kubernetes'))
         if (remote_identity ==
                 schemas.RemoteIdentityOptions.LOCAL_CREDENTIALS.value):
             # SA name doesn't matter since automounting credentials is disabled
             k8s_service_account_name = 'default'
             k8s_automount_sa_token = 'false'
         elif (remote_identity ==
               schemas.RemoteIdentityOptions.SERVICE_ACCOUNT.value):
```

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/lambda_cloud.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/oci.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/paperspace.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/paperspace.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/runpod.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/runpod.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/scp.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/scp.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/__init__.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/aws_catalog.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/aws_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/azure_catalog.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/azure_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/common.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/common.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/config.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/cudo_catalog.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/cudo_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/data_fetchers/fetch_aws.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/data_fetchers/fetch_aws.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/data_fetchers/fetch_azure.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/data_fetchers/fetch_azure.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/fluidstack_catalog.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/fluidstack_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/gcp_catalog.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/gcp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/ibm_catalog.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/ibm_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/kubernetes_catalog.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/kubernetes_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/lambda_catalog.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/lambda_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/oci_catalog.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/oci_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/paperspace_catalog.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/paperspace_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/runpod_catalog.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/runpod_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/scp_catalog.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/scp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/service_catalog/vsphere_catalog.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/service_catalog/vsphere_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/utils/gcp_utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/utils/gcp_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/utils/lambda_utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/utils/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/utils/oci_utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/utils/oci_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/utils/scp_utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/utils/scp_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/clouds/vsphere.py` & `skypilot_nightly-1.0.0.dev20240510/sky/clouds/vsphere.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/core.py` & `skypilot_nightly-1.0.0.dev20240510/sky/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -484,14 +484,27 @@
         except exceptions.NotSupportedError as e:
             raise exceptions.NotSupportedError(
                 f'{colorama.Fore.YELLOW}Scheduling autostop on cluster '
                 f'{cluster_name!r}...skipped.{colorama.Style.RESET_ALL}\n'
                 f'  {_stop_not_supported_message(handle.launched_resources)}.'
             ) from e
 
+    # Check if autodown is required and supported
+    if not is_cancel:
+        try:
+            cloud.check_features_are_supported(
+                handle.launched_resources,
+                {clouds.CloudImplementationFeatures.AUTO_TERMINATE})
+        except exceptions.NotSupportedError as e:
+            raise exceptions.NotSupportedError(
+                f'{colorama.Fore.YELLOW}{operation} on cluster '
+                f'{cluster_name!r}...skipped.{colorama.Style.RESET_ALL}\n'
+                f'  Auto{option_str} is not supported on {cloud!r} - '
+                f'see reason above.') from e
+
     usage_lib.record_cluster_name_for_current_operation(cluster_name)
     backend.set_autostop(handle, idle_minutes, down)
 
 
 # ==================
 # = Job Management =
 # ==================
```

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/dag.py` & `skypilot_nightly-1.0.0.dev20240510/sky/dag.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/data/data_transfer.py` & `skypilot_nightly-1.0.0.dev20240510/sky/data/data_transfer.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/data/data_utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/data/mounting_utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/data/mounting_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/data/storage.py` & `skypilot_nightly-1.0.0.dev20240510/sky/data/storage.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/data/storage_utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/data/storage_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/exceptions.py` & `skypilot_nightly-1.0.0.dev20240510/sky/exceptions.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/execution.py` & `skypilot_nightly-1.0.0.dev20240510/sky/execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,16 +203,20 @@
                 verb = 'torn down' if down else 'stopped'
                 logger.info(f'{colorama.Style.DIM}The cluster will '
                             f'be {verb} after 1 minutes of idleness '
                             '(after all jobs finish).'
                             f'{colorama.Style.RESET_ALL}')
                 idle_minutes_to_autostop = 1
             stages.remove(Stage.DOWN)
-            if not down:
-                requested_features.add(clouds.CloudImplementationFeatures.STOP)
+            if idle_minutes_to_autostop >= 0:
+                requested_features.add(
+                    clouds.CloudImplementationFeatures.AUTO_TERMINATE)
+                if not down:
+                    requested_features.add(
+                        clouds.CloudImplementationFeatures.STOP)
         # NOTE: in general we may not have sufficiently specified info
         # (cloud/resource) to check STOP_SPOT_INSTANCE here. This is checked in
         # the backend.
 
     elif idle_minutes_to_autostop is not None:
         # TODO(zhwu): Autostop is not supported for non-CloudVmRayBackend.
         with ux_utils.print_exception_no_traceback():
```

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/global_user_state.py` & `skypilot_nightly-1.0.0.dev20240510/sky/global_user_state.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/jobs/__init__.py` & `skypilot_nightly-1.0.0.dev20240510/sky/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/jobs/constants.py` & `skypilot_nightly-1.0.0.dev20240510/sky/jobs/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/jobs/controller.py` & `skypilot_nightly-1.0.0.dev20240510/sky/jobs/controller.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/jobs/core.py` & `skypilot_nightly-1.0.0.dev20240510/sky/jobs/core.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/jobs/dashboard/dashboard.py` & `skypilot_nightly-1.0.0.dev20240510/sky/jobs/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/jobs/dashboard/static/favicon.ico` & `skypilot_nightly-1.0.0.dev20240510/sky/jobs/dashboard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/jobs/dashboard/templates/index.html` & `skypilot_nightly-1.0.0.dev20240510/sky/jobs/dashboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/jobs/recovery_strategy.py` & `skypilot_nightly-1.0.0.dev20240510/sky/jobs/recovery_strategy.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/jobs/state.py` & `skypilot_nightly-1.0.0.dev20240510/sky/jobs/state.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/jobs/utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/jobs/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/optimizer.py` & `skypilot_nightly-1.0.0.dev20240510/sky/optimizer.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/__init__.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/aws/__init__.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/aws/config.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/aws/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/aws/instance.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/aws/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/aws/utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/aws/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/azure/instance.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/azure/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/common.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/common.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/cudo/__init__.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/cudo/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/cudo/cudo_machine_type.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/cudo/cudo_machine_type.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/cudo/cudo_wrapper.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/cudo/cudo_wrapper.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/cudo/instance.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/cudo/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/docker_utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/docker_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/fluidstack/__init__.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/fluidstack/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/fluidstack/fluidstack_utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/fluidstack/fluidstack_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/fluidstack/instance.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/fluidstack/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/gcp/__init__.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/gcp/config.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/gcp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/gcp/constants.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/gcp/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/gcp/instance.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/gcp/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/gcp/instance_utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/gcp/instance_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/instance_setup.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/instance_setup.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/kubernetes/__init__.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/kubernetes/config.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/kubernetes/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/kubernetes/instance.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/kubernetes/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/kubernetes/manifests/smarter-device-manager-daemonset.yaml` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/kubernetes/manifests/smarter-device-manager-daemonset.yaml`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/kubernetes/network.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/kubernetes/network.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/kubernetes/network_utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/kubernetes/network_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/kubernetes/utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/kubernetes/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -630,24 +630,26 @@
     user_details = kubeconfig['users']
 
     # Find user matching the target username
     user_details = next(
         user for user in user_details if user['name'] == target_username)
 
     remote_identity = skypilot_config.get_nested(
-        ('kubernetes', 'remote_identity'), schemas.REMOTE_IDENTITY_DEFAULT)
+        ('kubernetes', 'remote_identity'),
+        schemas.get_default_remote_identity('kubernetes'))
     if ('exec' in user_details.get('user', {}) and remote_identity
             == schemas.RemoteIdentityOptions.LOCAL_CREDENTIALS.value):
         ctx_name = current_context['name']
         exec_msg = ('exec-based authentication is used for '
                     f'Kubernetes context {ctx_name!r}.'
-                    ' This may cause issues when running Managed Jobs '
-                    'or SkyServe controller on Kubernetes. To fix, configure '
-                    'SkyPilot to create a service account for running pods by '
-                    'adding the following in ~/.sky/config.yaml:\n'
+                    ' This may cause issues with autodown or when running '
+                    'Managed Jobs or SkyServe controller on Kubernetes. '
+                    'To fix, configure SkyPilot to create a service account '
+                    'for running pods by setting the following in '
+                    '~/.sky/config.yaml:\n'
                     '    kubernetes:\n'
                     '      remote_identity: SERVICE_ACCOUNT\n'
                     '    More: https://skypilot.readthedocs.io/en/latest/'
                     'reference/config.html')
         return True, exec_msg
     return False, None
```

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/logging.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/logging.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/metadata_utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/paperspace/__init__.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/paperspace/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/paperspace/config.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/paperspace/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/paperspace/constants.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/paperspace/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/paperspace/instance.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/paperspace/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/paperspace/utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/paperspace/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/provisioner.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/provisioner.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/runpod/instance.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/runpod/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/runpod/utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/runpod/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/vsphere/__init__.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/vsphere/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/vsphere/common/cls_api_client.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/vsphere/common/cls_api_client.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/vsphere/common/cls_api_helper.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/vsphere/common/cls_api_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/vsphere/common/metadata_utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/vsphere/common/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/vsphere/common/service_manager.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/vsphere/common/service_manager.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/vsphere/common/service_manager_factory.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/vsphere/common/service_manager_factory.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/vsphere/common/ssl_helper.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/vsphere/common/ssl_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/vsphere/common/vapiconnect.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/vsphere/common/vapiconnect.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/vsphere/common/vim_utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/vsphere/common/vim_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/vsphere/instance.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/vsphere/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/provision/vsphere/vsphere_utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/provision/vsphere/vsphere_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/resources.py` & `skypilot_nightly-1.0.0.dev20240510/sky/resources.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/serve/__init__.py` & `skypilot_nightly-1.0.0.dev20240510/sky/serve/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/serve/autoscalers.py` & `skypilot_nightly-1.0.0.dev20240510/sky/serve/autoscalers.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/serve/constants.py` & `skypilot_nightly-1.0.0.dev20240510/sky/serve/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/serve/controller.py` & `skypilot_nightly-1.0.0.dev20240510/sky/serve/controller.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/serve/core.py` & `skypilot_nightly-1.0.0.dev20240510/sky/serve/core.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/serve/load_balancer.py` & `skypilot_nightly-1.0.0.dev20240510/sky/serve/load_balancer.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/serve/load_balancing_policies.py` & `skypilot_nightly-1.0.0.dev20240510/sky/serve/load_balancing_policies.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/serve/replica_managers.py` & `skypilot_nightly-1.0.0.dev20240510/sky/serve/replica_managers.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/serve/serve_state.py` & `skypilot_nightly-1.0.0.dev20240510/sky/serve/serve_state.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/serve/serve_utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/serve/serve_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/serve/service.py` & `skypilot_nightly-1.0.0.dev20240510/sky/serve/service.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/serve/service_spec.py` & `skypilot_nightly-1.0.0.dev20240510/sky/serve/service_spec.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/setup_files/MANIFEST.in` & `skypilot_nightly-1.0.0.dev20240510/sky/setup_files/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/setup_files/setup.py` & `skypilot_nightly-1.0.0.dev20240510/sky/setup_files/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/sky_logging.py` & `skypilot_nightly-1.0.0.dev20240510/sky/sky_logging.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/skylet/LICENSE` & `skypilot_nightly-1.0.0.dev20240510/sky/skylet/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/skylet/attempt_skylet.py` & `skypilot_nightly-1.0.0.dev20240510/sky/skylet/attempt_skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/skylet/autostop_lib.py` & `skypilot_nightly-1.0.0.dev20240510/sky/skylet/autostop_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/skylet/configs.py` & `skypilot_nightly-1.0.0.dev20240510/sky/skylet/configs.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/skylet/constants.py` & `skypilot_nightly-1.0.0.dev20240510/sky/skylet/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/skylet/events.py` & `skypilot_nightly-1.0.0.dev20240510/sky/skylet/events.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/skylet/job_lib.py` & `skypilot_nightly-1.0.0.dev20240510/sky/skylet/job_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/skylet/log_lib.py` & `skypilot_nightly-1.0.0.dev20240510/sky/skylet/log_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/skylet/log_lib.pyi` & `skypilot_nightly-1.0.0.dev20240510/sky/skylet/log_lib.pyi`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/azure/azure-config-template.json` & `skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/azure/azure-config-template.json`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/azure/azure-vm-template.json` & `skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/azure/azure-vm-template.json`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/azure/config.py` & `skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/azure/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/azure/node_provider.py` & `skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/azure/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/command_runner.py` & `skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/command_runner.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/ibm/node_provider.py` & `skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/ibm/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/ibm/utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/ibm/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/ibm/vpc_provider.py` & `skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/ibm/vpc_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/lambda_cloud/node_provider.py` & `skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/lambda_cloud/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/oci/node_provider.py` & `skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/oci/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/oci/query_helper.py` & `skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/oci/query_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/scp/config.py` & `skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/scp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/skylet/providers/scp/node_provider.py` & `skypilot_nightly-1.0.0.dev20240510/sky/skylet/providers/scp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/skylet/ray_patches/__init__.py` & `skypilot_nightly-1.0.0.dev20240510/sky/skylet/ray_patches/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/skylet/ray_patches/log_monitor.py.patch` & `skypilot_nightly-1.0.0.dev20240510/sky/skylet/ray_patches/log_monitor.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/skylet/ray_patches/resource_demand_scheduler.py.patch` & `skypilot_nightly-1.0.0.dev20240510/sky/skylet/ray_patches/resource_demand_scheduler.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/skylet/ray_patches/worker.py.patch` & `skypilot_nightly-1.0.0.dev20240510/sky/skylet/ray_patches/worker.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/skylet/skylet.py` & `skypilot_nightly-1.0.0.dev20240510/sky/skylet/skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/skylet/subprocess_daemon.py` & `skypilot_nightly-1.0.0.dev20240510/sky/skylet/subprocess_daemon.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/skypilot_config.py` & `skypilot_nightly-1.0.0.dev20240510/sky/skypilot_config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/status_lib.py` & `skypilot_nightly-1.0.0.dev20240510/sky/status_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/task.py` & `skypilot_nightly-1.0.0.dev20240510/sky/task.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/templates/aws-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240510/sky/templates/aws-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/templates/azure-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240510/sky/templates/azure-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/templates/cudo-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240510/sky/templates/cudo-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/templates/fluidstack-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240510/sky/templates/fluidstack-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/templates/gcp-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240510/sky/templates/gcp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/templates/ibm-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240510/sky/templates/ibm-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/templates/jobs-controller.yaml.j2` & `skypilot_nightly-1.0.0.dev20240510/sky/templates/jobs-controller.yaml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/templates/kubernetes-ingress.yml.j2` & `skypilot_nightly-1.0.0.dev20240510/sky/templates/kubernetes-ingress.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/templates/kubernetes-port-forward-proxy-command.sh.j2` & `skypilot_nightly-1.0.0.dev20240510/sky/templates/kubernetes-port-forward-proxy-command.sh.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/templates/kubernetes-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240510/sky/templates/kubernetes-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/templates/kubernetes-ssh-jump.yml.j2` & `skypilot_nightly-1.0.0.dev20240510/sky/templates/kubernetes-ssh-jump.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/templates/lambda-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240510/sky/templates/lambda-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/templates/local-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240510/sky/templates/local-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/templates/oci-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240510/sky/templates/oci-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/templates/paperspace-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240510/sky/templates/paperspace-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/templates/runpod-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240510/sky/templates/runpod-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/templates/scp-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240510/sky/templates/scp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/templates/sky-serve-controller.yaml.j2` & `skypilot_nightly-1.0.0.dev20240510/sky/templates/sky-serve-controller.yaml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/templates/vsphere-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240510/sky/templates/vsphere-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/usage/constants.py` & `skypilot_nightly-1.0.0.dev20240510/sky/usage/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/usage/usage_lib.py` & `skypilot_nightly-1.0.0.dev20240510/sky/usage/usage_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/utils/accelerator_registry.py` & `skypilot_nightly-1.0.0.dev20240510/sky/utils/accelerator_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/utils/cli_utils/status_utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/utils/cli_utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/utils/cluster_yaml_utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/utils/cluster_yaml_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/utils/command_runner.py` & `skypilot_nightly-1.0.0.dev20240510/sky/utils/command_runner.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/utils/command_runner.pyi` & `skypilot_nightly-1.0.0.dev20240510/sky/utils/command_runner.pyi`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/utils/common_utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/utils/controller_utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/utils/controller_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/utils/dag_utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/utils/dag_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/utils/db_utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/utils/env_options.py` & `skypilot_nightly-1.0.0.dev20240510/sky/utils/env_options.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/utils/kubernetes/create_cluster.sh` & `skypilot_nightly-1.0.0.dev20240510/sky/utils/kubernetes/create_cluster.sh`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/utils/kubernetes/delete_cluster.sh` & `skypilot_nightly-1.0.0.dev20240510/sky/utils/kubernetes/delete_cluster.sh`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/utils/kubernetes/generate_kind_config.py` & `skypilot_nightly-1.0.0.dev20240510/sky/utils/kubernetes/generate_kind_config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/utils/kubernetes/generate_static_kubeconfig.sh` & `skypilot_nightly-1.0.0.dev20240510/sky/utils/kubernetes/generate_static_kubeconfig.sh`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/utils/kubernetes/gpu_labeler.py` & `skypilot_nightly-1.0.0.dev20240510/sky/utils/kubernetes/gpu_labeler.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml` & `skypilot_nightly-1.0.0.dev20240510/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml` & `skypilot_nightly-1.0.0.dev20240510/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py` & `skypilot_nightly-1.0.0.dev20240510/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/utils/kubernetes_enums.py` & `skypilot_nightly-1.0.0.dev20240510/sky/utils/kubernetes_enums.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/utils/log_utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/utils/resources_utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/utils/resources_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/utils/rich_utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/utils/rich_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/utils/schemas.py` & `skypilot_nightly-1.0.0.dev20240510/sky/utils/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -531,15 +531,20 @@
     identity, which map to the service account/role to use. Those are not
     included in this enum.
     """
     LOCAL_CREDENTIALS = 'LOCAL_CREDENTIALS'
     SERVICE_ACCOUNT = 'SERVICE_ACCOUNT'
 
 
-REMOTE_IDENTITY_DEFAULT = RemoteIdentityOptions.LOCAL_CREDENTIALS.value
+def get_default_remote_identity(cloud: str) -> str:
+    """Get the default remote identity for the specified cloud."""
+    if cloud == 'kubernetes':
+        return RemoteIdentityOptions.SERVICE_ACCOUNT.value
+    return RemoteIdentityOptions.LOCAL_CREDENTIALS.value
+
 
 _REMOTE_IDENTITY_SCHEMA = {
     'remote_identity': {
         'type': 'string',
         'case_insensitive_enum': [
             option.value for option in RemoteIdentityOptions
         ]
```

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/utils/subprocess_utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/utils/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/utils/timeline.py` & `skypilot_nightly-1.0.0.dev20240510/sky/utils/timeline.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/utils/ux_utils.py` & `skypilot_nightly-1.0.0.dev20240510/sky/utils/ux_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/sky/utils/validator.py` & `skypilot_nightly-1.0.0.dev20240510/sky/utils/validator.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/skypilot_nightly.egg-info/PKG-INFO` & `skypilot_nightly-1.0.0.dev20240510/skypilot_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20240509
+Version: 1.0.0.dev20240510
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

### Comparing `skypilot_nightly-1.0.0.dev20240509/skypilot_nightly.egg-info/SOURCES.txt` & `skypilot_nightly-1.0.0.dev20240510/skypilot_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/skypilot_nightly.egg-info/requires.txt` & `skypilot_nightly-1.0.0.dev20240510/skypilot_nightly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/tests/test_cli.py` & `skypilot_nightly-1.0.0.dev20240510/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/tests/test_config.py` & `skypilot_nightly-1.0.0.dev20240510/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/tests/test_jobs.py` & `skypilot_nightly-1.0.0.dev20240510/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/tests/test_jobs_and_serve.py` & `skypilot_nightly-1.0.0.dev20240510/tests/test_jobs_and_serve.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/tests/test_list_accelerators.py` & `skypilot_nightly-1.0.0.dev20240510/tests/test_list_accelerators.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/tests/test_optimizer_dryruns.py` & `skypilot_nightly-1.0.0.dev20240510/tests/test_optimizer_dryruns.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/tests/test_optimizer_random_dag.py` & `skypilot_nightly-1.0.0.dev20240510/tests/test_optimizer_random_dag.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/tests/test_serve_autoscaler.py` & `skypilot_nightly-1.0.0.dev20240510/tests/test_serve_autoscaler.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/tests/test_smoke.py` & `skypilot_nightly-1.0.0.dev20240510/tests/test_smoke.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/tests/test_storage.py` & `skypilot_nightly-1.0.0.dev20240510/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/tests/test_wheels.py` & `skypilot_nightly-1.0.0.dev20240510/tests/test_wheels.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240509/tests/test_yaml_parser.py` & `skypilot_nightly-1.0.0.dev20240510/tests/test_yaml_parser.py`

 * *Files identical despite different names*

