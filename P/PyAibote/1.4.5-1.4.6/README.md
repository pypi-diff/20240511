# Comparing `tmp/PyAibote-1.4.5.tar.gz` & `tmp/PyAibote-1.4.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyAibote-1.4.5.tar", last modified: Tue Apr 30 06:53:58 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

