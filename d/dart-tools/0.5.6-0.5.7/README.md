# Comparing `tmp/dart_tools-0.5.6.tar.gz` & `tmp/dart_tools-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dart_tools-0.5.6.tar", last modified: Tue Apr 16 22:06:41 2024, max compression
+gzip compressed data, was "dart_tools-0.5.7.tar", last modified: Fri May 10 23:23:37 2024, max compression
```

## Comparing `dart_tools-0.5.6.tar` & `dart_tools-0.5.7.tar`

### file list

```diff
@@ -1,194 +1,191 @@
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2024-04-16 22:06:41.834949 dart_tools-0.5.6/
--rw-r--r--   0 zack       (501) staff       (20)     1061 2023-02-28 02:56:19.000000 dart_tools-0.5.6/LICENSE
--rw-r--r--   0 zack       (501) staff       (20)     7166 2024-04-16 22:06:41.834724 dart_tools-0.5.6/PKG-INFO
--rw-r--r--   0 zack       (501) staff       (20)     4220 2024-03-15 07:27:40.000000 dart_tools-0.5.6/README.md
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2024-04-16 22:06:41.788462 dart_tools-0.5.6/dart/
--rw-r--r--   0 zack       (501) staff       (20)      229 2023-12-01 08:32:06.000000 dart_tools-0.5.6/dart/__init__.py
--rwxr-xr-x   0 zack       (501) staff       (20)    28838 2024-04-16 22:05:57.000000 dart_tools-0.5.6/dart/dart.py
--rw-r--r--   0 zack       (501) staff       (20)       85 2023-12-01 08:32:06.000000 dart_tools-0.5.6/dart/exception.py
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2024-04-16 22:06:41.790170 dart_tools-0.5.6/dart/generated/
--rw-r--r--   0 zack       (501) staff       (20)      152 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/__init__.py
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2024-04-16 22:06:41.790501 dart_tools-0.5.6/dart/generated/api/
--rw-r--r--   0 zack       (501) staff       (20)       47 2024-04-16 22:06:24.000000 dart_tools-0.5.6/dart/generated/api/__init__.py
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2024-04-16 22:06:41.790959 dart_tools-0.5.6/dart/generated/api/transactions/
--rw-r--r--   0 zack       (501) staff       (20)        0 2024-04-16 22:06:24.000000 dart_tools-0.5.6/dart/generated/api/transactions/__init__.py
--rw-r--r--   0 zack       (501) staff       (20)     4663 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/api/transactions/transactions_create.py
--rw-r--r--   0 zack       (501) staff       (20)    12131 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/client.py
--rw-r--r--   0 zack       (501) staff       (20)      470 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/errors.py
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2024-04-16 22:06:41.832417 dart_tools-0.5.6/dart/generated/models/
--rw-r--r--   0 zack       (501) staff       (20)    11101 2024-04-16 22:06:24.000000 dart_tools-0.5.6/dart/generated/models/__init__.py
--rw-r--r--   0 zack       (501) staff       (20)     3474 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/attachment.py
--rw-r--r--   0 zack       (501) staff       (20)     3945 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/attachment_create.py
--rw-r--r--   0 zack       (501) staff       (20)     4270 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/attachment_update.py
--rw-r--r--   0 zack       (501) staff       (20)      704 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/batch.py
--rw-r--r--   0 zack       (501) staff       (20)     3879 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/brainstorm.py
--rw-r--r--   0 zack       (501) staff       (20)     3889 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/brainstorm_create.py
--rw-r--r--   0 zack       (501) staff       (20)      190 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/brainstorm_state.py
--rw-r--r--   0 zack       (501) staff       (20)     4833 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/brainstorm_update.py
--rw-r--r--   0 zack       (501) staff       (20)      742 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/color_name.py
--rw-r--r--   0 zack       (501) staff       (20)     4984 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/comment.py
--rw-r--r--   0 zack       (501) staff       (20)     3538 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/comment_create.py
--rw-r--r--   0 zack       (501) staff       (20)     2103 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/comment_reaction.py
--rw-r--r--   0 zack       (501) staff       (20)     2052 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/comment_reaction_create.py
--rw-r--r--   0 zack       (501) staff       (20)     2352 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/comment_reaction_update.py
--rw-r--r--   0 zack       (501) staff       (20)     3712 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/comment_update.py
--rw-r--r--   0 zack       (501) staff       (20)     7835 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/dartboard.py
--rw-r--r--   0 zack       (501) staff       (20)     8711 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/dartboard_create.py
--rw-r--r--   0 zack       (501) staff       (20)      244 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/dartboard_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     8880 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/dartboard_update.py
--rw-r--r--   0 zack       (501) staff       (20)      249 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/dartboards_list_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     1724 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/discord_integration.py
--rw-r--r--   0 zack       (501) staff       (20)     6853 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/doc.py
--rw-r--r--   0 zack       (501) staff       (20)     9649 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/doc_create.py
--rw-r--r--   0 zack       (501) staff       (20)      306 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/doc_source_type.py
--rw-r--r--   0 zack       (501) staff       (20)     9649 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/doc_update.py
--rw-r--r--   0 zack       (501) staff       (20)      421 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/entity_name.py
--rw-r--r--   0 zack       (501) staff       (20)    10339 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/event.py
--rw-r--r--   0 zack       (501) staff       (20)      549 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/event_actor.py
--rw-r--r--   0 zack       (501) staff       (20)     5770 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/event_create.py
--rw-r--r--   0 zack       (501) staff       (20)     3192 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/event_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     1775 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/event_subscription.py
--rw-r--r--   0 zack       (501) staff       (20)     6402 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/event_subscription_update.py
--rw-r--r--   0 zack       (501) staff       (20)      521 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/filter_applicability.py
--rw-r--r--   0 zack       (501) staff       (20)     3149 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/filter_assignee.py
--rw-r--r--   0 zack       (501) staff       (20)      150 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/filter_connector.py
--rw-r--r--   0 zack       (501) staff       (20)     3511 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/filter_group.py
--rw-r--r--   0 zack       (501) staff       (20)     1915 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/filter_search.py
--rw-r--r--   0 zack       (501) staff       (20)     3124 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/filter_set.py
--rw-r--r--   0 zack       (501) staff       (20)     5265 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/folder.py
--rw-r--r--   0 zack       (501) staff       (20)     6484 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/folder_create.py
--rw-r--r--   0 zack       (501) staff       (20)      183 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/folder_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     6653 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/folder_update.py
--rw-r--r--   0 zack       (501) staff       (20)      188 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/folders_list_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     4426 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/form.py
--rw-r--r--   0 zack       (501) staff       (20)     5169 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/form_create.py
--rw-r--r--   0 zack       (501) staff       (20)     3283 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/form_field.py
--rw-r--r--   0 zack       (501) staff       (20)     3306 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/form_field_create.py
--rw-r--r--   0 zack       (501) staff       (20)     3564 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/form_field_update.py
--rw-r--r--   0 zack       (501) staff       (20)     5251 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/form_update.py
--rw-r--r--   0 zack       (501) staff       (20)     4228 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/github_integration.py
--rw-r--r--   0 zack       (501) staff       (20)      245 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/github_integration_tenant_extension_status.py
--rw-r--r--   0 zack       (501) staff       (20)     2114 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/google_data.py
--rw-r--r--   0 zack       (501) staff       (20)      169 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/icon_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     4937 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/layout.py
--rw-r--r--   0 zack       (501) staff       (20)     1768 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/layout_config.py
--rw-r--r--   0 zack       (501) staff       (20)     4247 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/layout_create.py
--rw-r--r--   0 zack       (501) staff       (20)      203 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/layout_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     1751 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/layout_kind_config_map.py
--rw-r--r--   0 zack       (501) staff       (20)     4247 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/layout_update.py
--rw-r--r--   0 zack       (501) staff       (20)    24662 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/models_response.py
--rw-r--r--   0 zack       (501) staff       (20)     2825 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/notification.py
--rw-r--r--   0 zack       (501) staff       (20)     2619 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/notification_update.py
--rw-r--r--   0 zack       (501) staff       (20)     2310 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/notion_integration.py
--rw-r--r--   0 zack       (501) staff       (20)      217 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/notion_integration_tenant_extension_status.py
--rw-r--r--   0 zack       (501) staff       (20)    32625 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/operation.py
--rw-r--r--   0 zack       (501) staff       (20)      270 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/operation_kind.py
--rw-r--r--   0 zack       (501) staff       (20)      861 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/operation_model_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     3367 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/option.py
--rw-r--r--   0 zack       (501) staff       (20)     3330 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/option_create.py
--rw-r--r--   0 zack       (501) staff       (20)     3502 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/option_update.py
--rw-r--r--   0 zack       (501) staff       (20)     3104 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_attachment_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3068 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_comment_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3169 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_comment_reaction_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3092 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_dartboard_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3020 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_doc_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3056 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_folder_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3097 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_form_field_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3032 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_form_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3056 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_layout_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3056 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_option_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3082 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_property_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3181 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_relationship_kind_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3128 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_relationship_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3044 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_space_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3056 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_status_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3222 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_task_doc_relationship_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3085 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_task_link_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3032 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_task_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3056 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_tenant_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3222 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_user_dartboard_layout_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3032 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_user_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3032 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_view_list.py
--rw-r--r--   0 zack       (501) staff       (20)      195 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/priority.py
--rw-r--r--   0 zack       (501) staff       (20)      913 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/properties_list_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     3915 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/property_.py
--rw-r--r--   0 zack       (501) staff       (20)     3852 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/property_create.py
--rw-r--r--   0 zack       (501) staff       (20)      907 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/property_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     4247 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/property_update.py
--rw-r--r--   0 zack       (501) staff       (20)      177 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/recommendation_status.py
--rw-r--r--   0 zack       (501) staff       (20)     1839 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/relationship.py
--rw-r--r--   0 zack       (501) staff       (20)     2392 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/relationship_create.py
--rw-r--r--   0 zack       (501) staff       (20)     3014 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/relationship_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     3013 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/relationship_kind_create.py
--rw-r--r--   0 zack       (501) staff       (20)      257 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/relationship_kind_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     3187 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/relationship_kind_update.py
--rw-r--r--   0 zack       (501) staff       (20)      167 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/report_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     2093 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/request_body.py
--rw-r--r--   0 zack       (501) staff       (20)     1989 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/response_body.py
--rw-r--r--   0 zack       (501) staff       (20)     2300 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/slack_integration.py
--rw-r--r--   0 zack       (501) staff       (20)      216 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/slack_integration_tenant_extension_status.py
--rw-r--r--   0 zack       (501) staff       (20)     1611 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/sort.py
--rw-r--r--   0 zack       (501) staff       (20)     7814 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/space.py
--rw-r--r--   0 zack       (501) staff       (20)     9821 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/space_create.py
--rw-r--r--   0 zack       (501) staff       (20)      188 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/space_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     9903 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/space_update.py
--rw-r--r--   0 zack       (501) staff       (20)      151 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/sprint_mode.py
--rw-r--r--   0 zack       (501) staff       (20)     4280 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/status.py
--rw-r--r--   0 zack       (501) staff       (20)     4497 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/status_create.py
--rw-r--r--   0 zack       (501) staff       (20)      243 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/status_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     4980 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/status_update.py
--rw-r--r--   0 zack       (501) staff       (20)      249 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/statuses_list_kind.py
--rw-r--r--   0 zack       (501) staff       (20)      167 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/subscription.py
--rw-r--r--   0 zack       (501) staff       (20)      172 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/subtask_display_mode.py
--rw-r--r--   0 zack       (501) staff       (20)      403 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/summary_statistic_kind.py
--rw-r--r--   0 zack       (501) staff       (20)    11576 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/task.py
--rw-r--r--   0 zack       (501) staff       (20)    14468 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/task_create.py
--rw-r--r--   0 zack       (501) staff       (20)     2298 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/task_doc_relationship.py
--rw-r--r--   0 zack       (501) staff       (20)     1863 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/task_doc_relationship_create.py
--rw-r--r--   0 zack       (501) staff       (20)     3093 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/task_link.py
--rw-r--r--   0 zack       (501) staff       (20)     3668 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/task_link_create.py
--rw-r--r--   0 zack       (501) staff       (20)      661 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/task_link_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     3916 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/task_link_update.py
--rw-r--r--   0 zack       (501) staff       (20)     4890 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/task_notion_document.py
--rw-r--r--   0 zack       (501) staff       (20)     1337 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/task_notion_document_block_children_map.py
--rw-r--r--   0 zack       (501) staff       (20)     1294 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/task_notion_document_block_map.py
--rw-r--r--   0 zack       (501) staff       (20)     1289 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/task_notion_document_page_map.py
--rw-r--r--   0 zack       (501) staff       (20)     1225 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/task_properties.py
--rw-r--r--   0 zack       (501) staff       (20)      811 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/task_source_type.py
--rw-r--r--   0 zack       (501) staff       (20)    14468 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/task_update.py
--rw-r--r--   0 zack       (501) staff       (20)     8963 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/tenant.py
--rw-r--r--   0 zack       (501) staff       (20)     4446 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/tenant_update.py
--rw-r--r--   0 zack       (501) staff       (20)      186 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/theme.py
--rw-r--r--   0 zack       (501) staff       (20)     5226 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/transaction.py
--rw-r--r--   0 zack       (501) staff       (20)     2426 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/transaction_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     2470 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/transaction_response.py
--rw-r--r--   0 zack       (501) staff       (20)     5894 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/user.py
--rw-r--r--   0 zack       (501) staff       (20)     1718 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/user_dartboard_layout.py
--rw-r--r--   0 zack       (501) staff       (20)     1991 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/user_dartboard_layout_create.py
--rw-r--r--   0 zack       (501) staff       (20)      767 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/user_data_entity_retrieve_entity_kind.py
--rw-r--r--   0 zack       (501) staff       (20)      175 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/user_role.py
--rw-r--r--   0 zack       (501) staff       (20)      313 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/user_status.py
--rw-r--r--   0 zack       (501) staff       (20)     6910 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/user_update.py
--rw-r--r--   0 zack       (501) staff       (20)     1804 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/validation_error_response.py
--rw-r--r--   0 zack       (501) staff       (20)     1301 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/validation_error_response_items.py
--rw-r--r--   0 zack       (501) staff       (20)     6445 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/view.py
--rw-r--r--   0 zack       (501) staff       (20)     7752 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/view_create.py
--rw-r--r--   0 zack       (501) staff       (20)      203 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/view_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     7922 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/view_update.py
--rw-r--r--   0 zack       (501) staff       (20)     3316 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/yc_integration.py
--rw-r--r--   0 zack       (501) staff       (20)     1782 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/zapier_integration.py
--rw-r--r--   0 zack       (501) staff       (20)       25 2024-04-16 22:06:24.000000 dart_tools-0.5.6/dart/generated/py.typed
--rw-r--r--   0 zack       (501) staff       (20)      968 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/types.py
--rw-r--r--   0 zack       (501) staff       (20)     1905 2023-12-06 01:16:03.000000 dart_tools-0.5.6/dart/order_manager.py
--rw-r--r--   0 zack       (501) staff       (20)      569 2023-12-01 08:32:06.000000 dart_tools-0.5.6/dart/webhook.py
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2024-04-16 22:06:41.834422 dart_tools-0.5.6/dart_tools.egg-info/
--rw-r--r--   0 zack       (501) staff       (20)     7166 2024-04-16 22:06:41.000000 dart_tools-0.5.6/dart_tools.egg-info/PKG-INFO
--rw-r--r--   0 zack       (501) staff       (20)     7417 2024-04-16 22:06:41.000000 dart_tools-0.5.6/dart_tools.egg-info/SOURCES.txt
--rw-r--r--   0 zack       (501) staff       (20)        1 2024-04-16 22:06:41.000000 dart_tools-0.5.6/dart_tools.egg-info/dependency_links.txt
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2024-04-16 22:06:41.833928 dart_tools-0.5.6/dart_tools.egg-info/dist/
--rw-r--r--   0 zack       (501) staff       (20)     8788 2023-06-03 08:11:34.000000 dart_tools-0.5.6/dart_tools.egg-info/dist/dart-tools-0.3.3.tar.gz
--rw-r--r--   0 zack       (501) staff       (20)       34 2024-04-16 22:06:41.000000 dart_tools-0.5.6/dart_tools.egg-info/entry_points.txt
--rw-r--r--   0 zack       (501) staff       (20)       38 2024-04-16 22:06:41.000000 dart_tools-0.5.6/dart_tools.egg-info/requires.txt
--rw-r--r--   0 zack       (501) staff       (20)        5 2024-04-16 22:06:41.000000 dart_tools-0.5.6/dart_tools.egg-info/top_level.txt
--rw-r--r--   0 zack       (501) staff       (20)     1891 2024-04-16 22:06:10.000000 dart_tools-0.5.6/pyproject.toml
--rw-r--r--   0 zack       (501) staff       (20)       38 2024-04-16 22:06:41.834998 dart_tools-0.5.6/setup.cfg
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2024-05-10 23:23:37.067117 dart_tools-0.5.7/
+-rw-r--r--   0 zack       (501) staff       (20)     1061 2023-02-28 02:56:19.000000 dart_tools-0.5.7/LICENSE
+-rw-r--r--   0 zack       (501) staff       (20)     7166 2024-05-10 23:23:37.066887 dart_tools-0.5.7/PKG-INFO
+-rw-r--r--   0 zack       (501) staff       (20)     4220 2024-03-15 07:27:40.000000 dart_tools-0.5.7/README.md
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2024-05-10 23:23:37.039892 dart_tools-0.5.7/dart/
+-rw-r--r--   0 zack       (501) staff       (20)      229 2023-12-01 08:32:06.000000 dart_tools-0.5.7/dart/__init__.py
+-rwxr-xr-x   0 zack       (501) staff       (20)    28838 2024-04-16 22:05:57.000000 dart_tools-0.5.7/dart/dart.py
+-rw-r--r--   0 zack       (501) staff       (20)       85 2023-12-01 08:32:06.000000 dart_tools-0.5.7/dart/exception.py
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2024-05-10 23:23:37.040846 dart_tools-0.5.7/dart/generated/
+-rw-r--r--   0 zack       (501) staff       (20)      152 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/__init__.py
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2024-05-10 23:23:37.041027 dart_tools-0.5.7/dart/generated/api/
+-rw-r--r--   0 zack       (501) staff       (20)       47 2024-05-10 23:23:28.000000 dart_tools-0.5.7/dart/generated/api/__init__.py
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2024-05-10 23:23:37.041255 dart_tools-0.5.7/dart/generated/api/transactions/
+-rw-r--r--   0 zack       (501) staff       (20)        0 2024-05-10 23:23:28.000000 dart_tools-0.5.7/dart/generated/api/transactions/__init__.py
+-rw-r--r--   0 zack       (501) staff       (20)     4663 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/api/transactions/transactions_create.py
+-rw-r--r--   0 zack       (501) staff       (20)    12131 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/client.py
+-rw-r--r--   0 zack       (501) staff       (20)      470 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/errors.py
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2024-05-10 23:23:37.064855 dart_tools-0.5.7/dart/generated/models/
+-rw-r--r--   0 zack       (501) staff       (20)    10916 2024-05-10 23:23:28.000000 dart_tools-0.5.7/dart/generated/models/__init__.py
+-rw-r--r--   0 zack       (501) staff       (20)     3474 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/attachment.py
+-rw-r--r--   0 zack       (501) staff       (20)     3945 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/attachment_create.py
+-rw-r--r--   0 zack       (501) staff       (20)     4270 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/attachment_update.py
+-rw-r--r--   0 zack       (501) staff       (20)     3879 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/brainstorm.py
+-rw-r--r--   0 zack       (501) staff       (20)     3889 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/brainstorm_create.py
+-rw-r--r--   0 zack       (501) staff       (20)      190 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/brainstorm_state.py
+-rw-r--r--   0 zack       (501) staff       (20)     4833 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/brainstorm_update.py
+-rw-r--r--   0 zack       (501) staff       (20)      742 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/color_name.py
+-rw-r--r--   0 zack       (501) staff       (20)     4984 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/comment.py
+-rw-r--r--   0 zack       (501) staff       (20)     3538 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/comment_create.py
+-rw-r--r--   0 zack       (501) staff       (20)     2103 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/comment_reaction.py
+-rw-r--r--   0 zack       (501) staff       (20)     2052 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/comment_reaction_create.py
+-rw-r--r--   0 zack       (501) staff       (20)     2352 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/comment_reaction_update.py
+-rw-r--r--   0 zack       (501) staff       (20)     3712 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/comment_update.py
+-rw-r--r--   0 zack       (501) staff       (20)     7811 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/dartboard.py
+-rw-r--r--   0 zack       (501) staff       (20)     8687 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/dartboard_create.py
+-rw-r--r--   0 zack       (501) staff       (20)      230 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/dartboard_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     8856 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/dartboard_update.py
+-rw-r--r--   0 zack       (501) staff       (20)      235 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/dartboards_list_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     1724 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/discord_integration.py
+-rw-r--r--   0 zack       (501) staff       (20)     6853 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/doc.py
+-rw-r--r--   0 zack       (501) staff       (20)     9649 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/doc_create.py
+-rw-r--r--   0 zack       (501) staff       (20)      306 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/doc_source_type.py
+-rw-r--r--   0 zack       (501) staff       (20)     9649 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/doc_update.py
+-rw-r--r--   0 zack       (501) staff       (20)      421 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/entity_name.py
+-rw-r--r--   0 zack       (501) staff       (20)    10573 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/event.py
+-rw-r--r--   0 zack       (501) staff       (20)      549 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/event_actor.py
+-rw-r--r--   0 zack       (501) staff       (20)     6004 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/event_create.py
+-rw-r--r--   0 zack       (501) staff       (20)     3371 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/event_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     1775 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/event_subscription.py
+-rw-r--r--   0 zack       (501) staff       (20)     6636 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/event_subscription_update.py
+-rw-r--r--   0 zack       (501) staff       (20)      521 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/filter_applicability.py
+-rw-r--r--   0 zack       (501) staff       (20)     3149 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/filter_assignee.py
+-rw-r--r--   0 zack       (501) staff       (20)      150 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/filter_connector.py
+-rw-r--r--   0 zack       (501) staff       (20)     3511 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/filter_group.py
+-rw-r--r--   0 zack       (501) staff       (20)     1915 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/filter_search.py
+-rw-r--r--   0 zack       (501) staff       (20)     3124 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/filter_set.py
+-rw-r--r--   0 zack       (501) staff       (20)     4613 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/folder.py
+-rw-r--r--   0 zack       (501) staff       (20)     5501 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/folder_create.py
+-rw-r--r--   0 zack       (501) staff       (20)      183 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/folder_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     5670 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/folder_update.py
+-rw-r--r--   0 zack       (501) staff       (20)      188 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/folders_list_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     4426 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/form.py
+-rw-r--r--   0 zack       (501) staff       (20)     5169 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/form_create.py
+-rw-r--r--   0 zack       (501) staff       (20)     3283 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/form_field.py
+-rw-r--r--   0 zack       (501) staff       (20)     3306 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/form_field_create.py
+-rw-r--r--   0 zack       (501) staff       (20)     3564 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/form_field_update.py
+-rw-r--r--   0 zack       (501) staff       (20)     5251 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/form_update.py
+-rw-r--r--   0 zack       (501) staff       (20)     4228 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/github_integration.py
+-rw-r--r--   0 zack       (501) staff       (20)      245 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/github_integration_tenant_extension_status.py
+-rw-r--r--   0 zack       (501) staff       (20)     2114 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/google_data.py
+-rw-r--r--   0 zack       (501) staff       (20)      169 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/icon_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     4937 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/layout.py
+-rw-r--r--   0 zack       (501) staff       (20)     1768 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/layout_config.py
+-rw-r--r--   0 zack       (501) staff       (20)     4247 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/layout_create.py
+-rw-r--r--   0 zack       (501) staff       (20)      203 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/layout_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     1751 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/layout_kind_config_map.py
+-rw-r--r--   0 zack       (501) staff       (20)     4247 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/layout_update.py
+-rw-r--r--   0 zack       (501) staff       (20)    24662 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/models_response.py
+-rw-r--r--   0 zack       (501) staff       (20)     2825 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/notification.py
+-rw-r--r--   0 zack       (501) staff       (20)     2619 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/notification_update.py
+-rw-r--r--   0 zack       (501) staff       (20)     2310 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/notion_integration.py
+-rw-r--r--   0 zack       (501) staff       (20)      217 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/notion_integration_tenant_extension_status.py
+-rw-r--r--   0 zack       (501) staff       (20)    32625 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/operation.py
+-rw-r--r--   0 zack       (501) staff       (20)      270 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/operation_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)      861 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/operation_model_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     3367 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/option.py
+-rw-r--r--   0 zack       (501) staff       (20)     3330 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/option_create.py
+-rw-r--r--   0 zack       (501) staff       (20)     3502 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/option_update.py
+-rw-r--r--   0 zack       (501) staff       (20)     2844 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/paginated_attachment_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     2808 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/paginated_comment_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     2909 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/paginated_comment_reaction_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     2832 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/paginated_dartboard_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     2760 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/paginated_doc_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     2796 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/paginated_folder_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     2837 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/paginated_form_field_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     2772 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/paginated_form_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     2796 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/paginated_layout_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     2796 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/paginated_option_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     2822 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/paginated_property_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     2921 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/paginated_relationship_kind_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     2868 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/paginated_relationship_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     2784 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/paginated_space_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     2796 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/paginated_status_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     2962 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/paginated_task_doc_relationship_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     2825 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/paginated_task_link_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     2772 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/paginated_task_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     2796 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/paginated_tenant_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     2962 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/paginated_user_dartboard_layout_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     2772 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/paginated_user_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     2772 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/paginated_view_list.py
+-rw-r--r--   0 zack       (501) staff       (20)      195 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/priority.py
+-rw-r--r--   0 zack       (501) staff       (20)      913 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/properties_list_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     3915 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/property_.py
+-rw-r--r--   0 zack       (501) staff       (20)     3852 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/property_create.py
+-rw-r--r--   0 zack       (501) staff       (20)      907 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/property_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     4247 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/property_update.py
+-rw-r--r--   0 zack       (501) staff       (20)     1839 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/relationship.py
+-rw-r--r--   0 zack       (501) staff       (20)     2392 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/relationship_create.py
+-rw-r--r--   0 zack       (501) staff       (20)     3014 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/relationship_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     3013 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/relationship_kind_create.py
+-rw-r--r--   0 zack       (501) staff       (20)      257 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/relationship_kind_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     3187 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/relationship_kind_update.py
+-rw-r--r--   0 zack       (501) staff       (20)      167 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/report_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     2093 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/request_body.py
+-rw-r--r--   0 zack       (501) staff       (20)     1989 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/response_body.py
+-rw-r--r--   0 zack       (501) staff       (20)     2300 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/slack_integration.py
+-rw-r--r--   0 zack       (501) staff       (20)      216 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/slack_integration_tenant_extension_status.py
+-rw-r--r--   0 zack       (501) staff       (20)     1611 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/sort.py
+-rw-r--r--   0 zack       (501) staff       (20)     7814 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/space.py
+-rw-r--r--   0 zack       (501) staff       (20)     9821 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/space_create.py
+-rw-r--r--   0 zack       (501) staff       (20)      188 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/space_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     9903 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/space_update.py
+-rw-r--r--   0 zack       (501) staff       (20)      151 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/sprint_mode.py
+-rw-r--r--   0 zack       (501) staff       (20)     4280 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/status.py
+-rw-r--r--   0 zack       (501) staff       (20)     4497 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/status_create.py
+-rw-r--r--   0 zack       (501) staff       (20)      243 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/status_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     4980 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/status_update.py
+-rw-r--r--   0 zack       (501) staff       (20)      249 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/statuses_list_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)      167 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/subscription.py
+-rw-r--r--   0 zack       (501) staff       (20)      172 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/subtask_display_mode.py
+-rw-r--r--   0 zack       (501) staff       (20)      403 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/summary_statistic_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)    12044 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/task.py
+-rw-r--r--   0 zack       (501) staff       (20)    13364 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/task_create.py
+-rw-r--r--   0 zack       (501) staff       (20)     2298 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/task_doc_relationship.py
+-rw-r--r--   0 zack       (501) staff       (20)     1863 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/task_doc_relationship_create.py
+-rw-r--r--   0 zack       (501) staff       (20)     3093 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/task_link.py
+-rw-r--r--   0 zack       (501) staff       (20)     3668 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/task_link_create.py
+-rw-r--r--   0 zack       (501) staff       (20)      661 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/task_link_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     3916 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/task_link_update.py
+-rw-r--r--   0 zack       (501) staff       (20)     4890 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/task_notion_document.py
+-rw-r--r--   0 zack       (501) staff       (20)     1337 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/task_notion_document_block_children_map.py
+-rw-r--r--   0 zack       (501) staff       (20)     1294 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/task_notion_document_block_map.py
+-rw-r--r--   0 zack       (501) staff       (20)     1289 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/task_notion_document_page_map.py
+-rw-r--r--   0 zack       (501) staff       (20)     1225 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/task_properties.py
+-rw-r--r--   0 zack       (501) staff       (20)      811 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/task_source_type.py
+-rw-r--r--   0 zack       (501) staff       (20)    13364 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/task_update.py
+-rw-r--r--   0 zack       (501) staff       (20)     8816 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/tenant.py
+-rw-r--r--   0 zack       (501) staff       (20)     4446 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/tenant_update.py
+-rw-r--r--   0 zack       (501) staff       (20)      186 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/theme.py
+-rw-r--r--   0 zack       (501) staff       (20)     5226 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/transaction.py
+-rw-r--r--   0 zack       (501) staff       (20)     2426 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/transaction_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     2470 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/transaction_response.py
+-rw-r--r--   0 zack       (501) staff       (20)     6056 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/user.py
+-rw-r--r--   0 zack       (501) staff       (20)     1718 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/user_dartboard_layout.py
+-rw-r--r--   0 zack       (501) staff       (20)     1991 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/user_dartboard_layout_create.py
+-rw-r--r--   0 zack       (501) staff       (20)      767 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/user_data_entity_retrieve_entity_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)      175 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/user_role.py
+-rw-r--r--   0 zack       (501) staff       (20)      313 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/user_status.py
+-rw-r--r--   0 zack       (501) staff       (20)     7155 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/user_update.py
+-rw-r--r--   0 zack       (501) staff       (20)     1804 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/validation_error_response.py
+-rw-r--r--   0 zack       (501) staff       (20)     1301 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/validation_error_response_items.py
+-rw-r--r--   0 zack       (501) staff       (20)     6609 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/view.py
+-rw-r--r--   0 zack       (501) staff       (20)     7999 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/view_create.py
+-rw-r--r--   0 zack       (501) staff       (20)      203 2024-05-10 23:23:29.000000 dart_tools-0.5.7/dart/generated/models/view_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     8169 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/view_update.py
+-rw-r--r--   0 zack       (501) staff       (20)     1782 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/models/zapier_integration.py
+-rw-r--r--   0 zack       (501) staff       (20)       25 2024-05-10 23:23:28.000000 dart_tools-0.5.7/dart/generated/py.typed
+-rw-r--r--   0 zack       (501) staff       (20)      968 2024-05-10 23:23:30.000000 dart_tools-0.5.7/dart/generated/types.py
+-rw-r--r--   0 zack       (501) staff       (20)     1905 2023-12-06 01:16:03.000000 dart_tools-0.5.7/dart/order_manager.py
+-rw-r--r--   0 zack       (501) staff       (20)      569 2023-12-01 08:32:06.000000 dart_tools-0.5.7/dart/webhook.py
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2024-05-10 23:23:37.066470 dart_tools-0.5.7/dart_tools.egg-info/
+-rw-r--r--   0 zack       (501) staff       (20)     7166 2024-05-10 23:23:37.000000 dart_tools-0.5.7/dart_tools.egg-info/PKG-INFO
+-rw-r--r--   0 zack       (501) staff       (20)     7299 2024-05-10 23:23:37.000000 dart_tools-0.5.7/dart_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 zack       (501) staff       (20)        1 2024-05-10 23:23:37.000000 dart_tools-0.5.7/dart_tools.egg-info/dependency_links.txt
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2024-05-10 23:23:37.065879 dart_tools-0.5.7/dart_tools.egg-info/dist/
+-rw-r--r--   0 zack       (501) staff       (20)     8788 2023-06-03 08:11:34.000000 dart_tools-0.5.7/dart_tools.egg-info/dist/dart-tools-0.3.3.tar.gz
+-rw-r--r--   0 zack       (501) staff       (20)       34 2024-05-10 23:23:37.000000 dart_tools-0.5.7/dart_tools.egg-info/entry_points.txt
+-rw-r--r--   0 zack       (501) staff       (20)       38 2024-05-10 23:23:37.000000 dart_tools-0.5.7/dart_tools.egg-info/requires.txt
+-rw-r--r--   0 zack       (501) staff       (20)        5 2024-05-10 23:23:37.000000 dart_tools-0.5.7/dart_tools.egg-info/top_level.txt
+-rw-r--r--   0 zack       (501) staff       (20)     1891 2024-05-10 23:05:06.000000 dart_tools-0.5.7/pyproject.toml
+-rw-r--r--   0 zack       (501) staff       (20)       38 2024-05-10 23:23:37.067164 dart_tools-0.5.7/setup.cfg
```

### Comparing `dart_tools-0.5.6/LICENSE` & `dart_tools-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/PKG-INFO` & `dart_tools-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dart-tools
-Version: 0.5.6
+Version: 0.5.7
 Summary: The Dart CLI and Python Library
 Author-email: Dart Software Team <software@itsdart.com>
 License: MIT License
         
         Copyright (c) 2023 Dart
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dart-tools Version: 0.5.6 Summary: The Dart CLI and
+Metadata-Version: 2.1 Name: dart-tools Version: 0.5.7 Summary: The Dart CLI and
 Python Library Author-email: Dart Software Team
 itsdart.com> License: MIT License Copyright (c) 2023 Dart Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `dart_tools-0.5.6/README.md` & `dart_tools-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/dart.py` & `dart_tools-0.5.7/dart/dart.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/api/transactions/transactions_create.py` & `dart_tools-0.5.7/dart/generated/api/transactions/transactions_create.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/client.py` & `dart_tools-0.5.7/dart/generated/client.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/__init__.py` & `dart_tools-0.5.7/dart/generated/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """ Contains all the data models used in inputs/outputs """
 
 from .attachment import Attachment
 from .attachment_create import AttachmentCreate
 from .attachment_update import AttachmentUpdate
-from .batch import Batch
 from .brainstorm import Brainstorm
 from .brainstorm_create import BrainstormCreate
 from .brainstorm_state import BrainstormState
 from .brainstorm_update import BrainstormUpdate
 from .color_name import ColorName
 from .comment import Comment
 from .comment_create import CommentCreate
@@ -94,15 +93,14 @@
 from .paginated_view_list import PaginatedViewList
 from .priority import Priority
 from .properties_list_kind import PropertiesListKind
 from .property_ import Property
 from .property_create import PropertyCreate
 from .property_kind import PropertyKind
 from .property_update import PropertyUpdate
-from .recommendation_status import RecommendationStatus
 from .relationship import Relationship
 from .relationship_create import RelationshipCreate
 from .relationship_kind import RelationshipKind
 from .relationship_kind_create import RelationshipKindCreate
 from .relationship_kind_kind import RelationshipKindKind
 from .relationship_kind_update import RelationshipKindUpdate
 from .report_kind import ReportKind
@@ -154,22 +152,20 @@
 from .user_update import UserUpdate
 from .validation_error_response import ValidationErrorResponse
 from .validation_error_response_items import ValidationErrorResponseItems
 from .view import View
 from .view_create import ViewCreate
 from .view_kind import ViewKind
 from .view_update import ViewUpdate
-from .yc_integration import YcIntegration
 from .zapier_integration import ZapierIntegration
 
 __all__ = (
     "Attachment",
     "AttachmentCreate",
     "AttachmentUpdate",
-    "Batch",
     "Brainstorm",
     "BrainstormCreate",
     "BrainstormState",
     "BrainstormUpdate",
     "ColorName",
     "Comment",
     "CommentCreate",
@@ -256,15 +252,14 @@
     "PaginatedViewList",
     "Priority",
     "PropertiesListKind",
     "Property",
     "PropertyCreate",
     "PropertyKind",
     "PropertyUpdate",
-    "RecommendationStatus",
     "Relationship",
     "RelationshipCreate",
     "RelationshipKind",
     "RelationshipKindCreate",
     "RelationshipKindKind",
     "RelationshipKindUpdate",
     "ReportKind",
@@ -316,10 +311,9 @@
     "UserUpdate",
     "ValidationErrorResponse",
     "ValidationErrorResponseItems",
     "View",
     "ViewCreate",
     "ViewKind",
     "ViewUpdate",
-    "YcIntegration",
     "ZapierIntegration",
 )
```

