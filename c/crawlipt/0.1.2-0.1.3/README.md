# Comparing `tmp/crawlipt-0.1.2.tar.gz` & `tmp/crawlipt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlipt-0.1.2.tar", last modified: Thu May  9 16:17:20 2024, max compression
+gzip compressed data, was "crawlipt-0.1.3.tar", last modified: Fri May 10 08:12:11 2024, max compression
```

## Comparing `crawlipt-0.1.2.tar` & `crawlipt-0.1.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:17:20.218213 crawlipt-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-09 16:17:16.000000 crawlipt-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-09 16:17:16.000000 crawlipt-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-09 16:17:20.218213 crawlipt-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-09 16:17:16.000000 crawlipt-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:17:20.214213 crawlipt-0.1.2/crawlipt/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-09 16:17:16.000000 crawlipt-0.1.2/crawlipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-09 16:17:16.000000 crawlipt-0.1.2/crawlipt/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-09 16:17:16.000000 crawlipt-0.1.2/crawlipt/action.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:17:20.218213 crawlipt-0.1.2/crawlipt/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-09 16:17:16.000000 crawlipt-0.1.2/crawlipt/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-09 16:17:16.000000 crawlipt-0.1.2/crawlipt/actions/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-09 16:17:16.000000 crawlipt-0.1.2/crawlipt/actions/click.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-09 16:17:16.000000 crawlipt-0.1.2/crawlipt/actions/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-09 16:17:16.000000 crawlipt-0.1.2/crawlipt/actions/input.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-09 16:17:16.000000 crawlipt-0.1.2/crawlipt/actions/redirect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-09 16:17:16.000000 crawlipt-0.1.2/crawlipt/actions/scroll.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-09 16:17:16.000000 crawlipt-0.1.2/crawlipt/actions/select.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-09 16:17:16.000000 crawlipt-0.1.2/crawlipt/actions/slide.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-09 16:17:16.000000 crawlipt-0.1.2/crawlipt/actions/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-09 16:17:16.000000 crawlipt-0.1.2/crawlipt/actions/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-09 16:17:16.000000 crawlipt-0.1.2/crawlipt/actions/window.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-09 16:17:16.000000 crawlipt-0.1.2/crawlipt/annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-09 16:17:16.000000 crawlipt-0.1.2/crawlipt/condition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:17:20.218213 crawlipt-0.1.2/crawlipt/conditions/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-09 16:17:16.000000 crawlipt-0.1.2/crawlipt/conditions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-09 16:17:16.000000 crawlipt-0.1.2/crawlipt/conditions/element.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-09 16:17:16.000000 crawlipt-0.1.2/crawlipt/conditions/frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-09 16:17:16.000000 crawlipt-0.1.2/crawlipt/conditions/presence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-09 16:17:16.000000 crawlipt-0.1.2/crawlipt/conditions/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-09 16:17:16.000000 crawlipt-0.1.2/crawlipt/conditions/visibility.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-09 16:17:16.000000 crawlipt-0.1.2/crawlipt/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-09 16:17:16.000000 crawlipt-0.1.2/crawlipt/pojo.py
--rw-r--r--   0 runner    (1001) docker     (127)    28543 2024-05-09 16:17:16.000000 crawlipt-0.1.2/crawlipt/script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:17:20.218213 crawlipt-0.1.2/crawlipt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-09 16:17:20.000000 crawlipt-0.1.2/crawlipt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-09 16:17:20.000000 crawlipt-0.1.2/crawlipt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 16:17:20.000000 crawlipt-0.1.2/crawlipt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-09 16:17:20.000000 crawlipt-0.1.2/crawlipt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 16:17:20.000000 crawlipt-0.1.2/crawlipt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 16:17:20.218213 crawlipt-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-09 16:17:16.000000 crawlipt-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:12:11.954051 crawlipt-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-10 08:12:08.000000 crawlipt-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-10 08:12:08.000000 crawlipt-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-10 08:12:11.954051 crawlipt-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-10 08:12:08.000000 crawlipt-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:12:11.950051 crawlipt-0.1.3/crawlipt/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-10 08:12:08.000000 crawlipt-0.1.3/crawlipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-10 08:12:08.000000 crawlipt-0.1.3/crawlipt/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-10 08:12:08.000000 crawlipt-0.1.3/crawlipt/action.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:12:11.954051 crawlipt-0.1.3/crawlipt/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-10 08:12:08.000000 crawlipt-0.1.3/crawlipt/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-10 08:12:08.000000 crawlipt-0.1.3/crawlipt/actions/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-05-10 08:12:08.000000 crawlipt-0.1.3/crawlipt/actions/click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-10 08:12:08.000000 crawlipt-0.1.3/crawlipt/actions/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-10 08:12:08.000000 crawlipt-0.1.3/crawlipt/actions/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-10 08:12:08.000000 crawlipt-0.1.3/crawlipt/actions/redirect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-10 08:12:08.000000 crawlipt-0.1.3/crawlipt/actions/scroll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-10 08:12:08.000000 crawlipt-0.1.3/crawlipt/actions/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-10 08:12:08.000000 crawlipt-0.1.3/crawlipt/actions/slide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-10 08:12:08.000000 crawlipt-0.1.3/crawlipt/actions/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-10 08:12:08.000000 crawlipt-0.1.3/crawlipt/actions/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-10 08:12:08.000000 crawlipt-0.1.3/crawlipt/actions/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-10 08:12:08.000000 crawlipt-0.1.3/crawlipt/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-10 08:12:08.000000 crawlipt-0.1.3/crawlipt/condition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:12:11.954051 crawlipt-0.1.3/crawlipt/conditions/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-10 08:12:08.000000 crawlipt-0.1.3/crawlipt/conditions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-10 08:12:08.000000 crawlipt-0.1.3/crawlipt/conditions/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-10 08:12:08.000000 crawlipt-0.1.3/crawlipt/conditions/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-10 08:12:08.000000 crawlipt-0.1.3/crawlipt/conditions/presence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-10 08:12:08.000000 crawlipt-0.1.3/crawlipt/conditions/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-10 08:12:08.000000 crawlipt-0.1.3/crawlipt/conditions/visibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-10 08:12:08.000000 crawlipt-0.1.3/crawlipt/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-10 08:12:08.000000 crawlipt-0.1.3/crawlipt/pojo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29184 2024-05-10 08:12:08.000000 crawlipt-0.1.3/crawlipt/script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:12:11.954051 crawlipt-0.1.3/crawlipt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-10 08:12:11.000000 crawlipt-0.1.3/crawlipt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-10 08:12:11.000000 crawlipt-0.1.3/crawlipt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:12:11.000000 crawlipt-0.1.3/crawlipt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-10 08:12:11.000000 crawlipt-0.1.3/crawlipt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 08:12:11.000000 crawlipt-0.1.3/crawlipt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 08:12:11.954051 crawlipt-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-10 08:12:08.000000 crawlipt-0.1.3/setup.py
```

### Comparing `crawlipt-0.1.2/LICENSE` & `crawlipt-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `crawlipt-0.1.2/PKG-INFO` & `crawlipt-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlipt
-Version: 0.1.2
+Version: 0.1.3
 Summary: The script for selenium in python
 Home-page: https://github.com/WwwwwyDev/crawlipt
 Author: WwwwwyDev
 Author-email: wwy20001014@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: selenium>=4.0.0
 
 
 <!-- markdownlint-disable MD033 MD041 -->
 <p align="center">
-  <a href="https://github.com/WwwwwyDev/crawlipt"><img src="https://s2.loli.net/2024/04/19/1T7sZdrjbEfci8W.png" alt="crawlist" style="width:254px; height:208px" ></a>
+  <a href="https://github.com/WwwwwyDev/crawlipt"><img src="https://s2.loli.net/2024/05/10/PCcpwynVMmURjBv.png" alt="crawlist" style="width:75%; height:75%" ></a>
 </p>
 
 <div align="center">
 
 # crawlipt
 
 <!-- prettier-ignore-start -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: crawlipt Version: 0.1.2 Summary: The script for
+Metadata-Version: 2.1 Name: crawlipt Version: 0.1.3 Summary: The script for
 selenium in python Home-page: https://github.com/WwwwwyDev/crawlipt Author:
 WwwwwyDev Author-email: wwy20001014@foxmail.com License: MIT Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Requires-Python: >=3.10.0 Description-Content-Type:
```

