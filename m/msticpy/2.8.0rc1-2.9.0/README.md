# Comparing `tmp/msticpy-2.8.0rc1.tar.gz` & `tmp/msticpy-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msticpy-2.8.0rc1.tar", last modified: Wed Sep 27 01:05:04 2023, max compression
+gzip compressed data, was "msticpy-2.9.0.tar", last modified: Wed Nov 15 22:08:45 2023, max compression
```

## Comparing `msticpy-2.8.0rc1.tar` & `msticpy-2.9.0.tar`

### file list

```diff
@@ -1,424 +1,429 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.403398 msticpy-2.8.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2023-09-27 01:04:51.000000 msticpy-2.8.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      236 2023-09-27 01:04:51.000000 msticpy-2.8.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)   487752 2023-09-27 01:04:51.000000 msticpy-2.8.0rc1/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    28060 2023-09-27 01:05:04.399398 msticpy-2.8.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15960 2023-09-27 01:04:51.000000 msticpy-2.8.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.319396 msticpy-2.8.0rc1/msticpy/
--rw-r--r--   0 runner    (1001) docker     (127)     7090 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.323396 msticpy-2.8.0rc1/msticpy/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.323396 msticpy-2.8.0rc1/msticpy/analysis/anomalous_sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/analysis/anomalous_sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8125 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/analysis/anomalous_sequence/anomalous.py
--rw-r--r--   0 runner    (1001) docker     (127)    29469 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/analysis/anomalous_sequence/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/analysis/anomalous_sequence/sessionize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.323396 msticpy-2.8.0rc1/msticpy/analysis/anomalous_sequence/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/analysis/anomalous_sequence/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10732 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/analysis/anomalous_sequence/utils/cmds_only.py
--rw-r--r--   0 runner    (1001) docker     (127)    15670 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/analysis/anomalous_sequence/utils/cmds_params_only.py
--rw-r--r--   0 runner    (1001) docker     (127)    21586 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/analysis/anomalous_sequence/utils/cmds_params_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/analysis/anomalous_sequence/utils/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/analysis/anomalous_sequence/utils/laplace_smooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6404 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/analysis/anomalous_sequence/utils/probabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/analysis/cluster_auditd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/analysis/code_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)    23201 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/analysis/eventcluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     7202 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/analysis/observationlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/analysis/outliers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7610 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/analysis/polling_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     9898 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/analysis/syslog_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16759 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/analysis/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.327396 msticpy-2.8.0rc1/msticpy/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5962 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/auth/azure_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    15638 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/auth/azure_auth_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9115 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/auth/cloud_mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6446 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/auth/cloud_mappings_offline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/auth/cred_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/auth/keyring_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    18623 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/auth/keyvault_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7185 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/auth/keyvault_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/auth/msal_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     9358 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/auth/secret_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.327396 msticpy-2.8.0rc1/msticpy/common/
--rw-r--r--   0 runner    (1001) docker     (127)      875 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/common/azure_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/common/check_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/common/data_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/common/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17918 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19073 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/common/pkg_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11516 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/common/provider_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/common/proxy_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/common/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6358 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/common/timespan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.327396 msticpy-2.8.0rc1/msticpy/common/utility/
--rw-r--r--   0 runner    (1001) docker     (127)      838 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/common/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/common/utility/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     6074 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/common/utility/ipython.py
--rw-r--r--   0 runner    (1001) docker     (127)    10117 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/common/utility/package.py
--rw-r--r--   0 runner    (1001) docker     (127)    10757 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/common/utility/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    15928 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/common/wsconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.331396 msticpy-2.8.0rc1/msticpy/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/config/ce_azure.py
--rw-r--r--   0 runner    (1001) docker     (127)    12752 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/config/ce_azure_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (127)    13346 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/config/ce_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/config/ce_data_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/config/ce_keyvault.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/config/ce_msticpy.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/config/ce_other_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9086 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/config/ce_provider_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/config/ce_simple_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/config/ce_ti_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11988 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/config/ce_user_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)    12385 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/config/comp_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)    19231 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/config/compound_ctrls.py
--rw-r--r--   0 runner    (1001) docker     (127)     7080 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/config/file_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)    24855 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/config/mp_config_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     7160 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/config/mp_config_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)    18380 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/config/mp_config_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    35348 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/config/query_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.331396 msticpy-2.8.0rc1/msticpy/context/
--rw-r--r--   0 runner    (1001) docker     (127)      815 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.335396 msticpy-2.8.0rc1/msticpy/context/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36046 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/azure/azure_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11307 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/azure/sentinel_analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5409 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/azure/sentinel_bookmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)    14499 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/azure/sentinel_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    14993 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/azure/sentinel_dynamic_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)    25652 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/azure/sentinel_dynamic_summary_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    16951 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/azure/sentinel_incidents.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/azure/sentinel_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    15868 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/azure/sentinel_ti.py
--rw-r--r--   0 runner    (1001) docker     (127)    10844 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/azure/sentinel_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11179 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/azure/sentinel_watchlists.py
--rw-r--r--   0 runner    (1001) docker     (127)    12444 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/azure/sentinel_workspaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     8468 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/contextlookup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.335396 msticpy-2.8.0rc1/msticpy/context/contextproviders/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/contextproviders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10638 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/contextproviders/context_provider_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/contextproviders/http_context_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     8885 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/contextproviders/servicenow.py
--rw-r--r--   0 runner    (1001) docker     (127)    11287 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/domain_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    33053 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/geoip.py
--rw-r--r--   0 runner    (1001) docker     (127)     9261 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/http_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    25638 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/ip_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    27130 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/lookup_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    10684 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/preprocess_observable.py
--rw-r--r--   0 runner    (1001) docker     (127)    14327 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/provider_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9907 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/tilookup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.339396 msticpy-2.8.0rc1/msticpy/context/tiproviders/
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/tiproviders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/tiproviders/abuseipdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/tiproviders/alienvault_otx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/tiproviders/azure_sent_byoti.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/tiproviders/crowdsec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/tiproviders/greynoise.py
--rw-r--r--   0 runner    (1001) docker     (127)     5523 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/tiproviders/ibm_xforce.py
--rw-r--r--   0 runner    (1001) docker     (127)     5007 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/tiproviders/intsights.py
--rw-r--r--   0 runner    (1001) docker     (127)    14334 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/tiproviders/kql_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6095 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/tiproviders/mblookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     9223 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/tiproviders/open_page_rank.py
--rw-r--r--   0 runner    (1001) docker     (127)    10986 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/tiproviders/pulsedive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/tiproviders/result_severity.py
--rw-r--r--   0 runner    (1001) docker     (127)    13914 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/tiproviders/riskiq.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/tiproviders/ti_http_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    10303 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/tiproviders/ti_provider_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5506 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/tiproviders/tor_exit_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/tiproviders/virustotal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.339396 msticpy-2.8.0rc1/msticpy/context/vtlookupv3/
--rw-r--r--   0 runner    (1001) docker     (127)      959 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/vtlookupv3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15011 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/vtlookupv3/vtfile_behavior.py
--rw-r--r--   0 runner    (1001) docker     (127)    29926 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/vtlookupv3/vtlookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    32775 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/context/vtlookupv3/vtlookupv3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.339396 msticpy-2.8.0rc1/msticpy/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.339396 msticpy-2.8.0rc1/msticpy/data/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/azure/azure_blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/azure/azure_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/azure_blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/azure_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/azure_sentinel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.343397 msticpy-2.8.0rc1/msticpy/data/core/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18277 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/core/data_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/core/data_query_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3791 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/core/param_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/core/query_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/core/query_defns.py
--rw-r--r--   0 runner    (1001) docker     (127)    15204 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/core/query_provider_connections_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    11306 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/core/query_provider_utils_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    19514 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/core/query_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    13127 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/core/query_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/core/query_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    14411 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/data_obfus.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/data_providers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.343397 msticpy-2.8.0rc1/msticpy/data/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37124 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/drivers/azure_kusto_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    25223 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/drivers/azure_monitor_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    15415 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/drivers/cybereason_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     9709 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/drivers/driver_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6815 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/drivers/elastic_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    22566 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/drivers/kql_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    11953 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/drivers/kusto_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4688 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/drivers/local_data_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    12895 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/drivers/local_osquery_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7660 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/drivers/local_velociraptor_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/drivers/mdatp_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    29511 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/drivers/mordor_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    13922 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/drivers/odata_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6182 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/drivers/resource_graph_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/drivers/security_graph_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    15713 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/drivers/sentinel_query_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    18939 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/drivers/splunk_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    22229 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/drivers/sumologic_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.315396 msticpy-2.8.0rc1/msticpy/data/queries/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.343397 msticpy-2.8.0rc1/msticpy/data/queries/cybereason/
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/cybereason/cybereason_connections.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/cybereason/cybereason_hosts.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/cybereason/cybereason_processes.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.347397 msticpy-2.8.0rc1/msticpy/data/queries/localdata/
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/localdata/local_data.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.347397 msticpy-2.8.0rc1/msticpy/data/queries/m365d/
--rw-r--r--   0 runner    (1001) docker     (127)     9682 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/m365d/kql_m365_alerts.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/m365d/kql_m365_file.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    29360 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/m365d/kql_m365_hunting.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/m365d/kql_m365_identity.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/m365d/kql_m365_network.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/m365d/kql_m365_process.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/m365d/kql_m365_user.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.347397 msticpy-2.8.0rc1/msticpy/data/queries/mde/
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/mde/kql_mdatp_alerts.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/mde/kql_mdatp_file.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    28945 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/mde/kql_mdatp_hunting.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/mde/kql_mdatp_network.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3067 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/mde/kql_mdatp_process.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/mde/kql_mdatp_user.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.347397 msticpy-2.8.0rc1/msticpy/data/queries/msgraph/
--rw-r--r--   0 runner    (1001) docker     (127)     6344 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/msgraph/graph_alerts.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.351397 msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/
--rw-r--r--   0 runner    (1001) docker     (127)     7745 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_alert.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_az_dns.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_az_network.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8924 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_azure.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_azuresentinel.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_heartbeat_info.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_lxauditd.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5552 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_activity.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_apps.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11594 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_logon.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5582 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_sysmon.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11588 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_net.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_o365.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_threatintel.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_timeseries.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7767 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_winevent.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7063 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_winevent_logon.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11583 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_winevent_proc.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.351397 msticpy-2.8.0rc1/msticpy/data/queries/resourcegraph/
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/resourcegraph/resource_graph_queries.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/resourcegraph/sentinel_resources.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.351397 msticpy-2.8.0rc1/msticpy/data/queries/splunk/
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/splunk/splunk_alert_queries.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/splunk/splunk_authentication_queries.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/splunk/splunk_queries.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.351397 msticpy-2.8.0rc1/msticpy/data/queries/sumologic/
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/queries/sumologic/sumologic_queries.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      897 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/query_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/query_defns.py
--rw-r--r--   0 runner    (1001) docker     (127)    20260 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/sql_to_kql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.351397 msticpy-2.8.0rc1/msticpy/data/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      501 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8963 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/storage/azure_blob_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.351397 msticpy-2.8.0rc1/msticpy/data/uploaders/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/uploaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7515 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/uploaders/loganalytics_uploader.py
--rw-r--r--   0 runner    (1001) docker     (127)     8973 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/uploaders/splunk_uploader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/data/uploaders/uploader_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.351397 msticpy-2.8.0rc1/msticpy/datamodel/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.355397 msticpy-2.8.0rc1/msticpy/datamodel/entities/
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6847 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/entities/account.py
--rw-r--r--   0 runner    (1001) docker     (127)    14897 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/entities/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/entities/azure_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/entities/cloud_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/entities/cloud_logon_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/entities/dns.py
--rw-r--r--   0 runner    (1001) docker     (127)    22029 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/entities/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/entities/entity_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/entities/entity_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     6182 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/entities/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/entities/file_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/entities/geo_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/entities/graph_property.py
--rw-r--r--   0 runner    (1001) docker     (127)     4978 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/entities/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/entities/host_logon_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/entities/iot_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/entities/ip_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/entities/mail_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     7051 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/entities/mail_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/entities/mailbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/entities/malware.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/entities/network_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6852 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/entities/process.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/entities/registry_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/entities/registry_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/entities/security_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/entities/submission_mail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/entities/threat_intelligence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/entities/unknown_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/entities/url.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/pivot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.355397 msticpy-2.8.0rc1/msticpy/datamodel/soc/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/soc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6164 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/soc/incident.py
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/datamodel/soc/sentinel_alert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.359397 msticpy-2.8.0rc1/msticpy/init/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16745 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/init/azure_ml_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    20176 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/init/azure_synapse_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/init/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    10448 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/init/mp_pandas_accessors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/init/mp_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)    31530 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/init/nbinit.py
--rw-r--r--   0 runner    (1001) docker     (127)     7014 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/init/nbmagics.py
--rw-r--r--   0 runner    (1001) docker     (127)    13591 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/init/pivot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.359397 msticpy-2.8.0rc1/msticpy/init/pivot_core/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/init/pivot_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9063 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/init/pivot_core/pivot_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/init/pivot_core/pivot_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/init/pivot_core/pivot_magic_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    15811 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/init/pivot_core/pivot_pd_accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10435 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/init/pivot_core/pivot_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    19763 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/init/pivot_core/pivot_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     7457 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/init/pivot_core/pivot_register_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.359397 msticpy-2.8.0rc1/msticpy/init/pivot_init/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/init/pivot_init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26897 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/init/pivot_init/pivot_data_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/init/pivot_init/pivot_ti_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     6819 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/init/pivot_init/vt_pivot.py
--rw-r--r--   0 runner    (1001) docker     (127)     9345 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/init/user_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/msticpyconfig.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.363397 msticpy-2.8.0rc1/msticpy/nbtools/
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/nbtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/nbtools/data_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/nbtools/entityschema.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/nbtools/foliummap.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/nbtools/morph_charts.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/nbtools/nbdisplay.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/nbtools/nbwidgets.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/nbtools/observationlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/nbtools/process_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     7868 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/nbtools/security_alert.py
--rw-r--r--   0 runner    (1001) docker     (127)    11227 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/nbtools/security_alert_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    18315 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/nbtools/security_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/nbtools/security_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/nbtools/ti_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/nbtools/timeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/nbtools/timeline_duration.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/nbtools/timeline_pd_accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/nbtools/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/nbtools/utility.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/nbtools/wsconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.363397 msticpy-2.8.0rc1/msticpy/nbwidgets/
--rw-r--r--   0 runner    (1001) docker     (127)      976 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/nbwidgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5862 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/nbwidgets/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/nbwidgets/get_environment_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/nbwidgets/get_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/nbwidgets/lookback.py
--rw-r--r--   0 runner    (1001) docker     (127)     5689 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/nbwidgets/option_buttons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/nbwidgets/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)    14485 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/nbwidgets/query_time.py
--rw-r--r--   0 runner    (1001) docker     (127)    11759 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/nbwidgets/select_alert.py
--rw-r--r--   0 runner    (1001) docker     (127)    10931 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/nbwidgets/select_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     6858 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/nbwidgets/select_subset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.367397 msticpy-2.8.0rc1/msticpy/resources/
--rw-r--r--   0 runner    (1001) docker     (127)   104245 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/resources/WinSecurityEvent.json
--rw-r--r--   0 runner    (1001) docker     (127)      188 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/resources/cmd_line_rules.json
--rw-r--r--   0 runner    (1001) docker     (127)     6899 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/resources/mp_pivot_reg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8822 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/resources/mpconfig_defaults.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/resources/obfuscation_cols.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.367397 msticpy-2.8.0rc1/msticpy/sectools/
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/sectools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/sectools/auditdextract.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/sectools/base64unpack.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/sectools/cmd_line.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/sectools/domain_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/sectools/eventcluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/sectools/geoip.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/sectools/iocextract.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/sectools/ip_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/sectools/proc_tree_build_mde.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/sectools/proc_tree_build_winlx.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/sectools/proc_tree_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/sectools/proc_tree_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/sectools/proc_tree_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/sectools/sectools_magics.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/sectools/syslog_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/sectools/tilookup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.367397 msticpy-2.8.0rc1/msticpy/sectools/tiproviders/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/sectools/tiproviders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/sectools/tiproviders/ti_provider_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/sectools/vtlookup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.367397 msticpy-2.8.0rc1/msticpy/sectools/vtlookupv3/
--rw-r--r--   0 runner    (1001) docker     (127)      702 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/sectools/vtlookupv3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/sectools/vtlookupv3/vtfile_behavior.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/sectools/vtlookupv3/vtlookupv3.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/sectools/vtlookupv3/vtobject_browser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.371397 msticpy-2.8.0rc1/msticpy/transform/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16277 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/transform/auditdextract.py
--rw-r--r--   0 runner    (1001) docker     (127)    30712 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/transform/base64unpack.py
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/transform/cmd_line.py
--rw-r--r--   0 runner    (1001) docker     (127)    28354 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/transform/iocextract.py
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/transform/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    13044 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/transform/proc_tree_build_mde.py
--rw-r--r--   0 runner    (1001) docker     (127)    12671 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/transform/proc_tree_build_winlx.py
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/transform/proc_tree_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8496 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/transform/proc_tree_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    13847 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/transform/process_tree_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.375397 msticpy-2.8.0rc1/msticpy/vis/
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/vis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/vis/code_view.py
--rw-r--r--   0 runner    (1001) docker     (127)    18620 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/vis/data_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9261 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/vis/data_viewer_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)    17654 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/vis/entity_graph_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/vis/figure_dimension.py
--rw-r--r--   0 runner    (1001) docker     (127)    33234 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/vis/foliummap.py
--rw-r--r--   0 runner    (1001) docker     (127)    10309 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/vis/matrix_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    14928 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/vis/mordor_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/vis/morph_charts.py
--rw-r--r--   0 runner    (1001) docker     (127)    23583 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/vis/mp_pandas_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     9180 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/vis/nbdisplay.py
--rw-r--r--   0 runner    (1001) docker     (127)    10997 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/vis/network_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    22523 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/vis/process_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/vis/query_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6445 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/vis/ti_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)    17827 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/vis/timeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    13654 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/vis/timeline_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     8776 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/vis/timeline_duration.py
--rw-r--r--   0 runner    (1001) docker     (127)    10655 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/vis/timeline_pd_accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12034 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/vis/timeline_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     8771 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/vis/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/msticpy/vis/vtobject_browser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:05:04.319396 msticpy-2.8.0rc1/msticpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28060 2023-09-27 01:05:04.000000 msticpy-2.8.0rc1/msticpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14218 2023-09-27 01:05:04.000000 msticpy-2.8.0rc1/msticpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-27 01:05:04.000000 msticpy-2.8.0rc1/msticpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-27 01:05:04.000000 msticpy-2.8.0rc1/msticpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     4613 2023-09-27 01:05:04.000000 msticpy-2.8.0rc1/msticpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-09-27 01:05:04.000000 msticpy-2.8.0rc1/msticpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      209 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (127)      626 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      895 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2023-09-27 01:05:04.403398 msticpy-2.8.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2023-09-27 01:04:52.000000 msticpy-2.8.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.455237 msticpy-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2023-11-15 22:08:35.000000 msticpy-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2023-11-15 22:08:35.000000 msticpy-2.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)   487752 2023-11-15 22:08:35.000000 msticpy-2.9.0/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    28071 2023-11-15 22:08:45.455237 msticpy-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15960 2023-11-15 22:08:35.000000 msticpy-2.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.367238 msticpy-2.9.0/msticpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.371238 msticpy-2.9.0/msticpy/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.371238 msticpy-2.9.0/msticpy/analysis/anomalous_sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/analysis/anomalous_sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8125 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/analysis/anomalous_sequence/anomalous.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29469 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/analysis/anomalous_sequence/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/analysis/anomalous_sequence/sessionize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.371238 msticpy-2.9.0/msticpy/analysis/anomalous_sequence/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/analysis/anomalous_sequence/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10732 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/analysis/anomalous_sequence/utils/cmds_only.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15670 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/analysis/anomalous_sequence/utils/cmds_params_only.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21586 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/analysis/anomalous_sequence/utils/cmds_params_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/analysis/anomalous_sequence/utils/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/analysis/anomalous_sequence/utils/laplace_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6404 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/analysis/anomalous_sequence/utils/probabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/analysis/cluster_auditd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/analysis/code_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23201 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/analysis/eventcluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7224 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/analysis/observationlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/analysis/outliers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7610 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/analysis/polling_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9898 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/analysis/syslog_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16759 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/analysis/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.375238 msticpy-2.9.0/msticpy/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5962 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/auth/azure_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17098 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/auth/azure_auth_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9115 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/auth/cloud_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6446 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/auth/cloud_mappings_offline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/auth/cred_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/auth/keyring_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18623 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/auth/keyvault_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7185 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/auth/keyvault_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/auth/msal_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9358 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/auth/secret_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.375238 msticpy-2.9.0/msticpy/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/common/azure_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/common/check_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5757 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/common/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/common/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17918 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19073 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/common/pkg_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11516 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/common/provider_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/common/proxy_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/common/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6358 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/common/timespan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.379238 msticpy-2.9.0/msticpy/common/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/common/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/common/utility/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6074 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/common/utility/ipython.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10120 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/common/utility/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10757 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/common/utility/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16746 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/common/wsconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.379238 msticpy-2.9.0/msticpy/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/config/ce_azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12758 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/config/ce_azure_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13346 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/config/ce_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/config/ce_data_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/config/ce_keyvault.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/config/ce_msticpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/config/ce_other_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9086 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/config/ce_provider_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/config/ce_simple_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/config/ce_ti_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12012 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/config/ce_user_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12385 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/config/comp_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19231 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/config/compound_ctrls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7080 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/config/file_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24855 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/config/mp_config_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7160 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/config/mp_config_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18385 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/config/mp_config_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35348 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/config/query_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.383238 msticpy-2.9.0/msticpy/context/
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.383238 msticpy-2.9.0/msticpy/context/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36046 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/azure/azure_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11307 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/azure/sentinel_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5409 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/azure/sentinel_bookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14499 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/azure/sentinel_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15013 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/azure/sentinel_dynamic_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25652 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/azure/sentinel_dynamic_summary_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16951 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/azure/sentinel_incidents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/azure/sentinel_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15868 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/azure/sentinel_ti.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10844 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/azure/sentinel_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11242 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/azure/sentinel_watchlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12464 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/azure/sentinel_workspaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8468 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/contextlookup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.387238 msticpy-2.9.0/msticpy/context/contextproviders/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/contextproviders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10638 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/contextproviders/context_provider_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/contextproviders/http_context_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8885 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/contextproviders/servicenow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11418 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/domain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33053 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/geoip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9261 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/http_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25638 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/ip_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27130 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/lookup_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10684 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/preprocess_observable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14327 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/provider_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9907 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/tilookup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.391238 msticpy-2.9.0/msticpy/context/tiproviders/
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/tiproviders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/tiproviders/abuseipdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/tiproviders/alienvault_otx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/tiproviders/azure_sent_byoti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/tiproviders/crowdsec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/tiproviders/greynoise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5523 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/tiproviders/ibm_xforce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5076 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/tiproviders/intsights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/tiproviders/ip_quality_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14354 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/tiproviders/kql_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6095 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/tiproviders/mblookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9162 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/tiproviders/open_page_rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10986 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/tiproviders/pulsedive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/tiproviders/result_severity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13914 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/tiproviders/riskiq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4743 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/tiproviders/ti_http_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10303 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/tiproviders/ti_provider_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5506 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/tiproviders/tor_exit_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/tiproviders/virustotal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.391238 msticpy-2.9.0/msticpy/context/vtlookupv3/
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/vtlookupv3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15011 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/vtlookupv3/vtfile_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29926 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/vtlookupv3/vtlookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32775 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/context/vtlookupv3/vtlookupv3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.391238 msticpy-2.9.0/msticpy/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.391238 msticpy-2.9.0/msticpy/data/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/azure/azure_blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/azure/azure_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/azure_blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/azure_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/azure_sentinel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.395238 msticpy-2.9.0/msticpy/data/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18288 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/core/data_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/core/data_query_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/core/param_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/core/query_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/core/query_defns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15214 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/core/query_provider_connections_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11312 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/core/query_provider_utils_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19514 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/core/query_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13127 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/core/query_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/core/query_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14411 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/data_obfus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/data_providers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.399238 msticpy-2.9.0/msticpy/data/drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37116 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/drivers/azure_kusto_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25311 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/drivers/azure_monitor_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21726 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/drivers/cybereason_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9709 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/drivers/driver_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/drivers/elastic_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22566 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/drivers/kql_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11953 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/drivers/kusto_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4688 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/drivers/local_data_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12895 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/drivers/local_osquery_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7660 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/drivers/local_velociraptor_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5386 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/drivers/mdatp_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29539 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/drivers/mordor_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14001 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/drivers/odata_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6182 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/drivers/resource_graph_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/drivers/security_graph_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15713 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/drivers/sentinel_query_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19397 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/drivers/splunk_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22229 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/drivers/sumologic_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.363238 msticpy-2.9.0/msticpy/data/queries/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.399238 msticpy-2.9.0/msticpy/data/queries/cybereason/
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/cybereason/cybereason_connections.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/cybereason/cybereason_hosts.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/cybereason/cybereason_processes.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.399238 msticpy-2.9.0/msticpy/data/queries/localdata/
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/localdata/local_data.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.399238 msticpy-2.9.0/msticpy/data/queries/m365d/
+-rw-r--r--   0 runner    (1001) docker     (127)     9682 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/m365d/kql_m365_alerts.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/m365d/kql_m365_file.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    29220 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/m365d/kql_m365_hunting.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/m365d/kql_m365_identity.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/m365d/kql_m365_network.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/m365d/kql_m365_process.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/m365d/kql_m365_user.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.403238 msticpy-2.9.0/msticpy/data/queries/mde/
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/mde/kql_mdatp_alerts.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/mde/kql_mdatp_file.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    28801 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/mde/kql_mdatp_hunting.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/mde/kql_mdatp_network.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/mde/kql_mdatp_process.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/mde/kql_mdatp_user.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.403238 msticpy-2.9.0/msticpy/data/queries/msgraph/
+-rw-r--r--   0 runner    (1001) docker     (127)     6344 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/msgraph/graph_alerts.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.407238 msticpy-2.9.0/msticpy/data/queries/mssentinel/
+-rw-r--r--   0 runner    (1001) docker     (127)     7745 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_alert.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_az_dns.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_az_network.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8924 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_azure.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_azuresentinel.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_heartbeat_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_lxauditd.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5552 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_activity.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_apps.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11594 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_logon.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5582 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_sysmon.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11588 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_net.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_o365.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_threatintel.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_timeseries.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7767 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_winevent.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7063 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_winevent_logon.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11583 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_winevent_proc.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.407238 msticpy-2.9.0/msticpy/data/queries/resourcegraph/
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/resourcegraph/resource_graph_queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/resourcegraph/sentinel_resources.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.407238 msticpy-2.9.0/msticpy/data/queries/splunk/
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/splunk/splunk_alert_queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/splunk/splunk_authentication_queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/splunk/splunk_queries.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.407238 msticpy-2.9.0/msticpy/data/queries/sumologic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/queries/sumologic/sumologic_queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/query_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/query_defns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20260 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/sql_to_kql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.407238 msticpy-2.9.0/msticpy/data/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8963 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/storage/azure_blob_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.407238 msticpy-2.9.0/msticpy/data/uploaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/uploaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7515 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/uploaders/loganalytics_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8973 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/uploaders/splunk_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/data/uploaders/uploader_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.407238 msticpy-2.9.0/msticpy/datamodel/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.415238 msticpy-2.9.0/msticpy/datamodel/entities/
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7666 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15340 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/azure_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/cloud_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/cloud_logon_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/dns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22165 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/entity_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/entity_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6275 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/file_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/geo_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/graph_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/host_logon_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/iot_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/mail_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7051 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/mail_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/mailbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/mailbox_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/malware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/network_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/oauth_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6852 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/registry_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/registry_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/security_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/service_principal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/submission_mail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/threat_intelligence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/unknown_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/entities/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/pivot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.415238 msticpy-2.9.0/msticpy/datamodel/soc/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/soc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/soc/incident.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/datamodel/soc/sentinel_alert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.415238 msticpy-2.9.0/msticpy/init/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16745 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/init/azure_ml_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20176 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/init/azure_synapse_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/init/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10448 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/init/mp_pandas_accessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/init/mp_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32752 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/init/nbinit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7014 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/init/nbmagics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13684 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/init/pivot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.415238 msticpy-2.9.0/msticpy/init/pivot_core/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/init/pivot_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9063 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/init/pivot_core/pivot_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/init/pivot_core/pivot_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/init/pivot_core/pivot_magic_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15811 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/init/pivot_core/pivot_pd_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10435 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/init/pivot_core/pivot_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19763 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/init/pivot_core/pivot_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/init/pivot_core/pivot_register_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.419238 msticpy-2.9.0/msticpy/init/pivot_init/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/init/pivot_init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26897 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/init/pivot_init/pivot_data_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/init/pivot_init/pivot_ti_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6819 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/init/pivot_init/vt_pivot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9359 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/init/user_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/lazy_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/msticpyconfig.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.423238 msticpy-2.9.0/msticpy/nbtools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/nbtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/nbtools/data_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/nbtools/entityschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/nbtools/foliummap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/nbtools/morph_charts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/nbtools/nbdisplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/nbtools/nbwidgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/nbtools/observationlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/nbtools/process_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7868 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/nbtools/security_alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11227 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/nbtools/security_alert_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18315 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/nbtools/security_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/nbtools/security_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/nbtools/ti_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/nbtools/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/nbtools/timeline_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/nbtools/timeline_pd_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/nbtools/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/nbtools/utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/nbtools/wsconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.423238 msticpy-2.9.0/msticpy/nbwidgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/nbwidgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5862 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/nbwidgets/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/nbwidgets/get_environment_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/nbwidgets/get_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/nbwidgets/lookback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5689 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/nbwidgets/option_buttons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/nbwidgets/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14485 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/nbwidgets/query_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11759 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/nbwidgets/select_alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10931 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/nbwidgets/select_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6858 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/nbwidgets/select_subset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.423238 msticpy-2.9.0/msticpy/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)   104245 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/resources/WinSecurityEvent.json
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/resources/cmd_line_rules.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6899 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/resources/mp_pivot_reg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8939 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/resources/mpconfig_defaults.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/resources/obfuscation_cols.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.427238 msticpy-2.9.0/msticpy/sectools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/sectools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/sectools/auditdextract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/sectools/base64unpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/sectools/cmd_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/sectools/domain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/sectools/eventcluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/sectools/geoip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/sectools/iocextract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/sectools/ip_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/sectools/proc_tree_build_mde.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/sectools/proc_tree_build_winlx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/sectools/proc_tree_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/sectools/proc_tree_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/sectools/proc_tree_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/sectools/sectools_magics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/sectools/syslog_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/sectools/tilookup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.427238 msticpy-2.9.0/msticpy/sectools/tiproviders/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/sectools/tiproviders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/sectools/tiproviders/ti_provider_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/sectools/vtlookup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.427238 msticpy-2.9.0/msticpy/sectools/vtlookupv3/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/sectools/vtlookupv3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/sectools/vtlookupv3/vtfile_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/sectools/vtlookupv3/vtlookupv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/sectools/vtlookupv3/vtobject_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.431238 msticpy-2.9.0/msticpy/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16277 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/transform/auditdextract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30712 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/transform/base64unpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/transform/cmd_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28354 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/transform/iocextract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/transform/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13044 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/transform/proc_tree_build_mde.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12678 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/transform/proc_tree_build_winlx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/transform/proc_tree_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8496 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/transform/proc_tree_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13847 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/transform/process_tree_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.435238 msticpy-2.9.0/msticpy/vis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/vis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/vis/code_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18620 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/vis/data_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9348 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/vis/data_viewer_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17654 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/vis/entity_graph_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/vis/figure_dimension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33234 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/vis/foliummap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10309 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/vis/matrix_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14928 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/vis/mordor_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/vis/morph_charts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23583 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/vis/mp_pandas_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9180 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/vis/nbdisplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10997 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/vis/network_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22523 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/vis/process_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/vis/query_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/vis/ti_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17827 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/vis/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13654 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/vis/timeline_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8776 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/vis/timeline_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10655 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/vis/timeline_pd_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12034 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/vis/timeline_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8771 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/vis/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2023-11-15 22:08:35.000000 msticpy-2.9.0/msticpy/vis/vtobject_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:08:45.367238 msticpy-2.9.0/msticpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28071 2023-11-15 22:08:45.000000 msticpy-2.9.0/msticpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14439 2023-11-15 22:08:45.000000 msticpy-2.9.0/msticpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-15 22:08:45.000000 msticpy-2.9.0/msticpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-15 22:08:45.000000 msticpy-2.9.0/msticpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2023-11-15 22:08:45.000000 msticpy-2.9.0/msticpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-15 22:08:45.000000 msticpy-2.9.0/msticpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2023-11-15 22:08:35.000000 msticpy-2.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2023-11-15 22:08:35.000000 msticpy-2.9.0/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2023-11-15 22:08:35.000000 msticpy-2.9.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2023-11-15 22:08:35.000000 msticpy-2.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2023-11-15 22:08:45.455237 msticpy-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2023-11-15 22:08:35.000000 msticpy-2.9.0/setup.py
```

### Comparing `msticpy-2.8.0rc1/LICENSE` & `msticpy-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/NOTICE.txt` & `msticpy-2.9.0/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/PKG-INFO` & `msticpy-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msticpy
-Version: 2.8.0rc1
+Version: 2.9.0
 Summary: MSTIC Security Tools
 Home-page: https://github.com/microsoft/msticpy
 Author: Ian Hellen
 Author-email: ianhelle@microsoft.com
 Maintainer: Pete Bryan
 Maintainer-email: peter.bryan@microsoft.com
 License: MIT License
