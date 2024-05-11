# Comparing `tmp/xingchen-1.1.1.tar.gz` & `tmp/xingchen-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xingchen-1.1.1.tar", last modified: Thu May  2 15:18:37 2024, max compression
+gzip compressed data, was "xingchen-1.1.2.tar", last modified: Sat May 11 01:41:23 2024, max compression
```

## Comparing `xingchen-1.1.1.tar` & `xingchen-1.1.2.tar`

### file list

```diff
@@ -1,150 +1,164 @@
-drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-02 15:18:37.538490 xingchen-1.1.1/
--rw-r--r--   0 frankin    (501) staff       (20)      333 2024-05-02 15:18:37.538590 xingchen-1.1.1/PKG-INFO
--rw-r--r--   0 frankin    (501) staff       (20)    11848 2024-05-02 15:15:25.000000 xingchen-1.1.1/README.md
--rw-r--r--   0 frankin    (501) staff       (20)      771 2024-05-02 15:02:56.000000 xingchen-1.1.1/pyproject.toml
--rw-r--r--   0 frankin    (501) staff       (20)       69 2024-05-02 15:18:37.538930 xingchen-1.1.1/setup.cfg
--rw-r--r--   0 frankin    (501) staff       (20)     1152 2024-05-02 15:03:02.000000 xingchen-1.1.1/setup.py
-drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-02 15:18:37.486548 xingchen-1.1.1/test/
--rw-r--r--   0 frankin    (501) staff       (20)     1655 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_advanced_settings.py
--rw-r--r--   0 frankin    (501) staff       (20)     2985 2024-03-05 07:23:56.000000 xingchen-1.1.1/test/test_base_chat_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     3120 2024-04-11 03:27:03.000000 xingchen-1.1.1/test/test_base_chat_request_aca_chat_ext_param.py
--rw-r--r--   0 frankin    (501) staff       (20)     2206 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_character_advanced_config.py
--rw-r--r--   0 frankin    (501) staff       (20)     3105 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_character_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)     3052 2024-03-05 07:24:20.000000 xingchen-1.1.1/test/test_character_create_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     3728 2024-03-05 07:23:29.000000 xingchen-1.1.1/test/test_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1448 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_character_key.py
--rw-r--r--   0 frankin    (501) staff       (20)     1734 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_character_permission_config.py
--rw-r--r--   0 frankin    (501) staff       (20)     1742 2024-03-05 07:24:07.000000 xingchen-1.1.1/test/test_character_query_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1533 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_character_query_where.py
--rw-r--r--   0 frankin    (501) staff       (20)     3182 2024-03-05 07:24:03.000000 xingchen-1.1.1/test/test_character_update_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     3150 2024-03-05 07:23:52.000000 xingchen-1.1.1/test/test_character_version_create_or_update_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2815 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_chat_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)     2088 2024-03-05 07:23:33.000000 xingchen-1.1.1/test/test_chat_history_query_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1851 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_chat_history_query_where.py
--rw-r--r--   0 frankin    (501) staff       (20)     1786 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_chat_message_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)     2018 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_chat_message_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     4043 2024-03-05 07:25:26.000000 xingchen-1.1.1/test/test_chat_req_params.py
--rw-r--r--   0 frankin    (501) staff       (20)     1549 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_chat_room_user_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1711 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_context.py
--rw-r--r--   0 frankin    (501) staff       (20)     1459 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_file_info_vo.py
--rw-r--r--   0 frankin    (501) staff       (20)     1508 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_gateway_context.py
--rw-r--r--   0 frankin    (501) staff       (20)     1744 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_gateway_issued_params.py
--rw-r--r--   0 frankin    (501) staff       (20)     1798 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_input.py
--rw-r--r--   0 frankin    (501) staff       (20)     1577 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_message.py
--rw-r--r--   0 frankin    (501) staff       (20)     1604 2024-03-05 07:23:48.000000 xingchen-1.1.1/test/test_message_rating_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     1359 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_meta.py
--rw-r--r--   0 frankin    (501) staff       (20)     1608 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_model_parameters.py
--rw-r--r--   0 frankin    (501) staff       (20)     4471 2024-03-05 07:22:54.000000 xingchen-1.1.1/test/test_page_result_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2507 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_page_result_chat_message_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1486 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_repository.py
--rw-r--r--   0 frankin    (501) staff       (20)     1720 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_repository_info.py
--rw-r--r--   0 frankin    (501) staff       (20)     1629 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_result_dto_boolean.py
--rw-r--r--   0 frankin    (501) staff       (20)     4244 2024-03-05 07:23:36.000000 xingchen-1.1.1/test/test_result_dto_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1805 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_result_dto_character_key.py
--rw-r--r--   0 frankin    (501) staff       (20)     4549 2024-03-05 07:22:38.000000 xingchen-1.1.1/test/test_result_dto_list_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     5085 2024-03-05 07:24:24.000000 xingchen-1.1.1/test/test_result_dto_page_result_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2970 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_result_dto_page_result_chat_message_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1368 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_scenario.py
--rw-r--r--   0 frankin    (501) staff       (20)     1654 2024-03-05 07:24:31.000000 xingchen-1.1.1/test/test_sys_reminder_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     1496 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_user_profile.py
-drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-02 15:18:37.489544 xingchen-1.1.1/xingchen/
--rw-r--r--   0 frankin    (501) staff       (20)     6093 2024-04-25 08:50:36.000000 xingchen-1.1.1/xingchen/__init__.py
--rw-r--r--   0 frankin    (501) staff       (20)     3290 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/aca_util.py
-drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-02 15:18:37.493831 xingchen-1.1.1/xingchen/api/
--rw-r--r--   0 frankin    (501) staff       (20)      410 2024-04-25 08:50:36.000000 xingchen-1.1.1/xingchen/api/__init__.py
--rw-r--r--   0 frankin    (501) staff       (20)    60683 2024-04-25 09:41:08.000000 xingchen-1.1.1/xingchen/api/character_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)    12628 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/api/chat_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)     8021 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/api/chat_extract_message_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)    29175 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/api/chat_message_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)     7592 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/api/common_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)     5384 2024-04-11 06:12:19.000000 xingchen-1.1.1/xingchen/api/groupchat_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)    30795 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/api_client.py
--rw-r--r--   0 frankin    (501) staff       (20)      852 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/api_response.py
--rw-r--r--   0 frankin    (501) staff       (20)    15709 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/configuration.py
--rw-r--r--   0 frankin    (501) staff       (20)     5442 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/exceptions.py
-drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-02 15:18:37.534247 xingchen-1.1.1/xingchen/models/
--rw-r--r--   0 frankin    (501) staff       (20)     3374 2024-04-25 05:48:37.000000 xingchen-1.1.1/xingchen/models/__init__.py
--rw-r--r--   0 frankin    (501) staff       (20)     2725 2024-03-05 06:43:53.000000 xingchen-1.1.1/xingchen/models/advanced_settings.py
--rw-r--r--   0 frankin    (501) staff       (20)     2618 2024-04-11 03:27:03.000000 xingchen-1.1.1/xingchen/models/base_chat_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     4766 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/character_advanced_config.py
--rw-r--r--   0 frankin    (501) staff       (20)     4800 2024-03-07 08:00:22.000000 xingchen-1.1.1/xingchen/models/character_create_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2023 2024-04-25 05:48:37.000000 xingchen-1.1.1/xingchen/models/character_desc_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2345 2024-04-25 05:48:37.000000 xingchen-1.1.1/xingchen/models/character_desc_generated_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     7409 2024-03-07 08:02:21.000000 xingchen-1.1.1/xingchen/models/character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2686 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/character_key.py
--rw-r--r--   0 frankin    (501) staff       (20)     2467 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/character_permission_config.py
--rw-r--r--   0 frankin    (501) staff       (20)     3094 2024-03-05 07:28:35.000000 xingchen-1.1.1/xingchen/models/character_query_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2273 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/character_query_where.py
--rw-r--r--   0 frankin    (501) staff       (20)     5138 2024-04-25 09:41:54.000000 xingchen-1.1.1/xingchen/models/character_update_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     4759 2024-04-25 09:19:54.000000 xingchen-1.1.1/xingchen/models/character_version_create_or_update_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2906 2024-03-05 03:00:03.000000 xingchen-1.1.1/xingchen/models/chat_context.py
--rw-r--r--   0 frankin    (501) staff       (20)     3097 2024-03-05 07:28:35.000000 xingchen-1.1.1/xingchen/models/chat_history_query_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2917 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/chat_history_query_where.py
--rw-r--r--   0 frankin    (501) staff       (20)     3943 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/chat_message_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     6915 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/chat_req_params.py
--rw-r--r--   0 frankin    (501) staff       (20)     2722 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/chat_room_user_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     3673 2024-02-04 06:24:45.000000 xingchen-1.1.1/xingchen/models/context.py
-drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-02 15:18:37.536452 xingchen-1.1.1/xingchen/models/custom/
--rw-r--r--   0 frankin    (501) staff       (20)       89 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/custom/__init__.py
--rw-r--r--   0 frankin    (501) staff       (20)     1992 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/custom/base_response.py
--rw-r--r--   0 frankin    (501) staff       (20)     1873 2024-03-05 07:02:49.000000 xingchen-1.1.1/xingchen/models/custom/character_model_parameters.py
--rw-r--r--   0 frankin    (501) staff       (20)     4815 2024-03-05 07:11:26.000000 xingchen-1.1.1/xingchen/models/custom/chat_response.py
-drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-02 15:18:37.538106 xingchen-1.1.1/xingchen/models/custom/groupchat/
--rw-r--r--   0 frankin    (501) staff       (20)       92 2024-04-09 12:57:52.000000 xingchen-1.1.1/xingchen/models/custom/groupchat/__init__.py
--rw-r--r--   0 frankin    (501) staff       (20)     2778 2024-04-11 07:45:59.000000 xingchen-1.1.1/xingchen/models/custom/groupchat/group_chat_ext_param.py
--rw-r--r--   0 frankin    (501) staff       (20)     1763 2024-04-09 13:04:39.000000 xingchen-1.1.1/xingchen/models/custom/groupchat/group_chat_reply_setting.py
--rw-r--r--   0 frankin    (501) staff       (20)     1303 2024-04-11 02:56:10.000000 xingchen-1.1.1/xingchen/models/custom/groupchat/group_chat_room_info.py
--rw-r--r--   0 frankin    (501) staff       (20)     2026 2024-03-06 07:00:38.000000 xingchen-1.1.1/xingchen/models/custom/platform_publish_config.py
--rw-r--r--   0 frankin    (501) staff       (20)     1818 2024-02-01 06:33:25.000000 xingchen-1.1.1/xingchen/models/custom/reset_history_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     1778 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/extract_data.py
--rw-r--r--   0 frankin    (501) staff       (20)     2162 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/extract_kv_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2399 2024-04-25 05:48:37.000000 xingchen-1.1.1/xingchen/models/extract_memory_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     2239 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/extract_summary_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1718 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/file_conver_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1712 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/file_conver_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     2191 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/file_info_vo.py
--rw-r--r--   0 frankin    (501) staff       (20)     7800 2024-02-02 08:00:56.000000 xingchen-1.1.1/xingchen/models/function_call.py
--rw-r--r--   0 frankin    (501) staff       (20)     2239 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/gateway_context.py
--rw-r--r--   0 frankin    (501) staff       (20)     2417 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/gateway_issued_params.py
--rw-r--r--   0 frankin    (501) staff       (20)     2494 2024-04-11 07:26:08.000000 xingchen-1.1.1/xingchen/models/input.py
--rw-r--r--   0 frankin    (501) staff       (20)     1506 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/keyword.py
--rw-r--r--   0 frankin    (501) staff       (20)     1698 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/kv_memory_config.py
--rw-r--r--   0 frankin    (501) staff       (20)     2237 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/long_term_memory.py
--rw-r--r--   0 frankin    (501) staff       (20)     2089 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/memory.py
--rw-r--r--   0 frankin    (501) staff       (20)     1582 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/memory_summary.py
--rw-r--r--   0 frankin    (501) staff       (20)     2692 2024-01-29 06:06:46.000000 xingchen-1.1.1/xingchen/models/message.py
--rw-r--r--   0 frankin    (501) staff       (20)     2251 2024-03-05 07:28:35.000000 xingchen-1.1.1/xingchen/models/message_rating_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     2057 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/meta.py
--rw-r--r--   0 frankin    (501) staff       (20)     2899 2024-01-29 05:42:57.000000 xingchen-1.1.1/xingchen/models/model_parameters.py
--rw-r--r--   0 frankin    (501) staff       (20)     2904 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/page_result_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2929 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/page_result_chat_message_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1681 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/platform_plugin.py
--rw-r--r--   0 frankin    (501) staff       (20)     2009 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/polling_image_detail_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1965 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/reject_answer_plugin.py
--rw-r--r--   0 frankin    (501) staff       (20)     2303 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/reject_condition.py
--rw-r--r--   0 frankin    (501) staff       (20)     2290 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/repository.py
--rw-r--r--   0 frankin    (501) staff       (20)     2719 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/repository_info.py
--rw-r--r--   0 frankin    (501) staff       (20)     2578 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/result_dto_boolean.py
--rw-r--r--   0 frankin    (501) staff       (20)     2561 2024-04-25 05:48:37.000000 xingchen-1.1.1/xingchen/models/result_dto_character_desc_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2893 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/result_dto_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2893 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/result_dto_character_key.py
--rw-r--r--   0 frankin    (501) staff       (20)     2517 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/result_dto_extract_kv_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2573 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/result_dto_extract_summary_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2539 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/result_dto_file_conver_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     3110 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/result_dto_list_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     3015 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/result_dto_page_result_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     3040 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/result_dto_page_result_chat_message_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2617 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/result_dto_polling_image_detail_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2062 2023-11-21 03:10:04.000000 xingchen-1.1.1/xingchen/models/scenario.py
--rw-r--r--   0 frankin    (501) staff       (20)     1702 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/stop_chat_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     2386 2024-03-05 07:28:35.000000 xingchen-1.1.1/xingchen/models/sys_reminder_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     2193 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/text_to_image_plugin.py
--rw-r--r--   0 frankin    (501) staff       (20)     2177 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/user_profile.py
--rw-r--r--   0 frankin    (501) staff       (20)        0 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/py.typed
--rw-r--r--   0 frankin    (501) staff       (20)    12934 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/rest.py
-drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-02 15:18:37.490853 xingchen-1.1.1/xingchen.egg-info/
--rw-r--r--   0 frankin    (501) staff       (20)      333 2024-05-02 15:18:37.000000 xingchen-1.1.1/xingchen.egg-info/PKG-INFO
--rw-r--r--   0 frankin    (501) staff       (20)     5014 2024-05-02 15:18:37.000000 xingchen-1.1.1/xingchen.egg-info/SOURCES.txt
--rw-r--r--   0 frankin    (501) staff       (20)        1 2024-05-02 15:18:37.000000 xingchen-1.1.1/xingchen.egg-info/dependency_links.txt
--rw-r--r--   0 frankin    (501) staff       (20)       85 2024-05-02 15:18:37.000000 xingchen-1.1.1/xingchen.egg-info/requires.txt
--rw-r--r--   0 frankin    (501) staff       (20)        9 2024-05-02 15:18:37.000000 xingchen-1.1.1/xingchen.egg-info/top_level.txt
+drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-11 01:41:23.155467 xingchen-1.1.2/
+-rw-r--r--   0 frankin    (501) staff       (20)      333 2024-05-11 01:41:23.155549 xingchen-1.1.2/PKG-INFO
+-rw-r--r--   0 frankin    (501) staff       (20)    11848 2024-05-02 15:15:25.000000 xingchen-1.1.2/README.md
+-rw-r--r--   0 frankin    (501) staff       (20)      771 2024-05-02 15:02:56.000000 xingchen-1.1.2/pyproject.toml
+-rw-r--r--   0 frankin    (501) staff       (20)       69 2024-05-11 01:41:23.155831 xingchen-1.1.2/setup.cfg
+-rw-r--r--   0 frankin    (501) staff       (20)     1152 2024-05-11 01:40:10.000000 xingchen-1.1.2/setup.py
+drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-11 01:41:23.121679 xingchen-1.1.2/test/
+-rw-r--r--   0 frankin    (501) staff       (20)     1655 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_advanced_settings.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2985 2024-03-05 07:23:56.000000 xingchen-1.1.2/test/test_base_chat_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3120 2024-04-11 03:27:03.000000 xingchen-1.1.2/test/test_base_chat_request_aca_chat_ext_param.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2206 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_character_advanced_config.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3105 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_character_api_sub.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3052 2024-03-05 07:24:20.000000 xingchen-1.1.2/test/test_character_create_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3728 2024-03-05 07:23:29.000000 xingchen-1.1.2/test/test_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1448 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_character_key.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1734 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_character_permission_config.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1742 2024-03-05 07:24:07.000000 xingchen-1.1.2/test/test_character_query_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1533 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_character_query_where.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3182 2024-03-05 07:24:03.000000 xingchen-1.1.2/test/test_character_update_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3150 2024-03-05 07:23:52.000000 xingchen-1.1.2/test/test_character_version_create_or_update_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2815 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_chat_api_sub.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2088 2024-03-05 07:23:33.000000 xingchen-1.1.2/test/test_chat_history_query_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1851 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_chat_history_query_where.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1786 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_chat_message_api_sub.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2018 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_chat_message_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4043 2024-03-05 07:25:26.000000 xingchen-1.1.2/test/test_chat_req_params.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1549 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_chat_room_user_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1711 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_context.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1459 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_file_info_vo.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1508 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_gateway_context.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1744 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_gateway_issued_params.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1798 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_input.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1577 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_message.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1604 2024-03-05 07:23:48.000000 xingchen-1.1.2/test/test_message_rating_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1359 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_meta.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1608 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_model_parameters.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4471 2024-03-05 07:22:54.000000 xingchen-1.1.2/test/test_page_result_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2507 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_page_result_chat_message_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1486 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_repository.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1720 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_repository_info.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1629 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_result_dto_boolean.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4244 2024-03-05 07:23:36.000000 xingchen-1.1.2/test/test_result_dto_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1805 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_result_dto_character_key.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4549 2024-03-05 07:22:38.000000 xingchen-1.1.2/test/test_result_dto_list_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     5085 2024-03-05 07:24:24.000000 xingchen-1.1.2/test/test_result_dto_page_result_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2970 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_result_dto_page_result_chat_message_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1368 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_scenario.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1654 2024-03-05 07:24:31.000000 xingchen-1.1.2/test/test_sys_reminder_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1496 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_user_profile.py
+drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-11 01:41:23.124129 xingchen-1.1.2/xingchen/
+-rw-r--r--   0 frankin    (501) staff       (20)     6865 2024-05-11 01:40:18.000000 xingchen-1.1.2/xingchen/__init__.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3764 2024-05-09 03:46:30.000000 xingchen-1.1.2/xingchen/aca_util.py
+drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-11 01:41:23.128739 xingchen-1.1.2/xingchen/api/
+-rw-r--r--   0 frankin    (501) staff       (20)      410 2024-04-25 08:50:36.000000 xingchen-1.1.2/xingchen/api/__init__.py
+-rw-r--r--   0 frankin    (501) staff       (20)    60683 2024-04-25 09:41:08.000000 xingchen-1.1.2/xingchen/api/character_api_sub.py
+-rw-r--r--   0 frankin    (501) staff       (20)    12628 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/api/chat_api_sub.py
+-rw-r--r--   0 frankin    (501) staff       (20)     8021 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/api/chat_extract_message_api_sub.py
+-rw-r--r--   0 frankin    (501) staff       (20)    29175 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/api/chat_message_api_sub.py
+-rw-r--r--   0 frankin    (501) staff       (20)     7592 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/api/common_api_sub.py
+-rw-r--r--   0 frankin    (501) staff       (20)     5384 2024-04-11 06:12:19.000000 xingchen-1.1.2/xingchen/api/groupchat_api_sub.py
+-rw-r--r--   0 frankin    (501) staff       (20)     5637 2024-05-09 11:02:34.000000 xingchen-1.1.2/xingchen/api/openai_api_sub.py
+-rw-r--r--   0 frankin    (501) staff       (20)    30795 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/api_client.py
+-rw-r--r--   0 frankin    (501) staff       (20)      852 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/api_response.py
+-rw-r--r--   0 frankin    (501) staff       (20)    15709 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/configuration.py
+-rw-r--r--   0 frankin    (501) staff       (20)     5442 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/exceptions.py
+drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-11 01:41:23.148125 xingchen-1.1.2/xingchen/models/
+-rw-r--r--   0 frankin    (501) staff       (20)     3374 2024-04-25 05:48:37.000000 xingchen-1.1.2/xingchen/models/__init__.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2725 2024-03-05 06:43:53.000000 xingchen-1.1.2/xingchen/models/advanced_settings.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2618 2024-04-11 03:27:03.000000 xingchen-1.1.2/xingchen/models/base_chat_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4766 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/character_advanced_config.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4800 2024-03-07 08:00:22.000000 xingchen-1.1.2/xingchen/models/character_create_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2023 2024-04-25 05:48:37.000000 xingchen-1.1.2/xingchen/models/character_desc_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2345 2024-04-25 05:48:37.000000 xingchen-1.1.2/xingchen/models/character_desc_generated_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     7409 2024-03-07 08:02:21.000000 xingchen-1.1.2/xingchen/models/character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2686 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/character_key.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2467 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/character_permission_config.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3094 2024-03-05 07:28:35.000000 xingchen-1.1.2/xingchen/models/character_query_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2273 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/character_query_where.py
+-rw-r--r--   0 frankin    (501) staff       (20)     5138 2024-04-25 09:41:54.000000 xingchen-1.1.2/xingchen/models/character_update_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4759 2024-04-25 09:19:54.000000 xingchen-1.1.2/xingchen/models/character_version_create_or_update_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2906 2024-03-05 03:00:03.000000 xingchen-1.1.2/xingchen/models/chat_context.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3097 2024-03-05 07:28:35.000000 xingchen-1.1.2/xingchen/models/chat_history_query_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2917 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/chat_history_query_where.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3943 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/chat_message_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     6915 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/chat_req_params.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2722 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/chat_room_user_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3673 2024-02-04 06:24:45.000000 xingchen-1.1.2/xingchen/models/context.py
+drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-11 01:41:23.149917 xingchen-1.1.2/xingchen/models/custom/
+-rw-r--r--   0 frankin    (501) staff       (20)       89 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/custom/__init__.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1992 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/custom/base_response.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1873 2024-03-05 07:02:49.000000 xingchen-1.1.2/xingchen/models/custom/character_model_parameters.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4814 2024-05-09 03:25:22.000000 xingchen-1.1.2/xingchen/models/custom/chat_response.py
+drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-11 01:41:23.151471 xingchen-1.1.2/xingchen/models/custom/groupchat/
+-rw-r--r--   0 frankin    (501) staff       (20)       92 2024-04-09 12:57:52.000000 xingchen-1.1.2/xingchen/models/custom/groupchat/__init__.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2778 2024-04-11 07:45:59.000000 xingchen-1.1.2/xingchen/models/custom/groupchat/group_chat_ext_param.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1763 2024-04-09 13:04:39.000000 xingchen-1.1.2/xingchen/models/custom/groupchat/group_chat_reply_setting.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1303 2024-04-11 02:56:10.000000 xingchen-1.1.2/xingchen/models/custom/groupchat/group_chat_room_info.py
+drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-11 01:41:23.155200 xingchen-1.1.2/xingchen/models/custom/openai/
+-rw-r--r--   0 frankin    (501) staff       (20)        0 2024-05-09 01:43:25.000000 xingchen-1.1.2/xingchen/models/custom/openai/__init__.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1431 2024-05-09 06:12:12.000000 xingchen-1.1.2/xingchen/models/custom/openai/openai_choice.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4347 2024-05-09 03:51:49.000000 xingchen-1.1.2/xingchen/models/custom/openai/openai_completion_req.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2254 2024-05-09 06:28:07.000000 xingchen-1.1.2/xingchen/models/custom/openai/openai_completion_resp.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1767 2024-05-09 02:04:02.000000 xingchen-1.1.2/xingchen/models/custom/openai/openai_req_function.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2005 2024-05-09 02:22:04.000000 xingchen-1.1.2/xingchen/models/custom/openai/openai_req_message.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1733 2024-05-09 02:39:47.000000 xingchen-1.1.2/xingchen/models/custom/openai/openai_req_tool.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1627 2024-05-09 02:38:45.000000 xingchen-1.1.2/xingchen/models/custom/openai/openai_resp_function.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2016 2024-05-09 06:18:11.000000 xingchen-1.1.2/xingchen/models/custom/openai/openai_resp_message.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1855 2024-05-09 06:19:13.000000 xingchen-1.1.2/xingchen/models/custom/openai/openai_resp_tool.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1655 2024-05-09 02:30:52.000000 xingchen-1.1.2/xingchen/models/custom/openai/openai_tool_choice.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1568 2024-05-09 01:57:55.000000 xingchen-1.1.2/xingchen/models/custom/openai/openai_usage.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2026 2024-03-06 07:00:38.000000 xingchen-1.1.2/xingchen/models/custom/platform_publish_config.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1818 2024-02-01 06:33:25.000000 xingchen-1.1.2/xingchen/models/custom/reset_history_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1778 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/extract_data.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2162 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/extract_kv_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2399 2024-04-25 05:48:37.000000 xingchen-1.1.2/xingchen/models/extract_memory_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2239 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/extract_summary_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1718 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/file_conver_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1712 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/file_conver_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2191 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/file_info_vo.py
+-rw-r--r--   0 frankin    (501) staff       (20)     7800 2024-02-02 08:00:56.000000 xingchen-1.1.2/xingchen/models/function_call.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2239 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/gateway_context.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2417 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/gateway_issued_params.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2494 2024-04-11 07:26:08.000000 xingchen-1.1.2/xingchen/models/input.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1506 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/keyword.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1698 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/kv_memory_config.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2237 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/long_term_memory.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2089 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/memory.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1582 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/memory_summary.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2692 2024-01-29 06:06:46.000000 xingchen-1.1.2/xingchen/models/message.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2251 2024-03-05 07:28:35.000000 xingchen-1.1.2/xingchen/models/message_rating_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2057 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/meta.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2899 2024-01-29 05:42:57.000000 xingchen-1.1.2/xingchen/models/model_parameters.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2904 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/page_result_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2929 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/page_result_chat_message_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1681 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/platform_plugin.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2009 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/polling_image_detail_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1965 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/reject_answer_plugin.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2303 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/reject_condition.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2290 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/repository.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2719 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/repository_info.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2578 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/result_dto_boolean.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2561 2024-04-25 05:48:37.000000 xingchen-1.1.2/xingchen/models/result_dto_character_desc_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2893 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/result_dto_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2893 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/result_dto_character_key.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2517 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/result_dto_extract_kv_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2573 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/result_dto_extract_summary_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2539 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/result_dto_file_conver_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3110 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/result_dto_list_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3015 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/result_dto_page_result_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3040 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/result_dto_page_result_chat_message_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2617 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/result_dto_polling_image_detail_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2062 2023-11-21 03:10:04.000000 xingchen-1.1.2/xingchen/models/scenario.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1702 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/stop_chat_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2386 2024-03-05 07:28:35.000000 xingchen-1.1.2/xingchen/models/sys_reminder_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2193 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/text_to_image_plugin.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2177 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/user_profile.py
+-rw-r--r--   0 frankin    (501) staff       (20)        0 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/py.typed
+-rw-r--r--   0 frankin    (501) staff       (20)    12934 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/rest.py
+drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-11 01:41:23.125342 xingchen-1.1.2/xingchen.egg-info/
+-rw-r--r--   0 frankin    (501) staff       (20)      333 2024-05-11 01:41:23.000000 xingchen-1.1.2/xingchen.egg-info/PKG-INFO
+-rw-r--r--   0 frankin    (501) staff       (20)     5654 2024-05-11 01:41:23.000000 xingchen-1.1.2/xingchen.egg-info/SOURCES.txt
+-rw-r--r--   0 frankin    (501) staff       (20)        1 2024-05-11 01:41:23.000000 xingchen-1.1.2/xingchen.egg-info/dependency_links.txt
+-rw-r--r--   0 frankin    (501) staff       (20)       85 2024-05-11 01:41:23.000000 xingchen-1.1.2/xingchen.egg-info/requires.txt
+-rw-r--r--   0 frankin    (501) staff       (20)        9 2024-05-11 01:41:23.000000 xingchen-1.1.2/xingchen.egg-info/top_level.txt
```

### Comparing `xingchen-1.1.1/README.md` & `xingchen-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/pyproject.toml` & `xingchen-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/setup.py` & `xingchen-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "xingchen"
-VERSION = "1.1.1"
+VERSION = "1.1.2"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 1.10.5, < 2",
     "aenum",
     "sseclient-py >= 1.8.0"
