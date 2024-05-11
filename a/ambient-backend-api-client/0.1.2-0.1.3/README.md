# Comparing `tmp/ambient_backend_api_client-0.1.2.tar.gz` & `tmp/ambient_backend_api_client-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambient_backend_api_client-0.1.2.tar", last modified: Thu May  9 02:41:37 2024, max compression
+gzip compressed data, was "ambient_backend_api_client-0.1.3.tar", last modified: Sat May 11 02:12:16 2024, max compression
```

## Comparing `ambient_backend_api_client-0.1.2.tar` & `ambient_backend_api_client-0.1.3.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-09 02:41:37.019666 ambient_backend_api_client-0.1.2/
--rw-r--r--   0 jose       (501) staff       (20)      582 2024-05-09 02:41:37.019603 ambient_backend_api_client-0.1.2/PKG-INFO
--rw-r--r--   0 jose       (501) staff       (20)    11406 2024-05-09 02:41:13.000000 ambient_backend_api_client-0.1.2/README.md
-drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-09 02:41:36.988267 ambient_backend_api_client-0.1.2/ambient_backend_api_client/
--rw-r--r--   0 jose       (501) staff       (20)     5352 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/__init__.py
-drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-09 02:41:36.993959 ambient_backend_api_client-0.1.2/ambient_backend_api_client/api/
--rw-r--r--   0 jose       (501) staff       (20)      656 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/api/__init__.py
--rw-r--r--   0 jose       (501) staff       (20)    71865 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/api/clusters_api.py
--rw-r--r--   0 jose       (501) staff       (20)    10046 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/api/health_api.py
--rw-r--r--   0 jose       (501) staff       (20)    81888 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/api/nodes_api.py
--rw-r--r--   0 jose       (501) staff       (20)    53254 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/api/notifications_api.py
--rw-r--r--   0 jose       (501) staff       (20)    19071 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/api/ping_api.py
--rw-r--r--   0 jose       (501) staff       (20)    21780 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/api/requests_api.py
--rw-r--r--   0 jose       (501) staff       (20)    42278 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/api/services_api.py
--rw-r--r--   0 jose       (501) staff       (20)    31740 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/api/unimplemented_api.py
--rw-r--r--   0 jose       (501) staff       (20)    62218 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/api/users_api.py
--rw-r--r--   0 jose       (501) staff       (20)    26521 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/api_client.py
--rw-r--r--   0 jose       (501) staff       (20)      652 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/api_response.py
--rw-r--r--   0 jose       (501) staff       (20)    14468 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/configuration.py
--rw-r--r--   0 jose       (501) staff       (20)     5972 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/exceptions.py
-drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-09 02:41:37.006334 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/
--rw-r--r--   0 jose       (501) staff       (20)     4092 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/__init__.py
--rw-r--r--   0 jose       (501) staff       (20)      806 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/account_type.py
--rw-r--r--   0 jose       (501) staff       (20)      799 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/ambient_action_enum.py
--rw-r--r--   0 jose       (501) staff       (20)      867 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/ambient_event_type_enum.py
--rw-r--r--   0 jose       (501) staff       (20)      757 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/architecture_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     3064 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/auth0_device_code_response.py
--rw-r--r--   0 jose       (501) staff       (20)     5870 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/cluster.py
--rw-r--r--   0 jose       (501) staff       (20)     5710 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/cluster_create.py
--rw-r--r--   0 jose       (501) staff       (20)     3477 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/create_service_acct_request.py
--rw-r--r--   0 jose       (501) staff       (20)      765 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/creation_method.py
--rw-r--r--   0 jose       (501) staff       (20)     4031 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/event.py
--rw-r--r--   0 jose       (501) staff       (20)     1401 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/event_label.py
--rw-r--r--   0 jose       (501) staff       (20)     3748 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/event_template.py
--rw-r--r--   0 jose       (501) staff       (20)     2995 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/http_validation_error.py
--rw-r--r--   0 jose       (501) staff       (20)      989 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/interface_type_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     2786 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/list_results_response.py
--rw-r--r--   0 jose       (501) staff       (20)      936 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/models_cluster_status_enum.py
--rw-r--r--   0 jose       (501) staff       (20)      853 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/models_node_status_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     4605 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/network_interface.py
--rw-r--r--   0 jose       (501) staff       (20)     6732 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/node.py
--rw-r--r--   0 jose       (501) staff       (20)      769 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/node_architecture_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     6997 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/node_create.py
--rw-r--r--   0 jose       (501) staff       (20)      751 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/node_role_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     5059 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/notification.py
--rw-r--r--   0 jose       (501) staff       (20)     3245 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/notification_list.py
--rw-r--r--   0 jose       (501) staff       (20)     3037 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/notification_request.py
--rw-r--r--   0 jose       (501) staff       (20)      803 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/notification_severity_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     5309 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/organization_create.py
--rw-r--r--   0 jose       (501) staff       (20)      812 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/owner_type_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     3514 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/post_clusters_response.py
--rw-r--r--   0 jose       (501) staff       (20)     3510 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/post_service_response.py
--rw-r--r--   0 jose       (501) staff       (20)     5516 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/request.py
--rw-r--r--   0 jose       (501) staff       (20)      826 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/request_status_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     1125 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/resource_type_enum.py
--rw-r--r--   0 jose       (501) staff       (20)      731 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/role_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     5757 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/service.py
--rw-r--r--   0 jose       (501) staff       (20)     6005 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/service_create.py
--rw-r--r--   0 jose       (501) staff       (20)     3205 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/service_list.py
--rw-r--r--   0 jose       (501) staff       (20)      788 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/service_state.py
--rw-r--r--   0 jose       (501) staff       (20)      836 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/service_status_enum.py
--rw-r--r--   0 jose       (501) staff       (20)      838 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/status_enum_input.py
--rw-r--r--   0 jose       (501) staff       (20)      834 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/subscription_model_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     3113 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/token_response.py
--rw-r--r--   0 jose       (501) staff       (20)     6441 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/user.py
--rw-r--r--   0 jose       (501) staff       (20)     2573 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/user_preferences.py
--rw-r--r--   0 jose       (501) staff       (20)      815 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/user_role_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     3096 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/validation_error.py
--rw-r--r--   0 jose       (501) staff       (20)     4885 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/validation_error_loc_inner.py
--rw-r--r--   0 jose       (501) staff       (20)        0 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/py.typed
--rw-r--r--   0 jose       (501) staff       (20)     6854 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client/rest.py
-drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-09 02:41:37.019353 ambient_backend_api_client-0.1.2/ambient_backend_api_client.egg-info/
--rw-r--r--   0 jose       (501) staff       (20)      582 2024-05-09 02:41:36.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client.egg-info/PKG-INFO
--rw-r--r--   0 jose       (501) staff       (20)     5293 2024-05-09 02:41:36.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 jose       (501) staff       (20)        1 2024-05-09 02:41:36.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 jose       (501) staff       (20)      112 2024-05-09 02:41:36.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client.egg-info/requires.txt
--rw-r--r--   0 jose       (501) staff       (20)       27 2024-05-09 02:41:36.000000 ambient_backend_api_client-0.1.2/ambient_backend_api_client.egg-info/top_level.txt
--rw-r--r--   0 jose       (501) staff       (20)     2018 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/pyproject.toml
--rw-r--r--   0 jose       (501) staff       (20)       69 2024-05-09 02:41:37.019881 ambient_backend_api_client-0.1.2/setup.cfg
--rw-r--r--   0 jose       (501) staff       (20)     1406 2024-05-09 02:40:41.000000 ambient_backend_api_client-0.1.2/setup.py
-drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-09 02:41:37.019065 ambient_backend_api_client-0.1.2/test/
--rw-r--r--   0 jose       (501) staff       (20)      702 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_account_type.py
--rw-r--r--   0 jose       (501) staff       (20)      745 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_ambient_action_enum.py
--rw-r--r--   0 jose       (501) staff       (20)      767 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_ambient_event_type_enum.py
--rw-r--r--   0 jose       (501) staff       (20)      737 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_architecture_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     1908 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_auth0_device_code_response.py
--rw-r--r--   0 jose       (501) staff       (20)     2285 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_cluster.py
--rw-r--r--   0 jose       (501) staff       (20)     2288 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_cluster_create.py
--rw-r--r--   0 jose       (501) staff       (20)     1937 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_clusters_api.py
--rw-r--r--   0 jose       (501) staff       (20)     1681 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_create_service_acct_request.py
--rw-r--r--   0 jose       (501) staff       (20)      723 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_creation_method.py
--rw-r--r--   0 jose       (501) staff       (20)     1955 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_event.py
--rw-r--r--   0 jose       (501) staff       (20)      695 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_event_label.py
--rw-r--r--   0 jose       (501) staff       (20)     1739 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_event_template.py
--rw-r--r--   0 jose       (501) staff       (20)      764 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_health_api.py
--rw-r--r--   0 jose       (501) staff       (20)     1732 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_http_validation_error.py
--rw-r--r--   0 jose       (501) staff       (20)      745 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_interface_type_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     1689 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_list_results_response.py
--rw-r--r--   0 jose       (501) staff       (20)      788 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_models_cluster_status_enum.py
--rw-r--r--   0 jose       (501) staff       (20)      767 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_models_node_status_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     1708 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_network_interface.py
--rw-r--r--   0 jose       (501) staff       (20)     2793 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_node.py
--rw-r--r--   0 jose       (501) staff       (20)      766 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_node_architecture_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     2797 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_node_create.py
--rw-r--r--   0 jose       (501) staff       (20)      710 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_node_role_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     1982 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_nodes_api.py
--rw-r--r--   0 jose       (501) staff       (20)     2137 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_notification.py
--rw-r--r--   0 jose       (501) staff       (20)     3238 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_notification_list.py
--rw-r--r--   0 jose       (501) staff       (20)     1736 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_notification_request.py
--rw-r--r--   0 jose       (501) staff       (20)      794 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_notification_severity_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     1678 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_notifications_api.py
--rw-r--r--   0 jose       (501) staff       (20)     2020 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_organization_create.py
--rw-r--r--   0 jose       (501) staff       (20)      717 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_owner_type_enum.py
--rw-r--r--   0 jose       (501) staff       (20)      890 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_ping_api.py
--rw-r--r--   0 jose       (501) staff       (20)     3788 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_post_clusters_response.py
--rw-r--r--   0 jose       (501) staff       (20)     3726 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_post_service_response.py
--rw-r--r--   0 jose       (501) staff       (20)     2132 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_request.py
--rw-r--r--   0 jose       (501) staff       (20)      745 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_request_status_enum.py
--rw-r--r--   0 jose       (501) staff       (20)      997 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_requests_api.py
--rw-r--r--   0 jose       (501) staff       (20)      738 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_resource_type_enum.py
--rw-r--r--   0 jose       (501) staff       (20)      681 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_role_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     2226 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_service.py
--rw-r--r--   0 jose       (501) staff       (20)     2264 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_service_create.py
--rw-r--r--   0 jose       (501) staff       (20)     3830 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_service_list.py
--rw-r--r--   0 jose       (501) staff       (20)      709 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_service_state.py
--rw-r--r--   0 jose       (501) staff       (20)      745 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_service_status_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     1311 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_services_api.py
--rw-r--r--   0 jose       (501) staff       (20)      731 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_status_enum_input.py
--rw-r--r--   0 jose       (501) staff       (20)      773 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_subscription_model_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     1657 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_token_response.py
--rw-r--r--   0 jose       (501) staff       (20)     1226 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_unimplemented_api.py
--rw-r--r--   0 jose       (501) staff       (20)     2339 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_user.py
--rw-r--r--   0 jose       (501) staff       (20)     1410 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_user_preferences.py
--rw-r--r--   0 jose       (501) staff       (20)      710 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_user_role_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     1623 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_users_api.py
--rw-r--r--   0 jose       (501) staff       (20)     1626 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_validation_error.py
--rw-r--r--   0 jose       (501) staff       (20)     1475 2024-05-09 02:39:25.000000 ambient_backend_api_client-0.1.2/test/test_validation_error_loc_inner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:12:16.181112 ambient_backend_api_client-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-11 02:12:16.181112 ambient_backend_api_client-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11406 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:12:16.161112 ambient_backend_api_client-0.1.3/ambient_backend_api_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:12:16.165112 ambient_backend_api_client-0.1.3/ambient_backend_api_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71865 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/api/clusters_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10046 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/api/health_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81888 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/api/nodes_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53254 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/api/notifications_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19071 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/api/ping_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21780 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/api/requests_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42278 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/api/services_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31740 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/api/unimplemented_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62218 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/api/users_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26521 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14468 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:12:16.173112 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/account_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/ambient_action_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/ambient_event_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/architecture_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/auth0_device_code_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/cluster_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/create_service_acct_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/creation_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/event_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/event_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/interface_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/list_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/models_cluster_status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/models_node_status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/network_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/node_architecture_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6997 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/node_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/node_role_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/notification_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/notification_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/notification_severity_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/organization_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/owner_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/post_clusters_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/post_service_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/request_status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/resource_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/role_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5056 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/service_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/service_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/service_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/service_status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/status_enum_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/subscription_model_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/user_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/user_role_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/validation_error_loc_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:12:16.161112 ambient_backend_api_client-0.1.3/ambient_backend_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-11 02:12:16.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-11 02:12:16.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 02:12:16.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-11 02:12:16.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-11 02:12:16.000000 ambient_backend_api_client-0.1.3/ambient_backend_api_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-11 02:12:16.181112 ambient_backend_api_client-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:12:16.181112 ambient_backend_api_client-0.1.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_account_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_ambient_action_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_ambient_event_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_architecture_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_auth0_device_code_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_cluster_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_clusters_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_create_service_acct_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_creation_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_event_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_event_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_health_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_interface_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_list_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_models_cluster_status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_models_node_status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_network_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_node_architecture_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_node_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_node_role_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_nodes_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_notification_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_notification_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_notification_severity_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_notifications_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_organization_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_owner_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_ping_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_post_clusters_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_post_service_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_request_status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_requests_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_resource_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_role_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_service_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_service_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_service_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_service_status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_services_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_status_enum_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_subscription_model_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_unimplemented_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_user_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_user_role_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_users_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-11 02:12:06.000000 ambient_backend_api_client-0.1.3/test/test_validation_error_loc_inner.py
```

### Comparing `ambient_backend_api_client-0.1.2/README.md` & `ambient_backend_api_client-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/__init__.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/api/__init__.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/api/clusters_api.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/api/clusters_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/api/health_api.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/api/health_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/api/nodes_api.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/api/nodes_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/api/notifications_api.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/api/notifications_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/api/ping_api.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/api/ping_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/api/requests_api.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/api/requests_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/api/services_api.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/api/services_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/api/unimplemented_api.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/api/unimplemented_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/api/users_api.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/api/users_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/api_client.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/api_response.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/api_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/configuration.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/configuration.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/exceptions.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/__init__.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/account_type.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/account_type.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/ambient_action_enum.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/ambient_action_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/ambient_event_type_enum.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/ambient_event_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/architecture_enum.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/architecture_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/auth0_device_code_response.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/auth0_device_code_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/cluster.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/cluster.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 class Cluster(BaseModel):
     """
     Cluster
     """ # noqa: E501
     name: StrictStr
     resource_type: Optional[ResourceTypeEnum] = None
