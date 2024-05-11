# Comparing `tmp/bittrade_binance_websocket-0.4.5.tar.gz` & `tmp/bittrade_binance_websocket-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bittrade_binance_websocket-0.4.5.tar", max compression
+gzip compressed data, was "bittrade_binance_websocket-0.4.6.tar", max compression
```

## Comparing `bittrade_binance_websocket-0.4.5.tar` & `bittrade_binance_websocket-0.4.6.tar`

### file list

```diff
@@ -1,83 +1,84 @@
--rw-r--r--   0        0        0     4488 2023-03-07 05:41:03.026348 bittrade_binance_websocket-0.4.5/README.md
--rw-r--r--   0        0        0       24 2023-03-07 05:17:43.720880 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/__init__.py
--rw-r--r--   0        0        0      169 2023-03-24 09:56:30.829676 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/channels/__init__.py
--rw-r--r--   0        0        0     1349 2023-03-24 09:56:30.829844 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/channels/book_ticker.py
--rw-r--r--   0        0        0     1310 2023-03-24 09:56:30.829984 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/channels/depth.py
--rw-r--r--   0        0        0      238 2023-03-24 09:56:30.830247 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/channels/message.py
--rw-r--r--   0        0        0      437 2023-03-26 22:59:27.836025 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/channels/open_orders.py
--rw-r--r--   0        0        0     2150 2023-03-24 09:56:30.830917 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/channels/subscribe.py
--rw-r--r--   0        0        0      387 2023-03-24 09:56:30.831631 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/connection/__init__.py
--rw-r--r--   0        0        0      984 2023-03-26 22:59:27.836890 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/connection/connection_operators.py
--rw-r--r--   0        0        0     3748 2024-05-09 07:48:41.282667 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/connection/generic.py
--rw-r--r--   0        0        0     2836 2024-03-31 00:34:09.193021 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/connection/http.py
--rw-r--r--   0        0        0     1020 2023-03-24 09:56:30.834946 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/connection/private.py
--rw-r--r--   0        0        0     2843 2023-03-28 23:26:32.900253 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/connection/private_user_stream.py
--rw-r--r--   0        0        0      866 2023-03-24 09:56:30.835882 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/connection/public_stream.py
--rw-r--r--   0        0        0     3556 2023-03-07 05:17:43.704616 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/connection/reconnect.py
--rw-r--r--   0        0        0        0 2023-03-24 09:56:30.836219 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/events/__init__.py
--rw-r--r--   0        0        0     3411 2023-04-04 10:06:55.441962 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/events/add_order.py
--rw-r--r--   0        0        0     4603 2023-04-04 10:06:55.443228 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/events/cancel_order.py
--rw-r--r--   0        0        0     1222 2023-03-24 09:56:30.837752 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/events/ping.py
--rw-r--r--   0        0        0     1955 2023-03-26 22:59:27.837933 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/events/request_response.py
--rw-r--r--   0        0        0     1160 2023-03-24 09:56:30.838014 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/events/time.py
--rw-r--r--   0        0        0      109 2023-03-24 09:56:30.843408 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/framework/__init__.py
--rw-r--r--   0        0        0    11013 2024-04-16 08:51:05.177221 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/framework/framework.py
--rw-r--r--   0        0        0        0 2023-03-07 05:17:43.701890 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/messages/__init__.py
--rw-r--r--   0        0        0        0 2023-03-07 05:17:43.699712 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/messages/filters/__init__.py
--rw-r--r--   0        0        0      628 2023-03-24 09:56:30.844042 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/messages/filters/kind.py
--rw-r--r--   0        0        0      197 2023-03-07 05:17:43.702941 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/messages/heartbeat.py
--rw-r--r--   0        0        0      709 2023-03-07 05:17:43.703639 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/messages/json.py
--rw-r--r--   0        0        0      710 2023-03-24 09:56:30.844242 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/messages/listen.py
--rw-r--r--   0        0        0      500 2023-03-26 22:59:27.838272 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/__init__.py
--rw-r--r--   0        0        0      200 2023-03-26 22:59:27.838358 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/accounts.py
--rw-r--r--   0        0        0       76 2023-03-24 09:56:30.844826 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/contingency_type.py
--rw-r--r--   0        0        0     2461 2024-05-03 22:43:05.431269 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/endpoints.py
--rw-r--r--   0        0        0     1597 2023-04-12 10:32:29.217681 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/enhanced_websocket.py
--rw-r--r--   0        0        0     5670 2024-04-16 08:51:09.517146 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/framework.py
--rw-r--r--   0        0        0      872 2024-03-07 07:45:37.550442 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/loan.py
--rw-r--r--   0        0        0      430 2023-03-26 22:59:27.838973 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/message.py
--rw-r--r--   0        0        0      404 2023-03-24 09:56:30.847283 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/oco_list_status.py
--rw-r--r--   0        0        0     5822 2023-12-29 07:38:44.204038 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/order.py
--rw-r--r--   0        0        0      951 2023-03-24 09:56:30.847605 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/order_status.py
--rw-r--r--   0        0        0      316 2023-03-24 09:56:30.847749 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/permission.py
--rw-r--r--   0        0        0      289 2024-01-31 20:08:59.754811 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/portfolio.py
--rw-r--r--   0        0        0      170 2023-04-04 10:06:55.444253 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/private.py
--rw-r--r--   0        0        0      441 2023-03-24 09:56:30.848482 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/request.py
--rw-r--r--   0        0        0      280 2023-03-26 23:08:09.996282 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/response_message.py
--rw-r--r--   0        0        0      556 2024-05-03 22:39:51.170025 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/rest/__init__.py
--rw-r--r--   0        0        0     2255 2024-05-04 00:22:51.578642 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/rest/api_key.py
--rw-r--r--   0        0        0       85 2023-03-07 06:12:01.053861 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/rest/get_time.py
--rw-r--r--   0        0        0       91 2023-03-24 09:56:30.849188 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/rest/listen_key.py
--rw-r--r--   0        0        0      595 2023-03-28 03:30:34.779137 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/rest/margin_account.py
--rw-r--r--   0        0        0     4822 2024-03-20 05:48:12.475535 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/rest/subaccount.py
--rw-r--r--   0        0        0      155 2023-08-11 03:01:00.567477 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/rest/symbol_price_book_ticker.py
--rw-r--r--   0        0        0       98 2023-03-26 22:59:27.839358 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/rest/symbol_price_ticker.py
--rw-r--r--   0        0        0      254 2023-03-24 09:56:30.849325 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/symbol_status.py
--rw-r--r--   0        0        0     1112 2023-04-13 04:00:27.126562 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/trade.py
--rw-r--r--   0        0        0       16 2023-03-07 05:17:43.713863 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/operators/__init__.py
--rw-r--r--   0        0        0      740 2023-03-07 05:17:43.715065 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/operators/orderbook/__init__.py
--rw-r--r--   0        0        0      696 2023-03-26 22:59:27.840157 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/operators/stream/response_messages.py
--rw-r--r--   0        0        0        0 2023-03-07 05:21:43.314741 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/__init__.py
--rw-r--r--   0        0        0     1428 2024-03-21 03:36:28.175760 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/account_information.py
--rw-r--r--   0        0        0     4562 2024-05-03 22:50:11.064813 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/api_key.py
--rw-r--r--   0        0        0     1199 2024-03-21 03:40:41.482848 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/cancel_order.py
--rw-r--r--   0        0        0     1198 2024-03-21 03:39:54.416229 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/create_order.py
--rw-r--r--   0        0        0      724 2023-04-01 05:17:10.507682 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/current_open_orders.py
--rw-r--r--   0        0        0      533 2023-03-07 07:26:25.278031 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/get_time.py
--rw-r--r--   0        0        0     1408 2024-03-21 03:54:13.880279 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/http_factory_decorator.py
--rw-r--r--   0        0        0     3288 2024-03-13 06:37:04.186727 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/listen_key.py
--rw-r--r--   0        0        0     2295 2024-03-07 08:46:32.989830 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/margin_loan.py
--rw-r--r--   0        0        0      541 2024-01-31 20:10:47.047786 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/margin_portfolio.py
--rw-r--r--   0        0        0      680 2023-03-28 03:38:33.700120 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/query_margin_account.py
--rw-r--r--   0        0        0      718 2023-03-28 03:39:36.381947 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/query_margin_fee_data.py
--rw-r--r--   0        0        0      553 2024-03-07 08:45:29.544664 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/query_margin_price_index.py
--rw-r--r--   0        0        0      697 2024-03-24 01:17:20.975687 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/query_max_transfer_out_amount.py
--rw-r--r--   0        0        0     2731 2024-04-16 08:49:52.006258 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/subaccount.py
--rw-r--r--   0        0        0     1241 2023-04-01 05:22:24.238266 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/symbol_orders_cancel.py
--rw-r--r--   0        0        0      687 2023-08-11 03:01:27.219437 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/symbol_price_book_ticker.py
--rw-r--r--   0        0        0      669 2023-03-26 22:59:27.840905 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/symbol_price_ticker.py
--rw-r--r--   0        0        0     2271 2023-04-13 07:43:16.471911 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/trade_list.py
--rw-r--r--   0        0        0     3848 2024-05-03 01:25:21.922596 bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/sign.py
--rw-r--r--   0        0        0     1771 2024-05-09 07:56:05.787668 bittrade_binance_websocket-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     6057 1970-01-01 00:00:00.000000 bittrade_binance_websocket-0.4.5/setup.py
--rw-r--r--   0        0        0     5706 1970-01-01 00:00:00.000000 bittrade_binance_websocket-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     4488 2023-03-07 05:41:03.026348 bittrade_binance_websocket-0.4.6/README.md
+-rw-r--r--   0        0        0       24 2023-03-07 05:17:43.720880 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/__init__.py
+-rw-r--r--   0        0        0      169 2023-03-24 09:56:30.829676 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/channels/__init__.py
+-rw-r--r--   0        0        0     1349 2023-03-24 09:56:30.829844 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/channels/book_ticker.py
+-rw-r--r--   0        0        0     1310 2023-03-24 09:56:30.829984 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/channels/depth.py
+-rw-r--r--   0        0        0      238 2023-03-24 09:56:30.830247 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/channels/message.py
+-rw-r--r--   0        0        0      437 2023-03-26 22:59:27.836025 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/channels/open_orders.py
+-rw-r--r--   0        0        0     2150 2023-03-24 09:56:30.830917 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/channels/subscribe.py
+-rw-r--r--   0        0        0      387 2023-03-24 09:56:30.831631 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/connection/__init__.py
+-rw-r--r--   0        0        0      984 2023-03-26 22:59:27.836890 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/connection/connection_operators.py
+-rw-r--r--   0        0        0     3936 2024-05-11 03:13:11.161116 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/connection/generic.py
+-rw-r--r--   0        0        0     2836 2024-03-31 00:34:09.193021 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/connection/http.py
+-rw-r--r--   0        0        0     1020 2023-03-24 09:56:30.834946 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/connection/private.py
+-rw-r--r--   0        0        0     2843 2023-03-28 23:26:32.900253 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/connection/private_user_stream.py
+-rw-r--r--   0        0        0      866 2023-03-24 09:56:30.835882 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/connection/public_stream.py
+-rw-r--r--   0        0        0     3556 2023-03-07 05:17:43.704616 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/connection/reconnect.py
+-rw-r--r--   0        0        0        0 2023-03-24 09:56:30.836219 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/events/__init__.py
+-rw-r--r--   0        0        0     1449 2024-05-11 03:09:29.393009 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/events/account_status.py
+-rw-r--r--   0        0        0     3411 2023-04-04 10:06:55.441962 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/events/add_order.py
+-rw-r--r--   0        0        0     4603 2023-04-04 10:06:55.443228 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/events/cancel_order.py
+-rw-r--r--   0        0        0     1222 2023-03-24 09:56:30.837752 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/events/ping.py
+-rw-r--r--   0        0        0     1955 2023-03-26 22:59:27.837933 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/events/request_response.py
+-rw-r--r--   0        0        0     1160 2023-03-24 09:56:30.838014 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/events/time.py
+-rw-r--r--   0        0        0      109 2023-03-24 09:56:30.843408 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/framework/__init__.py
+-rw-r--r--   0        0        0    11013 2024-04-16 08:51:05.177221 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/framework/framework.py
+-rw-r--r--   0        0        0        0 2023-03-07 05:17:43.701890 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/messages/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-07 05:17:43.699712 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/messages/filters/__init__.py
+-rw-r--r--   0        0        0      628 2023-03-24 09:56:30.844042 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/messages/filters/kind.py
+-rw-r--r--   0        0        0      197 2023-03-07 05:17:43.702941 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/messages/heartbeat.py
+-rw-r--r--   0        0        0      709 2023-03-07 05:17:43.703639 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/messages/json.py
+-rw-r--r--   0        0        0      710 2023-03-24 09:56:30.844242 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/messages/listen.py
+-rw-r--r--   0        0        0      500 2023-03-26 22:59:27.838272 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/__init__.py
+-rw-r--r--   0        0        0      200 2023-03-26 22:59:27.838358 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/accounts.py
+-rw-r--r--   0        0        0       76 2023-03-24 09:56:30.844826 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/contingency_type.py
+-rw-r--r--   0        0        0     2461 2024-05-03 22:43:05.431269 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/endpoints.py
+-rw-r--r--   0        0        0     1597 2023-04-12 10:32:29.217681 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/enhanced_websocket.py
+-rw-r--r--   0        0        0     5670 2024-04-16 08:51:09.517146 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/framework.py
+-rw-r--r--   0        0        0      872 2024-03-07 07:45:37.550442 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/loan.py
+-rw-r--r--   0        0        0      430 2023-03-26 22:59:27.838973 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/message.py
+-rw-r--r--   0        0        0      404 2023-03-24 09:56:30.847283 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/oco_list_status.py
+-rw-r--r--   0        0        0     5822 2023-12-29 07:38:44.204038 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/order.py
+-rw-r--r--   0        0        0      951 2023-03-24 09:56:30.847605 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/order_status.py
+-rw-r--r--   0        0        0      316 2023-03-24 09:56:30.847749 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/permission.py
+-rw-r--r--   0        0        0      289 2024-01-31 20:08:59.754811 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/portfolio.py
+-rw-r--r--   0        0        0      170 2023-04-04 10:06:55.444253 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/private.py
+-rw-r--r--   0        0        0      441 2023-03-24 09:56:30.848482 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/request.py
+-rw-r--r--   0        0        0      280 2023-03-26 23:08:09.996282 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/response_message.py
+-rw-r--r--   0        0        0      556 2024-05-03 22:39:51.170025 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/rest/__init__.py
+-rw-r--r--   0        0        0     2255 2024-05-04 00:22:51.578642 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/rest/api_key.py
+-rw-r--r--   0        0        0       85 2023-03-07 06:12:01.053861 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/rest/get_time.py
+-rw-r--r--   0        0        0       91 2023-03-24 09:56:30.849188 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/rest/listen_key.py
+-rw-r--r--   0        0        0      595 2023-03-28 03:30:34.779137 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/rest/margin_account.py
+-rw-r--r--   0        0        0     4822 2024-03-20 05:48:12.475535 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/rest/subaccount.py
+-rw-r--r--   0        0        0      155 2023-08-11 03:01:00.567477 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/rest/symbol_price_book_ticker.py
+-rw-r--r--   0        0        0       98 2023-03-26 22:59:27.839358 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/rest/symbol_price_ticker.py
+-rw-r--r--   0        0        0      254 2023-03-24 09:56:30.849325 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/symbol_status.py
+-rw-r--r--   0        0        0     1112 2023-04-13 04:00:27.126562 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/trade.py
+-rw-r--r--   0        0        0       16 2023-03-07 05:17:43.713863 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/operators/__init__.py
+-rw-r--r--   0        0        0      740 2023-03-07 05:17:43.715065 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/operators/orderbook/__init__.py
+-rw-r--r--   0        0        0      696 2023-03-26 22:59:27.840157 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/operators/stream/response_messages.py
+-rw-r--r--   0        0        0        0 2023-03-07 05:21:43.314741 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/__init__.py
+-rw-r--r--   0        0        0     1428 2024-03-21 03:36:28.175760 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/account_information.py
+-rw-r--r--   0        0        0     4562 2024-05-03 22:50:11.064813 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/api_key.py
+-rw-r--r--   0        0        0     1199 2024-03-21 03:40:41.482848 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/cancel_order.py
+-rw-r--r--   0        0        0     1198 2024-03-21 03:39:54.416229 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/create_order.py
+-rw-r--r--   0        0        0      724 2023-04-01 05:17:10.507682 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/current_open_orders.py
+-rw-r--r--   0        0        0      533 2023-03-07 07:26:25.278031 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/get_time.py
+-rw-r--r--   0        0        0     1408 2024-03-21 03:54:13.880279 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/http_factory_decorator.py
+-rw-r--r--   0        0        0     3288 2024-03-13 06:37:04.186727 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/listen_key.py
+-rw-r--r--   0        0        0     2295 2024-03-07 08:46:32.989830 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/margin_loan.py
+-rw-r--r--   0        0        0      541 2024-01-31 20:10:47.047786 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/margin_portfolio.py
+-rw-r--r--   0        0        0      680 2023-03-28 03:38:33.700120 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/query_margin_account.py
+-rw-r--r--   0        0        0      718 2023-03-28 03:39:36.381947 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/query_margin_fee_data.py
+-rw-r--r--   0        0        0      553 2024-03-07 08:45:29.544664 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/query_margin_price_index.py
+-rw-r--r--   0        0        0      697 2024-03-24 01:17:20.975687 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/query_max_transfer_out_amount.py
+-rw-r--r--   0        0        0     2731 2024-04-16 08:49:52.006258 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/subaccount.py
+-rw-r--r--   0        0        0     1241 2023-04-01 05:22:24.238266 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/symbol_orders_cancel.py
+-rw-r--r--   0        0        0      687 2023-08-11 03:01:27.219437 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/symbol_price_book_ticker.py
+-rw-r--r--   0        0        0      669 2023-03-26 22:59:27.840905 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/symbol_price_ticker.py
+-rw-r--r--   0        0        0     2271 2023-04-13 07:43:16.471911 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/trade_list.py
+-rw-r--r--   0        0        0     3924 2024-05-11 03:09:29.393889 bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/sign.py
+-rw-r--r--   0        0        0     1772 2024-05-11 03:13:56.636048 bittrade_binance_websocket-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0     6057 1970-01-01 00:00:00.000000 bittrade_binance_websocket-0.4.6/setup.py
+-rw-r--r--   0        0        0     5706 1970-01-01 00:00:00.000000 bittrade_binance_websocket-0.4.6/PKG-INFO
```

### Comparing `bittrade_binance_websocket-0.4.5/README.md` & `bittrade_binance_websocket-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/channels/book_ticker.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/channels/book_ticker.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/channels/depth.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/channels/depth.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/channels/subscribe.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/channels/subscribe.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/connection/connection_operators.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/connection/connection_operators.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/connection/generic.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/connection/generic.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,37 +28,40 @@
 ) -> Observable[WebsocketBundle]:
     def subscribe(
         observer: ObserverBase[WebsocketBundle],
         scheduler_: Optional[SchedulerBase] = None,
     ):
         _scheduler = scheduler or scheduler_ or ThreadPoolScheduler()
         connection: WebSocketApp | None = None
