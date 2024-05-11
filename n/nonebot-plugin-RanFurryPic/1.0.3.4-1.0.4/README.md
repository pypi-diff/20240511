# Comparing `tmp/nonebot_plugin_ranfurrypic-1.0.3.4.tar.gz` & `tmp/nonebot_plugin_ranfurrypic-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ranfurrypic-1.0.3.4.tar", last modified: Sat May 11 13:37:14 2024, max compression
+gzip compressed data, was "nonebot_plugin_ranfurrypic-1.0.4.tar", last modified: Sat May 11 13:49:46 2024, max compression
```

## Comparing `nonebot_plugin_ranfurrypic-1.0.3.4.tar` & `nonebot_plugin_ranfurrypic-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 13:37:14.016548 nonebot_plugin_ranfurrypic-1.0.3.4/
--rw-rw-rw-   0        0        0     1082 2024-05-10 14:34:54.000000 nonebot_plugin_ranfurrypic-1.0.3.4/LICENSE
--rw-rw-rw-   0        0        0     3066 2024-05-11 13:37:14.013551 nonebot_plugin_ranfurrypic-1.0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     2613 2024-05-11 13:13:22.000000 nonebot_plugin_ranfurrypic-1.0.3.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 13:37:13.999561 nonebot_plugin_ranfurrypic-1.0.3.4/nonebot_plugin_RanFurryPic/
--rw-rw-rw-   0        0        0     2845 2024-05-11 13:35:33.000000 nonebot_plugin_ranfurrypic-1.0.3.4/nonebot_plugin_RanFurryPic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 13:37:14.012551 nonebot_plugin_ranfurrypic-1.0.3.4/nonebot_plugin_RanFurryPic.egg-info/
--rw-rw-rw-   0        0        0     3066 2024-05-11 13:37:13.000000 nonebot_plugin_ranfurrypic-1.0.3.4/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-05-11 13:37:13.000000 nonebot_plugin_ranfurrypic-1.0.3.4/nonebot_plugin_RanFurryPic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 13:37:13.000000 nonebot_plugin_ranfurrypic-1.0.3.4/nonebot_plugin_RanFurryPic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-05-11 13:37:13.000000 nonebot_plugin_ranfurrypic-1.0.3.4/nonebot_plugin_RanFurryPic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-05-11 13:37:13.000000 nonebot_plugin_ranfurrypic-1.0.3.4/nonebot_plugin_RanFurryPic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      387 2024-05-11 13:36:38.000000 nonebot_plugin_ranfurrypic-1.0.3.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-11 13:37:14.016548 nonebot_plugin_ranfurrypic-1.0.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1090 2024-05-11 13:08:27.000000 nonebot_plugin_ranfurrypic-1.0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 13:49:46.381610 nonebot_plugin_ranfurrypic-1.0.4/
+-rw-rw-rw-   0        0        0     1082 2024-05-10 14:34:54.000000 nonebot_plugin_ranfurrypic-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     3062 2024-05-11 13:49:46.380611 nonebot_plugin_ranfurrypic-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2613 2024-05-11 13:13:22.000000 nonebot_plugin_ranfurrypic-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 13:49:46.366624 nonebot_plugin_ranfurrypic-1.0.4/nonebot_plugin_RanFurryPic/
+-rw-rw-rw-   0        0        0     2845 2024-05-11 13:35:33.000000 nonebot_plugin_ranfurrypic-1.0.4/nonebot_plugin_RanFurryPic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 13:49:46.379612 nonebot_plugin_ranfurrypic-1.0.4/nonebot_plugin_RanFurryPic.egg-info/
+-rw-rw-rw-   0        0        0     3062 2024-05-11 13:49:46.000000 nonebot_plugin_ranfurrypic-1.0.4/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2024-05-11 13:49:46.000000 nonebot_plugin_ranfurrypic-1.0.4/nonebot_plugin_RanFurryPic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 13:49:46.000000 nonebot_plugin_ranfurrypic-1.0.4/nonebot_plugin_RanFurryPic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-11 13:49:46.000000 nonebot_plugin_ranfurrypic-1.0.4/nonebot_plugin_RanFurryPic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-05-11 13:49:46.000000 nonebot_plugin_ranfurrypic-1.0.4/nonebot_plugin_RanFurryPic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      383 2024-05-11 13:48:53.000000 nonebot_plugin_ranfurrypic-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-11 13:49:46.381610 nonebot_plugin_ranfurrypic-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1090 2024-05-11 13:08:27.000000 nonebot_plugin_ranfurrypic-1.0.4/setup.py
```

### Comparing `nonebot_plugin_ranfurrypic-1.0.3.4/LICENSE` & `nonebot_plugin_ranfurrypic-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ranfurrypic-1.0.3.4/PKG-INFO` & `nonebot_plugin_ranfurrypic-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_RanFurryPic
-Version: 1.0.3.4
+Version: 1.0.4
 Summary: 基于NoneBot2进行适配的兽云随机毛图插件
 Home-page: https://github.com/Ekac00/nonebot-plugin-RanFurryPic
 Author: Ekac
