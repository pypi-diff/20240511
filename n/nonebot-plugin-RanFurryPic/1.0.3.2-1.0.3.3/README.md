# Comparing `tmp/nonebot_plugin_ranfurrypic-1.0.3.2.tar.gz` & `tmp/nonebot_plugin_ranfurrypic-1.0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ranfurrypic-1.0.3.2.tar", last modified: Sat May 11 12:58:42 2024, max compression
+gzip compressed data, was "nonebot_plugin_ranfurrypic-1.0.3.3.tar", last modified: Sat May 11 13:09:17 2024, max compression
```

## Comparing `nonebot_plugin_ranfurrypic-1.0.3.2.tar` & `nonebot_plugin_ranfurrypic-1.0.3.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 12:58:42.180837 nonebot_plugin_ranfurrypic-1.0.3.2/
--rw-rw-rw-   0        0        0     1082 2024-05-10 14:34:54.000000 nonebot_plugin_ranfurrypic-1.0.3.2/LICENSE
--rw-rw-rw-   0        0        0     2889 2024-05-11 12:58:42.178839 nonebot_plugin_ranfurrypic-1.0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     2515 2024-05-11 12:16:25.000000 nonebot_plugin_ranfurrypic-1.0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 12:58:42.159856 nonebot_plugin_ranfurrypic-1.0.3.2/nonebot_plugin_RanFurryPic/
--rw-rw-rw-   0        0        0     2711 2024-05-11 12:16:25.000000 nonebot_plugin_ranfurrypic-1.0.3.2/nonebot_plugin_RanFurryPic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 12:58:42.177838 nonebot_plugin_ranfurrypic-1.0.3.2/nonebot_plugin_RanFurryPic.egg-info/
--rw-rw-rw-   0        0        0     2889 2024-05-11 12:58:42.000000 nonebot_plugin_ranfurrypic-1.0.3.2/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2024-05-11 12:58:42.000000 nonebot_plugin_ranfurrypic-1.0.3.2/nonebot_plugin_RanFurryPic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 12:58:42.000000 nonebot_plugin_ranfurrypic-1.0.3.2/nonebot_plugin_RanFurryPic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-05-11 12:58:42.000000 nonebot_plugin_ranfurrypic-1.0.3.2/nonebot_plugin_RanFurryPic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-05-11 12:58:42.000000 nonebot_plugin_ranfurrypic-1.0.3.2/nonebot_plugin_RanFurryPic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      387 2024-05-11 12:58:27.000000 nonebot_plugin_ranfurrypic-1.0.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-11 12:58:42.180837 nonebot_plugin_ranfurrypic-1.0.3.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-11 13:09:17.789526 nonebot_plugin_ranfurrypic-1.0.3.3/
+-rw-rw-rw-   0        0        0     1082 2024-05-10 14:34:54.000000 nonebot_plugin_ranfurrypic-1.0.3.3/LICENSE
+-rw-rw-rw-   0        0        0     2968 2024-05-11 13:09:17.788527 nonebot_plugin_ranfurrypic-1.0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2515 2024-05-11 12:16:25.000000 nonebot_plugin_ranfurrypic-1.0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 13:09:17.752549 nonebot_plugin_ranfurrypic-1.0.3.3/nonebot_plugin_RanFurryPic/
+-rw-rw-rw-   0        0        0     2857 2024-05-11 13:07:56.000000 nonebot_plugin_ranfurrypic-1.0.3.3/nonebot_plugin_RanFurryPic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 13:09:17.787528 nonebot_plugin_ranfurrypic-1.0.3.3/nonebot_plugin_RanFurryPic.egg-info/
+-rw-rw-rw-   0        0        0     2968 2024-05-11 13:09:17.000000 nonebot_plugin_ranfurrypic-1.0.3.3/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2024-05-11 13:09:17.000000 nonebot_plugin_ranfurrypic-1.0.3.3/nonebot_plugin_RanFurryPic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 13:09:17.000000 nonebot_plugin_ranfurrypic-1.0.3.3/nonebot_plugin_RanFurryPic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-11 13:09:17.000000 nonebot_plugin_ranfurrypic-1.0.3.3/nonebot_plugin_RanFurryPic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-05-11 13:09:17.000000 nonebot_plugin_ranfurrypic-1.0.3.3/nonebot_plugin_RanFurryPic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      387 2024-05-11 13:08:02.000000 nonebot_plugin_ranfurrypic-1.0.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-11 13:09:17.789526 nonebot_plugin_ranfurrypic-1.0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1090 2024-05-11 13:08:27.000000 nonebot_plugin_ranfurrypic-1.0.3.3/setup.py
```

### Comparing `nonebot_plugin_ranfurrypic-1.0.3.2/LICENSE` & `nonebot_plugin_ranfurrypic-1.0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ranfurrypic-1.0.3.2/PKG-INFO` & `nonebot_plugin_ranfurrypic-1.0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_RanFurryPic
-Version: 1.0.3.2
+Version: 1.0.3.3
 Summary: 基于NoneBot2进行适配的兽云随机毛图插件
