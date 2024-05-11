# Comparing `tmp/fast_tradier_client-1.0.2.tar.gz` & `tmp/fast_tradier_client-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_tradier_client-1.0.2.tar", last modified: Fri May 10 01:18:13 2024, max compression
+gzip compressed data, was "fast_tradier_client-1.0.3.tar", last modified: Fri May 10 04:42:10 2024, max compression
```

## Comparing `fast_tradier_client-1.0.2.tar` & `fast_tradier_client-1.0.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:18:13.741325 fast_tradier_client-1.0.2/
--rw-rw-rw-   0 root         (0) root         (0)     1073 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)    11014 2024-05-10 01:18:13.741325 fast_tradier_client-1.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    10270 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:18:13.737324 fast_tradier_client-1.0.2/fast_tradier/
--rw-rw-rw-   0 root         (0) root         (0)    16899 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/FastTradierAsyncClient.py
--rw-rw-rw-   0 root         (0) root         (0)    16356 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/FastTradierClient.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:18:13.741325 fast_tradier_client-1.0.2/fast_tradier/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)     3237 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/interfaces/IBrokerAsyncClient.py
--rw-rw-rw-   0 root         (0) root         (0)     3063 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/interfaces/IBrokerClient.py
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/interfaces/IModel.py
--rw-rw-rw-   0 root         (0) root         (0)      291 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/interfaces/IRealTimeQuoteProvider.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/interfaces/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:18:13.741325 fast_tradier_client-1.0.2/fast_tradier/models/
--rw-rw-rw-   0 root         (0) root         (0)      479 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/DataClassModelBase.py
--rw-rw-rw-   0 root         (0) root         (0)     1471 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/ModelBase.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:18:13.741325 fast_tradier_client-1.0.2/fast_tradier/models/account/
--rw-rw-rw-   0 root         (0) root         (0)     1224 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/account/AccountBalance.py
--rw-rw-rw-   0 root         (0) root         (0)     1640 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/account/AccountOrder.py
--rw-rw-rw-   0 root         (0) root         (0)      367 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/account/Position.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/account/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:18:13.741325 fast_tradier_client-1.0.2/fast_tradier/models/market_data/
--rw-rw-rw-   0 root         (0) root         (0)      647 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/market_data/Hlocv.py
--rw-rw-rw-   0 root         (0) root         (0)     2311 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/market_data/Quote.py
--rw-rw-rw-   0 root         (0) root         (0)     1035 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/market_data/TradierQuote.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/market_data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:18:13.741325 fast_tradier_client-1.0.2/fast_tradier/models/trading/
--rw-rw-rw-   0 root         (0) root         (0)      115 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/trading/Duration.py
--rw-rw-rw-   0 root         (0) root         (0)     2440 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/trading/EquityOrder.py
--rw-rw-rw-   0 root         (0) root         (0)      169 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/trading/Interval.py
--rw-rw-rw-   0 root         (0) root         (0)     2108 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/trading/OptionOrder.py
--rw-rw-rw-   0 root         (0) root         (0)       95 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/trading/OrderBase.py
--rw-rw-rw-   0 root         (0) root         (0)      330 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/trading/PriceTypes.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/trading/Sides.py
--rw-rw-rw-   0 root         (0) root         (0)     2385 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/trading/TOSTradierConverter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/models/trading/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:18:13.741325 fast_tradier_client-1.0.2/fast_tradier/utils/
--rw-rw-rw-   0 root         (0) root         (0)     1284 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/utils/OptionUtils.py
--rw-rw-rw-   0 root         (0) root         (0)     1888 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/utils/TimeUtils.py
--rw-rw-rw-   0 root         (0) root         (0)     2020 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/utils/YFinanceQuoteProvider.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/fast_tradier/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:18:13.741325 fast_tradier_client-1.0.2/fast_tradier_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11014 2024-05-10 01:18:13.000000 fast_tradier_client-1.0.2/fast_tradier_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1529 2024-05-10 01:18:13.000000 fast_tradier_client-1.0.2/fast_tradier_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 01:18:13.000000 fast_tradier_client-1.0.2/fast_tradier_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2024-05-10 01:18:13.000000 fast_tradier_client-1.0.2/fast_tradier_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-10 01:18:13.000000 fast_tradier_client-1.0.2/fast_tradier_client.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      907 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-10 01:18:13.741325 fast_tradier_client-1.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      473 2024-05-10 01:17:39.000000 fast_tradier_client-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 04:42:10.279065 fast_tradier_client-1.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    11014 2024-05-10 04:42:10.279065 fast_tradier_client-1.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    10270 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 04:42:10.275066 fast_tradier_client-1.0.3/fast_tradier/
+-rw-rw-rw-   0 root         (0) root         (0)    16899 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/FastTradierAsyncClient.py
+-rw-rw-rw-   0 root         (0) root         (0)    16356 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/FastTradierClient.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 04:42:10.275066 fast_tradier_client-1.0.3/fast_tradier/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)     3237 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/interfaces/IBrokerAsyncClient.py
+-rw-rw-rw-   0 root         (0) root         (0)     3063 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/interfaces/IBrokerClient.py
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/interfaces/IModel.py
+-rw-rw-rw-   0 root         (0) root         (0)      291 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/interfaces/IRealTimeQuoteProvider.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/interfaces/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 04:42:10.275066 fast_tradier_client-1.0.3/fast_tradier/models/
+-rw-rw-rw-   0 root         (0) root         (0)      479 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/DataClassModelBase.py
+-rw-rw-rw-   0 root         (0) root         (0)     1471 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/ModelBase.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 04:42:10.275066 fast_tradier_client-1.0.3/fast_tradier/models/account/
+-rw-rw-rw-   0 root         (0) root         (0)     1224 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/account/AccountBalance.py
+-rw-rw-rw-   0 root         (0) root         (0)     1895 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/account/AccountOrder.py
+-rw-rw-rw-   0 root         (0) root         (0)      367 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/account/Position.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/account/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 04:42:10.275066 fast_tradier_client-1.0.3/fast_tradier/models/market_data/
+-rw-rw-rw-   0 root         (0) root         (0)      647 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/market_data/Hlocv.py
+-rw-rw-rw-   0 root         (0) root         (0)     2311 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/market_data/Quote.py
+-rw-rw-rw-   0 root         (0) root         (0)     1035 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/market_data/TradierQuote.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/market_data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 04:42:10.275066 fast_tradier_client-1.0.3/fast_tradier/models/trading/
+-rw-rw-rw-   0 root         (0) root         (0)      115 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/trading/Duration.py
+-rw-rw-rw-   0 root         (0) root         (0)     2440 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/trading/EquityOrder.py
+-rw-rw-rw-   0 root         (0) root         (0)      169 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/trading/Interval.py
+-rw-rw-rw-   0 root         (0) root         (0)     3320 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/trading/OptionOrder.py
+-rw-rw-rw-   0 root         (0) root         (0)       95 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/trading/OrderBase.py
+-rw-rw-rw-   0 root         (0) root         (0)      330 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/trading/PriceTypes.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/trading/Sides.py
+-rw-rw-rw-   0 root         (0) root         (0)     2385 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/trading/TOSTradierConverter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/trading/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 04:42:10.275066 fast_tradier_client-1.0.3/fast_tradier/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     1284 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/utils/OptionUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/utils/TimeUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2020 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/utils/YFinanceQuoteProvider.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 04:42:10.275066 fast_tradier_client-1.0.3/fast_tradier_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11014 2024-05-10 04:42:10.000000 fast_tradier_client-1.0.3/fast_tradier_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1529 2024-05-10 04:42:10.000000 fast_tradier_client-1.0.3/fast_tradier_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 04:42:10.000000 fast_tradier_client-1.0.3/fast_tradier_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2024-05-10 04:42:10.000000 fast_tradier_client-1.0.3/fast_tradier_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-10 04:42:10.000000 fast_tradier_client-1.0.3/fast_tradier_client.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      907 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-10 04:42:10.279065 fast_tradier_client-1.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      473 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/setup.py
```

### Comparing `fast_tradier_client-1.0.2/LICENSE` & `fast_tradier_client-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.2/PKG-INFO` & `fast_tradier_client-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_tradier_client
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Tradier client for trading stocks and options through Tradier API
 Home-page: https://pypi.org/project/fast-tradier-client/
 Author: Tony W
 Author-email: Tony Wang <ivytony@gmail.com>
 Project-URL: Homepage, https://bitbucket.org/rcholic/fast-tradier-client
 Project-URL: Bug Tracker, https://bitbucket.org/rcholic/fast-tradier-client/jira?statuses=new&statuses=indeterminate&sort=-updated&page=1
 Keywords: python,fast-tradier-client,tradier
