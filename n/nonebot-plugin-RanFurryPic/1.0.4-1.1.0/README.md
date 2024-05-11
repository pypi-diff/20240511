# Comparing `tmp/nonebot_plugin_ranfurrypic-1.0.4.tar.gz` & `tmp/nonebot_plugin_ranfurrypic-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ranfurrypic-1.0.4.tar", last modified: Sat May 11 13:49:46 2024, max compression
+gzip compressed data, was "nonebot_plugin_ranfurrypic-1.1.0.tar", last modified: Sat May 11 15:19:07 2024, max compression
```

## Comparing `nonebot_plugin_ranfurrypic-1.0.4.tar` & `nonebot_plugin_ranfurrypic-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 13:49:46.381610 nonebot_plugin_ranfurrypic-1.0.4/
--rw-rw-rw-   0        0        0     1082 2024-05-10 14:34:54.000000 nonebot_plugin_ranfurrypic-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     3062 2024-05-11 13:49:46.380611 nonebot_plugin_ranfurrypic-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2613 2024-05-11 13:13:22.000000 nonebot_plugin_ranfurrypic-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 13:49:46.366624 nonebot_plugin_ranfurrypic-1.0.4/nonebot_plugin_RanFurryPic/
--rw-rw-rw-   0        0        0     2845 2024-05-11 13:35:33.000000 nonebot_plugin_ranfurrypic-1.0.4/nonebot_plugin_RanFurryPic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 13:49:46.379612 nonebot_plugin_ranfurrypic-1.0.4/nonebot_plugin_RanFurryPic.egg-info/
--rw-rw-rw-   0        0        0     3062 2024-05-11 13:49:46.000000 nonebot_plugin_ranfurrypic-1.0.4/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-05-11 13:49:46.000000 nonebot_plugin_ranfurrypic-1.0.4/nonebot_plugin_RanFurryPic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 13:49:46.000000 nonebot_plugin_ranfurrypic-1.0.4/nonebot_plugin_RanFurryPic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-05-11 13:49:46.000000 nonebot_plugin_ranfurrypic-1.0.4/nonebot_plugin_RanFurryPic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-05-11 13:49:46.000000 nonebot_plugin_ranfurrypic-1.0.4/nonebot_plugin_RanFurryPic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      383 2024-05-11 13:48:53.000000 nonebot_plugin_ranfurrypic-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-11 13:49:46.381610 nonebot_plugin_ranfurrypic-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1090 2024-05-11 13:08:27.000000 nonebot_plugin_ranfurrypic-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 15:19:07.140524 nonebot_plugin_ranfurrypic-1.1.0/
+-rw-rw-rw-   0        0        0     1082 2024-05-10 14:34:54.000000 nonebot_plugin_ranfurrypic-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2874 2024-05-11 15:19:07.139526 nonebot_plugin_ranfurrypic-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2507 2024-05-11 14:12:40.000000 nonebot_plugin_ranfurrypic-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 15:19:07.112542 nonebot_plugin_ranfurrypic-1.1.0/nonebot_plugin_RanFurryPic/
+-rw-rw-rw-   0        0        0     5262 2024-05-11 15:10:20.000000 nonebot_plugin_ranfurrypic-1.1.0/nonebot_plugin_RanFurryPic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 15:19:07.138526 nonebot_plugin_ranfurrypic-1.1.0/nonebot_plugin_RanFurryPic.egg-info/
+-rw-rw-rw-   0        0        0     2874 2024-05-11 15:19:07.000000 nonebot_plugin_ranfurrypic-1.1.0/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-05-11 15:19:07.000000 nonebot_plugin_ranfurrypic-1.1.0/nonebot_plugin_RanFurryPic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 15:19:07.000000 nonebot_plugin_ranfurrypic-1.1.0/nonebot_plugin_RanFurryPic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-11 15:19:07.000000 nonebot_plugin_ranfurrypic-1.1.0/nonebot_plugin_RanFurryPic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-05-11 15:19:07.000000 nonebot_plugin_ranfurrypic-1.1.0/nonebot_plugin_RanFurryPic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      380 2024-05-11 15:15:22.000000 nonebot_plugin_ranfurrypic-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-11 15:19:07.141523 nonebot_plugin_ranfurrypic-1.1.0/setup.cfg
```

### Comparing `nonebot_plugin_ranfurrypic-1.0.4/LICENSE` & `nonebot_plugin_ranfurrypic-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ranfurrypic-1.0.4/PKG-INFO` & `nonebot_plugin_ranfurrypic-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_RanFurryPic
-Version: 1.0.4
+Version: 1.1.0
 Summary: 基于NoneBot2进行适配的兽云随机毛图插件
