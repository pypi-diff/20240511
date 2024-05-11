# Comparing `tmp/airtestproject-0.1.4.tar.gz` & `tmp/airtestproject-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "G:\pyProject\odin-testautomation\TestAutomation\dist\.tmp-sez17b0r\airtestproject-0.1.4.tar", last modified: Fri May 10 23:50:20 2024, max compression
+gzip compressed data, was "G:\pyProject\odin-testautomation\TestAutomation\dist\.tmp-6u47b0xg\airtestproject-0.1.5.tar", last modified: Sat May 11 00:14:44 2024, max compression
```

## Comparing `airtestproject-0.1.4.tar` & `airtestproject-0.1.5.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 23:50:20.019267 airtestproject-0.1.4/
--rw-rw-rw-   0        0        0     1093 2024-05-10 09:37:02.000000 airtestproject-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      659 2024-05-10 23:50:20.018270 airtestproject-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      134 2024-05-10 09:55:18.000000 airtestproject-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 23:50:19.930506 airtestproject-0.1.4/airtestProject/
--rw-rw-rw-   0        0        0        0 2024-05-09 06:02:26.000000 airtestproject-0.1.4/airtestProject/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 23:50:19.942474 airtestproject-0.1.4/airtestProject/abstractBase/
--rw-rw-rw-   0        0        0     1786 2024-05-09 11:56:31.000000 airtestproject-0.1.4/airtestProject/abstractBase/OperateBase.py
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.4/airtestProject/abstractBase/__init__.py
--rw-rw-rw-   0        0        0      196 2024-04-25 04:13:07.000000 airtestproject-0.1.4/airtestProject/abstractBase/loginBase.py
-drwxrwxrwx   0        0        0        0 2024-05-10 23:50:19.946463 airtestproject-0.1.4/airtestProject/commons/
-drwxrwxrwx   0        0        0        0 2024-05-10 23:50:19.947460 airtestproject-0.1.4/airtestProject/commons/Position/
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.4/airtestProject/commons/Position/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 23:50:19.950452 airtestproject-0.1.4/airtestProject/commons/Position/odin/
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.4/airtestProject/commons/Position/odin/__init__.py
--rw-rw-rw-   0        0        0       35 2024-04-15 08:30:41.000000 airtestproject-0.1.4/airtestProject/commons/Position/odin/odinPos.py
--rw-rw-rw-   0        0        0    11611 2024-05-10 08:12:02.000000 airtestproject-0.1.4/airtestProject/commons/UWA.py
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.4/airtestProject/commons/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 23:50:19.952447 airtestproject-0.1.4/airtestProject/commons/page/
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.4/airtestProject/commons/page/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 23:50:19.958431 airtestproject-0.1.4/airtestProject/commons/page/odin/
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.4/airtestProject/commons/page/odin/__init__.py
--rw-rw-rw-   0        0        0    19248 2024-05-10 14:46:42.000000 airtestproject-0.1.4/airtestProject/commons/page/odin/funcListCheck.py
--rw-rw-rw-   0        0        0     9193 2024-05-10 14:46:42.000000 airtestproject-0.1.4/airtestProject/commons/page/odin/login.py
--rw-rw-rw-   0        0        0     6203 2024-05-10 14:46:42.000000 airtestproject-0.1.4/airtestProject/commons/page/odin/run.py
-drwxrwxrwx   0        0        0        0 2024-05-10 23:50:19.960425 airtestproject-0.1.4/airtestProject/commons/process/
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.4/airtestProject/commons/process/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 23:50:19.963417 airtestproject-0.1.4/airtestProject/commons/process/odin/
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.4/airtestProject/commons/process/odin/__init__.py
--rw-rw-rw-   0        0        0     1636 2024-05-10 14:46:42.000000 airtestproject-0.1.4/airtestProject/commons/process/odin/profile.py
-drwxrwxrwx   0        0        0        0 2024-05-10 23:50:19.996329 airtestproject-0.1.4/airtestProject/commons/utils/
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.4/airtestProject/commons/utils/__init__.py
--rw-rw-rw-   0        0        0     5314 2024-05-10 14:46:42.000000 airtestproject-0.1.4/airtestProject/commons/utils/air.py
--rw-rw-rw-   0        0        0      705 2024-05-10 15:22:52.000000 airtestproject-0.1.4/airtestProject/commons/utils/appStart.py
--rw-rw-rw-   0        0        0     3523 2024-05-10 14:46:42.000000 airtestproject-0.1.4/airtestProject/commons/utils/command.py
--rw-rw-rw-   0        0        0     2740 2024-04-26 03:34:41.000000 airtestproject-0.1.4/airtestProject/commons/utils/deploy.py
--rw-rw-rw-   0        0        0     5661 2024-04-29 08:44:46.000000 airtestproject-0.1.4/airtestProject/commons/utils/excel_image.py
--rw-rw-rw-   0        0        0      687 2024-04-10 04:18:58.000000 airtestproject-0.1.4/airtestProject/commons/utils/exception.py
--rw-rw-rw-   0        0        0     3384 2024-04-10 04:18:58.000000 airtestproject-0.1.4/airtestProject/commons/utils/factory.py
--rw-rw-rw-   0        0        0    12632 2024-05-10 14:46:42.000000 airtestproject-0.1.4/airtestProject/commons/utils/ganaratePyCase.py
--rw-rw-rw-   0        0        0     2730 2024-05-10 14:46:42.000000 airtestproject-0.1.4/airtestProject/commons/utils/genaratePy.py
--rw-rw-rw-   0        0        0     3548 2024-05-10 14:46:42.000000 airtestproject-0.1.4/airtestProject/commons/utils/gotCommon.py
--rw-rw-rw-   0        0        0     5472 2024-05-08 10:15:18.000000 airtestproject-0.1.4/airtestProject/commons/utils/logger.py
--rw-rw-rw-   0        0        0    11058 2024-05-10 14:46:42.000000 airtestproject-0.1.4/airtestProject/commons/utils/myAirtest.py
--rw-rw-rw-   0        0        0     7332 2024-05-10 14:46:42.000000 airtestproject-0.1.4/airtestProject/commons/utils/myPoco.py
--rw-rw-rw-   0        0        0     8142 2024-05-10 14:46:42.000000 airtestproject-0.1.4/airtestProject/commons/utils/ocrTemplate.py
--rw-rw-rw-   0        0        0     9032 2024-05-10 14:46:42.000000 airtestproject-0.1.4/airtestProject/commons/utils/page.py
--rw-rw-rw-   0        0        0     6154 2024-05-10 10:40:07.000000 airtestproject-0.1.4/airtestProject/commons/utils/reportUtil.py
--rw-rw-rw-   0        0        0     1444 2024-04-12 14:52:30.000000 airtestproject-0.1.4/airtestProject/commons/utils/send.py
--rw-rw-rw-   0        0        0     1676 2024-05-10 08:00:06.000000 airtestproject-0.1.4/airtestProject/commons/utils/tools.py
--rw-rw-rw-   0        0        0    14349 2024-05-10 14:46:42.000000 airtestproject-0.1.4/airtestProject/commons/utils/utils.py
--rw-rw-rw-   0        0        0      497 2024-04-30 04:52:37.000000 airtestproject-0.1.4/airtestProject/config.py
-drwxrwxrwx   0        0        0        0 2024-05-10 23:50:20.000318 airtestproject-0.1.4/airtestProject/factory/
--rw-rw-rw-   0        0        0      292 2024-04-12 14:52:30.000000 airtestproject-0.1.4/airtestProject/factory/SingletonFactory.py
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.4/airtestProject/factory/__init__.py
--rw-rw-rw-   0        0        0     1930 2024-05-10 14:46:42.000000 airtestproject-0.1.4/airtestProject/factory/operateFactory.py
-drwxrwxrwx   0        0        0        0 2024-05-10 23:50:20.012288 airtestproject-0.1.4/airtestProject/manager/
--rw-rw-rw-   0        0        0     9413 2024-05-10 23:48:07.000000 airtestproject-0.1.4/airtestProject/manager/DeviceManager.py
--rw-rw-rw-   0        0        0     6827 2024-04-30 04:52:37.000000 airtestproject-0.1.4/airtestProject/manager/LogManager.py
--rw-rw-rw-   0        0        0     2895 2024-05-10 14:46:42.000000 airtestproject-0.1.4/airtestProject/manager/PackageManager.py
--rw-rw-rw-   0        0        0    24575 2024-05-10 14:46:42.000000 airtestproject-0.1.4/airtestProject/manager/ReportManager.py
--rw-rw-rw-   0        0        0     1786 2024-05-10 14:46:42.000000 airtestproject-0.1.4/airtestProject/manager/TaskManager.py
--rw-rw-rw-   0        0        0     4832 2024-05-10 14:46:42.000000 airtestproject-0.1.4/airtestProject/manager/TestCaseManager.py
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.4/airtestProject/manager/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 23:50:20.015279 airtestproject-0.1.4/airtestProject/scripts/
--rw-rw-rw-   0        0        0     1959 2024-05-10 15:22:52.000000 airtestproject-0.1.4/airtestProject/scripts/OdinExample.py
--rw-rw-rw-   0        0        0        0 2024-03-12 02:10:28.000000 airtestproject-0.1.4/airtestProject/scripts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 23:50:20.016276 airtestproject-0.1.4/airtestProject.egg-info/
--rw-rw-rw-   0        0        0      659 2024-05-10 23:50:19.000000 airtestproject-0.1.4/airtestProject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2229 2024-05-10 23:50:19.000000 airtestproject-0.1.4/airtestProject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 23:50:19.000000 airtestproject-0.1.4/airtestProject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      159 2024-05-10 23:50:19.000000 airtestproject-0.1.4/airtestProject.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-10 23:50:19.000000 airtestproject-0.1.4/airtestProject.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 23:50:20.019267 airtestproject-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      851 2024-05-10 23:48:33.000000 airtestproject-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 00:14:44.124967 airtestproject-0.1.5/
+-rw-rw-rw-   0        0        0     1093 2024-05-10 09:37:02.000000 airtestproject-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      789 2024-05-11 00:14:44.122973 airtestproject-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2024-05-11 00:14:26.000000 airtestproject-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 00:14:44.036204 airtestproject-0.1.5/airtestProject/
+-rw-rw-rw-   0        0        0        0 2024-05-09 06:02:26.000000 airtestproject-0.1.5/airtestProject/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 00:14:44.049170 airtestproject-0.1.5/airtestProject/abstractBase/
+-rw-rw-rw-   0        0        0     1786 2024-05-09 11:56:31.000000 airtestproject-0.1.5/airtestProject/abstractBase/OperateBase.py
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.5/airtestProject/abstractBase/__init__.py
+-rw-rw-rw-   0        0        0      196 2024-04-25 04:13:07.000000 airtestproject-0.1.5/airtestProject/abstractBase/loginBase.py
+drwxrwxrwx   0        0        0        0 2024-05-11 00:14:44.053159 airtestproject-0.1.5/airtestProject/commons/
+drwxrwxrwx   0        0        0        0 2024-05-11 00:14:44.054155 airtestproject-0.1.5/airtestProject/commons/Position/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.5/airtestProject/commons/Position/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 00:14:44.057171 airtestproject-0.1.5/airtestProject/commons/Position/odin/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.5/airtestProject/commons/Position/odin/__init__.py
+-rw-rw-rw-   0        0        0       35 2024-04-15 08:30:41.000000 airtestproject-0.1.5/airtestProject/commons/Position/odin/odinPos.py
+-rw-rw-rw-   0        0        0    11611 2024-05-10 08:12:02.000000 airtestproject-0.1.5/airtestProject/commons/UWA.py
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.5/airtestProject/commons/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 00:14:44.058164 airtestproject-0.1.5/airtestProject/commons/page/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.5/airtestProject/commons/page/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 00:14:44.065126 airtestproject-0.1.5/airtestProject/commons/page/odin/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.5/airtestProject/commons/page/odin/__init__.py
+-rw-rw-rw-   0        0        0    19248 2024-05-10 14:46:42.000000 airtestproject-0.1.5/airtestProject/commons/page/odin/funcListCheck.py
+-rw-rw-rw-   0        0        0     9193 2024-05-10 14:46:42.000000 airtestproject-0.1.5/airtestProject/commons/page/odin/login.py
+-rw-rw-rw-   0        0        0     6203 2024-05-10 14:46:42.000000 airtestproject-0.1.5/airtestProject/commons/page/odin/run.py
+drwxrwxrwx   0        0        0        0 2024-05-11 00:14:44.067120 airtestproject-0.1.5/airtestProject/commons/process/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.5/airtestProject/commons/process/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 00:14:44.070142 airtestproject-0.1.5/airtestProject/commons/process/odin/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.5/airtestProject/commons/process/odin/__init__.py
+-rw-rw-rw-   0        0        0     1636 2024-05-10 14:46:42.000000 airtestproject-0.1.5/airtestProject/commons/process/odin/profile.py
+drwxrwxrwx   0        0        0        0 2024-05-11 00:14:44.102052 airtestproject-0.1.5/airtestProject/commons/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.5/airtestProject/commons/utils/__init__.py
+-rw-rw-rw-   0        0        0     5314 2024-05-10 14:46:42.000000 airtestproject-0.1.5/airtestProject/commons/utils/air.py
+-rw-rw-rw-   0        0        0      705 2024-05-10 15:22:52.000000 airtestproject-0.1.5/airtestProject/commons/utils/appStart.py
+-rw-rw-rw-   0        0        0     3523 2024-05-10 14:46:42.000000 airtestproject-0.1.5/airtestProject/commons/utils/command.py
+-rw-rw-rw-   0        0        0     2740 2024-04-26 03:34:41.000000 airtestproject-0.1.5/airtestProject/commons/utils/deploy.py
+-rw-rw-rw-   0        0        0     5655 2024-05-11 00:07:48.000000 airtestproject-0.1.5/airtestProject/commons/utils/excel_image.py
+-rw-rw-rw-   0        0        0      687 2024-04-10 04:18:58.000000 airtestproject-0.1.5/airtestProject/commons/utils/exception.py
+-rw-rw-rw-   0        0        0     3384 2024-04-10 04:18:58.000000 airtestproject-0.1.5/airtestProject/commons/utils/factory.py
+-rw-rw-rw-   0        0        0    12632 2024-05-10 14:46:42.000000 airtestproject-0.1.5/airtestProject/commons/utils/ganaratePyCase.py
+-rw-rw-rw-   0        0        0     2730 2024-05-10 14:46:42.000000 airtestproject-0.1.5/airtestProject/commons/utils/genaratePy.py
+-rw-rw-rw-   0        0        0     3548 2024-05-10 14:46:42.000000 airtestproject-0.1.5/airtestProject/commons/utils/gotCommon.py
+-rw-rw-rw-   0        0        0     5472 2024-05-08 10:15:18.000000 airtestproject-0.1.5/airtestProject/commons/utils/logger.py
+-rw-rw-rw-   0        0        0    11125 2024-05-10 23:59:21.000000 airtestproject-0.1.5/airtestProject/commons/utils/myAirtest.py
+-rw-rw-rw-   0        0        0     7332 2024-05-10 14:46:42.000000 airtestproject-0.1.5/airtestProject/commons/utils/myPoco.py
+-rw-rw-rw-   0        0        0     8139 2024-05-10 23:57:10.000000 airtestproject-0.1.5/airtestProject/commons/utils/ocrTemplate.py
+-rw-rw-rw-   0        0        0     9032 2024-05-10 14:46:42.000000 airtestproject-0.1.5/airtestProject/commons/utils/page.py
+-rw-rw-rw-   0        0        0     6154 2024-05-10 10:40:07.000000 airtestproject-0.1.5/airtestProject/commons/utils/reportUtil.py
+-rw-rw-rw-   0        0        0     1444 2024-04-12 14:52:30.000000 airtestproject-0.1.5/airtestProject/commons/utils/send.py
+-rw-rw-rw-   0        0        0     1744 2024-05-11 00:02:22.000000 airtestproject-0.1.5/airtestProject/commons/utils/tools.py
+-rw-rw-rw-   0        0        0    14349 2024-05-10 14:46:42.000000 airtestproject-0.1.5/airtestProject/commons/utils/utils.py
+-rw-rw-rw-   0        0        0      497 2024-04-30 04:52:37.000000 airtestproject-0.1.5/airtestProject/config.py
+drwxrwxrwx   0        0        0        0 2024-05-11 00:14:44.106017 airtestproject-0.1.5/airtestProject/factory/
+-rw-rw-rw-   0        0        0      292 2024-04-12 14:52:30.000000 airtestproject-0.1.5/airtestProject/factory/SingletonFactory.py
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.5/airtestProject/factory/__init__.py
+-rw-rw-rw-   0        0        0     1930 2024-05-10 14:46:42.000000 airtestproject-0.1.5/airtestProject/factory/operateFactory.py
+drwxrwxrwx   0        0        0        0 2024-05-11 00:14:44.117015 airtestproject-0.1.5/airtestProject/manager/
+-rw-rw-rw-   0        0        0     9413 2024-05-10 23:48:07.000000 airtestproject-0.1.5/airtestProject/manager/DeviceManager.py
+-rw-rw-rw-   0        0        0     6827 2024-04-30 04:52:37.000000 airtestproject-0.1.5/airtestProject/manager/LogManager.py
+-rw-rw-rw-   0        0        0     2895 2024-05-10 14:46:42.000000 airtestproject-0.1.5/airtestProject/manager/PackageManager.py
+-rw-rw-rw-   0        0        0    24575 2024-05-10 14:46:42.000000 airtestproject-0.1.5/airtestProject/manager/ReportManager.py
+-rw-rw-rw-   0        0        0     1786 2024-05-10 14:46:42.000000 airtestproject-0.1.5/airtestProject/manager/TaskManager.py
+-rw-rw-rw-   0        0        0     4832 2024-05-10 14:46:42.000000 airtestproject-0.1.5/airtestProject/manager/TestCaseManager.py
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.5/airtestProject/manager/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 00:14:44.119980 airtestproject-0.1.5/airtestProject/scripts/
+-rw-rw-rw-   0        0        0     1959 2024-05-10 15:22:52.000000 airtestproject-0.1.5/airtestProject/scripts/OdinExample.py
+-rw-rw-rw-   0        0        0        0 2024-03-12 02:10:28.000000 airtestproject-0.1.5/airtestProject/scripts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 00:14:44.121974 airtestproject-0.1.5/airtestProject.egg-info/
+-rw-rw-rw-   0        0        0      789 2024-05-11 00:14:43.000000 airtestproject-0.1.5/airtestProject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2229 2024-05-11 00:14:44.000000 airtestproject-0.1.5/airtestProject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 00:14:43.000000 airtestproject-0.1.5/airtestProject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      159 2024-05-11 00:14:43.000000 airtestproject-0.1.5/airtestProject.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-11 00:14:43.000000 airtestproject-0.1.5/airtestProject.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-11 00:14:44.124967 airtestproject-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      851 2024-05-11 00:12:46.000000 airtestproject-0.1.5/setup.py
```

### Comparing `airtestproject-0.1.4/LICENSE` & `airtestproject-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.4/PKG-INFO` & `airtestproject-0.1.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airtestProject
-Version: 0.1.4
+Version: 0.1.5
 Author: mortal_sjh
 Author-email: mortal_sjh@qq.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: airtest==1.3.3
 Requires-Dist: openpyxl==1.1.0
