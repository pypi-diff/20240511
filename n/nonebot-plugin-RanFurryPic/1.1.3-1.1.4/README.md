# Comparing `tmp/nonebot_plugin_ranfurrypic-1.1.3.tar.gz` & `tmp/nonebot_plugin_ranfurrypic-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ranfurrypic-1.1.3.tar", last modified: Sat May 11 15:53:28 2024, max compression
+gzip compressed data, was "nonebot_plugin_ranfurrypic-1.1.4.tar", last modified: Sat May 11 15:56:36 2024, max compression
```

## Comparing `nonebot_plugin_ranfurrypic-1.1.3.tar` & `nonebot_plugin_ranfurrypic-1.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 15:53:28.716264 nonebot_plugin_ranfurrypic-1.1.3/
--rw-rw-rw-   0        0        0     1082 2024-05-10 14:34:54.000000 nonebot_plugin_ranfurrypic-1.1.3/LICENSE
--rw-rw-rw-   0        0        0     2926 2024-05-11 15:53:28.715268 nonebot_plugin_ranfurrypic-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2559 2024-05-11 15:32:32.000000 nonebot_plugin_ranfurrypic-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 15:53:28.690281 nonebot_plugin_ranfurrypic-1.1.3/nonebot_plugin_RanFurryPic/
--rw-rw-rw-   0        0        0     3145 2024-05-11 15:52:58.000000 nonebot_plugin_ranfurrypic-1.1.3/nonebot_plugin_RanFurryPic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 15:53:28.714265 nonebot_plugin_ranfurrypic-1.1.3/nonebot_plugin_RanFurryPic.egg-info/
--rw-rw-rw-   0        0        0     2926 2024-05-11 15:53:28.000000 nonebot_plugin_ranfurrypic-1.1.3/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2024-05-11 15:53:28.000000 nonebot_plugin_ranfurrypic-1.1.3/nonebot_plugin_RanFurryPic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 15:53:28.000000 nonebot_plugin_ranfurrypic-1.1.3/nonebot_plugin_RanFurryPic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-11 15:53:28.000000 nonebot_plugin_ranfurrypic-1.1.3/nonebot_plugin_RanFurryPic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-05-11 15:53:28.000000 nonebot_plugin_ranfurrypic-1.1.3/nonebot_plugin_RanFurryPic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      380 2024-05-11 15:51:39.000000 nonebot_plugin_ranfurrypic-1.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-11 15:53:28.716264 nonebot_plugin_ranfurrypic-1.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-11 15:56:36.854638 nonebot_plugin_ranfurrypic-1.1.4/
+-rw-rw-rw-   0        0        0     1082 2024-05-10 14:34:54.000000 nonebot_plugin_ranfurrypic-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0     2953 2024-05-11 15:56:36.852639 nonebot_plugin_ranfurrypic-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2586 2024-05-11 15:55:57.000000 nonebot_plugin_ranfurrypic-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 15:56:36.836649 nonebot_plugin_ranfurrypic-1.1.4/nonebot_plugin_RanFurryPic/
+-rw-rw-rw-   0        0        0     3145 2024-05-11 15:52:58.000000 nonebot_plugin_ranfurrypic-1.1.4/nonebot_plugin_RanFurryPic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 15:56:36.851640 nonebot_plugin_ranfurrypic-1.1.4/nonebot_plugin_RanFurryPic.egg-info/
+-rw-rw-rw-   0        0        0     2953 2024-05-11 15:56:36.000000 nonebot_plugin_ranfurrypic-1.1.4/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-05-11 15:56:36.000000 nonebot_plugin_ranfurrypic-1.1.4/nonebot_plugin_RanFurryPic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 15:56:36.000000 nonebot_plugin_ranfurrypic-1.1.4/nonebot_plugin_RanFurryPic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-11 15:56:36.000000 nonebot_plugin_ranfurrypic-1.1.4/nonebot_plugin_RanFurryPic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-05-11 15:56:36.000000 nonebot_plugin_ranfurrypic-1.1.4/nonebot_plugin_RanFurryPic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      380 2024-05-11 15:55:21.000000 nonebot_plugin_ranfurrypic-1.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-11 15:56:36.854638 nonebot_plugin_ranfurrypic-1.1.4/setup.cfg
```

### Comparing `nonebot_plugin_ranfurrypic-1.1.3/LICENSE` & `nonebot_plugin_ranfurrypic-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ranfurrypic-1.1.3/PKG-INFO` & `nonebot_plugin_ranfurrypic-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_RanFurryPic
-Version: 1.1.3
+Version: 1.1.4
 Summary: 基于NoneBot2进行适配的兽云随机毛图插件
 Author-email: Ekac <2396382559@qq.com>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2
@@ -86,7 +86,8 @@
 
 ## TODO LIST
 
 待解决问题:
 
  - [x] 使用httpx发送请求，避免线程堵塞(后期：艹这里让星火帮我改一次就过审核了讯飞nb！)
  - [ ] 自定义消息发送结果（指在`.env`中修改
+ - [ ] 添加搜毛功能
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.1.3 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.1.4 Summary:
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Author-email: Ekac
 <2396382559@qq.com> License: MIT Requires-Python: >=3.9 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-
 Dist: httpx Requires-Dist: nonebot-adapter-onebot
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
   # nonebot-plugin-RanFurryPic _â¨ éæºæ¯å¾ â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
