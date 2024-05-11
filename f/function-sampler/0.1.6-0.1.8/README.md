# Comparing `tmp/function_sampler-0.1.6.tar.gz` & `tmp/function_sampler-0.1.8-cp311-cp311-manylinux_2_28_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "function_sampler-0.1.6.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

