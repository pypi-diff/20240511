# Comparing `tmp/tiktok_captcha_solver-0.0.1.tar.gz` & `tmp/tiktok_captcha_solver-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiktok_captcha_solver-0.0.1.tar", last modified: Tue May  7 03:10:25 2024, max compression
+gzip compressed data, was "tiktok_captcha_solver-0.0.2.tar", last modified: Fri May 10 13:15:55 2024, max compression
```

## Comparing `tiktok_captcha_solver-0.0.1.tar` & `tiktok_captcha_solver-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-07 03:10:25.137794 tiktok_captcha_solver-0.0.1/
--rw-r--r--   0 gregb     (1000) gregb     (1000)     1984 2024-05-07 03:10:25.137794 tiktok_captcha_solver-0.0.1/PKG-INFO
--rw-r--r--   0 gregb     (1000) gregb     (1000)     1054 2024-05-07 03:09:32.000000 tiktok_captcha_solver-0.0.1/README.md
--rw-r--r--   0 gregb     (1000) gregb     (1000)     1033 2024-05-07 03:07:51.000000 tiktok_captcha_solver-0.0.1/pyproject.toml
--rw-r--r--   0 gregb     (1000) gregb     (1000)       38 2024-05-07 03:10:25.137794 tiktok_captcha_solver-0.0.1/setup.cfg
-drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-07 03:10:25.135794 tiktok_captcha_solver-0.0.1/tiktok_captcha_solver/
--rw-r--r--   0 gregb     (1000) gregb     (1000)        0 2024-05-05 05:46:39.000000 tiktok_captcha_solver-0.0.1/tiktok_captcha_solver/__init__.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)     1769 2024-05-06 04:28:16.000000 tiktok_captcha_solver-0.0.1/tiktok_captcha_solver/api.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)      219 2024-05-05 17:02:10.000000 tiktok_captcha_solver-0.0.1/tiktok_captcha_solver/downloader.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)      335 2024-05-05 06:12:30.000000 tiktok_captcha_solver-0.0.1/tiktok_captcha_solver/models.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)     7759 2024-05-06 12:48:31.000000 tiktok_captcha_solver-0.0.1/tiktok_captcha_solver/sadcaptcha.py
-drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-07 03:10:25.136794 tiktok_captcha_solver-0.0.1/tiktok_captcha_solver/tests/
--rw-r--r--   0 gregb     (1000) gregb     (1000)        0 2024-05-05 16:49:30.000000 tiktok_captcha_solver-0.0.1/tiktok_captcha_solver/tests/__init__.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)     1264 2024-05-05 17:22:04.000000 tiktok_captcha_solver-0.0.1/tiktok_captcha_solver/tests/test_api.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)      189 2024-05-05 17:34:44.000000 tiktok_captcha_solver-0.0.1/tiktok_captcha_solver/tests/test_downloader.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)     1839 2024-05-06 05:12:34.000000 tiktok_captcha_solver-0.0.1/tiktok_captcha_solver/tests/test_sadcaptcha.py
-drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-07 03:10:25.137794 tiktok_captcha_solver-0.0.1/tiktok_captcha_solver.egg-info/
--rw-r--r--   0 gregb     (1000) gregb     (1000)     1984 2024-05-07 03:10:25.000000 tiktok_captcha_solver-0.0.1/tiktok_captcha_solver.egg-info/PKG-INFO
--rw-r--r--   0 gregb     (1000) gregb     (1000)      589 2024-05-07 03:10:25.000000 tiktok_captcha_solver-0.0.1/tiktok_captcha_solver.egg-info/SOURCES.txt
--rw-r--r--   0 gregb     (1000) gregb     (1000)        1 2024-05-07 03:10:25.000000 tiktok_captcha_solver-0.0.1/tiktok_captcha_solver.egg-info/dependency_links.txt
--rw-r--r--   0 gregb     (1000) gregb     (1000)       76 2024-05-07 03:10:25.000000 tiktok_captcha_solver-0.0.1/tiktok_captcha_solver.egg-info/requires.txt
--rw-r--r--   0 gregb     (1000) gregb     (1000)       22 2024-05-07 03:10:25.000000 tiktok_captcha_solver-0.0.1/tiktok_captcha_solver.egg-info/top_level.txt
+drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-10 13:15:55.801166 tiktok_captcha_solver-0.0.2/
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     2509 2024-05-10 13:15:55.801166 tiktok_captcha_solver-0.0.2/PKG-INFO
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     1579 2024-05-10 13:09:44.000000 tiktok_captcha_solver-0.0.2/README.md
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     1033 2024-05-10 13:15:24.000000 tiktok_captcha_solver-0.0.2/pyproject.toml
+-rw-r--r--   0 gregb     (1000) gregb     (1000)       38 2024-05-10 13:15:55.801166 tiktok_captcha_solver-0.0.2/setup.cfg
+drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-10 13:15:55.798166 tiktok_captcha_solver-0.0.2/src/
+drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-10 13:15:55.799166 tiktok_captcha_solver-0.0.2/src/tiktok_captcha_solver/
+-rw-r--r--   0 gregb     (1000) gregb     (1000)       64 2024-05-10 13:09:13.000000 tiktok_captcha_solver-0.0.2/src/tiktok_captcha_solver/__init__.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     1769 2024-05-07 22:47:01.000000 tiktok_captcha_solver-0.0.2/src/tiktok_captcha_solver/api.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)      219 2024-05-05 17:02:10.000000 tiktok_captcha_solver-0.0.2/src/tiktok_captcha_solver/downloader.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)      335 2024-05-05 06:12:30.000000 tiktok_captcha_solver-0.0.2/src/tiktok_captcha_solver/models.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     8081 2024-05-07 22:47:01.000000 tiktok_captcha_solver-0.0.2/src/tiktok_captcha_solver/sadcaptcha.py
+drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-10 13:15:55.801166 tiktok_captcha_solver-0.0.2/src/tiktok_captcha_solver/tests/
+-rw-r--r--   0 gregb     (1000) gregb     (1000)        0 2024-05-05 16:49:30.000000 tiktok_captcha_solver-0.0.2/src/tiktok_captcha_solver/tests/__init__.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     1264 2024-05-05 17:22:04.000000 tiktok_captcha_solver-0.0.2/src/tiktok_captcha_solver/tests/test_api.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)      189 2024-05-05 17:34:44.000000 tiktok_captcha_solver-0.0.2/src/tiktok_captcha_solver/tests/test_downloader.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     1861 2024-05-07 22:03:34.000000 tiktok_captcha_solver-0.0.2/src/tiktok_captcha_solver/tests/test_sadcaptcha.py
+drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-10 13:15:55.801166 tiktok_captcha_solver-0.0.2/src/tiktok_captcha_solver.egg-info/
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     2509 2024-05-10 13:15:55.000000 tiktok_captcha_solver-0.0.2/src/tiktok_captcha_solver.egg-info/PKG-INFO
+-rw-r--r--   0 gregb     (1000) gregb     (1000)      645 2024-05-10 13:15:55.000000 tiktok_captcha_solver-0.0.2/src/tiktok_captcha_solver.egg-info/SOURCES.txt
+-rw-r--r--   0 gregb     (1000) gregb     (1000)        1 2024-05-10 13:15:55.000000 tiktok_captcha_solver-0.0.2/src/tiktok_captcha_solver.egg-info/dependency_links.txt
+-rw-r--r--   0 gregb     (1000) gregb     (1000)       76 2024-05-10 13:15:55.000000 tiktok_captcha_solver-0.0.2/src/tiktok_captcha_solver.egg-info/requires.txt
+-rw-r--r--   0 gregb     (1000) gregb     (1000)       22 2024-05-10 13:15:55.000000 tiktok_captcha_solver-0.0.2/src/tiktok_captcha_solver.egg-info/top_level.txt
```

### Comparing `tiktok_captcha_solver-0.0.1/PKG-INFO` & `tiktok_captcha_solver-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiktok-captcha-solver
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package integrates with Selenium to solve any TikTok captcha in one line of code.
 Author-email: Toughdata LLC <greg@toughdata.net>
 Project-URL: Homepage, https://www.sadcaptcha.com
 Project-URL: Source, https://github.com/gbiz123/tiktok-captcha-solver/
 Keywords: tiktok,captcha,solver,selenium,rotate,puzzle,3d
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -26,37 +26,54 @@
 The purpose is to make integrating SadCaptcha into your selenium app as simple as one line of code.
 
 ## Requirements
 - Python >= 3.10
 - Selenium properly installed and in `PATH`
 
 ## Installation