```

### Comparing `fast_tradier_client-1.0.2/README.md` & `fast_tradier_client-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.2/fast_tradier/FastTradierAsyncClient.py` & `fast_tradier_client-1.0.3/fast_tradier/FastTradierAsyncClient.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.2/fast_tradier/FastTradierClient.py` & `fast_tradier_client-1.0.3/fast_tradier/FastTradierClient.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.2/fast_tradier/interfaces/IBrokerAsyncClient.py` & `fast_tradier_client-1.0.3/fast_tradier/interfaces/IBrokerAsyncClient.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.2/fast_tradier/interfaces/IBrokerClient.py` & `fast_tradier_client-1.0.3/fast_tradier/interfaces/IBrokerClient.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.2/fast_tradier/models/ModelBase.py` & `fast_tradier_client-1.0.3/fast_tradier/models/ModelBase.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.2/fast_tradier/models/account/AccountBalance.py` & `fast_tradier_client-1.0.3/fast_tradier/models/account/AccountBalance.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.2/fast_tradier/models/market_data/Hlocv.py` & `fast_tradier_client-1.0.3/fast_tradier/models/market_data/Hlocv.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.2/fast_tradier/models/market_data/Quote.py` & `fast_tradier_client-1.0.3/fast_tradier/models/market_data/Quote.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.2/fast_tradier/models/market_data/TradierQuote.py` & `fast_tradier_client-1.0.3/fast_tradier/models/market_data/TradierQuote.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.2/fast_tradier/models/trading/EquityOrder.py` & `fast_tradier_client-1.0.3/fast_tradier/models/trading/EquityOrder.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.2/fast_tradier/models/trading/OptionOrder.py` & `fast_tradier_client-1.0.3/fast_tradier/models/trading/OptionOrder.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,35 +2,32 @@
 
 from fast_tradier.models.trading.TOSTradierConverter import TOSTradierConverter
 from fast_tradier.models.ModelBase import ModelBase
 from fast_tradier.models.trading.Sides import OptionOrderSide
 from fast_tradier.models.trading.PriceTypes import OptionPriceType
 from fast_tradier.models.trading.Duration import Duration
 from fast_tradier.models.trading.OrderBase import OrderBase
