# Comparing `tmp/nonebot_plugin_ranfurrypic-1.0.1.tar.gz` & `tmp/nonebot_plugin_ranfurrypic-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ranfurrypic-1.0.1.tar", last modified: Fri May 10 15:45:35 2024, max compression
+gzip compressed data, was "nonebot_plugin_ranfurrypic-1.0.2.tar", last modified: Fri May 10 16:38:17 2024, max compression
```

## Comparing `nonebot_plugin_ranfurrypic-1.0.1.tar` & `nonebot_plugin_ranfurrypic-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 15:45:35.069488 nonebot_plugin_ranfurrypic-1.0.1/
--rw-rw-rw-   0        0        0     1082 2024-05-10 14:34:54.000000 nonebot_plugin_ranfurrypic-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     2910 2024-05-10 15:45:35.067487 nonebot_plugin_ranfurrypic-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2349 2024-05-10 13:33:04.000000 nonebot_plugin_ranfurrypic-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 15:45:35.066489 nonebot_plugin_ranfurrypic-1.0.1/nonebot_plugin_RanFurryPic.egg-info/
--rw-rw-rw-   0        0        0     2910 2024-05-10 15:45:34.000000 nonebot_plugin_ranfurrypic-1.0.1/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2024-05-10 15:45:35.000000 nonebot_plugin_ranfurrypic-1.0.1/nonebot_plugin_RanFurryPic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 15:45:34.000000 nonebot_plugin_ranfurrypic-1.0.1/nonebot_plugin_RanFurryPic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 15:45:34.000000 nonebot_plugin_ranfurrypic-1.0.1/nonebot_plugin_RanFurryPic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 15:45:35.069488 nonebot_plugin_ranfurrypic-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1090 2024-05-10 15:42:45.000000 nonebot_plugin_ranfurrypic-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 16:38:17.732718 nonebot_plugin_ranfurrypic-1.0.2/
+-rw-rw-rw-   0        0        0     1082 2024-05-10 14:34:54.000000 nonebot_plugin_ranfurrypic-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2834 2024-05-10 16:38:17.728720 nonebot_plugin_ranfurrypic-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2349 2024-05-10 13:33:04.000000 nonebot_plugin_ranfurrypic-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 16:38:17.727721 nonebot_plugin_ranfurrypic-1.0.2/nonebot_plugin_RanFurryPic.egg-info/
+-rw-rw-rw-   0        0        0     2834 2024-05-10 16:38:17.000000 nonebot_plugin_ranfurrypic-1.0.2/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2024-05-10 16:38:17.000000 nonebot_plugin_ranfurrypic-1.0.2/nonebot_plugin_RanFurryPic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 16:38:17.000000 nonebot_plugin_ranfurrypic-1.0.2/nonebot_plugin_RanFurryPic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-10 16:38:17.000000 nonebot_plugin_ranfurrypic-1.0.2/nonebot_plugin_RanFurryPic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-10 16:38:17.000000 nonebot_plugin_ranfurrypic-1.0.2/nonebot_plugin_RanFurryPic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      359 2024-05-10 16:36:26.000000 nonebot_plugin_ranfurrypic-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-10 16:38:17.732718 nonebot_plugin_ranfurrypic-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1090 2024-05-10 16:37:43.000000 nonebot_plugin_ranfurrypic-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 16:38:17.726722 nonebot_plugin_ranfurrypic-1.0.2/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-10 16:24:30.000000 nonebot_plugin_ranfurrypic-1.0.2/tests/__init__.py
```

### Comparing `nonebot_plugin_ranfurrypic-1.0.1/LICENSE` & `nonebot_plugin_ranfurrypic-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ranfurrypic-1.0.1/PKG-INFO` & `nonebot_plugin_ranfurrypic-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: nonebot-plugin-RanFurryPic
-Version: 1.0.1
+Name: nonebot_plugin_RanFurryPic
+Version: 1.0.2
 Summary: 基于NoneBot2进行适配的兽云随机毛图插件
 Home-page: https://github.com/Ekac00/nonebot-plugin-RanFurryPic
 Author: Ekac
