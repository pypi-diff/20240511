# Comparing `tmp/customtkintermessagebox-0.0.2.tar.gz` & `tmp/customtkintermessagebox-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customtkintermessagebox-0.0.2.tar", last modified: Sat May 11 17:07:32 2024, max compression
+gzip compressed data, was "customtkintermessagebox-0.0.3.tar", last modified: Sat May 11 17:14:02 2024, max compression
```

## Comparing `customtkintermessagebox-0.0.2.tar` & `customtkintermessagebox-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 17:07:32.094369 customtkintermessagebox-0.0.2/
-drwxrwxrwx   0        0        0        0 2024-05-11 17:07:32.051295 customtkintermessagebox-0.0.2/CustomTkinterMessagebox/
--rw-rw-rw-   0        0        0       25 2024-05-11 14:56:39.000000 customtkintermessagebox-0.0.2/CustomTkinterMessagebox/__init__.py
--rw-rw-rw-   0        0        0     2027 2024-05-11 16:03:23.000000 customtkintermessagebox-0.0.2/CustomTkinterMessagebox/messagebox.py
-drwxrwxrwx   0        0        0        0 2024-05-11 17:07:32.091929 customtkintermessagebox-0.0.2/CustomTkinterMessagebox.egg-info/
--rw-rw-rw-   0        0        0     5839 2024-05-11 17:07:31.000000 customtkintermessagebox-0.0.2/CustomTkinterMessagebox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2024-05-11 17:07:31.000000 customtkintermessagebox-0.0.2/CustomTkinterMessagebox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 17:07:31.000000 customtkintermessagebox-0.0.2/CustomTkinterMessagebox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2024-05-11 17:07:31.000000 customtkintermessagebox-0.0.2/CustomTkinterMessagebox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-11 17:07:31.000000 customtkintermessagebox-0.0.2/CustomTkinterMessagebox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1106 2024-05-11 15:01:43.000000 customtkintermessagebox-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     5839 2024-05-11 17:07:32.092571 customtkintermessagebox-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1281 2024-05-11 16:01:37.000000 customtkintermessagebox-0.0.2/examples.py
--rw-rw-rw-   0        0        0       42 2024-05-11 17:07:32.094369 customtkintermessagebox-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      470 2024-05-11 17:07:05.000000 customtkintermessagebox-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 17:14:02.669749 customtkintermessagebox-0.0.3/
+drwxrwxrwx   0        0        0        0 2024-05-11 17:14:02.639021 customtkintermessagebox-0.0.3/CustomTkinterMessagebox/
+-rw-rw-rw-   0        0        0       25 2024-05-11 14:56:39.000000 customtkintermessagebox-0.0.3/CustomTkinterMessagebox/__init__.py
+-rw-rw-rw-   0        0        0     2027 2024-05-11 16:03:23.000000 customtkintermessagebox-0.0.3/CustomTkinterMessagebox/messagebox.py
+drwxrwxrwx   0        0        0        0 2024-05-11 17:14:02.669749 customtkintermessagebox-0.0.3/CustomTkinterMessagebox.egg-info/
+-rw-rw-rw-   0        0        0      575 2024-05-11 17:14:02.000000 customtkintermessagebox-0.0.3/CustomTkinterMessagebox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2024-05-11 17:14:02.000000 customtkintermessagebox-0.0.3/CustomTkinterMessagebox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 17:14:02.000000 customtkintermessagebox-0.0.3/CustomTkinterMessagebox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2024-05-11 17:14:02.000000 customtkintermessagebox-0.0.3/CustomTkinterMessagebox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-11 17:14:02.000000 customtkintermessagebox-0.0.3/CustomTkinterMessagebox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1106 2024-05-11 15:01:43.000000 customtkintermessagebox-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      575 2024-05-11 17:14:02.669749 customtkintermessagebox-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1281 2024-05-11 16:01:37.000000 customtkintermessagebox-0.0.3/examples.py
+-rw-rw-rw-   0        0        0       42 2024-05-11 17:14:02.669749 customtkintermessagebox-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      685 2024-05-11 17:13:48.000000 customtkintermessagebox-0.0.3/setup.py
```

### Comparing `customtkintermessagebox-0.0.2/CustomTkinterMessagebox/messagebox.py` & `customtkintermessagebox-0.0.3/CustomTkinterMessagebox/messagebox.py`

 * *Files identical despite different names*

### Comparing `customtkintermessagebox-0.0.2/LICENSE` & `customtkintermessagebox-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `customtkintermessagebox-0.0.2/examples.py` & `customtkintermessagebox-0.0.3/examples.py`

 * *Files identical despite different names*

