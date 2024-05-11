# Comparing `tmp/airtestproject-0.1.2.tar.gz` & `tmp/airtestproject-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "G:\pyProject\odin-testautomation\TestAutomation\dist\.tmp-c2obb5gw\airtestproject-0.1.2.tar", last modified: Fri May 10 15:23:01 2024, max compression
+gzip compressed data, was "G:\pyProject\odin-testautomation\TestAutomation\dist\.tmp-8z5fmj0i\airtestproject-0.1.3.tar", last modified: Fri May 10 23:36:58 2024, max compression
```

## Comparing `airtestproject-0.1.2.tar` & `airtestproject-0.1.3.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 15:23:01.924800 airtestproject-0.1.2/
--rw-rw-rw-   0        0        0     1093 2024-05-10 09:37:02.000000 airtestproject-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      623 2024-05-10 15:23:01.923803 airtestproject-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      134 2024-05-10 09:55:18.000000 airtestproject-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 15:23:01.841024 airtestproject-0.1.2/airtestProject/
--rw-rw-rw-   0        0        0        0 2024-05-09 06:02:26.000000 airtestproject-0.1.2/airtestProject/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:23:01.852992 airtestproject-0.1.2/airtestProject/abstractBase/
--rw-rw-rw-   0        0        0     1786 2024-05-09 11:56:31.000000 airtestproject-0.1.2/airtestProject/abstractBase/OperateBase.py
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.2/airtestProject/abstractBase/__init__.py
--rw-rw-rw-   0        0        0      196 2024-04-25 04:13:07.000000 airtestproject-0.1.2/airtestProject/abstractBase/loginBase.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:23:01.855985 airtestproject-0.1.2/airtestProject/commons/
-drwxrwxrwx   0        0        0        0 2024-05-10 15:23:01.857979 airtestproject-0.1.2/airtestProject/commons/Position/
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.2/airtestProject/commons/Position/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:23:01.859973 airtestproject-0.1.2/airtestProject/commons/Position/odin/
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.2/airtestProject/commons/Position/odin/__init__.py
--rw-rw-rw-   0        0        0       35 2024-04-15 08:30:41.000000 airtestproject-0.1.2/airtestProject/commons/Position/odin/odinPos.py
--rw-rw-rw-   0        0        0    11611 2024-05-10 08:12:02.000000 airtestproject-0.1.2/airtestProject/commons/UWA.py
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.2/airtestProject/commons/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:23:01.861967 airtestproject-0.1.2/airtestProject/commons/page/
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.2/airtestProject/commons/page/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:23:01.866955 airtestproject-0.1.2/airtestProject/commons/page/odin/
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.2/airtestProject/commons/page/odin/__init__.py
--rw-rw-rw-   0        0        0    19248 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/commons/page/odin/funcListCheck.py
--rw-rw-rw-   0        0        0     9193 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/commons/page/odin/login.py
--rw-rw-rw-   0        0        0     6203 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/commons/page/odin/run.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:23:01.868977 airtestproject-0.1.2/airtestProject/commons/process/
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.2/airtestProject/commons/process/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:23:01.871941 airtestproject-0.1.2/airtestProject/commons/process/odin/
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.2/airtestProject/commons/process/odin/__init__.py
--rw-rw-rw-   0        0        0     1636 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/commons/process/odin/profile.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:23:01.902889 airtestproject-0.1.2/airtestProject/commons/utils/
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.2/airtestProject/commons/utils/__init__.py
--rw-rw-rw-   0        0        0     5314 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/commons/utils/air.py
--rw-rw-rw-   0        0        0      705 2024-05-10 15:22:52.000000 airtestproject-0.1.2/airtestProject/commons/utils/appStart.py
--rw-rw-rw-   0        0        0     3523 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/commons/utils/command.py
--rw-rw-rw-   0        0        0     2740 2024-04-26 03:34:41.000000 airtestproject-0.1.2/airtestProject/commons/utils/deploy.py
--rw-rw-rw-   0        0        0     5661 2024-04-29 08:44:46.000000 airtestproject-0.1.2/airtestProject/commons/utils/excel_image.py
--rw-rw-rw-   0        0        0      687 2024-04-10 04:18:58.000000 airtestproject-0.1.2/airtestProject/commons/utils/exception.py
--rw-rw-rw-   0        0        0     3384 2024-04-10 04:18:58.000000 airtestproject-0.1.2/airtestProject/commons/utils/factory.py
--rw-rw-rw-   0        0        0    12632 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/commons/utils/ganaratePyCase.py
--rw-rw-rw-   0        0        0     2730 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/commons/utils/genaratePy.py
--rw-rw-rw-   0        0        0     3548 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/commons/utils/gotCommon.py
--rw-rw-rw-   0        0        0     5472 2024-05-08 10:15:18.000000 airtestproject-0.1.2/airtestProject/commons/utils/logger.py
--rw-rw-rw-   0        0        0    11058 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/commons/utils/myAirtest.py
--rw-rw-rw-   0        0        0     7332 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/commons/utils/myPoco.py
--rw-rw-rw-   0        0        0     8142 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/commons/utils/ocrTemplate.py
--rw-rw-rw-   0        0        0     9032 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/commons/utils/page.py
--rw-rw-rw-   0        0        0     6154 2024-05-10 10:40:07.000000 airtestproject-0.1.2/airtestProject/commons/utils/reportUtil.py
--rw-rw-rw-   0        0        0     1444 2024-04-12 14:52:30.000000 airtestproject-0.1.2/airtestProject/commons/utils/send.py
--rw-rw-rw-   0        0        0     1676 2024-05-10 08:00:06.000000 airtestproject-0.1.2/airtestProject/commons/utils/tools.py
--rw-rw-rw-   0        0        0    14349 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/commons/utils/utils.py
--rw-rw-rw-   0        0        0      497 2024-04-30 04:52:37.000000 airtestproject-0.1.2/airtestProject/config.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:23:01.907848 airtestproject-0.1.2/airtestProject/factory/
--rw-rw-rw-   0        0        0      292 2024-04-12 14:52:30.000000 airtestproject-0.1.2/airtestProject/factory/SingletonFactory.py
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.2/airtestProject/factory/__init__.py
--rw-rw-rw-   0        0        0     1930 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/factory/operateFactory.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:23:01.917819 airtestproject-0.1.2/airtestProject/manager/
--rw-rw-rw-   0        0        0     9282 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/manager/DeviceManager.py
--rw-rw-rw-   0        0        0     6827 2024-04-30 04:52:37.000000 airtestproject-0.1.2/airtestProject/manager/LogManager.py
--rw-rw-rw-   0        0        0     2895 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/manager/PackageManager.py
--rw-rw-rw-   0        0        0    24575 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/manager/ReportManager.py
--rw-rw-rw-   0        0        0     1786 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/manager/TaskManager.py
--rw-rw-rw-   0        0        0     4832 2024-05-10 14:46:42.000000 airtestproject-0.1.2/airtestProject/manager/TestCaseManager.py
--rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.2/airtestProject/manager/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:23:01.920811 airtestproject-0.1.2/airtestProject/scripts/
--rw-rw-rw-   0        0        0     1959 2024-05-10 15:22:52.000000 airtestproject-0.1.2/airtestProject/scripts/OdinExample.py
--rw-rw-rw-   0        0        0        0 2024-03-12 02:10:28.000000 airtestproject-0.1.2/airtestProject/scripts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:23:01.922805 airtestproject-0.1.2/airtestProject.egg-info/
--rw-rw-rw-   0        0        0      623 2024-05-10 15:23:01.000000 airtestproject-0.1.2/airtestProject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2229 2024-05-10 15:23:01.000000 airtestproject-0.1.2/airtestProject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 15:23:01.000000 airtestproject-0.1.2/airtestProject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      139 2024-05-10 15:23:01.000000 airtestproject-0.1.2/airtestProject.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-10 15:23:01.000000 airtestproject-0.1.2/airtestProject.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 15:23:01.924800 airtestproject-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      819 2024-05-10 14:47:14.000000 airtestproject-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 23:36:58.363271 airtestproject-0.1.3/
+-rw-rw-rw-   0        0        0     1093 2024-05-10 09:37:02.000000 airtestproject-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      659 2024-05-10 23:36:58.362274 airtestproject-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      134 2024-05-10 09:55:18.000000 airtestproject-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 23:36:58.252567 airtestproject-0.1.3/airtestProject/
+-rw-rw-rw-   0        0        0        0 2024-05-09 06:02:26.000000 airtestproject-0.1.3/airtestProject/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 23:36:58.267527 airtestproject-0.1.3/airtestProject/abstractBase/
+-rw-rw-rw-   0        0        0     1786 2024-05-09 11:56:31.000000 airtestproject-0.1.3/airtestProject/abstractBase/OperateBase.py
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.3/airtestProject/abstractBase/__init__.py
+-rw-rw-rw-   0        0        0      196 2024-04-25 04:13:07.000000 airtestproject-0.1.3/airtestProject/abstractBase/loginBase.py
+drwxrwxrwx   0        0        0        0 2024-05-10 23:36:58.271517 airtestproject-0.1.3/airtestProject/commons/
+drwxrwxrwx   0        0        0        0 2024-05-10 23:36:58.273512 airtestproject-0.1.3/airtestProject/commons/Position/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.3/airtestProject/commons/Position/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 23:36:58.277554 airtestproject-0.1.3/airtestProject/commons/Position/odin/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.3/airtestProject/commons/Position/odin/__init__.py
+-rw-rw-rw-   0        0        0       35 2024-04-15 08:30:41.000000 airtestproject-0.1.3/airtestProject/commons/Position/odin/odinPos.py
+-rw-rw-rw-   0        0        0    11611 2024-05-10 08:12:02.000000 airtestproject-0.1.3/airtestProject/commons/UWA.py
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.3/airtestProject/commons/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 23:36:58.279497 airtestproject-0.1.3/airtestProject/commons/page/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.3/airtestProject/commons/page/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 23:36:58.286476 airtestproject-0.1.3/airtestProject/commons/page/odin/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.3/airtestProject/commons/page/odin/__init__.py
+-rw-rw-rw-   0        0        0    19248 2024-05-10 14:46:42.000000 airtestproject-0.1.3/airtestProject/commons/page/odin/funcListCheck.py
+-rw-rw-rw-   0        0        0     9193 2024-05-10 14:46:42.000000 airtestproject-0.1.3/airtestProject/commons/page/odin/login.py
+-rw-rw-rw-   0        0        0     6203 2024-05-10 14:46:42.000000 airtestproject-0.1.3/airtestProject/commons/page/odin/run.py
+drwxrwxrwx   0        0        0        0 2024-05-10 23:36:58.288472 airtestproject-0.1.3/airtestProject/commons/process/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.3/airtestProject/commons/process/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 23:36:58.292463 airtestproject-0.1.3/airtestProject/commons/process/odin/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.3/airtestProject/commons/process/odin/__init__.py
+-rw-rw-rw-   0        0        0     1636 2024-05-10 14:46:42.000000 airtestproject-0.1.3/airtestProject/commons/process/odin/profile.py
+drwxrwxrwx   0        0        0        0 2024-05-10 23:36:58.335346 airtestproject-0.1.3/airtestProject/commons/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.3/airtestProject/commons/utils/__init__.py
+-rw-rw-rw-   0        0        0     5314 2024-05-10 14:46:42.000000 airtestproject-0.1.3/airtestProject/commons/utils/air.py
+-rw-rw-rw-   0        0        0      705 2024-05-10 15:22:52.000000 airtestproject-0.1.3/airtestProject/commons/utils/appStart.py
+-rw-rw-rw-   0        0        0     3523 2024-05-10 14:46:42.000000 airtestproject-0.1.3/airtestProject/commons/utils/command.py
+-rw-rw-rw-   0        0        0     2740 2024-04-26 03:34:41.000000 airtestproject-0.1.3/airtestProject/commons/utils/deploy.py
+-rw-rw-rw-   0        0        0     5661 2024-04-29 08:44:46.000000 airtestproject-0.1.3/airtestProject/commons/utils/excel_image.py
+-rw-rw-rw-   0        0        0      687 2024-04-10 04:18:58.000000 airtestproject-0.1.3/airtestProject/commons/utils/exception.py
+-rw-rw-rw-   0        0        0     3384 2024-04-10 04:18:58.000000 airtestproject-0.1.3/airtestProject/commons/utils/factory.py
+-rw-rw-rw-   0        0        0    12632 2024-05-10 14:46:42.000000 airtestproject-0.1.3/airtestProject/commons/utils/ganaratePyCase.py
+-rw-rw-rw-   0        0        0     2730 2024-05-10 14:46:42.000000 airtestproject-0.1.3/airtestProject/commons/utils/genaratePy.py
+-rw-rw-rw-   0        0        0     3548 2024-05-10 14:46:42.000000 airtestproject-0.1.3/airtestProject/commons/utils/gotCommon.py
+-rw-rw-rw-   0        0        0     5472 2024-05-08 10:15:18.000000 airtestproject-0.1.3/airtestProject/commons/utils/logger.py
+-rw-rw-rw-   0        0        0    11058 2024-05-10 14:46:42.000000 airtestproject-0.1.3/airtestProject/commons/utils/myAirtest.py
+-rw-rw-rw-   0        0        0     7332 2024-05-10 14:46:42.000000 airtestproject-0.1.3/airtestProject/commons/utils/myPoco.py
+-rw-rw-rw-   0        0        0     8142 2024-05-10 14:46:42.000000 airtestproject-0.1.3/airtestProject/commons/utils/ocrTemplate.py
+-rw-rw-rw-   0        0        0     9032 2024-05-10 14:46:42.000000 airtestproject-0.1.3/airtestProject/commons/utils/page.py
+-rw-rw-rw-   0        0        0     6154 2024-05-10 10:40:07.000000 airtestproject-0.1.3/airtestProject/commons/utils/reportUtil.py
+-rw-rw-rw-   0        0        0     1444 2024-04-12 14:52:30.000000 airtestproject-0.1.3/airtestProject/commons/utils/send.py
+-rw-rw-rw-   0        0        0     1676 2024-05-10 08:00:06.000000 airtestproject-0.1.3/airtestProject/commons/utils/tools.py
+-rw-rw-rw-   0        0        0    14349 2024-05-10 14:46:42.000000 airtestproject-0.1.3/airtestProject/commons/utils/utils.py
+-rw-rw-rw-   0        0        0      497 2024-04-30 04:52:37.000000 airtestproject-0.1.3/airtestProject/config.py
+drwxrwxrwx   0        0        0        0 2024-05-10 23:36:58.341332 airtestproject-0.1.3/airtestProject/factory/
+-rw-rw-rw-   0        0        0      292 2024-04-12 14:52:30.000000 airtestproject-0.1.3/airtestProject/factory/SingletonFactory.py
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.3/airtestProject/factory/__init__.py
+-rw-rw-rw-   0        0        0     1930 2024-05-10 14:46:42.000000 airtestproject-0.1.3/airtestProject/factory/operateFactory.py
+drwxrwxrwx   0        0        0        0 2024-05-10 23:36:58.354295 airtestproject-0.1.3/airtestProject/manager/
+-rw-rw-rw-   0        0        0     9282 2024-05-10 14:46:42.000000 airtestproject-0.1.3/airtestProject/manager/DeviceManager.py
+-rw-rw-rw-   0        0        0     6827 2024-04-30 04:52:37.000000 airtestproject-0.1.3/airtestProject/manager/LogManager.py
+-rw-rw-rw-   0        0        0     2895 2024-05-10 14:46:42.000000 airtestproject-0.1.3/airtestProject/manager/PackageManager.py
+-rw-rw-rw-   0        0        0    24575 2024-05-10 14:46:42.000000 airtestproject-0.1.3/airtestProject/manager/ReportManager.py
+-rw-rw-rw-   0        0        0     1786 2024-05-10 14:46:42.000000 airtestproject-0.1.3/airtestProject/manager/TaskManager.py
+-rw-rw-rw-   0        0        0     4832 2024-05-10 14:46:42.000000 airtestproject-0.1.3/airtestProject/manager/TestCaseManager.py
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:30:56.000000 airtestproject-0.1.3/airtestProject/manager/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 23:36:58.358286 airtestproject-0.1.3/airtestProject/scripts/
+-rw-rw-rw-   0        0        0     1959 2024-05-10 15:22:52.000000 airtestproject-0.1.3/airtestProject/scripts/OdinExample.py
+-rw-rw-rw-   0        0        0        0 2024-03-12 02:10:28.000000 airtestproject-0.1.3/airtestProject/scripts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 23:36:58.360279 airtestproject-0.1.3/airtestProject.egg-info/
+-rw-rw-rw-   0        0        0      659 2024-05-10 23:36:58.000000 airtestproject-0.1.3/airtestProject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2229 2024-05-10 23:36:58.000000 airtestproject-0.1.3/airtestProject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 23:36:58.000000 airtestproject-0.1.3/airtestProject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      159 2024-05-10 23:36:58.000000 airtestproject-0.1.3/airtestProject.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-10 23:36:58.000000 airtestproject-0.1.3/airtestProject.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 23:36:58.363271 airtestproject-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      851 2024-05-10 23:36:48.000000 airtestproject-0.1.3/setup.py
```

### Comparing `airtestproject-0.1.2/LICENSE` & `airtestproject-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/PKG-INFO` & `airtestproject-0.1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: airtestProject
-Version: 0.1.2
+Version: 0.1.3
 Author: mortal_sjh
 Author-email: mortal_sjh@qq.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: airtest==1.3.3
 Requires-Dist: openpyxl==1.1.0
 Requires-Dist: pocoui==1.0.94
 Requires-Dist: qrcode==7.4.2
 Requires-Dist: Requests==2.31.0
 Requires-Dist: watchdog==4.0.0
 Requires-Dist: easyocr==1.7.1
 Requires-Dist: paddleocr==2.7.3
 Requires-Dist: loguru==0.5.3
