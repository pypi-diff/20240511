# Comparing `tmp/robin_stocks-3.0.6.tar.gz` & `tmp/robin_stocks-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robin_stocks-3.0.6.tar", last modified: Mon Aug  7 02:53:30 2023, max compression
+gzip compressed data, was "robin_stocks-3.1.0.tar", last modified: Sat May 11 01:11:34 2024, max compression
```

## Comparing `robin_stocks-3.0.6.tar` & `robin_stocks-3.1.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-08-07 02:53:30.754207 robin_stocks-3.0.6/
--rw-r--r--   0 josh       (501) staff       (20)     1062 2018-10-17 16:32:18.000000 robin_stocks-3.0.6/LICENSE.txt
--rw-r--r--   0 josh       (501) staff       (20)       88 2018-09-27 04:22:53.000000 robin_stocks-3.0.6/MANIFEST.in
--rw-r--r--   0 josh       (501) staff       (20)     5087 2023-08-07 02:53:30.753597 robin_stocks-3.0.6/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)     4629 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/README.rst
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-08-07 02:53:30.713166 robin_stocks-3.0.6/robin_stocks/
--rw-r--r--   0 josh       (501) staff       (20)       47 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/__init__.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-08-07 02:53:30.724437 robin_stocks-3.0.6/robin_stocks/gemini/
--rw-r--r--   0 josh       (501) staff       (20)      789 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/gemini/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)    12995 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/gemini/account.py
--rw-r--r--   0 josh       (501) staff       (20)     2499 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/gemini/authentication.py
--rw-r--r--   0 josh       (501) staff       (20)    10801 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/gemini/crypto.py
--rw-r--r--   0 josh       (501) staff       (20)      585 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/gemini/globals.py
--rw-r--r--   0 josh       (501) staff       (20)     6140 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/gemini/helper.py
--rw-r--r--   0 josh       (501) staff       (20)    18993 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/gemini/orders.py
--rw-r--r--   0 josh       (501) staff       (20)     3859 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/gemini/urls.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-08-07 02:53:30.735188 robin_stocks-3.0.6/robin_stocks/robinhood/
--rw-r--r--   0 josh       (501) staff       (20)     5064 2023-06-17 04:58:36.000000 robin_stocks-3.0.6/robin_stocks/robinhood/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)    30664 2023-06-17 05:10:20.000000 robin_stocks-3.0.6/robin_stocks/robinhood/account.py
--rw-r--r--   0 josh       (501) staff       (20)     8596 2021-10-20 03:38:49.000000 robin_stocks-3.0.6/robin_stocks/robinhood/authentication.py
--rw-r--r--   0 josh       (501) staff       (20)     9715 2021-05-12 02:09:12.000000 robin_stocks-3.0.6/robin_stocks/robinhood/crypto.py
--rw-r--r--   0 josh       (501) staff       (20)     6602 2023-05-22 00:46:39.000000 robin_stocks-3.0.6/robin_stocks/robinhood/export.py
--rw-r--r--   0 josh       (501) staff       (20)      902 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/robinhood/globals.py
--rw-r--r--   0 josh       (501) staff       (20)    13293 2023-08-07 02:51:23.000000 robin_stocks-3.0.6/robin_stocks/robinhood/helper.py
--rw-r--r--   0 josh       (501) staff       (20)    11649 2021-02-27 17:30:21.000000 robin_stocks-3.0.6/robin_stocks/robinhood/markets.py
--rw-r--r--   0 josh       (501) staff       (20)    20412 2023-06-17 04:58:36.000000 robin_stocks-3.0.6/robin_stocks/robinhood/options.py
--rw-r--r--   0 josh       (501) staff       (20)    65728 2023-08-07 02:51:23.000000 robin_stocks-3.0.6/robin_stocks/robinhood/orders.py
--rw-r--r--   0 josh       (501) staff       (20)     9622 2023-05-22 00:46:39.000000 robin_stocks-3.0.6/robin_stocks/robinhood/profiles.py
--rw-r--r--   0 josh       (501) staff       (20)    25274 2023-07-06 02:38:32.000000 robin_stocks-3.0.6/robin_stocks/robinhood/stocks.py
--rw-r--r--   0 josh       (501) staff       (20)     7682 2023-07-06 02:38:32.000000 robin_stocks-3.0.6/robin_stocks/robinhood/urls.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-08-07 02:53:30.746057 robin_stocks-3.0.6/robin_stocks/tda/
--rw-r--r--   0 josh       (501) staff       (20)      713 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/tda/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)     4761 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/tda/accounts.py
--rw-r--r--   0 josh       (501) staff       (20)     6608 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/tda/authentication.py
--rw-r--r--   0 josh       (501) staff       (20)      753 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/tda/globals.py
--rw-r--r--   0 josh       (501) staff       (20)     9765 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/tda/helper.py
--rw-r--r--   0 josh       (501) staff       (20)     3433 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/tda/markets.py
--rw-r--r--   0 josh       (501) staff       (20)     4714 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/tda/orders.py
--rw-r--r--   0 josh       (501) staff       (20)    12030 2021-02-20 06:33:23.000000 robin_stocks-3.0.6/robin_stocks/tda/stocks.py
--rw-r--r--   0 josh       (501) staff       (20)     3161 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/tda/urls.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-08-07 02:53:30.718209 robin_stocks-3.0.6/robin_stocks.egg-info/
--rw-r--r--   0 josh       (501) staff       (20)     5087 2023-08-07 02:53:30.000000 robin_stocks-3.0.6/robin_stocks.egg-info/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)     1330 2023-08-07 02:53:30.000000 robin_stocks-3.0.6/robin_stocks.egg-info/SOURCES.txt
--rw-r--r--   0 josh       (501) staff       (20)        1 2023-08-07 02:53:30.000000 robin_stocks-3.0.6/robin_stocks.egg-info/dependency_links.txt
--rw-r--r--   0 josh       (501) staff       (20)        1 2018-02-23 03:52:33.000000 robin_stocks-3.0.6/robin_stocks.egg-info/not-zip-safe
--rw-r--r--   0 josh       (501) staff       (20)       42 2023-08-07 02:53:30.000000 robin_stocks-3.0.6/robin_stocks.egg-info/requires.txt
--rw-r--r--   0 josh       (501) staff       (20)       19 2023-08-07 02:53:30.000000 robin_stocks-3.0.6/robin_stocks.egg-info/top_level.txt
--rw-r--r--   0 josh       (501) staff       (20)       38 2023-08-07 02:53:30.754360 robin_stocks-3.0.6/setup.cfg
--rw-r--r--   0 josh       (501) staff       (20)      931 2023-08-07 02:52:29.000000 robin_stocks-3.0.6/setup.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-08-07 02:53:30.752811 robin_stocks-3.0.6/tests/
--rw-r--r--   0 josh       (501) staff       (20)        0 2020-06-15 04:00:04.000000 robin_stocks-3.0.6/tests/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)     9843 2023-05-22 02:31:15.000000 robin_stocks-3.0.6/tests/app_tests.py
--rw-r--r--   0 josh       (501) staff       (20)     2157 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/tests/test_gemini.py
--rw-r--r--   0 josh       (501) staff       (20)    32945 2023-07-06 02:51:59.000000 robin_stocks-3.0.6/tests/test_robinhood.py
--rw-r--r--   0 josh       (501) staff       (20)      571 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/tests/test_tda.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-05-11 01:11:34.366855 robin_stocks-3.1.0/
+-rw-r--r--   0 josh       (501) staff       (20)     1062 2018-10-17 16:32:18.000000 robin_stocks-3.1.0/LICENSE.txt
+-rw-r--r--   0 josh       (501) staff       (20)       88 2018-09-27 04:22:53.000000 robin_stocks-3.1.0/MANIFEST.in
+-rw-r--r--   0 josh       (501) staff       (20)     5087 2024-05-11 01:11:34.366170 robin_stocks-3.1.0/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)     4629 2021-02-20 06:32:12.000000 robin_stocks-3.1.0/README.rst
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-05-11 01:11:34.322820 robin_stocks-3.1.0/robin_stocks/
+-rw-r--r--   0 josh       (501) staff       (20)       47 2021-02-20 06:32:12.000000 robin_stocks-3.1.0/robin_stocks/__init__.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-05-11 01:11:34.334282 robin_stocks-3.1.0/robin_stocks/gemini/
+-rw-r--r--   0 josh       (501) staff       (20)      789 2021-02-20 06:32:12.000000 robin_stocks-3.1.0/robin_stocks/gemini/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)    12995 2021-02-20 06:32:12.000000 robin_stocks-3.1.0/robin_stocks/gemini/account.py
+-rw-r--r--   0 josh       (501) staff       (20)     2499 2021-02-20 06:32:12.000000 robin_stocks-3.1.0/robin_stocks/gemini/authentication.py
+-rw-r--r--   0 josh       (501) staff       (20)    10801 2021-02-20 06:32:12.000000 robin_stocks-3.1.0/robin_stocks/gemini/crypto.py
+-rw-r--r--   0 josh       (501) staff       (20)      585 2021-02-20 06:32:12.000000 robin_stocks-3.1.0/robin_stocks/gemini/globals.py
+-rw-r--r--   0 josh       (501) staff       (20)     6140 2021-02-20 06:32:12.000000 robin_stocks-3.1.0/robin_stocks/gemini/helper.py
+-rw-r--r--   0 josh       (501) staff       (20)    18993 2021-02-20 06:32:12.000000 robin_stocks-3.1.0/robin_stocks/gemini/orders.py
+-rw-r--r--   0 josh       (501) staff       (20)     3859 2021-02-20 06:32:12.000000 robin_stocks-3.1.0/robin_stocks/gemini/urls.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-05-11 01:11:34.348097 robin_stocks-3.1.0/robin_stocks/robinhood/
+-rw-r--r--   0 josh       (501) staff       (20)     5064 2023-06-17 04:58:36.000000 robin_stocks-3.1.0/robin_stocks/robinhood/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)    30746 2024-05-11 01:09:34.000000 robin_stocks-3.1.0/robin_stocks/robinhood/account.py
+-rw-r--r--   0 josh       (501) staff       (20)     8596 2021-10-20 03:38:49.000000 robin_stocks-3.1.0/robin_stocks/robinhood/authentication.py
+-rw-r--r--   0 josh       (501) staff       (20)     9715 2021-05-12 02:09:12.000000 robin_stocks-3.1.0/robin_stocks/robinhood/crypto.py
+-rw-r--r--   0 josh       (501) staff       (20)     6602 2023-05-22 00:46:39.000000 robin_stocks-3.1.0/robin_stocks/robinhood/export.py
+-rw-r--r--   0 josh       (501) staff       (20)      902 2024-05-11 01:09:34.000000 robin_stocks-3.1.0/robin_stocks/robinhood/globals.py
+-rw-r--r--   0 josh       (501) staff       (20)    13293 2023-08-07 02:51:23.000000 robin_stocks-3.1.0/robin_stocks/robinhood/helper.py
+-rw-r--r--   0 josh       (501) staff       (20)    11649 2021-02-27 17:30:21.000000 robin_stocks-3.1.0/robin_stocks/robinhood/markets.py
+-rw-r--r--   0 josh       (501) staff       (20)    20562 2024-05-11 01:09:34.000000 robin_stocks-3.1.0/robin_stocks/robinhood/options.py
+-rw-r--r--   0 josh       (501) staff       (20)    66194 2024-05-11 01:09:34.000000 robin_stocks-3.1.0/robin_stocks/robinhood/orders.py
+-rw-r--r--   0 josh       (501) staff       (20)    10075 2024-05-11 01:09:34.000000 robin_stocks-3.1.0/robin_stocks/robinhood/profiles.py
+-rw-r--r--   0 josh       (501) staff       (20)    25274 2023-07-06 02:38:32.000000 robin_stocks-3.1.0/robin_stocks/robinhood/stocks.py
+-rw-r--r--   0 josh       (501) staff       (20)     7994 2024-05-11 01:09:34.000000 robin_stocks-3.1.0/robin_stocks/robinhood/urls.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-05-11 01:11:34.357829 robin_stocks-3.1.0/robin_stocks/tda/
+-rw-r--r--   0 josh       (501) staff       (20)      713 2021-02-20 06:32:12.000000 robin_stocks-3.1.0/robin_stocks/tda/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)     4761 2021-02-20 06:32:12.000000 robin_stocks-3.1.0/robin_stocks/tda/accounts.py
+-rw-r--r--   0 josh       (501) staff       (20)     6608 2021-02-20 06:32:12.000000 robin_stocks-3.1.0/robin_stocks/tda/authentication.py
+-rw-r--r--   0 josh       (501) staff       (20)      753 2021-02-20 06:32:12.000000 robin_stocks-3.1.0/robin_stocks/tda/globals.py
+-rw-r--r--   0 josh       (501) staff       (20)     9765 2021-02-20 06:32:12.000000 robin_stocks-3.1.0/robin_stocks/tda/helper.py
+-rw-r--r--   0 josh       (501) staff       (20)     3433 2021-02-20 06:32:12.000000 robin_stocks-3.1.0/robin_stocks/tda/markets.py
+-rw-r--r--   0 josh       (501) staff       (20)     4714 2021-02-20 06:32:12.000000 robin_stocks-3.1.0/robin_stocks/tda/orders.py
+-rw-r--r--   0 josh       (501) staff       (20)    12030 2021-02-20 06:33:23.000000 robin_stocks-3.1.0/robin_stocks/tda/stocks.py
+-rw-r--r--   0 josh       (501) staff       (20)     3161 2021-02-20 06:32:12.000000 robin_stocks-3.1.0/robin_stocks/tda/urls.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-05-11 01:11:34.326026 robin_stocks-3.1.0/robin_stocks.egg-info/
+-rw-r--r--   0 josh       (501) staff       (20)     5087 2024-05-11 01:11:34.000000 robin_stocks-3.1.0/robin_stocks.egg-info/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)     1330 2024-05-11 01:11:34.000000 robin_stocks-3.1.0/robin_stocks.egg-info/SOURCES.txt
+-rw-r--r--   0 josh       (501) staff       (20)        1 2024-05-11 01:11:34.000000 robin_stocks-3.1.0/robin_stocks.egg-info/dependency_links.txt
+-rw-r--r--   0 josh       (501) staff       (20)        1 2018-02-23 03:52:33.000000 robin_stocks-3.1.0/robin_stocks.egg-info/not-zip-safe
+-rw-r--r--   0 josh       (501) staff       (20)       42 2024-05-11 01:11:34.000000 robin_stocks-3.1.0/robin_stocks.egg-info/requires.txt
+-rw-r--r--   0 josh       (501) staff       (20)       19 2024-05-11 01:11:34.000000 robin_stocks-3.1.0/robin_stocks.egg-info/top_level.txt
+-rw-r--r--   0 josh       (501) staff       (20)       38 2024-05-11 01:11:34.367870 robin_stocks-3.1.0/setup.cfg
+-rw-r--r--   0 josh       (501) staff       (20)      931 2024-05-11 01:10:13.000000 robin_stocks-3.1.0/setup.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-05-11 01:11:34.364744 robin_stocks-3.1.0/tests/
+-rw-r--r--   0 josh       (501) staff       (20)        0 2020-06-15 04:00:04.000000 robin_stocks-3.1.0/tests/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)     9843 2023-05-22 02:31:15.000000 robin_stocks-3.1.0/tests/app_tests.py
+-rw-r--r--   0 josh       (501) staff       (20)     2157 2021-02-20 06:32:12.000000 robin_stocks-3.1.0/tests/test_gemini.py
+-rw-r--r--   0 josh       (501) staff       (20)    32945 2023-07-06 02:51:59.000000 robin_stocks-3.1.0/tests/test_robinhood.py
+-rw-r--r--   0 josh       (501) staff       (20)      571 2021-02-20 06:32:12.000000 robin_stocks-3.1.0/tests/test_tda.py
```

### Comparing `robin_stocks-3.0.6/LICENSE.txt` & `robin_stocks-3.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.6/PKG-INFO` & `robin_stocks-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robin_stocks
-Version: 3.0.6
+Version: 3.1.0
 Summary: A Python wrapper around the Robinhood API
 Home-page: https://github.com/jmfernandes/robin_stocks
 Author: Josh Fernandes
 Author-email: joshfernandes@mac.com
 License: MIT
 Keywords: robinhood,robin stocks,finance app,stocks,options,trading,investing
 Requires: requests