### Comparing `crawlipt-0.1.2/README.md` & `crawlipt-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <!-- markdownlint-disable MD033 MD041 -->
 <p align="center">
-  <a href="https://github.com/WwwwwyDev/crawlipt"><img src="https://s2.loli.net/2024/04/19/1T7sZdrjbEfci8W.png" alt="crawlist" style="width:254px; height:208px" ></a>
+  <a href="https://github.com/WwwwwyDev/crawlipt"><img src="https://s2.loli.net/2024/05/10/PCcpwynVMmURjBv.png" alt="crawlist" style="width:75%; height:75%" ></a>
 </p>
 
 <div align="center">
 
 # crawlipt
 
 <!-- prettier-ignore-start -->
```

### Comparing `crawlipt-0.1.2/crawlipt/actions/alert.py` & `crawlipt-0.1.3/crawlipt/actions/alert.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.1.2/crawlipt/actions/click.py` & `crawlipt-0.1.3/crawlipt/actions/click.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 from selenium.webdriver.remote.webdriver import WebDriver
 from crawlipt.annotation import check, alias
 
 
 class Click:
     @staticmethod
     @check(exclude="driver")
-    @alias("C")
     def click(driver: WebDriver, xpath: str) -> None:
         """
         Handling click events of first element
         :param driver: selenium webdriver
         :param xpath: click on the xpath path of the button
         """
         element = driver.find_element(By.XPATH, xpath)
         element.click()
 
     @staticmethod
     @check(exclude="driver")