-    identifier: Optional[StrictStr] = '02439f7a-5a39-457d-b117-9a8d9effe62f'
+    identifier: Optional[StrictStr] = '0956813f-647c-49af-a983-cc590a5cf901'
     owner_id: Optional[StrictStr] = None
     owner_type: Optional[OwnerTypeEnum] = None
     description: Optional[StrictStr] = None
     requests: Optional[List[StrictStr]] = None
     notifications: Optional[List[StrictStr]] = None
     role: RoleEnum
     architecture: ArchitectureEnum
@@ -124,15 +124,15 @@
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "name": obj.get("name"),
             "resource_type": obj.get("resource_type"),
-            "identifier": obj.get("identifier") if obj.get("identifier") is not None else '02439f7a-5a39-457d-b117-9a8d9effe62f',
+            "identifier": obj.get("identifier") if obj.get("identifier") is not None else '0956813f-647c-49af-a983-cc590a5cf901',
             "owner_id": obj.get("owner_id"),
             "owner_type": obj.get("owner_type"),
             "description": obj.get("description"),
             "requests": obj.get("requests"),
             "notifications": obj.get("notifications"),
             "role": obj.get("role"),
             "architecture": obj.get("architecture"),
```

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/cluster_create.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/cluster_create.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 class ClusterCreate(BaseModel):
     """
     ClusterCreate
     """ # noqa: E501
     name: StrictStr
     resource_type: Optional[ResourceTypeEnum] = None
-    identifier: Optional[StrictStr] = '02439f7a-5a39-457d-b117-9a8d9effe62f'
+    identifier: Optional[StrictStr] = '0956813f-647c-49af-a983-cc590a5cf901'
     owner_id: Optional[StrictStr] = None
     owner_type: Optional[OwnerTypeEnum] = None
     description: Optional[StrictStr] = None
     requests: Optional[List[StrictStr]] = None
     notifications: Optional[List[StrictStr]] = None
     role: RoleEnum
     architecture: ArchitectureEnum
@@ -122,15 +122,15 @@
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "name": obj.get("name"),
             "resource_type": obj.get("resource_type"),
-            "identifier": obj.get("identifier") if obj.get("identifier") is not None else '02439f7a-5a39-457d-b117-9a8d9effe62f',
+            "identifier": obj.get("identifier") if obj.get("identifier") is not None else '0956813f-647c-49af-a983-cc590a5cf901',
             "owner_id": obj.get("owner_id"),
             "owner_type": obj.get("owner_type"),
             "description": obj.get("description"),
             "requests": obj.get("requests"),
             "notifications": obj.get("notifications"),
             "role": obj.get("role"),
             "architecture": obj.get("architecture"),
```

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/create_service_acct_request.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/create_service_acct_request.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/creation_method.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/creation_method.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/event.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/event.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/event_label.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/event_label.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/event_template.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/event_template.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/http_validation_error.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/interface_type_enum.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/interface_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/list_results_response.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/list_results_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from typing_extensions import Self
 
 class ListResultsResponse(BaseModel):
     """
     ListResultsResponse
     """ # noqa: E501
     count: StrictInt
