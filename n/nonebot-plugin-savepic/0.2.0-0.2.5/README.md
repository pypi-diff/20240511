# Comparing `tmp/nonebot_plugin_savepic-0.2.0.tar.gz` & `tmp/nonebot_plugin_savepic-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_savepic-0.2.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_savepic-0.2.5.tar", max compression
```

## Comparing `nonebot_plugin_savepic-0.2.0.tar` & `nonebot_plugin_savepic-0.2.5.tar`

### file list

```diff
@@ -1,12 +1,17 @@
--rw-r--r--   0        0        0     1060 2023-08-03 04:29:59.872363 nonebot_plugin_savepic-0.2.0/LICENSE
--rw-r--r--   0        0        0     1984 2023-08-03 04:29:59.872363 nonebot_plugin_savepic-0.2.0/README.md
--rw-r--r--   0        0        0     6304 2023-08-03 04:29:59.872363 nonebot_plugin_savepic-0.2.0/nonebot_plugin_savepic/__init__.py
--rw-r--r--   0        0        0      206 2023-08-03 04:29:59.876363 nonebot_plugin_savepic-0.2.0/nonebot_plugin_savepic/config.py
--rw-r--r--   0        0        0     1052 2023-08-03 04:29:59.876363 nonebot_plugin_savepic-0.2.0/nonebot_plugin_savepic/ext_listener.py
--rw-r--r--   0        0        0      846 2023-08-03 04:29:59.876363 nonebot_plugin_savepic-0.2.0/nonebot_plugin_savepic/migrations/1a654e02179b_.py
--rw-r--r--   0        0        0      744 2023-08-03 04:29:59.876363 nonebot_plugin_savepic-0.2.0/nonebot_plugin_savepic/model.py
--rw-r--r--   0        0        0     6653 2023-08-03 04:29:59.876363 nonebot_plugin_savepic-0.2.0/nonebot_plugin_savepic/pic_sql.py
--rw-r--r--   0        0        0     1548 2023-08-03 04:29:59.876363 nonebot_plugin_savepic-0.2.0/nonebot_plugin_savepic/picture.py
--rw-r--r--   0        0        0      920 2023-08-03 04:29:59.876363 nonebot_plugin_savepic-0.2.0/nonebot_plugin_savepic/rule.py
--rw-r--r--   0        0        0      642 2023-08-03 04:29:59.876363 nonebot_plugin_savepic-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2856 1970-01-01 00:00:00.000000 nonebot_plugin_savepic-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-05-10 20:45:13.367812 nonebot_plugin_savepic-0.2.5/LICENSE
+-rw-r--r--   0        0        0     2770 2024-05-10 20:45:13.367812 nonebot_plugin_savepic-0.2.5/README.md
+-rw-r--r--   0        0        0    13952 2024-05-10 20:45:13.367812 nonebot_plugin_savepic-0.2.5/nonebot_plugin_savepic/__init__.py
+-rw-r--r--   0        0        0     1726 2024-05-10 20:45:13.367812 nonebot_plugin_savepic-0.2.5/nonebot_plugin_savepic/ai_utils.py
+-rw-r--r--   0        0        0      602 2024-05-10 20:45:13.367812 nonebot_plugin_savepic-0.2.5/nonebot_plugin_savepic/config.py
+-rw-r--r--   0        0        0      786 2024-05-10 20:45:13.367812 nonebot_plugin_savepic-0.2.5/nonebot_plugin_savepic/countpic.py
+-rw-r--r--   0        0        0      662 2024-05-10 20:45:13.367812 nonebot_plugin_savepic-0.2.5/nonebot_plugin_savepic/error.py
+-rw-r--r--   0        0        0      906 2024-05-10 20:45:13.367812 nonebot_plugin_savepic-0.2.5/nonebot_plugin_savepic/ext_listener.py
+-rw-r--r--   0        0        0     3868 2024-05-10 20:45:13.367812 nonebot_plugin_savepic-0.2.5/nonebot_plugin_savepic/model.py
+-rw-r--r--   0        0        0        0 2024-05-10 20:45:13.367812 nonebot_plugin_savepic-0.2.5/nonebot_plugin_savepic/networks/__init__.py
+-rw-r--r--   0        0        0     8015 2024-05-10 20:45:13.367812 nonebot_plugin_savepic-0.2.5/nonebot_plugin_savepic/networks/resnet_big.py
+-rw-r--r--   0        0        0    13267 2024-05-10 20:45:13.367812 nonebot_plugin_savepic-0.2.5/nonebot_plugin_savepic/pic_sql.py
+-rw-r--r--   0        0        0     2250 2024-05-10 20:45:13.367812 nonebot_plugin_savepic-0.2.5/nonebot_plugin_savepic/picture.py
+-rw-r--r--   0        0        0     1391 2024-05-10 20:45:13.367812 nonebot_plugin_savepic-0.2.5/nonebot_plugin_savepic/randpic.py
+-rw-r--r--   0        0        0     1407 2024-05-10 20:45:13.367812 nonebot_plugin_savepic-0.2.5/nonebot_plugin_savepic/rule.py
+-rw-r--r--   0        0        0      691 2024-05-10 20:45:13.371812 nonebot_plugin_savepic-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     3784 1970-01-01 00:00:00.000000 nonebot_plugin_savepic-0.2.5/PKG-INFO
```

### Comparing `nonebot_plugin_savepic-0.2.0/LICENSE` & `nonebot_plugin_savepic-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_savepic-0.2.0/README.md` & `nonebot_plugin_savepic-0.2.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -18,18 +18,35 @@
 
 保存表情包
 
 ### randpic
 
 抽取表情包
 
