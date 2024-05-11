# Comparing `tmp/nonebot_plugin_ranfurrypic-1.0.3.3.tar.gz` & `tmp/nonebot_plugin_ranfurrypic-1.0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ranfurrypic-1.0.3.3.tar", last modified: Sat May 11 13:09:17 2024, max compression
+gzip compressed data, was "nonebot_plugin_ranfurrypic-1.0.3.4.tar", last modified: Sat May 11 13:37:14 2024, max compression
```

## Comparing `nonebot_plugin_ranfurrypic-1.0.3.3.tar` & `nonebot_plugin_ranfurrypic-1.0.3.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 13:09:17.789526 nonebot_plugin_ranfurrypic-1.0.3.3/
--rw-rw-rw-   0        0        0     1082 2024-05-10 14:34:54.000000 nonebot_plugin_ranfurrypic-1.0.3.3/LICENSE
--rw-rw-rw-   0        0        0     2968 2024-05-11 13:09:17.788527 nonebot_plugin_ranfurrypic-1.0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     2515 2024-05-11 12:16:25.000000 nonebot_plugin_ranfurrypic-1.0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 13:09:17.752549 nonebot_plugin_ranfurrypic-1.0.3.3/nonebot_plugin_RanFurryPic/
--rw-rw-rw-   0        0        0     2857 2024-05-11 13:07:56.000000 nonebot_plugin_ranfurrypic-1.0.3.3/nonebot_plugin_RanFurryPic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 13:09:17.787528 nonebot_plugin_ranfurrypic-1.0.3.3/nonebot_plugin_RanFurryPic.egg-info/
--rw-rw-rw-   0        0        0     2968 2024-05-11 13:09:17.000000 nonebot_plugin_ranfurrypic-1.0.3.3/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-05-11 13:09:17.000000 nonebot_plugin_ranfurrypic-1.0.3.3/nonebot_plugin_RanFurryPic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 13:09:17.000000 nonebot_plugin_ranfurrypic-1.0.3.3/nonebot_plugin_RanFurryPic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-05-11 13:09:17.000000 nonebot_plugin_ranfurrypic-1.0.3.3/nonebot_plugin_RanFurryPic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-05-11 13:09:17.000000 nonebot_plugin_ranfurrypic-1.0.3.3/nonebot_plugin_RanFurryPic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      387 2024-05-11 13:08:02.000000 nonebot_plugin_ranfurrypic-1.0.3.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-11 13:09:17.789526 nonebot_plugin_ranfurrypic-1.0.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1090 2024-05-11 13:08:27.000000 nonebot_plugin_ranfurrypic-1.0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 13:37:14.016548 nonebot_plugin_ranfurrypic-1.0.3.4/
+-rw-rw-rw-   0        0        0     1082 2024-05-10 14:34:54.000000 nonebot_plugin_ranfurrypic-1.0.3.4/LICENSE
+-rw-rw-rw-   0        0        0     3066 2024-05-11 13:37:14.013551 nonebot_plugin_ranfurrypic-1.0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2613 2024-05-11 13:13:22.000000 nonebot_plugin_ranfurrypic-1.0.3.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 13:37:13.999561 nonebot_plugin_ranfurrypic-1.0.3.4/nonebot_plugin_RanFurryPic/
+-rw-rw-rw-   0        0        0     2845 2024-05-11 13:35:33.000000 nonebot_plugin_ranfurrypic-1.0.3.4/nonebot_plugin_RanFurryPic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 13:37:14.012551 nonebot_plugin_ranfurrypic-1.0.3.4/nonebot_plugin_RanFurryPic.egg-info/
+-rw-rw-rw-   0        0        0     3066 2024-05-11 13:37:13.000000 nonebot_plugin_ranfurrypic-1.0.3.4/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2024-05-11 13:37:13.000000 nonebot_plugin_ranfurrypic-1.0.3.4/nonebot_plugin_RanFurryPic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 13:37:13.000000 nonebot_plugin_ranfurrypic-1.0.3.4/nonebot_plugin_RanFurryPic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-11 13:37:13.000000 nonebot_plugin_ranfurrypic-1.0.3.4/nonebot_plugin_RanFurryPic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-05-11 13:37:13.000000 nonebot_plugin_ranfurrypic-1.0.3.4/nonebot_plugin_RanFurryPic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      387 2024-05-11 13:36:38.000000 nonebot_plugin_ranfurrypic-1.0.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-11 13:37:14.016548 nonebot_plugin_ranfurrypic-1.0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1090 2024-05-11 13:08:27.000000 nonebot_plugin_ranfurrypic-1.0.3.4/setup.py
```

### Comparing `nonebot_plugin_ranfurrypic-1.0.3.3/LICENSE` & `nonebot_plugin_ranfurrypic-1.0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ranfurrypic-1.0.3.3/PKG-INFO` & `nonebot_plugin_ranfurrypic-1.0.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_RanFurryPic
-Version: 1.0.3.3
+Version: 1.0.3.4
 Summary: 基于NoneBot2进行适配的兽云随机毛图插件
 Home-page: https://github.com/Ekac00/nonebot-plugin-RanFurryPic
 Author: Ekac
 Author-email: Ekac00 <2396382559@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -68,18 +68,22 @@
 在 nonebot2 项目的插件目录下, 打开命令行, 输入安装命令
 
     pip install nonebot-plugin-RanFurryPic
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
 <<<<<<< HEAD
