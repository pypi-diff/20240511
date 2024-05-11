# Comparing `tmp/cvxpy-1.5.0.tar.gz` & `tmp/cvxpy-1.5.1-cp38-cp38-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxpy-1.5.0.tar", last modified: Thu May  9 04:48:07 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