-    timestamp: Optional[StrictStr] = 'Wed May  8 20:38:23 2024'
+    timestamp: Optional[StrictStr] = 'Fri May 10 19:20:26 2024'
     results: List[Any]
     __properties: ClassVar[List[str]] = ["count", "timestamp", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
@@ -79,13 +79,13 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "count": obj.get("count"),
-            "timestamp": obj.get("timestamp") if obj.get("timestamp") is not None else 'Wed May  8 20:38:23 2024',
+            "timestamp": obj.get("timestamp") if obj.get("timestamp") is not None else 'Fri May 10 19:20:26 2024',
             "results": obj.get("results")
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/models_cluster_status_enum.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/models_cluster_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/models_node_status_enum.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/models_node_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/network_interface.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/network_interface.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/node.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/node.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/node_architecture_enum.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/node_architecture_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/node_create.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/node_create.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/node_role_enum.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/node_role_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/notification.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/notification.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/notification_list.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/notification_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from typing_extensions import Self
 
 class NotificationList(BaseModel):
     """
     NotificationList
     """ # noqa: E501
     count: StrictInt
-    timestamp: Optional[StrictStr] = 'Wed May  8 20:38:23 2024'
+    timestamp: Optional[StrictStr] = 'Fri May 10 19:20:26 2024'
     results: List[Notification]
     __properties: ClassVar[List[str]] = ["count", "timestamp", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
@@ -87,13 +87,13 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "count": obj.get("count"),
-            "timestamp": obj.get("timestamp") if obj.get("timestamp") is not None else 'Wed May  8 20:38:23 2024',
+            "timestamp": obj.get("timestamp") if obj.get("timestamp") is not None else 'Fri May 10 19:20:26 2024',
             "results": [Notification.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/notification_request.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/notification_request.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/notification_severity_enum.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/notification_severity_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/organization_create.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/organization_create.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/owner_type_enum.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/owner_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/post_clusters_response.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/post_clusters_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from typing_extensions import Self
 
 class PostClustersResponse(BaseModel):
     """
     PostClustersResponse
     """ # noqa: E501
     request_id: StrictStr
-    requested_ts: Optional[StrictStr] = 'Wed May  8 20:38:23 2024'
+    requested_ts: Optional[StrictStr] = 'Fri May 10 19:20:26 2024'
     location_root: Optional[StrictStr] = 'http://localhost:8001/requests/'
     refresh_interval: Optional[StrictInt] = 10
     cluster: Cluster
     __properties: ClassVar[List[str]] = ["request_id", "requested_ts", "location_root", "refresh_interval", "cluster"]
 
     model_config = ConfigDict(
         populate_by_name=True,
@@ -85,15 +85,15 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "request_id": obj.get("request_id"),
-            "requested_ts": obj.get("requested_ts") if obj.get("requested_ts") is not None else 'Wed May  8 20:38:23 2024',
+            "requested_ts": obj.get("requested_ts") if obj.get("requested_ts") is not None else 'Fri May 10 19:20:26 2024',
             "location_root": obj.get("location_root") if obj.get("location_root") is not None else 'http://localhost:8001/requests/',
             "refresh_interval": obj.get("refresh_interval") if obj.get("refresh_interval") is not None else 10,
             "cluster": Cluster.from_dict(obj["cluster"]) if obj.get("cluster") is not None else None
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/post_service_response.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/post_service_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from typing_extensions import Self
 
 class PostServiceResponse(BaseModel):
     """
     PostServiceResponse
     """ # noqa: E501
     request_id: StrictStr
-    requested_ts: Optional[StrictStr] = 'Wed May  8 20:38:23 2024'
+    requested_ts: Optional[StrictStr] = 'Fri May 10 19:20:26 2024'
     location_root: Optional[StrictStr] = 'http://localhost:8001/requests/'
     refresh_interval: Optional[StrictInt] = 10
     service: Service
     __properties: ClassVar[List[str]] = ["request_id", "requested_ts", "location_root", "refresh_interval", "service"]
 
     model_config = ConfigDict(
         populate_by_name=True,
@@ -85,15 +85,15 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "request_id": obj.get("request_id"),
-            "requested_ts": obj.get("requested_ts") if obj.get("requested_ts") is not None else 'Wed May  8 20:38:23 2024',
+            "requested_ts": obj.get("requested_ts") if obj.get("requested_ts") is not None else 'Fri May 10 19:20:26 2024',
             "location_root": obj.get("location_root") if obj.get("location_root") is not None else 'http://localhost:8001/requests/',
             "refresh_interval": obj.get("refresh_interval") if obj.get("refresh_interval") is not None else 10,
             "service": Service.from_dict(obj["service"]) if obj.get("service") is not None else None
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/request.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     owner_id: StrictStr
     owner_type: OwnerTypeEnum
     description: Optional[StrictStr] = None
     requests: Optional[List[StrictStr]] = None
     notifications: Optional[List[StrictStr]] = None
     status: Optional[RequestStatusEnum] = None
     error: Optional[StrictStr] = None
-    requested_ts: Optional[Union[StrictFloat, StrictInt]] = 1.7152223033432431E9
+    requested_ts: Optional[Union[StrictFloat, StrictInt]] = 1.715390426038406E9
     started_ts: Optional[Union[StrictFloat, StrictInt]] = None
     failed_ts: Optional[Union[StrictFloat, StrictInt]] = None
     completed_ts: Optional[Union[StrictFloat, StrictInt]] = None
     notes: Optional[List[StrictStr]] = None
     data: Optional[Dict[str, Any]] = None
     __properties: ClassVar[List[str]] = ["name", "resource_type", "identifier", "owner_id", "owner_type", "description", "requests", "notifications", "status", "error", "requested_ts", "started_ts", "failed_ts", "completed_ts", "notes", "data"]
 
@@ -129,15 +129,15 @@
             "owner_id": obj.get("owner_id"),
             "owner_type": obj.get("owner_type"),
             "description": obj.get("description"),
             "requests": obj.get("requests"),
             "notifications": obj.get("notifications"),
             "status": obj.get("status"),
             "error": obj.get("error"),
-            "requested_ts": obj.get("requested_ts") if obj.get("requested_ts") is not None else 1.7152223033432431E9,
+            "requested_ts": obj.get("requested_ts") if obj.get("requested_ts") is not None else 1.715390426038406E9,
             "started_ts": obj.get("started_ts"),
             "failed_ts": obj.get("failed_ts"),
             "completed_ts": obj.get("completed_ts"),
             "notes": obj.get("notes"),
             "data": obj.get("data")
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/request_status_enum.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/request_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/resource_type_enum.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/resource_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/role_enum.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/role_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/service.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/user.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,45 +13,49 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictBool, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
+from ambient_backend_api_client.models.account_type import AccountType
+from ambient_backend_api_client.models.creation_method import CreationMethod
 from ambient_backend_api_client.models.owner_type_enum import OwnerTypeEnum
 from ambient_backend_api_client.models.resource_type_enum import ResourceTypeEnum
-from ambient_backend_api_client.models.service_state import ServiceState
-from ambient_backend_api_client.models.service_status_enum import ServiceStatusEnum
+from ambient_backend_api_client.models.user_preferences import UserPreferences
+from ambient_backend_api_client.models.user_role_enum import UserRoleEnum
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Service(BaseModel):
+class User(BaseModel):
     """
-    Service
+    User
     """ # noqa: E501
     name: StrictStr
     resource_type: Optional[ResourceTypeEnum] = None
-    identifier: Optional[StrictStr] = None
-    owner_id: Optional[StrictStr] = None
-    owner_type: Optional[OwnerTypeEnum] = None
+    identifier: StrictStr
+    owner_id: StrictStr
+    owner_type: OwnerTypeEnum
     description: Optional[StrictStr] = None
     requests: Optional[List[StrictStr]] = None
     notifications: Optional[List[StrictStr]] = None
-    image: StrictStr
-    replicas: StrictInt
-    cluster_groups: Optional[List[StrictStr]] = None
-    tags: Optional[List[StrictStr]] = None
-    clusters: Optional[List[StrictStr]] = None
-    ports: Optional[List[StrictStr]] = None
-    compose_location: Optional[StrictStr] = None
-    state: Optional[ServiceState] = None
-    status: ServiceStatusEnum
-    __properties: ClassVar[List[str]] = ["name", "resource_type", "identifier", "owner_id", "owner_type", "description", "requests", "notifications", "image", "replicas", "cluster_groups", "tags", "clusters", "ports", "compose_location", "state", "status"]
+    account_type: Optional[AccountType] = None
+    creation_method: Optional[CreationMethod] = None
+    email: StrictStr
+    first_name: StrictStr
+    last_name: StrictStr
+    role: Optional[UserRoleEnum] = None
+    preferences: Optional[UserPreferences] = None
+    auth_provider_uid: Optional[StrictStr] = None
+    phone_number: Optional[StrictStr] = None
+    username: Optional[StrictStr] = None
+    is_super_admin: Optional[StrictBool] = None
+    __properties: ClassVar[List[str]] = ["name", "resource_type", "identifier", "owner_id", "owner_type", "description", "requests", "notifications", "account_type", "creation_method", "email", "first_name", "last_name", "role", "preferences", "auth_provider_uid", "phone_number", "username", "is_super_admin"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -63,15 +67,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Service from a JSON string"""
+        """Create an instance of User from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -84,49 +88,52 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # set to None if identifier (nullable) is None
+        # override the default output from pydantic by calling `to_dict()` of preferences
+        if self.preferences:
+            _dict['preferences'] = self.preferences.to_dict()
+        # set to None if description (nullable) is None
         # and model_fields_set contains the field
-        if self.identifier is None and "identifier" in self.model_fields_set:
-            _dict['identifier'] = None
+        if self.description is None and "description" in self.model_fields_set:
+            _dict['description'] = None
 
-        # set to None if owner_id (nullable) is None
+        # set to None if preferences (nullable) is None
         # and model_fields_set contains the field
-        if self.owner_id is None and "owner_id" in self.model_fields_set:
-            _dict['owner_id'] = None
+        if self.preferences is None and "preferences" in self.model_fields_set:
+            _dict['preferences'] = None
 
-        # set to None if owner_type (nullable) is None
+        # set to None if auth_provider_uid (nullable) is None
         # and model_fields_set contains the field
-        if self.owner_type is None and "owner_type" in self.model_fields_set:
-            _dict['owner_type'] = None
+        if self.auth_provider_uid is None and "auth_provider_uid" in self.model_fields_set:
+            _dict['auth_provider_uid'] = None
 
-        # set to None if description (nullable) is None
+        # set to None if phone_number (nullable) is None
         # and model_fields_set contains the field
-        if self.description is None and "description" in self.model_fields_set:
-            _dict['description'] = None
+        if self.phone_number is None and "phone_number" in self.model_fields_set:
+            _dict['phone_number'] = None
 
-        # set to None if ports (nullable) is None
+        # set to None if username (nullable) is None
         # and model_fields_set contains the field
-        if self.ports is None and "ports" in self.model_fields_set:
-            _dict['ports'] = None
+        if self.username is None and "username" in self.model_fields_set:
+            _dict['username'] = None
 
-        # set to None if compose_location (nullable) is None
+        # set to None if is_super_admin (nullable) is None
         # and model_fields_set contains the field
-        if self.compose_location is None and "compose_location" in self.model_fields_set:
-            _dict['compose_location'] = None
+        if self.is_super_admin is None and "is_super_admin" in self.model_fields_set:
+            _dict['is_super_admin'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Service from a dict"""
+        """Create an instance of User from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
@@ -134,20 +141,22 @@
             "resource_type": obj.get("resource_type"),
             "identifier": obj.get("identifier"),
             "owner_id": obj.get("owner_id"),
             "owner_type": obj.get("owner_type"),
             "description": obj.get("description"),
             "requests": obj.get("requests"),
             "notifications": obj.get("notifications"),
-            "image": obj.get("image"),
-            "replicas": obj.get("replicas"),
-            "cluster_groups": obj.get("cluster_groups"),
-            "tags": obj.get("tags"),
-            "clusters": obj.get("clusters"),
-            "ports": obj.get("ports"),
-            "compose_location": obj.get("compose_location"),
-            "state": obj.get("state"),
-            "status": obj.get("status")
+            "account_type": obj.get("account_type"),
+            "creation_method": obj.get("creation_method"),
+            "email": obj.get("email"),
+            "first_name": obj.get("first_name"),
+            "last_name": obj.get("last_name"),
+            "role": obj.get("role"),
+            "preferences": UserPreferences.from_dict(obj["preferences"]) if obj.get("preferences") is not None else None,
+            "auth_provider_uid": obj.get("auth_provider_uid"),
+            "phone_number": obj.get("phone_number"),
+            "username": obj.get("username"),
+            "is_super_admin": obj.get("is_super_admin")
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/service_create.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/service_create.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from ambient_backend_api_client.models.owner_type_enum import OwnerTypeEnum
 from ambient_backend_api_client.models.resource_type_enum import ResourceTypeEnum
 from ambient_backend_api_client.models.service_state import ServiceState
 from ambient_backend_api_client.models.service_status_enum import ServiceStatusEnum
 from typing import Optional, Set
 from typing_extensions import Self
@@ -35,23 +35,19 @@
     identifier: Optional[StrictStr] = None
     owner_id: Optional[StrictStr] = None
     owner_type: Optional[OwnerTypeEnum] = None
     description: Optional[StrictStr] = None
     requests: Optional[List[StrictStr]] = None
     notifications: Optional[List[StrictStr]] = None
     image: StrictStr
-    replicas: StrictInt
-    cluster_groups: Optional[List[StrictStr]] = None
     tags: Optional[List[StrictStr]] = None
-    clusters: Optional[List[StrictStr]] = None
     ports: Optional[List[StrictStr]] = None
-    compose_location: Optional[StrictStr] = None
     state: Optional[ServiceState] = None
     status: Optional[ServiceStatusEnum] = None
-    __properties: ClassVar[List[str]] = ["name", "resource_type", "identifier", "owner_id", "owner_type", "description", "requests", "notifications", "image", "replicas", "cluster_groups", "tags", "clusters", "ports", "compose_location", "state", "status"]
+    __properties: ClassVar[List[str]] = ["name", "resource_type", "identifier", "owner_id", "owner_type", "description", "requests", "notifications", "image", "tags", "ports", "state", "status"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -109,19 +105,14 @@
             _dict['description'] = None
 
         # set to None if ports (nullable) is None
         # and model_fields_set contains the field
         if self.ports is None and "ports" in self.model_fields_set:
             _dict['ports'] = None
 
-        # set to None if compose_location (nullable) is None
-        # and model_fields_set contains the field
-        if self.compose_location is None and "compose_location" in self.model_fields_set:
-            _dict['compose_location'] = None
-
         # set to None if status (nullable) is None
         # and model_fields_set contains the field
         if self.status is None and "status" in self.model_fields_set:
             _dict['status'] = None
 
         return _dict
 
@@ -140,19 +131,15 @@
             "identifier": obj.get("identifier"),
             "owner_id": obj.get("owner_id"),
             "owner_type": obj.get("owner_type"),
             "description": obj.get("description"),
             "requests": obj.get("requests"),
             "notifications": obj.get("notifications"),
             "image": obj.get("image"),
-            "replicas": obj.get("replicas"),
-            "cluster_groups": obj.get("cluster_groups"),
             "tags": obj.get("tags"),
-            "clusters": obj.get("clusters"),
             "ports": obj.get("ports"),
-            "compose_location": obj.get("compose_location"),
             "state": obj.get("state"),
             "status": obj.get("status")
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/service_list.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/service_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from typing_extensions import Self
 
 class ServiceList(BaseModel):
     """
     ServiceList
     """ # noqa: E501
     count: StrictInt
-    timestamp: Optional[StrictStr] = 'Wed May  8 20:38:23 2024'
+    timestamp: Optional[StrictStr] = 'Fri May 10 19:20:26 2024'
     results: List[Service]
     __properties: ClassVar[List[str]] = ["count", "timestamp", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
@@ -87,13 +87,13 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "count": obj.get("count"),
-            "timestamp": obj.get("timestamp") if obj.get("timestamp") is not None else 'Wed May  8 20:38:23 2024',
+            "timestamp": obj.get("timestamp") if obj.get("timestamp") is not None else 'Fri May 10 19:20:26 2024',
             "results": [Service.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/service_state.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/service_state.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/service_status_enum.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/service_status_enum.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,19 +22,18 @@
     """
     ServiceStatusEnum
     """
 
     """
     allowed enum values
     """
-    ACTIVE = 'active'
-    INACTIVE = 'inactive'
-    DELETED = 'deleted'
+    SUCCESS = 'success'
     PENDING = 'pending'
-    ERROR = 'error'
+    FAILURE = 'failure'
+    DELETED = 'deleted'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Create an instance of ServiceStatusEnum from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/status_enum_input.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/status_enum_input.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/subscription_model_enum.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/subscription_model_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/token_response.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/token_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/user.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/service.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,49 +13,41 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictBool, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from ambient_backend_api_client.models.account_type import AccountType
-from ambient_backend_api_client.models.creation_method import CreationMethod
 from ambient_backend_api_client.models.owner_type_enum import OwnerTypeEnum
 from ambient_backend_api_client.models.resource_type_enum import ResourceTypeEnum
-from ambient_backend_api_client.models.user_preferences import UserPreferences
-from ambient_backend_api_client.models.user_role_enum import UserRoleEnum
+from ambient_backend_api_client.models.service_state import ServiceState
+from ambient_backend_api_client.models.service_status_enum import ServiceStatusEnum
 from typing import Optional, Set
 from typing_extensions import Self
 
-class User(BaseModel):
+class Service(BaseModel):
     """
-    User
+    Service
     """ # noqa: E501
     name: StrictStr
     resource_type: Optional[ResourceTypeEnum] = None
-    identifier: StrictStr
-    owner_id: StrictStr
-    owner_type: OwnerTypeEnum
+    identifier: Optional[StrictStr] = None
+    owner_id: Optional[StrictStr] = None
+    owner_type: Optional[OwnerTypeEnum] = None
     description: Optional[StrictStr] = None
     requests: Optional[List[StrictStr]] = None
     notifications: Optional[List[StrictStr]] = None
-    account_type: Optional[AccountType] = None
-    creation_method: Optional[CreationMethod] = None
-    email: StrictStr
-    first_name: StrictStr
-    last_name: StrictStr
-    role: Optional[UserRoleEnum] = None
-    preferences: Optional[UserPreferences] = None
-    auth_provider_uid: Optional[StrictStr] = None
-    phone_number: Optional[StrictStr] = None
-    username: Optional[StrictStr] = None
-    is_super_admin: Optional[StrictBool] = None
-    __properties: ClassVar[List[str]] = ["name", "resource_type", "identifier", "owner_id", "owner_type", "description", "requests", "notifications", "account_type", "creation_method", "email", "first_name", "last_name", "role", "preferences", "auth_provider_uid", "phone_number", "username", "is_super_admin"]
+    image: StrictStr
+    tags: Optional[List[StrictStr]] = None
+    ports: Optional[List[StrictStr]] = None
+    state: Optional[ServiceState] = None
+    status: ServiceStatusEnum
+    __properties: ClassVar[List[str]] = ["name", "resource_type", "identifier", "owner_id", "owner_type", "description", "requests", "notifications", "image", "tags", "ports", "state", "status"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -67,15 +59,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of User from a JSON string"""
+        """Create an instance of Service from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -88,52 +80,44 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of preferences
-        if self.preferences:
-            _dict['preferences'] = self.preferences.to_dict()
-        # set to None if description (nullable) is None
-        # and model_fields_set contains the field
-        if self.description is None and "description" in self.model_fields_set:
-            _dict['description'] = None
-
-        # set to None if preferences (nullable) is None
+        # set to None if identifier (nullable) is None
         # and model_fields_set contains the field
-        if self.preferences is None and "preferences" in self.model_fields_set:
-            _dict['preferences'] = None
+        if self.identifier is None and "identifier" in self.model_fields_set:
+            _dict['identifier'] = None
 
-        # set to None if auth_provider_uid (nullable) is None
+        # set to None if owner_id (nullable) is None
         # and model_fields_set contains the field
-        if self.auth_provider_uid is None and "auth_provider_uid" in self.model_fields_set:
-            _dict['auth_provider_uid'] = None
+        if self.owner_id is None and "owner_id" in self.model_fields_set:
+            _dict['owner_id'] = None
 
-        # set to None if phone_number (nullable) is None
+        # set to None if owner_type (nullable) is None
         # and model_fields_set contains the field
-        if self.phone_number is None and "phone_number" in self.model_fields_set:
-            _dict['phone_number'] = None
+        if self.owner_type is None and "owner_type" in self.model_fields_set:
+            _dict['owner_type'] = None
 
-        # set to None if username (nullable) is None
+        # set to None if description (nullable) is None
         # and model_fields_set contains the field
-        if self.username is None and "username" in self.model_fields_set:
-            _dict['username'] = None
+        if self.description is None and "description" in self.model_fields_set:
+            _dict['description'] = None
 
-        # set to None if is_super_admin (nullable) is None
+        # set to None if ports (nullable) is None
         # and model_fields_set contains the field
-        if self.is_super_admin is None and "is_super_admin" in self.model_fields_set:
-            _dict['is_super_admin'] = None
+        if self.ports is None and "ports" in self.model_fields_set:
+            _dict['ports'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of User from a dict"""
+        """Create an instance of Service from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
@@ -141,22 +125,16 @@
             "resource_type": obj.get("resource_type"),
             "identifier": obj.get("identifier"),
             "owner_id": obj.get("owner_id"),
             "owner_type": obj.get("owner_type"),
             "description": obj.get("description"),
             "requests": obj.get("requests"),
             "notifications": obj.get("notifications"),
-            "account_type": obj.get("account_type"),
-            "creation_method": obj.get("creation_method"),
-            "email": obj.get("email"),
-            "first_name": obj.get("first_name"),
-            "last_name": obj.get("last_name"),
-            "role": obj.get("role"),
-            "preferences": UserPreferences.from_dict(obj["preferences"]) if obj.get("preferences") is not None else None,
-            "auth_provider_uid": obj.get("auth_provider_uid"),
-            "phone_number": obj.get("phone_number"),
-            "username": obj.get("username"),
-            "is_super_admin": obj.get("is_super_admin")
+            "image": obj.get("image"),
+            "tags": obj.get("tags"),
+            "ports": obj.get("ports"),
+            "state": obj.get("state"),
+            "status": obj.get("status")
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/user_preferences.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/user_preferences.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/user_role_enum.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/user_role_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/validation_error.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/models/validation_error_loc_inner.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/models/validation_error_loc_inner.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client/rest.py` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client/rest.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/ambient_backend_api_client.egg-info/SOURCES.txt` & `ambient_backend_api_client-0.1.3/ambient_backend_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/pyproject.toml` & `ambient_backend_api_client-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/setup.py` & `ambient_backend_api_client-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "ambient_backend_api_client"
-VERSION = "0.1.2"
+VERSION = "0.1.3"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "aiohttp >= 3.0.0",
     "aiohttp-retry >= 2.8.3",
     "pydantic >= 2",
```

### Comparing `ambient_backend_api_client-0.1.2/test/test_account_type.py` & `ambient_backend_api_client-0.1.3/test/test_account_type.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_ambient_action_enum.py` & `ambient_backend_api_client-0.1.3/test/test_ambient_action_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_ambient_event_type_enum.py` & `ambient_backend_api_client-0.1.3/test/test_ambient_event_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_architecture_enum.py` & `ambient_backend_api_client-0.1.3/test/test_architecture_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_auth0_device_code_response.py` & `ambient_backend_api_client-0.1.3/test/test_auth0_device_code_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_cluster.py` & `ambient_backend_api_client-0.1.3/test/test_cluster.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_cluster_create.py` & `ambient_backend_api_client-0.1.3/test/test_cluster_create.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_clusters_api.py` & `ambient_backend_api_client-0.1.3/test/test_clusters_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_create_service_acct_request.py` & `ambient_backend_api_client-0.1.3/test/test_create_service_acct_request.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_creation_method.py` & `ambient_backend_api_client-0.1.3/test/test_creation_method.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_event.py` & `ambient_backend_api_client-0.1.3/test/test_event.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_event_label.py` & `ambient_backend_api_client-0.1.3/test/test_event_label.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_event_template.py` & `ambient_backend_api_client-0.1.3/test/test_event_template.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_health_api.py` & `ambient_backend_api_client-0.1.3/test/test_health_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_http_validation_error.py` & `ambient_backend_api_client-0.1.3/test/test_http_validation_error.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_interface_type_enum.py` & `ambient_backend_api_client-0.1.3/test/test_interface_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_list_results_response.py` & `ambient_backend_api_client-0.1.3/test/test_list_results_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_models_cluster_status_enum.py` & `ambient_backend_api_client-0.1.3/test/test_models_cluster_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_models_node_status_enum.py` & `ambient_backend_api_client-0.1.3/test/test_models_node_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_network_interface.py` & `ambient_backend_api_client-0.1.3/test/test_network_interface.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_node.py` & `ambient_backend_api_client-0.1.3/test/test_node.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_node_architecture_enum.py` & `ambient_backend_api_client-0.1.3/test/test_node_architecture_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_node_create.py` & `ambient_backend_api_client-0.1.3/test/test_node_create.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_node_role_enum.py` & `ambient_backend_api_client-0.1.3/test/test_node_role_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_nodes_api.py` & `ambient_backend_api_client-0.1.3/test/test_nodes_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_notification.py` & `ambient_backend_api_client-0.1.3/test/test_notification.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_notification_list.py` & `ambient_backend_api_client-0.1.3/test/test_notification_list.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_notification_request.py` & `ambient_backend_api_client-0.1.3/test/test_notification_request.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_notification_severity_enum.py` & `ambient_backend_api_client-0.1.3/test/test_notification_severity_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_notifications_api.py` & `ambient_backend_api_client-0.1.3/test/test_notifications_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_organization_create.py` & `ambient_backend_api_client-0.1.3/test/test_organization_create.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_owner_type_enum.py` & `ambient_backend_api_client-0.1.3/test/test_owner_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_ping_api.py` & `ambient_backend_api_client-0.1.3/test/test_ping_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_post_clusters_response.py` & `ambient_backend_api_client-0.1.3/test/test_post_clusters_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_post_service_response.py` & `ambient_backend_api_client-0.1.3/test/test_post_service_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_request.py` & `ambient_backend_api_client-0.1.3/test/test_request.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_request_status_enum.py` & `ambient_backend_api_client-0.1.3/test/test_request_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_requests_api.py` & `ambient_backend_api_client-0.1.3/test/test_requests_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_resource_type_enum.py` & `ambient_backend_api_client-0.1.3/test/test_resource_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_role_enum.py` & `ambient_backend_api_client-0.1.3/test/test_role_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_service.py` & `ambient_backend_api_client-0.1.3/test/test_service.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_service_create.py` & `ambient_backend_api_client-0.1.3/test/test_service_create.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_service_list.py` & `ambient_backend_api_client-0.1.3/test/test_service_list.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_service_state.py` & `ambient_backend_api_client-0.1.3/test/test_service_state.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_service_status_enum.py` & `ambient_backend_api_client-0.1.3/test/test_service_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_services_api.py` & `ambient_backend_api_client-0.1.3/test/test_services_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_status_enum_input.py` & `ambient_backend_api_client-0.1.3/test/test_status_enum_input.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_subscription_model_enum.py` & `ambient_backend_api_client-0.1.3/test/test_subscription_model_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_token_response.py` & `ambient_backend_api_client-0.1.3/test/test_token_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_unimplemented_api.py` & `ambient_backend_api_client-0.1.3/test/test_unimplemented_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_user.py` & `ambient_backend_api_client-0.1.3/test/test_user.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_user_preferences.py` & `ambient_backend_api_client-0.1.3/test/test_user_preferences.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_user_role_enum.py` & `ambient_backend_api_client-0.1.3/test/test_user_role_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_users_api.py` & `ambient_backend_api_client-0.1.3/test/test_users_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_validation_error.py` & `ambient_backend_api_client-0.1.3/test/test_validation_error.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.2/test/test_validation_error_loc_inner.py` & `ambient_backend_api_client-0.1.3/test/test_validation_error_loc_inner.py`

 * *Files identical despite different names*