+    plugins = ["nonebot_plugin_template"]
+=======
+<<<<<<< HEAD
     plugins = ["nonebot_plugin_RanFurryPic"]
 =======
     plugins = ["nonebot_plugin_template"]
 >>>>>>> 12a75b0 (v1.0)
+>>>>>>> 9106e15 (first commit)
 
 </details>
 
 ## ⚙️ 配置
 
 1.0版本暂无配置项，可即安即用。
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.0.3.3
+Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.0.3.4
 Summary: åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Home-page:
 https://github.com/Ekac00/nonebot-plugin-RanFurryPic Author: Ekac Author-email:
 Ekac00 <2396382559@qq.com> License: MIT Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2
 Requires-Dist: requests Requires-Dist: nonebot-adapter-onebot
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
@@ -14,13 +14,14 @@
 æ³¨æï¼æ¬æä»¶éè¦`requests`åºåéè¯·æ±ï¼æ­¤åºå¨1.0çæ¬ä¸­æªæ·»å è³ä¾èµï¼è¯·æå¨è¿è¡å®è£ï¼
 pip install requests ä½¿ç¨ nb-cli å®è£ï¼æ¨èï¼ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot-plugin-RanFurryPic ä½¿ç¨PIPå®è£ å¨ nonebot2
 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, è¾å¥å®è£å½ä»¤ pip install
 nonebot-plugin-RanFurryPic æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ <<<<<<< HEAD
-plugins = ["nonebot_plugin_RanFurryPic"] ======= plugins =
-["nonebot_plugin_template"] >>>>>>> 12a75b0 (v1.0) ## âï¸ éç½®
+plugins = ["nonebot_plugin_template"] ======= <<<<<<< HEAD plugins =
+["nonebot_plugin_RanFurryPic"] ======= plugins = ["nonebot_plugin_template"]
+>>>>>>> 12a75b0 (v1.0) >>>>>>> 9106e15 (first commit) ## âï¸ éç½®
 1.0çæ¬ææ éç½®é¡¹ï¼å¯å³å®å³ç¨ã ## ð ä½¿ç¨ ### æä»¤è¡¨ |
 æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:--
 --:| | æ¥åªæ¯ | ç¾¤å | å¦ | ç¾¤è | éæºæ¯å¾ | | furry | ç¾¤å |
 å¦ | ç¾¤è | éæºæ¯å¾ | | æ¯æ¯ | ç¾¤å | å¦ | ç¾¤è | éæºæ¯å¾ |
```

### Comparing `nonebot_plugin_ranfurrypic-1.0.3.3/README.md` & `nonebot_plugin_ranfurrypic-1.0.3.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -53,18 +53,22 @@
 在 nonebot2 项目的插件目录下, 打开命令行, 输入安装命令
 
     pip install nonebot-plugin-RanFurryPic
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
 <<<<<<< HEAD
+    plugins = ["nonebot_plugin_template"]
+=======
+<<<<<<< HEAD
     plugins = ["nonebot_plugin_RanFurryPic"]
 =======
     plugins = ["nonebot_plugin_template"]
 >>>>>>> 12a75b0 (v1.0)
+>>>>>>> 9106e15 (first commit)
 
 </details>
 
 ## ⚙️ 配置
 
 1.0版本暂无配置项，可即安即用。
```

#### html2text {}

```diff
@@ -8,13 +8,14 @@
 æ³¨æï¼æ¬æä»¶éè¦`requests`åºåéè¯·æ±ï¼æ­¤åºå¨1.0çæ¬ä¸­æªæ·»å è³ä¾èµï¼è¯·æå¨è¿è¡å®è£ï¼
 pip install requests ä½¿ç¨ nb-cli å®è£ï¼æ¨èï¼ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot-plugin-RanFurryPic ä½¿ç¨PIPå®è£ å¨ nonebot2
 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, è¾å¥å®è£å½ä»¤ pip install
 nonebot-plugin-RanFurryPic æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ <<<<<<< HEAD