```

### Comparing `robin_stocks-3.0.6/README.rst` & `robin_stocks-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.6/robin_stocks/gemini/__init__.py` & `robin_stocks-3.1.0/robin_stocks/gemini/__init__.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.6/robin_stocks/gemini/account.py` & `robin_stocks-3.1.0/robin_stocks/gemini/account.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.6/robin_stocks/gemini/authentication.py` & `robin_stocks-3.1.0/robin_stocks/gemini/authentication.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.6/robin_stocks/gemini/crypto.py` & `robin_stocks-3.1.0/robin_stocks/gemini/crypto.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.6/robin_stocks/gemini/globals.py` & `robin_stocks-3.1.0/robin_stocks/gemini/globals.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.6/robin_stocks/gemini/helper.py` & `robin_stocks-3.1.0/robin_stocks/gemini/helper.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.6/robin_stocks/gemini/orders.py` & `robin_stocks-3.1.0/robin_stocks/gemini/orders.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.6/robin_stocks/gemini/urls.py` & `robin_stocks-3.1.0/robin_stocks/gemini/urls.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.6/robin_stocks/robinhood/__init__.py` & `robin_stocks-3.1.0/robin_stocks/robinhood/__init__.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.6/robin_stocks/robinhood/account.py` & `robin_stocks-3.1.0/robin_stocks/robinhood/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -807,30 +807,29 @@
         except:
             pass
 
     return(holdings)
 
 
 @login_required
