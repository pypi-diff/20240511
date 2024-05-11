# Comparing `tmp/fast_tradier_client-1.0.4.tar.gz` & `tmp/fast_tradier_client-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_tradier_client-1.0.4.tar", last modified: Sat May 11 02:30:03 2024, max compression
+gzip compressed data, was "fast_tradier_client-1.0.5.tar", last modified: Sat May 11 17:48:31 2024, max compression
```

## Comparing `fast_tradier_client-1.0.4.tar` & `fast_tradier_client-1.0.5.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 02:30:03.285582 fast_tradier_client-1.0.4/
--rw-rw-rw-   0 root         (0) root         (0)     1073 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)    11014 2024-05-11 02:30:03.285582 fast_tradier_client-1.0.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    10270 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 02:30:03.281582 fast_tradier_client-1.0.4/fast_tradier/
--rw-rw-rw-   0 root         (0) root         (0)    16899 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/FastTradierAsyncClient.py
--rw-rw-rw-   0 root         (0) root         (0)    16356 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/FastTradierClient.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 02:30:03.281582 fast_tradier_client-1.0.4/fast_tradier/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)     3237 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/interfaces/IBrokerAsyncClient.py
--rw-rw-rw-   0 root         (0) root         (0)     3063 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/interfaces/IBrokerClient.py
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/interfaces/IModel.py
--rw-rw-rw-   0 root         (0) root         (0)      291 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/interfaces/IRealTimeQuoteProvider.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/interfaces/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 02:30:03.281582 fast_tradier_client-1.0.4/fast_tradier/models/
--rw-rw-rw-   0 root         (0) root         (0)      479 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/DataClassModelBase.py
--rw-rw-rw-   0 root         (0) root         (0)     1471 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/ModelBase.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 02:30:03.281582 fast_tradier_client-1.0.4/fast_tradier/models/account/
--rw-rw-rw-   0 root         (0) root         (0)     1224 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/account/AccountBalance.py
--rw-rw-rw-   0 root         (0) root         (0)     1895 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/account/AccountOrder.py
--rw-rw-rw-   0 root         (0) root         (0)      367 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/account/Position.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/account/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 02:30:03.281582 fast_tradier_client-1.0.4/fast_tradier/models/market_data/
--rw-rw-rw-   0 root         (0) root         (0)      647 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/market_data/Hlocv.py
--rw-rw-rw-   0 root         (0) root         (0)     2311 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/market_data/Quote.py
--rw-rw-rw-   0 root         (0) root         (0)     1035 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/market_data/TradierQuote.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/market_data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 02:30:03.285582 fast_tradier_client-1.0.4/fast_tradier/models/trading/
--rw-rw-rw-   0 root         (0) root         (0)      115 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/trading/Duration.py
--rw-rw-rw-   0 root         (0) root         (0)     2440 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/trading/EquityOrder.py
--rw-rw-rw-   0 root         (0) root         (0)      169 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/trading/Interval.py
--rw-rw-rw-   0 root         (0) root         (0)     3265 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/trading/OptionOrder.py
--rw-rw-rw-   0 root         (0) root         (0)       95 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/trading/OrderBase.py
--rw-rw-rw-   0 root         (0) root         (0)      330 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/trading/PriceTypes.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/trading/Sides.py
--rw-rw-rw-   0 root         (0) root         (0)     2385 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/trading/TOSTradierConverter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/models/trading/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 02:30:03.285582 fast_tradier_client-1.0.4/fast_tradier/utils/
--rw-rw-rw-   0 root         (0) root         (0)     1284 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/utils/OptionUtils.py
--rw-rw-rw-   0 root         (0) root         (0)     1888 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/utils/TimeUtils.py
--rw-rw-rw-   0 root         (0) root         (0)     2020 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/utils/YFinanceQuoteProvider.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/fast_tradier/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 02:30:03.285582 fast_tradier_client-1.0.4/fast_tradier_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11014 2024-05-11 02:30:03.000000 fast_tradier_client-1.0.4/fast_tradier_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1529 2024-05-11 02:30:03.000000 fast_tradier_client-1.0.4/fast_tradier_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 02:30:03.000000 fast_tradier_client-1.0.4/fast_tradier_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2024-05-11 02:30:03.000000 fast_tradier_client-1.0.4/fast_tradier_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-11 02:30:03.000000 fast_tradier_client-1.0.4/fast_tradier_client.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      907 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-11 02:30:03.285582 fast_tradier_client-1.0.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      473 2024-05-11 02:29:34.000000 fast_tradier_client-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 17:48:31.790020 fast_tradier_client-1.0.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    11018 2024-05-11 17:48:31.786020 fast_tradier_client-1.0.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    10274 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 17:48:31.786020 fast_tradier_client-1.0.5/fast_tradier/
+-rw-rw-rw-   0 root         (0) root         (0)    16961 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/fast_tradier/FastTradierAsyncClient.py
+-rw-rw-rw-   0 root         (0) root         (0)    16390 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/fast_tradier/FastTradierClient.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/fast_tradier/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 17:48:31.786020 fast_tradier_client-1.0.5/fast_tradier/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)     3237 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/fast_tradier/interfaces/IBrokerAsyncClient.py
+-rw-rw-rw-   0 root         (0) root         (0)     3063 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/fast_tradier/interfaces/IBrokerClient.py
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/fast_tradier/interfaces/IModel.py
+-rw-rw-rw-   0 root         (0) root         (0)      291 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/fast_tradier/interfaces/IRealTimeQuoteProvider.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/fast_tradier/interfaces/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 17:48:31.786020 fast_tradier_client-1.0.5/fast_tradier/models/
+-rw-rw-rw-   0 root         (0) root         (0)      479 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/fast_tradier/models/DataClassModelBase.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/fast_tradier/models/ModelBase.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/fast_tradier/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 17:48:31.786020 fast_tradier_client-1.0.5/fast_tradier/models/account/
+-rw-rw-rw-   0 root         (0) root         (0)     1224 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/fast_tradier/models/account/AccountBalance.py
+-rw-rw-rw-   0 root         (0) root         (0)     1895 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/fast_tradier/models/account/AccountOrder.py
+-rw-rw-rw-   0 root         (0) root         (0)      367 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/fast_tradier/models/account/Position.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/fast_tradier/models/account/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 17:48:31.786020 fast_tradier_client-1.0.5/fast_tradier/models/market_data/
+-rw-rw-rw-   0 root         (0) root         (0)      554 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/fast_tradier/models/market_data/Hlocv.py
+-rw-rw-rw-   0 root         (0) root         (0)     2246 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/fast_tradier/models/market_data/Quote.py
+-rw-rw-rw-   0 root         (0) root         (0)      942 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/fast_tradier/models/market_data/TradierQuote.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/fast_tradier/models/market_data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 17:48:31.786020 fast_tradier_client-1.0.5/fast_tradier/models/trading/
+-rw-rw-rw-   0 root         (0) root         (0)      115 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/fast_tradier/models/trading/Duration.py
+-rw-rw-rw-   0 root         (0) root         (0)      751 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/fast_tradier/models/trading/EquityOrder.py
+-rw-rw-rw-   0 root         (0) root         (0)      169 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/fast_tradier/models/trading/Interval.py
+-rw-rw-rw-   0 root         (0) root         (0)     3548 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/fast_tradier/models/trading/OptionOrder.py
+-rw-rw-rw-   0 root         (0) root         (0)       94 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/fast_tradier/models/trading/OrderBase.py
+-rw-rw-rw-   0 root         (0) root         (0)      330 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/fast_tradier/models/trading/PriceTypes.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/fast_tradier/models/trading/Sides.py
+-rw-rw-rw-   0 root         (0) root         (0)     2385 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/fast_tradier/models/trading/TOSTradierConverter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/fast_tradier/models/trading/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 17:48:31.786020 fast_tradier_client-1.0.5/fast_tradier/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     1284 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/fast_tradier/utils/OptionUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/fast_tradier/utils/TimeUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2020 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/fast_tradier/utils/YFinanceQuoteProvider.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/fast_tradier/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 17:48:31.786020 fast_tradier_client-1.0.5/fast_tradier_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11018 2024-05-11 17:48:31.000000 fast_tradier_client-1.0.5/fast_tradier_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1529 2024-05-11 17:48:31.000000 fast_tradier_client-1.0.5/fast_tradier_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 17:48:31.000000 fast_tradier_client-1.0.5/fast_tradier_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2024-05-11 17:48:31.000000 fast_tradier_client-1.0.5/fast_tradier_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-11 17:48:31.000000 fast_tradier_client-1.0.5/fast_tradier_client.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      907 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-11 17:48:31.790020 fast_tradier_client-1.0.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      473 2024-05-11 17:48:04.000000 fast_tradier_client-1.0.5/setup.py
```

### Comparing `fast_tradier_client-1.0.4/LICENSE` & `fast_tradier_client-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.4/PKG-INFO` & `fast_tradier_client-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_tradier_client
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Tradier client for trading stocks and options through Tradier API
 Home-page: https://pypi.org/project/fast-tradier-client/
 Author: Tony W
 Author-email: Tony Wang <ivytony@gmail.com>
 Project-URL: Homepage, https://bitbucket.org/rcholic/fast-tradier-client
 Project-URL: Bug Tracker, https://bitbucket.org/rcholic/fast-tradier-client/jira?statuses=new&statuses=indeterminate&sort=-updated&page=1
 Keywords: python,fast-tradier-client,tradier
