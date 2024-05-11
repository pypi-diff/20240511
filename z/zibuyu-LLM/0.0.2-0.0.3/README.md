# Comparing `tmp/zibuyu_LLM-0.0.2-py3-none-any.whl.zip` & `tmp/zibuyu_LLM-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 57002 bytes, number of entries: 16
--rw-rw-rw-  2.0 fat      241 b- defN 24-May-09 06:10 api/__init__.py
--rw-rw-rw-  2.0 fat    32008 b- defN 24-May-06 10:01 api/minmax_api.py
--rw-rw-rw-  2.0 fat      241 b- defN 24-May-09 06:09 web/__init__.py
--rw-rw-rw-  2.0 fat     7155 b- defN 24-May-09 06:22 web/baichuan.py
--rw-rw-rw-  2.0 fat     7099 b- defN 24-May-11 01:45 web/base.py
--rw-rw-rw-  2.0 fat    14828 b- defN 24-May-09 13:49 web/deepseek.py
--rw-rw-rw-  2.0 fat     9927 b- defN 24-May-09 13:53 web/kimi.py
--rw-rw-rw-  2.0 fat    37591 b- defN 24-May-09 16:21 web/minmax.py
--rw-rw-rw-  2.0 fat    37650 b- defN 24-May-10 11:10 web/qwen.py
--rw-rw-rw-  2.0 fat     8138 b- defN 24-May-09 06:22 web/wanxiang.py
--rw-rw-rw-  2.0 fat    14485 b- defN 24-May-10 11:12 web/xinchen.py
--rw-rw-rw-  2.0 fat    25572 b- defN 24-May-11 02:18 web/xunfei.py
--rw-rw-rw-  2.0 fat     1226 b- defN 24-May-11 06:56 zibuyu_LLM-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-11 06:56 zibuyu_LLM-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 24-May-11 06:56 zibuyu_LLM-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1162 b- defN 24-May-11 06:56 zibuyu_LLM-0.0.2.dist-info/RECORD
-16 files, 197423 bytes uncompressed, 55154 bytes compressed:  72.1%
+Zip file size: 57358 bytes, number of entries: 16
+-rw-rw-rw-  2.0 fat      241 b- defN 24-May-09 06:10 llm_api/__init__.py
+-rw-rw-rw-  2.0 fat    32008 b- defN 24-May-06 10:01 llm_api/minmax_api.py
+-rw-rw-rw-  2.0 fat      664 b- defN 24-May-11 08:30 llm_web/__init__.py
+-rw-rw-rw-  2.0 fat     7155 b- defN 24-May-09 06:22 llm_web/baichuan.py
+-rw-rw-rw-  2.0 fat     7099 b- defN 24-May-11 01:45 llm_web/base.py
+-rw-rw-rw-  2.0 fat    14828 b- defN 24-May-09 13:49 llm_web/deepseek.py
+-rw-rw-rw-  2.0 fat     9927 b- defN 24-May-09 13:53 llm_web/kimi.py
+-rw-rw-rw-  2.0 fat    37603 b- defN 24-May-11 08:30 llm_web/minmax.py
+-rw-rw-rw-  2.0 fat    37650 b- defN 24-May-10 11:10 llm_web/qwen.py
+-rw-rw-rw-  2.0 fat     8138 b- defN 24-May-09 06:22 llm_web/wanxiang.py
+-rw-rw-rw-  2.0 fat    14485 b- defN 24-May-10 11:12 llm_web/xinchen.py
+-rw-rw-rw-  2.0 fat    25572 b- defN 24-May-11 02:18 llm_web/xunfei.py
+-rw-rw-rw-  2.0 fat     1264 b- defN 24-May-11 08:30 zibuyu_LLM-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-11 08:30 zibuyu_LLM-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 24-May-11 08:30 zibuyu_LLM-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1211 b- defN 24-May-11 08:30 zibuyu_LLM-0.0.3.dist-info/RECORD
+16 files, 197953 bytes uncompressed, 55414 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -1,49 +1,49 @@
-Filename: api/__init__.py
+Filename: llm_api/__init__.py
 Comment: 
 
-Filename: api/minmax_api.py
+Filename: llm_api/minmax_api.py
 Comment: 
 
-Filename: web/__init__.py
+Filename: llm_web/__init__.py
 Comment: 
 
-Filename: web/baichuan.py
+Filename: llm_web/baichuan.py
 Comment: 
 
-Filename: web/base.py
+Filename: llm_web/base.py
 Comment: 
 
-Filename: web/deepseek.py
+Filename: llm_web/deepseek.py
 Comment: 
 
