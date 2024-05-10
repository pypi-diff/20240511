# Comparing `tmp/pulumi_fastly-8.7.0a1715303918.tar.gz` & `tmp/pulumi_fastly-8.7.0a1715351477.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_fastly-8.7.0a1715303918.tar", last modified: Fri May 10 01:31:40 2024, max compression
+gzip compressed data, was "pulumi_fastly-8.7.0a1715351477.tar", last modified: Fri May 10 14:36:08 2024, max compression
```

## Comparing `pulumi_fastly-8.7.0a1715303918.tar` & `pulumi_fastly-8.7.0a1715351477.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:31:40.555321 pulumi_fastly-8.7.0a1715303918/
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-10 01:31:40.555321 pulumi_fastly-8.7.0a1715303918/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:31:40.555321 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   521901 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    24103 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/alert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:31:40.555321 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    12973 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/configstore.py
--rw-r--r--   0 runner    (1001) docker     (127)     9889 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/configstore_entries.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_configstores.py
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_datacenters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_fastly_ip_ranges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_kvstores.py
--rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_package_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_secretstores.py
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_activation_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     9816 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_certificate_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_configuration_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_platform_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_platform_certificate_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_private_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_private_key_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     8313 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_subscription_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_vcl_snippets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_waf_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    13864 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/kvstore.py
--rw-r--r--   0 runner    (1001) docker     (127)   472074 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10266 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/secretstore.py
--rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/service_acl_entries.py
--rw-r--r--   0 runner    (1001) docker     (127)    11719 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/service_authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    92401 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/service_compute.py
--rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/service_dictionary_items.py
--rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/service_dynamic_snippet_content.py
--rw-r--r--   0 runner    (1001) docker     (127)   121205 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/service_vcl.py
--rw-r--r--   0 runner    (1001) docker     (127)    91888 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/service_waf_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    17972 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/tls_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)    22949 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)    20467 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/tls_mutual_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)    25864 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/tls_platform_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)    14407 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/tls_private_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/tls_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/tls_subscription_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11638 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:31:40.555321 pulumi_fastly-8.7.0a1715303918/pulumi_fastly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-10 01:31:40.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-10 01:31:40.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 01:31:40.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 01:31:40.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 01:31:40.000000 pulumi_fastly-8.7.0a1715303918/pulumi_fastly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-10 01:31:34.000000 pulumi_fastly-8.7.0a1715303918/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 01:31:40.555321 pulumi_fastly-8.7.0a1715303918/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:36:08.398364 pulumi_fastly-8.7.0a1715351477/
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-10 14:36:08.398364 pulumi_fastly-8.7.0a1715351477/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:36:08.398364 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   522888 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24377 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/alert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:36:08.398364 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12973 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/configstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9889 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/configstore_entries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_configstores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_datacenters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_fastly_ip_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_kvstores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_package_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_secretstores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_tls_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_tls_activation_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9816 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_tls_certificate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_tls_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_tls_configuration_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_tls_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_tls_platform_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_tls_platform_certificate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_tls_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_tls_private_key_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8313 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_tls_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_tls_subscription_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_vcl_snippets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_waf_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15807 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13864 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)   473470 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10266 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/secretstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/service_acl_entries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11719 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/service_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92401 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/service_compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/service_dictionary_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/service_dynamic_snippet_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)   121205 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/service_vcl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91888 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/service_waf_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17972 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/tls_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22949 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20467 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/tls_mutual_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25864 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/tls_platform_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14407 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/tls_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/tls_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/tls_subscription_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11638 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:36:08.398364 pulumi_fastly-8.7.0a1715351477/pulumi_fastly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-10 14:36:08.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-10 14:36:08.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:36:08.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 14:36:08.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 14:36:08.000000 pulumi_fastly-8.7.0a1715351477/pulumi_fastly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-10 14:36:02.000000 pulumi_fastly-8.7.0a1715351477/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 14:36:08.398364 pulumi_fastly-8.7.0a1715351477/setup.cfg
```

### Comparing `pulumi_fastly-8.7.0a1715303918/PKG-INFO` & `pulumi_fastly-8.7.0a1715351477/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_fastly
-Version: 8.7.0a1715303918
+Version: 8.7.0a1715351477
 Summary: A Pulumi package for creating and managing fastly cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-fastly
 Keywords: pulumi,fastly
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_fastly-8.7.0a1715303918/README.md` & `pulumi_fastly-8.7.0a1715351477/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/__init__.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from .get_tls_platform_certificate_ids import *
 from .get_tls_private_key import *
 from .get_tls_private_key_ids import *
 from .get_tls_subscription import *
 from .get_tls_subscription_ids import *
 from .get_vcl_snippets import *
 from .get_waf_rules import *
