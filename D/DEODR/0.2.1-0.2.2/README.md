# Comparing `tmp/DEODR-0.2.1.tar.gz` & `tmp/DEODR-0.2.2-cp312-cp312-musllinux_1_1_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DEODR-0.2.1.tar", last modified: Sun Jul 16 11:04:30 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

