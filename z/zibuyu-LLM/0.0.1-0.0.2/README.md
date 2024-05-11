# Comparing `tmp/zibuyu_LLM-0.0.1-py3-none-any.whl.zip` & `tmp/zibuyu_LLM-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 56719 bytes, number of entries: 16
+Zip file size: 57002 bytes, number of entries: 16
 -rw-rw-rw-  2.0 fat      241 b- defN 24-May-09 06:10 api/__init__.py
 -rw-rw-rw-  2.0 fat    32008 b- defN 24-May-06 10:01 api/minmax_api.py
 -rw-rw-rw-  2.0 fat      241 b- defN 24-May-09 06:09 web/__init__.py
 -rw-rw-rw-  2.0 fat     7155 b- defN 24-May-09 06:22 web/baichuan.py
 -rw-rw-rw-  2.0 fat     7099 b- defN 24-May-11 01:45 web/base.py
 -rw-rw-rw-  2.0 fat    14828 b- defN 24-May-09 13:49 web/deepseek.py
 -rw-rw-rw-  2.0 fat     9927 b- defN 24-May-09 13:53 web/kimi.py
 -rw-rw-rw-  2.0 fat    37591 b- defN 24-May-09 16:21 web/minmax.py
 -rw-rw-rw-  2.0 fat    37650 b- defN 24-May-10 11:10 web/qwen.py
 -rw-rw-rw-  2.0 fat     8138 b- defN 24-May-09 06:22 web/wanxiang.py
 -rw-rw-rw-  2.0 fat    14485 b- defN 24-May-10 11:12 web/xinchen.py
 -rw-rw-rw-  2.0 fat    25572 b- defN 24-May-11 02:18 web/xunfei.py
--rw-rw-rw-  2.0 fat      883 b- defN 24-May-11 05:25 zibuyu_LLM-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-11 05:25 zibuyu_LLM-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 24-May-11 05:25 zibuyu_LLM-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1161 b- defN 24-May-11 05:25 zibuyu_LLM-0.0.1.dist-info/RECORD
-16 files, 197079 bytes uncompressed, 54871 bytes compressed:  72.2%
+-rw-rw-rw-  2.0 fat     1226 b- defN 24-May-11 06:56 zibuyu_LLM-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-11 06:56 zibuyu_LLM-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 24-May-11 06:56 zibuyu_LLM-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1162 b- defN 24-May-11 06:56 zibuyu_LLM-0.0.2.dist-info/RECORD
+16 files, 197423 bytes uncompressed, 55154 bytes compressed:  72.1%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: web/xinchen.py
 Comment: 
 
 Filename: web/xunfei.py
 Comment: 
 
-Filename: zibuyu_LLM-0.0.1.dist-info/METADATA
+Filename: zibuyu_LLM-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: zibuyu_LLM-0.0.1.dist-info/WHEEL
+Filename: zibuyu_LLM-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: zibuyu_LLM-0.0.1.dist-info/top_level.txt
+Filename: zibuyu_LLM-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: zibuyu_LLM-0.0.1.dist-info/RECORD
+Filename: zibuyu_LLM-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `zibuyu_LLM-0.0.1.dist-info/RECORD` & `zibuyu_LLM-0.0.2.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -6,11 +6,11 @@
 web/deepseek.py,sha256=PEVDXpV1qjVLMShz3Bd0LG0SnUkW5HkLhut4bYkP464,14828
 web/kimi.py,sha256=RxVO6azaT7Xw-hobl8k6kdzXkzMVUh-YOt8jFDe_CPk,9927
 web/minmax.py,sha256=MGKgSdsamZQgk7bFxdrKVgzAHgw6TW9F252eXh5w6IU,37591
 web/qwen.py,sha256=zgxDa-MsYdgoLNahaco_1DfX6duhEaaN8E7gT77H0mw,37650
 web/wanxiang.py,sha256=ML92G-1KpvAkSGUZujOHDEX-iHm6fzuPPe3Lq_6mLxw,8138
 web/xinchen.py,sha256=BmJdcFykMKnLdUUu5TvfEg2BCdcOZ19kqDpi9suB3X8,14485
 web/xunfei.py,sha256=kNnHPs__p07mf5_a3-9zdUyPKDHK7DGMFa_2Dee5b1w,25572
-zibuyu_LLM-0.0.1.dist-info/METADATA,sha256=BIFLg1-sgtMBtDMJcNE68q5TE-3Lpdx3PDeWle10Bzw,883
-zibuyu_LLM-0.0.1.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-zibuyu_LLM-0.0.1.dist-info/top_level.txt,sha256=lpfVTTvr_OnoRgurRAaARNiZCC1Z79GYsRHW_WiC5J8,8
-zibuyu_LLM-0.0.1.dist-info/RECORD,,
+zibuyu_LLM-0.0.2.dist-info/METADATA,sha256=bWBvr5ahI-M1qVYvVfYhO5mIUmKEF8xWUz82rsLn5Vk,1226
+zibuyu_LLM-0.0.2.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+zibuyu_LLM-0.0.2.dist-info/top_level.txt,sha256=lpfVTTvr_OnoRgurRAaARNiZCC1Z79GYsRHW_WiC5J8,8
+zibuyu_LLM-0.0.2.dist-info/RECORD,,
```

