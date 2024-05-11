# Comparing `tmp/tsugu-0.5.7.tar.gz` & `tmp/tsugu-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-0.5.7.tar", last modified: Sun Apr 28 15:47:54 2024, max compression
+gzip compressed data, was "tsugu-0.6.0.tar", last modified: Sat May 11 18:18:16 2024, max compression
```

## Comparing `tsugu-0.5.7.tar` & `tsugu-0.6.0.tar`

### file list

```diff
@@ -1,20 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:47:54.488944 tsugu-0.5.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-28 15:47:46.000000 tsugu-0.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-04-28 15:47:54.488944 tsugu-0.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-04-28 15:47:46.000000 tsugu-0.5.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 15:47:54.488944 tsugu-0.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-28 15:47:46.000000 tsugu-0.5.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:47:54.484944 tsugu-0.5.7/test/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-28 15:47:46.000000 tsugu-0.5.7/test/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:47:54.484944 tsugu-0.5.7/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-28 15:47:46.000000 tsugu-0.5.7/tsugu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21285 2024-04-28 15:47:46.000000 tsugu-0.5.7/tsugu/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12544 2024-04-28 15:47:46.000000 tsugu-0.5.7/tsugu/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-28 15:47:46.000000 tsugu-0.5.7/tsugu/router.py
--rw-r--r--   0 runner    (1001) docker     (127)    22011 2024-04-28 15:47:46.000000 tsugu-0.5.7/tsugu/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:47:54.488944 tsugu-0.5.7/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-04-28 15:47:54.000000 tsugu-0.5.7/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-28 15:47:54.000000 tsugu-0.5.7/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 15:47:54.000000 tsugu-0.5.7/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-28 15:47:54.000000 tsugu-0.5.7/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-28 15:47:54.000000 tsugu-0.5.7/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:18:16.669835 tsugu-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-11 18:18:02.000000 tsugu-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6498 2024-05-11 18:18:16.669835 tsugu-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-05-11 18:18:02.000000 tsugu-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 18:18:16.669835 tsugu-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-11 18:18:02.000000 tsugu-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:18:16.665835 tsugu-0.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-11 18:18:02.000000 tsugu-0.6.0/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:18:16.669835 tsugu-0.6.0/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-11 18:18:02.000000 tsugu-0.6.0/tsugu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-05-11 18:18:02.000000 tsugu-0.6.0/tsugu/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-11 18:18:02.000000 tsugu-0.6.0/tsugu/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:18:16.669835 tsugu-0.6.0/tsugu/local/
+-rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-05-11 18:18:02.000000 tsugu-0.6.0/tsugu/local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:18:16.669835 tsugu-0.6.0/tsugu/local/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    15094 2024-05-11 18:18:02.000000 tsugu-0.6.0/tsugu/local/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:18:16.669835 tsugu-0.6.0/tsugu/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-05-11 18:18:02.000000 tsugu-0.6.0/tsugu/remote/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:18:16.669835 tsugu-0.6.0/tsugu/remote/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-11 18:18:02.000000 tsugu-0.6.0/tsugu/remote/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-05-11 18:18:02.000000 tsugu-0.6.0/tsugu/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:18:16.669835 tsugu-0.6.0/tsugu/universal_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-11 18:18:02.000000 tsugu-0.6.0/tsugu/universal_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:18:16.669835 tsugu-0.6.0/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6498 2024-05-11 18:18:16.000000 tsugu-0.6.0/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-11 18:18:16.000000 tsugu-0.6.0/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 18:18:16.000000 tsugu-0.6.0/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-11 18:18:16.000000 tsugu-0.6.0/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-11 18:18:16.000000 tsugu-0.6.0/tsugu.egg-info/top_level.txt
```

### Comparing `tsugu-0.5.7/LICENSE` & `tsugu-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-0.5.7/PKG-INFO` & `tsugu-0.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.5.7
+Version: 0.6.0
 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py
 Author: kumoSleeping
 Author-email: zjr2992@outlook.com
 License: MIT
 Description: 
         <h1 align="center"> Tsugu Python Frontend <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
@@ -37,37 +37,27 @@
         - [x] 自然语言输入 -> 返回结果
         - [ ] 独立路由输入 -> 返回结果 `部分支持`
         - [x] 本地数据库 (sqlite3)
         - [x] 远程数据库 (客户端)
         - [x] 配置项 (基础配置、代理、命令别名 等)
         
         
-        <h2 align="center"> 安装与更新 </h2>
+        <h2 align="center"> 安装 </h2>
         
         ## 安装 tsugu 模块
         ```shell
         pip install tsugu
         ```
         
-        ## 更新
-        ```shell
-        pip install tsugu --upgrade
-        ```
-        
-        ## 使用官方源安装
-        ```shell
-        pip install tsugu --index-url https://pypi.org/simple/
-        ```
         ## 后端需求
         
         - 出图：需要支持 `v2 API` (2024.2.28日以后的后端版本)
-        - utils：需要支持 `v2 API` 
         - 用户数据：需要一个启用了**数据库**的后端，需要支持 `v2 API`
         
-        > 三个后端设置可以不同，默认全部设置为**公共后端**。
+        > 后端设置可以不同，默认全部设置为**公共后端**。
         
         ***
         
         
         <h2 align="center"> 测试与调用 </h2>
         
         
@@ -78,91 +68,64 @@
         - `handler` 是 `tsugu` 的一个同步函数，用于直接处理用户输入的自然语言并返回查询结果: 
         
         ```python
         import io
         import tsugu
         
         # 四个参数，分别意味着 消息内容 用户id 平台 频道id
-        for i in tsugu.handler('查卡 ars 1x', '1528593481', 'red', '666808414'):
-            # 字符串
-            print(i) if isinstance(i, str) else None
-            # 图片
-            print(f"[图像大小: {len(i) / 1024:.2f}KB]") if isinstance(i, bytes) else None
-            # from PIL import Image
-            # Image.open(io.BytesIO(i)).show() if isinstance(i, bytes) else None
+        for i in tsugu.handler(message='查卡 ars 1x', user_id='1528593481', platform='red', channel_id='666808414'):
+            print('文本: ',i) if isinstance(i, str) else None
+            print(f"[图片]") if isinstance(i, bytes) else None
         ```
         
         > 在常用的qqbot中，群号就是 `channel_id`。   
         > 当你使用QQ号作为 `user_id` 时，`platform` 可以填写 `red`。   
         
         
         - 异步框架下，可以使用 `run_in_executor` 方法:
+        > ~~未来会支持异步版本~~   
+        > run_in_executor 一辈子吧
         
-        > 以 lagrange-python 群聊为例，其他异步框架请自行查阅文档。
-        ```python
-        loop = asyncio.get_running_loop()
-        args = (event.msg, str(event.uin), 'red', str(event.grp_id))
-        response = await loop.run_in_executor(None, tsugu.handler, *args)
-        
-        # 不发送消息
-        if not response:
-            return
-        
-        msg_list = []
-        for item in response:
-            # 处理文本类型的消息
-            msg_list.append(Text(item)) if isinstance(item, str) else None
-            msg_list.append(await client.upload_grp_image(BytesIO(item), event.grp_id)) if isinstance(item, bytes) else None
-        
-        await client.send_grp_msg(msg_list, event.grp_id)
-        ```
-        
-        ## 调用 `tsugu.database`
+        ## 使用本地数据库
         
         ```py
         import tsugu
         
         tsugu.database(path="./data.db")
+        ```
         
         # 此操作会自动创建或使用本地数据库为 tsugu.bot 提供用户数据。
         # 远程数据库将不使用。
