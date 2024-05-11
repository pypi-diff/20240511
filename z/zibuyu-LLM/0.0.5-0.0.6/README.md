# Comparing `tmp/zibuyu_LLM-0.0.5-py3-none-any.whl.zip` & `tmp/zibuyu_LLM-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 60031 bytes, number of entries: 18
+Zip file size: 60105 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat      305 b- defN 24-May-11 08:41 zibuyu_llm_api/__init__.py
 -rw-rw-rw-  2.0 fat    31879 b- defN 24-May-11 08:41 zibuyu_llm_api/minmax_api.py
 -rw-rw-rw-  2.0 fat      735 b- defN 24-May-11 08:46 zibuyu_llm_web/__init__.py
 -rw-rw-rw-  2.0 fat     7135 b- defN 24-May-11 08:37 zibuyu_llm_web/baichuan.py
 -rw-rw-rw-  2.0 fat     7099 b- defN 24-May-11 01:45 zibuyu_llm_web/base.py
 -rw-rw-rw-  2.0 fat    14808 b- defN 24-May-11 08:37 zibuyu_llm_web/deepseek.py
 -rw-rw-rw-  2.0 fat      732 b- defN 24-May-11 08:49 zibuyu_llm_web/errors.py
 -rw-rw-rw-  2.0 fat     9907 b- defN 24-May-11 08:37 zibuyu_llm_web/kimi.py
 -rw-rw-rw-  2.0 fat    37604 b- defN 24-May-11 08:41 zibuyu_llm_web/minmax.py
 -rw-rw-rw-  2.0 fat    37630 b- defN 24-May-11 08:37 zibuyu_llm_web/qwen.py
 -rw-rw-rw-  2.0 fat     5132 b- defN 24-May-09 13:49 zibuyu_llm_web/types.py
 -rw-rw-rw-  2.0 fat     8118 b- defN 24-May-11 08:37 zibuyu_llm_web/wanxiang.py
 -rw-rw-rw-  2.0 fat    14465 b- defN 24-May-11 08:37 zibuyu_llm_web/xinchen.py
--rw-rw-rw-  2.0 fat    25562 b- defN 24-May-11 08:37 zibuyu_llm_web/xunfei.py
--rw-rw-rw-  2.0 fat     1341 b- defN 24-May-11 08:51 zibuyu_LLM-0.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-11 08:51 zibuyu_LLM-0.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       30 b- defN 24-May-11 08:51 zibuyu_LLM-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1455 b- defN 24-May-11 08:51 zibuyu_LLM-0.0.5.dist-info/RECORD
-18 files, 204029 bytes uncompressed, 57673 bytes compressed:  71.7%
+-rw-rw-rw-  2.0 fat    25770 b- defN 24-May-11 09:08 zibuyu_llm_web/xunfei.py
+-rw-rw-rw-  2.0 fat     1388 b- defN 24-May-11 09:09 zibuyu_LLM-0.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-11 09:09 zibuyu_LLM-0.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       30 b- defN 24-May-11 09:09 zibuyu_LLM-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1455 b- defN 24-May-11 09:09 zibuyu_LLM-0.0.6.dist-info/RECORD
+18 files, 204284 bytes uncompressed, 57747 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: zibuyu_llm_web/xinchen.py
 Comment: 
 
 Filename: zibuyu_llm_web/xunfei.py
 Comment: 
 
-Filename: zibuyu_LLM-0.0.5.dist-info/METADATA
+Filename: zibuyu_LLM-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: zibuyu_LLM-0.0.5.dist-info/WHEEL
+Filename: zibuyu_LLM-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: zibuyu_LLM-0.0.5.dist-info/top_level.txt
+Filename: zibuyu_LLM-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: zibuyu_LLM-0.0.5.dist-info/RECORD
+Filename: zibuyu_LLM-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zibuyu_llm_web/xunfei.py