+### mvpic
+
+重命名表情包，或者修改表情包所属的群域
+
+例如：
+```
+/mvpic -l name.jpg -g waaaaa.gif
+```
+就是把本群的 name.jpg 改成全局名为 waaaaa.gif 的表情包
+
+同理
+```
+/mvpic -g waaaaa.gif -l waaaaa.gif
+```
+就是从全局移到本群（接收到命令的群）
+
 ### 直接发送文件名
 
 发送文件名即可发送表情包
 
+
 ## 💿 安装
 
 <details open>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
     nb plugin install nonebot-plugin-savepic
@@ -71,14 +88,21 @@
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | savepic_admin | 否 | 无 | 权限用户 |
 | savepic_dir | 否 | savepic | 图片本地保存位置 |
+| simpic_enable | 否 | False | 是否开启基于RNN模型的AI相似度检索功能，如果开启要填写 Pinecone 相关配置 |
+| pinecone_apikey | 否 | 无 | pinecone 的 Key |
+| pinecone_environment | 否 | 无 | pinecone 的 enviroment，是数据库的属性之一 |
+| pinecone_index | 否 | savepic | 同上。 |
+| dashscope_api | 否 | 无 | dashscope 的 APIKey。 用于开启基于语义的相似度检索功能 |
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
-| savepic | 群员 | 是 | 群聊 | 保存图片 |
-| randpic | 群员 | 是 | 全部 | 随机图片 |
+| savepic | 群员 | 否 | 群聊 | 保存图片 |
+| randpic | 群员 | 否 | 全部 | 随机图片 |
+| mvpic | 管理员 | 否 | 群聊 | 重命名图片 |
+
```

#### html2text {}

```diff
@@ -1,20 +1,33 @@
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
  # nonebot-plugin-savepic _â¨ ä¸ä¸ªå­åå¾ççæä»¶ â¨_ ## ð ä»ç»
       éåèª Fran ç Savepic ### savepic ä¿å­è¡¨æå ### randpic