@@ -102,19 +102,19 @@
 Requires-Dist: pygeohash>=1.2.0; extra == "dev"
 Requires-Dist: pylint>=2.5.3; extra == "dev"
 Requires-Dist: pyroma>=3.1; extra == "dev"
 Requires-Dist: pytest-check>=1.0.1; extra == "dev"
 Requires-Dist: pytest-cov>=2.11.1; extra == "dev"
 Requires-Dist: pytest-xdist>=2.5.0; extra == "dev"
 Requires-Dist: pytest>=5.0.1; extra == "dev"
-Requires-Dist: readthedocs-sphinx-ext==2.2.2; extra == "dev"
+Requires-Dist: readthedocs-sphinx-ext==2.2.3; extra == "dev"
 Requires-Dist: responses>=0.13.2; extra == "dev"
 Requires-Dist: respx>=0.20.1; extra == "dev"
 Requires-Dist: sphinx-rtd-theme>=1.0.0; extra == "dev"
-Requires-Dist: sphinx>=5.0.1; extra == "dev"
+Requires-Dist: sphinx<8.0.0,>=5.0.1; extra == "dev"
 Requires-Dist: types-attrs>=19.0.0; extra == "dev"
 Provides-Extra: vt3
 Requires-Dist: vt-py>=0.6.1; extra == "vt3"
 Requires-Dist: vt-graph-api>=2.0; extra == "vt3"
 Requires-Dist: nest_asyncio>=1.4.0; extra == "vt3"
 Provides-Extra: splunk
 Requires-Dist: splunk-sdk>=1.6.0; extra == "splunk"
@@ -216,21 +216,21 @@
 Requires-Dist: pygeohash>=1.2.0; extra == "test"
 Requires-Dist: pylint>=2.5.3; extra == "test"
 Requires-Dist: pyroma>=3.1; extra == "test"
 Requires-Dist: pytest-check>=1.0.1; extra == "test"
 Requires-Dist: pytest-cov>=2.11.1; extra == "test"
 Requires-Dist: pytest-xdist>=2.5.0; extra == "test"
 Requires-Dist: pytest>=5.0.1; extra == "test"
-Requires-Dist: readthedocs-sphinx-ext==2.2.2; extra == "test"
+Requires-Dist: readthedocs-sphinx-ext==2.2.3; extra == "test"
 Requires-Dist: responses>=0.13.2; extra == "test"
 Requires-Dist: respx>=0.20.1; extra == "test"
 Requires-Dist: scikit-learn>=1.0.0; extra == "test"
 Requires-Dist: scipy>=1.1.0; extra == "test"
 Requires-Dist: sphinx-rtd-theme>=1.0.0; extra == "test"
-Requires-Dist: sphinx>=5.0.1; extra == "test"
+Requires-Dist: sphinx<8.0.0,>=5.0.1; extra == "test"
 Requires-Dist: splunk-sdk>=1.6.0; extra == "test"
 Requires-Dist: statsmodels>=0.11.1; extra == "test"
 Requires-Dist: sumologic-sdk>=0.1.11; extra == "test"
 Requires-Dist: types-attrs>=19.0.0; extra == "test"
 Requires-Dist: vt-graph-api>=2.0; extra == "test"
 Requires-Dist: vt-py>=0.6.1; extra == "test"
 Provides-Extra: azsentinel
```

### Comparing `msticpy-2.8.0rc1/README.md` & `msticpy-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/__init__.py` & `msticpy-2.9.0/msticpy/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -129,90 +129,45 @@
 from .common.exceptions import (
     MsticpyException,
     MsticpyImportExtraError,
     MsticpyMissingDependencyError,
 )
 from .common.utility import search_name as search
 from .init.logging import set_logging_level, setup_logging
+from .lazy_importer import lazy_import
 
 __version__ = VERSION
 __author__ = "Ian Hellen, Pete Bryan, Ashwin Patil"
 
 refresh_config = settings.refresh_config
 get_config = settings.get_config
 setup_logging()
 
 if not os.environ.get("KQLMAGIC_EXTRAS_REQUIRES"):
     os.environ["KQLMAGIC_EXTRAS_REQUIRES"] = "jupyter-basic"
 