```diff
@@ -26,29 +26,35 @@
     model_name = 'XunFeiWeb'
     base_url = 'https://xinghuo.xfyun.cn'
 
     def __init__(
             self,
             account: str = None,
             password: str = None,
+            cookie: str = None,
             sso_session_id: str = None,
             logger_obj: logging.Logger = None,
-            error_dir: str = None
+            error_dir: str = None,
+            *args,
+            **kwargs
     ):
         self.logger = logger_obj
         self.account = account
         self.password = password
+        self.cookie = cookie
         self._sso_session_id = sso_session_id
         self._account_id: str = ''
         self.__gt_token = ''
         self.error_dir = error_dir
 
         super().__init__()
+        self.request_session.cookies.update(self.cookies_dict)
 
-        self.request_session.cookies.set('ssoSessionId', self._sso_session_id)
+        if self._sso_session_id:
+            self.request_session.cookies.set('ssoSessionId', self._sso_session_id)
 
         self.__headers = {
             'Accept': "*/*",
             "Accept-Encoding": "gzip, deflate, br, zstd",
             "Accept-Language": "zh-CN,zh;q=0.9,en;q=0.8",
 
             "Cache-Control": "no-cache",
```

## Comparing `zibuyu_LLM-0.0.5.dist-info/METADATA` & `zibuyu_LLM-0.0.6.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zibuyu-LLM
-Version: 0.0.5
+Version: 0.0.6
 Summary: 子不语个人工具包-LLM
 Author: 子不语
 License: MIT
 Keywords: LLM,zibuyu
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -37,14 +37,16 @@
 - 通义千问（Qwen）
 - 通义星辰（XinChen)
 - 通义万相（XinXiang）
 - 讯飞星火（Spark）
 
 # 版本记录
 
+`0.0.6`：修改讯飞星火调用的传值
+
 `0.0.5`：增加error与types模块
 
 `0.0.4`：修复导包路径问题
 
 `0.0.3`：修复导包路径问题
 
 `0.0.2`：无变化，增加Readme文件
```

## Comparing `zibuyu_LLM-0.0.5.dist-info/RECORD` & `zibuyu_LLM-0.0.6.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -7,12 +7,12 @@
 zibuyu_llm_web/errors.py,sha256=Vib55tBOR1goqM7ddmx51TbJ8vKEXOCJEqcbvjTNaWw,732
 zibuyu_llm_web/kimi.py,sha256=SuG6u6FbZqD_AntxeXp3fuih2UMDtNzFbUSJSmeuoik,9907
 zibuyu_llm_web/minmax.py,sha256=Z_gPGiRdBOdg_2Xu_wfufItWLe-bR19CufykNZsxm74,37604
 zibuyu_llm_web/qwen.py,sha256=Iil5TckkFwroECpjC_Zf-PyZQ9iIbLKcSeSYOr_l3Lw,37630
 zibuyu_llm_web/types.py,sha256=xzN-TgzwMB0xZKFXusHxwpY2Eqm3iRBm2qMUmKzRm8I,5132
 zibuyu_llm_web/wanxiang.py,sha256=YU9R42VaxWlY7gpcT_qAkguSqhCfDuK19-lpWaWgRDA,8118
 zibuyu_llm_web/xinchen.py,sha256=PJAKtZCaj445CpVhUL035lhDuCH0NO5gdu0vyLuoymw,14465
-zibuyu_llm_web/xunfei.py,sha256=8gpfaPbzWEv1lK9Vlv_hXUKBfn0-ExaUsb0H6WqaULg,25562
-zibuyu_LLM-0.0.5.dist-info/METADATA,sha256=AtiXKaDIhvQBcBnXwL9CWbxtir8CHtyKshTHaEE7VLo,1341
-zibuyu_LLM-0.0.5.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-zibuyu_LLM-0.0.5.dist-info/top_level.txt,sha256=QF6FI2Tcc78mYBpfy15YWDU-j16KK_2WqGF-3kj8Jew,30
-zibuyu_LLM-0.0.5.dist-info/RECORD,,
+zibuyu_llm_web/xunfei.py,sha256=CuUg9BELktRmoVTkHlsFu8__YZGlmd0uCb4VFBeqY68,25770
+zibuyu_LLM-0.0.6.dist-info/METADATA,sha256=c0FH2TdEoCwj6Gm5mHy1DxynTPDskS6wa2q_K8WTnS0,1388
+zibuyu_LLM-0.0.6.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+zibuyu_LLM-0.0.6.dist-info/top_level.txt,sha256=QF6FI2Tcc78mYBpfy15YWDU-j16KK_2WqGF-3kj8Jew,30
+zibuyu_LLM-0.0.6.dist-info/RECORD,,
```

