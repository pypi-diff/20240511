# Comparing `tmp/extensionmigrationassistant-0.1.0.tar.gz` & `tmp/extensionmigrationassistant-0.1.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extensionmigrationassistant-0.1.0.tar", last modified: Sat May 11 12:06:16 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

