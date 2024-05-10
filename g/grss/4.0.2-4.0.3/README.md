# Comparing `tmp/grss-4.0.2.tar.gz` & `tmp/grss-4.0.3-cp312-cp312-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grss-4.0.2.tar", last modified: Sat Apr 27 18:54:56 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