@@ -19,8 +19,12 @@
 
 ### 测试包体
 
 pip inatsll airtestProject 即可下载安装。
 
 最好用的airtest二次封装。
 
-三七出品必属精品
+三七出品必属精品。
+
+使用封装好的auto_setup需要在根目录下创建文件夹log和reports
+
+需要在跟目录文件夹下创建images
```

### Comparing `airtestproject-0.1.4/airtestProject/abstractBase/OperateBase.py` & `airtestproject-0.1.5/airtestProject/abstractBase/OperateBase.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.4/airtestProject/commons/UWA.py` & `airtestproject-0.1.5/airtestProject/commons/UWA.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.4/airtestProject/commons/page/odin/funcListCheck.py` & `airtestproject-0.1.5/airtestProject/commons/page/odin/funcListCheck.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.4/airtestProject/commons/page/odin/login.py` & `airtestproject-0.1.5/airtestProject/commons/page/odin/login.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.4/airtestProject/commons/page/odin/run.py` & `airtestproject-0.1.5/airtestProject/commons/page/odin/run.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.4/airtestProject/commons/process/odin/profile.py` & `airtestproject-0.1.5/airtestProject/commons/process/odin/profile.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.4/airtestProject/commons/utils/air.py` & `airtestproject-0.1.5/airtestProject/commons/utils/air.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.4/airtestProject/commons/utils/appStart.py` & `airtestproject-0.1.5/airtestProject/commons/utils/appStart.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.4/airtestProject/commons/utils/command.py` & `airtestproject-0.1.5/airtestProject/commons/utils/command.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.4/airtestProject/commons/utils/deploy.py` & `airtestproject-0.1.5/airtestProject/commons/utils/deploy.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.4/airtestProject/commons/utils/excel_image.py` & `airtestproject-0.1.5/airtestProject/commons/utils/excel_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,16 +59,16 @@
 
 
 def handle_images(deps, archive, project, dir_name) -> []:
     """
     将图片二进制内容另存为
     """
     images = {}