+from fast_tradier.models.ModelBase import NewModelBase
 from pydantic import BaseModel, ConfigDict
 
-class NewModelBase(BaseModel):
-    model_config = ConfigDict(use_enum_values=True)
-    
-    def to_json(self) -> Mapping[str, Any]:
-        return self.model_dump()
-
 class OptionLeg(NewModelBase):
+    model_config = ConfigDict(use_enum_values=True)
     underlying_symbol: str
     option_symbol: str
     quantity: int
     side: OptionOrderSide
     
     def reverse_side(self) -> None:
         if self.side == OptionOrderSide.SellToOpen or self.side == OptionOrderSide.SellToOpen.value:
             setattr(self, "side", OptionOrderSide.BuyToClose)
         elif self.side == OptionOrderSide.BuyToOpen or self.side == OptionOrderSide.BuyToOpen.value:
             setattr(self, "side", OptionOrderSide.SellToClose)
 
 class OptionOrder(NewModelBase):
+    model_config = ConfigDict(use_enum_values=True)
     ticker: str
     price: float
     price_type: OptionPriceType
     duration: Duration
     option_legs: List[OptionLeg]
     status: str = "pending"
     order_class: str = "multileg" # could be "option"
@@ -52,8 +49,41 @@
         '''deep clone option_legs'''
         cloned_legs = []
         for opt_leg in self.option_legs:
             leg = OptionLeg(**(opt_leg.to_json()))
             if reverse_side:
                 leg.reverse_side()
 