-    def clickMulti(driver: WebDriver, xpath: str, cnt: str | int, frequency: int = 0.1) -> None:
+    @alias("click.multi")
+    def clickMulti(driver: WebDriver, xpath: str, cnt: str | int, frequency: float = 0.1) -> None:
         """
         Handling click events of first element multiple times
         :param driver: selenium webdriver
         :param xpath: click on the xpath path of the button
         :param cnt: click count of the button
         :param frequency: click frequency of the button
         """
@@ -36,38 +36,41 @@
         while cnt:
             cnt -= 1
             element.click()
             time.sleep(random.uniform(frequency / 2, frequency))
 
     @staticmethod
     @check(exclude="driver")
+    @alias("click.js")
     def clickByJs(driver: WebDriver, xpath: str) -> None:
         """
         Handling click events of first element by js 'arguments[0].click();'
         :param driver: selenium webdriver
         :param xpath: click on the xpath path of the button
         """
         element = driver.find_element(By.XPATH, xpath)
         driver.execute_script("arguments[0].click();", element)
 
     @staticmethod
     @check(exclude="driver")
+    @alias("click.all")
     def clickAll(driver: WebDriver, xpath: str) -> None:
         """
         Handling click events of all element
         :param driver: selenium webdriver
         :param xpath: click on the xpath path of the button
         """
         elements = driver.find_elements(By.XPATH, xpath)
         for element in elements:
             if EC.element_to_be_clickable(element):
                 element.click()
 
     @staticmethod
     @check(exclude="driver")
+    @alias("click.all.js")
     def clickAllByJs(driver: WebDriver, xpath: str) -> None:
         """
         Handling click events of all element by js 'arguments[0].click();'
         :param driver: selenium webdriver
         :param xpath: click on the xpath path of the button
         """
         elements = driver.find_elements(By.XPATH, xpath)
