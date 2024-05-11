# Comparing `tmp/aic_tools_alpaca-1.0.0.tar.gz` & `tmp/aic_tools_alpaca-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aic_tools_alpaca-1.0.0.tar", last modified: Thu May  2 04:08:12 2024, max compression
+gzip compressed data, was "aic_tools_alpaca-1.0.1.tar", last modified: Sat May 11 19:33:10 2024, max compression
```

## Comparing `aic_tools_alpaca-1.0.0.tar` & `aic_tools_alpaca-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxr-x   0 serhii    (1000) serhii    (1000)        0 2024-05-02 04:08:12.569329 aic_tools_alpaca-1.0.0/
--rw-r--r--   0 serhii    (1000) serhii    (1000)      605 2024-05-02 04:08:12.569329 aic_tools_alpaca-1.0.0/PKG-INFO
--rw-rw-r--   0 serhii    (1000) serhii    (1000)      311 2024-04-22 11:29:53.000000 aic_tools_alpaca-1.0.0/README.md
-drwxrwxr-x   0 serhii    (1000) serhii    (1000)        0 2024-05-02 04:08:12.567329 aic_tools_alpaca-1.0.0/aic_tools_alpaca/
--rw-rw-r--   0 serhii    (1000) serhii    (1000)        0 2024-04-21 15:47:15.000000 aic_tools_alpaca-1.0.0/aic_tools_alpaca/__init__.py
--rw-rw-r--   0 serhii    (1000) serhii    (1000)     1889 2024-05-01 10:51:28.000000 aic_tools_alpaca-1.0.0/aic_tools_alpaca/account_info.py
-drwxrwxr-x   0 serhii    (1000) serhii    (1000)        0 2024-05-02 04:08:12.568329 aic_tools_alpaca-1.0.0/aic_tools_alpaca.egg-info/
--rw-r--r--   0 serhii    (1000) serhii    (1000)      605 2024-05-02 04:08:11.000000 aic_tools_alpaca-1.0.0/aic_tools_alpaca.egg-info/PKG-INFO
--rw-rw-r--   0 serhii    (1000) serhii    (1000)      344 2024-05-02 04:08:11.000000 aic_tools_alpaca-1.0.0/aic_tools_alpaca.egg-info/SOURCES.txt
--rw-rw-r--   0 serhii    (1000) serhii    (1000)        1 2024-05-02 04:08:11.000000 aic_tools_alpaca-1.0.0/aic_tools_alpaca.egg-info/dependency_links.txt
--rw-rw-r--   0 serhii    (1000) serhii    (1000)       38 2024-05-02 04:08:11.000000 aic_tools_alpaca-1.0.0/aic_tools_alpaca.egg-info/requires.txt
--rw-rw-r--   0 serhii    (1000) serhii    (1000)       23 2024-05-02 04:08:11.000000 aic_tools_alpaca-1.0.0/aic_tools_alpaca.egg-info/top_level.txt
--rw-rw-r--   0 serhii    (1000) serhii    (1000)       38 2024-05-02 04:08:12.569329 aic_tools_alpaca-1.0.0/setup.cfg
--rw-rw-r--   0 serhii    (1000) serhii    (1000)      784 2024-05-02 03:48:52.000000 aic_tools_alpaca-1.0.0/setup.py
-drwxrwxr-x   0 serhii    (1000) serhii    (1000)        0 2024-05-02 04:08:12.568329 aic_tools_alpaca-1.0.0/tests/
--rw-rw-r--   0 serhii    (1000) serhii    (1000)        0 2024-04-21 16:42:01.000000 aic_tools_alpaca-1.0.0/tests/__init__.py
--rw-rw-r--   0 serhii    (1000) serhii    (1000)      438 2024-05-01 10:51:28.000000 aic_tools_alpaca-1.0.0/tests/handy_test.py
--rw-rw-r--   0 serhii    (1000) serhii    (1000)     1771 2024-05-01 10:51:28.000000 aic_tools_alpaca-1.0.0/tests/test_account_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:33:10.369110 aic_tools_alpaca-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-11 19:33:03.000000 aic_tools_alpaca-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-11 19:33:10.369110 aic_tools_alpaca-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-11 19:33:03.000000 aic_tools_alpaca-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:33:10.365110 aic_tools_alpaca-1.0.1/aic_tools_alpaca/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-11 19:33:03.000000 aic_tools_alpaca-1.0.1/aic_tools_alpaca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-11 19:33:03.000000 aic_tools_alpaca-1.0.1/aic_tools_alpaca/account_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:33:10.369110 aic_tools_alpaca-1.0.1/aic_tools_alpaca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-11 19:33:10.000000 aic_tools_alpaca-1.0.1/aic_tools_alpaca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-11 19:33:10.000000 aic_tools_alpaca-1.0.1/aic_tools_alpaca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 19:33:10.000000 aic_tools_alpaca-1.0.1/aic_tools_alpaca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 19:33:10.000000 aic_tools_alpaca-1.0.1/aic_tools_alpaca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-11 19:33:10.000000 aic_tools_alpaca-1.0.1/aic_tools_alpaca.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-11 19:33:03.000000 aic_tools_alpaca-1.0.1/develop.md
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-11 19:33:03.000000 aic_tools_alpaca-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 19:33:10.369110 aic_tools_alpaca-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-11 19:33:03.000000 aic_tools_alpaca-1.0.1/setup.py
```

### Comparing `aic_tools_alpaca-1.0.0/aic_tools_alpaca/account_info.py` & `aic_tools_alpaca-1.0.1/aic_tools_alpaca/account_info.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,42 @@
-import os
-
 from crewai_tools import BaseTool
