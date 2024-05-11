# Comparing `tmp/nonebot_plugin_ranfurrypic-1.0.3.tar.gz` & `tmp/nonebot_plugin_ranfurrypic-1.0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ranfurrypic-1.0.3.tar", last modified: Fri May 10 23:31:12 2024, max compression
+gzip compressed data, was "nonebot_plugin_ranfurrypic-1.0.3.1.tar", last modified: Sat May 11 12:50:18 2024, max compression
```

## Comparing `nonebot_plugin_ranfurrypic-1.0.3.tar` & `nonebot_plugin_ranfurrypic-1.0.3.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 23:31:12.258126 nonebot_plugin_ranfurrypic-1.0.3/
--rw-rw-rw-   0        0        0     1082 2024-05-10 14:34:54.000000 nonebot_plugin_ranfurrypic-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     2834 2024-05-10 23:31:12.257127 nonebot_plugin_ranfurrypic-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2349 2024-05-10 13:33:04.000000 nonebot_plugin_ranfurrypic-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 23:31:12.255128 nonebot_plugin_ranfurrypic-1.0.3/nonebot_plugin_RanFurryPic.egg-info/
--rw-rw-rw-   0        0        0     2834 2024-05-10 23:31:12.000000 nonebot_plugin_ranfurrypic-1.0.3/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2024-05-10 23:31:12.000000 nonebot_plugin_ranfurrypic-1.0.3/nonebot_plugin_RanFurryPic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 23:31:12.000000 nonebot_plugin_ranfurrypic-1.0.3/nonebot_plugin_RanFurryPic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-05-10 23:31:12.000000 nonebot_plugin_ranfurrypic-1.0.3/nonebot_plugin_RanFurryPic.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 23:31:12.000000 nonebot_plugin_ranfurrypic-1.0.3/nonebot_plugin_RanFurryPic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      359 2024-05-10 23:30:56.000000 nonebot_plugin_ranfurrypic-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-10 23:31:12.258126 nonebot_plugin_ranfurrypic-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1090 2024-05-10 23:30:54.000000 nonebot_plugin_ranfurrypic-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 12:50:18.472422 nonebot_plugin_ranfurrypic-1.0.3.1/
+-rw-rw-rw-   0        0        0     1082 2024-05-10 14:34:54.000000 nonebot_plugin_ranfurrypic-1.0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     2850 2024-05-11 12:50:18.469424 nonebot_plugin_ranfurrypic-1.0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2515 2024-05-11 12:16:25.000000 nonebot_plugin_ranfurrypic-1.0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 12:50:18.445443 nonebot_plugin_ranfurrypic-1.0.3.1/nonebot_plugin_RanFurryPic/
+-rw-rw-rw-   0        0        0     2711 2024-05-11 12:16:25.000000 nonebot_plugin_ranfurrypic-1.0.3.1/nonebot_plugin_RanFurryPic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 12:50:18.467425 nonebot_plugin_ranfurrypic-1.0.3.1/nonebot_plugin_RanFurryPic.egg-info/
+-rw-rw-rw-   0        0        0     2850 2024-05-11 12:50:18.000000 nonebot_plugin_ranfurrypic-1.0.3.1/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-05-11 12:50:18.000000 nonebot_plugin_ranfurrypic-1.0.3.1/nonebot_plugin_RanFurryPic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 12:50:18.000000 nonebot_plugin_ranfurrypic-1.0.3.1/nonebot_plugin_RanFurryPic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-11 12:50:18.000000 nonebot_plugin_ranfurrypic-1.0.3.1/nonebot_plugin_RanFurryPic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-05-11 12:50:18.000000 nonebot_plugin_ranfurrypic-1.0.3.1/nonebot_plugin_RanFurryPic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      361 2024-05-11 12:49:50.000000 nonebot_plugin_ranfurrypic-1.0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-11 12:50:18.472422 nonebot_plugin_ranfurrypic-1.0.3.1/setup.cfg
```

### Comparing `nonebot_plugin_ranfurrypic-1.0.3/LICENSE` & `nonebot_plugin_ranfurrypic-1.0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ranfurrypic-1.0.3/PKG-INFO` & `nonebot_plugin_ranfurrypic-1.0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_RanFurryPic
-Version: 1.0.3
+Version: 1.0.3.1
 Summary: 基于NoneBot2进行适配的兽云随机毛图插件
-Home-page: https://github.com/Ekac00/nonebot-plugin-RanFurryPic
-Author: Ekac
 Author-email: Ekac00 <2396382559@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2
 Requires-Dist: requests