-            cloned_legs.append(leg)
+            cloned_legs.append(leg)
+        return cloned_legs
+    
+    def to_json(self) -> Mapping[str, Any]:
+        """
+        Override to_json so that the format complies to Tradier API.
+        Returns:
+            Mapping[str, Any]: _description_
+        """
+        result: Dict[str, Any] = {
+            "id": self.id,
+            "status": self.status,
+            "symbol": self.ticker,
+            "duration": self.duration,
+            "price": self.price,
+            "type": self.price_type,
+            "class": self.order_class,
+        }
+
+        if len(self.option_legs) == 1:
+            result["option_symbol"] = self.option_legs[0].option_symbol
+            result["side"] = self.option_legs[0].side
+            result["quantity"] = self.option_legs[0].quantity
+        elif len(self.option_legs) > 1:
+            for i in range(len(self.option_legs)):
+                opt_item = self.option_legs[i]
+                symbol_key = f"option_symbol[{i}]"
+                result[symbol_key] = opt_item.option_symbol
+                side_key = f"side[{i}]"
+                result[side_key] = f"{opt_item.side}"
+                quant_key = f"quantity[{i}]"
+                result[quant_key] = f"{opt_item.quantity}"
+
+        return result
```

### Comparing `fast_tradier_client-1.0.2/fast_tradier/models/trading/TOSTradierConverter.py` & `fast_tradier_client-1.0.3/fast_tradier/models/trading/TOSTradierConverter.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.2/fast_tradier/utils/OptionUtils.py` & `fast_tradier_client-1.0.3/fast_tradier/utils/OptionUtils.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.2/fast_tradier/utils/TimeUtils.py` & `fast_tradier_client-1.0.3/fast_tradier/utils/TimeUtils.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.2/fast_tradier/utils/YFinanceQuoteProvider.py` & `fast_tradier_client-1.0.3/fast_tradier/utils/YFinanceQuoteProvider.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.2/fast_tradier_client.egg-info/PKG-INFO` & `fast_tradier_client-1.0.3/fast_tradier_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-tradier-client
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Tradier client for trading stocks and options through Tradier API
 Home-page: https://pypi.org/project/fast-tradier-client/
 Author: Tony W
 Author-email: Tony Wang <ivytony@gmail.com>
 Project-URL: Homepage, https://bitbucket.org/rcholic/fast-tradier-client
 Project-URL: Bug Tracker, https://bitbucket.org/rcholic/fast-tradier-client/jira?statuses=new&statuses=indeterminate&sort=-updated&page=1
 Keywords: python,fast-tradier-client,tradier
```

### Comparing `fast_tradier_client-1.0.2/fast_tradier_client.egg-info/SOURCES.txt` & `fast_tradier_client-1.0.3/fast_tradier_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.2/pyproject.toml` & `fast_tradier_client-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fast_tradier_client"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Tony Wang", email="ivytony@gmail.com" },
 ]
 description = "A Tradier client for trading stocks and options through Tradier API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

