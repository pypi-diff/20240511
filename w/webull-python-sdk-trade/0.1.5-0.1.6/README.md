# Comparing `tmp/webull-python-sdk-trade-0.1.5.tar.gz` & `tmp/webull_python_sdk_trade-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webull-python-sdk-trade-0.1.5.tar", last modified: Sat Feb 11 06:16:13 2023, max compression
+gzip compressed data, was "webull_python_sdk_trade-0.1.6.tar", last modified: Sat May 11 03:38:26 2024, max compression
```

## Comparing `webull-python-sdk-trade-0.1.5.tar` & `webull_python_sdk_trade-0.1.6.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 06:16:13.494977 webull-python-sdk-trade-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/ChangeLog.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-02-11 06:16:13.494977 webull-python-sdk-trade-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-11 06:16:13.494977 webull-python-sdk-trade-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 06:16:13.490977 webull-python-sdk-trade-0.1.5/webull_python_sdk_trade.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-02-11 06:16:13.000000 webull-python-sdk-trade-0.1.5/webull_python_sdk_trade.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-02-11 06:16:13.000000 webull-python-sdk-trade-0.1.5/webull_python_sdk_trade.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-11 06:16:13.000000 webull-python-sdk-trade-0.1.5/webull_python_sdk_trade.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-02-11 06:16:13.000000 webull-python-sdk-trade-0.1.5/webull_python_sdk_trade.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-11 06:16:13.000000 webull-python-sdk-trade-0.1.5/webull_python_sdk_trade.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 06:16:13.490977 webull-python-sdk-trade-0.1.5/webullsdktrade/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 06:16:13.490977 webull-python-sdk-trade-0.1.5/webullsdktrade/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/common/account_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/common/category.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/common/combo_ticker_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/common/combo_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/common/currency.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/common/forbid_reason.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/common/instrument_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/common/markets.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/common/order_entrust_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/common/order_side.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/common/order_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/common/order_tif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/common/order_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/common/trade_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/common/trading_date_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/common/trailing_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 06:16:13.490977 webull-python-sdk-trade-0.1.5/webullsdktrade/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/events/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/grpc_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 06:16:13.494977 webull-python-sdk-trade-0.1.5/webullsdktrade/request/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/request/cancel_order_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/request/get_account_balance_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/request/get_account_positions_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/request/get_account_profile_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/request/get_app_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/request/get_open_orders_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/request/get_order_detail_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/request/get_today_orders_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/request/get_trade_calendar_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/request/get_trade_instrument_detail_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/request/palce_order_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/request/replace_order_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 06:16:13.494977 webull-python-sdk-trade-0.1.5/webullsdktrade/trade/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/trade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/trade/account_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/trade/order_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/trade/trade_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-02-11 06:16:00.000000 webull-python-sdk-trade-0.1.5/webullsdktrade/trade/trade_instrument.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:38:26.064902 webull_python_sdk_trade-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/ChangeLog.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-11 03:38:26.064902 webull_python_sdk_trade-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 03:38:26.064902 webull_python_sdk_trade-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:38:26.064902 webull_python_sdk_trade-0.1.6/webull_python_sdk_trade.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-11 03:38:26.000000 webull_python_sdk_trade-0.1.6/webull_python_sdk_trade.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-11 03:38:26.000000 webull_python_sdk_trade-0.1.6/webull_python_sdk_trade.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 03:38:26.000000 webull_python_sdk_trade-0.1.6/webull_python_sdk_trade.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-11 03:38:26.000000 webull_python_sdk_trade-0.1.6/webull_python_sdk_trade.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-11 03:38:26.000000 webull_python_sdk_trade-0.1.6/webull_python_sdk_trade.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:38:26.056902 webull_python_sdk_trade-0.1.6/webullsdktrade/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:38:26.060902 webull_python_sdk_trade-0.1.6/webullsdktrade/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/common/account_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/common/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/common/combo_ticker_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/common/combo_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/common/currency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/common/forbid_reason.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/common/instrument_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/common/markets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/common/order_entrust_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/common/order_side.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/common/order_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/common/order_tif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/common/order_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/common/trade_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/common/trading_date_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/common/trailing_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:38:26.060902 webull_python_sdk_trade-0.1.6/webullsdktrade/events/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/events/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/grpc_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:38:26.060902 webull_python_sdk_trade-0.1.6/webullsdktrade/request/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/request/cancel_order_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/request/get_account_balance_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/request/get_account_positions_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/request/get_account_profile_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/request/get_app_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/request/get_open_orders_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/request/get_order_detail_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/request/get_today_orders_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/request/get_trade_calendar_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/request/get_trade_instrument_detail_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/request/palce_order_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/request/replace_order_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:38:26.060902 webull_python_sdk_trade-0.1.6/webullsdktrade/trade/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/trade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/trade/account_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8441 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/trade/order_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/trade/trade_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-11 03:38:18.000000 webull_python_sdk_trade-0.1.6/webullsdktrade/trade/trade_instrument.py
```

### Comparing `webull-python-sdk-trade-0.1.5/setup.py` & `webull_python_sdk_trade-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 RD_CONTENT_TYPE = "text/markdown"
 LICENSE = "Apache License 2.0"
 
 with open("README.rst") as fp:
     LONG_DESCRIPTION = fp.read()
 
 requires = [
-    "webull-python-sdk-trade-events-core==0.1.5",
-    "webull-python-sdk-core==0.1.5"
+    "webull-python-sdk-trade-events-core==0.1.6",
+    "webull-python-sdk-core==0.1.6"
 ]
 
 setup_args = {
     'version': VERSION,
     'author': AUTHOR,
     'author_email': AUTHOR_EMAIL,
     'description': DESCRIPTION,
```

### Comparing `webull-python-sdk-trade-0.1.5/webull_python_sdk_trade.egg-info/SOURCES.txt` & `webull_python_sdk_trade-0.1.6/webull_python_sdk_trade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/api.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/api.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/common/account_type.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/common/account_type.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/common/category.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/common/category.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/common/combo_ticker_type.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/common/combo_ticker_type.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/common/combo_type.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/common/combo_type.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/common/currency.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/common/currency.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,12 +13,12 @@
 # limitations under the License.
 
 # coding=utf-8
 from webullsdkcore.common.easy_enum import EasyEnum
 
 
 class Currency(EasyEnum):
-    CNY = (1, "CNY")
+    CNH = (1, "CNH")
     CAD = (2, "CAD")
     HKD = (3, "HKD")
     USD = (4, "USD")
```

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/common/forbid_reason.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/common/forbid_reason.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/common/instrument_type.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/common/instrument_type.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/common/markets.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/common/markets.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/common/order_entrust_type.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/common/order_entrust_type.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/common/order_side.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/common/order_side.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/common/order_status.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/common/order_status.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/common/order_tif.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/common/order_tif.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/common/order_type.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/common/order_type.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/common/trade_policy.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/common/trade_policy.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/common/trading_date_type.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/common/trading_date_type.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/common/trailing_type.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/common/trailing_type.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/events/types.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/events/types.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/grpc_api.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/grpc_api.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/request/cancel_order_request.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/request/cancel_order_request.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/request/get_account_balance_request.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/request/get_account_balance_request.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/request/get_account_positions_request.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/request/get_account_positions_request.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/request/get_account_profile_request.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/request/get_account_profile_request.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/request/get_app_subscriptions.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/request/get_app_subscriptions.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/request/get_open_orders_request.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/request/get_open_orders_request.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/request/get_order_detail_request.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/request/get_order_detail_request.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/request/get_today_orders_request.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/request/get_today_orders_request.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/request/get_trade_calendar_request.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/request/get_trade_calendar_request.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/request/get_trade_instrument_detail_request.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/request/get_trade_instrument_detail_request.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/request/palce_order_request.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/request/palce_order_request.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/request/replace_order_request.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/request/replace_order_request.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/trade/account_info.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/trade/account_info.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/trade/order_operation.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/trade/order_operation.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/trade/trade_calendar.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/trade/trade_calendar.py`

 * *Files identical despite different names*

### Comparing `webull-python-sdk-trade-0.1.5/webullsdktrade/trade/trade_instrument.py` & `webull_python_sdk_trade-0.1.6/webullsdktrade/trade/trade_instrument.py`

 * *Files identical despite different names*

