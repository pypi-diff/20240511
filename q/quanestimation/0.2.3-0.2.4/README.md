# Comparing `tmp/quanestimation-0.2.3.tar.gz` & `tmp/quanestimation-0.2.4-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quanestimation-0.2.3.tar", last modified: Thu Mar 21 15:45:55 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

