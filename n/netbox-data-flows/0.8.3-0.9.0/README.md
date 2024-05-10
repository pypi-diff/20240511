# Comparing `tmp/netbox_data_flows-0.8.3.tar.gz` & `tmp/netbox_data_flows-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_data_flows-0.8.3.tar", last modified: Thu May  9 17:22:44 2024, max compression
+gzip compressed data, was "netbox_data_flows-0.9.0.tar", last modified: Fri May 10 22:55:47 2024, max compression
```

## Comparing `netbox_data_flows-0.8.3.tar` & `netbox_data_flows-0.9.0.tar`

### file list

```diff
@@ -1,107 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.179002 netbox_data_flows-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-05-09 17:22:44.179002 netbox_data_flows-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.163002 netbox_data_flows-0.8.3/netbox_data_flows/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.167002 netbox_data_flows-0.8.3/netbox_data_flows/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.167002 netbox_data_flows-0.8.3/netbox_data_flows/api/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/api/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/api/serializers/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/api/serializers/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/api/serializers/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/api/serializers/nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/api/serializers/objectaliases.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/choices.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.167002 netbox_data_flows-0.8.3/netbox_data_flows/filtersets/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/filtersets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/filtersets/addins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/filtersets/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/filtersets/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/filtersets/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/filtersets/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/filtersets/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.167002 netbox_data_flows-0.8.3/netbox_data_flows/forms/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/forms/applicationroles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/forms/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)    14082 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/forms/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/forms/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/forms/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.171002 netbox_data_flows-0.8.3/netbox_data_flows/graphql/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/graphql/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/graphql/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/graphql/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/graphql/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.171002 netbox_data_flows-0.8.3/netbox_data_flows/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.171002 netbox_data_flows-0.8.3/netbox_data_flows/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/management/commands/delete_orphaned_aliases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.171002 netbox_data_flows-0.8.3/netbox_data_flows/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    14554 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/migrations/0002_alter_objectalias_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/migrations/0004_reindex_netbox_data_flows.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/migrations/0005_dataflowgroup_slug.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/migrations/0006_reindex_netbox_data_flows.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/migrations/0007_remove_objectalias_size.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/migrations/0008_delete_orphaned_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/migrations/0009_fix_empty_dfg_slugs.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/migrations/0010_alter_objectaliastarget_options.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.175002 netbox_data_flows-0.8.3/netbox_data_flows/models/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/models/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/models/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/models/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     7741 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/models/objectaliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/navigation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/search.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.175002 netbox_data_flows-0.8.3/netbox_data_flows/tables/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/tables/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/tables/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/tables/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/tables/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.159002 netbox_data_flows-0.8.3/netbox_data_flows/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.175002 netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/application.html
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/applicationrole.html
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/dataflow.html
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/dataflow_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/dataflow_tab.html
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.175002 netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/inc/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/inc/objectaliastarget_actions.html
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/objectalias.html
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.175002 netbox_data_flows-0.8.3/netbox_data_flows/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8285 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/utils/aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/utils/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.179002 netbox_data_flows-0.8.3/netbox_data_flows/views/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/views/applicationroles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/views/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/views/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/views/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/views/model_tabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/views/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.179002 netbox_data_flows-0.8.3/netbox_data_flows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-05-09 17:22:44.000000 netbox_data_flows-0.8.3/netbox_data_flows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-09 17:22:44.000000 netbox_data_flows-0.8.3/netbox_data_flows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 17:22:44.000000 netbox_data_flows-0.8.3/netbox_data_flows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 17:22:43.000000 netbox_data_flows-0.8.3/netbox_data_flows.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-09 17:22:44.000000 netbox_data_flows-0.8.3/netbox_data_flows.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 17:22:44.179002 netbox_data_flows-0.8.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.773944 netbox_data_flows-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-05-10 22:55:47.773944 netbox_data_flows-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.761944 netbox_data_flows-0.9.0/netbox_data_flows/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.761944 netbox_data_flows-0.9.0/netbox_data_flows/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.761944 netbox_data_flows-0.9.0/netbox_data_flows/api/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/api/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/api/serializers/applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/api/serializers/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/api/serializers/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/api/serializers/objectaliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/choices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.761944 netbox_data_flows-0.9.0/netbox_data_flows/filtersets/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/filtersets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/filtersets/addins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/filtersets/applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/filtersets/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/filtersets/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/filtersets/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/filtersets/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.765944 netbox_data_flows-0.9.0/netbox_data_flows/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/forms/applicationroles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/forms/applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13729 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/forms/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/forms/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/forms/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.765944 netbox_data_flows-0.9.0/netbox_data_flows/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.765944 netbox_data_flows-0.9.0/netbox_data_flows/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/management/commands/delete_orphaned_aliases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.765944 netbox_data_flows-0.9.0/netbox_data_flows/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    14554 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/migrations/0002_alter_objectalias_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/migrations/0004_reindex_netbox_data_flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/migrations/0005_dataflowgroup_slug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/migrations/0006_reindex_netbox_data_flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/migrations/0007_remove_objectalias_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/migrations/0008_delete_orphaned_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/migrations/0009_fix_empty_dfg_slugs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/migrations/0010_alter_objectaliastarget_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.765944 netbox_data_flows-0.9.0/netbox_data_flows/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/models/applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/models/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/models/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7757 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/models/objectaliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.769944 netbox_data_flows-0.9.0/netbox_data_flows/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/tables/applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/tables/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/tables/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/tables/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.757944 netbox_data_flows-0.9.0/netbox_data_flows/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.769944 netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/application.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/applicationrole.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/dataflow.html
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/dataflow_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/dataflow_tab.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.769944 netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/inc/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/inc/objectaliastarget_actions.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/objectalias.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.769944 netbox_data_flows-0.9.0/netbox_data_flows/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8122 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/utils/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/utils/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.769944 netbox_data_flows-0.9.0/netbox_data_flows/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/views/applicationroles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/views/applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/views/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/views/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/views/model_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/netbox_data_flows/views/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:55:47.773944 netbox_data_flows-0.9.0/netbox_data_flows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-05-10 22:55:47.000000 netbox_data_flows-0.9.0/netbox_data_flows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-10 22:55:47.000000 netbox_data_flows-0.9.0/netbox_data_flows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 22:55:47.000000 netbox_data_flows-0.9.0/netbox_data_flows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 22:55:47.000000 netbox_data_flows-0.9.0/netbox_data_flows.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-10 22:55:47.000000 netbox_data_flows-0.9.0/netbox_data_flows.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-10 22:55:36.000000 netbox_data_flows-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 22:55:47.773944 netbox_data_flows-0.9.0/setup.cfg
```

### Comparing `netbox_data_flows-0.8.3/LICENSE` & `netbox_data_flows-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.8.3/PKG-INFO` & `netbox_data_flows-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: netbox-data-flows
-Version: 0.8.3
+Version: 0.9.0
 Summary: NetBox plugin to document data flows between systems and applications.
 Author: Thomas Fargeix
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/Alef-Burzmali/netbox-data-flows
 Project-URL: Bug Tracker, https://github.com/Alef-Burzmali/netbox-data-flows/issues
 Keywords: netbox,netbox-plugins
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: System :: Networking
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # netbox-data-flows
 
 Plugin for [NetBox](https://github.com/netbox-community/netbox) to document
 Data Flows between systems and applications.
@@ -34,16 +34,18 @@
 
 ## Installation and Configuration
 
 Full reference: [Using Plugins - NetBox Documentation](https://docs.netbox.dev/en/stable/plugins/)
 
 ### Requirements
 
-* NetBox (=3.7.x)
-* Python 3.8 or higher
+* NetBox (>=4.0.0)
+* Python 3.10 or higher
+
+Use version 0.8.x if you need compatibility with NetBox 3.7.x
 
 This is the last version compatible with NetBox 3. Future releases will support 4.0 only.
 
 *Note:* the plugin uses some classes that are not explicitely exported in 
 NetBox's plugin API, such as MPTT Tree-based models. Upward compatiblity is
 not guaranteed.
```

### Comparing `netbox_data_flows-0.8.3/README.md` & `netbox_data_flows-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,18 @@
 
 ## Installation and Configuration
 
 Full reference: [Using Plugins - NetBox Documentation](https://docs.netbox.dev/en/stable/plugins/)
 
 ### Requirements
 
-* NetBox (=3.7.x)
-* Python 3.8 or higher
+* NetBox (>=4.0.0)
+* Python 3.10 or higher
+
+Use version 0.8.x if you need compatibility with NetBox 3.7.x
 
 This is the last version compatible with NetBox 3. Future releases will support 4.0 only.
 
 *Note:* the plugin uses some classes that are not explicitely exported in 
 NetBox's plugin API, such as MPTT Tree-based models. Upward compatiblity is
 not guaranteed.
```

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/__init__.py` & `netbox_data_flows-0.9.0/netbox_data_flows/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from netbox.plugins import PluginConfig
 
-__version__ = "0.8.3"
+__version__ = "0.9.0"
 
 
 class DataFlowsConfig(PluginConfig):
     name = "netbox_data_flows"
     verbose_name = "Data Flows"
     description = (
         "NetBox plugin to document data flows between "
         "systems and applications."
     )
     version = __version__
     base_url = "data-flows"
     author = "Thomas Fargeix"
     required_settings = []
     default_settings = {}
-    min_version = "3.7.0"
-    max_version = "3.7.9"
+    min_version = "4.0.0"
+    max_version = "4.0.99"
 
     def ready(self):
         from . import signals  # noqa: F401
 
         super().ready()
```

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/api/serializers/applications.py` & `netbox_data_flows-0.9.0/netbox_data_flows/api/serializers/applications.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from rest_framework import serializers
 
 from netbox.api.serializers import NetBoxModelSerializer
 
 from netbox_data_flows import models
 
-from . import nested
-
 
 __all__ = (
     "ApplicationSerializer",
     "ApplicationRoleSerializer",
 )
 
 
@@ -30,22 +28,30 @@
             "slug",
             "tags",
             "custom_fields",
             "created",
             "last_updated",
             "application_count",
         )
+        brief_fields = (
+            "id",
+            "url",
+            "display",
+            "name",
+            "description",
+            "slug",
+        )
 
 
 class ApplicationSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name="plugins-api:netbox_data_flows-api:application-detail"
     )
     dataflow_count = serializers.IntegerField(read_only=True)
-    role = nested.NestedApplicationRoleSerializer()
+    role = ApplicationRoleSerializer(nested=True)
 
     class Meta:
         model = models.Application
         fields = (
             "id",
             "url",
             "display",
@@ -55,7 +61,15 @@
             "comments",
             "tags",
             "custom_fields",
             "created",
             "last_updated",
             "dataflow_count",
         )
+        brief_fields = (
+            "id",
+            "url",
+            "display",
+            "name",
+            "description",
+            "slug",
+        )
```

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/api/serializers/dataflows.py` & `netbox_data_flows-0.9.0/netbox_data_flows/api/serializers/dataflows.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 from rest_framework import serializers
 
 from netbox.api.fields import ChoiceField, SerializedPKRelatedField
 from netbox.api.serializers import NetBoxModelSerializer
 
 from netbox_data_flows import models, choices
 
-from . import nested
+from .applications import ApplicationSerializer
+from .groups import DataFlowGroupSerializer
+from .objectaliases import ObjectAliasSerializer
 
 
 __all__ = ("DataFlowSerializer",)
 
 
 class DataFlowSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name="plugins-api:netbox_data_flows-api:dataflow-detail"
     )
 
-    application = nested.NestedApplicationSerializer(
-        required=False, allow_null=True, default=None
+    application = ApplicationSerializer(
+        nested=True, required=False, allow_null=True, default=None
     )
-    group = nested.NestedDataFlowGroupSerializer(
-        required=False, allow_null=True, default=None
+    group = DataFlowGroupSerializer(
+        nested=True, required=False, allow_null=True, default=None
     )
 
     status = ChoiceField(choices=choices.DataFlowStatusChoices, required=False)
     inherited_status = ChoiceField(
         choices=choices.DataFlowInheritedStatusChoices,
         required=False,
         read_only=True,
     )
     protocol = ChoiceField(
         choices=choices.DataFlowProtocolChoices, required=False
     )
 
     sources = SerializedPKRelatedField(
         queryset=models.ObjectAlias.objects.all(),
-        serializer=nested.NestedObjectAliasSerializer,
+        serializer=ObjectAliasSerializer,
+        nested=True,
         required=False,
         many=True,
     )
     destinations = SerializedPKRelatedField(
         queryset=models.ObjectAlias.objects.all(),
-        serializer=nested.NestedObjectAliasSerializer,
+        serializer=ObjectAliasSerializer,
+        nested=True,
         required=False,
         many=True,
     )
 
     class Meta:
         model = models.DataFlow
         fields = (
@@ -65,7 +69,14 @@
             "last_updated",
             "protocol",
             "source_ports",
             "destination_ports",
             "sources",
             "destinations",
         )
+        brief_fields = (
+            "id",
+            "url",
+            "display",
+            "name",
+            "description",
+        )
```

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/api/serializers/groups.py` & `netbox_data_flows-0.9.0/netbox_data_flows/api/serializers/groups.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,77 @@
 from rest_framework import serializers
 
 from netbox.api.fields import ChoiceField
-from netbox.api.serializers import NetBoxModelSerializer
+from netbox.api.serializers import (
+    NetBoxModelSerializer,
+    WritableNestedSerializer,
+)
 
 from netbox_data_flows import models, choices
 
-from . import nested
+from .applications import ApplicationSerializer
 
 
-__all__ = ("DataFlowGroupSerializer",)
+__all__ = (
+    "NestedDataFlowGroupSerializer",
+    "DataFlowGroupSerializer",
+)
+
+
+class NestedDataFlowGroupSerializer(WritableNestedSerializer):
+    url = serializers.HyperlinkedIdentityField(
+        view_name="plugins-api:netbox_data_flows-api:dataflowgroup-detail"
+    )
+
+    status = ChoiceField(choices=choices.DataFlowStatusChoices, required=False)
+    _depth = serializers.IntegerField(source="level", read_only=True)
+
+    class Meta:
+        model = models.DataFlowGroup
+        fields = (
+            "id",
+            "url",
+            "display",
+            "name",
+            "description",
+            "slug",
+            "status",
+            "_depth",
+        )
+        brief_fields = (
+            "id",
+            "url",
+            "display",
+            "name",
+            "description",
+            "slug",
+            "status",
+            "_depth",
+        )
 
 
 class DataFlowGroupSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name="plugins-api:netbox_data_flows-api:dataflowgroup-detail"
     )
 
     status = ChoiceField(choices=choices.DataFlowStatusChoices, required=False)
     inherited_status = ChoiceField(
         choices=choices.DataFlowInheritedStatusChoices,
         required=False,
         read_only=True,
     )
 