-def build_user_profile():
+def build_user_profile(account_number=None):
     """Builds a dictionary of important information regarding the user account.
 
     :returns: Returns a dictionary that has total equity, extended hours equity, cash, and divendend total.
 
     """
     user = {}
 
-    portfolios_data = load_portfolio_profile()
-    accounts_data = load_account_profile()
+    portfolios_data = load_portfolio_profile(account_number=account_number)
+    accounts_data = load_account_profile(account_number=account_number)
 
     if portfolios_data:
         user['equity'] = portfolios_data['equity']
         user['extended_hours_equity'] = portfolios_data['extended_hours_equity']
 
     if accounts_data:
-        cash = "{0:.2f}".format(
-            float(accounts_data['cash']) + float(accounts_data['uncleared_deposits']))
+        cash = "{0:.2f}".format(float(accounts_data['portfolio_cash'])) # float(accounts_data['cash']) + uncleared_deposits 
         user['cash'] = cash
 
     user['dividend_total'] = get_total_dividends()
 
     return(user)
```

### Comparing `robin_stocks-3.0.6/robin_stocks/robinhood/authentication.py` & `robin_stocks-3.1.0/robin_stocks/robinhood/authentication.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.6/robin_stocks/robinhood/crypto.py` & `robin_stocks-3.1.0/robin_stocks/robinhood/crypto.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.6/robin_stocks/robinhood/export.py` & `robin_stocks-3.1.0/robin_stocks/robinhood/export.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.6/robin_stocks/robinhood/globals.py` & `robin_stocks-3.1.0/robin_stocks/robinhood/globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # The session object for making get and post requests.
 SESSION = Session()
 SESSION.headers = {
     "Accept": "*/*",
     "Accept-Encoding": "gzip,deflate,br",
     "Accept-Language": "en-US,en;q=1",
     "Content-Type": "application/x-www-form-urlencoded; charset=utf-8",
-    "X-Robinhood-API-Version": "1.315.0",
+    "X-Robinhood-API-Version": "1.431.4",
     "Connection": "keep-alive",
     "User-Agent": "*"
 }
 
 #All print() statement direct their output to this stream
 #by default, we use stdout which is the existing behavior
 #but a client can change to any normal Python stream that