+        already_connected = False
 
         def action(*args: Any):
-            nonlocal connection
+            nonlocal connection, already_connected
 
             def on_error(_ws: WebSocketApp, error: Exception):
                 logger.error("[SOCKET][RAW] Websocket errored %s", error)
-                # TODO any other errors we should handle as "not yet connected"?
-                if getattr(error, "errno", None) not in [61]:
+                # There are cases (like no internet connection) where the socket will never open, but will error. We don't want to emit closed in that case
+                if already_connected:
                     observer.on_next((enhanced, WEBSOCKET_STATUS, WEBSOCKET_CLOSED))
                 observer.on_error(error)
 
             def on_close(_ws: WebSocketApp, close_status_code: int, close_msg: str):
                 logger.warning(
                     "[SOCKET][RAW] Websocket closed | url: %s, status: %s, close message: %s",
                     url,
                     close_status_code,
                     close_msg,
                 )
                 observer.on_next((enhanced, WEBSOCKET_STATUS, WEBSOCKET_CLOSED))
                 observer.on_error(Exception("Socket closed"))
 
             def on_open(_ws: WebSocketApp):
+                nonlocal already_connected
                 logger.info("[SOCKET][RAW] Websocket opened at %s", url)
+                already_connected = True
                 observer.on_next((enhanced, WEBSOCKET_STATUS, WEBSOCKET_OPENED))
 
             def on_message(ws: WebSocketApp, message: bytes | str):
                 pass_message = orjson.loads(message)
                 category = WEBSOCKET_MESSAGE
                 raw_logger.debug(message)
                 logger.debug("[SOCKET][RAW] %s", message)
