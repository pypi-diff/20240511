# Comparing `tmp/zibuyu_LLM-0.0.4-py3-none-any.whl.zip` & `tmp/zibuyu_LLM-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 59938 bytes, number of entries: 18
+Zip file size: 60031 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat      305 b- defN 24-May-11 08:41 zibuyu_llm_api/__init__.py
 -rw-rw-rw-  2.0 fat    31879 b- defN 24-May-11 08:41 zibuyu_llm_api/minmax_api.py
--rw-rw-rw-  2.0 fat      664 b- defN 24-May-11 08:30 zibuyu_llm_web/__init__.py
+-rw-rw-rw-  2.0 fat      735 b- defN 24-May-11 08:46 zibuyu_llm_web/__init__.py
 -rw-rw-rw-  2.0 fat     7135 b- defN 24-May-11 08:37 zibuyu_llm_web/baichuan.py
 -rw-rw-rw-  2.0 fat     7099 b- defN 24-May-11 01:45 zibuyu_llm_web/base.py
 -rw-rw-rw-  2.0 fat    14808 b- defN 24-May-11 08:37 zibuyu_llm_web/deepseek.py
--rw-rw-rw-  2.0 fat      626 b- defN 24-May-10 01:59 zibuyu_llm_web/errors.py
+-rw-rw-rw-  2.0 fat      732 b- defN 24-May-11 08:49 zibuyu_llm_web/errors.py
 -rw-rw-rw-  2.0 fat     9907 b- defN 24-May-11 08:37 zibuyu_llm_web/kimi.py
 -rw-rw-rw-  2.0 fat    37604 b- defN 24-May-11 08:41 zibuyu_llm_web/minmax.py
 -rw-rw-rw-  2.0 fat    37630 b- defN 24-May-11 08:37 zibuyu_llm_web/qwen.py
 -rw-rw-rw-  2.0 fat     5132 b- defN 24-May-09 13:49 zibuyu_llm_web/types.py
 -rw-rw-rw-  2.0 fat     8118 b- defN 24-May-11 08:37 zibuyu_llm_web/wanxiang.py
 -rw-rw-rw-  2.0 fat    14465 b- defN 24-May-11 08:37 zibuyu_llm_web/xinchen.py
 -rw-rw-rw-  2.0 fat    25562 b- defN 24-May-11 08:37 zibuyu_llm_web/xunfei.py
--rw-rw-rw-  2.0 fat     1302 b- defN 24-May-11 08:41 zibuyu_LLM-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-11 08:41 zibuyu_LLM-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       30 b- defN 24-May-11 08:41 zibuyu_LLM-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1455 b- defN 24-May-11 08:41 zibuyu_LLM-0.0.4.dist-info/RECORD
-18 files, 203813 bytes uncompressed, 57580 bytes compressed:  71.7%
+-rw-rw-rw-  2.0 fat     1341 b- defN 24-May-11 08:51 zibuyu_LLM-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-11 08:51 zibuyu_LLM-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       30 b- defN 24-May-11 08:51 zibuyu_LLM-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1455 b- defN 24-May-11 08:51 zibuyu_LLM-0.0.5.dist-info/RECORD
+18 files, 204029 bytes uncompressed, 57673 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: zibuyu_llm_web/xinchen.py
 Comment: 
 
 Filename: zibuyu_llm_web/xunfei.py
 Comment: 
 
-Filename: zibuyu_LLM-0.0.4.dist-info/METADATA
+Filename: zibuyu_LLM-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: zibuyu_LLM-0.0.4.dist-info/WHEEL
+Filename: zibuyu_LLM-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: zibuyu_LLM-0.0.4.dist-info/top_level.txt
+Filename: zibuyu_LLM-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: zibuyu_LLM-0.0.4.dist-info/RECORD
+Filename: zibuyu_LLM-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zibuyu_llm_web/__init__.py

```diff
@@ -14,19 +14,23 @@
 from .xinchen import XinChenWeb
 from .xunfei import XunFeiWeb
 from .kimi import KimiWeb
 from .minmax import MinMaxWeb
 from .deepseek import DeepSeekWeb
 from .baichuan import BaiChuanWeb
 from .wanxiang import WanXiangWeb
+from . import errors
+from . import types
 
 
 __all__ = [
     'QwenWeb',
     'XinChenWeb',
     'XunFeiWeb',
     'KimiWeb',
     'MinMaxWeb',
     'DeepSeekWeb',
     'BaiChuanWeb',
     'WanXiangWeb',
+    'errors',
+    'types'
 ]
```

## zibuyu_llm_web/errors.py