```

### Comparing `robin_stocks-3.0.6/robin_stocks/robinhood/helper.py` & `robin_stocks-3.1.0/robin_stocks/robinhood/helper.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.6/robin_stocks/robinhood/markets.py` & `robin_stocks-3.1.0/robin_stocks/robinhood/markets.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.6/robin_stocks/robinhood/options.py` & `robin_stocks-3.1.0/robin_stocks/robinhood/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,38 +17,38 @@
         marketString = 'Loading Market Data '
         sys.stdout.write(marketString)
         sys.stdout.write(next(spinner))
         sys.stdout.flush()
         sys.stdout.write('\b'*(len(marketString)+1))
 
 @login_required
-def get_aggregate_positions(info=None):
+def get_aggregate_positions(info=None, account_number=None):
     """Collapses all option orders for a stock into a single dictionary.
 
     :param info: Will filter the results to get a specific value.
     :type info: Optional[str]
     :returns: Returns a list of dictionaries of key/value pairs for each order. If info parameter is provided, \
     a list of strings is returned where the strings are the value of the key that matches info.
 
     """
-    url = aggregate_url()
+    url = aggregate_url(account_number=account_number)
     data = request_get(url, 'pagination')
     return(filter_data(data, info))
 
 @login_required
-def get_aggregate_open_positions(info=None):
+def get_aggregate_open_positions(info=None, account_number=None):
     """Collapses all open option positions for a stock into a single dictionary.
 
     :param info: Will filter the results to get a specific value.
     :type info: Optional[str]
     :returns: Returns a list of dictionaries of key/value pairs for each order. If info parameter is provided, \
     a list of strings is returned where the strings are the value of the key that matches info.
 
     """
-    url = aggregate_url()
+    url = aggregate_url(account_number=account_number)
     payload = {'nonzero': 'True'}
     data = request_get(url, 'pagination', payload)
     return(filter_data(data, info))
 
 
 @login_required
 def get_market_options(info=None):
@@ -63,24 +63,24 @@
     url = option_orders_url()
     data = request_get(url, 'pagination')
 
     return(filter_data(data, info))
 
 
 @login_required
