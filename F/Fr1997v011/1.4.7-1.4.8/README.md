# Comparing `tmp/Fr1997v011-1.4.7.tar.gz` & `tmp/Fr1997v011-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fr1997v011-1.4.7.tar", last modified: Thu May  9 11:07:09 2024, max compression
+gzip compressed data, was "Fr1997v011-1.4.8.tar", last modified: Fri May 10 10:27:13 2024, max compression
```

## Comparing `Fr1997v011-1.4.7.tar` & `Fr1997v011-1.4.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 11:07:09.201178 Fr1997v011-1.4.7/
-drwxrwxrwx   0        0        0        0 2024-05-09 11:07:09.194603 Fr1997v011-1.4.7/Fr1997v011.egg-info/
--rw-rw-rw-   0        0        0      182 2024-05-09 11:07:09.000000 Fr1997v011-1.4.7/Fr1997v011.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-05-09 11:07:09.000000 Fr1997v011-1.4.7/Fr1997v011.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 11:07:09.000000 Fr1997v011-1.4.7/Fr1997v011.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-09 11:07:09.000000 Fr1997v011-1.4.7/Fr1997v011.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-05-09 11:07:09.000000 Fr1997v011-1.4.7/Fr1997v011.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.4.7/LICENSE
--rw-rw-rw-   0        0        0      182 2024-05-09 11:07:09.200179 Fr1997v011-1.4.7/PKG-INFO
--rw-rw-rw-   0        0        0      773 2024-05-09 11:07:08.000000 Fr1997v011-1.4.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 11:07:09.195592 Fr1997v011-1.4.7/fr1997_mode/
--rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.4.7/fr1997_mode/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 11:07:09.196591 Fr1997v011-1.4.7/fr1997_mode/mode_func/
--rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.4.7/fr1997_mode/mode_func/__init__.py
--rw-rw-rw-   0        0        0   177160 2024-05-09 11:07:04.000000 Fr1997v011-1.4.7/fr1997_mode/mode_func/all_func.py
-drwxrwxrwx   0        0        0        0 2024-05-09 11:07:09.198094 Fr1997v011-1.4.7/fr1997_mode/mode_static/
--rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.4.7/fr1997_mode/mode_static/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-09 11:07:09.201178 Fr1997v011-1.4.7/setup.cfg
--rw-rw-rw-   0        0        0      322 2024-05-09 11:07:04.000000 Fr1997v011-1.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 10:27:13.528760 Fr1997v011-1.4.8/
+drwxrwxrwx   0        0        0        0 2024-05-10 10:27:13.510642 Fr1997v011-1.4.8/Fr1997v011.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-05-10 10:27:13.000000 Fr1997v011-1.4.8/Fr1997v011.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-05-10 10:27:13.000000 Fr1997v011-1.4.8/Fr1997v011.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 10:27:13.000000 Fr1997v011-1.4.8/Fr1997v011.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-10 02:52:07.000000 Fr1997v011-1.4.8/Fr1997v011.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-05-10 10:27:13.000000 Fr1997v011-1.4.8/Fr1997v011.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.4.8/LICENSE
+-rw-rw-rw-   0        0        0      182 2024-05-10 10:27:13.526250 Fr1997v011-1.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2024-05-10 02:52:13.000000 Fr1997v011-1.4.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 10:27:13.512235 Fr1997v011-1.4.8/fr1997_mode/
+-rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.4.8/fr1997_mode/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 10:27:13.521299 Fr1997v011-1.4.8/fr1997_mode/mode_func/
+-rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.4.8/fr1997_mode/mode_func/__init__.py
+-rw-rw-rw-   0        0        0   177405 2024-05-10 10:27:11.000000 Fr1997v011-1.4.8/fr1997_mode/mode_func/all_func.py
+drwxrwxrwx   0        0        0        0 2024-05-10 10:27:13.523249 Fr1997v011-1.4.8/fr1997_mode/mode_static/
+-rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.4.8/fr1997_mode/mode_static/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-10 10:27:13.529770 Fr1997v011-1.4.8/setup.cfg
+-rw-rw-rw-   0        0        0      322 2024-05-10 02:52:06.000000 Fr1997v011-1.4.8/setup.py
```

### Comparing `Fr1997v011-1.4.7/LICENSE` & `Fr1997v011-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `Fr1997v011-1.4.7/README.md` & `Fr1997v011-1.4.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ```sh
 python setup.py sdist
 ```
 
 ### （本地）安装包
 
 ```sh