@@ -66,15 +64,19 @@
 <summary>使用PIP安装</summary>
 在 nonebot2 项目的插件目录下, 打开命令行, 输入安装命令
 
     pip install nonebot-plugin-RanFurryPic
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
+<<<<<<< HEAD
+    plugins = ["nonebot_plugin_RanFurryPic"]
+=======
     plugins = ["nonebot_plugin_template"]
+>>>>>>> 12a75b0 (v1.0)
 
 </details>
 
 ## ⚙️ 配置
 
 1.0版本暂无配置项，可即安即用。
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.0.3 Summary:
-åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Home-page: https://
-github.com/Ekac00/nonebot-plugin-RanFurryPic Author: Ekac Author-email: Ekac00
-<2396382559@qq.com> License: MIT Requires-Python: >=3.8 Description-Content-
-Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-
-Dist: requests
+Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.0.3.1
+Summary: åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Author-email:
+Ekac00 <2396382559@qq.com> License: MIT Requires-Python: >=3.8 Description-
+Content-Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2
+Requires-Dist: requests
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
   # nonebot-plugin-RanFurryPic _â¨ éæºæ¯å¾ â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ ## ð ä»ç»
 å½äºå®æ¹æä»¶å¤ªå¤æï¼åè½å¤ªæï¼çä¸æï¼ä¸å¼å®¹ï¼æåæä»¶ç»æï¼
 æ¬æä»¶ä½¿ç¨å®æ¹_A_P_Iè¿è¡ç¼åï¼æ éä»¤çï¼æ éTokenï¼å³å¯ä½¿ç¨éæºæ¯å¾åè½
 ä¹°å®¶ç§ [https://img2.imgtp.com/2024/05/10/U4xrcU7e.png]## ð¿ å®è£ ###
 æ³¨æï¼æ¬æä»¶éè¦`requests`åºåéè¯·æ±ï¼æ­¤åºå¨1.0çæ¬ä¸­æªæ·»å è³ä¾èµï¼è¯·æå¨è¿è¡å®è£ï¼
 pip install requests ä½¿ç¨ nb-cli å®è£ï¼æ¨èï¼ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot-plugin-RanFurryPic ä½¿ç¨PIPå®è£ å¨ nonebot2
 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, è¾å¥å®è£å½ä»¤ pip install
 nonebot-plugin-RanFurryPic æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
-`pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
-["nonebot_plugin_template"] ## âï¸ éç½®
+`pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ <<<<<<< HEAD
+plugins = ["nonebot_plugin_RanFurryPic"] ======= plugins =
+["nonebot_plugin_template"] >>>>>>> 12a75b0 (v1.0) ## âï¸ éç½®
 1.0çæ¬ææ éç½®é¡¹ï¼å¯å³å®å³ç¨ã ## ð ä½¿ç¨ ### æä»¤è¡¨ |
 æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:--
 --:| | æ¥åªæ¯ | ç¾¤å | å¦ | ç¾¤è | éæºæ¯å¾ | | furry | ç¾¤å |
 å¦ | ç¾¤è | éæºæ¯å¾ | | æ¯æ¯ | ç¾¤å | å¦ | ç¾¤è | éæºæ¯å¾ |
```

### Comparing `nonebot_plugin_ranfurrypic-1.0.3/README.md` & `nonebot_plugin_ranfurrypic-1.0.3.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,73 +1,77 @@
-<div align="center">
-  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
-  <br>
-  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
-</div>
-
-<div align="center">
-
-# nonebot-plugin-RanFurryPic
-
-_✨ 随机毛图 ✨_
-
-
-<a href="./LICENSE">
-    <img src="https://img.shields.io/github/license/owner/nonebot-plugin-template.svg" alt="license">
-</a>
-<a href="https://pypi.python.org/pypi/nonebot-plugin-template">
-    <img src="https://img.shields.io/pypi/v/nonebot-plugin-template.svg" alt="pypi">
-</a>
-<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
-
-</div>
-
-基于NoneBot2进行适配的兽云随机毛图插件
-
-## 📖 介绍
-
-兽云官方插件太复杂？功能太杂？看不懂？不兼容？损坏文件结构？
-本插件使用官方<a href="https://console-docs.apipost.cn/preview/6bf01cfebd3e5f96/c4e20a5d1a5db86c?target_id=83fb4f89-221c-4196-bb85-4abf73af73af">API</a>进行编写，无需令牌，无需Token，即可使用随机毛图功能
-
-<details>
-<summary>买家秀</summary>
-
-<img src="https://img2.imgtp.com/2024/05/10/U4xrcU7e.png">
-
-</details>
-
-## 💿 安装
-
-### 注意！本插件需要`requests`库发送请求，此库在1.0版本中未添加至依赖，请手动进行安装！
-    pip install requests
-
-<details open>
-<summary>使用 nb-cli 安装（推荐）</summary>
-在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
-
-    nb plugin install nonebot-plugin-RanFurryPic
-
-</details>
-
-<details>
-<summary>使用PIP安装</summary>
-在 nonebot2 项目的插件目录下, 打开命令行, 输入安装命令
-
-    pip install nonebot-plugin-RanFurryPic
-
-打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
-
-    plugins = ["nonebot_plugin_template"]
-
-</details>
-
-## ⚙️ 配置
-
-1.0版本暂无配置项，可即安即用。
-
-## 🎉 使用
-### 指令表
-| 指令 | 权限 | 需要@ | 范围 | 说明 |
-|:-----:|:----:|:----:|:----:|:----:|
-| 来只毛 | 群员 | 否 | 群聊 | 随机毛图 |
-| furry | 群员 | 否 | 群聊 | 随机毛图 |
-| 毛毛 | 群员 | 否 | 群聊 | 随机毛图 |
+<div align="center">
+  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
+  <br>
+  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
+</div>
+
+<div align="center">
+
+# nonebot-plugin-RanFurryPic
+
+_✨ 随机毛图 ✨_
+
+
+<a href="./LICENSE">
+    <img src="https://img.shields.io/github/license/owner/nonebot-plugin-template.svg" alt="license">
+</a>
+<a href="https://pypi.python.org/pypi/nonebot-plugin-template">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-template.svg" alt="pypi">
+</a>
+<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+
+</div>
+
+基于NoneBot2进行适配的兽云随机毛图插件
+
+## 📖 介绍
+
+兽云官方插件太复杂？功能太杂？看不懂？不兼容？损坏文件结构？
+本插件使用官方<a href="https://console-docs.apipost.cn/preview/6bf01cfebd3e5f96/c4e20a5d1a5db86c?target_id=83fb4f89-221c-4196-bb85-4abf73af73af">API</a>进行编写，无需令牌，无需Token，即可使用随机毛图功能
+
+<details>
+<summary>买家秀</summary>
+
+<img src="https://img2.imgtp.com/2024/05/10/U4xrcU7e.png">
+
+</details>
+
+## 💿 安装
+
+### 注意！本插件需要`requests`库发送请求，此库在1.0版本中未添加至依赖，请手动进行安装！
+    pip install requests
+
+<details open>
+<summary>使用 nb-cli 安装（推荐）</summary>
+在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
+
+    nb plugin install nonebot-plugin-RanFurryPic
+
+</details>
+
+<details>
+<summary>使用PIP安装</summary>
+在 nonebot2 项目的插件目录下, 打开命令行, 输入安装命令
+
+    pip install nonebot-plugin-RanFurryPic
+
+打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
+
+<<<<<<< HEAD
+    plugins = ["nonebot_plugin_RanFurryPic"]
+=======
+    plugins = ["nonebot_plugin_template"]
+>>>>>>> 12a75b0 (v1.0)
+
+</details>
+
+## ⚙️ 配置
+
+1.0版本暂无配置项，可即安即用。
+
+## 🎉 使用
+### 指令表
+| 指令 | 权限 | 需要@ | 范围 | 说明 |
+|:-----:|:----:|:----:|:----:|:----:|
+| 来只毛 | 群员 | 否 | 群聊 | 随机毛图 |
+| furry | 群员 | 否 | 群聊 | 随机毛图 |
+| 毛毛 | 群员 | 否 | 群聊 | 随机毛图 |
```

#### html2text {}

```diff
@@ -7,13 +7,14 @@
 ä¹°å®¶ç§ [https://img2.imgtp.com/2024/05/10/U4xrcU7e.png]## ð¿ å®è£ ###
 æ³¨æï¼æ¬æä»¶éè¦`requests`åºåéè¯·æ±ï¼æ­¤åºå¨1.0çæ¬ä¸­æªæ·»å è³ä¾èµï¼è¯·æå¨è¿è¡å®è£ï¼
 pip install requests ä½¿ç¨ nb-cli å®è£ï¼æ¨èï¼ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot-plugin-RanFurryPic ä½¿ç¨PIPå®è£ å¨ nonebot2
 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, è¾å¥å®è£å½ä»¤ pip install
 nonebot-plugin-RanFurryPic æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
-`pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
-["nonebot_plugin_template"] ## âï¸ éç½®
+`pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ <<<<<<< HEAD
+plugins = ["nonebot_plugin_RanFurryPic"] ======= plugins =
+["nonebot_plugin_template"] >>>>>>> 12a75b0 (v1.0) ## âï¸ éç½®
 1.0çæ¬ææ éç½®é¡¹ï¼å¯å³å®å³ç¨ã ## ð ä½¿ç¨ ### æä»¤è¡¨ |
 æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:--
 --:| | æ¥åªæ¯ | ç¾¤å | å¦ | ç¾¤è | éæºæ¯å¾ | | furry | ç¾¤å |
 å¦ | ç¾¤è | éæºæ¯å¾ | | æ¯æ¯ | ç¾¤å | å¦ | ç¾¤è | éæºæ¯å¾ |
```

### Comparing `nonebot_plugin_ranfurrypic-1.0.3/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO` & `nonebot_plugin_ranfurrypic-1.0.3.1/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_RanFurryPic
-Version: 1.0.3
+Version: 1.0.3.1
 Summary: 基于NoneBot2进行适配的兽云随机毛图插件
-Home-page: https://github.com/Ekac00/nonebot-plugin-RanFurryPic
-Author: Ekac
 Author-email: Ekac00 <2396382559@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2
 Requires-Dist: requests
@@ -66,15 +64,19 @@
 <summary>使用PIP安装</summary>
 在 nonebot2 项目的插件目录下, 打开命令行, 输入安装命令
 
     pip install nonebot-plugin-RanFurryPic
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
+<<<<<<< HEAD
+    plugins = ["nonebot_plugin_RanFurryPic"]
+=======
     plugins = ["nonebot_plugin_template"]
+>>>>>>> 12a75b0 (v1.0)
 
 </details>
 
 ## ⚙️ 配置
 
 1.0版本暂无配置项，可即安即用。
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.0.3 Summary:
-åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Home-page: https://
-github.com/Ekac00/nonebot-plugin-RanFurryPic Author: Ekac Author-email: Ekac00
-<2396382559@qq.com> License: MIT Requires-Python: >=3.8 Description-Content-
-Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-
-Dist: requests
+Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.0.3.1
+Summary: åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Author-email:
+Ekac00 <2396382559@qq.com> License: MIT Requires-Python: >=3.8 Description-
+Content-Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2
+Requires-Dist: requests
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
   # nonebot-plugin-RanFurryPic _â¨ éæºæ¯å¾ â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ ## ð ä»ç»
 å½äºå®æ¹æä»¶å¤ªå¤æï¼åè½å¤ªæï¼çä¸æï¼ä¸å¼å®¹ï¼æåæä»¶ç»æï¼
 æ¬æä»¶ä½¿ç¨å®æ¹_A_P_Iè¿è¡ç¼åï¼æ éä»¤çï¼æ éTokenï¼å³å¯ä½¿ç¨éæºæ¯å¾åè½
 ä¹°å®¶ç§ [https://img2.imgtp.com/2024/05/10/U4xrcU7e.png]## ð¿ å®è£ ###
 æ³¨æï¼æ¬æä»¶éè¦`requests`åºåéè¯·æ±ï¼æ­¤åºå¨1.0çæ¬ä¸­æªæ·»å è³ä¾èµï¼è¯·æå¨è¿è¡å®è£ï¼
 pip install requests ä½¿ç¨ nb-cli å®è£ï¼æ¨èï¼ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot-plugin-RanFurryPic ä½¿ç¨PIPå®è£ å¨ nonebot2
 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, è¾å¥å®è£å½ä»¤ pip install
 nonebot-plugin-RanFurryPic æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
-`pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
-["nonebot_plugin_template"] ## âï¸ éç½®
+`pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ <<<<<<< HEAD
+plugins = ["nonebot_plugin_RanFurryPic"] ======= plugins =
+["nonebot_plugin_template"] >>>>>>> 12a75b0 (v1.0) ## âï¸ éç½®
 1.0çæ¬ææ éç½®é¡¹ï¼å¯å³å®å³ç¨ã ## ð ä½¿ç¨ ### æä»¤è¡¨ |
 æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:--
 --:| | æ¥åªæ¯ | ç¾¤å | å¦ | ç¾¤è | éæºæ¯å¾ | | furry | ç¾¤å |
 å¦ | ç¾¤è | éæºæ¯å¾ | | æ¯æ¯ | ç¾¤å | å¦ | ç¾¤è | éæºæ¯å¾ |
```

