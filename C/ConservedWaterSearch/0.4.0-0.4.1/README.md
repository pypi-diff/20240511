# Comparing `tmp/ConservedWaterSearch-0.4.0.tar.gz` & `tmp/ConservedWaterSearch-0.4.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ConservedWaterSearch-0.4.0.tar", last modified: Tue Apr  9 21:06:40 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

