# Comparing `tmp/nonebot_plugin_kurogames-0.1.0.tar.gz` & `tmp/nonebot_plugin_kurogames-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_kurogames-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_kurogames-0.1.2.tar", max compression
```

## Comparing `nonebot_plugin_kurogames-0.1.0.tar` & `nonebot_plugin_kurogames-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1062 2024-05-11 06:32:29.178514 nonebot_plugin_kurogames-0.1.0/LICENSE
--rw-r--r--   0        0        0     2823 2024-05-11 06:32:29.178514 nonebot_plugin_kurogames-0.1.0/README.md
--rw-r--r--   0        0        0     8272 2024-05-11 06:32:29.178514 nonebot_plugin_kurogames-0.1.0/nonebot_plugin_kurogames/Static/PNSResult.html
--rw-r--r--   0        0        0    36234 2024-05-11 06:32:29.178514 nonebot_plugin_kurogames-0.1.0/nonebot_plugin_kurogames/Static/Pics/ACTIONICON.png
--rw-r--r--   0        0        0    25514 2024-05-11 06:32:29.178514 nonebot_plugin_kurogames-0.1.0/nonebot_plugin_kurogames/Static/Pics/ARENAICON.png
--rw-r--r--   0        0        0    41565 2024-05-11 06:32:29.178514 nonebot_plugin_kurogames-0.1.0/nonebot_plugin_kurogames/Static/Pics/BLACKCARD.png
--rw-r--r--   0        0        0    36944 2024-05-11 06:32:29.182514 nonebot_plugin_kurogames-0.1.0/nonebot_plugin_kurogames/Static/Pics/BOSSICON.png
--rw-r--r--   0        0        0  5682114 2024-05-11 06:32:29.194514 nonebot_plugin_kurogames-0.1.0/nonebot_plugin_kurogames/Static/Pics/LAMIA.png
--rw-r--r--   0        0        0    10716 2024-05-11 06:32:29.194514 nonebot_plugin_kurogames-0.1.0/nonebot_plugin_kurogames/Static/Pics/PNS.png
--rw-r--r--   0        0        0    40106 2024-05-11 06:32:29.194514 nonebot_plugin_kurogames-0.1.0/nonebot_plugin_kurogames/Static/Pics/STRONGHOLDICON.png
--rw-r--r--   0        0        0    39390 2024-05-11 06:32:29.194514 nonebot_plugin_kurogames-0.1.0/nonebot_plugin_kurogames/Static/Pics/TRANSFINITEICON.png
--rw-r--r--   0        0        0     1391 2024-05-11 06:32:29.194514 nonebot_plugin_kurogames-0.1.0/nonebot_plugin_kurogames/__init__.py
--rw-r--r--   0        0        0      498 2024-05-11 06:32:29.194514 nonebot_plugin_kurogames-0.1.0/nonebot_plugin_kurogames/handler/calculate_time_stamp.py
--rw-r--r--   0        0        0     3279 2024-05-11 06:32:29.194514 nonebot_plugin_kurogames-0.1.0/nonebot_plugin_kurogames/handler/pns_dao.py
--rw-r--r--   0        0        0     2982 2024-05-11 06:32:29.194514 nonebot_plugin_kurogames-0.1.0/nonebot_plugin_kurogames/handler/pns_handlers/pns_data_handler.py
--rw-r--r--   0        0        0     3059 2024-05-11 06:32:29.198514 nonebot_plugin_kurogames-0.1.0/nonebot_plugin_kurogames/handler/pns_handlers/pns_detail_handler.py
--rw-r--r--   0        0        0     1725 2024-05-11 06:32:29.198514 nonebot_plugin_kurogames-0.1.0/nonebot_plugin_kurogames/handler/pns_handlers/pns_login_handler.py
--rw-r--r--   0        0        0     2498 2024-05-11 06:32:29.198514 nonebot_plugin_kurogames-0.1.0/nonebot_plugin_kurogames/handler/pns_handlers/pns_pic_render.py
--rw-r--r--   0        0        0      483 2024-05-11 06:32:29.198514 nonebot_plugin_kurogames-0.1.0/nonebot_plugin_kurogames/handler/token_judgement.py
--rw-r--r--   0        0        0      585 2024-05-11 06:32:29.198514 nonebot_plugin_kurogames-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3745 1970-01-01 00:00:00.000000 nonebot_plugin_kurogames-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-11 12:37:39.826664 nonebot_plugin_kurogames-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2823 2024-05-11 12:37:39.826664 nonebot_plugin_kurogames-0.1.2/README.md
+-rw-r--r--   0        0        0     8272 2024-05-11 12:37:39.826664 nonebot_plugin_kurogames-0.1.2/nonebot_plugin_kurogames/Static/PNSResult.html
+-rw-r--r--   0        0        0    36234 2024-05-11 12:37:39.826664 nonebot_plugin_kurogames-0.1.2/nonebot_plugin_kurogames/Static/Pics/ACTIONICON.png
+-rw-r--r--   0        0        0    25514 2024-05-11 12:37:39.826664 nonebot_plugin_kurogames-0.1.2/nonebot_plugin_kurogames/Static/Pics/ARENAICON.png
+-rw-r--r--   0        0        0    41565 2024-05-11 12:37:39.826664 nonebot_plugin_kurogames-0.1.2/nonebot_plugin_kurogames/Static/Pics/BLACKCARD.png
+-rw-r--r--   0        0        0    36944 2024-05-11 12:37:39.826664 nonebot_plugin_kurogames-0.1.2/nonebot_plugin_kurogames/Static/Pics/BOSSICON.png
+-rw-r--r--   0        0        0  5682114 2024-05-11 12:37:39.842664 nonebot_plugin_kurogames-0.1.2/nonebot_plugin_kurogames/Static/Pics/LAMIA.png
+-rw-r--r--   0        0        0    10716 2024-05-11 12:37:39.842664 nonebot_plugin_kurogames-0.1.2/nonebot_plugin_kurogames/Static/Pics/PNS.png
+-rw-r--r--   0        0        0    40106 2024-05-11 12:37:39.842664 nonebot_plugin_kurogames-0.1.2/nonebot_plugin_kurogames/Static/Pics/STRONGHOLDICON.png
+-rw-r--r--   0        0        0    39390 2024-05-11 12:37:39.842664 nonebot_plugin_kurogames-0.1.2/nonebot_plugin_kurogames/Static/Pics/TRANSFINITEICON.png
+-rw-r--r--   0        0        0     1391 2024-05-11 12:37:39.842664 nonebot_plugin_kurogames-0.1.2/nonebot_plugin_kurogames/__init__.py
+-rw-r--r--   0        0        0      498 2024-05-11 12:37:39.842664 nonebot_plugin_kurogames-0.1.2/nonebot_plugin_kurogames/handler/calculate_time_stamp.py
+-rw-r--r--   0        0        0     3279 2024-05-11 12:37:39.842664 nonebot_plugin_kurogames-0.1.2/nonebot_plugin_kurogames/handler/pns_dao.py
+-rw-r--r--   0        0        0     2982 2024-05-11 12:37:39.842664 nonebot_plugin_kurogames-0.1.2/nonebot_plugin_kurogames/handler/pns_handlers/pns_data_handler.py
+-rw-r--r--   0        0        0     3059 2024-05-11 12:37:39.842664 nonebot_plugin_kurogames-0.1.2/nonebot_plugin_kurogames/handler/pns_handlers/pns_detail_handler.py
+-rw-r--r--   0        0        0     1725 2024-05-11 12:37:39.842664 nonebot_plugin_kurogames-0.1.2/nonebot_plugin_kurogames/handler/pns_handlers/pns_login_handler.py
+-rw-r--r--   0        0        0     2498 2024-05-11 12:37:39.842664 nonebot_plugin_kurogames-0.1.2/nonebot_plugin_kurogames/handler/pns_handlers/pns_pic_render.py
+-rw-r--r--   0        0        0      483 2024-05-11 12:37:39.842664 nonebot_plugin_kurogames-0.1.2/nonebot_plugin_kurogames/handler/token_judgement.py
+-rw-r--r--   0        0        0      539 2024-05-11 12:37:39.842664 nonebot_plugin_kurogames-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3673 1970-01-01 00:00:00.000000 nonebot_plugin_kurogames-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_kurogames-0.1.0/LICENSE` & `nonebot_plugin_kurogames-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.0/README.md` & `nonebot_plugin_kurogames-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.0/nonebot_plugin_kurogames/Static/PNSResult.html` & `nonebot_plugin_kurogames-0.1.2/nonebot_plugin_kurogames/Static/PNSResult.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.0/nonebot_plugin_kurogames/Static/Pics/ACTIONICON.png` & `nonebot_plugin_kurogames-0.1.2/nonebot_plugin_kurogames/Static/Pics/ACTIONICON.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.0/nonebot_plugin_kurogames/Static/Pics/ARENAICON.png` & `nonebot_plugin_kurogames-0.1.2/nonebot_plugin_kurogames/Static/Pics/ARENAICON.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.0/nonebot_plugin_kurogames/Static/Pics/BLACKCARD.png` & `nonebot_plugin_kurogames-0.1.2/nonebot_plugin_kurogames/Static/Pics/BLACKCARD.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.0/nonebot_plugin_kurogames/Static/Pics/BOSSICON.png` & `nonebot_plugin_kurogames-0.1.2/nonebot_plugin_kurogames/Static/Pics/BOSSICON.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.0/nonebot_plugin_kurogames/Static/Pics/LAMIA.png` & `nonebot_plugin_kurogames-0.1.2/nonebot_plugin_kurogames/Static/Pics/LAMIA.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.0/nonebot_plugin_kurogames/Static/Pics/PNS.png` & `nonebot_plugin_kurogames-0.1.2/nonebot_plugin_kurogames/Static/Pics/PNS.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.0/nonebot_plugin_kurogames/Static/Pics/STRONGHOLDICON.png` & `nonebot_plugin_kurogames-0.1.2/nonebot_plugin_kurogames/Static/Pics/STRONGHOLDICON.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.0/nonebot_plugin_kurogames/Static/Pics/TRANSFINITEICON.png` & `nonebot_plugin_kurogames-0.1.2/nonebot_plugin_kurogames/Static/Pics/TRANSFINITEICON.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.0/nonebot_plugin_kurogames/__init__.py` & `nonebot_plugin_kurogames-0.1.2/nonebot_plugin_kurogames/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.0/nonebot_plugin_kurogames/handler/pns_dao.py` & `nonebot_plugin_kurogames-0.1.2/nonebot_plugin_kurogames/handler/pns_dao.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.0/nonebot_plugin_kurogames/handler/pns_handlers/pns_data_handler.py` & `nonebot_plugin_kurogames-0.1.2/nonebot_plugin_kurogames/handler/pns_handlers/pns_data_handler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.0/nonebot_plugin_kurogames/handler/pns_handlers/pns_detail_handler.py` & `nonebot_plugin_kurogames-0.1.2/nonebot_plugin_kurogames/handler/pns_handlers/pns_detail_handler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.0/nonebot_plugin_kurogames/handler/pns_handlers/pns_login_handler.py` & `nonebot_plugin_kurogames-0.1.2/nonebot_plugin_kurogames/handler/pns_handlers/pns_login_handler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.0/nonebot_plugin_kurogames/handler/pns_handlers/pns_pic_render.py` & `nonebot_plugin_kurogames-0.1.2/nonebot_plugin_kurogames/handler/pns_handlers/pns_pic_render.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.0/pyproject.toml` & `nonebot_plugin_kurogames-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 [tool.poetry]
 name = "nonebot-plugin-kurogames"
