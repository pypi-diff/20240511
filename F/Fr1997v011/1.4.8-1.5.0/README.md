# Comparing `tmp/Fr1997v011-1.4.8.tar.gz` & `tmp/Fr1997v011-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fr1997v011-1.4.8.tar", last modified: Fri May 10 10:27:13 2024, max compression
+gzip compressed data, was "Fr1997v011-1.5.0.tar", last modified: Sat May 11 02:07:40 2024, max compression
```

## Comparing `Fr1997v011-1.4.8.tar` & `Fr1997v011-1.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 10:27:13.528760 Fr1997v011-1.4.8/
-drwxrwxrwx   0        0        0        0 2024-05-10 10:27:13.510642 Fr1997v011-1.4.8/Fr1997v011.egg-info/
--rw-rw-rw-   0        0        0      182 2024-05-10 10:27:13.000000 Fr1997v011-1.4.8/Fr1997v011.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-05-10 10:27:13.000000 Fr1997v011-1.4.8/Fr1997v011.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 10:27:13.000000 Fr1997v011-1.4.8/Fr1997v011.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-10 02:52:07.000000 Fr1997v011-1.4.8/Fr1997v011.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-05-10 10:27:13.000000 Fr1997v011-1.4.8/Fr1997v011.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.4.8/LICENSE
--rw-rw-rw-   0        0        0      182 2024-05-10 10:27:13.526250 Fr1997v011-1.4.8/PKG-INFO
--rw-rw-rw-   0        0        0      773 2024-05-10 02:52:13.000000 Fr1997v011-1.4.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 10:27:13.512235 Fr1997v011-1.4.8/fr1997_mode/
--rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.4.8/fr1997_mode/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 10:27:13.521299 Fr1997v011-1.4.8/fr1997_mode/mode_func/
--rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.4.8/fr1997_mode/mode_func/__init__.py
--rw-rw-rw-   0        0        0   177405 2024-05-10 10:27:11.000000 Fr1997v011-1.4.8/fr1997_mode/mode_func/all_func.py
-drwxrwxrwx   0        0        0        0 2024-05-10 10:27:13.523249 Fr1997v011-1.4.8/fr1997_mode/mode_static/
--rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.4.8/fr1997_mode/mode_static/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-10 10:27:13.529770 Fr1997v011-1.4.8/setup.cfg
--rw-rw-rw-   0        0        0      322 2024-05-10 02:52:06.000000 Fr1997v011-1.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 02:07:40.623409 Fr1997v011-1.5.0/
+drwxrwxrwx   0        0        0        0 2024-05-11 02:07:40.617410 Fr1997v011-1.5.0/Fr1997v011.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-05-11 02:07:40.000000 Fr1997v011-1.5.0/Fr1997v011.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-05-11 02:07:40.000000 Fr1997v011-1.5.0/Fr1997v011.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 02:07:40.000000 Fr1997v011-1.5.0/Fr1997v011.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-11 02:07:40.000000 Fr1997v011-1.5.0/Fr1997v011.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-05-11 02:07:40.000000 Fr1997v011-1.5.0/Fr1997v011.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0      182 2024-05-11 02:07:40.622409 Fr1997v011-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2024-05-10 02:52:13.000000 Fr1997v011-1.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 02:07:40.618409 Fr1997v011-1.5.0/fr1997_mode/
+-rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.5.0/fr1997_mode/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 02:07:40.620419 Fr1997v011-1.5.0/fr1997_mode/mode_func/
+-rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.5.0/fr1997_mode/mode_func/__init__.py
+-rw-rw-rw-   0        0        0   177247 2024-05-11 01:57:53.000000 Fr1997v011-1.5.0/fr1997_mode/mode_func/all_func.py
+drwxrwxrwx   0        0        0        0 2024-05-11 02:07:40.621410 Fr1997v011-1.5.0/fr1997_mode/mode_static/
+-rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.5.0/fr1997_mode/mode_static/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-11 02:07:40.623409 Fr1997v011-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      322 2024-05-11 02:07:36.000000 Fr1997v011-1.5.0/setup.py
```

### Comparing `Fr1997v011-1.4.8/LICENSE` & `Fr1997v011-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Fr1997v011-1.4.8/README.md` & `Fr1997v011-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `Fr1997v011-1.4.8/fr1997_mode/mode_func/all_func.py` & `Fr1997v011-1.5.0/fr1997_mode/mode_func/all_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 """
     配置文件
         所有配置在这个地方读取 
         使用内存缓存机制 memcache
         没有读取到内存中的配置，这个包相当于不能用
     pip3 cache purge
-    pip3 install -i https://pypi.tuna.tsinghua.edu.cn/simple Fr1997v011==1.4.5
+    pip3 install -i https://pypi.tuna.tsinghua.edu.cn/simple Fr1997v011==1.4.8
 """
 
 """
     pip3 install --upgrade Fr1997v011
     pip3 install redis
     pip3 install pymysql
     pip3 install elasticsearch
@@ -4465,9 +4465,7 @@
 mode_pros = ModeStatic()  # 其它函数
 mode_cos = Cos()  # cos
 mode_fr_cos = Cos(server_select='personal')  # cos 高阳
 mode_myself = MyGy()
 
 mode_pro = ModeFunc()  # main
 
-# print(mode_xhs.xhs_video_main('https://www.xiaohongshu.com/explore/64b49c82000000002f028a01'))
-# print(mode_douyin.api_douyin_video('7359496982328528154'))
```

