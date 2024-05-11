# Comparing `tmp/lama2923-1.0.2.tar.gz` & `tmp/lama2923-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lama2923-1.0.2.tar", last modified: Tue Apr 16 14:30:29 2024, max compression
+gzip compressed data, was "lama2923-1.0.3.tar", last modified: Sat May 11 11:20:56 2024, max compression
```

## Comparing `lama2923-1.0.2.tar` & `lama2923-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 14:30:29.721843 lama2923-1.0.2/
--rw-rw-rw-   0        0        0      956 2024-04-16 14:30:29.720842 lama2923-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-16 14:30:29.703208 lama2923-1.0.2/lama2923/
--rw-rw-rw-   0        0        0    26494 2024-04-16 14:29:11.000000 lama2923-1.0.2/lama2923/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:30:29.717845 lama2923-1.0.2/lama2923.egg-info/
--rw-rw-rw-   0        0        0      956 2024-04-16 14:30:29.000000 lama2923-1.0.2/lama2923.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-04-16 14:30:29.000000 lama2923-1.0.2/lama2923.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 14:30:29.000000 lama2923-1.0.2/lama2923.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-16 14:30:29.000000 lama2923-1.0.2/lama2923.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-16 14:30:29.000000 lama2923-1.0.2/lama2923.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 14:30:29.722845 lama2923-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1294 2024-04-16 14:30:13.000000 lama2923-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 11:20:56.891153 lama2923-1.0.3/
+-rw-rw-rw-   0        0        0      956 2024-05-11 11:20:56.890142 lama2923-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-11 11:20:56.877144 lama2923-1.0.3/lama2923/
+-rw-rw-rw-   0        0        0    26528 2024-05-11 11:19:51.000000 lama2923-1.0.3/lama2923/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 11:20:56.888143 lama2923-1.0.3/lama2923.egg-info/
+-rw-rw-rw-   0        0        0      956 2024-05-11 11:20:56.000000 lama2923-1.0.3/lama2923.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2024-05-11 11:20:56.000000 lama2923-1.0.3/lama2923.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 11:20:56.000000 lama2923-1.0.3/lama2923.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-11 11:20:56.000000 lama2923-1.0.3/lama2923.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-11 11:20:56.000000 lama2923-1.0.3/lama2923.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-11 11:20:56.891153 lama2923-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1294 2024-05-11 11:20:37.000000 lama2923-1.0.3/setup.py
```

### Comparing `lama2923-1.0.2/PKG-INFO` & `lama2923-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lama2923
-Version: 1.0.2
+Version: 1.0.3
 Summary: Sikimsonik bir kütüphane
 Author: lama2923
 Author-email: lama2923.v2@gmail.com
 Keywords: example project setuptools development discord lama2923
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lama2923-1.0.2/lama2923/__init__.py` & `lama2923-1.0.3/lama2923/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -451,33 +451,37 @@
             url = f'https://discord.com/api/v9/guilds/{Guild_id}/channels'
             response = requests.get(url, headers=headers)
             if response.status_code == 200:
                 return [response.status_code, response.json()]
             else:
                 return response.status_code   
 
-        def send_tts_message(self, Channel_id, Message):
-            payload = {'content': str(Message), 'tts': True}
-            headers = {'Authorization': str(self.token)}
-            response = requests.post(f'https://discord.com/api/v9/channels/{Channel_id}/messages', data=payload, headers=headers)
-            return response.status_code
-        
+            
+
         def send_reply_message(self, Channel_id, Message, ReplyMessage_id):
             payload = {'content': str(Message), 'message_reference': {'message_id': ReplyMessage_id}}
             headers = {'Authorization': str(self.token)}
             response = requests.post(f'https://discord.com/api/v9/channels/{Channel_id}/messages', data=payload, headers=headers)
             return response.status_code
         
         def change_user_nickname(self, Guild_id, Nickname):
             headers = {'Authorization': str(self.token)}
             payload = {'nick': str(Nickname)}
             response = requests.patch(f'https://discord.com/api/v9/guilds/{Guild_id}/members/@me/nick', json=payload, headers=headers)
             return response.status_code
 
-        def get_user_info(self, User_id):
+        def get_user_info(self):
+            headers = {'Authorization': str(self.token)}
+            response = requests.get('https://discord.com/api/v9/users/@me', headers=headers)
+            if response.status_code == 200:
+                return [response.status_code, response.json()]
+            else:
+                return response.status_code
+        
+        def get_spesific_user_info(self, User_id):
             headers = {'Authorization': str(self.token)}
             url = f'https://discord.com/api/v9/users/{User_id}'
             response = requests.get(url, headers=headers)
             if response.status_code == 200:
                 return [response.status_code, response.json()]
             else:
                 return response.status_code
```

### Comparing `lama2923-1.0.2/lama2923.egg-info/PKG-INFO` & `lama2923-1.0.3/lama2923.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lama2923
-Version: 1.0.2
+Version: 1.0.3
 Summary: Sikimsonik bir kütüphane
 Author: lama2923
 Author-email: lama2923.v2@gmail.com
 Keywords: example project setuptools development discord lama2923
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lama2923-1.0.2/setup.py` & `lama2923-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Komutlar.txt dosyasından komutlar ile terminalde setup dosyasını çalıştırım upload edebilirsin.
 
 setup(
     name='lama2923',
-    version='1.0.2',
+    version='1.0.3',
     description='Sikimsonik bir kütüphane',
     long_description="Discord Apı ile işlemler, Webhook ile işlemler, lprint, linput gibi güzel görünümlü yazılar... kısacası projenizde kullanabilceğiniz tasarım olarak ve sistem olarak kullanabilceğiniz bir kütüphane, ayrıca bu kütüphanenin ana dili Türkçe.",
     author='lama2923',
     author_email='lama2923.v2@gmail.com',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
```

