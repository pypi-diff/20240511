# Comparing `tmp/veracode_api_py-0.9.8.tar.gz` & `tmp/veracode_api_py-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veracode_api_py-0.9.8.tar", last modified: Wed Feb 24 14:30:46 2021, max compression
+gzip compressed data, was "veracode_api_py-0.9.9.tar", last modified: Wed Feb 24 14:57:48 2021, max compression
```

## Comparing `veracode_api_py-0.9.8.tar` & `veracode_api_py-0.9.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 tjarrett-admin   (502) staff       (20)        0 2021-02-24 14:30:46.627880 veracode_api_py-0.9.8/
--rw-r--r--   0 tjarrett-admin   (502) staff       (20)      725 2021-02-24 14:30:46.627983 veracode_api_py-0.9.8/PKG-INFO
--rw-r--r--   0 tjarrett-admin   (502) staff       (20)       39 2020-09-03 16:58:47.000000 veracode_api_py-0.9.8/setup.cfg
--rw-r--r--   0 tjarrett-admin   (502) staff       (20)     1045 2021-02-24 14:25:11.168770 veracode_api_py-0.9.8/setup.py
-drwxr-xr-x   0 tjarrett-admin   (502) staff       (20)        0 2021-02-24 14:30:46.627792 veracode_api_py-0.9.8/veracode_api_py/
--rw-r--r--   0 tjarrett-admin   (502) staff       (20)      533 2021-02-09 17:38:39.607963 veracode_api_py-0.9.8/veracode_api_py/__init__.py
--rw-r--r--   0 tjarrett-admin   (502) staff       (20)    10688 2021-02-24 14:23:18.788960 veracode_api_py-0.9.8/veracode_api_py/api.py
--rw-r--r--   0 tjarrett-admin   (502) staff       (20)     5756 2021-02-24 13:53:19.422605 veracode_api_py-0.9.8/veracode_api_py/apihelper.py
--rw-r--r--   0 tjarrett-admin   (502) staff       (20)     3901 2021-02-09 17:38:39.610070 veracode_api_py-0.9.8/veracode_api_py/applications.py
--rw-r--r--   0 tjarrett-admin   (502) staff       (20)     3291 2021-02-09 17:40:03.058683 veracode_api_py-0.9.8/veracode_api_py/collections.py
--rw-r--r--   0 tjarrett-admin   (502) staff       (20)      633 2021-02-09 17:38:39.611335 veracode_api_py-0.9.8/veracode_api_py/constants.py
--rw-r--r--   0 tjarrett-admin   (502) staff       (20)      231 2020-09-03 16:27:53.000000 veracode_api_py-0.9.8/veracode_api_py/exceptions.py
--rw-r--r--   0 tjarrett-admin   (502) staff       (20)     2293 2021-02-24 13:55:14.846231 veracode_api_py-0.9.8/veracode_api_py/findings.py
--rw-r--r--   0 tjarrett-admin   (502) staff       (20)      375 2021-02-24 13:58:59.927372 veracode_api_py-0.9.8/veracode_api_py/healthcheck.py
--rw-r--r--   0 tjarrett-admin   (502) staff       (20)     7284 2021-02-24 14:30:37.701791 veracode_api_py-0.9.8/veracode_api_py/identity.py
--rw-r--r--   0 tjarrett-admin   (502) staff       (20)      823 2021-02-09 17:38:39.613839 veracode_api_py-0.9.8/veracode_api_py/log.py
--rw-r--r--   0 tjarrett-admin   (502) staff       (20)     3053 2021-02-09 17:38:39.614392 veracode_api_py-0.9.8/veracode_api_py/policy.py
--rw-r--r--   0 tjarrett-admin   (502) staff       (20)     6015 2021-02-09 17:38:39.615153 veracode_api_py-0.9.8/veracode_api_py/sca.py
--rw-r--r--   0 tjarrett-admin   (502) staff       (20)     2644 2021-02-09 17:38:39.615651 veracode_api_py-0.9.8/veracode_api_py/xmlapi.py
+drwxr-xr-x   0 tjarrett-admin   (502) staff       (20)        0 2021-02-24 14:57:48.044315 veracode_api_py-0.9.9/
+-rw-r--r--   0 tjarrett-admin   (502) staff       (20)      725 2021-02-24 14:57:48.044455 veracode_api_py-0.9.9/PKG-INFO
+-rw-r--r--   0 tjarrett-admin   (502) staff       (20)       39 2020-09-03 16:58:47.000000 veracode_api_py-0.9.9/setup.cfg
+-rw-r--r--   0 tjarrett-admin   (502) staff       (20)     1045 2021-02-24 14:56:40.111111 veracode_api_py-0.9.9/setup.py
+drwxr-xr-x   0 tjarrett-admin   (502) staff       (20)        0 2021-02-24 14:57:48.044230 veracode_api_py-0.9.9/veracode_api_py/
+-rw-r--r--   0 tjarrett-admin   (502) staff       (20)      533 2021-02-09 17:38:39.607963 veracode_api_py-0.9.9/veracode_api_py/__init__.py
+-rw-r--r--   0 tjarrett-admin   (502) staff       (20)    10709 2021-02-24 14:55:44.030860 veracode_api_py-0.9.9/veracode_api_py/api.py
+-rw-r--r--   0 tjarrett-admin   (502) staff       (20)     5756 2021-02-24 13:53:19.422605 veracode_api_py-0.9.9/veracode_api_py/apihelper.py
+-rw-r--r--   0 tjarrett-admin   (502) staff       (20)     3901 2021-02-09 17:38:39.610070 veracode_api_py-0.9.9/veracode_api_py/applications.py
+-rw-r--r--   0 tjarrett-admin   (502) staff       (20)     3291 2021-02-09 17:40:03.058683 veracode_api_py-0.9.9/veracode_api_py/collections.py
+-rw-r--r--   0 tjarrett-admin   (502) staff       (20)      633 2021-02-09 17:38:39.611335 veracode_api_py-0.9.9/veracode_api_py/constants.py
+-rw-r--r--   0 tjarrett-admin   (502) staff       (20)      231 2020-09-03 16:27:53.000000 veracode_api_py-0.9.9/veracode_api_py/exceptions.py
+-rw-r--r--   0 tjarrett-admin   (502) staff       (20)     2391 2021-02-24 14:54:10.447673 veracode_api_py-0.9.9/veracode_api_py/findings.py
+-rw-r--r--   0 tjarrett-admin   (502) staff       (20)      375 2021-02-24 13:58:59.927372 veracode_api_py-0.9.9/veracode_api_py/healthcheck.py
+-rw-r--r--   0 tjarrett-admin   (502) staff       (20)     7284 2021-02-24 14:30:37.701791 veracode_api_py-0.9.9/veracode_api_py/identity.py
+-rw-r--r--   0 tjarrett-admin   (502) staff       (20)      823 2021-02-09 17:38:39.613839 veracode_api_py-0.9.9/veracode_api_py/log.py
+-rw-r--r--   0 tjarrett-admin   (502) staff       (20)     3053 2021-02-09 17:38:39.614392 veracode_api_py-0.9.9/veracode_api_py/policy.py
+-rw-r--r--   0 tjarrett-admin   (502) staff       (20)     6015 2021-02-09 17:38:39.615153 veracode_api_py-0.9.9/veracode_api_py/sca.py
+-rw-r--r--   0 tjarrett-admin   (502) staff       (20)     2644 2021-02-09 17:38:39.615651 veracode_api_py-0.9.9/veracode_api_py/xmlapi.py
```

### Comparing `veracode_api_py-0.9.8/PKG-INFO` & `veracode_api_py-0.9.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: veracode_api_py
-Version: 0.9.8
+Version: 0.9.9
 Summary: Python helper library for working with the Veracode APIs. Handles retries, pagination, and other features of the modern Veracode REST APIs.
 Home-page: https://github.com/tjarrettveracode
 Author: Tim Jarrett
 Author-email: tjarrett@veracode.com
 License: MIT
 Download-URL: https://github.com/tjarrettveracode/veracode-api-py/archive/v_094.tar.gz
 Description: UNKNOWN
