# Comparing `tmp/kuzu-0.4.2.dev3.tar.gz` & `tmp/kuzu-0.4.2.dev4-cp39-cp39-manylinux_2_27_aarch64.manylinux_2_28_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuzu-0.4.2.dev3.tar", last modified: Fri May 10 08:05:00 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