-    # if not PILImage:  # Pillow not installed, drop images
-    #     return images
+    # if not PILImage:  # Pillow not installed, drop img
+    #     return img
 
     for dep in deps:
         if dep.Type != IMAGE_NS:
             msg = "{0} 不支持的图像格式".format(dep.Type)
             print(msg)
             continue
```

### Comparing `airtestproject-0.1.4/airtestProject/commons/utils/exception.py` & `airtestproject-0.1.5/airtestProject/commons/utils/exception.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.4/airtestProject/commons/utils/factory.py` & `airtestproject-0.1.5/airtestProject/commons/utils/factory.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.4/airtestProject/commons/utils/ganaratePyCase.py` & `airtestproject-0.1.5/airtestProject/commons/utils/ganaratePyCase.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.4/airtestProject/commons/utils/genaratePy.py` & `airtestproject-0.1.5/airtestProject/commons/utils/genaratePy.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.4/airtestProject/commons/utils/gotCommon.py` & `airtestproject-0.1.5/airtestProject/commons/utils/gotCommon.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.4/airtestProject/commons/utils/logger.py` & `airtestproject-0.1.5/airtestProject/commons/utils/logger.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.4/airtestProject/commons/utils/myAirtest.py` & `airtestproject-0.1.5/airtestProject/commons/utils/myAirtest.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from airtest.core.error import TargetNotFoundError
 
 from airtestProject.commons.utils.logger import log
 from airtestProject.abstractBase.OperateBase import OperateABC
 import time
 
 from airtestProject.commons.utils.ocrTemplate import OcrTemplate
