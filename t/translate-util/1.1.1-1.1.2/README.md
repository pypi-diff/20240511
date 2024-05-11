# Comparing `tmp/translate_util-1.1.1.tar.gz` & `tmp/translate_util-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/translate_util-1.1.1.tar", last modified: Mon May  6 07:21:46 2024, max compression
+gzip compressed data, was "dist/translate_util-1.1.2.tar", last modified: Sat May 11 03:02:30 2024, max compression
```

## Comparing `translate_util-1.1.1.tar` & `translate_util-1.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-06 07:21:46.000000 translate_util-1.1.1/
--rw-r--r--   0 admin      (501) staff       (20)     1752 2024-05-06 07:21:46.000000 translate_util-1.1.1/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      755 2024-05-06 07:21:40.000000 translate_util-1.1.1/README.md
--rw-r--r--   0 admin      (501) staff       (20)       38 2024-05-06 07:21:46.000000 translate_util-1.1.1/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     1158 2024-05-06 07:21:40.000000 translate_util-1.1.1/setup.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-06 07:21:46.000000 translate_util-1.1.1/translate_util/
--rw-r--r--   0 admin      (501) staff       (20)       60 2020-06-12 15:15:27.000000 translate_util-1.1.1/translate_util/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)      713 2024-05-06 03:30:42.000000 translate_util-1.1.1/translate_util/base_translate.py
--rw-r--r--   0 admin      (501) staff       (20)      756 2020-06-13 13:57:02.000000 translate_util-1.1.1/translate_util/common_request.py
--rw-r--r--   0 admin      (501) staff       (20)     5817 2022-08-24 03:09:35.000000 translate_util-1.1.1/translate_util/translate_baidu.py
--rw-r--r--   0 admin      (501) staff       (20)     2937 2024-05-06 04:03:54.000000 translate_util-1.1.1/translate_util/translate_google.py
--rw-r--r--   0 admin      (501) staff       (20)     1608 2022-08-24 03:14:57.000000 translate_util-1.1.1/translate_util/translate_iciba.py
--rw-r--r--   0 admin      (501) staff       (20)     4178 2024-05-06 03:55:52.000000 translate_util-1.1.1/translate_util/translate_tool.py
--rw-r--r--   0 admin      (501) staff       (20)     1801 2022-08-24 03:16:53.000000 translate_util-1.1.1/translate_util/translate_youdao.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-06 07:21:46.000000 translate_util-1.1.1/translate_util.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     1752 2024-05-06 07:21:46.000000 translate_util-1.1.1/translate_util.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      471 2024-05-06 07:21:46.000000 translate_util-1.1.1/translate_util.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2024-05-06 07:21:46.000000 translate_util-1.1.1/translate_util.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       63 2024-05-06 07:21:46.000000 translate_util-1.1.1/translate_util.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)       15 2024-05-06 07:21:46.000000 translate_util-1.1.1/translate_util.egg-info/top_level.txt
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-11 03:02:30.000000 translate_util-1.1.2/
+-rw-r--r--   0 admin      (501) staff       (20)     1796 2024-05-11 03:02:30.000000 translate_util-1.1.2/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      791 2024-05-11 03:02:15.000000 translate_util-1.1.2/README.md
+-rw-r--r--   0 admin      (501) staff       (20)       38 2024-05-11 03:02:30.000000 translate_util-1.1.2/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     1158 2024-05-11 03:02:15.000000 translate_util-1.1.2/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-11 03:02:30.000000 translate_util-1.1.2/translate_util/
+-rw-r--r--   0 admin      (501) staff       (20)       60 2020-06-12 15:15:27.000000 translate_util-1.1.2/translate_util/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      713 2024-05-06 03:30:42.000000 translate_util-1.1.2/translate_util/base_translate.py
+-rw-r--r--   0 admin      (501) staff       (20)      756 2020-06-13 13:57:02.000000 translate_util-1.1.2/translate_util/common_request.py
+-rw-r--r--   0 admin      (501) staff       (20)     5817 2022-08-24 03:09:35.000000 translate_util-1.1.2/translate_util/translate_baidu.py
+-rw-r--r--   0 admin      (501) staff       (20)     2936 2024-05-11 03:02:15.000000 translate_util-1.1.2/translate_util/translate_google.py
+-rw-r--r--   0 admin      (501) staff       (20)     1608 2022-08-24 03:14:57.000000 translate_util-1.1.2/translate_util/translate_iciba.py
+-rw-r--r--   0 admin      (501) staff       (20)     4178 2024-05-06 03:55:52.000000 translate_util-1.1.2/translate_util/translate_tool.py
+-rw-r--r--   0 admin      (501) staff       (20)     1801 2022-08-24 03:16:53.000000 translate_util-1.1.2/translate_util/translate_youdao.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-11 03:02:30.000000 translate_util-1.1.2/translate_util.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     1796 2024-05-11 03:02:30.000000 translate_util-1.1.2/translate_util.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      471 2024-05-11 03:02:30.000000 translate_util-1.1.2/translate_util.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2024-05-11 03:02:30.000000 translate_util-1.1.2/translate_util.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       63 2024-05-11 03:02:30.000000 translate_util-1.1.2/translate_util.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)       15 2024-05-11 03:02:30.000000 translate_util-1.1.2/translate_util.egg-info/top_level.txt
```

### Comparing `translate_util-1.1.1/PKG-INFO` & `translate_util-1.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: translate_util
-Version: 1.1.1
+Version: 1.1.2
 Summary: translate tool support(google)
 Home-page: https://github.com/abo123456789/translate_util
 Author: cc
 Author-email: abcdef123456chen@sohu.com
 Maintainer: cc
 Maintainer-email: abcdef123456chen@sohu.com
 License: MIT License