+from .integration import *
 from .kvstore import *
 from .provider import *
 from .secretstore import *
 from .service_acl_entries import *
 from .service_authorization import *
 from .service_compute import *
 from .service_dictionary_items import *
@@ -84,14 +85,22 @@
   "fqn": "pulumi_fastly",
   "classes": {
    "fastly:index/configstoreEntries:ConfigstoreEntries": "ConfigstoreEntries"
   }
  },
  {
   "pkg": "fastly",
+  "mod": "index/integration",
+  "fqn": "pulumi_fastly",
+  "classes": {
+   "fastly:index/integration:Integration": "Integration"
+  }
+ },
+ {
+  "pkg": "fastly",
   "mod": "index/kvstore",
   "fqn": "pulumi_fastly",
   "classes": {
    "fastly:index/kvstore:Kvstore": "Kvstore"
   }
  },
  {
```

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/_inputs.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,29 +137,33 @@
 
 
 @pulumi.input_type
 class AlertEvaluationStrategyArgs:
     def __init__(__self__, *,
                  period: pulumi.Input[str],
                  threshold: pulumi.Input[float],
-                 type: pulumi.Input[str]):
+                 type: pulumi.Input[str],
+                 ignore_below: Optional[pulumi.Input[float]] = None):
         """
-        :param pulumi.Input[str] period: The length of time to evaluate whether the conditions have been met. The data is polled every minute. One of: `5m`, `15m`, `30m`.
+        :param pulumi.Input[str] period: The length of time to evaluate whether the conditions have been met. The data is polled every minute. One of: `2m`, `3m`, `5m`, `15m`, `30m`.
         :param pulumi.Input[float] threshold: Threshold used to alert.
-        :param pulumi.Input[str] type: Type of strategy to use to evaluate. One of: `above_threshold`, `below_threshold`.
+        :param pulumi.Input[str] type: Type of strategy to use to evaluate. One of: `above_threshold`, `all_above_threshold`, `below_threshold`, `percent_absolute`, `percent_decrease`, `percent_increase`.
+        :param pulumi.Input[float] ignore_below: Threshold for the denominator value used in evaluations that calculate a rate or ratio. Usually used to filter out noise.
         """
         pulumi.set(__self__, "period", period)
         pulumi.set(__self__, "threshold", threshold)
         pulumi.set(__self__, "type", type)
+        if ignore_below is not None:
+            pulumi.set(__self__, "ignore_below", ignore_below)
 
     @property
     @pulumi.getter
     def period(self) -> pulumi.Input[str]:
         """
-        The length of time to evaluate whether the conditions have been met. The data is polled every minute. One of: `5m`, `15m`, `30m`.
+        The length of time to evaluate whether the conditions have been met. The data is polled every minute. One of: `2m`, `3m`, `5m`, `15m`, `30m`.
         """
         return pulumi.get(self, "period")
 
     @period.setter
     def period(self, value: pulumi.Input[str]):
         pulumi.set(self, "period", value)
 
@@ -175,22 +179,34 @@
     def threshold(self, value: pulumi.Input[float]):
         pulumi.set(self, "threshold", value)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
         """
-        Type of strategy to use to evaluate. One of: `above_threshold`, `below_threshold`.
+        Type of strategy to use to evaluate. One of: `above_threshold`, `all_above_threshold`, `below_threshold`, `percent_absolute`, `percent_decrease`, `percent_increase`.
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
+    @property
+    @pulumi.getter(name="ignoreBelow")
+    def ignore_below(self) -> Optional[pulumi.Input[float]]:
+        """
+        Threshold for the denominator value used in evaluations that calculate a rate or ratio. Usually used to filter out noise.
+        """
+        return pulumi.get(self, "ignore_below")
+
+    @ignore_below.setter
+    def ignore_below(self, value: Optional[pulumi.Input[float]]):
+        pulumi.set(self, "ignore_below", value)
+
 
 @pulumi.input_type
 class ServiceACLEntriesEntryArgs:
     def __init__(__self__, *,
                  ip: pulumi.Input[str],
                  comment: Optional[pulumi.Input[str]] = None,
                  id: Optional[pulumi.Input[str]] = None,
```

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/_utilities.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/alert.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/alert.py`

 * *Files 2% similar despite different names*

```diff
@@ -301,24 +301,26 @@
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         example = fastly.ServiceVcl("example", name="my_vcl_service")
+        example_integration = fastly.Integration("example", name="my_integration")
         example_alert = fastly.Alert("example",
             name="my_vcl_service errors",
             service_id=example.id,
             source="stats",
             metric="status_5xx",
             evaluation_strategy=fastly.AlertEvaluationStrategyArgs(
                 type="above_threshold",
                 period="5m",
                 threshold=10,
-            ))
+            ),
+            integration_ids=[example_integration.id])
         ```
 
         ## Import
 
         Fastly Alerts can be imported using their ID, e.g.
 
         ```sh
