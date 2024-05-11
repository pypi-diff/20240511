# Comparing `tmp/codefly_sdk-0.0.8.tar.gz` & `tmp/codefly_sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codefly_sdk-0.0.8.tar", max compression
+gzip compressed data, was "codefly_sdk-0.0.9.tar", max compression
```

## Comparing `codefly_sdk-0.0.8.tar` & `codefly_sdk-0.0.9.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2024-01-15 12:50:49.311456 codefly_sdk-0.0.8/codefly/__init__.py
--rw-r--r--   0        0        0     5335 2024-03-27 13:34:54.300470 codefly_sdk-0.0.8/codefly/codefly.py
--rw-r--r--   0        0        0      393 2024-03-27 13:36:16.752309 codefly_sdk-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      444 1970-01-01 00:00:00.000000 codefly_sdk-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-01-15 12:50:49.311456 codefly_sdk-0.0.9/codefly/__init__.py
+-rw-r--r--   0        0        0     5507 2024-03-28 21:52:46.367234 codefly_sdk-0.0.9/codefly/codefly.py
+-rw-r--r--   0        0        0      393 2024-03-29 14:46:40.039816 codefly_sdk-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      444 1970-01-01 00:00:00.000000 codefly_sdk-0.0.9/PKG-INFO
```

### Comparing `codefly_sdk-0.0.8/codefly/codefly.py` & `codefly_sdk-0.0.9/codefly/codefly.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,24 +92,33 @@
 
 
 def decode_base64(data: str) -> str:
     decoded_bytes = base64.b64decode(data)
     return decoded_bytes.decode('utf-8')
 
 
-def configuration(name: str = None, key: str = None, service: Optional[str] = None, application: Optional[str] = None) -> Optional[str]:
+def is_running() -> bool:
+    """Returns true if we are in running mode."""
+    key = "CODEFLY__RUNNING"
+    return os.getenv(key) is not None
+
+
+def configuration(name: str = None, key: str = None, service: Optional[str] = None,
+                  application: Optional[str] = None) -> Optional[str]:
     if not name:
         raise KeyError("name is required")
     if not key:
         raise KeyError("key is required")
     if service:
         return _get_service_configuration(service, name, key, application=application)
     return _get_project_configuration(name, key)
 
-def secret(name: str = None, key: str = None, service: Optional[str] = None, application: Optional[str] = None) -> Optional[str]:
+
+def secret(name: str = None, key: str = None, service: Optional[str] = None, application: Optional[str] = None) -> \
+        Optional[str]:
     if not name:
         raise KeyError("name is required")
     if not key:
         raise KeyError("key is required")
     if service:
         return _get_service_configuration(service, name, key, application=application, is_secret=True)
     return _get_project_configuration(name, key, is_secret=True)
@@ -145,16 +154,14 @@
     print(key)
     value = os.getenv(key)
     if not value:
         return None
     return decode_base64(value)
 
 
-
-
 def user_id_from_headers(headers: Dict[str, str]) -> Optional[str]:
     return headers.get("X-CODEFLY-USER-ID")
 
 
 def user_email_from_headers(headers: Dict[str, str]) -> Optional[str]:
     return headers.get("X-CODEFLY-USER-EMAIL")
```

