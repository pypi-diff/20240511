# Comparing `tmp/customtkintermessagebox-0.0.1.tar.gz` & `tmp/customtkintermessagebox-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customtkintermessagebox-0.0.1.tar", last modified: Sat May 11 16:59:04 2024, max compression
+gzip compressed data, was "customtkintermessagebox-0.0.2.tar", last modified: Sat May 11 17:07:32 2024, max compression
```

## Comparing `customtkintermessagebox-0.0.1.tar` & `customtkintermessagebox-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 16:59:04.943999 customtkintermessagebox-0.0.1/
-drwxrwxrwx   0        0        0        0 2024-05-11 16:59:04.884717 customtkintermessagebox-0.0.1/CustomTkinterMessagebox/
--rw-rw-rw-   0        0        0       25 2024-05-11 14:56:39.000000 customtkintermessagebox-0.0.1/CustomTkinterMessagebox/__init__.py
--rw-rw-rw-   0        0        0     2027 2024-05-11 16:03:23.000000 customtkintermessagebox-0.0.1/CustomTkinterMessagebox/messagebox.py
-drwxrwxrwx   0        0        0        0 2024-05-11 16:59:04.943999 customtkintermessagebox-0.0.1/CustomTkinterMessagebox.egg-info/
--rw-rw-rw-   0        0        0     5839 2024-05-11 16:59:04.000000 customtkintermessagebox-0.0.1/CustomTkinterMessagebox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2024-05-11 16:59:04.000000 customtkintermessagebox-0.0.1/CustomTkinterMessagebox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 16:59:04.000000 customtkintermessagebox-0.0.1/CustomTkinterMessagebox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2024-05-11 16:59:04.000000 customtkintermessagebox-0.0.1/CustomTkinterMessagebox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-11 16:59:04.000000 customtkintermessagebox-0.0.1/CustomTkinterMessagebox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1106 2024-05-11 15:01:43.000000 customtkintermessagebox-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     5839 2024-05-11 16:59:04.943999 customtkintermessagebox-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1281 2024-05-11 16:01:37.000000 customtkintermessagebox-0.0.1/examples.py
--rw-rw-rw-   0        0        0       42 2024-05-11 16:59:04.943999 customtkintermessagebox-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      514 2024-05-11 16:58:40.000000 customtkintermessagebox-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 17:07:32.094369 customtkintermessagebox-0.0.2/
+drwxrwxrwx   0        0        0        0 2024-05-11 17:07:32.051295 customtkintermessagebox-0.0.2/CustomTkinterMessagebox/
+-rw-rw-rw-   0        0        0       25 2024-05-11 14:56:39.000000 customtkintermessagebox-0.0.2/CustomTkinterMessagebox/__init__.py
+-rw-rw-rw-   0        0        0     2027 2024-05-11 16:03:23.000000 customtkintermessagebox-0.0.2/CustomTkinterMessagebox/messagebox.py
+drwxrwxrwx   0        0        0        0 2024-05-11 17:07:32.091929 customtkintermessagebox-0.0.2/CustomTkinterMessagebox.egg-info/
+-rw-rw-rw-   0        0        0     5839 2024-05-11 17:07:31.000000 customtkintermessagebox-0.0.2/CustomTkinterMessagebox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2024-05-11 17:07:31.000000 customtkintermessagebox-0.0.2/CustomTkinterMessagebox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 17:07:31.000000 customtkintermessagebox-0.0.2/CustomTkinterMessagebox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2024-05-11 17:07:31.000000 customtkintermessagebox-0.0.2/CustomTkinterMessagebox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-11 17:07:31.000000 customtkintermessagebox-0.0.2/CustomTkinterMessagebox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1106 2024-05-11 15:01:43.000000 customtkintermessagebox-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     5839 2024-05-11 17:07:32.092571 customtkintermessagebox-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1281 2024-05-11 16:01:37.000000 customtkintermessagebox-0.0.2/examples.py
+-rw-rw-rw-   0        0        0       42 2024-05-11 17:07:32.094369 customtkintermessagebox-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      470 2024-05-11 17:07:05.000000 customtkintermessagebox-0.0.2/setup.py
```

### Comparing `customtkintermessagebox-0.0.1/CustomTkinterMessagebox/messagebox.py` & `customtkintermessagebox-0.0.2/CustomTkinterMessagebox/messagebox.py`

 * *Files identical despite different names*

### Comparing `customtkintermessagebox-0.0.1/CustomTkinterMessagebox.egg-info/PKG-INFO` & `customtkintermessagebox-0.0.2/CustomTkinterMessagebox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CustomTkinterMessagebox
-Version: 0.0.1
+Version: 0.0.2
 Summary: Messagebox for CustomTkinter
 Author: Jorge Magno
 Author-email: jorge.estudos0@gmail.com
 License: MIT License
 Keywords: customtkinter
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `customtkintermessagebox-0.0.1/LICENSE` & `customtkintermessagebox-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `customtkintermessagebox-0.0.1/PKG-INFO` & `customtkintermessagebox-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CustomTkinterMessagebox
-Version: 0.0.1
+Version: 0.0.2
 Summary: Messagebox for CustomTkinter
 Author: Jorge Magno
 Author-email: jorge.estudos0@gmail.com
 License: MIT License
 Keywords: customtkinter
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `customtkintermessagebox-0.0.1/examples.py` & `customtkintermessagebox-0.0.2/examples.py`

 * *Files identical despite different names*
