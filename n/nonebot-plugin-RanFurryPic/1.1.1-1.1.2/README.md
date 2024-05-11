# Comparing `tmp/nonebot_plugin_ranfurrypic-1.1.1.tar.gz` & `tmp/nonebot_plugin_ranfurrypic-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ranfurrypic-1.1.1.tar", last modified: Sat May 11 15:23:04 2024, max compression
+gzip compressed data, was "nonebot_plugin_ranfurrypic-1.1.2.tar", last modified: Sat May 11 15:33:22 2024, max compression
```

## Comparing `nonebot_plugin_ranfurrypic-1.1.1.tar` & `nonebot_plugin_ranfurrypic-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 15:23:04.090557 nonebot_plugin_ranfurrypic-1.1.1/
--rw-rw-rw-   0        0        0     1082 2024-05-10 14:34:54.000000 nonebot_plugin_ranfurrypic-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     2874 2024-05-11 15:23:04.089558 nonebot_plugin_ranfurrypic-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2507 2024-05-11 14:12:40.000000 nonebot_plugin_ranfurrypic-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 15:23:04.075566 nonebot_plugin_ranfurrypic-1.1.1/nonebot_plugin_RanFurryPic/
--rw-rw-rw-   0        0        0     5262 2024-05-11 15:22:26.000000 nonebot_plugin_ranfurrypic-1.1.1/nonebot_plugin_RanFurryPic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 15:23:04.088560 nonebot_plugin_ranfurrypic-1.1.1/nonebot_plugin_RanFurryPic.egg-info/
--rw-rw-rw-   0        0        0     2874 2024-05-11 15:23:04.000000 nonebot_plugin_ranfurrypic-1.1.1/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2024-05-11 15:23:04.000000 nonebot_plugin_ranfurrypic-1.1.1/nonebot_plugin_RanFurryPic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 15:23:04.000000 nonebot_plugin_ranfurrypic-1.1.1/nonebot_plugin_RanFurryPic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-11 15:23:04.000000 nonebot_plugin_ranfurrypic-1.1.1/nonebot_plugin_RanFurryPic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-05-11 15:23:04.000000 nonebot_plugin_ranfurrypic-1.1.1/nonebot_plugin_RanFurryPic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      380 2024-05-11 15:22:39.000000 nonebot_plugin_ranfurrypic-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-11 15:23:04.091557 nonebot_plugin_ranfurrypic-1.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-11 15:33:22.657315 nonebot_plugin_ranfurrypic-1.1.2/
+-rw-rw-rw-   0        0        0     1082 2024-05-10 14:34:54.000000 nonebot_plugin_ranfurrypic-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     2926 2024-05-11 15:33:22.656300 nonebot_plugin_ranfurrypic-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2559 2024-05-11 15:32:32.000000 nonebot_plugin_ranfurrypic-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 15:33:22.629318 nonebot_plugin_ranfurrypic-1.1.2/nonebot_plugin_RanFurryPic/
+-rw-rw-rw-   0        0        0     5262 2024-05-11 15:22:26.000000 nonebot_plugin_ranfurrypic-1.1.2/nonebot_plugin_RanFurryPic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 15:33:22.654305 nonebot_plugin_ranfurrypic-1.1.2/nonebot_plugin_RanFurryPic.egg-info/
+-rw-rw-rw-   0        0        0     2926 2024-05-11 15:33:22.000000 nonebot_plugin_ranfurrypic-1.1.2/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-05-11 15:33:22.000000 nonebot_plugin_ranfurrypic-1.1.2/nonebot_plugin_RanFurryPic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 15:33:22.000000 nonebot_plugin_ranfurrypic-1.1.2/nonebot_plugin_RanFurryPic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-11 15:33:22.000000 nonebot_plugin_ranfurrypic-1.1.2/nonebot_plugin_RanFurryPic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-05-11 15:33:22.000000 nonebot_plugin_ranfurrypic-1.1.2/nonebot_plugin_RanFurryPic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      380 2024-05-11 15:30:55.000000 nonebot_plugin_ranfurrypic-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-11 15:33:22.657315 nonebot_plugin_ranfurrypic-1.1.2/setup.cfg
```

### Comparing `nonebot_plugin_ranfurrypic-1.1.1/LICENSE` & `nonebot_plugin_ranfurrypic-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ranfurrypic-1.1.1/PKG-INFO` & `nonebot_plugin_ranfurrypic-1.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_RanFurryPic
-Version: 1.1.1
+Version: 1.1.2
 Summary: 基于NoneBot2进行适配的兽云随机毛图插件
 Author-email: Ekac <2396382559@qq.com>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2