-This project will be available as a `pip` package soon. 
-For now, just clone the repo and build it using the following commands:
+This project can be installed with `pip`. Just run the following command:
 ```
-git clone https://github.com/gbiz123/tiktok-captcha-solver
-cd tiktok-captcha-solver
-pip install -e .
+pip install tiktok-captcha-solver
 ```
 
-## Usage
+## Selenium client 
 Import the package, set up the SadCaptcha class, and call it whenever you need.
+This turns the entire captcha detection, solution, retry, and verification process into a single line of code.
+It is the recommended method if you are using Selenium.
 
 ```py
-from sadcaptcha import SadCaptcha
+from tiktok_captcha_solver import SadCaptcha
 import undetected_chromedriver as uc
 
 driver = uc.Chrome(headless=False)
 api_key = "YOUR_API_KEY_HERE"
 sadcaptcha = SadCaptcha(driver, api_key)
 
 # Selenium code that causes a TikTok captcha...
 
 sadcaptcha.solve_captcha_if_present()
 ```
 
 That's it!
 
+## API Client
+If you are not using Selenium, you can still import and use the API client to help you make calls to SadCaptcha
+```py
+from tiktok_captcha_solver import ApiClient
+
+api_key = "YOUR_API_KEY_HERE"
+client = ApiClient(api_key)
+
+# Rotate
+res = client.rotate("base64 encoded outer", "base64 encoded inner")
+
+# Puzzle
+res = client.puzzle("base64 encoded puzzle", "base64 encoded piece")
+
+# Shapes
+res = client.shapes("base64 encoded shapes image")
+```
+
 ## Contact
 - Homepage: https://www.sadcaptcha.com/
 - Email: info@toughdata.net
 - Telegram @toughdata