-æ½åè¡¨æå ### ç´æ¥åéæä»¶å åéæä»¶åå³å¯åéè¡¨æå
-               ## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
-é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
-     install nonebot-plugin-savepic ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
-  é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
-è¾å¥ç¸åºçå®è£å½ä»¤ pip pip install nonebot-plugin-savepic pdm pdm add
-  nonebot-plugin-savepic poetry poetry add nonebot-plugin-savepic conda conda
-     install nonebot-plugin-savepic æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
-  `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
-           ["nonebot_plugin_savepic"] ## âï¸ éç½® å¨ nonebot2
+                           æ½åè¡¨æå ### mvpic
+éå½åè¡¨æåï¼æèä¿®æ¹è¡¨æåæå±çç¾¤å ä¾å¦ï¼ ``` /mvpic
+ -l name.jpg -g waaaaa.gif ``` å°±æ¯ææ¬ç¾¤ç name.jpg æ¹æå¨å±åä¸º
+   waaaaa.gif çè¡¨æå åç ``` /mvpic -g waaaaa.gif -l waaaaa.gif ```
+          å°±æ¯ä»å¨å±ç§»å°æ¬ç¾¤ï¼æ¥æ¶å°å½ä»¤çç¾¤ï¼ ###
+   ç´æ¥åéæä»¶å åéæä»¶åå³å¯åéè¡¨æå ## ð¿ å®è£
+    ä½¿ç¨ nb-cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
+    è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-savepic
+        ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
+ æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
+   pip pip install nonebot-plugin-savepic pdm pdm add nonebot-plugin-savepic
+ poetry poetry add nonebot-plugin-savepic conda conda install nonebot-plugin-
+ savepic æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
+  [tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_savepic"] ##
+                          âï¸ éç½® å¨ nonebot2
  é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
 é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | savepic_admin | å¦ | æ 
-| æéç¨æ· | | savepic_dir | å¦ | savepic | å¾çæ¬å°ä¿å­ä½ç½® | ##
-ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:---
-     --:|:----:|:----:|:----:|:----:| | savepic | ç¾¤å | æ¯ | ç¾¤è |
-       ä¿å­å¾ç | | randpic | ç¾¤å | æ¯ | å¨é¨ | éæºå¾ç |
+ | æéç¨æ· | | savepic_dir | å¦ | savepic | å¾çæ¬å°ä¿å­ä½ç½® | |
+                         simpic_enable | å¦ | False |
+ æ¯å¦å¼å¯åºäºRNNæ¨¡åçAIç¸ä¼¼åº¦æ£ç´¢åè½ï¼å¦æå¼å¯è¦å¡«å
+ Pinecone ç¸å³éç½® | | pinecone_apikey | å¦ | æ  | pinecone ç Key | |
+                pinecone_environment | å¦ | æ  | pinecone ç
+ enviromentï¼æ¯æ°æ®åºçå±æ§ä¹ä¸ | | pinecone_index | å¦ | savepic |
+       åä¸ã | | dashscope_api | å¦ | æ  | dashscope ç APIKeyã
+ç¨äºå¼å¯åºäºè¯­ä¹çç¸ä¼¼åº¦æ£ç´¢åè½ | ## ð ä½¿ç¨ ### æä»¤è¡¨
+| æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:
+----:| | savepic | ç¾¤å | å¦ | ç¾¤è | ä¿å­å¾ç | | randpic | ç¾¤å |
+      å¦ | å¨é¨ | éæºå¾ç | | mvpic | ç®¡çå | å¦ | ç¾¤è |
+                               éå½åå¾ç |
```

### Comparing `nonebot_plugin_savepic-0.2.0/nonebot_plugin_savepic/ext_listener.py` & `nonebot_plugin_savepic-0.2.5/nonebot_plugin_savepic/ext_listener.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,21 @@
-from nonebot import on_message
+from nonebot.plugin import on_endswith
 from nonebot.adapters.onebot.v11.event import MessageEvent
 from nonebot.internal.adapter.bot import Bot
 from nonebot.adapters.onebot.v11.message import MessageSegment as V11Seg
 from nonebot.adapters.onebot.v11.event import GroupMessageEvent
+from .pic_sql import select_pic
+from .picture import load_pic
 
-from .pic_sql import load_pic, select_pic
-
-
-async def endswith_pic(event: MessageEvent):
-    text = event.message.extract_plain_text().strip()
-    if " " in text:
-        return False
-    return text.endswith((".jpg", ".png", ".gif"))
-
-
-pic_listen = on_message(rule=endswith_pic)
+pic_listen = on_endswith((".jpg", ".png", ".gif"), priority=50, block=False)
 
 
 @pic_listen.handle()
 async def _(bot: Bot, event: MessageEvent):
-    name = event.message.extract_plain_text().strip()
+    name = event.get_plaintext().strip()
     group_id = (
         "globe"
         if not isinstance(event, GroupMessageEvent)
         else f"qq_group:{event.group_id}"
     )
     try:
         pic = await select_pic(name, group_id)
```

### Comparing `nonebot_plugin_savepic-0.2.0/nonebot_plugin_savepic/picture.py` & `nonebot_plugin_savepic-0.2.5/nonebot_plugin_savepic/picture.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,21 @@
-import scipy.fftpack as fft
-import numpy as np
+import nonebot
 import httpx
+import hashlib
 import os
 from PIL import Image
-from io import BytesIO
+from .config import Config
 
+if False:
+    from .model import EmoSame
+
+_emo_same = None
 _httpx_async = None