+Requires-Dist: paddlepaddle==2.6.1
 
 ### 测试包体
 
 pip inatsll airtestProject 即可下载安装。
 
 最好用的airtest二次封装。
```

### Comparing `airtestproject-0.1.2/airtestProject/abstractBase/OperateBase.py` & `airtestproject-0.1.3/airtestProject/abstractBase/OperateBase.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject/commons/UWA.py` & `airtestproject-0.1.3/airtestProject/commons/UWA.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject/commons/page/odin/funcListCheck.py` & `airtestproject-0.1.3/airtestProject/commons/page/odin/funcListCheck.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject/commons/page/odin/login.py` & `airtestproject-0.1.3/airtestProject/commons/page/odin/login.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject/commons/page/odin/run.py` & `airtestproject-0.1.3/airtestProject/commons/page/odin/run.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject/commons/process/odin/profile.py` & `airtestproject-0.1.3/airtestProject/commons/process/odin/profile.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject/commons/utils/air.py` & `airtestproject-0.1.3/airtestProject/commons/utils/air.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject/commons/utils/appStart.py` & `airtestproject-0.1.3/airtestProject/commons/utils/appStart.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject/commons/utils/command.py` & `airtestproject-0.1.3/airtestProject/commons/utils/command.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject/commons/utils/deploy.py` & `airtestproject-0.1.3/airtestProject/commons/utils/deploy.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject/commons/utils/excel_image.py` & `airtestproject-0.1.3/airtestProject/commons/utils/excel_image.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject/commons/utils/exception.py` & `airtestproject-0.1.3/airtestProject/commons/utils/exception.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject/commons/utils/factory.py` & `airtestproject-0.1.3/airtestProject/commons/utils/factory.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject/commons/utils/ganaratePyCase.py` & `airtestproject-0.1.3/airtestProject/commons/utils/ganaratePyCase.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject/commons/utils/genaratePy.py` & `airtestproject-0.1.3/airtestProject/commons/utils/genaratePy.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject/commons/utils/gotCommon.py` & `airtestproject-0.1.3/airtestProject/commons/utils/gotCommon.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject/commons/utils/logger.py` & `airtestproject-0.1.3/airtestProject/commons/utils/logger.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject/commons/utils/myAirtest.py` & `airtestproject-0.1.3/airtestProject/commons/utils/myAirtest.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject/commons/utils/myPoco.py` & `airtestproject-0.1.3/airtestProject/commons/utils/myPoco.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject/commons/utils/ocrTemplate.py` & `airtestproject-0.1.3/airtestProject/commons/utils/ocrTemplate.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject/commons/utils/page.py` & `airtestproject-0.1.3/airtestProject/commons/utils/page.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject/commons/utils/reportUtil.py` & `airtestproject-0.1.3/airtestProject/commons/utils/reportUtil.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject/commons/utils/send.py` & `airtestproject-0.1.3/airtestProject/commons/utils/send.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject/commons/utils/tools.py` & `airtestproject-0.1.3/airtestProject/commons/utils/tools.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject/commons/utils/utils.py` & `airtestproject-0.1.3/airtestProject/commons/utils/utils.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject/factory/operateFactory.py` & `airtestproject-0.1.3/airtestProject/factory/operateFactory.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject/manager/DeviceManager.py` & `airtestproject-0.1.3/airtestProject/manager/DeviceManager.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject/manager/LogManager.py` & `airtestproject-0.1.3/airtestProject/manager/LogManager.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject/manager/PackageManager.py` & `airtestproject-0.1.3/airtestProject/manager/PackageManager.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject/manager/ReportManager.py` & `airtestproject-0.1.3/airtestProject/manager/ReportManager.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject/manager/TaskManager.py` & `airtestproject-0.1.3/airtestProject/manager/TaskManager.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject/manager/TestCaseManager.py` & `airtestproject-0.1.3/airtestProject/manager/TestCaseManager.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject/scripts/OdinExample.py` & `airtestproject-0.1.3/airtestProject/scripts/OdinExample.py`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/airtestProject.egg-info/PKG-INFO` & `airtestproject-0.1.3/airtestProject.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: airtestProject
-Version: 0.1.2
+Version: 0.1.3
 Author: mortal_sjh
 Author-email: mortal_sjh@qq.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: airtest==1.3.3
 Requires-Dist: openpyxl==1.1.0
 Requires-Dist: pocoui==1.0.94
 Requires-Dist: qrcode==7.4.2
 Requires-Dist: Requests==2.31.0
 Requires-Dist: watchdog==4.0.0
 Requires-Dist: easyocr==1.7.1
 Requires-Dist: paddleocr==2.7.3
 Requires-Dist: loguru==0.5.3
+Requires-Dist: paddlepaddle==2.6.1
 
 ### 测试包体
 
 pip inatsll airtestProject 即可下载安装。
 
 最好用的airtest二次封装。
```

### Comparing `airtestproject-0.1.2/airtestProject.egg-info/SOURCES.txt` & `airtestproject-0.1.3/airtestProject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airtestproject-0.1.2/setup.py` & `airtestproject-0.1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name='airtestProject',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(include=['airtestProject', 'airtestProject.*']),
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         "airtest==1.3.3",
         "openpyxl==1.1.0",
         "pocoui==1.0.94",
         "qrcode==7.4.2",
         "Requests==2.31.0",
         "watchdog==4.0.0",
         "easyocr==1.7.1",
         "paddleocr==2.7.3",
-        "loguru==0.5.3"
+        "loguru==0.5.3",
+        "paddlepaddle==2.6.1"
         # 项目依赖项列表
     ],
     python_requires='>=3.9',
     author="mortal_sjh",                                     # 作者
     author_email="mortal_sjh@qq.com"
 )
```
