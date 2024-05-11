# Comparing `tmp/pizzoo-0.9.1.tar.gz` & `tmp/pizzoo-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pizzoo-0.9.1.tar", last modified: Fri May 10 22:23:51 2024, max compression
+gzip compressed data, was "pizzoo-0.9.2.tar", last modified: Sat May 11 00:52:17 2024, max compression
```

## Comparing `pizzoo-0.9.1.tar` & `pizzoo-0.9.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 22:23:51.810691 pizzoo-0.9.1/
--rw-rw-rw-   0        0        0      760 2024-05-10 22:23:51.809689 pizzoo-0.9.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-10 22:23:51.804692 pizzoo-0.9.1/pizzoo/
--rw-rw-rw-   0        0        0    21798 2024-05-04 08:50:51.000000 pizzoo-0.9.1/pizzoo/__init__.py
--rw-rw-rw-   0        0        0     1444 2024-04-19 15:38:24.000000 pizzoo-0.9.1/pizzoo/_constants.py
--rw-rw-rw-   0        0        0    17046 2024-05-03 00:00:18.000000 pizzoo-0.9.1/pizzoo/_renderers.py
--rw-rw-rw-   0        0        0      705 2024-04-28 16:47:36.000000 pizzoo-0.9.1/pizzoo/_utils.py
--rw-rw-rw-   0        0        0    21871 2024-05-10 19:21:17.000000 pizzoo-0.9.1/pizzoo/game.py
-drwxrwxrwx   0        0        0        0 2024-05-10 22:23:51.809689 pizzoo-0.9.1/pizzoo.egg-info/
--rw-rw-rw-   0        0        0      760 2024-05-10 22:23:51.000000 pizzoo-0.9.1/pizzoo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-05-10 22:23:51.000000 pizzoo-0.9.1/pizzoo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 22:23:51.000000 pizzoo-0.9.1/pizzoo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-05-10 22:23:51.000000 pizzoo-0.9.1/pizzoo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-10 22:23:51.000000 pizzoo-0.9.1/pizzoo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 22:23:51.810691 pizzoo-0.9.1/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-05-10 22:23:40.000000 pizzoo-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 00:52:17.280512 pizzoo-0.9.2/
+-rw-rw-rw-   0        0        0     6712 2024-05-11 00:52:17.280512 pizzoo-0.9.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-11 00:52:17.276511 pizzoo-0.9.2/pizzoo/
+-rw-rw-rw-   0        0        0    21798 2024-05-04 08:50:51.000000 pizzoo-0.9.2/pizzoo/__init__.py
+-rw-rw-rw-   0        0        0     1444 2024-04-19 15:38:24.000000 pizzoo-0.9.2/pizzoo/_constants.py
+-rw-rw-rw-   0        0        0    17046 2024-05-03 00:00:18.000000 pizzoo-0.9.2/pizzoo/_renderers.py
+-rw-rw-rw-   0        0        0      705 2024-04-28 16:47:36.000000 pizzoo-0.9.2/pizzoo/_utils.py
+-rw-rw-rw-   0        0        0    21871 2024-05-10 19:21:17.000000 pizzoo-0.9.2/pizzoo/game.py
+drwxrwxrwx   0        0        0        0 2024-05-11 00:52:17.279513 pizzoo-0.9.2/pizzoo.egg-info/
+-rw-rw-rw-   0        0        0     6712 2024-05-11 00:52:17.000000 pizzoo-0.9.2/pizzoo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-05-11 00:52:17.000000 pizzoo-0.9.2/pizzoo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 00:52:17.000000 pizzoo-0.9.2/pizzoo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-11 00:52:17.000000 pizzoo-0.9.2/pizzoo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-11 00:52:17.000000 pizzoo-0.9.2/pizzoo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-11 00:52:17.281511 pizzoo-0.9.2/setup.cfg
+-rw-rw-rw-   0        0        0     1172 2024-05-11 00:52:13.000000 pizzoo-0.9.2/setup.py
```

### Comparing `pizzoo-0.9.1/pizzoo/__init__.py` & `pizzoo-0.9.2/pizzoo/__init__.py`

 * *Files identical despite different names*

### Comparing `pizzoo-0.9.1/pizzoo/_constants.py` & `pizzoo-0.9.2/pizzoo/_constants.py`

 * *Files identical despite different names*

### Comparing `pizzoo-0.9.1/pizzoo/_renderers.py` & `pizzoo-0.9.2/pizzoo/_renderers.py`

 * *Files identical despite different names*

### Comparing `pizzoo-0.9.1/pizzoo/_utils.py` & `pizzoo-0.9.2/pizzoo/_utils.py`

 * *Files identical despite different names*

### Comparing `pizzoo-0.9.1/pizzoo/game.py` & `pizzoo-0.9.2/pizzoo/game.py`

 * *Files identical despite different names*

### Comparing `pizzoo-0.9.1/setup.py` & `pizzoo-0.9.2/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from setuptools import setup
 
+long_description = open('%s\\README.md' % 'C:\\Users\\Usuario\\Documents\\Projects\\pizzoo').read()
+
 # https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/
 setup(
     name="pizzoo",
-    version="0.9.1",
+    version="0.9.2",
     author="Pablo Huet",
     description="Pizzoo is a library for rendering on pixel matrix screens, with direct support for the Divoom Pixoo64 device, and easy integration for any other one. It includes full animation buffer manipulation, a micro game engine, as well as XML/HTML like templates compilation.",
-    license="MIT",
+    long_description=long_description,
+	long_description_content_type='text/markdown',
+	license="MIT",
     keywords="pixoo, pixoo64, divoom, screen, pixel, matrix, render, buffer, LED matrix, LED, raspberry, raspberry pi",
     url="https://github.com/pabletos/pizzoo#readme",
     packages=['pizzoo'],
     install_requires=[
         'requests ~= 2.31.0',
         'Pillow ~= 10.0.0',
 		'bdfparser ~= 2.2.0'
```