### Comparing `dart_tools-0.5.6/dart/generated/models/attachment.py` & `dart_tools-0.5.7/dart/generated/models/attachment.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/attachment_create.py` & `dart_tools-0.5.7/dart/generated/models/attachment_create.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/attachment_update.py` & `dart_tools-0.5.7/dart/generated/models/attachment_update.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/brainstorm.py` & `dart_tools-0.5.7/dart/generated/models/brainstorm.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/brainstorm_create.py` & `dart_tools-0.5.7/dart/generated/models/brainstorm_create.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/brainstorm_update.py` & `dart_tools-0.5.7/dart/generated/models/brainstorm_update.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/color_name.py` & `dart_tools-0.5.7/dart/generated/models/color_name.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/comment.py` & `dart_tools-0.5.7/dart/generated/models/comment.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/comment_create.py` & `dart_tools-0.5.7/dart/generated/models/comment_create.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/comment_reaction.py` & `dart_tools-0.5.7/dart/generated/models/comment_reaction.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/comment_reaction_create.py` & `dart_tools-0.5.7/dart/generated/models/comment_reaction_create.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/comment_reaction_update.py` & `dart_tools-0.5.7/dart/generated/models/comment_reaction_update.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/comment_update.py` & `dart_tools-0.5.7/dart/generated/models/comment_update.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/dartboard.py` & `dart_tools-0.5.7/dart/generated/models/dartboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     """
     Attributes:
         duid (str):
         space_duid (str):
         kind (DartboardKind): * `Active` - ACTIVE
             * `Next` - NEXT
             * `Backlog` - BACKLOG
-            * `YC` - YC
             * `Finished` - FINISHED
             * `Custom` - CUSTOM
         order (str):
         title (str):
         description (str):
         icon_kind (IconKind): * `None` - NONE
             * `Icon` - ICON
```

### Comparing `dart_tools-0.5.6/dart/generated/models/dartboard_create.py` & `dart_tools-0.5.7/dart/generated/models/dartboard_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     Attributes:
         duid (str):
         space_duid (str):
         order (str):
         kind (Union[Unset, DartboardKind]): * `Active` - ACTIVE
             * `Next` - NEXT
             * `Backlog` - BACKLOG
-            * `YC` - YC
             * `Finished` - FINISHED
             * `Custom` - CUSTOM
         title (Union[Unset, str]):
         description (Union[Unset, str]):
         icon_kind (Union[Unset, IconKind]): * `None` - NONE
             * `Icon` - ICON
             * `Emoji` - EMOJI
```

### Comparing `dart_tools-0.5.6/dart/generated/models/dartboard_update.py` & `dart_tools-0.5.7/dart/generated/models/dartboard_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     """
     Attributes:
         duid (str):
         space_duid (Union[Unset, str]):
         kind (Union[Unset, DartboardKind]): * `Active` - ACTIVE
             * `Next` - NEXT
             * `Backlog` - BACKLOG
-            * `YC` - YC
             * `Finished` - FINISHED
             * `Custom` - CUSTOM
         order (Union[Unset, str]):
         title (Union[Unset, str]):
         description (Union[Unset, str]):
         icon_kind (Union[Unset, IconKind]): * `None` - NONE
             * `Icon` - ICON
```

### Comparing `dart_tools-0.5.6/dart/generated/models/discord_integration.py` & `dart_tools-0.5.7/dart/generated/models/discord_integration.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/doc.py` & `dart_tools-0.5.7/dart/generated/models/doc.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/doc_create.py` & `dart_tools-0.5.7/dart/generated/models/doc_create.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/doc_update.py` & `dart_tools-0.5.7/dart/generated/models/doc_update.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/event.py` & `dart_tools-0.5.7/dart/generated/models/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,19 @@
             * `ai/content` - AI_CONTENT
             * `ai/translate` - AI_TRANSLATE
             * `ai/emoji` - AI_EMOJI
             * `ai/feedback` - AI_FEEDBACK
             * `ai/icon` - AI_ICON
             * `ai/report` - AI_REPORT
             * `ai/plan` - AI_PLAN
+            * `ai/brainstorm_start` - AI_BRAINSTORM_START
+            * `ai/detect_duplicates` - AI_DETECT_DUPLICATES
+            * `ai/filters` - AI_FILTERS
+            * `ai/execute` - AI_EXECUTE
+            * `ai/image` - AI_IMAGE
             * `load/signup` - LOAD_SIGNUP
             * `help/resource_click` - HELP_RESOURCE_CLICK
             * `usage/submit_feedback` - USAGE_SUBMIT_FEEDBACK
             * `usage/undo` - USAGE_UNDO
             * `usage/redo` - USAGE_REDO
             * `usage/open_command_center` - USAGE_OPEN_COMMAND_CENTER
             * `usage/open_rightbar` - USAGE_OPEN_RIGHTBAR
```

### Comparing `dart_tools-0.5.6/dart/generated/models/event_actor.py` & `dart_tools-0.5.7/dart/generated/models/event_actor.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/event_create.py` & `dart_tools-0.5.7/dart/generated/models/event_create.py`

 * *Files 11% similar despite different names*

```diff
@@ -62,14 +62,19 @@
             * `ai/content` - AI_CONTENT
             * `ai/translate` - AI_TRANSLATE
             * `ai/emoji` - AI_EMOJI
             * `ai/feedback` - AI_FEEDBACK
             * `ai/icon` - AI_ICON
             * `ai/report` - AI_REPORT
             * `ai/plan` - AI_PLAN
+            * `ai/brainstorm_start` - AI_BRAINSTORM_START
+            * `ai/detect_duplicates` - AI_DETECT_DUPLICATES
+            * `ai/filters` - AI_FILTERS
+            * `ai/execute` - AI_EXECUTE
+            * `ai/image` - AI_IMAGE
             * `load/signup` - LOAD_SIGNUP
             * `help/resource_click` - HELP_RESOURCE_CLICK
             * `usage/submit_feedback` - USAGE_SUBMIT_FEEDBACK
             * `usage/undo` - USAGE_UNDO
             * `usage/redo` - USAGE_REDO
             * `usage/open_command_center` - USAGE_OPEN_COMMAND_CENTER
             * `usage/open_rightbar` - USAGE_OPEN_RIGHTBAR
```

### Comparing `dart_tools-0.5.6/dart/generated/models/event_kind.py` & `dart_tools-0.5.7/dart/generated/models/event_kind.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from enum import Enum
 
 
 class EventKind(str, Enum):
+    AIBRAINSTORM_START = "ai/brainstorm_start"
     AICONTENT = "ai/content"
+    AIDETECT_DUPLICATES = "ai/detect_duplicates"
     AIEMOJI = "ai/emoji"
+    AIEXECUTE = "ai/execute"
     AIFEEDBACK = "ai/feedback"
+    AIFILTERS = "ai/filters"
     AIICON = "ai/icon"
+    AIIMAGE = "ai/image"
     AIPLAN = "ai/plan"
     AIPROPS = "ai/props"
     AIREPORT = "ai/report"
     AISUBTASKS = "ai/subtasks"
     AITRANSLATE = "ai/translate"
     BRAINSTORMSTART = "brainstorm/start"
     BRAINSTORMSTOP = "brainstorm/stop"
```

### Comparing `dart_tools-0.5.6/dart/generated/models/event_subscription.py` & `dart_tools-0.5.7/dart/generated/models/event_subscription.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/event_subscription_update.py` & `dart_tools-0.5.7/dart/generated/models/event_subscription_update.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,14 +62,19 @@
             * `ai/content` - AI_CONTENT
             * `ai/translate` - AI_TRANSLATE
             * `ai/emoji` - AI_EMOJI
             * `ai/feedback` - AI_FEEDBACK
             * `ai/icon` - AI_ICON
             * `ai/report` - AI_REPORT
             * `ai/plan` - AI_PLAN
+            * `ai/brainstorm_start` - AI_BRAINSTORM_START
+            * `ai/detect_duplicates` - AI_DETECT_DUPLICATES
+            * `ai/filters` - AI_FILTERS
+            * `ai/execute` - AI_EXECUTE
+            * `ai/image` - AI_IMAGE
             * `load/signup` - LOAD_SIGNUP
             * `help/resource_click` - HELP_RESOURCE_CLICK
             * `usage/submit_feedback` - USAGE_SUBMIT_FEEDBACK
             * `usage/undo` - USAGE_UNDO
             * `usage/redo` - USAGE_REDO
             * `usage/open_command_center` - USAGE_OPEN_COMMAND_CENTER
             * `usage/open_rightbar` - USAGE_OPEN_RIGHTBAR
```

### Comparing `dart_tools-0.5.6/dart/generated/models/filter_applicability.py` & `dart_tools-0.5.7/dart/generated/models/filter_applicability.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/filter_assignee.py` & `dart_tools-0.5.7/dart/generated/models/filter_assignee.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/filter_group.py` & `dart_tools-0.5.7/dart/generated/models/filter_group.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/filter_search.py` & `dart_tools-0.5.7/dart/generated/models/filter_search.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/filter_set.py` & `dart_tools-0.5.7/dart/generated/models/filter_set.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/folder.py` & `dart_tools-0.5.7/dart/generated/models/form_create.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,34 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..models.color_name import ColorName
-from ..models.folder_kind import FolderKind
 from ..models.icon_kind import IconKind
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="Folder")
+T = TypeVar("T", bound="FormCreate")
 
 
 @_attrs_define
-class Folder:
+class FormCreate:
     """
     Attributes:
         duid (str):
-        space_duid (str):
-        kind (FolderKind): * `Other` - OTHER
-            * `Default` - DEFAULT
-            * `Reports` - REPORTS
-        accessible_by_team (bool):
-        accessible_by_user_duids (List[str]):
         order (str):
-        title (str):
-        description (str):
-        icon_kind (IconKind): * `None` - NONE
+        hidden (Union[Unset, bool]):
+        public (Union[Unset, bool]):
+        title (Union[Unset, str]):
+        description (Union[Unset, str]):
+        icon_kind (Union[Unset, IconKind]): * `None` - NONE
             * `Icon` - ICON
             * `Emoji` - EMOJI