-Author-email: Ekac00 <2396382559@qq.com>
+Author-email: Ekac <2396382559@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2
 Requires-Dist: requests
 Requires-Dist: nonebot-adapter-onebot
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.0.3.4
-Summary: åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Home-page:
-https://github.com/Ekac00/nonebot-plugin-RanFurryPic Author: Ekac Author-email:
-Ekac00 <2396382559@qq.com> License: MIT Requires-Python: >=3.8 Description-
-Content-Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2
-Requires-Dist: requests Requires-Dist: nonebot-adapter-onebot
+Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.0.4 Summary:
+åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Home-page: https://
+github.com/Ekac00/nonebot-plugin-RanFurryPic Author: Ekac Author-email: Ekac
+<2396382559@qq.com> License: MIT Requires-Python: >=3.8 Description-Content-
+Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-
+Dist: requests Requires-Dist: nonebot-adapter-onebot
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
   # nonebot-plugin-RanFurryPic _â¨ éæºæ¯å¾ â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ ## ð ä»ç»
 å½äºå®æ¹æä»¶å¤ªå¤æï¼åè½å¤ªæï¼çä¸æï¼ä¸å¼å®¹ï¼æåæä»¶ç»æï¼
 æ¬æä»¶ä½¿ç¨å®æ¹_A_P_Iè¿è¡ç¼åï¼æ éä»¤çï¼æ éTokenï¼å³å¯ä½¿ç¨éæºæ¯å¾åè½
 ä¹°å®¶ç§ [https://img2.imgtp.com/2024/05/10/U4xrcU7e.png]## ð¿ å®è£ ###
```

### Comparing `nonebot_plugin_ranfurrypic-1.0.3.4/README.md` & `nonebot_plugin_ranfurrypic-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ranfurrypic-1.0.3.4/nonebot_plugin_RanFurryPic/__init__.py` & `nonebot_plugin_ranfurrypic-1.0.4/nonebot_plugin_RanFurryPic/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ranfurrypic-1.0.3.4/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO` & `nonebot_plugin_ranfurrypic-1.0.4/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_RanFurryPic
-Version: 1.0.3.4
+Version: 1.0.4
 Summary: 基于NoneBot2进行适配的兽云随机毛图插件
 Home-page: https://github.com/Ekac00/nonebot-plugin-RanFurryPic
 Author: Ekac
-Author-email: Ekac00 <2396382559@qq.com>
+Author-email: Ekac <2396382559@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2
 Requires-Dist: requests
 Requires-Dist: nonebot-adapter-onebot
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.0.3.4
-Summary: åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Home-page:
-https://github.com/Ekac00/nonebot-plugin-RanFurryPic Author: Ekac Author-email:
-Ekac00 <2396382559@qq.com> License: MIT Requires-Python: >=3.8 Description-
-Content-Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2
-Requires-Dist: requests Requires-Dist: nonebot-adapter-onebot
+Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.0.4 Summary:
+åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Home-page: https://
+github.com/Ekac00/nonebot-plugin-RanFurryPic Author: Ekac Author-email: Ekac
+<2396382559@qq.com> License: MIT Requires-Python: >=3.8 Description-Content-
+Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-
+Dist: requests Requires-Dist: nonebot-adapter-onebot
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
   # nonebot-plugin-RanFurryPic _â¨ éæºæ¯å¾ â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ ## ð ä»ç»
 å½äºå®æ¹æä»¶å¤ªå¤æï¼åè½å¤ªæï¼çä¸æï¼ä¸å¼å®¹ï¼æåæä»¶ç»æï¼
 æ¬æä»¶ä½¿ç¨å®æ¹_A_P_Iè¿è¡ç¼åï¼æ éä»¤çï¼æ éTokenï¼å³å¯ä½¿ç¨éæºæ¯å¾åè½
 ä¹°å®¶ç§ [https://img2.imgtp.com/2024/05/10/U4xrcU7e.png]## ð¿ å®è£ ###
```

### Comparing `nonebot_plugin_ranfurrypic-1.0.3.4/setup.py` & `nonebot_plugin_ranfurrypic-1.0.4/setup.py`

 * *Files identical despite different names*

