# Comparing `tmp/fal-1.0.0.tar.gz` & `tmp/fal-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fal-1.0.0.tar", last modified: Fri May 10 14:49:30 2024, max compression
+gzip compressed data, was "fal-1.0.1.tar", last modified: Fri May 10 22:29:31 2024, max compression
```

## Comparing `fal-1.0.0.tar` & `fal-1.0.1.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.128540 fal-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-10 14:49:23.000000 fal-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-10 14:49:30.128540 fal-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-10 14:49:23.000000 fal-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.124540 fal-1.0.0/fal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-10 14:49:30.000000 fal-1.0.0/fal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-10 14:49:30.000000 fal-1.0.0/fal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:49:30.000000 fal-1.0.0/fal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-10 14:49:30.000000 fal-1.0.0/fal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-10 14:49:30.000000 fal-1.0.0/fal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-10 14:49:30.000000 fal-1.0.0/fal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.108540 fal-1.0.0/openapi-fal-rest/
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.108540 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.108540 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.108540 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/applications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/applications/app_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.108540 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/billing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/billing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/billing/get_user_details.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.108540 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/files/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/files/check_dir_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/files/upload_local_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.108540 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/workflows/create_or_update_workflow_workflows_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/workflows/delete_workflow_workflows_user_id_workflow_name_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/workflows/execute_workflow_workflows_user_id_workflow_name_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/workflows/get_workflow_workflows_user_id_workflow_name_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/workflows/get_workflows_workflows_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.112540 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/app_metadata_response_app_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/body_upload_local_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/customer_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/execute_workflow_workflows_user_id_workflow_name_post_json_body_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/execute_workflow_workflows_user_id_workflow_name_post_response_200_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/hash_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/lock_reason.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/page_workflow_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/typed_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/workflow_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/workflow_contents_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/workflow_contents_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/workflow_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/workflow_detail_contents_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/workflow_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/workflow_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/workflow_node_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/workflow_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/workflow_schema_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/workflow_schema_output.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/openapi_fal_rest/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-10 14:49:23.000000 fal-1.0.0/openapi-fal-rest/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-10 14:49:23.000000 fal-1.0.0/openapi_rest.config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-10 14:49:23.000000 fal-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 14:49:30.128540 fal-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.104540 fal-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.116540 fal-1.0.0/src/fal/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-10 14:49:29.000000 fal-1.0.0/src/fal/_fal_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    36287 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13826 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.116540 fal-1.0.0/src/fal/auth/
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/auth/auth0.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/auth/local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.116540 fal-1.0.0/src/fal/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/cli/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/cli/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/cli/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/cli/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/cli/secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.120540 fal-1.0.0/src/fal/console/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/console/icons.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/console/ux.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.120540 fal-1.0.0/src/fal/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/exceptions/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/exceptions/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/flags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.120540 fal-1.0.0/src/fal/logging/
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/logging/isolate.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/logging/style.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/logging/trace.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/logging/user.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/rest_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    19976 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.120540 fal-1.0.0/src/fal/toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/toolkit/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.120540 fal-1.0.0/src/fal/toolkit/file/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/toolkit/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/toolkit/file/file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.120540 fal-1.0.0/src/fal/toolkit/file/providers/
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/toolkit/file/providers/fal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/toolkit/file/providers/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/toolkit/file/providers/r2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/toolkit/file/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.120540 fal-1.0.0/src/fal/toolkit/image/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/toolkit/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/toolkit/image/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/toolkit/optimize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.120540 fal-1.0.0/src/fal/toolkit/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/toolkit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15487 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/toolkit/utils/download_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14682 2024-05-10 14:49:23.000000 fal-1.0.0/src/fal/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.124540 fal-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:23.000000 fal-1.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.124540 fal-1.0.0/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:23.000000 fal-1.0.0/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-10 14:49:23.000000 fal-1.0.0/tests/cli/test_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-10 14:49:23.000000 fal-1.0.0/tests/cli/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-10 14:49:23.000000 fal-1.0.0/tests/cli/test_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-10 14:49:23.000000 fal-1.0.0/tests/cli/test_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-10 14:49:23.000000 fal-1.0.0/tests/cli/test_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-10 14:49:23.000000 fal-1.0.0/tests/cli/test_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-10 14:49:23.000000 fal-1.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-05-10 14:49:23.000000 fal-1.0.0/tests/integration_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.124540 fal-1.0.0/tests/mainify_package/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-10 14:49:23.000000 fal-1.0.0/tests/mainify_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-10 14:49:23.000000 fal-1.0.0/tests/mainify_package/impl.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-10 14:49:23.000000 fal-1.0.0/tests/mainify_package/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-10 14:49:23.000000 fal-1.0.0/tests/mainify_target.py
--rw-r--r--   0 runner    (1001) docker     (127)    17322 2024-05-10 14:49:23.000000 fal-1.0.0/tests/test_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    16201 2024-05-10 14:49:23.000000 fal-1.0.0/tests/test_stability.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.124540 fal-1.0.0/tests/toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-10 14:49:23.000000 fal-1.0.0/tests/toolkit/file_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-05-10 14:49:23.000000 fal-1.0.0/tests/toolkit/image_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:30.124540 fal-1.0.0/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-10 14:49:23.000000 fal-1.0.0/tools/demo_script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:31.657440 fal-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-10 22:29:24.000000 fal-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-10 22:29:31.657440 fal-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-10 22:29:24.000000 fal-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:31.657440 fal-1.0.1/fal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-10 22:29:31.000000 fal-1.0.1/fal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-10 22:29:31.000000 fal-1.0.1/fal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 22:29:31.000000 fal-1.0.1/fal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-10 22:29:31.000000 fal-1.0.1/fal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-10 22:29:31.000000 fal-1.0.1/fal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-10 22:29:31.000000 fal-1.0.1/fal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:31.637440 fal-1.0.1/openapi-fal-rest/
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:31.641440 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:31.641440 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:31.641440 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/api/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/api/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/api/applications/app_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:31.641440 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/api/billing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/api/billing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/api/billing/get_user_details.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:31.641440 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/api/files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/api/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/api/files/check_dir_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/api/files/upload_local_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:31.641440 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/api/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/api/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/api/workflows/create_or_update_workflow_workflows_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/api/workflows/delete_workflow_workflows_user_id_workflow_name_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/api/workflows/execute_workflow_workflows_user_id_workflow_name_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/api/workflows/get_workflow_workflows_user_id_workflow_name_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/api/workflows/get_workflows_workflows_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:31.645440 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/app_metadata_response_app_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/body_upload_local_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/customer_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/execute_workflow_workflows_user_id_workflow_name_post_json_body_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/execute_workflow_workflows_user_id_workflow_name_post_response_200_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/hash_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/lock_reason.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/page_workflow_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/typed_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/workflow_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/workflow_contents_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/workflow_contents_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/workflow_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/workflow_detail_contents_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/workflow_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/workflow_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/workflow_node_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/workflow_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/workflow_schema_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/workflow_schema_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/openapi_fal_rest/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-10 22:29:24.000000 fal-1.0.1/openapi-fal-rest/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-10 22:29:24.000000 fal-1.0.1/openapi_rest.config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-10 22:29:24.000000 fal-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 22:29:31.661440 fal-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:31.633440 fal-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:31.649440 fal-1.0.1/src/fal/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-10 22:29:31.000000 fal-1.0.1/src/fal/_fal_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36287 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13826 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:31.649440 fal-1.0.1/src/fal/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/auth/auth0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/auth/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:31.649440 fal-1.0.1/src/fal/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/cli/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/cli/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/cli/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/cli/secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:31.649440 fal-1.0.1/src/fal/console/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/console/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/console/ux.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:31.653440 fal-1.0.1/src/fal/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/exceptions/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/exceptions/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/flags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:31.653440 fal-1.0.1/src/fal/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/logging/isolate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/logging/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/logging/trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/logging/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/rest_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19976 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:31.653440 fal-1.0.1/src/fal/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/toolkit/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:31.653440 fal-1.0.1/src/fal/toolkit/file/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/toolkit/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/toolkit/file/file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:31.653440 fal-1.0.1/src/fal/toolkit/file/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/toolkit/file/providers/fal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/toolkit/file/providers/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/toolkit/file/providers/r2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/toolkit/file/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:31.653440 fal-1.0.1/src/fal/toolkit/image/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/toolkit/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/toolkit/image/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/toolkit/optimize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:31.653440 fal-1.0.1/src/fal/toolkit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/toolkit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15487 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/toolkit/utils/download_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14682 2024-05-10 22:29:24.000000 fal-1.0.1/src/fal/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:31.657440 fal-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:24.000000 fal-1.0.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:31.657440 fal-1.0.1/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:24.000000 fal-1.0.1/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-10 22:29:24.000000 fal-1.0.1/tests/cli/test_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-10 22:29:24.000000 fal-1.0.1/tests/cli/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-10 22:29:24.000000 fal-1.0.1/tests/cli/test_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-10 22:29:24.000000 fal-1.0.1/tests/cli/test_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-10 22:29:24.000000 fal-1.0.1/tests/cli/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-10 22:29:24.000000 fal-1.0.1/tests/cli/test_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-10 22:29:24.000000 fal-1.0.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-05-10 22:29:24.000000 fal-1.0.1/tests/integration_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:31.657440 fal-1.0.1/tests/mainify_package/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-10 22:29:24.000000 fal-1.0.1/tests/mainify_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-10 22:29:24.000000 fal-1.0.1/tests/mainify_package/impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-10 22:29:24.000000 fal-1.0.1/tests/mainify_package/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-10 22:29:24.000000 fal-1.0.1/tests/mainify_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17322 2024-05-10 22:29:24.000000 fal-1.0.1/tests/test_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16201 2024-05-10 22:29:24.000000 fal-1.0.1/tests/test_stability.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:31.657440 fal-1.0.1/tests/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-10 22:29:24.000000 fal-1.0.1/tests/toolkit/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-05-10 22:29:24.000000 fal-1.0.1/tests/toolkit/image_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:29:31.657440 fal-1.0.1/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-10 22:29:24.000000 fal-1.0.1/tools/demo_script.py
```

### Comparing `fal-1.0.0/PKG-INFO` & `fal-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fal
-Version: 1.0.0
+Version: 1.0.1
 Summary: fal is an easy-to-use Serverless Python Framework
 Author: Features & Labels <hello@fal.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: isolate[build]<1.0,>=0.12.3
 Requires-Dist: isolate-proto==0.4.0
 Requires-Dist: grpcio<2,>=1.50.0