-def get_all_option_positions(info=None):
+def get_all_option_positions(info=None, account_number=None):
     """Returns all option positions ever held for the account.
 
     :param info: Will filter the results to get a specific value.
     :type info: Optional[str]
     :returns: Returns a list of dictionaries of key/value pairs for each option. If info parameter is provided, \
     a list of strings is returned where the strings are the value of the key that matches info.
 
     """
-    url = option_positions_url()
+    url = option_positions_url(account_number=account_number)
     data = request_get(url, 'pagination')
     return(filter_data(data, info))
 
 
 @login_required
 def get_open_option_positions(account_number=None, info=None):
     """Returns all open option positions for the account.
```

### Comparing `robin_stocks-3.0.6/robin_stocks/robinhood/orders.py` & `robin_stocks-3.1.0/robin_stocks/robinhood/orders.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,15 +316,15 @@
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the purchase of stocks, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
 
     """ 
-    return order(symbol, quantity, "buy", account_number, None, None, timeInForce, extendedHours, jsonify)
+    return order(symbol, quantity, "buy", None, None, account_number, timeInForce, extendedHours, jsonify)
 
 
 @login_required
 def order_buy_fractional_by_quantity(symbol, quantity, account_number=None, timeInForce='gfd', extendedHours=False, jsonify=True):
     """Submits a market order to be executed immediately for fractional shares by specifying the amount that you want to trade.
     Good for share fractions up to 6 decimal places. Robinhood does not currently support placing limit, stop, or stop loss orders
     for fractional trades.
@@ -342,15 +342,15 @@
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the purchase of stocks, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
 
     """ 
-    return order(symbol, quantity, "buy", account_number, None, None, timeInForce, extendedHours, jsonify)
+    return order(symbol, quantity, "buy", None, None, account_number, timeInForce, extendedHours, jsonify)
 
 
 @login_required
 def order_buy_fractional_by_price(symbol, amountInDollars, account_number=None, timeInForce='gfd', extendedHours=False, jsonify=True, market_hours='regular_hours'):
     """Submits a market order to be executed immediately for fractional shares by specifying the amount in dollars that you want to trade.
     Good for share fractions up to 6 decimal places. Robinhood does not currently support placing limit, stop, or stop loss orders
     for fractional trades.
@@ -376,15 +376,15 @@
         print("ERROR: Fractional share price should meet minimum 1.00.", file=get_output())
         return None
 
     # turn the money amount into decimal number of shares
     price = next(iter(get_latest_price(symbol, 'ask_price', extendedHours)), 0.00)
     fractional_shares = 0 if (price == 0.00) else round_price(amountInDollars/float(price))
     
-    return order(symbol, fractional_shares, "buy", None, None, account_number,  timeInForce, extendedHours, jsonify, market_hours)
+    return order(symbol, fractional_shares, "buy", None, None, account_number, timeInForce, extendedHours, jsonify, market_hours)
 
 
 @login_required
 def order_buy_limit(symbol, quantity, limitPrice, account_number=None, timeInForce='gtc', extendedHours=False, jsonify=True):
     """Submits a limit order to be executed once a certain price is reached.
 
     :param symbol: The stock ticker of the stock to purchase.
@@ -403,15 +403,15 @@
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the purchase of stocks, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
 
     """ 
-    return order(symbol, quantity, "buy", account_number, limitPrice, None, timeInForce, extendedHours, jsonify)
+    return order(symbol, quantity, "buy", limitPrice, None, account_number, timeInForce, extendedHours, jsonify)
 
 
 @login_required
 def order_buy_stop_loss(symbol, quantity, stopPrice, account_number=None, timeInForce='gtc', extendedHours=False, jsonify=True):
     """Submits a stop order to be turned into a market order once a certain stop price is reached.
 
     :param symbol: The stock ticker of the stock to purchase.
@@ -430,15 +430,15 @@
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the purchase of stocks, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
 
     """ 
-    return order(symbol, quantity, "buy", account_number, None, stopPrice, timeInForce, extendedHours, jsonify)
+    return order(symbol, quantity, "buy", None, stopPrice, account_number, timeInForce, extendedHours, jsonify)
 
 
 @login_required
 def order_buy_stop_limit(symbol, quantity, limitPrice, stopPrice, account_number=None, timeInForce='gtc', extendedHours=False, jsonify=True):
     """Submits a stop order to be turned into a limit order once a certain stop price is reached.
 
     :param symbol: The stock ticker of the stock to purchase.
@@ -459,15 +459,15 @@
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the purchase of stocks, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
 
     """ 
-    return order(symbol, quantity, "buy", account_number, limitPrice, stopPrice, timeInForce, extendedHours, jsonify)
+    return order(symbol, quantity, "buy", limitPrice, stopPrice, account_number, timeInForce, extendedHours, jsonify)
 
 
 @login_required
 def order_buy_trailing_stop(symbol, quantity, trailAmount, trailType='percentage', timeInForce='gtc', extendedHours=False, jsonify=True):
     """Submits a trailing stop buy order to be turned into a market order when traling stop price reached.
 
     :param symbol: The stock ticker of the stock to buy.
@@ -489,15 +489,15 @@
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
 
     :returns: Dictionary that contains information regarding the purchase of stocks, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
     """
-    return order_trailing_stop(symbol, quantity, "buy", trailAmount, trailType, timeInForce, extendedHours, jsonify)
+    return order_trailing_stop(symbol, quantity, "buy", trailAmount, trailType, None, timeInForce, extendedHours, jsonify)
 
 
 @login_required
 def order_sell_market(symbol, quantity, account_number=None, timeInForce='gtc', extendedHours=False, jsonify=True):
     """Submits a market order to be executed immediately.
 
     :param symbol: The stock ticker of the stock to sell.