```diff
@@ -25,7 +25,11 @@
 
 class LoginFailError(Exception):
     message = "登录失败"
 
 
 class APIConnectionError(Exception):
     message = "网络连接错误"
+
+
+class SpiderHasToChangeError(Exception):
+    message = "网页出现新逻辑，爬虫需要更换"
```

## Comparing `zibuyu_LLM-0.0.4.dist-info/METADATA` & `zibuyu_LLM-0.0.5.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zibuyu-LLM
-Version: 0.0.4
+Version: 0.0.5
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
 
+`0.0.5`：增加error与types模块
+
 `0.0.4`：修复导包路径问题
 
 `0.0.3`：修复导包路径问题
 
 `0.0.2`：无变化，增加Readme文件
 
 `0.0.1`：第一次上传
```

## Comparing `zibuyu_LLM-0.0.4.dist-info/RECORD` & `zibuyu_LLM-0.0.5.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 zibuyu_llm_api/__init__.py,sha256=Ox3V8_X8l52LqJ_ATAWv0xpxBZxq5o1xn16TcEvSUl4,305
 zibuyu_llm_api/minmax_api.py,sha256=6gZMHkmSfwsmbFtjkJF2W9uUX35zmdk1vLwIlcUuOJo,31879
-zibuyu_llm_web/__init__.py,sha256=xdRXWFnKvV1qInfVCbEoBZgPCow1MZW5yBXcHEaetQI,664
+zibuyu_llm_web/__init__.py,sha256=1YEBJuq9b5XG8jUOtgdrMNDiSiHZ9_OCT6PxH_xDoiY,735
 zibuyu_llm_web/baichuan.py,sha256=fAuBHzrQ_fVJqSXBlnq49oDFlbS45DaIyrbNMnvx1cU,7135
 zibuyu_llm_web/base.py,sha256=s7GYbP70kKt7nhMLK0Jp22gVu2EfmS30eA5b6k_aYa8,7099
 zibuyu_llm_web/deepseek.py,sha256=Y_ewOKxagkwftYFjqOoMBsj1T-lXMOW3_yM6ccN6xr4,14808
-zibuyu_llm_web/errors.py,sha256=hX6XPbJeMCQ_SSMdC6ld9rIQpbZYFVJPj0qcNu12aPg,626
+zibuyu_llm_web/errors.py,sha256=Vib55tBOR1goqM7ddmx51TbJ8vKEXOCJEqcbvjTNaWw,732
 zibuyu_llm_web/kimi.py,sha256=SuG6u6FbZqD_AntxeXp3fuih2UMDtNzFbUSJSmeuoik,9907
 zibuyu_llm_web/minmax.py,sha256=Z_gPGiRdBOdg_2Xu_wfufItWLe-bR19CufykNZsxm74,37604
 zibuyu_llm_web/qwen.py,sha256=Iil5TckkFwroECpjC_Zf-PyZQ9iIbLKcSeSYOr_l3Lw,37630
 zibuyu_llm_web/types.py,sha256=xzN-TgzwMB0xZKFXusHxwpY2Eqm3iRBm2qMUmKzRm8I,5132
 zibuyu_llm_web/wanxiang.py,sha256=YU9R42VaxWlY7gpcT_qAkguSqhCfDuK19-lpWaWgRDA,8118
 zibuyu_llm_web/xinchen.py,sha256=PJAKtZCaj445CpVhUL035lhDuCH0NO5gdu0vyLuoymw,14465
 zibuyu_llm_web/xunfei.py,sha256=8gpfaPbzWEv1lK9Vlv_hXUKBfn0-ExaUsb0H6WqaULg,25562
-zibuyu_LLM-0.0.4.dist-info/METADATA,sha256=c5cJC_pWXHMr0LLIRQFvlm0I81uSn6tN_M4zmYxeFW8,1302
-zibuyu_LLM-0.0.4.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-zibuyu_LLM-0.0.4.dist-info/top_level.txt,sha256=QF6FI2Tcc78mYBpfy15YWDU-j16KK_2WqGF-3kj8Jew,30
-zibuyu_LLM-0.0.4.dist-info/RECORD,,
+zibuyu_LLM-0.0.5.dist-info/METADATA,sha256=AtiXKaDIhvQBcBnXwL9CWbxtir8CHtyKshTHaEE7VLo,1341
+zibuyu_LLM-0.0.5.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+zibuyu_LLM-0.0.5.dist-info/top_level.txt,sha256=QF6FI2Tcc78mYBpfy15YWDU-j16KK_2WqGF-3kj8Jew,30
+zibuyu_LLM-0.0.5.dist-info/RECORD,,
```