-        icon_name_or_emoji (str):
-        color_name (ColorName): * `Red` - RED
+        icon_name_or_emoji (Union[Unset, str]):
+        color_name (Union[Unset, ColorName]): * `Red` - RED
             * `Dark Blue` - DARK_BLUE
             * `Dark Orange` - DARK_ORANGE
             * `Dark Green` - DARK_GREEN
             * `Purple` - PURPLE
             * `Dark Teal` - DARK_TEAL
             * `Pink` - PINK
             * `Orange` - ORANGE
@@ -49,115 +44,113 @@
             * `Light Purple` - LIGHT_PURPLE
             * `Light Orange` - LIGHT_ORANGE
             * `Light Pink` - LIGHT_PINK
             * `Tan` - TAN
             * `Dark Gray` - DARK_GRAY
             * `Light Brown` - LIGHT_BROWN
             * `Light Gray` - LIGHT_GRAY
-        updated_by_client_duid (Union[Unset, None, str]):
     """
 
     duid: str
-    space_duid: str
-    kind: FolderKind
-    accessible_by_team: bool
-    accessible_by_user_duids: List[str]
     order: str
-    title: str
-    description: str
-    icon_kind: IconKind
-    icon_name_or_emoji: str
-    color_name: ColorName
-    updated_by_client_duid: Union[Unset, None, str] = UNSET
+    hidden: Union[Unset, bool] = UNSET
+    public: Union[Unset, bool] = UNSET
+    title: Union[Unset, str] = UNSET
+    description: Union[Unset, str] = UNSET
+    icon_kind: Union[Unset, IconKind] = UNSET
+    icon_name_or_emoji: Union[Unset, str] = UNSET
+    color_name: Union[Unset, ColorName] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         duid = self.duid
-        space_duid = self.space_duid
-        kind = self.kind.value
-
-        accessible_by_team = self.accessible_by_team
-        accessible_by_user_duids = self.accessible_by_user_duids
-
         order = self.order
+        hidden = self.hidden
+        public = self.public
         title = self.title
         description = self.description
-        icon_kind = self.icon_kind.value
+        icon_kind: Union[Unset, str] = UNSET
+        if not isinstance(self.icon_kind, Unset):
+            icon_kind = self.icon_kind.value
 
         icon_name_or_emoji = self.icon_name_or_emoji
-        color_name = self.color_name.value
-
-        updated_by_client_duid = self.updated_by_client_duid
+        color_name: Union[Unset, str] = UNSET
+        if not isinstance(self.color_name, Unset):
+            color_name = self.color_name.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "duid": duid,
-                "spaceDuid": space_duid,
-                "kind": kind,
-                "accessibleByTeam": accessible_by_team,
-                "accessibleByUserDuids": accessible_by_user_duids,
                 "order": order,
-                "title": title,
-                "description": description,
-                "iconKind": icon_kind,
-                "iconNameOrEmoji": icon_name_or_emoji,
-                "colorName": color_name,
             }
         )
-        if updated_by_client_duid is not UNSET:
-            field_dict["updatedByClientDuid"] = updated_by_client_duid
+        if hidden is not UNSET:
+            field_dict["hidden"] = hidden
+        if public is not UNSET:
+            field_dict["public"] = public
+        if title is not UNSET:
+            field_dict["title"] = title
+        if description is not UNSET:
+            field_dict["description"] = description
+        if icon_kind is not UNSET:
+            field_dict["iconKind"] = icon_kind
+        if icon_name_or_emoji is not UNSET:
+            field_dict["iconNameOrEmoji"] = icon_name_or_emoji
+        if color_name is not UNSET:
+            field_dict["colorName"] = color_name
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         duid = d.pop("duid")
 
-        space_duid = d.pop("spaceDuid")
-
-        kind = FolderKind(d.pop("kind"))
-
-        accessible_by_team = d.pop("accessibleByTeam")
-
-        accessible_by_user_duids = cast(List[str], d.pop("accessibleByUserDuids"))
-
         order = d.pop("order")
 
-        title = d.pop("title")
+        hidden = d.pop("hidden", UNSET)
+
+        public = d.pop("public", UNSET)
 
-        description = d.pop("description")
+        title = d.pop("title", UNSET)
 
-        icon_kind = IconKind(d.pop("iconKind"))
+        description = d.pop("description", UNSET)
 
-        icon_name_or_emoji = d.pop("iconNameOrEmoji")
+        _icon_kind = d.pop("iconKind", UNSET)
+        icon_kind: Union[Unset, IconKind]
+        if isinstance(_icon_kind, Unset):
+            icon_kind = UNSET
+        else:
+            icon_kind = IconKind(_icon_kind)
 
-        color_name = ColorName(d.pop("colorName"))
+        icon_name_or_emoji = d.pop("iconNameOrEmoji", UNSET)
 
-        updated_by_client_duid = d.pop("updatedByClientDuid", UNSET)
+        _color_name = d.pop("colorName", UNSET)
+        color_name: Union[Unset, ColorName]
+        if isinstance(_color_name, Unset):
+            color_name = UNSET
+        else:
+            color_name = ColorName(_color_name)
 
-        folder = cls(
+        form_create = cls(
             duid=duid,
-            space_duid=space_duid,
-            kind=kind,
-            accessible_by_team=accessible_by_team,
-            accessible_by_user_duids=accessible_by_user_duids,
             order=order,
+            hidden=hidden,
+            public=public,
             title=title,
             description=description,
             icon_kind=icon_kind,
             icon_name_or_emoji=icon_name_or_emoji,
             color_name=color_name,
-            updated_by_client_duid=updated_by_client_duid,
         )
 
-        folder.additional_properties = d
-        return folder
+        form_create.additional_properties = d
+        return form_create
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart_tools-0.5.6/dart/generated/models/folder_create.py` & `dart_tools-0.5.7/dart/generated/models/folder_update.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..models.color_name import ColorName
 from ..models.folder_kind import FolderKind
 from ..models.icon_kind import IconKind
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="FolderCreate")
+T = TypeVar("T", bound="FolderUpdate")
 
 
 @_attrs_define
-class FolderCreate:
+class FolderUpdate:
     """
     Attributes:
         duid (str):
-        space_duid (str):
-        order (str):
+        space_duid (Union[Unset, str]):
         kind (Union[Unset, FolderKind]): * `Other` - OTHER
             * `Default` - DEFAULT
             * `Reports` - REPORTS
-        accessible_by_team (Union[Unset, bool]):
-        accessible_by_user_duids (Union[Unset, List[str]]):
+        order (Union[Unset, str]):
         title (Union[Unset, str]):
         description (Union[Unset, str]):
         icon_kind (Union[Unset, IconKind]): * `None` - NONE
             * `Icon` - ICON
             * `Emoji` - EMOJI
         icon_name_or_emoji (Union[Unset, str]):
         color_name (Union[Unset, ColorName]): * `Red` - RED
@@ -52,39 +50,32 @@
             * `Tan` - TAN
             * `Dark Gray` - DARK_GRAY
             * `Light Brown` - LIGHT_BROWN
             * `Light Gray` - LIGHT_GRAY
     """
 
     duid: str
-    space_duid: str
-    order: str
+    space_duid: Union[Unset, str] = UNSET
     kind: Union[Unset, FolderKind] = UNSET
-    accessible_by_team: Union[Unset, bool] = UNSET
-    accessible_by_user_duids: Union[Unset, List[str]] = UNSET
+    order: Union[Unset, str] = UNSET
     title: Union[Unset, str] = UNSET
     description: Union[Unset, str] = UNSET
     icon_kind: Union[Unset, IconKind] = UNSET
     icon_name_or_emoji: Union[Unset, str] = UNSET
     color_name: Union[Unset, ColorName] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         duid = self.duid
         space_duid = self.space_duid
-        order = self.order
         kind: Union[Unset, str] = UNSET
         if not isinstance(self.kind, Unset):
             kind = self.kind.value
 
-        accessible_by_team = self.accessible_by_team
-        accessible_by_user_duids: Union[Unset, List[str]] = UNSET
-        if not isinstance(self.accessible_by_user_duids, Unset):
-            accessible_by_user_duids = self.accessible_by_user_duids
-
+        order = self.order
         title = self.title
         description = self.description
         icon_kind: Union[Unset, str] = UNSET
         if not isinstance(self.icon_kind, Unset):
             icon_kind = self.icon_kind.value
 
         icon_name_or_emoji = self.icon_name_or_emoji
@@ -93,24 +84,22 @@
             color_name = self.color_name.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "duid": duid,
-                "spaceDuid": space_duid,
-                "order": order,
             }
         )
+        if space_duid is not UNSET:
+            field_dict["spaceDuid"] = space_duid
         if kind is not UNSET:
             field_dict["kind"] = kind
-        if accessible_by_team is not UNSET:
-            field_dict["accessibleByTeam"] = accessible_by_team
-        if accessible_by_user_duids is not UNSET:
-            field_dict["accessibleByUserDuids"] = accessible_by_user_duids
+        if order is not UNSET:
+            field_dict["order"] = order
         if title is not UNSET:
             field_dict["title"] = title
         if description is not UNSET:
             field_dict["description"] = description
         if icon_kind is not UNSET:
             field_dict["iconKind"] = icon_kind
         if icon_name_or_emoji is not UNSET:
@@ -121,28 +110,24 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         duid = d.pop("duid")
 
-        space_duid = d.pop("spaceDuid")
-
-        order = d.pop("order")
+        space_duid = d.pop("spaceDuid", UNSET)
 
         _kind = d.pop("kind", UNSET)
         kind: Union[Unset, FolderKind]
         if isinstance(_kind, Unset):
             kind = UNSET
         else:
             kind = FolderKind(_kind)
 
-        accessible_by_team = d.pop("accessibleByTeam", UNSET)
-
-        accessible_by_user_duids = cast(List[str], d.pop("accessibleByUserDuids", UNSET))
+        order = d.pop("order", UNSET)
 
         title = d.pop("title", UNSET)
 
         description = d.pop("description", UNSET)
 
         _icon_kind = d.pop("iconKind", UNSET)
         icon_kind: Union[Unset, IconKind]
@@ -156,30 +141,28 @@
         _color_name = d.pop("colorName", UNSET)
         color_name: Union[Unset, ColorName]
         if isinstance(_color_name, Unset):
             color_name = UNSET
         else:
             color_name = ColorName(_color_name)
 
-        folder_create = cls(
+        folder_update = cls(
             duid=duid,
             space_duid=space_duid,
-            order=order,
             kind=kind,
-            accessible_by_team=accessible_by_team,
-            accessible_by_user_duids=accessible_by_user_duids,
+            order=order,
             title=title,
             description=description,
             icon_kind=icon_kind,
             icon_name_or_emoji=icon_name_or_emoji,
             color_name=color_name,
         )
 
-        folder_create.additional_properties = d
-        return folder_create
+        folder_update.additional_properties = d
+        return folder_update
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart_tools-0.5.6/dart/generated/models/folder_update.py` & `dart_tools-0.5.7/dart/generated/models/folder_create.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..models.color_name import ColorName
 from ..models.folder_kind import FolderKind
 from ..models.icon_kind import IconKind
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="FolderUpdate")
+T = TypeVar("T", bound="FolderCreate")
 
 
 @_attrs_define
-class FolderUpdate:
+class FolderCreate:
     """
     Attributes:
         duid (str):
-        space_duid (Union[Unset, str]):
+        space_duid (str):
+        order (str):
         kind (Union[Unset, FolderKind]): * `Other` - OTHER
             * `Default` - DEFAULT
             * `Reports` - REPORTS
-        accessible_by_team (Union[Unset, bool]):
-        accessible_by_user_duids (Union[Unset, List[str]]):
-        order (Union[Unset, str]):
         title (Union[Unset, str]):
         description (Union[Unset, str]):
         icon_kind (Union[Unset, IconKind]): * `None` - NONE
             * `Icon` - ICON
             * `Emoji` - EMOJI
         icon_name_or_emoji (Union[Unset, str]):
         color_name (Union[Unset, ColorName]): * `Red` - RED
@@ -52,39 +50,32 @@
             * `Tan` - TAN
             * `Dark Gray` - DARK_GRAY
             * `Light Brown` - LIGHT_BROWN
             * `Light Gray` - LIGHT_GRAY
     """
 
     duid: str
-    space_duid: Union[Unset, str] = UNSET
+    space_duid: str
+    order: str
     kind: Union[Unset, FolderKind] = UNSET
-    accessible_by_team: Union[Unset, bool] = UNSET
-    accessible_by_user_duids: Union[Unset, List[str]] = UNSET
-    order: Union[Unset, str] = UNSET
     title: Union[Unset, str] = UNSET
     description: Union[Unset, str] = UNSET
     icon_kind: Union[Unset, IconKind] = UNSET
     icon_name_or_emoji: Union[Unset, str] = UNSET
     color_name: Union[Unset, ColorName] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         duid = self.duid
         space_duid = self.space_duid
+        order = self.order
         kind: Union[Unset, str] = UNSET
         if not isinstance(self.kind, Unset):
             kind = self.kind.value
 
-        accessible_by_team = self.accessible_by_team
-        accessible_by_user_duids: Union[Unset, List[str]] = UNSET
-        if not isinstance(self.accessible_by_user_duids, Unset):
-            accessible_by_user_duids = self.accessible_by_user_duids
-
-        order = self.order
         title = self.title
         description = self.description
         icon_kind: Union[Unset, str] = UNSET
         if not isinstance(self.icon_kind, Unset):
             icon_kind = self.icon_kind.value
 
         icon_name_or_emoji = self.icon_name_or_emoji
@@ -93,26 +84,20 @@
             color_name = self.color_name.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "duid": duid,
+                "spaceDuid": space_duid,
+                "order": order,
             }
         )
-        if space_duid is not UNSET:
-            field_dict["spaceDuid"] = space_duid
         if kind is not UNSET:
             field_dict["kind"] = kind
-        if accessible_by_team is not UNSET:
-            field_dict["accessibleByTeam"] = accessible_by_team
-        if accessible_by_user_duids is not UNSET:
-            field_dict["accessibleByUserDuids"] = accessible_by_user_duids
-        if order is not UNSET:
-            field_dict["order"] = order
         if title is not UNSET:
             field_dict["title"] = title
         if description is not UNSET:
             field_dict["description"] = description
         if icon_kind is not UNSET:
             field_dict["iconKind"] = icon_kind
         if icon_name_or_emoji is not UNSET:
@@ -123,29 +108,25 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         duid = d.pop("duid")
 
-        space_duid = d.pop("spaceDuid", UNSET)
+        space_duid = d.pop("spaceDuid")
+
+        order = d.pop("order")
 
         _kind = d.pop("kind", UNSET)
         kind: Union[Unset, FolderKind]
         if isinstance(_kind, Unset):
             kind = UNSET
         else:
             kind = FolderKind(_kind)
 
-        accessible_by_team = d.pop("accessibleByTeam", UNSET)
-
-        accessible_by_user_duids = cast(List[str], d.pop("accessibleByUserDuids", UNSET))
-
-        order = d.pop("order", UNSET)
-
         title = d.pop("title", UNSET)
 
         description = d.pop("description", UNSET)
 
         _icon_kind = d.pop("iconKind", UNSET)
         icon_kind: Union[Unset, IconKind]
         if isinstance(_icon_kind, Unset):
@@ -158,30 +139,28 @@
         _color_name = d.pop("colorName", UNSET)
         color_name: Union[Unset, ColorName]
         if isinstance(_color_name, Unset):
             color_name = UNSET
         else:
             color_name = ColorName(_color_name)
 
-        folder_update = cls(
+        folder_create = cls(
             duid=duid,
             space_duid=space_duid,
-            kind=kind,
-            accessible_by_team=accessible_by_team,
-            accessible_by_user_duids=accessible_by_user_duids,
             order=order,
+            kind=kind,
             title=title,
             description=description,
             icon_kind=icon_kind,
             icon_name_or_emoji=icon_name_or_emoji,
             color_name=color_name,
         )
 
-        folder_update.additional_properties = d
-        return folder_update
+        folder_create.additional_properties = d
+        return folder_create
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart_tools-0.5.6/dart/generated/models/form.py` & `dart_tools-0.5.7/dart/generated/models/form.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/form_create.py` & `dart_tools-0.5.7/dart/generated/models/form_update.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..models.color_name import ColorName
 from ..models.icon_kind import IconKind
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="FormCreate")
+T = TypeVar("T", bound="FormUpdate")
 
 
 @_attrs_define
-class FormCreate:
+class FormUpdate:
     """
     Attributes:
         duid (str):
-        order (str):
         hidden (Union[Unset, bool]):
         public (Union[Unset, bool]):
+        order (Union[Unset, str]):
         title (Union[Unset, str]):
         description (Union[Unset, str]):
         icon_kind (Union[Unset, IconKind]): * `None` - NONE
             * `Icon` - ICON
             * `Emoji` - EMOJI
         icon_name_or_emoji (Union[Unset, str]):
         color_name (Union[Unset, ColorName]): * `Red` - RED
@@ -47,29 +47,29 @@
             * `Tan` - TAN
             * `Dark Gray` - DARK_GRAY
             * `Light Brown` - LIGHT_BROWN
             * `Light Gray` - LIGHT_GRAY
     """
 
     duid: str
-    order: str
     hidden: Union[Unset, bool] = UNSET
     public: Union[Unset, bool] = UNSET
+    order: Union[Unset, str] = UNSET
     title: Union[Unset, str] = UNSET
     description: Union[Unset, str] = UNSET
     icon_kind: Union[Unset, IconKind] = UNSET
     icon_name_or_emoji: Union[Unset, str] = UNSET
     color_name: Union[Unset, ColorName] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         duid = self.duid
-        order = self.order
         hidden = self.hidden
         public = self.public
+        order = self.order
         title = self.title
         description = self.description
         icon_kind: Union[Unset, str] = UNSET
         if not isinstance(self.icon_kind, Unset):
             icon_kind = self.icon_kind.value
 
         icon_name_or_emoji = self.icon_name_or_emoji
@@ -78,21 +78,22 @@
             color_name = self.color_name.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "duid": duid,
-                "order": order,
             }
         )
         if hidden is not UNSET:
             field_dict["hidden"] = hidden
         if public is not UNSET:
             field_dict["public"] = public
+        if order is not UNSET:
+            field_dict["order"] = order
         if title is not UNSET:
             field_dict["title"] = title
         if description is not UNSET:
             field_dict["description"] = description
         if icon_kind is not UNSET:
             field_dict["iconKind"] = icon_kind
         if icon_name_or_emoji is not UNSET:
@@ -103,20 +104,20 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         duid = d.pop("duid")
 
-        order = d.pop("order")
-
         hidden = d.pop("hidden", UNSET)
 
         public = d.pop("public", UNSET)
 
+        order = d.pop("order", UNSET)
+
         title = d.pop("title", UNSET)
 
         description = d.pop("description", UNSET)
 
         _icon_kind = d.pop("iconKind", UNSET)
         icon_kind: Union[Unset, IconKind]
         if isinstance(_icon_kind, Unset):
@@ -129,28 +130,28 @@
         _color_name = d.pop("colorName", UNSET)
         color_name: Union[Unset, ColorName]
         if isinstance(_color_name, Unset):
             color_name = UNSET
         else:
             color_name = ColorName(_color_name)
 
-        form_create = cls(
+        form_update = cls(
             duid=duid,
-            order=order,
             hidden=hidden,
             public=public,
+            order=order,
             title=title,
             description=description,
             icon_kind=icon_kind,
             icon_name_or_emoji=icon_name_or_emoji,
             color_name=color_name,
         )
 
-        form_create.additional_properties = d
-        return form_create
+        form_update.additional_properties = d
+        return form_update
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart_tools-0.5.6/dart/generated/models/form_field.py` & `dart_tools-0.5.7/dart/generated/models/form_field.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/form_field_create.py` & `dart_tools-0.5.7/dart/generated/models/form_field_create.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/form_field_update.py` & `dart_tools-0.5.7/dart/generated/models/form_field_update.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/form_update.py` & `dart_tools-0.5.7/dart/generated/models/status_update.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..models.color_name import ColorName
-from ..models.icon_kind import IconKind
+from ..models.status_kind import StatusKind
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="FormUpdate")
+T = TypeVar("T", bound="StatusUpdate")
 
 
 @_attrs_define
-class FormUpdate:
+class StatusUpdate:
     """
     Attributes:
         duid (str):
-        hidden (Union[Unset, bool]):
-        public (Union[Unset, bool]):
+        property_duid (Union[Unset, str]):
+        kind (Union[Unset, StatusKind]): * `Unstarted` - UNSTARTED
+            * `Started` - STARTED
+            * `Blocked` - BLOCKED
+            * `Finished` - FINISHED
+            * `Canceled` - CANCELED
+        locked (Union[Unset, bool]):
         order (Union[Unset, str]):
         title (Union[Unset, str]):
-        description (Union[Unset, str]):
-        icon_kind (Union[Unset, IconKind]): * `None` - NONE
-            * `Icon` - ICON
-            * `Emoji` - EMOJI
-        icon_name_or_emoji (Union[Unset, str]):
         color_name (Union[Unset, ColorName]): * `Red` - RED
             * `Dark Blue` - DARK_BLUE
             * `Dark Orange` - DARK_ORANGE
             * `Dark Green` - DARK_GREEN
             * `Purple` - PURPLE
             * `Dark Teal` - DARK_TEAL
             * `Pink` - PINK
@@ -44,114 +44,109 @@
             * `Light Purple` - LIGHT_PURPLE
             * `Light Orange` - LIGHT_ORANGE
             * `Light Pink` - LIGHT_PINK
             * `Tan` - TAN
             * `Dark Gray` - DARK_GRAY
             * `Light Brown` - LIGHT_BROWN
             * `Light Gray` - LIGHT_GRAY