```

### Comparing `fal-1.0.0/README.md` & `fal-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/fal.egg-info/PKG-INFO` & `fal-1.0.1/fal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fal
-Version: 1.0.0
+Version: 1.0.1
 Summary: fal is an easy-to-use Serverless Python Framework
 Author: Features & Labels <hello@fal.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: isolate[build]<1.0,>=0.12.3
 Requires-Dist: isolate-proto==0.4.0
 Requires-Dist: grpcio<2,>=1.50.0
```

### Comparing `fal-1.0.0/fal.egg-info/SOURCES.txt` & `fal-1.0.1/fal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/fal.egg-info/requires.txt` & `fal-1.0.1/fal.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/README.md` & `fal-1.0.1/openapi-fal-rest/README.md`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/applications/app_metadata.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/api/applications/app_metadata.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/billing/get_user_details.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/api/billing/get_user_details.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/files/check_dir_hash.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/api/files/check_dir_hash.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/files/upload_local_file.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/api/files/upload_local_file.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/workflows/create_or_update_workflow_workflows_post.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/api/workflows/create_or_update_workflow_workflows_post.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/workflows/delete_workflow_workflows_user_id_workflow_name_delete.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/api/workflows/delete_workflow_workflows_user_id_workflow_name_delete.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/workflows/execute_workflow_workflows_user_id_workflow_name_post.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/api/workflows/execute_workflow_workflows_user_id_workflow_name_post.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/workflows/get_workflow_workflows_user_id_workflow_name_get.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/api/workflows/get_workflow_workflows_user_id_workflow_name_get.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/api/workflows/get_workflows_workflows_get.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/api/workflows/get_workflows_workflows_get.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/client.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/client.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/__init__.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/app_metadata_response_app_metadata.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/app_metadata_response_app_metadata.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/body_upload_local_file.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/body_upload_local_file.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/customer_details.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/customer_details.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/execute_workflow_workflows_user_id_workflow_name_post_json_body_type_0.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/execute_workflow_workflows_user_id_workflow_name_post_json_body_type_0.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/execute_workflow_workflows_user_id_workflow_name_post_response_200_type_0.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/execute_workflow_workflows_user_id_workflow_name_post_response_200_type_0.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/hash_check.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/hash_check.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/http_validation_error.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/lock_reason.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/lock_reason.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/page_workflow_item.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/page_workflow_item.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/typed_workflow.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/typed_workflow.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/validation_error.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/workflow_contents.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/workflow_contents.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/workflow_contents_nodes.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/workflow_contents_nodes.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/workflow_contents_output.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/workflow_contents_output.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/workflow_detail.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/workflow_detail.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/workflow_detail_contents_type_0.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/workflow_detail_contents_type_0.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/workflow_item.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/workflow_item.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/workflow_node.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/workflow_node.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/workflow_schema.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/workflow_schema.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/workflow_schema_input.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/workflow_schema_input.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/models/workflow_schema_output.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/models/workflow_schema_output.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/openapi_fal_rest/types.py` & `fal-1.0.1/openapi-fal-rest/openapi_fal_rest/types.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/openapi-fal-rest/pyproject.toml` & `fal-1.0.1/openapi-fal-rest/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/pyproject.toml` & `fal-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/__init__.py` & `fal-1.0.1/src/fal/__init__.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/_serialization.py` & `fal-1.0.1/src/fal/_serialization.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/api.py` & `fal-1.0.1/src/fal/api.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/app.py` & `fal-1.0.1/src/fal/app.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/apps.py` & `fal-1.0.1/src/fal/apps.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/auth/__init__.py` & `fal-1.0.1/src/fal/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/auth/auth0.py` & `fal-1.0.1/src/fal/auth/auth0.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/auth/local.py` & `fal-1.0.1/src/fal/auth/local.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/cli/apps.py` & `fal-1.0.1/src/fal/cli/apps.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
             and args.max_concurrency is None
             and args.min_concurrency is None
         ):
             args.console.log("No parameters for update were provided, ignoring.")
             return
 
         alias_info = connection.update_application(
-            application_name=args.app_alias,
+            application_name=args.app_name,
             keep_alive=args.keep_alive,
             max_multiplexing=args.max_multiplexing,
             max_concurrency=args.max_concurrency,
             min_concurrency=args.min_concurrency,
         )
         table = _apps_table([alias_info])
 
@@ -133,14 +133,18 @@
     parser = subparsers.add_parser(
         "scale",
         description=scale_help,
         help=scale_help,
         parents=parents,
     )
     parser.add_argument(
+        "app_name",
+        help="Application name.",
+    )
+    parser.add_argument(
         "--keep-alive",
         type=int,
         help="Keep alive (seconds).",
     )
     parser.add_argument(
         "--max-multiplexing",
         type=int,
```