```

### Comparing `veracode_api_py-0.9.8/setup.py` & `veracode_api_py-0.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
   name = 'veracode_api_py',         
   packages = ['veracode_api_py'],   
-  version = '0.9.8',      
+  version = '0.9.9',      
   license='MIT',        
   description = 'Python helper library for working with the Veracode APIs. Handles retries, pagination, and other features of the modern Veracode REST APIs.',   
   author = 'Tim Jarrett',                  
   author_email = 'tjarrett@veracode.com',      
   url = 'https://github.com/tjarrettveracode',   
   download_url = 'https://github.com/tjarrettveracode/veracode-api-py/archive/v_094.tar.gz',    
   keywords = ['veracode', 'veracode-api'],
```

### Comparing `veracode_api_py-0.9.8/veracode_api_py/__init__.py` & `veracode_api_py-0.9.9/veracode_api_py/__init__.py`

 * *Files identical despite different names*

### Comparing `veracode_api_py-0.9.8/veracode_api_py/api.py` & `veracode_api_py-0.9.9/veracode_api_py/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,16 +133,16 @@
 
     def get_dynamic_flaw_info(self,app,issueid):
         return Findings().get_dynamic_flaw_info(app,issueid)
 
     def get_summary_report(self,app,sandbox=None):
         return SummaryReport().get_summary_report(app,sandbox)
 