```

### Comparing `xingchen-1.1.1/test/test_advanced_settings.py` & `xingchen-1.1.2/test/test_advanced_settings.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_base_chat_request.py` & `xingchen-1.1.2/test/test_base_chat_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_base_chat_request_aca_chat_ext_param.py` & `xingchen-1.1.2/test/test_base_chat_request_aca_chat_ext_param.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_character_advanced_config.py` & `xingchen-1.1.2/test/test_character_advanced_config.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_character_api_sub.py` & `xingchen-1.1.2/test/test_character_api_sub.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_character_create_dto.py` & `xingchen-1.1.2/test/test_character_create_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_character_dto.py` & `xingchen-1.1.2/test/test_character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_character_key.py` & `xingchen-1.1.2/test/test_character_key.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_character_permission_config.py` & `xingchen-1.1.2/test/test_character_permission_config.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_character_query_dto.py` & `xingchen-1.1.2/test/test_character_query_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_character_query_where.py` & `xingchen-1.1.2/test/test_character_query_where.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_character_update_dto.py` & `xingchen-1.1.2/test/test_character_update_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_character_version_create_or_update_dto.py` & `xingchen-1.1.2/test/test_character_version_create_or_update_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_chat_api_sub.py` & `xingchen-1.1.2/test/test_chat_api_sub.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_chat_history_query_dto.py` & `xingchen-1.1.2/test/test_chat_history_query_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_chat_history_query_where.py` & `xingchen-1.1.2/test/test_chat_history_query_where.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_chat_message_api_sub.py` & `xingchen-1.1.2/test/test_chat_message_api_sub.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_chat_message_dto.py` & `xingchen-1.1.2/test/test_chat_message_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_chat_req_params.py` & `xingchen-1.1.2/test/test_chat_req_params.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_chat_room_user_dto.py` & `xingchen-1.1.2/test/test_chat_room_user_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_context.py` & `xingchen-1.1.2/test/test_context.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_file_info_vo.py` & `xingchen-1.1.2/test/test_file_info_vo.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_gateway_context.py` & `xingchen-1.1.2/test/test_gateway_context.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_gateway_issued_params.py` & `xingchen-1.1.2/test/test_gateway_issued_params.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_input.py` & `xingchen-1.1.2/test/test_input.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_message.py` & `xingchen-1.1.2/test/test_message.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_message_rating_request.py` & `xingchen-1.1.2/test/test_message_rating_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_meta.py` & `xingchen-1.1.2/test/test_meta.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_model_parameters.py` & `xingchen-1.1.2/test/test_model_parameters.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_page_result_character_dto.py` & `xingchen-1.1.2/test/test_page_result_character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_page_result_chat_message_dto.py` & `xingchen-1.1.2/test/test_page_result_chat_message_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_repository.py` & `xingchen-1.1.2/test/test_repository.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_repository_info.py` & `xingchen-1.1.2/test/test_repository_info.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_result_dto_boolean.py` & `xingchen-1.1.2/test/test_result_dto_boolean.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_result_dto_character_dto.py` & `xingchen-1.1.2/test/test_result_dto_character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_result_dto_character_key.py` & `xingchen-1.1.2/test/test_result_dto_character_key.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_result_dto_list_character_dto.py` & `xingchen-1.1.2/test/test_result_dto_list_character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_result_dto_page_result_character_dto.py` & `xingchen-1.1.2/test/test_result_dto_page_result_character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_result_dto_page_result_chat_message_dto.py` & `xingchen-1.1.2/test/test_result_dto_page_result_chat_message_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_scenario.py` & `xingchen-1.1.2/test/test_scenario.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_sys_reminder_request.py` & `xingchen-1.1.2/test/test_sys_reminder_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_user_profile.py` & `xingchen-1.1.2/test/test_user_profile.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/__init__.py` & `xingchen-1.1.2/xingchen/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
     The version of the OpenAPI document: v2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