@@ -29,14 +29,15 @@
             # translate other language to chinese (default use google)
             print(translate_other2cn('china'))
             
             # translate other language to english (default use google)
             print(translate_other2en('中国'))
             
             # translate other language to de ,support any language
+            # tl demo: zh-CN/de/fr/en/it/es
             print(translate_text('china', tl='de'))
             
             
         ```
         
         ### OTHER SUPPORT
         any customization demand,contact me with email
```

### Comparing `translate_util-1.1.1/README.md` & `translate_util-1.1.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     # translate other language to chinese (default use google)
     print(translate_other2cn('china'))
     
     # translate other language to english (default use google)
     print(translate_other2en('中国'))
     
     # translate other language to de ,support any language
+    # tl demo: zh-CN/de/fr/en/it/es
     print(translate_text('china', tl='de'))
     
     
 ```
 
 ### OTHER SUPPORT
 any customization demand,contact me with email
```

### Comparing `translate_util-1.1.1/setup.py` & `translate_util-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # @TIME 2020/04/29 23:26
 # coding=utf-8
 
 from setuptools import setup, find_packages
 
 setup(
     name='translate_util',
-    version='1.1.1',
+    version='1.1.2',
     description=(
         'translate tool support(google)'
     ),
     long_description_content_type="text/markdown",
     long_description=open('README.md').read(),
     author='cc',
     author_email='abcdef123456chen@sohu.com',
```

### Comparing `translate_util-1.1.1/translate_util/base_translate.py` & `translate_util-1.1.2/translate_util/base_translate.py`

 * *Files identical despite different names*

### Comparing `translate_util-1.1.1/translate_util/common_request.py` & `translate_util-1.1.2/translate_util/common_request.py`

 * *Files identical despite different names*

### Comparing `translate_util-1.1.1/translate_util/translate_baidu.py` & `translate_util-1.1.2/translate_util/translate_baidu.py`

 * *Files identical despite different names*

### Comparing `translate_util-1.1.1/translate_util/translate_google.py` & `translate_util-1.1.2/translate_util/translate_google.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # -*- coding:utf-8 -*-
 # @Author cc
 # @TIME 2020/5/25 16:02
 import re
+import urllib.parse
 
 import requests
 
 from translate_util.base_translate import BaseTranslate
 
 
 class GoogleTranslate(BaseTranslate):
-
     def trans_text_other2cn(self):
         return self.trans_text(self.content, tl='zh-CN')
 
     def trans_text_other2en(self):
         return self.trans_text(self.content, tl='en')
 
     def trans_text(self, st: [str, bytes], sl='auto', tl='zh-CN') -> str:
@@ -22,15 +22,15 @@
         :param st: 待翻译的字符串
         :param sl: 待翻译的语言 默认auto
         :param tl: 翻译成的语言
         :return: 翻译后的字符串
         """
         url = "https://www.google.com.hk/async/translate"
 
-        payload = f"async=translate,sl:{sl},tl:{tl},st:{st.encode('utf-8')},id:1672056488960,qc:true,ac:true,_id:tw-async-translate,_pms:s,_fmt:pc"
+        payload = f"async=translate,sl:{sl},tl:{tl},st:{urllib.parse.quote(st)},id:1672056488960,qc:true,ac:true,_id:tw-async-translate,_pms:s,_fmt:pc"
         headers = {
             'sec-ch-ua': '"Not?A_Brand";v="8", "Chromium";v="108", "Google Chrome";v="108"',
             'DNT': '1',
             'sec-ch-ua-mobile': '?0',
             'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/108.0.0.0 Safari/537.36',
             'sec-ch-ua-arch': '"x86"',
             'sec-ch-ua-full-version': '"108.0.5359.125"',
@@ -48,15 +48,14 @@
             'Sec-Fetch-Dest': 'empty',
             'host': 'www.google.com.hk',
             'Cookie': '1P_JAR=2022-12-26-12; NID=511=eVLI1bG9nhyOZtqU14JBHm5Be00epdxfR4XmfQeehYyIkzgpXi6dbpNY75ZMVyS7aOjoM2oZ5WdoR8eNq6wi1-e_J0NeoyI0dtsHW-_8Ik4PGrqvuGHdcvVC03zTOEK2TY1FZL85Wimo_ZPIE3hGIrmGPSiel6-rRRW9lD30UPs'
         }
 
         response = requests.request("POST", url, headers=headers, data=payload)
         res_text = response.content.decode()
-        print(res_text)
         res_array = re.findall(r'id="tw-answ-target-text">(.*?)</span>', res_text,
                                flags=re.IGNORECASE)
         return res_array[0]
 
 
 if __name__ == '__main__':
     for source_text in ['china', 'je suis un']:
```

### Comparing `translate_util-1.1.1/translate_util/translate_iciba.py` & `translate_util-1.1.2/translate_util/translate_iciba.py`

 * *Files identical despite different names*

### Comparing `translate_util-1.1.1/translate_util/translate_tool.py` & `translate_util-1.1.2/translate_util/translate_tool.py`

 * *Files identical despite different names*

### Comparing `translate_util-1.1.1/translate_util/translate_youdao.py` & `translate_util-1.1.2/translate_util/translate_youdao.py`

 * *Files identical despite different names*

### Comparing `translate_util-1.1.1/translate_util.egg-info/PKG-INFO` & `translate_util-1.1.2/translate_util.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: translate-util
-Version: 1.1.1
+Version: 1.1.2
 Summary: translate tool support(google)
 Home-page: https://github.com/abo123456789/translate_util
 Author: cc
 Author-email: abcdef123456chen@sohu.com
 Maintainer: cc
 Maintainer-email: abcdef123456chen@sohu.com
 License: MIT License
@@ -29,14 +29,15 @@
             # translate other language to chinese (default use google)
             print(translate_other2cn('china'))
             
             # translate other language to english (default use google)
             print(translate_other2en('中国'))
             
             # translate other language to de ,support any language
+            # tl demo: zh-CN/de/fr/en/it/es
             print(translate_text('china', tl='de'))
             
             
         ```
         
         ### OTHER SUPPORT
         any customization demand,contact me with email
```

