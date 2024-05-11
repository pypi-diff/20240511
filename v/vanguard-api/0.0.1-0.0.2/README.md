# Comparing `tmp/vanguard_api-0.0.1.tar.gz` & `tmp/vanguard_api-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vanguard_api-0.0.1.tar", last modified: Tue May  7 10:38:46 2024, max compression
+gzip compressed data, was "vanguard_api-0.0.2.tar", last modified: Sat May 11 01:19:30 2024, max compression
```

## Comparing `vanguard_api-0.0.1.tar` & `vanguard_api-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:38:46.691939 vanguard_api-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-07 10:38:42.000000 vanguard_api-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-07 10:38:46.691939 vanguard_api-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-07 10:38:42.000000 vanguard_api-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 10:38:46.691939 vanguard_api-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-07 10:38:42.000000 vanguard_api-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:38:46.691939 vanguard_api-0.0.1/vanguard/
--rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-05-07 10:38:42.000000 vanguard_api-0.0.1/vanguard/account.py
--rw-r--r--   0 runner    (1001) docker     (127)    13047 2024-05-07 10:38:42.000000 vanguard_api-0.0.1/vanguard/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-05-07 10:38:42.000000 vanguard_api-0.0.1/vanguard/session.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-07 10:38:42.000000 vanguard_api-0.0.1/vanguard/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:38:46.691939 vanguard_api-0.0.1/vanguard_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-07 10:38:46.000000 vanguard_api-0.0.1/vanguard_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-07 10:38:46.000000 vanguard_api-0.0.1/vanguard_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 10:38:46.000000 vanguard_api-0.0.1/vanguard_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 10:38:46.000000 vanguard_api-0.0.1/vanguard_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 10:38:46.000000 vanguard_api-0.0.1/vanguard_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:19:30.526579 vanguard_api-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-11 01:19:26.000000 vanguard_api-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-11 01:19:30.526579 vanguard_api-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-11 01:19:26.000000 vanguard_api-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 01:19:30.526579 vanguard_api-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-11 01:19:26.000000 vanguard_api-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:19:30.526579 vanguard_api-0.0.2/vanguard/
+-rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-05-11 01:19:26.000000 vanguard_api-0.0.2/vanguard/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13047 2024-05-11 01:19:26.000000 vanguard_api-0.0.2/vanguard/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9530 2024-05-11 01:19:26.000000 vanguard_api-0.0.2/vanguard/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-11 01:19:26.000000 vanguard_api-0.0.2/vanguard/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:19:30.526579 vanguard_api-0.0.2/vanguard_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-11 01:19:30.000000 vanguard_api-0.0.2/vanguard_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-11 01:19:30.000000 vanguard_api-0.0.2/vanguard_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 01:19:30.000000 vanguard_api-0.0.2/vanguard_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-11 01:19:30.000000 vanguard_api-0.0.2/vanguard_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-11 01:19:30.000000 vanguard_api-0.0.2/vanguard_api.egg-info/top_level.txt
```

### Comparing `vanguard_api-0.0.1/LICENSE` & `vanguard_api-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vanguard_api-0.0.1/PKG-INFO` & `vanguard_api-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vanguard-api
-Version: 0.0.1
+Version: 0.0.2
 Summary: An unofficial API for Vanguard Invest
 Home-page: https://github.com/MaxxRK/vanguard-api
-Download-URL: https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.1.tar.gz
+Download-URL: https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.2.tar.gz
 Author: MaxxRK
 Author-email: maxxrk@pm.me
 License: MIT
 Keywords: VANGUARD,API
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
@@ -45,15 +45,15 @@
 ```
 If you would like some more information on this, you can find it [here](https://playwright.dev/python/docs/intro).
 
 ## Quickstart
 Checkout `test.py` for a quickstart example it will: 
 - Login and print account info.
 - Print out Holdings.
-- Place a market order for 'INTC' on the first account in the `account_numbers` list
+- Place a dry run market order for 'INTC' on the first account in the `account_numbers` list
 - Print out the order confirmation
 
 
 ---
 
  ## Implemented Features
  - [x] Login
```

