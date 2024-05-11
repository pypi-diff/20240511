# Comparing `tmp/fast_tradier_client-1.0.3.tar.gz` & `tmp/fast_tradier_client-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_tradier_client-1.0.3.tar", last modified: Fri May 10 04:42:10 2024, max compression
+gzip compressed data, was "fast_tradier_client-1.0.4.tar", last modified: Sat May 11 02:30:03 2024, max compression
```

## Comparing `fast_tradier_client-1.0.3.tar` & `fast_tradier_client-1.0.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 04:42:10.279065 fast_tradier_client-1.0.3/
--rw-rw-rw-   0 root         (0) root         (0)     1073 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)    11014 2024-05-10 04:42:10.279065 fast_tradier_client-1.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    10270 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 04:42:10.275066 fast_tradier_client-1.0.3/fast_tradier/
--rw-rw-rw-   0 root         (0) root         (0)    16899 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/FastTradierAsyncClient.py
--rw-rw-rw-   0 root         (0) root         (0)    16356 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/FastTradierClient.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 04:42:10.275066 fast_tradier_client-1.0.3/fast_tradier/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)     3237 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/interfaces/IBrokerAsyncClient.py
--rw-rw-rw-   0 root         (0) root         (0)     3063 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/interfaces/IBrokerClient.py
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/interfaces/IModel.py
--rw-rw-rw-   0 root         (0) root         (0)      291 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/interfaces/IRealTimeQuoteProvider.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/interfaces/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 04:42:10.275066 fast_tradier_client-1.0.3/fast_tradier/models/
--rw-rw-rw-   0 root         (0) root         (0)      479 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/DataClassModelBase.py
--rw-rw-rw-   0 root         (0) root         (0)     1471 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/ModelBase.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 04:42:10.275066 fast_tradier_client-1.0.3/fast_tradier/models/account/
--rw-rw-rw-   0 root         (0) root         (0)     1224 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/account/AccountBalance.py
--rw-rw-rw-   0 root         (0) root         (0)     1895 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/account/AccountOrder.py
--rw-rw-rw-   0 root         (0) root         (0)      367 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/account/Position.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/account/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 04:42:10.275066 fast_tradier_client-1.0.3/fast_tradier/models/market_data/
--rw-rw-rw-   0 root         (0) root         (0)      647 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/market_data/Hlocv.py
--rw-rw-rw-   0 root         (0) root         (0)     2311 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/market_data/Quote.py
--rw-rw-rw-   0 root         (0) root         (0)     1035 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/market_data/TradierQuote.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/market_data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 04:42:10.275066 fast_tradier_client-1.0.3/fast_tradier/models/trading/
--rw-rw-rw-   0 root         (0) root         (0)      115 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/trading/Duration.py
--rw-rw-rw-   0 root         (0) root         (0)     2440 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/trading/EquityOrder.py
--rw-rw-rw-   0 root         (0) root         (0)      169 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/trading/Interval.py
--rw-rw-rw-   0 root         (0) root         (0)     3320 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/trading/OptionOrder.py
--rw-rw-rw-   0 root         (0) root         (0)       95 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/trading/OrderBase.py
--rw-rw-rw-   0 root         (0) root         (0)      330 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/trading/PriceTypes.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/trading/Sides.py
--rw-rw-rw-   0 root         (0) root         (0)     2385 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/trading/TOSTradierConverter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/models/trading/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 04:42:10.275066 fast_tradier_client-1.0.3/fast_tradier/utils/
--rw-rw-rw-   0 root         (0) root         (0)     1284 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/utils/OptionUtils.py
--rw-rw-rw-   0 root         (0) root         (0)     1888 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/utils/TimeUtils.py
--rw-rw-rw-   0 root         (0) root         (0)     2020 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/utils/YFinanceQuoteProvider.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/fast_tradier/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 04:42:10.275066 fast_tradier_client-1.0.3/fast_tradier_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11014 2024-05-10 04:42:10.000000 fast_tradier_client-1.0.3/fast_tradier_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1529 2024-05-10 04:42:10.000000 fast_tradier_client-1.0.3/fast_tradier_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 04:42:10.000000 fast_tradier_client-1.0.3/fast_tradier_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2024-05-10 04:42:10.000000 fast_tradier_client-1.0.3/fast_tradier_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-10 04:42:10.000000 fast_tradier_client-1.0.3/fast_tradier_client.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      907 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-10 04:42:10.279065 fast_tradier_client-1.0.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      473 2024-05-10 04:41:42.000000 fast_tradier_client-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 02:30:03.285582 fast_tradier_client-1.0.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    11014 2024-05-11 02:30:03.285582 fast_tradier_client-1.0.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    10270 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 02:30:03.281582 fast_tradier_client-1.0.4/fast_tradier/
+-rw-rw-rw-   0 root         (0) root         (0)    16899 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/FastTradierAsyncClient.py
+-rw-rw-rw-   0 root         (0) root         (0)    16356 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/FastTradierClient.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 02:30:03.281582 fast_tradier_client-1.0.4/fast_tradier/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)     3237 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/interfaces/IBrokerAsyncClient.py
+-rw-rw-rw-   0 root         (0) root         (0)     3063 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/interfaces/IBrokerClient.py
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/interfaces/IModel.py
+-rw-rw-rw-   0 root         (0) root         (0)      291 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/interfaces/IRealTimeQuoteProvider.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/interfaces/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 02:30:03.281582 fast_tradier_client-1.0.4/fast_tradier/models/
+-rw-rw-rw-   0 root         (0) root         (0)      479 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/DataClassModelBase.py
+-rw-rw-rw-   0 root         (0) root         (0)     1471 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/ModelBase.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 02:30:03.281582 fast_tradier_client-1.0.4/fast_tradier/models/account/
+-rw-rw-rw-   0 root         (0) root         (0)     1224 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/account/AccountBalance.py
+-rw-rw-rw-   0 root         (0) root         (0)     1895 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/account/AccountOrder.py
+-rw-rw-rw-   0 root         (0) root         (0)      367 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/account/Position.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/account/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 02:30:03.281582 fast_tradier_client-1.0.4/fast_tradier/models/market_data/
+-rw-rw-rw-   0 root         (0) root         (0)      647 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/market_data/Hlocv.py
+-rw-rw-rw-   0 root         (0) root         (0)     2311 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/market_data/Quote.py
+-rw-rw-rw-   0 root         (0) root         (0)     1035 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/market_data/TradierQuote.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/market_data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 02:30:03.285582 fast_tradier_client-1.0.4/fast_tradier/models/trading/
+-rw-rw-rw-   0 root         (0) root         (0)      115 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/trading/Duration.py
+-rw-rw-rw-   0 root         (0) root         (0)     2440 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/trading/EquityOrder.py
+-rw-rw-rw-   0 root         (0) root         (0)      169 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/trading/Interval.py
+-rw-rw-rw-   0 root         (0) root         (0)     3265 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/trading/OptionOrder.py
+-rw-rw-rw-   0 root         (0) root         (0)       95 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/trading/OrderBase.py
+-rw-rw-rw-   0 root         (0) root         (0)      330 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/trading/PriceTypes.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/trading/Sides.py
+-rw-rw-rw-   0 root         (0) root         (0)     2385 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/trading/TOSTradierConverter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/trading/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 02:30:03.285582 fast_tradier_client-1.0.4/fast_tradier/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     1284 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/utils/OptionUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/utils/TimeUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2020 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/utils/YFinanceQuoteProvider.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 02:30:03.285582 fast_tradier_client-1.0.4/fast_tradier_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11014 2024-05-11 02:30:03.000000 fast_tradier_client-1.0.4/fast_tradier_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1529 2024-05-11 02:30:03.000000 fast_tradier_client-1.0.4/fast_tradier_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 02:30:03.000000 fast_tradier_client-1.0.4/fast_tradier_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2024-05-11 02:30:03.000000 fast_tradier_client-1.0.4/fast_tradier_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-11 02:30:03.000000 fast_tradier_client-1.0.4/fast_tradier_client.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      907 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-11 02:30:03.285582 fast_tradier_client-1.0.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      473 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/setup.py
```

### Comparing `fast_tradier_client-1.0.3/LICENSE` & `fast_tradier_client-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.3/PKG-INFO` & `fast_tradier_client-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_tradier_client
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Tradier client for trading stocks and options through Tradier API
 Home-page: https://pypi.org/project/fast-tradier-client/
 Author: Tony W
 Author-email: Tony Wang <ivytony@gmail.com>
 Project-URL: Homepage, https://bitbucket.org/rcholic/fast-tradier-client
 Project-URL: Bug Tracker, https://bitbucket.org/rcholic/fast-tradier-client/jira?statuses=new&statuses=indeterminate&sort=-updated&page=1
 Keywords: python,fast-tradier-client,tradier
