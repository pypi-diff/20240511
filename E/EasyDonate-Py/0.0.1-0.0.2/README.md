# Comparing `tmp/easydonate_py-0.0.1.tar.gz` & `tmp/easydonate_py-0.0.2.tar.gz`

## Comparing `easydonate_py-0.0.1.tar` & `easydonate_py-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 easydonate_py-0.0.1/src/EasyDonate_Py/__init__.py
--rw-r--r--   0        0        0     9153 2020-02-02 00:00:00.000000 easydonate_py-0.0.1/src/EasyDonate_Py/plugins.py
--rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 easydonate_py-0.0.1/src/EasyDonate_Py/shop.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 easydonate_py-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 easydonate_py-0.0.1/README.md
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 easydonate_py-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 easydonate_py-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 easydonate_py-0.0.2/src/EasyDonate_Py/__init__.py
+-rw-r--r--   0        0        0     8248 2020-02-02 00:00:00.000000 easydonate_py-0.0.2/src/EasyDonate_Py/plugins.py
+-rw-r--r--   0        0        0     5321 2020-02-02 00:00:00.000000 easydonate_py-0.0.2/src/EasyDonate_Py/shop.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 easydonate_py-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 easydonate_py-0.0.2/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 easydonate_py-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 easydonate_py-0.0.2/PKG-INFO
```

### Comparing `easydonate_py-0.0.1/src/EasyDonate_Py/plugins.py` & `easydonate_py-0.0.2/src/EasyDonate_Py/plugins.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,207 +1,207 @@
 import requests
 