+from airtestProject.commons.utils.tools import get_folder_path_up
 
 
 class AirTest(OperateABC):
 
     def __init__(self, language):
         super(AirTest, self).__init__()
         self.this_dict = None
```

### Comparing `airtestproject-0.1.4/airtestProject/commons/utils/myPoco.py` & `airtestproject-0.1.5/airtestProject/commons/utils/myPoco.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.4/airtestProject/commons/utils/ocrTemplate.py` & `airtestproject-0.1.5/airtestProject/commons/utils/ocrTemplate.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,10 +203,10 @@
         except aircv.BaseError as err:
             G.LOGGING.debug(repr(err))
             return None
         else:
             return ret
 
 # 测试代码
-# img_text = cv2.imread(r"G:\pyProject\odin-testautomation\TestAutomation\airtestProject\commons\images\odin\test (2).png")
+# img_text = cv2.imread(r"G:\pyProject\odin-testautomation\TestAutomation\airtestProject\commons\img\odin\test (2).png")
 # rett = OcrTemplate("RTT: 142ms", language=['ch']).match_in(img_text)
 # print(rett)
```

### Comparing `airtestproject-0.1.4/airtestProject/commons/utils/page.py` & `airtestproject-0.1.5/airtestProject/commons/utils/page.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.4/airtestProject/commons/utils/reportUtil.py` & `airtestproject-0.1.5/airtestProject/commons/utils/reportUtil.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.4/airtestProject/commons/utils/send.py` & `airtestproject-0.1.5/airtestProject/commons/utils/send.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.4/airtestProject/commons/utils/tools.py` & `airtestproject-0.1.5/airtestProject/commons/utils/tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,29 +17,29 @@
     while True:
         if os.path.exists(os.path.join(result_path, folder_name)):
             # 当前文件路径下有对应文件夹路径
             result_path = os.path.join(result_path, folder_name)
             break
         elif result_path == os.path.dirname(result_path):
             # 去到根目录还未找到文件夹路径