@@ -42,15 +42,15 @@
     "cost_basis": 207.01,
     "date_acquired": "2018-08-08T14:41:11.405Z",
     "id": 130089,
     "quantity": 1.00000000,
     "symbol": "AAPL"
 }
 
-position = Position(account_position)
+position = Position(**account_position)
 print(position.to_json())
 print(position.symbol)
 print(position.date_acquired)
 print('-------' * 10)
 
 quote1 = {
         "symbol": "VXX190517P00016000",
@@ -85,15 +85,15 @@
         "contract_size": 100,
         "expiration_date": "2019-05-17",
         "expiration_type": "standard",
         "option_type": "put",
         "root_symbol": "VXX"
       }
 
-my_q = Quote(quote1)
+my_q = Quote(**quote1)
 print(my_q.symbol)
 print(my_q.ask_date_datetime)
 ```
 
 2. Test Client:
 ```python
```

### Comparing `fast_tradier_client-1.0.4/README.md` & `fast_tradier_client-1.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "cost_basis": 207.01,
     "date_acquired": "2018-08-08T14:41:11.405Z",
     "id": 130089,
     "quantity": 1.00000000,
     "symbol": "AAPL"
 }
 
-position = Position(account_position)
+position = Position(**account_position)
 print(position.to_json())
 print(position.symbol)
 print(position.date_acquired)
 print('-------' * 10)
 
 quote1 = {
         "symbol": "VXX190517P00016000",
@@ -68,15 +68,15 @@
         "contract_size": 100,
         "expiration_date": "2019-05-17",
         "expiration_type": "standard",
         "option_type": "put",
         "root_symbol": "VXX"
       }
 
