# Comparing `tmp/sp_lh3_constant_contact-0.1.5.tar.gz` & `tmp/sp_lh3_constant_contact-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sp_lh3_constant_contact-0.1.5.tar", max compression
+gzip compressed data, was "sp_lh3_constant_contact-0.1.6.tar", max compression
```

## Comparing `sp_lh3_constant_contact-0.1.5.tar` & `sp_lh3_constant_contact-0.1.6.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      950 2024-05-11 03:36:53.906989 sp_lh3_constant_contact-0.1.5/README.md
--rw-r--r--   0        0        0      647 2024-05-11 03:36:31.909266 sp_lh3_constant_contact-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3087 2024-05-11 03:27:20.026236 sp_lh3_constant_contact-0.1.5/sp_lh3_constant_contact/__init__.py
--rw-r--r--   0        0        0     1783 1970-01-01 00:00:00.000000 sp_lh3_constant_contact-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      950 2024-05-11 03:36:53.906989 sp_lh3_constant_contact-0.1.6/README.md
+-rw-r--r--   0        0        0      647 2024-05-11 06:30:43.710335 sp_lh3_constant_contact-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3372 2024-05-11 06:29:08.540663 sp_lh3_constant_contact-0.1.6/sp_lh3_constant_contact/__init__.py
+-rw-r--r--   0        0        0     1783 1970-01-01 00:00:00.000000 sp_lh3_constant_contact-0.1.6/PKG-INFO
```

### Comparing `sp_lh3_constant_contact-0.1.5/README.md` & `sp_lh3_constant_contact-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `sp_lh3_constant_contact-0.1.5/pyproject.toml` & `sp_lh3_constant_contact-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sp-lh3-constant-contact"
-version = "0.1.5"
+version = "0.1.6"
 description = "This script will assess a transcript to check if the operator has taken more than 5 min to reply to any message from the patron"
 authors = ["Guinslym <guinslym@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/guinslym/sp_lh3_constant_contact"
 homepage = "https://github.com/guinslym/sp_lh3_constant_contact"
 
 [tool.poetry.dependencies]
```

### Comparing `sp_lh3_constant_contact-0.1.5/sp_lh3_constant_contact/__init__.py` & `sp_lh3_constant_contact-0.1.6/sp_lh3_constant_contact/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,15 +67,17 @@
                     )
 
                     # Print the message
                     # print(f"ChatId: {chat_id} - Student time: {previous_student_time} - Operator time:  {time} - {sender_type}: Message: {text}")
 
                     # reset the timer for students to avoid duplicates
                     previous_student_time = current_time
-
+                else:
+                    # reset the timer for students to avoid msg where operator has sent multiple message and that one of them is flag : nnonn-constant contact compare to the last time the student sent a msg
+                    previous_student_time = current_time
     # if discrepancies:
     # tprint(discrepancies)
     return discrepancies
 
 
 """
 def main():
```

### Comparing `sp_lh3_constant_contact-0.1.5/PKG-INFO` & `sp_lh3_constant_contact-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sp-lh3-constant-contact
-Version: 0.1.5
+Version: 0.1.6
 Summary: This script will assess a transcript to check if the operator has taken more than 5 min to reply to any message from the patron
 Home-page: https://github.com/guinslym/sp_lh3_constant_contact
 Author: Guinslym
 Author-email: guinslym@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