### Comparing `vanguard_api-0.0.1/README.md` & `vanguard_api-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ```
 If you would like some more information on this, you can find it [here](https://playwright.dev/python/docs/intro).
 
 ## Quickstart
 Checkout `test.py` for a quickstart example it will: 
 - Login and print account info.
 - Print out Holdings.
-- Place a market order for 'INTC' on the first account in the `account_numbers` list
+- Place a dry run market order for 'INTC' on the first account in the `account_numbers` list
 - Print out the order confirmation
 
 
 ---
 
  ## Implemented Features
  - [x] Login
```

### Comparing `vanguard_api-0.0.1/setup.py` & `vanguard_api-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="vanguard-api",
-    version="0.0.1",
+    version="0.0.2",
     author="MaxxRK",
     author_email="maxxrk@pm.me",
     description="An unofficial API for Vanguard Invest",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/MaxxRK/vanguard-api",
-    download_url="https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.1.tar.gz",
+    download_url="https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.2.tar.gz",
     keywords=["VANGUARD", "API"],
     install_requires=["playwright", "playwright-stealth"],
     packages=["vanguard"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Internet :: WWW/HTTP :: Session",
```

### Comparing `vanguard_api-0.0.1/vanguard/account.py` & `vanguard_api-0.0.2/vanguard/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,21 +82,27 @@
                         stock_symbols.append(description.strip())
                     if j == 2:
                         stock_descriptions.append(description.strip())
                 stock_price_elements = row.query_selector_all("td")
                 for k, price in enumerate(stock_price_elements):
                     if k == 0:
                         price_text = price.inner_text()
-                        stock_prices.append(float(price_text.replace("$", "").replace(",", "").strip()))
+                        try:
+                            stock_prices.append(float(price_text.replace("$", "").replace(",", "").strip()))
+                        except ValueError:
+                            stock_prices.append(0.00)
                     elif k == 1:
                         dollar_changes.append(price.inner_text())
                     elif k == 2:
                         percent_changes.append(price.inner_text())
                     elif k == 3:
-                        quantities.append(float(price.inner_text()))
+                        try:
+                            quantities.append(float(price.inner_text()))
+                        except ValueError:
+                            quantities.append(0.00)
             if i == len(table_rows) - 1:
                 for (stock_symbol, stock_description, stock_price, dollar_change,
                                     percent_change, quantity) in zip_longest(stock_symbols, stock_descriptions,
                                                         stock_prices, dollar_changes,
                                                         percent_changes, quantities, fillvalue=None):
                     stocks.append({
                         "symbol": stock_symbol,
```

### Comparing `vanguard_api-0.0.1/vanguard/order.py` & `vanguard_api-0.0.2/vanguard/order.py`

 * *Files identical despite different names*

### Comparing `vanguard_api-0.0.1/vanguard/session.py` & `vanguard_api-0.0.2/vanguard/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         with open(self.profile_path, "w") as f:
             json.dump(storage_state, f)
 
     def close_browser(self):
         """Closes the browser."""
         if self.debug:
             self.context.tracing.stop(
-                path=f'vanguard_trace{self.title if self.title is not None else ""}.zip'
+                path=f'./vanguard_trace{self.title if self.title is not None else ""}.zip'
             )
         self.save_storage_state()
         self.browser.close()
         self.playwright.stop()
         
     def go_url(self, url):
         """Navigates to the specified URL."""
@@ -139,23 +139,23 @@
 
         Raises:
             Exception: If there is an error during the login process in step one.
         """
         try:
             self.password = password
             self.go_url(landing_page())
-            try:
-                self.page.wait_for_url(
-                        landing_page(),
-                        wait_until="domcontentloaded",
-                        timeout=8000
-                    )
-                return False
-            except PlaywrightTimeoutError:
-                pass
+            for _ in range(30):
+                try:
+                    self.page.wait_for_selector("#username-password-submit-btn-1", timeout=1000)
+                except PlaywrightTimeoutError:
+                    break
+                try:
+                    self.page.wait_for_selector("body > vg-vgn-nav > div:nth-child(1) > greetings-widget", timeout=1000)
+                except PlaywrightTimeoutError:
+                    return False
             self.page.wait_for_selector("#username-password-submit-btn-1", timeout=30000)
             username_box = self.page.query_selector("#USER")
             username_box.type(username, delay=random.randint(50, 500))
             username_box.press("Tab")
             password_box = self.page.query_selector("#PASSWORD-blocked")
             password_box.type(password, delay=random.randint(50, 500))
             sleep(random.uniform(1, 3))
```

### Comparing `vanguard_api-0.0.1/vanguard_api.egg-info/PKG-INFO` & `vanguard_api-0.0.2/vanguard_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vanguard-api
-Version: 0.0.1
+Version: 0.0.2
 Summary: An unofficial API for Vanguard Invest
 Home-page: https://github.com/MaxxRK/vanguard-api
-Download-URL: https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.1.tar.gz
+Download-URL: https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.2.tar.gz
 Author: MaxxRK
 Author-email: maxxrk@pm.me
 License: MIT
 Keywords: VANGUARD,API
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
@@ -45,15 +45,15 @@
 ```
 If you would like some more information on this, you can find it [here](https://playwright.dev/python/docs/intro).
 
 ## Quickstart
 Checkout `test.py` for a quickstart example it will: 
 - Login and print account info.
 - Print out Holdings.
-- Place a market order for 'INTC' on the first account in the `account_numbers` list
+- Place a dry run market order for 'INTC' on the first account in the `account_numbers` list
 - Print out the order confirmation
 
 
 ---
 
  ## Implemented Features
  - [x] Login
```