-class additional_payment():
-    def additional_payment_settings(shop_key):
-        url = "https://easydonate.ru/api/v3/plugin/EasyDonate.Surcharge/getSettings"
-        headers={"Shop-Key": shop_key}
-        response = requests.get(url=url, headers=headers)
-        if response.status_code == 200:
-            data = response.json()
-            if data["success"] == "true":
-                return data
-            else:
-                print("Возможно плагин отключен.")
-        else:
-            print({'error': f"Ошибка: {response.status_code}"})
-    def additional_payment_user(shop_key, username):
-        url = "https://easydonate.ru/api/v3/plugin/EasyDonate.Surcharge/getDiscounts"
-        headers={"Shop-Key": shop_key}
-        params={'username': username}
-        response = requests.get(url=url, headers=headers, params=params)
-        if response.status_code == 200:
-            data = response.json()
-            if data["success"] == "true":
-                return data
-            else:
-                print("Возможно плагин отключен.")
-        else:
-            print({'error': f"Ошибка: {response.status_code}"})
-    def additional_payment_id(shop_key, username, product_id):
-        url = "https://easydonate.ru/api/v3/plugin/EasyDonate.Surcharge/getDiscounts"
-        headers={"Shop-Key": shop_key}
-        params={'username': username, 'product_id': product_id}
-        response = requests.get(url=url, headers=headers, params=params)
-        if response.status_code == 200:
-            data = response.json()
-            if data["success"] == "true":
-                return data
-            else:
-                print("Возможно плагин отключен.")
-        else:
-            print({'error': f"Ошибка: {response.status_code}"})
-
-class last_payments():
-    def last_payments_settings(shop_key):
-        url = "https://easydonate.ru/api/v3/plugin/EasyDonate.LastPayments/getSettings"
-        headers={"Shop-Key": shop_key}
-        response = requests.get(url=url, headers=headers)
-        if response.status_code == 200:
-            data = response.json()
-            if data["success"] == "true":
-                return data
-            else:
-                print("Возможно плагин отключен.")
-        else:
-            print({'error': f"Ошибка: {response.status_code}"})
-    def last_payments_get(shop_key):
-        url = "https://easydonate.ru/api/v3/plugin/EasyDonate.LastPayments/getPayments"
-        headers={"Shop-Key": shop_key}
-        response = requests.get(url=url, headers=headers)
-        if response.status_code == 200:
-            data = response.json()
-            if data["success"] == "true":
-                return data
-            else:
-                print("Возможно плагин отключен.")
-        else:
-            print({'error': f"Ошибка: {response.status_code}"})
-
-class custom_message():
-    def custom_message_settings(shop_key):
-        url = "https://easydonate.ru/api/v3/plugin/EasyDonate.CustomMessages/getSettings"
-        headers={"Shop-Key": shop_key}
-        response = requests.get(url=url, headers=headers)
-        if response.status_code == 200:
-            data = response.json()
-            if data["success"] == "true":
-                return data
-            else:
-                print("Возможно плагин отключен.")
-        else:
-            print({'error': f"Ошибка: {response.status_code}"})
-
-class discord_widget():
-    def discord_widget_settings(shop_key):
-        url = "https://easydonate.ru/api/v3/plugin/Discord.Widget/getSettings"
-        headers={"Shop-Key": shop_key}
-        response = requests.get(url=url, headers=headers)
-        if response.status_code == 200:
-            data = response.json()
-            if data["success"] == "true":
-                return data
-            else:
-                print("Возможно плагин отключен.")
-        else:
-            print({'error': f"Ошибка: {response.status_code}"})
-    def discord_widget_get(shop_key):
-        url = "https://easydonate.ru/api/v3/plugin/Discord.Widget/getEmbed"
-        headers={"Shop-Key": shop_key}
-        response = requests.get(url=url, headers=headers)
-        if response.status_code == 200:
-            data = response.json()
-            if data["success"] == "true":
-                return data
-            else:
-                print("Возможно плагин отключен.")
-        else:
-            print({'error': f"Ошибка: {response.status_code}"})
-
-class vk():
-    def vk_widget_settings(shop_key):
-        url = "https://easydonate.ru/api/v3/plugin/Vkontakte.Widget/getSettings"
-        headers={"Shop-Key": shop_key}
-        response = requests.get(url=url, headers=headers)
-        if response.status_code == 200:
-            data = response.json()
-            if data["success"] == "true":
-                return data
-            else:
-                print("Возможно плагин отключен.")
-        else:
-            print({'error': f"Ошибка: {response.status_code}"})
-    def vk_widget_get(shop_key):
-        url = "https://easydonate.ru/api/v3/plugin/Vkontakte.Widget/getEmbed"
-        headers={"Shop-Key": shop_key}
-        response = requests.get(url=url, headers=headers)
-        if response.status_code == 200:
-            data = response.json()
-            if data["success"] == "true":
-                return data
-            else:
-                print("Возможно плагин отключен.")
-        else:
-            print({'error': f"Ошибка: {response.status_code}"})
-    def vk_news_settings(shop_key):
-        url = "https://easydonate.ru/api/v3/plugin/Vkontakte.News/getSettings"
-        headers={"Shop-Key": shop_key}
-        response = requests.get(url=url, headers=headers)
-        if response.status_code == 200:
-            data = response.json()
-            if data["success"] == "true":
-                return data
-            else:
-                print("Возможно плагин отключен.")
-        else:
-            print({'error': f"Ошибка: {response.status_code}"})
-    def vk_news_get(shop_key):
-        url = "https://easydonate.ru/api/v3/plugin/Vkontakte.News/getNews"
-        headers={"Shop-Key": shop_key}
-        response = requests.get(url=url, headers=headers)
-        if response.status_code == 200:
-            data = response.json()
-            if data["success"] == "true":
-                return data
-            else:
-                print("Возможно плагин отключен.")
-        else:
-            print({'error': f"Ошибка: {response.status_code}"})
-    def vk_messages_settings(shop_key):
-        url = "https://easydonate.ru/api/v3/plugin/Vkontakte.MessagesWidget/getSettings"
-        headers={"Shop-Key": shop_key}
-        response = requests.get(url=url, headers=headers)
-        if response.status_code == 200:
-            data = response.json()
-            if data["success"] == "true":
-                return data
-            else:
-                print("Возможно плагин отключен.")
-        else:
-            print({'error': f"Ошибка: {response.status_code}"})
-    def vk_messages_widget(shop_key):
-        url = "https://easydonate.ru/api/v3/plugin/Vkontakte.MessagesWidget/getEmbed"
-        headers={"Shop-Key": shop_key}
-        response = requests.get(url=url, headers=headers)
-        if response.status_code == 200:
-            data = response.json()
-            if data["success"] == "true":
-                return data
-            else:
-                print("Возможно плагин отключен.")
-        else:
-            print({'error': f"Ошибка: {response.status_code}"})
-
-class yandex_metrika():
-    def yandex_metrika_settings(shop_key):
-        url = "https://easydonate.ru/api/v3/plugin/Yandex.Metrika/getSettings"
-        headers={"Shop-Key": shop_key}
-        response = requests.get(url=url, headers=headers)
-        if response.status_code == 200:
-            data = response.json()
-            if data["success"] == "true":
-                return data
-            else:
-                print("Возможно плагин отключен.")
-        else:
-            print({'error': f"Ошибка: {response.status_code}"})
-    def yandex_metrika_widget(shop_key):
-        url = "https://easydonate.ru/api/v3/plugin/Yandex.Metrika/getEmbed"
-        headers={"Shop-Key": shop_key}
-        response = requests.get(url=url, headers=headers)
-        if response.status_code == 200:
-            data = response.json()
-            if data["success"] == "true":
-                return data
-            else:
-                print("Возможно плагин отключен.")
-        else:
-            print({'error': f"Ошибка: {response.status_code}"})
+
+def additional_payment_settings(shop_key):
+    url = "https://easydonate.ru/api/v3/plugin/EasyDonate.Surcharge/getSettings"
+    headers={"Shop-Key": shop_key}
+    response = requests.get(url=url, headers=headers)
+    if response.status_code == 200:
+        data = response.json()
+        if data["success"] == "true":
+            return data
+        else:
+            print("Возможно плагин отключен.")
+    else:
+        print({'error': f"Ошибка: {response.status_code}"})
+def additional_payment_user(shop_key, username):
+    url = "https://easydonate.ru/api/v3/plugin/EasyDonate.Surcharge/getDiscounts"
+    headers={"Shop-Key": shop_key}
+    params={'username': username}
+    response = requests.get(url=url, headers=headers, params=params)
+    if response.status_code == 200:
+        data = response.json()
+        if data["success"] == "true":
+            return data
+        else:
+            print("Возможно плагин отключен.")
+    else:
+        print({'error': f"Ошибка: {response.status_code}"})
+def additional_payment_id(shop_key, username, product_id):
+    url = "https://easydonate.ru/api/v3/plugin/EasyDonate.Surcharge/getDiscounts"
+    headers={"Shop-Key": shop_key}
+    params={'username': username, 'product_id': product_id}
+    response = requests.get(url=url, headers=headers, params=params)
+    if response.status_code == 200:
+        data = response.json()
+        if data["success"] == "true":
+            return data
+        else:
+            print("Возможно плагин отключен.")
+    else:
+        print({'error': f"Ошибка: {response.status_code}"})
+
+
+def last_payments_settings(shop_key):
+    url = "https://easydonate.ru/api/v3/plugin/EasyDonate.LastPayments/getSettings"
+    headers={"Shop-Key": shop_key}
+    response = requests.get(url=url, headers=headers)
+    if response.status_code == 200:
+        data = response.json()
+        if data["success"] == "true":
+            return data
+        else:
+            print("Возможно плагин отключен.")
+    else:
+        print({'error': f"Ошибка: {response.status_code}"})
+def last_payments_get(shop_key):
+    url = "https://easydonate.ru/api/v3/plugin/EasyDonate.LastPayments/getPayments"
+    headers={"Shop-Key": shop_key}
+    response = requests.get(url=url, headers=headers)
+    if response.status_code == 200:
+        data = response.json()
+        if data["success"] == "true":
+            return data
+        else:
+            print("Возможно плагин отключен.")
+    else:
+        print({'error': f"Ошибка: {response.status_code}"})
+
+
+def custom_message_settings(shop_key):
+    url = "https://easydonate.ru/api/v3/plugin/EasyDonate.CustomMessages/getSettings"
+    headers={"Shop-Key": shop_key}
+    response = requests.get(url=url, headers=headers)
+    if response.status_code == 200:
+        data = response.json()
+        if data["success"] == "true":
+            return data
+        else:
+            print("Возможно плагин отключен.")
+    else:
+        print({'error': f"Ошибка: {response.status_code}"})
+
+
+def discord_widget_settings(shop_key):
+    url = "https://easydonate.ru/api/v3/plugin/Discord.Widget/getSettings"
+    headers={"Shop-Key": shop_key}
+    response = requests.get(url=url, headers=headers)
+    if response.status_code == 200:
+        data = response.json()
+        if data["success"] == "true":
+            return data
+        else:
+            print("Возможно плагин отключен.")
+    else:
+        print({'error': f"Ошибка: {response.status_code}"})
+def discord_widget_get(shop_key):
+    url = "https://easydonate.ru/api/v3/plugin/Discord.Widget/getEmbed"
+    headers={"Shop-Key": shop_key}
+    response = requests.get(url=url, headers=headers)
+    if response.status_code == 200:
+        data = response.json()
+        if data["success"] == "true":
+            return data
+        else:
+            print("Возможно плагин отключен.")
+    else:
+        print({'error': f"Ошибка: {response.status_code}"})
+
+
+def vk_widget_settings(shop_key):
+    url = "https://easydonate.ru/api/v3/plugin/Vkontakte.Widget/getSettings"
+    headers={"Shop-Key": shop_key}
+    response = requests.get(url=url, headers=headers)
+    if response.status_code == 200:
+        data = response.json()
+        if data["success"] == "true":
+            return data
+        else:
+            print("Возможно плагин отключен.")
+    else:
+        print({'error': f"Ошибка: {response.status_code}"})
+def vk_widget_get(shop_key):
+    url = "https://easydonate.ru/api/v3/plugin/Vkontakte.Widget/getEmbed"
+    headers={"Shop-Key": shop_key}
+    response = requests.get(url=url, headers=headers)
+    if response.status_code == 200:
+        data = response.json()
+        if data["success"] == "true":
+            return data
+        else:
+            print("Возможно плагин отключен.")
+    else:
+        print({'error': f"Ошибка: {response.status_code}"})
+def vk_news_settings(shop_key):
+    url = "https://easydonate.ru/api/v3/plugin/Vkontakte.News/getSettings"
+    headers={"Shop-Key": shop_key}
+    response = requests.get(url=url, headers=headers)
+    if response.status_code == 200:
+        data = response.json()
+        if data["success"] == "true":
+            return data
+        else:
+            print("Возможно плагин отключен.")
+    else:
+        print({'error': f"Ошибка: {response.status_code}"})
+def vk_news_get(shop_key):
+    url = "https://easydonate.ru/api/v3/plugin/Vkontakte.News/getNews"
+    headers={"Shop-Key": shop_key}
+    response = requests.get(url=url, headers=headers)
+    if response.status_code == 200:
+        data = response.json()
+        if data["success"] == "true":
+            return data
+        else:
+            print("Возможно плагин отключен.")
+    else:
+        print({'error': f"Ошибка: {response.status_code}"})
+def vk_messages_settings(shop_key):
+    url = "https://easydonate.ru/api/v3/plugin/Vkontakte.MessagesWidget/getSettings"
+    headers={"Shop-Key": shop_key}
+    response = requests.get(url=url, headers=headers)
+    if response.status_code == 200:
+        data = response.json()
+        if data["success"] == "true":
+            return data
+        else:
+            print("Возможно плагин отключен.")
+    else:
+        print({'error': f"Ошибка: {response.status_code}"})
+def vk_messages_widget(shop_key):
+    url = "https://easydonate.ru/api/v3/plugin/Vkontakte.MessagesWidget/getEmbed"
+    headers={"Shop-Key": shop_key}
+    response = requests.get(url=url, headers=headers)
+    if response.status_code == 200:
+        data = response.json()
+        if data["success"] == "true":
+            return data
+        else:
+            print("Возможно плагин отключен.")
+    else:
+        print({'error': f"Ошибка: {response.status_code}"})
+
+
+def yandex_metrika_settings(shop_key):
+    url = "https://easydonate.ru/api/v3/plugin/Yandex.Metrika/getSettings"
+    headers={"Shop-Key": shop_key}
+    response = requests.get(url=url, headers=headers)
+    if response.status_code == 200:
+        data = response.json()
+        if data["success"] == "true":
+            return data
+        else:
+            print("Возможно плагин отключен.")
+    else:
+        print({'error': f"Ошибка: {response.status_code}"})
+def yandex_metrika_widget(shop_key):
+    url = "https://easydonate.ru/api/v3/plugin/Yandex.Metrika/getEmbed"
+    headers={"Shop-Key": shop_key}
+    response = requests.get(url=url, headers=headers)
+    if response.status_code == 200:
+        data = response.json()
+        if data["success"] == "true":
+            return data
+        else:
+            print("Возможно плагин отключен.")
+    else:
+        print({'error': f"Ошибка: {response.status_code}"})
```

### Comparing `easydonate_py-0.0.1/src/EasyDonate_Py/shop.py` & `easydonate_py-0.0.2/src/EasyDonate_Py/shop.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,153 +1,153 @@
 import requests
 