+gdriver = nonebot.get_driver()
+plugin_config = Config.parse_obj(gdriver.config)
 
 
 def remove_alpha(im: Image) -> Image:
     # Only process if image has transparency (http://stackoverflow.com/a/1963146)
     if im.mode in ("RGBA", "LA") or (im.mode == "P" and "transparency" in im.info):
         # Need to convert to RGBA if LA format due to a bug in PIL (http://stackoverflow.com/a/1963146)
         alpha = im.convert("RGBA").split()[-1]
@@ -21,28 +27,51 @@
         bg.paste(im, mask=alpha)
         return bg
 
     else:
         return im
 
 
+def del_pic(url: str):
+    if url.startswith("http"):
+        return
+    if os.path.exists(url):
+        os.remove(url)
+
+
 async def load_pic(url: str) -> bytes:
     global _httpx_async
     if url.startswith("http"):
         if not _httpx_async:
             _httpx_async = httpx.AsyncClient()
         resp = await _httpx_async.get(url)
         resp.raise_for_status()
         return resp.content
     if os.path.exists(url):
         with open(url, "rb") as f:
             return f.read()
-    raise Exception("不支持的 URL")
+    raise Exception(f"不支持的 URL\n{url}")
+
 
+async def write_pic(url: str, des_dir: str = None) -> str:
+    if not des_dir:
+        des_dir = "savepic"
+    if not os.path.exists(des_dir):
+        os.makedirs(des_dir)
+
+    byte = await load_pic(url)
+    filename = hashlib.sha256(byte).hexdigest()
+    while os.path.exists(os.path.join(des_dir, filename)):
+        filename += "_"
+    with open(os.path.join(des_dir, filename), "wb") as f:
+        f.write(byte)
+    return os.path.join(des_dir, filename)
+
+
+@gdriver.on_startup
+async def _():
+    global _emo_same, plugin_config
+    if not plugin_config.simpic_enable:  # AI 相似度判断
+        return
 
-def p_hash(img: bytes) -> bytes:
-    pic = remove_alpha(
-        Image.open(BytesIO(img)).resize((128, 128), Image.Resampling.LANCZOS)
-    ).convert("L")
-    dct = fft.dct(np.array(pic))
-    average = np.median(dct)
-    return np.packbits(dct[:16, :16] > average).tobytes()
+    # if not _emo_same:
+    #     _emo_same = EmoSame(plugin_config.p_model_path, plugin_config.q_model_path)
```

### Comparing `nonebot_plugin_savepic-0.2.0/nonebot_plugin_savepic/rule.py` & `nonebot_plugin_savepic-0.2.5/nonebot_plugin_savepic/rule.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """ 
 This module is used to define the permission of the bot.
 """
 
-import nonebot
+from nonebot import get_plugin_config
 from nonebot.adapters import Bot, Event
 from nonebot.internal.permission import Permission
-
+from nonebot.adapters.onebot.v11.event import GroupMessageEvent as V11G
 from .config import Config
 
-global_config = nonebot.get_driver().config
-plugin_config = Config.parse_obj(global_config)
+plugin_config = get_plugin_config(Config)
 
 
 class Savepic_Admin(Permission):
     """检查当前事件是否是消息事件且属于 Savepic_Admin"""
 
     __slots__ = ()
 
@@ -28,8 +27,26 @@
         return (
             f"{bot.adapter.get_name().split(maxsplit=1)[0].lower()}:{user_id}"
             in plugin_config.savepic_admin
             or user_id in plugin_config.savepic_admin  # 兼容旧配置
         )
 
 
+class BlackGroup(Permission):
+
+    __slots__ = ()
+
+    def __repr__(self) -> str:
+        return "BlackGroup()"
+
+    async def __call__(self, bot: Bot, event: Event) -> bool:
+        if not isinstance(event, V11G):
+            return True
+        try:
+            group_id = str(event.group_id)
+        except Exception:
+            return True
+        return group_id not in plugin_config.black_group
+
+
 PIC_AMDIN = Permission(Savepic_Admin())
+BLACK_GROUP = Permission(BlackGroup())
```

### Comparing `nonebot_plugin_savepic-0.2.0/pyproject.toml` & `nonebot_plugin_savepic-0.2.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-savepic"
-version = "0.2.0"
+version = "0.2.5"
 description = "保存表情包（语录）与随机出图"
 authors = ["Yan <1964649083@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_savepic"}]
 homepage = "https://github.com/Yan-Zero/nonebot-plugin-savepic"
 