-Filename: web/kimi.py
+Filename: llm_web/kimi.py
 Comment: 
 
-Filename: web/minmax.py
+Filename: llm_web/minmax.py
 Comment: 
 
-Filename: web/qwen.py
+Filename: llm_web/qwen.py
 Comment: 
 
-Filename: web/wanxiang.py
+Filename: llm_web/wanxiang.py
 Comment: 
 
-Filename: web/xinchen.py
+Filename: llm_web/xinchen.py
 Comment: 
 
-Filename: web/xunfei.py
+Filename: llm_web/xunfei.py
 Comment: 
 
-Filename: zibuyu_LLM-0.0.2.dist-info/METADATA
+Filename: zibuyu_LLM-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: zibuyu_LLM-0.0.2.dist-info/WHEEL
+Filename: zibuyu_LLM-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: zibuyu_LLM-0.0.2.dist-info/top_level.txt
+Filename: zibuyu_LLM-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: zibuyu_LLM-0.0.2.dist-info/RECORD
+Filename: zibuyu_LLM-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `api/minmax_api.py` & `llm_api/minmax_api.py`

 * *Files identical despite different names*

## Comparing `web/baichuan.py` & `llm_web/baichuan.py`

 * *Files identical despite different names*

## Comparing `web/base.py` & `llm_web/base.py`

 * *Files identical despite different names*

## Comparing `web/deepseek.py` & `llm_web/deepseek.py`

 * *Files identical despite different names*

## Comparing `web/kimi.py` & `llm_web/kimi.py`

 * *Files identical despite different names*