@@ -84,9 +84,9 @@
 | furry | 群员 | 否 | 群聊 | 随机毛图 |
 | 毛毛 | 群员 | 否 | 群聊 | 随机毛图 |
 
 ## TODO LIST
 
 待解决问题:
 
- - [ ] 使用httpx发送请求，避免线程堵塞（防止被dll骂
+ - [x] 使用httpx发送请求，避免线程堵塞(后期：艹这里让星火帮我改一次就过审核了讯飞nb！)
  - [ ] 自定义消息发送结果（指在`.env`中修改
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.1.2 Summary:
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Author-email: Ekac
 <2396382559@qq.com> License: MIT Requires-Python: >=3.9 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-
 Dist: httpx Requires-Dist: nonebot-adapter-onebot
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
   # nonebot-plugin-RanFurryPic _â¨ éæºæ¯å¾ â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
@@ -18,10 +18,11 @@
 è¾å¥å®è£å½ä»¤ pip install nonebot-plugin-RanFurryPic æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]`
 é¨åè¿½å åå¥ plugins = ["nonebot_plugin_RanFurryPic"] ## âï¸ éç½®
 1.0çæ¬ææ éç½®é¡¹ï¼å¯å³å®å³ç¨ã ## ð ä½¿ç¨ ### æä»¤è¡¨ |
 æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:--
 --:| | æ¥åªæ¯ | ç¾¤å | å¦ | ç¾¤è | éæºæ¯å¾ | | furry | ç¾¤å |
 å¦ | ç¾¤è | éæºæ¯å¾ | | æ¯æ¯ | ç¾¤å | å¦ | ç¾¤è | éæºæ¯å¾ |
-## TODO LIST å¾è§£å³é®é¢: - [ ]
-ä½¿ç¨httpxåéè¯·æ±ï¼é¿åçº¿ç¨å µå¡ï¼é²æ­¢è¢«dlléª - [ ]
+## TODO LIST å¾è§£å³é®é¢: - [x]
+ä½¿ç¨httpxåéè¯·æ±ï¼é¿åçº¿ç¨å µå¡
+(åæï¼è¹è¿éè®©æç«å¸®ææ¹ä¸æ¬¡å°±è¿å®¡æ ¸äºè®¯é£nbï¼) - [ ]
 èªå®ä¹æ¶æ¯åéç»æï¼æå¨`.env`ä¸­ä¿®æ¹
```

### Comparing `nonebot_plugin_ranfurrypic-1.1.1/README.md` & `nonebot_plugin_ranfurrypic-1.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -71,9 +71,9 @@
 | furry | 群员 | 否 | 群聊 | 随机毛图 |
 | 毛毛 | 群员 | 否 | 群聊 | 随机毛图 |
 
 ## TODO LIST
 
 待解决问题:
 
- - [ ] 使用httpx发送请求，避免线程堵塞（防止被dll骂
+ - [x] 使用httpx发送请求，避免线程堵塞(后期：艹这里让星火帮我改一次就过审核了讯飞nb！)
  - [ ] 自定义消息发送结果（指在`.env`中修改
