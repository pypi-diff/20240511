# Comparing `tmp/pyaogmaneo-2.6.0.tar.gz` & `tmp/pyaogmaneo-2.6.1-cp312-cp312-win32.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaogmaneo-2.6.0.tar", last modified: Wed May  8 22:24:20 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