```

### Comparing `tiktok_captcha_solver-0.0.1/README.md` & `tiktok_captcha_solver-0.0.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -3,37 +3,54 @@
 The purpose is to make integrating SadCaptcha into your selenium app as simple as one line of code.
 
 ## Requirements
 - Python >= 3.10
 - Selenium properly installed and in `PATH`
 
 ## Installation
-This project will be available as a `pip` package soon. 
-For now, just clone the repo and build it using the following commands:
+This project can be installed with `pip`. Just run the following command:
 ```
-git clone https://github.com/gbiz123/tiktok-captcha-solver
-cd tiktok-captcha-solver
-pip install -e .
+pip install tiktok-captcha-solver
 ```
 
-## Usage
+## Selenium client 
 Import the package, set up the SadCaptcha class, and call it whenever you need.
+This turns the entire captcha detection, solution, retry, and verification process into a single line of code.
+It is the recommended method if you are using Selenium.
 
 ```py
-from sadcaptcha import SadCaptcha
+from tiktok_captcha_solver import SadCaptcha
 import undetected_chromedriver as uc
 
 driver = uc.Chrome(headless=False)
 api_key = "YOUR_API_KEY_HERE"
 sadcaptcha = SadCaptcha(driver, api_key)
 
 # Selenium code that causes a TikTok captcha...
 
 sadcaptcha.solve_captcha_if_present()
 ```
 
 That's it!
 
+## API Client
+If you are not using Selenium, you can still import and use the API client to help you make calls to SadCaptcha
+```py
+from tiktok_captcha_solver import ApiClient
+
+api_key = "YOUR_API_KEY_HERE"
+client = ApiClient(api_key)
+
+# Rotate
+res = client.rotate("base64 encoded outer", "base64 encoded inner")
+
+# Puzzle
+res = client.puzzle("base64 encoded puzzle", "base64 encoded piece")
+
+# Shapes
+res = client.shapes("base64 encoded shapes image")
+```
+
 ## Contact
 - Homepage: https://www.sadcaptcha.com/
 - Email: info@toughdata.net
 - Telegram @toughdata
```

### Comparing `tiktok_captcha_solver-0.0.1/pyproject.toml` & `tiktok_captcha_solver-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"  # If not defined, then legacy behavior can happen.
 
 [project]
 name = "tiktok-captcha-solver"