-Home-page: https://github.com/Ekac00/nonebot-plugin-RanFurryPic
-Author: Ekac
 Author-email: Ekac <2396382559@qq.com>
 License: MIT
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2
-Requires-Dist: requests
+Requires-Dist: httpx
 Requires-Dist: nonebot-adapter-onebot
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
@@ -37,28 +35,26 @@
 </div>
 
 基于NoneBot2进行适配的兽云随机毛图插件
 
 ## 📖 介绍
 
 兽云官方插件太复杂？功能太杂？看不懂？不兼容？损坏文件结构？
-本插件使用官方<a href="https://console-docs.apipost.cn/preview/6bf01cfebd3e5f96/c4e20a5d1a5db86c?target_id=83fb4f89-221c-4196-bb85-4abf73af73af">API</a>进行编写，无需令牌，无需Token，即可使用随机毛图功能
+本插件使用官方<a href="https://console-docs.apipost.cn/preview/6bf01cfebd3e5f96/c4e20a5d1a5db86c?target_id=83fb4f89-221c-4196-bb85-4abf73af73af">API</a>进行编写，无需令牌，无需Token，即可使用随机毛图功能<br><br>
+在开始前请先点一个免费的star吧谢谢啦~
 
 <details>
 <summary>买家秀</summary>
 
 <img src="https://img2.imgtp.com/2024/05/10/U4xrcU7e.png">
 
 </details>
 
 ## 💿 安装
 
-### 注意！本插件需要`requests`库发送请求，此库在1.0版本中未添加至依赖，请手动进行安装！
-    pip install requests
-
 <details open>
 <summary>使用 nb-cli 安装（推荐）</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
     nb plugin install nonebot-plugin-RanFurryPic
 
 </details>
@@ -67,30 +63,30 @@
 <summary>使用PIP安装</summary>
 在 nonebot2 项目的插件目录下, 打开命令行, 输入安装命令
 
     pip install nonebot-plugin-RanFurryPic
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
-<<<<<<< HEAD
-    plugins = ["nonebot_plugin_template"]
-=======
-<<<<<<< HEAD
     plugins = ["nonebot_plugin_RanFurryPic"]
-=======
-    plugins = ["nonebot_plugin_template"]
->>>>>>> 12a75b0 (v1.0)
->>>>>>> 9106e15 (first commit)
+
 
 </details>
 
 ## ⚙️ 配置
 
 1.0版本暂无配置项，可即安即用。
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | 来只毛 | 群员 | 否 | 群聊 | 随机毛图 |
 | furry | 群员 | 否 | 群聊 | 随机毛图 |
 | 毛毛 | 群员 | 否 | 群聊 | 随机毛图 |
+
+## TODO LIST
+
+待解决问题:
+
+ - [ ] 使用httpx发送请求，避免线程堵塞（防止被dll骂
+ - [ ] 自定义消息发送结果（指在`.env`中修改
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.0.4 Summary:
-åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Home-page: https://
-github.com/Ekac00/nonebot-plugin-RanFurryPic Author: Ekac Author-email: Ekac
-<2396382559@qq.com> License: MIT Requires-Python: >=3.8 Description-Content-
+Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.1.0 Summary:
+åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Author-email: Ekac
+<2396382559@qq.com> License: MIT Requires-Python: >=3.9 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-
-Dist: requests Requires-Dist: nonebot-adapter-onebot
+Dist: httpx Requires-Dist: nonebot-adapter-onebot
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
   # nonebot-plugin-RanFurryPic _â¨ éæºæ¯å¾ â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ ## ð ä»ç»
 å½äºå®æ¹æä»¶å¤ªå¤æï¼åè½å¤ªæï¼çä¸æï¼ä¸å¼å®¹ï¼æåæä»¶ç»æï¼
 æ¬æä»¶ä½¿ç¨å®æ¹_A_P_Iè¿è¡ç¼åï¼æ éä»¤çï¼æ éTokenï¼å³å¯ä½¿ç¨éæºæ¯å¾åè½