-__version__ = "1.0.7"
+__version__ = "1.1.2"
 
 # import apis into sdk package
 from xingchen.api.character_api_sub import CharacterApiSub
 from xingchen.api.chat_api_sub import ChatApiSub
 from xingchen.api.chat_message_api_sub import ChatMessageApiSub
 from xingchen.api.groupchat_api_sub import GroupChatApiSub
 from xingchen.api.chat_extract_message_api_sub import ChatExtractMessageApiSub
@@ -104,7 +104,18 @@
 from xingchen.models.polling_image_detail_dto import PollingImageDetailDTO
 from xingchen.models.result_dto_character_desc_dto import ResultDTOCharacterDescDTO
 from xingchen.models.result_dto_file_conver_dto import ResultDTOFileConvertDTO
 from xingchen.models.result_dto_polling_image_detail_dto import ResultDTOPollingImageDetailDTO
 from xingchen.models.result_dto_extract_kv_dto import ResultDTOExtractKVDTO
 from xingchen.models.result_dto_extract_summary_dto import ResultDTOExtractSummaryDTO
 
+# OpenAI models
+from xingchen.models.custom.openai.openai_req_function import OpenAiReqFunction
+from xingchen.models.custom.openai.openai_resp_function import OpenAiRespFunction
+from xingchen.models.custom.openai.openai_usage import OpenAiUsage
+from xingchen.models.custom.openai.openai_req_message import OpenAiReqMessage
+from xingchen.models.custom.openai.openai_resp_message import OpenAiRespMessage
+from xingchen.models.custom.openai.openai_req_tool import OpenAiReqTool
+from xingchen.models.custom.openai.openai_resp_tool import OpenAiRespTool
+from xingchen.models.custom.openai.openai_completion_req import OpenAiCompletionReq
+from xingchen.models.custom.openai.openai_completion_resp import OpenAiCompletionResp
+from xingchen.api.openai_api_sub import OpenAiApiSub
```

### Comparing `xingchen-1.1.1/xingchen/aca_util.py` & `xingchen-1.1.2/xingchen/aca_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from xingchen.models import ChatReqParams, BaseChatRequest, Input
-from xingchen.models.custom import ChatResponse,ChatResult
+from xingchen.models.custom import ChatResponse, ChatResult
+from xingchen.models.custom.openai.openai_completion_resp import OpenAiCompletionResp
 
 from sseclient import SSEClient
 import json
 
 api_router_map = {
     '/v2/api/chat/send': 'aca-chat-send',
     '/v2/api/groupchat/send': 'aca-groupchat-send',
@@ -21,15 +22,16 @@
     '/v2/api/chat/reset': 'aca-chat-reset',
     '/v2/api/extract/kv': 'aca-extract-memory-kv',
     '/v2/api/extract/summary': 'aca-extract-memory-summary',
     '/v2/api/character/auto/desc': 'aca-char-auto-desc',
     '/v2/api/chat/polling/image': 'aca-polling-image',
     '/v2/api/chat/stop': 'aca-chat-stop',
     '/v2/api/common/file/asyn/upload': 'aca-doc-converter-submit',
-    '/v2/api/common/file/asyn/download': 'aca-doc-converter-result'
+    '/v2/api/common/file/asyn/download': 'aca-doc-converter-result',
+    '/v2/api/completions': 'aca-openai-completion',
 }
 
 
 def get_service_router(path, async_req):
     if not path:
         return None
     if path.__eq__('/v2/api/chat/send') and async_req:
@@ -86,7 +88,18 @@
             return
         yield ChatResponse(
             success=True,
             http_status_code=200,
             code=200,
             data=ChatResult.from_dict(d)
         )
+
+
+def handle_openai_sse_response(client: SSEClient):
+    events = client.events()
+    for event in events:
+        d = json.loads(event.data)
+        error_code = d.get('errorCode', None)
+        if error_code is not None:
+            yield ChatResponse.from_dict(d)
+            return
+        yield OpenAiCompletionResp.from_dict(d)
```

### Comparing `xingchen-1.1.1/xingchen/api/character_api_sub.py` & `xingchen-1.1.2/xingchen/api/character_api_sub.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/api/chat_api_sub.py` & `xingchen-1.1.2/xingchen/api/chat_api_sub.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/api/chat_extract_message_api_sub.py` & `xingchen-1.1.2/xingchen/api/chat_extract_message_api_sub.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/api/chat_message_api_sub.py` & `xingchen-1.1.2/xingchen/api/chat_message_api_sub.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/api/common_api_sub.py` & `xingchen-1.1.2/xingchen/api/common_api_sub.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/api/groupchat_api_sub.py` & `xingchen-1.1.2/xingchen/api/groupchat_api_sub.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/api_client.py` & `xingchen-1.1.2/xingchen/api_client.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/api_response.py` & `xingchen-1.1.2/xingchen/api_response.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/configuration.py` & `xingchen-1.1.2/xingchen/configuration.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/exceptions.py` & `xingchen-1.1.2/xingchen/exceptions.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/__init__.py` & `xingchen-1.1.2/xingchen/models/__init__.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/advanced_settings.py` & `xingchen-1.1.2/xingchen/models/advanced_settings.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/base_chat_request.py` & `xingchen-1.1.2/xingchen/models/base_chat_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/character_advanced_config.py` & `xingchen-1.1.2/xingchen/models/character_advanced_config.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/character_create_dto.py` & `xingchen-1.1.2/xingchen/models/character_create_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/character_desc_dto.py` & `xingchen-1.1.2/xingchen/models/character_desc_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/character_desc_generated_request.py` & `xingchen-1.1.2/xingchen/models/character_desc_generated_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/character_dto.py` & `xingchen-1.1.2/xingchen/models/character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/character_key.py` & `xingchen-1.1.2/xingchen/models/character_key.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/character_permission_config.py` & `xingchen-1.1.2/xingchen/models/character_permission_config.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/character_query_dto.py` & `xingchen-1.1.2/xingchen/models/character_query_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/character_query_where.py` & `xingchen-1.1.2/xingchen/models/character_query_where.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/character_update_dto.py` & `xingchen-1.1.2/xingchen/models/character_update_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/character_version_create_or_update_dto.py` & `xingchen-1.1.2/xingchen/models/character_version_create_or_update_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/chat_context.py` & `xingchen-1.1.2/xingchen/models/chat_context.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/chat_history_query_dto.py` & `xingchen-1.1.2/xingchen/models/chat_history_query_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/chat_history_query_where.py` & `xingchen-1.1.2/xingchen/models/chat_history_query_where.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/chat_message_dto.py` & `xingchen-1.1.2/xingchen/models/chat_message_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/chat_req_params.py` & `xingchen-1.1.2/xingchen/models/chat_req_params.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/chat_room_user_dto.py` & `xingchen-1.1.2/xingchen/models/chat_room_user_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/context.py` & `xingchen-1.1.2/xingchen/models/context.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/custom/base_response.py` & `xingchen-1.1.2/xingchen/models/custom/base_response.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/custom/character_model_parameters.py` & `xingchen-1.1.2/xingchen/models/custom/character_model_parameters.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/custom/chat_response.py` & `xingchen-1.1.2/xingchen/models/custom/chat_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 from __future__ import annotations
 
 import json
 import pprint
 
 from pydantic import BaseModel, Field, StrictStr, StrictInt, conlist