```

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/connection/http.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/connection/http.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/connection/private.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/connection/private.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/connection/private_user_stream.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/connection/private_user_stream.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/connection/public_stream.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/connection/public_stream.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/connection/reconnect.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/connection/reconnect.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/events/add_order.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/events/add_order.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/events/cancel_order.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/events/cancel_order.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/events/ping.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/events/ping.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/events/request_response.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/events/request_response.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/events/time.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/events/time.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/framework/framework.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/framework/framework.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/messages/filters/kind.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/messages/filters/kind.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/messages/json.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/messages/json.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/messages/listen.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/messages/listen.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/endpoints.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/endpoints.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/enhanced_websocket.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/enhanced_websocket.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/framework.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/framework.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/loan.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/loan.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/order.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/order.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/order_status.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/order_status.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/rest/__init__.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/rest/api_key.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/rest/api_key.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/rest/margin_account.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/rest/margin_account.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/rest/subaccount.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/rest/subaccount.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/models/trade.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/models/trade.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/operators/orderbook/__init__.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/operators/orderbook/__init__.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/operators/stream/response_messages.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/operators/stream/response_messages.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/account_information.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/account_information.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/api_key.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/api_key.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/cancel_order.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/cancel_order.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/create_order.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/create_order.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/current_open_orders.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/current_open_orders.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/get_time.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/get_time.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/http_factory_decorator.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/http_factory_decorator.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/listen_key.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/listen_key.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/margin_loan.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/margin_loan.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/margin_portfolio.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/margin_portfolio.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/query_margin_account.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/query_margin_account.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/query_margin_fee_data.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/query_margin_fee_data.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/query_margin_price_index.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/query_margin_price_index.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/query_max_transfer_out_amount.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/query_max_transfer_out_amount.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/subaccount.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/subaccount.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/symbol_orders_cancel.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/symbol_orders_cancel.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/symbol_price_book_ticker.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/symbol_price_book_ticker.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/symbol_price_ticker.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/symbol_price_ticker.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/rest/trade_list.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/rest/trade_list.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.5/bittrade_binance_websocket/sign.py` & `bittrade_binance_websocket-0.4.6/bittrade_binance_websocket/sign.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,17 @@
     sorted_tuple = tuple()
     keys = sorted(values)
     for key in keys:
         value = values[key]
         if isinstance(value, Enum):
             value = cast(Enum, value).value
 
+        if isinstance(value, bool):
+            value = str(value).lower()
+
         # remove None
         if value is not None:
             sorted_tuple = sorted_tuple + (
                 (
                     key,
                     value,
                 ),
```

