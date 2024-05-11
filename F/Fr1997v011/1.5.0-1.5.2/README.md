# Comparing `tmp/Fr1997v011-1.5.0.tar.gz` & `tmp/Fr1997v011-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fr1997v011-1.5.0.tar", last modified: Sat May 11 02:07:40 2024, max compression
+gzip compressed data, was "Fr1997v011-1.5.2.tar", last modified: Sat May 11 06:06:23 2024, max compression
```

## Comparing `Fr1997v011-1.5.0.tar` & `Fr1997v011-1.5.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 02:07:40.623409 Fr1997v011-1.5.0/
-drwxrwxrwx   0        0        0        0 2024-05-11 02:07:40.617410 Fr1997v011-1.5.0/Fr1997v011.egg-info/
--rw-rw-rw-   0        0        0      182 2024-05-11 02:07:40.000000 Fr1997v011-1.5.0/Fr1997v011.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-05-11 02:07:40.000000 Fr1997v011-1.5.0/Fr1997v011.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 02:07:40.000000 Fr1997v011-1.5.0/Fr1997v011.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-11 02:07:40.000000 Fr1997v011-1.5.0/Fr1997v011.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-05-11 02:07:40.000000 Fr1997v011-1.5.0/Fr1997v011.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.5.0/LICENSE
--rw-rw-rw-   0        0        0      182 2024-05-11 02:07:40.622409 Fr1997v011-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0      773 2024-05-10 02:52:13.000000 Fr1997v011-1.5.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 02:07:40.618409 Fr1997v011-1.5.0/fr1997_mode/
--rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.5.0/fr1997_mode/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 02:07:40.620419 Fr1997v011-1.5.0/fr1997_mode/mode_func/
--rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.5.0/fr1997_mode/mode_func/__init__.py
--rw-rw-rw-   0        0        0   177247 2024-05-11 01:57:53.000000 Fr1997v011-1.5.0/fr1997_mode/mode_func/all_func.py
-drwxrwxrwx   0        0        0        0 2024-05-11 02:07:40.621410 Fr1997v011-1.5.0/fr1997_mode/mode_static/
--rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.5.0/fr1997_mode/mode_static/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-11 02:07:40.623409 Fr1997v011-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0      322 2024-05-11 02:07:36.000000 Fr1997v011-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 06:06:23.477290 Fr1997v011-1.5.2/
+drwxrwxrwx   0        0        0        0 2024-05-11 06:06:23.457288 Fr1997v011-1.5.2/Fr1997v011.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-05-11 06:06:23.000000 Fr1997v011-1.5.2/Fr1997v011.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-05-11 06:06:23.000000 Fr1997v011-1.5.2/Fr1997v011.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 06:06:23.000000 Fr1997v011-1.5.2/Fr1997v011.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-11 06:06:23.000000 Fr1997v011-1.5.2/Fr1997v011.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-05-11 06:06:23.000000 Fr1997v011-1.5.2/Fr1997v011.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.5.2/LICENSE
+-rw-rw-rw-   0        0        0      182 2024-05-11 06:06:23.470488 Fr1997v011-1.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2024-05-11 02:51:24.000000 Fr1997v011-1.5.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 06:06:23.459288 Fr1997v011-1.5.2/fr1997_mode/
+-rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.5.2/fr1997_mode/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 06:06:23.465289 Fr1997v011-1.5.2/fr1997_mode/mode_func/
+-rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.5.2/fr1997_mode/mode_func/__init__.py
+-rw-rw-rw-   0        0        0   177699 2024-05-11 06:05:45.000000 Fr1997v011-1.5.2/fr1997_mode/mode_func/all_func.py
+drwxrwxrwx   0        0        0        0 2024-05-11 06:06:23.467288 Fr1997v011-1.5.2/fr1997_mode/mode_static/
+-rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.5.2/fr1997_mode/mode_static/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-11 06:06:23.478289 Fr1997v011-1.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      322 2024-05-11 06:06:20.000000 Fr1997v011-1.5.2/setup.py
```

### Comparing `Fr1997v011-1.5.0/LICENSE` & `Fr1997v011-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Fr1997v011-1.5.0/README.md` & `Fr1997v011-1.5.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ```sh
 python setup.py sdist
 ```
 
 ### （本地）安装包
 
 ```sh
-pip install dist/Fr1997v011-1.4.8.tar.gz
+pip install dist/Fr1997v011-1.5.1.tar.gz
 ```
 
 ### 下载包
 
 ```sh
 pip install Fr1997v011
 ```
```

### Comparing `Fr1997v011-1.5.0/fr1997_mode/mode_func/all_func.py` & `Fr1997v011-1.5.2/fr1997_mode/mode_func/all_func.py`

 * *Files 0% similar despite different names*

```diff
@@ -1453,14 +1453,20 @@
 
         # 视频下载地址
         try:
             download_addr_url_list = res_data['video']['download_addr']['url_list']
         except:
             download_addr_url_list = []
 
+        # 视频下载地址 第二类型
+        try:
+            download_addr_url_list2 = res_data['video']['play_addr']['url_list']
+        except:
+            download_addr_url_list2 = []
+
         # mp3 url
         try:
             mp3_url_list = res_data['music']['play_url']['url_list']
 
             if '.mp3' in res_data['music']['play_url']['url_list'][0]:
                 pass
             else:
@@ -1485,14 +1491,15 @@
         base_ret_data['update_time'] = int(time.time()),
         base_ret_data['create_date'] = create_time
         base_ret_data['release_time'] = release_time
         base_ret_data['nickname'] = nickname
         base_ret_data['author_head'] = author_head
         base_ret_data['describe'] = describe
 
+        base_ret_data['download_addr_url_list2'] = download_addr_url_list2
         base_ret_data['download_addr_url_list'] = download_addr_url_list
         base_ret_data['mp3_url_list'] = mp3_url_list
 
         if tp == 'django_video_info':
             return {
                 "video_id": res_data["aweme_id"],
                 "v_id": v_id,
@@ -2183,15 +2190,18 @@
 
     def xhs_web_video_main_data(self, data_json, note_id):
         def ret_json(code=200, msg=None, data=None):
             return {'code': code, 'msg': msg, 'data': data}
 
         try:
             note_info = data_json['note']['noteDetailMap'][note_id]['note']
-            # print(note_info)
+
+            aweme_type = note_info.get('type')
+            if aweme_type is None or aweme_type != 'video':
+                return ret_json(200, '请输入视频作品')
 
             # 关于视频链接
             find_dld_video_url = 0
             dld_video_url = None
             stream = note_info['video']['media']['stream']
             for m in stream:
                 if stream[m] and find_dld_video_url == 0:
@@ -2202,14 +2212,15 @@
                         pass
 
             if not dld_video_url:
                 return ret_json(200, '未找到url')
 
             return ret_json(200, 'ok', {
                 'note_id': note_id,
+                'aweme_type': 1,
                 'create_date': int(note_info['time'] / 1000),
                 'title': mode_text.word_change(note_info['title']),
                 'desc': mode_text.word_change(note_info['desc']),
                 'location': note_info.get('ipLocation', ''),
                 'duration': note_info['video']['capa']['duration'],
                 'dld_video_url': dld_video_url,
```