-        # 更多功能可能在未来版本中添加。
-        ```
+        
         > 注意，先进行此操作，后进行 `load_config_json` 操作，旧版本 `config.json` 会覆盖数据库路径，导致数据库无法使用。
         
         
-        ## 查看与更改 `tsugu.config` 配置
+        ## 使用配置文件
         
-        - 输出配置到 `config.json` 文件:
-        ```py
-        import tsugu
-        
-        tsugu.config.output_config_json('./config.json')
-        ```
-        
-        - 利用此文件，你可以更改配置项，然后重新加载配置:
         ```py
         import tsugu
         
         tsugu.config.load_config_json('./config.json')
         ```
+        > 如果不存在，会创建默认配置文件。
+        
+        > 注意，不清楚的配置项请不要更改，更改配置项可能会导致不可预知的错误。
         
         
         - 你也可以直接更改配置，但不推荐:   
         
         ```py
         import tsugu
         
         # 更改的后端地址。
         tsugu.config.backend = "http://127.0.0.0.1:3000"
         
         # 添加关闭抽卡模拟的群号。
         tsugu.config.ban_gacha_simulate_group_data = ["114514", "1919810"]
         ```
-        > 注意，不清楚的配置项请不要更改，更改配置项可能会导致不可预知的错误。
         
         
         
         
         ## 使用 `tsugu.router` 路由与内部方法
         
         - 如果想自己进行自然语言处理，你可以使用单独的路由:
@@ -196,28 +159,41 @@
         
         <h2 align="center"> 相对应登录端 </h2>
         
         | 部署方式 | 传送门 |
         | --- | --- |
         | **lpt 登陆端部署** | [![release](https://img.shields.io/github/v/release/kumoSleeping/lgr-tsugu-py?style=flat-square)](https://github.com/kumoSleeping/lgr-tsugu-py) |
         
-        基于 v2 api 的 `Go` + `Lagrange` 的登录端正由 [WindowsSov8](https://github.com/WindowsSov8forUs) 开发中，敬请期待。
-        基于 v2 api 的 `C#` + `Lagrange` 的登录端正由 [棱镜](https://github.com/DreamPrism) 开发中，敬请期待。   
-        基于本项目的 `NoneBot2` 插件也由 [zhaomaoniu](https://github.com/zhaomaoniu) 开发中，敬请期待。
-        
          <details>
         <summary><b>客服ano酱指导(这里可以点击)</b></summary>
          
         **注意，如果你不知道什么是BanGDream，请不要随意加群**    
         **本群还是欢迎加群的（**    
         [BanGDreamBot开发聊天群](https://qm.qq.com/q/zjUPQkrdpm)   
         温馨的聊天环境～   
         
         </details>
         
+        # 关于安装
+        
+        ## 更新
+        ```shell
+        pip install tsugu --upgrade
+        ```
+        
+        ## 使用官方源安装
+        ```shell
+        pip install tsugu --index-url https://pypi.org/simple/
+        ```
+        
+        ## 使用清华源安装(可能不能即使更新)
+        ```shell
+        pip install tsugu --index-url https://pypi.tuna.tsinghua.edu.cn/simple
+        ```
+        
         
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

#### html2text {}

```diff
@@ -1,83 +1,65 @@
-Metadata-Version: 2.1 Name: tsugu Version: 0.5.7 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.6.0 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
 - [x] èªç¶è¯­è¨è¾å¥ -> è¿åç»æ - [ ] ç¬ç«è·¯ç±è¾å¥ -
 > è¿åç»æ `é¨åæ¯æ` - [x] æ¬å°æ°æ®åº (sqlite3) - [x]
 è¿ç¨æ°æ®åº (å®¢æ·ç«¯) - [x] éç½®é¡¹
 (åºç¡éç½®ãä»£çãå½ä»¤å«å ç­)
-                          ********** ?å?®??è?£??ä?¸??æ??´?æ??° **********
-## å®è£ tsugu æ¨¡å ```shell pip install tsugu ``` ## æ´æ° ```shell pip
-install tsugu --upgrade ``` ## ä½¿ç¨å®æ¹æºå®è£ ```shell pip install tsugu
---index-url https://pypi.org/simple/ ``` ## åç«¯éæ± -
+                              ********** ?å?®??è?£? **********
+## å®è£ tsugu æ¨¡å ```shell pip install tsugu ``` ## åç«¯éæ± -
 åºå¾ï¼éè¦æ¯æ `v2 API` (2024.2.28æ¥ä»¥åçåç«¯çæ¬) -
-utilsï¼éè¦æ¯æ `v2 API` -
 ç¨æ·æ°æ®ï¼éè¦ä¸ä¸ªå¯ç¨äº**æ°æ®åº**çåç«¯ï¼éè¦æ¯æ `v2
-API` >
-ä¸ä¸ªåç«¯è®¾ç½®å¯ä»¥ä¸åï¼é»è®¤å¨é¨è®¾ç½®ä¸º**å¬å±åç«¯**ã ***
+API` > åç«¯è®¾ç½®å¯ä»¥ä¸åï¼é»è®¤å¨é¨è®¾ç½®ä¸º**å¬å±åç«¯**ã ***
                           ********** ?æ?µ??è?¯??ä?¸??è?°??ç??¨ **********
 ## è°ç¨ `tsugu.handler` - `handler` æ¯ `tsugu`
 çä¸ä¸ªåæ­¥å½æ°ï¼ç¨äºç´æ¥å¤çç¨æ·è¾å¥çèªç¶è¯­è¨å¹¶è¿åæ¥è¯¢ç»æ:
 ```python import io import tsugu # åä¸ªåæ°ï¼åå«æå³ç æ¶æ¯åå®¹
-ç¨æ·id å¹³å° é¢éid for i in tsugu.handler('æ¥å¡ ars 1x', '1528593481',
-'red', '666808414'): # å­ç¬¦ä¸² print(i) if isinstance(i, str) else None #
-å¾ç print(f"[å¾åå¤§å°: {len(i) / 1024:.2f}KB]") if isinstance(i, bytes)
-else None # from PIL import Image # Image.open(io.BytesIO(i)).show() if
-isinstance(i, bytes) else None ``` > å¨å¸¸ç¨çqqbotä¸­ï¼ç¾¤å·å°±æ¯
-`channel_id`ã > å½ä½ ä½¿ç¨QQå·ä½ä¸º `user_id` æ¶ï¼`platform`
-å¯ä»¥å¡«å `red`ã - å¼æ­¥æ¡æ¶ä¸ï¼å¯ä»¥ä½¿ç¨ `run_in_executor`
-æ¹æ³: > ä»¥ lagrange-python
-ç¾¤èä¸ºä¾ï¼å¶ä»å¼æ­¥æ¡æ¶è¯·èªè¡æ¥éææ¡£ã ```python loop =
-asyncio.get_running_loop() args = (event.msg, str(event.uin), 'red', str
-(event.grp_id)) response = await loop.run_in_executor(None, tsugu.handler,
-*args) # ä¸åéæ¶æ¯ if not response: return msg_list = [] for item in
-response: # å¤çææ¬ç±»åçæ¶æ¯ msg_list.append(Text(item)) if
-isinstance(item, str) else None msg_list.append(await client.upload_grp_image
-(BytesIO(item), event.grp_id)) if isinstance(item, bytes) else None await
-client.send_grp_msg(msg_list, event.grp_id) ``` ## è°ç¨ `tsugu.database`
-```py import tsugu tsugu.database(path="./data.db") #
+ç¨æ·id å¹³å° é¢éid for i in tsugu.handler(message='æ¥å¡ ars 1x',
+user_id='1528593481', platform='red', channel_id='666808414'): print('ææ¬:
+',i) if isinstance(i, str) else None print(f"[å¾ç]") if isinstance(i, bytes)
+else None ``` > å¨å¸¸ç¨çqqbotä¸­ï¼ç¾¤å·å°±æ¯ `channel_id`ã >
+å½ä½ ä½¿ç¨QQå·ä½ä¸º `user_id` æ¶ï¼`platform` å¯ä»¥å¡«å `red`ã -
+å¼æ­¥æ¡æ¶ä¸ï¼å¯ä»¥ä½¿ç¨ `run_in_executor` æ¹æ³: >
+~~æªæ¥ä¼æ¯æå¼æ­¥çæ¬~~ > run_in_executor ä¸è¾å­å§ ##
+ä½¿ç¨æ¬å°æ°æ®åº ```py import tsugu tsugu.database(path="./data.db") ``` #
 æ­¤æä½ä¼èªå¨åå»ºæä½¿ç¨æ¬å°æ°æ®åºä¸º tsugu.bot
-æä¾ç¨æ·æ°æ®ã # è¿ç¨æ°æ®åºå°ä¸ä½¿ç¨ã #
-æ´å¤åè½å¯è½å¨æªæ¥çæ¬ä¸­æ·»å ã ``` >
+æä¾ç¨æ·æ°æ®ã # è¿ç¨æ°æ®åºå°ä¸ä½¿ç¨ã >
 æ³¨æï¼åè¿è¡æ­¤æä½ï¼åè¿è¡ `load_config_json` æä½ï¼æ§çæ¬
 `config.json` ä¼è¦çæ°æ®åºè·¯å¾ï¼å¯¼è´æ°æ®åºæ æ³ä½¿ç¨ã ##
-æ¥çä¸æ´æ¹ `tsugu.config` éç½® - è¾åºéç½®å° `config.json` æä»¶:
-```py import tsugu tsugu.config.output_config_json('./config.json') ``` -
-å©ç¨æ­¤æä»¶ï¼ä½ å¯ä»¥æ´æ¹éç½®é¡¹ï¼ç¶åéæ°å è½½éç½®: ```py
-import tsugu tsugu.config.load_config_json('./config.json') ``` -
-ä½ ä¹å¯ä»¥ç´æ¥æ´æ¹éç½®ï¼ä½ä¸æ¨è: ```py import tsugu #
+ä½¿ç¨éç½®æä»¶ ```py import tsugu tsugu.config.load_config_json('./
+config.json') ``` > å¦æä¸å­å¨ï¼ä¼åå»ºé»è®¤éç½®æä»¶ã >
+æ³¨æï¼ä¸æ¸æ¥çéç½®é¡¹è¯·ä¸è¦æ´æ¹ï¼æ´æ¹éç½®é¡¹å¯è½ä¼å¯¼è´ä¸å¯é¢ç¥çéè¯¯ã
+- ä½ ä¹å¯ä»¥ç´æ¥æ´æ¹éç½®ï¼ä½ä¸æ¨è: ```py import tsugu #
 æ´æ¹çåç«¯å°åã tsugu.config.backend = "http://127.0.0.0.1:3000" #
 æ·»å å³é­æ½å¡æ¨¡æçç¾¤å·ã tsugu.config.ban_gacha_simulate_group_data
-= ["114514", "1919810"] ``` >
-æ³¨æï¼ä¸æ¸æ¥çéç½®é¡¹è¯·ä¸è¦æ´æ¹ï¼æ´æ¹éç½®é¡¹å¯è½ä¼å¯¼è´ä¸å¯é¢ç¥çéè¯¯ã
-## ä½¿ç¨ `tsugu.router` è·¯ç±ä¸åé¨æ¹æ³ -
+= ["114514", "1919810"] ``` ## ä½¿ç¨ `tsugu.router` è·¯ç±ä¸åé¨æ¹æ³ -
 å¦ææ³èªå·±è¿è¡èªç¶è¯­è¨å¤çï¼ä½ å¯ä»¥ä½¿ç¨åç¬çè·¯ç±: ```py
 import tsugu # è·åç¨æ·æ°æ® reply = tsugu.router.get_user_data("red",
 "1234567890") # æ¥å¡ reply = tsugu.router.card("çº¢ ksm", [0, 3], 5) #
 è®¾ç½®ç©å®¶è½¦çè½¬å reply = tsugu.router.set_car_forward("red",
 "1234567890", True) ``` -
 æ­¤å¤è¿æ´é²äºä¸äºåé¨æ¹æ³ï¼éè¦å¯ä»¥ä½¿ç¨: ```py import tsugu
 tsugu.interior_local_method.bind_player_verification("red", "1234567890", True)
 tsugu.interior_remote_method.bind_player_verification("red", "1234567890", 0,
 '1000011232', True) tsugu.interior_local_method.submit_car_number_msg("123456
 å¤§åq1", "1234567890", "red") ``` ***
                         ********** ?ç??¸?å?¯?¹?å?º??ç??»?å?½??ç?«?¯ **********
 | é¨ç½²æ¹å¼ | ä¼ éé¨ | | --- | --- | | **lpt ç»éç«¯é¨ç½²** | [!
 [release](https://img.shields.io/github/v/release/kumoSleeping/lgr-tsugu-
-py?style=flat-square)](https://github.com/kumoSleeping/lgr-tsugu-py) | åºäº
-v2 api ç `Go` + `Lagrange` çç»å½ç«¯æ­£ç± [WindowsSov8](https://
-github.com/WindowsSov8forUs) å¼åä¸­ï¼æ¬è¯·æå¾ã åºäº v2 api ç `C#`
-+ `Lagrange` çç»å½ç«¯æ­£ç± [æ£±é](https://github.com/DreamPrism)
-å¼åä¸­ï¼æ¬è¯·æå¾ã åºäºæ¬é¡¹ç®ç `NoneBot2` æä»¶ä¹ç±
-[zhaomaoniu](https://github.com/zhaomaoniu) å¼åä¸­ï¼æ¬è¯·æå¾ã
+py?style=flat-square)](https://github.com/kumoSleeping/lgr-tsugu-py) |
 ?å?®?¢?æ??aannoo?é??±?æ???å?¯?¼((?è?¿??é???å??¯?ä?»?¥?ç??¹?å??»))
 **æ³¨æï¼å¦æä½ ä¸ç¥éä»ä¹æ¯BanGDreamï¼è¯·ä¸è¦éæå ç¾¤**
 **æ¬ç¾¤è¿æ¯æ¬¢è¿å ç¾¤çï¼** [BanGDreamBotå¼åèå¤©ç¾¤](https://
-qm.qq.com/q/zjUPQkrdpm) æ¸©é¦¨çèå¤©ç¯å¢ï½ Platform: UNKNOWN Classifier:
-Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
-MIT License Classifier: Operating System :: OS Independent Requires-Python:
->=3.8 Description-Content-Type: text/markdown
+qm.qq.com/q/zjUPQkrdpm) æ¸©é¦¨çèå¤©ç¯å¢ï½ # å³äºå®è£ ## æ´æ°
+```shell pip install tsugu --upgrade ``` ## ä½¿ç¨å®æ¹æºå®è£ ```shell pip
+install tsugu --index-url https://pypi.org/simple/ ``` ## ä½¿ç¨æ¸åæºå®è£
+(å¯è½ä¸è½å³ä½¿æ´æ°) ```shell pip install tsugu --index-url https://
+pypi.tuna.tsinghua.edu.cn/simple ``` Platform: UNKNOWN Classifier: Programming
+Language :: Python :: 3.8 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Requires-Python: >=3.8
+Description-Content-Type: text/markdown
```

### Comparing `tsugu-0.5.7/README.md` & `tsugu-0.6.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -29,37 +29,27 @@
 - [x] 自然语言输入 -> 返回结果
 - [ ] 独立路由输入 -> 返回结果 `部分支持`
 - [x] 本地数据库 (sqlite3)
 - [x] 远程数据库 (客户端)
 - [x] 配置项 (基础配置、代理、命令别名 等)
 
 
-<h2 align="center"> 安装与更新 </h2>
+<h2 align="center"> 安装 </h2>
 
 ## 安装 tsugu 模块
 ```shell
 pip install tsugu
 ```
 
-## 更新
-```shell
-pip install tsugu --upgrade
-```
-
-## 使用官方源安装
-```shell
-pip install tsugu --index-url https://pypi.org/simple/
-```
 ## 后端需求
 
 - 出图：需要支持 `v2 API` (2024.2.28日以后的后端版本)
-- utils：需要支持 `v2 API` 
 - 用户数据：需要一个启用了**数据库**的后端，需要支持 `v2 API`
 
-> 三个后端设置可以不同，默认全部设置为**公共后端**。
+> 后端设置可以不同，默认全部设置为**公共后端**。
 
 ***
 
 
 <h2 align="center"> 测试与调用 </h2>
 
 
@@ -70,91 +60,64 @@
 - `handler` 是 `tsugu` 的一个同步函数，用于直接处理用户输入的自然语言并返回查询结果: 
 
 ```python
 import io
 import tsugu
 
 # 四个参数，分别意味着 消息内容 用户id 平台 频道id
-for i in tsugu.handler('查卡 ars 1x', '1528593481', 'red', '666808414'):
-    # 字符串
-    print(i) if isinstance(i, str) else None
-    # 图片
-    print(f"[图像大小: {len(i) / 1024:.2f}KB]") if isinstance(i, bytes) else None
-    # from PIL import Image
-    # Image.open(io.BytesIO(i)).show() if isinstance(i, bytes) else None
+for i in tsugu.handler(message='查卡 ars 1x', user_id='1528593481', platform='red', channel_id='666808414'):
+    print('文本: ',i) if isinstance(i, str) else None
+    print(f"[图片]") if isinstance(i, bytes) else None
 ```
 
 > 在常用的qqbot中，群号就是 `channel_id`。   
 > 当你使用QQ号作为 `user_id` 时，`platform` 可以填写 `red`。   
 
 
 - 异步框架下，可以使用 `run_in_executor` 方法:
+> ~~未来会支持异步版本~~   
+> run_in_executor 一辈子吧
 
-> 以 lagrange-python 群聊为例，其他异步框架请自行查阅文档。
-```python
-loop = asyncio.get_running_loop()
-args = (event.msg, str(event.uin), 'red', str(event.grp_id))
-response = await loop.run_in_executor(None, tsugu.handler, *args)
-
-# 不发送消息
-if not response:
-    return
-
-msg_list = []
-for item in response:
-    # 处理文本类型的消息
-    msg_list.append(Text(item)) if isinstance(item, str) else None
-    msg_list.append(await client.upload_grp_image(BytesIO(item), event.grp_id)) if isinstance(item, bytes) else None
-
-await client.send_grp_msg(msg_list, event.grp_id)
-```
-
-## 调用 `tsugu.database`
+## 使用本地数据库
 
 ```py
 import tsugu
 
 tsugu.database(path="./data.db")
+```
 
 # 此操作会自动创建或使用本地数据库为 tsugu.bot 提供用户数据。
 # 远程数据库将不使用。
-# 更多功能可能在未来版本中添加。
-```
+
 > 注意，先进行此操作，后进行 `load_config_json` 操作，旧版本 `config.json` 会覆盖数据库路径，导致数据库无法使用。
 
 
-## 查看与更改 `tsugu.config` 配置
+## 使用配置文件
 
-- 输出配置到 `config.json` 文件:
-```py
-import tsugu
-
-tsugu.config.output_config_json('./config.json')
-```
-
-- 利用此文件，你可以更改配置项，然后重新加载配置:
 ```py
 import tsugu
 
 tsugu.config.load_config_json('./config.json')
 ```
+> 如果不存在，会创建默认配置文件。
+
+> 注意，不清楚的配置项请不要更改，更改配置项可能会导致不可预知的错误。
 
 
 - 你也可以直接更改配置，但不推荐:   
 
 ```py
 import tsugu
 
 # 更改的后端地址。
 tsugu.config.backend = "http://127.0.0.0.1:3000"
 
 # 添加关闭抽卡模拟的群号。
 tsugu.config.ban_gacha_simulate_group_data = ["114514", "1919810"]
 ```
-> 注意，不清楚的配置项请不要更改，更改配置项可能会导致不可预知的错误。
 
 
 
 
 ## 使用 `tsugu.router` 路由与内部方法
 
 - 如果想自己进行自然语言处理，你可以使用单独的路由:
@@ -188,22 +151,35 @@
 
 <h2 align="center"> 相对应登录端 </h2>
 
 | 部署方式 | 传送门 |
 | --- | --- |
 | **lpt 登陆端部署** | [![release](https://img.shields.io/github/v/release/kumoSleeping/lgr-tsugu-py?style=flat-square)](https://github.com/kumoSleeping/lgr-tsugu-py) |
 
-基于 v2 api 的 `Go` + `Lagrange` 的登录端正由 [WindowsSov8](https://github.com/WindowsSov8forUs) 开发中，敬请期待。
-基于 v2 api 的 `C#` + `Lagrange` 的登录端正由 [棱镜](https://github.com/DreamPrism) 开发中，敬请期待。   
-基于本项目的 `NoneBot2` 插件也由 [zhaomaoniu](https://github.com/zhaomaoniu) 开发中，敬请期待。
-
  <details>
 <summary><b>客服ano酱指导(这里可以点击)</b></summary>
  
 **注意，如果你不知道什么是BanGDream，请不要随意加群**    
 **本群还是欢迎加群的（**    
 [BanGDreamBot开发聊天群](https://qm.qq.com/q/zjUPQkrdpm)   
 温馨的聊天环境～   
 
 </details>
 
+# 关于安装
+
+## 更新
+```shell
+pip install tsugu --upgrade
+```
+
+## 使用官方源安装
+```shell
+pip install tsugu --index-url https://pypi.org/simple/
+```
+
+## 使用清华源安装(可能不能即使更新)
+```shell
+pip install tsugu --index-url https://pypi.tuna.tsinghua.edu.cn/simple
+```
+
```

#### html2text {}

```diff
@@ -3,75 +3,57 @@
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
 - [x] èªç¶è¯­è¨è¾å¥ -> è¿åç»æ - [ ] ç¬ç«è·¯ç±è¾å¥ -
 > è¿åç»æ `é¨åæ¯æ` - [x] æ¬å°æ°æ®åº (sqlite3) - [x]
 è¿ç¨æ°æ®åº (å®¢æ·ç«¯) - [x] éç½®é¡¹
 (åºç¡éç½®ãä»£çãå½ä»¤å«å ç­)
-                          ********** ?å?®??è?£??ä?¸??æ??´?æ??° **********
-## å®è£ tsugu æ¨¡å ```shell pip install tsugu ``` ## æ´æ° ```shell pip
-install tsugu --upgrade ``` ## ä½¿ç¨å®æ¹æºå®è£ ```shell pip install tsugu
---index-url https://pypi.org/simple/ ``` ## åç«¯éæ± -
+                              ********** ?å?®??è?£? **********
+## å®è£ tsugu æ¨¡å ```shell pip install tsugu ``` ## åç«¯éæ± -
 åºå¾ï¼éè¦æ¯æ `v2 API` (2024.2.28æ¥ä»¥åçåç«¯çæ¬) -
-utilsï¼éè¦æ¯æ `v2 API` -
 ç¨æ·æ°æ®ï¼éè¦ä¸ä¸ªå¯ç¨äº**æ°æ®åº**çåç«¯ï¼éè¦æ¯æ `v2
-API` >
-ä¸ä¸ªåç«¯è®¾ç½®å¯ä»¥ä¸åï¼é»è®¤å¨é¨è®¾ç½®ä¸º**å¬å±åç«¯**ã ***
+API` > åç«¯è®¾ç½®å¯ä»¥ä¸åï¼é»è®¤å¨é¨è®¾ç½®ä¸º**å¬å±åç«¯**ã ***
                           ********** ?æ?µ??è?¯??ä?¸??è?°??ç??¨ **********
 ## è°ç¨ `tsugu.handler` - `handler` æ¯ `tsugu`
 çä¸ä¸ªåæ­¥å½æ°ï¼ç¨äºç´æ¥å¤çç¨æ·è¾å¥çèªç¶è¯­è¨å¹¶è¿åæ¥è¯¢ç»æ:
 ```python import io import tsugu # åä¸ªåæ°ï¼åå«æå³ç æ¶æ¯åå®¹
-ç¨æ·id å¹³å° é¢éid for i in tsugu.handler('æ¥å¡ ars 1x', '1528593481',
-'red', '666808414'): # å­ç¬¦ä¸² print(i) if isinstance(i, str) else None #
-å¾ç print(f"[å¾åå¤§å°: {len(i) / 1024:.2f}KB]") if isinstance(i, bytes)
-else None # from PIL import Image # Image.open(io.BytesIO(i)).show() if
-isinstance(i, bytes) else None ``` > å¨å¸¸ç¨çqqbotä¸­ï¼ç¾¤å·å°±æ¯
-`channel_id`ã > å½ä½ ä½¿ç¨QQå·ä½ä¸º `user_id` æ¶ï¼`platform`
-å¯ä»¥å¡«å `red`ã - å¼æ­¥æ¡æ¶ä¸ï¼å¯ä»¥ä½¿ç¨ `run_in_executor`
-æ¹æ³: > ä»¥ lagrange-python
-ç¾¤èä¸ºä¾ï¼å¶ä»å¼æ­¥æ¡æ¶è¯·èªè¡æ¥éææ¡£ã ```python loop =
-asyncio.get_running_loop() args = (event.msg, str(event.uin), 'red', str
-(event.grp_id)) response = await loop.run_in_executor(None, tsugu.handler,
-*args) # ä¸åéæ¶æ¯ if not response: return msg_list = [] for item in
-response: # å¤çææ¬ç±»åçæ¶æ¯ msg_list.append(Text(item)) if
-isinstance(item, str) else None msg_list.append(await client.upload_grp_image
-(BytesIO(item), event.grp_id)) if isinstance(item, bytes) else None await
-client.send_grp_msg(msg_list, event.grp_id) ``` ## è°ç¨ `tsugu.database`
-```py import tsugu tsugu.database(path="./data.db") #
+ç¨æ·id å¹³å° é¢éid for i in tsugu.handler(message='æ¥å¡ ars 1x',
+user_id='1528593481', platform='red', channel_id='666808414'): print('ææ¬:
+',i) if isinstance(i, str) else None print(f"[å¾ç]") if isinstance(i, bytes)
+else None ``` > å¨å¸¸ç¨çqqbotä¸­ï¼ç¾¤å·å°±æ¯ `channel_id`ã >
+å½ä½ ä½¿ç¨QQå·ä½ä¸º `user_id` æ¶ï¼`platform` å¯ä»¥å¡«å `red`ã -
+å¼æ­¥æ¡æ¶ä¸ï¼å¯ä»¥ä½¿ç¨ `run_in_executor` æ¹æ³: >
+~~æªæ¥ä¼æ¯æå¼æ­¥çæ¬~~ > run_in_executor ä¸è¾å­å§ ##
+ä½¿ç¨æ¬å°æ°æ®åº ```py import tsugu tsugu.database(path="./data.db") ``` #
 æ­¤æä½ä¼èªå¨åå»ºæä½¿ç¨æ¬å°æ°æ®åºä¸º tsugu.bot
-æä¾ç¨æ·æ°æ®ã # è¿ç¨æ°æ®åºå°ä¸ä½¿ç¨ã #
-æ´å¤åè½å¯è½å¨æªæ¥çæ¬ä¸­æ·»å ã ``` >
+æä¾ç¨æ·æ°æ®ã # è¿ç¨æ°æ®åºå°ä¸ä½¿ç¨ã >
 æ³¨æï¼åè¿è¡æ­¤æä½ï¼åè¿è¡ `load_config_json` æä½ï¼æ§çæ¬
 `config.json` ä¼è¦çæ°æ®åºè·¯å¾ï¼å¯¼è´æ°æ®åºæ æ³ä½¿ç¨ã ##
-æ¥çä¸æ´æ¹ `tsugu.config` éç½® - è¾åºéç½®å° `config.json` æä»¶:
-```py import tsugu tsugu.config.output_config_json('./config.json') ``` -
-å©ç¨æ­¤æä»¶ï¼ä½ å¯ä»¥æ´æ¹éç½®é¡¹ï¼ç¶åéæ°å è½½éç½®: ```py
-import tsugu tsugu.config.load_config_json('./config.json') ``` -
-ä½ ä¹å¯ä»¥ç´æ¥æ´æ¹éç½®ï¼ä½ä¸æ¨è: ```py import tsugu #
+ä½¿ç¨éç½®æä»¶ ```py import tsugu tsugu.config.load_config_json('./
+config.json') ``` > å¦æä¸å­å¨ï¼ä¼åå»ºé»è®¤éç½®æä»¶ã >
+æ³¨æï¼ä¸æ¸æ¥çéç½®é¡¹è¯·ä¸è¦æ´æ¹ï¼æ´æ¹éç½®é¡¹å¯è½ä¼å¯¼è´ä¸å¯é¢ç¥çéè¯¯ã
+- ä½ ä¹å¯ä»¥ç´æ¥æ´æ¹éç½®ï¼ä½ä¸æ¨è: ```py import tsugu #
 æ´æ¹çåç«¯å°åã tsugu.config.backend = "http://127.0.0.0.1:3000" #
 æ·»å å³é­æ½å¡æ¨¡æçç¾¤å·ã tsugu.config.ban_gacha_simulate_group_data
-= ["114514", "1919810"] ``` >
-æ³¨æï¼ä¸æ¸æ¥çéç½®é¡¹è¯·ä¸è¦æ´æ¹ï¼æ´æ¹éç½®é¡¹å¯è½ä¼å¯¼è´ä¸å¯é¢ç¥çéè¯¯ã
-## ä½¿ç¨ `tsugu.router` è·¯ç±ä¸åé¨æ¹æ³ -
+= ["114514", "1919810"] ``` ## ä½¿ç¨ `tsugu.router` è·¯ç±ä¸åé¨æ¹æ³ -
 å¦ææ³èªå·±è¿è¡èªç¶è¯­è¨å¤çï¼ä½ å¯ä»¥ä½¿ç¨åç¬çè·¯ç±: ```py
 import tsugu # è·åç¨æ·æ°æ® reply = tsugu.router.get_user_data("red",
 "1234567890") # æ¥å¡ reply = tsugu.router.card("çº¢ ksm", [0, 3], 5) #
 è®¾ç½®ç©å®¶è½¦çè½¬å reply = tsugu.router.set_car_forward("red",
 "1234567890", True) ``` -
 æ­¤å¤è¿æ´é²äºä¸äºåé¨æ¹æ³ï¼éè¦å¯ä»¥ä½¿ç¨: ```py import tsugu
 tsugu.interior_local_method.bind_player_verification("red", "1234567890", True)
 tsugu.interior_remote_method.bind_player_verification("red", "1234567890", 0,
 '1000011232', True) tsugu.interior_local_method.submit_car_number_msg("123456
 å¤§åq1", "1234567890", "red") ``` ***
                         ********** ?ç??¸?å?¯?¹?å?º??ç??»?å?½??ç?«?¯ **********
 | é¨ç½²æ¹å¼ | ä¼ éé¨ | | --- | --- | | **lpt ç»éç«¯é¨ç½²** | [!
 [release](https://img.shields.io/github/v/release/kumoSleeping/lgr-tsugu-
-py?style=flat-square)](https://github.com/kumoSleeping/lgr-tsugu-py) | åºäº
-v2 api ç `Go` + `Lagrange` çç»å½ç«¯æ­£ç± [WindowsSov8](https://
-github.com/WindowsSov8forUs) å¼åä¸­ï¼æ¬è¯·æå¾ã åºäº v2 api ç `C#`
-+ `Lagrange` çç»å½ç«¯æ­£ç± [æ£±é](https://github.com/DreamPrism)
-å¼åä¸­ï¼æ¬è¯·æå¾ã åºäºæ¬é¡¹ç®ç `NoneBot2` æä»¶ä¹ç±
-[zhaomaoniu](https://github.com/zhaomaoniu) å¼åä¸­ï¼æ¬è¯·æå¾ã
+py?style=flat-square)](https://github.com/kumoSleeping/lgr-tsugu-py) |
 ?å?®?¢?æ??aannoo?é??±?æ???å?¯?¼((?è?¿??é???å??¯?ä?»?¥?ç??¹?å??»))
 **æ³¨æï¼å¦æä½ ä¸ç¥éä»ä¹æ¯BanGDreamï¼è¯·ä¸è¦éæå ç¾¤**
 **æ¬ç¾¤è¿æ¯æ¬¢è¿å ç¾¤çï¼** [BanGDreamBotå¼åèå¤©ç¾¤](https://
-qm.qq.com/q/zjUPQkrdpm) æ¸©é¦¨çèå¤©ç¯å¢ï½
+qm.qq.com/q/zjUPQkrdpm) æ¸©é¦¨çèå¤©ç¯å¢ï½ # å³äºå®è£ ## æ´æ°
+```shell pip install tsugu --upgrade ``` ## ä½¿ç¨å®æ¹æºå®è£ ```shell pip
+install tsugu --index-url https://pypi.org/simple/ ``` ## ä½¿ç¨æ¸åæºå®è£
+(å¯è½ä¸è½å³ä½¿æ´æ°) ```shell pip install tsugu --index-url https://
+pypi.tuna.tsinghua.edu.cn/simple ```
```

### Comparing `tsugu-0.5.7/setup.py` & `tsugu-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='0.5.7',
+    version='0.6.0',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py',
```

### Comparing `tsugu-0.5.7/test/test_main.py` & `tsugu-0.6.0/test/test_main.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.5.7/tsugu/router.py` & `tsugu-0.6.0/tsugu/router.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import List, Union
-from .utils import *
+from .universal_utils import v2api_from_backend, help_command
+from . import local
+from . import remote
 
 
 class Router:
     def __init__(self):
         pass
 
     @staticmethod
@@ -72,71 +74,71 @@
 
 class InteriorLocal:
     def __init__(self):
         pass
 
     @staticmethod
     def bind_player_request(platform: str, user_id: str):
-        return bind_player_request(platform, user_id)
+        return local.utils.bind_player_request(platform, user_id)
 
     @staticmethod
     def bind_player_verification(platform: str, user_id: str, server: int, player_id: str, status: bool):
-        return bind_player_verification(platform, user_id, server, player_id, status)
+        return local.utils.bind_player_verification(platform, user_id, server, player_id, status)
 
     @staticmethod
     def set_car_forward(platform: str, user_id: str, status: bool):
-        return set_car_forward(platform, user_id, status)
+        return local.utils.set_car_forward(platform, user_id, status)
 
     @staticmethod
     def set_default_server(platform: str, user_id: str, text: str):
-        return set_default_server(platform, user_id, text)
+        return local.utils.set_default_server(platform, user_id, text)
 
     @staticmethod
     def set_server_mode(platform: str, user_id: str, text: str):
-        return set_server_mode(platform, user_id, text)
+        return local.utils.set_server_mode(platform, user_id, text)
 
     @staticmethod
     def get_user_data(platform: str, user_id: str):
-        return get_user_data(platform, user_id)
+        return local.utils.get_user_data(platform, user_id)
 
     @staticmethod
     def submit_car_number_msg(message: str, user_id: str, platform: Union[str, None] = None):
-        return submit_car_number_msg(message, user_id, platform)
+        return local.utils.submit_car_number_msg(message, user_id, platform)
 
 
 interior_local_method = InteriorLocal()
 
 
 class InteriorRemote:
     def __init__(self):
         pass
 
     @staticmethod
     def bind_player_request(platform: str, user_id: str):
-        return Remote.bind_player_request(platform, user_id)
+        return remote.utils.bind_player_request(platform, user_id)
 
     @staticmethod
     def bind_player_verification(platform: str, user_id: str, server: int, player_id: str, status: bool):
-        return Remote.bind_player_verification(platform, user_id, server, player_id, status)
+        return remote.utils.bind_player_verification(platform, user_id, server, player_id, status)
 
     @staticmethod
     def set_car_forward(platform: str, user_id: str, status: bool):
-        return Remote.set_car_forward(platform, user_id, status)
+        return remote.utils.set_car_forward(platform, user_id, status)
 
     @staticmethod
     def set_default_server(platform: str, user_id: str, text: str):
-        return Remote.set_default_server(platform, user_id, text)
+        return remote.utils.set_default_server(platform, user_id, text)
 
     @staticmethod
     def set_server_mode(platform: str, user_id: str, text: str):
-        return Remote.set_server_mode(platform, user_id, text)
+        return remote.utils.set_server_mode(platform, user_id, text)
 
     @staticmethod
     def get_user_data(platform: str, user_id: str):
-        return Remote.get_user_data(platform, user_id)
+        return remote.utils.get_user_data(platform, user_id)
 
     @staticmethod
     def submit_car_number_msg(message: str, user_id: str, platform: Union[str, None] = None):
-        return submit_car_number_msg(message, user_id, platform)
+        return remote.utils.submit_car_number_msg(message, user_id, platform)
 
 
 interior_remote_method = InteriorRemote()
```

### Comparing `tsugu-0.5.7/tsugu/utils.py` & `tsugu-0.6.0/tsugu/local/utils/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,39 @@
-from typing import List
-import re
-import json
-import sqlite3
 import os
 import sys
+import sqlite3
+from loguru import logger
+import json
 import random
 import urllib3
-from urllib3.exceptions import HTTPError
-from loguru import logger
+import re
+
+from ...universal_utils import config
+from ...universal_utils import text_response, convert_server_names_to_indices, query_server_info, server_exists
+from ...universal_utils import v2api_from_backend
 
-from .config import config
+
+def v2_api_command(message, command_matched, api, platform, user_id, channel_id):
+    text = message[len(command_matched):].strip()
+
+    if api in ['cardIllustration', 'ycm']:  # 无需验证server信息
+        return v2api_from_backend(api, text)
+
+    if api == 'gachaSimulate':
+        if channel_id in config.ban_gacha_simulate_group_data:
+            return text_response('此群禁止使用模拟抽卡功能')
+
+    # 获取用户数据
+    user_data = get_user_data(platform, user_id)
+    try:
+        if user_data['status'] != 'success':
+            return text_response('获取用户数据失败：内部错误')
+        return v2api_from_backend(api, text, user_data['data']['default_server'], user_data['data']['server_mode'])
+    except Exception as e:
+        return text_response('获取用户数据失败：数据库错误')
 
 
 class DatabaseManager:
     def __init__(self, path):
         self.path = path
         self.conn = None
         self.cursor = None
@@ -50,208 +70,30 @@
         if self.cursor:
             self.cursor.execute(query)
             return self.cursor.fetchall()
         else:
             return []
 
 
-db_manager = DatabaseManager(config.user_database_path)
+db_manager = DatabaseManager(config._user_database_path)
 
 
-def database(path: str | None = None):
+def database(path: str = None):
     '''
-    初始化数据库
+    启用本地用户数据库，同时不再使用远程数据库
+    本地数据库不存在时自动创建
+    :param path: 数据库文件路径
     :return:
     '''
     if not path:
         path = (os.path.dirname(sys.modules['__main__'].__file__))
-    config.user_database_path = path
+    config._user_database_path = path
     db_manager.init_db(path)
 
 
-def text_response(string):
-    return [{"type": "string", "string": string}]
-
-
-def convert_server_names_to_indices(server_names: str) -> list:
-    indices_list = [config.server_name_to_index.get(name, "Unknown") for name in server_names.split(" ")]
-    result = [index for index in indices_list if index != "Unknown"]
-    # 转化成数字，例如 ["0", "1"] -> [0, 1]
-    return [int(i) for i in result]
-
-
-def query_server_info(server_name: str) -> int:
-    server = convert_server_names_to_indices(server_name)[0] if convert_server_names_to_indices(server_name) else None
-    return server
-
-
-def server_exists(server):
-    if server or server == 0:
-        return True
-    return False
-
-
-def requests_post_for_user(url, data):
-    if config.user_data_backend_use_proxy:
-        http = urllib3.ProxyManager(config.proxy_url, cert_reqs='CERT_NONE')
-    else:
-        http = urllib3.PoolManager(cert_reqs='CERT_NONE')
-    try:
-        response = http.request('POST', url, headers={'Content-Type': 'application/json'}, body=json.dumps(data))
-        # 检查响应的状态码是否为 200
-        if response.status == 200:
-            return json.loads(response.data.decode('utf-8'))
-        elif response.status == 400:
-            return json.loads(response.data.decode('utf-8'))
-        else:
-            # 处理其他状态码
-            return {"status": "error", "message": "服务器出现了问题，请稍后再试。"}
-
-    except HTTPError as http_err:
-        logger.error(f'HTTP 错误：{http_err}')
-        return {"status": "error", "message": "服务器出现了问题，请稍后再试。"}
-
-    except Exception as e:
-        logger.error(f'发生异常：{e}')
-        return {"status": "error", "message": "发生了未知错误。"}
-
-
-def requests_post_for_backend(url, data):
-    if config.backend_use_proxy:
-        http = urllib3.ProxyManager(config.proxy_url, cert_reqs='CERT_NONE')
-    else:
-        http = urllib3.PoolManager(cert_reqs='CERT_NONE')
-    try:
-        response = http.request('POST', url, headers={'Content-Type': 'application/json'}, body=json.dumps(data))
-
-        # 检查响应的状态码是否为 200
-        if response.status == 200:
-            return json.loads(response.data.decode('utf-8'))
-        else:
-            # 处理其他状态码
-            return text_response("服务器出现了问题，请稍后再试。")
-
-    except HTTPError as http_err:
-        logger.error(f'HTTP 错误：{http_err}')
-        return text_response("服务器出现了问题，请稍后再试。")
-
-    except Exception as e:
-        logger.error(f'发生异常：{e}')
-        return text_response("发生了未知错误。")
-
-
-def v2api_from_backend(api, text, default_servers: List[int] = None, server=3):
-    if default_servers is None:
-        default_servers = [3, 0]
-    path = f"/v2/{api}"
-    data = {
-        "default_servers": default_servers,
-        "server": server,
-        "text": text,
-        "useEasyBG": config.use_easy_bg,
-        "compress": config.compress
-    }
-    res = requests_post_for_backend(f"{config.backend}{path}", data)
-    return res
-
-
-def v2_api_command(message, command_matched, api, platform, user_id, channel_id):
-    text = message[len(command_matched):].strip()
-
-    if api in ['cardIllustration', 'ycm']:  # 无需验证server信息
-        return v2api_from_backend(api, text)
-
-    if api == 'gachaSimulate':
-        if channel_id in config.ban_gacha_simulate_group_data:
-            return text_response('此群禁止使用模拟抽卡功能')
-
-    # 获取用户数据
-    import logging
-    logging.debug(config.user_database_path)
-    user_data = get_user_data(platform, user_id) if config.user_database_path else Remote.get_user_data(platform, user_id)
-    try:
-        if user_data['status'] != 'success':
-            return text_response('获取用户数据失败：内部错误')
-        return v2api_from_backend(api, text, user_data['data']['default_server'], user_data['data']['server_mode'])
-    except Exception as e:
-        return text_response('获取用户数据失败：网络 / 前端错误')
-
-
-def submit_car_number_msg(message, user_id, platform=None):
-    # 检查car_config['car']中的关键字
-    for keyword in config.car_config["car"]:
-        if str(keyword) in message:
-            break
-    else:
-        return False
-    # 检查car_config['fake']中的关键字
-    for keyword in config.car_config["fake"]:
-        if str(keyword) in message:
-            return False
-    pattern = r"^\d{5}(\D|$)|^\d{6}(\D|$)"
-    if not re.match(pattern, message):
-        return False
-
-    # 获取用户数据
-    try:
-        if platform:
-            user_data = get_user_data(platform, user_id) if config.user_database_path else Remote.get_user_data(platform, user_id)
-            if not user_data['data']['car']:
-                return True
-    except Exception as e:
-        logger.error('unknown user')
-        # 默认不开启关闭车牌，继续提交
-        pass
-
-    try:
-        car_id = message[:6]
-        if not car_id.isdigit() and car_id[:5].isdigit():
-            car_id = car_id[:5]
-
-        # 构建 URL
-        url = f"https://api.bandoristation.com/index.php?function=submit_room_number&number={car_id}&user_id={user_id}&raw_message={message}&source={config.token_name}&token={config.bandori_station_token}"
-
-        if config.submit_car_number_use_proxy:
-            http = urllib3.ProxyManager(config.proxy_url, cert_reqs='CERT_NONE')
-        else:
-            http = urllib3.PoolManager(cert_reqs='CERT_NONE')
-
-        # 发送请求
-        response = http.request('GET', url)
-
-        # 检查响应的状态码是否为 200
-        if response.status == 200:
-            return True
-        else:
-            logger.error(f"[Tsugu] 提交车牌失败，HTTP响应码: {response.status}")
-            return True  # 虽然提交失败，但是确定了是车牌消息
-
-    except Exception as e:
-        logger.error(f"[Tsugu] 发生异常: {e}")
-        return True  # 虽然提交失败，但是确定了是车牌消息
-
-
-def match_command(message, cmd_dict):
-    for command, api_value in cmd_dict.items():
-        if message.startswith(command):
-            return command, api_value
-    return None, None
-
-
-def load_commands_from_config(data):
-    # 初始化一个空字典来存储命令到操作的映射
-    cmd_dict = {}
-    for item in data:
-        api = item['api']
-        for command_name in item['command_name']:
-            cmd_dict[command_name] = api
-    return cmd_dict
-
-
-
 def get_user_data(platform: str, user_id: str):
 
     cursor = db_manager.conn.cursor()
     cursor.execute("SELECT * FROM users WHERE user_id = ? AND platform = ?", (user_id, platform))
     row = cursor.fetchone()
 
     if row:
@@ -297,20 +139,20 @@
         # 先查找默认服务器对应的记录
         server: int = user_data['data']['server_mode']
         for i in game_ids:
             if i.get("server") == server:
                 player_id = str(i.get("game_id"))
                 server = int(i.get("server"))
 
-                text = f'已查找默认服务器 {config.server_index_to_name[str(server)]} 的记录'
+                text = f'已查找默认服务器 {config._server_index_to_name[str(server)]} 的记录'
                 break
         else:
             # 再查找第一个记录
             if game_ids:
-                return text_response(f'未在 {len(game_ids)} 条记录中找到 {config.server_index_to_name[str(server)]} 的记录')
+                return text_response(f'未在 {len(game_ids)} 条记录中找到 {config._server_index_to_name[str(server)]} 的记录')
             else:
                 pass  # 前面已经判断过了没绑定任何的情况
     elif isinstance(args, int):
         # 查找对应数字的记录
         if args == 0:
             return text_response('哪来的0（')
         if args > len(game_ids) or args < 1:
@@ -322,15 +164,15 @@
 
     elif isinstance(args, str):
         server = query_server_info(args)
         # 查找对应服务器的记录
         for i in game_ids:
             if i.get("server") == server:
                 player_id = str(i.get("game_id"))
-                text = f'已查找服务器 {config.server_index_to_name[str(server)]} 的记录'
+                text = f'已查找服务器 {config._server_index_to_name[str(server)]} 的记录'
                 break
         else:
             return text_response(f'未找到记录，请检查是否绑定过此服务器')
     else:
         return text_response('参数错误，的服务器可能不合法')
     result: list = v2api_from_backend('player', player_id, server=server)
     new_item = {"type": "string", "string": text}
@@ -424,15 +266,15 @@
     if verify_code == "" or not verify_code:
         return text_response('请先获取验证代码')
     # 检测重复性
     game_ids = json.loads(user_data['data']['game_ids'])
     for i in game_ids:
         if i.get("game_id") == player_id and i.get("server") == server:
             return text_response('请勿重复绑定')
-    server_s_name = config.server_index_to_s_name[str(server)]
+    server_s_name = config._server_index_to_s_name[str(server)]
 
     # 构建 URL
     url = f'https://bestdori.com/api/player/{server_s_name}/{player_id}?mode=2'
     if config.verify_player_bind_use_proxy:
         http = urllib3.ProxyManager(config.proxy_url, cert_reqs='CERT_NONE')
     else:
         http = urllib3.PoolManager(cert_reqs='CERT_NONE')
@@ -490,98 +332,62 @@
             cursor.execute("UPDATE users SET game_ids = ? WHERE user_id = ? AND platform = ?", (updated_game_ids_json, user_id, platform))
             db_manager.conn.commit()
             return text_response('解绑成功喵')
         return text_response(f'解绑失败，当前有 {record} 个记录，发送"解除绑定 {record}"来获解除第{record}个记录，以此类推')
     return text_response('解绑失败，请检查输入是否正确')
 
 
-def help_command(command_name=None):
-    if not command_name:
-        # 读取 config.help_doc_dict 中的所有键
-        command_list = list(config.help_doc_dict.keys())
-        command_list.sort()
-        print(command_list)
-        return text_response(f'当前支持的命令有：\n{", ".join(command_list)}\n 请使用"help 命令名"来查看命令的详细帮助')
+def submit_car_number_msg(message, user_id, platform=None):
+    # 检查car_config['car']中的关键字
+    for keyword in config.car_config["car"]:
+        if str(keyword) in message:
+            break
     else:
-        # 读取 config.help_doc_dict 中的指定键
-        help_text = config.help_doc_dict.get(command_name)
-        if help_text:
-            return text_response(help_text)
-        return None
+        return False
+    # 检查car_config['fake']中的关键字
+    for keyword in config.car_config["fake"]:
+        if str(keyword) in message:
+            return False
+    pattern = r"^\d{5}(\D|$)|^\d{6}(\D|$)"
+    if not re.match(pattern, message):
+        return False
 
+    # 获取用户数据
+    try:
+        if platform:
+            user_data = get_user_data(platform, user_id)
+            if not user_data['data']['car']:
+                return True
+    except Exception as e:
+        logger.error('unknown user')
+        # 默认不开启关闭车牌，继续提交
+        pass
 
-class Remote:
-    @staticmethod
-    def get_user_data(platform: str, user_id: str):
-        data = {
-            'platform': platform,
-            'user_id': user_id
-        }
-        result = requests_post_for_user(f"{config.user_data_backend}/user/getUserData", data)
-        return result
+    try:
+        car_id = message[:6]
+        if not car_id.isdigit() and car_id[:5].isdigit():
+            car_id = car_id[:5]
 
-    @staticmethod
-    def bind_player_request(platform: str, user_id: str, server: int, bind_type: bool):
-        data = {
-            'platform': platform,
-            'user_id': user_id,
-            'server': server,
-            'bindType': bind_type  # 布尔，表示绑定还是解绑
-        }
-        result = requests_post_for_user(f"{config.user_data_backend}/user/bindPlayerRequest", data)
-        return result
+        # 构建 URL
+        url = f"https://api.bandoristation.com/index.php?function=submit_room_number&number={car_id}&user_id={user_id}&raw_message={message}&source={config.token_name}&token={config.bandori_station_token}"
 
-    @staticmethod
-    def bind_player_verification(platform: str, user_id: str, server: int, player_id: str, bind_type: bool):
-        data = {
-            'platform': platform,
-            'user_id': user_id,
-            'server': server,
-            'playerId': player_id,
-            'bindType': bind_type  # 布尔，表示绑定还是解绑
-        }
-        result = requests_post_for_user(f"{config.user_data_backend}/user/bindPlayerVerification", data)
-        return result
+        if config.submit_car_number_use_proxy:
+            http = urllib3.ProxyManager(config.proxy_url, cert_reqs='CERT_NONE')
+        else:
+            http = urllib3.PoolManager(cert_reqs='CERT_NONE')
 
-    @staticmethod
-    def player_status(user_id, platform, server=None):
-        user_data = Remote.get_user_data(platform, user_id)
-        if user_data['status'] != 'success':
-            return text_response('获取用户数据失败')
-        if server is None:
-            server = user_data['data']['server_mode']
-        player_id = user_data['data']['server_list'][server]['playerId']
-        if player_id == 0:
-            return text_response(f'未绑定玩家，请使用 绑定玩家 进行绑定')
-        return v2api_from_backend('player', str(player_id), server=server)
+        # 发送请求
+        response = http.request('GET', url)
 
-    @staticmethod
-    def set_car_forward(platform, user_id, status):
-        data = {
-            'platform': platform,
-            'user_id': user_id,
-            'status': status
-        }
-        result = requests_post_for_user(f"{config.user_data_backend}/user/changeUserData/setCarForwarding", data)
-        return result
+        # 检查响应的状态码是否为 200
+        if response.status == 200:
+            return True
+        else:
+            logger.error(f"[Tsugu] 提交车牌失败，HTTP响应码: {response.status}")
+            return True  # 虽然提交失败，但是确定了是车牌消息
 
-    @staticmethod
-    def set_default_server(platform, user_id, text):
-        data = {
-            'platform': platform,
-            'user_id': user_id,
-            'text': text
-        }
-        result = requests_post_for_user(f"{config.user_data_backend}/user/changeUserData/setDefaultServer", data)
-        return result
+    except Exception as e:
+        logger.error(f"[Tsugu] 发生异常: {e}")
+        return True  # 虽然提交失败，但是确定了是车牌消息
 
-    @staticmethod
-    def set_server_mode(platform, user_id, text):
-        data = {
-            'platform': platform,
-            'user_id': user_id,
-            'text': text
-        }
-        result = requests_post_for_user(f"{config.user_data_backend}/user/changeUserData/setServerMode", data)
-        return result
```

### Comparing `tsugu-0.5.7/tsugu.egg-info/PKG-INFO` & `tsugu-0.6.0/tsugu.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.5.7
+Version: 0.6.0
 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py
 Author: kumoSleeping
 Author-email: zjr2992@outlook.com
 License: MIT
 Description: 
         <h1 align="center"> Tsugu Python Frontend <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
@@ -37,37 +37,27 @@
         - [x] 自然语言输入 -> 返回结果
         - [ ] 独立路由输入 -> 返回结果 `部分支持`
         - [x] 本地数据库 (sqlite3)
         - [x] 远程数据库 (客户端)
         - [x] 配置项 (基础配置、代理、命令别名 等)
         
         
-        <h2 align="center"> 安装与更新 </h2>
+        <h2 align="center"> 安装 </h2>
         
         ## 安装 tsugu 模块
         ```shell
         pip install tsugu
         ```
         
-        ## 更新
-        ```shell
-        pip install tsugu --upgrade
-        ```
-        
-        ## 使用官方源安装
-        ```shell
-        pip install tsugu --index-url https://pypi.org/simple/
-        ```
         ## 后端需求
         
         - 出图：需要支持 `v2 API` (2024.2.28日以后的后端版本)
-        - utils：需要支持 `v2 API` 
         - 用户数据：需要一个启用了**数据库**的后端，需要支持 `v2 API`
         
-        > 三个后端设置可以不同，默认全部设置为**公共后端**。
+        > 后端设置可以不同，默认全部设置为**公共后端**。
         
         ***
         
         
         <h2 align="center"> 测试与调用 </h2>
         
         
@@ -78,91 +68,64 @@
         - `handler` 是 `tsugu` 的一个同步函数，用于直接处理用户输入的自然语言并返回查询结果: 
         
         ```python
         import io
         import tsugu
         
         # 四个参数，分别意味着 消息内容 用户id 平台 频道id
-        for i in tsugu.handler('查卡 ars 1x', '1528593481', 'red', '666808414'):
-            # 字符串
-            print(i) if isinstance(i, str) else None
-            # 图片
-            print(f"[图像大小: {len(i) / 1024:.2f}KB]") if isinstance(i, bytes) else None
-            # from PIL import Image
-            # Image.open(io.BytesIO(i)).show() if isinstance(i, bytes) else None
+        for i in tsugu.handler(message='查卡 ars 1x', user_id='1528593481', platform='red', channel_id='666808414'):
+            print('文本: ',i) if isinstance(i, str) else None
+            print(f"[图片]") if isinstance(i, bytes) else None
         ```
         
         > 在常用的qqbot中，群号就是 `channel_id`。   
         > 当你使用QQ号作为 `user_id` 时，`platform` 可以填写 `red`。   
         
         
         - 异步框架下，可以使用 `run_in_executor` 方法:
+        > ~~未来会支持异步版本~~   
+        > run_in_executor 一辈子吧
         
-        > 以 lagrange-python 群聊为例，其他异步框架请自行查阅文档。
-        ```python
-        loop = asyncio.get_running_loop()
-        args = (event.msg, str(event.uin), 'red', str(event.grp_id))
-        response = await loop.run_in_executor(None, tsugu.handler, *args)
-        
-        # 不发送消息
-        if not response:
-            return
-        
-        msg_list = []
-        for item in response:
-            # 处理文本类型的消息
-            msg_list.append(Text(item)) if isinstance(item, str) else None
-            msg_list.append(await client.upload_grp_image(BytesIO(item), event.grp_id)) if isinstance(item, bytes) else None
-        
-        await client.send_grp_msg(msg_list, event.grp_id)
-        ```
-        
-        ## 调用 `tsugu.database`
+        ## 使用本地数据库
         
         ```py
         import tsugu
         
         tsugu.database(path="./data.db")
+        ```
         
         # 此操作会自动创建或使用本地数据库为 tsugu.bot 提供用户数据。
         # 远程数据库将不使用。
-        # 更多功能可能在未来版本中添加。
-        ```
+        
         > 注意，先进行此操作，后进行 `load_config_json` 操作，旧版本 `config.json` 会覆盖数据库路径，导致数据库无法使用。
         
         
-        ## 查看与更改 `tsugu.config` 配置
+        ## 使用配置文件
         
-        - 输出配置到 `config.json` 文件:
-        ```py
-        import tsugu
-        
-        tsugu.config.output_config_json('./config.json')
-        ```
-        
-        - 利用此文件，你可以更改配置项，然后重新加载配置:
         ```py
         import tsugu
         
         tsugu.config.load_config_json('./config.json')
         ```
+        > 如果不存在，会创建默认配置文件。
+        
+        > 注意，不清楚的配置项请不要更改，更改配置项可能会导致不可预知的错误。
         
         
         - 你也可以直接更改配置，但不推荐:   
         
         ```py
         import tsugu
         
         # 更改的后端地址。
         tsugu.config.backend = "http://127.0.0.0.1:3000"
         
         # 添加关闭抽卡模拟的群号。
         tsugu.config.ban_gacha_simulate_group_data = ["114514", "1919810"]
         ```
-        > 注意，不清楚的配置项请不要更改，更改配置项可能会导致不可预知的错误。
         
         
         
         
         ## 使用 `tsugu.router` 路由与内部方法
         
         - 如果想自己进行自然语言处理，你可以使用单独的路由:
@@ -196,28 +159,41 @@
         
         <h2 align="center"> 相对应登录端 </h2>
         
         | 部署方式 | 传送门 |
         | --- | --- |
         | **lpt 登陆端部署** | [![release](https://img.shields.io/github/v/release/kumoSleeping/lgr-tsugu-py?style=flat-square)](https://github.com/kumoSleeping/lgr-tsugu-py) |
         
-        基于 v2 api 的 `Go` + `Lagrange` 的登录端正由 [WindowsSov8](https://github.com/WindowsSov8forUs) 开发中，敬请期待。
-        基于 v2 api 的 `C#` + `Lagrange` 的登录端正由 [棱镜](https://github.com/DreamPrism) 开发中，敬请期待。   
-        基于本项目的 `NoneBot2` 插件也由 [zhaomaoniu](https://github.com/zhaomaoniu) 开发中，敬请期待。
-        
          <details>
         <summary><b>客服ano酱指导(这里可以点击)</b></summary>
          
         **注意，如果你不知道什么是BanGDream，请不要随意加群**    
         **本群还是欢迎加群的（**    
         [BanGDreamBot开发聊天群](https://qm.qq.com/q/zjUPQkrdpm)   
         温馨的聊天环境～   
         
         </details>
         
+        # 关于安装
+        
+        ## 更新
+        ```shell
+        pip install tsugu --upgrade
+        ```
+        
+        ## 使用官方源安装
+        ```shell
+        pip install tsugu --index-url https://pypi.org/simple/
+        ```
+        
+        ## 使用清华源安装(可能不能即使更新)
+        ```shell
+        pip install tsugu --index-url https://pypi.tuna.tsinghua.edu.cn/simple
+        ```
+        
         
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

#### html2text {}

```diff
@@ -1,83 +1,65 @@
-Metadata-Version: 2.1 Name: tsugu Version: 0.5.7 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.6.0 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
 - [x] èªç¶è¯­è¨è¾å¥ -> è¿åç»æ - [ ] ç¬ç«è·¯ç±è¾å¥ -
 > è¿åç»æ `é¨åæ¯æ` - [x] æ¬å°æ°æ®åº (sqlite3) - [x]
 è¿ç¨æ°æ®åº (å®¢æ·ç«¯) - [x] éç½®é¡¹
 (åºç¡éç½®ãä»£çãå½ä»¤å«å ç­)
-                          ********** ?å?®??è?£??ä?¸??æ??´?æ??° **********
-## å®è£ tsugu æ¨¡å ```shell pip install tsugu ``` ## æ´æ° ```shell pip
-install tsugu --upgrade ``` ## ä½¿ç¨å®æ¹æºå®è£ ```shell pip install tsugu
---index-url https://pypi.org/simple/ ``` ## åç«¯éæ± -
+                              ********** ?å?®??è?£? **********
+## å®è£ tsugu æ¨¡å ```shell pip install tsugu ``` ## åç«¯éæ± -
 åºå¾ï¼éè¦æ¯æ `v2 API` (2024.2.28æ¥ä»¥åçåç«¯çæ¬) -
-utilsï¼éè¦æ¯æ `v2 API` -
 ç¨æ·æ°æ®ï¼éè¦ä¸ä¸ªå¯ç¨äº**æ°æ®åº**çåç«¯ï¼éè¦æ¯æ `v2
-API` >
-ä¸ä¸ªåç«¯è®¾ç½®å¯ä»¥ä¸åï¼é»è®¤å¨é¨è®¾ç½®ä¸º**å¬å±åç«¯**ã ***
+API` > åç«¯è®¾ç½®å¯ä»¥ä¸åï¼é»è®¤å¨é¨è®¾ç½®ä¸º**å¬å±åç«¯**ã ***
                           ********** ?æ?µ??è?¯??ä?¸??è?°??ç??¨ **********
 ## è°ç¨ `tsugu.handler` - `handler` æ¯ `tsugu`
 çä¸ä¸ªåæ­¥å½æ°ï¼ç¨äºç´æ¥å¤çç¨æ·è¾å¥çèªç¶è¯­è¨å¹¶è¿åæ¥è¯¢ç»æ:
 ```python import io import tsugu # åä¸ªåæ°ï¼åå«æå³ç æ¶æ¯åå®¹
-ç¨æ·id å¹³å° é¢éid for i in tsugu.handler('æ¥å¡ ars 1x', '1528593481',
-'red', '666808414'): # å­ç¬¦ä¸² print(i) if isinstance(i, str) else None #
-å¾ç print(f"[å¾åå¤§å°: {len(i) / 1024:.2f}KB]") if isinstance(i, bytes)
-else None # from PIL import Image # Image.open(io.BytesIO(i)).show() if
-isinstance(i, bytes) else None ``` > å¨å¸¸ç¨çqqbotä¸­ï¼ç¾¤å·å°±æ¯
-`channel_id`ã > å½ä½ ä½¿ç¨QQå·ä½ä¸º `user_id` æ¶ï¼`platform`
-å¯ä»¥å¡«å `red`ã - å¼æ­¥æ¡æ¶ä¸ï¼å¯ä»¥ä½¿ç¨ `run_in_executor`
-æ¹æ³: > ä»¥ lagrange-python
-ç¾¤èä¸ºä¾ï¼å¶ä»å¼æ­¥æ¡æ¶è¯·èªè¡æ¥éææ¡£ã ```python loop =
-asyncio.get_running_loop() args = (event.msg, str(event.uin), 'red', str
-(event.grp_id)) response = await loop.run_in_executor(None, tsugu.handler,
-*args) # ä¸åéæ¶æ¯ if not response: return msg_list = [] for item in
-response: # å¤çææ¬ç±»åçæ¶æ¯ msg_list.append(Text(item)) if
-isinstance(item, str) else None msg_list.append(await client.upload_grp_image
-(BytesIO(item), event.grp_id)) if isinstance(item, bytes) else None await
-client.send_grp_msg(msg_list, event.grp_id) ``` ## è°ç¨ `tsugu.database`
-```py import tsugu tsugu.database(path="./data.db") #
+ç¨æ·id å¹³å° é¢éid for i in tsugu.handler(message='æ¥å¡ ars 1x',
+user_id='1528593481', platform='red', channel_id='666808414'): print('ææ¬:
+',i) if isinstance(i, str) else None print(f"[å¾ç]") if isinstance(i, bytes)
+else None ``` > å¨å¸¸ç¨çqqbotä¸­ï¼ç¾¤å·å°±æ¯ `channel_id`ã >
+å½ä½ ä½¿ç¨QQå·ä½ä¸º `user_id` æ¶ï¼`platform` å¯ä»¥å¡«å `red`ã -
+å¼æ­¥æ¡æ¶ä¸ï¼å¯ä»¥ä½¿ç¨ `run_in_executor` æ¹æ³: >
+~~æªæ¥ä¼æ¯æå¼æ­¥çæ¬~~ > run_in_executor ä¸è¾å­å§ ##
+ä½¿ç¨æ¬å°æ°æ®åº ```py import tsugu tsugu.database(path="./data.db") ``` #
 æ­¤æä½ä¼èªå¨åå»ºæä½¿ç¨æ¬å°æ°æ®åºä¸º tsugu.bot
-æä¾ç¨æ·æ°æ®ã # è¿ç¨æ°æ®åºå°ä¸ä½¿ç¨ã #
-æ´å¤åè½å¯è½å¨æªæ¥çæ¬ä¸­æ·»å ã ``` >
+æä¾ç¨æ·æ°æ®ã # è¿ç¨æ°æ®åºå°ä¸ä½¿ç¨ã >
 æ³¨æï¼åè¿è¡æ­¤æä½ï¼åè¿è¡ `load_config_json` æä½ï¼æ§çæ¬
 `config.json` ä¼è¦çæ°æ®åºè·¯å¾ï¼å¯¼è´æ°æ®åºæ æ³ä½¿ç¨ã ##
-æ¥çä¸æ´æ¹ `tsugu.config` éç½® - è¾åºéç½®å° `config.json` æä»¶:
-```py import tsugu tsugu.config.output_config_json('./config.json') ``` -
-å©ç¨æ­¤æä»¶ï¼ä½ å¯ä»¥æ´æ¹éç½®é¡¹ï¼ç¶åéæ°å è½½éç½®: ```py
-import tsugu tsugu.config.load_config_json('./config.json') ``` -
-ä½ ä¹å¯ä»¥ç´æ¥æ´æ¹éç½®ï¼ä½ä¸æ¨è: ```py import tsugu #
+ä½¿ç¨éç½®æä»¶ ```py import tsugu tsugu.config.load_config_json('./
+config.json') ``` > å¦æä¸å­å¨ï¼ä¼åå»ºé»è®¤éç½®æä»¶ã >
+æ³¨æï¼ä¸æ¸æ¥çéç½®é¡¹è¯·ä¸è¦æ´æ¹ï¼æ´æ¹éç½®é¡¹å¯è½ä¼å¯¼è´ä¸å¯é¢ç¥çéè¯¯ã
+- ä½ ä¹å¯ä»¥ç´æ¥æ´æ¹éç½®ï¼ä½ä¸æ¨è: ```py import tsugu #
 æ´æ¹çåç«¯å°åã tsugu.config.backend = "http://127.0.0.0.1:3000" #
 æ·»å å³é­æ½å¡æ¨¡æçç¾¤å·ã tsugu.config.ban_gacha_simulate_group_data
-= ["114514", "1919810"] ``` >
-æ³¨æï¼ä¸æ¸æ¥çéç½®é¡¹è¯·ä¸è¦æ´æ¹ï¼æ´æ¹éç½®é¡¹å¯è½ä¼å¯¼è´ä¸å¯é¢ç¥çéè¯¯ã
-## ä½¿ç¨ `tsugu.router` è·¯ç±ä¸åé¨æ¹æ³ -
+= ["114514", "1919810"] ``` ## ä½¿ç¨ `tsugu.router` è·¯ç±ä¸åé¨æ¹æ³ -
 å¦ææ³èªå·±è¿è¡èªç¶è¯­è¨å¤çï¼ä½ å¯ä»¥ä½¿ç¨åç¬çè·¯ç±: ```py
 import tsugu # è·åç¨æ·æ°æ® reply = tsugu.router.get_user_data("red",
 "1234567890") # æ¥å¡ reply = tsugu.router.card("çº¢ ksm", [0, 3], 5) #
 è®¾ç½®ç©å®¶è½¦çè½¬å reply = tsugu.router.set_car_forward("red",
 "1234567890", True) ``` -
 æ­¤å¤è¿æ´é²äºä¸äºåé¨æ¹æ³ï¼éè¦å¯ä»¥ä½¿ç¨: ```py import tsugu
 tsugu.interior_local_method.bind_player_verification("red", "1234567890", True)
 tsugu.interior_remote_method.bind_player_verification("red", "1234567890", 0,
 '1000011232', True) tsugu.interior_local_method.submit_car_number_msg("123456
 å¤§åq1", "1234567890", "red") ``` ***
                         ********** ?ç??¸?å?¯?¹?å?º??ç??»?å?½??ç?«?¯ **********
 | é¨ç½²æ¹å¼ | ä¼ éé¨ | | --- | --- | | **lpt ç»éç«¯é¨ç½²** | [!
 [release](https://img.shields.io/github/v/release/kumoSleeping/lgr-tsugu-
-py?style=flat-square)](https://github.com/kumoSleeping/lgr-tsugu-py) | åºäº
-v2 api ç `Go` + `Lagrange` çç»å½ç«¯æ­£ç± [WindowsSov8](https://
-github.com/WindowsSov8forUs) å¼åä¸­ï¼æ¬è¯·æå¾ã åºäº v2 api ç `C#`
-+ `Lagrange` çç»å½ç«¯æ­£ç± [æ£±é](https://github.com/DreamPrism)
-å¼åä¸­ï¼æ¬è¯·æå¾ã åºäºæ¬é¡¹ç®ç `NoneBot2` æä»¶ä¹ç±
-[zhaomaoniu](https://github.com/zhaomaoniu) å¼åä¸­ï¼æ¬è¯·æå¾ã
+py?style=flat-square)](https://github.com/kumoSleeping/lgr-tsugu-py) |
 ?å?®?¢?æ??aannoo?é??±?æ???å?¯?¼((?è?¿??é???å??¯?ä?»?¥?ç??¹?å??»))
 **æ³¨æï¼å¦æä½ ä¸ç¥éä»ä¹æ¯BanGDreamï¼è¯·ä¸è¦éæå ç¾¤**
 **æ¬ç¾¤è¿æ¯æ¬¢è¿å ç¾¤çï¼** [BanGDreamBotå¼åèå¤©ç¾¤](https://
-qm.qq.com/q/zjUPQkrdpm) æ¸©é¦¨çèå¤©ç¯å¢ï½ Platform: UNKNOWN Classifier:
-Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
-MIT License Classifier: Operating System :: OS Independent Requires-Python:
->=3.8 Description-Content-Type: text/markdown
+qm.qq.com/q/zjUPQkrdpm) æ¸©é¦¨çèå¤©ç¯å¢ï½ # å³äºå®è£ ## æ´æ°
+```shell pip install tsugu --upgrade ``` ## ä½¿ç¨å®æ¹æºå®è£ ```shell pip
+install tsugu --index-url https://pypi.org/simple/ ``` ## ä½¿ç¨æ¸åæºå®è£
+(å¯è½ä¸è½å³ä½¿æ´æ°) ```shell pip install tsugu --index-url https://
+pypi.tuna.tsinghua.edu.cn/simple ``` Platform: UNKNOWN Classifier: Programming
+Language :: Python :: 3.8 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Requires-Python: >=3.8
+Description-Content-Type: text/markdown
```

