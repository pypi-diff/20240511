# Comparing `tmp/nonebot_plugin_ranfurrypic-1.0.3.1.tar.gz` & `tmp/nonebot_plugin_ranfurrypic-1.0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ranfurrypic-1.0.3.1.tar", last modified: Sat May 11 12:50:18 2024, max compression
+gzip compressed data, was "nonebot_plugin_ranfurrypic-1.0.3.2.tar", last modified: Sat May 11 12:58:42 2024, max compression
```

## Comparing `nonebot_plugin_ranfurrypic-1.0.3.1.tar` & `nonebot_plugin_ranfurrypic-1.0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 12:50:18.472422 nonebot_plugin_ranfurrypic-1.0.3.1/
--rw-rw-rw-   0        0        0     1082 2024-05-10 14:34:54.000000 nonebot_plugin_ranfurrypic-1.0.3.1/LICENSE
--rw-rw-rw-   0        0        0     2850 2024-05-11 12:50:18.469424 nonebot_plugin_ranfurrypic-1.0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     2515 2024-05-11 12:16:25.000000 nonebot_plugin_ranfurrypic-1.0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 12:50:18.445443 nonebot_plugin_ranfurrypic-1.0.3.1/nonebot_plugin_RanFurryPic/
--rw-rw-rw-   0        0        0     2711 2024-05-11 12:16:25.000000 nonebot_plugin_ranfurrypic-1.0.3.1/nonebot_plugin_RanFurryPic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 12:50:18.467425 nonebot_plugin_ranfurrypic-1.0.3.1/nonebot_plugin_RanFurryPic.egg-info/
--rw-rw-rw-   0        0        0     2850 2024-05-11 12:50:18.000000 nonebot_plugin_ranfurrypic-1.0.3.1/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2024-05-11 12:50:18.000000 nonebot_plugin_ranfurrypic-1.0.3.1/nonebot_plugin_RanFurryPic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 12:50:18.000000 nonebot_plugin_ranfurrypic-1.0.3.1/nonebot_plugin_RanFurryPic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-05-11 12:50:18.000000 nonebot_plugin_ranfurrypic-1.0.3.1/nonebot_plugin_RanFurryPic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-05-11 12:50:18.000000 nonebot_plugin_ranfurrypic-1.0.3.1/nonebot_plugin_RanFurryPic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      361 2024-05-11 12:49:50.000000 nonebot_plugin_ranfurrypic-1.0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-11 12:50:18.472422 nonebot_plugin_ranfurrypic-1.0.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-11 12:58:42.180837 nonebot_plugin_ranfurrypic-1.0.3.2/
+-rw-rw-rw-   0        0        0     1082 2024-05-10 14:34:54.000000 nonebot_plugin_ranfurrypic-1.0.3.2/LICENSE
+-rw-rw-rw-   0        0        0     2889 2024-05-11 12:58:42.178839 nonebot_plugin_ranfurrypic-1.0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2515 2024-05-11 12:16:25.000000 nonebot_plugin_ranfurrypic-1.0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 12:58:42.159856 nonebot_plugin_ranfurrypic-1.0.3.2/nonebot_plugin_RanFurryPic/
+-rw-rw-rw-   0        0        0     2711 2024-05-11 12:16:25.000000 nonebot_plugin_ranfurrypic-1.0.3.2/nonebot_plugin_RanFurryPic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 12:58:42.177838 nonebot_plugin_ranfurrypic-1.0.3.2/nonebot_plugin_RanFurryPic.egg-info/
+-rw-rw-rw-   0        0        0     2889 2024-05-11 12:58:42.000000 nonebot_plugin_ranfurrypic-1.0.3.2/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-05-11 12:58:42.000000 nonebot_plugin_ranfurrypic-1.0.3.2/nonebot_plugin_RanFurryPic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 12:58:42.000000 nonebot_plugin_ranfurrypic-1.0.3.2/nonebot_plugin_RanFurryPic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-11 12:58:42.000000 nonebot_plugin_ranfurrypic-1.0.3.2/nonebot_plugin_RanFurryPic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-05-11 12:58:42.000000 nonebot_plugin_ranfurrypic-1.0.3.2/nonebot_plugin_RanFurryPic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      387 2024-05-11 12:58:27.000000 nonebot_plugin_ranfurrypic-1.0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-11 12:58:42.180837 nonebot_plugin_ranfurrypic-1.0.3.2/setup.cfg
```

### Comparing `nonebot_plugin_ranfurrypic-1.0.3.1/LICENSE` & `nonebot_plugin_ranfurrypic-1.0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ranfurrypic-1.0.3.1/PKG-INFO` & `nonebot_plugin_ranfurrypic-1.0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_RanFurryPic
-Version: 1.0.3.1
+Version: 1.0.3.2
 Summary: 基于NoneBot2进行适配的兽云随机毛图插件
 Author-email: Ekac00 <2396382559@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2
 Requires-Dist: requests
+Requires-Dist: nonebot-adapter-onebot
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.0.3.1
+Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.0.3.2
 Summary: åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Author-email:
 Ekac00 <2396382559@qq.com> License: MIT Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2
-Requires-Dist: requests
+Requires-Dist: requests Requires-Dist: nonebot-adapter-onebot
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
   # nonebot-plugin-RanFurryPic _â¨ éæºæ¯å¾ â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ ## ð ä»ç»
 å½äºå®æ¹æä»¶å¤ªå¤æï¼åè½å¤ªæï¼çä¸æï¼ä¸å¼å®¹ï¼æåæä»¶ç»æï¼
 æ¬æä»¶ä½¿ç¨å®æ¹_A_P_Iè¿è¡ç¼åï¼æ éä»¤çï¼æ éTokenï¼å³å¯ä½¿ç¨éæºæ¯å¾åè½
 ä¹°å®¶ç§ [https://img2.imgtp.com/2024/05/10/U4xrcU7e.png]## ð¿ å®è£ ###
```

### Comparing `nonebot_plugin_ranfurrypic-1.0.3.1/README.md` & `nonebot_plugin_ranfurrypic-1.0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ranfurrypic-1.0.3.1/nonebot_plugin_RanFurryPic/__init__.py` & `nonebot_plugin_ranfurrypic-1.0.3.2/nonebot_plugin_RanFurryPic/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ranfurrypic-1.0.3.1/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO` & `nonebot_plugin_ranfurrypic-1.0.3.2/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_RanFurryPic
-Version: 1.0.3.1
+Version: 1.0.3.2
 Summary: 基于NoneBot2进行适配的兽云随机毛图插件
 Author-email: Ekac00 <2396382559@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2
 Requires-Dist: requests
+Requires-Dist: nonebot-adapter-onebot
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.0.3.1
+Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.0.3.2
 Summary: åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Author-email:
 Ekac00 <2396382559@qq.com> License: MIT Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2
-Requires-Dist: requests
+Requires-Dist: requests Requires-Dist: nonebot-adapter-onebot
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
   # nonebot-plugin-RanFurryPic _â¨ éæºæ¯å¾ â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ ## ð ä»ç»
 å½äºå®æ¹æä»¶å¤ªå¤æï¼åè½å¤ªæï¼çä¸æï¼ä¸å¼å®¹ï¼æåæä»¶ç»æï¼
 æ¬æä»¶ä½¿ç¨å®æ¹_A_P_Iè¿è¡ç¼åï¼æ éä»¤çï¼æ éTokenï¼å³å¯ä½¿ç¨éæºæ¯å¾åè½
 ä¹°å®¶ç§ [https://img2.imgtp.com/2024/05/10/U4xrcU7e.png]## ð¿ å®è£ ###
```