```

### Comparing `fast_tradier_client-1.0.3/README.md` & `fast_tradier_client-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.3/fast_tradier/FastTradierAsyncClient.py` & `fast_tradier_client-1.0.4/fast_tradier/FastTradierAsyncClient.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.3/fast_tradier/FastTradierClient.py` & `fast_tradier_client-1.0.4/fast_tradier/FastTradierClient.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.3/fast_tradier/interfaces/IBrokerAsyncClient.py` & `fast_tradier_client-1.0.4/fast_tradier/interfaces/IBrokerAsyncClient.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.3/fast_tradier/interfaces/IBrokerClient.py` & `fast_tradier_client-1.0.4/fast_tradier/interfaces/IBrokerClient.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.3/fast_tradier/models/ModelBase.py` & `fast_tradier_client-1.0.4/fast_tradier/models/ModelBase.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.3/fast_tradier/models/account/AccountBalance.py` & `fast_tradier_client-1.0.4/fast_tradier/models/account/AccountBalance.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.3/fast_tradier/models/account/AccountOrder.py` & `fast_tradier_client-1.0.4/fast_tradier/models/account/AccountOrder.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.3/fast_tradier/models/market_data/Hlocv.py` & `fast_tradier_client-1.0.4/fast_tradier/models/market_data/Hlocv.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.3/fast_tradier/models/market_data/Quote.py` & `fast_tradier_client-1.0.4/fast_tradier/models/market_data/Quote.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.3/fast_tradier/models/market_data/TradierQuote.py` & `fast_tradier_client-1.0.4/fast_tradier/models/market_data/TradierQuote.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.3/fast_tradier/models/trading/EquityOrder.py` & `fast_tradier_client-1.0.4/fast_tradier/models/trading/EquityOrder.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.3/fast_tradier/models/trading/OptionOrder.py` & `fast_tradier_client-1.0.4/fast_tradier/models/trading/OptionOrder.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from fast_tradier.models.trading.TOSTradierConverter import TOSTradierConverter
 from fast_tradier.models.ModelBase import ModelBase
 from fast_tradier.models.trading.Sides import OptionOrderSide
 from fast_tradier.models.trading.PriceTypes import OptionPriceType
 from fast_tradier.models.trading.Duration import Duration
 from fast_tradier.models.trading.OrderBase import OrderBase
 from fast_tradier.models.ModelBase import NewModelBase