-class shop():
-    def shop_info(shop_key):
-        url = "https://easydonate.ru/api/v3/shop"
-        headers={"Shop-Key": shop_key}
-        response = requests.get(url=url, headers=headers)
-        if response.status_code == 200:
-            data = response.json()
-            if data["success"] == "true":
-                return data
-            else:
-                print("Не найдена информация!")
-        else:
-            print({'error': f"Ошибка: {response.status_code}"})
-
-class product():
-    def get_products(shop_key):
-        url = "https://easydonate.ru/api/v3/shop/products"
-        headers={"Shop-Key": shop_key}
-        response = requests.get(url=url, headers=headers)
-        if response.status_code == 200:
-            data = response.json()
-            if data["success"] == "true":
-                return data
-            else:
-                print("Не найдена информация!")
-        else:
-            print({'error': f"Ошибка: {response.status_code}"})
-
-    def get_product(shop_key, id):
-        url = f"https://easydonate.ru/api/v3/shop/product/{id}"
-        headers={"Shop-Key": shop_key}
-        response = requests.get(url=url, headers=headers)
-        if response.status_code == 200:
-            data = response.json()
-            if data["success"] == "true":
-                return data
-            else:
-                print("Не найдена информация!")
-        else:
-            print({'error': f"Ошибка: {response.status_code}"})
-
-class server():
-    def get_servers(shop_key):
-        url = "https://easydonate.ru/api/v3/shop/servers"
-        headers={"Shop-Key": shop_key}
-        response = requests.get(url=url, headers=headers)
-        if response.status_code == 200:
-            data = response.json()
-            if data["success"] == "true":
-                return data
-            else:
-                print("Не найдена информация!")
-        else:
-            print({'error': f"Ошибка: {response.status_code}"})
-
-    def get_server(shop_key, id):
-        url = f"https://easydonate.ru/api/v3/shop/server/{id}"
-        headers={"Shop-Key": shop_key}
-        response = requests.get(url=url, headers=headers)
-        if response.status_code == 200:
-            data = response.json()
-            if data["success"] == "true":
-                return data
-            else:
-                print("Не найдена информация!")
-        else:
-            print({'error': f"Ошибка: {response.status_code}"})
-
-class vouchers():
-    def mass_sales(shop_key):
-        url = "https://easydonate.ru/api/v3/shop/massSales"
-        headers={"Shop-Key": shop_key}
-        response = requests.get(url=url, headers=headers)
-        if response.status_code == 200:
-            data = response.json()
-            if data["success"] == "true":
-                return data
-            else:
-                print("Не найдена информация!")
-        else:
-            print({'error': f"Ошибка: {response.status_code}"})
-
-    def coupons(shop_key, where_active):
-        url = f"https://easydonate.ru/api/v3/shop/coupons"
-        headers={"Shop-Key": shop_key}
-        params = {
-            'where_active': where_active
-        }
-        if where_active:
-            response = requests.get(url=url, headers=headers, params=params)
-        else:
-            response = requests.get(url=url, headers=headers)
-        if response.status_code == 200:
-            data = response.json()
-            if data["success"] == "true":
-                return data
-            else:
-                print("Не найдена информация!")
-        else:
-            print({'error': f"Ошибка: {response.status_code}"})
-
-class paymets():
-    def payments(shop_key):
-        url = "https://easydonate.ru/api/v3/shop/payments"
-        headers={"Shop-Key": shop_key}
+
+def shop_info(shop_key):
+    url = "https://easydonate.ru/api/v3/shop"
+    headers={"Shop-Key": shop_key}
+    response = requests.get(url=url, headers=headers)
+    if response.status_code == 200:
+        data = response.json()
+        if data["success"] == "true":
+            return data
+        else:
+            print("Не найдена информация!")
+    else:
+        print({'error': f"Ошибка: {response.status_code}"})
+
+
+def get_products(shop_key):
+    url = "https://easydonate.ru/api/v3/shop/products"
+    headers={"Shop-Key": shop_key}
+    response = requests.get(url=url, headers=headers)
+    if response.status_code == 200:
+        data = response.json()
+        if data["success"] == "true":
+            return data
+        else:
+            print("Не найдена информация!")
+    else:
+        print({'error': f"Ошибка: {response.status_code}"})
+
+def get_product(shop_key, id):
+    url = f"https://easydonate.ru/api/v3/shop/product/{id}"
+    headers={"Shop-Key": shop_key}
+    response = requests.get(url=url, headers=headers)
+    if response.status_code == 200:
+        data = response.json()
+        if data["success"] == "true":
+            return data
+        else:
+            print("Не найдена информация!")
+    else:
+        print({'error': f"Ошибка: {response.status_code}"})
+
+
+def get_servers(shop_key):
+    url = "https://easydonate.ru/api/v3/shop/servers"
+    headers={"Shop-Key": shop_key}
+    response = requests.get(url=url, headers=headers)
+    if response.status_code == 200:
+        data = response.json()
+        if data["success"] == "true":
+            return data
+        else:
+            print("Не найдена информация!")
+    else:
+        print({'error': f"Ошибка: {response.status_code}"})
+
+def get_server(shop_key, id):
+    url = f"https://easydonate.ru/api/v3/shop/server/{id}"
+    headers={"Shop-Key": shop_key}
+    response = requests.get(url=url, headers=headers)
+    if response.status_code == 200:
+        data = response.json()
+        if data["success"] == "true":
+            return data
+        else:
+            print("Не найдена информация!")
+    else:
+        print({'error': f"Ошибка: {response.status_code}"})
+
+
+def mass_sales(shop_key):
+    url = "https://easydonate.ru/api/v3/shop/massSales"
+    headers={"Shop-Key": shop_key}
+    response = requests.get(url=url, headers=headers)
+    if response.status_code == 200:
+        data = response.json()
+        if data["success"] == "true":
+            return data
+        else:
+            print("Не найдена информация!")
+    else:
+        print({'error': f"Ошибка: {response.status_code}"})
+
+def coupons(shop_key, where_active):
+    url = f"https://easydonate.ru/api/v3/shop/coupons"
+    headers={"Shop-Key": shop_key}
+    params = {
+        'where_active': where_active
+    }
+    if where_active:
+        response = requests.get(url=url, headers=headers, params=params)
+    else:
         response = requests.get(url=url, headers=headers)