+Home-page: https://github.com/Ekac00/nonebot-plugin-RanFurryPic
+Author: Ekac
 Author-email: Ekac00 <2396382559@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2
 Requires-Dist: requests
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.0.3.2
-Summary: åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Author-email:
+Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.0.3.3
+Summary: åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Home-page:
+https://github.com/Ekac00/nonebot-plugin-RanFurryPic Author: Ekac Author-email:
 Ekac00 <2396382559@qq.com> License: MIT Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2
 Requires-Dist: requests Requires-Dist: nonebot-adapter-onebot
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
   # nonebot-plugin-RanFurryPic _â¨ éæºæ¯å¾ â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ ## ð ä»ç»
```

### Comparing `nonebot_plugin_ranfurrypic-1.0.3.2/README.md` & `nonebot_plugin_ranfurrypic-1.0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ranfurrypic-1.0.3.2/nonebot_plugin_RanFurryPic/__init__.py` & `nonebot_plugin_ranfurrypic-1.0.3.3/nonebot_plugin_RanFurryPic/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from nonebot.adapters.onebot.v11 import MessageSegment
 import requests
 from nonebot.plugin import PluginMetadata
 
 __plugin_meta__ = PluginMetadata(
     name="nonebot-plugin-RanFurryPic",
     description="基于NoneBot2进行适配的兽云随机毛图插件",
+    usage="预设指令有furry、来只毛、毛毛三种指令，发送后将会调用兽云的随即图片API并返回图片及基本介绍",
 
     type="application",
     # 发布必填，当前有效类型有：`library`（为其他插件编写提供功能），`application`（向机器人用户提供功能）。
 
     homepage="https://github.com/Ekac00/nonebot-plugin-RanFurryPic/",
     # 发布必填。
```

### Comparing `nonebot_plugin_ranfurrypic-1.0.3.2/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO` & `nonebot_plugin_ranfurrypic-1.0.3.3/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_RanFurryPic
-Version: 1.0.3.2
+Version: 1.0.3.3
 Summary: 基于NoneBot2进行适配的兽云随机毛图插件
+Home-page: https://github.com/Ekac00/nonebot-plugin-RanFurryPic
+Author: Ekac
 Author-email: Ekac00 <2396382559@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2
 Requires-Dist: requests
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.0.3.2
-Summary: åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Author-email:
+Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.0.3.3
+Summary: åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Home-page:
+https://github.com/Ekac00/nonebot-plugin-RanFurryPic Author: Ekac Author-email:
 Ekac00 <2396382559@qq.com> License: MIT Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2
 Requires-Dist: requests Requires-Dist: nonebot-adapter-onebot
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
   # nonebot-plugin-RanFurryPic _â¨ éæºæ¯å¾ â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ ## ð ä»ç»
```

