# Comparing `tmp/guava3-0.1.tar.gz` & `tmp/guava3-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guava3-0.1.tar", last modified: Sat May 11 01:23:18 2024, max compression
+gzip compressed data, was "guava3-0.2.tar", last modified: Sat May 11 02:12:08 2024, max compression
```

## Comparing `guava3-0.1.tar` & `guava3-0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 pedromello   (501) staff       (20)        0 2024-05-11 01:23:18.935626 guava3-0.1/
--rw-r--r--   0 pedromello   (501) staff       (20)      443 2024-05-11 01:23:18.935422 guava3-0.1/PKG-INFO
--rw-r--r--   0 pedromello   (501) staff       (20)       18 2024-04-30 01:23:38.000000 guava3-0.1/README.md
-drwxr-xr-x   0 pedromello   (501) staff       (20)        0 2024-05-11 01:23:18.932764 guava3-0.1/guava3/
--rw-r--r--   0 pedromello   (501) staff       (20)        0 2024-04-29 23:41:59.000000 guava3-0.1/guava3/__init__.py
--rw-r--r--   0 pedromello   (501) staff       (20)     1673 2024-05-11 00:11:52.000000 guava3-0.1/guava3/conversation.py
--rw-r--r--   0 pedromello   (501) staff       (20)    16792 2024-05-10 22:22:54.000000 guava3-0.1/guava3/entities.py
--rw-r--r--   0 pedromello   (501) staff       (20)     9562 2024-05-10 22:55:46.000000 guava3-0.1/guava3/function_library.py
-drwxr-xr-x   0 pedromello   (501) staff       (20)        0 2024-05-11 01:23:18.934820 guava3-0.1/guava3/implementations/
--rw-r--r--   0 pedromello   (501) staff       (20)        0 2024-05-11 00:44:14.000000 guava3-0.1/guava3/implementations/__init__.py
--rw-r--r--   0 pedromello   (501) staff       (20)    41449 2024-05-11 00:56:12.000000 guava3-0.1/guava3/implementations/images.py
--rw-r--r--   0 pedromello   (501) staff       (20)      965 2024-05-11 01:15:17.000000 guava3-0.1/guava3/implementations/notebook.py
--rw-r--r--   0 pedromello   (501) staff       (20)     1160 2024-05-11 01:18:02.000000 guava3-0.1/guava3/implementations/terminal.py
--rw-r--r--   0 pedromello   (501) staff       (20)    10409 2024-05-11 01:04:03.000000 guava3-0.1/guava3/implementations/widgets.py
--rw-r--r--   0 pedromello   (501) staff       (20)     4156 2024-05-10 22:20:15.000000 guava3-0.1/guava3/serializers.py
--rw-r--r--   0 pedromello   (501) staff       (20)     5501 2024-05-11 00:05:58.000000 guava3-0.1/guava3/utils.py
-drwxr-xr-x   0 pedromello   (501) staff       (20)        0 2024-05-11 01:23:18.933493 guava3-0.1/guava3.egg-info/
--rw-r--r--   0 pedromello   (501) staff       (20)      443 2024-05-11 01:23:18.000000 guava3-0.1/guava3.egg-info/PKG-INFO
--rw-r--r--   0 pedromello   (501) staff       (20)      465 2024-05-11 01:23:18.000000 guava3-0.1/guava3.egg-info/SOURCES.txt
--rw-r--r--   0 pedromello   (501) staff       (20)        1 2024-05-11 01:23:18.000000 guava3-0.1/guava3.egg-info/dependency_links.txt
--rw-r--r--   0 pedromello   (501) staff       (20)       92 2024-05-11 01:23:18.000000 guava3-0.1/guava3.egg-info/requires.txt
--rw-r--r--   0 pedromello   (501) staff       (20)        7 2024-05-11 01:23:18.000000 guava3-0.1/guava3.egg-info/top_level.txt
--rw-r--r--   0 pedromello   (501) staff       (20)       38 2024-05-11 01:23:18.935664 guava3-0.1/setup.cfg
--rw-r--r--   0 pedromello   (501) staff       (20)      583 2024-05-11 01:23:16.000000 guava3-0.1/setup.py
+drwxr-xr-x   0 pedromello   (501) staff       (20)        0 2024-05-11 02:12:08.820358 guava3-0.2/
+-rw-r--r--   0 pedromello   (501) staff       (20)      545 2024-05-11 02:12:08.820174 guava3-0.2/PKG-INFO
+-rw-r--r--   0 pedromello   (501) staff       (20)       18 2024-04-30 01:23:38.000000 guava3-0.2/README.md
+drwxr-xr-x   0 pedromello   (501) staff       (20)        0 2024-05-11 02:12:08.817677 guava3-0.2/guava3/
+-rw-r--r--   0 pedromello   (501) staff       (20)        0 2024-04-29 23:41:59.000000 guava3-0.2/guava3/__init__.py
+-rw-r--r--   0 pedromello   (501) staff       (20)     1673 2024-05-11 00:11:52.000000 guava3-0.2/guava3/conversation.py
+-rw-r--r--   0 pedromello   (501) staff       (20)    16792 2024-05-10 22:22:54.000000 guava3-0.2/guava3/entities.py
+-rw-r--r--   0 pedromello   (501) staff       (20)     9562 2024-05-10 22:55:46.000000 guava3-0.2/guava3/function_library.py
+drwxr-xr-x   0 pedromello   (501) staff       (20)        0 2024-05-11 02:12:08.819818 guava3-0.2/guava3/implementations/
+-rw-r--r--   0 pedromello   (501) staff       (20)        0 2024-05-11 00:44:14.000000 guava3-0.2/guava3/implementations/__init__.py
+-rw-r--r--   0 pedromello   (501) staff       (20)    41449 2024-05-11 00:56:12.000000 guava3-0.2/guava3/implementations/images.py
+-rw-r--r--   0 pedromello   (501) staff       (20)      965 2024-05-11 01:15:17.000000 guava3-0.2/guava3/implementations/notebook.py
+-rw-r--r--   0 pedromello   (501) staff       (20)     1160 2024-05-11 01:18:02.000000 guava3-0.2/guava3/implementations/terminal.py
+-rw-r--r--   0 pedromello   (501) staff       (20)    10409 2024-05-11 01:04:03.000000 guava3-0.2/guava3/implementations/widgets.py
+-rw-r--r--   0 pedromello   (501) staff       (20)     4156 2024-05-10 22:20:15.000000 guava3-0.2/guava3/serializers.py
+-rw-r--r--   0 pedromello   (501) staff       (20)     5501 2024-05-11 00:05:58.000000 guava3-0.2/guava3/utils.py
+drwxr-xr-x   0 pedromello   (501) staff       (20)        0 2024-05-11 02:12:08.818412 guava3-0.2/guava3.egg-info/
+-rw-r--r--   0 pedromello   (501) staff       (20)      545 2024-05-11 02:12:08.000000 guava3-0.2/guava3.egg-info/PKG-INFO
+-rw-r--r--   0 pedromello   (501) staff       (20)      465 2024-05-11 02:12:08.000000 guava3-0.2/guava3.egg-info/SOURCES.txt
+-rw-r--r--   0 pedromello   (501) staff       (20)        1 2024-05-11 02:12:08.000000 guava3-0.2/guava3.egg-info/dependency_links.txt
+-rw-r--r--   0 pedromello   (501) staff       (20)      134 2024-05-11 02:12:08.000000 guava3-0.2/guava3.egg-info/requires.txt
+-rw-r--r--   0 pedromello   (501) staff       (20)        7 2024-05-11 02:12:08.000000 guava3-0.2/guava3.egg-info/top_level.txt
+-rw-r--r--   0 pedromello   (501) staff       (20)       38 2024-05-11 02:12:08.820397 guava3-0.2/setup.cfg
+-rw-r--r--   0 pedromello   (501) staff       (20)      668 2024-05-11 02:10:49.000000 guava3-0.2/setup.py
```

### Comparing `guava3-0.1/guava3/conversation.py` & `guava3-0.2/guava3/conversation.py`

 * *Files identical despite different names*

### Comparing `guava3-0.1/guava3/entities.py` & `guava3-0.2/guava3/entities.py`

 * *Files identical despite different names*

### Comparing `guava3-0.1/guava3/function_library.py` & `guava3-0.2/guava3/function_library.py`

 * *Files identical despite different names*

### Comparing `guava3-0.1/guava3/implementations/images.py` & `guava3-0.2/guava3/implementations/images.py`

 * *Files identical despite different names*

### Comparing `guava3-0.1/guava3/implementations/notebook.py` & `guava3-0.2/guava3/implementations/notebook.py`

 * *Files identical despite different names*

### Comparing `guava3-0.1/guava3/implementations/terminal.py` & `guava3-0.2/guava3/implementations/terminal.py`

 * *Files identical despite different names*

### Comparing `guava3-0.1/guava3/implementations/widgets.py` & `guava3-0.2/guava3/implementations/widgets.py`

 * *Files identical despite different names*

### Comparing `guava3-0.1/guava3/serializers.py` & `guava3-0.2/guava3/serializers.py`

 * *Files identical despite different names*

### Comparing `guava3-0.1/guava3/utils.py` & `guava3-0.2/guava3/utils.py`

 * *Files identical despite different names*