-from typing import Optional
+from typing import Optional, Any
 
 from xingchen.models.message import Message
 from xingchen.models.context import Context
 from xingchen.models.custom.base_response import BaseResponse
 
 
 class Choice(BaseModel):
@@ -119,15 +119,15 @@
             'choices': obj.get('choices'),
             'usage': obj.get('usage'),
             'context': obj.get('context')
         })
 
 
 class ChatResponse(BaseResponse):
-    data: Optional[ChatResult] = Field(None, alias="chatResult")
+    data: Optional[Any] = Field(None, alias="chatResult")
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         return pprint.pformat(self.dict(by_alias=False, exclude_none=True))
@@ -156,8 +156,8 @@
             'error_message': obj.get('errorMessage'),
             'error_name': obj.get('errorName'),
             'http_status_code': obj.get('httpStatusCode'),
             'code': obj.get('code'),
             'error_message_key': obj.get('errorMessageKey'),
             'success': obj.get('success'),
             'data': obj.get('data')
-        })
+        })
```

### Comparing `xingchen-1.1.1/xingchen/models/custom/groupchat/group_chat_ext_param.py` & `xingchen-1.1.2/xingchen/models/custom/groupchat/group_chat_ext_param.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/custom/groupchat/group_chat_reply_setting.py` & `xingchen-1.1.2/xingchen/models/custom/groupchat/group_chat_reply_setting.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/custom/groupchat/group_chat_room_info.py` & `xingchen-1.1.2/xingchen/models/custom/groupchat/group_chat_room_info.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/custom/platform_publish_config.py` & `xingchen-1.1.2/xingchen/models/custom/platform_publish_config.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/custom/reset_history_request.py` & `xingchen-1.1.2/xingchen/models/custom/reset_history_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/extract_data.py` & `xingchen-1.1.2/xingchen/models/extract_data.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/extract_kv_dto.py` & `xingchen-1.1.2/xingchen/models/extract_kv_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/extract_memory_request.py` & `xingchen-1.1.2/xingchen/models/extract_memory_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/extract_summary_dto.py` & `xingchen-1.1.2/xingchen/models/extract_summary_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/file_conver_dto.py` & `xingchen-1.1.2/xingchen/models/file_conver_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/file_conver_request.py` & `xingchen-1.1.2/xingchen/models/file_conver_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/file_info_vo.py` & `xingchen-1.1.2/xingchen/models/file_info_vo.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/function_call.py` & `xingchen-1.1.2/xingchen/models/function_call.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/gateway_context.py` & `xingchen-1.1.2/xingchen/models/gateway_context.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/gateway_issued_params.py` & `xingchen-1.1.2/xingchen/models/gateway_issued_params.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/input.py` & `xingchen-1.1.2/xingchen/models/input.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/keyword.py` & `xingchen-1.1.2/xingchen/models/keyword.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/kv_memory_config.py` & `xingchen-1.1.2/xingchen/models/kv_memory_config.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/long_term_memory.py` & `xingchen-1.1.2/xingchen/models/long_term_memory.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/memory.py` & `xingchen-1.1.2/xingchen/models/memory.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/memory_summary.py` & `xingchen-1.1.2/xingchen/models/memory_summary.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/message.py` & `xingchen-1.1.2/xingchen/models/message.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/message_rating_request.py` & `xingchen-1.1.2/xingchen/models/message_rating_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/meta.py` & `xingchen-1.1.2/xingchen/models/meta.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/model_parameters.py` & `xingchen-1.1.2/xingchen/models/model_parameters.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/page_result_character_dto.py` & `xingchen-1.1.2/xingchen/models/page_result_character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/page_result_chat_message_dto.py` & `xingchen-1.1.2/xingchen/models/page_result_chat_message_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/platform_plugin.py` & `xingchen-1.1.2/xingchen/models/platform_plugin.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/polling_image_detail_dto.py` & `xingchen-1.1.2/xingchen/models/polling_image_detail_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/reject_answer_plugin.py` & `xingchen-1.1.2/xingchen/models/reject_answer_plugin.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/reject_condition.py` & `xingchen-1.1.2/xingchen/models/reject_condition.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/repository.py` & `xingchen-1.1.2/xingchen/models/repository.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/repository_info.py` & `xingchen-1.1.2/xingchen/models/repository_info.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/result_dto_boolean.py` & `xingchen-1.1.2/xingchen/models/result_dto_boolean.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/result_dto_character_desc_dto.py` & `xingchen-1.1.2/xingchen/models/result_dto_character_desc_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/result_dto_character_dto.py` & `xingchen-1.1.2/xingchen/models/result_dto_character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/result_dto_character_key.py` & `xingchen-1.1.2/xingchen/models/result_dto_character_key.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/result_dto_extract_kv_dto.py` & `xingchen-1.1.2/xingchen/models/result_dto_extract_kv_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/result_dto_extract_summary_dto.py` & `xingchen-1.1.2/xingchen/models/result_dto_extract_summary_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/result_dto_file_conver_dto.py` & `xingchen-1.1.2/xingchen/models/result_dto_file_conver_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/result_dto_list_character_dto.py` & `xingchen-1.1.2/xingchen/models/result_dto_list_character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/result_dto_page_result_character_dto.py` & `xingchen-1.1.2/xingchen/models/result_dto_page_result_character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/result_dto_page_result_chat_message_dto.py` & `xingchen-1.1.2/xingchen/models/result_dto_page_result_chat_message_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/result_dto_polling_image_detail_dto.py` & `xingchen-1.1.2/xingchen/models/result_dto_polling_image_detail_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/scenario.py` & `xingchen-1.1.2/xingchen/models/scenario.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/stop_chat_request.py` & `xingchen-1.1.2/xingchen/models/stop_chat_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/sys_reminder_request.py` & `xingchen-1.1.2/xingchen/models/sys_reminder_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/text_to_image_plugin.py` & `xingchen-1.1.2/xingchen/models/text_to_image_plugin.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/user_profile.py` & `xingchen-1.1.2/xingchen/models/user_profile.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/rest.py` & `xingchen-1.1.2/xingchen/rest.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen.egg-info/SOURCES.txt` & `xingchen-1.1.2/xingchen.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 xingchen/api/__init__.py
 xingchen/api/character_api_sub.py
 xingchen/api/chat_api_sub.py
 xingchen/api/chat_extract_message_api_sub.py
 xingchen/api/chat_message_api_sub.py
 xingchen/api/common_api_sub.py
 xingchen/api/groupchat_api_sub.py