-plugins = ["nonebot_plugin_RanFurryPic"] ======= plugins =
-["nonebot_plugin_template"] >>>>>>> 12a75b0 (v1.0) ## âï¸ éç½®
+plugins = ["nonebot_plugin_template"] ======= <<<<<<< HEAD plugins =
+["nonebot_plugin_RanFurryPic"] ======= plugins = ["nonebot_plugin_template"]
+>>>>>>> 12a75b0 (v1.0) >>>>>>> 9106e15 (first commit) ## âï¸ éç½®
 1.0çæ¬ææ éç½®é¡¹ï¼å¯å³å®å³ç¨ã ## ð ä½¿ç¨ ### æä»¤è¡¨ |
 æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:--
 --:| | æ¥åªæ¯ | ç¾¤å | å¦ | ç¾¤è | éæºæ¯å¾ | | furry | ç¾¤å |
 å¦ | ç¾¤è | éæºæ¯å¾ | | æ¯æ¯ | ç¾¤å | å¦ | ç¾¤è | éæºæ¯å¾ |
```

### Comparing `nonebot_plugin_ranfurrypic-1.0.3.3/nonebot_plugin_RanFurryPic/__init__.py` & `nonebot_plugin_ranfurrypic-1.0.3.4/nonebot_plugin_RanFurryPic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     type="application",
     # 发布必填，当前有效类型有：`library`（为其他插件编写提供功能），`application`（向机器人用户提供功能）。
 
     homepage="https://github.com/Ekac00/nonebot-plugin-RanFurryPic/",
     # 发布必填。
 
-    supported_adapters={"~onebot.v11", "~fastapi"},
+    supported_adapters={"~onebot.v11"},
     # 支持的适配器集合，其中 `~` 在此处代表前缀 `nonebot.adapters.`，其余适配器亦按此格式填写。
     # 若插件可以保证兼容所有适配器（即仅使用基本适配器功能）可不填写，否则应该列出插件支持的适配器。
 )
 
 furry = on_command("来只毛", aliases={"毛毛", "furry"}, priority=10, block=True)
 
 @furry.handle()
```

### Comparing `nonebot_plugin_ranfurrypic-1.0.3.3/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO` & `nonebot_plugin_ranfurrypic-1.0.3.4/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_RanFurryPic
-Version: 1.0.3.3
+Version: 1.0.3.4
 Summary: 基于NoneBot2进行适配的兽云随机毛图插件
 Home-page: https://github.com/Ekac00/nonebot-plugin-RanFurryPic
 Author: Ekac
 Author-email: Ekac00 <2396382559@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -68,18 +68,22 @@
 在 nonebot2 项目的插件目录下, 打开命令行, 输入安装命令
 
     pip install nonebot-plugin-RanFurryPic
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
 <<<<<<< HEAD
+    plugins = ["nonebot_plugin_template"]
+=======
+<<<<<<< HEAD
     plugins = ["nonebot_plugin_RanFurryPic"]
 =======
     plugins = ["nonebot_plugin_template"]
 >>>>>>> 12a75b0 (v1.0)
+>>>>>>> 9106e15 (first commit)
 
 </details>
 
 ## ⚙️ 配置
 
 1.0版本暂无配置项，可即安即用。
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.0.3.3
+Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.0.3.4
 Summary: åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Home-page:
 https://github.com/Ekac00/nonebot-plugin-RanFurryPic Author: Ekac Author-email:
 Ekac00 <2396382559@qq.com> License: MIT Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2
 Requires-Dist: requests Requires-Dist: nonebot-adapter-onebot
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
@@ -14,13 +14,14 @@
 æ³¨æï¼æ¬æä»¶éè¦`requests`åºåéè¯·æ±ï¼æ­¤åºå¨1.0çæ¬ä¸­æªæ·»å è³ä¾èµï¼è¯·æå¨è¿è¡å®è£ï¼
 pip install requests ä½¿ç¨ nb-cli å®è£ï¼æ¨èï¼ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot-plugin-RanFurryPic ä½¿ç¨PIPå®è£ å¨ nonebot2
 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, è¾å¥å®è£å½ä»¤ pip install
 nonebot-plugin-RanFurryPic æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ <<<<<<< HEAD
-plugins = ["nonebot_plugin_RanFurryPic"] ======= plugins =
-["nonebot_plugin_template"] >>>>>>> 12a75b0 (v1.0) ## âï¸ éç½®
+plugins = ["nonebot_plugin_template"] ======= <<<<<<< HEAD plugins =
+["nonebot_plugin_RanFurryPic"] ======= plugins = ["nonebot_plugin_template"]
+>>>>>>> 12a75b0 (v1.0) >>>>>>> 9106e15 (first commit) ## âï¸ éç½®
 1.0çæ¬ææ éç½®é¡¹ï¼å¯å³å®å³ç¨ã ## ð ä½¿ç¨ ### æä»¤è¡¨ |
 æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:--
 --:| | æ¥åªæ¯ | ç¾¤å | å¦ | ç¾¤è | éæºæ¯å¾ | | furry | ç¾¤å |
 å¦ | ç¾¤è | éæºæ¯å¾ | | æ¯æ¯ | ç¾¤å | å¦ | ç¾¤è | éæºæ¯å¾ |
```

### Comparing `nonebot_plugin_ranfurrypic-1.0.3.3/setup.py` & `nonebot_plugin_ranfurrypic-1.0.3.4/setup.py`

 * *Files identical despite different names*