```

### Comparing `crawlipt-0.1.2/crawlipt/actions/get.py` & `crawlipt-0.1.3/crawlipt/actions/get.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webdriver import WebDriver
 
-from crawlipt.annotation import check
+from crawlipt.annotation import check, alias
 
 
 class Get:
 
     @staticmethod
     @check(exclude="driver")
+    @alias("get.innerText")
     def getInnerText(driver: WebDriver, xpath: str) -> str:
         """
         get inner text of element
         :param driver: selenium webdriver
         :param xpath: The xpath path of the element
         """
         element = driver.find_element(By.XPATH, xpath)
         res = element.get_attribute('innerText')
         if res is None:
             res = ""
         return res
 
     @staticmethod
     @check(exclude="driver")
+    @alias("get.textContent")
     def getTextContent(driver: WebDriver, xpath: str) -> str:
         """
         get text content of element
         :param driver: selenium webdriver
         :param xpath: The xpath path of the element
         """
         element = driver.find_element(By.XPATH, xpath)
         res = element.get_attribute('textContent')
         if res is None:
             res = ""
         return res
 
     @staticmethod
     @check(exclude="driver")
+    @alias("get.attribute")
     def getAttribute(driver: WebDriver, xpath: str, name: str) -> str:
         """
         get the attribute of an element
         :param driver: selenium webdriver
         :param xpath: The xpath path of the element
         :param name: The name of the attribute
         """
```

### Comparing `crawlipt-0.1.2/crawlipt/actions/input.py` & `crawlipt-0.1.3/crawlipt/actions/input.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,30 +4,29 @@
 
 from crawlipt.annotation import check, alias
 
 
 class Input:
     @staticmethod
     @check(exclude="driver")
-    @alias("I")
     def input(driver: WebDriver, xpath: str, text: str) -> None:
         """
         Handling keyboard input events
         :param driver: selenium webdriver
         :param xpath: The xpath path of the input box
         :param text: text needs to be passed in
         """
         element = driver.find_element(By.XPATH, xpath)
         element.send_keys(text)
 
     @staticmethod
     @check(exclude="driver")
-    @alias("E")
     def enter(driver: WebDriver, xpath: str) -> None:
         """
         Press the enter key once
         :param driver: selenium webdriver
         :param xpath: The xpath path of the input box
         :return: Whether successful
         """
         element = driver.find_element(By.XPATH, xpath)
         element.send_keys(Keys.RETURN)
+
```

### Comparing `crawlipt-0.1.2/crawlipt/actions/redirect.py` & `crawlipt-0.1.3/crawlipt/actions/redirect.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,37 +3,38 @@
 
 from crawlipt.annotation import check, alias
 
 
 class Redirect:
     @staticmethod
     @check(exclude="driver")
+    @alias("redirect.search")
     def searchRedirect(driver: WebDriver, url: str, keyword: str) -> None:
         """
         Replace % s in the path with keyword and redirect it
         :param driver:  selenium webdriver
         :param url: Link containing %s
         :param keyword: keyword needs to be passed in
         """
         url = url.replace(r"%s", keyword)
         driver.get(url)
 
     @staticmethod
     @check(exclude="driver")
-    @alias("R")
     def redirect(driver: WebDriver, url: str) -> None:
         """
         Direct redirection
         :param driver:  selenium webdriver
         :param url: Links that require redirection
         """
         driver.get(url)
 
     @staticmethod
     @check(exclude="driver")
+    @alias("redirect.new")
     def redirectNewTab(driver: WebDriver, url: str) -> None:
         """
         redirect to a new tab
         :param driver:  selenium webdriver
         :param url: Links that require redirection
         """
         js = f'window.open("{url}")'