@@ -514,15 +514,15 @@
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the selling of stocks, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
 
     """ 
-    return order(symbol, quantity, "sell", account_number, None, None, timeInForce, extendedHours, jsonify)
+    return order(symbol, quantity, "sell", None, None, account_number, timeInForce, extendedHours, jsonify)
 
 
 @login_required
 def order_sell_fractional_by_quantity(symbol, quantity, account_number=None, timeInForce='gfd', priceType='bid_price', extendedHours=False, jsonify=True, market_hours='regular_hours'):
     """Submits a market order to be executed immediately for fractional shares by specifying the amount that you want to trade.
     Good for share fractions up to 6 decimal places. Robinhood does not currently support placing limit, stop, or stop loss orders
     for fractional trades.
@@ -540,15 +540,15 @@
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the purchase of stocks, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
 
     """ 
-    return order(symbol, quantity, "sell", None, None, account_number,  timeInForce, extendedHours, jsonify, market_hours)
+    return order(symbol, quantity, "sell", None, None, account_number, timeInForce, extendedHours, jsonify, market_hours)
 
 
 @login_required
 def order_sell_fractional_by_price(symbol, amountInDollars, account_number=None, timeInForce='gfd', extendedHours=False, jsonify=True):
     """Submits a market order to be executed immediately for fractional shares by specifying the amount in dollars that you want to trade.
     Good for share fractions up to 6 decimal places. Robinhood does not currently support placing limit, stop, or stop loss orders
     for fractional trades.
@@ -573,15 +573,15 @@
     if amountInDollars < 1:
         print("ERROR: Fractional share price should meet minimum 1.00.", file=get_output())
         return None
     # turn the money amount into decimal number of shares
     price = next(iter(get_latest_price(symbol, 'bid_price', extendedHours)), 0.00)
     fractional_shares = 0 if (price == 0.00) else round_price(amountInDollars/float(price))
 
-    return order(symbol, fractional_shares, "sell", account_number, None, None, timeInForce, extendedHours, jsonify)
+    return order(symbol, fractional_shares, "sell", None, None, account_number, timeInForce, extendedHours, jsonify)
 
 
 @login_required
 def order_sell_limit(symbol, quantity, limitPrice, account_number=None, timeInForce='gtc', extendedHours=False, jsonify=True):
     """Submits a limit order to be executed once a certain price is reached.
 
     :param symbol: The stock ticker of the stock to sell.
@@ -600,15 +600,15 @@
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the selling of stocks, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
 
     """ 
-    return order(symbol, quantity, "sell", account_number, limitPrice, None, timeInForce, extendedHours, jsonify)
+    return order(symbol, quantity, "sell", limitPrice, None, account_number, timeInForce, extendedHours, jsonify)
 
 
 @login_required
 def order_sell_stop_loss(symbol, quantity, stopPrice, account_number=None, timeInForce='gtc', extendedHours=False, jsonify=True):
     """Submits a stop order to be turned into a market order once a certain stop price is reached.
 
     :param symbol: The stock ticker of the stock to sell.
@@ -627,15 +627,15 @@
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the selling of stocks, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
 
     """ 
-    return order(symbol, quantity, "sell", account_number, None, stopPrice, timeInForce, extendedHours, jsonify)
+    return order(symbol, quantity, "sell", None, stopPrice, account_number, timeInForce, extendedHours, jsonify)
 
 
 @login_required
 def order_sell_stop_limit(symbol, quantity, limitPrice, stopPrice, account_number=None, timeInForce='gtc', extendedHours=False, jsonify=True):
     """Submits a stop order to be turned into a limit order once a certain stop price is reached.
 
     :param symbol: The stock ticker of the stock to sell.
@@ -656,15 +656,15 @@
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the selling of stocks, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
 
     """ 
-    return order(symbol, quantity, "sell", account_number, limitPrice, stopPrice, timeInForce, extendedHours, jsonify)
+    return order(symbol, quantity, "sell", limitPrice, stopPrice, account_number, timeInForce, extendedHours, jsonify)
 
 
 @login_required
 def order_sell_trailing_stop(symbol, quantity, trailAmount, trailType='percentage', timeInForce='gtc', extendedHours=False, jsonify=True):
     """Submits a trailing stop sell order to be turned into a market order when traling stop price reached.
 
     :param symbol: The stock ticker of the stock to sell.
@@ -686,15 +686,15 @@
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
 
     :returns: Dictionary that contains information regarding the purchase of stocks, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
     """