-Author-email: 2396382559@qq.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Author-email: Ekac00 <2396382559@qq.com>
+License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: nonebot2
+Requires-Dist: requests
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
```

#### html2text {}

```diff
@@ -1,14 +1,13 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-RanFurryPic Version: 1.0.1 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.0.2 Summary:
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Home-page: https://
-github.com/Ekac00/nonebot-plugin-RanFurryPic Author: Ekac Author-email:
-2396382559@qq.com Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
-License-File: LICENSE
+github.com/Ekac00/nonebot-plugin-RanFurryPic Author: Ekac Author-email: Ekac00
+<2396382559@qq.com> License: MIT Requires-Python: >=3.8 Description-Content-
+Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-
+Dist: requests
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
   # nonebot-plugin-RanFurryPic _â¨ éæºæ¯å¾ â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ ## ð ä»ç»
 å½äºå®æ¹æä»¶å¤ªå¤æï¼åè½å¤ªæï¼çä¸æï¼ä¸å¼å®¹ï¼æåæä»¶ç»æï¼
 æ¬æä»¶ä½¿ç¨å®æ¹_A_P_Iè¿è¡ç¼åï¼æ éä»¤çï¼æ éTokenï¼å³å¯ä½¿ç¨éæºæ¯å¾åè½
 ä¹°å®¶ç§ [https://img2.imgtp.com/2024/05/10/U4xrcU7e.png]## ð¿ å®è£ ###
```

### Comparing `nonebot_plugin_ranfurrypic-1.0.1/README.md` & `nonebot_plugin_ranfurrypic-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ranfurrypic-1.0.1/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO` & `nonebot_plugin_ranfurrypic-1.0.2/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: nonebot-plugin-RanFurryPic
-Version: 1.0.1
+Name: nonebot_plugin_RanFurryPic
+Version: 1.0.2
 Summary: 基于NoneBot2进行适配的兽云随机毛图插件
 Home-page: https://github.com/Ekac00/nonebot-plugin-RanFurryPic
 Author: Ekac
-Author-email: 2396382559@qq.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Author-email: Ekac00 <2396382559@qq.com>
+License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: nonebot2
+Requires-Dist: requests
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
```

#### html2text {}

```diff
@@ -1,14 +1,13 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-RanFurryPic Version: 1.0.1 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.0.2 Summary:
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Home-page: https://
-github.com/Ekac00/nonebot-plugin-RanFurryPic Author: Ekac Author-email:
-2396382559@qq.com Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
-License-File: LICENSE
+github.com/Ekac00/nonebot-plugin-RanFurryPic Author: Ekac Author-email: Ekac00
+<2396382559@qq.com> License: MIT Requires-Python: >=3.8 Description-Content-
+Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-
+Dist: requests
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
   # nonebot-plugin-RanFurryPic _â¨ éæºæ¯å¾ â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ ## ð ä»ç»
 å½äºå®æ¹æä»¶å¤ªå¤æï¼åè½å¤ªæï¼çä¸æï¼ä¸å¼å®¹ï¼æåæä»¶ç»æï¼
 æ¬æä»¶ä½¿ç¨å®æ¹_A_P_Iè¿è¡ç¼åï¼æ éä»¤çï¼æ éTokenï¼å³å¯ä½¿ç¨éæºæ¯å¾åè½
 ä¹°å®¶ç§ [https://img2.imgtp.com/2024/05/10/U4xrcU7e.png]## ð¿ å®è£ ###
```

### Comparing `nonebot_plugin_ranfurrypic-1.0.1/setup.py` & `nonebot_plugin_ranfurrypic-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools #导入setuptools打包工具
  
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="nonebot-plugin-RanFurryPic", # 用自己的名替换其中的YOUR_USERNAME_
-    version="1.0.1",    #包版本号，便于维护版本
+    version="1.0.2",    #包版本号，便于维护版本
     author="Ekac",    #作者，可以写自己的姓名
     author_email="2396382559@qq.com",    #作者联系方式，可写自己的邮箱地址
     description="基于NoneBot2进行适配的兽云随机毛图插件",#包的简述
     long_description=long_description,    #包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/Ekac00/nonebot-plugin-RanFurryPic",    #自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
```