-            raise "未找到 'images' 文件夹"
+            raise Exception(f"未找到 '{folder_name}' 文件夹，需要在根目录下创建{folder_name}文件夹")
         else:
             # 向上查找文件夹路径
             result_path = os.path.dirname(result_path)
     return result_path
 
 
 def get_folder_path_down(current_path, folder_name):
-    # 检查当前路径下是否有 'images' 文件夹
-    if 'images' in os.listdir(current_path):
+    # 检查当前路径下是否有 'img' 文件夹
+    if folder_name in os.listdir(current_path):
         return os.path.join(current_path, folder_name)
 
     # 在每个子目录中递归查找
     for subdir in os.listdir(current_path):
         full_subdir = os.path.join(current_path, subdir)
         if os.path.isdir(full_subdir):
             result = get_folder_path_down(current_path, folder_name)
             if result is not None:
                 return result
 
-    # 如果在当前路径及其所有子目录中都没有找到 'images' 文件夹，返回 None
+    # 如果在当前路径及其所有子目录中都没有找到 'img' 文件夹，返回 None
     return None
```

### Comparing `airtestproject-0.1.4/airtestProject/commons/utils/utils.py` & `airtestproject-0.1.5/airtestProject/commons/utils/utils.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.4/airtestProject/factory/operateFactory.py` & `airtestproject-0.1.5/airtestProject/factory/operateFactory.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.4/airtestProject/manager/DeviceManager.py` & `airtestproject-0.1.5/airtestProject/manager/DeviceManager.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.4/airtestProject/manager/LogManager.py` & `airtestproject-0.1.5/airtestProject/manager/LogManager.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.4/airtestProject/manager/PackageManager.py` & `airtestproject-0.1.5/airtestProject/manager/PackageManager.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.4/airtestProject/manager/ReportManager.py` & `airtestproject-0.1.5/airtestProject/manager/ReportManager.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.4/airtestProject/manager/TaskManager.py` & `airtestproject-0.1.5/airtestProject/manager/TaskManager.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.4/airtestProject/manager/TestCaseManager.py` & `airtestproject-0.1.5/airtestProject/manager/TestCaseManager.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.4/airtestProject/scripts/OdinExample.py` & `airtestproject-0.1.5/airtestProject/scripts/OdinExample.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.4/airtestProject.egg-info/PKG-INFO` & `airtestproject-0.1.5/airtestProject.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airtestProject
-Version: 0.1.4
+Version: 0.1.5
 Author: mortal_sjh
 Author-email: mortal_sjh@qq.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: airtest==1.3.3
 Requires-Dist: openpyxl==1.1.0
@@ -19,8 +19,12 @@
 
 ### 测试包体
 
 pip inatsll airtestProject 即可下载安装。
 
 最好用的airtest二次封装。
 
-三七出品必属精品
+三七出品必属精品。
+
+使用封装好的auto_setup需要在根目录下创建文件夹log和reports
+
+需要在跟目录文件夹下创建images
```

### Comparing `airtestproject-0.1.4/airtestProject.egg-info/SOURCES.txt` & `airtestproject-0.1.5/airtestProject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.4/setup.py` & `airtestproject-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name='airtestProject',
-    version='0.1.4',
+    version='0.1.5',
     packages=find_packages(include=['airtestProject', 'airtestProject.*']),
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         "airtest==1.3.3",
         "openpyxl==1.1.0",
         "pocoui==1.0.94",
```

