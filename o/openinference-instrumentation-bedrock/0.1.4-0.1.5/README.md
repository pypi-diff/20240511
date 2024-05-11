# Comparing `tmp/openinference_instrumentation_bedrock-0.1.4.tar.gz` & `tmp/openinference_instrumentation_bedrock-0.1.5.tar.gz`

## Comparing `openinference_instrumentation_bedrock-0.1.4.tar` & `openinference_instrumentation_bedrock-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     7938 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.4/src/openinference/instrumentation/bedrock/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.4/src/openinference/instrumentation/bedrock/package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.4/src/openinference/instrumentation/bedrock/py.typed
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.4/src/openinference/instrumentation/bedrock/version.py
--rw-r--r--   0        0        0    11168 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.4/tests/test_instrumentor.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.4/.gitignore
--rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.4/LICENSE
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.4/README.md
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     8052 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.5/src/openinference/instrumentation/bedrock/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.5/src/openinference/instrumentation/bedrock/package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.5/src/openinference/instrumentation/bedrock/py.typed
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.5/src/openinference/instrumentation/bedrock/version.py
+-rw-r--r--   0        0        0    11168 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.5/tests/test_instrumentor.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.5/.gitignore
+-rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.5/README.md
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.5/PKG-INFO
```

### Comparing `openinference_instrumentation_bedrock-0.1.4/src/openinference/instrumentation/bedrock/__init__.py` & `openinference_instrumentation_bedrock-0.1.5/src/openinference/instrumentation/bedrock/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,14 +143,16 @@
 
                     if vendor == "ai21":
                         content = str(response_body.get("completions"))
                     elif vendor == "anthropic":
                         content = str(response_body.get("completion"))
                     elif vendor == "cohere":
                         content = str(response_body.get("generations"))
+                    elif vendor == "meta":
+                        content = str(response_body.get("generation"))
                     else:
                         content = ""
 
                     if content:
                         _set_span_attribute(span, SpanAttributes.OUTPUT_VALUE, content)
 
                 span.set_attributes(dict(get_attributes_from_context()))
```

### Comparing `openinference_instrumentation_bedrock-0.1.4/tests/test_instrumentor.py` & `openinference_instrumentation_bedrock-0.1.5/tests/test_instrumentor.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_bedrock-0.1.4/LICENSE` & `openinference_instrumentation_bedrock-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_bedrock-0.1.4/README.md` & `openinference_instrumentation_bedrock-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_bedrock-0.1.4/pyproject.toml` & `openinference_instrumentation_bedrock-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_bedrock-0.1.4/PKG-INFO` & `openinference_instrumentation_bedrock-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: openinference-instrumentation-bedrock
-Version: 0.1.4
+Version: 0.1.5
 Summary: OpenInference Bedrock Instrumentation
 Project-URL: Homepage, https://github.com/Arize-ai/openinference/tree/main/python/instrumentation/openinference-instrumentation-bedrock
 Author-email: OpenInference Authors <oss@arize.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