```

### Comparing `crawlipt-0.1.2/crawlipt/actions/select.py` & `crawlipt-0.1.3/crawlipt/actions/select.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.support.select import Select as WebSelect
-from crawlipt.annotation import check
+from crawlipt.annotation import check, alias
 
 
 class Select:
     @staticmethod
     @check(exclude="driver")
+    @alias("select.text")
     def selectByText(driver: WebDriver, xpath: str, text: str) -> None:
         """
         Handling select events
         :param driver: selenium webdriver
         :param xpath: the xpath path of the select element
         :param text: the text of selecting
         """
         select = WebSelect(driver.find_element(By.XPATH, xpath))
         select.select_by_visible_text(text)
 
     @staticmethod
     @check(exclude="driver")
+    @alias("select.value")
     def selectByValue(driver: WebDriver, xpath: str, value: str) -> None:
         """
         Handling select events
         :param driver: selenium webdriver
         :param xpath: the xpath path of the select element
         :param value: the value of selecting
         """
         select = WebSelect(driver.find_element(By.XPATH, xpath))
         select.select_by_value(value)
 
     @staticmethod
     @check(exclude="driver")
+    @alias("select.index")
     def selectByIndex(driver: WebDriver, xpath: str, index: int) -> None:
         """
         Handling select events
         :param driver: selenium webdriver
         :param xpath: the xpath path of the select element
         :param index: the index of selecting
         """
```

### Comparing `crawlipt-0.1.2/crawlipt/actions/slide.py` & `crawlipt-0.1.3/crawlipt/actions/slide.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.1.2/crawlipt/actions/switch.py` & `crawlipt-0.1.3/crawlipt/actions/switch.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,52 @@
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webdriver import WebDriver
-from crawlipt.annotation import check
+from crawlipt.annotation import check, alias
 
 
 class Switch:
     @staticmethod
     @check(exclude="driver")
+    @alias("switch.tab.last")
     def switchLastTab(driver: WebDriver) -> None:
         """
         Switch to the last handle
         :param driver: selenium webdriver
         """
         window_handles = driver.window_handles
         driver.switch_to.window(window_handles[-1])
 
     @staticmethod
     @check(exclude="driver")
+    @alias("switch.tab")
     def switchTab(driver: WebDriver, index: int | str) -> None:
         """
         Switch to the index handle
         :param driver: selenium webdriver
         :param index: The index handle
         """
         if isinstance(index, str):
             index = int(index)
         window_handles = driver.window_handles
         driver.switch_to.window(window_handles[index])
 
     @staticmethod
     @check(exclude="driver")
+    @alias("switch.frame")
     def switchToFrame(driver: WebDriver, xpath: str) -> None:
         """
         Switch to the inner frame
         :param driver: selenium webdriver
         :param xpath: The xpath of frame
         """
         frame = driver.find_element(By.XPATH, xpath)
         driver.switch_to.frame(frame)
 
     @staticmethod
     @check(exclude="driver")
+    @alias("switch.frame.out")
     def switchOutFrame(driver: WebDriver) -> None:
         """
         Switch to the outer frame
         :param driver: selenium webdriver
         """
         driver.switch_to.parent_frame()
```

### Comparing `crawlipt-0.1.2/crawlipt/actions/util.py` & `crawlipt-0.1.3/crawlipt/actions/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import random
 import time
+from typing import Any
 
 from selenium.webdriver.remote.webdriver import WebDriver
 
-from crawlipt.annotation import check
+from crawlipt.annotation import check, alias
 
 
 class Util:
 
     @staticmethod
     @check(exclude="driver")
-    def log(driver: WebDriver, msg: str) -> None:
+    def log(driver: WebDriver, msg: Any) -> None:
         """
         log the msg on the console
         :param driver: selenium webdriver
         :param msg: message to log
         """
         if not driver:
             return
@@ -32,18 +33,31 @@
             return
         if isinstance(num, str):
             num = int(num)
         time.sleep(num)
 
     @staticmethod
     @check(exclude="driver")