-version = "0.0.1"
+version = "0.0.2"
 
 description = "This package integrates with Selenium to solve any TikTok captcha in one line of code."
 readme = "README.md"
 requires-python = ">=3.10"
 
 keywords = ["tiktok", "captcha", "solver", "selenium", "rotate", "puzzle", "3d"]
```

### Comparing `tiktok_captcha_solver-0.0.1/tiktok_captcha_solver/api.py` & `tiktok_captcha_solver-0.0.2/src/tiktok_captcha_solver/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -103,9 +103,9 @@
 00000660: 706f 696e 745f 7477 6f5f 7072 6f70 6f72  point_two_propor
 00000670: 7469 6f6e 5f78 3d72 6573 756c 742e 6765  tion_x=result.ge
 00000680: 7428 2270 6f69 6e74 5477 6f50 726f 706f  t("pointTwoPropo
 00000690: 7274 696f 6e58 2229 2c0a 2020 2020 2020  rtionX"),.      
 000006a0: 2020 2020 2020 706f 696e 745f 7477 6f5f        point_two_
 000006b0: 7072 6f70 6f72 7469 6f6e 5f79 3d72 6573  proportion_y=res
 000006c0: 756c 742e 6765 7428 2270 6f69 6e74 5477  ult.get("pointTw
-000006d0: 6f50 726f 706f 7274 696f 6e58 2229 0a20  oProportionX"). 
+000006d0: 6f50 726f 706f 7274 696f 6e59 2229 0a20  oProportionY"). 
 000006e0: 2020 2020 2020 2029 0a                          ).
```

### Comparing `tiktok_captcha_solver-0.0.1/tiktok_captcha_solver/sadcaptcha.py` & `tiktok_captcha_solver-0.0.2/src/tiktok_captcha_solver/sadcaptcha.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """This class handles the captcha solving"""
 
 import time
 from typing import Literal
 from selenium.webdriver import ActionChains, Chrome
+from selenium.webdriver.common.actions.action_builder import ActionBuilder
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webelement import WebElement
 from undetected_chromedriver import logging
+from undetected_chromedriver.patcher import random
 
 from .api import ApiClient
 from .downloader import download_image_b64
 
 class SadCaptcha:
 
     client: ApiClient
@@ -59,15 +61,15 @@
 
     def solve_shapes(self, retries: int = 3) -> None:
         for _ in range(retries):
             image = download_image_b64(self._get_shapes_image_url())
             solution = self.client.shapes(image)
             image_element = self.chromedriver.find_element(By.CSS_SELECTOR, "#captcha-verify-image")
             self._click_proportional(image_element, solution.point_one_proportion_x, solution.point_one_proportion_y)
-            self._click_proportional(image_element, solution.point_two_proportion_y, solution.point_two_proportion_y)
+            self._click_proportional(image_element, solution.point_two_proportion_x, solution.point_two_proportion_y)
             self.chromedriver.find_element(By.CSS_SELECTOR, ".verify-captcha-submit-button").click()
             if self._check_captcha_success():
                 return
 
     def solve_rotate(self, retries: int = 3) -> None:
         for _ in range(retries):
             outer = download_image_b64(self._get_rotate_outer_image_url())
@@ -158,21 +160,25 @@
         to the width and height of the entire element
 
         Args:
             element: WebElement to click inside
             proportion_x: float from 0 to 1 defining the proportion x location to click 
             proportion_y: float from 0 to 1 defining the proportion y location to click 
         """
-        offset_x = (proportion_x * element.size["width"])
-        offset_y = (proportion_y * element.size["height"]) 
-        ActionChains(self.chromedriver) \
-            .move_to_element_with_offset(element, offset_x, offset_y) \
+        x_origin = element.location["x"]
+        y_origin = element.location["y"]
+        x_offset = (proportion_x * element.size["width"])
+        y_offset = (proportion_y * element.size["height"]) 
+        action = ActionBuilder(self.chromedriver)
+        action.pointer_action \
+            .move_to_location(x_origin + x_offset, y_origin + y_offset) \
+            .pause(random.randint(1, 10) / 11) \
             .click() \
-            .perform()
-        time.sleep(1.337)
+            .pause(random.randint(1, 10) / 11)
+        action.perform()
 
     def _drag_element(self, css_selector: str, x: int, y: int) -> None:
         e = self.chromedriver.find_element(By.CSS_SELECTOR, css_selector)
         actions = ActionChains(self.chromedriver, duration=500)
         actions.click_and_hold(e)
         actions.move_by_offset(x - 15, 0)
         time.sleep(0.001)
```

### Comparing `tiktok_captcha_solver-0.0.1/tiktok_captcha_solver/tests/test_api.py` & `tiktok_captcha_solver-0.0.2/src/tiktok_captcha_solver/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `tiktok_captcha_solver-0.0.1/tiktok_captcha_solver/tests/test_sadcaptcha.py` & `tiktok_captcha_solver-0.0.2/src/tiktok_captcha_solver/tests/test_sadcaptcha.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,18 +28,18 @@
     return uc.Chrome(service=ChromeDriverManager().install(), headless=False, use_subprocess=False)
 
 
 def open_tiktkok_login(driver: uc.Chrome) -> None:
     driver.get("https://www.tiktok.com/login/phone-or-email/email")
     time.sleep(10)
     write_username = driver.find_element(By.XPATH, '//input[contains(@name,"username")]');
-    write_username.send_keys("greg@toughdata.net");
+    write_username.send_keys(os.environ["TIKTOK_USERNAME"]);
     time.sleep(2);
     write_password = driver.find_element(By.XPATH, '//input[contains(@type,"password")]');
-    write_password.send_keys("th.etoughapi1!");
+    write_password.send_keys(os.environ["TIKTOK_PASSWORD"]);
     time.sleep(2)
     login_btn = driver.find_element(By.XPATH, '//button[contains(@data-e2e,"login-button")]').click();
     time.sleep(8)
 
 def test_solve_captcha():
     driver = make_driver()
     open_tiktkok_login(driver)
```

### Comparing `tiktok_captcha_solver-0.0.1/tiktok_captcha_solver.egg-info/PKG-INFO` & `tiktok_captcha_solver-0.0.2/src/tiktok_captcha_solver.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiktok-captcha-solver
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package integrates with Selenium to solve any TikTok captcha in one line of code.
 Author-email: Toughdata LLC <greg@toughdata.net>
 Project-URL: Homepage, https://www.sadcaptcha.com
 Project-URL: Source, https://github.com/gbiz123/tiktok-captcha-solver/
 Keywords: tiktok,captcha,solver,selenium,rotate,puzzle,3d
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -26,37 +26,54 @@
 The purpose is to make integrating SadCaptcha into your selenium app as simple as one line of code.
 
 ## Requirements
 - Python >= 3.10
 - Selenium properly installed and in `PATH`
 
 ## Installation
-This project will be available as a `pip` package soon. 
-For now, just clone the repo and build it using the following commands:
+This project can be installed with `pip`. Just run the following command:
 ```
-git clone https://github.com/gbiz123/tiktok-captcha-solver
-cd tiktok-captcha-solver
-pip install -e .
+pip install tiktok-captcha-solver
 ```
 
-## Usage
+## Selenium client 
 Import the package, set up the SadCaptcha class, and call it whenever you need.
+This turns the entire captcha detection, solution, retry, and verification process into a single line of code.
+It is the recommended method if you are using Selenium.
 
 ```py
-from sadcaptcha import SadCaptcha
+from tiktok_captcha_solver import SadCaptcha
 import undetected_chromedriver as uc
 
 driver = uc.Chrome(headless=False)
 api_key = "YOUR_API_KEY_HERE"
 sadcaptcha = SadCaptcha(driver, api_key)
 
 # Selenium code that causes a TikTok captcha...
 
 sadcaptcha.solve_captcha_if_present()
 ```
 
 That's it!
 
+## API Client
+If you are not using Selenium, you can still import and use the API client to help you make calls to SadCaptcha
+```py
+from tiktok_captcha_solver import ApiClient
+
+api_key = "YOUR_API_KEY_HERE"
+client = ApiClient(api_key)
+
+# Rotate
+res = client.rotate("base64 encoded outer", "base64 encoded inner")
+
+# Puzzle
+res = client.puzzle("base64 encoded puzzle", "base64 encoded piece")
+
+# Shapes
+res = client.shapes("base64 encoded shapes image")
+```
+
 ## Contact
 - Homepage: https://www.sadcaptcha.com/
 - Email: info@toughdata.net
 - Telegram @toughdata
```

