# Comparing `tmp/fal-0.9.5.tar.gz` & `tmp/fal-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fal-0.9.5.tar", max compression
+gzip compressed data, was "fal-1.0.0.tar", last modified: Fri May 10 14:49:30 2024, max compression
```

## Comparing `fal-0.9.5.tar` & `fal-1.0.0.tar`

### file list

```diff
@@ -1,90 +1,154 @@
--rw-r--r--   0        0        0    10531 2023-07-17 22:49:47.483137 fal-0.9.5/README.md
--rw-r--r--   0        0        0     2429 2023-07-17 22:49:59.455077 fal-0.9.5/pyproject.toml
--rw-r--r--   0        0        0      639 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal/__init__.py
--rw-r--r--   0        0        0       18 2023-07-17 22:49:59.947077 fal-0.9.5/src/dbt/adapters/fal/__version__.py
--rw-r--r--   0        0        0      392 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal/connections.py
--rw-r--r--   0        0        0     3369 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal/impl.py
--rw-r--r--   0        0        0     2768 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal/load_db_profile.py
--rw-r--r--   0        0        0     4091 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal/wrappers.py
--rw-r--r--   0        0        0      344 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/__init__.py
--rw-r--r--   0        0        0       18 2023-07-17 22:49:59.947077 fal-0.9.5/src/dbt/adapters/fal_experimental/__version__.py
--rw-r--r--   0        0        0     4861 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/adapter.py
--rw-r--r--   0        0        0     8381 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/adapter_support.py
--rw-r--r--   0        0        0     1627 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/connections.py
--rw-r--r--   0        0        0     8714 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/impl.py
--rw-r--r--   0        0        0     3192 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/support/athena.py
--rw-r--r--   0        0        0     2686 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/support/bigquery.py
--rw-r--r--   0        0        0      980 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/support/duckdb.py
--rw-r--r--   0        0        0     2977 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/support/postgres.py
--rw-r--r--   0        0        0     1633 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/support/redshift.py
--rw-r--r--   0        0        0     2781 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/support/snowflake.py
--rw-r--r--   0        0        0      821 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/support/trino.py
--rw-r--r--   0        0        0       25 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/telemetry/__init__.py
--rw-r--r--   0        0        0    10813 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/telemetry/telemetry.py
--rw-r--r--   0        0        0     6572 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/teleport.py
--rw-r--r--   0        0        0     1153 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/teleport_adapter_support.py
--rw-r--r--   0        0        0     4719 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/teleport_support/duckdb.py
--rw-r--r--   0        0        0     2972 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/teleport_support/snowflake.py
--rw-r--r--   0        0        0     1256 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/utils/__init__.py
--rw-r--r--   0        0        0     9804 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/utils/environments.py
--rw-r--r--   0        0        0     1970 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/utils/yaml_helper.py
--rw-r--r--   0        0        0      208 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/fal/adapters/python/__init__.py
--rw-r--r--   0        0        0    11898 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/fal/adapters/python/connections.py
--rw-r--r--   0        0        0    10015 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/fal/adapters/python/impl.py
--rw-r--r--   0        0        0      181 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/fal/adapters/teleport/__init__.py
--rw-r--r--   0        0        0     3498 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/fal/adapters/teleport/impl.py
--rw-r--r--   0        0        0     2310 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/fal/adapters/teleport/info.py
--rw-r--r--   0        0        0       52 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/include/fal/__init__.py
--rw-r--r--   0        0        0       70 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/include/fal/dbt_project.yml
--rw-r--r--   0        0        0     1213 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/include/fal/macros/materializations/table.sql
--rw-r--r--   0        0        0      265 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/include/fal/macros/teleport_duckdb.sql
--rw-r--r--   0        0        0      921 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/include/fal/macros/teleport_snowflake.sql
--rw-r--r--   0        0        0       52 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/include/fal_experimental/__init__.py
--rw-r--r--   0        0        0       83 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/include/fal_experimental/dbt_project.yml
--rw-r--r--   0        0        0      989 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/include/fal_experimental/macros/materializations/table.sql
--rw-r--r--   0        0        0     1905 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/__init__.py
--rw-r--r--   0        0        0      238 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/dbt/__init__.py
--rw-r--r--   0        0        0       30 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/dbt/cli/__init__.py
--rw-r--r--   0        0        0     7650 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/dbt/cli/args.py
--rw-r--r--   0        0        0     1550 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/dbt/cli/cli.py
--rw-r--r--   0        0        0     5482 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/dbt/cli/dbt_runner.py
--rw-r--r--   0        0        0     5857 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/dbt/cli/fal_runner.py
--rw-r--r--   0        0        0     4475 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/dbt/cli/flow_runner.py
--rw-r--r--   0        0        0       56 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/dbt/cli/model_generator/__init__.py
--rw-r--r--   0        0        0     5543 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/dbt/cli/model_generator/model_generator.py
--rw-r--r--   0        0        0     3180 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/dbt/cli/model_generator/module_check.py
--rw-r--r--   0        0        0     9759 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/dbt/cli/selectors.py
--rw-r--r--   0        0        0    12349 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/dbt/fal_script.py
--rw-r--r--   0        0        0        0 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/dbt/feature_store/__init__.py
--rw-r--r--   0        0        0      401 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/dbt/feature_store/feature.py
--rw-r--r--   0        0        0        0 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/dbt/integration/__init__.py
--rw-r--r--   0        0        0    24589 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/dbt/integration/lib.py
--rw-r--r--   0        0        0     3273 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/integration/logger.py
--rw-r--r--   0        0        0     1867 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/integration/magics.py
--rw-r--r--   0        0        0     9103 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/integration/parse.py
--rw-r--r--   0        0        0    27168 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/integration/project.py
--rw-r--r--   0        0        0        0 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/integration/utils/__init__.py
--rw-r--r--   0        0        0     1970 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/integration/utils/yaml_helper.py
--rw-r--r--   0        0        0      317 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/integration/version.py
--rw-r--r--   0        0        0     1530 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/new/project.py
--rw-r--r--   0        0        0     8411 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/node_graph.py
--rw-r--r--   0        0        0        0 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/packages/__init__.py
--rw-r--r--   0        0        0     1603 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/packages/bridge.py
--rw-r--r--   0        0        0     5562 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/packages/dependency_analysis.py
--rw-r--r--   0        0        0      805 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/packages/environments/__init__.py
--rw-r--r--   0        0        0     9499 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/packages/environments/base.py
--rw-r--r--   0        0        0     4407 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/packages/environments/conda.py
--rw-r--r--   0        0        0     3381 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/packages/environments/virtual_env.py
--rw-r--r--   0        0        0     4823 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/packages/isolated_runner.py
--rw-r--r--   0        0        0        0 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/planner/__init__.py
--rw-r--r--   0        0        0     5669 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/planner/executor.py
--rw-r--r--   0        0        0     6496 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/planner/plan.py
--rw-r--r--   0        0        0     6790 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/planner/schedule.py
--rw-r--r--   0        0        0     9079 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/planner/tasks.py
--rw-r--r--   0        0        0        0 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/telemetry/__init__.py
--rw-r--r--   0        0        0    11487 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/telemetry/telemetry.py
--rw-r--r--   0        0        0     3060 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/typing.py
--rw-r--r--   0        0        0     1728 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/utils.py
--rw-r--r--   0        0        0       33 2023-07-17 22:49:47.499137 fal-0.9.5/tests/_fal_testing/__init__.py
--rw-r--r--   0        0        0     1794 2023-07-17 22:49:47.499137 fal-0.9.5/tests/_fal_testing/utils.py
--rw-r--r--   0        0        0    12552 1970-01-01 00:00:00.000000 fal-0.9.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.128540 fal-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-10 14:49:23.000000 fal-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-10 14:49:30.128540 fal-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-10 14:49:23.000000 fal-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.124540 fal-1.0.0/fal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-10 14:49:30.000000 fal-1.0.0/fal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-10 14:49:30.000000 fal-1.0.0/fal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:49:30.000000 fal-1.0.0/fal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-10 14:49:30.000000 fal-1.0.0/fal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-10 14:49:30.000000 fal-1.0.0/fal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-10 14:49:30.000000 fal-1.0.0/fal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.108540 fal-1.0.0/openapi-fal-rest/
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.108540 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.108540 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.108540 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/applications/app_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.108540 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/billing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/billing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/billing/get_user_details.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.108540 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/files/check_dir_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/files/upload_local_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.108540 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/workflows/create_or_update_workflow_workflows_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/workflows/delete_workflow_workflows_user_id_workflow_name_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/workflows/execute_workflow_workflows_user_id_workflow_name_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/workflows/get_workflow_workflows_user_id_workflow_name_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/workflows/get_workflows_workflows_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.112540 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/app_metadata_response_app_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/body_upload_local_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/customer_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/execute_workflow_workflows_user_id_workflow_name_post_json_body_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/execute_workflow_workflows_user_id_workflow_name_post_response_200_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/hash_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/lock_reason.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/page_workflow_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/typed_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/workflow_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/workflow_contents_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/workflow_contents_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/workflow_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/workflow_detail_contents_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/workflow_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/workflow_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/workflow_node_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/workflow_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/workflow_schema_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/workflow_schema_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-10 14:49:23.000000 fal-1.0.0/openapi_rest.config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-10 14:49:23.000000 fal-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 14:49:30.128540 fal-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.104540 fal-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.116540 fal-1.0.0/src/fal/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-10 14:49:29.000000 fal-1.0.0/src/fal/_fal_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36287 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13826 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.116540 fal-1.0.0/src/fal/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/auth/auth0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/auth/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.116540 fal-1.0.0/src/fal/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/cli/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/cli/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/cli/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/cli/secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.120540 fal-1.0.0/src/fal/console/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/console/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/console/ux.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.120540 fal-1.0.0/src/fal/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/exceptions/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/exceptions/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/flags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.120540 fal-1.0.0/src/fal/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/logging/isolate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/logging/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/logging/trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/logging/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/rest_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19976 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.120540 fal-1.0.0/src/fal/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/toolkit/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.120540 fal-1.0.0/src/fal/toolkit/file/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/toolkit/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/toolkit/file/file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.120540 fal-1.0.0/src/fal/toolkit/file/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/toolkit/file/providers/fal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/toolkit/file/providers/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/toolkit/file/providers/r2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/toolkit/file/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.120540 fal-1.0.0/src/fal/toolkit/image/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/toolkit/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/toolkit/image/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/toolkit/optimize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.120540 fal-1.0.0/src/fal/toolkit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/toolkit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15487 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/toolkit/utils/download_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14682 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.124540 fal-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:23.000000 fal-1.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.124540 fal-1.0.0/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:23.000000 fal-1.0.0/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-10 14:49:23.000000 fal-1.0.0/tests/cli/test_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-10 14:49:23.000000 fal-1.0.0/tests/cli/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-10 14:49:23.000000 fal-1.0.0/tests/cli/test_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-10 14:49:23.000000 fal-1.0.0/tests/cli/test_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-10 14:49:23.000000 fal-1.0.0/tests/cli/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-10 14:49:23.000000 fal-1.0.0/tests/cli/test_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-10 14:49:23.000000 fal-1.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-05-10 14:49:23.000000 fal-1.0.0/tests/integration_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.124540 fal-1.0.0/tests/mainify_package/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-10 14:49:23.000000 fal-1.0.0/tests/mainify_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-10 14:49:23.000000 fal-1.0.0/tests/mainify_package/impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-10 14:49:23.000000 fal-1.0.0/tests/mainify_package/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-10 14:49:23.000000 fal-1.0.0/tests/mainify_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17322 2024-05-10 14:49:23.000000 fal-1.0.0/tests/test_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16201 2024-05-10 14:49:23.000000 fal-1.0.0/tests/test_stability.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.124540 fal-1.0.0/tests/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-10 14:49:23.000000 fal-1.0.0/tests/toolkit/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-05-10 14:49:23.000000 fal-1.0.0/tests/toolkit/image_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.124540 fal-1.0.0/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-10 14:49:23.000000 fal-1.0.0/tools/demo_script.py
```