+    @alias("interval.random")
     def intervalRandom(driver: WebDriver, num: str | int) -> None:
         """
         delay [num/2, num] seconds
         :param driver: selenium webdriver
         :param num: the interval number
         """
         if not driver:
             return
         if isinstance(num, str):
             num = int(num)
-        time.sleep(random.uniform(num/2, num))
+        time.sleep(random.uniform(num / 2, num))
+
+    @staticmethod
+    @check(exclude="driver")
+    def execute(driver: WebDriver, js: str) -> Any:
+        """
+        execute the js code
+        :param driver: selenium webdriver
+        :param js: str of js code text
+        """
+        return driver.execute_script(js)
+
+
```

### Comparing `crawlipt-0.1.2/crawlipt/actions/window.py` & `crawlipt-0.1.3/crawlipt/actions/window.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     @check(exclude="driver")
     @alias("window.clear")
     def clear(driver: WebDriver) -> None:
         """
         close all windows
         :param driver: selenium webdriver
         """
-        for _ in range(driver.window_handles.__len__()-1):
+        for _ in range(driver.window_handles.__len__() - 1):
             driver.close()
         driver.get("data:,")
 
     @staticmethod
     @check(exclude="driver")
     @alias("window.back")
     def back(driver: WebDriver) -> None:
@@ -51,7 +51,17 @@
     @alias("window.url")
     def url(driver: WebDriver) -> str:
         """
         return the current url
         :param driver: selenium webdriver
         """
         return driver.current_url
+
+    @staticmethod
+    @check(exclude="driver")
+    @alias("window.html")
+    def html(driver: WebDriver) -> str:
+        """
+        return the current page source
+        :param driver: selenium webdriver
+        """
+        return driver.page_source
```

### Comparing `crawlipt-0.1.2/crawlipt/annotation.py` & `crawlipt-0.1.3/crawlipt/annotation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from inspect import signature
 from functools import wraps
