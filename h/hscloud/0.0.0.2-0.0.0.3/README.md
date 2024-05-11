# Comparing `tmp/hscloud-0.0.0.2.tar.gz` & `tmp/hscloud-0.0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hscloud-0.0.0.2.tar", last modified: Thu May  9 10:11:46 2024, max compression
+gzip compressed data, was "hscloud-0.0.0.3.tar", last modified: Sat May 11 11:01:47 2024, max compression
```

## Comparing `hscloud-0.0.0.2.tar` & `hscloud-0.0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 10:11:46.207146 hscloud-0.0.0.2/
--rw-rw-rw-   0        0        0        0 2023-12-18 08:14:13.000000 hscloud-0.0.0.2/LICENSE
--rw-rw-rw-   0        0        0      432 2024-05-09 10:11:46.204146 hscloud-0.0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2505 2024-05-09 10:10:45.000000 hscloud-0.0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 10:11:46.186142 hscloud-0.0.0.2/hscloud/
--rw-rw-rw-   0        0        0      258 2024-05-09 07:57:46.000000 hscloud-0.0.0.2/hscloud/__init__.py
--rw-rw-rw-   0        0        0     3653 2024-05-09 07:55:39.000000 hscloud-0.0.0.2/hscloud/helpers.py
--rw-rw-rw-   0        0        0      944 2024-05-09 10:09:38.000000 hscloud-0.0.0.2/hscloud/hscloud.py
-drwxrwxrwx   0        0        0        0 2024-05-09 10:11:46.202143 hscloud-0.0.0.2/hscloud.egg-info/
--rw-rw-rw-   0        0        0      432 2024-05-09 10:11:46.000000 hscloud-0.0.0.2/hscloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2024-05-09 10:11:46.000000 hscloud-0.0.0.2/hscloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 10:11:46.000000 hscloud-0.0.0.2/hscloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-05-09 10:11:46.000000 hscloud-0.0.0.2/hscloud.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2024-05-09 10:11:46.000000 hscloud-0.0.0.2/hscloud.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-09 10:11:46.000000 hscloud-0.0.0.2/hscloud.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 10:11:46.207146 hscloud-0.0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      887 2024-05-09 10:11:11.000000 hscloud-0.0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 11:01:47.176418 hscloud-0.0.0.3/
+-rw-rw-rw-   0        0        0        0 2023-12-18 08:14:13.000000 hscloud-0.0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      432 2024-05-11 11:01:47.174418 hscloud-0.0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2505 2024-05-09 10:10:45.000000 hscloud-0.0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 11:01:47.158417 hscloud-0.0.0.3/hscloud/
+-rw-rw-rw-   0        0        0      258 2024-05-09 07:57:46.000000 hscloud-0.0.0.3/hscloud/__init__.py
+-rw-rw-rw-   0        0        0     3653 2024-05-09 07:55:39.000000 hscloud-0.0.0.3/hscloud/helpers.py
+-rw-rw-rw-   0        0        0      951 2024-05-11 10:55:00.000000 hscloud-0.0.0.3/hscloud/hscloud.py
+drwxrwxrwx   0        0        0        0 2024-05-11 11:01:47.172417 hscloud-0.0.0.3/hscloud.egg-info/
+-rw-rw-rw-   0        0        0      432 2024-05-11 11:01:47.000000 hscloud-0.0.0.3/hscloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2024-05-11 11:01:47.000000 hscloud-0.0.0.3/hscloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 11:01:47.000000 hscloud-0.0.0.3/hscloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-05-11 11:01:47.000000 hscloud-0.0.0.3/hscloud.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2024-05-11 11:01:47.000000 hscloud-0.0.0.3/hscloud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-11 11:01:47.000000 hscloud-0.0.0.3/hscloud.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-11 11:01:47.176418 hscloud-0.0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      887 2024-05-11 10:55:26.000000 hscloud-0.0.0.3/setup.py
```

### Comparing `hscloud-0.0.0.2/README.md` & `hscloud-0.0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `hscloud-0.0.0.2/hscloud/helpers.py` & `hscloud-0.0.0.3/hscloud/helpers.py`

 * *Files identical despite different names*

### Comparing `hscloud-0.0.0.2/hscloud/hscloud.py` & `hscloud-0.0.0.3/hscloud/hscloud.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,9 +20,9 @@
 
     def get_devices(self) -> tuple:
         return Helpers.devices(self.endpoint, self.access_token)
 
     def get_status(self, devicesn) -> tuple:
         return Helpers.status(self.endpoint, self.access_token, devicesn)
 
-    def update(self, devicesn, **kwargs) -> tuple:
+    def update_status(self, devicesn, **kwargs) -> tuple:
         return Helpers.update(self.endpoint, self.access_token, devicesn, **kwargs)
```

### Comparing `hscloud-0.0.0.2/setup.py` & `hscloud-0.0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name = 'hscloud',
     packages = ['hscloud'],
     include_package_data=True,
-    version = '0.0.0.2',
+    version = '0.0.0.3',
     license='MIT',
     description = 'Library to login to Dreo cloud and get device info.',
     author = 'Kane Wang',
     author_email = 'app@hesung.com',
     url = 'https://github.com/dreo-team/hscloud',
     download_url = 'https://github.com/dreo-team/hscloud/dist/hscloud-0.0.11.tar.gz',
     install_requires=[
```