-    return order_trailing_stop(symbol, quantity, "sell", trailAmount, trailType, timeInForce, extendedHours, jsonify)
+    return order_trailing_stop(symbol, quantity, "sell", trailAmount, trailType, None, timeInForce, extendedHours, jsonify)
 
 
 @login_required
 def order_trailing_stop(symbol, quantity, side, trailAmount, trailType='percentage', account_number=None, timeInForce='gtc', extendedHours=False, jsonify=True):
     """Submits a trailing stop order to be turned into a market order when traling stop price reached.
 
     :param symbol: The stock ticker of the stock to trade.
@@ -829,48 +829,55 @@
         if side == "buy":
             price = stopPrice
         else:
             price = None
         trigger = "stop"
     else:
         price = round_price(next(iter(get_latest_price(symbol, priceType, extendedHours)), 0.00))
+        
+    from datetime import datetime
     payload = {
         'account': load_account_profile(account_number=account_number, info='url'),
         'instrument': get_instruments_by_symbols(symbol, info='url')[0],
         'symbol': symbol,
         'price': price,
+        'ask_price': round_price(next(iter(get_latest_price(symbol, "ask_price", extendedHours)), 0.00)),
+        'bid_ask_timestamp': datetime.now().strftime('%Y-%m-%d %H:%M:%S.%f'),
+        'bid_price': round_price(next(iter(get_latest_price(symbol, "bid_price", extendedHours)), 0.00)),
         'quantity': quantity,
         'ref_id': str(uuid4()),
         'type': orderType,
         'stop_price': stopPrice,
         'time_in_force': timeInForce,
         'trigger': trigger,
         'side': side,
         'market_hours': market_hours, # choices are ['regular_hours', 'all_day_hours']
         'extended_hours': extendedHours,
         'order_form_version': 4
     }
     # adjust market orders
     if orderType == 'market':
         del payload['stop_price']
-        del payload['extended_hours'] 
+        # if market_hours == 'regular_hours': 
+        #     del payload['extended_hours'] 
         
     if market_hours == 'regular_hours':
         if side == "buy":
             payload['preset_percent_limit'] = "0.05"
             payload['type'] = 'limit' 
         # regular market sell
         elif orderType == 'market' and side == 'sell':
             del payload['price']   
     elif market_hours == 'all_day_hours': 
+       
         payload['type'] = 'limit' 
         payload['quantity']=int(payload['quantity']) # round to integer instead of fractional
         
     url = orders_url()
-
+    # print(payload)
     data = request_post(url, payload, jsonify_data=jsonify)
 
     return(data)
 
 
 @login_required
 def order_option_credit_spread(price, symbol, quantity, spread, timeInForce='gtc', account_number=None, jsonify=True):
@@ -897,15 +904,15 @@
     :type account_number: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the trading of options, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
     """
-    return(order_option_spread("credit", price, symbol, quantity, spread, account_number, timeInForce, jsonify))
+    return(order_option_spread("credit", price, symbol, quantity, spread, timeInForce, account_number, jsonify))
 
 
 @login_required
 def order_option_debit_spread(price, symbol, quantity, spread, timeInForce='gtc', account_number=None, jsonify=True):
     """Submits a limit order for an option debit spread.
 
     :param price: The limit price to trigger a sell of the option.
@@ -929,15 +936,15 @@
     :type account_number: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the trading of options, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
     """
-    return(order_option_spread("debit", price, symbol, quantity, spread, account_number, timeInForce, jsonify))
+    return(order_option_spread("debit", price, symbol, quantity, spread, timeInForce, account_number, jsonify))
 
 
 @login_required
 def order_option_spread(direction, price, symbol, quantity, spread, account_number=None, timeInForce='gtc', jsonify=True):
     """Submits a limit order for an option spread. i.e. place a debit / credit spread
 
     :param direction: Can be "credit" or "debit".
@@ -976,15 +983,15 @@
     for each in spread:
         optionID = id_for_option(symbol,
                                         each['expirationDate'],
                                         each['strike'],
                                         each['optionType'])
         legs.append({'position_effect': each['effect'],
                      'side': each['action'],
-                     'ratio_quantity': 1,
+                     'ratio_quantity': each['ratio_quantity'],
                      'option': option_instruments_url(optionID)})
 
     payload = {
         'account': load_account_profile(account_number=account_number, info='url'),
         'direction': direction,
         'time_in_force': timeInForce,
         'legs': legs,
@@ -1057,14 +1064,15 @@
         'quantity': quantity,
         'override_day_trade_checks': False,
         'override_dtbp_checks': False,
         'ref_id': str(uuid4()),
     }
 
     url = option_orders_url()
+    # print(payload)
     data = request_post(url, payload, json=True, jsonify_data=jsonify)
 
     return(data)
 
 
 @login_required
 def order_buy_option_stop_limit(positionEffect, creditOrDebit, limitPrice, stopPrice, symbol, quantity, expirationDate, strike, optionType='both', account_number=None, timeInForce='gtc', jsonify=True):
```

### Comparing `robin_stocks-3.0.6/robin_stocks/robinhood/profiles.py` & `robin_stocks-3.1.0/robin_stocks/robinhood/profiles.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 """Contains functions for getting all the information tied to a user account."""
 from robin_stocks.robinhood.helper import *
 from robin_stocks.robinhood.urls import *
 
 
 @login_required
-def load_account_profile(account_number=None, info=None):
+def load_account_profile(account_number=None, info=None, dataType="indexzero"):
     """Gets the information associated with the accounts profile,including day
     trading information and cash being held by Robinhood.
 
     :param acccount_number: the robinhood account number.
     :type acccount_number: Optional[str]
     :param info: The name of the key whose value is to be returned from the function.
     :type info: Optional[str]
+    :param dataType: Determines how to filter the data. 'regular' returns the unfiltered data. \
+    'results' will return data['results']. 'pagination' will return data['results'] and append it with any \
+    data that is in data['next']. 'indexzero' will return data['results'][0].
+    :type dataType: Optional[str]
     :returns: The function returns a dictionary of key/value pairs. \
     If a string is passed in to the info parameter, then the function will return \
     a string corresponding to the value of the key whose name matches the info parameter.
     :Dictionary Keys: * url
                       * portfolio_cash
                       * can_downgrade_to_cash
                       * user
@@ -61,15 +65,15 @@
                       * rhs_stock_loan_consent_status
 
     """
     url = account_profile_url(account_number)
     if account_number is not None:
          data = request_get(url)
     else:
-        data = request_get(url, 'indexzero')
+        data = request_get(url, dataType)
     return(filter_data(data, info))
 
 
 @login_required
 def load_basic_profile(info=None):
     """Gets the information associated with the personal profile,
     such as phone number, city, marital status, and date of birth.