-        if response.status_code == 200:
-            data = response.json()
-            if data["success"] == "true":
-                return data
-            else:
-                print("Не найдена информация!")
-        else:
-            print({'error': f"Ошибка: {response.status_code}"})
+    if response.status_code == 200:
+        data = response.json()
+        if data["success"] == "true":
+            return data
+        else:
+            print("Не найдена информация!")
+    else:
+        print({'error': f"Ошибка: {response.status_code}"})
+
+
+def payments(shop_key):
+    url = "https://easydonate.ru/api/v3/shop/payments"
+    headers={"Shop-Key": shop_key}
+    response = requests.get(url=url, headers=headers)
+    if response.status_code == 200:
+        data = response.json()
+        if data["success"] == "true":
+            return data
+        else:
+            print("Не найдена информация!")
+    else:
+        print({'error': f"Ошибка: {response.status_code}"})
         
-    def payment(shop_key, id):
-        url = f"https://easydonate.ru/api/v3/shop/payment/{id}"
-        headers={"Shop-Key": shop_key}
-        response = requests.get(url=url, headers=headers)
-        if response.status_code == 200:
-            data = response.json()
-            if data["success"] == "true":
-                return data
-            else:
-                print("Не найдена информация!")
-        else:
-            print({'error': f"Ошибка: {response.status_code}"})
-
-    def create_payment(shop_key, customer, server_id, products, email, coupon, success_url):
-        url = "https://easydonate.ru/api/v3/shop/payment/create"
-        headers={"Shop-Key": shop_key}
-        params = {
-            'customer': customer,
-            'server_id': server_id,
-            'products': products
-        }
-        if email:
-            params['email'] = email
-        if coupon:
-            params['coupon'] = coupon
-        if success_url:
-            params['success_url'] = success_url
-        response = requests.get(url=url, headers=headers, params=params)
-        if response.status_code == 200:
-            data = response.json()
-            if data["success"] == "true":
-                return data
-            else:
-                print("Не найдена информация или неправильно введены параметры.")
-        else:
-            print({'error': f"Ошибка: {response.status_code}"})
+def payment(shop_key, id):
+    url = f"https://easydonate.ru/api/v3/shop/payment/{id}"
+    headers={"Shop-Key": shop_key}
+    response = requests.get(url=url, headers=headers)
+    if response.status_code == 200:
+        data = response.json()
+        if data["success"] == "true":
+            return data
+        else:
+            print("Не найдена информация!")
+    else:
+        print({'error': f"Ошибка: {response.status_code}"})
+
+def create_payment(shop_key, customer, server_id, products, email, coupon, success_url):
+    url = "https://easydonate.ru/api/v3/shop/payment/create"
+    headers={"Shop-Key": shop_key}
+    params = {
+        'customer': customer,
+        'server_id': server_id,
+        'products': products
+    }
+    if email:
+        params['email'] = email
+    if coupon:
+        params['coupon'] = coupon
+    if success_url:
+        params['success_url'] = success_url
+    response = requests.get(url=url, headers=headers, params=params)
+    if response.status_code == 200:
+        data = response.json()
+        if data["success"] == "true":
+            return data
+        else:
+            print("Не найдена информация или неправильно введены параметры.")
+    else:
+        print({'error': f"Ошибка: {response.status_code}"})
```

### Comparing `easydonate_py-0.0.1/LICENSE.txt` & `easydonate_py-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easydonate_py-0.0.1/README.md` & `easydonate_py-0.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Начало
 
 Первым делом мы должны установить нашу библиотеку.
