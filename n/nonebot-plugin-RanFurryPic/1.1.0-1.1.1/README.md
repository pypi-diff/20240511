# Comparing `tmp/nonebot_plugin_ranfurrypic-1.1.0.tar.gz` & `tmp/nonebot_plugin_ranfurrypic-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ranfurrypic-1.1.0.tar", last modified: Sat May 11 15:19:07 2024, max compression
+gzip compressed data, was "nonebot_plugin_ranfurrypic-1.1.1.tar", last modified: Sat May 11 15:23:04 2024, max compression
```

## Comparing `nonebot_plugin_ranfurrypic-1.1.0.tar` & `nonebot_plugin_ranfurrypic-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 15:19:07.140524 nonebot_plugin_ranfurrypic-1.1.0/
--rw-rw-rw-   0        0        0     1082 2024-05-10 14:34:54.000000 nonebot_plugin_ranfurrypic-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     2874 2024-05-11 15:19:07.139526 nonebot_plugin_ranfurrypic-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2507 2024-05-11 14:12:40.000000 nonebot_plugin_ranfurrypic-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 15:19:07.112542 nonebot_plugin_ranfurrypic-1.1.0/nonebot_plugin_RanFurryPic/
--rw-rw-rw-   0        0        0     5262 2024-05-11 15:10:20.000000 nonebot_plugin_ranfurrypic-1.1.0/nonebot_plugin_RanFurryPic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 15:19:07.138526 nonebot_plugin_ranfurrypic-1.1.0/nonebot_plugin_RanFurryPic.egg-info/
--rw-rw-rw-   0        0        0     2874 2024-05-11 15:19:07.000000 nonebot_plugin_ranfurrypic-1.1.0/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2024-05-11 15:19:07.000000 nonebot_plugin_ranfurrypic-1.1.0/nonebot_plugin_RanFurryPic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 15:19:07.000000 nonebot_plugin_ranfurrypic-1.1.0/nonebot_plugin_RanFurryPic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-11 15:19:07.000000 nonebot_plugin_ranfurrypic-1.1.0/nonebot_plugin_RanFurryPic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-05-11 15:19:07.000000 nonebot_plugin_ranfurrypic-1.1.0/nonebot_plugin_RanFurryPic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      380 2024-05-11 15:15:22.000000 nonebot_plugin_ranfurrypic-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-11 15:19:07.141523 nonebot_plugin_ranfurrypic-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-11 15:23:04.090557 nonebot_plugin_ranfurrypic-1.1.1/
+-rw-rw-rw-   0        0        0     1082 2024-05-10 14:34:54.000000 nonebot_plugin_ranfurrypic-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2874 2024-05-11 15:23:04.089558 nonebot_plugin_ranfurrypic-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2507 2024-05-11 14:12:40.000000 nonebot_plugin_ranfurrypic-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 15:23:04.075566 nonebot_plugin_ranfurrypic-1.1.1/nonebot_plugin_RanFurryPic/
+-rw-rw-rw-   0        0        0     5262 2024-05-11 15:22:26.000000 nonebot_plugin_ranfurrypic-1.1.1/nonebot_plugin_RanFurryPic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 15:23:04.088560 nonebot_plugin_ranfurrypic-1.1.1/nonebot_plugin_RanFurryPic.egg-info/
+-rw-rw-rw-   0        0        0     2874 2024-05-11 15:23:04.000000 nonebot_plugin_ranfurrypic-1.1.1/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-05-11 15:23:04.000000 nonebot_plugin_ranfurrypic-1.1.1/nonebot_plugin_RanFurryPic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 15:23:04.000000 nonebot_plugin_ranfurrypic-1.1.1/nonebot_plugin_RanFurryPic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-11 15:23:04.000000 nonebot_plugin_ranfurrypic-1.1.1/nonebot_plugin_RanFurryPic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-05-11 15:23:04.000000 nonebot_plugin_ranfurrypic-1.1.1/nonebot_plugin_RanFurryPic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      380 2024-05-11 15:22:39.000000 nonebot_plugin_ranfurrypic-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-11 15:23:04.091557 nonebot_plugin_ranfurrypic-1.1.1/setup.cfg
```

### Comparing `nonebot_plugin_ranfurrypic-1.1.0/LICENSE` & `nonebot_plugin_ranfurrypic-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ranfurrypic-1.1.0/PKG-INFO` & `nonebot_plugin_ranfurrypic-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_RanFurryPic
-Version: 1.1.0
+Version: 1.1.1
 Summary: 基于NoneBot2进行适配的兽云随机毛图插件
 Author-email: Ekac <2396382559@qq.com>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.1.1 Summary:
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Author-email: Ekac
 <2396382559@qq.com> License: MIT Requires-Python: >=3.9 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-
 Dist: httpx Requires-Dist: nonebot-adapter-onebot
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
   # nonebot-plugin-RanFurryPic _â¨ éæºæ¯å¾ â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
```

### Comparing `nonebot_plugin_ranfurrypic-1.1.0/README.md` & `nonebot_plugin_ranfurrypic-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ranfurrypic-1.1.0/nonebot_plugin_RanFurryPic/__init__.py` & `nonebot_plugin_ranfurrypic-1.1.1/nonebot_plugin_RanFurryPic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,18 +78,16 @@
     async with httpx.AsyncClient() as client:
         id_response = await client.get(id_url, headers=headers)
         if id_response.status_code == 200:
             pic_json = id_response.json()
             pic_id = pic_json["picture"]["picture"]
             logger.success(f"状态码：{id_response.status_code}\n原始内容：{id_response.text}\n图片ID:{pic_id}")
         else:
-            logger.error(f"请求失败！
-状态码：{id_response.status_code}")
-            return f"请求失败！
-状态码：{id_response.status_code}"
+            logger.error(f"请求失败！\n状态码：{id_response.status_code}")
+            return f"请求失败！\n状态码：{id_response.status_code}"
 
     # 发送图片请求
     pic_url = "https://cloud.foxtail.cn/api/function/pictures?picture=" + pic_id
     pic_id_url = ""
     async with httpx.AsyncClient() as client:
         pic_response = await client.get(pic_url, headers=headers)
         if pic_response.status_code == 200:
```

### Comparing `nonebot_plugin_ranfurrypic-1.1.0/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO` & `nonebot_plugin_ranfurrypic-1.1.1/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_RanFurryPic
-Version: 1.1.0
+Version: 1.1.1
 Summary: 基于NoneBot2进行适配的兽云随机毛图插件
 Author-email: Ekac <2396382559@qq.com>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.1.1 Summary:
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Author-email: Ekac
 <2396382559@qq.com> License: MIT Requires-Python: >=3.9 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-
 Dist: httpx Requires-Dist: nonebot-adapter-onebot
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
   # nonebot-plugin-RanFurryPic _â¨ éæºæ¯å¾ â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
```