## Comparing `web/minmax.py` & `llm_web/minmax.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
         self.__voice_info_dict: Optional[dict] = None
 
         # 语音相关_请求参数
         self.__voice_user_data = {
             'msgID': "",  # 消息ID
             'timbre': "",  # 配音音色
-            'device_platform': "web",
+            'device_platform': "llm_web",
             'app_id': "3001",
             'uuid': '',  # uuid，待填充
             'device_id': '',  # 设备ID，待填充
             'version_code': "21200",
             'os_name': "Windows",
             'browser_name': "chrome",
             'server_version': "101",
@@ -85,15 +85,15 @@
             'screen_width': 1920,
             'screen_height': 1080,
             'unix': '',  # 时间戳，待填充
         }
 
         # 公用请求参数
         self.__user_data = {
-            'device_platform': "web",
+            'device_platform': "llm_web",
             'app_id': "3001",
             'uuid': '',  # uuid，待填充
             'device_id': '',  # 设备ID，待填充
             'version_code': "21200",
             'os_name': "Windows",
             'browser_name': "chrome",
             'server_version': "101",
@@ -989,15 +989,15 @@
 
     def test(self):
         unix = '1715264091000'
 
         user_data = {
             'msgID': 244977956405796869,
             'timbre': "male-botong",
-            'device_platform': "web",
+            'device_platform': "llm_web",
             'app_id': "3001",
             'uuid': '7c251825-9626-4e8a-81df-d8a3cbf58c50',  # uuid，待填充
             'device_id': '244976245380423685',  # 设备ID，待填充
             'version_code': "21200",
             'os_name': "Windows",
             'browser_name': "chrome",
             'server_version': "101",
```

## Comparing `web/qwen.py` & `llm_web/qwen.py`

 * *Files identical despite different names*

## Comparing `web/wanxiang.py` & `llm_web/wanxiang.py`

 * *Files identical despite different names*

## Comparing `web/xinchen.py` & `llm_web/xinchen.py`

 * *Files identical despite different names*

## Comparing `web/xunfei.py` & `llm_web/xunfei.py`

 * *Files identical despite different names*

## Comparing `zibuyu_LLM-0.0.2.dist-info/METADATA` & `zibuyu_LLM-0.0.3.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zibuyu-LLM
-Version: 0.0.2
+Version: 0.0.3
 Summary: 子不语个人工具包-LLM
 Author: 子不语
 License: MIT
 Keywords: LLM,zibuyu
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -37,10 +37,12 @@
 - 通义千问（Qwen）
 - 通义星辰（XinChen)
 - 通义万相（XinXiang）
 - 讯飞星火（Spark）
 
 # 版本记录
 
+`0.0.3`：修复导包路径问题
+
 `0.0.2`：无变化，增加Readme文件
 
 `0.0.1`：第一次上传
```

## Comparing `zibuyu_LLM-0.0.2.dist-info/RECORD` & `zibuyu_LLM-0.0.3.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-api/__init__.py,sha256=-BaxH2cB58GSlGGBIVoB0Qdz_RX5ypIFz5EfyttDU0U,241
-api/minmax_api.py,sha256=mE3-EV4S_DWbgQkZp9wHmBSdh4jX3AAbJuy8oQuoq_Y,32008
-web/__init__.py,sha256=-BaxH2cB58GSlGGBIVoB0Qdz_RX5ypIFz5EfyttDU0U,241
-web/baichuan.py,sha256=ceejWfJRES43jaVBG6SEBmYpJhJLBcNwcSWZe7Ykdmk,7155
-web/base.py,sha256=s7GYbP70kKt7nhMLK0Jp22gVu2EfmS30eA5b6k_aYa8,7099
-web/deepseek.py,sha256=PEVDXpV1qjVLMShz3Bd0LG0SnUkW5HkLhut4bYkP464,14828
-web/kimi.py,sha256=RxVO6azaT7Xw-hobl8k6kdzXkzMVUh-YOt8jFDe_CPk,9927
-web/minmax.py,sha256=MGKgSdsamZQgk7bFxdrKVgzAHgw6TW9F252eXh5w6IU,37591
-web/qwen.py,sha256=zgxDa-MsYdgoLNahaco_1DfX6duhEaaN8E7gT77H0mw,37650
-web/wanxiang.py,sha256=ML92G-1KpvAkSGUZujOHDEX-iHm6fzuPPe3Lq_6mLxw,8138
-web/xinchen.py,sha256=BmJdcFykMKnLdUUu5TvfEg2BCdcOZ19kqDpi9suB3X8,14485
-web/xunfei.py,sha256=kNnHPs__p07mf5_a3-9zdUyPKDHK7DGMFa_2Dee5b1w,25572
-zibuyu_LLM-0.0.2.dist-info/METADATA,sha256=bWBvr5ahI-M1qVYvVfYhO5mIUmKEF8xWUz82rsLn5Vk,1226
-zibuyu_LLM-0.0.2.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-zibuyu_LLM-0.0.2.dist-info/top_level.txt,sha256=lpfVTTvr_OnoRgurRAaARNiZCC1Z79GYsRHW_WiC5J8,8
-zibuyu_LLM-0.0.2.dist-info/RECORD,,
+llm_api/__init__.py,sha256=-BaxH2cB58GSlGGBIVoB0Qdz_RX5ypIFz5EfyttDU0U,241
+llm_api/minmax_api.py,sha256=mE3-EV4S_DWbgQkZp9wHmBSdh4jX3AAbJuy8oQuoq_Y,32008
+llm_web/__init__.py,sha256=xdRXWFnKvV1qInfVCbEoBZgPCow1MZW5yBXcHEaetQI,664
+llm_web/baichuan.py,sha256=ceejWfJRES43jaVBG6SEBmYpJhJLBcNwcSWZe7Ykdmk,7155
+llm_web/base.py,sha256=s7GYbP70kKt7nhMLK0Jp22gVu2EfmS30eA5b6k_aYa8,7099
+llm_web/deepseek.py,sha256=PEVDXpV1qjVLMShz3Bd0LG0SnUkW5HkLhut4bYkP464,14828
+llm_web/kimi.py,sha256=RxVO6azaT7Xw-hobl8k6kdzXkzMVUh-YOt8jFDe_CPk,9927
+llm_web/minmax.py,sha256=LPOz2ovZJMU3J_SgQsQpXl_R-C8-72vvODvilFCiyjA,37603
+llm_web/qwen.py,sha256=zgxDa-MsYdgoLNahaco_1DfX6duhEaaN8E7gT77H0mw,37650
+llm_web/wanxiang.py,sha256=ML92G-1KpvAkSGUZujOHDEX-iHm6fzuPPe3Lq_6mLxw,8138
+llm_web/xinchen.py,sha256=BmJdcFykMKnLdUUu5TvfEg2BCdcOZ19kqDpi9suB3X8,14485
+llm_web/xunfei.py,sha256=kNnHPs__p07mf5_a3-9zdUyPKDHK7DGMFa_2Dee5b1w,25572
+zibuyu_LLM-0.0.3.dist-info/METADATA,sha256=BNo6zJh2cC5aKNUHns13KbGmdzsWStZ7iCbi-VKxZh0,1264
+zibuyu_LLM-0.0.3.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+zibuyu_LLM-0.0.3.dist-info/top_level.txt,sha256=TCq8ARNfKyr4m0hMN-ExmIQlKRvssaVk2VUi1y1c1-8,16
+zibuyu_LLM-0.0.3.dist-info/RECORD,,
```