-```pip install EasyDonate-Py```
+```pip install EasyDonate-Py==0.0.2``` или ```pip install --upgrade EasyDonate_Py```
 
 
 # Получение информации о магазине
 
 Получение информации о **магазине** осуществляется через функцию ```shop_info(shop_key="<ВАШ СЕКРЕТНЫЙ КЛЮЧ МАГАЗИНА>")```
 
 ### Все функции
```

### Comparing `easydonate_py-0.0.1/pyproject.toml` & `easydonate_py-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "EasyDonate-Py"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
  { name="refil", email="ru90671@gmail.com" },
- { name="flizan", email="" }
+ { name="flizan", email="sushkov.code@yandex.com" }
 ]
 description = "Простая библиотека для взаимодействия с EasyDonate API"
 readme = "README.md"
 requires-python = ">=3.10.0"
 classifiers = [
    "Programming Language :: Python :: 3",
    "License :: OSI Approved :: MIT License",
```

### Comparing `easydonate_py-0.0.1/PKG-INFO` & `easydonate_py-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.3
 Name: EasyDonate-Py
-Version: 0.0.1
+Version: 0.0.2
 Summary: Простая библиотека для взаимодействия с EasyDonate API
 Project-URL: Homepage, https://github.com/TUUVCOME/easydonate-py
 Project-URL: Issues, https://github.com/TUUVCOME/easydonate-py/issues
-Author: flizan
-Author-email: refil <ru90671@gmail.com>
+Author-email: refil <ru90671@gmail.com>, flizan <sushkov.code@yandex.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 
 # Начало
 
 Первым делом мы должны установить нашу библиотеку.
-```pip install EasyDonate-Py```
+```pip install EasyDonate-Py==0.0.2``` или ```pip install --upgrade EasyDonate_Py```
 
 
 # Получение информации о магазине
 
 Получение информации о **магазине** осуществляется через функцию ```shop_info(shop_key="<ВАШ СЕКРЕТНЫЙ КЛЮЧ МАГАЗИНА>")```
 
 ### Все функции
```