-version = "0.1.0"
+version = "0.1.2"
 description = "库洛游戏数据详情 谢比螺六~"
 authors = ["ConcyWee <concywee@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ConcyWee/nonebot-plugin-kurogames"
 repository = "https://github.com/ConcyWee/nonebot-plugin-kurogames"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 nonebot2 = ">=2.2.1"
-nonebot-adapters-onebot = ">=2.2.3"
+nonebot-adapter-onebot = ">=2.2.3"
 httpx = ">=0.27.0"
-sqlite3 = ">=3.37.0"
-playwright = ">=1.28.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_kurogames-0.1.0/PKG-INFO` & `nonebot_plugin_kurogames-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-kurogames
-Version: 0.1.0
+Version: 0.1.2
 Summary: 库洛游戏数据详情 谢比螺六~
 Home-page: https://github.com/ConcyWee/nonebot-plugin-kurogames
 License: MIT
 Author: ConcyWee
 Author-email: concywee@163.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: httpx (>=0.27.0)
-Requires-Dist: nonebot-adapters-onebot (>=2.2.3)
+Requires-Dist: nonebot-adapter-onebot (>=2.2.3)
 Requires-Dist: nonebot2 (>=2.2.1)
-Requires-Dist: playwright (>=1.28.0)
-Requires-Dist: sqlite3 (>=3.37.0)
 Project-URL: Repository, https://github.com/ConcyWee/nonebot-plugin-kurogames
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
```

#### html2text {}

```diff
@@ -1,20 +1,19 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-kurogames Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-kurogames Version: 0.1.2 Summary:
 åºæ´æ¸¸ææ°æ®è¯¦æ è°¢æ¯èºå­~ Home-page: https://github.com/ConcyWee/
 nonebot-plugin-kurogames License: MIT Author: ConcyWee Author-email:
 concywee@163.com Requires-Python: >=3.8 Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Requires-Dist: httpx (>=0.27.0) Requires-Dist: nonebot-adapters-
-onebot (>=2.2.3) Requires-Dist: nonebot2 (>=2.2.1) Requires-Dist: playwright
-(>=1.28.0) Requires-Dist: sqlite3 (>=3.37.0) Project-URL: Repository, https://
-github.com/ConcyWee/nonebot-plugin-kurogames Description-Content-Type: text/
-markdown
+Python :: 3.12 Requires-Dist: httpx (>=0.27.0) Requires-Dist: nonebot-adapter-
+onebot (>=2.2.3) Requires-Dist: nonebot2 (>=2.2.1) Project-URL: Repository,
+https://github.com/ConcyWee/nonebot-plugin-kurogames Description-Content-Type:
+text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
  # nonebot-plugin-kurogames _â¨ ä¸æ¬¾åºæ´æ¸¸ææ°æ®è¯¦æ è°¢æ¯èºå­~
                           â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## ð ä»ç» è¾å¥å½ä»¤å³å¯æ¥è¯¢åºæ´æ¸¸ææ°æ®è¯¦æ
 tokençè·åæ¹æ³è¯·èªè¡æ¥æ¾å¦~ tokenæ ¼å¼å¦ä¸æç¤º ![image](https:
 //github.com/ConcyWee/nonebot-plugin-kurogames/assets/36001297/1fc32ace-cca4-
```

