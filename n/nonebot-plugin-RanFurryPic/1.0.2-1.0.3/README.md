# Comparing `tmp/nonebot_plugin_ranfurrypic-1.0.2.tar.gz` & `tmp/nonebot_plugin_ranfurrypic-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ranfurrypic-1.0.2.tar", last modified: Fri May 10 16:38:17 2024, max compression
+gzip compressed data, was "nonebot_plugin_ranfurrypic-1.0.3.tar", last modified: Fri May 10 23:31:12 2024, max compression
```

## Comparing `nonebot_plugin_ranfurrypic-1.0.2.tar` & `nonebot_plugin_ranfurrypic-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 16:38:17.732718 nonebot_plugin_ranfurrypic-1.0.2/
--rw-rw-rw-   0        0        0     1082 2024-05-10 14:34:54.000000 nonebot_plugin_ranfurrypic-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     2834 2024-05-10 16:38:17.728720 nonebot_plugin_ranfurrypic-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2349 2024-05-10 13:33:04.000000 nonebot_plugin_ranfurrypic-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 16:38:17.727721 nonebot_plugin_ranfurrypic-1.0.2/nonebot_plugin_RanFurryPic.egg-info/
--rw-rw-rw-   0        0        0     2834 2024-05-10 16:38:17.000000 nonebot_plugin_ranfurrypic-1.0.2/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2024-05-10 16:38:17.000000 nonebot_plugin_ranfurrypic-1.0.2/nonebot_plugin_RanFurryPic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 16:38:17.000000 nonebot_plugin_ranfurrypic-1.0.2/nonebot_plugin_RanFurryPic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-05-10 16:38:17.000000 nonebot_plugin_ranfurrypic-1.0.2/nonebot_plugin_RanFurryPic.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-10 16:38:17.000000 nonebot_plugin_ranfurrypic-1.0.2/nonebot_plugin_RanFurryPic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      359 2024-05-10 16:36:26.000000 nonebot_plugin_ranfurrypic-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-10 16:38:17.732718 nonebot_plugin_ranfurrypic-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1090 2024-05-10 16:37:43.000000 nonebot_plugin_ranfurrypic-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-10 16:38:17.726722 nonebot_plugin_ranfurrypic-1.0.2/tests/
--rw-rw-rw-   0        0        0        0 2024-05-10 16:24:30.000000 nonebot_plugin_ranfurrypic-1.0.2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 23:31:12.258126 nonebot_plugin_ranfurrypic-1.0.3/
+-rw-rw-rw-   0        0        0     1082 2024-05-10 14:34:54.000000 nonebot_plugin_ranfurrypic-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2834 2024-05-10 23:31:12.257127 nonebot_plugin_ranfurrypic-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2349 2024-05-10 13:33:04.000000 nonebot_plugin_ranfurrypic-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 23:31:12.255128 nonebot_plugin_ranfurrypic-1.0.3/nonebot_plugin_RanFurryPic.egg-info/
+-rw-rw-rw-   0        0        0     2834 2024-05-10 23:31:12.000000 nonebot_plugin_ranfurrypic-1.0.3/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2024-05-10 23:31:12.000000 nonebot_plugin_ranfurrypic-1.0.3/nonebot_plugin_RanFurryPic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 23:31:12.000000 nonebot_plugin_ranfurrypic-1.0.3/nonebot_plugin_RanFurryPic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-10 23:31:12.000000 nonebot_plugin_ranfurrypic-1.0.3/nonebot_plugin_RanFurryPic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 23:31:12.000000 nonebot_plugin_ranfurrypic-1.0.3/nonebot_plugin_RanFurryPic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      359 2024-05-10 23:30:56.000000 nonebot_plugin_ranfurrypic-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-10 23:31:12.258126 nonebot_plugin_ranfurrypic-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1090 2024-05-10 23:30:54.000000 nonebot_plugin_ranfurrypic-1.0.3/setup.py
```

### Comparing `nonebot_plugin_ranfurrypic-1.0.2/LICENSE` & `nonebot_plugin_ranfurrypic-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ranfurrypic-1.0.2/PKG-INFO` & `nonebot_plugin_ranfurrypic-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_RanFurryPic
-Version: 1.0.2
+Version: 1.0.3
 Summary: 基于NoneBot2进行适配的兽云随机毛图插件
 Home-page: https://github.com/Ekac00/nonebot-plugin-RanFurryPic
 Author: Ekac
 Author-email: Ekac00 <2396382559@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.0.2 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.0.3 Summary:
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Home-page: https://
 github.com/Ekac00/nonebot-plugin-RanFurryPic Author: Ekac Author-email: Ekac00
 <2396382559@qq.com> License: MIT Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-
 Dist: requests
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
```

### Comparing `nonebot_plugin_ranfurrypic-1.0.2/README.md` & `nonebot_plugin_ranfurrypic-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ranfurrypic-1.0.2/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO` & `nonebot_plugin_ranfurrypic-1.0.3/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_RanFurryPic
-Version: 1.0.2
+Version: 1.0.3
 Summary: 基于NoneBot2进行适配的兽云随机毛图插件
 Home-page: https://github.com/Ekac00/nonebot-plugin-RanFurryPic
 Author: Ekac
 Author-email: Ekac00 <2396382559@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.0.2 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.0.3 Summary:
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Home-page: https://
 github.com/Ekac00/nonebot-plugin-RanFurryPic Author: Ekac Author-email: Ekac00
 <2396382559@qq.com> License: MIT Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-
 Dist: requests
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
```

### Comparing `nonebot_plugin_ranfurrypic-1.0.2/setup.py` & `nonebot_plugin_ranfurrypic-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools #导入setuptools打包工具
  
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="nonebot-plugin-RanFurryPic", # 用自己的名替换其中的YOUR_USERNAME_
-    version="1.0.2",    #包版本号，便于维护版本
+    version="1.0.3",    #包版本号，便于维护版本
     author="Ekac",    #作者，可以写自己的姓名
     author_email="2396382559@qq.com",    #作者联系方式，可写自己的邮箱地址
     description="基于NoneBot2进行适配的兽云随机毛图插件",#包的简述
     long_description=long_description,    #包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/Ekac00/nonebot-plugin-RanFurryPic",    #自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
```