-_STATIC_ATTRIBS = list(locals().keys())
-
-_DEFAULT_IMPORTS = {
-    "az_connect": "msticpy.auth.azure_auth",
-    "current_providers": "msticpy.init.nbinit",
-    "ContextLookup": "msticpy.context.contextlookup",
-    "GeoLiteLookup": "msticpy.context.geoip",
-    "init_notebook": "msticpy.init.nbinit",
-    "reset_ipython_exception_handler": "msticpy.init.nbinit",
-    "MicrosoftSentinel": "msticpy.context.azure",
-    "MpConfigEdit": "msticpy.config.mp_config_edit",
-    "MpConfigFile": "msticpy.config.mp_config_file",
-    "QueryProvider": "msticpy.data",
-    "TILookup": "msticpy.context.tilookup",
-    "TimeSpan": "msticpy.common.timespan",
-    "WorkspaceConfig": "msticpy.common.wsconfig",
-    "entities": "msticpy.datamodel",
-    "Pivot": "msticpy.init.pivot",
+_LAZY_IMPORTS = {
+    "msticpy.auth.azure_auth.az_connect",
+    "msticpy.common.timespan.TimeSpan",
+    "msticpy.common.wsconfig.WorkspaceConfig",
+    "msticpy.config.mp_config_edit.MpConfigEdit",
+    "msticpy.config.mp_config_file.MpConfigFile",
+    "msticpy.context.azure.MicrosoftSentinel",
+    "msticpy.context.contextlookup.ContextLookup",
+    "msticpy.context.geoip.GeoLiteLookup",
+    "msticpy.context.tilookup.TILookup",
+    "msticpy.data.QueryProvider",
+    "msticpy.datamodel.entities",
+    "msticpy.init.nbinit.current_providers",
+    "msticpy.init.nbinit.init_notebook",
+    "msticpy.init.nbinit.reset_ipython_exception_handler",
+    "msticpy.init.pivot.Pivot",
 }
 
-
-def __getattr__(attrib: str) -> Any:
-    """
-    Import and return an attribute of MSTICPy.
-
-    Parameters
-    ----------
-    attrib : str
-        The attribute name
-
-    Returns
-    -------
-    Any
-        The attribute value.
-
-    Raises
-    ------
-    AttributeError
-        No attribute found.
-
-    """
-    if attrib in _DEFAULT_IMPORTS:
-        try:
-            return getattr(importlib.import_module(_DEFAULT_IMPORTS[attrib]), attrib)
-        except (MsticpyImportExtraError, MsticpyImportExtraError):
-            raise
-        except (ImportError, MsticpyException) as err:
-            warnings.warn(f"Unable to import module for 'msticpy.{attrib}'")
-            print(
-                f"WARNING. The msticpy attribute '{attrib}' is not loadable.",
-                "You may need to install one or more additional dependencies.\n",
-                "Please check the exception details below for more information.",
-                "\n".join(
-                    traceback.format_exception(
-                        type(err), value=err, tb=err.__traceback__
-                    )
-                ),
-            )
-            raise AttributeError(f"msticpy failed to load '{attrib}'") from err
-    raise AttributeError(f"msticpy has no attribute '{attrib}'")
-
-
-def __dir__():
-    """Return attribute list."""
-    return sorted(set(_STATIC_ATTRIBS + list(_DEFAULT_IMPORTS)))
+module, __getattr__, __dir__ = lazy_import(__name__, _LAZY_IMPORTS)
 
 
 def load_plugins(plugin_paths: Union[str, Iterable[str]]):
     """
     Load plugins from specified paths or configuration.
 
     Parameters
```

### Comparing `msticpy-2.8.0rc1/msticpy/analysis/__init__.py` & `msticpy-2.9.0/msticpy/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/analysis/anomalous_sequence/anomalous.py` & `msticpy-2.9.0/msticpy/analysis/anomalous_sequence/anomalous.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/analysis/anomalous_sequence/model.py` & `msticpy-2.9.0/msticpy/analysis/anomalous_sequence/model.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/analysis/anomalous_sequence/sessionize.py` & `msticpy-2.9.0/msticpy/analysis/anomalous_sequence/sessionize.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/analysis/anomalous_sequence/utils/cmds_only.py` & `msticpy-2.9.0/msticpy/analysis/anomalous_sequence/utils/cmds_only.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/analysis/anomalous_sequence/utils/cmds_params_only.py` & `msticpy-2.9.0/msticpy/analysis/anomalous_sequence/utils/cmds_params_only.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/analysis/anomalous_sequence/utils/cmds_params_values.py` & `msticpy-2.9.0/msticpy/analysis/anomalous_sequence/utils/cmds_params_values.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/analysis/anomalous_sequence/utils/data_structures.py` & `msticpy-2.9.0/msticpy/analysis/anomalous_sequence/utils/data_structures.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/analysis/anomalous_sequence/utils/laplace_smooth.py` & `msticpy-2.9.0/msticpy/analysis/anomalous_sequence/utils/laplace_smooth.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/analysis/anomalous_sequence/utils/probabilities.py` & `msticpy-2.9.0/msticpy/analysis/anomalous_sequence/utils/probabilities.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/analysis/cluster_auditd.py` & `msticpy-2.9.0/msticpy/analysis/cluster_auditd.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/analysis/code_cleanup.py` & `msticpy-2.9.0/msticpy/analysis/code_cleanup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/analysis/eventcluster.py` & `msticpy-2.9.0/msticpy/analysis/eventcluster.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/analysis/observationlist.py` & `msticpy-2.9.0/msticpy/analysis/observationlist.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
         Returns
         -------
         Set[str]
             Set of all field names.
 
         """
-        return {field.name for field in attr.fields(cls)}
+        return {field.name for field in attr.fields(cls)}  # type: ignore[misc]
 
     def display(self):
         """Display the observation."""
         display(Markdown(f"### {self.caption}"))
         if self.description:
             display(Markdown(self.description))
         if self.score:
```

### Comparing `msticpy-2.8.0rc1/msticpy/analysis/outliers.py` & `msticpy-2.9.0/msticpy/analysis/outliers.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/analysis/polling_detection.py` & `msticpy-2.9.0/msticpy/analysis/polling_detection.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/analysis/syslog_utils.py` & `msticpy-2.9.0/msticpy/analysis/syslog_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/analysis/timeseries.py` & `msticpy-2.9.0/msticpy/analysis/timeseries.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/auth/__init__.py` & `msticpy-2.9.0/msticpy/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/auth/azure_auth.py` & `msticpy-2.9.0/msticpy/auth/azure_auth.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/auth/azure_auth_core.py` & `msticpy-2.9.0/msticpy/auth/azure_auth_core.py`

 * *Files 22% similar despite different names*

```diff
@@ -54,28 +54,65 @@
 
     AZURE_CLIENT_ID = "AZURE_CLIENT_ID"  # The app ID for the service principal
     AZURE_TENANT_ID = "AZURE_TENANT_ID"  # The service principal's Azure AD tenant ID
     # pylint: disable=line-too-long
     # [SuppressMessage("Microsoft.Security", "CS002:SecretInNextLine", Justification="This is an enum of env variable names")]
     AZURE_CLIENT_SECRET = "AZURE_CLIENT_SECRET"  # nosec  # noqa
 
+    # Certificate auth:
+    # A path to certificate and private key pair in PEM or PFX format
+    AZURE_CLIENT_CERTIFICATE_PATH = "AZURE_CLIENT_CERTIFICATE_PATH"
+    # (Optional) The password protecting the certificate file
+    # (for PFX (PKCS12) certificates).
+    AZURE_CLIENT_CERTIFICATE_PASSWORD = (
+        "AZURE_CLIENT_CERTIFICATE_PASSWORD"  # nosec  # noqa
+    )
+    # (Optional) Specifies whether an authentication request will include an x5c
+    # header to support subject name / issuer based authentication.
+    # When set to `true` or `1`, authentication requests include the x5c header.
+    AZURE_CLIENT_SEND_CERTIFICATE_CHAIN = "AZURE_CLIENT_SEND_CERTIFICATE_CHAIN"
+
+    # Username and password:
+    AZURE_USERNAME = "AZURE_USERNAME"  # The username/upn of an AAD user account.
+    # [SuppressMessage("Microsoft.Security", "CS002:SecretInNextLine", Justification="This is an enum of env variable names")]
+    AZURE_PASSWORD = "AZURE_PASSWORD"  # User password  # nosec  # noqa
+
+
+_VALID_ENV_VAR_COMBOS = (
+    (
+        AzureCredEnvNames.AZURE_CLIENT_ID,
+        AzureCredEnvNames.AZURE_CLIENT_SECRET,
+        AzureCredEnvNames.AZURE_TENANT_ID,
+    ),
+    (
+        AzureCredEnvNames.AZURE_CLIENT_ID,
+        AzureCredEnvNames.AZURE_TENANT_ID,
+        AzureCredEnvNames.AZURE_CLIENT_CERTIFICATE_PATH,
+    ),
+    (
+        AzureCredEnvNames.AZURE_CLIENT_ID,
+        AzureCredEnvNames.AZURE_USERNAME,
+        AzureCredEnvNames.AZURE_PASSWORD,
+        AzureCredEnvNames.AZURE_TENANT_ID,
+    ),
+)
+
 
 def _build_env_client(
     aad_uri: Optional[str] = None, **kwargs
 ) -> Optional[EnvironmentCredential]:
     """Build a credential from environment variables."""
     del kwargs
-    if (
-        AzureCredEnvNames.AZURE_CLIENT_ID not in os.environ
-        and AzureCredEnvNames.AZURE_CLIENT_SECRET not in os.environ
-    ):
-        # avoid creating env credential if require envs not set.
-        logger.info("'env' credential requested but required env vars not set")
-        return None
-    return EnvironmentCredential(authority=aad_uri)  # type: ignore
+    for env_vars in _VALID_ENV_VAR_COMBOS:
+        if all(var in os.environ for var in env_vars):
+            return EnvironmentCredential(authority=aad_uri)  # type: ignore
+
+    # avoid creating env credential if require envs not set.
+    logger.info("'env' credential requested but required env vars not set")
+    return None
 
 
 def _build_cli_client(**kwargs) -> AzureCliCredential:
     """Build a credential from Azure CLI."""
     del kwargs
     return AzureCliCredential()
```

### Comparing `msticpy-2.8.0rc1/msticpy/auth/cloud_mappings.py` & `msticpy-2.9.0/msticpy/auth/cloud_mappings.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/auth/cloud_mappings_offline.py` & `msticpy-2.9.0/msticpy/auth/cloud_mappings_offline.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/auth/cred_wrapper.py` & `msticpy-2.9.0/msticpy/auth/cred_wrapper.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/auth/keyring_client.py` & `msticpy-2.9.0/msticpy/auth/keyring_client.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/auth/keyvault_client.py` & `msticpy-2.9.0/msticpy/auth/keyvault_client.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/auth/keyvault_settings.py` & `msticpy-2.9.0/msticpy/auth/keyvault_settings.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/auth/msal_auth.py` & `msticpy-2.9.0/msticpy/auth/msal_auth.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/auth/secret_settings.py` & `msticpy-2.9.0/msticpy/auth/secret_settings.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/common/__init__.py` & `msticpy-2.9.0/msticpy/common/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/common/azure_auth.py` & `msticpy-2.9.0/msticpy/common/azure_auth.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/common/check_version.py` & `msticpy-2.9.0/msticpy/common/check_version.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/common/data_types.py` & `msticpy-2.9.0/msticpy/data/core/query_container.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,78 +1,36 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
-"""Object container class."""
-from typing import Any, Dict, Optional, Type
+"""Query hierarchy attribute class."""
+from functools import partial
 
-from .._version import VERSION
-from ..common.utility import check_kwarg
+from ..._version import VERSION
+from ...common.data_types import ObjectContainer
 
 __version__ = VERSION
 __author__ = "Ian Hellen"
 
 
-class ObjectContainer:
+class QueryContainer(ObjectContainer):
     """Empty class used to create hierarchical attributes."""
 
-    _subclasses: Dict[str, Type] = {}
-
-    def __len__(self):
-        """Return number of items in the attribute collection."""
-        return len(self.__dict__)
-
-    def __iter__(self):
-        """Return iterator over the attributes."""
-        return iter(self.__dict__.items())
-
-    def __getattr__(self, name):
-        """Print usable error message if attribute not found."""
-        if "." in name:
-            try:
-                attr = _get_dot_attrib(self, name)
-            except KeyError:
-                pass
-            else:
-                return attr
-        nm_err: Optional[Exception] = None
-        try:
-            # check for similar-named attributes in __dict__
-            check_kwarg(name, list(self.__dict__.keys()))
-        except NameError as err:
-            nm_err = err
-        if nm_err:
-            raise AttributeError(
-                f"{self.__class__.__name__} object has no attribute {name}"
-            ) from nm_err
-        raise AttributeError(
-            f"{self.__class__.__name__} object has no attribute {name}"
-        )
-
     def __repr__(self):
         """Return list of attributes."""
         repr_list = []
         for name, obj in self.__dict__.items():
-            if isinstance(obj, ObjectContainer):
+            if isinstance(obj, QueryContainer):
                 repr_list.append(f"{name} (container)")
+            elif isinstance(obj, partial):
+                repr_list.append(f"{name} (query)")
             elif not name.startswith("_"):
                 repr_list.append(f"{name} {type(obj).__name__}")
         return "\n".join(repr_list)
 
     def __call__(self, *args, **kwargs):
         """Return list of attributes or help."""
         if args or kwargs:
-            print("This attribute is a container, not a function.")
+            print("This attribute is a container, not a query.")
             print("Items in this container:")
         print(repr(self))
-
-
-def _get_dot_attrib(obj, elem_path: str) -> Any:
-    """Return attribute at dotted path."""
-    path_elems = elem_path.split(".")
-    cur_node = obj
-    for elem in path_elems:
-        cur_node = getattr(cur_node, elem, None)
-        if cur_node is None:
-            raise KeyError(f"{elem} value of {elem_path} is not a valid path")
-    return cur_node
```

### Comparing `msticpy-2.8.0rc1/msticpy/common/data_utils.py` & `msticpy-2.9.0/msticpy/common/data_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/common/exceptions.py` & `msticpy-2.9.0/msticpy/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/common/pkg_config.py` & `msticpy-2.9.0/msticpy/common/pkg_config.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/common/provider_settings.py` & `msticpy-2.9.0/msticpy/common/provider_settings.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/common/proxy_settings.py` & `msticpy-2.9.0/msticpy/common/proxy_settings.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/common/settings.py` & `msticpy-2.9.0/msticpy/common/settings.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/common/timespan.py` & `msticpy-2.9.0/msticpy/common/timespan.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/common/utility/__init__.py` & `msticpy-2.9.0/msticpy/common/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/common/utility/format.py` & `msticpy-2.9.0/msticpy/common/utility/format.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/common/utility/ipython.py` & `msticpy-2.9.0/msticpy/common/utility/ipython.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/common/utility/package.py` & `msticpy-2.9.0/msticpy/common/utility/package.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,15 +319,15 @@
 
 
 def init_dir(static_attribs: List[str], dynamic_imports: Dict[str, str]):
     """Return list of available attributes."""
     return sorted(set(static_attribs + list(dynamic_imports)))
 
 
-def lazy_import(module: str, attrib: str, call: bool = False):
+def delayed_import(module: str, attrib: str, call: bool = False):
     """Import attribute from module on demand."""
     attribute = None
 
     def import_item(*args, **kwargs):
         """Return the attribute, importing module if needed."""
         nonlocal attribute
         if attribute is None:
```

### Comparing `msticpy-2.8.0rc1/msticpy/common/utility/types.py` & `msticpy-2.9.0/msticpy/common/utility/types.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/common/wsconfig.py` & `msticpy-2.9.0/msticpy/common/wsconfig.py`

 * *Files 6% similar despite different names*

```diff
@@ -244,25 +244,42 @@
                 cls.CONF_RES_GROUP_KEY: settings.get(cls.PKG_CONF_RES_GROUP_KEY),  # type: ignore
             }
         )
 
     @classmethod
     def from_connection_string(cls, connection_str: str) -> "WorkspaceConfig":
         """Create a WorkstationConfig from a connection string."""
-        tenant_regex = r".*tenant\(\s?['\"](?P<tenant_id>[\w]+)['\"].*"
-        workspace_regex = r".*workspace\(\s?['\"](?P<workspace_id>[\w]+)['\"].*"
-        tenant_id = workspace_id = None
-        if match := re.match(tenant_regex, connection_str):
+        tenant_regex = r"""
+        .*tenant\s?=\s?['\"]\{?
+        (?P<tenant_id>[0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12})
+        \}?['\"].*"""
+        workspace_regex = r"""
+        .*workspace\s?=\s?['\"]\{?
+        (?P<workspace_id>[0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12})
+        \}?['\"].*"""
+        ws_name_regex = r".*alias\s?=\s?['\"]\{?(?P<workspace_name>\w+)['\"].*"
+
+        tenant_id = workspace_id = workspace_name = None
+        if match := re.match(tenant_regex, connection_str, re.IGNORECASE | re.VERBOSE):
             tenant_id = match.groupdict()["tenant_id"]
-        if match := re.match(workspace_regex, connection_str):
+        else:
+            raise ValueError("Could not find tenant ID in connection string.")
+        if match := re.match(
+            workspace_regex, connection_str, re.IGNORECASE | re.VERBOSE
+        ):
             workspace_id = match.groupdict()["workspace_id"]
+        else:
+            raise ValueError("Could not find workspace ID in connection string.")
+        if match := re.match(ws_name_regex, connection_str, re.IGNORECASE | re.VERBOSE):
+            workspace_name = match.groupdict()["workspace_name"]
         return cls(
             config={
                 cls.CONF_WS_ID_KEY: workspace_id,  # type: ignore[dict-item]
                 cls.CONF_TENANT_ID_KEY: tenant_id,  # type: ignore[dict-item]
+                cls.CONF_WS_NAME_KEY: workspace_name,  # type: ignore[dict-item]
             }
         )
 
     @staticmethod
     def _read_config_values(file_path: str) -> Dict[str, str]:
         """Read configuration file."""
         if not file_path:
```

### Comparing `msticpy-2.8.0rc1/msticpy/config/ce_azure.py` & `msticpy-2.9.0/msticpy/config/ce_azure.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/config/ce_azure_sentinel.py` & `msticpy-2.9.0/msticpy/config/ce_azure_sentinel.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 # --------------------------------------------------------------------------
 """Module docstring."""
 from datetime import datetime
 
 import ipywidgets as widgets
 
 from .._version import VERSION
-from ..common.utility.package import lazy_import
+from ..common.utility.package import delayed_import
 
 # from ..context.azure.sentinel_core import MicrosoftSentinel
 from .ce_common import (
     ITEM_LIST_LAYOUT,
     get_or_create_mpc_section,
     get_wgt_ctrl,
     print_debug,
 )
 from .comp_edit import CEItemsBase, CompEditDisplayMixin
 from .mp_config_control import MpConfigControls
 
 __version__ = VERSION
 __author__ = "Ian Hellen"
 
-ms_sentinel = lazy_import("msticpy.context.azure.sentinel_core", "MicrosoftSentinel")
+ms_sentinel = delayed_import("msticpy.context.azure.sentinel_core", "MicrosoftSentinel")
 
 
 # pylint: disable=too-many-ancestors
 class CEAzureSentinel(CEItemsBase):
     """Microsoft Sentinel Workspaces editor component."""
 
     _DESCRIPTION = "Microsoft Sentinel workspace settings"
```

### Comparing `msticpy-2.8.0rc1/msticpy/config/ce_common.py` & `msticpy-2.9.0/msticpy/config/ce_common.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/config/ce_data_providers.py` & `msticpy-2.9.0/msticpy/config/ce_data_providers.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/config/ce_keyvault.py` & `msticpy-2.9.0/msticpy/config/ce_keyvault.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/config/ce_msticpy.py` & `msticpy-2.9.0/msticpy/config/ce_msticpy.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/config/ce_other_providers.py` & `msticpy-2.9.0/msticpy/config/ce_other_providers.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/config/ce_provider_base.py` & `msticpy-2.9.0/msticpy/config/ce_provider_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/config/ce_simple_settings.py` & `msticpy-2.9.0/msticpy/config/ce_simple_settings.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/config/ce_ti_providers.py` & `msticpy-2.9.0/msticpy/config/ce_ti_providers.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/config/ce_user_defaults.py` & `msticpy-2.9.0/msticpy/config/ce_user_defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,16 @@
         Parameters
         ----------
         mp_controls : MpConfigControls
             The config/controls/settings database
 
         """
         super().__init__(mp_controls)
-        from ..data import DataEnvironment  # pylint: disable=import-outside-toplevel
+        # pylint: disable=import-outside-toplevel
+        from ..data.core.query_defns import DataEnvironment
 
         self._data_env_enum = DataEnvironment
 
         get_or_create_mpc_section(self.mp_controls, self._COMP_PATH)
         self.select_item.options = self._get_select_opts()
         self.select_item.layout = ITEM_LIST_LAYOUT["layout"]
         self.select_item.style = ITEM_LIST_LAYOUT["style"]
```

### Comparing `msticpy-2.8.0rc1/msticpy/config/comp_edit.py` & `msticpy-2.9.0/msticpy/config/comp_edit.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/config/compound_ctrls.py` & `msticpy-2.9.0/msticpy/config/compound_ctrls.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/config/file_browser.py` & `msticpy-2.9.0/msticpy/config/file_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/config/mp_config_control.py` & `msticpy-2.9.0/msticpy/config/mp_config_control.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/config/mp_config_edit.py` & `msticpy-2.9.0/msticpy/config/mp_config_edit.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/config/mp_config_file.py` & `msticpy-2.9.0/msticpy/config/mp_config_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,24 +21,21 @@
 try:
     from ..auth.keyvault_client import BHKeyVaultClient, MsticpyKeyVaultConfigError
 
     _KEYVAULT = True
 except ImportError:
     _KEYVAULT = False
 
-try:
-    from ..context.azure.sentinel_core import MicrosoftSentinel
-
-    _SENTINEL = True
-except ImportError:
-    _SENTINEL = False
 from ..common.pkg_config import current_config_path, refresh_config, validate_config
+from ..common.utility.package import delayed_import
 from .comp_edit import CompEditDisplayMixin, CompEditStatusMixin
 from .file_browser import FileBrowser
 
+ms_sentinel = delayed_import("msticpy.context.azure.sentinel_core", "MicrosoftSentinel")
+
 __version__ = VERSION
 __author__ = "Ian Hellen"
 
 
 _CONFIG_MAP = {
     "resource_group": "ResourceGroup",
     "subscription_id": "SubscriptionId",
@@ -302,15 +299,15 @@
         -------
         Dict[str, Dict[str, str]]
             Dictionary with a single element keyed by workspace name
             The value is the workspace settings dictionary for the
             workspace.
 
         """
-        return MicrosoftSentinel.get_workspace_details_from_url(url)
+        return ms_sentinel().get_workspace_details_from_url(url)
 
     def _show_sentinel_workspace(self, show: bool = True):
         """Fetch settings from Sentinel Portal URL."""
         if not self._txt_import_url.value:
             return
         self._last_workspace = self.get_workspace_from_url(self._txt_import_url.value)
         workspace_settings = pprint.pformat(self._last_workspace, compact=True)
```

### Comparing `msticpy-2.8.0rc1/msticpy/config/query_editor.py` & `msticpy-2.9.0/msticpy/config/query_editor.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/__init__.py` & `msticpy-2.9.0/msticpy/context/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,21 +2,28 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 """Context Providers Subpackage."""
 from typing import Any
 
-# flake8: noqa: F403
 from ..common.utility import ImportPlaceholder
-from .geoip import GeoLiteLookup, IPStackLookup
-from .tilookup import TILookup
+from ..lazy_importer import lazy_import
 from .vtlookupv3 import VT3_AVAILABLE
 
 vtlookupv3: Any
 if VT3_AVAILABLE:
     from .vtlookupv3 import vtlookupv3
 else:
     # vtlookup3 will not load if vt package not installed
     vtlookupv3 = ImportPlaceholder(  # type: ignore
         "vtlookupv3", ["vt-py", "vt-graph-api", "nest_asyncio"]
     )
+
+
+_LAZY_IMPORTS = {
+    "msticpy.context.geoip.GeoLiteLookup",
+    "msticpy.context.geoip.IPStackLookup",
+    "msticpy.context.tilookup.TILookup",
+}
+
+module, __getattr__, __dir__ = lazy_import(__name__, _LAZY_IMPORTS)
```

### Comparing `msticpy-2.8.0rc1/msticpy/context/azure/azure_data.py` & `msticpy-2.9.0/msticpy/context/azure/azure_data.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/azure/sentinel_analytics.py` & `msticpy-2.9.0/msticpy/context/azure/sentinel_analytics.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/azure/sentinel_bookmarks.py` & `msticpy-2.9.0/msticpy/context/azure/sentinel_bookmarks.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/azure/sentinel_core.py` & `msticpy-2.9.0/msticpy/context/azure/sentinel_core.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/azure/sentinel_dynamic_summary.py` & `msticpy-2.9.0/msticpy/context/azure/sentinel_dynamic_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import httpx
 import pandas as pd
 
 from ..._version import VERSION
 from ...common.exceptions import MsticpyAzureConnectionError, MsticpyParameterError
 from ...common.pkg_config import get_config, get_http_timeout