@@ -21,8 +21,8 @@
 1.0çæ¬ææ éç½®é¡¹ï¼å¯å³å®å³ç¨ã ## ð ä½¿ç¨ ### æä»¤è¡¨ |
 æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:--
 --:| | æ¥åªæ¯ | ç¾¤å | å¦ | ç¾¤è | éæºæ¯å¾ | | furry | ç¾¤å |
 å¦ | ç¾¤è | éæºæ¯å¾ | | æ¯æ¯ | ç¾¤å | å¦ | ç¾¤è | éæºæ¯å¾ |
 ## TODO LIST å¾è§£å³é®é¢: - [x]
 ä½¿ç¨httpxåéè¯·æ±ï¼é¿åçº¿ç¨å µå¡
 (åæï¼è¹è¿éè®©æç«å¸®ææ¹ä¸æ¬¡å°±è¿å®¡æ ¸äºè®¯é£nbï¼) - [ ]
-èªå®ä¹æ¶æ¯åéç»æï¼æå¨`.env`ä¸­ä¿®æ¹
+èªå®ä¹æ¶æ¯åéç»æï¼æå¨`.env`ä¸­ä¿®æ¹ - [ ] æ·»å ææ¯åè½
```

### Comparing `nonebot_plugin_ranfurrypic-1.1.3/README.md` & `nonebot_plugin_ranfurrypic-1.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -73,7 +73,8 @@
 
 ## TODO LIST
 
 待解决问题:
 
  - [x] 使用httpx发送请求，避免线程堵塞(后期：艹这里让星火帮我改一次就过审核了讯飞nb！)
  - [ ] 自定义消息发送结果（指在`.env`中修改
+ - [ ] 添加搜毛功能
```

#### html2text {}

```diff
@@ -16,8 +16,8 @@
 1.0çæ¬ææ éç½®é¡¹ï¼å¯å³å®å³ç¨ã ## ð ä½¿ç¨ ### æä»¤è¡¨ |
 æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:--
 --:| | æ¥åªæ¯ | ç¾¤å | å¦ | ç¾¤è | éæºæ¯å¾ | | furry | ç¾¤å |
 å¦ | ç¾¤è | éæºæ¯å¾ | | æ¯æ¯ | ç¾¤å | å¦ | ç¾¤è | éæºæ¯å¾ |
 ## TODO LIST å¾è§£å³é®é¢: - [x]
 ä½¿ç¨httpxåéè¯·æ±ï¼é¿åçº¿ç¨å µå¡
 (åæï¼è¹è¿éè®©æç«å¸®ææ¹ä¸æ¬¡å°±è¿å®¡æ ¸äºè®¯é£nbï¼) - [ ]
-èªå®ä¹æ¶æ¯åéç»æï¼æå¨`.env`ä¸­ä¿®æ¹
+èªå®ä¹æ¶æ¯åéç»æï¼æå¨`.env`ä¸­ä¿®æ¹ - [ ] æ·»å ææ¯åè½
```

### Comparing `nonebot_plugin_ranfurrypic-1.1.3/nonebot_plugin_RanFurryPic/__init__.py` & `nonebot_plugin_ranfurrypic-1.1.4/nonebot_plugin_RanFurryPic/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ranfurrypic-1.1.3/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO` & `nonebot_plugin_ranfurrypic-1.1.4/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_RanFurryPic
-Version: 1.1.3
+Version: 1.1.4
 Summary: 基于NoneBot2进行适配的兽云随机毛图插件
 Author-email: Ekac <2396382559@qq.com>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2
@@ -86,7 +86,8 @@
 
 ## TODO LIST
 
 待解决问题:
 
  - [x] 使用httpx发送请求，避免线程堵塞(后期：艹这里让星火帮我改一次就过审核了讯飞nb！)
  - [ ] 自定义消息发送结果（指在`.env`中修改
+ - [ ] 添加搜毛功能
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.1.3 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.1.4 Summary:
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Author-email: Ekac
 <2396382559@qq.com> License: MIT Requires-Python: >=3.9 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-
 Dist: httpx Requires-Dist: nonebot-adapter-onebot
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
   # nonebot-plugin-RanFurryPic _â¨ éæºæ¯å¾ â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
@@ -21,8 +21,8 @@
 1.0çæ¬ææ éç½®é¡¹ï¼å¯å³å®å³ç¨ã ## ð ä½¿ç¨ ### æä»¤è¡¨ |
 æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:--
 --:| | æ¥åªæ¯ | ç¾¤å | å¦ | ç¾¤è | éæºæ¯å¾ | | furry | ç¾¤å |
 å¦ | ç¾¤è | éæºæ¯å¾ | | æ¯æ¯ | ç¾¤å | å¦ | ç¾¤è | éæºæ¯å¾ |
 ## TODO LIST å¾è§£å³é®é¢: - [x]
 ä½¿ç¨httpxåéè¯·æ±ï¼é¿åçº¿ç¨å µå¡
 (åæï¼è¹è¿éè®©æç«å¸®ææ¹ä¸æ¬¡å°±è¿å®¡æ ¸äºè®¯é£nbï¼) - [ ]
-èªå®ä¹æ¶æ¯åéç»æï¼æå¨`.env`ä¸­ä¿®æ¹
+èªå®ä¹æ¶æ¯åéç»æï¼æå¨`.env`ä¸­ä¿®æ¹ - [ ] æ·»å ææ¯åè½
```

