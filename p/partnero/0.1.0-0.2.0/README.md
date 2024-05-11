# Comparing `tmp/partnero-0.1.0.tar.gz` & `tmp/partnero-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "partnero-0.1.0.tar", max compression
+gzip compressed data, was "partnero-0.2.0.tar", max compression
```

## Comparing `partnero-0.1.0.tar` & `partnero-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2024-05-08 20:40:12.678382 partnero-0.1.0/README.md
--rw-r--r--   0        0        0      280 2024-05-08 17:26:41.216816 partnero-0.1.0/partnero/__init__.py
--rw-r--r--   0        0        0      300 2024-05-08 16:20:35.149516 partnero-0.1.0/partnero/authentication.py
--rw-r--r--   0        0        0     1312 2024-05-08 18:07:06.986275 partnero-0.1.0/partnero/base_api.py
--rw-r--r--   0        0        0     1284 2024-05-08 16:33:28.222508 partnero-0.1.0/partnero/coupon_api.py
--rw-r--r--   0        0        0     2700 2024-05-08 19:59:47.860354 partnero-0.1.0/partnero/customer_api.py
--rw-r--r--   0        0        0     1607 2024-05-08 19:50:23.319651 partnero-0.1.0/partnero/partner_api.py
--rw-r--r--   0        0        0      960 2024-05-08 16:33:53.721224 partnero-0.1.0/partnero/promotion_code_api.py
--rw-r--r--   0        0        0      863 2024-05-08 16:32:27.832217 partnero-0.1.0/partnero/transaction_api.py
--rw-r--r--   0        0        0      320 2024-05-08 16:07:55.023365 partnero-0.1.0/partnero/utils.py
--rw-r--r--   0        0        0     1140 2024-05-08 16:33:08.677141 partnero-0.1.0/partnero/webhook_api.py
--rw-r--r--   0        0        0      336 2024-05-08 20:52:14.294911 partnero-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 partnero-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3206 2024-05-11 01:49:12.829698 partnero-0.2.0/README.md
+-rw-r--r--   0        0        0      434 2024-05-11 01:49:12.829698 partnero-0.2.0/partnero/__init__.py
+-rw-r--r--   0        0        0      712 2024-05-11 01:49:12.829698 partnero-0.2.0/partnero/authentication.py
+-rw-r--r--   0        0        0     1892 2024-05-11 01:49:12.829698 partnero-0.2.0/partnero/base_api.py
+-rw-r--r--   0        0        0     1284 2024-05-11 01:49:12.829698 partnero-0.2.0/partnero/coupon_api.py
+-rw-r--r--   0        0        0     2701 2024-05-11 01:49:12.833698 partnero-0.2.0/partnero/customer_api.py
+-rw-r--r--   0        0        0     1607 2024-05-11 01:49:12.833698 partnero-0.2.0/partnero/partner_api.py
+-rw-r--r--   0        0        0      960 2024-05-11 01:49:12.833698 partnero-0.2.0/partnero/promotion_code_api.py
+-rw-r--r--   0        0        0      863 2024-05-11 01:49:12.833698 partnero-0.2.0/partnero/transaction_api.py
+-rw-r--r--   0        0        0      320 2024-05-11 01:49:12.833698 partnero-0.2.0/partnero/utils.py
+-rw-r--r--   0        0        0     1140 2024-05-11 01:49:12.833698 partnero-0.2.0/partnero/webhook_api.py
+-rw-r--r--   0        0        0      919 2024-05-11 01:49:12.833698 partnero-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3684 1970-01-01 00:00:00.000000 partnero-0.2.0/PKG-INFO
```

### Comparing `partnero-0.1.0/partnero/coupon_api.py` & `partnero-0.2.0/partnero/coupon_api.py`

 * *Files identical despite different names*

### Comparing `partnero-0.1.0/partnero/customer_api.py` & `partnero-0.2.0/partnero/customer_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         """
         validate_email(email)
         validate_key(partner_key, "partner_key")
         validate_key(customer_key, "customer_key")
         data = {'partner': {'key': partner_key}, 'key': customer_key, 'email': email, 'name': name}
         return self.send_request('POST', 'customers', data=data)
 
-    def get_partner(self, email: str = None, customer_key: str = None) -> dict:
+    def get_customer(self, email: str = None, customer_key: str = None) -> dict:
         """
         Search for partners based on provided parameters. Parameters are optional.
         :param email: Email of the customer to search for.
         :param customer_key: ID of the customer to search for.
         """
         params = {k: v for k, v in [('email', email), ('key', customer_key)] if v is not None}
         return self.send_request('GET', 'customers:search', params=params)
```

### Comparing `partnero-0.1.0/partnero/partner_api.py` & `partnero-0.2.0/partnero/partner_api.py`

 * *Files identical despite different names*

### Comparing `partnero-0.1.0/partnero/promotion_code_api.py` & `partnero-0.2.0/partnero/promotion_code_api.py`

 * *Files identical despite different names*

### Comparing `partnero-0.1.0/partnero/transaction_api.py` & `partnero-0.2.0/partnero/transaction_api.py`

 * *Files identical despite different names*

### Comparing `partnero-0.1.0/partnero/webhook_api.py` & `partnero-0.2.0/partnero/webhook_api.py`

 * *Files identical despite different names*

