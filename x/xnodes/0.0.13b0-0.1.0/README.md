# Comparing `tmp/xnodes-0.0.13b0.tar.gz` & `tmp/xnodes-0.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xnodes-0.0.13b0.tar", last modified: Thu Aug 10 11:13:00 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