+xingchen/api/openai_api_sub.py
 xingchen/models/__init__.py
 xingchen/models/advanced_settings.py
 xingchen/models/base_chat_request.py
 xingchen/models/character_advanced_config.py
 xingchen/models/character_create_dto.py
 xingchen/models/character_desc_dto.py
 xingchen/models/character_desc_generated_request.py
@@ -134,8 +135,20 @@
 xingchen/models/custom/character_model_parameters.py
 xingchen/models/custom/chat_response.py
 xingchen/models/custom/platform_publish_config.py
 xingchen/models/custom/reset_history_request.py
 xingchen/models/custom/groupchat/__init__.py
 xingchen/models/custom/groupchat/group_chat_ext_param.py
 xingchen/models/custom/groupchat/group_chat_reply_setting.py
-xingchen/models/custom/groupchat/group_chat_room_info.py
+xingchen/models/custom/groupchat/group_chat_room_info.py
+xingchen/models/custom/openai/__init__.py
+xingchen/models/custom/openai/openai_choice.py
+xingchen/models/custom/openai/openai_completion_req.py
+xingchen/models/custom/openai/openai_completion_resp.py
+xingchen/models/custom/openai/openai_req_function.py
+xingchen/models/custom/openai/openai_req_message.py
+xingchen/models/custom/openai/openai_req_tool.py
+xingchen/models/custom/openai/openai_resp_function.py
+xingchen/models/custom/openai/openai_resp_message.py
+xingchen/models/custom/openai/openai_resp_tool.py
+xingchen/models/custom/openai/openai_tool_choice.py
+xingchen/models/custom/openai/openai_usage.py
```