@@ -14,12 +14,14 @@
 nonebot-plugin-datastore = "^1.1.0"
 asyncpg = "^0.28.0"
 nonebot-adapter-onebot = "^2.2.3"
 arclet-alconna = "^1.7.14"
 numpy = "^1.25.2"
 scipy = "^1.11.1"
 pillow = "^10.0.0"
+dashscope = "^1.17.0"
+pinecone-client = "^3.2.2"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_savepic-0.2.0/PKG-INFO` & `nonebot_plugin_savepic-0.2.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-savepic
-Version: 0.2.0
+Version: 0.2.5
 Summary: 保存表情包（语录）与随机出图
 Home-page: https://github.com/Yan-Zero/nonebot-plugin-savepic
 License: MIT
 Author: Yan
 Author-email: 1964649083@qq.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: arclet-alconna (>=1.7.14,<2.0.0)
 Requires-Dist: asyncpg (>=0.28.0,<0.29.0)
+Requires-Dist: dashscope (>=1.17.0,<2.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
 Requires-Dist: nonebot-plugin-datastore (>=1.1.0,<2.0.0)
 Requires-Dist: nonebot2 (>=2.0.1,<3.0.0)
 Requires-Dist: numpy (>=1.25.2,<2.0.0)
 Requires-Dist: pillow (>=10.0.0,<11.0.0)
+Requires-Dist: pinecone-client (>=3.2.2,<4.0.0)
 Requires-Dist: scipy (>=1.11.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
@@ -41,18 +44,35 @@
 
 保存表情包
 
 ### randpic
 
 抽取表情包
 
+### mvpic
+
+重命名表情包，或者修改表情包所属的群域
+
+例如：
+```
+/mvpic -l name.jpg -g waaaaa.gif
+```
+就是把本群的 name.jpg 改成全局名为 waaaaa.gif 的表情包
+
+同理
+```
+/mvpic -g waaaaa.gif -l waaaaa.gif
+```
+就是从全局移到本群（接收到命令的群）
+
 ### 直接发送文件名
 
 发送文件名即可发送表情包
 
+
 ## 💿 安装
 
 <details open>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
     nb plugin install nonebot-plugin-savepic
@@ -94,15 +114,22 @@
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | savepic_admin | 否 | 无 | 权限用户 |
 | savepic_dir | 否 | savepic | 图片本地保存位置 |
+| simpic_enable | 否 | False | 是否开启基于RNN模型的AI相似度检索功能，如果开启要填写 Pinecone 相关配置 |
+| pinecone_apikey | 否 | 无 | pinecone 的 Key |
+| pinecone_environment | 否 | 无 | pinecone 的 enviroment，是数据库的属性之一 |
+| pinecone_index | 否 | savepic | 同上。 |
+| dashscope_api | 否 | 无 | dashscope 的 APIKey。 用于开启基于语义的相似度检索功能 |
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
-| savepic | 群员 | 是 | 群聊 | 保存图片 |
-| randpic | 群员 | 是 | 全部 | 随机图片 |
+| savepic | 群员 | 否 | 群聊 | 保存图片 |
+| randpic | 群员 | 否 | 全部 | 随机图片 |
+| mvpic | 管理员 | 否 | 群聊 | 重命名图片 |
+
```

#### html2text {}

```diff
@@ -1,32 +1,47 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-savepic Version: 0.2.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-savepic Version: 0.2.5 Summary:
 ä¿å­è¡¨æåï¼è¯­å½ï¼ä¸éæºåºå¾ Home-page: https://github.com/Yan-
 Zero/nonebot-plugin-savepic License: MIT Author: Yan Author-email:
 1964649083@qq.com Requires-Python: >=3.10,<3.13 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: arclet-alconna (>=1.7.14,<2.0.0)
-Requires-Dist: asyncpg (>=0.28.0,<0.29.0) Requires-Dist: nonebot-adapter-onebot
-(>=2.2.3,<3.0.0) Requires-Dist: nonebot-plugin-datastore (>=1.1.0,<2.0.0)
-Requires-Dist: nonebot2 (>=2.0.1,<3.0.0) Requires-Dist: numpy (>=1.25.2,<2.0.0)
-Requires-Dist: pillow (>=10.0.0,<11.0.0) Requires-Dist: scipy (>=1.11.1,<2.0.0)
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: arclet-alconna (>=1.7.14,<2.0.0) Requires-Dist: asyncpg
+(>=0.28.0,<0.29.0) Requires-Dist: dashscope (>=1.17.0,<2.0.0) Requires-Dist:
+nonebot-adapter-onebot (>=2.2.3,<3.0.0) Requires-Dist: nonebot-plugin-datastore
+(>=1.1.0,<2.0.0) Requires-Dist: nonebot2 (>=2.0.1,<3.0.0) Requires-Dist: numpy
+(>=1.25.2,<2.0.0) Requires-Dist: pillow (>=10.0.0,<11.0.0) Requires-Dist:
+pinecone-client (>=3.2.2,<4.0.0) Requires-Dist: scipy (>=1.11.1,<2.0.0)
 Description-Content-Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
  # nonebot-plugin-savepic _â¨ ä¸ä¸ªå­åå¾ççæä»¶ â¨_ ## ð ä»ç»
       éåèª Fran ç Savepic ### savepic ä¿å­è¡¨æå ### randpic
-æ½åè¡¨æå ### ç´æ¥åéæä»¶å åéæä»¶åå³å¯åéè¡¨æå
-               ## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
-é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
-     install nonebot-plugin-savepic ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
-  é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
-è¾å¥ç¸åºçå®è£å½ä»¤ pip pip install nonebot-plugin-savepic pdm pdm add
-  nonebot-plugin-savepic poetry poetry add nonebot-plugin-savepic conda conda
-     install nonebot-plugin-savepic æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
-  `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
-           ["nonebot_plugin_savepic"] ## âï¸ éç½® å¨ nonebot2
+                           æ½åè¡¨æå ### mvpic
+éå½åè¡¨æåï¼æèä¿®æ¹è¡¨æåæå±çç¾¤å ä¾å¦ï¼ ``` /mvpic
+ -l name.jpg -g waaaaa.gif ``` å°±æ¯ææ¬ç¾¤ç name.jpg æ¹æå¨å±åä¸º
+   waaaaa.gif çè¡¨æå åç ``` /mvpic -g waaaaa.gif -l waaaaa.gif ```
+          å°±æ¯ä»å¨å±ç§»å°æ¬ç¾¤ï¼æ¥æ¶å°å½ä»¤çç¾¤ï¼ ###
+   ç´æ¥åéæä»¶å åéæä»¶åå³å¯åéè¡¨æå ## ð¿ å®è£
+    ä½¿ç¨ nb-cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
+    è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-savepic
+        ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
+ æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
+   pip pip install nonebot-plugin-savepic pdm pdm add nonebot-plugin-savepic
+ poetry poetry add nonebot-plugin-savepic conda conda install nonebot-plugin-
+ savepic æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
+  [tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_savepic"] ##
+                          âï¸ éç½® å¨ nonebot2
  é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
 é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | savepic_admin | å¦ | æ 
-| æéç¨æ· | | savepic_dir | å¦ | savepic | å¾çæ¬å°ä¿å­ä½ç½® | ##
-ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:---
-     --:|:----:|:----:|:----:|:----:| | savepic | ç¾¤å | æ¯ | ç¾¤è |
-       ä¿å­å¾ç | | randpic | ç¾¤å | æ¯ | å¨é¨ | éæºå¾ç |
+ | æéç¨æ· | | savepic_dir | å¦ | savepic | å¾çæ¬å°ä¿å­ä½ç½® | |
+                         simpic_enable | å¦ | False |
+ æ¯å¦å¼å¯åºäºRNNæ¨¡åçAIç¸ä¼¼åº¦æ£ç´¢åè½ï¼å¦æå¼å¯è¦å¡«å
+ Pinecone ç¸å³éç½® | | pinecone_apikey | å¦ | æ  | pinecone ç Key | |
+                pinecone_environment | å¦ | æ  | pinecone ç
+ enviromentï¼æ¯æ°æ®åºçå±æ§ä¹ä¸ | | pinecone_index | å¦ | savepic |
+       åä¸ã | | dashscope_api | å¦ | æ  | dashscope ç APIKeyã
+ç¨äºå¼å¯åºäºè¯­ä¹çç¸ä¼¼åº¦æ£ç´¢åè½ | ## ð ä½¿ç¨ ### æä»¤è¡¨
+| æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:
+----:| | savepic | ç¾¤å | å¦ | ç¾¤è | ä¿å­å¾ç | | randpic | ç¾¤å |
+      å¦ | å¨é¨ | éæºå¾ç | | mvpic | ç®¡çå | å¦ | ç¾¤è |
+                               éå½åå¾ç |
```