@@ -348,24 +350,26 @@
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         example = fastly.ServiceVcl("example", name="my_vcl_service")
+        example_integration = fastly.Integration("example", name="my_integration")
         example_alert = fastly.Alert("example",
             name="my_vcl_service errors",
             service_id=example.id,
             source="stats",
             metric="status_5xx",
             evaluation_strategy=fastly.AlertEvaluationStrategyArgs(
                 type="above_threshold",
                 period="5m",
                 threshold=10,
-            ))
+            ),
+            integration_ids=[example_integration.id])
         ```
 
         ## Import
 
         Fastly Alerts can be imported using their ID, e.g.
 
         ```sh
```

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/config/__init__.pyi` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/config/vars.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/configstore.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/configstore.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/configstore_entries.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/configstore_entries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_configstores.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_configstores.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_datacenters.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_datacenters.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_dictionaries.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_dictionaries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_fastly_ip_ranges.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_fastly_ip_ranges.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_kvstores.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_kvstores.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_package_hash.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_package_hash.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_secretstores.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_secretstores.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_services.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_services.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_activation.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_tls_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_activation_ids.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_tls_activation_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_certificate.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_tls_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_certificate_ids.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_tls_certificate_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_configuration.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_tls_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_configuration_ids.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_tls_configuration_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_domain.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_tls_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_platform_certificate.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_tls_platform_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_platform_certificate_ids.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_tls_platform_certificate_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_private_key.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_tls_private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_private_key_ids.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_tls_private_key_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_subscription.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_tls_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_tls_subscription_ids.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_tls_subscription_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/get_waf_rules.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/get_waf_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/kvstore.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/kvstore.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/outputs.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,32 +136,53 @@
         Addresses of a subset of backends that the alert monitors.
         """
         return pulumi.get(self, "origins")
 
 
 @pulumi.output_type
 class AlertEvaluationStrategy(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "ignoreBelow":
+            suggest = "ignore_below"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in AlertEvaluationStrategy. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        AlertEvaluationStrategy.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        AlertEvaluationStrategy.__key_warning(key)
+        return super().get(key, default)
+
     def __init__(__self__, *,
                  period: str,
                  threshold: float,
-                 type: str):
+                 type: str,
+                 ignore_below: Optional[float] = None):
         """
-        :param str period: The length of time to evaluate whether the conditions have been met. The data is polled every minute. One of: `5m`, `15m`, `30m`.
+        :param str period: The length of time to evaluate whether the conditions have been met. The data is polled every minute. One of: `2m`, `3m`, `5m`, `15m`, `30m`.
         :param float threshold: Threshold used to alert.
