# Comparing `tmp/proxynt-1.1.8.tar.gz` & `tmp/proxynt-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxynt-1.1.8.tar", last modified: Tue Feb 21 16:02:07 2023, max compression
+gzip compressed data, was "proxynt-1.1.9.tar", last modified: Tue Feb 28 11:12:55 2023, max compression
```

## Comparing `proxynt-1.1.8.tar` & `proxynt-1.1.9.tar`

### file list

```diff
@@ -1,98 +1,100 @@
-drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-21 16:02:07.403789 proxynt-1.1.8/
--rw-rw-r--   0 wukt      (1000) wukt      (1000)      105 2023-01-03 12:45:38.000000 proxynt-1.1.8/MANIFEST.in
--rw-rw-r--   0 wukt      (1000) wukt      (1000)     5740 2023-02-21 16:02:07.403789 proxynt-1.1.8/PKG-INFO
--rw-rw-r--   0 wukt      (1000) wukt      (1000)        0 2023-01-03 11:11:36.000000 proxynt-1.1.8/__init__.py
-drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-21 16:02:07.395789 proxynt-1.1.8/client/
--rw-rw-r--   0 wukt      (1000) wukt      (1000)        0 2022-10-30 01:31:26.000000 proxynt-1.1.8/client/__init__.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)      503 2023-02-05 03:00:46.000000 proxynt-1.1.8/client/clear_nonce_task.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)     2916 2022-12-19 13:08:54.000000 proxynt-1.1.8/client/heart_beat_task.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)     5850 2023-02-05 03:00:46.000000 proxynt-1.1.8/client/tcp_forward_client.py
-drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-21 16:02:07.395789 proxynt-1.1.8/common/
--rw-rw-r--   0 wukt      (1000) wukt      (1000)        0 2022-10-30 01:31:26.000000 proxynt-1.1.8/common/__init__.py
-drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-21 16:02:07.395789 proxynt-1.1.8/common/crypto/
--rw-rw-r--   0 wukt      (1000) wukt      (1000)      685 2022-12-21 08:33:33.000000 proxynt-1.1.8/common/crypto/__init__.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)     8261 2023-02-05 03:00:46.000000 proxynt-1.1.8/common/crypto/table.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)      739 2023-02-05 03:00:46.000000 proxynt-1.1.8/common/encrypt_utils.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)     2306 2023-01-05 12:04:30.000000 proxynt-1.1.8/common/logger_factory.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)     5227 2023-02-21 15:57:43.000000 proxynt-1.1.8/common/nat_serialization.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)     2652 2022-12-21 08:33:33.000000 proxynt-1.1.8/common/pool.py
-drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-21 16:02:07.399789 proxynt-1.1.8/common/websocket/
--rw-rw-r--   0 wukt      (1000) wukt      (1000)      801 2022-12-19 13:08:54.000000 proxynt-1.1.8/common/websocket/__init__.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)    13303 2022-12-19 13:08:54.000000 proxynt-1.1.8/common/websocket/_abnf.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)    18061 2022-12-19 13:08:54.000000 proxynt-1.1.8/common/websocket/_app.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)     2118 2022-12-19 13:08:54.000000 proxynt-1.1.8/common/websocket/_cookiejar.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)    19555 2022-12-19 13:08:54.000000 proxynt-1.1.8/common/websocket/_core.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)     2105 2022-12-19 13:08:54.000000 proxynt-1.1.8/common/websocket/_exceptions.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)     6004 2022-12-21 08:33:33.000000 proxynt-1.1.8/common/websocket/_handshake.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)    11617 2022-12-21 08:33:33.000000 proxynt-1.1.8/common/websocket/_http.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)     1418 2022-12-19 13:08:54.000000 proxynt-1.1.8/common/websocket/_logging.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)     4859 2022-12-19 13:08:54.000000 proxynt-1.1.8/common/websocket/_socket.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)     1122 2022-12-19 13:08:54.000000 proxynt-1.1.8/common/websocket/_ssl_compat.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)     4797 2022-12-19 13:08:54.000000 proxynt-1.1.8/common/websocket/_url.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)     3516 2022-12-19 13:08:54.000000 proxynt-1.1.8/common/websocket/_utils.py
--rwxrwxr-x   0 wukt      (1000) wukt      (1000)     6909 2022-12-19 13:08:54.000000 proxynt-1.1.8/common/websocket/_wsdump.py
-drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-21 16:02:07.399789 proxynt-1.1.8/common/websocket/tests/
--rw-rw-r--   0 wukt      (1000) wukt      (1000)        0 2022-12-19 13:08:54.000000 proxynt-1.1.8/common/websocket/tests/__init__.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)      481 2022-12-19 13:08:54.000000 proxynt-1.1.8/common/websocket/tests/echo-server.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)     4175 2022-12-19 13:08:54.000000 proxynt-1.1.8/common/websocket/tests/test_abnf.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)     9689 2022-12-19 13:08:54.000000 proxynt-1.1.8/common/websocket/tests/test_app.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)     4325 2022-12-19 13:08:54.000000 proxynt-1.1.8/common/websocket/tests/test_cookiejar.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)     9623 2022-12-19 13:08:54.000000 proxynt-1.1.8/common/websocket/tests/test_http.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)    14589 2022-12-19 13:08:54.000000 proxynt-1.1.8/common/websocket/tests/test_url.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)    18072 2022-12-19 13:08:54.000000 proxynt-1.1.8/common/websocket/tests/test_websocket.py
-drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-21 16:02:07.399789 proxynt-1.1.8/constant/
--rw-rw-r--   0 wukt      (1000) wukt      (1000)        0 2022-10-30 01:31:26.000000 proxynt-1.1.8/constant/__init__.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)      141 2022-12-19 13:08:54.000000 proxynt-1.1.8/constant/message_type_constnat.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)      458 2023-02-21 16:01:41.000000 proxynt-1.1.8/constant/system_constant.py
-drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-21 16:02:07.399789 proxynt-1.1.8/context/
--rw-rw-r--   0 wukt      (1000) wukt      (1000)        0 2022-10-30 01:31:26.000000 proxynt-1.1.8/context/__init__.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)     2593 2023-02-05 03:00:46.000000 proxynt-1.1.8/context/context_utils.py
-drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-21 16:02:07.399789 proxynt-1.1.8/entity/
--rw-rw-r--   0 wukt      (1000) wukt      (1000)        0 2022-10-30 01:31:26.000000 proxynt-1.1.8/entity/__init__.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)      419 2022-12-18 02:37:43.000000 proxynt-1.1.8/entity/client_config_entity.py
-drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-21 16:02:07.399789 proxynt-1.1.8/entity/message/
--rw-rw-r--   0 wukt      (1000) wukt      (1000)        0 2022-10-30 01:31:26.000000 proxynt-1.1.8/entity/message/__init__.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)      328 2022-12-18 02:13:47.000000 proxynt-1.1.8/entity/message/message_entity.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)      332 2023-02-21 15:27:29.000000 proxynt-1.1.8/entity/message/push_config_entity.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)      187 2023-02-05 03:00:46.000000 proxynt-1.1.8/entity/message/tcp_over_websocket_message.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)      452 2022-12-18 02:37:43.000000 proxynt-1.1.8/entity/server_config_entity.py
-drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-21 16:02:07.399789 proxynt-1.1.8/exceptions/
--rw-rw-r--   0 wukt      (1000) wukt      (1000)        0 2022-10-30 01:31:26.000000 proxynt-1.1.8/exceptions/__init__.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)       41 2022-10-30 01:31:26.000000 proxynt-1.1.8/exceptions/duplicated_name.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)       42 2022-10-30 01:31:26.000000 proxynt-1.1.8/exceptions/invalid_password.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)       38 2023-02-05 03:00:46.000000 proxynt-1.1.8/exceptions/replay_error.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)       41 2023-02-05 03:00:46.000000 proxynt-1.1.8/exceptions/signature_error.py
-drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-21 16:02:07.403789 proxynt-1.1.8/proxynt.egg-info/
--rw-rw-r--   0 wukt      (1000) wukt      (1000)     5740 2023-02-21 16:02:07.000000 proxynt-1.1.8/proxynt.egg-info/PKG-INFO
--rw-rw-r--   0 wukt      (1000) wukt      (1000)     2335 2023-02-21 16:02:07.000000 proxynt-1.1.8/proxynt.egg-info/SOURCES.txt
--rw-rw-r--   0 wukt      (1000) wukt      (1000)        1 2023-02-21 16:02:07.000000 proxynt-1.1.8/proxynt.egg-info/dependency_links.txt
--rw-rw-r--   0 wukt      (1000) wukt      (1000)      107 2023-02-21 16:02:07.000000 proxynt-1.1.8/proxynt.egg-info/entry_points.txt
--rw-rw-r--   0 wukt      (1000) wukt      (1000)       26 2023-02-21 16:02:07.000000 proxynt-1.1.8/proxynt.egg-info/requires.txt
--rw-rw-r--   0 wukt      (1000) wukt      (1000)        8 2023-02-21 16:02:07.000000 proxynt-1.1.8/proxynt.egg-info/top_level.txt
--rw-rw-r--   0 wukt      (1000) wukt      (1000)     8644 2023-02-21 15:27:29.000000 proxynt-1.1.8/run_client.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)     6016 2023-02-05 03:00:46.000000 proxynt-1.1.8/run_server.py
-drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-21 16:02:07.399789 proxynt-1.1.8/server/
--rw-rw-r--   0 wukt      (1000) wukt      (1000)        0 2022-10-30 01:31:26.000000 proxynt-1.1.8/server/__init__.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)    11912 2023-02-21 15:27:29.000000 proxynt-1.1.8/server/admin_http_handler.py
-drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-21 16:02:07.399789 proxynt-1.1.8/server/task/
--rw-rw-r--   0 wukt      (1000) wukt      (1000)        0 2023-01-08 02:23:12.000000 proxynt-1.1.8/server/task/__init__.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)      543 2023-01-08 02:14:34.000000 proxynt-1.1.8/server/task/check_cookie_task.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)      505 2023-02-05 03:00:46.000000 proxynt-1.1.8/server/task/clear_nonce_task.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)     2133 2022-12-19 13:08:54.000000 proxynt-1.1.8/server/task/heart_beat_task.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)    10838 2023-02-05 03:00:46.000000 proxynt-1.1.8/server/tcp_forward_client.py
-drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-21 16:02:07.399789 proxynt-1.1.8/server/template/
--rw-rw-r--   0 wukt      (1000) wukt      (1000)        0 2023-01-03 11:33:58.000000 proxynt-1.1.8/server/template/__init__.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)     1677 2023-01-08 02:26:19.000000 proxynt-1.1.8/server/template/base.html
-drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-21 16:02:07.399789 proxynt-1.1.8/server/template/css/
-drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-21 16:02:07.399789 proxynt-1.1.8/server/template/css/fonts/
--rw-rw-r--   0 wukt      (1000) wukt      (1000)    28200 2022-12-18 02:37:43.000000 proxynt-1.1.8/server/template/css/fonts/element-icons.woff
--rw-rw-r--   0 wukt      (1000) wukt      (1000)   239740 2022-12-18 02:37:43.000000 proxynt-1.1.8/server/template/css/index.css
--rw-rw-r--   0 wukt      (1000) wukt      (1000)     7961 2023-02-21 15:56:42.000000 proxynt-1.1.8/server/template/ele_index.html
-drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-21 16:02:07.403789 proxynt-1.1.8/server/template/js/
--rw-rw-r--   0 wukt      (1000) wukt      (1000)    14265 2022-12-18 02:37:43.000000 proxynt-1.1.8/server/template/js/axios.min.js
--rw-rw-r--   0 wukt      (1000) wukt      (1000)   664111 2022-12-18 02:37:43.000000 proxynt-1.1.8/server/template/js/index.js
--rw-rw-r--   0 wukt      (1000) wukt      (1000)    93670 2022-12-18 02:37:43.000000 proxynt-1.1.8/server/template/js/vue.min.js
--rw-rw-r--   0 wukt      (1000) wukt      (1000)     1481 2022-12-18 02:37:43.000000 proxynt-1.1.8/server/template/login.html
--rw-rw-r--   0 wukt      (1000) wukt      (1000)     6805 2023-02-21 15:27:29.000000 proxynt-1.1.8/server/websocket_handler.py
--rw-rw-r--   0 wukt      (1000) wukt      (1000)       38 2023-02-21 16:02:07.403789 proxynt-1.1.8/setup.cfg
--rw-rw-r--   0 wukt      (1000) wukt      (1000)      915 2023-02-18 03:50:45.000000 proxynt-1.1.8/setup.py
+drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-28 11:12:55.778970 proxynt-1.1.9/
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)      105 2023-01-03 12:45:38.000000 proxynt-1.1.9/MANIFEST.in
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)     5352 2023-02-28 11:12:55.778970 proxynt-1.1.9/PKG-INFO
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)        0 2023-01-03 11:11:36.000000 proxynt-1.1.9/__init__.py
+drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-28 11:12:55.762679 proxynt-1.1.9/client/
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)        0 2022-10-30 01:31:26.000000 proxynt-1.1.9/client/__init__.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)      503 2023-02-05 03:00:46.000000 proxynt-1.1.9/client/clear_nonce_task.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)     2916 2022-12-19 13:08:54.000000 proxynt-1.1.9/client/heart_beat_task.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)     6409 2023-02-28 11:11:24.000000 proxynt-1.1.9/client/tcp_forward_client.py
+drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-28 11:12:55.762679 proxynt-1.1.9/common/
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)        0 2022-10-30 01:31:26.000000 proxynt-1.1.9/common/__init__.py
+drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-28 11:12:55.762679 proxynt-1.1.9/common/crypto/
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)      685 2022-12-21 08:33:33.000000 proxynt-1.1.9/common/crypto/__init__.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)     8261 2023-02-05 03:00:46.000000 proxynt-1.1.9/common/crypto/table.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)      739 2023-02-05 03:00:46.000000 proxynt-1.1.9/common/encrypt_utils.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)     2231 2023-02-28 11:11:24.000000 proxynt-1.1.9/common/logger_factory.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)     5227 2023-02-21 15:57:43.000000 proxynt-1.1.9/common/nat_serialization.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)     4655 2023-02-28 11:11:24.000000 proxynt-1.1.9/common/pool.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)      413 2023-02-28 11:11:24.000000 proxynt-1.1.9/common/register_append_data.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)      989 2023-02-28 11:11:24.000000 proxynt-1.1.9/common/speed_limit.py
+drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-28 11:12:55.766752 proxynt-1.1.9/common/websocket/
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)      801 2022-12-19 13:08:54.000000 proxynt-1.1.9/common/websocket/__init__.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)    13303 2022-12-19 13:08:54.000000 proxynt-1.1.9/common/websocket/_abnf.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)    18061 2022-12-19 13:08:54.000000 proxynt-1.1.9/common/websocket/_app.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)     2118 2022-12-19 13:08:54.000000 proxynt-1.1.9/common/websocket/_cookiejar.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)    19555 2022-12-19 13:08:54.000000 proxynt-1.1.9/common/websocket/_core.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)     2105 2022-12-19 13:08:54.000000 proxynt-1.1.9/common/websocket/_exceptions.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)     6004 2022-12-21 08:33:33.000000 proxynt-1.1.9/common/websocket/_handshake.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)    11617 2022-12-21 08:33:33.000000 proxynt-1.1.9/common/websocket/_http.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)     1418 2022-12-19 13:08:54.000000 proxynt-1.1.9/common/websocket/_logging.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)     4859 2022-12-19 13:08:54.000000 proxynt-1.1.9/common/websocket/_socket.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)     1122 2022-12-19 13:08:54.000000 proxynt-1.1.9/common/websocket/_ssl_compat.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)     4797 2022-12-19 13:08:54.000000 proxynt-1.1.9/common/websocket/_url.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)     3516 2022-12-19 13:08:54.000000 proxynt-1.1.9/common/websocket/_utils.py
+-rwxrwxr-x   0 wukt      (1000) wukt      (1000)     6909 2022-12-19 13:08:54.000000 proxynt-1.1.9/common/websocket/_wsdump.py
+drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-28 11:12:55.766752 proxynt-1.1.9/common/websocket/tests/
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)        0 2022-12-19 13:08:54.000000 proxynt-1.1.9/common/websocket/tests/__init__.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)      481 2022-12-19 13:08:54.000000 proxynt-1.1.9/common/websocket/tests/echo-server.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)     4175 2022-12-19 13:08:54.000000 proxynt-1.1.9/common/websocket/tests/test_abnf.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)     9689 2022-12-19 13:08:54.000000 proxynt-1.1.9/common/websocket/tests/test_app.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)     4325 2022-12-19 13:08:54.000000 proxynt-1.1.9/common/websocket/tests/test_cookiejar.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)     9623 2022-12-19 13:08:54.000000 proxynt-1.1.9/common/websocket/tests/test_http.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)    14589 2022-12-19 13:08:54.000000 proxynt-1.1.9/common/websocket/tests/test_url.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)    18072 2022-12-19 13:08:54.000000 proxynt-1.1.9/common/websocket/tests/test_websocket.py
+drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-28 11:12:55.770825 proxynt-1.1.9/constant/
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)        0 2022-10-30 01:31:26.000000 proxynt-1.1.9/constant/__init__.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)      142 2023-02-28 11:11:24.000000 proxynt-1.1.9/constant/message_type_constnat.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)      456 2023-02-28 11:11:24.000000 proxynt-1.1.9/constant/system_constant.py
+drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-28 11:12:55.770825 proxynt-1.1.9/context/
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)        0 2022-10-30 01:31:26.000000 proxynt-1.1.9/context/__init__.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)     2593 2023-02-05 03:00:46.000000 proxynt-1.1.9/context/context_utils.py
+drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-28 11:12:55.770825 proxynt-1.1.9/entity/
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)        0 2022-10-30 01:31:26.000000 proxynt-1.1.9/entity/__init__.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)      442 2023-02-28 11:11:24.000000 proxynt-1.1.9/entity/client_config_entity.py
+drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-28 11:12:55.770825 proxynt-1.1.9/entity/message/
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)        0 2022-10-30 01:31:26.000000 proxynt-1.1.9/entity/message/__init__.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)      328 2022-12-18 02:13:47.000000 proxynt-1.1.9/entity/message/message_entity.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)      355 2023-02-28 11:11:24.000000 proxynt-1.1.9/entity/message/push_config_entity.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)      187 2023-02-05 03:00:46.000000 proxynt-1.1.9/entity/message/tcp_over_websocket_message.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)      452 2022-12-18 02:37:43.000000 proxynt-1.1.9/entity/server_config_entity.py
+drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-28 11:12:55.770825 proxynt-1.1.9/exceptions/
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)        0 2022-10-30 01:31:26.000000 proxynt-1.1.9/exceptions/__init__.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)       41 2022-10-30 01:31:26.000000 proxynt-1.1.9/exceptions/duplicated_name.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)       42 2022-10-30 01:31:26.000000 proxynt-1.1.9/exceptions/invalid_password.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)       38 2023-02-05 03:00:46.000000 proxynt-1.1.9/exceptions/replay_error.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)       41 2023-02-05 03:00:46.000000 proxynt-1.1.9/exceptions/signature_error.py
+drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-28 11:12:55.778970 proxynt-1.1.9/proxynt.egg-info/
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)     5352 2023-02-28 11:12:55.000000 proxynt-1.1.9/proxynt.egg-info/PKG-INFO
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)     2392 2023-02-28 11:12:55.000000 proxynt-1.1.9/proxynt.egg-info/SOURCES.txt
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)        1 2023-02-28 11:12:55.000000 proxynt-1.1.9/proxynt.egg-info/dependency_links.txt
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)      107 2023-02-28 11:12:55.000000 proxynt-1.1.9/proxynt.egg-info/entry_points.txt
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)       26 2023-02-28 11:12:55.000000 proxynt-1.1.9/proxynt.egg-info/requires.txt
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)        8 2023-02-28 11:12:55.000000 proxynt-1.1.9/proxynt.egg-info/top_level.txt
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)     8902 2023-02-28 11:12:32.000000 proxynt-1.1.9/run_client.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)     6016 2023-02-05 03:00:46.000000 proxynt-1.1.9/run_server.py
+drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-28 11:12:55.770825 proxynt-1.1.9/server/
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)        0 2022-10-30 01:31:26.000000 proxynt-1.1.9/server/__init__.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)    13012 2023-02-28 11:11:24.000000 proxynt-1.1.9/server/admin_http_handler.py
+drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-28 11:12:55.770825 proxynt-1.1.9/server/task/
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)        0 2023-01-08 02:23:12.000000 proxynt-1.1.9/server/task/__init__.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)      543 2023-01-08 02:14:34.000000 proxynt-1.1.9/server/task/check_cookie_task.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)      505 2023-02-05 03:00:46.000000 proxynt-1.1.9/server/task/clear_nonce_task.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)     2133 2022-12-19 13:08:54.000000 proxynt-1.1.9/server/task/heart_beat_task.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)    11673 2023-02-28 11:11:24.000000 proxynt-1.1.9/server/tcp_forward_client.py
+drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-28 11:12:55.774897 proxynt-1.1.9/server/template/
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)        0 2023-01-03 11:33:58.000000 proxynt-1.1.9/server/template/__init__.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)     1677 2023-01-08 02:26:19.000000 proxynt-1.1.9/server/template/base.html
+drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-28 11:12:55.774897 proxynt-1.1.9/server/template/css/
+drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-28 11:12:55.774897 proxynt-1.1.9/server/template/css/fonts/
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)    28200 2022-12-18 02:37:43.000000 proxynt-1.1.9/server/template/css/fonts/element-icons.woff
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)   239740 2022-12-18 02:37:43.000000 proxynt-1.1.9/server/template/css/index.css
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)     9517 2023-02-28 11:11:24.000000 proxynt-1.1.9/server/template/ele_index.html
+drwxrwxr-x   0 wukt      (1000) wukt      (1000)        0 2023-02-28 11:12:55.774897 proxynt-1.1.9/server/template/js/
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)    14265 2022-12-18 02:37:43.000000 proxynt-1.1.9/server/template/js/axios.min.js
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)   664111 2022-12-18 02:37:43.000000 proxynt-1.1.9/server/template/js/index.js
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)    93670 2022-12-18 02:37:43.000000 proxynt-1.1.9/server/template/js/vue.min.js
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)     1481 2022-12-18 02:37:43.000000 proxynt-1.1.9/server/template/login.html
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)     7155 2023-02-28 11:11:24.000000 proxynt-1.1.9/server/websocket_handler.py
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)       38 2023-02-28 11:12:55.778970 proxynt-1.1.9/setup.cfg
+-rw-rw-r--   0 wukt      (1000) wukt      (1000)      915 2023-02-18 03:50:45.000000 proxynt-1.1.9/setup.py
```

### Comparing `proxynt-1.1.8/PKG-INFO` & `proxynt-1.1.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,143 +1,110 @@
 Metadata-Version: 2.1
 Name: proxynt