@@ -132,15 +136,15 @@
     """
     url = investment_profile_url()
     data = request_get(url)
     return(filter_data(data, info))
 
 
 @login_required
-def load_portfolio_profile(info=None):
+def load_portfolio_profile(account_number=None, info=None):
     """Gets the information associated with the portfolios profile,
     such as withdrawable amount, market value of account, and excess margin.
 
     :param info: The name of the key whose value is to be returned from the function.
     :type info: Optional[str]
     :returns: The function returns a dictionary of key/value pairs. \
     If a string is passed in to the info parameter, then the function will return \
@@ -165,16 +169,19 @@
                       * adjusted_equity_previous_close
                       * adjusted_portfolio_equity_previous_close
                       * withdrawable_amount
                       * unwithdrawable_deposits
                       * unwithdrawable_grants
 
     """
-    url = portfolio_profile_url()
-    data = request_get(url, 'indexzero')
+    url = portfolio_profile_url(account_number)
+    if account_number is not None:
+        data = request_get(url)
+    else:
+        data = request_get(url, 'indexzero')
     return(filter_data(data, info))
 
 
 @login_required
 def load_security_profile(info=None):
     """Gets the information associated with the security profile.
```

### Comparing `robin_stocks-3.0.6/robin_stocks/robinhood/stocks.py` & `robin_stocks-3.1.0/robin_stocks/robinhood/stocks.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.6/robin_stocks/robinhood/urls.py` & `robin_stocks-3.1.0/robin_stocks/robinhood/urls.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,27 +14,30 @@
 # Profiles
 
 
 def account_profile_url(account_number=None):
     if account_number:
         return('https://api.robinhood.com/accounts/'+account_number)
     else:
-        return('https://api.robinhood.com/accounts/')
+        return('https://api.robinhood.com/accounts/?default_to_all_accounts=true')
 
 
 def basic_profile_url():
     return('https://api.robinhood.com/user/basic_info/')
 
 
 def investment_profile_url():
     return('https://api.robinhood.com/user/investment_profile/')
 
 
-def portfolio_profile_url():
-    return('https://api.robinhood.com/portfolios/')
+def portfolio_profile_url(account_number=None):
+    if account_number:
+        return('https://api.robinhood.com/portfolios/'+account_number)
+    else:
+        return('https://api.robinhood.com/portfolios/')
 
 
 def security_profile_url():
     return('https://api.robinhood.com/user/additional_info/')
 
 
 def user_profile_url():
@@ -188,16 +191,19 @@
 
 def market_category_url(category):
     return('https://api.robinhood.com/midlands/tags/tag/{}/'.format(category))
 
 # options
 
 
-def aggregate_url():
-    return('https://api.robinhood.com/options/aggregate_positions/')
+def aggregate_url(account_number):
+    if account_number:
+        return('https://api.robinhood.com/options/aggregate_positions/?account_numbers='+account_number)
+    else:
+        return('https://api.robinhood.com/options/aggregate_positions/')
 
 
 def chains_url(symbol):
     return('https://api.robinhood.com/options/chains/{0}/'.format(id_for_chain(symbol)))
 
 
 def option_historicals_url(id):
```

### Comparing `robin_stocks-3.0.6/robin_stocks/tda/__init__.py` & `robin_stocks-3.1.0/robin_stocks/tda/__init__.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.6/robin_stocks/tda/accounts.py` & `robin_stocks-3.1.0/robin_stocks/tda/accounts.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.6/robin_stocks/tda/authentication.py` & `robin_stocks-3.1.0/robin_stocks/tda/authentication.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.6/robin_stocks/tda/globals.py` & `robin_stocks-3.1.0/robin_stocks/tda/globals.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.6/robin_stocks/tda/helper.py` & `robin_stocks-3.1.0/robin_stocks/tda/helper.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.6/robin_stocks/tda/markets.py` & `robin_stocks-3.1.0/robin_stocks/tda/markets.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.6/robin_stocks/tda/orders.py` & `robin_stocks-3.1.0/robin_stocks/tda/orders.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.6/robin_stocks/tda/stocks.py` & `robin_stocks-3.1.0/robin_stocks/tda/stocks.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.6/robin_stocks/tda/urls.py` & `robin_stocks-3.1.0/robin_stocks/tda/urls.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.6/robin_stocks.egg-info/PKG-INFO` & `robin_stocks-3.1.0/robin_stocks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robin-stocks
-Version: 3.0.6
+Version: 3.1.0
 Summary: A Python wrapper around the Robinhood API
 Home-page: https://github.com/jmfernandes/robin_stocks
 Author: Josh Fernandes
 Author-email: joshfernandes@mac.com
 License: MIT
 Keywords: robinhood,robin stocks,finance app,stocks,options,trading,investing
 Requires: requests
```

### Comparing `robin_stocks-3.0.6/robin_stocks.egg-info/SOURCES.txt` & `robin_stocks-3.1.0/robin_stocks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.6/setup.py` & `robin_stocks-3.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='robin_stocks',
-      version='3.0.6',
+      version='3.1.0',
       description='A Python wrapper around the Robinhood API',
       long_description=long_description,
       long_description_content_type='text/x-rst',
       url='https://github.com/jmfernandes/robin_stocks',
       author='Josh Fernandes',
       author_email='joshfernandes@mac.com',
       keywords=['robinhood','robin stocks','finance app','stocks','options','trading','investing'],
```

### Comparing `robin_stocks-3.0.6/tests/app_tests.py` & `robin_stocks-3.1.0/tests/app_tests.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.6/tests/test_gemini.py` & `robin_stocks-3.1.0/tests/test_gemini.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.6/tests/test_robinhood.py` & `robin_stocks-3.1.0/tests/test_robinhood.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.6/tests/test_tda.py` & `robin_stocks-3.1.0/tests/test_tda.py`

 * *Files identical despite different names*