-from ...data import QueryProvider
+from ...data.core.data_providers import QueryProvider
 from .azure_data import get_api_headers
 
 # pylint: disable=unused-import
 from .sentinel_dynamic_summary_types import (  # noqa: F401
     DynamicSummary,
     DynamicSummaryItem,
     df_to_dynamic_summary,
```

### Comparing `msticpy-2.8.0rc1/msticpy/context/azure/sentinel_dynamic_summary_types.py` & `msticpy-2.9.0/msticpy/context/azure/sentinel_dynamic_summary_types.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/azure/sentinel_incidents.py` & `msticpy-2.9.0/msticpy/context/azure/sentinel_incidents.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/azure/sentinel_search.py` & `msticpy-2.9.0/msticpy/context/azure/sentinel_search.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/azure/sentinel_ti.py` & `msticpy-2.9.0/msticpy/context/azure/sentinel_ti.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/azure/sentinel_utils.py` & `msticpy-2.9.0/msticpy/context/azure/sentinel_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/azure/sentinel_watchlists.py` & `msticpy-2.9.0/msticpy/context/azure/sentinel_watchlists.py`

 * *Files 2% similar despite different names*

```diff
@@ -324,9 +324,11 @@
         Returns
         -------
         bool
             Whether the Watchlist exists or not.
 
         """
         # Check requested watchlist actually exists
-        existing_watchlists = self.list_watchlists()["name"].values
-        return watchlist_name in existing_watchlists
+        existing_watchlists = self.list_watchlists()
+        if existing_watchlists.empty:
+            return False
+        return watchlist_name in existing_watchlists["name"].values
```

### Comparing `msticpy-2.8.0rc1/msticpy/context/azure/sentinel_workspaces.py` & `msticpy-2.9.0/msticpy/context/azure/sentinel_workspaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from msrestazure import tools as az_tools
 
 from ..._version import VERSION
 from ...auth.azure_auth_core import AzureCloudConfig
 from ...common.data_utils import df_has_data
 from ...common.pkg_config import get_http_timeout
 from ...common.utility import mp_ua_header
-from ...data import QueryProvider
+from ...data.core.data_providers import QueryProvider
 
 __version__ = VERSION
 __author__ = "Ian Hellen"
 
 ParsedUrlComponents = namedtuple(
     "ParsedUrlComponents",
     "domain, resource_id, tenant_name, res_components, raw_res_id",
```

### Comparing `msticpy-2.8.0rc1/msticpy/context/contextlookup.py` & `msticpy-2.9.0/msticpy/context/contextlookup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/contextproviders/context_provider_base.py` & `msticpy-2.9.0/msticpy/context/contextproviders/context_provider_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/contextproviders/http_context_provider.py` & `msticpy-2.9.0/msticpy/context/contextproviders/http_context_provider.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/contextproviders/servicenow.py` & `msticpy-2.9.0/msticpy/context/contextproviders/servicenow.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/domain_utils.py` & `msticpy-2.9.0/msticpy/context/domain_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 Includes functions to conduct common investigation steps when dealing
 with a domain or url, such as getting a screenshot or validating the TLD.
 
 """
 import json
 import ssl
 import time
+from dataclasses import asdict
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, Optional, Tuple
 from urllib.error import HTTPError, URLError
 
 import cryptography as crypto
 import httpx
@@ -257,15 +258,18 @@
 
     Returns
     -------
     dict:
         Returns subdomain and TLD components from a domain.
 
     """
-    return tldextract.extract(domain.lower())._asdict()
+    result = tldextract.extract(domain.lower())
+    if isinstance(result, tuple):
+        return result._asdict()  # type: ignore
+    return asdict(result)
 
 
 def url_components(url: str) -> Dict[str, str]:
     """Return parsed Url components as dict."""
     try:
         return parse_url(url)._asdict()
     except LocationParseError:
```

### Comparing `msticpy-2.8.0rc1/msticpy/context/geoip.py` & `msticpy-2.9.0/msticpy/context/geoip.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/http_provider.py` & `msticpy-2.9.0/msticpy/context/http_provider.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/ip_utils.py` & `msticpy-2.9.0/msticpy/context/ip_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/lookup.py` & `msticpy-2.9.0/msticpy/context/lookup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/lookup_result.py` & `msticpy-2.9.0/msticpy/context/lookup_result.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/preprocess_observable.py` & `msticpy-2.9.0/msticpy/context/preprocess_observable.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/provider_base.py` & `msticpy-2.9.0/msticpy/context/provider_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/tilookup.py` & `msticpy-2.9.0/msticpy/context/tilookup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/tiproviders/abuseipdb.py` & `msticpy-2.9.0/msticpy/context/tiproviders/abuseipdb.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/tiproviders/alienvault_otx.py` & `msticpy-2.9.0/msticpy/context/tiproviders/alienvault_otx.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/tiproviders/azure_sent_byoti.py` & `msticpy-2.9.0/msticpy/context/tiproviders/azure_sent_byoti.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/tiproviders/crowdsec.py` & `msticpy-2.9.0/msticpy/context/tiproviders/crowdsec.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/tiproviders/greynoise.py` & `msticpy-2.9.0/msticpy/context/tiproviders/greynoise.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/tiproviders/ibm_xforce.py` & `msticpy-2.9.0/msticpy/context/tiproviders/ibm_xforce.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/tiproviders/intsights.py` & `msticpy-2.9.0/msticpy/context/tiproviders/intsights.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,50 +42,50 @@
 class IntSights(HttpTIProvider):
     """IntSights Lookup."""
 
     _BASE_URL = "https://api.ti.insight.rapid7.com"
 
     _QUERIES = {
         "ipv4": _IntSightsParams(
-            path="/public/v2/iocs/ioc-by-value",
+            path="/public/v3/iocs/ioc-by-value",
             params={"iocValue": "{observable}"},
             headers=_DEF_HEADERS,
         ),
         "ipv6": _IntSightsParams(
-            path="/public/v2/iocs/ioc-by-value",
+            path="/public/v3/iocs/ioc-by-value",
             params={"iocValue": "{observable}"},
             headers=_DEF_HEADERS,
         ),
         "dns": _IntSightsParams(
-            path="/public/v2/iocs/ioc-by-value",
+            path="/public/v3/iocs/ioc-by-value",
             params={"iocValue": "{observable}"},
             headers=_DEF_HEADERS,
         ),
         "url": _IntSightsParams(
-            path="/public/v2/iocs/ioc-by-value",
+            path="/public/v3/iocs/ioc-by-value",
             params={"iocValue": "{observable}"},
             headers=_DEF_HEADERS,
         ),
         "md5_hash": _IntSightsParams(
-            path="/public/v2/iocs/ioc-by-value",
+            path="/public/v3/iocs/ioc-by-value",
             params={"iocValue": "{observable}"},
             headers=_DEF_HEADERS,
         ),
         "sha1_hash": _IntSightsParams(
-            path="/public/v2/iocs/ioc-by-value",
+            path="/public/v3/iocs/ioc-by-value",
             params={"iocValue": "{observable}"},
             headers=_DEF_HEADERS,
         ),
         "sha256_hash": _IntSightsParams(
-            path="/public/v2/iocs/ioc-by-value",
+            path="/public/v3/iocs/ioc-by-value",
             params={"iocValue": "{observable}"},
             headers=_DEF_HEADERS,
         ),
         "email": _IntSightsParams(
-            path="/public/v2/iocs/ioc-by-value",
+            path="/public/v3/iocs/ioc-by-value",
             params={"iocValue": "{observable}"},
             headers=_DEF_HEADERS,
         ),
     }
 
     _REQUIRED_PARAMS = ["ApiID", "AuthKey"]
 
@@ -107,35 +107,36 @@
 
         """
         if self._failed_response(response) or not isinstance(
             response["RawResult"], dict
         ):
             return False, ResultSeverity.information, "Not found."
 
-        if response["RawResult"]["Whitelist"] == "True":
+        if response["RawResult"].get("whitelisted", False):
             return False, ResultSeverity.information, "Whitelisted."
 
-        sev = response["RawResult"]["Severity"]
+        sev = response["RawResult"].get("severity", "Low")
         result_dict = {
-            "threat_actors": response["RawResult"]["RelatedThreatActors"],
-            "geolocation": response["RawResult"].get("Geolocation", ""),
+            "threat_actors": response["RawResult"].get("relatedThreatActors", ""),
+            "geolocation": response["RawResult"].get("geolocation", None),
             "response_code": response["Status"],
-            "tags": response["RawResult"]["Tags"] + response["RawResult"]["SystemTags"],
-            "malware": response["RawResult"]["RelatedMalware"],
-            "campaigns": response["RawResult"]["RelatedCampaigns"],
-            "sources": response["RawResult"]["Sources"],
-            "score": response["RawResult"]["Score"],
+            "tags": response["RawResult"].get("tags", [])
+            + response["RawResult"].get("SystemTags", []),
+            "malware": response["RawResult"].get("relatedMalware", []),
+            "campaigns": response["RawResult"].get("relatedCampaigns", []),
+            "score": response["RawResult"].get("score", 0),
             "first_seen": dt.datetime.strptime(
-                response["RawResult"]["FirstSeen"], "%Y-%m-%dT%H:%M:%S.%fZ"
+                response["RawResult"].get("firstSeen", None), "%Y-%m-%dT%H:%M:%S.%fZ"
             ),
             "last_seen": dt.datetime.strptime(
-                response["RawResult"]["LastSeen"], "%Y-%m-%dT%H:%M:%S.%fZ"
+                response["RawResult"].get("lastSeen", None), "%Y-%m-%dT%H:%M:%S.%fZ"
             ),
             "last_update": dt.datetime.strptime(
-                response["RawResult"]["LastUpdate"], "%Y-%m-%dT%H:%M:%S.%fZ"
+                response["RawResult"].get("lastUpdateDate", None),
+                "%Y-%m-%dT%H:%M:%S.%fZ",
             ),
         }
 
         severity = (
             ResultSeverity.information
             if sev == "Low"
             else ResultSeverity.warning
```

### Comparing `msticpy-2.8.0rc1/msticpy/context/tiproviders/kql_base.py` & `msticpy-2.9.0/msticpy/context/tiproviders/kql_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 import pandas as pd
 
 from ..._version import VERSION
 from ...common.exceptions import MsticpyConfigError
 from ...common.utility import export
 from ...common.wsconfig import WorkspaceConfig
-from ...data import QueryProvider
+from ...data.core.data_providers import QueryProvider
 from ..lookup_result import LookupStatus
 from ..provider_base import generate_items
 from .ti_provider_base import ResultSeverity, TIProvider
 
 __version__ = VERSION
 __author__ = "Ian Hellen"
```

### Comparing `msticpy-2.8.0rc1/msticpy/context/tiproviders/mblookup.py` & `msticpy-2.9.0/msticpy/context/tiproviders/mblookup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/tiproviders/open_page_rank.py` & `msticpy-2.9.0/msticpy/context/tiproviders/open_page_rank.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,19 @@
 
 __version__ = VERSION
 __author__ = "Ian Hellen"
 
 
 @export
 class OPR(HttpTIProvider):
-    """Open PageRank Lookup."""
+    """
+    Open PageRank Lookup.
+
+    See https://www.domcop.com/openpagerank/what-is-openpagerank
+    """
 
     _BASE_URL = "https://openpagerank.com"
 
     _QUERIES = {
         "dns": APILookupParams(
             path="/api/v1.0/getPageRank",
             params={"domains[0]": "{observable}"},
@@ -46,18 +50,14 @@
     _REQUIRED_PARAMS = ["AuthKey"]
 
     def __init__(self, **kwargs):
         """Initialize a new instance of the class."""
         super().__init__(**kwargs)
 
         self._provider_name = self.__class__.__name__
-        print(
-            "Using Open PageRank.",
-            "See https://www.domcop.com/openpagerank/what-is-openpagerank",
-        )
 
     async def lookup_iocs_async(
         self,
         data: Union[pd.DataFrame, Dict[str, str], Iterable[str]],
         ioc_col: str = None,
         ioc_type_col: str = None,
         query_type: str = None,
```

### Comparing `msticpy-2.8.0rc1/msticpy/context/tiproviders/pulsedive.py` & `msticpy-2.9.0/msticpy/context/tiproviders/pulsedive.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/tiproviders/result_severity.py` & `msticpy-2.9.0/msticpy/context/tiproviders/result_severity.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/tiproviders/riskiq.py` & `msticpy-2.9.0/msticpy/context/tiproviders/riskiq.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/tiproviders/ti_http_provider.py` & `msticpy-2.9.0/msticpy/context/tiproviders/ti_http_provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,14 +83,18 @@
             verb, req_params = self._substitute_parms(
                 result["SafeIoc"], result["IocType"], query_type
             )
             if verb == "GET":
                 response = self._httpx_client.get(
                     **req_params, timeout=get_http_timeout(**kwargs)
                 )
+            elif verb == "POST":
+                response = self._httpx_client.post(
+                    **req_params, timeout=get_http_timeout(**kwargs)
+                )
             else:
                 raise NotImplementedError(f"Unsupported verb {verb}")
 
             result["Status"] = response.status_code
             result["Reference"] = req_params["url"]
             if result["Status"] == 200:
                 try:
```

### Comparing `msticpy-2.8.0rc1/msticpy/context/tiproviders/ti_provider_base.py` & `msticpy-2.9.0/msticpy/context/tiproviders/ti_provider_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/tiproviders/tor_exit_nodes.py` & `msticpy-2.9.0/msticpy/context/tiproviders/tor_exit_nodes.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/tiproviders/virustotal.py` & `msticpy-2.9.0/msticpy/context/tiproviders/virustotal.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/vtlookupv3/__init__.py` & `msticpy-2.9.0/msticpy/context/vtlookupv3/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/vtlookupv3/vtfile_behavior.py` & `msticpy-2.9.0/msticpy/context/vtlookupv3/vtfile_behavior.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/vtlookupv3/vtlookup.py` & `msticpy-2.9.0/msticpy/context/vtlookupv3/vtlookup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/context/vtlookupv3/vtlookupv3.py` & `msticpy-2.9.0/msticpy/context/vtlookupv3/vtlookupv3.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/__init__.py` & `msticpy-2.9.0/msticpy/data/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,14 +17,20 @@
 - core - core data query provider components
 - drivers - query provider interface drivers for external data sources.
 - queries - queries for core data providers
 - uploaders - loaders for some data services.
 
 """
 from .._version import VERSION
-from ..common.exceptions import MsticpyImportExtraError
 
-# flake8: noqa: F403
-from .core.data_providers import QueryProvider
-from .core.query_defns import DataEnvironment, DataFamily
+# from ..common.exceptions import MsticpyImportExtraError
+from ..lazy_importer import lazy_import
 
 __version__ = VERSION
+
+_LAZY_IMPORTS = {
+    "msticpy.data.core.data_providers.QueryProvider",
+    "msticpy.data.core.query_defns.DataEnvironment",
+    "msticpy.data.core.query_defns.DataFamily",
+}
+
+module, __getattr__, __dir__ = lazy_import(__name__, _LAZY_IMPORTS)
```

### Comparing `msticpy-2.8.0rc1/msticpy/data/azure/__init__.py` & `msticpy-2.9.0/msticpy/data/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/azure/azure_blob_storage.py` & `msticpy-2.9.0/msticpy/data/azure/azure_blob_storage.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/azure/azure_data.py` & `msticpy-2.9.0/msticpy/data/azure/azure_data.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/azure_blob_storage.py` & `msticpy-2.9.0/msticpy/data/azure_blob_storage.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/azure_data.py` & `msticpy-2.9.0/msticpy/data/azure_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 See :py:mod:`msticpy.context.azure.azure_data`
 """
 import warnings
 
 # flake8: noqa: F403, F401
 # pylint: disable=unused-import
-from ..context.azure import AzureData
+from ..context.azure.azure_data import AzureData
 
 WARN_MSSG = (
     "This module has moved to msticpy.context.azure.azure_data\n"
     "Please change your import to reflect this new location."
     "This will be removed in MSTICPy v2.2.0"
 )
 warnings.warn(WARN_MSSG, category=DeprecationWarning)
```

### Comparing `msticpy-2.8.0rc1/msticpy/data/azure_sentinel.py` & `msticpy-2.9.0/msticpy/data/azure_sentinel.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/core/data_providers.py` & `msticpy-2.9.0/msticpy/data/core/data_providers.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
 
 import pandas as pd
 
 from ..._version import VERSION
 from ...common.pkg_config import get_config
 from ...common.utility import export, valid_pyname
-from ...nbwidgets import QueryTime
+from ...nbwidgets.query_time import QueryTime
 from .. import drivers
 from ..drivers.driver_base import DriverBase, DriverProps
 from .param_extractor import extract_query_params
 from .query_container import QueryContainer
 from .query_defns import DataEnvironment
 from .query_provider_connections_mixin import QueryProviderConnectionsMixin
 from .query_provider_utils_mixin import QueryProviderUtilsMixin
```

### Comparing `msticpy-2.8.0rc1/msticpy/data/core/data_query_reader.py` & `msticpy-2.9.0/msticpy/data/core/data_query_reader.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/core/param_extractor.py` & `msticpy-2.9.0/msticpy/data/core/param_extractor.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/core/query_defns.py` & `msticpy-2.9.0/msticpy/data/core/query_defns.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     LogAnalytics = 1  # alias of MSSentinel
     MSSentinel_New = 1  # alias of MSSentinel
     Kusto = 2  # alias of Kusto
     AzureDataExplorer = 2  # alias of Kusto
     Kusto_New = 2  # alias of Kusto
     MSGraph = 4
     SecurityGraph = 4
+
     MDE = 5
     MDATP = 5  # alias of MDE
     LocalData = 6
     Splunk = 7
     OTRF = 8
     Mordor = 8
     ResourceGraph = 9
@@ -111,14 +112,15 @@
     OSQuery = 15
     MSSentinel_Legacy = 16
     MSSentinel_KQLM = 16
     Kusto_Legacy = 17
     Kusto_KQLM = 17
     VelociraptorLogs = 18
     Velociraptor = 18
+    M365DGraph = 20
 
     @classmethod
     def parse(cls, value: Union[str, int]) -> "DataEnvironment":
         """
         Convert string or int to enum.
 
         Parameters
```

### Comparing `msticpy-2.8.0rc1/msticpy/data/core/query_provider_connections_mixin.py` & `msticpy-2.9.0/msticpy/data/core/query_provider_connections_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,15 +347,16 @@
             for query_id, thread_task in ids_and_tasks.items():
                 try:
                     result = await thread_task
                     logger.info("Query task '%s' completed successfully.", query_id)
                     results.append(result)
                 except Exception:  # pylint: disable=broad-except
                     logger.warning(
-                        "Query task '%s' failed with exception", query_id, exc_info=True
+                        "Query task '%s' failed with exception",
+                        query_id,
                     )
                     failed_tasks[query_id] = thread_task
 
             if retry and failed_tasks:
                 for query_id, thread_task in failed_tasks.items():
                     try:
                         logger.info("Retrying query task '%s'", query_id)
```

### Comparing `msticpy-2.8.0rc1/msticpy/data/core/query_provider_utils_mixin.py` & `msticpy-2.9.0/msticpy/data/core/query_provider_utils_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 # --------------------------------------------------------------------------
 """Query Provider mixin methods."""
 import re
 from collections import abc
 from typing import Dict, Iterable, List, NamedTuple, Optional, Pattern, Protocol, Union
 
 from ..._version import VERSION
-from ...common.utility.package import lazy_import
+from ...common.utility.package import delayed_import
 from ..drivers.driver_base import DriverBase
 from .query_defns import DataEnvironment
 from .query_source import QuerySource
 from .query_store import QueryStore
 
 __version__ = VERSION
 __author__ = "Ian Hellen"
 
-query_browser = lazy_import("msticpy.vis.query_browser", "browse_queries")
+query_browser = delayed_import("msticpy.vis.query_browser", "browse_queries")
 
 
 # pylint: disable=too-few-public-methods
 class QueryProviderProtocol(Protocol):
     """Protocol for required properties of QueryProvider class."""
 
     _query_provider: DriverBase
```

### Comparing `msticpy-2.8.0rc1/msticpy/data/core/query_source.py` & `msticpy-2.9.0/msticpy/data/core/query_source.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/core/query_store.py` & `msticpy-2.9.0/msticpy/data/core/query_store.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/core/query_template.py` & `msticpy-2.9.0/msticpy/data/core/query_template.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/data_obfus.py` & `msticpy-2.9.0/msticpy/data/data_obfus.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/data_providers.py` & `msticpy-2.9.0/msticpy/data/data_providers.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/drivers/__init__.py` & `msticpy-2.9.0/msticpy/data/drivers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     DataEnvironment.Kusto_New: ("azure_kusto_driver", "AzureKustoDriver"),
     DataEnvironment.VelociraptorLogs: (
         "local_velociraptor_driver",
         "VelociraptorLogDriver",
     ),
     DataEnvironment.MSSentinel_Legacy: ("kql_driver", "KqlDriver"),
     DataEnvironment.Kusto_Legacy: ("kusto_driver", "KustoDriver"),
+    DataEnvironment.M365DGraph: ("mdatp_driver", "MDATPDriver"),
 }
 
 CUSTOM_PROVIDERS: Dict[str, type] = {}
 
 
 @singledispatch
 def import_driver(data_environment) -> type:
```

### Comparing `msticpy-2.8.0rc1/msticpy/data/drivers/azure_kusto_driver.py` & `msticpy-2.9.0/msticpy/data/drivers/azure_kusto_driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -442,18 +442,18 @@
             response = self.client.execute(  # type: ignore[union-attr]
                 database=database, query=query, properties=connection_props
             )
             data = dataframe_from_result_table(response.primary_results[0])
             status = _parse_query_status(response)
             logger.info("Query completed: %s", str(status))
         except KustoApiError as err:
-            logger.exception("Query failed: %s", err)
+            logger.error("Query failed: %s", err)
             _raise_kusto_error(err)
         except KustoServiceError as err:
-            logger.exception("Query failed: %s", err)
+            logger.error("Query failed: %s", err)
             _raise_unknown_query_error(err)
         return data, status
 
     def get_database_names(self) -> List[str]:
         """Get a list of database names from the connected cluster."""
         if self.client is None:
             _raise_not_connected_error()
```

### Comparing `msticpy-2.8.0rc1/msticpy/data/drivers/azure_monitor_driver.py` & `msticpy-2.9.0/msticpy/data/drivers/azure_monitor_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 --------
 Azure SDK code: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor
 
 Azure SDK docs: https://learn.microsoft.com/python/api/overview/
 azure/monitor-query-readme?view=azure-python
 
 """
+import contextlib
 import logging
 from datetime import datetime
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Union, cast
 
 import httpx
 import pandas as pd
 from azure.core.exceptions import HttpResponseError
@@ -405,18 +406,19 @@
         if workspace_name or connection_str is None:
             ws_config = WorkspaceConfig(workspace=workspace_name)  # type: ignore
             logger.info(
                 "WorkspaceConfig created from workspace name %s", workspace_name
             )
         elif isinstance(connection_str, str):
             self._def_connection_str = connection_str
-            ws_config = WorkspaceConfig.from_connection_string(connection_str)
-            logger.info(
-                "WorkspaceConfig created from connection_str %s", connection_str
-            )
+            with contextlib.suppress(ValueError):
+                ws_config = WorkspaceConfig.from_connection_string(connection_str)
+                logger.info(
+                    "WorkspaceConfig created from connection_str %s", connection_str
+                )
         elif isinstance(connection_str, WorkspaceConfig):
             logger.info("WorkspaceConfig as parameter %s", connection_str.workspace_id)
             ws_config = connection_str
 
         if not ws_config:
             logger.warning("No workspace set")
             raise MsticpyKqlConnectionError(
@@ -471,19 +473,17 @@
             ", ".join(self._workspace_ids),
         )
 
     def _get_time_span_value(self, **kwargs):
         """Return the timespan for the query API call."""
         default_time_params = kwargs.get("default_time_params", False)
         time_params = kwargs.get("time_span", {})
-        if (
-            default_time_params
-            or "start" not in time_params
-            or "end" not in time_params
-        ):
+        start = time_params.get("start")
+        end = time_params.get("end")
+        if default_time_params or start is None or end is None:
             time_span_value = None
             logger.info("No time parameters supplied.")
         else:
             time_span = TimeSpan(
                 start=time_params["start"],
                 end=time_params["end"],
             )
```

### Comparing `msticpy-2.8.0rc1/msticpy/data/drivers/driver_base.py` & `msticpy-2.9.0/msticpy/data/drivers/driver_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/drivers/elastic_driver.py` & `msticpy-2.9.0/msticpy/data/drivers/elastic_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/drivers/kql_driver.py` & `msticpy-2.9.0/msticpy/data/drivers/kql_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/drivers/kusto_driver.py` & `msticpy-2.9.0/msticpy/data/drivers/kusto_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/drivers/local_data_driver.py` & `msticpy-2.9.0/msticpy/data/drivers/local_data_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/drivers/local_osquery_driver.py` & `msticpy-2.9.0/msticpy/data/drivers/local_osquery_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/drivers/local_velociraptor_driver.py` & `msticpy-2.9.0/msticpy/data/drivers/local_velociraptor_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/drivers/mdatp_driver.py` & `msticpy-2.9.0/msticpy/data/drivers/mdatp_driver.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # --------------------------------------------------------------------------
 """MDATP OData Driver class."""
 from typing import Any, Optional, Union
 
 import pandas as pd
 
 from ..._version import VERSION
+from ...auth.azure_auth_core import AzureCloudConfig
 from ...auth.cloud_mappings import (
     get_defender_endpoint,
     get_m365d_endpoint,
     get_m365d_login_endpoint,
 )
 from ...common.data_utils import ensure_df_datetimes
 from ...common.utility import export
@@ -44,35 +45,47 @@
             The instance name from config to use
 
         """
         super().__init__(**kwargs)
         cs_dict = _get_driver_settings(
             self.CONFIG_NAME, self._ALT_CONFIG_NAMES, instance
         )
+
         self.cloud = cs_dict.pop("cloud", "global")
         if "cloud" in kwargs and kwargs["cloud"]:
             self.cloud = kwargs["cloud"]
 
         api_uri, oauth_uri, api_suffix = _select_api_uris(
             self.data_environment, self.cloud
         )
-        self.add_query_filter("data_environments", ("MDE", "M365D", "MDATP"))
+        self.add_query_filter(
+            "data_environments", ("MDE", "M365D", "MDATP", "GraphHunting")
+        )
 
         self.req_body = {
             "client_id": None,
             "client_secret": None,
             "grant_type": "client_credentials",
             "resource": api_uri,
         }
         self.oauth_url = oauth_uri
         self.api_root = api_uri
         self.api_ver = "api"
         self.api_suffix = api_suffix
         if self.data_environment == DataEnvironment.M365D:
             self.scopes = [f"{api_uri}/AdvancedHunting.Read"]
+        elif self.data_environment == DataEnvironment.M365DGraph:
+            self.api_ver = kwargs.get("api_ver", "v1.0")
+            self.req_body = {
+                "client_id": None,
+                "client_secret": None,
+                "grant_type": "client_credentials",
+                "scope": f"{self.api_root}.default",
+            }
+            self.scopes = [f"{api_uri}/ThreatHunting.Read.All"]
         else:
             self.scopes = [f"{api_uri}/AdvancedQuery.Read"]
 
         if connection_str:
             self.current_connection = connection_str
             self.connect(connection_str)
 
@@ -98,33 +111,50 @@
         """
         del query_source, kwargs
         data, response = self.query_with_results(
             query, body=True, api_end=self.api_suffix
         )
         if isinstance(data, pd.DataFrame):
             # If we got a schema we should convert the DateTimes to pandas datetimes
-            if "Schema" not in response:
+            if ("Schema" or "schema") not in response:
                 return data
-            date_fields = [
-                field["Name"]
-                for field in response["Schema"]
-                if field["Type"] == "DateTime"
-            ]
+
+            if self.data_environment == DataEnvironment.M365DGraph:
+                date_fields = [
+                    field["name"]
+                    for field in response["schema"]
+                    if field["type"] == "DateTime"
+                ]
+            else:
+                date_fields = [
+                    field["Name"]
+                    for field in response["Schema"]
+                    if field["Type"] == "DateTime"
+                ]
             data = ensure_df_datetimes(data, columns=date_fields)
             return data
         return response
 
 
 def _select_api_uris(data_environment, cloud):
     """Return API and login URIs for selected provider type."""
     login_uri = get_m365d_login_endpoint(cloud)
     if data_environment == DataEnvironment.M365D:
         return (
             get_m365d_endpoint(cloud),
             f"{login_uri}{{tenantId}}/oauth2/token",
             "/advancedhunting/run",
         )
+    if data_environment == DataEnvironment.M365DGraph:
+        az_cloud_config = AzureCloudConfig(cloud=cloud)
+        api_uri = az_cloud_config.endpoints.get("microsoftGraphResourceId")
+        graph_login = az_cloud_config.authority_uri
+        return (
+            api_uri,
+            f"{graph_login}{{tenantId}}/oauth2/v2.0/token",
+            "/security/runHuntingQuery",
+        )
     return (
         get_defender_endpoint(cloud),
         f"{login_uri}{{tenantId}}/oauth2/token",
         "/advancedqueries/run",
     )
```

### Comparing `msticpy-2.8.0rc1/msticpy/data/drivers/mordor_driver.py` & `msticpy-2.9.0/msticpy/data/drivers/mordor_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -437,17 +437,15 @@
     except TypeError:
         return datetime.min
 
 
 DS_PREFIX = "https://raw.githubusercontent.com/OTRF/Security-Datasets/master/datasets/"
 
 
-# pylint: disable=not-an-iterable, no-member
-
-
+# pylint: disable=not-an-iterable, no-member, too-many-instance-attributes
 @attr.s(auto_attribs=True)
 class MordorEntry:
     """Mordor data set metadata."""
 
     title: str
     id: str
     type: str
```

### Comparing `msticpy-2.8.0rc1/msticpy/data/drivers/odata_driver.py` & `msticpy-2.9.0/msticpy/data/drivers/odata_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,15 +273,16 @@
         if isinstance(json_response, int):
             print(
                 "Warning - query did not complete successfully.",
                 "Check returned response.",
             )
             return None, json_response  # type: ignore
 
-        result = json_response.get("Results", json_response)
+        results_key = "Results" if "Results" in json_response else "results"
+        result = json_response.get(results_key, json_response)
 
         if not result:
             print("Warning - query did not return any results.")
             return None, json_response  # type: ignore
         return pd.json_normalize(result), json_response
 
     # pylint: enable=too-many-branches
```

### Comparing `msticpy-2.8.0rc1/msticpy/data/drivers/resource_graph_driver.py` & `msticpy-2.9.0/msticpy/data/drivers/resource_graph_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/drivers/security_graph_driver.py` & `msticpy-2.9.0/msticpy/data/drivers/security_graph_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/drivers/sentinel_query_reader.py` & `msticpy-2.9.0/msticpy/data/drivers/sentinel_query_reader.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/drivers/splunk_driver.py` & `msticpy-2.9.0/msticpy/data/drivers/splunk_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,22 +31,22 @@
     raise MsticpyImportExtraError(
         "Cannot use this feature without splunk-sdk installed",
         title="Error importing splunk-sdk",
         extra="splunk",
     ) from imp_err
 
 __version__ = VERSION
-__author__ = "Ashwin Patil"
+__author__ = "Ashwin Patil, Tatsuya Hasegawa"
 
 logger = logging.getLogger(__name__)
 
 
 SPLUNK_CONNECT_ARGS = {
     "host": "(string) The host name (the default is 'localhost').",
-    "port": "(integer) The port number (the default is 8089).",
+    "port": "(string) The port number (the default is '8089').",
     "http_scheme": "('https' or 'http') The scheme for accessing the service "
     + "(the default is 'https').",
     "verify": "(Boolean) Enable (True) or disable (False) SSL verrification for "
     + "https connections. (optional, the default is True)",
     "owner": "(string) The owner context of the namespace (optional).",
     "app": "(string) The app context of the namespace (optional).",
     "sharing": "('global', 'system', 'app', or 'user') "
@@ -56,33 +56,35 @@
     "cookie": "(string) A session cookie. When provided, you don’t need to call"
     + " login(). This parameter is only supported for Splunk 6.2+.",
     "autologin": "(boolean) When True, automatically tries to log in again if"
     + " the session terminates.",
     "username": "(string) The Splunk account username, which is used to "
     + "authenticate the Splunk instance.",
     "password": "(string) The password for the Splunk account.",
+    "splunkToken": "(string) The Authorization Bearer Token <JWT> created in the Splunk.",
 }
 
 
 @export
 class SplunkDriver(DriverBase):
     """Driver to connect and query from Splunk."""
 
-    _SPLUNK_REQD_ARGS = ["host", "username", "password"]
-    _CONNECT_DEFAULTS: Dict[str, Any] = {"port": 8089}
+    _SPLUNK_REQD_ARGS = ["host"]
+    _CONNECT_DEFAULTS: Dict[str, Any] = {"port": "8089"}
     _TIME_FORMAT = '"%Y-%m-%d %H:%M:%S.%6N"'
 
     def __init__(self, **kwargs):
         """Instantiate Splunk Driver."""
         super().__init__(**kwargs)
         self.service = None
         self._loaded = True
         self._connected = False
         if kwargs.get("debug", False):
             logger.setLevel(logging.DEBUG)
+        self._required_params = self._SPLUNK_REQD_ARGS
 
         self.set_driver_property(
             DriverProps.PUBLIC_ATTRS,
             {
                 "client": self.service,
                 "saved_searches": self._saved_searches,
                 "fired_alerts": self._fired_alerts,
@@ -138,15 +140,15 @@
         except Exception as err:
             raise MsticpyConnectionError(
                 f"Error connecting to Splunk: {err}",
                 title="Splunk connection",
                 help_uri="https://msticpy.readthedocs.io/en/latest/DataProviders.html",
             ) from err
         self._connected = True
-        print("connected")
+        print("Connected.")
 
     def _get_connect_args(
         self, connection_str: Optional[str], **kwargs
     ) -> Dict[str, Any]:
         """Check and consolidate connection parameters."""
         cs_dict: Dict[str, Any] = self._CONNECT_DEFAULTS
         # Fetch any config settings
@@ -168,20 +170,27 @@
         cs_dict["port"] = int(cs_dict["port"])
         verify_opt = cs_dict.get("verify")
         if isinstance(verify_opt, str):
             cs_dict["verify"] = "true" in verify_opt.casefold()
         elif isinstance(verify_opt, bool):
             cs_dict["verify"] = verify_opt
 
-        missing_args = set(self._SPLUNK_REQD_ARGS) - cs_dict.keys()
+        # Different required parameters for the REST API authentication method
+        # between user/pass and authorization bearer token
+        if "username" in cs_dict:
+            self._required_params = ["host", "username", "password"]
+        else:
+            self._required_params = ["host", "splunkToken"]
+
+        missing_args = set(self._required_params) - cs_dict.keys()
         if missing_args:
             raise MsticpyUserConfigError(
                 "One or more connection parameters missing for Splunk connector",
                 ", ".join(missing_args),
-                f"Required parameters are {', '.join(self._SPLUNK_REQD_ARGS)}",
+                f"Required parameters are {', '.join(self._required_params)}",
                 "All parameters:",
                 *[f"{arg}: {desc}" for arg, desc in SPLUNK_CONNECT_ARGS.items()],
                 title="no Splunk connection parameters",
             )
         return cs_dict
 
     def query(
```

### Comparing `msticpy-2.8.0rc1/msticpy/data/drivers/sumologic_driver.py` & `msticpy-2.9.0/msticpy/data/drivers/sumologic_driver.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/cybereason/cybereason_connections.yaml` & `msticpy-2.9.0/msticpy/data/queries/cybereason/cybereason_connections.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/cybereason/cybereason_hosts.yaml` & `msticpy-2.9.0/msticpy/data/queries/cybereason/cybereason_hosts.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/cybereason/cybereason_processes.yaml` & `msticpy-2.9.0/msticpy/data/queries/cybereason/cybereason_processes.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/localdata/local_data.yaml` & `msticpy-2.9.0/msticpy/data/queries/localdata/local_data.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/m365d/kql_m365_alerts.yaml` & `msticpy-2.9.0/msticpy/data/queries/m365d/kql_m365_alerts.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/m365d/kql_m365_file.yaml` & `msticpy-2.9.0/msticpy/data/queries/m365d/kql_m365_file.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/m365d/kql_m365_hunting.yaml` & `msticpy-2.9.0/msticpy/data/queries/m365d/kql_m365_hunting.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,14 @@
   data_environments: [MDATP, MDE, M365D, LogAnalytics]
   data_families: [MDEHunting, M365DHunting]
   tags: ['user']
 defaults:
   metadata:
     data_source: 'hunting_queries'
   parameters:
-      start:
-        description: Query start time
-        type: datetime
-      end:
-        description: Query end time
-        type: datetime
       add_query_items:
         description: Additional query clauses
         type: str
         default: ''
       time_column:
         description: The name of the column detailing the time the event was generated.
         type: str
@@ -409,15 +403,15 @@
         ) on AccountName
         | extend Command = tostring(extractjson("$.Command", AdditionalFields))
         | where Command !in (WhitelistedCmdlets)
         | summarize ({time_column}, ReportId)=argmax({time_column}, ReportId),
             makeset(Command), count(), min({time_column}) by
             AccountName, DeviceName, DeviceId
         | order by AccountName asc
-        | where min_Timestamp > ago(1d)
+        | where min_{time_column} > ago(1d)
         {add_query_items}'
       uri: "https://github.com/microsoft/WindowsDefenderATP-Hunting-Queries/blob/master/Lateral%20Movement/ServiceAccountsPerformingRemotePS.txt"
   accessibility_persistence:
     description: This query looks for persistence or privilege escalation done using Windows Accessibility features.
     metadata:
     args:
       query: '
```

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/m365d/kql_m365_identity.yaml` & `msticpy-2.9.0/msticpy/data/queries/m365d/kql_m365_identity.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/m365d/kql_m365_network.yaml` & `msticpy-2.9.0/msticpy/data/queries/m365d/kql_m365_network.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/m365d/kql_m365_process.yaml` & `msticpy-2.9.0/msticpy/data/queries/m365d/kql_m365_process.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/m365d/kql_m365_user.yaml` & `msticpy-2.9.0/msticpy/data/queries/m365d/kql_m365_user.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/mde/kql_mdatp_alerts.yaml` & `msticpy-2.9.0/msticpy/data/queries/mde/kql_mdatp_alerts.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/mde/kql_mdatp_file.yaml` & `msticpy-2.9.0/msticpy/data/queries/mde/kql_mdatp_file.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/mde/kql_mdatp_hunting.yaml` & `msticpy-2.9.0/msticpy/data/queries/mde/kql_mdatp_hunting.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,14 @@
   data_environments: [MDATP, MDE, M365D, LogAnalytics]
   data_families: [MDEHunting, M365DHunting]
   tags: ['user']
 defaults:
   metadata:
     data_source: 'hunting_queries'
   parameters:
-      start:
-        description: Query start time
-        type: datetime
-      end:
-        description: Query end time
-        type: datetime
       add_query_items:
         description: Additional query clauses
         type: str
         default: ''
 sources:
   doc_with_link:
     description: Looks for a Word document attachment, from which a link was clicked, and after which there was a browser download.
```

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/mde/kql_mdatp_network.yaml` & `msticpy-2.9.0/msticpy/data/queries/mde/kql_mdatp_network.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/mde/kql_mdatp_process.yaml` & `msticpy-2.9.0/msticpy/data/queries/mde/kql_mdatp_process.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/mde/kql_mdatp_user.yaml` & `msticpy-2.9.0/msticpy/data/queries/mde/kql_mdatp_user.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/msgraph/graph_alerts.yaml` & `msticpy-2.9.0/msticpy/data/queries/msgraph/graph_alerts.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_alert.yaml` & `msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_alert.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_az_dns.yaml` & `msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_az_dns.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_az_network.yaml` & `msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_az_network.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_azure.yaml` & `msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_azure.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_azuresentinel.yaml` & `msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_azuresentinel.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_heartbeat_info.yaml` & `msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_heartbeat_info.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_lxauditd.yaml` & `msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_lxauditd.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_activity.yaml` & `msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_activity.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_apps.yaml` & `msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_apps.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_logon.yaml` & `msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_logon.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_sysmon.yaml` & `msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_lxsyslog_sysmon.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_net.yaml` & `msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_net.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_o365.yaml` & `msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_o365.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_threatintel.yaml` & `msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_threatintel.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_timeseries.yaml` & `msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_timeseries.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_winevent.yaml` & `msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_winevent.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_winevent_logon.yaml` & `msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_winevent_logon.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/mssentinel/kql_sent_winevent_proc.yaml` & `msticpy-2.9.0/msticpy/data/queries/mssentinel/kql_sent_winevent_proc.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/resourcegraph/resource_graph_queries.yaml` & `msticpy-2.9.0/msticpy/data/queries/resourcegraph/resource_graph_queries.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/resourcegraph/sentinel_resources.yaml` & `msticpy-2.9.0/msticpy/data/queries/resourcegraph/sentinel_resources.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/splunk/splunk_alert_queries.yaml` & `msticpy-2.9.0/msticpy/data/queries/splunk/splunk_alert_queries.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/splunk/splunk_authentication_queries.yaml` & `msticpy-2.9.0/msticpy/data/queries/splunk/splunk_authentication_queries.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/splunk/splunk_queries.yaml` & `msticpy-2.9.0/msticpy/data/queries/splunk/splunk_queries.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/queries/sumologic/sumologic_queries.yaml` & `msticpy-2.9.0/msticpy/data/queries/sumologic/sumologic_queries.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/query_container.py` & `msticpy-2.9.0/msticpy/data/query_container.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/query_defns.py` & `msticpy-2.9.0/msticpy/data/query_defns.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/sql_to_kql.py` & `msticpy-2.9.0/msticpy/data/sql_to_kql.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/storage/azure_blob_storage.py` & `msticpy-2.9.0/msticpy/data/storage/azure_blob_storage.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/uploaders/__init__.py` & `msticpy-2.9.0/msticpy/data/uploaders/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/uploaders/loganalytics_uploader.py` & `msticpy-2.9.0/msticpy/data/uploaders/loganalytics_uploader.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/uploaders/splunk_uploader.py` & `msticpy-2.9.0/msticpy/data/uploaders/splunk_uploader.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/data/uploaders/uploader_base.py` & `msticpy-2.9.0/msticpy/data/uploaders/uploader_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/entities/__init__.py` & `msticpy-2.9.0/msticpy/datamodel/entities/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 """Entity sub-package."""
 import difflib
+from typing import List
 
 from .account import Account
 from .alert import Alert
 from .azure_resource import AzureResource
 from .cloud_application import CloudApplication
 from .cloud_logon_session import CloudLogonSession
 from .dns import Dns
@@ -25,96 +26,129 @@
 from .host import Host
 from .host_logon_session import HostLogonSession
 from .iot_device import IoTDevice
 from .ip_address import IpAddress
 from .mail_cluster import MailCluster
 from .mail_message import MailMessage
 from .mailbox import Mailbox
+from .mailbox_configuration import MailboxConfiguration
 from .malware import Malware
 from .network_connection import NetworkConnection
+from .oauth_application import OAuthApplication
 from .process import Process
 from .registry_key import RegistryKey
 from .registry_value import RegistryValue
 from .security_group import SecurityGroup
+from .service_principal import ServicePrincipal
 from .submission_mail import SubmissionMail
 from .threat_intelligence import Threatintelligence
 from .unknown_entity import UnknownEntity
 from .url import Url
 
 from ..soc.incident import Incident  # isort: skip
 
+
+# Defender class equivalents
+class User(Account):
+    """Alias for Account."""
+
+
+class Ip(IpAddress):
+    """Alias for IpAddress."""
+
+
+class Machine(Host):
+    """Alias for Host."""
+
+
 # Dictionary to map text names of types to the class.
 Entity.ENTITY_NAME_MAP.update(
     {
         "account": Account,
-        "azureresource": AzureResource,
+        "alert": Alert,
+        "alerts": Alert,
         "azure-resource": AzureResource,
-        "host": Host,
-        "process": Process,
-        "file": File,
-        "cloudapplication": CloudApplication,
+        "azureresource": AzureResource,
         "cloud-application": CloudApplication,
+        "cloud-logon-session": CloudLogonSession,
+        "cloudapplication": CloudApplication,
+        "cloudlogonsession": CloudLogonSession,
         "dns": Dns,
         "dnsresolve": Dns,
-        "ipaddress": IpAddress,
+        "file": File,
+        "filehash": FileHash,
+        "geolocation": GeoLocation,
+        "host-logon-session": HostLogonSession,
+        "host": Host,
+        "hostlogonsession": HostLogonSession,
+        "incident": Incident,
         "iotdevice": IoTDevice,
         "ip": IpAddress,
-        "networkconnection": NetworkConnection,
-        "network-connection": NetworkConnection,
-        "mailbox": Mailbox,
-        "mail-message": MailMessage,
-        "mailmessage": MailMessage,
+        "ipaddress": IpAddress,
+        "location": GeoLocation,
+        "machine": Machine,
         "mail-cluster": MailCluster,
+        "mail-message": MailMessage,
+        "mailbox": Mailbox,
         "mailcluster": MailCluster,
+        "mailboxconfiguration": MailboxConfiguration,
+        "mailmessage": MailMessage,
         "malware": Malware,
+        "network-connection": NetworkConnection,
+        "networkconnection": NetworkConnection,
+        "oauthapplication": OAuthApplication,
+        "process": Process,
         "registry-key": RegistryKey,
-        "registrykey": RegistryKey,
         "registry-value": RegistryValue,
+        "registrykey": RegistryKey,
         "registryvalue": RegistryValue,
-        "host-logon-session": HostLogonSession,
-        "hostlogonsession": HostLogonSession,
-        "filehash": FileHash,
         "security-group": SecurityGroup,
         "securitygroup": SecurityGroup,
+        "ServicePrincipal": ServicePrincipal,
         "SubmissionMail": SubmissionMail,
-        "alerts": Alert,
-        "alert": Alert,
         "threatintelligence": Threatintelligence,
-        "url": Url,
         "unknown": UnknownEntity,
-        "geolocation": GeoLocation,
-        "location": GeoLocation,
-        "incident": Incident,
-        "cloud-logon-session": CloudLogonSession,
+        "url": Url,
+        "user": User,
     }
 )
 
 
 def find_entity(entity):
     """Find entity name."""
     entity_cf = entity.casefold()
-    entity_classes = {
+    entity_cls_dict = {
         cls.__name__.casefold(): cls for cls in Entity.ENTITY_NAME_MAP.values()
     }
     if entity_cf in Entity.ENTITY_NAME_MAP:
         print(f"Match found '{Entity.ENTITY_NAME_MAP[entity].__name__}'")
         return Entity.ENTITY_NAME_MAP[entity]
-    if entity_cf in entity_classes:
-        print(f"Match found '{entity_classes[entity_cf].__name__}'")
-        return entity_classes[entity_cf]
+    if entity_cf in entity_cls_dict:
+        print(f"Match found '{entity_cls_dict[entity_cf].__name__}'")
+        return entity_cls_dict[entity_cf]
     # Try to find the closest matches
-    closest = difflib.get_close_matches(entity, entity_classes.keys(), cutoff=0.4)
+    closest = difflib.get_close_matches(entity, entity_cls_dict.keys(), cutoff=0.4)
     mssg = [f"No exact match found for '{entity}'. "]
     if len(closest) == 1:
-        mssg.append(f"Closest match is '{entity_classes[closest[0]].__name__}'")
+        mssg.append(f"Closest match is '{entity_cls_dict[closest[0]].__name__}'")
     elif closest:
-        match_list = [f"'{entity_classes[mtch].__name__}'" for mtch in closest]
+        match_list = [f"'{entity_cls_dict[match].__name__}'" for match in closest]
         mssg.append(f"Closest matches are {', '.join(match_list)}")
     else:
         mssg.extend(
             [
                 "No close match found. Entities available:",
-                *(cls.__name__ for cls in entity_classes.values()),
+                *(cls.__name__ for cls in entity_cls_dict.values()),
             ]
         )
     print("\n".join(mssg))
     return None
+
+
+def list_entities() -> List[str]:
+    """List entities."""
+    return sorted([cls.__name__ for cls in set(Entity.ENTITY_NAME_MAP.values())])
+
+
+def entity_classes() -> List[type]:
+    """Return a list of all entity classes."""
+    return list(set(Entity.ENTITY_NAME_MAP.values()))
```

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/entities/account.py` & `msticpy-2.9.0/msticpy/datamodel/entities/account.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 """Account Entity class."""
 from typing import Any, Mapping, Optional
 
 from ..._version import VERSION
+from ...common.data_types import SplitProperty
 from ...common.utility import export
 from .entity import Entity
 from .host import Host
 
 __version__ = VERSION
 __author__ = "Ian Hellen"
 
@@ -45,18 +46,22 @@
         Account PUID
     IsDomainJoined : bool
         Account IsDomainJoined
     DisplayName : str
         Account DisplayName
     ObjectGuid : str
         The object ID of the user account
+    Upn : str
+        The User principal name of the account
 
     """
 
     ID_PROPERTIES = ["QualifiedName", "Sid", "AadUserId", "PUID", "ObjectGuid"]
+    Upn = SplitProperty("Name", "UPNSuffix", "@")
+    UPN = Upn
 
     def __init__(
         self,
         src_entity: Mapping[str, Any] = None,
         src_event: Mapping[str, Any] = None,
         role: str = "subject",
         **kwargs,
@@ -88,20 +93,23 @@
         self.Name: Optional[str] = None
         self.NTDomain: Optional[str] = None
         self.UPNSuffix: Optional[str] = None
         self.Host: Optional[Host] = None
         self.LogonId: Optional[str] = None
         self.Sid: Optional[str] = None
         self.AadTenantId: Optional[str] = None
-        self.AadUserId: Optional[str] = None
+        self._AadUserId: Optional[str] = None
         self.PUID: Optional[str] = None
         self.IsDomainJoined: bool = False
         self.DisplayName: Optional[str] = None
         self.ObjectGuid: Optional[str] = None
-
+        if "Upn" in kwargs:
+            self.Upn = kwargs.pop("Upn")
+        if "AadUserId" in kwargs:
+            self.AadUserId = kwargs.pop("AadUserId")
         super().__init__(src_entity=src_entity, **kwargs)
         if src_event is not None:
             self._create_from_event(src_event, role)
 
     @property
     def description_str(self) -> str:
         """Return Entity Description."""
@@ -109,14 +117,24 @@
 
     @property
     def name_str(self) -> str:
         """Return Entity Name."""
         return self.Name or self.DisplayName or "Unknown Account"
 
     @property
+    def AadUserId(self) -> Optional[str]:  # noqa: N802
+        """Return the Azure AD user ID or the ObjectGuid."""
+        return self._AadUserId or self.ObjectGuid
+
+    @AadUserId.setter
+    def AadUserId(self, value: str):  # noqa: N802
+        """Set the Azure AD user ID."""
+        self._AadUserId = value
+
+    @property
     def qualified_name(self) -> str:
         """Windows qualified account name."""
         if "Name" not in self:
             return ""
         name = self["Name"]
         if "NTDomain" in self and self.NTDomain:
             return f"{self.NTDomain}\\{name}"
@@ -172,14 +190,18 @@
 
         if "UPNSuffix" in src_event:
             self.UPNSuffix = src_event["UPNSuffix"]
         elif "UpnSuffix" in src_event:
             self.UPNSuffix = src_event["UpnSuffix"]
         else:
             self.UPNSuffix = None
+        if "Upn" in src_event:
+            self.Upn = src_event["Upn"]
+        if "UPN" in src_event:
+            self.Upn = src_event["UPN"]
 
     _entity_schema = {
         # Name (type System.String)
         "Name": None,
         # NTDomain (type System.String)
         "NTDomain": None,
         # UPNSuffix (type System.String)
@@ -198,11 +220,12 @@
         # PUID (type System.Nullable`1[System.Guid])
         "PUID": None,
         # IsDomainJoined (type System.Nullable`1[System.Boolean])
         "IsDomainJoined": None,
         # DisplayName (type System.String)
         "DisplayName": None,
         "ObjectGuid": None,
+        "Upn": None,
         "TimeGenerated": None,
         "StartTime": None,
         "EndTime": None,
     }
```

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/entities/alert.py` & `msticpy-2.9.0/msticpy/datamodel/entities/alert.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,19 +82,21 @@
         """
         self.DisplayName: Optional[str] = None
         self.CompromisedEntity: Optional[str] = None
         self.Count: Any = None
         self.StartTimeUtc: Optional[datetime] = None
         self.EndTimeUtc: Optional[datetime] = None
         self.Severity: Any = None
+        self.SystemAlertId: Optional[str] = None
         self.SystemAlertIds: List[str] = []
         self.AlertType: Optional[str] = None
         self.VendorName: Optional[str] = None
         self.ProviderName: Optional[str] = None
         self.Entities: Optional[List] = None
+        self.Version = "3.0"
         super().__init__(src_entity=src_entity, **kwargs)
         if src_entity is not None:
             self._create_from_ent(src_entity)
 
         if isinstance(src_event, pd.Series) and not src_event.empty:
             self._create_from_event(src_event)
 
@@ -128,22 +130,34 @@
 
     @property
     def description_str(self) -> str:
         """Return Entity Description."""
         if self.StartTime and self.CompromisedEntity:
             return f"{self.DisplayName} ({self.StartTime}) {self.CompromisedEntity}"
         else:
-            return f"{self.DisplayName} - {self.SystemAlertIds}"
+            return f"{self.DisplayName} - {self.AlertId}"
 
     @property
     def name_str(self) -> str:
         """Return Entity Name."""
         alert_name = self.AlertDisplayName or self.DisplayName or None
         return f"Alert: {alert_name}" or self.__class__.__name__
 
+    @property
+    def AlertId(self) -> Optional[str]:  # noqa: N802
+        """Return the system alert ID."""
+        return self.SystemAlertId or (
+            self.SystemAlertIds[0] if self.SystemAlertIds else None
+        )
+
+    @AlertId.setter
+    def AlertId(self, value: str):  # noqa: N802
+        """Set the system alert ID."""
+        self.SystemAlertId = value
+
     def _add_additional_data(self, src_entity: Mapping[str, Any]):
         """Populate additional alert properties."""
         if isinstance(src_entity, dict):
             prop_list = src_entity.items()
         elif type(src_entity).__name__ == "SecurityAlert":
             prop_list = src_entity.properties.items()  # type: ignore
         # pylint: disable=all
```

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/entities/azure_resource.py` & `msticpy-2.9.0/msticpy/datamodel/entities/azure_resource.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/entities/cloud_application.py` & `msticpy-2.9.0/msticpy/datamodel/entities/cloud_application.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/entities/cloud_logon_session.py` & `msticpy-2.9.0/msticpy/datamodel/entities/cloud_logon_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 class CloudLogonSession(Entity):
     """
     CloudLogonSession Entity class.
 
     Attributes
     ----------
     SessionId : str
-        The loggon session ID
+        The logon session ID
     Account : str
         The Account
     UserAgent : str
         The UserAgent
     StartTime: str
         The time the session started
```

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/entities/dns.py` & `msticpy-2.9.0/msticpy/datamodel/entities/dns.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     """
     DNS Resolve Entity class.
 
     Attributes
     ----------
     DomainName : str
         DnsResolve DomainName
-    IpAdresses : List[str]
-        DnsResolve IpAdresses
+    IpAddresses : List[str]
+        DnsResolve IpAddresses
     DnsServerIp : IPAddress
         DnsResolve DnsServerIp
     HostIpAddress : IPAddress
         DnsResolve HostIpAddress
 
     """
 
@@ -53,35 +53,35 @@
         ----------------
         kwargs : Dict[str, Any]
             Supply the entity properties as a set of
             kw arguments.
 
         """
         self.DomainName: Optional[str] = None
-        self.IpAdresses: List[IpAddress] = []
+        self.IpAddresses: List[IpAddress] = []
         self.DnsServerIp: Optional[IpAddress] = None
         self.HostIpAddress: Optional[IpAddress] = None
         super().__init__(src_entity=src_entity, **kwargs)
 
     @property
     def description_str(self) -> str:
         """Return Entity Description."""
-        return f"{self.DomainName}: IPs: {repr(self.IpAdresses)}"
+        return f"{self.DomainName}: IPs: {repr(self.IpAddresses)}"
 
     @property
     def name_str(self) -> str:
         """Return Entity Name."""
         return self.DomainName or self.__class__.__name__
 
     _entity_schema = {
         # DomainName (type System.String)
         "DomainName": None,
-        # IpAdresses (type System.Collections.Generic.List`1
+        # IpAddresses (type System.Collections.Generic.List`1
         # [Microsoft.Azure.Security.Detection.AlertContracts.V3.Entities.IP])
-        "IpAdresses": (List, "IpAddress"),
+        "IpAddresses": (List, "IpAddress"),
         # DnsServerIp (type Microsoft.Azure.Security.Detection
         # .AlertContracts.V3.Entities.IP)
         "DnsServerIp": "IpAddress",
         # HostIpAddress (type Microsoft.Azure.Security.Detection
         # .AlertContracts.V3.Entities.IP)
         "HostIpAddress": "IpAddress",
         "TimeGenerated": None,
```

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/entities/entity.py` & `msticpy-2.9.0/msticpy/datamodel/entities/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,16 +211,15 @@
     def __contains__(self, key: str):
         """Allow property in test."""
         # In operator overload
         return key in self.__dict__
 
     def __getattr__(self, name: str):
         """Return the value of the named property 'name'."""
-        props = ["name_str", "description_str"]
-        if name in self._entity_schema or name in props:
+        if name in self._entity_schema or name in {"name_str", "description_str"}:
             return None
         raise AttributeError(f"{name} is not a valid attribute.")
 
     def __iter__(self):
         """Iterate over entity_properties."""
         return iter(self.properties)
 
@@ -304,15 +303,17 @@
             return False
         return self.properties == other.properties
 
     def __hash__(self) -> int:
         """Return the hash of the entity based on non-empty property values."""
         return hash(
             " ".join(
-                f"{prop}:{val}" for prop, val in self.properties.items() if str(val)
+                f"{prop}:{val}"
+                for prop, val in self.properties.items()
+                if str(val) and prop not in ("edges", "TimeGenerated")
             )
         )
 
     def is_equivalent(self, other: Any) -> bool:
         """
         Return True if the entities are equivalent.
 
@@ -340,14 +341,15 @@
         if not isinstance(other, Entity):
             return False
         return not any(
             self.__dict__[prop] != other.__dict__[prop]
             and self.__dict__[prop]
             and other.__dict__[prop]
             for prop in self.__dict__  # pylint: disable=consider-using-dict-items
+            if prop not in ("edges", "TimeGenerated") and not prop.startswith("_")
         )
 
     def merge(self, other: Any) -> "Entity":
         """
         Merge with other entity to create new entity.
 
         Returns
```

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/entities/entity_enums.py` & `msticpy-2.9.0/msticpy/datamodel/entities/entity_enums.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/entities/entity_graph.py` & `msticpy-2.9.0/msticpy/datamodel/entities/entity_graph.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/entities/file.py` & `msticpy-2.9.0/msticpy/datamodel/entities/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 """File Entity class."""
 from typing import Any, List, Mapping, Optional
 
 from ..._version import VERSION
+from ...common.data_types import SharedProperty
 from ...common.utility import export
 from .entity import Entity
 from .entity_enums import Algorithm, OSFamily
 from .file_hash import FileHash
 from .host import Host
 
 __version__ = VERSION
@@ -45,14 +46,15 @@
         File Sha256Ac
     FileHashes : List[FileHash]
         File FileHashes
 
     """
 
     ID_PROPERTIES = ["FullPath", "Sha1", "Sha256", "Sha256ac", "Md5"]
+    FolderPath = SharedProperty("Directory")
 
     def __init__(
         self,
         src_entity: Mapping[str, Any] = None,
         src_event: Mapping[str, Any] = None,
         role: str = "new",
         **kwargs,
```

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/entities/file_hash.py` & `msticpy-2.9.0/msticpy/datamodel/entities/file_hash.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/entities/geo_location.py` & `msticpy-2.9.0/msticpy/datamodel/entities/geo_location.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/entities/graph_property.py` & `msticpy-2.9.0/msticpy/datamodel/entities/graph_property.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/entities/host.py` & `msticpy-2.9.0/msticpy/datamodel/entities/host.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 """Host Entity class."""
 from typing import Any, Mapping, Optional
 
 from ..._version import VERSION
+from ...common.data_types import SplitProperty
 from ...common.utility import export
 from .entity import Entity
 from .entity_enums import OSFamily
 
 __version__ = VERSION
 __author__ = "Ian Hellen"
 
@@ -42,15 +43,16 @@
     OSVersion : str
         Host OSVersion
     IsDomainJoined : bool
         Host IsDomainJoined
 
     """
 
-    ID_PROPERTIES = ["fqdn", "AzureID", "OMSAgentID"]
+    ID_PROPERTIES = ["fqdn", "AzureID", "OMSAgentID", "DeviceId"]
+    DeviceName = SplitProperty("HostName", "DnsDomain", ".")
 
     def __init__(
         self,
         src_entity: Mapping[str, Any] = None,
         src_event: Mapping[str, Any] = None,
         **kwargs,
     ):
@@ -79,14 +81,15 @@
         self.HostName: Optional[str] = None
         self.NetBiosName: Optional[str] = None
         self.AzureID: Optional[str] = None
         self.OMSAgentID: Optional[str] = None
         self.OSFamily: OSFamily = OSFamily.Windows
         self.OSVersion: Optional[str] = None
         self.IsDomainJoined: bool = False
+        self.DeviceId: Optional[str] = None
 
         super().__init__(src_entity=src_entity, **kwargs)
         self._computer = None
         if src_event is not None:
             self._create_from_event(src_event)
 
     @property
@@ -129,14 +132,17 @@
             else:
                 self.HostName = src_event["Computer"]
         elif "HostName" in src_event:
             self.HostName = src_event["HostName"]
             if "DnsDomain" in src_event:
                 self.DnsDomain = src_event["DnsDomain"]
         self.NetBiosName = self.HostName
+        self.AzureID = src_event.get("AzureID")
+        self.DeviceId = src_event.get("DeviceId")
+        self.DeviceName = src_event.get("DeviceName")
 
     _entity_schema = {
         # DnsDomain (type System.String)
         "DnsDomain": None,
         # NTDomain (type System.String)
         "NTDomain": None,
         # HostName (type System.String)
@@ -148,11 +154,13 @@
         # OMSAgentID (type System.String)
         "OMSAgentID": None,
         # OSFamily (type System.Nullable`1
         # [Microsoft.Azure.Security.Detection.AlertContracts.V3.Entities.OSFamily])
         "OSFamily": "OSFamily",
         # IsDomainJoined (type System.Nullable`1[System.Boolean])
         "IsDomainJoined": None,
+        "DeviceId": None,
+        "DeviceName": None,
         "TimeGenerated": None,
         "StartTime": None,
         "EndTime": None,
     }
```

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/entities/host_logon_session.py` & `msticpy-2.9.0/msticpy/datamodel/entities/host_logon_session.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/entities/iot_device.py` & `msticpy-2.9.0/msticpy/datamodel/entities/iot_device.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/entities/ip_address.py` & `msticpy-2.9.0/msticpy/datamodel/entities/ip_address.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/entities/mail_cluster.py` & `msticpy-2.9.0/msticpy/datamodel/entities/mail_cluster.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/entities/mail_message.py` & `msticpy-2.9.0/msticpy/datamodel/entities/mail_message.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/entities/mailbox.py` & `msticpy-2.9.0/msticpy/datamodel/entities/mailbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,16 @@
         if src_event:
             self._create_from_event(src_event)
 
     def _create_from_event(self, src_event):
         self.MailboxPrimaryAddress = src_event.get("MailboxPrimaryAddress")
         self.Upn = src_event.get("Upn")
         self.DisplayName = src_event.get("DisplayName")
+        self.ExternalDirectoryObjectId = src_event.get("ExternalDirectoryObjectId")
+        self.RiskLevel = src_event.get("RiskLevel")
 
     @property
     def description_str(self):
         """Return Entity Description."""
         return (
             f"{self.MailboxPrimaryAddress} - {self.RiskLevel}"
             or self.__class__.__name__
```

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/entities/malware.py` & `msticpy-2.9.0/msticpy/datamodel/entities/malware.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/entities/network_connection.py` & `msticpy-2.9.0/msticpy/datamodel/entities/network_connection.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/entities/process.py` & `msticpy-2.9.0/msticpy/datamodel/entities/process.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/entities/registry_key.py` & `msticpy-2.9.0/msticpy/datamodel/entities/registry_key.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/entities/registry_value.py` & `msticpy-2.9.0/msticpy/datamodel/entities/registry_value.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/entities/security_group.py` & `msticpy-2.9.0/msticpy/datamodel/entities/security_group.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/entities/submission_mail.py` & `msticpy-2.9.0/msticpy/datamodel/entities/submission_mail.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/entities/threat_intelligence.py` & `msticpy-2.9.0/msticpy/datamodel/entities/threat_intelligence.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/entities/unknown_entity.py` & `msticpy-2.9.0/msticpy/datamodel/entities/unknown_entity.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/entities/url.py` & `msticpy-2.9.0/msticpy/datamodel/entities/url.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/pivot.py` & `msticpy-2.9.0/msticpy/datamodel/pivot.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/soc/incident.py` & `msticpy-2.9.0/msticpy/datamodel/soc/incident.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/datamodel/soc/sentinel_alert.py` & `msticpy-2.9.0/msticpy/datamodel/soc/sentinel_alert.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/init/__init__.py` & `msticpy-2.9.0/msticpy/init/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/init/azure_ml_tools.py` & `msticpy-2.9.0/msticpy/init/azure_ml_tools.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/init/azure_synapse_tools.py` & `msticpy-2.9.0/msticpy/init/azure_synapse_tools.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/init/logging.py` & `msticpy-2.9.0/msticpy/init/logging.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/init/mp_pandas_accessors.py` & `msticpy-2.9.0/msticpy/init/mp_pandas_accessors.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/init/mp_plugins.py` & `msticpy-2.9.0/msticpy/init/mp_plugins.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/init/nbinit.py` & `msticpy-2.9.0/msticpy/init/nbinit.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,40 +179,40 @@
 # pylint: disable=use-dict-literal
 _NB_IMPORTS = [
     dict(pkg="pandas", alias="pd"),
     dict(pkg="IPython", tgt="get_ipython"),
     dict(pkg="IPython.display", tgt="display"),
     dict(pkg="IPython.display", tgt="HTML"),
     dict(pkg="IPython.display", tgt="Markdown"),
-    dict(pkg="ipywidgets", alias="widgets"),
+    # dict(pkg="ipywidgets", alias="widgets"),
     dict(pkg="pathlib", tgt="Path"),
     dict(pkg="numpy", alias="np"),
 ]
 if sns is not None:
     _NB_IMPORTS.append(dict(pkg="seaborn", alias="sns"))
 
 _MP_IMPORTS = [
     dict(pkg="msticpy"),
     dict(pkg="msticpy.data", tgt="QueryProvider"),
-    dict(pkg="msticpy.vis.foliummap", tgt="FoliumMap"),
-    dict(pkg="msticpy.context", tgt="TILookup"),
-    dict(pkg="msticpy.context", tgt="GeoLiteLookup"),
-    dict(pkg="msticpy.context", tgt="IPStackLookup"),
-    dict(pkg="msticpy.transform", tgt="IoCExtract"),
+    # dict(pkg="msticpy.vis.foliummap", tgt="FoliumMap"),
+    # dict(pkg="msticpy.context", tgt="TILookup"),
+    # dict(pkg="msticpy.context", tgt="GeoLiteLookup"),
+    # dict(pkg="msticpy.context", tgt="IPStackLookup"),
+    # dict(pkg="msticpy.transform", tgt="IoCExtract"),
     dict(pkg="msticpy.common.utility", tgt="md"),
     dict(pkg="msticpy.common.utility", tgt="md_warn"),
     dict(pkg="msticpy.common.wsconfig", tgt="WorkspaceConfig"),
     dict(pkg="msticpy.init.pivot", tgt="Pivot"),
     dict(pkg="msticpy.datamodel", tgt="entities"),
     dict(pkg="msticpy.init", tgt="nbmagics"),
-    dict(pkg="msticpy.nbtools", tgt="SecurityAlert"),
+    # dict(pkg="msticpy.nbtools", tgt="SecurityAlert"),
     dict(pkg="msticpy.vis", tgt="mp_pandas_plot"),
-    dict(pkg="msticpy.vis", tgt="nbdisplay"),
+    # dict(pkg="msticpy.vis", tgt="nbdisplay"),
     dict(pkg="msticpy.init", tgt="mp_pandas_accessors"),
-    dict(pkg="msticpy", tgt="nbwidgets"),
+    # dict(pkg="msticpy", tgt="nbwidgets"),
 ]
 
 _MP_IMPORT_ALL: List[Dict[str, str]] = [
     dict(module_name="msticpy.datamodel.entities"),
 ]
 # pylint: enable=use-dict-literal
 
@@ -226,44 +226,15 @@
 )
 
 current_providers: Dict[str, Any] = {}  # pylint: disable=invalid-name
 
 _SYNAPSE_KWARGS = ["identity_type", "storage_svc_name", "tenant_id", "cloud"]
 
 
-def _pr_output(*args):
-    """Output to IPython display or print."""
-    if not _VERBOSITY():
-        return
-    if is_ipython():
-        display(HTML(" ".join([*args, "<br>"]).replace("\n", "<br>")))
-    else:
-        print(*args)
-
-
-def _err_output(*args):
-    """Output to IPython display or print - always output regardless of verbosity."""
-    if is_ipython():
-        display(HTML(" ".join([*args, "<br>"]).replace("\n", "<br>")))
-        display(
-            HTML(
-                "For more info and options run:"
-                "<pre>import msticpy as mp\nhelp(mp.nbinit)</pre>"
-            )
-        )
-    else:
-        print(*args)
-        print(
-            "\nFor more info and options run:",
-            "\n    import msticpy as mp",
-            "\n    help(mp.nbinit)",
-        )
-
-
-# pylint: disable=too-many-statements
+# pylint: disable=too-many-statements, too-many-branches
 def init_notebook(
     namespace: Optional[Dict[str, Any]] = None,
     def_imports: str = "all",
     additional_packages: List[str] = None,
     extra_imports: List[str] = None,
     **kwargs,
 ):
@@ -379,16 +350,14 @@
     Getting started notebook
     https://github.com/Azure/Azure-Sentinel-Notebooks/blob/master/A%20Getting%20Started%20Guide%20For%20Azure%20Sentinel%20ML%20Notebooks.ipynb
 
     Configuring your environment notebook
     https://github.com/Azure/Azure-Sentinel-Notebooks/blob/master/ConfiguringNotebookEnvironment.ipynb
 
     """
-    global current_providers  # pylint: disable=global-statement, invalid-name
-
     if namespace is None and get_ipython():
         namespace = get_ipython().user_global_ns
     else:
         namespace = namespace if (namespace is not None) else {}
     check_kwargs(
         kwargs,
         [
@@ -409,40 +378,36 @@
 
     _set_verbosity(**kwargs)
 
     _pr_output("<hr><h4>Starting Notebook initialization...</h4>")
     logger.info("Starting Notebook initialization")
     # Check Azure ML environment
     if _detect_env("aml", **kwargs) and is_in_aml():
-        check_aml_settings(*_get_aml_globals(namespace))
+        try:
+            check_aml_settings(*_get_aml_globals(namespace))
+        except Exception as err:  # pylint: disable=broad-except
+            logger.warning("Error initializing Azure ML environment: %s", err)
     else:
         # If not in AML check and print version status
-        stdout_cap = io.StringIO()
-        with redirect_stdout(stdout_cap):
-            check_version()
-            output = stdout_cap.getvalue()
-            _pr_output(output)
-            logger.info("Check version failures: %s", output)
+        _check_msticpy_version()
 
     if _detect_env("synapse", **kwargs) and is_in_synapse():
         synapse_params = {
             key: val for key, val in kwargs.items() if key in _SYNAPSE_KWARGS
         }
-        init_synapse(**synapse_params)
+        try:
+            init_synapse(**synapse_params)
+        except Exception as err:  # pylint: disable=broad-except
+            logger.warning("Error initializing Synapse environment: %s", err)
 
     # Handle required packages and imports
     _pr_output("Processing imports....")
-    stdout_cap = io.StringIO()
-    with redirect_stdout(stdout_cap):
-        imp_ok = _global_imports(
-            namespace, additional_packages, user_install, extra_imports, def_imports
-        )
-        output = stdout_cap.getvalue()
-        _pr_output(output)
-        logger.info("Import failures: %s", output)
+    imp_ok = _import_packages(
+        namespace, def_imports, additional_packages, extra_imports, user_install
+    )
 
     # Configuration check
     if no_config_check:
         conf_ok = True
     else:
         _pr_output("Checking configuration....")
         conf_ok = _get_or_create_config()
@@ -458,44 +423,114 @@
         if _VERBOSITY() == 2:  # type: ignore
             _pr_output("Friendly exceptions enabled.")
         InteractiveShell.showtraceback = _hook_ipython_exceptions(  # type: ignore
             InteractiveShell.showtraceback
         )
 
     # load pivots
-    stdout_cap = io.StringIO()
-    with redirect_stdout(stdout_cap):
-        _pr_output("Loading pivots.")
-        _load_pivots(namespace=namespace)
-        output = stdout_cap.getvalue()
-        _pr_output(output)
-        logger.info("Pivot load failures: %s", output)
+    _load_pivot_functions(namespace)
 
     # User defaults
+    _load_user_defaults(namespace)
+
+    # show any warnings
+    _show_init_warnings(imp_ok, conf_ok)
+    _pr_output("<h4>Notebook initialization complete</h4>")
+    logger.info("Notebook initialization complete")
+
+
+def _pr_output(*args):
+    """Output to IPython display or print."""
+    if not _VERBOSITY():
+        return
+    if is_ipython():
+        display(HTML(" ".join([*args, "<br>"]).replace("\n", "<br>")))
+    else:
+        print(*args)
+
+
+def _err_output(*args):
+    """Output to IPython display or print - always output regardless of verbosity."""
+    if is_ipython():
+        display(HTML(" ".join([*args, "<br>"]).replace("\n", "<br>")))
+        display(
+            HTML(
+                "For more info and options run:"
+                "<pre>import msticpy as mp\nhelp(mp.nbinit)</pre>"
+            )
+        )
+    else:
+        print(*args)
+        print(
+            "\nFor more info and options run:",
+            "\n    import msticpy as mp",
+            "\n    help(mp.nbinit)",
+        )
+
+
+def _load_user_defaults(namespace):
+    """Load user defaults, if defined."""
+    global current_providers  # pylint: disable=global-statement, invalid-name
     stdout_cap = io.StringIO()
     with redirect_stdout(stdout_cap):
         _pr_output("Loading user defaults.")
         prov_dict = load_user_defaults()
         output = stdout_cap.getvalue()
-        _pr_output(output)
-        logger.info(output)
-        logger.info("User default load failures: %s", output)
+        if output.strip():
+            _pr_output(output)
+            logger.info(output)
+            logger.info("User default load failures: %s", output)
 
     if prov_dict:
         namespace.update(prov_dict)
         current_providers = prov_dict
         _pr_output("Auto-loaded components:", ", ".join(prov_dict.keys()))
 
-    # show any warnings
-    _show_init_warnings(imp_ok, conf_ok)
-    _pr_output("<h4>Notebook initialization complete</h4>")
-    logger.info("Notebook initialization complete")
+
+def _load_pivot_functions(namespace):
+    """Load pivot functions."""
+    stdout_cap = io.StringIO()
+    with redirect_stdout(stdout_cap):
+        _pr_output("Loading pivots.")
+        _load_pivots(namespace=namespace)
+        output = stdout_cap.getvalue()
+        if output.strip():
+            _pr_output(output)
+            logger.info("Pivot load failures: %s", output)
+
+
+def _import_packages(
+    namespace, def_imports, additional_packages, extra_imports, user_install
+):
+    """Import packages from default set or supplied as parameters."""
+    stdout_cap = io.StringIO()
+    with redirect_stdout(stdout_cap):
+        imp_ok = _global_imports(
+            namespace, additional_packages, user_install, extra_imports, def_imports
+        )
+        output = stdout_cap.getvalue()
+        if output.strip():
+            _pr_output(output)
+            logger.info("Import failures: %s", output)
+    return imp_ok
+
+
+def _check_msticpy_version():
+    """Check msticpy version."""
+    stdout_cap = io.StringIO()
+    with redirect_stdout(stdout_cap):
+        check_version()
+        output = stdout_cap.getvalue()
+        if output.strip():
+            _pr_output(output)
+            logger.info("Check version failures: %s", output)
 
 
 def _show_init_warnings(imp_ok, conf_ok):
+    """Show any warnings from init_notebook."""
     if imp_ok and conf_ok:
         return True
     md("<font color='orange'><h3>Notebook setup completed with some warnings.</h3>")
     if not imp_ok:
         md("One or more libraries did not import successfully.")
         md(_AZNB_GUIDE)
     if not conf_ok:
@@ -576,14 +611,15 @@
 def _global_imports(
     namespace: Dict[str, Any],
     additional_packages: List[str] = None,
     user_install: bool = False,
     extra_imports: List[str] = None,
     def_imports: str = "all",
 ):
+    """Import packages from default set (defined statically)."""
     import_list = []
     imports, imports_all = _build_import_list(def_imports)
 
     for imp_pkg in imports:
         try:
             _imp_from_package(nm_spc=namespace, **imp_pkg)
             import_list.append(_extract_pkg_name(imp_pkg))
```

### Comparing `msticpy-2.8.0rc1/msticpy/init/nbmagics.py` & `msticpy-2.9.0/msticpy/init/nbmagics.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/init/pivot.py` & `msticpy-2.9.0/msticpy/init/pivot.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,28 +11,26 @@
 from importlib import import_module
 from pathlib import Path
 from types import ModuleType
 from typing import Any, Callable, Dict, Iterable, Optional, Type
 
 import pkg_resources
 
-# pylint: disable=unused-import
-from .. import datamodel  # noqa:F401
 from .._version import VERSION
 from ..common.timespan import TimeSpan
 from ..context.tilookup import TILookup
-from ..data import QueryProvider
+from ..data.core.data_providers import QueryProvider
 from ..datamodel import entities
 
 with warnings.catch_warnings():
     warnings.simplefilter("ignore", category=DeprecationWarning)
     from ..datamodel import pivot as legacy_pivot
 
 from ..common.utility.types import SingletonClass
-from ..nbwidgets import QueryTime
+from ..nbwidgets.query_time import QueryTime
 from . import pivot_init
 
 # pylint: disable=unused-import, no-name-in-module
 from .pivot_core import pivot_pd_accessor  # noqa: F401
 from .pivot_core.pivot_browser import PivotBrowser
 from .pivot_core.pivot_register import PivotRegistration
 from .pivot_core.pivot_register_reader import (
@@ -424,17 +422,19 @@
         else:
             entity_names = [entity]
         for entity_name in entity_names:
             entity_cls = getattr(entities, entity_name)
             for attr in dir(entity_cls):
                 attr_obj = getattr(entity_cls, attr)
                 if type(attr_obj).__name__ == "PivotContainer":
-                    delattr(entity_cls, attr)
+                    with contextlib.suppress(AttributeError):
+                        delattr(entity_cls, attr)
                 if callable(attr_obj) and hasattr(attr_obj, "pivot_properties"):
-                    delattr(entity_cls, attr)
+                    with contextlib.suppress(AttributeError):
+                        delattr(entity_cls, attr)
 
     @staticmethod
     def browse():
         """Return PivotBrowser."""
         return PivotBrowser()
```

### Comparing `msticpy-2.8.0rc1/msticpy/init/pivot_core/pivot_browser.py` & `msticpy-2.9.0/msticpy/init/pivot_core/pivot_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/init/pivot_core/pivot_container.py` & `msticpy-2.9.0/msticpy/init/pivot_core/pivot_container.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/init/pivot_core/pivot_magic_core.py` & `msticpy-2.9.0/msticpy/init/pivot_core/pivot_magic_core.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/init/pivot_core/pivot_pd_accessor.py` & `msticpy-2.9.0/msticpy/init/pivot_core/pivot_pd_accessor.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/init/pivot_core/pivot_pipeline.py` & `msticpy-2.9.0/msticpy/init/pivot_core/pivot_pipeline.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/init/pivot_core/pivot_register.py` & `msticpy-2.9.0/msticpy/init/pivot_core/pivot_register.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/init/pivot_core/pivot_register_reader.py` & `msticpy-2.9.0/msticpy/init/pivot_core/pivot_register_reader.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/init/pivot_init/pivot_data_queries.py` & `msticpy-2.9.0/msticpy/init/pivot_init/pivot_data_queries.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/init/pivot_init/pivot_ti_provider.py` & `msticpy-2.9.0/msticpy/init/pivot_init/pivot_ti_provider.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/init/pivot_init/vt_pivot.py` & `msticpy-2.9.0/msticpy/init/pivot_init/vt_pivot.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/init/user_config.py` & `msticpy-2.9.0/msticpy/init/user_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
         az_data.connect(**connect_args)
         print("Connected. ", end="")
     return "az_data", az_data
 
 
 def _load_azsent_api(comp_settings=None, **kwargs):
     del kwargs
-    from ..context.azure import MicrosoftSentinel
+    from ..context.azure.sentinel_core import MicrosoftSentinel
 
     res_id = comp_settings.pop("res_id", None)
     if res_id:
         az_sent = MicrosoftSentinel(res_id=res_id)
     else:
         az_sent = MicrosoftSentinel()
     connect = comp_settings.pop("connect", True)
```

### Comparing `msticpy-2.8.0rc1/msticpy/nbtools/data_viewer.py` & `msticpy-2.9.0/msticpy/nbtools/data_viewer.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/nbtools/entityschema.py` & `msticpy-2.9.0/msticpy/nbtools/entityschema.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/nbtools/foliummap.py` & `msticpy-2.9.0/msticpy/nbtools/foliummap.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/nbtools/morph_charts.py` & `msticpy-2.9.0/msticpy/nbtools/morph_charts.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/nbtools/nbdisplay.py` & `msticpy-2.9.0/msticpy/nbtools/nbdisplay.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/nbtools/nbwidgets.py` & `msticpy-2.9.0/msticpy/nbtools/nbwidgets.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/nbtools/observationlist.py` & `msticpy-2.9.0/msticpy/nbtools/observationlist.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/nbtools/process_tree.py` & `msticpy-2.9.0/msticpy/nbtools/process_tree.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/nbtools/security_alert.py` & `msticpy-2.9.0/msticpy/nbtools/security_alert.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/nbtools/security_alert_graph.py` & `msticpy-2.9.0/msticpy/nbtools/security_alert_graph.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/nbtools/security_base.py` & `msticpy-2.9.0/msticpy/nbtools/security_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/nbtools/security_event.py` & `msticpy-2.9.0/msticpy/nbtools/security_event.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/nbtools/ti_browser.py` & `msticpy-2.9.0/msticpy/nbtools/ti_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/nbtools/timeline.py` & `msticpy-2.9.0/msticpy/nbtools/timeline.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/nbtools/timeline_duration.py` & `msticpy-2.9.0/msticpy/nbtools/timeline_duration.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/nbtools/timeline_pd_accessor.py` & `msticpy-2.9.0/msticpy/nbtools/timeline_pd_accessor.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/nbtools/timeseries.py` & `msticpy-2.9.0/msticpy/nbtools/timeseries.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/nbtools/utility.py` & `msticpy-2.9.0/msticpy/nbtools/utility.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/nbtools/wsconfig.py` & `msticpy-2.9.0/msticpy/nbtools/wsconfig.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/nbwidgets/core.py` & `msticpy-2.9.0/msticpy/nbwidgets/core.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/nbwidgets/get_environment_key.py` & `msticpy-2.9.0/msticpy/nbwidgets/get_environment_key.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/nbwidgets/get_text.py` & `msticpy-2.9.0/msticpy/nbwidgets/get_text.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/nbwidgets/lookback.py` & `msticpy-2.9.0/msticpy/nbwidgets/lookback.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/nbwidgets/option_buttons.py` & `msticpy-2.9.0/msticpy/nbwidgets/option_buttons.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/nbwidgets/progress.py` & `msticpy-2.9.0/msticpy/nbwidgets/progress.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/nbwidgets/query_time.py` & `msticpy-2.9.0/msticpy/nbwidgets/query_time.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/nbwidgets/select_alert.py` & `msticpy-2.9.0/msticpy/nbwidgets/select_alert.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/nbwidgets/select_item.py` & `msticpy-2.9.0/msticpy/nbwidgets/select_item.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/nbwidgets/select_subset.py` & `msticpy-2.9.0/msticpy/nbwidgets/select_subset.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/resources/WinSecurityEvent.json` & `msticpy-2.9.0/msticpy/resources/WinSecurityEvent.json`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/resources/mp_pivot_reg.yaml` & `msticpy-2.9.0/msticpy/resources/mp_pivot_reg.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/resources/mpconfig_defaults.yaml` & `msticpy-2.9.0/msticpy/resources/mpconfig_defaults.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,19 @@
       ApiID: str()
       AuthKey: *cred_key
   Pulsedive:
     Args:
       AuthKey: *cred_key
     Primary: bool(default=False)
     Provider: "Pulsedive"
+  IPQualityScore:
+    Args:
+      AuthKey: *cred_key
+    Primary: bool(default=False)
+    Provider: "IPQualityScore"
 OtherProviders:
   GeoIPLite:
     Args:
       AuthKey: *cred_key
       DBFolder: str(default="~/.msticpy")
     Provider: "GeoLiteLookup"
   IPStack:
```

### Comparing `msticpy-2.8.0rc1/msticpy/resources/obfuscation_cols.yaml` & `msticpy-2.9.0/msticpy/resources/obfuscation_cols.yaml`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/sectools/__init__.py` & `msticpy-2.9.0/msticpy/sectools/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,24 +27,22 @@
 - proc_tree_utils -> msticpy.transform
 - sectools_magics -> msticpy.init.nbmagics
 - syslog_utils -> msticpy.analysis
 
 The sectools sub-package will be removed in version 2.0.0
 
 """
-import contextlib
-
-# from . import process_tree_utils as ptree
 from .._version import VERSION
-from ..context.geoip import GeoLiteLookup, IPStackLookup, geo_distance
-from ..context.tilookup import TILookup
-from ..transform import base64unpack as base64
+from ..lazy_importer import lazy_import
 
-# flake8: noqa: F403
-# pylint: disable=W0401
-from ..transform.iocextract import IoCExtract
+__version__ = VERSION
 
-with contextlib.suppress(ImportError):
-    from IPython import get_ipython
+_LAZY_IMPORTS = {
+    "msticpy.context.geoip.GeoLiteLookup",
+    "msticpy.context.geoip.IPStackLookup",
+    "msticpy.context.geoip.geo_distance",
+    "msticpy.context.tilookup.TILookup",
+    "msticpy.transform.base64unpack as base64",
+    "msticpy.transform.iocextract.IoCExtract",
+}
 
-    from ..init import nbmagics as sectool_magics
-__version__ = VERSION
+module, __getattr__, __dir__ = lazy_import(__name__, _LAZY_IMPORTS)
```

### Comparing `msticpy-2.8.0rc1/msticpy/sectools/auditdextract.py` & `msticpy-2.9.0/msticpy/sectools/auditdextract.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/sectools/base64unpack.py` & `msticpy-2.9.0/msticpy/sectools/base64unpack.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/sectools/cmd_line.py` & `msticpy-2.9.0/msticpy/sectools/cmd_line.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/sectools/domain_utils.py` & `msticpy-2.9.0/msticpy/sectools/domain_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/sectools/eventcluster.py` & `msticpy-2.9.0/msticpy/sectools/eventcluster.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/sectools/geoip.py` & `msticpy-2.9.0/msticpy/sectools/geoip.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/sectools/iocextract.py` & `msticpy-2.9.0/msticpy/sectools/iocextract.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/sectools/ip_utils.py` & `msticpy-2.9.0/msticpy/sectools/ip_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/sectools/proc_tree_build_mde.py` & `msticpy-2.9.0/msticpy/sectools/proc_tree_build_mde.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/sectools/proc_tree_build_winlx.py` & `msticpy-2.9.0/msticpy/sectools/proc_tree_build_winlx.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/sectools/proc_tree_builder.py` & `msticpy-2.9.0/msticpy/sectools/proc_tree_builder.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/sectools/proc_tree_schema.py` & `msticpy-2.9.0/msticpy/sectools/proc_tree_schema.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/sectools/proc_tree_utils.py` & `msticpy-2.9.0/msticpy/sectools/proc_tree_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/sectools/sectools_magics.py` & `msticpy-2.9.0/msticpy/sectools/sectools_magics.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/sectools/syslog_utils.py` & `msticpy-2.9.0/msticpy/sectools/syslog_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/sectools/tilookup.py` & `msticpy-2.9.0/msticpy/sectools/tilookup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/sectools/tiproviders/ti_provider_base.py` & `msticpy-2.9.0/msticpy/sectools/tiproviders/ti_provider_base.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/sectools/vtlookup.py` & `msticpy-2.9.0/msticpy/sectools/vtlookup.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/sectools/vtlookupv3/vtfile_behavior.py` & `msticpy-2.9.0/msticpy/sectools/vtlookupv3/vtfile_behavior.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/sectools/vtlookupv3/vtlookupv3.py` & `msticpy-2.9.0/msticpy/sectools/vtlookupv3/vtlookupv3.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/sectools/vtlookupv3/vtobject_browser.py` & `msticpy-2.9.0/msticpy/sectools/vtlookupv3/vtobject_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/transform/auditdextract.py` & `msticpy-2.9.0/msticpy/transform/auditdextract.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/transform/base64unpack.py` & `msticpy-2.9.0/msticpy/transform/base64unpack.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/transform/cmd_line.py` & `msticpy-2.9.0/msticpy/transform/cmd_line.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/transform/iocextract.py` & `msticpy-2.9.0/msticpy/transform/iocextract.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/transform/network.py` & `msticpy-2.9.0/msticpy/transform/network.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/transform/proc_tree_build_mde.py` & `msticpy-2.9.0/msticpy/transform/proc_tree_build_mde.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/transform/proc_tree_build_winlx.py` & `msticpy-2.9.0/msticpy/transform/proc_tree_build_winlx.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,15 @@
 
 
 def _extract_inferred_parents(
     merged_procs: pd.DataFrame, schema: "ProcSchema"  # type: ignore  # noqa: F821
 ) -> pd.DataFrame:
     """Find any inferred parents and creates rows for them."""
     tz_aware = merged_procs.iloc[0][schema.time_stamp].tz
-    time_zero = pd.Timestamp(0) if tz_aware is None else pd.Timestamp(0, tz=0)
+    time_zero = pd.Timestamp(0) if tz_aware is None else pd.Timestamp(0, tz=tz_aware)
 
     # Fill in missing values for root processes
     root_procs_crit = merged_procs[Col.source_index_par].isna()
     merged_procs.loc[root_procs_crit, "NewProcessId_par"] = merged_procs[
         schema.parent_id
     ]
     parent_col_name = schema.parent_name or "ParentName"
```

### Comparing `msticpy-2.8.0rc1/msticpy/transform/proc_tree_builder.py` & `msticpy-2.9.0/msticpy/transform/proc_tree_builder.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/transform/proc_tree_schema.py` & `msticpy-2.9.0/msticpy/transform/proc_tree_schema.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/transform/process_tree_utils.py` & `msticpy-2.9.0/msticpy/transform/process_tree_utils.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/vis/__init__.py` & `msticpy-2.9.0/msticpy/vis/__init__.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/vis/code_view.py` & `msticpy-2.9.0/msticpy/vis/code_view.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/vis/data_viewer.py` & `msticpy-2.9.0/msticpy/vis/data_viewer.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/vis/data_viewer_panel.py` & `msticpy-2.9.0/msticpy/vis/data_viewer_panel.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         Other Parameters
         ----------------
         selectable : Union[bool, str], optional
             Whether rows should be selectable, by default "checkbox"
         show_index : bool, optional
             If True show the DataFrame index as a column, by default  True.
         show_tenant_id : bool, optional
-            If True show the TenantId column, by default  True.
+            If True show the TenantId column, by default False.
         max_col_width : int, optional
             Sets the maximum column width to display, by default 500
         detail_cols : List[str]
             List of columns for which details are displayed in collapsible
             field beneath each table row.
         kwargs :
             Other keyword arguments are passed to the panel
@@ -81,24 +81,30 @@
             )
         if data.empty:
             raise ValueError("No data available in 'data'")
 
         # Drop empty columns
         self.data = data.dropna(axis="columns", how="all")
         # Set up hidden columns
-        self._hidden_columns = self._default_hidden_cols(selected_cols, **kwargs)
-        if kwargs.pop("hide_tenantid", False) and "TenantId" in self._hidden_columns:
+        hidden_cols = kwargs.pop("hidden_cols", None)
+        self._hidden_columns = self._default_hidden_cols(selected_cols, hidden_cols)
+
+        if (
+            not kwargs.pop("show_tenant_id", False)
+            and "TenantId" in self._hidden_columns
+        ):
             self._hidden_columns.remove("TenantId")
+
         # Create the tabulator control
         self.data_table = pn.widgets.Tabulator(
             self.data,
             header_filters=kwargs.pop("header_filters", True),
             selectable=kwargs.pop("selectable", "checkbox"),
             show_index=kwargs.pop("show_index", False),
-            configuration=self._create_configuration(),
+            configuration=self._create_configuration(kwargs),
             pagination="local",
             row_content=self._create_row_formatter(kwargs.pop("detail_cols", None)),
             embed_content=False,
             height=kwargs.pop("height", self._DEF_HEIGHT),
             **kwargs,
         )
         # Add the column chooser
@@ -143,40 +149,40 @@
     ) -> Optional[Callable]:
         """Build formatter function for row-details."""
         if not detail_columns:
             return None
         row_view_cols = set(detail_columns) & set(self.data.columns)
         return partial(_display_column_details, columns=row_view_cols)
 
-    def _create_configuration(self, **kwargs) -> Dict[str, Any]:
+    def _create_configuration(self, kwargs) -> Dict[str, Any]:
         """Create Tabulator configuration dict to pass to JS Tabulator."""
         return {
             "columnDefaults": {"maxWidth": kwargs.pop("max_col_width", 500)},
             "clipboardCopyRowRange": "selected",
             "clipboardCopyConfig": {
                 "columnHeaders": True,
                 "columnGroups": False,
                 "rowGroups": False,
                 "columnCalcs": False,
                 "dataTree": False,
                 "formatCells": False,
             },
         }
 
-    def _default_hidden_cols(self, selected_cols, **kwargs) -> List[str]:
+    def _default_hidden_cols(self, selected_cols, hidden_cols) -> List[str]:
         """Return list of of columns hidden by default."""
         return [
             hidden_col
             for hidden_col in self._DEFAULT_HIDDEN_COLS
             if (
                 hidden_col in self.data.columns
                 and selected_cols
                 and hidden_col not in selected_cols
             )
-        ] + (kwargs.pop("hidden_cols", None) or [])
+        ] + (hidden_cols or [])
 
 
 class DataTableColumnChooser:
     """DataTableColumnChooser class."""
 
     def __init__(self, data, selected_cols=None):
         """Initialize the DataTableColumnChooser class."""
```

### Comparing `msticpy-2.8.0rc1/msticpy/vis/entity_graph_tools.py` & `msticpy-2.9.0/msticpy/vis/entity_graph_tools.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/vis/figure_dimension.py` & `msticpy-2.9.0/msticpy/vis/figure_dimension.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/vis/foliummap.py` & `msticpy-2.9.0/msticpy/vis/foliummap.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/vis/matrix_plot.py` & `msticpy-2.9.0/msticpy/vis/matrix_plot.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/vis/mordor_browser.py` & `msticpy-2.9.0/msticpy/vis/mordor_browser.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/vis/morph_charts.py` & `msticpy-2.9.0/msticpy/vis/morph_charts.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/vis/mp_pandas_plot.py` & `msticpy-2.9.0/msticpy/vis/mp_pandas_plot.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/vis/nbdisplay.py` & `msticpy-2.9.0/msticpy/vis/nbdisplay.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/vis/network_plot.py` & `msticpy-2.9.0/msticpy/vis/network_plot.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/vis/process_tree.py` & `msticpy-2.9.0/msticpy/vis/process_tree.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/vis/query_browser.py` & `msticpy-2.9.0/msticpy/vis/query_browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """QueryProvider Query Browser."""
 import textwrap
 from typing import Any, Generator
 
 from IPython.display import HTML
 
 from .._version import VERSION
-from ..nbwidgets import SelectItem
+from ..nbwidgets.select_item import SelectItem
 
 __version__ = VERSION
 __author__ = "Ian Hellen"
 
 
 def browse_queries(query_provider: Any, **kwargs) -> SelectItem:
     """
```

### Comparing `msticpy-2.8.0rc1/msticpy/vis/ti_browser.py` & `msticpy-2.9.0/msticpy/vis/ti_browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import pprint
 from typing import List, Union
 
 import pandas as pd
 from IPython.display import HTML
 
 from .._version import VERSION
-from ..nbwidgets import SelectItem
+from ..nbwidgets.select_item import SelectItem
 
 __version__ = VERSION
 __author__ = "Ian Hellen"
 
 
 def browse_results(
     data: pd.DataFrame, severities: Union[List[str], str, None] = None, **kwargs
```

### Comparing `msticpy-2.8.0rc1/msticpy/vis/timeline.py` & `msticpy-2.9.0/msticpy/vis/timeline.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/vis/timeline_common.py` & `msticpy-2.9.0/msticpy/vis/timeline_common.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/vis/timeline_duration.py` & `msticpy-2.9.0/msticpy/vis/timeline_duration.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/vis/timeline_pd_accessor.py` & `msticpy-2.9.0/msticpy/vis/timeline_pd_accessor.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/vis/timeline_values.py` & `msticpy-2.9.0/msticpy/vis/timeline_values.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/vis/timeseries.py` & `msticpy-2.9.0/msticpy/vis/timeseries.py`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/msticpy/vis/vtobject_browser.py` & `msticpy-2.9.0/msticpy/vis/vtobject_browser.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import Dict, Optional
 
 import ipywidgets as widgets
 import pandas as pd
 
 from .._version import VERSION
 from ..context.vtlookupv3.vtlookupv3 import VTLookupV3, timestamps_to_utcdate
-from ..nbwidgets import IPyDisplayMixin
+from ..nbwidgets.core import IPyDisplayMixin
 
 __version__ = VERSION
 __author__ = "Ian Hellen"
 
 
 _NOT_FOUND = "Not found"
 
@@ -26,14 +26,15 @@
         "border": "solid gray 1px",
         "margin": "1pt",
         "padding": "5pt",
     }
 )
 
 
+# pylint: disable=too-few-public-methods
 class VTObjectBrowser(IPyDisplayMixin):
     """VirusTotal object attributes browser."""
 
     _BASIC_TITLE = "VirusTotal File hash lookup"
 
     def __init__(self, file_id: Optional[str] = None):
         """
```

### Comparing `msticpy-2.8.0rc1/msticpy.egg-info/PKG-INFO` & `msticpy-2.9.0/msticpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msticpy
-Version: 2.8.0rc1
+Version: 2.9.0
 Summary: MSTIC Security Tools
 Home-page: https://github.com/microsoft/msticpy
 Author: Ian Hellen
 Author-email: ianhelle@microsoft.com
 Maintainer: Pete Bryan
 Maintainer-email: peter.bryan@microsoft.com
 License: MIT License
@@ -102,19 +102,19 @@
 Requires-Dist: pygeohash>=1.2.0; extra == "dev"
 Requires-Dist: pylint>=2.5.3; extra == "dev"
 Requires-Dist: pyroma>=3.1; extra == "dev"
 Requires-Dist: pytest-check>=1.0.1; extra == "dev"
 Requires-Dist: pytest-cov>=2.11.1; extra == "dev"
 Requires-Dist: pytest-xdist>=2.5.0; extra == "dev"
 Requires-Dist: pytest>=5.0.1; extra == "dev"
-Requires-Dist: readthedocs-sphinx-ext==2.2.2; extra == "dev"
+Requires-Dist: readthedocs-sphinx-ext==2.2.3; extra == "dev"
 Requires-Dist: responses>=0.13.2; extra == "dev"
 Requires-Dist: respx>=0.20.1; extra == "dev"
 Requires-Dist: sphinx-rtd-theme>=1.0.0; extra == "dev"
-Requires-Dist: sphinx>=5.0.1; extra == "dev"
+Requires-Dist: sphinx<8.0.0,>=5.0.1; extra == "dev"
 Requires-Dist: types-attrs>=19.0.0; extra == "dev"
 Provides-Extra: vt3
 Requires-Dist: vt-py>=0.6.1; extra == "vt3"
 Requires-Dist: vt-graph-api>=2.0; extra == "vt3"
 Requires-Dist: nest_asyncio>=1.4.0; extra == "vt3"
 Provides-Extra: splunk
 Requires-Dist: splunk-sdk>=1.6.0; extra == "splunk"
@@ -216,21 +216,21 @@
 Requires-Dist: pygeohash>=1.2.0; extra == "test"
 Requires-Dist: pylint>=2.5.3; extra == "test"
 Requires-Dist: pyroma>=3.1; extra == "test"
 Requires-Dist: pytest-check>=1.0.1; extra == "test"
 Requires-Dist: pytest-cov>=2.11.1; extra == "test"
 Requires-Dist: pytest-xdist>=2.5.0; extra == "test"
 Requires-Dist: pytest>=5.0.1; extra == "test"
-Requires-Dist: readthedocs-sphinx-ext==2.2.2; extra == "test"
+Requires-Dist: readthedocs-sphinx-ext==2.2.3; extra == "test"
 Requires-Dist: responses>=0.13.2; extra == "test"
 Requires-Dist: respx>=0.20.1; extra == "test"
 Requires-Dist: scikit-learn>=1.0.0; extra == "test"
 Requires-Dist: scipy>=1.1.0; extra == "test"
 Requires-Dist: sphinx-rtd-theme>=1.0.0; extra == "test"
-Requires-Dist: sphinx>=5.0.1; extra == "test"
+Requires-Dist: sphinx<8.0.0,>=5.0.1; extra == "test"
 Requires-Dist: splunk-sdk>=1.6.0; extra == "test"
 Requires-Dist: statsmodels>=0.11.1; extra == "test"
 Requires-Dist: sumologic-sdk>=0.1.11; extra == "test"
 Requires-Dist: types-attrs>=19.0.0; extra == "test"
 Requires-Dist: vt-graph-api>=2.0; extra == "test"
 Requires-Dist: vt-py>=0.6.1; extra == "test"
 Provides-Extra: azsentinel
```

### Comparing `msticpy-2.8.0rc1/msticpy.egg-info/SOURCES.txt` & `msticpy-2.9.0/msticpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 requirements-all.txt
 requirements-dev.txt
 requirements.txt
 setup.cfg
 setup.py
 msticpy/__init__.py
 msticpy/_version.py
+msticpy/lazy_importer.py
 msticpy/msticpyconfig.yaml
 msticpy.egg-info/PKG-INFO
 msticpy.egg-info/SOURCES.txt
 msticpy.egg-info/dependency_links.txt
 msticpy.egg-info/not-zip-safe
 msticpy.egg-info/requires.txt
 msticpy.egg-info/top_level.txt
@@ -116,14 +117,15 @@
 msticpy/context/tiproviders/abuseipdb.py
 msticpy/context/tiproviders/alienvault_otx.py
 msticpy/context/tiproviders/azure_sent_byoti.py
 msticpy/context/tiproviders/crowdsec.py
 msticpy/context/tiproviders/greynoise.py
 msticpy/context/tiproviders/ibm_xforce.py
 msticpy/context/tiproviders/intsights.py
+msticpy/context/tiproviders/ip_quality_score.py
 msticpy/context/tiproviders/kql_base.py
 msticpy/context/tiproviders/mblookup.py
 msticpy/context/tiproviders/open_page_rank.py
 msticpy/context/tiproviders/pulsedive.py
 msticpy/context/tiproviders/result_severity.py
 msticpy/context/tiproviders/riskiq.py
 msticpy/context/tiproviders/ti_http_provider.py
@@ -243,20 +245,23 @@
 msticpy/datamodel/entities/host.py
 msticpy/datamodel/entities/host_logon_session.py
 msticpy/datamodel/entities/iot_device.py
 msticpy/datamodel/entities/ip_address.py
 msticpy/datamodel/entities/mail_cluster.py
 msticpy/datamodel/entities/mail_message.py
 msticpy/datamodel/entities/mailbox.py
+msticpy/datamodel/entities/mailbox_configuration.py
 msticpy/datamodel/entities/malware.py
 msticpy/datamodel/entities/network_connection.py
+msticpy/datamodel/entities/oauth_application.py
 msticpy/datamodel/entities/process.py
 msticpy/datamodel/entities/registry_key.py
 msticpy/datamodel/entities/registry_value.py
 msticpy/datamodel/entities/security_group.py
+msticpy/datamodel/entities/service_principal.py
 msticpy/datamodel/entities/submission_mail.py
 msticpy/datamodel/entities/threat_intelligence.py
 msticpy/datamodel/entities/unknown_entity.py
 msticpy/datamodel/entities/url.py
 msticpy/datamodel/soc/__init__.py
 msticpy/datamodel/soc/incident.py
 msticpy/datamodel/soc/sentinel_alert.py
```

### Comparing `msticpy-2.8.0rc1/msticpy.egg-info/requires.txt` & `msticpy-2.9.0/msticpy.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -136,19 +136,19 @@
 pygeohash>=1.2.0
 pylint>=2.5.3
 pyroma>=3.1
 pytest-check>=1.0.1
 pytest-cov>=2.11.1
 pytest-xdist>=2.5.0
 pytest>=5.0.1
-readthedocs-sphinx-ext==2.2.2
+readthedocs-sphinx-ext==2.2.3
 responses>=0.13.2
 respx>=0.20.1
 sphinx-rtd-theme>=1.0.0
-sphinx>=5.0.1
+sphinx<8.0.0,>=5.0.1
 types-attrs>=19.0.0
 
 [keyvault]
 
 [kql]
 KqlmagicCustom[jupyter-extended]>=0.1.114.post22
 
@@ -226,21 +226,21 @@
 pygeohash>=1.2.0
 pylint>=2.5.3
 pyroma>=3.1
 pytest-check>=1.0.1
 pytest-cov>=2.11.1
 pytest-xdist>=2.5.0
 pytest>=5.0.1
-readthedocs-sphinx-ext==2.2.2
+readthedocs-sphinx-ext==2.2.3
 responses>=0.13.2
 respx>=0.20.1
 scikit-learn>=1.0.0
 scipy>=1.1.0
 sphinx-rtd-theme>=1.0.0
-sphinx>=5.0.1
+sphinx<8.0.0,>=5.0.1
 splunk-sdk>=1.6.0
 statsmodels>=0.11.1
 sumologic-sdk>=0.1.11
 types-attrs>=19.0.0
 vt-graph-api>=2.0
 vt-py>=0.6.1
```

### Comparing `msticpy-2.8.0rc1/requirements-all.txt` & `msticpy-2.9.0/requirements-all.txt`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/requirements-dev.txt` & `msticpy-2.9.0/requirements-dev.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,13 +25,13 @@
 pygeohash>=1.2.0
 pylint>=2.5.3
 pyroma>=3.1
 pytest-check>=1.0.1
 pytest-cov>=2.11.1
 pytest-xdist>=2.5.0
 pytest>=5.0.1
-readthedocs-sphinx-ext==2.2.2
+readthedocs-sphinx-ext==2.2.3
 responses>=0.13.2
 respx>=0.20.1
 sphinx-rtd-theme>=1.0.0
-sphinx>=5.0.1
+sphinx>=5.0.1,<8.0.0
 types-attrs>=19.0.0
```

### Comparing `msticpy-2.8.0rc1/requirements.txt` & `msticpy-2.9.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/setup.cfg` & `msticpy-2.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `msticpy-2.8.0rc1/setup.py` & `msticpy-2.9.0/setup.py`

 * *Files identical despite different names*