-Version: 1.1.8
+Version: 1.1.9
 Summary: UNKNOWN
 Home-page: https://github.com/sazima/proxynt
 License: UNKNOWN
-Description: # 
-        
-        [中文](https://github.com/sazima/proxynt/blob/master/readme.md)
+Description: [中文](https://github.com/sazima/proxynt/blob/master/readme.md)
         
         ProxyNT is a reverse proxy server that can expose a local server to the internet through NATs and firewalls
-        ## Principle
         
         ![原理](https://i.imgtg.com/2023/02/08/cqhoI.png)
         
-        
         ## Features
-        - Easily manage port forwarding from anywhere via a browser
-        - Uses WebSocket encryption for secure communication between the public server and local client
-        - Easy to install with pip.
-        - Stable, automatically reconnects, and has been used in production environments
-        
-        ## Common Use Cases
-        
-        1. Host web servers from home
-        2. Manage IoT devices
+        1. Open port mapping via browser anytime and anywhere
+        2. Encrypted transmission between public network server and local network client via WebSocket
+        3. Few dependencies, one-click installation via pip
+        4. Stable, automatically reconnect, and already in production environment
+        5. Support for rate limiting
+        
+        ## Common Scenarios
+        1. Hosting website server at home
+        2. Managing IoT devices
         
         ## Installation
         
-        ```bash
-        pip install proxynt
         ```
-        
-        
-        ## Usage
-        Client
-        ```bash
-        nt_client --help
-        # start client
-        nt_client -c config_c.json
+        pip install -U proxynt
         ```
-        Server
         
-        ```bash
-        # view help
-        nt_server --help
-        # start server
-        nt_server -c config_s.json
-        ```
-        After starting the server, open the management page in a browser:
-        ```bash
-        The management page URL is the WebSocket path + /admin,
-        for example:
-        http://192.168.9.224:18888/websocket_path/admin
-        ```
-        ![ui](https://i.imgtg.com/2023/02/08/cqirD.png)
         
         ## Example: Accessing an Internal Network Machine via SSH
         
         Suppose the public server's IP is 192.168.9.224.
         
-        #### 1. Configure config_s.json on the public server
+        #### 1. Create `config_s.json` file on the public network machine
         
+        `config_s.json` content:
         
         ```json
         {
           "port": 18888,
           "password": "helloworld",
           "path": "/websocket_path",
           "admin": {
             "enable": true,  
             "admin_password": "new_password"  
           }
         }
         ```
-        Explanation:
         
-        - port: listening port
-        - password: connection password
-        - path: WebSocket path
-        - admin: management page configuration (not required)
-        - admin.enable: whether to enable the management page
-        - admin.admin_password: management password
         
-        Then start the server with:
-        ```bash
-        nt_server -c config_s.json
-        ```
         
-        #### 2. Configure config_c.json on the machine to be accessed
+        Then start:
+        `nt_server -c config_s.json`
+        
+        Explanation:
+        - `port`: Listening port
+        - `password`: Connection password
+        - `path`: WebSocket path
+        - `admin`: Management page configuration (optional)
+        - `admin.enable`: Whether to enable management page
+        - `admin.admin_password`: Management password
+        
+        #### 2. Create `config_c.json` file on the local network computer that needs to be accessed
+        
+        `config_c.json` content:
         
         ```json
         {
           "server": {
             "port": 18888,
             "host": "192.168.9.224",
             "https": false,
             "password": "helloworld",
             "path": "/websocket_path"
           },
           "client_name": "home_pc",
-          "client": [
-            {
-              "name": "ssh1",
-              "remote_port": 12222,
-              "local_port": 22,
-              "local_ip": "127.0.0.1"
-            }
-          ]
+          "client": []
         }
         ```
         
+        Then start:
+        `nt_client -c config_c.json`
+        
         Explanation:
+        - `server`: Configuration of the server to be connected, including port, IP address, whether to use HTTPS, password, and WebSocket path.
+        - `client_name`: Client name, needs to be unique.
+        - `client`: Empty array.
         
-        - `server`: configuration for the server to connect to, including port, IP address, whether to use HTTPS, password, and WebSocket path.
-        - `client_name`: name of the client, which must be unique.
-        - `client`: list of port forwarding configurations, mapping port 22 on the local machine to port 12222 on the server in this example.
+        #### 3. Open the server webpage `http://192.168.9.224:18888/websocket_path/admin` and add a port:
         
-        Then start the client with:
-        ```bash
-        nt_client -c config_c.json
-        ```
+        ![VWCvq.md.png](https://i.imgtg.com/2023/02/27/VWCvq.md.png)
         
-        #### 3. SSH connection
         
-        ```
+        Explanation: The management page path is **WebSocket path + /admin** .
+        #### 4. Configuration succeeded, use SSH to connect:
+        
+        ```bash
         ssh -oPort=12222 test@192.168.9.224
         ```
         
-        #### Open the management page
         
-        ```
-        http://192.168.9.224:18888/websocketpath/admin
-        ```
-        
-        ## Full Configuration Description (please delete the comments when using)
+        ## Complete Configuration Instructions (please delete the comments when using)
         
         
         - Client config_c.json
         
         ```json
         
         {
@@ -182,16 +149,26 @@
             "admin": {  
                 "enable": true,  // Whether to enable admin page
                 "admin_password": "new_password"  // Password for admin page
             }
         }
         
         ```
+        
+        
+        
+        ## Stargazers over time
+        
+        [![Stargazers over time](https://starchart.cc/sazima/proxynt.svg)](https://starchart.cc/sazima/proxynt)
+        
+        
         ## Update history
         
+        - 1.1.9: Bandwidth limitation
+        - 1.1.8: Display client version
         - 1.1.7: Fixed duplicate client_name
         - 1.1.6: Fixed client WebSocketException: socket is already opened.
```

### Comparing `proxynt-1.1.8/client/heart_beat_task.py` & `proxynt-1.1.9/client/heart_beat_task.py`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/client/tcp_forward_client.py` & `proxynt-1.1.9/client/tcp_forward_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,22 @@
+import asyncio
 import logging
 import socket
+import threading
 import time
 import traceback
 from threading import Lock
 from typing import Dict
 
 from common import websocket
 from common.logger_factory import LoggerFactory
 from common.nat_serialization import NatSerialization
 from common.pool import SelectPool
+from common.register_append_data import ResisterAppendData
+from common.speed_limit import SpeedLimiter
 from constant.message_type_constnat import MessageTypeConstant
 from constant.system_constant import SystemConstant
 from context.context_utils import ContextUtils
 from entity.message.message_entity import MessageEntity
 
 
 class TcpForwardClient:
@@ -21,25 +25,30 @@
         self.socket_to_uid: Dict[socket.socket, bytes] = dict()
         # self.name_to_addr: Dict[str, Tuple[str, int]] = name_to_addr
         self.uid_to_name: Dict[bytes, str] = dict()
         self.is_running = True
         self.ws = ws
         self.lock = Lock()
 
-        self.socket_event_loop =  SelectPool()
+        self.socket_event_loop = SelectPool()
 
     def start_forward(self):
         self.socket_event_loop.is_running = True
         self.socket_event_loop.run()
 
-    def handle_message(self, each: socket.socket):
-        # time.time()
+    def handle_message(self, each: socket.socket, data: ResisterAppendData):
         uid = self.socket_to_uid[each]
+        if data.speed_limiter and data.speed_limiter.is_exceed()[0]:
+            if LoggerFactory.get_logger().isEnabledFor(logging.DEBUG):
+                LoggerFactory.get_logger().debug('over speed')
+            self.socket_event_loop.unregister_and_register_delay(each, data, 1)
         try:
-            recv = each.recv(SystemConstant.CHUNK_SIZE)
+            recv = each.recv(data.read_size)
+            if data.speed_limiter:
+                data.speed_limiter.add(len(recv))
         except OSError:
             return
         send_message: MessageEntity = {
             'type_': MessageTypeConstant.WEBSOCKET_OVER_TCP,
             'data': {
                 'name': self.uid_to_name[uid],
                 'data': recv,
@@ -53,15 +62,15 @@
             LoggerFactory.get_logger().debug(f'send to ws cost time {time.time() - start_time}')
         if not recv:
             try:
                 self.close_connection(each)
             except Exception:
                 LoggerFactory.get_logger().error(f'close error: {traceback.format_exc()}')
 
-    def create_socket(self, name: str, uid: bytes, ip_port: str):
+    def create_socket(self, name: str, uid: bytes, ip_port: str, speed_limiter: SpeedLimiter):
         if uid in self.uid_to_socket:
             return
         with self.lock:
             if uid in self.uid_to_socket:  # 再次判断
                 return
             try:
                 if LoggerFactory.get_logger().isEnabledFor(logging.DEBUG):
@@ -71,15 +80,15 @@
                 ip, port = ip_port.split(':')
                 s.connect((ip, int(port)))
                 self.uid_to_socket[uid] = s  #
                 self.uid_to_name[uid] = name
                 self.socket_to_uid[s] = uid
                 if LoggerFactory.get_logger().isEnabledFor(logging.DEBUG):
                     LoggerFactory.get_logger().debug(f'register socket {name}, {uid}')
-                self.socket_event_loop.register(s, self.handle_message)
+                self.socket_event_loop.register(s, ResisterAppendData(self.handle_message, speed_limiter))
                 if LoggerFactory.get_logger().isEnabledFor(logging.DEBUG):
                     LoggerFactory.get_logger().debug(f'register socket success {name}, {uid}')
             except Exception:
                 LoggerFactory.get_logger().error(traceback.format_exc())
                 self.close_remote_socket(uid, name)
 
     def close_connection(self, socket_client: socket.socket):
```

### Comparing `proxynt-1.1.8/common/crypto/__init__.py` & `proxynt-1.1.9/common/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/common/crypto/table.py` & `proxynt-1.1.9/common/crypto/table.py`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/common/encrypt_utils.py` & `proxynt-1.1.9/common/encrypt_utils.py`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/common/logger_factory.py` & `proxynt-1.1.9/common/logger_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import os
 import logging
 import os
-from logging.handlers import TimedRotatingFileHandler
+from logging.handlers import TimedRotatingFileHandler, RotatingFileHandler
 
 from context.context_utils import ContextUtils
 
 
 # from pytz import timezone
 
 
 class LoggerFactory:
     fmt = '%(asctime)s  %(name)s %(levelname)s %(pathname)s %(funcName)s %(lineno)d : %(message)s'
     logger = logging.getLogger("logger")
     default_log_file = os.path.join('log', 'log.log')
-    backupCount = 30
+    backupCount = 10
+    MAX_BYTES = 1024 * 1024 * 5  # 5 MB
     # tz = 'Asia/Shanghai'
 
     @classmethod
     def get_logger(cls):
         if hasattr(cls, '_log'):
             return cls.logger
         cls.logger.setLevel(ContextUtils.get_log_level())
@@ -41,18 +42,16 @@
             if  cls.check_log_directory(ContextUtils.get_log_file()):
                 log_file = ContextUtils.get_log_file()
             else:
                 print(f'set log file to default: {os.path.abspath(cls.default_log_file)}')
                 log_file = cls.default_log_file
         else:
             log_file = cls.default_log_file
-        # log_file = ContextUtils.get_log_file() if ContextUtils.get_log_file() else  cls.default_log_file
         cls.check_log_directory(log_file)
-        print(f'log_file: {log_file}')
-        handler = TimedRotatingFileHandler(log_file, when="d", backupCount=cls.backupCount)
+        handler = RotatingFileHandler(log_file,  backupCount=cls.backupCount, maxBytes=cls.MAX_BYTES)
         formatter = logging.Formatter(cls.fmt)
         handler.setFormatter(formatter)
         logger.addHandler(handler)
 
     @classmethod
     def check_log_directory(cls, log_file: str):
         try:
```

### Comparing `proxynt-1.1.8/common/nat_serialization.py` & `proxynt-1.1.9/common/nat_serialization.py`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/common/websocket/__init__.py` & `proxynt-1.1.9/common/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/common/websocket/_abnf.py` & `proxynt-1.1.9/common/websocket/_abnf.py`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/common/websocket/_app.py` & `proxynt-1.1.9/common/websocket/_app.py`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/common/websocket/_cookiejar.py` & `proxynt-1.1.9/common/websocket/_cookiejar.py`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/common/websocket/_core.py` & `proxynt-1.1.9/common/websocket/_core.py`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/common/websocket/_exceptions.py` & `proxynt-1.1.9/common/websocket/_exceptions.py`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/common/websocket/_handshake.py` & `proxynt-1.1.9/common/websocket/_handshake.py`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/common/websocket/_http.py` & `proxynt-1.1.9/common/websocket/_http.py`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/common/websocket/_logging.py` & `proxynt-1.1.9/common/websocket/_logging.py`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/common/websocket/_socket.py` & `proxynt-1.1.9/common/websocket/_socket.py`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/common/websocket/_ssl_compat.py` & `proxynt-1.1.9/common/websocket/_ssl_compat.py`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/common/websocket/_url.py` & `proxynt-1.1.9/common/websocket/_url.py`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/common/websocket/_utils.py` & `proxynt-1.1.9/common/websocket/_utils.py`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/common/websocket/_wsdump.py` & `proxynt-1.1.9/common/websocket/_wsdump.py`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/common/websocket/tests/test_abnf.py` & `proxynt-1.1.9/common/websocket/tests/test_abnf.py`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/common/websocket/tests/test_app.py` & `proxynt-1.1.9/common/websocket/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/common/websocket/tests/test_cookiejar.py` & `proxynt-1.1.9/common/websocket/tests/test_cookiejar.py`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/common/websocket/tests/test_http.py` & `proxynt-1.1.9/common/websocket/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/common/websocket/tests/test_url.py` & `proxynt-1.1.9/common/websocket/tests/test_url.py`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/common/websocket/tests/test_websocket.py` & `proxynt-1.1.9/common/websocket/tests/test_websocket.py`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/context/context_utils.py` & `proxynt-1.1.9/context/context_utils.py`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/proxynt.egg-info/PKG-INFO` & `proxynt-1.1.9/proxynt.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,143 +1,110 @@
 Metadata-Version: 2.1
 Name: proxynt
-Version: 1.1.8
+Version: 1.1.9
 Summary: UNKNOWN
 Home-page: https://github.com/sazima/proxynt
 License: UNKNOWN
-Description: # 
-        
-        [中文](https://github.com/sazima/proxynt/blob/master/readme.md)
+Description: [中文](https://github.com/sazima/proxynt/blob/master/readme.md)
         
         ProxyNT is a reverse proxy server that can expose a local server to the internet through NATs and firewalls
-        ## Principle
         
         ![原理](https://i.imgtg.com/2023/02/08/cqhoI.png)
         
-        
         ## Features
-        - Easily manage port forwarding from anywhere via a browser
-        - Uses WebSocket encryption for secure communication between the public server and local client
-        - Easy to install with pip.
-        - Stable, automatically reconnects, and has been used in production environments
-        
-        ## Common Use Cases
-        
-        1. Host web servers from home
-        2. Manage IoT devices
+        1. Open port mapping via browser anytime and anywhere
+        2. Encrypted transmission between public network server and local network client via WebSocket
+        3. Few dependencies, one-click installation via pip
+        4. Stable, automatically reconnect, and already in production environment
+        5. Support for rate limiting
+        
+        ## Common Scenarios
+        1. Hosting website server at home
+        2. Managing IoT devices
         
         ## Installation
         
-        ```bash
-        pip install proxynt
         ```
-        
-        
-        ## Usage
-        Client
-        ```bash
-        nt_client --help
-        # start client
-        nt_client -c config_c.json
+        pip install -U proxynt
         ```
-        Server
         
-        ```bash
-        # view help
-        nt_server --help
-        # start server
-        nt_server -c config_s.json
-        ```
-        After starting the server, open the management page in a browser:
-        ```bash
-        The management page URL is the WebSocket path + /admin,
-        for example:
-        http://192.168.9.224:18888/websocket_path/admin
-        ```
-        ![ui](https://i.imgtg.com/2023/02/08/cqirD.png)
         
         ## Example: Accessing an Internal Network Machine via SSH
         
         Suppose the public server's IP is 192.168.9.224.
         
-        #### 1. Configure config_s.json on the public server
+        #### 1. Create `config_s.json` file on the public network machine
         
+        `config_s.json` content:
         
         ```json
         {
           "port": 18888,
           "password": "helloworld",
           "path": "/websocket_path",
           "admin": {
             "enable": true,  
             "admin_password": "new_password"  
           }
         }
         ```
-        Explanation:
         
-        - port: listening port
-        - password: connection password
-        - path: WebSocket path
-        - admin: management page configuration (not required)
-        - admin.enable: whether to enable the management page
-        - admin.admin_password: management password
         
-        Then start the server with:
-        ```bash
-        nt_server -c config_s.json
-        ```
         
-        #### 2. Configure config_c.json on the machine to be accessed
+        Then start:
+        `nt_server -c config_s.json`
+        
+        Explanation:
+        - `port`: Listening port
+        - `password`: Connection password
+        - `path`: WebSocket path
+        - `admin`: Management page configuration (optional)
+        - `admin.enable`: Whether to enable management page
+        - `admin.admin_password`: Management password
+        
+        #### 2. Create `config_c.json` file on the local network computer that needs to be accessed
+        
+        `config_c.json` content:
         
         ```json
         {
           "server": {
             "port": 18888,
             "host": "192.168.9.224",
             "https": false,
             "password": "helloworld",
             "path": "/websocket_path"
           },
           "client_name": "home_pc",
-          "client": [
-            {
-              "name": "ssh1",
-              "remote_port": 12222,
-              "local_port": 22,
-              "local_ip": "127.0.0.1"
-            }
-          ]
+          "client": []
         }
         ```
         
+        Then start:
+        `nt_client -c config_c.json`
+        
         Explanation:
+        - `server`: Configuration of the server to be connected, including port, IP address, whether to use HTTPS, password, and WebSocket path.
+        - `client_name`: Client name, needs to be unique.
+        - `client`: Empty array.
         
-        - `server`: configuration for the server to connect to, including port, IP address, whether to use HTTPS, password, and WebSocket path.
-        - `client_name`: name of the client, which must be unique.
-        - `client`: list of port forwarding configurations, mapping port 22 on the local machine to port 12222 on the server in this example.
+        #### 3. Open the server webpage `http://192.168.9.224:18888/websocket_path/admin` and add a port:
         
-        Then start the client with:
-        ```bash
-        nt_client -c config_c.json
-        ```
+        ![VWCvq.md.png](https://i.imgtg.com/2023/02/27/VWCvq.md.png)
         
-        #### 3. SSH connection
         
-        ```
+        Explanation: The management page path is **WebSocket path + /admin** .
+        #### 4. Configuration succeeded, use SSH to connect:
+        
+        ```bash
         ssh -oPort=12222 test@192.168.9.224
         ```
         
-        #### Open the management page
         
-        ```
-        http://192.168.9.224:18888/websocketpath/admin
-        ```
-        
-        ## Full Configuration Description (please delete the comments when using)
+        ## Complete Configuration Instructions (please delete the comments when using)
         
         
         - Client config_c.json
         
         ```json
         
         {
@@ -182,16 +149,26 @@
             "admin": {  
                 "enable": true,  // Whether to enable admin page
                 "admin_password": "new_password"  // Password for admin page
             }
         }
         
         ```
+        
+        
+        
+        ## Stargazers over time
+        
+        [![Stargazers over time](https://starchart.cc/sazima/proxynt.svg)](https://starchart.cc/sazima/proxynt)
+        
+        
         ## Update history
         
+        - 1.1.9: Bandwidth limitation
+        - 1.1.8: Display client version
         - 1.1.7: Fixed duplicate client_name
         - 1.1.6: Fixed client WebSocketException: socket is already opened.
```

### Comparing `proxynt-1.1.8/proxynt.egg-info/SOURCES.txt` & `proxynt-1.1.9/proxynt.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 ./client/heart_beat_task.py
 ./client/tcp_forward_client.py
 ./common/__init__.py
 ./common/encrypt_utils.py
 ./common/logger_factory.py
 ./common/nat_serialization.py
 ./common/pool.py
+./common/register_append_data.py
+./common/speed_limit.py
 ./common/crypto/__init__.py
 ./common/crypto/table.py
 ./common/websocket/__init__.py
 ./common/websocket/_abnf.py
 ./common/websocket/_app.py
 ./common/websocket/_cookiejar.py
 ./common/websocket/_core.py
```

### Comparing `proxynt-1.1.8/run_client.py` & `proxynt-1.1.9/run_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 import socket
 import sys
 import threading
 import time
 import traceback
 from optparse import OptionParser
 from threading import Thread
-from typing import List, Set
+from typing import List, Set, Dict
 
+from tornado import ioloop
 
 sys.path.insert(0, os.path.dirname(os.path.abspath(__file__)))
 
+from common.speed_limit import SpeedLimiter
 from common.websocket import WebSocketException
-from tornado import ioloop
 
 from client.clear_nonce_task import ClearNonceTask
 from client.heart_beat_task import HeatBeatTask
 from client.tcp_forward_client import TcpForwardClient
 from common import websocket
 from common.logger_factory import LoggerFactory
 from common.nat_serialization import NatSerialization
@@ -37,48 +38,39 @@
 except (ImportError, ModuleNotFoundError):
     _logger = None
 
 DEFAULT_CONFIG = './config_c.json'
 
 DEFAULT_LOGGER_LEVEL = logging.INFO
 
-name_to_level = {
+NAME_TO_LEVEL = {
     'debug': logging.DEBUG,
     'info': logging.INFO,
     'warn': logging.WARN,
     'error': logging.ERROR
 }
 
-level_to_name = {
-    k: v.upper() for v, k in name_to_level.items()
-}
 OPEN_CLOSE_LOCK = threading.Lock()
 
+name_to_speed_limiter: Dict[str, SpeedLimiter] = {}
 
 def get_config() -> ClientConfigEntity:
     parser = OptionParser(usage="""usage: %prog -c config_c.json 
     
 config_c.json example: 
 {
   "server": {
     "port": 18888,
     "host": "192.168.9.224",
     "https": false,
     "password": "helloworld",
     "path": "/websocket_path"
   },
    "client_name": "ubuntu1",
-  "client": [
-    {
-      "name": "ssh1",
-      "remote_port": 12222,
-      "local_port": 22,
-      "local_ip": "127.0.0.1"
-    }
-  ],
+  "client": [],
   "log_file": "/var/log/nt/nt.log"
 }
     """, version=SystemConstant.VERSION)
     parser.add_option("-c", "--config",
                       type='str',
                       dest='config',
                       default=DEFAULT_CONFIG,
@@ -88,24 +80,25 @@
                       type='str',
                       dest='log_level',
                       default='info',
                       help="log level: debug, info, warn , error"
                       )
     (options, args) = parser.parse_args()
     log_level = options.log_level
-    if log_level not in name_to_level:
+    if log_level not in NAME_TO_LEVEL:
         print('invalid log level.')
         sys.exit()
-    ContextUtils.set_log_level(name_to_level[log_level])
+    ContextUtils.set_log_level(NAME_TO_LEVEL[log_level])
     config_path = options.config
     with open(config_path, 'r') as rf:
         config_data: ClientConfigEntity = json.loads(rf.read())
     ContextUtils.set_config_file_path(os.path.abspath(config_path))
     ContextUtils.set_password(config_data['server']['password'])
     name_set: Set[str] = set()
+    config_data.setdefault('client', [])
     for client in config_data['client']:
         if client['name'] in name_set:
             raise DuplicatedName()
         name_set.add(client['name'])
     return config_data
 
 
@@ -121,30 +114,33 @@
 
     def on_message(self, ws, message: bytes):
         try:
             message_data: MessageEntity = NatSerialization.loads(message, ContextUtils.get_password())
             start_time = time.time()
             time_ = message_data['type_']
             if message_data['type_'] == MessageTypeConstant.WEBSOCKET_OVER_TCP:
-                # LoggerFactory.get_logger().debug(f'get websocket message {message_data}')
                 data: TcpOverWebsocketMessage = message_data['data']
                 uid = data['uid']
                 name = data['name']
                 b = data['data']
-                self.forward_client.create_socket(name, uid, data['ip_port'])
+                self.forward_client.create_socket(name, uid, data['ip_port'], name_to_speed_limiter.get(name))
                 self.forward_client.send_by_uid(uid, b)
             elif message_data['type_'] == MessageTypeConstant.REQUEST_TO_CONNECT:
                 data: TcpOverWebsocketMessage = message_data['data']
                 uid = data['uid']
                 name = data['name']
                 b = data['data']
-                self.forward_client.create_socket(name, uid, data['ip_port'])
+                self.forward_client.create_socket(name, uid, data['ip_port'], name_to_speed_limiter.get(name))
             elif message_data['type_'] == MessageTypeConstant.PING:
                 self.heart_beat_task.set_recv_heart_beat_time(time.time())
-
+            elif message_data['type_'] == MessageTypeConstant.PUSH_CONFIG:
+                push_config: PushConfigEntity = message_data['data']
+                for d in push_config['config_list']:
+                    if d.get('speed_limit'):
+                        name_to_speed_limiter[d['name']] = SpeedLimiter(d['speed_limit'])
         except Exception:
             LoggerFactory.get_logger().error(traceback.format_exc())
         # LoggerFactory.get_logger().debug(f'on message {time_} cost time {time.time() - start_time}')
 
     def on_error(self, ws, error):
         LoggerFactory.get_logger().error(f'error:  {error} ')
```

### Comparing `proxynt-1.1.8/run_server.py` & `proxynt-1.1.9/run_server.py`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/server/admin_http_handler.py` & `proxynt-1.1.9/server/admin_http_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import base64
 import json
 import os
 import time
 import traceback
-from typing import List, Set
+from typing import List, Set, Tuple
 
 from tornado.web import RequestHandler
 
 from common.logger_factory import LoggerFactory
 from constant.system_constant import SystemConstant
 from context.context_utils import ContextUtils
 from entity.message.push_config_entity import PushConfigEntity, ClientData
@@ -116,14 +116,15 @@
                 'data': return_list,
                 'msg': ''
             })
         except Exception:
             LoggerFactory.get_logger().error(traceback.format_exc())
 
     def delete(self, *args, **kwargs):
+        """删除"""
         try:
             # request_data = json.loads(self.request.body)
             cookie_dict = ContextUtils.get_cookie_to_time()
             result = self.get_cookie(COOKIE_KEY)
             if result not in cookie_dict or time.time() - cookie_dict[result] >= SystemConstant.COOKIE_EXPIRE_SECONDS:
                 self.write({
                     'code': NOT_LOGIN,
@@ -157,124 +158,142 @@
             self.update_config_file()
             if client_name in MyWebSocketaHandler.client_name_to_handler:
                 MyWebSocketaHandler.client_name_to_handler[client_name].close(0, 'close by server')
         except Exception:
             LoggerFactory.get_logger().error(traceback.format_exc())
 
     async def post(self):
+        """新增  或 编辑"""
         try:
             cookie_dict = ContextUtils.get_cookie_to_time()
             result = self.get_cookie(COOKIE_KEY)
             if result not in cookie_dict or time.time() - cookie_dict[result] >= SystemConstant.COOKIE_EXPIRE_SECONDS:
                 self.write({
                     'code': NOT_LOGIN,
                     'data': '',
                     'msg': '登录信息已经过期, 请重新刷新页面'
                 })
                 return
-            online_client_name_list: List[str] = list(MyWebSocketaHandler.client_name_to_handler.keys())
             request_data = json.loads(self.request.body)
             LoggerFactory.get_logger().info(f'add config {request_data}')
             client_name = request_data.get('client_name')
             name = request_data.get('name')
             remote_port = int(request_data.get('remote_port'))
+            is_edit = request_data.get('is_edit', False)  # 是否是编辑
             local_ip = request_data.get('local_ip')
             local_port = int(request_data.get('local_port'))
+            speed_limit = float(request_data.get('speed_limit'))
             if not client_name:
                 self.write({
                     'code': 400,
                     'data': '',
                     'msg': 'client name 不能为空'
                 })
                 return
             if not remote_port:
                 self.write({
                     'code': 400,
                     'data': '',
                     'msg': '远程ip不能为空'
                 })
                 return
-            if not local_ip:
+            if speed_limit < 0:
                 self.write({
                     'code': 400,
                     'data': '',
-                    'msg': '必填local_ip'
+                    'msg': '限速必须大于等于0'
                 })
                 return
-            if not local_port or (local_port <= 0 or local_port > 65535):
+            if not local_ip:
                 self.write({
                     'code': 400,
                     'data': '',
-                    'msg': '本地port不合法'
+                    'msg': '必填local_ip'
                 })
                 return
-            if client_name in MyWebSocketaHandler.client_name_to_handler:
-                handler = MyWebSocketaHandler.client_name_to_handler[client_name]
-                names = handler.names
-            else:
-                names = set()
-            if not name or name in names:
+            if not local_port or (local_port <= 0 or local_port > 65535):
                 self.write({
                     'code': 400,
                     'data': '',
-                    'msg': 'name不合法或者重复'
+                    'msg': '本地port不合法'
                 })
                 return
-            if self.is_port_in_use(remote_port):
+            if remote_port < MIN_PORT:
                 self.write({
                     'code': 400,
                     'data': '',
-                    'msg': '远程端口已占用, 请更换端口'
+                    'msg': f'端口最小为 {MIN_PORT}, 请更换端口'
                 })
                 return
-            if remote_port < MIN_PORT:
+            if not is_edit:
+                is_ok, msg = self._add(client_name, name, remote_port, local_port, local_ip, speed_limit)
+            else:
+                is_ok, msg = self._edit(client_name, name, remote_port, local_port, local_ip, speed_limit)
+            if not is_ok:
                 self.write({
                     'code': 400,
                     'data': '',
-                    'msg': f'端口最小为 {MIN_PORT}, 请更换端口'
+                    'msg': msg
                 })
                 return
-
-            new_config: ClientData = {
-                'name': name,
-                'remote_port': remote_port,
-                'local_port': local_port,
-                'local_ip': local_ip
-            }
-
-            client_name_to_config_in_server = ContextUtils.get_client_name_to_config_in_server()
-            if client_name in client_name_to_config_in_server:
-                for c in client_name_to_config_in_server[client_name]:
-                    if c['name'] == name:
-                        self.write({
-                            'code': 400,
-                            'data': '',
-                            'msg': 'name不合法'
-                        })
-                        return
-                client_name_to_config_in_server[client_name].append(new_config)  # 更新配置
-            else:
-                client_name_to_config_in_server[client_name] = [new_config]  # 更新配置
             if client_name in MyWebSocketaHandler.client_name_to_handler:
                 MyWebSocketaHandler.client_name_to_handler[client_name].close(0, 'close by server')
             self.write({
                 'code': 200,
                 'data': '',
                 'msg': '成功'
             })
             self.update_config_file()
             return
-            # with open(config_file_path, 'rb') as rf:
-            #     server_config_data: ServerConfigEntity = json.load(rf)
-            # client_config = server_config_data.get('client_config')
-            # if not client_config:
-            #     pass
         except Exception:
             LoggerFactory.get_logger().error(traceback.format_exc())
 
+    def _edit(self, client_name: str, name: str, remote_port: int, local_port: int, local_ip: str, speed_limit: float) -> Tuple[bool, str]:
+        client_name_to_config_in_server = ContextUtils.get_client_name_to_config_in_server()
+        if client_name not in client_name_to_config_in_server:
+            return True,  '该客户端名称不存在'
+        for c in client_name_to_config_in_server[client_name]:
+            if c['name'] == name:  # 修改的这条配置
+                if c['remote_port'] != remote_port:
+                    if self.is_port_in_use(remote_port):
+                        return False, '远程端口已占用, 请更换端口'
+                c['local_ip'] = local_ip
+                c['remote_port'] = remote_port
+                c['local_port'] = local_port
+                c['speed_limit'] = speed_limit
+                return True, ''
+        return False, '编辑的名称不存在'
+
+    def _add(self, client_name: str, name: str, remote_port: int, local_port: int, local_ip: str, speed_limit: float ) -> Tuple[bool, str]:
+        client_name_to_config_in_server = ContextUtils.get_client_name_to_config_in_server()
+        if client_name in MyWebSocketaHandler.client_name_to_handler:
+            handler = MyWebSocketaHandler.client_name_to_handler[client_name]
+            names = handler.names
+        else:
+            names = set()
+        if name in names:
+            return False, 'name不合法或者重复'
+        if self.is_port_in_use(remote_port):
+            return False, '远程端口已占用, 请更换端口'
+        new_config: ClientData = {
+            'name': name,
+            'remote_port': remote_port,
+            'local_port': local_port,
+            'local_ip': local_ip,
+            'speed_limit': speed_limit
+        }
+        if client_name in client_name_to_config_in_server:
+            for c in client_name_to_config_in_server[client_name]:
+                if c['name'] == name:
+                    return False,  'name不合法'
+            client_name_to_config_in_server[client_name].append(new_config)  # 更新配置
+        else:
+            client_name_to_config_in_server[client_name] = [new_config]  # 更新配置
+        return True, ''
+
     def update_config_file(self):
         with open(ContextUtils.get_config_file_path(), 'r') as rf:
             content = rf.read()
         server_config: ServerConfigEntity = json.loads(content)
         server_config['client_config'] = ContextUtils.get_client_name_to_config_in_server()
         with open(ContextUtils.get_config_file_path(), 'w') as wf:
             wf.write(json.dumps(server_config, ensure_ascii=False, indent=4))
```

### Comparing `proxynt-1.1.8/server/task/check_cookie_task.py` & `proxynt-1.1.9/server/task/check_cookie_task.py`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/server/task/heart_beat_task.py` & `proxynt-1.1.9/server/task/heart_beat_task.py`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/server/tcp_forward_client.py` & `proxynt-1.1.9/server/tcp_forward_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,31 +12,35 @@
 import os
 
 import tornado
 
 from common.logger_factory import LoggerFactory
 from common.nat_serialization import NatSerialization
 from common.pool import SelectPool
+from common.register_append_data import ResisterAppendData
+from common.speed_limit import SpeedLimiter
 from constant.message_type_constnat import MessageTypeConstant
 from constant.system_constant import SystemConstant
 from context.context_utils import ContextUtils
 from entity.message.message_entity import MessageEntity
 
 
 class TcpForwardClient:
     _instance = None
 
     def __init__(self,  loop, tornado_loop):
         self.socket_event_loop =  SelectPool()
-        self.uid_to_client: Dict[bytes, socket.socket] = dict()
-        self.client_to_uid: Dict[socket.socket, bytes] = dict()
-        self.uid_to_name_ip_port : Dict[bytes, Tuple[str, str]]  = dict()
+        self.uid_to_client: Dict[bytes, socket.socket] = dict()   # uid 对应的连接公网端口的客户端
+        self.client_to_uid: Dict[socket.socket, bytes] = dict()  # 连接公网端口的客户端 对应的uid
+        self.uid_to_name_ip_port : Dict[bytes, Tuple[str, str]]  = dict()  # uid 对应的内网ipport
+
+        self.uid_to_listen_socket_server: Dict[bytes, socket.socket]  = dict()  # uid对应的监听socket
 
-        self.uid_to_listen_socket_server: Dict[bytes, socket.socket]  = dict()
         self.listen_socket_server_to_name_ip_port: Dict[socket.socket, Tuple[str, str]]  = dict()
+
         self.listen_socket_server_to_handler: Dict[socket.socket, 'MyWebSocketaHandler']  = dict()
 
         self.listen_socket_server_to_uid_set: Dict[socket.socket, Set] = defaultdict(set)
         self.client_name_to_listen_socket_server: Dict[str, List[socket.socket]] = defaultdict(list)
 
         self.tornado_loop = tornado_loop
         self.close_lock = Lock()
@@ -47,26 +51,24 @@
     @classmethod
     def get_instance(cls) -> 'TcpForwardClient':
         if cls._instance is None:
             cls._instance = cls(asyncio.get_event_loop(), tornado.ioloop.IOLoop.current())
             Thread(target=cls._instance.socket_event_loop.run).start()
         return cls._instance
 
-    def register_client(self, s: socket.socket):
-        self.socket_event_loop.register(s, self.handle_message)
-
-    async def register_listen_server(self, s: socket.socket, name: str, ip_port: str, websocket_handler: 'MyWebSocketaHandler'):
+    async def register_listen_server(self, s: socket.socket, name: str, ip_port: str, websocket_handler: 'MyWebSocketaHandler', speed_limit_size: float):
         client_name = websocket_handler.client_name
         if client_name not in self.client_name_to_lock:
             self.client_name_to_lock[client_name] = AsyncioLock()
         async with self.client_name_to_lock.get(client_name):
             self.listen_socket_server_to_name_ip_port[s] = (name, ip_port)
             self.listen_socket_server_to_handler[s] = websocket_handler
             self.client_name_to_listen_socket_server[client_name].append(s)
-            self.socket_event_loop.register(s, self.start_accept)
+            append_data = ResisterAppendData(self.start_accept, SpeedLimiter(speed_limit_size) if speed_limit_size else None)
+            self.socket_event_loop.register(s, append_data)
 
     async def close_by_client_name(self, client_name: str):
         if client_name not in self.client_name_to_listen_socket_server:
             return
         if client_name not in self.client_name_to_lock:
             self.client_name_to_lock[client_name] = AsyncioLock()
         async with self.client_name_to_lock.get(client_name):
@@ -103,19 +105,25 @@
                     self.uid_to_listen_socket_server.pop(u)
                 if u in self.uid_to_name_ip_port:
                     self.uid_to_name_ip_port.pop(u)
             self.client_name_to_listen_socket_server.pop(client_name)
             self.client_name_to_lock.pop(client_name)
         # self.client_name_to_lock.o
 
-    def handle_message(self, each: socket.socket):
+    def handle_message(self, each: socket.socket,  data: ResisterAppendData):
         # 发送到websocket
         each: socket.socket
+        if data.speed_limiter and data.speed_limiter.is_exceed()[0]:
+            if LoggerFactory.get_logger().isEnabledFor(logging.DEBUG):
+                LoggerFactory.get_logger().debug('over speed')
+            self.socket_event_loop.unregister_and_register_delay(each, data, 1)
         try:
-            recv = each.recv(SystemConstant.CHUNK_SIZE)
+            recv = each.recv(data.read_size)
+            if data.speed_limiter:
+                data.speed_limiter.add(len(recv))
         except ConnectionResetError:
             recv = b''
         # client = self.uid_to_client[uid]
         uid = self.client_to_uid[each]
         name, ip_port = self.uid_to_name_ip_port[uid]
         send_message: MessageEntity = {
             'type_': MessageTypeConstant.WEBSOCKET_OVER_TCP,
@@ -137,15 +145,15 @@
         try:
 
             self.tornado_loop.add_callback(
                 partial(handler.write_message, NatSerialization.dumps(send_message, ContextUtils.get_password())), True)
         except Exception:
             LoggerFactory.get_logger().error(traceback.format_exc())
 
-    def start_accept(self, s: socket):
+    def start_accept(self, s: socket, register_append_data: ResisterAppendData):
         # LoggerFactory.get_logger().info(f'start accept {self.listen_port}')
         # self.socket_event_loop.is_running = True
         # Thread(target=self.socket_event_loop.run).start()
         # while self.is_running:
         #     rs, ws, es = select.select([self.socket], [self.socket], [self.socket])
         #     for each in rs:
         #         if self.socket is None:
@@ -154,23 +162,23 @@
             client, address = s.accept()
         except OSError:
             return
         LoggerFactory.get_logger().info(f'get connect : {address}')
         # 当前 服务端的client 也会对应服务端连接内网服务的一个 client
         uid = os.urandom(4)
         handler = self.listen_socket_server_to_handler[s]
-
         self.listen_socket_server_to_uid_set[s].add(uid)
         self.uid_to_client[uid] = client
         self.client_to_uid[client] = uid
         self.uid_to_listen_socket_server[uid] = s
         name, ip_port = self.listen_socket_server_to_name_ip_port[s]
         self.uid_to_name_ip_port[uid] = (name, ip_port)
         Thread(target=self.request_to_connect, args=(uid, )).start()
-        self.register_client(client)
+        append_data = ResisterAppendData(self.handle_message, register_append_data.speed_limiter)
+        self.socket_event_loop.register(client, append_data)
 
     def request_to_connect(self, uid: bytes):
         """请求连接客户端"""
         client = self.uid_to_client[uid]
         name, ip_port = self.uid_to_name_ip_port[uid]
         send_message: MessageEntity = {
             'type_': MessageTypeConstant.REQUEST_TO_CONNECT,
```

### Comparing `proxynt-1.1.8/server/template/base.html` & `proxynt-1.1.9/server/template/base.html`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/server/template/css/fonts/element-icons.woff` & `proxynt-1.1.9/server/template/css/fonts/element-icons.woff`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/server/template/css/index.css` & `proxynt-1.1.9/server/template/css/index.css`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/server/template/ele_index.html` & `proxynt-1.1.9/server/template/ele_index.html`

 * *Files 12% similar despite different names*

```diff
@@ -73,426 +73,523 @@
 00000480: abaf e58f a322 0a20 2020 2020 2020 2020  .....".         
 00000490: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000004a0: 2020 2077 6964 7468 3d22 3138 3022 3e0a     width="180">.
 000004b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000004c0: 2020 2020 3c2f 656c 2d74 6162 6c65 2d63      </el-table-c
 000004d0: 6f6c 756d 6e3e 0a20 2020 2020 2020 2020  olumn>.         
 000004e0: 2020 2020 2020 2020 2020 203c 656c 2d74             <el-t
-000004f0: 6162 6c65 2d63 6f6c 756d 6e20 6c61 6265  able-column labe
-00000500: 6c3d 22e6 938d e4bd 9c22 2077 6964 7468  l="......" width
-00000510: 3d22 3130 3022 3e0a 0a20 2020 2020 2020  ="100">..       
-00000520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000530: 203c 7465 6d70 6c61 7465 2073 6c6f 742d   <template slot-
-00000540: 7363 6f70 653d 2273 636f 7065 223e 0a0a  scope="scope">..
-00000550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000560: 2020 2020 2020 2020 2020 2020 3c65 6c2d              <el-
-00000570: 6275 7474 6f6e 203a 6469 7361 626c 6564  button :disabled
-00000580: 3d22 7072 6f70 732e 726f 772e 6361 6e5f  ="props.row.can_
-00000590: 6465 6c65 7465 5f6e 616d 6573 2e69 6e64  delete_names.ind
-000005a0: 6578 4f66 2873 636f 7065 2e72 6f77 2e6e  exOf(scope.row.n
-000005b0: 616d 6529 203d 3d3d 202d 3120 220a 2020  ame) === -1 ".  
-000005c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005e0: 2020 2020 2073 697a 653d 226d 696e 6922       size="mini"
-000005f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000610: 2020 2020 2020 2020 4063 6c69 636b 3d22          @click="
-00000620: 6861 6e64 6c65 4465 6c65 7465 2870 726f  handleDelete(pro
-00000630: 7073 2e72 6f77 2e63 6c69 656e 745f 6e61  ps.row.client_na
-00000640: 6d65 2c20 7363 6f70 652e 726f 772e 6e61  me, scope.row.na
-00000650: 6d65 2922 3ee5 88a0 e999 a40a 2020 2020  me)">.......    
-00000660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000670: 2020 2020 2020 2020 3c2f 656c 2d62 7574          </el-but
-00000680: 746f 6e3e 0a20 2020 2020 2020 2020 2020  ton>.           
-00000690: 2020 2020 2020 2020 2020 2020 203c 2f74               </t
-000006a0: 656d 706c 6174 653e 0a20 2020 2020 2020  emplate>.       
-000006b0: 2020 2020 2020 2020 2020 2020 203c 2f65               </e
-000006c0: 6c2d 7461 626c 652d 636f 6c75 6d6e 3e0a  l-table-column>.
+000004f0: 6162 6c65 2d63 6f6c 756d 6e0a 2020 2020  able-column.    
+00000500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000510: 2020 2020 2020 2020 7072 6f70 3d22 7370          prop="sp
+00000520: 6565 645f 6c69 6d69 7422 0a20 2020 2020  eed_limit".     
+00000530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000540: 2020 2020 2020 206c 6162 656c 3d22 e999         label="..
+00000550: 90e9 809f 28e5 8d95 e4bd 8d4d 4229 220a  ....(......MB)".
+00000560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000570: 2020 2020 2020 2020 2020 2020 7769 6474              widt
+00000580: 683d 2231 3830 223e 0a20 2020 2020 2020  h="180">.       
+00000590: 2020 2020 2020 2020 2020 2020 203c 2f65               </e
+000005a0: 6c2d 7461 626c 652d 636f 6c75 6d6e 3e0a  l-table-column>.
+000005b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005c0: 2020 2020 3c65 6c2d 7461 626c 652d 636f      <el-table-co
+000005d0: 6c75 6d6e 206c 6162 656c 3d22 e693 8de4  lumn label="....
+000005e0: bd9c 2220 7769 6474 683d 2232 3030 223e  .." width="200">
+000005f0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000600: 2020 2020 2020 2020 2020 3c74 656d 706c            <templ
+00000610: 6174 6520 736c 6f74 2d73 636f 7065 3d22  ate slot-scope="
+00000620: 7363 6f70 6522 3e0a 2020 2020 2020 2020  scope">.        
+00000630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000640: 2020 2020 3c65 6c2d 726f 773e 0a20 2020      <el-row>.   
+00000650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000660: 2020 2020 2020 2020 2020 2020 203c 656c               <el
+00000670: 2d62 7574 746f 6e20 3a64 6973 6162 6c65  -button :disable
+00000680: 643d 2270 726f 7073 2e72 6f77 2e63 616e  d="props.row.can
+00000690: 5f64 656c 6574 655f 6e61 6d65 732e 696e  _delete_names.in
+000006a0: 6465 784f 6628 7363 6f70 652e 726f 772e  dexOf(scope.row.
+000006b0: 6e61 6d65 2920 3d3d 3d20 2d31 2022 0a20  name) === -1 ". 
+000006c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000006d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006e0: 3c2f 656c 2d74 6162 6c65 3e0a 2020 2020  </el-table>.    
-000006f0: 2020 2020 2020 2020 3c2f 7465 6d70 6c61          </templa
-00000700: 7465 3e0a 2020 2020 2020 2020 3c2f 656c  te>.        </el
-00000710: 2d74 6162 6c65 2d63 6f6c 756d 6e3e 0a20  -table-column>. 
-00000720: 2020 2020 2020 203c 656c 2d74 6162 6c65         <el-table
-00000730: 2d63 6f6c 756d 6e0a 2020 2020 2020 2020  -column.        
-00000740: 2020 2020 2020 2020 7072 6f70 3d22 636c          prop="cl
-00000750: 6965 6e74 5f6e 616d 6522 0a20 2020 2020  ient_name".     
-00000760: 2020 2020 2020 2020 2020 206c 6162 656c             label
-00000770: 3d22 e590 8de7 a7b0 220a 2020 2020 2020  ="......".      
-00000780: 2020 3e0a 2020 2020 2020 2020 3c2f 656c    >.        </el
-00000790: 2d74 6162 6c65 2d63 6f6c 756d 6e3e 0a20  -table-column>. 
-000007a0: 2020 2020 2020 203c 656c 2d74 6162 6c65         <el-table
-000007b0: 2d63 6f6c 756d 6e0a 2020 2020 2020 2020  -column.        
-000007c0: 2020 2020 2020 2020 7072 6f70 3d22 7665          prop="ve
-000007d0: 7273 696f 6e22 0a20 2020 2020 2020 2020  rsion".         
-000007e0: 2020 2020 2020 206c 6162 656c 3d22 e789         label="..
-000007f0: 88e6 9cac 220a 2020 2020 2020 2020 3e0a  ....".        >.
-00000800: 2020 2020 2020 2020 3c2f 656c 2d74 6162          </el-tab
-00000810: 6c65 2d63 6f6c 756d 6e3e 0a20 2020 2020  le-column>.     
-00000820: 2020 203c 656c 2d74 6162 6c65 2d63 6f6c     <el-table-col
-00000830: 756d 6e0a 2020 2020 2020 2020 2020 2020  umn.            
-00000840: 2020 2020 7072 6f70 3d22 7374 6174 7573      prop="status
-00000850: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00000860: 2020 6c61 6265 6c3d 22e7 8ab6 e680 8122    label="......"
-00000870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000880: 203a 6669 6c74 6572 733d 225b 7b20 7465   :filters="[{ te
-00000890: 7874 3a20 276f 6e6c 696e 6527 2c20 7661  xt: 'online', va
-000008a0: 6c75 653a 2027 6f6e 6c69 6e65 2720 7d2c  lue: 'online' },
-000008b0: 207b 2074 6578 743a 2027 6f66 666c 696e   { text: 'offlin
-000008c0: 6527 2c20 7661 6c75 653a 2027 6f66 666c  e', value: 'offl
-000008d0: 696e 6527 207d 5d22 0a20 2020 2020 2020  ine' }]".       
-000008e0: 2020 2020 2020 2020 2066 696c 7465 722d           filter-
-000008f0: 706c 6163 656d 656e 743d 2262 6f74 746f  placement="botto
-00000900: 6d2d 656e 6422 3e0a 2020 2020 2020 2020  m-end">.        
-00000910: 2020 2020 3c74 656d 706c 6174 6520 736c      <template sl
-00000920: 6f74 2d73 636f 7065 3d22 7363 6f70 6522  ot-scope="scope"
-00000930: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00000940: 2020 3c65 6c2d 7461 670a 2020 2020 2020    <el-tag.      
-00000950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000960: 2020 3a74 7970 653d 2273 636f 7065 2e72    :type="scope.r
-00000970: 6f77 2e73 7461 7475 7320 3d3d 3d20 276f  ow.status === 'o
-00000980: 6666 6c69 6e65 2720 3f20 2764 616e 6765  ffline' ? 'dange
-00000990: 7227 203a 2027 7375 6363 6573 7327 220a  r' : 'success'".
-000009a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009b0: 2020 2020 2020 2020 6469 7361 626c 652d          disable-
-000009c0: 7472 616e 7369 7469 6f6e 733e 7b5b 7363  transitions>{[sc
-000009d0: 6f70 652e 726f 772e 7374 6174 7573 5d7d  ope.row.status]}
-000009e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000009f0: 203c 2f65 6c2d 7461 673e 0a20 2020 2020   </el-tag>.     
-00000a00: 2020 2020 2020 203c 2f74 656d 706c 6174         </templat
-00000a10: 653e 0a20 2020 2020 2020 203c 2f65 6c2d  e>.        </el-
-00000a20: 7461 626c 652d 636f 6c75 6d6e 3e0a 2020  table-column>.  
-00000a30: 2020 2020 2020 3c65 6c2d 7461 626c 652d        <el-table-
-00000a40: 636f 6c75 6d6e 206c 6162 656c 3d22 e693  column label="..
-00000a50: 8de4 bd9c 223e 0a20 2020 2020 2020 2020  ....">.         
-00000a60: 2020 203c 7465 6d70 6c61 7465 2073 6c6f     <template slo
-00000a70: 742d 7363 6f70 653d 2273 636f 7065 223e  t-scope="scope">
-00000a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000a90: 203c 656c 2d62 7574 746f 6e0a 2020 2020   <el-button.    
-00000aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ab0: 2020 2020 7369 7a65 3d22 6d69 6e69 220a      size="mini".
-00000ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ad0: 2020 2020 2020 2020 4063 6c69 636b 3d22          @click="
-00000ae0: 6861 6e64 6c65 4164 6428 7363 6f70 652e  handleAdd(scope.
-00000af0: 726f 7729 223e e696 b0e5 a29e e985 8de7  row)">..........
-00000b00: bdae 0a20 2020 2020 2020 2020 2020 2020  ...             
-00000b10: 2020 203c 2f65 6c2d 6275 7474 6f6e 3e0a     </el-button>.
-00000b20: 2020 2020 2020 2020 2020 2020 3c2f 7465              </te
-00000b30: 6d70 6c61 7465 3e0a 2020 2020 2020 2020  mplate>.        
-00000b40: 3c2f 656c 2d74 6162 6c65 2d63 6f6c 756d  </el-table-colum
-00000b50: 6e3e 0a20 2020 203c 2f65 6c2d 7461 626c  n>.    </el-tabl
-00000b60: 653e 0a0a 2020 2020 3c65 6c2d 6469 616c  e>..    <el-dial
-00000b70: 6f67 2074 6974 6c65 3d22 e696 b0e5 a29e  og title="......
-00000b80: e985 8de7 bdae e590 8ee8 afa5 e5ae a2e6  ................
-00000b90: 88b7 e7ab afe5 b086 e987 8de6 96b0 e8bf  ................
-00000ba0: 9ee6 8ea5 2220 3a76 6973 6962 6c65 2e73  ...." :visible.s
-00000bb0: 796e 633d 2264 6961 6c6f 6746 6f72 6d56  ync="dialogFormV
-00000bc0: 6973 6962 6c65 223e 0a20 2020 2020 2020  isible">.       
-00000bd0: 203c 656c 2d66 6f72 6d20 3a6d 6f64 656c   <el-form :model
-00000be0: 3d22 666f 726d 223e 0a20 2020 2020 2020  ="form">.       
-00000bf0: 2020 2020 203c 656c 2d66 6f72 6d2d 6974       <el-form-it
-00000c00: 656d 206c 6162 656c 3d22 e590 8de7 a7b0  em label="......
-00000c10: 2220 3a6c 6162 656c 2d77 6964 7468 3d22  " :label-width="
-00000c20: 666f 726d 4c61 6265 6c57 6964 7468 223e  formLabelWidth">
-00000c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000c40: 203c 656c 2d69 6e70 7574 2076 2d6d 6f64   <el-input v-mod
-00000c50: 656c 3d22 666f 726d 2e6e 616d 6522 2061  el="form.name" a
-00000c60: 7574 6f63 6f6d 706c 6574 653d 226f 6666  utocomplete="off
-00000c70: 223e 3c2f 656c 2d69 6e70 7574 3e0a 2020  "></el-input>.  
-00000c80: 2020 2020 2020 2020 2020 3c2f 656c 2d66            </el-f
-00000c90: 6f72 6d2d 6974 656d 3e0a 2020 2020 2020  orm-item>.      
-00000ca0: 2020 2020 2020 3c65 6c2d 666f 726d 2d69        <el-form-i
-00000cb0: 7465 6d20 6c61 6265 6c3d 22e8 bf9c e7a8  tem label=".....
-00000cc0: 8be7 abaf e58f a322 203a 6c61 6265 6c2d  ......." :label-
-00000cd0: 7769 6474 683d 2266 6f72 6d4c 6162 656c  width="formLabel
-00000ce0: 5769 6474 6822 3e0a 2020 2020 2020 2020  Width">.        
-00000cf0: 2020 2020 2020 2020 3c65 6c2d 696e 7075          <el-inpu
-00000d00: 7420 762d 6d6f 6465 6c3d 2266 6f72 6d2e  t v-model="form.
-00000d10: 7265 6d6f 7465 5f70 6f72 7422 2074 7970  remote_port" typ
-00000d20: 653d 276e 756d 6265 7227 2061 7574 6f63  e='number' autoc
-00000d30: 6f6d 706c 6574 653d 226f 6666 223e 3c2f  omplete="off"></
-00000d40: 656c 2d69 6e70 7574 3e0a 2020 2020 2020  el-input>.      
-00000d50: 2020 2020 2020 3c2f 656c 2d66 6f72 6d2d        </el-form-
-00000d60: 6974 656d 3e0a 0a20 2020 2020 2020 2020  item>..         
-00000d70: 2020 203c 656c 2d66 6f72 6d2d 6974 656d     <el-form-item
-00000d80: 206c 6162 656c 3d22 e69c ace5 9cb0 6970   label="......ip
-00000d90: 2220 3a6c 6162 656c 2d77 6964 7468 3d22  " :label-width="
-00000da0: 666f 726d 4c61 6265 6c57 6964 7468 223e  formLabelWidth">
-00000db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000dc0: 203c 656c 2d69 6e70 7574 2076 2d6d 6f64   <el-input v-mod
-00000dd0: 656c 3d22 666f 726d 2e6c 6f63 616c 5f69  el="form.local_i
-00000de0: 7022 2061 7574 6f63 6f6d 706c 6574 653d  p" autocomplete=
-00000df0: 226f 6666 223e 3c2f 656c 2d69 6e70 7574  "off"></el-input
-00000e00: 3e0a 2020 2020 2020 2020 2020 2020 3c2f  >.            </
-00000e10: 656c 2d66 6f72 6d2d 6974 656d 3e0a 2020  el-form-item>.  
-00000e20: 2020 2020 2020 2020 2020 3c65 6c2d 666f            <el-fo
-00000e30: 726d 2d69 7465 6d20 6c61 6265 6c3d 22e6  rm-item label=".
-00000e40: 9cac e59c b0e7 abaf e58f a322 203a 6c61  ..........." :la
-00000e50: 6265 6c2d 7769 6474 683d 2266 6f72 6d4c  bel-width="formL
-00000e60: 6162 656c 5769 6474 6822 3e0a 2020 2020  abelWidth">.    
-00000e70: 2020 2020 2020 2020 2020 2020 3c65 6c2d              <el-
-00000e80: 696e 7075 7420 762d 6d6f 6465 6c3d 2266  input v-model="f
-00000e90: 6f72 6d2e 6c6f 6361 6c5f 706f 7274 2220  orm.local_port" 
-00000ea0: 7479 7065 3d27 6e75 6d62 6572 2720 6175  type='number' au
-00000eb0: 746f 636f 6d70 6c65 7465 3d22 6f66 6622  tocomplete="off"
-00000ec0: 3e3c 2f65 6c2d 696e 7075 743e 0a20 2020  ></el-input>.   
-00000ed0: 2020 2020 2020 2020 203c 2f65 6c2d 666f           </el-fo
-00000ee0: 726d 2d69 7465 6d3e 0a20 2020 2020 2020  rm-item>.       
-00000ef0: 203c 2f65 6c2d 666f 726d 3e0a 2020 2020   </el-form>.    
-00000f00: 2020 2020 3c64 6976 2073 6c6f 743d 2266      <div slot="f
-00000f10: 6f6f 7465 7222 2063 6c61 7373 3d22 6469  ooter" class="di
-00000f20: 616c 6f67 2d66 6f6f 7465 7222 3e0a 2020  alog-footer">.  
-00000f30: 2020 2020 2020 2020 2020 3c65 6c2d 6275            <el-bu
-00000f40: 7474 6f6e 2040 636c 6963 6b3d 2264 6961  tton @click="dia
-00000f50: 6c6f 6746 6f72 6d56 6973 6962 6c65 203d  logFormVisible =
-00000f60: 2066 616c 7365 223e e58f 9620 e6b6 883c   false">... ...<
-00000f70: 2f65 6c2d 6275 7474 6f6e 3e0a 2020 2020  /el-button>.    
-00000f80: 2020 2020 2020 2020 3c65 6c2d 6275 7474          <el-butt
-00000f90: 6f6e 2074 7970 653d 2270 7269 6d61 7279  on type="primary
-00000fa0: 2220 4063 6c69 636b 3d22 7375 626d 6974  " @click="submit
-00000fb0: 4164 6422 3ee7 a1ae 20e5 ae9a 3c2f 656c  Add">... ...</el
-00000fc0: 2d62 7574 746f 6e3e 0a20 2020 2020 2020  -button>.       
-00000fd0: 203c 2f64 6976 3e0a 2020 2020 3c2f 656c   </div>.    </el
-00000fe0: 2d64 6961 6c6f 673e 0a3c 2f64 6976 3e0a  -dialog>.</div>.
-00000ff0: 3c73 6372 6970 743e 0a20 2020 206e 6577  <script>.    new
-00001000: 2056 7565 287b 0a20 2020 2020 2020 2065   Vue({.        e
-00001010: 6c3a 2027 2361 7070 272c 0a20 2020 2020  l: '#app',.     
-00001020: 2020 2064 656c 696d 6974 6572 733a 205b     delimiters: [
-00001030: 277b 5b27 2c20 275d 7d27 5d2c 202f 2f20  '{[', ']}'], // 
-00001040: e8bf 99e5 8fa5 e58f afe4 bba5 e68c 87e5  ................
-00001050: ae9a 207b 5b20 5d7d 20e4 b8ba e68f 92e5  .. {[ ]} .......
-00001060: 80bc e8a1 a8e8 bebe e5bc 8fe7 9a84 e696  ................
-00001070: b0e7 aca6 e58f b70a 2020 2020 2020 2020  ........        
-00001080: 6461 7461 2829 207b 0a20 2020 2020 2020  data() {.       
-00001090: 2020 2020 2072 6574 7572 6e20 7b0a 2020       return {.  
-000010a0: 2020 2020 2020 2020 2020 2020 2020 7461                ta
-000010b0: 626c 6544 6174 613a 205b 7b63 6c69 656e  bleData: [{clien
-000010c0: 745f 6e61 6d65 3a20 2773 7368 277d 5d2c  t_name: 'ssh'}],
-000010d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000010e0: 2064 6961 6c6f 6746 6f72 6d56 6973 6962   dialogFormVisib
-000010f0: 6c65 3a20 6661 6c73 652c 0a20 2020 2020  le: false,.     
-00001100: 2020 2020 2020 2020 2020 2066 6f72 6d4c             formL
-00001110: 6162 656c 5769 6474 683a 2027 3132 3070  abelWidth: '120p
-00001120: 7827 2c0a 2020 2020 2020 2020 2020 2020  x',.            
-00001130: 2020 2020 666f 726d 3a20 7b0a 2020 2020      form: {.    
-00001140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001150: 636c 6965 6e74 5f6e 616d 653a 2027 272c  client_name: '',
-00001160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001170: 2020 2020 206e 616d 653a 2027 272c 0a20       name: '',. 
-00001180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001190: 2020 206c 6f63 616c 5f70 6f72 743a 2027     local_port: '
-000011a0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-000011b0: 2020 2020 2020 206c 6f63 616c 5f69 703a         local_ip:
-000011c0: 2027 3132 372e 302e 302e 3127 2c0a 2020   '127.0.0.1',.  
-000011d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011e0: 2020 7265 6d6f 7465 5f70 6f72 743a 2027    remote_port: '
-000011f0: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-00001200: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-00001210: 2020 2020 2069 6e74 6572 7661 6c54 6173       intervalTas
-00001220: 6b3a 2027 270a 0a20 2020 2020 2020 2020  k: ''..         
-00001230: 2020 207d 0a20 2020 2020 2020 207d 2c0a     }.        },.
-00001240: 2020 2020 2020 2020 6d6f 756e 7465 6428          mounted(
-00001250: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
-00001260: 7468 6973 2e67 6574 436c 6965 6e74 4c69  this.getClientLi
-00001270: 7374 2829 0a20 2020 2020 2020 2020 2020  st().           
-00001280: 2074 6869 732e 696e 7465 7276 616c 5461   this.intervalTa
-00001290: 736b 203d 2073 6574 496e 7465 7276 616c  sk = setInterval
-000012a0: 2874 6869 732e 6765 7443 6c69 656e 744c  (this.getClientL
-000012b0: 6973 742c 2033 3030 3029 0a20 2020 2020  ist, 3000).     
-000012c0: 2020 207d 2c0a 2020 2020 2020 2020 6265     },.        be
-000012d0: 666f 7265 4465 7374 726f 7928 2920 7b0a  foreDestroy() {.
-000012e0: 2020 2020 2020 2020 2020 2020 7468 6973              this
-000012f0: 2e69 6e74 6572 7661 6c54 6173 6b2e 7374  .intervalTask.st
-00001300: 6f70 2829 0a20 2020 2020 2020 207d 2c0a  op().        },.
-00001310: 2020 2020 2020 2020 6d65 7468 6f64 733a          methods:
-00001320: 207b 0a20 2020 2020 2020 2020 2020 2068   {.            h
-00001330: 616e 646c 6541 6464 2872 6f77 2920 7b0a  andleAdd(row) {.
-00001340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001350: 7468 6973 2e66 6f72 6d20 3d20 7b0a 2020  this.form = {.  
-00001360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001370: 2020 636c 6965 6e74 5f6e 616d 653a 2027    client_name: '
-00001380: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00001390: 2020 2020 2020 206e 616d 653a 2027 272c         name: '',
-000013a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000013b0: 2020 2020 206c 6f63 616c 5f70 6f72 743a       local_port:
-000013c0: 2027 272c 0a20 2020 2020 2020 2020 2020   '',.           
-000013d0: 2020 2020 2020 2020 206c 6f63 616c 5f69           local_i
-000013e0: 703a 2027 3132 372e 302e 302e 3127 2c0a  p: '127.0.0.1',.
-000013f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001400: 2020 2020 7265 6d6f 7465 5f70 6f72 743a      remote_port:
-00001410: 2027 270a 2020 2020 2020 2020 2020 2020   ''.            
-00001420: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
-00001430: 2020 2020 2020 7468 6973 2e66 6f72 6d2e        this.form.
-00001440: 636c 6965 6e74 5f6e 616d 6520 3d20 726f  client_name = ro
-00001450: 772e 636c 6965 6e74 5f6e 616d 650a 2020  w.client_name.  
-00001460: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00001470: 6e73 6f6c 652e 6c6f 6728 726f 7729 3b0a  nsole.log(row);.
-00001480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001490: 7468 6973 2e64 6961 6c6f 6746 6f72 6d56  this.dialogFormV
-000014a0: 6973 6962 6c65 203d 2074 7275 650a 2020  isible = true.  
-000014b0: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-000014c0: 2020 2020 2020 2020 2073 7562 6d69 7441           submitA
-000014d0: 6464 2829 207b 0a20 2020 2020 2020 2020  dd() {.         
-000014e0: 2020 2020 2020 202f 2f20 636f 6e73 7420         // const 
-000014f0: 7572 6c20 3d20 7769 6e64 6f77 2e6c 6f63  url = window.loc
-00001500: 6174 696f 6e2e 6872 6566 202b 2027 2f61  ation.href + '/a
-00001510: 7069 270a 2020 2020 2020 2020 2020 2020  pi'.            
-00001520: 2020 2020 7661 7220 7572 6c20 3d20 7769      var url = wi
-00001530: 6e64 6f77 2e6c 6f63 6174 696f 6e2e 6872  ndow.location.hr
-00001540: 6566 2e73 706c 6974 2827 3f27 295b 305d  ef.split('?')[0]
-00001550: 202b 2027 2f61 7069 270a 0a20 2020 2020   + '/api'..     
-00001560: 2020 2020 2020 2020 2020 2063 6f6e 736f             conso
-00001570: 6c65 2e6c 6f67 2874 6869 732e 666f 726d  le.log(this.form
-00001580: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00001590: 2020 6178 696f 732e 706f 7374 2875 726c    axios.post(url
-000015a0: 2c20 7468 6973 2e66 6f72 6d29 2e74 6865  , this.form).the
-000015b0: 6e28 7265 7320 3d3e 207b 0a20 2020 2020  n(res => {.     
-000015c0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000015d0: 6620 2872 6573 2e64 6174 612e 636f 6465  f (res.data.code
-000015e0: 2021 3d3d 2032 3030 2920 7b0a 2020 2020   !== 200) {.    
-000015f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001600: 2020 2020 7265 7475 726e 2061 6c65 7274      return alert
-00001610: 2872 6573 2e64 6174 612e 6d73 6729 0a20  (res.data.msg). 
-00001620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001630: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
-00001640: 2020 2020 2020 2020 2074 6869 732e 6469           this.di
-00001650: 616c 6f67 466f 726d 5669 7369 626c 6520  alogFormVisible 
-00001660: 3d20 6661 6c73 650a 2020 2020 2020 2020  = false.        
-00001670: 2020 2020 2020 2020 7d29 2e63 6174 6368          }).catch
-00001680: 2865 7272 203d 3e20 7b0a 2020 2020 2020  (err => {.      
-00001690: 2020 2020 2020 2020 2020 2020 2020 636f                co
-000016a0: 6e73 6f6c 652e 6c6f 6728 6572 7229 0a20  nsole.log(err). 
-000016b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016c0: 2020 2074 6869 732e 246d 6573 7361 6765     this.$message
-000016d0: 2e65 7272 6f72 2827 e994 99e4 ba86 e593  .error('........
-000016e0: a6ef bc8c e8bf 99e6 98af e4b8 80e6 9da1  ................
-000016f0: e994 99e8 afaf e6b6 88e6 81af 2729 0a20  ............'). 
-00001700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001710: 2020 2061 6c65 7274 2827 e69c 8de5 8aa1     alert('......
-00001720: e599 a8e5 87ba e78e b0e9 9499 e8af af27  ...............'
-00001730: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00001740: 2020 7d29 0a20 2020 2020 2020 2020 2020    }).           
-00001750: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-00001760: 6861 6e64 6c65 4465 6c65 7465 2863 6c69  handleDelete(cli
-00001770: 656e 745f 6e61 6d65 2c20 6e61 6d65 2920  ent_name, name) 
-00001780: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00001790: 2020 7661 7220 7572 6c20 3d20 7769 6e64    var url = wind
-000017a0: 6f77 2e6c 6f63 6174 696f 6e2e 6872 6566  ow.location.href
-000017b0: 2e73 706c 6974 2827 3f27 295b 305d 202b  .split('?')[0] +
-000017c0: 2027 2f61 7069 270a 2020 2020 2020 2020   '/api'.        
-000017d0: 2020 2020 2020 2020 636f 6e73 7420 7061          const pa
-000017e0: 7261 6d73 203d 207b 0a20 2020 2020 2020  rams = {.       
-000017f0: 2020 2020 2020 2020 2020 2020 2063 6c69               cli
-00001800: 656e 745f 6e61 6d65 3a20 636c 6965 6e74  ent_name: client
-00001810: 5f6e 616d 652c 0a20 2020 2020 2020 2020  _name,.         
-00001820: 2020 2020 2020 2020 2020 206e 616d 653a             name:
-00001830: 206e 616d 650a 2020 2020 2020 2020 2020   name.          
-00001840: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00001850: 2020 2020 2020 2020 7468 6973 2e24 636f          this.$co
-00001860: 6e66 6972 6d28 27e5 88a0 e999 a4e5 908e  nfirm('.........
-00001870: e8af a5e5 aea2 e688 b7e7 abaf e5b0 86e9  ................
-00001880: 878d e696 b0e8 bf9e e68e a52c 20e6 98af  ..........., ...
-00001890: e590 a6e7 bba7 e7bb ad3f 272c 2027 e68f  .........?', '..
-000018a0: 90e7 a4ba 272c 207b 0a20 2020 2020 2020  ....', {.       
-000018b0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-000018c0: 6669 726d 4275 7474 6f6e 5465 7874 3a20  firmButtonText: 
-000018d0: 27e7 a1ae e5ae 9a27 2c0a 2020 2020 2020  '......',.      
-000018e0: 2020 2020 2020 2020 2020 2020 2020 6361                ca
-000018f0: 6e63 656c 4275 7474 6f6e 5465 7874 3a20  ncelButtonText: 
-00001900: 27e5 8f96 e6b6 8827 2c0a 2020 2020 2020  '......',.      
-00001910: 2020 2020 2020 2020 2020 2020 2020 7479                ty
-00001920: 7065 3a20 2777 6172 6e69 6e67 270a 2020  pe: 'warning'.  
-00001930: 2020 2020 2020 2020 2020 2020 2020 7d29                })
-00001940: 2e74 6865 6e28 2829 203d 3e20 7b0a 2020  .then(() => {.  
-00001950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001960: 2020 6178 696f 732e 6465 6c65 7465 2875    axios.delete(u
-00001970: 726c 2c20 7b0a 2020 2020 2020 2020 2020  rl, {.          
-00001980: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-00001990: 7261 6d73 3a20 7061 7261 6d73 0a20 2020  rams: params.   
-000019a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019b0: 207d 292e 7468 656e 2872 6573 203d 3e20   }).then(res => 
-000019c0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-000019d0: 2020 2020 2020 2020 2020 6966 2028 7265            if (re
-000019e0: 732e 6461 7461 2e63 6f64 6520 213d 3d20  s.data.code !== 
-000019f0: 3230 3029 207b 0a20 2020 2020 2020 2020  200) {.         
+000006e0: 2020 2020 2020 2020 2020 7369 7a65 3d22            size="
+000006f0: 6d69 6e69 220a 2020 2020 2020 2020 2020  mini".          
+00000700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000720: 2040 636c 6963 6b3d 2268 616e 646c 6544   @click="handleD
+00000730: 656c 6574 6528 7072 6f70 732e 726f 772e  elete(props.row.
+00000740: 636c 6965 6e74 5f6e 616d 652c 2073 636f  client_name, sco
+00000750: 7065 2e72 6f77 2e6e 616d 6529 223e e588  pe.row.name)">..
+00000760: a0e9 99a4 0a20 2020 2020 2020 2020 2020  .....           
+00000770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000780: 2020 2020 203c 2f65 6c2d 6275 7474 6f6e       </el-button
+00000790: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000007a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007b0: 2020 3c65 6c2d 6275 7474 6f6e 203a 6469    <el-button :di
+000007c0: 7361 626c 6564 3d22 7072 6f70 732e 726f  sabled="props.ro
+000007d0: 772e 6361 6e5f 6465 6c65 7465 5f6e 616d  w.can_delete_nam
+000007e0: 6573 2e69 6e64 6578 4f66 2873 636f 7065  es.indexOf(scope
+000007f0: 2e72 6f77 2e6e 616d 6529 203d 3d3d 202d  .row.name) === -
+00000800: 3120 220a 2020 2020 2020 2020 2020 2020  1 ".            
+00000810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000820: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00000830: 697a 653d 226d 696e 6922 0a20 2020 2020  ize="mini".     
+00000840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000860: 2020 2020 2020 4063 6c69 636b 3d22 6861        @click="ha
+00000870: 6e64 6c65 4564 6974 2873 636f 7065 2e72  ndleEdit(scope.r
+00000880: 6f77 2c20 7072 6f70 732e 726f 772e 636c  ow, props.row.cl
+00000890: 6965 6e74 5f6e 616d 6529 223e e7bc 96e8  ient_name)">....
+000008a0: be91 0a20 2020 2020 2020 2020 2020 2020  ...             
+000008b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008c0: 2020 203c 2f65 6c2d 6275 7474 6f6e 3e0a     </el-button>.
+000008d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008e0: 2020 2020 2020 2020 2020 2020 3c2f 656c              </el
+000008f0: 2d72 6f77 3e0a 0a0a 2020 2020 2020 2020  -row>...        
+00000900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000910: 3c2f 7465 6d70 6c61 7465 3e0a 2020 2020  </template>.    
+00000920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000930: 3c2f 656c 2d74 6162 6c65 2d63 6f6c 756d  </el-table-colum
+00000940: 6e3e 0a20 2020 2020 2020 2020 2020 2020  n>.             
+00000950: 2020 203c 2f65 6c2d 7461 626c 653e 0a20     </el-table>. 
+00000960: 2020 2020 2020 2020 2020 203c 2f74 656d             </tem
+00000970: 706c 6174 653e 0a20 2020 2020 2020 203c  plate>.        <
+00000980: 2f65 6c2d 7461 626c 652d 636f 6c75 6d6e  /el-table-column
+00000990: 3e0a 2020 2020 2020 2020 3c65 6c2d 7461  >.        <el-ta
+000009a0: 626c 652d 636f 6c75 6d6e 0a20 2020 2020  ble-column.     
+000009b0: 2020 2020 2020 2020 2020 2070 726f 703d             prop=
+000009c0: 2263 6c69 656e 745f 6e61 6d65 220a 2020  "client_name".  
+000009d0: 2020 2020 2020 2020 2020 2020 2020 6c61                la
+000009e0: 6265 6c3d 22e5 908d e7a7 b022 0a20 2020  bel="......".   
+000009f0: 2020 2020 203e 0a20 2020 2020 2020 203c       >.        <
+00000a00: 2f65 6c2d 7461 626c 652d 636f 6c75 6d6e  /el-table-column
+00000a10: 3e0a 2020 2020 2020 2020 3c65 6c2d 7461  >.        <el-ta
+00000a20: 626c 652d 636f 6c75 6d6e 0a20 2020 2020  ble-column.     
+00000a30: 2020 2020 2020 2020 2020 2070 726f 703d             prop=
+00000a40: 2276 6572 7369 6f6e 220a 2020 2020 2020  "version".      
+00000a50: 2020 2020 2020 2020 2020 6c61 6265 6c3d            label=
+00000a60: 22e7 8988 e69c ac22 0a20 2020 2020 2020  "......".       
+00000a70: 203e 0a20 2020 2020 2020 203c 2f65 6c2d   >.        </el-
+00000a80: 7461 626c 652d 636f 6c75 6d6e 3e0a 2020  table-column>.  
+00000a90: 2020 2020 2020 3c65 6c2d 7461 626c 652d        <el-table-
+00000aa0: 636f 6c75 6d6e 0a20 2020 2020 2020 2020  column.         
+00000ab0: 2020 2020 2020 2070 726f 703d 2273 7461         prop="sta
+00000ac0: 7475 7322 0a20 2020 2020 2020 2020 2020  tus".           
+00000ad0: 2020 2020 206c 6162 656c 3d22 e78a b6e6       label="....
+00000ae0: 8081 220a 2020 2020 2020 2020 2020 2020  ..".            
+00000af0: 2020 2020 3a66 696c 7465 7273 3d22 5b7b      :filters="[{
+00000b00: 2074 6578 743a 2027 6f6e 6c69 6e65 272c   text: 'online',
+00000b10: 2076 616c 7565 3a20 276f 6e6c 696e 6527   value: 'online'
+00000b20: 207d 2c20 7b20 7465 7874 3a20 276f 6666   }, { text: 'off
+00000b30: 6c69 6e65 272c 2076 616c 7565 3a20 276f  line', value: 'o
+00000b40: 6666 6c69 6e65 2720 7d5d 220a 2020 2020  ffline' }]".    
+00000b50: 2020 2020 2020 2020 2020 2020 6669 6c74              filt
+00000b60: 6572 2d70 6c61 6365 6d65 6e74 3d22 626f  er-placement="bo
+00000b70: 7474 6f6d 2d65 6e64 223e 0a20 2020 2020  ttom-end">.     
+00000b80: 2020 2020 2020 203c 7465 6d70 6c61 7465         <template
+00000b90: 2073 6c6f 742d 7363 6f70 653d 2273 636f   slot-scope="sco
+00000ba0: 7065 223e 0a20 2020 2020 2020 2020 2020  pe">.           
+00000bb0: 2020 2020 203c 656c 2d74 6167 0a20 2020       <el-tag.   
+00000bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000bd0: 2020 2020 203a 7479 7065 3d22 7363 6f70       :type="scop
+00000be0: 652e 726f 772e 7374 6174 7573 203d 3d3d  e.row.status ===
+00000bf0: 2027 6f66 666c 696e 6527 203f 2027 6461   'offline' ? 'da
+00000c00: 6e67 6572 2720 3a20 2773 7563 6365 7373  nger' : 'success
+00000c10: 2722 0a20 2020 2020 2020 2020 2020 2020  '".             
+00000c20: 2020 2020 2020 2020 2020 2064 6973 6162             disab
+00000c30: 6c65 2d74 7261 6e73 6974 696f 6e73 3e7b  le-transitions>{
+00000c40: 5b73 636f 7065 2e72 6f77 2e73 7461 7475  [scope.row.statu
+00000c50: 735d 7d0a 2020 2020 2020 2020 2020 2020  s]}.            
+00000c60: 2020 2020 3c2f 656c 2d74 6167 3e0a 2020      </el-tag>.  
+00000c70: 2020 2020 2020 2020 2020 3c2f 7465 6d70            </temp
+00000c80: 6c61 7465 3e0a 2020 2020 2020 2020 3c2f  late>.        </
+00000c90: 656c 2d74 6162 6c65 2d63 6f6c 756d 6e3e  el-table-column>
+00000ca0: 0a20 2020 2020 2020 203c 656c 2d74 6162  .        <el-tab
+00000cb0: 6c65 2d63 6f6c 756d 6e20 6c61 6265 6c3d  le-column label=
+00000cc0: 22e6 938d e4bd 9c22 3e0a 2020 2020 2020  "......">.      
+00000cd0: 2020 2020 2020 3c74 656d 706c 6174 6520        <template 
+00000ce0: 736c 6f74 2d73 636f 7065 3d22 7363 6f70  slot-scope="scop
+00000cf0: 6522 3e0a 2020 2020 2020 2020 2020 2020  e">.            
+00000d00: 2020 2020 3c65 6c2d 6275 7474 6f6e 0a20      <el-button. 
+00000d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d20: 2020 2020 2020 2073 697a 653d 226d 696e         size="min
+00000d30: 6922 0a20 2020 2020 2020 2020 2020 2020  i".             
+00000d40: 2020 2020 2020 2020 2020 2040 636c 6963             @clic
+00000d50: 6b3d 2268 616e 646c 6541 6464 2873 636f  k="handleAdd(sco
+00000d60: 7065 2e72 6f77 2922 3ee6 96b0 e5a2 9ee9  pe.row)">.......
+00000d70: 858d e7bd ae0a 2020 2020 2020 2020 2020  ......          
+00000d80: 2020 2020 2020 3c2f 656c 2d62 7574 746f        </el-butto
+00000d90: 6e3e 0a20 2020 2020 2020 2020 2020 203c  n>.            <
+00000da0: 2f74 656d 706c 6174 653e 0a20 2020 2020  /template>.     
+00000db0: 2020 203c 2f65 6c2d 7461 626c 652d 636f     </el-table-co
+00000dc0: 6c75 6d6e 3e0a 2020 2020 3c2f 656c 2d74  lumn>.    </el-t
+00000dd0: 6162 6c65 3e0a 0a20 2020 203c 656c 2d64  able>..    <el-d
+00000de0: 6961 6c6f 6720 7469 746c 653d 22e7 a1ae  ialog title="...
+00000df0: e5ae 9ae5 908e e5ae a2e6 88b7 e7ab afe5  ................
+00000e00: b086 e987 8de6 96b0 e8bf 9ee6 8ea5 2220  .............." 
+00000e10: 3a76 6973 6962 6c65 2e73 796e 633d 2264  :visible.sync="d
+00000e20: 6961 6c6f 6746 6f72 6d56 6973 6962 6c65  ialogFormVisible
+00000e30: 223e 0a20 2020 2020 2020 203c 656c 2d66  ">.        <el-f
+00000e40: 6f72 6d20 3a6d 6f64 656c 3d22 666f 726d  orm :model="form
+00000e50: 223e 0a20 2020 2020 2020 2020 2020 203c  ">.            <
+00000e60: 656c 2d66 6f72 6d2d 6974 656d 206c 6162  el-form-item lab
+00000e70: 656c 3d22 e590 8de7 a7b0 2220 3a6c 6162  el="......" :lab
+00000e80: 656c 2d77 6964 7468 3d22 666f 726d 4c61  el-width="formLa
+00000e90: 6265 6c57 6964 7468 2220 3e0a 2020 2020  belWidth" >.    
+00000ea0: 2020 2020 2020 2020 2020 2020 3c65 6c2d              <el-
+00000eb0: 696e 7075 7420 762d 6d6f 6465 6c3d 2266  input v-model="f
+00000ec0: 6f72 6d2e 6e61 6d65 2220 6175 746f 636f  orm.name" autoco
+00000ed0: 6d70 6c65 7465 3d22 6f66 6622 203a 6469  mplete="off" :di
+00000ee0: 7361 626c 6564 3d22 666f 726d 2e69 735f  sabled="form.is_
+00000ef0: 6564 6974 223e 3c2f 656c 2d69 6e70 7574  edit"></el-input
+00000f00: 3e0a 2020 2020 2020 2020 2020 2020 3c2f  >.            </
+00000f10: 656c 2d66 6f72 6d2d 6974 656d 3e0a 2020  el-form-item>.  
+00000f20: 2020 2020 2020 2020 2020 3c65 6c2d 666f            <el-fo
+00000f30: 726d 2d69 7465 6d20 6c61 6265 6c3d 22e8  rm-item label=".
+00000f40: bf9c e7a8 8be7 abaf e58f a322 203a 6c61  ..........." :la
+00000f50: 6265 6c2d 7769 6474 683d 2266 6f72 6d4c  bel-width="formL
+00000f60: 6162 656c 5769 6474 6822 3e0a 2020 2020  abelWidth">.    
+00000f70: 2020 2020 2020 2020 2020 2020 3c65 6c2d              <el-
+00000f80: 696e 7075 7420 762d 6d6f 6465 6c3d 2266  input v-model="f
+00000f90: 6f72 6d2e 7265 6d6f 7465 5f70 6f72 7422  orm.remote_port"
+00000fa0: 2074 7970 653d 276e 756d 6265 7227 2061   type='number' a
+00000fb0: 7574 6f63 6f6d 706c 6574 653d 226f 6666  utocomplete="off
+00000fc0: 223e 3c2f 656c 2d69 6e70 7574 3e0a 2020  "></el-input>.  
+00000fd0: 2020 2020 2020 2020 2020 3c2f 656c 2d66            </el-f
+00000fe0: 6f72 6d2d 6974 656d 3e0a 0a20 2020 2020  orm-item>..     
+00000ff0: 2020 2020 2020 203c 656c 2d66 6f72 6d2d         <el-form-
+00001000: 6974 656d 206c 6162 656c 3d22 e69c ace5  item label="....
+00001010: 9cb0 6970 2220 3a6c 6162 656c 2d77 6964  ..ip" :label-wid
+00001020: 7468 3d22 666f 726d 4c61 6265 6c57 6964  th="formLabelWid
+00001030: 7468 223e 0a20 2020 2020 2020 2020 2020  th">.           
+00001040: 2020 2020 203c 656c 2d69 6e70 7574 2076       <el-input v
+00001050: 2d6d 6f64 656c 3d22 666f 726d 2e6c 6f63  -model="form.loc
+00001060: 616c 5f69 7022 2061 7574 6f63 6f6d 706c  al_ip" autocompl
+00001070: 6574 653d 226f 6666 223e 3c2f 656c 2d69  ete="off"></el-i
+00001080: 6e70 7574 3e0a 2020 2020 2020 2020 2020  nput>.          
+00001090: 2020 3c2f 656c 2d66 6f72 6d2d 6974 656d    </el-form-item
+000010a0: 3e0a 2020 2020 2020 2020 2020 2020 3c65  >.            <e
+000010b0: 6c2d 666f 726d 2d69 7465 6d20 6c61 6265  l-form-item labe
+000010c0: 6c3d 22e6 9cac e59c b0e7 abaf e58f a322  l="............"
+000010d0: 203a 6c61 6265 6c2d 7769 6474 683d 2266   :label-width="f
+000010e0: 6f72 6d4c 6162 656c 5769 6474 6822 3e0a  ormLabelWidth">.
+000010f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001100: 3c65 6c2d 696e 7075 7420 762d 6d6f 6465  <el-input v-mode
+00001110: 6c3d 2266 6f72 6d2e 6c6f 6361 6c5f 706f  l="form.local_po
+00001120: 7274 2220 7479 7065 3d27 6e75 6d62 6572  rt" type='number
+00001130: 2720 6175 746f 636f 6d70 6c65 7465 3d22  ' autocomplete="
+00001140: 6f66 6622 3e3c 2f65 6c2d 696e 7075 743e  off"></el-input>
+00001150: 0a20 2020 2020 2020 2020 2020 203c 2f65  .            </e
+00001160: 6c2d 666f 726d 2d69 7465 6d3e 0a0a 2020  l-form-item>..  
+00001170: 2020 2020 2020 2020 2020 3c65 6c2d 666f            <el-fo
+00001180: 726d 2d69 7465 6d20 6c61 6265 6c3d 22e9  rm-item label=".
+00001190: 9990 e980 9f28 4d42 2922 203a 6c61 6265  .....(MB)" :labe
+000011a0: 6c2d 7769 6474 683d 2266 6f72 6d4c 6162  l-width="formLab
+000011b0: 656c 5769 6474 6822 3e0a 2020 2020 2020  elWidth">.      
+000011c0: 2020 2020 2020 2020 2020 3c65 6c2d 746f            <el-to
+000011d0: 6f6c 7469 7020 636c 6173 733d 2269 7465  oltip class="ite
+000011e0: 6d22 2065 6666 6563 743d 2264 6172 6b22  m" effect="dark"
+000011f0: 2063 6f6e 7465 6e74 3d22 e999 90e9 809f   content="......
+00001200: 2c20 30e8 a1a8 e7a4 bae4 b88d e999 90e5  , 0.............
+00001210: 88b6 2220 706c 6163 656d 656e 743d 2262  .." placement="b
+00001220: 6f74 746f 6d22 3e0a 2020 2020 2020 2020  ottom">.        
+00001230: 2020 2020 2020 2020 2020 2020 3c65 6c2d              <el-
+00001240: 696e 7075 7420 762d 6d6f 6465 6c3d 2266  input v-model="f
+00001250: 6f72 6d2e 7370 6565 645f 6c69 6d69 7422  orm.speed_limit"
+00001260: 2074 7970 653d 276e 756d 6265 7227 2061   type='number' a
+00001270: 7574 6f63 6f6d 706c 6574 653d 226f 6666  utocomplete="off
+00001280: 223e 3c2f 656c 2d69 6e70 7574 3e0a 2020  "></el-input>.  
+00001290: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+000012a0: 656c 2d74 6f6f 6c74 6970 3e0a 2020 2020  el-tooltip>.    
+000012b0: 2020 2020 2020 2020 3c2f 656c 2d66 6f72          </el-for
+000012c0: 6d2d 6974 656d 3e0a 2020 2020 2020 2020  m-item>.        
+000012d0: 3c2f 656c 2d66 6f72 6d3e 0a20 2020 2020  </el-form>.     
+000012e0: 2020 203c 6469 7620 736c 6f74 3d22 666f     <div slot="fo
+000012f0: 6f74 6572 2220 636c 6173 733d 2264 6961  oter" class="dia
+00001300: 6c6f 672d 666f 6f74 6572 223e 0a20 2020  log-footer">.   
+00001310: 2020 2020 2020 2020 203c 656c 2d62 7574           <el-but
+00001320: 746f 6e20 4063 6c69 636b 3d22 6469 616c  ton @click="dial
+00001330: 6f67 466f 726d 5669 7369 626c 6520 3d20  ogFormVisible = 
+00001340: 6661 6c73 6522 3ee5 8f96 20e6 b688 3c2f  false">... ...</
+00001350: 656c 2d62 7574 746f 6e3e 0a20 2020 2020  el-button>.     
+00001360: 2020 2020 2020 203c 656c 2d62 7574 746f         <el-butto
+00001370: 6e20 7479 7065 3d22 7072 696d 6172 7922  n type="primary"
+00001380: 2040 636c 6963 6b3d 2273 7562 6d69 7441   @click="submitA
+00001390: 6464 4f72 4564 6974 223e e7a1 ae20 e5ae  ddOrEdit">... ..
+000013a0: 9a3c 2f65 6c2d 6275 7474 6f6e 3e0a 2020  .</el-button>.  
+000013b0: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
+000013c0: 203c 2f65 6c2d 6469 616c 6f67 3e0a 3c2f   </el-dialog>.</
+000013d0: 6469 763e 0a3c 7363 7269 7074 3e0a 2020  div>.<script>.  
+000013e0: 2020 6e65 7720 5675 6528 7b0a 2020 2020    new Vue({.    
+000013f0: 2020 2020 656c 3a20 2723 6170 7027 2c0a      el: '#app',.
+00001400: 2020 2020 2020 2020 6465 6c69 6d69 7465          delimite
+00001410: 7273 3a20 5b27 7b5b 272c 2027 5d7d 275d  rs: ['{[', ']}']
+00001420: 2c20 2f2f 20e8 bf99 e58f a5e5 8faf e4bb  , // ...........
+00001430: a5e6 8c87 e5ae 9a20 7b5b 205d 7d20 e4b8  ....... {[ ]} ..
+00001440: bae6 8f92 e580 bce8 a1a8 e8be bee5 bc8f  ................
+00001450: e79a 84e6 96b0 e7ac a6e5 8fb7 0a20 2020  .............   
+00001460: 2020 2020 2064 6174 6128 2920 7b0a 2020       data() {.  
+00001470: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00001480: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00001490: 2020 2074 6162 6c65 4461 7461 3a20 5b7b     tableData: [{
+000014a0: 636c 6965 6e74 5f6e 616d 653a 2027 7373  client_name: 'ss
+000014b0: 6827 7d5d 2c0a 2020 2020 2020 2020 2020  h'}],.          
+000014c0: 2020 2020 2020 6469 616c 6f67 466f 726d        dialogForm
+000014d0: 5669 7369 626c 653a 2066 616c 7365 2c0a  Visible: false,.
+000014e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014f0: 666f 726d 4c61 6265 6c57 6964 7468 3a20  formLabelWidth: 
+00001500: 2731 3230 7078 272c 0a20 2020 2020 2020  '120px',.       
+00001510: 2020 2020 2020 2020 2066 6f72 6d3a 207b           form: {
+00001520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001530: 2020 2020 2063 6c69 656e 745f 6e61 6d65       client_name
+00001540: 3a20 2727 2c0a 2020 2020 2020 2020 2020  : '',.          
+00001550: 2020 2020 2020 2020 2020 6e61 6d65 3a20            name: 
+00001560: 2727 2c0a 2020 2020 2020 2020 2020 2020  '',.            
+00001570: 2020 2020 2020 2020 6c6f 6361 6c5f 706f          local_po
+00001580: 7274 3a20 2727 2c0a 2020 2020 2020 2020  rt: '',.        
+00001590: 2020 2020 2020 2020 2020 2020 6c6f 6361              loca
+000015a0: 6c5f 6970 3a20 2731 3237 2e30 2e30 2e31  l_ip: '127.0.0.1
+000015b0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+000015c0: 2020 2020 2020 2072 656d 6f74 655f 706f         remote_po
+000015d0: 7274 3a20 2727 2c0a 2020 2020 2020 2020  rt: '',.        
+000015e0: 2020 2020 2020 2020 2020 2020 7370 6565              spee
+000015f0: 645f 6c69 6d69 743a 2030 0a20 2020 2020  d_limit: 0.     
+00001600: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+00001610: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00001620: 7465 7276 616c 5461 736b 3a20 2727 0a0a  tervalTask: ''..
+00001630: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00001640: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00001650: 206d 6f75 6e74 6564 2829 207b 0a20 2020   mounted() {.   
+00001660: 2020 2020 2020 2020 2074 6869 732e 6765           this.ge
+00001670: 7443 6c69 656e 744c 6973 7428 290a 2020  tClientList().  
+00001680: 2020 2020 2020 2020 2020 7468 6973 2e69            this.i
+00001690: 6e74 6572 7661 6c54 6173 6b20 3d20 7365  ntervalTask = se
+000016a0: 7449 6e74 6572 7661 6c28 7468 6973 2e67  tInterval(this.g
+000016b0: 6574 436c 6965 6e74 4c69 7374 2c20 3330  etClientList, 30
+000016c0: 3030 290a 2020 2020 2020 2020 7d2c 0a20  00).        },. 
+000016d0: 2020 2020 2020 2062 6566 6f72 6544 6573         beforeDes
+000016e0: 7472 6f79 2829 207b 0a20 2020 2020 2020  troy() {.       
+000016f0: 2020 2020 2074 6869 732e 696e 7465 7276       this.interv
+00001700: 616c 5461 736b 2e73 746f 7028 290a 2020  alTask.stop().  
+00001710: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00001720: 206d 6574 686f 6473 3a20 7b0a 2020 2020   methods: {.    
+00001730: 2020 2020 2020 2020 6861 6e64 6c65 4164          handleAd
+00001740: 6428 726f 7729 207b 0a20 2020 2020 2020  d(row) {.       
+00001750: 2020 2020 2020 2020 2074 6869 732e 666f           this.fo
+00001760: 726d 203d 207b 0a20 2020 2020 2020 2020  rm = {.         
+00001770: 2020 2020 2020 2020 2020 2069 735f 6564             is_ed
+00001780: 6974 3a20 6661 6c73 652c 0a20 2020 2020  it: false,.     
+00001790: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000017a0: 6c69 656e 745f 6e61 6d65 3a20 2727 2c0a  lient_name: '',.
+000017b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017c0: 2020 2020 6e61 6d65 3a20 2727 2c0a 2020      name: '',.  
+000017d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017e0: 2020 6c6f 6361 6c5f 706f 7274 3a20 2727    local_port: ''
+000017f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001800: 2020 2020 2020 6c6f 6361 6c5f 6970 3a20        local_ip: 
+00001810: 2731 3237 2e30 2e30 2e31 272c 0a20 2020  '127.0.0.1',.   
+00001820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001830: 2072 656d 6f74 655f 706f 7274 3a20 2727   remote_port: ''
+00001840: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001850: 2020 2020 2020 7370 6565 645f 6c69 6d69        speed_limi
+00001860: 743a 2030 0a20 2020 2020 2020 2020 2020  t: 0.           
+00001870: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
+00001880: 2020 2020 2020 2074 6869 732e 666f 726d         this.form
+00001890: 2e63 6c69 656e 745f 6e61 6d65 203d 2072  .client_name = r
+000018a0: 6f77 2e63 6c69 656e 745f 6e61 6d65 0a20  ow.client_name. 
+000018b0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000018c0: 6f6e 736f 6c65 2e6c 6f67 2872 6f77 293b  onsole.log(row);
+000018d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000018e0: 2074 6869 732e 6469 616c 6f67 466f 726d   this.dialogForm
+000018f0: 5669 7369 626c 6520 3d20 7472 7565 0a20  Visible = true. 
+00001900: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+00001910: 2020 2020 2020 2020 2020 6861 6e64 6c65            handle
+00001920: 4564 6974 2872 6f77 2c20 636c 6965 6e74  Edit(row, client
+00001930: 5f6e 616d 6529 207b 0a20 2020 2020 2020  _name) {.       
+00001940: 2020 2020 2020 2020 2074 6869 732e 666f           this.fo
+00001950: 726d 203d 207b 0a20 2020 2020 2020 2020  rm = {.         
+00001960: 2020 2020 2020 2020 2020 2069 735f 6564             is_ed
+00001970: 6974 3a20 7472 7565 2c0a 2020 2020 2020  it: true,.      
+00001980: 2020 2020 2020 2020 2020 2020 2020 636c                cl
+00001990: 6965 6e74 5f6e 616d 653a 2063 6c69 656e  ient_name: clien
+000019a0: 745f 6e61 6d65 2c0a 2020 2020 2020 2020  t_name,.        
+000019b0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+000019c0: 3a20 726f 772e 6e61 6d65 2c0a 2020 2020  : row.name,.    
+000019d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019e0: 6c6f 6361 6c5f 706f 7274 3a20 726f 772e  local_port: row.
+000019f0: 6c6f 6361 6c5f 706f 7274 2c0a 2020 2020  local_port,.    
 00001a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a10: 2020 2072 6574 7572 6e20 616c 6572 7428     return alert(
-00001a20: 7265 732e 6461 7461 2e6d 7367 290a 2020  res.data.msg).  
-00001a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a40: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00001a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a60: 7468 6973 2e64 6961 6c6f 6746 6f72 6d56  this.dialogFormV
-00001a70: 6973 6962 6c65 203d 2066 616c 7365 0a20  isible = false. 
-00001a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a90: 2020 207d 292e 6361 7463 6828 6572 7220     }).catch(err 
-00001aa0: 3d3e 207b 0a20 2020 2020 2020 2020 2020  => {.           
-00001ab0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00001ac0: 736f 6c65 2e6c 6f67 2865 7272 290a 2020  sole.log(err).  
-00001ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ae0: 2020 2020 2020 616c 6572 7428 27e6 9c8d        alert('...
-00001af0: e58a a1e5 99a8 e587 bae7 8eb0 e994 99e8  ................
-00001b00: afaf 2729 0a20 2020 2020 2020 2020 2020  ..').           
-00001b10: 2020 2020 2020 2020 207d 290a 0a20 2020           })..   
-00001b20: 2020 2020 2020 2020 2020 2020 207d 290a               }).
-00001b30: 0a0a 2020 2020 2020 2020 2020 2020 7d2c  ..            },
-00001b40: 0a20 2020 2020 2020 2020 2020 2067 6574  .            get
-00001b50: 436c 6965 6e74 4c69 7374 2829 207b 0a20  ClientList() {. 
-00001b60: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-00001b70: 6172 2075 726c 203d 2077 696e 646f 772e  ar url = window.
-00001b80: 6c6f 6361 7469 6f6e 2e68 7265 662e 7370  location.href.sp
-00001b90: 6c69 7428 273f 2729 5b30 5d20 2b20 272f  lit('?')[0] + '/
-00001ba0: 6170 6927 0a20 2020 2020 2020 2020 2020  api'.           
-00001bb0: 2020 2020 2061 7869 6f73 2e67 6574 2875       axios.get(u
-00001bc0: 726c 2c20 7b0a 2020 2020 2020 2020 2020  rl, {.          
-00001bd0: 2020 2020 2020 2020 2020 6865 6164 6572            header
-00001be0: 733a 207b 746f 6b65 6e3a 206c 6f63 616c  s: {token: local
-00001bf0: 5374 6f72 6167 652e 6765 7449 7465 6d28  Storage.getItem(
-00001c00: 2774 6f6b 656e 2729 7d0a 2020 2020 2020  'token')}.      
-00001c10: 2020 2020 2020 2020 2020 7d29 2e74 6865            }).the
-00001c20: 6e28 7265 7320 3d3e 207b 0a20 2020 2020  n(res => {.     
-00001c30: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00001c40: 6f6e 736f 6c65 2e6c 6f67 2872 6573 290a  onsole.log(res).
-00001c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c60: 2020 2020 636f 6e73 7420 636f 6465 203d      const code =
-00001c70: 2072 6573 2e64 6174 612e 636f 6465 0a20   res.data.code. 
-00001c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c90: 2020 2069 6620 2863 6f64 6520 213d 3d20     if (code !== 
-00001ca0: 3230 3029 207b 0a20 2020 2020 2020 2020  200) {.         
-00001cb0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00001cc0: 6869 732e 246d 6573 7361 6765 2e65 7272  his.$message.err
-00001cd0: 6f72 2872 6573 2e64 6174 612e 6d73 6729  or(res.data.msg)
-00001ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001cf0: 2020 2020 2020 2020 2069 6620 2863 6f64           if (cod
-00001d00: 6520 3d3d 3d20 3430 3129 207b 0a20 2020  e === 401) {.   
-00001d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d20: 2020 2020 2020 2020 2073 6574 5469 6d65           setTime
-00001d30: 6f75 7428 2829 203d 3e20 7b0a 2020 2020  out(() => {.    
-00001d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d50: 2020 2020 2020 2020 2020 2020 6c6f 6361              loca
-00001d60: 7469 6f6e 2e72 656c 6f61 6428 293b 0a20  tion.reload();. 
-00001d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d80: 2020 2020 2020 2020 2020 207d 2c20 3230             }, 20
-00001d90: 3030 290a 2020 2020 2020 2020 2020 2020  00).            
-00001da0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00001db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001dc0: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-00001dd0: 2020 2020 2020 2020 7468 6973 2e74 6162          this.tab
-00001de0: 6c65 4461 7461 203d 2072 6573 2e64 6174  leData = res.dat
-00001df0: 612e 6461 7461 0a20 2020 2020 2020 2020  a.data.         
-00001e00: 2020 2020 2020 2020 2020 2063 6f6e 736f             conso
-00001e10: 6c65 2e6c 6f67 2874 6869 732e 7461 626c  le.log(this.tabl
-00001e20: 6544 6174 6129 0a20 2020 2020 2020 2020  eData).         
-00001e30: 2020 2020 2020 207d 292e 6361 7463 6828         }).catch(
-00001e40: 6572 7220 3d3e 207b 0a20 2020 2020 2020  err => {.       
-00001e50: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00001e60: 736f 6c65 2e6c 6f67 2865 7272 290a 2020  sole.log(err).  
-00001e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e80: 2020 7468 6973 2e24 6d65 7373 6167 652e    this.$message.
-00001e90: 6572 726f 7228 6572 7229 0a20 2020 2020  error(err).     
-00001ea0: 2020 2020 2020 2020 2020 2020 2020 202f                 /
-00001eb0: 2f20 616c 6572 7428 27e6 9c8d e58a a1e5  / alert('.......
-00001ec0: 99a8 e587 bae7 8eb0 e994 99e8 afaf 2729  ..............')
-00001ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001ee0: 207d 290a 2020 2020 2020 2020 2020 2020   }).            
-00001ef0: 7d0a 2020 2020 2020 2020 7d0a 2020 2020  }.        }.    
-00001f00: 7d29 0a3c 2f73 6372 6970 743e 0a0a 0a7b  }).</script>...{
-00001f10: 2520 656e 6420 257d 0a                   % end %}.
+00001a10: 6c6f 6361 6c5f 6970 3a20 726f 772e 6c6f  local_ip: row.lo
+00001a20: 6361 6c5f 6970 2c0a 2020 2020 2020 2020  cal_ip,.        
+00001a30: 2020 2020 2020 2020 2020 2020 7265 6d6f              remo
+00001a40: 7465 5f70 6f72 743a 2072 6f77 2e72 656d  te_port: row.rem
+00001a50: 6f74 655f 706f 7274 2c0a 2020 2020 2020  ote_port,.      
+00001a60: 2020 2020 2020 2020 2020 2020 2020 7370                sp
+00001a70: 6565 645f 6c69 6d69 743a 2072 6f77 2e73  eed_limit: row.s
+00001a80: 7065 6564 5f6c 696d 6974 0a20 2020 2020  peed_limit.     
+00001a90: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00001aa0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+00001ab0: 736f 6c65 2e6c 6f67 2827 2d2d 2d2d 2d2d  sole.log('------
+00001ac0: 2d27 2c20 2072 6f77 293b 0a20 2020 2020  -',  row);.     
+00001ad0: 2020 2020 2020 2020 2020 2074 6869 732e             this.
+00001ae0: 6469 616c 6f67 466f 726d 5669 7369 626c  dialogFormVisibl
+00001af0: 6520 3d20 7472 7565 0a20 2020 2020 2020  e = true.       
+00001b00: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00001b10: 2020 2020 7375 626d 6974 4164 644f 7245      submitAddOrE
+00001b20: 6469 7428 2920 7b0a 2020 2020 2020 2020  dit() {.        
+00001b30: 2020 2020 2020 2020 7661 7220 7572 6c20          var url 
+00001b40: 3d20 7769 6e64 6f77 2e6c 6f63 6174 696f  = window.locatio
+00001b50: 6e2e 6872 6566 2e73 706c 6974 2827 3f27  n.href.split('?'
+00001b60: 295b 305d 202b 2027 2f61 7069 270a 0a20  )[0] + '/api'.. 
+00001b70: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00001b80: 6f6e 736f 6c65 2e6c 6f67 2874 6869 732e  onsole.log(this.
+00001b90: 666f 726d 290a 2020 2020 2020 2020 2020  form).          
+00001ba0: 2020 2020 2020 6178 696f 732e 706f 7374        axios.post
+00001bb0: 2875 726c 2c20 7468 6973 2e66 6f72 6d29  (url, this.form)
+00001bc0: 2e74 6865 6e28 7265 7320 3d3e 207b 0a20  .then(res => {. 
+00001bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001be0: 2020 2069 6620 2872 6573 2e64 6174 612e     if (res.data.
+00001bf0: 636f 6465 2021 3d3d 2032 3030 2920 7b0a  code !== 200) {.
+00001c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c10: 2020 2020 2020 2020 7265 7475 726e 2061          return a
+00001c20: 6c65 7274 2872 6573 2e64 6174 612e 6d73  lert(res.data.ms
+00001c30: 6729 0a20 2020 2020 2020 2020 2020 2020  g).             
+00001c40: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00001c50: 2020 2020 2020 2020 2020 2020 2074 6869               thi
+00001c60: 732e 6469 616c 6f67 466f 726d 5669 7369  s.dialogFormVisi
+00001c70: 626c 6520 3d20 6661 6c73 650a 2020 2020  ble = false.    
+00001c80: 2020 2020 2020 2020 2020 2020 7d29 2e63              }).c
+00001c90: 6174 6368 2865 7272 203d 3e20 7b0a 2020  atch(err => {.  
+00001ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001cb0: 2020 636f 6e73 6f6c 652e 6c6f 6728 6572    console.log(er
+00001cc0: 7229 0a20 2020 2020 2020 2020 2020 2020  r).             
+00001cd0: 2020 2020 2020 2074 6869 732e 246d 6573         this.$mes
+00001ce0: 7361 6765 2e65 7272 6f72 2827 e994 99e4  sage.error('....
+00001cf0: ba86 e593 a6ef bc8c e8bf 99e6 98af e4b8  ................
+00001d00: 80e6 9da1 e994 99e8 afaf e6b6 88e6 81af  ................
+00001d10: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
+00001d20: 2020 2020 2020 2061 6c65 7274 2827 e69c         alert('..
+00001d30: 8de5 8aa1 e599 a8e5 87ba e78e b0e9 9499  ................
+00001d40: e8af af27 290a 2020 2020 2020 2020 2020  ...').          
+00001d50: 2020 2020 2020 7d29 0a20 2020 2020 2020        }).       
+00001d60: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00001d70: 2020 2020 6861 6e64 6c65 4465 6c65 7465      handleDelete
+00001d80: 2863 6c69 656e 745f 6e61 6d65 2c20 6e61  (client_name, na
+00001d90: 6d65 2920 7b0a 2020 2020 2020 2020 2020  me) {.          
+00001da0: 2020 2020 2020 7661 7220 7572 6c20 3d20        var url = 
+00001db0: 7769 6e64 6f77 2e6c 6f63 6174 696f 6e2e  window.location.
+00001dc0: 6872 6566 2e73 706c 6974 2827 3f27 295b  href.split('?')[
+00001dd0: 305d 202b 2027 2f61 7069 270a 2020 2020  0] + '/api'.    
+00001de0: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
+00001df0: 7420 7061 7261 6d73 203d 207b 0a20 2020  t params = {.   
+00001e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e10: 2063 6c69 656e 745f 6e61 6d65 3a20 636c   client_name: cl
+00001e20: 6965 6e74 5f6e 616d 652c 0a20 2020 2020  ient_name,.     
+00001e30: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00001e40: 616d 653a 206e 616d 650a 2020 2020 2020  ame: name.      
+00001e50: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00001e60: 2020 2020 2020 2020 2020 2020 7468 6973              this
+00001e70: 2e24 636f 6e66 6972 6d28 27e5 88a0 e999  .$confirm('.....
+00001e80: a4e5 908e e8af a5e5 aea2 e688 b7e7 abaf  ................
+00001e90: e5b0 86e9 878d e696 b0e8 bf9e e68e a52c  ...............,
+00001ea0: 20e6 98af e590 a6e7 bba7 e7bb ad3f 272c   ............?',
+00001eb0: 2027 e68f 90e7 a4ba 272c 207b 0a20 2020   '......', {.   
+00001ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ed0: 2063 6f6e 6669 726d 4275 7474 6f6e 5465   confirmButtonTe
+00001ee0: 7874 3a20 27e7 a1ae e5ae 9a27 2c0a 2020  xt: '......',.  
+00001ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f00: 2020 6361 6e63 656c 4275 7474 6f6e 5465    cancelButtonTe
+00001f10: 7874 3a20 27e5 8f96 e6b6 8827 2c0a 2020  xt: '......',.  
+00001f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f30: 2020 7479 7065 3a20 2777 6172 6e69 6e67    type: 'warning
+00001f40: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+00001f50: 2020 7d29 2e74 6865 6e28 2829 203d 3e20    }).then(() => 
+00001f60: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00001f70: 2020 2020 2020 6178 696f 732e 6465 6c65        axios.dele
+00001f80: 7465 2875 726c 2c20 7b0a 2020 2020 2020  te(url, {.      
+00001f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fa0: 2020 7061 7261 6d73 3a20 7061 7261 6d73    params: params
+00001fb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001fc0: 2020 2020 207d 292e 7468 656e 2872 6573       }).then(res
+00001fd0: 203d 3e20 7b0a 2020 2020 2020 2020 2020   => {.          
+00001fe0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00001ff0: 2028 7265 732e 6461 7461 2e63 6f64 6520   (res.data.code 
+00002000: 213d 3d20 3230 3029 207b 0a20 2020 2020  !== 200) {.     
+00002010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002020: 2020 2020 2020 2072 6574 7572 6e20 616c         return al
+00002030: 6572 7428 7265 732e 6461 7461 2e6d 7367  ert(res.data.msg
+00002040: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00002050: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00002060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002070: 2020 2020 7468 6973 2e64 6961 6c6f 6746      this.dialogF
+00002080: 6f72 6d56 6973 6962 6c65 203d 2066 616c  ormVisible = fal
+00002090: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
+000020a0: 2020 2020 2020 207d 292e 6361 7463 6828         }).catch(
+000020b0: 6572 7220 3d3e 207b 0a20 2020 2020 2020  err => {.       
+000020c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000020d0: 2063 6f6e 736f 6c65 2e6c 6f67 2865 7272   console.log(err
+000020e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000020f0: 2020 2020 2020 2020 2020 616c 6572 7428            alert(
+00002100: 27e6 9c8d e58a a1e5 99a8 e587 bae7 8eb0  '...............
+00002110: e994 99e8 afaf 2729 0a20 2020 2020 2020  ......').       
+00002120: 2020 2020 2020 2020 2020 2020 207d 290a               }).
+00002130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002140: 207d 290a 0a0a 2020 2020 2020 2020 2020   })...          
+00002150: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+00002160: 2067 6574 436c 6965 6e74 4c69 7374 2829   getClientList()
+00002170: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00002180: 2020 2076 6172 2075 726c 203d 2077 696e     var url = win
+00002190: 646f 772e 6c6f 6361 7469 6f6e 2e68 7265  dow.location.hre
+000021a0: 662e 7370 6c69 7428 273f 2729 5b30 5d20  f.split('?')[0] 
+000021b0: 2b20 272f 6170 6927 0a20 2020 2020 2020  + '/api'.       
+000021c0: 2020 2020 2020 2020 2061 7869 6f73 2e67           axios.g
+000021d0: 6574 2875 726c 2c20 7b0a 2020 2020 2020  et(url, {.      
+000021e0: 2020 2020 2020 2020 2020 2020 2020 6865                he
+000021f0: 6164 6572 733a 207b 746f 6b65 6e3a 206c  aders: {token: l
+00002200: 6f63 616c 5374 6f72 6167 652e 6765 7449  ocalStorage.getI
+00002210: 7465 6d28 2774 6f6b 656e 2729 7d0a 2020  tem('token')}.  
+00002220: 2020 2020 2020 2020 2020 2020 2020 7d29                })
+00002230: 2e74 6865 6e28 7265 7320 3d3e 207b 0a20  .then(res => {. 
+00002240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002250: 2020 2063 6f6e 736f 6c65 2e6c 6f67 2872     console.log(r
+00002260: 6573 290a 2020 2020 2020 2020 2020 2020  es).            
+00002270: 2020 2020 2020 2020 636f 6e73 7420 636f          const co
+00002280: 6465 203d 2072 6573 2e64 6174 612e 636f  de = res.data.co
+00002290: 6465 0a20 2020 2020 2020 2020 2020 2020  de.             
+000022a0: 2020 2020 2020 2069 6620 2863 6f64 6520         if (code 
+000022b0: 213d 3d20 3230 3029 207b 0a20 2020 2020  !== 200) {.     
+000022c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022d0: 2020 2074 6869 732e 246d 6573 7361 6765     this.$message
+000022e0: 2e65 7272 6f72 2872 6573 2e64 6174 612e  .error(res.data.
+000022f0: 6d73 6729 0a20 2020 2020 2020 2020 2020  msg).           
+00002300: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00002310: 2863 6f64 6520 3d3d 3d20 3430 3129 207b  (code === 401) {
+00002320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002330: 2020 2020 2020 2020 2020 2020 2073 6574               set
+00002340: 5469 6d65 6f75 7428 2829 203d 3e20 7b0a  Timeout(() => {.
+00002350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002370: 6c6f 6361 7469 6f6e 2e72 656c 6f61 6428  location.reload(
+00002380: 293b 0a20 2020 2020 2020 2020 2020 2020  );.             
+00002390: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+000023a0: 2c20 3230 3030 290a 2020 2020 2020 2020  , 2000).        
+000023b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023c0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+000023d0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+000023e0: 2020 2020 2020 2020 2020 2020 7468 6973              this
+000023f0: 2e74 6162 6c65 4461 7461 203d 2072 6573  .tableData = res
+00002400: 2e64 6174 612e 6461 7461 0a20 2020 2020  .data.data.     
+00002410: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00002420: 6f6e 736f 6c65 2e6c 6f67 2874 6869 732e  onsole.log(this.
+00002430: 7461 626c 6544 6174 6129 0a20 2020 2020  tableData).     
+00002440: 2020 2020 2020 2020 2020 207d 292e 6361             }).ca
+00002450: 7463 6828 6572 7220 3d3e 207b 0a20 2020  tch(err => {.   
+00002460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002470: 2063 6f6e 736f 6c65 2e6c 6f67 2865 7272   console.log(err
+00002480: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00002490: 2020 2020 2020 7468 6973 2e24 6d65 7373        this.$mess
+000024a0: 6167 652e 6572 726f 7228 6572 7229 0a20  age.error(err). 
+000024b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024c0: 2020 202f 2f20 616c 6572 7428 27e6 9c8d     // alert('...
+000024d0: e58a a1e5 99a8 e587 bae7 8eb0 e994 99e8  ................
+000024e0: afaf 2729 0a20 2020 2020 2020 2020 2020  ..').           
+000024f0: 2020 2020 207d 290a 2020 2020 2020 2020       }).        
+00002500: 2020 2020 7d0a 2020 2020 2020 2020 7d0a      }.        }.
+00002510: 2020 2020 7d29 0a3c 2f73 6372 6970 743e      }).</script>
+00002520: 0a0a 0a7b 2520 656e 6420 257d 0a         ...{% end %}.
```

### Comparing `proxynt-1.1.8/server/template/js/axios.min.js` & `proxynt-1.1.9/server/template/js/axios.min.js`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/server/template/js/index.js` & `proxynt-1.1.9/server/template/js/index.js`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/server/template/js/vue.min.js` & `proxynt-1.1.9/server/template/js/vue.min.js`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/server/template/login.html` & `proxynt-1.1.9/server/template/login.html`

 * *Files identical despite different names*

### Comparing `proxynt-1.1.8/server/websocket_handler.py` & `proxynt-1.1.9/server/websocket_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         start_time = time.time()
         try:
             await (super(MyWebSocketaHandler, self).write_message(bytes(message), binary))
             if LoggerFactory.get_logger().isEnabledFor(logging.DEBUG):
                 LoggerFactory.get_logger().debug(f'write message cost time {time.time() - start_time}, len: {len(message)}')
             return
         except Exception:
-            LoggerFactory.get_logger().info(message)
+            LoggerFactory.get_logger().info(f'send error: {message[:10]}')
             LoggerFactory.get_logger().error(traceback.format_exc())
             raise
 
     def on_message(self, m_bytes):
         asyncio.ensure_future(self.on_message_async(m_bytes))
 
     async def on_message_async(self, message):
@@ -104,30 +104,34 @@
                         try:
                             listen_socket = tcp_forward_client.create_listen_socket(d['remote_port'])
                         except OSError:
                             self.close(None, 'Address already in use')
                             # tcp_forward_client.close_by_client_name(self.client_name)
                             raise
                         ip_port = d['local_ip'] + ':' + str(d['local_port'])
-                        await tcp_forward_client.register_listen_server(listen_socket, d['name'], ip_port, self)
+                        d.setdefault('speed_limit', 0)
+                        speed_limit: float = d.get('speed_limit', 0)  # 网速限制
+                        await tcp_forward_client.register_listen_server(listen_socket, d['name'], ip_port, self, speed_limit)
                         listen_socket_list.append(listen_socket)
                     self.handler_to_recv_time[self] = time.time()
                     self.client_name_to_handler[client_name] = self
                     self.push_config = push_config
+                await self.write_message(NatSerialization.dumps(message_dict, key), binary=True)  # 更新完配置再发给客户端
             elif message_dict['type_'] == MessageTypeConstant.PING:
                 self.handler_to_recv_time[self] = time.time()
             if LoggerFactory.get_logger().isEnabledFor(logging.DEBUG):
                 LoggerFactory.get_logger().debug(f'on message cost time {time.time() - start_time}')
         except Exception:
             LoggerFactory.get_logger().error(traceback.format_exc())
 
     def on_close(self, code: int = None, reason: str = None) -> None:
         asyncio.ensure_future(self._on_close(code, reason))
 
     async def _on_close(self, code: int = None, reason: str = None) -> None:
+        print('close', self.client_name)
         try:
             async with self.lock:
                 if self.client_name:
                     if self in self.handler_to_recv_time:
                         self.handler_to_recv_time.pop(self)
                     if self.client_name in self.client_name_to_handler:
                         self.client_name_to_handler.pop(self.client_name)
```

### Comparing `proxynt-1.1.8/setup.py` & `proxynt-1.1.9/setup.py`

 * *Files identical despite different names*

