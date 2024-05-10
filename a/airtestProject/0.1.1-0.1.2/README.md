# Comparing `tmp/airtestproject-0.1.1.tar.gz` & `tmp/airtestproject-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "G:\pyProject\odin-testautomation\TestAutomation\dist\.tmp-hjmf8lgp\airtestproject-0.1.1.tar", last modified: Fri May 10 10:40:34 2024, max compression
+gzip compressed data, was "G:\pyProject\odin-testautomation\TestAutomation\dist\.tmp-c2obb5gw\airtestproject-0.1.2.tar", last modified: Fri May 10 15:23:01 2024, max compression
```

## Comparing `airtestproject-0.1.1.tar` & `airtestproject-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,75 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 10:40:34.570884 airtestproject-0.1.1/
--rw-rw-rw-   0        0        0     1093 2024-05-10 09:37:02.000000 airtestproject-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      623 2024-05-10 10:40:34.569887 airtestproject-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      134 2024-05-10 09:55:18.000000 airtestproject-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 10:40:34.568889 airtestproject-0.1.1/airtestProject.egg-info/
--rw-rw-rw-   0        0        0      623 2024-05-10 10:40:34.000000 airtestproject-0.1.1/airtestProject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2024-05-10 10:40:34.000000 airtestproject-0.1.1/airtestProject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 10:40:34.000000 airtestproject-0.1.1/airtestProject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      139 2024-05-10 10:40:34.000000 airtestproject-0.1.1/airtestProject.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 10:40:34.000000 airtestproject-0.1.1/airtestProject.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 10:40:34.571880 airtestproject-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      819 2024-05-10 10:40:26.000000 airtestproject-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:23:01.924800 airtestproject-0.1.2/
+-rw-rw-rw-   0        0        0     1093 2024-05-10 09:37:02.000000 airtestproject-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      623 2024-05-10 15:23:01.923803 airtestproject-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      134 2024-05-10 09:55:18.000000 airtestproject-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 15:23:01.841024 airtestproject-0.1.2/airtestProject/
+-rw-rw-rw-   0        0        0        0 2024-05-09 06:02:26.000000 airtestproject-0.1.2/airtestProject/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:23:01.852992 airtestproject-0.1.2/airtestProject/abstractBase/
+-rw-rw-rw-   0        0        0     1786 2024-05-09 11:56:31.000000 airtestproject-0.1.2/airtestProject/abstractBase/OperateBase.py
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.2/airtestProject/abstractBase/__init__.py
+-rw-rw-rw-   0        0        0      196 2024-04-25 04:13:07.000000 airtestproject-0.1.2/airtestProject/abstractBase/loginBase.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:23:01.855985 airtestproject-0.1.2/airtestProject/commons/
+drwxrwxrwx   0        0        0        0 2024-05-10 15:23:01.857979 airtestproject-0.1.2/airtestProject/commons/Position/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.2/airtestProject/commons/Position/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:23:01.859973 airtestproject-0.1.2/airtestProject/commons/Position/odin/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.2/airtestProject/commons/Position/odin/__init__.py
+-rw-rw-rw-   0        0        0       35 2024-04-15 08:30:41.000000 airtestproject-0.1.2/airtestProject/commons/Position/odin/odinPos.py
+-rw-rw-rw-   0        0        0    11611 2024-05-10 08:12:02.000000 airtestproject-0.1.2/airtestProject/commons/UWA.py
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.2/airtestProject/commons/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:23:01.861967 airtestproject-0.1.2/airtestProject/commons/page/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.2/airtestProject/commons/page/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:23:01.866955 airtestproject-0.1.2/airtestProject/commons/page/odin/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.2/airtestProject/commons/page/odin/__init__.py
+-rw-rw-rw-   0        0        0    19248 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/commons/page/odin/funcListCheck.py
+-rw-rw-rw-   0        0        0     9193 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/commons/page/odin/login.py
+-rw-rw-rw-   0        0        0     6203 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/commons/page/odin/run.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:23:01.868977 airtestproject-0.1.2/airtestProject/commons/process/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.2/airtestProject/commons/process/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:23:01.871941 airtestproject-0.1.2/airtestProject/commons/process/odin/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.2/airtestProject/commons/process/odin/__init__.py
+-rw-rw-rw-   0        0        0     1636 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/commons/process/odin/profile.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:23:01.902889 airtestproject-0.1.2/airtestProject/commons/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.2/airtestProject/commons/utils/__init__.py
+-rw-rw-rw-   0        0        0     5314 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/commons/utils/air.py
+-rw-rw-rw-   0        0        0      705 2024-05-10 15:22:52.000000 airtestproject-0.1.2/airtestProject/commons/utils/appStart.py
+-rw-rw-rw-   0        0        0     3523 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/commons/utils/command.py
+-rw-rw-rw-   0        0        0     2740 2024-04-26 03:34:41.000000 airtestproject-0.1.2/airtestProject/commons/utils/deploy.py
+-rw-rw-rw-   0        0        0     5661 2024-04-29 08:44:46.000000 airtestproject-0.1.2/airtestProject/commons/utils/excel_image.py
+-rw-rw-rw-   0        0        0      687 2024-04-10 04:18:58.000000 airtestproject-0.1.2/airtestProject/commons/utils/exception.py
+-rw-rw-rw-   0        0        0     3384 2024-04-10 04:18:58.000000 airtestproject-0.1.2/airtestProject/commons/utils/factory.py
+-rw-rw-rw-   0        0        0    12632 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/commons/utils/ganaratePyCase.py
+-rw-rw-rw-   0        0        0     2730 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/commons/utils/genaratePy.py
+-rw-rw-rw-   0        0        0     3548 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/commons/utils/gotCommon.py
+-rw-rw-rw-   0        0        0     5472 2024-05-08 10:15:18.000000 airtestproject-0.1.2/airtestProject/commons/utils/logger.py
+-rw-rw-rw-   0        0        0    11058 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/commons/utils/myAirtest.py
+-rw-rw-rw-   0        0        0     7332 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/commons/utils/myPoco.py
+-rw-rw-rw-   0        0        0     8142 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/commons/utils/ocrTemplate.py
+-rw-rw-rw-   0        0        0     9032 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/commons/utils/page.py
+-rw-rw-rw-   0        0        0     6154 2024-05-10 10:40:07.000000 airtestproject-0.1.2/airtestProject/commons/utils/reportUtil.py
+-rw-rw-rw-   0        0        0     1444 2024-04-12 14:52:30.000000 airtestproject-0.1.2/airtestProject/commons/utils/send.py
+-rw-rw-rw-   0        0        0     1676 2024-05-10 08:00:06.000000 airtestproject-0.1.2/airtestProject/commons/utils/tools.py
+-rw-rw-rw-   0        0        0    14349 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/commons/utils/utils.py
+-rw-rw-rw-   0        0        0      497 2024-04-30 04:52:37.000000 airtestproject-0.1.2/airtestProject/config.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:23:01.907848 airtestproject-0.1.2/airtestProject/factory/
+-rw-rw-rw-   0        0        0      292 2024-04-12 14:52:30.000000 airtestproject-0.1.2/airtestProject/factory/SingletonFactory.py
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.2/airtestProject/factory/__init__.py
+-rw-rw-rw-   0        0        0     1930 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/factory/operateFactory.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:23:01.917819 airtestproject-0.1.2/airtestProject/manager/
+-rw-rw-rw-   0        0        0     9282 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/manager/DeviceManager.py
+-rw-rw-rw-   0        0        0     6827 2024-04-30 04:52:37.000000 airtestproject-0.1.2/airtestProject/manager/LogManager.py
+-rw-rw-rw-   0        0        0     2895 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/manager/PackageManager.py
+-rw-rw-rw-   0        0        0    24575 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/manager/ReportManager.py
+-rw-rw-rw-   0        0        0     1786 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/manager/TaskManager.py
+-rw-rw-rw-   0        0        0     4832 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/manager/TestCaseManager.py
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.2/airtestProject/manager/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:23:01.920811 airtestproject-0.1.2/airtestProject/scripts/
+-rw-rw-rw-   0        0        0     1959 2024-05-10 15:22:52.000000 airtestproject-0.1.2/airtestProject/scripts/OdinExample.py
+-rw-rw-rw-   0        0        0        0 2024-03-12 02:10:28.000000 airtestproject-0.1.2/airtestProject/scripts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:23:01.922805 airtestproject-0.1.2/airtestProject.egg-info/
+-rw-rw-rw-   0        0        0      623 2024-05-10 15:23:01.000000 airtestproject-0.1.2/airtestProject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2229 2024-05-10 15:23:01.000000 airtestproject-0.1.2/airtestProject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 15:23:01.000000 airtestproject-0.1.2/airtestProject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      139 2024-05-10 15:23:01.000000 airtestproject-0.1.2/airtestProject.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-10 15:23:01.000000 airtestproject-0.1.2/airtestProject.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 15:23:01.924800 airtestproject-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      819 2024-05-10 14:47:14.000000 airtestproject-0.1.2/setup.py
```

### Comparing `airtestproject-0.1.1/LICENSE` & `airtestproject-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.1/PKG-INFO` & `airtestproject-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airtestProject
-Version: 0.1.1
+Version: 0.1.2
 Author: mortal_sjh
 Author-email: mortal_sjh@qq.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: airtest==1.3.3
 Requires-Dist: openpyxl==1.1.0
```

### Comparing `airtestproject-0.1.1/airtestProject.egg-info/PKG-INFO` & `airtestproject-0.1.2/airtestProject.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airtestProject
-Version: 0.1.1
+Version: 0.1.2
 Author: mortal_sjh
 Author-email: mortal_sjh@qq.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: airtest==1.3.3
 Requires-Dist: openpyxl==1.1.0
```

### Comparing `airtestproject-0.1.1/setup.py` & `airtestproject-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name='airtestProject',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(include=['airtestProject', 'airtestProject.*']),
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         "airtest==1.3.3",
         "openpyxl==1.1.0",
         "pocoui==1.0.94",
```