+        description (Union[Unset, str]):
     """
 
     duid: str
-    hidden: Union[Unset, bool] = UNSET
-    public: Union[Unset, bool] = UNSET
+    property_duid: Union[Unset, str] = UNSET
+    kind: Union[Unset, StatusKind] = UNSET
+    locked: Union[Unset, bool] = UNSET
     order: Union[Unset, str] = UNSET
     title: Union[Unset, str] = UNSET
-    description: Union[Unset, str] = UNSET
-    icon_kind: Union[Unset, IconKind] = UNSET
-    icon_name_or_emoji: Union[Unset, str] = UNSET
     color_name: Union[Unset, ColorName] = UNSET
+    description: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         duid = self.duid
-        hidden = self.hidden
-        public = self.public
+        property_duid = self.property_duid
+        kind: Union[Unset, str] = UNSET
+        if not isinstance(self.kind, Unset):
+            kind = self.kind.value
+
+        locked = self.locked
         order = self.order
         title = self.title
-        description = self.description
-        icon_kind: Union[Unset, str] = UNSET
-        if not isinstance(self.icon_kind, Unset):
-            icon_kind = self.icon_kind.value
-
-        icon_name_or_emoji = self.icon_name_or_emoji
         color_name: Union[Unset, str] = UNSET
         if not isinstance(self.color_name, Unset):
             color_name = self.color_name.value
 
+        description = self.description
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "duid": duid,
             }
         )
-        if hidden is not UNSET:
-            field_dict["hidden"] = hidden
-        if public is not UNSET:
-            field_dict["public"] = public
+        if property_duid is not UNSET:
+            field_dict["propertyDuid"] = property_duid
+        if kind is not UNSET:
+            field_dict["kind"] = kind
+        if locked is not UNSET:
+            field_dict["locked"] = locked
         if order is not UNSET:
             field_dict["order"] = order
         if title is not UNSET:
             field_dict["title"] = title
-        if description is not UNSET:
-            field_dict["description"] = description
-        if icon_kind is not UNSET:
-            field_dict["iconKind"] = icon_kind
-        if icon_name_or_emoji is not UNSET:
-            field_dict["iconNameOrEmoji"] = icon_name_or_emoji
         if color_name is not UNSET:
             field_dict["colorName"] = color_name
+        if description is not UNSET:
+            field_dict["description"] = description
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         duid = d.pop("duid")
 
-        hidden = d.pop("hidden", UNSET)
+        property_duid = d.pop("propertyDuid", UNSET)
+
+        _kind = d.pop("kind", UNSET)
+        kind: Union[Unset, StatusKind]
+        if isinstance(_kind, Unset):
+            kind = UNSET
+        else:
+            kind = StatusKind(_kind)
 
-        public = d.pop("public", UNSET)
+        locked = d.pop("locked", UNSET)
 
         order = d.pop("order", UNSET)
 
         title = d.pop("title", UNSET)
 
-        description = d.pop("description", UNSET)
-
-        _icon_kind = d.pop("iconKind", UNSET)
-        icon_kind: Union[Unset, IconKind]
-        if isinstance(_icon_kind, Unset):
-            icon_kind = UNSET
-        else:
-            icon_kind = IconKind(_icon_kind)
-
-        icon_name_or_emoji = d.pop("iconNameOrEmoji", UNSET)
-
         _color_name = d.pop("colorName", UNSET)
         color_name: Union[Unset, ColorName]
         if isinstance(_color_name, Unset):
             color_name = UNSET
         else:
             color_name = ColorName(_color_name)
 
-        form_update = cls(
+        description = d.pop("description", UNSET)
+
+        status_update = cls(
             duid=duid,
-            hidden=hidden,
-            public=public,
+            property_duid=property_duid,
+            kind=kind,
+            locked=locked,
             order=order,
             title=title,
-            description=description,
-            icon_kind=icon_kind,
-            icon_name_or_emoji=icon_name_or_emoji,
             color_name=color_name,
+            description=description,
         )
 
-        form_update.additional_properties = d
-        return form_update
+        status_update.additional_properties = d
+        return status_update
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart_tools-0.5.6/dart/generated/models/github_integration.py` & `dart_tools-0.5.7/dart/generated/models/github_integration.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/google_data.py` & `dart_tools-0.5.7/dart/generated/models/google_data.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/layout.py` & `dart_tools-0.5.7/dart/generated/models/layout.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/layout_config.py` & `dart_tools-0.5.7/dart/generated/models/layout_config.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/layout_create.py` & `dart_tools-0.5.7/dart/generated/models/layout_create.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/layout_kind_config_map.py` & `dart_tools-0.5.7/dart/generated/models/layout_kind_config_map.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/layout_update.py` & `dart_tools-0.5.7/dart/generated/models/layout_update.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/models_response.py` & `dart_tools-0.5.7/dart/generated/models/models_response.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/notification.py` & `dart_tools-0.5.7/dart/generated/models/notification.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/notification_update.py` & `dart_tools-0.5.7/dart/generated/models/notification_update.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/notion_integration.py` & `dart_tools-0.5.7/dart/generated/models/notion_integration.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/operation.py` & `dart_tools-0.5.7/dart/generated/models/operation.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/operation_model_kind.py` & `dart_tools-0.5.7/dart/generated/models/operation_model_kind.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/option.py` & `dart_tools-0.5.7/dart/generated/models/option.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/option_create.py` & `dart_tools-0.5.7/dart/generated/models/option_create.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/option_update.py` & `dart_tools-0.5.7/dart/generated/models/option_update.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/paginated_attachment_list.py` & `dart_tools-0.5.7/dart/generated/models/paginated_attachment_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,75 +12,75 @@
 T = TypeVar("T", bound="PaginatedAttachmentList")
 
 
 @_attrs_define
 class PaginatedAttachmentList:
     """
     Attributes:
-        count (Union[Unset, int]):  Example: 123.
+        count (int):  Example: 123.
+        results (List['Attachment']):
         next_ (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=400&limit=100.
         previous (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=200&limit=100.
-        results (Union[Unset, List['Attachment']]):
     """
 
-    count: Union[Unset, int] = UNSET
+    count: int
+    results: List["Attachment"]
     next_: Union[Unset, None, str] = UNSET
     previous: Union[Unset, None, str] = UNSET
-    results: Union[Unset, List["Attachment"]] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         count = self.count
+        results = []
+        for results_item_data in self.results:
+            results_item = results_item_data.to_dict()
+
+            results.append(results_item)
+
         next_ = self.next_
         previous = self.previous
-        results: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.results, Unset):
-            results = []
-            for results_item_data in self.results:
-                results_item = results_item_data.to_dict()
-
-                results.append(results_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if count is not UNSET:
-            field_dict["count"] = count
+        field_dict.update(
+            {
+                "count": count,
+                "results": results,
+            }
+        )
         if next_ is not UNSET:
             field_dict["next"] = next_
         if previous is not UNSET:
             field_dict["previous"] = previous
-        if results is not UNSET:
-            field_dict["results"] = results
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.attachment import Attachment
 
         d = src_dict.copy()
-        count = d.pop("count", UNSET)
-
-        next_ = d.pop("next", UNSET)
-
-        previous = d.pop("previous", UNSET)
+        count = d.pop("count")
 
         results = []
-        _results = d.pop("results", UNSET)
-        for results_item_data in _results or []:
+        _results = d.pop("results")
+        for results_item_data in _results:
             results_item = Attachment.from_dict(results_item_data)
 
             results.append(results_item)
 
+        next_ = d.pop("next", UNSET)
+
+        previous = d.pop("previous", UNSET)
+
         paginated_attachment_list = cls(
             count=count,
+            results=results,
             next_=next_,
             previous=previous,
-            results=results,
         )
 
         paginated_attachment_list.additional_properties = d
         return paginated_attachment_list
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `dart_tools-0.5.6/dart/generated/models/paginated_comment_list.py` & `dart_tools-0.5.7/dart/generated/models/paginated_comment_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,75 +12,75 @@
 T = TypeVar("T", bound="PaginatedCommentList")
 
 
 @_attrs_define
 class PaginatedCommentList:
     """
     Attributes:
-        count (Union[Unset, int]):  Example: 123.
+        count (int):  Example: 123.
+        results (List['Comment']):
         next_ (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=400&limit=100.
         previous (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=200&limit=100.
-        results (Union[Unset, List['Comment']]):
     """
 
-    count: Union[Unset, int] = UNSET
+    count: int
+    results: List["Comment"]
     next_: Union[Unset, None, str] = UNSET
     previous: Union[Unset, None, str] = UNSET
-    results: Union[Unset, List["Comment"]] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         count = self.count
+        results = []
+        for results_item_data in self.results:
+            results_item = results_item_data.to_dict()
+
+            results.append(results_item)
+
         next_ = self.next_
         previous = self.previous
-        results: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.results, Unset):
-            results = []
-            for results_item_data in self.results:
-                results_item = results_item_data.to_dict()
-
-                results.append(results_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if count is not UNSET:
-            field_dict["count"] = count
+        field_dict.update(
+            {
+                "count": count,
+                "results": results,
+            }
+        )
         if next_ is not UNSET:
             field_dict["next"] = next_
         if previous is not UNSET:
             field_dict["previous"] = previous
-        if results is not UNSET:
-            field_dict["results"] = results
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.comment import Comment
 
         d = src_dict.copy()
-        count = d.pop("count", UNSET)
-
-        next_ = d.pop("next", UNSET)
-
-        previous = d.pop("previous", UNSET)
+        count = d.pop("count")
 
         results = []
-        _results = d.pop("results", UNSET)
-        for results_item_data in _results or []:
+        _results = d.pop("results")
+        for results_item_data in _results:
             results_item = Comment.from_dict(results_item_data)
 
             results.append(results_item)
 
+        next_ = d.pop("next", UNSET)
+
+        previous = d.pop("previous", UNSET)
+
         paginated_comment_list = cls(
             count=count,
+            results=results,
             next_=next_,
             previous=previous,
-            results=results,
         )
 
         paginated_comment_list.additional_properties = d
         return paginated_comment_list
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `dart_tools-0.5.6/dart/generated/models/paginated_comment_reaction_list.py` & `dart_tools-0.5.7/dart/generated/models/paginated_option_list.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,89 +2,89 @@
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.comment_reaction import CommentReaction
+    from ..models.option import Option
 
 
-T = TypeVar("T", bound="PaginatedCommentReactionList")
+T = TypeVar("T", bound="PaginatedOptionList")
 
 
 @_attrs_define
-class PaginatedCommentReactionList:
+class PaginatedOptionList:
     """
     Attributes:
-        count (Union[Unset, int]):  Example: 123.
+        count (int):  Example: 123.
+        results (List['Option']):
         next_ (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=400&limit=100.
         previous (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=200&limit=100.
-        results (Union[Unset, List['CommentReaction']]):
     """
 
-    count: Union[Unset, int] = UNSET
+    count: int
+    results: List["Option"]
     next_: Union[Unset, None, str] = UNSET
     previous: Union[Unset, None, str] = UNSET
-    results: Union[Unset, List["CommentReaction"]] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         count = self.count
+        results = []
+        for results_item_data in self.results:
+            results_item = results_item_data.to_dict()
+
+            results.append(results_item)
+
         next_ = self.next_
         previous = self.previous
-        results: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.results, Unset):
-            results = []
-            for results_item_data in self.results:
-                results_item = results_item_data.to_dict()
-
-                results.append(results_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if count is not UNSET:
-            field_dict["count"] = count
+        field_dict.update(
+            {
+                "count": count,
+                "results": results,
+            }
+        )
         if next_ is not UNSET:
             field_dict["next"] = next_
         if previous is not UNSET:
             field_dict["previous"] = previous
-        if results is not UNSET:
-            field_dict["results"] = results
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.comment_reaction import CommentReaction
+        from ..models.option import Option
 
         d = src_dict.copy()
-        count = d.pop("count", UNSET)
-
-        next_ = d.pop("next", UNSET)
-
-        previous = d.pop("previous", UNSET)
+        count = d.pop("count")
 
         results = []
-        _results = d.pop("results", UNSET)
-        for results_item_data in _results or []:
-            results_item = CommentReaction.from_dict(results_item_data)
+        _results = d.pop("results")
+        for results_item_data in _results:
+            results_item = Option.from_dict(results_item_data)
 
             results.append(results_item)
 
-        paginated_comment_reaction_list = cls(
+        next_ = d.pop("next", UNSET)
+
+        previous = d.pop("previous", UNSET)
+
+        paginated_option_list = cls(
             count=count,
+            results=results,
             next_=next_,
             previous=previous,
-            results=results,
         )
 
-        paginated_comment_reaction_list.additional_properties = d
-        return paginated_comment_reaction_list
+        paginated_option_list.additional_properties = d
+        return paginated_option_list
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart_tools-0.5.6/dart/generated/models/paginated_dartboard_list.py` & `dart_tools-0.5.7/dart/generated/models/paginated_folder_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,89 +2,89 @@
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.dartboard import Dartboard
+    from ..models.folder import Folder
 
 
-T = TypeVar("T", bound="PaginatedDartboardList")
+T = TypeVar("T", bound="PaginatedFolderList")
 
 
 @_attrs_define
-class PaginatedDartboardList:
+class PaginatedFolderList:
     """
     Attributes:
-        count (Union[Unset, int]):  Example: 123.
+        count (int):  Example: 123.
+        results (List['Folder']):
         next_ (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=400&limit=100.
         previous (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=200&limit=100.
-        results (Union[Unset, List['Dartboard']]):
     """
 
-    count: Union[Unset, int] = UNSET
+    count: int
+    results: List["Folder"]
     next_: Union[Unset, None, str] = UNSET
     previous: Union[Unset, None, str] = UNSET
-    results: Union[Unset, List["Dartboard"]] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         count = self.count
+        results = []
+        for results_item_data in self.results:
+            results_item = results_item_data.to_dict()
+
+            results.append(results_item)
+
         next_ = self.next_
         previous = self.previous
-        results: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.results, Unset):
-            results = []
-            for results_item_data in self.results:
-                results_item = results_item_data.to_dict()
-
-                results.append(results_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if count is not UNSET:
-            field_dict["count"] = count
+        field_dict.update(
+            {
+                "count": count,
+                "results": results,
+            }
+        )
         if next_ is not UNSET:
             field_dict["next"] = next_
         if previous is not UNSET:
             field_dict["previous"] = previous
-        if results is not UNSET:
-            field_dict["results"] = results
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.dartboard import Dartboard
+        from ..models.folder import Folder
 
         d = src_dict.copy()
-        count = d.pop("count", UNSET)
-
-        next_ = d.pop("next", UNSET)
-
-        previous = d.pop("previous", UNSET)
+        count = d.pop("count")
 
         results = []
-        _results = d.pop("results", UNSET)
-        for results_item_data in _results or []:
-            results_item = Dartboard.from_dict(results_item_data)
+        _results = d.pop("results")
+        for results_item_data in _results:
+            results_item = Folder.from_dict(results_item_data)
 
             results.append(results_item)
 
-        paginated_dartboard_list = cls(
+        next_ = d.pop("next", UNSET)
+
+        previous = d.pop("previous", UNSET)
+
+        paginated_folder_list = cls(
             count=count,
+            results=results,
             next_=next_,
             previous=previous,
-            results=results,
         )
 
-        paginated_dartboard_list.additional_properties = d
-        return paginated_dartboard_list
+        paginated_folder_list.additional_properties = d
+        return paginated_folder_list
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart_tools-0.5.6/dart/generated/models/paginated_doc_list.py` & `dart_tools-0.5.7/dart/generated/models/paginated_status_list.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,89 +2,89 @@
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.doc import Doc
+    from ..models.status import Status
 
 
-T = TypeVar("T", bound="PaginatedDocList")
+T = TypeVar("T", bound="PaginatedStatusList")
 
 
 @_attrs_define
-class PaginatedDocList:
+class PaginatedStatusList:
     """
     Attributes:
-        count (Union[Unset, int]):  Example: 123.
+        count (int):  Example: 123.
+        results (List['Status']):
         next_ (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=400&limit=100.
         previous (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=200&limit=100.
-        results (Union[Unset, List['Doc']]):
     """
 
-    count: Union[Unset, int] = UNSET
+    count: int
+    results: List["Status"]
     next_: Union[Unset, None, str] = UNSET
     previous: Union[Unset, None, str] = UNSET
-    results: Union[Unset, List["Doc"]] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         count = self.count
+        results = []
+        for results_item_data in self.results:
+            results_item = results_item_data.to_dict()
+
+            results.append(results_item)
+
         next_ = self.next_
         previous = self.previous
-        results: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.results, Unset):
-            results = []
-            for results_item_data in self.results:
-                results_item = results_item_data.to_dict()
-
-                results.append(results_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if count is not UNSET:
-            field_dict["count"] = count
+        field_dict.update(
+            {
+                "count": count,
+                "results": results,
+            }
+        )
         if next_ is not UNSET:
             field_dict["next"] = next_
         if previous is not UNSET:
             field_dict["previous"] = previous
-        if results is not UNSET:
-            field_dict["results"] = results
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.doc import Doc
+        from ..models.status import Status
 
         d = src_dict.copy()
-        count = d.pop("count", UNSET)
-
-        next_ = d.pop("next", UNSET)
-
-        previous = d.pop("previous", UNSET)
+        count = d.pop("count")
 
         results = []
-        _results = d.pop("results", UNSET)
-        for results_item_data in _results or []:
-            results_item = Doc.from_dict(results_item_data)
+        _results = d.pop("results")
+        for results_item_data in _results:
+            results_item = Status.from_dict(results_item_data)
 
             results.append(results_item)
 
-        paginated_doc_list = cls(
+        next_ = d.pop("next", UNSET)
+
+        previous = d.pop("previous", UNSET)
+
+        paginated_status_list = cls(
             count=count,
+            results=results,
             next_=next_,
             previous=previous,
-            results=results,
         )
 
-        paginated_doc_list.additional_properties = d
-        return paginated_doc_list
+        paginated_status_list.additional_properties = d
+        return paginated_status_list
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart_tools-0.5.6/dart/generated/models/paginated_folder_list.py` & `dart_tools-0.5.7/dart/generated/models/paginated_property_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,89 +2,89 @@
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.folder import Folder
+    from ..models.property_ import Property
 
 
-T = TypeVar("T", bound="PaginatedFolderList")
+T = TypeVar("T", bound="PaginatedPropertyList")
 
 
 @_attrs_define
-class PaginatedFolderList:
+class PaginatedPropertyList:
     """
     Attributes:
-        count (Union[Unset, int]):  Example: 123.
+        count (int):  Example: 123.
+        results (List['Property']):
         next_ (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=400&limit=100.
         previous (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=200&limit=100.
-        results (Union[Unset, List['Folder']]):
     """
 
-    count: Union[Unset, int] = UNSET
+    count: int
+    results: List["Property"]
     next_: Union[Unset, None, str] = UNSET
     previous: Union[Unset, None, str] = UNSET
-    results: Union[Unset, List["Folder"]] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         count = self.count
+        results = []
+        for results_item_data in self.results:
+            results_item = results_item_data.to_dict()
+
+            results.append(results_item)
+
         next_ = self.next_
         previous = self.previous
-        results: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.results, Unset):
-            results = []
-            for results_item_data in self.results:
-                results_item = results_item_data.to_dict()
-
-                results.append(results_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if count is not UNSET:
-            field_dict["count"] = count
+        field_dict.update(
+            {
+                "count": count,
+                "results": results,
+            }
+        )
         if next_ is not UNSET:
             field_dict["next"] = next_
         if previous is not UNSET:
             field_dict["previous"] = previous
-        if results is not UNSET:
-            field_dict["results"] = results
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.folder import Folder
+        from ..models.property_ import Property
 
         d = src_dict.copy()
-        count = d.pop("count", UNSET)
-
-        next_ = d.pop("next", UNSET)
-
-        previous = d.pop("previous", UNSET)
+        count = d.pop("count")
 
         results = []
-        _results = d.pop("results", UNSET)
-        for results_item_data in _results or []:
-            results_item = Folder.from_dict(results_item_data)
+        _results = d.pop("results")
+        for results_item_data in _results:
+            results_item = Property.from_dict(results_item_data)
 
             results.append(results_item)
 
-        paginated_folder_list = cls(
+        next_ = d.pop("next", UNSET)
+
+        previous = d.pop("previous", UNSET)
+
+        paginated_property_list = cls(
             count=count,
+            results=results,
             next_=next_,
             previous=previous,
-            results=results,
         )
 
-        paginated_folder_list.additional_properties = d
-        return paginated_folder_list
+        paginated_property_list.additional_properties = d
+        return paginated_property_list
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart_tools-0.5.6/dart/generated/models/paginated_form_field_list.py` & `dart_tools-0.5.7/dart/generated/models/paginated_space_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,89 +2,89 @@
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.form_field import FormField
+    from ..models.space import Space
 
 
-T = TypeVar("T", bound="PaginatedFormFieldList")
+T = TypeVar("T", bound="PaginatedSpaceList")
 
 
 @_attrs_define
-class PaginatedFormFieldList:
+class PaginatedSpaceList:
     """
     Attributes:
-        count (Union[Unset, int]):  Example: 123.
+        count (int):  Example: 123.
+        results (List['Space']):
         next_ (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=400&limit=100.
         previous (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=200&limit=100.
-        results (Union[Unset, List['FormField']]):
     """
 
-    count: Union[Unset, int] = UNSET
+    count: int
+    results: List["Space"]
     next_: Union[Unset, None, str] = UNSET
     previous: Union[Unset, None, str] = UNSET
-    results: Union[Unset, List["FormField"]] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         count = self.count
+        results = []
+        for results_item_data in self.results:
+            results_item = results_item_data.to_dict()
+
+            results.append(results_item)
+
         next_ = self.next_
         previous = self.previous
-        results: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.results, Unset):
-            results = []
-            for results_item_data in self.results:
-                results_item = results_item_data.to_dict()
-
-                results.append(results_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if count is not UNSET:
-            field_dict["count"] = count
+        field_dict.update(
+            {
+                "count": count,
+                "results": results,
+            }
+        )
         if next_ is not UNSET:
             field_dict["next"] = next_
         if previous is not UNSET:
             field_dict["previous"] = previous
-        if results is not UNSET:
-            field_dict["results"] = results
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.form_field import FormField
+        from ..models.space import Space
 
         d = src_dict.copy()
-        count = d.pop("count", UNSET)
-
-        next_ = d.pop("next", UNSET)
-
-        previous = d.pop("previous", UNSET)
+        count = d.pop("count")
 
         results = []
-        _results = d.pop("results", UNSET)
-        for results_item_data in _results or []:
-            results_item = FormField.from_dict(results_item_data)
+        _results = d.pop("results")
+        for results_item_data in _results:
+            results_item = Space.from_dict(results_item_data)
 
             results.append(results_item)
 
-        paginated_form_field_list = cls(
+        next_ = d.pop("next", UNSET)
+
+        previous = d.pop("previous", UNSET)
+
+        paginated_space_list = cls(
             count=count,
+            results=results,
             next_=next_,
             previous=previous,
-            results=results,
         )
 
-        paginated_form_field_list.additional_properties = d
-        return paginated_form_field_list
+        paginated_space_list.additional_properties = d
+        return paginated_space_list
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart_tools-0.5.6/dart/generated/models/paginated_form_list.py` & `dart_tools-0.5.7/dart/generated/models/paginated_relationship_list.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,89 +2,89 @@
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.form import Form
+    from ..models.relationship import Relationship
 
 
-T = TypeVar("T", bound="PaginatedFormList")
+T = TypeVar("T", bound="PaginatedRelationshipList")
 
 
 @_attrs_define
-class PaginatedFormList:
+class PaginatedRelationshipList:
     """
     Attributes:
-        count (Union[Unset, int]):  Example: 123.
+        count (int):  Example: 123.
+        results (List['Relationship']):
         next_ (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=400&limit=100.
         previous (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=200&limit=100.
-        results (Union[Unset, List['Form']]):
     """
 
-    count: Union[Unset, int] = UNSET
+    count: int
+    results: List["Relationship"]
     next_: Union[Unset, None, str] = UNSET
     previous: Union[Unset, None, str] = UNSET
-    results: Union[Unset, List["Form"]] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         count = self.count
+        results = []
+        for results_item_data in self.results:
+            results_item = results_item_data.to_dict()
+
+            results.append(results_item)
+
         next_ = self.next_
         previous = self.previous
-        results: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.results, Unset):
-            results = []
-            for results_item_data in self.results:
-                results_item = results_item_data.to_dict()
-
-                results.append(results_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if count is not UNSET:
-            field_dict["count"] = count
+        field_dict.update(
+            {
+                "count": count,
+                "results": results,
+            }
+        )
         if next_ is not UNSET:
             field_dict["next"] = next_
         if previous is not UNSET:
             field_dict["previous"] = previous
-        if results is not UNSET:
-            field_dict["results"] = results
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.form import Form
+        from ..models.relationship import Relationship
 
         d = src_dict.copy()
-        count = d.pop("count", UNSET)
-
-        next_ = d.pop("next", UNSET)
-
-        previous = d.pop("previous", UNSET)
+        count = d.pop("count")
 
         results = []
-        _results = d.pop("results", UNSET)
-        for results_item_data in _results or []:
-            results_item = Form.from_dict(results_item_data)
+        _results = d.pop("results")
+        for results_item_data in _results:
+            results_item = Relationship.from_dict(results_item_data)
 
             results.append(results_item)
 
-        paginated_form_list = cls(
+        next_ = d.pop("next", UNSET)
+
+        previous = d.pop("previous", UNSET)
+
+        paginated_relationship_list = cls(
             count=count,
+            results=results,
             next_=next_,
             previous=previous,
-            results=results,
         )
 
-        paginated_form_list.additional_properties = d
-        return paginated_form_list
+        paginated_relationship_list.additional_properties = d
+        return paginated_relationship_list
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart_tools-0.5.6/dart/generated/models/paginated_layout_list.py` & `dart_tools-0.5.7/dart/generated/models/paginated_layout_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,75 +12,75 @@
 T = TypeVar("T", bound="PaginatedLayoutList")
 
 
 @_attrs_define
 class PaginatedLayoutList:
     """
     Attributes:
-        count (Union[Unset, int]):  Example: 123.
+        count (int):  Example: 123.
+        results (List['Layout']):
         next_ (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=400&limit=100.
         previous (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=200&limit=100.
-        results (Union[Unset, List['Layout']]):
     """
 
-    count: Union[Unset, int] = UNSET
+    count: int
+    results: List["Layout"]
     next_: Union[Unset, None, str] = UNSET
     previous: Union[Unset, None, str] = UNSET
-    results: Union[Unset, List["Layout"]] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         count = self.count
+        results = []
+        for results_item_data in self.results:
+            results_item = results_item_data.to_dict()
+
+            results.append(results_item)
+
         next_ = self.next_
         previous = self.previous
-        results: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.results, Unset):
-            results = []
-            for results_item_data in self.results:
-                results_item = results_item_data.to_dict()
-
-                results.append(results_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if count is not UNSET:
-            field_dict["count"] = count
+        field_dict.update(
+            {
+                "count": count,
+                "results": results,
+            }
+        )
         if next_ is not UNSET:
             field_dict["next"] = next_
         if previous is not UNSET:
             field_dict["previous"] = previous
-        if results is not UNSET:
-            field_dict["results"] = results
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.layout import Layout
 
         d = src_dict.copy()
-        count = d.pop("count", UNSET)
-
-        next_ = d.pop("next", UNSET)
-
-        previous = d.pop("previous", UNSET)
+        count = d.pop("count")
 
         results = []
-        _results = d.pop("results", UNSET)
-        for results_item_data in _results or []:
+        _results = d.pop("results")
+        for results_item_data in _results:
             results_item = Layout.from_dict(results_item_data)
 
             results.append(results_item)
 
+        next_ = d.pop("next", UNSET)
+
+        previous = d.pop("previous", UNSET)
+
         paginated_layout_list = cls(
             count=count,
+            results=results,
             next_=next_,
             previous=previous,
-            results=results,
         )
 
         paginated_layout_list.additional_properties = d
         return paginated_layout_list
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `dart_tools-0.5.6/dart/generated/models/paginated_option_list.py` & `dart_tools-0.5.7/dart/generated/models/paginated_view_list.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,89 +2,89 @@
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.option import Option
+    from ..models.view import View
 
 
-T = TypeVar("T", bound="PaginatedOptionList")
+T = TypeVar("T", bound="PaginatedViewList")
 
 
 @_attrs_define
-class PaginatedOptionList:
+class PaginatedViewList:
     """
     Attributes:
-        count (Union[Unset, int]):  Example: 123.
+        count (int):  Example: 123.
+        results (List['View']):
         next_ (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=400&limit=100.
         previous (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=200&limit=100.
-        results (Union[Unset, List['Option']]):
     """
 
-    count: Union[Unset, int] = UNSET
+    count: int
+    results: List["View"]
     next_: Union[Unset, None, str] = UNSET
     previous: Union[Unset, None, str] = UNSET
-    results: Union[Unset, List["Option"]] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         count = self.count
+        results = []
+        for results_item_data in self.results:
+            results_item = results_item_data.to_dict()
+
+            results.append(results_item)
+
         next_ = self.next_
         previous = self.previous
-        results: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.results, Unset):
-            results = []
-            for results_item_data in self.results:
-                results_item = results_item_data.to_dict()
-
-                results.append(results_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if count is not UNSET:
-            field_dict["count"] = count
+        field_dict.update(
+            {
+                "count": count,
+                "results": results,
+            }
+        )
         if next_ is not UNSET:
             field_dict["next"] = next_
         if previous is not UNSET:
             field_dict["previous"] = previous
-        if results is not UNSET:
-            field_dict["results"] = results
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.option import Option
+        from ..models.view import View
 
         d = src_dict.copy()
-        count = d.pop("count", UNSET)
-
-        next_ = d.pop("next", UNSET)
-
-        previous = d.pop("previous", UNSET)
+        count = d.pop("count")
 
         results = []
-        _results = d.pop("results", UNSET)
-        for results_item_data in _results or []:
-            results_item = Option.from_dict(results_item_data)
+        _results = d.pop("results")
+        for results_item_data in _results:
+            results_item = View.from_dict(results_item_data)
 
             results.append(results_item)
 
-        paginated_option_list = cls(
+        next_ = d.pop("next", UNSET)
+
+        previous = d.pop("previous", UNSET)
+
+        paginated_view_list = cls(
             count=count,
+            results=results,
             next_=next_,
             previous=previous,
-            results=results,
         )
 
-        paginated_option_list.additional_properties = d
-        return paginated_option_list
+        paginated_view_list.additional_properties = d
+        return paginated_view_list
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart_tools-0.5.6/dart/generated/models/paginated_property_list.py` & `dart_tools-0.5.7/dart/generated/models/paginated_relationship_kind_list.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,89 +2,89 @@
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.property_ import Property
+    from ..models.relationship_kind import RelationshipKind
 
 
-T = TypeVar("T", bound="PaginatedPropertyList")
+T = TypeVar("T", bound="PaginatedRelationshipKindList")
 
 
 @_attrs_define
-class PaginatedPropertyList:
+class PaginatedRelationshipKindList:
     """
     Attributes:
-        count (Union[Unset, int]):  Example: 123.
+        count (int):  Example: 123.
+        results (List['RelationshipKind']):
         next_ (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=400&limit=100.
         previous (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=200&limit=100.
-        results (Union[Unset, List['Property']]):
     """
 
-    count: Union[Unset, int] = UNSET
+    count: int
+    results: List["RelationshipKind"]
     next_: Union[Unset, None, str] = UNSET
     previous: Union[Unset, None, str] = UNSET
-    results: Union[Unset, List["Property"]] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         count = self.count
+        results = []
+        for results_item_data in self.results:
+            results_item = results_item_data.to_dict()
+
+            results.append(results_item)
+
         next_ = self.next_
         previous = self.previous
-        results: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.results, Unset):
-            results = []
-            for results_item_data in self.results:
-                results_item = results_item_data.to_dict()
-
-                results.append(results_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if count is not UNSET:
-            field_dict["count"] = count
+        field_dict.update(
+            {
+                "count": count,
+                "results": results,
+            }
+        )
         if next_ is not UNSET:
             field_dict["next"] = next_
         if previous is not UNSET:
             field_dict["previous"] = previous
-        if results is not UNSET:
-            field_dict["results"] = results
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.property_ import Property
+        from ..models.relationship_kind import RelationshipKind
 
         d = src_dict.copy()
-        count = d.pop("count", UNSET)
-
-        next_ = d.pop("next", UNSET)
-
-        previous = d.pop("previous", UNSET)
+        count = d.pop("count")
 
         results = []
-        _results = d.pop("results", UNSET)
-        for results_item_data in _results or []:
-            results_item = Property.from_dict(results_item_data)
+        _results = d.pop("results")
+        for results_item_data in _results:
+            results_item = RelationshipKind.from_dict(results_item_data)
 
             results.append(results_item)
 
-        paginated_property_list = cls(
+        next_ = d.pop("next", UNSET)
+
+        previous = d.pop("previous", UNSET)
+
+        paginated_relationship_kind_list = cls(
             count=count,
+            results=results,
             next_=next_,
             previous=previous,
-            results=results,
         )
 
-        paginated_property_list.additional_properties = d
-        return paginated_property_list
+        paginated_relationship_kind_list.additional_properties = d
+        return paginated_relationship_kind_list
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart_tools-0.5.6/dart/generated/models/paginated_relationship_kind_list.py` & `dart_tools-0.5.7/dart/generated/models/paginated_form_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,89 +2,89 @@
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.relationship_kind import RelationshipKind
+    from ..models.form import Form
 
 
-T = TypeVar("T", bound="PaginatedRelationshipKindList")
+T = TypeVar("T", bound="PaginatedFormList")
 
 
 @_attrs_define
-class PaginatedRelationshipKindList:
+class PaginatedFormList:
     """
     Attributes:
-        count (Union[Unset, int]):  Example: 123.
+        count (int):  Example: 123.
+        results (List['Form']):
         next_ (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=400&limit=100.
         previous (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=200&limit=100.
-        results (Union[Unset, List['RelationshipKind']]):
     """
 
-    count: Union[Unset, int] = UNSET
+    count: int
+    results: List["Form"]
     next_: Union[Unset, None, str] = UNSET
     previous: Union[Unset, None, str] = UNSET
-    results: Union[Unset, List["RelationshipKind"]] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         count = self.count
+        results = []
+        for results_item_data in self.results:
+            results_item = results_item_data.to_dict()
+
+            results.append(results_item)
+
         next_ = self.next_
         previous = self.previous
-        results: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.results, Unset):
-            results = []
-            for results_item_data in self.results:
-                results_item = results_item_data.to_dict()
-
-                results.append(results_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if count is not UNSET:
-            field_dict["count"] = count
+        field_dict.update(
+            {
+                "count": count,
+                "results": results,
+            }
+        )
         if next_ is not UNSET:
             field_dict["next"] = next_
         if previous is not UNSET:
             field_dict["previous"] = previous
-        if results is not UNSET:
-            field_dict["results"] = results
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.relationship_kind import RelationshipKind
+        from ..models.form import Form
 
         d = src_dict.copy()
-        count = d.pop("count", UNSET)
-
-        next_ = d.pop("next", UNSET)
-
-        previous = d.pop("previous", UNSET)
+        count = d.pop("count")
 
         results = []
-        _results = d.pop("results", UNSET)
-        for results_item_data in _results or []:
-            results_item = RelationshipKind.from_dict(results_item_data)
+        _results = d.pop("results")
+        for results_item_data in _results:
+            results_item = Form.from_dict(results_item_data)
 
             results.append(results_item)
 
-        paginated_relationship_kind_list = cls(
+        next_ = d.pop("next", UNSET)
+
+        previous = d.pop("previous", UNSET)
+
+        paginated_form_list = cls(
             count=count,
+            results=results,
             next_=next_,
             previous=previous,
-            results=results,
         )
 
-        paginated_relationship_kind_list.additional_properties = d
-        return paginated_relationship_kind_list
+        paginated_form_list.additional_properties = d
+        return paginated_form_list
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart_tools-0.5.6/dart/generated/models/paginated_relationship_list.py` & `dart_tools-0.5.7/dart/generated/models/paginated_user_dartboard_layout_list.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,89 +2,89 @@
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.relationship import Relationship
+    from ..models.user_dartboard_layout import UserDartboardLayout
 
 
-T = TypeVar("T", bound="PaginatedRelationshipList")
+T = TypeVar("T", bound="PaginatedUserDartboardLayoutList")
 
 
 @_attrs_define
-class PaginatedRelationshipList:
+class PaginatedUserDartboardLayoutList:
     """
     Attributes:
-        count (Union[Unset, int]):  Example: 123.
+        count (int):  Example: 123.
+        results (List['UserDartboardLayout']):
         next_ (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=400&limit=100.
         previous (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=200&limit=100.
-        results (Union[Unset, List['Relationship']]):
     """
 
-    count: Union[Unset, int] = UNSET
+    count: int
+    results: List["UserDartboardLayout"]
     next_: Union[Unset, None, str] = UNSET
     previous: Union[Unset, None, str] = UNSET
-    results: Union[Unset, List["Relationship"]] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         count = self.count
+        results = []
+        for results_item_data in self.results:
+            results_item = results_item_data.to_dict()
+
+            results.append(results_item)
+
         next_ = self.next_
         previous = self.previous
-        results: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.results, Unset):
-            results = []
-            for results_item_data in self.results:
-                results_item = results_item_data.to_dict()
-
-                results.append(results_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if count is not UNSET:
-            field_dict["count"] = count
+        field_dict.update(
+            {
+                "count": count,
+                "results": results,
+            }
+        )
         if next_ is not UNSET:
             field_dict["next"] = next_
         if previous is not UNSET:
             field_dict["previous"] = previous
-        if results is not UNSET:
-            field_dict["results"] = results
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.relationship import Relationship
+        from ..models.user_dartboard_layout import UserDartboardLayout
 
         d = src_dict.copy()
-        count = d.pop("count", UNSET)
-
-        next_ = d.pop("next", UNSET)
-
-        previous = d.pop("previous", UNSET)
+        count = d.pop("count")
 
         results = []
-        _results = d.pop("results", UNSET)
-        for results_item_data in _results or []:
-            results_item = Relationship.from_dict(results_item_data)
+        _results = d.pop("results")
+        for results_item_data in _results:
+            results_item = UserDartboardLayout.from_dict(results_item_data)
 
             results.append(results_item)
 
-        paginated_relationship_list = cls(
+        next_ = d.pop("next", UNSET)
+
+        previous = d.pop("previous", UNSET)
+
+        paginated_user_dartboard_layout_list = cls(
             count=count,
+            results=results,
             next_=next_,
             previous=previous,
-            results=results,
         )
 
-        paginated_relationship_list.additional_properties = d
-        return paginated_relationship_list
+        paginated_user_dartboard_layout_list.additional_properties = d
+        return paginated_user_dartboard_layout_list
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart_tools-0.5.6/dart/generated/models/paginated_space_list.py` & `dart_tools-0.5.7/dart/generated/models/paginated_task_list.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,89 +2,89 @@
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.space import Space
+    from ..models.task import Task
 
 
-T = TypeVar("T", bound="PaginatedSpaceList")
+T = TypeVar("T", bound="PaginatedTaskList")
 
 
 @_attrs_define
-class PaginatedSpaceList:
+class PaginatedTaskList:
     """
     Attributes:
-        count (Union[Unset, int]):  Example: 123.
+        count (int):  Example: 123.
+        results (List['Task']):
         next_ (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=400&limit=100.
         previous (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=200&limit=100.
-        results (Union[Unset, List['Space']]):
     """
 
-    count: Union[Unset, int] = UNSET
+    count: int
+    results: List["Task"]
     next_: Union[Unset, None, str] = UNSET
     previous: Union[Unset, None, str] = UNSET
-    results: Union[Unset, List["Space"]] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         count = self.count
+        results = []
+        for results_item_data in self.results:
+            results_item = results_item_data.to_dict()
+
+            results.append(results_item)
+
         next_ = self.next_
         previous = self.previous
-        results: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.results, Unset):
-            results = []
-            for results_item_data in self.results:
-                results_item = results_item_data.to_dict()
-
-                results.append(results_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if count is not UNSET:
-            field_dict["count"] = count
+        field_dict.update(
+            {
+                "count": count,
+                "results": results,
+            }
+        )
         if next_ is not UNSET:
             field_dict["next"] = next_
         if previous is not UNSET:
             field_dict["previous"] = previous
-        if results is not UNSET:
-            field_dict["results"] = results
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.space import Space
+        from ..models.task import Task
 
         d = src_dict.copy()
-        count = d.pop("count", UNSET)
-
-        next_ = d.pop("next", UNSET)
-
-        previous = d.pop("previous", UNSET)
+        count = d.pop("count")
 
         results = []
-        _results = d.pop("results", UNSET)
-        for results_item_data in _results or []:
-            results_item = Space.from_dict(results_item_data)
+        _results = d.pop("results")
+        for results_item_data in _results:
+            results_item = Task.from_dict(results_item_data)
 
             results.append(results_item)
 
-        paginated_space_list = cls(
+        next_ = d.pop("next", UNSET)
+
+        previous = d.pop("previous", UNSET)
+
+        paginated_task_list = cls(
             count=count,
+            results=results,
             next_=next_,
             previous=previous,
-            results=results,
         )
 
-        paginated_space_list.additional_properties = d
-        return paginated_space_list
+        paginated_task_list.additional_properties = d
+        return paginated_task_list
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart_tools-0.5.6/dart/generated/models/paginated_status_list.py` & `dart_tools-0.5.7/dart/generated/models/paginated_task_doc_relationship_list.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,89 +2,89 @@
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.status import Status
+    from ..models.task_doc_relationship import TaskDocRelationship
 
 
-T = TypeVar("T", bound="PaginatedStatusList")
+T = TypeVar("T", bound="PaginatedTaskDocRelationshipList")
 
 
 @_attrs_define
-class PaginatedStatusList:
+class PaginatedTaskDocRelationshipList:
     """
     Attributes:
-        count (Union[Unset, int]):  Example: 123.
+        count (int):  Example: 123.
+        results (List['TaskDocRelationship']):
         next_ (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=400&limit=100.
         previous (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=200&limit=100.
-        results (Union[Unset, List['Status']]):
     """
 
-    count: Union[Unset, int] = UNSET
+    count: int
+    results: List["TaskDocRelationship"]
     next_: Union[Unset, None, str] = UNSET
     previous: Union[Unset, None, str] = UNSET
-    results: Union[Unset, List["Status"]] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         count = self.count
+        results = []
+        for results_item_data in self.results:
+            results_item = results_item_data.to_dict()
+
+            results.append(results_item)
+
         next_ = self.next_
         previous = self.previous
-        results: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.results, Unset):
-            results = []
-            for results_item_data in self.results:
-                results_item = results_item_data.to_dict()
-
-                results.append(results_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if count is not UNSET:
-            field_dict["count"] = count
+        field_dict.update(
+            {
+                "count": count,
+                "results": results,
+            }
+        )
         if next_ is not UNSET:
             field_dict["next"] = next_
         if previous is not UNSET:
             field_dict["previous"] = previous
-        if results is not UNSET:
-            field_dict["results"] = results
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.status import Status
+        from ..models.task_doc_relationship import TaskDocRelationship
 
         d = src_dict.copy()
-        count = d.pop("count", UNSET)
-
-        next_ = d.pop("next", UNSET)
-
-        previous = d.pop("previous", UNSET)
+        count = d.pop("count")
 
         results = []
-        _results = d.pop("results", UNSET)
-        for results_item_data in _results or []:
-            results_item = Status.from_dict(results_item_data)
+        _results = d.pop("results")
+        for results_item_data in _results:
+            results_item = TaskDocRelationship.from_dict(results_item_data)
 
             results.append(results_item)
 
-        paginated_status_list = cls(
+        next_ = d.pop("next", UNSET)
+
+        previous = d.pop("previous", UNSET)
+
+        paginated_task_doc_relationship_list = cls(
             count=count,
+            results=results,
             next_=next_,
             previous=previous,
-            results=results,
         )
 
-        paginated_status_list.additional_properties = d
-        return paginated_status_list
+        paginated_task_doc_relationship_list.additional_properties = d
+        return paginated_task_doc_relationship_list
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart_tools-0.5.6/dart/generated/models/paginated_task_doc_relationship_list.py` & `dart_tools-0.5.7/dart/generated/models/paginated_user_list.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,89 +2,89 @@
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.task_doc_relationship import TaskDocRelationship
+    from ..models.user import User
 
 
-T = TypeVar("T", bound="PaginatedTaskDocRelationshipList")
+T = TypeVar("T", bound="PaginatedUserList")
 
 
 @_attrs_define
-class PaginatedTaskDocRelationshipList:
+class PaginatedUserList:
     """
     Attributes:
-        count (Union[Unset, int]):  Example: 123.
+        count (int):  Example: 123.
+        results (List['User']):
         next_ (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=400&limit=100.
         previous (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=200&limit=100.
-        results (Union[Unset, List['TaskDocRelationship']]):
     """
 
-    count: Union[Unset, int] = UNSET
+    count: int
+    results: List["User"]
     next_: Union[Unset, None, str] = UNSET
     previous: Union[Unset, None, str] = UNSET
-    results: Union[Unset, List["TaskDocRelationship"]] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         count = self.count
+        results = []
+        for results_item_data in self.results:
+            results_item = results_item_data.to_dict()
+
+            results.append(results_item)
+
         next_ = self.next_
         previous = self.previous
-        results: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.results, Unset):
-            results = []
-            for results_item_data in self.results:
-                results_item = results_item_data.to_dict()
-
-                results.append(results_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if count is not UNSET:
-            field_dict["count"] = count
+        field_dict.update(
+            {
+                "count": count,
+                "results": results,
+            }
+        )
         if next_ is not UNSET:
             field_dict["next"] = next_
         if previous is not UNSET:
             field_dict["previous"] = previous
-        if results is not UNSET:
-            field_dict["results"] = results
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.task_doc_relationship import TaskDocRelationship
+        from ..models.user import User
 
         d = src_dict.copy()
-        count = d.pop("count", UNSET)
-
-        next_ = d.pop("next", UNSET)
-
-        previous = d.pop("previous", UNSET)
+        count = d.pop("count")
 
         results = []
-        _results = d.pop("results", UNSET)
-        for results_item_data in _results or []:
-            results_item = TaskDocRelationship.from_dict(results_item_data)
+        _results = d.pop("results")
+        for results_item_data in _results:
+            results_item = User.from_dict(results_item_data)
 
             results.append(results_item)
 
-        paginated_task_doc_relationship_list = cls(
+        next_ = d.pop("next", UNSET)
+
+        previous = d.pop("previous", UNSET)
+
+        paginated_user_list = cls(
             count=count,
+            results=results,
             next_=next_,
             previous=previous,
-            results=results,
         )
 
-        paginated_task_doc_relationship_list.additional_properties = d
-        return paginated_task_doc_relationship_list
+        paginated_user_list.additional_properties = d
+        return paginated_user_list
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart_tools-0.5.6/dart/generated/models/paginated_task_link_list.py` & `dart_tools-0.5.7/dart/generated/models/paginated_task_link_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,75 +12,75 @@
 T = TypeVar("T", bound="PaginatedTaskLinkList")
 
 
 @_attrs_define
 class PaginatedTaskLinkList:
     """
     Attributes:
-        count (Union[Unset, int]):  Example: 123.
+        count (int):  Example: 123.
+        results (List['TaskLink']):
         next_ (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=400&limit=100.
         previous (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=200&limit=100.
-        results (Union[Unset, List['TaskLink']]):
     """
 
-    count: Union[Unset, int] = UNSET
+    count: int
+    results: List["TaskLink"]
     next_: Union[Unset, None, str] = UNSET
     previous: Union[Unset, None, str] = UNSET
-    results: Union[Unset, List["TaskLink"]] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         count = self.count
+        results = []
+        for results_item_data in self.results:
+            results_item = results_item_data.to_dict()
+
+            results.append(results_item)
+
         next_ = self.next_
         previous = self.previous
-        results: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.results, Unset):
-            results = []
-            for results_item_data in self.results:
-                results_item = results_item_data.to_dict()
-
-                results.append(results_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if count is not UNSET:
-            field_dict["count"] = count
+        field_dict.update(
+            {
+                "count": count,
+                "results": results,
+            }
+        )
         if next_ is not UNSET:
             field_dict["next"] = next_
         if previous is not UNSET:
             field_dict["previous"] = previous
-        if results is not UNSET:
-            field_dict["results"] = results
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.task_link import TaskLink
 
         d = src_dict.copy()
-        count = d.pop("count", UNSET)
-
-        next_ = d.pop("next", UNSET)
-
-        previous = d.pop("previous", UNSET)
+        count = d.pop("count")
 
         results = []
-        _results = d.pop("results", UNSET)
-        for results_item_data in _results or []:
+        _results = d.pop("results")
+        for results_item_data in _results:
             results_item = TaskLink.from_dict(results_item_data)
 
             results.append(results_item)
 
+        next_ = d.pop("next", UNSET)
+
+        previous = d.pop("previous", UNSET)
+
         paginated_task_link_list = cls(
             count=count,
+            results=results,
             next_=next_,
             previous=previous,
-            results=results,
         )
 
         paginated_task_link_list.additional_properties = d
         return paginated_task_link_list
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `dart_tools-0.5.6/dart/generated/models/paginated_task_list.py` & `dart_tools-0.5.7/dart/generated/models/paginated_form_field_list.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,89 +2,89 @@
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.task import Task
+    from ..models.form_field import FormField
 
 
-T = TypeVar("T", bound="PaginatedTaskList")
+T = TypeVar("T", bound="PaginatedFormFieldList")
 
 
 @_attrs_define
-class PaginatedTaskList:
+class PaginatedFormFieldList:
     """
     Attributes:
-        count (Union[Unset, int]):  Example: 123.
+        count (int):  Example: 123.
+        results (List['FormField']):
         next_ (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=400&limit=100.
         previous (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=200&limit=100.
-        results (Union[Unset, List['Task']]):
     """
 
-    count: Union[Unset, int] = UNSET
+    count: int
+    results: List["FormField"]
     next_: Union[Unset, None, str] = UNSET
     previous: Union[Unset, None, str] = UNSET
-    results: Union[Unset, List["Task"]] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         count = self.count
+        results = []
+        for results_item_data in self.results:
+            results_item = results_item_data.to_dict()
+
+            results.append(results_item)
+
         next_ = self.next_
         previous = self.previous
-        results: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.results, Unset):
-            results = []
-            for results_item_data in self.results:
-                results_item = results_item_data.to_dict()
-
-                results.append(results_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if count is not UNSET:
-            field_dict["count"] = count
+        field_dict.update(
+            {
+                "count": count,
+                "results": results,
+            }
+        )
         if next_ is not UNSET:
             field_dict["next"] = next_
         if previous is not UNSET:
             field_dict["previous"] = previous
-        if results is not UNSET:
-            field_dict["results"] = results
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.task import Task
+        from ..models.form_field import FormField
 
         d = src_dict.copy()
-        count = d.pop("count", UNSET)
-
-        next_ = d.pop("next", UNSET)
-
-        previous = d.pop("previous", UNSET)
+        count = d.pop("count")
 
         results = []
-        _results = d.pop("results", UNSET)
-        for results_item_data in _results or []:
-            results_item = Task.from_dict(results_item_data)
+        _results = d.pop("results")
+        for results_item_data in _results:
+            results_item = FormField.from_dict(results_item_data)
 
             results.append(results_item)
 
-        paginated_task_list = cls(
+        next_ = d.pop("next", UNSET)
+
+        previous = d.pop("previous", UNSET)
+
+        paginated_form_field_list = cls(
             count=count,
+            results=results,
             next_=next_,
             previous=previous,
-            results=results,
         )
 
-        paginated_task_list.additional_properties = d
-        return paginated_task_list
+        paginated_form_field_list.additional_properties = d
+        return paginated_form_field_list
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart_tools-0.5.6/dart/generated/models/paginated_tenant_list.py` & `dart_tools-0.5.7/dart/generated/models/paginated_doc_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,89 +2,89 @@
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.tenant import Tenant
+    from ..models.doc import Doc
 
 
-T = TypeVar("T", bound="PaginatedTenantList")
+T = TypeVar("T", bound="PaginatedDocList")
 
 
 @_attrs_define
-class PaginatedTenantList:
+class PaginatedDocList:
     """
     Attributes:
-        count (Union[Unset, int]):  Example: 123.
+        count (int):  Example: 123.
+        results (List['Doc']):
         next_ (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=400&limit=100.
         previous (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=200&limit=100.
-        results (Union[Unset, List['Tenant']]):
     """
 
-    count: Union[Unset, int] = UNSET
+    count: int
+    results: List["Doc"]
     next_: Union[Unset, None, str] = UNSET
     previous: Union[Unset, None, str] = UNSET
-    results: Union[Unset, List["Tenant"]] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         count = self.count
+        results = []
+        for results_item_data in self.results:
+            results_item = results_item_data.to_dict()
+
+            results.append(results_item)
+
         next_ = self.next_
         previous = self.previous
-        results: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.results, Unset):
-            results = []
-            for results_item_data in self.results:
-                results_item = results_item_data.to_dict()
-
-                results.append(results_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if count is not UNSET:
-            field_dict["count"] = count
+        field_dict.update(
+            {
+                "count": count,
+                "results": results,
+            }
+        )
         if next_ is not UNSET:
             field_dict["next"] = next_
         if previous is not UNSET:
             field_dict["previous"] = previous
-        if results is not UNSET:
-            field_dict["results"] = results
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.tenant import Tenant
+        from ..models.doc import Doc
 
         d = src_dict.copy()
-        count = d.pop("count", UNSET)
-
-        next_ = d.pop("next", UNSET)
-
-        previous = d.pop("previous", UNSET)
+        count = d.pop("count")
 
         results = []
-        _results = d.pop("results", UNSET)
-        for results_item_data in _results or []:
-            results_item = Tenant.from_dict(results_item_data)
+        _results = d.pop("results")
+        for results_item_data in _results:
+            results_item = Doc.from_dict(results_item_data)
 
             results.append(results_item)
 
-        paginated_tenant_list = cls(
+        next_ = d.pop("next", UNSET)
+
+        previous = d.pop("previous", UNSET)
+
+        paginated_doc_list = cls(
             count=count,
+            results=results,
             next_=next_,
             previous=previous,
-            results=results,
         )
 
-        paginated_tenant_list.additional_properties = d
-        return paginated_tenant_list
+        paginated_doc_list.additional_properties = d
+        return paginated_doc_list
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart_tools-0.5.6/dart/generated/models/paginated_user_dartboard_layout_list.py` & `dart_tools-0.5.7/dart/generated/models/paginated_tenant_list.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,89 +2,89 @@
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.user_dartboard_layout import UserDartboardLayout
+    from ..models.tenant import Tenant
 
 
-T = TypeVar("T", bound="PaginatedUserDartboardLayoutList")
+T = TypeVar("T", bound="PaginatedTenantList")
 
 
 @_attrs_define
-class PaginatedUserDartboardLayoutList:
+class PaginatedTenantList:
     """
     Attributes:
-        count (Union[Unset, int]):  Example: 123.
+        count (int):  Example: 123.
+        results (List['Tenant']):
         next_ (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=400&limit=100.
         previous (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=200&limit=100.
-        results (Union[Unset, List['UserDartboardLayout']]):
     """
 
-    count: Union[Unset, int] = UNSET
+    count: int
+    results: List["Tenant"]
     next_: Union[Unset, None, str] = UNSET
     previous: Union[Unset, None, str] = UNSET
-    results: Union[Unset, List["UserDartboardLayout"]] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         count = self.count
+        results = []
+        for results_item_data in self.results:
+            results_item = results_item_data.to_dict()
+
+            results.append(results_item)
+
         next_ = self.next_
         previous = self.previous
-        results: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.results, Unset):
-            results = []
-            for results_item_data in self.results:
-                results_item = results_item_data.to_dict()
-
-                results.append(results_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if count is not UNSET:
-            field_dict["count"] = count
+        field_dict.update(
+            {
+                "count": count,
+                "results": results,
+            }
+        )
         if next_ is not UNSET:
             field_dict["next"] = next_
         if previous is not UNSET:
             field_dict["previous"] = previous
-        if results is not UNSET:
-            field_dict["results"] = results
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.user_dartboard_layout import UserDartboardLayout
+        from ..models.tenant import Tenant
 
         d = src_dict.copy()
-        count = d.pop("count", UNSET)
-
-        next_ = d.pop("next", UNSET)
-
-        previous = d.pop("previous", UNSET)
+        count = d.pop("count")
 
         results = []
-        _results = d.pop("results", UNSET)
-        for results_item_data in _results or []:
-            results_item = UserDartboardLayout.from_dict(results_item_data)
+        _results = d.pop("results")
+        for results_item_data in _results:
+            results_item = Tenant.from_dict(results_item_data)
 
             results.append(results_item)
 
-        paginated_user_dartboard_layout_list = cls(
+        next_ = d.pop("next", UNSET)
+
+        previous = d.pop("previous", UNSET)
+
+        paginated_tenant_list = cls(
             count=count,
+            results=results,
             next_=next_,
             previous=previous,
-            results=results,
         )
 
-        paginated_user_dartboard_layout_list.additional_properties = d
-        return paginated_user_dartboard_layout_list
+        paginated_tenant_list.additional_properties = d
+        return paginated_tenant_list
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart_tools-0.5.6/dart/generated/models/paginated_user_list.py` & `dart_tools-0.5.7/dart/generated/models/response_body.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,90 +1,64 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
-from ..types import UNSET, Unset
-
 if TYPE_CHECKING:
-    from ..models.user import User
+    from ..models.transaction_response import TransactionResponse
 
 
-T = TypeVar("T", bound="PaginatedUserList")
+T = TypeVar("T", bound="ResponseBody")
 
 
 @_attrs_define
-class PaginatedUserList:
+class ResponseBody:
     """
     Attributes:
-        count (Union[Unset, int]):  Example: 123.
-        next_ (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=400&limit=100.
-        previous (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=200&limit=100.
-        results (Union[Unset, List['User']]):
+        results (List['TransactionResponse']):
     """
 
-    count: Union[Unset, int] = UNSET
-    next_: Union[Unset, None, str] = UNSET
-    previous: Union[Unset, None, str] = UNSET
-    results: Union[Unset, List["User"]] = UNSET
+    results: List["TransactionResponse"]
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        count = self.count
-        next_ = self.next_
-        previous = self.previous
-        results: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.results, Unset):
-            results = []
-            for results_item_data in self.results:
-                results_item = results_item_data.to_dict()
+        results = []
+        for results_item_data in self.results:
+            results_item = results_item_data.to_dict()
 
-                results.append(results_item)
+            results.append(results_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if count is not UNSET:
-            field_dict["count"] = count
-        if next_ is not UNSET:
-            field_dict["next"] = next_
-        if previous is not UNSET:
-            field_dict["previous"] = previous
-        if results is not UNSET:
-            field_dict["results"] = results
+        field_dict.update(
+            {
+                "results": results,
+            }
+        )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.user import User
+        from ..models.transaction_response import TransactionResponse
 
         d = src_dict.copy()
-        count = d.pop("count", UNSET)
-
-        next_ = d.pop("next", UNSET)
-
-        previous = d.pop("previous", UNSET)
-
         results = []
-        _results = d.pop("results", UNSET)
-        for results_item_data in _results or []:
-            results_item = User.from_dict(results_item_data)
+        _results = d.pop("results")
+        for results_item_data in _results:
+            results_item = TransactionResponse.from_dict(results_item_data)
 
             results.append(results_item)
 
-        paginated_user_list = cls(
-            count=count,
-            next_=next_,
-            previous=previous,
+        response_body = cls(
             results=results,
         )
 
-        paginated_user_list.additional_properties = d
-        return paginated_user_list
+        response_body.additional_properties = d
+        return response_body
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart_tools-0.5.6/dart/generated/models/paginated_view_list.py` & `dart_tools-0.5.7/dart/generated/models/paginated_comment_reaction_list.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,89 +2,89 @@
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.view import View
+    from ..models.comment_reaction import CommentReaction
 
 
-T = TypeVar("T", bound="PaginatedViewList")
+T = TypeVar("T", bound="PaginatedCommentReactionList")
 
 
 @_attrs_define
-class PaginatedViewList:
+class PaginatedCommentReactionList:
     """
     Attributes:
-        count (Union[Unset, int]):  Example: 123.
+        count (int):  Example: 123.
+        results (List['CommentReaction']):
         next_ (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=400&limit=100.
         previous (Union[Unset, None, str]):  Example: http://api.example.org/accounts/?offset=200&limit=100.
-        results (Union[Unset, List['View']]):
     """
 
-    count: Union[Unset, int] = UNSET
+    count: int
+    results: List["CommentReaction"]
     next_: Union[Unset, None, str] = UNSET
     previous: Union[Unset, None, str] = UNSET
-    results: Union[Unset, List["View"]] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         count = self.count
+        results = []
+        for results_item_data in self.results:
+            results_item = results_item_data.to_dict()
+
+            results.append(results_item)
+
         next_ = self.next_
         previous = self.previous
-        results: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.results, Unset):
-            results = []
-            for results_item_data in self.results:
-                results_item = results_item_data.to_dict()
-
-                results.append(results_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if count is not UNSET:
-            field_dict["count"] = count
+        field_dict.update(
+            {
+                "count": count,
+                "results": results,
+            }
+        )
         if next_ is not UNSET:
             field_dict["next"] = next_
         if previous is not UNSET:
             field_dict["previous"] = previous
-        if results is not UNSET:
-            field_dict["results"] = results
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.view import View
+        from ..models.comment_reaction import CommentReaction
 
         d = src_dict.copy()
-        count = d.pop("count", UNSET)
-
-        next_ = d.pop("next", UNSET)
-
-        previous = d.pop("previous", UNSET)
+        count = d.pop("count")
 
         results = []
-        _results = d.pop("results", UNSET)
-        for results_item_data in _results or []:
-            results_item = View.from_dict(results_item_data)
+        _results = d.pop("results")
+        for results_item_data in _results:
+            results_item = CommentReaction.from_dict(results_item_data)
 
             results.append(results_item)
 
-        paginated_view_list = cls(
+        next_ = d.pop("next", UNSET)
+
+        previous = d.pop("previous", UNSET)
+
+        paginated_comment_reaction_list = cls(
             count=count,
+            results=results,
             next_=next_,
             previous=previous,
-            results=results,
         )
 
-        paginated_view_list.additional_properties = d
-        return paginated_view_list
+        paginated_comment_reaction_list.additional_properties = d
+        return paginated_comment_reaction_list
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart_tools-0.5.6/dart/generated/models/properties_list_kind.py` & `dart_tools-0.5.7/dart/generated/models/properties_list_kind.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/property_.py` & `dart_tools-0.5.7/dart/generated/models/property_.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/property_create.py` & `dart_tools-0.5.7/dart/generated/models/property_create.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/property_kind.py` & `dart_tools-0.5.7/dart/generated/models/property_kind.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/property_update.py` & `dart_tools-0.5.7/dart/generated/models/property_update.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/relationship.py` & `dart_tools-0.5.7/dart/generated/models/relationship.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/relationship_create.py` & `dart_tools-0.5.7/dart/generated/models/relationship_create.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/relationship_kind.py` & `dart_tools-0.5.7/dart/generated/models/relationship_kind.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/relationship_kind_create.py` & `dart_tools-0.5.7/dart/generated/models/relationship_kind_create.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/relationship_kind_update.py` & `dart_tools-0.5.7/dart/generated/models/relationship_kind_update.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/request_body.py` & `dart_tools-0.5.7/dart/generated/models/request_body.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/response_body.py` & `dart_tools-0.5.7/dart/generated/models/user_dartboard_layout.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,56 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
-if TYPE_CHECKING:
-    from ..models.transaction_response import TransactionResponse
-
-
-T = TypeVar("T", bound="ResponseBody")
+T = TypeVar("T", bound="UserDartboardLayout")
 
 
 @_attrs_define
-class ResponseBody:
+class UserDartboardLayout:
     """
     Attributes:
-        results (List['TransactionResponse']):
+        user_duid (str):
+        layout_duid (str):
     """
 
-    results: List["TransactionResponse"]
+    user_duid: str
+    layout_duid: str
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        results = []
-        for results_item_data in self.results:
-            results_item = results_item_data.to_dict()
-
-            results.append(results_item)
+        user_duid = self.user_duid
+        layout_duid = self.layout_duid
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "results": results,
+                "userDuid": user_duid,
+                "layoutDuid": layout_duid,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.transaction_response import TransactionResponse
-
         d = src_dict.copy()
-        results = []
-        _results = d.pop("results")
-        for results_item_data in _results:
-            results_item = TransactionResponse.from_dict(results_item_data)
+        user_duid = d.pop("userDuid")
 
-            results.append(results_item)
+        layout_duid = d.pop("layoutDuid")
 
-        response_body = cls(
-            results=results,
+        user_dartboard_layout = cls(
+            user_duid=user_duid,
+            layout_duid=layout_duid,
         )
 
-        response_body.additional_properties = d
-        return response_body
+        user_dartboard_layout.additional_properties = d
+        return user_dartboard_layout
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart_tools-0.5.6/dart/generated/models/slack_integration.py` & `dart_tools-0.5.7/dart/generated/models/slack_integration.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/sort.py` & `dart_tools-0.5.7/dart/generated/models/sort.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/space.py` & `dart_tools-0.5.7/dart/generated/models/space.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/space_create.py` & `dart_tools-0.5.7/dart/generated/models/space_create.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/space_update.py` & `dart_tools-0.5.7/dart/generated/models/space_update.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/status.py` & `dart_tools-0.5.7/dart/generated/models/status.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/status_create.py` & `dart_tools-0.5.7/dart/generated/models/status_create.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/status_update.py` & `dart_tools-0.5.7/dart/generated/models/folder.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..models.color_name import ColorName
-from ..models.status_kind import StatusKind
+from ..models.folder_kind import FolderKind
+from ..models.icon_kind import IconKind
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="StatusUpdate")
+T = TypeVar("T", bound="Folder")
 
 
 @_attrs_define
-class StatusUpdate:
+class Folder:
     """
     Attributes:
         duid (str):
-        property_duid (Union[Unset, str]):
-        kind (Union[Unset, StatusKind]): * `Unstarted` - UNSTARTED
-            * `Started` - STARTED
-            * `Blocked` - BLOCKED
-            * `Finished` - FINISHED
-            * `Canceled` - CANCELED
-        locked (Union[Unset, bool]):
-        order (Union[Unset, str]):
-        title (Union[Unset, str]):
-        color_name (Union[Unset, ColorName]): * `Red` - RED
+        space_duid (str):
+        kind (FolderKind): * `Other` - OTHER
+            * `Default` - DEFAULT
+            * `Reports` - REPORTS
+        order (str):
+        title (str):
+        description (str):
+        icon_kind (IconKind): * `None` - NONE
+            * `Icon` - ICON
+            * `Emoji` - EMOJI
+        icon_name_or_emoji (str):
+        color_name (ColorName): * `Red` - RED
             * `Dark Blue` - DARK_BLUE
             * `Dark Orange` - DARK_ORANGE
             * `Dark Green` - DARK_GREEN
             * `Purple` - PURPLE
             * `Dark Teal` - DARK_TEAL
             * `Pink` - PINK
             * `Orange` - ORANGE
@@ -44,109 +47,102 @@
             * `Light Purple` - LIGHT_PURPLE
             * `Light Orange` - LIGHT_ORANGE
             * `Light Pink` - LIGHT_PINK
             * `Tan` - TAN
             * `Dark Gray` - DARK_GRAY
             * `Light Brown` - LIGHT_BROWN
             * `Light Gray` - LIGHT_GRAY
-        description (Union[Unset, str]):
+        updated_by_client_duid (Union[Unset, None, str]):
     """
 
     duid: str
-    property_duid: Union[Unset, str] = UNSET
-    kind: Union[Unset, StatusKind] = UNSET
-    locked: Union[Unset, bool] = UNSET
-    order: Union[Unset, str] = UNSET
-    title: Union[Unset, str] = UNSET
-    color_name: Union[Unset, ColorName] = UNSET
-    description: Union[Unset, str] = UNSET
+    space_duid: str
+    kind: FolderKind
+    order: str
+    title: str
+    description: str
+    icon_kind: IconKind
+    icon_name_or_emoji: str
+    color_name: ColorName
+    updated_by_client_duid: Union[Unset, None, str] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         duid = self.duid
-        property_duid = self.property_duid
-        kind: Union[Unset, str] = UNSET
-        if not isinstance(self.kind, Unset):
-            kind = self.kind.value
+        space_duid = self.space_duid
+        kind = self.kind.value
 
-        locked = self.locked
         order = self.order
         title = self.title
-        color_name: Union[Unset, str] = UNSET
-        if not isinstance(self.color_name, Unset):
-            color_name = self.color_name.value
-
         description = self.description
+        icon_kind = self.icon_kind.value
+
+        icon_name_or_emoji = self.icon_name_or_emoji
+        color_name = self.color_name.value
+
+        updated_by_client_duid = self.updated_by_client_duid
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "duid": duid,
+                "spaceDuid": space_duid,
+                "kind": kind,
+                "order": order,
+                "title": title,
+                "description": description,
+                "iconKind": icon_kind,
+                "iconNameOrEmoji": icon_name_or_emoji,
+                "colorName": color_name,
             }
         )
-        if property_duid is not UNSET:
-            field_dict["propertyDuid"] = property_duid
-        if kind is not UNSET:
-            field_dict["kind"] = kind
-        if locked is not UNSET:
-            field_dict["locked"] = locked
-        if order is not UNSET:
-            field_dict["order"] = order
-        if title is not UNSET:
-            field_dict["title"] = title
-        if color_name is not UNSET:
-            field_dict["colorName"] = color_name
-        if description is not UNSET:
-            field_dict["description"] = description
+        if updated_by_client_duid is not UNSET:
+            field_dict["updatedByClientDuid"] = updated_by_client_duid
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         duid = d.pop("duid")
 
-        property_duid = d.pop("propertyDuid", UNSET)
+        space_duid = d.pop("spaceDuid")
+
+        kind = FolderKind(d.pop("kind"))
 
-        _kind = d.pop("kind", UNSET)
-        kind: Union[Unset, StatusKind]
-        if isinstance(_kind, Unset):
-            kind = UNSET
-        else:
-            kind = StatusKind(_kind)
+        order = d.pop("order")
 
-        locked = d.pop("locked", UNSET)
+        title = d.pop("title")
 
-        order = d.pop("order", UNSET)
+        description = d.pop("description")
 
-        title = d.pop("title", UNSET)
+        icon_kind = IconKind(d.pop("iconKind"))
 
-        _color_name = d.pop("colorName", UNSET)
-        color_name: Union[Unset, ColorName]
-        if isinstance(_color_name, Unset):
-            color_name = UNSET
-        else:
-            color_name = ColorName(_color_name)
+        icon_name_or_emoji = d.pop("iconNameOrEmoji")
 
-        description = d.pop("description", UNSET)
+        color_name = ColorName(d.pop("colorName"))
 
-        status_update = cls(
+        updated_by_client_duid = d.pop("updatedByClientDuid", UNSET)
+
+        folder = cls(
             duid=duid,
-            property_duid=property_duid,
+            space_duid=space_duid,
             kind=kind,
-            locked=locked,
             order=order,
             title=title,
-            color_name=color_name,
             description=description,
+            icon_kind=icon_kind,
+            icon_name_or_emoji=icon_name_or_emoji,
+            color_name=color_name,
+            updated_by_client_duid=updated_by_client_duid,
         )
 
-        status_update.additional_properties = d
-        return status_update
+        folder.additional_properties = d
+        return folder
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart_tools-0.5.6/dart/generated/models/task.py` & `dart_tools-0.5.7/dart/generated/models/task.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Type, TypeVar, Union, cast
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from dateutil.parser import isoparse
 
 from ..models.priority import Priority
-from ..models.recommendation_status import RecommendationStatus
+from ..models.task_source_type import TaskSourceType
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
     from ..models.relationship import Relationship
     from ..models.task_link import TaskLink
     from ..models.task_notion_document import TaskNotionDocument
     from ..models.task_properties import TaskProperties
@@ -20,14 +20,38 @@
 
 
 @_attrs_define
 class Task:
     """
     Attributes:
         duid (str):
+        source_type (TaskSourceType): * `Unknown` - UNKNOWN
+            * `Import` - IMPORT
+            * `Onboarding` - ONBOARDING
+            * `Recommendation` - RECOMMENDATION
+            * `Recurrence` - RECURRENCE
+            * `Template` - TEMPLATE
+            * `ChatGPT` - CHAT_GPT
+            * `Email` - EMAIL
+            * `Slack` - SLACK
+            * `API` - API
+            * `CLI` - CLI
+            * `Application` - APPLICATION
+            * `AppTcm` - APP_TCM
+            * `AppInternalForm` - APP_INTERNAL_FORM
+            * `AppQuickAdd` - APP_QUICK_ADD
+            * `AppBoard` - APP_BOARD
+            * `AppSubtask` - APP_SUBTASK
+            * `AppRelationship` - APP_RELATIONSHIP
+            * `AppEnter` - APP_ENTER
+            * `AppReplicate` - APP_REPLICATE
+            * `AppPaste` - APP_PASTE
+            * `AppRoadmapList` - APP_ROADMAP_LIST
+            * `AppRoadmapTimeline` - APP_ROADMAP_TIMELINE
+            * `ExternalForm` - EXTERNAL_FORM
         created_at (datetime.datetime):
         updated_at (datetime.datetime):
         in_trash (bool):
         dartboard_duid (str):
         order (str):
         title (str):
         description (Any):
@@ -41,29 +65,28 @@
         relationships (List['Relationship']):
         recurrence (Any):
         properties (TaskProperties):
         updated_by_client_duid (Union[Unset, None, str]):
         created_by_duid (Optional[str]):
         updated_by_duid (Optional[str]):
         drafter_duid (Optional[str]):
-        recommendation_status (Optional[RecommendationStatus]): * `Accepted` - ACCEPTED
-            * `Declined` - DECLINED
         notion_document (Optional[TaskNotionDocument]):
         priority (Optional[Priority]): * `Critical` - CRITICAL
             * `High` - HIGH
             * `Medium` - MEDIUM
             * `Low` - LOW
         size (Optional[int]):
         start_at (Optional[datetime.datetime]):
         due_at (Optional[datetime.datetime]):
         remind_at (Optional[datetime.datetime]):
         recurrs_next_at (Optional[datetime.datetime]):
     """
 
     duid: str
+    source_type: TaskSourceType
     created_at: datetime.datetime
     updated_at: datetime.datetime
     in_trash: bool
     dartboard_duid: str
     order: str
     title: str
     description: Any
@@ -76,27 +99,28 @@
     attachment_duids: List[str]
     relationships: List["Relationship"]
     recurrence: Any
     properties: "TaskProperties"
     created_by_duid: Optional[str]
     updated_by_duid: Optional[str]
     drafter_duid: Optional[str]
-    recommendation_status: Optional[RecommendationStatus]
     notion_document: Optional["TaskNotionDocument"]
     priority: Optional[Priority]
     size: Optional[int]
     start_at: Optional[datetime.datetime]
     due_at: Optional[datetime.datetime]
     remind_at: Optional[datetime.datetime]
     recurrs_next_at: Optional[datetime.datetime]
     updated_by_client_duid: Union[Unset, None, str] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         duid = self.duid
+        source_type = self.source_type.value
+
         created_at = self.created_at.isoformat()
 
         updated_at = self.updated_at.isoformat()
 
         in_trash = self.in_trash
         dartboard_duid = self.dartboard_duid
         order = self.order
@@ -127,16 +151,14 @@
         recurrence = self.recurrence
         properties = self.properties.to_dict()
 
         updated_by_client_duid = self.updated_by_client_duid
         created_by_duid = self.created_by_duid
         updated_by_duid = self.updated_by_duid
         drafter_duid = self.drafter_duid
-        recommendation_status = self.recommendation_status.value if self.recommendation_status else None
-
         notion_document = self.notion_document.to_dict() if self.notion_document else None
 
         priority = self.priority.value if self.priority else None
 
         size = self.size
         start_at = self.start_at.isoformat() if self.start_at else None
 
@@ -147,14 +169,15 @@
         recurrs_next_at = self.recurrs_next_at.isoformat() if self.recurrs_next_at else None
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "duid": duid,
+                "sourceType": source_type,
                 "createdAt": created_at,
                 "updatedAt": updated_at,
                 "inTrash": in_trash,
                 "dartboardDuid": dartboard_duid,
                 "order": order,
                 "title": title,
                 "description": description,
@@ -167,15 +190,14 @@
                 "attachmentDuids": attachment_duids,
                 "relationships": relationships,
                 "recurrence": recurrence,
                 "properties": properties,
                 "createdByDuid": created_by_duid,
                 "updatedByDuid": updated_by_duid,
                 "drafterDuid": drafter_duid,
-                "recommendationStatus": recommendation_status,
                 "notionDocument": notion_document,
                 "priority": priority,
                 "size": size,
                 "startAt": start_at,
                 "dueAt": due_at,
                 "remindAt": remind_at,
                 "recurrsNextAt": recurrs_next_at,
@@ -192,14 +214,16 @@
         from ..models.task_link import TaskLink
         from ..models.task_notion_document import TaskNotionDocument
         from ..models.task_properties import TaskProperties
 
         d = src_dict.copy()
         duid = d.pop("duid")
 
+        source_type = TaskSourceType(d.pop("sourceType"))
+
         created_at = isoparse(d.pop("createdAt"))
 
         updated_at = isoparse(d.pop("updatedAt"))
 
         in_trash = d.pop("inTrash")
 
         dartboard_duid = d.pop("dartboardDuid")
@@ -244,21 +268,14 @@
 
         created_by_duid = d.pop("createdByDuid")
 
         updated_by_duid = d.pop("updatedByDuid")
 
         drafter_duid = d.pop("drafterDuid")
 
-        _recommendation_status = d.pop("recommendationStatus")
-        recommendation_status: Optional[RecommendationStatus]
-        if _recommendation_status is None:
-            recommendation_status = None
-        else:
-            recommendation_status = RecommendationStatus(_recommendation_status)
-
         _notion_document = d.pop("notionDocument")
         notion_document: Optional[TaskNotionDocument]
         if _notion_document is None:
             notion_document = None
         else:
             notion_document = TaskNotionDocument.from_dict(_notion_document)
 
@@ -297,14 +314,15 @@
         if _recurrs_next_at is None:
             recurrs_next_at = None
         else:
             recurrs_next_at = isoparse(_recurrs_next_at)
 
         task = cls(
             duid=duid,
+            source_type=source_type,
             created_at=created_at,
             updated_at=updated_at,
             in_trash=in_trash,
             dartboard_duid=dartboard_duid,
             order=order,
             title=title,
             description=description,
@@ -318,15 +336,14 @@
             relationships=relationships,
             recurrence=recurrence,
             properties=properties,
             updated_by_client_duid=updated_by_client_duid,
             created_by_duid=created_by_duid,
             updated_by_duid=updated_by_duid,
             drafter_duid=drafter_duid,
-            recommendation_status=recommendation_status,
             notion_document=notion_document,
             priority=priority,
             size=size,
             start_at=start_at,
             due_at=due_at,
             remind_at=remind_at,
             recurrs_next_at=recurrs_next_at,
```

### Comparing `dart_tools-0.5.6/dart/generated/models/task_create.py` & `dart_tools-0.5.7/dart/generated/models/task_create.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from dateutil.parser import isoparse
 
 from ..models.priority import Priority
-from ..models.recommendation_status import RecommendationStatus
 from ..models.task_source_type import TaskSourceType
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="TaskCreate")
 
 
 @_attrs_define
@@ -43,16 +42,14 @@
             * `AppRoadmapTimeline` - APP_ROADMAP_TIMELINE
             * `ExternalForm` - EXTERNAL_FORM Default: TaskSourceType.UNKNOWN.
         source_form_duid (Union[Unset, None, str]):
         created_by_duid (Union[Unset, None, str]):
         updated_by_duid (Union[Unset, None, str]):
         drafter_duid (Union[Unset, None, str]):
         in_trash (Union[Unset, bool]):
-        recommendation_status (Union[Unset, None, RecommendationStatus]): * `Accepted` - ACCEPTED
-            * `Declined` - DECLINED
         dartboard_duid (Union[Unset, str]):
         order (Union[Unset, str]):
         title (Union[Unset, str]):
         description (Union[Unset, Any]):
         description_markdown (Union[Unset, str]):
         status_duid (Union[Unset, str]):
         assigned_to_ai (Union[Unset, bool]):
@@ -76,15 +73,14 @@
     duid: str
     source_type: Union[Unset, TaskSourceType] = TaskSourceType.UNKNOWN
     source_form_duid: Union[Unset, None, str] = UNSET
     created_by_duid: Union[Unset, None, str] = UNSET
     updated_by_duid: Union[Unset, None, str] = UNSET
     drafter_duid: Union[Unset, None, str] = UNSET
     in_trash: Union[Unset, bool] = UNSET
-    recommendation_status: Union[Unset, None, RecommendationStatus] = UNSET
     dartboard_duid: Union[Unset, str] = UNSET
     order: Union[Unset, str] = UNSET
     title: Union[Unset, str] = UNSET
     description: Union[Unset, Any] = UNSET
     description_markdown: Union[Unset, str] = UNSET
     status_duid: Union[Unset, str] = UNSET
     assigned_to_ai: Union[Unset, bool] = UNSET
@@ -109,18 +105,14 @@
             source_type = self.source_type.value
 
         source_form_duid = self.source_form_duid
         created_by_duid = self.created_by_duid
         updated_by_duid = self.updated_by_duid
         drafter_duid = self.drafter_duid
         in_trash = self.in_trash
-        recommendation_status: Union[Unset, None, str] = UNSET
-        if not isinstance(self.recommendation_status, Unset):
-            recommendation_status = self.recommendation_status.value if self.recommendation_status else None
-
         dartboard_duid = self.dartboard_duid
         order = self.order
         title = self.title
         description = self.description
         description_markdown = self.description_markdown
         status_duid = self.status_duid
         assigned_to_ai = self.assigned_to_ai
@@ -179,16 +171,14 @@
             field_dict["createdByDuid"] = created_by_duid
         if updated_by_duid is not UNSET:
             field_dict["updatedByDuid"] = updated_by_duid
         if drafter_duid is not UNSET:
             field_dict["drafterDuid"] = drafter_duid
         if in_trash is not UNSET:
             field_dict["inTrash"] = in_trash
-        if recommendation_status is not UNSET:
-            field_dict["recommendationStatus"] = recommendation_status
         if dartboard_duid is not UNSET:
             field_dict["dartboardDuid"] = dartboard_duid
         if order is not UNSET:
             field_dict["order"] = order
         if title is not UNSET:
             field_dict["title"] = title
         if description is not UNSET:
@@ -244,23 +234,14 @@
 
         updated_by_duid = d.pop("updatedByDuid", UNSET)
 
         drafter_duid = d.pop("drafterDuid", UNSET)
 
         in_trash = d.pop("inTrash", UNSET)
 
-        _recommendation_status = d.pop("recommendationStatus", UNSET)
-        recommendation_status: Union[Unset, None, RecommendationStatus]
-        if _recommendation_status is None:
-            recommendation_status = None
-        elif isinstance(_recommendation_status, Unset):
-            recommendation_status = UNSET
-        else:
-            recommendation_status = RecommendationStatus(_recommendation_status)
-
         dartboard_duid = d.pop("dartboardDuid", UNSET)
 
         order = d.pop("order", UNSET)
 
         title = d.pop("title", UNSET)
 
         description = d.pop("description", UNSET)
@@ -334,15 +315,14 @@
             duid=duid,
             source_type=source_type,
             source_form_duid=source_form_duid,
             created_by_duid=created_by_duid,
             updated_by_duid=updated_by_duid,
             drafter_duid=drafter_duid,
             in_trash=in_trash,
-            recommendation_status=recommendation_status,
             dartboard_duid=dartboard_duid,
             order=order,
             title=title,
             description=description,
             description_markdown=description_markdown,
             status_duid=status_duid,
             assigned_to_ai=assigned_to_ai,
```

### Comparing `dart_tools-0.5.6/dart/generated/models/task_doc_relationship.py` & `dart_tools-0.5.7/dart/generated/models/task_doc_relationship.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/task_doc_relationship_create.py` & `dart_tools-0.5.7/dart/generated/models/task_doc_relationship_create.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/task_link.py` & `dart_tools-0.5.7/dart/generated/models/task_link.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/task_link_create.py` & `dart_tools-0.5.7/dart/generated/models/task_link_create.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/task_link_kind.py` & `dart_tools-0.5.7/dart/generated/models/task_link_kind.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/task_link_update.py` & `dart_tools-0.5.7/dart/generated/models/task_link_update.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/task_notion_document.py` & `dart_tools-0.5.7/dart/generated/models/task_notion_document.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/task_notion_document_block_children_map.py` & `dart_tools-0.5.7/dart/generated/models/task_notion_document_block_children_map.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/task_notion_document_block_map.py` & `dart_tools-0.5.7/dart/generated/models/task_notion_document_block_map.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/task_notion_document_page_map.py` & `dart_tools-0.5.7/dart/generated/models/task_notion_document_page_map.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/task_properties.py` & `dart_tools-0.5.7/dart/generated/models/task_properties.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/task_source_type.py` & `dart_tools-0.5.7/dart/generated/models/task_source_type.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/task_update.py` & `dart_tools-0.5.7/dart/generated/models/task_update.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from dateutil.parser import isoparse
 
 from ..models.priority import Priority
-from ..models.recommendation_status import RecommendationStatus
 from ..models.task_source_type import TaskSourceType
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="TaskUpdate")
 
 
 @_attrs_define
@@ -43,16 +42,14 @@
             * `AppRoadmapTimeline` - APP_ROADMAP_TIMELINE
             * `ExternalForm` - EXTERNAL_FORM Default: TaskSourceType.UNKNOWN.
         source_form_duid (Union[Unset, None, str]):
         created_by_duid (Union[Unset, None, str]):
         updated_by_duid (Union[Unset, None, str]):
         drafter_duid (Union[Unset, None, str]):
         in_trash (Union[Unset, bool]):
-        recommendation_status (Union[Unset, None, RecommendationStatus]): * `Accepted` - ACCEPTED
-            * `Declined` - DECLINED
         dartboard_duid (Union[Unset, str]):
         order (Union[Unset, str]):
         title (Union[Unset, str]):
         description (Union[Unset, Any]):
         description_markdown (Union[Unset, str]):
         status_duid (Union[Unset, str]):
         assigned_to_ai (Union[Unset, bool]):
@@ -76,15 +73,14 @@
     duid: str
     source_type: Union[Unset, TaskSourceType] = TaskSourceType.UNKNOWN
     source_form_duid: Union[Unset, None, str] = UNSET
     created_by_duid: Union[Unset, None, str] = UNSET
     updated_by_duid: Union[Unset, None, str] = UNSET
     drafter_duid: Union[Unset, None, str] = UNSET
     in_trash: Union[Unset, bool] = UNSET
-    recommendation_status: Union[Unset, None, RecommendationStatus] = UNSET
     dartboard_duid: Union[Unset, str] = UNSET
     order: Union[Unset, str] = UNSET
     title: Union[Unset, str] = UNSET
     description: Union[Unset, Any] = UNSET
     description_markdown: Union[Unset, str] = UNSET
     status_duid: Union[Unset, str] = UNSET
     assigned_to_ai: Union[Unset, bool] = UNSET
@@ -109,18 +105,14 @@
             source_type = self.source_type.value
 
         source_form_duid = self.source_form_duid
         created_by_duid = self.created_by_duid
         updated_by_duid = self.updated_by_duid
         drafter_duid = self.drafter_duid
         in_trash = self.in_trash
-        recommendation_status: Union[Unset, None, str] = UNSET
-        if not isinstance(self.recommendation_status, Unset):
-            recommendation_status = self.recommendation_status.value if self.recommendation_status else None
-
         dartboard_duid = self.dartboard_duid
         order = self.order
         title = self.title
         description = self.description
         description_markdown = self.description_markdown
         status_duid = self.status_duid
         assigned_to_ai = self.assigned_to_ai
@@ -179,16 +171,14 @@
             field_dict["createdByDuid"] = created_by_duid
         if updated_by_duid is not UNSET:
             field_dict["updatedByDuid"] = updated_by_duid
         if drafter_duid is not UNSET:
             field_dict["drafterDuid"] = drafter_duid
         if in_trash is not UNSET:
             field_dict["inTrash"] = in_trash
-        if recommendation_status is not UNSET:
-            field_dict["recommendationStatus"] = recommendation_status
         if dartboard_duid is not UNSET:
             field_dict["dartboardDuid"] = dartboard_duid
         if order is not UNSET:
             field_dict["order"] = order
         if title is not UNSET:
             field_dict["title"] = title
         if description is not UNSET:
@@ -244,23 +234,14 @@
 
         updated_by_duid = d.pop("updatedByDuid", UNSET)
 
         drafter_duid = d.pop("drafterDuid", UNSET)
 
         in_trash = d.pop("inTrash", UNSET)
 
-        _recommendation_status = d.pop("recommendationStatus", UNSET)
-        recommendation_status: Union[Unset, None, RecommendationStatus]
-        if _recommendation_status is None:
-            recommendation_status = None
-        elif isinstance(_recommendation_status, Unset):
-            recommendation_status = UNSET
-        else:
-            recommendation_status = RecommendationStatus(_recommendation_status)
-
         dartboard_duid = d.pop("dartboardDuid", UNSET)
 
         order = d.pop("order", UNSET)
 
         title = d.pop("title", UNSET)
 
         description = d.pop("description", UNSET)
@@ -334,15 +315,14 @@
             duid=duid,
             source_type=source_type,
             source_form_duid=source_form_duid,
             created_by_duid=created_by_duid,
             updated_by_duid=updated_by_duid,
             drafter_duid=drafter_duid,
             in_trash=in_trash,
-            recommendation_status=recommendation_status,
             dartboard_duid=dartboard_duid,
             order=order,
             title=title,
             description=description,
             description_markdown=description_markdown,
             status_duid=status_duid,
             assigned_to_ai=assigned_to_ai,
```

### Comparing `dart_tools-0.5.6/dart/generated/models/tenant.py` & `dart_tools-0.5.7/dart/generated/models/tenant.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,93 +1,94 @@
+import datetime
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Type, TypeVar
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
+from dateutil.parser import isoparse
 
 from ..models.subscription import Subscription
 
 if TYPE_CHECKING:
     from ..models.discord_integration import DiscordIntegration
     from ..models.github_integration import GithubIntegration
     from ..models.notion_integration import NotionIntegration
     from ..models.slack_integration import SlackIntegration
-    from ..models.yc_integration import YcIntegration
     from ..models.zapier_integration import ZapierIntegration
 
 
 T = TypeVar("T", bound="Tenant")
 
 
 @_attrs_define
 class Tenant:
     """
     Attributes:
         duid (str):
         is_dart (bool):
         name (str):
+        created_at (datetime.datetime):
         timezone (str):
         subscription (Subscription): * `Personal` - PERSONAL
             * `Premium` - PREMIUM
         entitlement_overrides (Any):
         backlog_enabled (bool):
         ai_assignment_enabled (bool):
         email_integration_enabled (bool):
         copy_parent_fields_on_create (bool):
         webhook_enabled (bool):
         webhook_secret (str):
         image_url (Optional[str]):
         webhook_url (Optional[str]):
-        yc (Optional[YcIntegration]):
         notion_integration (Optional[NotionIntegration]):
         slack_integration (Optional[SlackIntegration]):
         discord_integration (Optional[DiscordIntegration]):
         github_integration (Optional[GithubIntegration]):
         zapier_integration (Optional[ZapierIntegration]):
     """
 
     duid: str
     is_dart: bool
     name: str
+    created_at: datetime.datetime
     timezone: str
     subscription: Subscription
     entitlement_overrides: Any
     backlog_enabled: bool
     ai_assignment_enabled: bool
     email_integration_enabled: bool
     copy_parent_fields_on_create: bool
     webhook_enabled: bool
     webhook_secret: str
     image_url: Optional[str]
     webhook_url: Optional[str]
-    yc: Optional["YcIntegration"]
     notion_integration: Optional["NotionIntegration"]
     slack_integration: Optional["SlackIntegration"]
     discord_integration: Optional["DiscordIntegration"]
     github_integration: Optional["GithubIntegration"]
     zapier_integration: Optional["ZapierIntegration"]
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         duid = self.duid
         is_dart = self.is_dart
         name = self.name
+        created_at = self.created_at.isoformat()
+
         timezone = self.timezone
         subscription = self.subscription.value
 
         entitlement_overrides = self.entitlement_overrides
         backlog_enabled = self.backlog_enabled
         ai_assignment_enabled = self.ai_assignment_enabled
         email_integration_enabled = self.email_integration_enabled
         copy_parent_fields_on_create = self.copy_parent_fields_on_create
         webhook_enabled = self.webhook_enabled
         webhook_secret = self.webhook_secret
         image_url = self.image_url
         webhook_url = self.webhook_url
-        yc = self.yc.to_dict() if self.yc else None
-
         notion_integration = self.notion_integration.to_dict() if self.notion_integration else None
 
         slack_integration = self.slack_integration.to_dict() if self.slack_integration else None
 
         discord_integration = self.discord_integration.to_dict() if self.discord_integration else None
 
         github_integration = self.github_integration.to_dict() if self.github_integration else None
@@ -97,26 +98,26 @@
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "duid": duid,
                 "isDart": is_dart,
                 "name": name,
+                "createdAt": created_at,
                 "timezone": timezone,
                 "subscription": subscription,
                 "entitlementOverrides": entitlement_overrides,
                 "backlogEnabled": backlog_enabled,
                 "aiAssignmentEnabled": ai_assignment_enabled,
                 "emailIntegrationEnabled": email_integration_enabled,
                 "copyParentFieldsOnCreate": copy_parent_fields_on_create,
                 "webhookEnabled": webhook_enabled,
                 "webhookSecret": webhook_secret,
                 "imageUrl": image_url,
                 "webhookUrl": webhook_url,
-                "yc": yc,
                 "notionIntegration": notion_integration,
                 "slackIntegration": slack_integration,
                 "discordIntegration": discord_integration,
                 "githubIntegration": github_integration,
                 "zapierIntegration": zapier_integration,
             }
         )
@@ -125,24 +126,25 @@
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.discord_integration import DiscordIntegration
         from ..models.github_integration import GithubIntegration
         from ..models.notion_integration import NotionIntegration
         from ..models.slack_integration import SlackIntegration
-        from ..models.yc_integration import YcIntegration
         from ..models.zapier_integration import ZapierIntegration
 
         d = src_dict.copy()
         duid = d.pop("duid")
 
         is_dart = d.pop("isDart")
 
         name = d.pop("name")
 
+        created_at = isoparse(d.pop("createdAt"))
+
         timezone = d.pop("timezone")
 
         subscription = Subscription(d.pop("subscription"))
 
         entitlement_overrides = d.pop("entitlementOverrides")
 
         backlog_enabled = d.pop("backlogEnabled")
@@ -157,21 +159,14 @@
 
         webhook_secret = d.pop("webhookSecret")
 
         image_url = d.pop("imageUrl")
 
         webhook_url = d.pop("webhookUrl")
 
-        _yc = d.pop("yc")
-        yc: Optional[YcIntegration]
-        if _yc is None:
-            yc = None
-        else:
-            yc = YcIntegration.from_dict(_yc)
-
         _notion_integration = d.pop("notionIntegration")
         notion_integration: Optional[NotionIntegration]
         if _notion_integration is None:
             notion_integration = None
         else:
             notion_integration = NotionIntegration.from_dict(_notion_integration)
 
@@ -203,26 +198,26 @@
         else:
             zapier_integration = ZapierIntegration.from_dict(_zapier_integration)
 
         tenant = cls(
             duid=duid,
             is_dart=is_dart,
             name=name,
+            created_at=created_at,
             timezone=timezone,
             subscription=subscription,
             entitlement_overrides=entitlement_overrides,
             backlog_enabled=backlog_enabled,
             ai_assignment_enabled=ai_assignment_enabled,
             email_integration_enabled=email_integration_enabled,
             copy_parent_fields_on_create=copy_parent_fields_on_create,
             webhook_enabled=webhook_enabled,
             webhook_secret=webhook_secret,
             image_url=image_url,
             webhook_url=webhook_url,
-            yc=yc,
             notion_integration=notion_integration,
             slack_integration=slack_integration,
             discord_integration=discord_integration,
             github_integration=github_integration,
             zapier_integration=zapier_integration,
         )
```

### Comparing `dart_tools-0.5.6/dart/generated/models/tenant_update.py` & `dart_tools-0.5.7/dart/generated/models/tenant_update.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/transaction.py` & `dart_tools-0.5.7/dart/generated/models/transaction.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/transaction_kind.py` & `dart_tools-0.5.7/dart/generated/models/transaction_kind.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/transaction_response.py` & `dart_tools-0.5.7/dart/generated/models/transaction_response.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/user.py` & `dart_tools-0.5.7/dart/generated/models/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,15 @@
             * `Light Orange` - LIGHT_ORANGE
             * `Light Pink` - LIGHT_PINK
             * `Tan` - TAN
             * `Dark Gray` - DARK_GRAY
             * `Light Brown` - LIGHT_BROWN
             * `Light Gray` - LIGHT_GRAY
         sections (Any):
+        layout (Any):
         is_admin (bool):
         updated_by_client_duid (Union[Unset, None, str]):
         image_url (Optional[str]):
         auth_token (Optional[str]):
         google_data (Optional[GoogleData]):
     """
 
@@ -72,14 +73,15 @@
     role: UserRole
     email: str
     name: str
     abrev: str
     theme: Theme
     color_name: ColorName
     sections: Any
+    layout: Any
     is_admin: bool
     image_url: Optional[str]
     auth_token: Optional[str]
     google_data: Optional["GoogleData"]
     updated_by_client_duid: Union[Unset, None, str] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
@@ -93,14 +95,15 @@
         name = self.name
         abrev = self.abrev
         theme = self.theme.value
 
         color_name = self.color_name.value
 
         sections = self.sections
+        layout = self.layout
         is_admin = self.is_admin
         updated_by_client_duid = self.updated_by_client_duid
         image_url = self.image_url
         auth_token = self.auth_token
         google_data = self.google_data.to_dict() if self.google_data else None
 
         field_dict: Dict[str, Any] = {}
@@ -112,14 +115,15 @@
                 "role": role,
                 "email": email,
                 "name": name,
                 "abrev": abrev,
                 "theme": theme,
                 "colorName": color_name,
                 "sections": sections,
+                "layout": layout,
                 "isAdmin": is_admin,
                 "imageUrl": image_url,
                 "authToken": auth_token,
                 "googleData": google_data,
             }
         )
         if updated_by_client_duid is not UNSET:
@@ -146,14 +150,16 @@
 
         theme = Theme(d.pop("theme"))
 
         color_name = ColorName(d.pop("colorName"))
 
         sections = d.pop("sections")
 
+        layout = d.pop("layout")
+
         is_admin = d.pop("isAdmin")
 
         updated_by_client_duid = d.pop("updatedByClientDuid", UNSET)
 
         image_url = d.pop("imageUrl")
 
         auth_token = d.pop("authToken")
@@ -171,14 +177,15 @@
             role=role,
             email=email,
             name=name,
             abrev=abrev,
             theme=theme,
             color_name=color_name,
             sections=sections,
+            layout=layout,
             is_admin=is_admin,
             updated_by_client_duid=updated_by_client_duid,
             image_url=image_url,
             auth_token=auth_token,
             google_data=google_data,
         )
```

### Comparing `dart_tools-0.5.6/dart/generated/models/user_dartboard_layout.py` & `dart_tools-0.5.7/dart/generated/models/validation_error_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,55 @@
-from typing import Any, Dict, List, Type, TypeVar
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
-T = TypeVar("T", bound="UserDartboardLayout")
+if TYPE_CHECKING:
+    from ..models.validation_error_response_items import ValidationErrorResponseItems
+
+
+T = TypeVar("T", bound="ValidationErrorResponse")
 
 
 @_attrs_define
-class UserDartboardLayout:
+class ValidationErrorResponse:
     """
     Attributes:
-        user_duid (str):
-        layout_duid (str):
+        items (ValidationErrorResponseItems):
     """
 
-    user_duid: str
-    layout_duid: str
+    items: "ValidationErrorResponseItems"
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        user_duid = self.user_duid
-        layout_duid = self.layout_duid
+        items = self.items.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "userDuid": user_duid,
-                "layoutDuid": layout_duid,
+                "items": items,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        user_duid = d.pop("userDuid")
+        from ..models.validation_error_response_items import ValidationErrorResponseItems
 
-        layout_duid = d.pop("layoutDuid")
+        d = src_dict.copy()
+        items = ValidationErrorResponseItems.from_dict(d.pop("items"))
 
-        user_dartboard_layout = cls(
-            user_duid=user_duid,
-            layout_duid=layout_duid,
+        validation_error_response = cls(
+            items=items,
         )
 
-        user_dartboard_layout.additional_properties = d
-        return user_dartboard_layout
+        validation_error_response.additional_properties = d
+        return validation_error_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart_tools-0.5.6/dart/generated/models/user_dartboard_layout_create.py` & `dart_tools-0.5.7/dart/generated/models/user_dartboard_layout_create.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/user_data_entity_retrieve_entity_kind.py` & `dart_tools-0.5.7/dart/generated/models/user_data_entity_retrieve_entity_kind.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/user_update.py` & `dart_tools-0.5.7/dart/generated/models/user_update.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,28 +46,30 @@
             * `Tan` - TAN
             * `Dark Gray` - DARK_GRAY
             * `Light Brown` - LIGHT_BROWN
             * `Light Gray` - LIGHT_GRAY
         open_in_native_app (Union[Unset, bool]):
         first_day_of_week (Union[Unset, int]):
         sections (Union[Unset, Any]):
+        layout (Union[Unset, Any]):
         notification_default (Union[Unset, bool]):
         notification_in_app (Union[Unset, bool]):
         notification_email (Union[Unset, bool]):
         notification_slack (Union[Unset, bool]):
     """
 
     duid: str
     role: Union[Unset, UserRole] = UNSET
     name: Union[Unset, str] = UNSET
     theme: Union[Unset, Theme] = UNSET
     color_name: Union[Unset, ColorName] = UNSET
     open_in_native_app: Union[Unset, bool] = UNSET
     first_day_of_week: Union[Unset, int] = UNSET
     sections: Union[Unset, Any] = UNSET
+    layout: Union[Unset, Any] = UNSET
     notification_default: Union[Unset, bool] = UNSET
     notification_in_app: Union[Unset, bool] = UNSET
     notification_email: Union[Unset, bool] = UNSET
     notification_slack: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
@@ -84,14 +86,15 @@
         color_name: Union[Unset, str] = UNSET
         if not isinstance(self.color_name, Unset):
             color_name = self.color_name.value
 
         open_in_native_app = self.open_in_native_app
         first_day_of_week = self.first_day_of_week
         sections = self.sections
+        layout = self.layout
         notification_default = self.notification_default
         notification_in_app = self.notification_in_app
         notification_email = self.notification_email
         notification_slack = self.notification_slack
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
@@ -110,14 +113,16 @@
             field_dict["colorName"] = color_name
         if open_in_native_app is not UNSET:
             field_dict["openInNativeApp"] = open_in_native_app
         if first_day_of_week is not UNSET:
             field_dict["firstDayOfWeek"] = first_day_of_week
         if sections is not UNSET:
             field_dict["sections"] = sections
+        if layout is not UNSET:
+            field_dict["layout"] = layout
         if notification_default is not UNSET:
             field_dict["notificationDefault"] = notification_default
         if notification_in_app is not UNSET:
             field_dict["notificationInApp"] = notification_in_app
         if notification_email is not UNSET:
             field_dict["notificationEmail"] = notification_email
         if notification_slack is not UNSET:
@@ -155,14 +160,16 @@
 
         open_in_native_app = d.pop("openInNativeApp", UNSET)
 
         first_day_of_week = d.pop("firstDayOfWeek", UNSET)
 
         sections = d.pop("sections", UNSET)
 
+        layout = d.pop("layout", UNSET)
+
         notification_default = d.pop("notificationDefault", UNSET)
 
         notification_in_app = d.pop("notificationInApp", UNSET)
 
         notification_email = d.pop("notificationEmail", UNSET)
 
         notification_slack = d.pop("notificationSlack", UNSET)
@@ -172,14 +179,15 @@
             role=role,
             name=name,
             theme=theme,
             color_name=color_name,
             open_in_native_app=open_in_native_app,
             first_day_of_week=first_day_of_week,
             sections=sections,
+            layout=layout,
             notification_default=notification_default,
             notification_in_app=notification_in_app,
             notification_email=notification_email,
             notification_slack=notification_slack,
         )
 
         user_update.additional_properties = d
```

### Comparing `dart_tools-0.5.6/dart/generated/models/validation_error_response_items.py` & `dart_tools-0.5.7/dart/generated/models/validation_error_response_items.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/models/view.py` & `dart_tools-0.5.7/dart/generated/models/view.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         duid (str):
         kind (ViewKind): * `Custom` - CUSTOM
             * `Search` - SEARCH
             * `Trash` - TRASH
             * `My tasks` - MY_TASKS
         accessible_by_team (bool):
         accessible_by_user_duids (List[str]):
+        public (bool):
         order (str):
         title (str):
         description (str):
         icon_kind (IconKind): * `None` - NONE
             * `Icon` - ICON
             * `Emoji` - EMOJI
         icon_name_or_emoji (str):
@@ -60,14 +61,15 @@
         updated_by_client_duid (Union[Unset, None, str]):
     """
 
     duid: str
     kind: ViewKind
     accessible_by_team: bool
     accessible_by_user_duids: List[str]
+    public: bool
     order: str
     title: str
     description: str
     icon_kind: IconKind
     icon_name_or_emoji: str
     color_name: ColorName
     layout_duid: str
@@ -80,14 +82,15 @@
     def to_dict(self) -> Dict[str, Any]:
         duid = self.duid
         kind = self.kind.value
 
         accessible_by_team = self.accessible_by_team
         accessible_by_user_duids = self.accessible_by_user_duids
 
+        public = self.public
         order = self.order
         title = self.title
         description = self.description
         icon_kind = self.icon_kind.value
 
         icon_name_or_emoji = self.icon_name_or_emoji
         color_name = self.color_name.value
@@ -105,14 +108,15 @@
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "duid": duid,
                 "kind": kind,
                 "accessibleByTeam": accessible_by_team,
                 "accessibleByUserDuids": accessible_by_user_duids,
+                "public": public,
                 "order": order,
                 "title": title,
                 "description": description,
                 "iconKind": icon_kind,
                 "iconNameOrEmoji": icon_name_or_emoji,
                 "colorName": color_name,
                 "layoutDuid": layout_duid,
@@ -133,14 +137,16 @@
 
         kind = ViewKind(d.pop("kind"))
 
         accessible_by_team = d.pop("accessibleByTeam")
 
         accessible_by_user_duids = cast(List[str], d.pop("accessibleByUserDuids"))
 
+        public = d.pop("public")
+
         order = d.pop("order")
 
         title = d.pop("title")
 
         description = d.pop("description")
 
         icon_kind = IconKind(d.pop("iconKind"))
@@ -160,14 +166,15 @@
         updated_by_client_duid = d.pop("updatedByClientDuid", UNSET)
 
         view = cls(
             duid=duid,
             kind=kind,
             accessible_by_team=accessible_by_team,
             accessible_by_user_duids=accessible_by_user_duids,
+            public=public,
             order=order,
             title=title,
             description=description,
             icon_kind=icon_kind,
             icon_name_or_emoji=icon_name_or_emoji,
             color_name=color_name,
             layout_duid=layout_duid,
```

### Comparing `dart_tools-0.5.6/dart/generated/models/view_create.py` & `dart_tools-0.5.7/dart/generated/models/view_create.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     """
     Attributes:
         duid (str):
         order (str):
         layout_duid (str):
         accessible_by_team (Union[Unset, bool]):
         accessible_by_user_duids (Union[Unset, List[str]]):
+        public (Union[Unset, bool]):
         title (Union[Unset, str]):
         description (Union[Unset, str]):
         icon_kind (Union[Unset, IconKind]): * `None` - NONE
             * `Icon` - ICON
             * `Emoji` - EMOJI
         icon_name_or_emoji (Union[Unset, str]):
         color_name (Union[Unset, ColorName]): * `Red` - RED
@@ -55,14 +56,15 @@
     """
 
     duid: str
     order: str
     layout_duid: str
     accessible_by_team: Union[Unset, bool] = UNSET
     accessible_by_user_duids: Union[Unset, List[str]] = UNSET
+    public: Union[Unset, bool] = UNSET
     title: Union[Unset, str] = UNSET
     description: Union[Unset, str] = UNSET
     icon_kind: Union[Unset, IconKind] = UNSET
     icon_name_or_emoji: Union[Unset, str] = UNSET
     color_name: Union[Unset, ColorName] = UNSET
     favorited_by_user_duids: Union[Unset, List[str]] = UNSET
     always_shown_property_duids: Union[Unset, List[str]] = UNSET
@@ -74,14 +76,15 @@
         order = self.order
         layout_duid = self.layout_duid
         accessible_by_team = self.accessible_by_team
         accessible_by_user_duids: Union[Unset, List[str]] = UNSET
         if not isinstance(self.accessible_by_user_duids, Unset):
             accessible_by_user_duids = self.accessible_by_user_duids
 
+        public = self.public
         title = self.title
         description = self.description
         icon_kind: Union[Unset, str] = UNSET
         if not isinstance(self.icon_kind, Unset):
             icon_kind = self.icon_kind.value
 
         icon_name_or_emoji = self.icon_name_or_emoji
@@ -110,14 +113,16 @@
                 "layoutDuid": layout_duid,
             }
         )
         if accessible_by_team is not UNSET:
             field_dict["accessibleByTeam"] = accessible_by_team
         if accessible_by_user_duids is not UNSET:
             field_dict["accessibleByUserDuids"] = accessible_by_user_duids
+        if public is not UNSET:
+            field_dict["public"] = public
         if title is not UNSET:
             field_dict["title"] = title
         if description is not UNSET:
             field_dict["description"] = description
         if icon_kind is not UNSET:
             field_dict["iconKind"] = icon_kind
         if icon_name_or_emoji is not UNSET:
@@ -142,14 +147,16 @@
 
         layout_duid = d.pop("layoutDuid")
 
         accessible_by_team = d.pop("accessibleByTeam", UNSET)
 
         accessible_by_user_duids = cast(List[str], d.pop("accessibleByUserDuids", UNSET))
 
+        public = d.pop("public", UNSET)
+
         title = d.pop("title", UNSET)
 
         description = d.pop("description", UNSET)
 
         _icon_kind = d.pop("iconKind", UNSET)
         icon_kind: Union[Unset, IconKind]
         if isinstance(_icon_kind, Unset):
@@ -174,14 +181,15 @@
 
         view_create = cls(
             duid=duid,
             order=order,
             layout_duid=layout_duid,
             accessible_by_team=accessible_by_team,
             accessible_by_user_duids=accessible_by_user_duids,
+            public=public,
             title=title,
             description=description,
             icon_kind=icon_kind,
             icon_name_or_emoji=icon_name_or_emoji,
             color_name=color_name,
             favorited_by_user_duids=favorited_by_user_duids,
             always_shown_property_duids=always_shown_property_duids,
```

### Comparing `dart_tools-0.5.6/dart/generated/models/view_update.py` & `dart_tools-0.5.7/dart/generated/models/view_update.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 @_attrs_define
 class ViewUpdate:
     """
     Attributes:
         duid (str):
         accessible_by_team (Union[Unset, bool]):
         accessible_by_user_duids (Union[Unset, List[str]]):
+        public (Union[Unset, bool]):
         order (Union[Unset, str]):
         title (Union[Unset, str]):
         description (Union[Unset, str]):
         icon_kind (Union[Unset, IconKind]): * `None` - NONE
             * `Icon` - ICON
             * `Emoji` - EMOJI
         icon_name_or_emoji (Union[Unset, str]):
@@ -53,14 +54,15 @@
         always_shown_property_duids (Union[Unset, List[str]]):
         always_hidden_property_duids (Union[Unset, List[str]]):
     """
 
     duid: str
     accessible_by_team: Union[Unset, bool] = UNSET
     accessible_by_user_duids: Union[Unset, List[str]] = UNSET
+    public: Union[Unset, bool] = UNSET
     order: Union[Unset, str] = UNSET
     title: Union[Unset, str] = UNSET
     description: Union[Unset, str] = UNSET
     icon_kind: Union[Unset, IconKind] = UNSET
     icon_name_or_emoji: Union[Unset, str] = UNSET
     color_name: Union[Unset, ColorName] = UNSET
     layout_duid: Union[Unset, str] = UNSET
@@ -72,14 +74,15 @@
     def to_dict(self) -> Dict[str, Any]:
         duid = self.duid
         accessible_by_team = self.accessible_by_team
         accessible_by_user_duids: Union[Unset, List[str]] = UNSET
         if not isinstance(self.accessible_by_user_duids, Unset):
             accessible_by_user_duids = self.accessible_by_user_duids
 
+        public = self.public
         order = self.order
         title = self.title
         description = self.description
         icon_kind: Union[Unset, str] = UNSET
         if not isinstance(self.icon_kind, Unset):
             icon_kind = self.icon_kind.value
 
@@ -108,14 +111,16 @@
                 "duid": duid,
             }
         )
         if accessible_by_team is not UNSET:
             field_dict["accessibleByTeam"] = accessible_by_team
         if accessible_by_user_duids is not UNSET:
             field_dict["accessibleByUserDuids"] = accessible_by_user_duids
+        if public is not UNSET:
+            field_dict["public"] = public
         if order is not UNSET:
             field_dict["order"] = order
         if title is not UNSET:
             field_dict["title"] = title
         if description is not UNSET:
             field_dict["description"] = description
         if icon_kind is not UNSET:
@@ -140,14 +145,16 @@
         d = src_dict.copy()
         duid = d.pop("duid")
 
         accessible_by_team = d.pop("accessibleByTeam", UNSET)
 
         accessible_by_user_duids = cast(List[str], d.pop("accessibleByUserDuids", UNSET))
 
+        public = d.pop("public", UNSET)
+
         order = d.pop("order", UNSET)
 
         title = d.pop("title", UNSET)
 
         description = d.pop("description", UNSET)
 
         _icon_kind = d.pop("iconKind", UNSET)
@@ -174,14 +181,15 @@
 
         always_hidden_property_duids = cast(List[str], d.pop("alwaysHiddenPropertyDuids", UNSET))
 
         view_update = cls(
             duid=duid,
             accessible_by_team=accessible_by_team,
             accessible_by_user_duids=accessible_by_user_duids,
+            public=public,
             order=order,
             title=title,
             description=description,
             icon_kind=icon_kind,
             icon_name_or_emoji=icon_name_or_emoji,
             color_name=color_name,
             layout_duid=layout_duid,
```

### Comparing `dart_tools-0.5.6/dart/generated/models/zapier_integration.py` & `dart_tools-0.5.7/dart/generated/models/zapier_integration.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/generated/types.py` & `dart_tools-0.5.7/dart/generated/types.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/order_manager.py` & `dart_tools-0.5.7/dart/order_manager.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart/webhook.py` & `dart_tools-0.5.7/dart/webhook.py`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/dart_tools.egg-info/PKG-INFO` & `dart_tools-0.5.7/dart_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dart-tools
-Version: 0.5.6
+Version: 0.5.7
 Summary: The Dart CLI and Python Library
 Author-email: Dart Software Team <software@itsdart.com>
 License: MIT License
         
         Copyright (c) 2023 Dart
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dart-tools Version: 0.5.6 Summary: The Dart CLI and
+Metadata-Version: 2.1 Name: dart-tools Version: 0.5.7 Summary: The Dart CLI and
 Python Library Author-email: Dart Software Team
 itsdart.com> License: MIT License Copyright (c) 2023 Dart Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `dart_tools-0.5.6/dart_tools.egg-info/SOURCES.txt` & `dart_tools-0.5.7/dart_tools.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 dart/generated/api/__init__.py
 dart/generated/api/transactions/__init__.py
 dart/generated/api/transactions/transactions_create.py
 dart/generated/models/__init__.py
 dart/generated/models/attachment.py
 dart/generated/models/attachment_create.py
 dart/generated/models/attachment_update.py
-dart/generated/models/batch.py
 dart/generated/models/brainstorm.py
 dart/generated/models/brainstorm_create.py
 dart/generated/models/brainstorm_state.py
 dart/generated/models/brainstorm_update.py
 dart/generated/models/color_name.py
 dart/generated/models/comment.py
 dart/generated/models/comment_create.py
@@ -109,15 +108,14 @@
 dart/generated/models/paginated_view_list.py
 dart/generated/models/priority.py
 dart/generated/models/properties_list_kind.py
 dart/generated/models/property_.py
 dart/generated/models/property_create.py
 dart/generated/models/property_kind.py
 dart/generated/models/property_update.py
-dart/generated/models/recommendation_status.py
 dart/generated/models/relationship.py
 dart/generated/models/relationship_create.py
 dart/generated/models/relationship_kind.py
 dart/generated/models/relationship_kind_create.py
 dart/generated/models/relationship_kind_kind.py
 dart/generated/models/relationship_kind_update.py
 dart/generated/models/report_kind.py
@@ -169,15 +167,14 @@
 dart/generated/models/user_update.py
 dart/generated/models/validation_error_response.py
 dart/generated/models/validation_error_response_items.py
 dart/generated/models/view.py
 dart/generated/models/view_create.py
 dart/generated/models/view_kind.py
 dart/generated/models/view_update.py
-dart/generated/models/yc_integration.py
 dart/generated/models/zapier_integration.py
 dart_tools.egg-info/PKG-INFO
 dart_tools.egg-info/SOURCES.txt
 dart_tools.egg-info/dependency_links.txt
 dart_tools.egg-info/entry_points.txt
 dart_tools.egg-info/requires.txt
 dart_tools.egg-info/top_level.txt
```

### Comparing `dart_tools-0.5.6/dart_tools.egg-info/dist/dart-tools-0.3.3.tar.gz` & `dart_tools-0.5.7/dart_tools.egg-info/dist/dart-tools-0.3.3.tar.gz`

 * *Files identical despite different names*

### Comparing `dart_tools-0.5.6/pyproject.toml` & `dart_tools-0.5.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dart-tools"
-version = "0.5.6"
+version = "0.5.7"
 description = "The Dart CLI and Python Library"
 readme = "README.md"
 requires-python = ">=3.8"
 
 license = {file = "LICENSE"}
 keywords = ["dart", "cli", "projectmanagement", "taskmanagement"]
 authors = [
```