+from typing import Any
+
 from crawlipt.error import ParamTypeError
 
 
 def check(exclude: list | str):
     """
     Turn the function into a strongly typed function, check if the parameter type is legal, and if not, directly assert.
     \n You could use @check to Turn the function into a strongly typed function.
@@ -47,14 +49,16 @@
                     continue
                 if all_kwargs[name] == "__PRE_RETURN__":
                     continue
                 if isinstance(all_kwargs[name], str) and all_kwargs[name].startswith("__rf-") and all_kwargs[name].endswith("__"):
                     continue
                 if isinstance(all_kwargs[name], str) and all_kwargs[name].startswith("__v-") and all_kwargs[name].endswith("__"):
                     continue
+                if type_.annotation is Any:
+                    continue
                 if isinstance(all_kwargs[name], int) and type_.annotation is float:
                     all_kwargs[name] = float(all_kwargs.get(name))
                 if not isinstance(all_kwargs[name], type_.annotation):
                     raise ParamTypeError(f"Parameter {name} must be {type_.annotation}.")
             return func(*args, **kwargs)
 
         return inner_wrapper
```

### Comparing `crawlipt-0.1.2/crawlipt/conditions/element.py` & `crawlipt-0.1.3/crawlipt/conditions/element.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.1.2/crawlipt/conditions/frame.py` & `crawlipt-0.1.3/crawlipt/conditions/frame.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.1.2/crawlipt/conditions/presence.py` & `crawlipt-0.1.3/crawlipt/conditions/presence.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.1.2/crawlipt/conditions/text.py` & `crawlipt-0.1.3/crawlipt/conditions/text.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.1.2/crawlipt/conditions/visibility.py` & `crawlipt-0.1.3/crawlipt/conditions/visibility.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.1.2/crawlipt/pojo.py` & `crawlipt-0.1.3/crawlipt/pojo.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.1.2/crawlipt/script.py` & `crawlipt-0.1.3/crawlipt/script.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,14 +96,16 @@
             for key, value in temp_args.items():
                 if isinstance(value, str) and value.startswith("__rf-") and value.endswith("__"):
                     if value[5:-2] not in return_record.keys():
                         msg = f"The return_flag:{value[5:-2]} cannot be find in history record."
                         raise ScriptSyntaxError(ParamTypeError(msg), condition, pre_deep + str(current_deep))
                     annotation = signature(ScriptProcess.CONDITIONS[condition]).parameters[key].annotation
                     pre_return_flag = return_record[value[5:-2]]
+                    if pre_return_flag is Any or annotation is Any:
+                        continue
                     if pre_return_flag != annotation:
                         msg = f"The return_flag is {pre_return_flag}, But parameter {key} is {annotation}."
                         raise ScriptSyntaxError(ParamTypeError(msg), condition, pre_deep + str(current_deep))
         try:
             if return_flag:
                 return_record[return_flag] = signature(ScriptProcess.CONDITIONS[condition]).return_annotation
             ScriptProcess.CONDITIONS[condition](**temp_args)
@@ -182,25 +184,29 @@
                     temp_args[key] = value
             if "store" in signature(ScriptProcess.ACTIONS[method]).parameters:
                 temp_args["store"] = None
             if pre_return is not None:
                 for key, value in temp_args.items():
                     if value == "__PRE_RETURN__":
                         annotation = signature(ScriptProcess.ACTIONS[method]).parameters[key].annotation
+                        if pre_return is Any or annotation is Any:
+                            continue
                         if pre_return != annotation:
                             msg = f"The pre-return is {pre_return}, But parameter {key} is {annotation}."
                             raise ScriptSyntaxError(ParamTypeError(msg), method, pre_deep + str(current_deep))
             if return_record:
                 for key, value in temp_args.items():
                     if isinstance(value, str) and value.startswith("__rf-") and value.endswith("__"):
                         if value[5:-2] not in return_record.keys():
                             msg = f"The return_flag:{value[5:-2]} cannot be find in history record."
                             raise ScriptSyntaxError(ParamTypeError(msg), method, pre_deep + str(current_deep))
                         annotation = signature(ScriptProcess.ACTIONS[method]).parameters[key].annotation
                         pre_return_flag = return_record[value[5:-2]]
+                        if pre_return_flag is Any or annotation is Any:
+                            continue
                         if pre_return_flag != annotation:
                             msg = f"The return_flag is {pre_return_flag}, But parameter {key} is {annotation}."
                             raise ScriptSyntaxError(ParamTypeError(msg), method, pre_deep + str(current_deep))
             try:
                 if signature(ScriptProcess.ACTIONS[method]).return_annotation is not None:
                     pre_return = signature(ScriptProcess.ACTIONS[method]).return_annotation
                 if return_flag:
@@ -238,14 +244,15 @@
         if not is_success:
             fail_script = temp_condition.get("fail_script")
             if fail_script:
                 ScriptProcess._process_script(script=fail_script,
                                               global_script=global_script,
                                               webdriver=webdriver,
                                               interval=interval,
+                                              return_record=return_record,
                                               wait=wait,
                                               store=store,)
         return is_success
 
     @staticmethod
     @check
     def _process_script(script: dict, global_script: dict, webdriver: WebDriver, store: StoreBase = None,
@@ -435,23 +442,28 @@
             if not issubclass(signature(func).parameters["store"].annotation, StoreBase):
                 raise ParamTypeError("the 'store' parameter must be a subclass of StoreBase")
         if signature(func).parameters["driver"].annotation is not WebDriver:
             raise ParamTypeError("the 'driver' parameter must be a WebDriver of selenium.")
         for name in signature(func).parameters.keys():
             if name in ScriptProcess.__POP_KEY:
                 raise ParamTypeError(f"the parameter name: {name} conflicts with the keyword")
+        cnt = 0
         if func.__name__ not in ScriptProcess.ACTIONS:
+            cnt += 1
             ScriptProcess.ACTIONS[func.__name__] = func
         func_bak = func
         try:
             func = func.__func__
         except Exception:
             pass
         if "__crawlipt_func_name__" in func.__dict__:
+            cnt += 1
             ScriptProcess.ACTIONS[func.__crawlipt_func_name__] = func_bak
+        if not cnt:
+            raise ParamTypeError(f"Add failed")
 
     @staticmethod
     def add_condition(func: callable) -> None:
         """
         add your own condition
         """
         if not callable(func):
@@ -467,23 +479,28 @@
         if signature(func).parameters["driver"].annotation is not WebDriver:
             raise ParamTypeError("the 'driver' parameter must be a WebDriver of selenium.")
         if signature(func).return_annotation is not bool:
             raise ParamTypeError("the return of func must be the type of bool.")
         for name in signature(func).parameters.keys():
             if name in ScriptProcess.__POP_KEY:
                 raise ParamTypeError(f"the parameter name: {name} conflicts with the keyword")
+        cnt = 0
         if func.__name__ not in ScriptProcess.CONDITIONS:
+            cnt += 1
             ScriptProcess.CONDITIONS[func.__name__] = func
         func_bak = func
         try:
             func = func.__func__
         except Exception:
             pass
         if "__crawlipt_func_name__" in func.__dict__:
+            cnt += 1
             ScriptProcess.CONDITIONS[func.__crawlipt_func_name__] = func_bak
+        if not cnt:
+            raise ParamTypeError(f"Add failed")
 
 
 class Script(ScriptProcess):
 
     @check
     def __init__(self, script: dict | str | list, global_script: dict | str | list = None, interval: float = 0.5,
                  wait: float = 10, is_need_syntax_check: bool = True):
```

### Comparing `crawlipt-0.1.2/crawlipt.egg-info/PKG-INFO` & `crawlipt-0.1.3/crawlipt.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlipt
-Version: 0.1.2
+Version: 0.1.3
 Summary: The script for selenium in python
 Home-page: https://github.com/WwwwwyDev/crawlipt
 Author: WwwwwyDev
 Author-email: wwy20001014@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: selenium>=4.0.0
 
 
 <!-- markdownlint-disable MD033 MD041 -->
 <p align="center">
-  <a href="https://github.com/WwwwwyDev/crawlipt"><img src="https://s2.loli.net/2024/04/19/1T7sZdrjbEfci8W.png" alt="crawlist" style="width:254px; height:208px" ></a>
+  <a href="https://github.com/WwwwwyDev/crawlipt"><img src="https://s2.loli.net/2024/05/10/PCcpwynVMmURjBv.png" alt="crawlist" style="width:75%; height:75%" ></a>
 </p>
 
 <div align="center">
 
 # crawlipt
 
 <!-- prettier-ignore-start -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: crawlipt Version: 0.1.2 Summary: The script for
+Metadata-Version: 2.1 Name: crawlipt Version: 0.1.3 Summary: The script for
 selenium in python Home-page: https://github.com/WwwwwyDev/crawlipt Author:
 WwwwwyDev Author-email: wwy20001014@foxmail.com License: MIT Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Requires-Python: >=3.10.0 Description-Content-Type:
```

### Comparing `crawlipt-0.1.2/crawlipt.egg-info/SOURCES.txt` & `crawlipt-0.1.3/crawlipt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crawlipt-0.1.2/setup.py` & `crawlipt-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'crawlipt'
 DESCRIPTION = 'The script for selenium in python'
 URL = 'https://github.com/WwwwwyDev/crawlipt'
 EMAIL = 'wwy20001014@foxmail.com'
 AUTHOR = 'WwwwwyDev'
 REQUIRES_PYTHON = '>=3.10.0'
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "selenium>=4.0.0"
 ]
 
 # What packages are optional?
```