-pip install dist/Fr1997v011-1.4.7.tar.gz
+pip install dist/Fr1997v011-1.4.8.tar.gz
 ```
 
 ### 下载包
 
 ```sh
 pip install Fr1997v011
 ```
```

### Comparing `Fr1997v011-1.4.7/fr1997_mode/mode_func/all_func.py` & `Fr1997v011-1.4.8/fr1997_mode/mode_func/all_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -2183,43 +2183,46 @@
 
     def xhs_web_video_main_data(self, data_json, note_id):
         def ret_json(code=200, msg=None, data=None):
             return {'code': code, 'msg': msg, 'data': data}
 
         try:
             note_info = data_json['note']['noteDetailMap'][note_id]['note']
+            # print(note_info)
 
             # 关于视频链接
             find_dld_video_url = 0
             dld_video_url = None
             stream = note_info['video']['media']['stream']
             for m in stream:
                 if stream[m] and find_dld_video_url == 0:
                     try:
-                        dld_video_url = stream[m][0]['backupUrls'][0]
+                        # 有？无法转译
+                        dld_video_url = stream[m][0]['backupUrls'][-1]
                     except:
                         pass
 
             if not dld_video_url:
                 return ret_json(200, '未找到url')
 
             return ret_json(200, 'ok', {
+                'note_id': note_id,
                 'create_date': int(note_info['time'] / 1000),
                 'title': mode_text.word_change(note_info['title']),
                 'desc': mode_text.word_change(note_info['desc']),
-                'location': note_info['ipLocation'],
+                'location': note_info.get('ipLocation', ''),
                 'duration': note_info['video']['capa']['duration'],
                 'dld_video_url': dld_video_url,
 
                 'nickname': mode_text.word_change(note_info['user']['nickname']),
                 'user_id': note_info['user']['userId'],
                 'avatar': note_info['user']['avatar'],
             })
         except Exception as e:
-            return ret_json(200, e)
+            return ret_json(500, e)
 
     def xhs_video_id_pc(self, url):
         note_id = None
         if '://www.xiaohongshu.com/discovery' in url:
             note_id = url.split('://www.xiaohongshu.com/discovery/item/')[-1].split('?')[0]
 
         if '://www.xiaohongshu.com/explore/' in url:
@@ -4400,15 +4403,14 @@
             'msg': msg,
             'data_list': data_list,
             'data_dict': data_dict
         })
 
     @classmethod
     def code200(cls, msg='ok', data_list=None, data_dict=None):
-        print(data_list, data_dict)
         return cls.ret_json(200, msg, data_list, data_dict)
 
     @classmethod
     def code201(cls, msg='ok', data_list=None, data_dict=None):
         return cls.ret_json(201, msg, data_list, data_dict, 201)
 
     @classmethod
@@ -4463,7 +4465,9 @@
 mode_pros = ModeStatic()  # 其它函数
 mode_cos = Cos()  # cos
 mode_fr_cos = Cos(server_select='personal')  # cos 高阳
 mode_myself = MyGy()
 
 mode_pro = ModeFunc()  # main
 
+# print(mode_xhs.xhs_video_main('https://www.xiaohongshu.com/explore/64b49c82000000002f028a01'))
+# print(mode_douyin.api_douyin_video('7359496982328528154'))
```

