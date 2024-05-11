# Comparing `tmp/spatium-1.5.4.tar.gz` & `tmp/spatium-1.5.5-cp310-cp310-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatium-1.5.4.tar", last modified: Thu May  9 01:57:04 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