-my_q = Quote(quote1)
+my_q = Quote(**quote1)
 print(my_q.symbol)
 print(my_q.ask_date_datetime)
 ```
 
 2. Test Client:
 ```python
```

### Comparing `fast_tradier_client-1.0.4/fast_tradier/FastTradierAsyncClient.py` & `fast_tradier_client-1.0.5/fast_tradier/FastTradierAsyncClient.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,16 @@
     async def get_account_orders_async(self) -> List[AccountOrder]:
         url = f'{self.host_base}accounts/{self.account_id}/orders'
         client = httpx.AsyncClient() if self.__client is None else self.__client
         try:
             retrieved_orders = []
             response = await client.get(url=url, params={'includeTags': 'true'}, headers=self.__auth_headers)
             json_res = response.json()
-            if 'orders' in json_res:
+            print(json_res)
+            if 'orders' in json_res and 'order' in json_res['orders']:
                 order_obj = json_res['orders']['order']
                 if isinstance(order_obj, Dict):
                     retrieved_orders = [AccountOrder(**order_obj)]
                 elif isinstance(order_obj, List):
                     for order_json in order_obj:
                         retrieved_orders.append(AccountOrder(**order_json))
```

### Comparing `fast_tradier_client-1.0.4/fast_tradier/FastTradierClient.py` & `fast_tradier_client-1.0.5/fast_tradier/FastTradierClient.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,15 @@
     def get_account_orders(self) -> List[AccountOrder]:
         url = f'{self.host_base}accounts/{self.account_id}/orders'
         client = httpx.Client() if self.__client is None else self.__client
         try:
             retrieved_orders = []
             response = client.get(url=url, params={'includeTags': 'true'}, headers=self.__auth_headers)
             json_res = response.json()