-ä¹°å®¶ç§ [https://img2.imgtp.com/2024/05/10/U4xrcU7e.png]## ð¿ å®è£ ###
-æ³¨æï¼æ¬æä»¶éè¦`requests`åºåéè¯·æ±ï¼æ­¤åºå¨1.0çæ¬ä¸­æªæ·»å è³ä¾èµï¼è¯·æå¨è¿è¡å®è£ï¼
-pip install requests ä½¿ç¨ nb-cli å®è£ï¼æ¨èï¼ å¨ nonebot2
-é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
-install nonebot-plugin-RanFurryPic ä½¿ç¨PIPå®è£ å¨ nonebot2
-é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, è¾å¥å®è£å½ä»¤ pip install
-nonebot-plugin-RanFurryPic æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
-`pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ <<<<<<< HEAD
-plugins = ["nonebot_plugin_template"] ======= <<<<<<< HEAD plugins =
-["nonebot_plugin_RanFurryPic"] ======= plugins = ["nonebot_plugin_template"]
->>>>>>> 12a75b0 (v1.0) >>>>>>> 9106e15 (first commit) ## âï¸ éç½®
+
+å¨å¼å§åè¯·åç¹ä¸ä¸ªåè´¹çstarå§è°¢è°¢å¦~ ä¹°å®¶ç§ [https://
+img2.imgtp.com/2024/05/10/U4xrcU7e.png]## ð¿ å®è£ ä½¿ç¨ nb-cli
+å®è£ï¼æ¨èï¼ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
+è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-RanFurryPic
+ä½¿ç¨PIPå®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
+è¾å¥å®è£å½ä»¤ pip install nonebot-plugin-RanFurryPic æå¼ nonebot2
+é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]`
+é¨åè¿½å åå¥ plugins = ["nonebot_plugin_RanFurryPic"] ## âï¸ éç½®
 1.0çæ¬ææ éç½®é¡¹ï¼å¯å³å®å³ç¨ã ## ð ä½¿ç¨ ### æä»¤è¡¨ |
 æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:--
 --:| | æ¥åªæ¯ | ç¾¤å | å¦ | ç¾¤è | éæºæ¯å¾ | | furry | ç¾¤å |
 å¦ | ç¾¤è | éæºæ¯å¾ | | æ¯æ¯ | ç¾¤å | å¦ | ç¾¤è | éæºæ¯å¾ |
+## TODO LIST å¾è§£å³é®é¢: - [ ]
+ä½¿ç¨httpxåéè¯·æ±ï¼é¿åçº¿ç¨å µå¡ï¼é²æ­¢è¢«dlléª - [ ]
+èªå®ä¹æ¶æ¯åéç»æï¼æå¨`.env`ä¸­ä¿®æ¹
```

### Comparing `nonebot_plugin_ranfurrypic-1.0.4/README.md` & `nonebot_plugin_ranfurrypic-1.1.0/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: nonebot_plugin_RanFurryPic
+Version: 1.1.0
+Summary: 基于NoneBot2进行适配的兽云随机毛图插件
+Author-email: Ekac <2396382559@qq.com>
+License: MIT
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: nonebot2
+Requires-Dist: httpx
+Requires-Dist: nonebot-adapter-onebot
+
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
@@ -22,28 +35,26 @@
 </div>
 
 基于NoneBot2进行适配的兽云随机毛图插件
 
 ## 📖 介绍
 
 兽云官方插件太复杂？功能太杂？看不懂？不兼容？损坏文件结构？
-本插件使用官方<a href="https://console-docs.apipost.cn/preview/6bf01cfebd3e5f96/c4e20a5d1a5db86c?target_id=83fb4f89-221c-4196-bb85-4abf73af73af">API</a>进行编写，无需令牌，无需Token，即可使用随机毛图功能
+本插件使用官方<a href="https://console-docs.apipost.cn/preview/6bf01cfebd3e5f96/c4e20a5d1a5db86c?target_id=83fb4f89-221c-4196-bb85-4abf73af73af">API</a>进行编写，无需令牌，无需Token，即可使用随机毛图功能<br><br>
+在开始前请先点一个免费的star吧谢谢啦~
 
 <details>
 <summary>买家秀</summary>
 
 <img src="https://img2.imgtp.com/2024/05/10/U4xrcU7e.png">
 
 </details>
 
 ## 💿 安装
 
-### 注意！本插件需要`requests`库发送请求，此库在1.0版本中未添加至依赖，请手动进行安装！
-    pip install requests
-
 <details open>
 <summary>使用 nb-cli 安装（推荐）</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
     nb plugin install nonebot-plugin-RanFurryPic
 
 </details>
@@ -52,30 +63,30 @@
 <summary>使用PIP安装</summary>
 在 nonebot2 项目的插件目录下, 打开命令行, 输入安装命令
 
     pip install nonebot-plugin-RanFurryPic
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
-<<<<<<< HEAD
-    plugins = ["nonebot_plugin_template"]
-=======
-<<<<<<< HEAD
     plugins = ["nonebot_plugin_RanFurryPic"]
-=======
-    plugins = ["nonebot_plugin_template"]
->>>>>>> 12a75b0 (v1.0)
->>>>>>> 9106e15 (first commit)
+
 
 </details>
 
 ## ⚙️ 配置
 
 1.0版本暂无配置项，可即安即用。
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | 来只毛 | 群员 | 否 | 群聊 | 随机毛图 |
 | furry | 群员 | 否 | 群聊 | 随机毛图 |
 | 毛毛 | 群员 | 否 | 群聊 | 随机毛图 |
+
+## TODO LIST
+
+待解决问题:
+
+ - [ ] 使用httpx发送请求，避免线程堵塞（防止被dll骂
+ - [ ] 自定义消息发送结果（指在`.env`中修改
```

#### html2text {}

```diff
@@ -1,21 +1,27 @@
+Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.1.0 Summary:
+åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Author-email: Ekac
+<2396382559@qq.com> License: MIT Requires-Python: >=3.9 Description-Content-
+Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-
+Dist: httpx Requires-Dist: nonebot-adapter-onebot
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
   # nonebot-plugin-RanFurryPic _â¨ éæºæ¯å¾ â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ ## ð ä»ç»
 å½äºå®æ¹æä»¶å¤ªå¤æï¼åè½å¤ªæï¼çä¸æï¼ä¸å¼å®¹ï¼æåæä»¶ç»æï¼
 æ¬æä»¶ä½¿ç¨å®æ¹_A_P_Iè¿è¡ç¼åï¼æ éä»¤çï¼æ éTokenï¼å³å¯ä½¿ç¨éæºæ¯å¾åè½
-ä¹°å®¶ç§ [https://img2.imgtp.com/2024/05/10/U4xrcU7e.png]## ð¿ å®è£ ###
-æ³¨æï¼æ¬æä»¶éè¦`requests`åºåéè¯·æ±ï¼æ­¤åºå¨1.0çæ¬ä¸­æªæ·»å è³ä¾èµï¼è¯·æå¨è¿è¡å®è£ï¼
-pip install requests ä½¿ç¨ nb-cli å®è£ï¼æ¨èï¼ å¨ nonebot2
-é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
-install nonebot-plugin-RanFurryPic ä½¿ç¨PIPå®è£ å¨ nonebot2
-é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, è¾å¥å®è£å½ä»¤ pip install
-nonebot-plugin-RanFurryPic æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
-`pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ <<<<<<< HEAD
-plugins = ["nonebot_plugin_template"] ======= <<<<<<< HEAD plugins =
-["nonebot_plugin_RanFurryPic"] ======= plugins = ["nonebot_plugin_template"]
->>>>>>> 12a75b0 (v1.0) >>>>>>> 9106e15 (first commit) ## âï¸ éç½®
+
+å¨å¼å§åè¯·åç¹ä¸ä¸ªåè´¹çstarå§è°¢è°¢å¦~ ä¹°å®¶ç§ [https://
+img2.imgtp.com/2024/05/10/U4xrcU7e.png]## ð¿ å®è£ ä½¿ç¨ nb-cli
+å®è£ï¼æ¨èï¼ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
+è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-RanFurryPic
+ä½¿ç¨PIPå®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
+è¾å¥å®è£å½ä»¤ pip install nonebot-plugin-RanFurryPic æå¼ nonebot2
+é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]`
+é¨åè¿½å åå¥ plugins = ["nonebot_plugin_RanFurryPic"] ## âï¸ éç½®
 1.0çæ¬ææ éç½®é¡¹ï¼å¯å³å®å³ç¨ã ## ð ä½¿ç¨ ### æä»¤è¡¨ |
 æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:--
 --:| | æ¥åªæ¯ | ç¾¤å | å¦ | ç¾¤è | éæºæ¯å¾ | | furry | ç¾¤å |
 å¦ | ç¾¤è | éæºæ¯å¾ | | æ¯æ¯ | ç¾¤å | å¦ | ç¾¤è | éæºæ¯å¾ |
+## TODO LIST å¾è§£å³é®é¢: - [ ]
+ä½¿ç¨httpxåéè¯·æ±ï¼é¿åçº¿ç¨å µå¡ï¼é²æ­¢è¢«dlléª - [ ]
+èªå®ä¹æ¶æ¯åéç»æï¼æå¨`.env`ä¸­ä¿®æ¹
```

### Comparing `nonebot_plugin_ranfurrypic-1.0.4/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO` & `nonebot_plugin_ranfurrypic-1.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: nonebot_plugin_RanFurryPic
-Version: 1.0.4
-Summary: 基于NoneBot2进行适配的兽云随机毛图插件
-Home-page: https://github.com/Ekac00/nonebot-plugin-RanFurryPic
-Author: Ekac
-Author-email: Ekac <2396382559@qq.com>
-License: MIT
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: nonebot2
-Requires-Dist: requests
-Requires-Dist: nonebot-adapter-onebot
-
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
@@ -37,28 +22,26 @@
 </div>
 
 基于NoneBot2进行适配的兽云随机毛图插件
 
 ## 📖 介绍
 
 兽云官方插件太复杂？功能太杂？看不懂？不兼容？损坏文件结构？
-本插件使用官方<a href="https://console-docs.apipost.cn/preview/6bf01cfebd3e5f96/c4e20a5d1a5db86c?target_id=83fb4f89-221c-4196-bb85-4abf73af73af">API</a>进行编写，无需令牌，无需Token，即可使用随机毛图功能
+本插件使用官方<a href="https://console-docs.apipost.cn/preview/6bf01cfebd3e5f96/c4e20a5d1a5db86c?target_id=83fb4f89-221c-4196-bb85-4abf73af73af">API</a>进行编写，无需令牌，无需Token，即可使用随机毛图功能<br><br>
+在开始前请先点一个免费的star吧谢谢啦~
 
 <details>
 <summary>买家秀</summary>
 
 <img src="https://img2.imgtp.com/2024/05/10/U4xrcU7e.png">
 
 </details>
 
 ## 💿 安装
 
-### 注意！本插件需要`requests`库发送请求，此库在1.0版本中未添加至依赖，请手动进行安装！
-    pip install requests
-
 <details open>
 <summary>使用 nb-cli 安装（推荐）</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
     nb plugin install nonebot-plugin-RanFurryPic
 
 </details>
@@ -67,30 +50,30 @@
 <summary>使用PIP安装</summary>
 在 nonebot2 项目的插件目录下, 打开命令行, 输入安装命令
 
     pip install nonebot-plugin-RanFurryPic
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
-<<<<<<< HEAD
-    plugins = ["nonebot_plugin_template"]
-=======
-<<<<<<< HEAD
     plugins = ["nonebot_plugin_RanFurryPic"]
-=======
-    plugins = ["nonebot_plugin_template"]
->>>>>>> 12a75b0 (v1.0)
->>>>>>> 9106e15 (first commit)
+
 
 </details>
 
 ## ⚙️ 配置
 
 1.0版本暂无配置项，可即安即用。
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | 来只毛 | 群员 | 否 | 群聊 | 随机毛图 |
 | furry | 群员 | 否 | 群聊 | 随机毛图 |
 | 毛毛 | 群员 | 否 | 群聊 | 随机毛图 |
+
+## TODO LIST
+
+待解决问题:
+
+ - [ ] 使用httpx发送请求，避免线程堵塞（防止被dll骂
+ - [ ] 自定义消息发送结果（指在`.env`中修改
```

#### html2text {}

```diff
@@ -1,27 +1,22 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.0.4 Summary:
-åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Home-page: https://
-github.com/Ekac00/nonebot-plugin-RanFurryPic Author: Ekac Author-email: Ekac
-<2396382559@qq.com> License: MIT Requires-Python: >=3.8 Description-Content-
-Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-
-Dist: requests Requires-Dist: nonebot-adapter-onebot
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
   # nonebot-plugin-RanFurryPic _â¨ éæºæ¯å¾ â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ ## ð ä»ç»
 å½äºå®æ¹æä»¶å¤ªå¤æï¼åè½å¤ªæï¼çä¸æï¼ä¸å¼å®¹ï¼æåæä»¶ç»æï¼
 æ¬æä»¶ä½¿ç¨å®æ¹_A_P_Iè¿è¡ç¼åï¼æ éä»¤çï¼æ éTokenï¼å³å¯ä½¿ç¨éæºæ¯å¾åè½
-ä¹°å®¶ç§ [https://img2.imgtp.com/2024/05/10/U4xrcU7e.png]## ð¿ å®è£ ###
-æ³¨æï¼æ¬æä»¶éè¦`requests`åºåéè¯·æ±ï¼æ­¤åºå¨1.0çæ¬ä¸­æªæ·»å è³ä¾èµï¼è¯·æå¨è¿è¡å®è£ï¼
-pip install requests ä½¿ç¨ nb-cli å®è£ï¼æ¨èï¼ å¨ nonebot2
-é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
-install nonebot-plugin-RanFurryPic ä½¿ç¨PIPå®è£ å¨ nonebot2
-é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, è¾å¥å®è£å½ä»¤ pip install
-nonebot-plugin-RanFurryPic æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
-`pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ <<<<<<< HEAD
-plugins = ["nonebot_plugin_template"] ======= <<<<<<< HEAD plugins =
-["nonebot_plugin_RanFurryPic"] ======= plugins = ["nonebot_plugin_template"]
->>>>>>> 12a75b0 (v1.0) >>>>>>> 9106e15 (first commit) ## âï¸ éç½®
+
+å¨å¼å§åè¯·åç¹ä¸ä¸ªåè´¹çstarå§è°¢è°¢å¦~ ä¹°å®¶ç§ [https://
+img2.imgtp.com/2024/05/10/U4xrcU7e.png]## ð¿ å®è£ ä½¿ç¨ nb-cli
+å®è£ï¼æ¨èï¼ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
+è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-RanFurryPic
+ä½¿ç¨PIPå®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
+è¾å¥å®è£å½ä»¤ pip install nonebot-plugin-RanFurryPic æå¼ nonebot2
+é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]`
+é¨åè¿½å åå¥ plugins = ["nonebot_plugin_RanFurryPic"] ## âï¸ éç½®
 1.0çæ¬ææ éç½®é¡¹ï¼å¯å³å®å³ç¨ã ## ð ä½¿ç¨ ### æä»¤è¡¨ |
 æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:--
 --:| | æ¥åªæ¯ | ç¾¤å | å¦ | ç¾¤è | éæºæ¯å¾ | | furry | ç¾¤å |
 å¦ | ç¾¤è | éæºæ¯å¾ | | æ¯æ¯ | ç¾¤å | å¦ | ç¾¤è | éæºæ¯å¾ |
+## TODO LIST å¾è§£å³é®é¢: - [ ]
+ä½¿ç¨httpxåéè¯·æ±ï¼é¿åçº¿ç¨å µå¡ï¼é²æ­¢è¢«dlléª - [ ]
+èªå®ä¹æ¶æ¯åéç»æï¼æå¨`.env`ä¸­ä¿®æ¹
```