### Comparing `bittrade_binance_websocket-0.4.5/pyproject.toml` & `bittrade_binance_websocket-0.4.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bittrade-binance-websocket"
-version = "0.4.5"
+version = "0.4.6"
 description = "Reactive Websocket for Binance"
 authors = ["mat <matt@techspace.asia>"]
 readme = "README.md"
 repository = "https://github.com/TechSpaceAsia/bittrade-binance-websocket"
 homepage = "https://github.com/TechSpaceAsia/bittrade-binance-websocket"
 license = "MIT"
 classifiers = [
@@ -50,14 +50,15 @@
 
 
 
 
 
 
 
+
```

### Comparing `bittrade_binance_websocket-0.4.5/setup.py` & `bittrade_binance_websocket-0.4.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
  'requests>=2.28.2,<3.0.0',
  'returns>=0.19.0,<0.20.0',
  'websocket-client>=1.4.2,<2.0.0',
  'websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'bittrade-binance-websocket',
-    'version': '0.4.5',
+    'version': '0.4.6',
     'description': 'Reactive Websocket for Binance',
     'long_description': '# Binance Websocket\n\n[NOT RELEASED] This is very much a work in progress, despite being on pypi.\nMost things might be wrongly documented; API **will** change\n\n## Features\n\n- Reconnect with incremental backoff \n- Respond to ping\n- request/response factories e.g. `add_order_factory` make websocket events feel like calling an API\n- ... but provides more info than a simple request/response; \n  for instance, `add_order` goes through each stage submitted->pending->open or canceled, \n  emitting a notification at each stage\n\n## Installing\n\n`pip install bittrade-binance-websocket` or `poetry add bittrade-binance-websocket`\n\n## General considerations\n\n### Observables/Reactivex\n\nThe whole library is build with [Reactivex](https://rxpy.readthedocs.io/en/latest/).\n\nThough Observables seem complicated at first, they are the best way to handle - and (synchronously) test - complex situations that arise over time, like an invalid sequence of messages or socket disconnection and backoff reconnects.\n\nFor simple use cases, they are also rather easy to use as shown in the [examples](./examples) folder or in the Getting Started below\n\n### Concurrency\n\nInternally the library uses threads.\nFor your main program you don\'t have to worry about threads; you can block the main thread.\n\n## Getting started\n\n### Connect to the public feeds\n\n```python\nfrom bittrade_huobi_websocket import public_websocket_connection, subscribe_ticker\nfrom bittrade_huobi_websocket.operators import keep_messages_only, filter_new_socket_only\n\n# Prepare connection - note, this is a ConnectableObservable, so it will only trigger connection when we call its ``connect`` method\nsocket_connection = public_websocket_connection()\n# Prepare a feed with only "real" messages, dropping things like status update, heartbeat, etc…\nmessages = socket_connection.pipe(\n    keep_messages_only(),\n)\nsocket_connection.pipe(\n    filter_new_socket_only(),\n    subscribe_ticker(\'USDT/USD\', messages)\n).subscribe(\n    print, print, print  # you can do anything with the messages; here we simply print them out\n)\nsocket_connection.connect()\n```\n\n_(This script is complete, it should run "as is")_\n\n\n## Logging\n\nWe use Python\'s standard logging.\nYou can modify what logs you see as follows:\n\n```\nlogging.getLogger(\'bittrade_huobi_websocket\').addHandler(logging.StreamHandler())\n```\n\nIn addition, two special logger logs every message sent/received from the socket (except heartbeat) at the `DEBUG` level: `bittrade_huobi_websocket.raw_socket.sent` and `bittrade_huobi_websocket.raw_socket.received`\n\nTo view a full, timestamped history of the socket exchanges use\n\n```\nhandler = FileHandler("logs/raw_socket.log")\nhandler.setLevel(DEBUG)\nlogger = logging.getLogger("bittrade_huobi_websocket.raw_socket.sent")\nformatter = logging.Formatter("%(asctime)s.%(msecs)03d <== %(message)s", datefmt="%H:%M:%S")\nhandler.setFormatter(formatter)\nlogger.addHandler(handler)\nhandler = FileHandler("logs/raw_socket.log")\nhandler.setLevel(DEBUG)\nlogger = logging.getLogger("bittrade_huobi_websocket.raw_socket.received")\nformatter = logging.Formatter("%(asctime)s.%(msecs)03d --> %(message)s", datefmt="%H:%M:%S")\nhandler.setFormatter(formatter)\nlogger.addHandler(handler)\n```\n\n## Private feeds\n\nSimilar to [bittrade-kraken-rest](https://github.com/TechSpaceAsia/bittrade-kraken-rest), this library attempts to get as little access to sensitive information as possible.\n\nThis means that you\'ll need to implement the signature token yourself. The library never has access to your API secret.\n\nSee `examples/sign.py` for an example of implementation but it is generally as simple as:\n\n```python\nauthenticated_sockets = connection.pipe(\n    filter_new_socket_only(),\n    operators.map(add_token),\n    operators.share(),\n)\n```\n\n# Development guidelines\n\n## `*_http` methods\n\nREST functions over http should be suffixed with `_http` e.g. `get_book_http`.\nThey should return an Observable containing the *full* json body; this is easily achieved via `prepare_request` and `send_request`.\n\nWhere possible models should be defined to describe the *raw* result and *parsed result* if available/useful.\n\nReactive operators may be provided for parsing, but they should never be included in the *raw* functionality of the `*_http` function, only optional.\n\nAny operator that maps to CCXT types should be suffixed with `_ccxt` e.g. `parse_book_ccxt`.',
     'author': 'mat',
     'author_email': 'matt@techspace.asia',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/TechSpaceAsia/bittrade-binance-websocket',
```

### Comparing `bittrade_binance_websocket-0.4.5/PKG-INFO` & `bittrade_binance_websocket-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bittrade-binance-websocket
-Version: 0.4.5
+Version: 0.4.6
 Summary: Reactive Websocket for Binance
 Home-page: https://github.com/TechSpaceAsia/bittrade-binance-websocket
 License: MIT
 Author: mat
 Author-email: matt@techspace.asia
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
```

