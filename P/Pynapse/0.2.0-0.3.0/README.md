# Comparing `tmp/pynapse-0.2.0.tar.gz` & `tmp/pynapse-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynapse-0.2.0.tar", last modified: Sat May 11 03:55:43 2024, max compression
+gzip compressed data, was "pynapse-0.3.0.tar", last modified: Sat May 11 04:03:53 2024, max compression
```

## Comparing `pynapse-0.2.0.tar` & `pynapse-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 03:55:43.753703 pynapse-0.2.0/
--rw-rw-rw-   0        0        0       76 2024-05-11 03:55:43.751708 pynapse-0.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-11 03:55:43.725436 pynapse-0.2.0/Pynapse/
--rw-rw-rw-   0        0        0      151 2024-05-11 02:36:57.000000 pynapse-0.2.0/Pynapse/__init__.py
--rw-rw-rw-   0        0        0     2743 2024-05-11 03:54:04.000000 pynapse-0.2.0/Pynapse/main.py
-drwxrwxrwx   0        0        0        0 2024-05-11 03:55:43.750711 pynapse-0.2.0/Pynapse.egg-info/
--rw-rw-rw-   0        0        0       76 2024-05-11 03:55:43.000000 pynapse-0.2.0/Pynapse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2024-05-11 03:55:43.000000 pynapse-0.2.0/Pynapse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 03:55:43.000000 pynapse-0.2.0/Pynapse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-11 03:55:43.000000 pynapse-0.2.0/Pynapse.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-11 03:55:43.000000 pynapse-0.2.0/Pynapse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-05-11 03:19:58.000000 pynapse-0.2.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-11 03:55:43.753703 pynapse-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      179 2024-05-11 03:22:02.000000 pynapse-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 04:03:53.690986 pynapse-0.3.0/
+-rw-rw-rw-   0        0        0       76 2024-05-11 04:03:53.689014 pynapse-0.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-11 04:03:53.656944 pynapse-0.3.0/Pynapse/
+-rw-rw-rw-   0        0        0      180 2024-05-11 04:02:14.000000 pynapse-0.3.0/Pynapse/__init__.py
+-rw-rw-rw-   0        0        0     2743 2024-05-11 03:54:04.000000 pynapse-0.3.0/Pynapse/main.py
+drwxrwxrwx   0        0        0        0 2024-05-11 04:03:53.685806 pynapse-0.3.0/Pynapse.egg-info/
+-rw-rw-rw-   0        0        0       76 2024-05-11 04:03:53.000000 pynapse-0.3.0/Pynapse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2024-05-11 04:03:53.000000 pynapse-0.3.0/Pynapse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 04:03:53.000000 pynapse-0.3.0/Pynapse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-11 04:03:53.000000 pynapse-0.3.0/Pynapse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-11 04:03:53.000000 pynapse-0.3.0/Pynapse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-05-11 03:19:58.000000 pynapse-0.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-11 04:03:53.691985 pynapse-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      179 2024-05-11 04:03:47.000000 pynapse-0.3.0/setup.py
```

### Comparing `pynapse-0.2.0/Pynapse/main.py` & `pynapse-0.3.0/Pynapse/main.py`

 * *Files identical despite different names*

