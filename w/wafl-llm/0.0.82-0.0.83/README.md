# Comparing `tmp/wafl_llm-0.0.82.tar.gz` & `tmp/wafl_llm-0.0.83-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wafl_llm-0.0.82.tar", last modified: Sat Jan 27 15:10:04 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