### Comparing `fal-1.0.0/src/fal/cli/auth.py` & `fal-1.0.1/src/fal/cli/auth.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/cli/debug.py` & `fal-1.0.1/src/fal/cli/debug.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/cli/deploy.py` & `fal-1.0.1/src/fal/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/cli/keys.py` & `fal-1.0.1/src/fal/cli/keys.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/cli/main.py` & `fal-1.0.1/src/fal/cli/main.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/cli/parser.py` & `fal-1.0.1/src/fal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/cli/run.py` & `fal-1.0.1/src/fal/cli/run.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/cli/secrets.py` & `fal-1.0.1/src/fal/cli/secrets.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/flags.py` & `fal-1.0.1/src/fal/flags.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/logging/__init__.py` & `fal-1.0.1/src/fal/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/logging/isolate.py` & `fal-1.0.1/src/fal/logging/isolate.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/logging/trace.py` & `fal-1.0.1/src/fal/logging/trace.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/logging/user.py` & `fal-1.0.1/src/fal/logging/user.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/rest_client.py` & `fal-1.0.1/src/fal/rest_client.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/sdk.py` & `fal-1.0.1/src/fal/sdk.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/sync.py` & `fal-1.0.1/src/fal/sync.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/toolkit/__init__.py` & `fal-1.0.1/src/fal/toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/toolkit/file/file.py` & `fal-1.0.1/src/fal/toolkit/file/file.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/toolkit/file/providers/fal.py` & `fal-1.0.1/src/fal/toolkit/file/providers/fal.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/toolkit/file/providers/gcp.py` & `fal-1.0.1/src/fal/toolkit/file/providers/gcp.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/toolkit/file/providers/r2.py` & `fal-1.0.1/src/fal/toolkit/file/providers/r2.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/toolkit/file/types.py` & `fal-1.0.1/src/fal/toolkit/file/types.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/toolkit/image/image.py` & `fal-1.0.1/src/fal/toolkit/image/image.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/toolkit/optimize.py` & `fal-1.0.1/src/fal/toolkit/optimize.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/toolkit/utils/download_utils.py` & `fal-1.0.1/src/fal/toolkit/utils/download_utils.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/utils.py` & `fal-1.0.1/src/fal/utils.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/src/fal/workflows.py` & `fal-1.0.1/src/fal/workflows.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/tests/cli/test_apps.py` & `fal-1.0.1/tests/cli/test_apps.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,22 +27,23 @@
     assert args.app_rev == "myrev"
     assert args.auth == "public"
 
 
 def test_scale():
     args = parse_args(
         [
-            "apps", "scale",
+            "apps", "scale", "myapp",
             "--keep-alive", "123",
             "--max-multiplexing", "321",
             "--min-concurrency", "7",
             "--max-concurrency", "10",
         ]
     )
     assert args.func == _scale
+    assert args.app_name == "myapp"
     assert args.keep_alive == 123
     assert args.max_multiplexing == 321
     assert args.min_concurrency == 7
     assert args.max_concurrency == 10
 
 
 def test_runners():
```

### Comparing `fal-1.0.0/tests/cli/test_keys.py` & `fal-1.0.1/tests/cli/test_keys.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/tests/integration_test.py` & `fal-1.0.1/tests/integration_test.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/tests/test_apps.py` & `fal-1.0.1/tests/test_apps.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/tests/test_stability.py` & `fal-1.0.1/tests/test_stability.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/tests/toolkit/file_test.py` & `fal-1.0.1/tests/toolkit/file_test.py`

 * *Files identical despite different names*

### Comparing `fal-1.0.0/tests/toolkit/image_test.py` & `fal-1.0.1/tests/toolkit/image_test.py`

 * *Files identical despite different names*