-
-from dotenv import load_dotenv
-from alpaca.trading.client import TradingClient
-
-load_dotenv()
-api_key_id = os.getenv('API_KEY_ID')
-secret_key = os.getenv('SECRET_KEY')
-
-trading_client = TradingClient(api_key_id, secret_key, paper=True)
-acc = trading_client.get_account()
+from aic_tools_alpaca import TradingClientSingleton
 
 
 class CheckIfTradingBlocked(BaseTool):
     name: str = "Answer on: is trading prohibited?"
     description: str = """Answers the question whether trading is blocked for this account.
     If true, the account does not allow placing orders.
     If false, the account allows placing orders."""
 
     def _run(self) -> bool:
         # Your tool's logic here
-        return acc.trading_blocked
+        return TradingClientSingleton.get_instance().get_account().trading_blocked
 
 
 class GetTotalBuyingPower(BaseTool):
     name: str = "Accountant total purchasing power."
     description: str = """Returns a string with the number of dollars as the purchasing power of the accountant.
     Current available cash buying power. If multiplier = 2 then buying_power = max(equity-initial_margin(0) * 2).
     If multiplier = 1 then buying_power = cash."""
 
     def _run(self) -> str:
-        return f"{acc.buying_power}$"
+        return f"{TradingClientSingleton.get_instance().get_account().buying_power}$"
 
 
 class GetNonMarginableBuyingPower(BaseTool):
     name: str = "Accountant purchasing power without margin."
     description: str = "Returns a string with the number of dollars as the non marginable buying power for the account."
 
     def _run(self) -> str:
-        return f"{acc.non_marginable_buying_power}$"
+        return f"{TradingClientSingleton.get_instance().get_account().non_marginable_buying_power}$"
 
 
 class GetAccountEquity(BaseTool):
     name: str = "Answer on: what is portfolio value?"
     description: str = """Returns a string with the numbers of dollars that tell us the account equity.
     This value is cash + long_market_value + short_market_value.
     This value isn’t calculated in the SDK it is computed on the server and we return the raw value here.
     """
 
     def _run(self) -> str:
-        return f"{acc.equity}$"
+        return f"{TradingClientSingleton.get_instance().get_account().equity}$"
```

### Comparing `aic_tools_alpaca-1.0.0/setup.py` & `aic_tools_alpaca-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 # Call the function and store the requirements list
 install_requires = read_requirements()
 
 setup(
     name='aic_tools_alpaca',
-    version='1.0.0',
+    version='1.0.1',
     packages=find_packages(),
     description='Alpaca tools for AI Characters',
     long_description_content_type='text/markdown',
     long_description=open('README.md').read(),
     author='Viacheslav Kovalevskyi',
     author_email='viacheslav@kovalevskyi.com',
     license='MIT',
```