-    application = nested.NestedApplicationSerializer(
-        required=False, allow_null=True, default=None
+    application = ApplicationSerializer(
+        nested=True, required=False, allow_null=True, default=None
     )
-    parent = nested.NestedDataFlowGroupSerializer(
-        required=False, allow_null=True, default=None
+    parent = NestedDataFlowGroupSerializer(
+        nested=True, required=False, allow_null=True, default=None
     )
+    _depth = serializers.IntegerField(source="level", read_only=True)
 
     class Meta:
         model = models.DataFlowGroup
         fields = (
             "id",
             "url",
             "display",
@@ -44,8 +83,18 @@
             "status",
             "inherited_status",
             "comments",
             "tags",
             "custom_fields",
             "created",
             "last_updated",
+            "_depth",
+        )
+        brief_fields = (
+            "id",
+            "url",
+            "display",
+            "name",
+            "description",
+            "slug",
+            "status",
         )
```

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/api/serializers/nested.py` & `netbox_data_flows-0.9.0/netbox_data_flows/forms/applications.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,126 +1,139 @@
-from rest_framework import serializers
+from django import forms
 
-from netbox.api.serializers import WritableNestedSerializer
+from netbox.forms import (
+    NetBoxModelForm,
+    NetBoxModelBulkEditForm,
+    NetBoxModelFilterSetForm,
+    NetBoxModelImportForm,
+)
+from tenancy.forms import ContactModelFilterForm
+from utilities.forms.fields import (
+    CommentField,
+    CSVModelChoiceField,
+    DynamicModelChoiceField,
+    TagFilterField,
+)
+from utilities.forms.rendering import FieldSet
 
-from netbox_data_flows import models
+from netbox_data_flows.models import (
+    Application,
+    ApplicationRole,
+)
 
 
 __all__ = (
-    "NestedApplicationSerializer",
-    "NestedApplicationRoleSerializer",
-    "NestedDataFlowSerializer",
-    "NestedDataFlowGroupSerializer",
-    "NestedObjectAliasSerializer",
-    "NestedObjectAliasTargetSerializer",
+    "ApplicationForm",
+    "ApplicationBulkEditForm",
+    "ApplicationImportForm",
+    "ApplicationFilterForm",
 )
 
-
 #
-# applications
+# Object forms
 #
 
 
-class NestedApplicationRoleSerializer(WritableNestedSerializer):
-    url = serializers.HyperlinkedIdentityField(
-        view_name="plugins-api:netbox_data_flows-api:applicationrole-detail"
+class ApplicationForm(NetBoxModelForm):
+    role = DynamicModelChoiceField(
+        queryset=ApplicationRole.objects.all(),
+        required=False,
+        selector=True,
     )
+    comments = CommentField()
 
-    class Meta:
-        model = models.ApplicationRole
-        fields = ("id", "url", "display", "slug")
-
-
-class NestedApplicationSerializer(WritableNestedSerializer):
-    url = serializers.HyperlinkedIdentityField(
-        view_name="plugins-api:netbox_data_flows-api:application-detail"
+    fieldsets = (
+        FieldSet(
+            "name",
+            "role",
+            "description",
+            "tags",
+        ),
     )
-    role = NestedApplicationRoleSerializer()
 
     class Meta:
-        model = models.Application
-        fields = ("id", "url", "display", "role")
+        model = Application
+        fields = (
+            "name",
+            "role",
+            "description",
+            "comments",
+            "tags",
+        )
 
 
 #
-# dataflows
+# Bulk forms
 #
 
 
-class NestedDataFlowSerializer(WritableNestedSerializer):
-    url = serializers.HyperlinkedIdentityField(
-        view_name="plugins-api:netbox_data_flows-api:dataflow-detail"
-    )
-    _depth = serializers.IntegerField(source="level", read_only=True)
-    application = NestedApplicationSerializer()
-
-    class Meta:
-        model = models.DataFlow
-        fields = (
-            "id",
-            "url",
-            "display",
-            "application",
-            "name",
-            "status",
-            "_depth",
-        )
+class ApplicationBulkEditForm(NetBoxModelBulkEditForm):
+    model = Application
 
+    description = forms.CharField(max_length=200, required=False)
+    role = DynamicModelChoiceField(
+        queryset=ApplicationRole.objects.all(),
+        required=False,
+        selector=True,
+    )
+    comments = CommentField()
 
-#
-# dataflow groups
-#
+    fieldsets = (
+        FieldSet(
+            "role",
+            "description",
+        ),
+    )
+    nullable_fields = (
+        "role",
+        "description",
+        "comments",
+    )
 
 
-class NestedDataFlowGroupSerializer(WritableNestedSerializer):
-    url = serializers.HyperlinkedIdentityField(
-        view_name="plugins-api:netbox_data_flows-api:dataflowgroup-detail"
+class ApplicationImportForm(NetBoxModelImportForm):
+    role = CSVModelChoiceField(
+        queryset=ApplicationRole.objects.all(),
+        required=False,
+        to_field_name="slug",
+        help_text="Role of the application",
     )
-    _depth = serializers.IntegerField(source="level", read_only=True)
-    application = NestedApplicationSerializer()
 
     class Meta:
-        model = models.DataFlowGroup
+        model = Application
         fields = (
-            "id",
-            "url",
-            "display",
-            "application",
             "name",
-            "status",
-            "_depth",
+            "description",
+            "role",
         )
 
 
 #
-# Object aliases
+# Filter forms
 #
 
 
-class NestedObjectAliasTargetSerializer(WritableNestedSerializer):
-    url = serializers.HyperlinkedIdentityField(
-        view_name="plugins-api:netbox_data_flows-api:objectaliastarget-detail"
+class ApplicationFilterForm(ContactModelFilterForm, NetBoxModelFilterSetForm):
+    model = Application
+    tag = TagFilterField(model)
+
+    role = forms.ModelMultipleChoiceField(
+        queryset=ApplicationRole.objects.all(), required=False
+    )
+
+    fieldsets = (
+        FieldSet(
+            "filter_id",  # Saved Filter
+            "q",  # Search
+            "tag",
+        ),
+        FieldSet(
+            "role",
+            name="Application Role",
+        ),
+        FieldSet(
+            "contact",
+            "contact_role",
+            "contact_group",
+            name="Contacts",
+        ),
     )
-
-    class Meta:
-        model = models.ObjectAliasTarget
-        fields = (
-            "id",
-            "url",
-            "display",
-        )
-
-
-class NestedObjectAliasSerializer(WritableNestedSerializer):
-    url = serializers.HyperlinkedIdentityField(
-        view_name="plugins-api:netbox_data_flows-api:objectalias-detail"
-    )
-
-    class Meta:
-        model = models.ObjectAlias
-        fields = (
-            "id",
-            "url",
-            "display",
-            "name",
-            "description",
-        )
```

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/api/serializers/objectaliases.py` & `netbox_data_flows-0.9.0/netbox_data_flows/api/serializers/objectaliases.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,30 +28,43 @@
         model = models.ObjectAliasTarget
         fields = (
             "id",
             "url",
             "display",
             "target",
         )
+        brief_fields = (
+            "id",
+            "url",
+            "display",
+        )
 
 
 class ObjectAliasSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name="plugins-api:netbox_data_flows-api:objectalias-detail"
     )
     targets = SerializedPKRelatedField(
         queryset=models.ObjectAliasTarget.objects.all(),
         serializer=ObjectAliasTargetSerializer,
+        nested=True,
         required=True,
         many=True,
     )
 
     class Meta:
         model = models.ObjectAlias
         fields = (
             "id",
             "url",
             "display",
             "name",
             "description",
             "targets",
         )
+        brief_fields = (
+            "id",
+            "url",
+            "display",
+            "name",
+            "description",
+        )
```

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/api/urls.py` & `netbox_data_flows-0.9.0/netbox_data_flows/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/choices.py` & `netbox_data_flows-0.9.0/netbox_data_flows/choices.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/filtersets/addins.py` & `netbox_data_flows-0.9.0/netbox_data_flows/filtersets/addins.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/filtersets/applications.py` & `netbox_data_flows-0.9.0/netbox_data_flows/filtersets/applications.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/filtersets/dataflows.py` & `netbox_data_flows-0.9.0/netbox_data_flows/filtersets/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/filtersets/filters.py` & `netbox_data_flows-0.9.0/netbox_data_flows/filtersets/filters.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/filtersets/groups.py` & `netbox_data_flows-0.9.0/netbox_data_flows/filtersets/groups.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/filtersets/objectaliases.py` & `netbox_data_flows-0.9.0/netbox_data_flows/filtersets/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/forms/applicationroles.py` & `netbox_data_flows-0.9.0/netbox_data_flows/forms/applicationroles.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     NetBoxModelFilterSetForm,
     NetBoxModelImportForm,
 )
 from utilities.forms.fields import (
     SlugField,
     TagFilterField,
 )
+from utilities.forms.rendering import FieldSet
 
 from netbox_data_flows.models import (
     ApplicationRole,
 )
 
 __all__ = (
     "ApplicationRoleForm",
@@ -27,22 +28,19 @@
 #
 
 
 class ApplicationRoleForm(NetBoxModelForm):
     slug = SlugField()
 
     fieldsets = (
-        (
-            "Application Role",
-            (
-                "name",
-                "slug",
-                "description",
-                "tags",
-            ),
+        FieldSet(
+            "name",
+            "slug",
+            "description",
+            "tags",
         ),
     )
 
     class Meta:
         model = ApplicationRole
         fields = ("name", "slug", "description", "tags")
 
@@ -54,17 +52,16 @@
 
 class ApplicationRoleBulkEditForm(NetBoxModelBulkEditForm):
     model = ApplicationRole
 
     description = forms.CharField(max_length=200, required=False)
 
     fieldsets = (
-        (
-            "Application Role",
-            ("description",),
+        FieldSet(
+            "description",
         ),
     )
     nullable_fields = ("description",)
 
 
 class ApplicationRoleImportForm(NetBoxModelImportForm):
     class Meta:
```

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/forms/applications.py` & `netbox_data_flows-0.9.0/netbox_data_flows/tables/applications.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,149 +1,81 @@
-from django import forms
+import django_tables2 as tables
 
-from netbox.forms import (
-    NetBoxModelForm,
-    NetBoxModelBulkEditForm,
-    NetBoxModelFilterSetForm,
-    NetBoxModelImportForm,
-)
-from tenancy.forms import ContactModelFilterForm
-from utilities.forms.fields import (
-    CommentField,
-    CSVModelChoiceField,
-    DynamicModelChoiceField,
-    TagFilterField,
+from netbox.tables import (
+    columns,
+    NetBoxTable,
 )
+from tenancy.tables import ContactsColumnMixin
 
-from netbox_data_flows.models import (
-    Application,
-    ApplicationRole,
-)
+from netbox_data_flows.models import Application, ApplicationRole
 
 
 __all__ = (
-    "ApplicationForm",
-    "ApplicationBulkEditForm",
-    "ApplicationImportForm",
-    "ApplicationFilterForm",
+    "ApplicationRoleTable",
+    "ApplicationTable",
 )
 
-#
-# Object forms
-#
-
-
-class ApplicationForm(NetBoxModelForm):
-    role = DynamicModelChoiceField(
-        queryset=ApplicationRole.objects.all(),
-        required=False,
-        selector=True,
-    )
-    comments = CommentField()
-
-    fieldsets = (
-        (
-            "Application",
-            (
-                "name",
-                "role",
-                "description",
-                "tags",
-            ),
-        ),
+
+class ApplicationRoleTable(NetBoxTable):
+    name = tables.Column(
+        linkify=True,
+    )
+    application_count = columns.LinkedCountColumn(
+        viewname="plugins:netbox_data_flows:application_list",
+        url_params={"role_id": "pk"},
+        verbose_name="Applications",
+    )
+    tags = columns.TagColumn(
+        url_name="plugins:netbox_data_flows:applicationrole_list"
     )
 
-    class Meta:
-        model = Application
+    class Meta(NetBoxTable.Meta):
+        model = ApplicationRole
         fields = (
+            "pk",
+            "id",
             "name",
-            "role",
+            "slug",
+            "application_count",
             "description",
-            "comments",
             "tags",
+            "created",
+            "last_updated",
+            "actions",
         )
+        default_columns = ("name", "description", "application_count")
 
 
-#
-# Bulk forms
-#
-
-
-class ApplicationBulkEditForm(NetBoxModelBulkEditForm):
-    model = Application
-
-    description = forms.CharField(max_length=200, required=False)
-    role = DynamicModelChoiceField(
-        queryset=ApplicationRole.objects.all(),
-        required=False,
-        selector=True,
+class ApplicationTable(ContactsColumnMixin, NetBoxTable):
+    name = tables.Column(
+        linkify=True,
     )
-    comments = CommentField()
-
-    fieldsets = (
-        (
-            "Application",
-            (
-                "role",
-                "description",
-            ),
-        ),
+    role = tables.Column(
+        linkify=True,
     )
-    nullable_fields = (
-        "role",
-        "description",
-        "comments",
+    dataflow_count = columns.LinkedCountColumn(
+        viewname="plugins:netbox_data_flows:dataflow_list",
+        url_params={"application_id": "pk"},
+        verbose_name="Data Flows",
     )
-
-
-class ApplicationImportForm(NetBoxModelImportForm):
-    role = CSVModelChoiceField(
-        queryset=ApplicationRole.objects.all(),
-        required=False,
-        to_field_name="slug",
-        help_text="Role of the application",
+    tags = columns.TagColumn(
+        url_name="plugins:netbox_data_flows:application_list"
     )
 
-    class Meta:
+    class Meta(NetBoxTable.Meta):
         model = Application
         fields = (
+            "pk",
+            "id",
             "name",
             "description",
             "role",
+            "contacts",
+            "comments",
+            "dataflow_count",
+            "contacts",
+            "tags",
+            "created",
+            "last_updated",
+            "actions",
         )
-
-
-#
-# Filter forms
-#
-
-
-class ApplicationFilterForm(ContactModelFilterForm, NetBoxModelFilterSetForm):
-    model = Application
-    tag = TagFilterField(model)
-
-    role = forms.ModelMultipleChoiceField(
-        queryset=ApplicationRole.objects.all(), required=False
-    )
-
-    fieldsets = (
-        (
-            None,
-            (
-                "filter_id",  # Saved Filter
-                "q",  # Search
-                "tag",
-            ),
-        ),
-        (
-            "Application Role",
-            ("role",),
-        ),
-        (
-            "Contacts",
-            (
-                "contact",
-                "contact_role",
-                "contact_group",
-            ),
-        ),
-    )
+        default_columns = ("name", "role", "dataflow_count")
```

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/forms/dataflows.py` & `netbox_data_flows-0.9.0/netbox_data_flows/forms/dataflows.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     CSVModelChoiceField,
     CSVModelMultipleChoiceField,
     DynamicModelChoiceField,
     DynamicModelMultipleChoiceField,
     NumericArrayField,
     TagFilterField,
 )
+from utilities.forms.rendering import FieldSet
 
 from dcim.models import Device
 from ipam.models import Prefix, IPRange, IPAddress
 from ipam.constants import SERVICE_PORT_MIN, SERVICE_PORT_MAX
 from virtualization.models import VirtualMachine
 
 from netbox_data_flows import models, choices
@@ -83,34 +84,29 @@
     )
     destinations = DynamicModelMultipleChoiceField(
         queryset=models.ObjectAlias.objects.all(),
         required=False,
     )
 
     fieldsets = (
-        (
-            "Data Flow",
-            (
-                "application",
-                "group",
-                "name",
-                "description",
-                "status",
-                "tags",
-            ),
+        FieldSet(
+            "application",
+            "group",
+            "name",
+            "description",
+            "status",
+            "tags",
         ),
-        (
-            "Specifications",
-            (
-                "protocol",
-                "source_ports",
-                "destination_ports",
-                "sources",
-                "destinations",
-            ),
+        FieldSet(
+            "protocol",
+            "source_ports",
+            "destination_ports",
+            "sources",
+            "destinations",
+            name="Specifications",
         ),
     )
 
     class Meta:
         model = models.DataFlow
         fields = (
             "application",
@@ -191,32 +187,27 @@
     )
     destinations = DynamicModelMultipleChoiceField(
         queryset=models.ObjectAlias.objects.all(),
         required=False,
     )
 
     fieldsets = (
-        (
-            "Data Flow",
-            (
-                "application",
-                "group",
-                "description",
-                "status",
-            ),
+        FieldSet(
+            "application",
+            "group",
+            "description",
+            "status",
         ),
-        (
-            "Specifications",
-            (
-                "protocol",
-                "source_ports",
-                "destination_ports",
-                "sources",
-                "destinations",
-            ),
+        FieldSet(
+            "protocol",
+            "source_ports",
+            "destination_ports",
+            "sources",
+            "destinations",
+            name="Specifications",
         ),
     )
     nullable_fields = (
         "application",
         "group",
         "description",
         "comments",
@@ -317,34 +308,34 @@
         required=False,
         label="Application Role",
         help_text="Application Role(s) that the data flows are part of",
     )
     group_id = DynamicModelMultipleChoiceField(
         queryset=models.DataFlowGroup.objects.all(),
         required=False,
-        label="Direct group",
-        help_text="Direct group(s)",
+        label="Direct parent group",
+        help_text="Direct group(s) of the data flows",
     )
     recursive_group_id = DynamicModelMultipleChoiceField(
         queryset=models.DataFlowGroup.objects.all(),
         required=False,
-        label="Recursive group",
-        help_text="Recursive group(s)",
+        label="Ancestor group",
+        help_text="Parent or ancestor group(s) of the data flows",
     )
     tag = TagFilterField(model)
 
     status = forms.ChoiceField(
         choices=add_blank_choice(choices.DataFlowStatusChoices),
         required=False,
         help_text="Status of the data flows themselves",
     )
     inherited_status = forms.ChoiceField(
         choices=add_blank_choice(choices.DataFlowStatusChoices),
         required=False,
-        help_text="Status inherited from the data flow groups",
+        help_text="Status inherited from the ancestor groups",
     )
 
     protocol = forms.MultipleChoiceField(
         choices=choices.DataFlowProtocolChoices,
         required=False,
     )
     source_ports = forms.IntegerField(
@@ -433,67 +424,53 @@
         queryset=VirtualMachine.objects.all(),
         required=False,
         label="Destination Virtual Machines",
         help_text="Any IP address of the virtual machine",
     )
 
     fieldsets = (
-        (
-            None,
-            (
-                "filter_id",  # Saved Filter
-                "q",  # Search
-                "tag",
-            ),
-        ),
-        (
-            None,
-            (
-                "application_id",
-                "application_role_id",
-                "group_id",
-                "recursive_group_id",
-            ),
+        FieldSet(
+            "filter_id",  # Saved Filter
+            "q",  # Search
+            "tag",
+        ),
+        FieldSet(
+            "application_id",
+            "application_role_id",
+            "group_id",
+            "recursive_group_id",
         ),
-        (
-            "Status",
-            (
-                "status",
-                "inherited_status",
-            ),
-        ),
-        (
-            "Specifications",
-            (
-                "protocol",
-                "source_ports",
-                "destination_ports",
-            ),
+        FieldSet(
+            "status",
+            "inherited_status",
+            name="Status",
         ),
-        (
-            "Sources - all sources are OR'ed together, any will match",
-            (
-                "source_is_null",
-                "source_aliases",
-                "source_prefixes",
-                "source_ipranges",
-                "source_ipaddresses",
-                "source_devices",
-                "source_virtual_machines",
-            ),
+        FieldSet(
+            "protocol",
+            "source_ports",
+            "destination_ports",
+            name="Specifications",
         ),
-        (
-            (
+        FieldSet(
+            "source_is_null",
+            "source_aliases",
+            "source_prefixes",
+            "source_ipranges",
+            "source_ipaddresses",
+            "source_devices",
+            "source_virtual_machines",
+            name="Sources - all sources are OR'ed together, any will match",
+        ),
+        FieldSet(
+            "destination_is_null",
+            "destination_aliases",
+            "destination_prefixes",
+            "destination_ipranges",
+            "destination_ipaddresses",
+            "destination_devices",
+            "destination_virtual_machines",
+            name=(
                 "Destinations - all destinations are OR'ed together, "
                 "any will match"
             ),
-            (
-                "destination_is_null",
-                "destination_aliases",
-                "destination_prefixes",
-                "destination_ipranges",
-                "destination_ipaddresses",
-                "destination_devices",
-                "destination_virtual_machines",
-            ),
         ),
     )
```

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/forms/groups.py` & `netbox_data_flows-0.9.0/netbox_data_flows/forms/groups.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     CSVChoiceField,
     CSVModelChoiceField,
     DynamicModelChoiceField,
     DynamicModelMultipleChoiceField,
     SlugField,
     TagFilterField,
 )
+from utilities.forms.rendering import FieldSet
 
 from netbox_data_flows import models, choices
 
 
 __all__ = (
     "DataFlowGroupForm",
     "DataFlowGroupBulkEditForm",
@@ -45,25 +46,22 @@
         required=False,
         selector=True,
         help_text="Parent group of this Data Flow Group.",
     )
     comments = CommentField()
 
     fieldsets = (
-        (
-            "Data Flow Group",
-            (
-                "application",
-                "parent",
-                "name",
-                "slug",
-                "description",
-                "status",
-                "tags",
-            ),
+        FieldSet(
+            "application",
+            "parent",
+            "name",
+            "slug",
+            "description",
+            "status",
+            "tags",
         ),
     )
 
     class Meta:
         model = models.DataFlowGroup
         fields = (
             "application",
@@ -106,22 +104,19 @@
 
     status = forms.ChoiceField(
         choices=add_blank_choice(choices.DataFlowStatusChoices),
         required=False,
     )
 
     fieldsets = (
-        (
-            "Data Flow Groups",
-            (
-                "application",
-                "parent",
-                "description",
-                "status",
-            ),
+        FieldSet(
+            "application",
+            "parent",
+            "description",
+            "status",
         ),
     )
     nullable_fields = (
         "parent",
         "application",
         "comments",
     )
@@ -189,32 +184,24 @@
     )
     inherited_status = forms.ChoiceField(
         choices=add_blank_choice(choices.DataFlowStatusChoices),
         required=False,
     )
 
     fieldsets = (
-        (
-            None,
-            (
-                "filter_id",  # Saved Filter
-                "q",  # Search
-                "tag",
-            ),
+        FieldSet(
+            "filter_id",  # Saved Filter
+            "q",  # Search
+            "tag",
         ),
-        (
-            None,
-            (
-                "application",
-                "application_role",
-                "parent_id",
-                "ancestor_id",
-            ),
+        FieldSet(
+            "application",
+            "application_role",
+            "parent_id",
+            "ancestor_id",
         ),
-        (
-            "Status",
-            (
-                "status",
-                "inherited_status",
-            ),
+        FieldSet(
+            "status",
+            "inherited_status",
+            name="Status",
         ),
     )
```

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/forms/objectaliases.py` & `netbox_data_flows-0.9.0/netbox_data_flows/forms/objectaliases.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     NetBoxModelFilterSetForm,
     NetBoxModelImportForm,
 )
 from utilities.forms.fields import (
     TagFilterField,
     DynamicModelMultipleChoiceField,
 )
+from utilities.forms.rendering import FieldSet
 
 from dcim.models import Device
 from ipam.models import Prefix, IPRange, IPAddress
 from virtualization.models import VirtualMachine
 
 from netbox_data_flows import models
 from netbox_data_flows.utils.aliases import AddAliasesForm
@@ -29,21 +30,18 @@
 #
 # Object forms
 #
 
 
 class ObjectAliasForm(NetBoxModelForm):
     fieldsets = (
-        (
-            None,
-            (
-                "name",
-                "description",
-                "tags",
-            ),
+        FieldSet(
+            "name",
+            "description",
+            "tags",
         ),
     )
 
     class Meta:
         model = models.ObjectAlias
         fields = (
             "name",
@@ -59,17 +57,16 @@
 
 class ObjectAliasBulkEditForm(NetBoxModelBulkEditForm):
     model = models.ObjectAlias
 
     description = forms.CharField(max_length=200, required=False)
 
     fieldsets = (
-        (
-            None,
-            ("description",),
+        FieldSet(
+            "description",
         ),
     )
     nullable_fields = ("description",)
 
 
 class ObjectAliasImportForm(NetBoxModelImportForm):
     class Meta:
@@ -114,31 +111,26 @@
         queryset=VirtualMachine.objects.all(),
         required=False,
         label="Aliased Virtual Machines",
         help_text="Any IP address of the virtual machine",
     )
 
     fieldsets = (
-        (
-            None,
-            (
-                "filter_id",  # Saved Filter
-                "q",  # Search
-                "tag",
-            ),
+        FieldSet(
+            "filter_id",  # Saved Filter
+            "q",  # Search
+            "tag",
         ),
-        (
-            "Targets - all targets are OR'ed together, any will match",
-            (
-                "prefixes",
-                "ipranges",
-                "ipaddresses",
-                "devices",
-                "virtual_machines",
-            ),
+        FieldSet(
+            "prefixes",
+            "ipranges",
+            "ipaddresses",
+            "devices",
+            "virtual_machines",
+            name="Targets - all targets are OR'ed together, any will match",
         ),
     )
 
 
 #
 # Special forms
 #
```

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/management/commands/delete_orphaned_aliases.py` & `netbox_data_flows-0.9.0/netbox_data_flows/management/commands/delete_orphaned_aliases.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/migrations/0001_initial.py` & `netbox_data_flows-0.9.0/netbox_data_flows/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py` & `netbox_data_flows-0.9.0/netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/migrations/0005_dataflowgroup_slug.py` & `netbox_data_flows-0.9.0/netbox_data_flows/migrations/0005_dataflowgroup_slug.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/migrations/0008_delete_orphaned_aliases.py` & `netbox_data_flows-0.9.0/netbox_data_flows/migrations/0008_delete_orphaned_aliases.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/migrations/0009_fix_empty_dfg_slugs.py` & `netbox_data_flows-0.9.0/netbox_data_flows/migrations/0009_fix_empty_dfg_slugs.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/models/applications.py` & `netbox_data_flows-0.9.0/netbox_data_flows/models/applications.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from django.contrib.contenttypes.fields import GenericRelation
 from django.db import models
 from django.urls import reverse
 
 from netbox.models import NetBoxModel, OrganizationalModel
+from netbox.models.features import ContactsMixin
 
 
 __all__ = (
     "ApplicationRole",
     "Application",
 )
 
@@ -30,15 +30,15 @@
 
     def get_absolute_url(self):
         return reverse(
             "plugins:netbox_data_flows:applicationrole", args=[self.pk]
         )
 
 
-class Application(NetBoxModel):
+class Application(ContactsMixin, NetBoxModel):
     """Representation of an application hosted on devices or VM"""
 
     name = models.CharField(
         max_length=100, unique=True, help_text="The name of this application"
     )
     description = models.CharField(
         max_length=200,
@@ -48,15 +48,14 @@
         to=ApplicationRole,
         on_delete=models.SET_NULL,
         related_name="applications",
         blank=True,
         null=True,
         help_text="The role of this application",
     )
-    contacts = GenericRelation(to="tenancy.ContactAssignment")
     comments = models.TextField(blank=True)
 
     class Meta:
         ordering = ("name",)
 
     clone_fields = ("role",)
```

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/models/dataflows.py` & `netbox_data_flows-0.9.0/netbox_data_flows/models/dataflows.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from django.core.validators import MaxValueValidator, MinValueValidator
 from django.db import models
 from django.urls import reverse
 from django.utils.functional import cached_property
 
 from netbox.models import NetBoxModel
 from utilities.querysets import RestrictedQuerySet
-from utilities.utils import array_to_string
+from utilities.data import array_to_string
 
 from ipam.constants import SERVICE_PORT_MIN, SERVICE_PORT_MAX
 
 from netbox_data_flows.choices import (
     DataFlowProtocolChoices,
     DataFlowStatusChoices,
     DataFlowInheritedStatusChoices,
```

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/models/groups.py` & `netbox_data_flows-0.9.0/netbox_data_flows/models/groups.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/models/objectaliases.py` & `netbox_data_flows-0.9.0/netbox_data_flows/models/objectaliases.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from django.contrib.contenttypes.fields import GenericForeignKey
-from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import ValidationError
 from django.db import models
 from django.urls import reverse
 
+from core.models import ObjectType
 from netbox.models import NetBoxModel
 from utilities.querysets import RestrictedQuerySet
 
 from ipam.models import Prefix, IPRange, IPAddress
 
 from netbox_data_flows.utils.helpers import get_assignment_querystring
 from netbox_data_flows.utils.helpers import get_device_ipaddresses
@@ -36,22 +36,22 @@
 
 
 class ObjectAliasTargetQuerySet(RestrictedQuerySet):
     def contains(self, *objects):
         """
         Return ObjectAliasTarget containing any one of the objects in parameter
         """
-        ip_ct = ContentType.objects.get_for_model(IPAddress)
+        ip_ct = ObjectType.objects.get_for_model(IPAddress)
 
         if not objects:
             return self.none()
 
         query = models.Q()
         for t in objects:
-            ct = ContentType.objects.get_for_model(t.__class__)
+            ct = ObjectType.objects.get_for_model(t.__class__)
 
             if (ct.app_label, ct.model) in OBJECTALIAS_ASSIGNMENT_MODELS:
                 query |= models.Q(target_type=ct, target_id=t.pk)
             else:
                 try:
                     ip_addresses = get_device_ipaddresses(t)
                 except Exception as e:
@@ -72,33 +72,35 @@
 
     Provide a common interface for working with different DCIM types and a
     type for Many-to-Many generic relationships with any of these types.
 
     This object is intended to be transparent to the user.
     """
 
+    _netbox_private = True
+
     @classmethod
     def get_or_create(cls, target):
         """Return an existing instance for this target or create one"""
         instance = cls.objects.contains(target).first()
         if not instance:
-            ct = ContentType.objects.get_for_model(target.__class__)
+            ct = ObjectType.objects.get_for_model(target.__class__)
             type = (ct.app_label, ct.model)
 
             if type not in OBJECTALIAS_ASSIGNMENT_MODELS:
                 raise TypeError(
                     f"Unsupported type {':'.join(type)} for ObjectAliasTarget"
                 )
 
             instance = cls(target=target)
 
         return instance
 
     target_type = models.ForeignKey(
-        to=ContentType,
+        to="contenttypes.ContentType",
         limit_choices_to=OBJECTALIAS_ASSIGNMENT_QS,
         on_delete=models.PROTECT,
         related_name="+",
     )
     target_id = models.PositiveBigIntegerField()
     target = GenericForeignKey(
         ct_field="target_type",
```

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/navigation.py` & `netbox_data_flows-0.9.0/netbox_data_flows/navigation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from netbox.plugins import PluginMenu, PluginMenuButton, PluginMenuItem
-from utilities.choices import ButtonColorChoices
 
 
 #
 # Utility functions
 #
 
 APP_LABEL = "netbox_data_flows"
@@ -26,25 +25,23 @@
     if "add" in actions:
         buttons.append(
             PluginMenuButton(
                 link=f"plugins:{APP_LABEL}:{model_name}_add",
                 title="Add",
                 icon_class="mdi mdi-plus-thick",
                 permissions=[f"{APP_LABEL}.add_{model_name}"],
-                color=ButtonColorChoices.GREEN,
             )
         )
     if "import" in actions:
         buttons.append(
             PluginMenuButton(
                 link=f"plugins:{APP_LABEL}:{model_name}_import",
                 title="Import",
                 icon_class="mdi mdi-upload",
                 permissions=[f"{APP_LABEL}.add_{model_name}"],
-                color=ButtonColorChoices.CYAN,
             )
         )
 
     return buttons
 
 
 #
```

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/search.py` & `netbox_data_flows-0.9.0/netbox_data_flows/search.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/tables/applications.py` & `netbox_data_flows-0.9.0/netbox_data_flows/tables/groups.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,81 +1,69 @@
 import django_tables2 as tables
 
 from netbox.tables import (
+    ChoiceFieldColumn,
     columns,
     NetBoxTable,
 )
-from tenancy.tables import ContactsColumnMixin
 
-from netbox_data_flows.models import Application, ApplicationRole
+from netbox_data_flows.models import DataFlowGroup
 
 
-__all__ = (
-    "ApplicationRoleTable",
-    "ApplicationTable",
-)
+__all__ = ("DataFlowGroupTable",)
 
 
-class ApplicationRoleTable(NetBoxTable):
-    name = tables.Column(
+class DataFlowGroupTable(NetBoxTable):
+    application = tables.Column(
         linkify=True,
     )
-    application_count = columns.LinkedCountColumn(
-        viewname="plugins:netbox_data_flows:application_list",
-        url_params={"role_id": "pk"},
-        verbose_name="Applications",
-    )
-    tags = columns.TagColumn(
-        url_name="plugins:netbox_data_flows:applicationrole_list"
-    )
-
-    class Meta(NetBoxTable.Meta):
-        model = ApplicationRole
-        fields = (
-            "pk",
-            "id",
-            "name",
-            "slug",
-            "application_count",
-            "description",
-            "tags",
-            "created",
-            "last_updated",
-            "actions",
-        )
-        default_columns = ("name", "description", "application_count")
 
+    application_role = tables.Column(
+        linkify=True,
+        accessor=tables.A("application__role"),
+    )
 
-class ApplicationTable(ContactsColumnMixin, NetBoxTable):
-    name = tables.Column(
+    parent = tables.Column(
         linkify=True,
     )
-    role = tables.Column(
+
+    name = columns.MPTTColumn(
         linkify=True,
     )
+
+    status = ChoiceFieldColumn(accessor=tables.A("inherited_status_display"))
+
     dataflow_count = columns.LinkedCountColumn(
         viewname="plugins:netbox_data_flows:dataflow_list",
-        url_params={"application_id": "pk"},
+        url_params={"dataflowgroup_id": "pk"},
         verbose_name="Data Flows",
     )
+
     tags = columns.TagColumn(
-        url_name="plugins:netbox_data_flows:application_list"
+        url_name="plugins:netbox_data_flows:dataflowgroup_list"
     )
 
     class Meta(NetBoxTable.Meta):
-        model = Application
+        model = DataFlowGroup
         fields = (
             "pk",
             "id",
             "name",
+            "slug",
             "description",
-            "role",
-            "contacts",
-            "comments",
+            "status",
+            "application",
+            "application_role",
+            "parent",
             "dataflow_count",
-            "contacts",
+            "comments",
             "tags",
             "created",
             "last_updated",
             "actions",
         )
-        default_columns = ("name", "role", "dataflow_count")
+        default_columns = (
+            "name",
+            "application",
+            "application_role",
+            "dataflow_count",
+        )
```

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/tables/dataflows.py` & `netbox_data_flows-0.9.0/netbox_data_flows/tables/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/tables/groups.py` & `netbox_data_flows-0.9.0/netbox_data_flows/tables/objectaliases.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,104 @@
 import django_tables2 as tables
 
 from netbox.tables import (
-    ChoiceFieldColumn,
     columns,
     NetBoxTable,
 )
 
-from netbox_data_flows.models import DataFlowGroup
+from netbox_data_flows.models import ObjectAlias, ObjectAliasTarget
+from netbox_data_flows.utils.tables import RuntimeTemplateColumn
 
 
-__all__ = ("DataFlowGroupTable",)
+__all__ = (
+    "ObjectAliasTable",
+    "ObjectAliasTargetTable",
+)
+
 
+class ObjectAliasTargetTable(NetBoxTable):
+    extra_context = None
 
-class DataFlowGroupTable(NetBoxTable):
-    application = tables.Column(
+    type = tables.Column(
+        accessor=tables.A("type_verbose_name"),
+        order_by=tables.A("target_type"),
+        verbose_name="Type",
+    )
+    name = tables.Column(
         linkify=True,
+        orderable=False,
     )
-
-    application_role = tables.Column(
+    target = tables.Column(
         linkify=True,
-        accessor=tables.A("application__role"),
+        verbose_name="Object",
+        orderable=False,
     )
-
     parent = tables.Column(
         linkify=True,
+        verbose_name="Device/VM or VLAN",
+        orderable=False,
     )
-
-    name = columns.MPTTColumn(
-        linkify=True,
+    actions = RuntimeTemplateColumn(
+        template_name="netbox_data_flows/inc/objectaliastarget_actions.html",
+        orderable=False,
     )
 
-    status = ChoiceFieldColumn(accessor=tables.A("inherited_status_display"))
+    def __init__(self, *args, extra_context={}, **kwargs):
+        self.extra_context = dict(extra_context)
+        super().__init__(*args, **kwargs)
+
+    class Meta(NetBoxTable.Meta):
+        model = ObjectAliasTarget
+        fields = (
+            "pk",
+            "id",
+            "type",
+            "name",
+            "target",
+            "parent",
+            "family",
+            "created",
+            "last_updated",
+            "actions",
+        )
+        default_columns = (
+            "type",
+            "name",
+            "parent",
+            "actions",
+        )
 
-    dataflow_count = columns.LinkedCountColumn(
-        viewname="plugins:netbox_data_flows:dataflow_list",
-        url_params={"dataflowgroup_id": "pk"},
-        verbose_name="Data Flows",
-    )
 
+class ObjectAliasTable(NetBoxTable):
+    name = tables.Column(
+        linkify=True,
+    )
+    target_count = tables.Column(
+        verbose_name="Aliased objects",
+    )
+    # dataflow_count = columns.LinkedCountColumn(
+    #    viewname="plugins:netbox_data_flows:dataflow_list",
+    #    url_params={"pk": "pk"},
+    #    verbose_name="Objects",
+    # )
     tags = columns.TagColumn(
-        url_name="plugins:netbox_data_flows:dataflowgroup_list"
+        url_name="plugins:netbox_data_flows:objectalias_list"
     )
 
     class Meta(NetBoxTable.Meta):
-        model = DataFlowGroup
+        model = ObjectAlias
         fields = (
             "pk",
             "id",
             "name",
-            "slug",
             "description",
-            "status",
-            "application",
-            "application_role",
-            "parent",
-            "dataflow_count",
-            "comments",
+            "target_count",
             "tags",
             "created",
             "last_updated",
             "actions",
         )
         default_columns = (
             "name",
-            "application",
-            "application_role",
-            "dataflow_count",
+            "description",
+            "target_count",
         )
```

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/application.html` & `netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/application.html`

 * *Files 7% similar despite different names*

```diff
@@ -11,30 +11,28 @@
 {% endblock %}
 
 {% block content %}
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">Application</h5>
-        <div class="card-body">
-          <table class="table table-hover attr-table">
-            <tr>
-              <th scope="row">Name</th>
-              <td>{{ object.name }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Role</th>
-              <td>{{ object.role|placeholder|linkify }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Description</th>
-              <td>{{ object.description|placeholder }}</td>
-            </tr>
-          </table>
-        </div>
+        <table class="table table-hover attr-table">
+          <tr>
+            <th scope="row">Name</th>
+            <td>{{ object.name }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Role</th>
+            <td>{{ object.role|placeholder|linkify }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Description</th>
+            <td>{{ object.description|placeholder }}</td>
+          </tr>
+        </table>
       </div>
       {% include 'inc/panels/comments.html' %}
       {% include 'inc/panels/custom_fields.html' %}
       {% plugin_left_page object %}
     </div>
     <div class="col col-md-6">
       {% include 'inc/panels/tags.html' %}
@@ -62,11 +60,11 @@
         </div>
       </div>
     </div>
   </div>
 
   <div class="row mb-3">
     <div class="col col-md-12">
-        {% plugin_full_width_page object %}
+      {% plugin_full_width_page object %}
     </div>
   </div>
 {% endblock content %}
```

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/applicationrole.html` & `netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/applicationrole.html`

 * *Files 4% similar despite different names*

```diff
@@ -6,34 +6,32 @@
 {% load render_table from django_tables2 %}
 
 {% block content %}
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">Application Role</h5>
-        <div class="card-body">
-          <table class="table table-hover attr-table">
-            <tr>
-              <th scope="row">Name</th>
-              <td>{{ object.name }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Slug</th>
-              <td>{{ object.slug }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Description</th>
-              <td>{{ object.description|placeholder }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Applications</th>
-              <td>{{ object.applications.count }}</td>
-            </tr>
-          </table>
-        </div>
+        <table class="table table-hover attr-table">
+          <tr>
+            <th scope="row">Name</th>
+            <td>{{ object.name }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Slug</th>
+            <td>{{ object.slug }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Description</th>
+            <td>{{ object.description|placeholder }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Applications</th>
+            <td>{{ object.applications.count }}</td>
+          </tr>
+        </table>
       </div>
       {% include 'inc/panels/custom_fields.html' %}
       {% plugin_left_page object %}
     </div>
     <div class="col col-md-6">
       {% include 'inc/panels/tags.html' %}
       {% plugin_right_page object %}
```

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/dataflow.html` & `netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/dataflow.html`

 * *Files 8% similar despite different names*

```diff
@@ -13,87 +13,83 @@
 {% endblock %}
 
 {% block content %}
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">Data Flow</h5>
-        <div class="card-body">
-          <table class="table table-hover attr-table">
-            <tr>
-              <th scope="row">Application</th>
-              <td>{{ object.application|linkify }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Group</th>
-              <td>
-                {{ object.group|placeholder|linkify }}
-              </td>
-            </tr>
-            <tr>
-              <th scope="row">Description</th>
-              <td>{{ object.description|placeholder }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Status</th>
-              <td>{% badge object.inherited_status_display bg_color=object.get_status_color %}</td>
-            </tr>
-          </table>
-        </div>
+        <table class="table table-hover attr-table">
+          <tr>
+            <th scope="row">Application</th>
+            <td>{{ object.application|linkify }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Group</th>
+            <td>
+              {{ object.group|placeholder|linkify }}
+            </td>
+          </tr>
+          <tr>
+            <th scope="row">Description</th>
+            <td>{{ object.description|placeholder }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Status</th>
+            <td>{% badge object.inherited_status_display bg_color=object.get_status_color %}</td>
+          </tr>
+        </table>
       </div>
       {% include 'inc/panels/tags.html' %}
       {% include 'inc/panels/comments.html' %}
       {% include 'inc/panels/custom_fields.html' %}
       {% plugin_left_page object %}
     </div>
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">Specifications</h5>
-        <div class="card-body">
-          <table class="table table-hover attr-table">
-            <tr>
-              <th scope="row">Protocol</th>
-              <td>{{ object.get_protocol_display|placeholder }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Source ports</th>
-              <td>{{ object.source_port_list|placeholder }}</td>
+        <table class="table table-hover attr-table">
+          <tr>
+            <th scope="row">Protocol</th>
+            <td>{{ object.get_protocol_display|placeholder }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Source ports</th>
+            <td>{{ object.source_port_list|placeholder }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Destination ports</th>
+            <td>{{ object.destination_port_list|placeholder }}</td>
+          </tr>
+          {% for o in sources %}
+            <tr>
+              {% if forloop.first %}
+                <th scope="row" rowspan="{{ sources|length }}">Sources</th>
+              {% endif %}
+              <td>{{ o|linkify }}</td>
+            </tr>
+          {% empty %}
+            <tr>
+              <th scope="row">Sources</th>
+              <td>{{ ""|placeholder }}</td>
+            </tr>
+          {% endfor %}
+          {% for o in destinations %}
+            <tr>
+              {% if forloop.first %}
+                <th scope="row" rowspan="{{ destinations|length }}">Destinations</th>
+              {% endif %}
+              <td>{{ o|linkify }}</td>
             </tr>
+          {% empty %}
             <tr>
-              <th scope="row">Destination ports</th>
-              <td>{{ object.destination_port_list|placeholder }}</td>
+              <th scope="row">Destinations</th>
+              <td>{{ ""|placeholder }}</td>
             </tr>
-            {% for o in sources %}
-              <tr>
-                {% if forloop.first %}
-                  <th scope="row" rowspan="{{ sources|length }}">Sources</th>
-                {% endif %}
-                <td>{{ o|linkify }}</td>
-              </tr>
-            {% empty %}
-              <tr>
-                <th scope="row">Sources</th>
-                <td>{{ ""|placeholder }}</td>
-              </tr>
-            {% endfor %}
-            {% for o in destinations %}
-              <tr>
-                {% if forloop.first %}
-                  <th scope="row" rowspan="{{ destinations|length }}">Destinations</th>
-                {% endif %}
-                <td>{{ o|linkify }}</td>
-              </tr>
-            {% empty %}
-              <tr>
-                <th scope="row">Destinations</th>
-                <td>{{ ""|placeholder }}</td>
-              </tr>
-            {% endfor %}
-          </table>
-        </div>
+          {% endfor %}
+        </table>
       </div>
       {% plugin_right_page object %}
     </div>
   </div>
 
   {% if children_table %}
   <div class="row mb-3">
```

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/dataflow_list.html` & `netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/dataflow_list.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 {% extends 'generic/object_list.html' %}
 
 {% block title %}
   {{ model|meta:"verbose_name_plural"|bettertitle }}{% if as_rules %} as Rules{% endif %}
 {% endblock %}
 
-{% block extra_controls %}
+{# Hidden as currently not used #}
+{# block extra_controls % }
   {% if as_rules %}
     <a href="{% url 'plugins:netbox_data_flows:dataflow_list' %}" type="button" class="btn btn-sm btn-outline-secondary">
       <i class="mdi mdi-file-tree-outline"></i> As Data Flows
     </a>
   {% else %}
     <a href="{% url 'plugins:netbox_data_flows:dataflow_rules' %}" type="button" class="btn btn-sm btn-outline-secondary">
       <i class="mdi mdi-playlist-check"></i> As rules
     </a>
   {% endif %}
-{% endblock extra_controls %}
+{ % endblock extra_controls #}
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
 {% extends 'generic/object_list.html' %} {% block title %} {{ model|meta:
 "verbose_name_plural"|bettertitle }}{% if as_rules %} as Rules{% endif %} {%
-endblock %} {% block extra_controls %} {% if as_rules %}
+endblock %} {# Hidden as currently not used #} {# block extra_controls % } {%
+if as_rules %}
 _A_s_ _D_a_t_a_ _F_l_o_w_s
 {% else %}
 _A_s_ _r_u_l_e_s
-{% endif %} {% endblock extra_controls %}
+{% endif %} { % endblock extra_controls #}
```

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/dataflow_tab.html` & `netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/dataflow_tab.html`

 * *Files 8% similar despite different names*

```diff
@@ -33,11 +33,7 @@
         <div class="card-body table-responsive">
           {% render_table dataflow_destinations_table %}
         </div>
       </div>
     </div>
   </div>
 {% endblock %}
-
-{% block modals %}
-    {{ block.super }}
-{% endblock modals %}
```

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html` & `netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html`

 * *Files 15% similar despite different names*

```diff
@@ -14,30 +14,28 @@
 {% endblock %}
 
 {% block content %}
   <div class="row mb-3">
     <div class="col col-md-12">
       <div class="card">
         <h5 class="card-header">Specifications</h5>
-        <div class="card-body">
-          <table class="table table-hover attr-table">
-            <tr>
-              <th scope="row">Protocol</th>
-              <td>{{ object.get_protocol_display|placeholder }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Source ports</th>
-              <td>{{ object.source_port_list|placeholder }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Destination ports</th>
-              <td>{{ object.destination_port_list|placeholder }}</td>
-            </tr>
-          </table>
-        </div>
+        <table class="table table-hover attr-table">
+          <tr>
+            <th scope="row">Protocol</th>
+            <td>{{ object.get_protocol_display|placeholder }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Source ports</th>
+            <td>{{ object.source_port_list|placeholder }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Destination ports</th>
+            <td>{{ object.destination_port_list|placeholder }}</td>
+          </tr>
+        </table>
       </div>
     </div>
   </div>
 
   <div class="row mb-3">
     <div class="col col-md-12">
       <div class="card">
```

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html` & `netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html`

 * *Files 2% similar despite different names*

```diff
@@ -11,48 +11,46 @@
 {% endblock %}
 
 {% block content %}
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">Data Flow Group</h5>
-        <div class="card-body">
-          <table class="table table-hover attr-table">
-            <tr>
-              <th scope="row">Application</th>
-              <td>{{ object.application|linkify }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Parent</th>
-              <td>
-                {{ object.parent|placeholder|linkify }}
-              </td>
-            </tr>
-            <tr>
-              <th scope="row">Name</th>
-              <td>
-                {{ object.name }}
-              </td>
-            </tr>
-            <tr>
-              <th scope="row">Slug</th>
-              <td>
-                {{ object.slug }}
-              </td>
-            </tr>
-            <tr>
-              <th scope="row">Description</th>
-              <td>{{ object.description|placeholder }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Status</th>
-              <td>{% badge object.inherited_status_display bg_color=object.get_status_color %}</td>
-            </tr>
-          </table>
-        </div>
+        <table class="table table-hover attr-table">
+          <tr>
+            <th scope="row">Application</th>
+            <td>{{ object.application|linkify }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Parent</th>
+            <td>
+              {{ object.parent|placeholder|linkify }}
+            </td>
+          </tr>
+          <tr>
+            <th scope="row">Name</th>
+            <td>
+              {{ object.name }}
+            </td>
+          </tr>
+          <tr>
+            <th scope="row">Slug</th>
+            <td>
+              {{ object.slug }}
+            </td>
+          </tr>
+          <tr>
+            <th scope="row">Description</th>
+            <td>{{ object.description|placeholder }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Status</th>
+            <td>{% badge object.inherited_status_display bg_color=object.get_status_color %}</td>
+          </tr>
+        </table>
       </div>
       {% include 'inc/panels/tags.html' %}
       {% include 'inc/panels/comments.html' %}
       {% include 'inc/panels/custom_fields.html' %}
       {% plugin_left_page object %}
     </div>
     <div class="col col-md-6">
@@ -90,11 +88,11 @@
       </div>
     </div>
   </div>
   {% endif %}
 
   <div class="row mb-3">
     <div class="col col-md-12">
-        {% plugin_full_width_page object %}
+      {% plugin_full_width_page object %}
     </div>
   </div>
 {% endblock content %}
```

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/objectalias.html` & `netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/objectalias.html`

 * *Files 4% similar despite different names*

```diff
@@ -14,45 +14,43 @@
 {% endblock extra_controls %}
 
 {% block content %}
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">Object Alias</h5>
-        <div class="card-body">
-          <table class="table table-hover attr-table">
-            <tr>
-              <th scope="row">Name</th>
-              <td>{{ object.name }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Description</th>
-              <td>{{ object.description|placeholder }}</td>
-            </tr>
-          </table>
-        </div>
+        <table class="table table-hover attr-table">
+          <tr>
+            <th scope="row">Name</th>
+            <td>{{ object.name }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Description</th>
+            <td>{{ object.description|placeholder }}</td>
+          </tr>
+        </table>
       </div>
       {% include 'inc/panels/tags.html' %}
       {% include 'inc/panels/comments.html' %}
       {% include 'inc/panels/custom_fields.html' %}
       {% plugin_left_page object %}
     </div>
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">Member objects</h5>
         <div class="card-body table-responsive">
           {% render_table targets_table %}
         </div>
-          {% if perms.netbox_data_flows.change_objectalias %}
-            <div class="card-footer text-end noprint">
-              <a href="{% url 'plugins:netbox_data_flows:objectalias_addtarget' object.pk %}" class="btn btn-sm btn-primary">
-                <i class="mdi mdi-plus-thick"></i> Add aliased objects
-              </a>
-            </div>
-          {% endif %}
+      {% if perms.netbox_data_flows.change_objectalias %}
+        <div class="card-footer text-end noprint">
+          <a href="{% url 'plugins:netbox_data_flows:objectalias_addtarget' object.pk %}" class="btn btn-sm btn-primary">
+            <i class="mdi mdi-plus-thick"></i> Add aliased objects
+          </a>
+        </div>
+      {% endif %}
       </div>
       {% plugin_right_page object %}
     </div>
   </div>
 
   <div class="row mb-3">
     <div class="col col-md-12">
@@ -74,11 +72,11 @@
         </div>
       </div>
     </div>
   </div>
 
   <div class="row mb-3">
     <div class="col col-md-12">
-        {% plugin_full_width_page object %}
+      {% plugin_full_width_page object %}
     </div>
   </div>
 {% endblock content %}
```

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html` & `netbox_data_flows-0.9.0/netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html`

 * *Files 0% similar despite different names*

```diff
@@ -24,19 +24,19 @@
             <h5 class="modal-title">Confirm unlinking</h5>
           </div>
           <div class="modal-body">
             <p>Are you sure you want to <strong class="text-warning">unlink</strong> <strong>{{ alias }}</strong> from <strong>{{ object }}</strong>?</p>
             {% render_form form %}
           </div>
           <div class="modal-footer">
-            {% if return_url %}
+          {% if return_url %}
             <a href="{{ return_url }}" class="btn btn-outline-secondary">Cancel</a>
-            {% else %}
+          {% else %}
             <button type="button" class="btn btn-outline-secondary" data-bs-dismiss="modal">Cancel</button>
-            {% endif %}
+          {% endif %}
             <button type="submit" class="btn btn-warning">Unlink</button>
           </div>
         </form>
       </div>
     </div>
   </div>
 {% endblock %}
```

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/urls.py` & `netbox_data_flows-0.9.0/netbox_data_flows/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/utils/aliases.py` & `netbox_data_flows-0.9.0/netbox_data_flows/utils/aliases.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,38 +6,30 @@
 from django.db.models import ProtectedError
 from django.shortcuts import get_object_or_404, render, redirect
 from django.utils.html import escape
 from django.utils.safestring import mark_safe
 
 from netbox.views import generic as generic_views
 
-try:
-    from extras.signals import clear_events
-except ImportError:
-    # COMPAT: NetBox 3.6.x
-    from extras.signals import clear_webhooks as clear_events
+from extras.signals import clear_events
 from utilities.error_handlers import handle_protectederror
 from utilities.exceptions import AbortRequest, PermissionsViolation
-from utilities.forms import (
-    restrict_form_fields,
-    ConfirmationForm,
-    BootstrapMixin,
-)
+from utilities.forms import restrict_form_fields, ConfirmationForm
 from utilities.permissions import get_permission_for_model
-from utilities.utils import normalize_querydict
+from utilities.querydict import normalize_querydict
 
 
 __all__ = (
     "AddAliasesForm",
     "AddAliasesView",
     "RemoveAliasView",
 )
 
 
-class AddAliasesForm(BootstrapMixin, forms.Form):
+class AddAliasesForm(forms.Form):
     """Link aliased objects to an object"""
 
     aliased_fields = tuple()
 
     def get_aliased_objects(self):
         for field_name in self.aliased_fields:
             if self.cleaned_data[field_name]:
```

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/utils/helpers.py` & `netbox_data_flows-0.9.0/netbox_data_flows/utils/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from django.contrib.contenttypes.models import ContentType
-
+from core.models import ObjectType
 from ipam.models import IPAddress
 
 from django.db.models import Q
 from django.utils.safestring import mark_safe
 
 
 def object_list_to_string(
@@ -35,15 +34,15 @@
 
 def _get_ip_qs(device):
     """
     Return a querystring matching any IP assigned to the device
     """
 
     interfaces = device.interfaces.all()
-    ct = ContentType.objects.get_for_model(interfaces.model)
+    ct = ObjectType.objects.get_for_model(interfaces.model)
 
     return Q(
         assigned_object_type=ct.pk,
         assigned_object_id__in=interfaces,
     )
```

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/views/applicationroles.py` & `netbox_data_flows-0.9.0/netbox_data_flows/views/applicationroles.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/views/applications.py` & `netbox_data_flows-0.9.0/netbox_data_flows/views/applications.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/views/dataflows.py` & `netbox_data_flows-0.9.0/netbox_data_flows/views/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/views/groups.py` & `netbox_data_flows-0.9.0/netbox_data_flows/views/groups.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/views/model_tabs.py` & `netbox_data_flows-0.9.0/netbox_data_flows/views/model_tabs.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows/views/objectaliases.py` & `netbox_data_flows-0.9.0/netbox_data_flows/views/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows.egg-info/PKG-INFO` & `netbox_data_flows-0.9.0/netbox_data_flows.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: netbox-data-flows
-Version: 0.8.3
+Version: 0.9.0
 Summary: NetBox plugin to document data flows between systems and applications.
 Author: Thomas Fargeix
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/Alef-Burzmali/netbox-data-flows
 Project-URL: Bug Tracker, https://github.com/Alef-Burzmali/netbox-data-flows/issues
 Keywords: netbox,netbox-plugins
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: System :: Networking
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # netbox-data-flows
 
 Plugin for [NetBox](https://github.com/netbox-community/netbox) to document
 Data Flows between systems and applications.
@@ -34,16 +34,18 @@
 
 ## Installation and Configuration
 
 Full reference: [Using Plugins - NetBox Documentation](https://docs.netbox.dev/en/stable/plugins/)
 
 ### Requirements
 
-* NetBox (=3.7.x)
-* Python 3.8 or higher
+* NetBox (>=4.0.0)
+* Python 3.10 or higher
+
+Use version 0.8.x if you need compatibility with NetBox 3.7.x
 
 This is the last version compatible with NetBox 3. Future releases will support 4.0 only.
 
 *Note:* the plugin uses some classes that are not explicitely exported in 
 NetBox's plugin API, such as MPTT Tree-based models. Upward compatiblity is
 not guaranteed.
```

### Comparing `netbox_data_flows-0.8.3/netbox_data_flows.egg-info/SOURCES.txt` & `netbox_data_flows-0.9.0/netbox_data_flows.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,34 +16,28 @@
 netbox_data_flows/api/__init__.py
 netbox_data_flows/api/urls.py
 netbox_data_flows/api/views.py
 netbox_data_flows/api/serializers/__init__.py
 netbox_data_flows/api/serializers/applications.py
 netbox_data_flows/api/serializers/dataflows.py
 netbox_data_flows/api/serializers/groups.py
-netbox_data_flows/api/serializers/nested.py
 netbox_data_flows/api/serializers/objectaliases.py
 netbox_data_flows/filtersets/__init__.py
 netbox_data_flows/filtersets/addins.py
 netbox_data_flows/filtersets/applications.py
 netbox_data_flows/filtersets/dataflows.py
 netbox_data_flows/filtersets/filters.py
 netbox_data_flows/filtersets/groups.py
 netbox_data_flows/filtersets/objectaliases.py
 netbox_data_flows/forms/__init__.py
 netbox_data_flows/forms/applicationroles.py
 netbox_data_flows/forms/applications.py
 netbox_data_flows/forms/dataflows.py
 netbox_data_flows/forms/groups.py
 netbox_data_flows/forms/objectaliases.py
-netbox_data_flows/graphql/__init__.py
-netbox_data_flows/graphql/applications.py
-netbox_data_flows/graphql/dataflows.py
-netbox_data_flows/graphql/groups.py
-netbox_data_flows/graphql/objectaliases.py
 netbox_data_flows/management/__init__.py
 netbox_data_flows/management/commands/__init__.py
 netbox_data_flows/management/commands/delete_orphaned_aliases.py
 netbox_data_flows/migrations/0001_initial.py
 netbox_data_flows/migrations/0002_alter_objectalias_options.py
 netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py
 netbox_data_flows/migrations/0004_reindex_netbox_data_flows.py
```

### Comparing `netbox_data_flows-0.8.3/pyproject.toml` & `netbox_data_flows-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = "netbox-data-flows"
 description = "NetBox plugin to document data flows between systems and applications."
 authors = [
   { name="Thomas Fargeix" },
 ]
 license = {text = "Apache 2.0"}
 readme = {file = "README.md", content-type = "text/markdown"}
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 keywords = ["netbox", "netbox-plugins"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Plugins",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Topic :: System :: Networking",
```