-        :param str type: Type of strategy to use to evaluate. One of: `above_threshold`, `below_threshold`.
+        :param str type: Type of strategy to use to evaluate. One of: `above_threshold`, `all_above_threshold`, `below_threshold`, `percent_absolute`, `percent_decrease`, `percent_increase`.
+        :param float ignore_below: Threshold for the denominator value used in evaluations that calculate a rate or ratio. Usually used to filter out noise.
         """
         pulumi.set(__self__, "period", period)
         pulumi.set(__self__, "threshold", threshold)
         pulumi.set(__self__, "type", type)
+        if ignore_below is not None:
+            pulumi.set(__self__, "ignore_below", ignore_below)
 
     @property
     @pulumi.getter
     def period(self) -> str:
         """
-        The length of time to evaluate whether the conditions have been met. The data is polled every minute. One of: `5m`, `15m`, `30m`.
+        The length of time to evaluate whether the conditions have been met. The data is polled every minute. One of: `2m`, `3m`, `5m`, `15m`, `30m`.
         """
         return pulumi.get(self, "period")
 
     @property
     @pulumi.getter
     def threshold(self) -> float:
         """
@@ -169,18 +190,26 @@
         """
         return pulumi.get(self, "threshold")
 
     @property
     @pulumi.getter
     def type(self) -> str:
         """
-        Type of strategy to use to evaluate. One of: `above_threshold`, `below_threshold`.
+        Type of strategy to use to evaluate. One of: `above_threshold`, `all_above_threshold`, `below_threshold`, `percent_absolute`, `percent_decrease`, `percent_increase`.
         """
         return pulumi.get(self, "type")
 
+    @property
+    @pulumi.getter(name="ignoreBelow")
+    def ignore_below(self) -> Optional[float]:
+        """
+        Threshold for the denominator value used in evaluations that calculate a rate or ratio. Usually used to filter out noise.
+        """
+        return pulumi.get(self, "ignore_below")
+
 
 @pulumi.output_type
 class ServiceACLEntriesEntry(dict):
     def __init__(__self__, *,
                  ip: str,
                  comment: Optional[str] = None,
                  id: Optional[str] = None,
```

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/provider.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/secretstore.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/secretstore.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/service_acl_entries.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/service_acl_entries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/service_authorization.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/service_authorization.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/service_compute.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/service_compute.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/service_dictionary_items.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/service_dictionary_items.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/service_dynamic_snippet_content.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/service_dynamic_snippet_content.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/service_vcl.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/service_vcl.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/service_waf_configuration.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/service_waf_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/tls_activation.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/tls_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/tls_certificate.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/tls_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/tls_mutual_authentication.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/tls_mutual_authentication.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/tls_platform_certificate.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/tls_platform_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/tls_private_key.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/tls_private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/tls_subscription.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/tls_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/tls_subscription_validation.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/tls_subscription_validation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly/user.py` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly.egg-info/PKG-INFO` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_fastly
-Version: 8.7.0a1715303918
+Version: 8.7.0a1715351477
 Summary: A Pulumi package for creating and managing fastly cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-fastly
 Keywords: pulumi,fastly
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_fastly-8.7.0a1715303918/pulumi_fastly.egg-info/SOURCES.txt` & `pulumi_fastly-8.7.0a1715351477/pulumi_fastly.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 pulumi_fastly/get_tls_platform_certificate_ids.py
 pulumi_fastly/get_tls_private_key.py
 pulumi_fastly/get_tls_private_key_ids.py
 pulumi_fastly/get_tls_subscription.py
 pulumi_fastly/get_tls_subscription_ids.py
 pulumi_fastly/get_vcl_snippets.py
 pulumi_fastly/get_waf_rules.py
+pulumi_fastly/integration.py
 pulumi_fastly/kvstore.py
 pulumi_fastly/outputs.py
 pulumi_fastly/provider.py
 pulumi_fastly/pulumi-plugin.json
 pulumi_fastly/py.typed
 pulumi_fastly/secretstore.py
 pulumi_fastly/service_acl_entries.py
```

### Comparing `pulumi_fastly-8.7.0a1715303918/pyproject.toml` & `pulumi_fastly-8.7.0a1715351477/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_fastly"
   description = "A Pulumi package for creating and managing fastly cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "fastly"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "8.7.0a1715303918"
+  version = "8.7.0a1715351477"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-fastly"
 
 [build-system]
```

