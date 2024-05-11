# Comparing `tmp/xss_shield-0.1.1.tar.gz` & `tmp/xss_shield-0.1.2.tar.gz`

## Comparing `xss_shield-0.1.1.tar` & `xss_shield-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,7 @@
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 xss_shield-0.1.1/.github/workflows/python-app.yml
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 xss_shield-0.1.1/examples/example.ipynb
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 xss_shield-0.1.1/src/xss_shield/__init__.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 xss_shield-0.1.1/test/test_escape.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 xss_shield-0.1.1/.gitignore
--rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 xss_shield-0.1.1/LICENSE
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 xss_shield-0.1.1/README.md
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 xss_shield-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 xss_shield-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 xss_shield-0.1.2/examples/example.ipynb
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 xss_shield-0.1.2/src/xss_shield/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 xss_shield-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 xss_shield-0.1.2/LICENSE
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xss_shield-0.1.2/README.md
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 xss_shield-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 xss_shield-0.1.2/PKG-INFO
```

### Comparing `xss_shield-0.1.1/examples/example.ipynb` & `xss_shield-0.1.2/examples/example.ipynb`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9774305555555556%*

 * *Differences: {"'cells'": "{0: {'execution_count': 1, 'id': 'ca6cd635-e99a-499d-bca9-53e60c87fe4c', 'outputs': "*

 * *            "{0: {'text': ['&lt;script&gt;alert(&#34;Bad.&#34;)&#59;&lt;&#47;script&gt;\\n']}}}}"}*

```diff
@@ -1,20 +1,20 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 5,
-            "id": "5f41eab9-0fc3-43eb-add1-18f9ad56dc14",
+            "execution_count": 1,
+            "id": "ca6cd635-e99a-499d-bca9-53e60c87fe4c",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "&ampltscript&ampgtalert(&#34&#59Bad.&#34&#59)&#59&amplt/script&ampgt\n"
+                        "&lt;script&gt;alert(&#34;Bad.&#34;)&#59;&lt;&#47;script&gt;\n"
                     ]
                 }
             ],
             "source": [
                 "import xss_shield\n",
                 "unsafe_str = '<script>alert(\"Bad.\");</script>'\n",
                 "safe_str = xss_shield.escape(unsafe_str)\n",
```

### Comparing `xss_shield-0.1.1/.gitignore` & `xss_shield-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `xss_shield-0.1.1/pyproject.toml` & `xss_shield-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "xss-shield"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Gordon Zhang", email="jp20171211@163.com" },
 ]
 description = "A library used to stop your website from being attacked."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)",
+    "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 Homepage = "https://github.com/GordonZhang2024/xss-shield/"
 Issues = "https://github.com/GordonZhang2024/xss-shield/issues"
```