-from pydantic import BaseModel, ConfigDict
+from pydantic import BaseModel, ConfigDict, Field
 
 class OptionLeg(NewModelBase):
     model_config = ConfigDict(use_enum_values=True)
     underlying_symbol: str
     option_symbol: str
     quantity: int
     side: OptionOrderSide
@@ -19,23 +19,23 @@
     def reverse_side(self) -> None:
         if self.side == OptionOrderSide.SellToOpen or self.side == OptionOrderSide.SellToOpen.value:
             setattr(self, "side", OptionOrderSide.BuyToClose)
         elif self.side == OptionOrderSide.BuyToOpen or self.side == OptionOrderSide.BuyToOpen.value:
             setattr(self, "side", OptionOrderSide.SellToClose)
 
 class OptionOrder(NewModelBase):
-    model_config = ConfigDict(use_enum_values=True)
     ticker: str
     price: float
-    price_type: OptionPriceType
+    price_type: OptionPriceType = Field(..., alias="type")
     duration: Duration
     option_legs: List[OptionLeg]
     status: str = "pending"
-    order_class: str = "multileg" # could be "option"
+    order_class: str = Field("multileg", alias="class") # could be "option"
     id: Optional[int] = None
+    model_config = ConfigDict(use_enum_values=True, populate_by_name=True)
 
     def set_price(self, new_price: float) -> None:
         setattr(self, "price", new_price)
 
     def set_status(self, new_staus: str) -> None:
         setattr(self, "status", new_staus)
 
