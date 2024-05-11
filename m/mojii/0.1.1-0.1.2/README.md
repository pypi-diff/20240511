# Comparing `tmp/mojii-0.1.1-py3-none-any.whl.zip` & `tmp/mojii-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1500 bytes, number of entries: 6
+Zip file size: 1549 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-16 09:36 moji/__init__.py
--rw-rw-rw-  2.0 fat       35 b- defN 24-Apr-16 09:39 moji/moji.py
--rw-rw-rw-  2.0 fat      722 b- defN 24-May-02 22:37 mojii-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-02 22:37 mojii-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 24-May-02 22:37 mojii-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      425 b- defN 24-May-02 22:37 mojii-0.1.1.dist-info/RECORD
-6 files, 1279 bytes uncompressed, 726 bytes compressed:  43.2%
+-rw-rw-rw-  2.0 fat       94 b- defN 24-May-02 22:40 moji/moji.py
+-rw-rw-rw-  2.0 fat      722 b- defN 24-May-02 22:41 mojii-0.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-02 22:41 mojii-0.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 24-May-02 22:41 mojii-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      425 b- defN 24-May-02 22:41 mojii-0.1.2.dist-info/RECORD
+6 files, 1338 bytes uncompressed, 775 bytes compressed:  42.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: moji/__init__.py
 Comment: 
 
 Filename: moji/moji.py
 Comment: 
 
-Filename: mojii-0.1.1.dist-info/METADATA
+Filename: mojii-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: mojii-0.1.1.dist-info/WHEEL
+Filename: mojii-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: mojii-0.1.1.dist-info/top_level.txt
+Filename: mojii-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: mojii-0.1.1.dist-info/RECORD
+Filename: mojii-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## moji/moji.py

```diff
@@ -1,2 +1,7 @@
+import moji as s
 def a():
-    print('Hello World!')
+    print('Hello World!')
+
+
+if __name__ == '__main__':
+    a()
```

## Comparing `mojii-0.1.1.dist-info/METADATA` & `mojii-0.1.2.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mojii
-Version: 0.1.1
+Version: 0.1.2
 Summary: Demo library
 Author: Joffrey Bienvenu
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