-            if 'orders' in json_res:
+            if 'orders' in json_res and 'order' in json_res['orders']:
                 order_obj = json_res['orders']['order']
                 if isinstance(order_obj, Dict):
                     retrieved_orders = [AccountOrder(**order_obj)]
                 elif isinstance(order_obj, List):
                     for order_json in order_obj:
                         retrieved_orders.append(AccountOrder(**order_json))
```

### Comparing `fast_tradier_client-1.0.4/fast_tradier/interfaces/IBrokerAsyncClient.py` & `fast_tradier_client-1.0.5/fast_tradier/interfaces/IBrokerAsyncClient.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.4/fast_tradier/interfaces/IBrokerClient.py` & `fast_tradier_client-1.0.5/fast_tradier/interfaces/IBrokerClient.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.4/fast_tradier/models/ModelBase.py` & `fast_tradier_client-1.0.5/fast_tradier/models/ModelBase.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,11 +38,11 @@
 
     @classmethod
     def deserialize_from_json(cls, json_obj) -> Optional[ModelBase]:
         '''Parse json object to class object. Could throw exception if not parsable'''
         return jsonpickle.decode(json_obj)
 
 class NewModelBase(BaseModel):
-    model_config = ConfigDict(use_enum_values=True)
+    model_config = ConfigDict(use_enum_values=True, populate_by_name=True)
     
     def to_json(self) -> Mapping[str, Any]:
-        return self.model_dump()
+        return self.model_dump(by_alias=True)
```

### Comparing `fast_tradier_client-1.0.4/fast_tradier/models/account/AccountBalance.py` & `fast_tradier_client-1.0.5/fast_tradier/models/account/AccountBalance.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.4/fast_tradier/models/account/AccountOrder.py` & `fast_tradier_client-1.0.5/fast_tradier/models/account/AccountOrder.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.4/fast_tradier/models/market_data/Quote.py` & `fast_tradier_client-1.0.5/fast_tradier/models/market_data/Quote.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from fast_tradier.models.ModelBase import NewModelBase
 from fast_tradier.models.DataClassModelBase import DataClassModelBase
 
 class Quote(NewModelBase):
     symbol: str
     description: Optional[str] = None
     exch: Optional[str] = None
-    type: str
+    type_: str = Field(..., alias="type")
     last: Optional[float] = None
     change: Optional[float] = None
     volume: Optional[float] = None
     open_price: Optional[float] = Field(..., alias="open")
     high: Optional[float] = None
     low: Optional[float] = None
     close: Optional[float] = None
@@ -37,19 +37,15 @@
     ask_date: Optional[int] = None
     open_interest: Optional[int] = None
     contract_size: Optional[int] = None
     expiration_date: Optional[str] = None
     expiration_type: Optional[str] = None
     option_type: Optional[str] = None
     root_symbol: Optional[str] = None
-    model_config = ConfigDict(populate_by_name=True)
-
-    def to_json(self) -> Mapping[str, Any]:
-        result = self.model_dump(by_alias=True)
-        return result
+    model_config = ConfigDict(use_enum_values=True, populate_by_name=True)
 
     @property
     def is_option(self) -> bool:
         return self.type.upper() == 'OPTION'
 
     @property
     def is_stock(self) -> bool:
```

### Comparing `fast_tradier_client-1.0.4/fast_tradier/models/market_data/TradierQuote.py` & `fast_tradier_client-1.0.5/fast_tradier/models/market_data/TradierQuote.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,19 +10,15 @@
     high: float
     low: float
     close: float
     volume: float
     bid: Optional[float] = None
     ask: Optional[float] = None
     last_price: Optional[float] = None
-    model_config = ConfigDict(populate_by_name=True)
-
-    def to_json(self) -> Mapping[str, Any]:
-        result = self.model_dump(by_alias=True)
-        return result
+    model_config = ConfigDict(use_enum_values=True, populate_by_name=True)
 
     @property
     def ohlcv(self) -> Tuple:
         return self.open_price, self.high, self.low, self.close, self.volume
 
     @property
     def quote_type(self) -> str:
```

### Comparing `fast_tradier_client-1.0.4/fast_tradier/models/trading/OptionOrder.py` & `fast_tradier_client-1.0.5/fast_tradier/models/trading/OptionOrder.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,37 +6,44 @@
 from fast_tradier.models.trading.PriceTypes import OptionPriceType
 from fast_tradier.models.trading.Duration import Duration
 from fast_tradier.models.trading.OrderBase import OrderBase
 from fast_tradier.models.ModelBase import NewModelBase
 from pydantic import BaseModel, ConfigDict, Field
 
 class OptionLeg(NewModelBase):