@@ -58,23 +58,18 @@
     
     def to_json(self) -> Mapping[str, Any]:
         """
         Override to_json so that the format complies to Tradier API.
         Returns:
             Mapping[str, Any]: _description_
         """
-        result: Dict[str, Any] = {
-            "id": self.id,
-            "status": self.status,
-            "symbol": self.ticker,
-            "duration": self.duration,
-            "price": self.price,
-            "type": self.price_type,
-            "class": self.order_class,
-        }
+        temp_result = self.model_dump(by_alias=True)
+        result: Dict[str, Any] = {}
+        for k, v in temp_result.items():
+            result[k] = v
 
         if len(self.option_legs) == 1:
             result["option_symbol"] = self.option_legs[0].option_symbol
             result["side"] = self.option_legs[0].side
             result["quantity"] = self.option_legs[0].quantity
         elif len(self.option_legs) > 1:
             for i in range(len(self.option_legs)):
```

### Comparing `fast_tradier_client-1.0.3/fast_tradier/models/trading/TOSTradierConverter.py` & `fast_tradier_client-1.0.4/fast_tradier/models/trading/TOSTradierConverter.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.3/fast_tradier/utils/OptionUtils.py` & `fast_tradier_client-1.0.4/fast_tradier/utils/OptionUtils.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.3/fast_tradier/utils/TimeUtils.py` & `fast_tradier_client-1.0.4/fast_tradier/utils/TimeUtils.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.3/fast_tradier/utils/YFinanceQuoteProvider.py` & `fast_tradier_client-1.0.4/fast_tradier/utils/YFinanceQuoteProvider.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.3/fast_tradier_client.egg-info/PKG-INFO` & `fast_tradier_client-1.0.4/fast_tradier_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-tradier-client
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Tradier client for trading stocks and options through Tradier API
 Home-page: https://pypi.org/project/fast-tradier-client/
 Author: Tony W
 Author-email: Tony Wang <ivytony@gmail.com>
 Project-URL: Homepage, https://bitbucket.org/rcholic/fast-tradier-client
 Project-URL: Bug Tracker, https://bitbucket.org/rcholic/fast-tradier-client/jira?statuses=new&statuses=indeterminate&sort=-updated&page=1
 Keywords: python,fast-tradier-client,tradier
```

### Comparing `fast_tradier_client-1.0.3/fast_tradier_client.egg-info/SOURCES.txt` & `fast_tradier_client-1.0.4/fast_tradier_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.3/pyproject.toml` & `fast_tradier_client-1.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fast_tradier_client"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Tony Wang", email="ivytony@gmail.com" },
 ]
 description = "A Tradier client for trading stocks and options through Tradier API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