-    def add_annotation(self,app,issue_list,comment,action):
-        return Findings().add_annotation(app,issue_list,comment,action)
+    def add_annotation(self,app,issue_list,comment,action,sandbox=None):
+        return Findings().add_annotation(app,issue_list,comment,action,sandbox)
 
     ## Collections APIs
 
     def get_collections(self):
         return Collections().get_all()
 
     def get_collections_by_name(self,collection_name):
```

### Comparing `veracode_api_py-0.9.8/veracode_api_py/apihelper.py` & `veracode_api_py-0.9.9/veracode_api_py/apihelper.py`

 * *Files identical despite different names*

### Comparing `veracode_api_py-0.9.8/veracode_api_py/applications.py` & `veracode_api_py-0.9.9/veracode_api_py/applications.py`

 * *Files identical despite different names*

### Comparing `veracode_api_py-0.9.8/veracode_api_py/collections.py` & `veracode_api_py-0.9.9/veracode_api_py/collections.py`

 * *Files identical despite different names*

### Comparing `veracode_api_py-0.9.8/veracode_api_py/constants.py` & `veracode_api_py-0.9.9/veracode_api_py/constants.py`

 * *Files identical despite different names*

### Comparing `veracode_api_py-0.9.8/veracode_api_py/findings.py` & `veracode_api_py-0.9.9/veracode_api_py/findings.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,26 +30,29 @@
 
         return APIHelper()._rest_request(uri,"GET")
 
     def get_dynamic_flaw_info(self,app,issueid):
         uri = "appsec/v2/applications/{}/findings/{}/dynamic_flaw_info".format(app,issueid)
         return APIHelper()._rest_request(uri,"GET")
 
-    def add_annotation(self,app,issue_list,comment,action):
+    def add_annotation(self,app,issue_list,comment,action,sandbox=None):
         #pass issue_list as a list of issue ids
         uri = "appsec/v2/applications/{}/annotations".format(app)
 
+        if sandbox != None:
+            params = {'context': sandbox}
+
         annotation_def = {'comment': comment, 'action': action}
 
         converted_list = [str(element) for element in issue_list]
         issue_list_string = ','.join(converted_list)
         annotation_def['issue_list'] = issue_list_string 
         
         payload = json.dumps(annotation_def)
-        return APIHelper()._rest_request(uri,"POST",body=payload)
+        return APIHelper()._rest_request(uri,"POST",body=payload,params=params)
 
 class SummaryReport():
     def get_summary_report(self,app,sandbox=None):
         if sandbox != None:
             uri = "appsec/v2/applications/{}/summary_report?context={}".format(app,sandbox)
         else:
             uri = "appsec/v2/applications/{}/summary_report".format(app)
```

### Comparing `veracode_api_py-0.9.8/veracode_api_py/identity.py` & `veracode_api_py-0.9.9/veracode_api_py/identity.py`

 * *Files identical despite different names*

### Comparing `veracode_api_py-0.9.8/veracode_api_py/log.py` & `veracode_api_py-0.9.9/veracode_api_py/log.py`

 * *Files identical despite different names*

### Comparing `veracode_api_py-0.9.8/veracode_api_py/policy.py` & `veracode_api_py-0.9.9/veracode_api_py/policy.py`

 * *Files identical despite different names*

### Comparing `veracode_api_py-0.9.8/veracode_api_py/sca.py` & `veracode_api_py-0.9.9/veracode_api_py/sca.py`

 * *Files identical despite different names*

### Comparing `veracode_api_py-0.9.8/veracode_api_py/xmlapi.py` & `veracode_api_py-0.9.9/veracode_api_py/xmlapi.py`

 * *Files identical despite different names*