```

#### html2text {}

```diff
@@ -13,10 +13,11 @@
 è¾å¥å®è£å½ä»¤ pip install nonebot-plugin-RanFurryPic æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]`
 é¨åè¿½å åå¥ plugins = ["nonebot_plugin_RanFurryPic"] ## âï¸ éç½®
 1.0çæ¬ææ éç½®é¡¹ï¼å¯å³å®å³ç¨ã ## ð ä½¿ç¨ ### æä»¤è¡¨ |
 æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:--
 --:| | æ¥åªæ¯ | ç¾¤å | å¦ | ç¾¤è | éæºæ¯å¾ | | furry | ç¾¤å |
 å¦ | ç¾¤è | éæºæ¯å¾ | | æ¯æ¯ | ç¾¤å | å¦ | ç¾¤è | éæºæ¯å¾ |
-## TODO LIST å¾è§£å³é®é¢: - [ ]
-ä½¿ç¨httpxåéè¯·æ±ï¼é¿åçº¿ç¨å µå¡ï¼é²æ­¢è¢«dlléª - [ ]
+## TODO LIST å¾è§£å³é®é¢: - [x]
+ä½¿ç¨httpxåéè¯·æ±ï¼é¿åçº¿ç¨å µå¡
+(åæï¼è¹è¿éè®©æç«å¸®ææ¹ä¸æ¬¡å°±è¿å®¡æ ¸äºè®¯é£nbï¼) - [ ]
 èªå®ä¹æ¶æ¯åéç»æï¼æå¨`.env`ä¸­ä¿®æ¹
```

### Comparing `nonebot_plugin_ranfurrypic-1.1.1/nonebot_plugin_RanFurryPic/__init__.py` & `nonebot_plugin_ranfurrypic-1.1.2/nonebot_plugin_RanFurryPic/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ranfurrypic-1.1.1/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO` & `nonebot_plugin_ranfurrypic-1.1.2/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_RanFurryPic
-Version: 1.1.1
+Version: 1.1.2
 Summary: 基于NoneBot2进行适配的兽云随机毛图插件
 Author-email: Ekac <2396382559@qq.com>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2
@@ -84,9 +84,9 @@
 | furry | 群员 | 否 | 群聊 | 随机毛图 |
 | 毛毛 | 群员 | 否 | 群聊 | 随机毛图 |
 
 ## TODO LIST
 
 待解决问题:
 
- - [ ] 使用httpx发送请求，避免线程堵塞（防止被dll骂
+ - [x] 使用httpx发送请求，避免线程堵塞(后期：艹这里让星火帮我改一次就过审核了讯飞nb！)
  - [ ] 自定义消息发送结果（指在`.env`中修改
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.1.2 Summary:
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Author-email: Ekac
 <2396382559@qq.com> License: MIT Requires-Python: >=3.9 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-
 Dist: httpx Requires-Dist: nonebot-adapter-onebot
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
   # nonebot-plugin-RanFurryPic _â¨ éæºæ¯å¾ â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
@@ -18,10 +18,11 @@
 è¾å¥å®è£å½ä»¤ pip install nonebot-plugin-RanFurryPic æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]`
 é¨åè¿½å åå¥ plugins = ["nonebot_plugin_RanFurryPic"] ## âï¸ éç½®
 1.0çæ¬ææ éç½®é¡¹ï¼å¯å³å®å³ç¨ã ## ð ä½¿ç¨ ### æä»¤è¡¨ |
 æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:--
 --:| | æ¥åªæ¯ | ç¾¤å | å¦ | ç¾¤è | éæºæ¯å¾ | | furry | ç¾¤å |
 å¦ | ç¾¤è | éæºæ¯å¾ | | æ¯æ¯ | ç¾¤å | å¦ | ç¾¤è | éæºæ¯å¾ |
-## TODO LIST å¾è§£å³é®é¢: - [ ]
-ä½¿ç¨httpxåéè¯·æ±ï¼é¿åçº¿ç¨å µå¡ï¼é²æ­¢è¢«dlléª - [ ]
+## TODO LIST å¾è§£å³é®é¢: - [x]
+ä½¿ç¨httpxåéè¯·æ±ï¼é¿åçº¿ç¨å µå¡
+(åæï¼è¹è¿éè®©æç«å¸®ææ¹ä¸æ¬¡å°±è¿å®¡æ ¸äºè®¯é£nbï¼) - [ ]
 èªå®ä¹æ¶æ¯åéç»æï¼æå¨`.env`ä¸­ä¿®æ¹
```