-    model_config = ConfigDict(use_enum_values=True)
-    underlying_symbol: str
+    underlying_symbol: Optional[str] = None
     option_symbol: str
     quantity: int
     side: OptionOrderSide
+    model_config = ConfigDict(use_enum_values=True, populate_by_name=True)
     
     def reverse_side(self) -> None:
         if self.side == OptionOrderSide.SellToOpen or self.side == OptionOrderSide.SellToOpen.value:
             setattr(self, "side", OptionOrderSide.BuyToClose)
         elif self.side == OptionOrderSide.BuyToOpen or self.side == OptionOrderSide.BuyToOpen.value:
             setattr(self, "side", OptionOrderSide.SellToClose)
 
 class OptionOrder(NewModelBase):
-    ticker: str
-    price: float
+    symbol: str
+    price: Optional[float] = None
+    stop: Optional[float] = None
     price_type: OptionPriceType = Field(..., alias="type")
     duration: Duration
     option_legs: List[OptionLeg]
-    status: str = "pending"
+    side: Optional[OptionOrderSide] = None # required for single leg option order
+    status: Optional[str] = "pending"
     order_class: str = Field("multileg", alias="class") # could be "option"
     id: Optional[int] = None
+    tag: Optional[str] = None
     model_config = ConfigDict(use_enum_values=True, populate_by_name=True)
 
+    @property
+    def ticker(self) -> str:
+        return self.symbol
+
     def set_price(self, new_price: float) -> None:
         setattr(self, "price", new_price)
 
     def set_status(self, new_staus: str) -> None:
         setattr(self, "status", new_staus)
 
     def set_ticker(self, ticker_name: str) -> None:
```

### Comparing `fast_tradier_client-1.0.4/fast_tradier/models/trading/TOSTradierConverter.py` & `fast_tradier_client-1.0.5/fast_tradier/models/trading/TOSTradierConverter.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.4/fast_tradier/utils/OptionUtils.py` & `fast_tradier_client-1.0.5/fast_tradier/utils/OptionUtils.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.4/fast_tradier/utils/TimeUtils.py` & `fast_tradier_client-1.0.5/fast_tradier/utils/TimeUtils.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.4/fast_tradier/utils/YFinanceQuoteProvider.py` & `fast_tradier_client-1.0.5/fast_tradier/utils/YFinanceQuoteProvider.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.4/fast_tradier_client.egg-info/PKG-INFO` & `fast_tradier_client-1.0.5/fast_tradier_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-tradier-client
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Tradier client for trading stocks and options through Tradier API
 Home-page: https://pypi.org/project/fast-tradier-client/
 Author: Tony W
 Author-email: Tony Wang <ivytony@gmail.com>
 Project-URL: Homepage, https://bitbucket.org/rcholic/fast-tradier-client
 Project-URL: Bug Tracker, https://bitbucket.org/rcholic/fast-tradier-client/jira?statuses=new&statuses=indeterminate&sort=-updated&page=1
 Keywords: python,fast-tradier-client,tradier
@@ -42,15 +42,15 @@
     "cost_basis": 207.01,
     "date_acquired": "2018-08-08T14:41:11.405Z",
     "id": 130089,
     "quantity": 1.00000000,
     "symbol": "AAPL"
 }
 
-position = Position(account_position)
+position = Position(**account_position)
 print(position.to_json())
 print(position.symbol)
 print(position.date_acquired)
 print('-------' * 10)
 
 quote1 = {
         "symbol": "VXX190517P00016000",
@@ -85,15 +85,15 @@
         "contract_size": 100,
         "expiration_date": "2019-05-17",
         "expiration_type": "standard",
         "option_type": "put",
         "root_symbol": "VXX"
       }
 
-my_q = Quote(quote1)
+my_q = Quote(**quote1)
 print(my_q.symbol)
 print(my_q.ask_date_datetime)
 ```
 
 2. Test Client:
 ```python
```

### Comparing `fast_tradier_client-1.0.4/fast_tradier_client.egg-info/SOURCES.txt` & `fast_tradier_client-1.0.5/fast_tradier_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.4/pyproject.toml` & `fast_tradier_client-1.0.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fast_tradier_client"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Tony Wang", email="ivytony@gmail.com" },
 ]
 description = "A Tradier client for trading stocks and options through Tradier API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

