# Comparing `tmp/config_profile-0.0.1.tar.gz` & `tmp/config_profile-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "config_profile-0.0.1.tar", last modified: Sat May 11 20:16:14 2024, max compression
+gzip compressed data, was "config_profile-0.0.2.tar", last modified: Sat May 11 20:28:03 2024, max compression
```

## Comparing `config_profile-0.0.1.tar` & `config_profile-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 kyle       (501) staff       (20)        0 2024-05-11 20:16:14.056954 config_profile-0.0.1/
--rw-r--r--   0 kyle       (501) staff       (20)     1071 2024-05-08 00:04:07.000000 config_profile-0.0.1/LICENSE
--rw-r--r--   0 kyle       (501) staff       (20)      920 2024-05-11 20:16:14.056795 config_profile-0.0.1/PKG-INFO
--rw-r--r--   0 kyle       (501) staff       (20)      351 2024-05-11 20:00:51.000000 config_profile-0.0.1/README.md
-drwxr-xr-x   0 kyle       (501) staff       (20)        0 2024-05-11 20:16:14.056637 config_profile-0.0.1/config_profile.egg-info/
--rw-r--r--   0 kyle       (501) staff       (20)      920 2024-05-11 20:16:14.000000 config_profile-0.0.1/config_profile.egg-info/PKG-INFO
--rw-r--r--   0 kyle       (501) staff       (20)      193 2024-05-11 20:16:14.000000 config_profile-0.0.1/config_profile.egg-info/SOURCES.txt
--rw-r--r--   0 kyle       (501) staff       (20)        1 2024-05-11 20:16:14.000000 config_profile-0.0.1/config_profile.egg-info/dependency_links.txt
--rw-r--r--   0 kyle       (501) staff       (20)        1 2024-05-11 20:16:14.000000 config_profile-0.0.1/config_profile.egg-info/top_level.txt
--rw-r--r--   0 kyle       (501) staff       (20)      693 2024-05-11 15:30:43.000000 config_profile-0.0.1/pyproject.toml
--rw-r--r--   0 kyle       (501) staff       (20)       38 2024-05-11 20:16:14.056993 config_profile-0.0.1/setup.cfg
--rw-r--r--   0 kyle       (501) staff       (20)      157 2024-05-11 19:59:52.000000 config_profile-0.0.1/setup.py
+drwxr-xr-x   0 kyle       (501) staff       (20)        0 2024-05-11 20:28:03.019926 config_profile-0.0.2/
+-rw-r--r--   0 kyle       (501) staff       (20)     1071 2024-05-08 00:04:07.000000 config_profile-0.0.2/LICENSE
+-rw-r--r--   0 kyle       (501) staff       (20)      920 2024-05-11 20:28:03.019773 config_profile-0.0.2/PKG-INFO
+-rw-r--r--   0 kyle       (501) staff       (20)      351 2024-05-11 20:00:51.000000 config_profile-0.0.2/README.md
+drwxr-xr-x   0 kyle       (501) staff       (20)        0 2024-05-11 20:28:03.019626 config_profile-0.0.2/config_profile.egg-info/
+-rw-r--r--   0 kyle       (501) staff       (20)      920 2024-05-11 20:28:03.000000 config_profile-0.0.2/config_profile.egg-info/PKG-INFO
+-rw-r--r--   0 kyle       (501) staff       (20)      193 2024-05-11 20:28:03.000000 config_profile-0.0.2/config_profile.egg-info/SOURCES.txt
+-rw-r--r--   0 kyle       (501) staff       (20)        1 2024-05-11 20:28:03.000000 config_profile-0.0.2/config_profile.egg-info/dependency_links.txt
+-rw-r--r--   0 kyle       (501) staff       (20)        1 2024-05-11 20:28:03.000000 config_profile-0.0.2/config_profile.egg-info/top_level.txt
+-rw-r--r--   0 kyle       (501) staff       (20)      693 2024-05-11 20:27:47.000000 config_profile-0.0.2/pyproject.toml
+-rw-r--r--   0 kyle       (501) staff       (20)       38 2024-05-11 20:28:03.019958 config_profile-0.0.2/setup.cfg
+-rw-r--r--   0 kyle       (501) staff       (20)      375 2024-05-11 20:27:05.000000 config_profile-0.0.2/setup.py
```

### Comparing `config_profile-0.0.1/LICENSE` & `config_profile-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `config_profile-0.0.1/PKG-INFO` & `config_profile-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: config_profile
-Version: 0.0.1
+Version: 0.0.2
 Summary: Application configuration made simple
 Author-email: Kyle Holzinger <kyleholzinger@hey.com>, Jamie Cristini <jamie@j2health.com>
 Project-URL: Homepage, https://github.com/avegancafe/config-profile
 Project-URL: Issues, https://github.com/avegancafe/config-profile/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `config_profile-0.0.1/config_profile.egg-info/PKG-INFO` & `config_profile-0.0.2/config_profile.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: config_profile
-Version: 0.0.1
+Version: 0.0.2
 Summary: Application configuration made simple
 Author-email: Kyle Holzinger <kyleholzinger@hey.com>, Jamie Cristini <jamie@j2health.com>
 Project-URL: Homepage, https://github.com/avegancafe/config-profile
 Project-URL: Issues, https://github.com/avegancafe/config-profile/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `config_profile-0.0.1/pyproject.toml` & `config_profile-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "config_profile"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Kyle Holzinger", email="kyleholzinger@hey.com" },
 	{ name="Jamie Cristini", email="jamie@j2health.com" },
 ]
 description = "Application configuration made simple"
 readme = "README.md"
 requires-python = ">=3.12"
```

