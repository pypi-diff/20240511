# Comparing `tmp/auto-test-common-2.0.5.tar.gz` & `tmp/auto-test-common-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-test-common-2.0.5.tar", last modified: Fri May 10 01:39:43 2024, max compression
+gzip compressed data, was "auto-test-common-2.0.6.tar", last modified: Fri May 10 08:01:57 2024, max compression
```

## Comparing `auto-test-common-2.0.5.tar` & `auto-test-common-2.0.6.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 01:39:43.135099 auto-test-common-2.0.5/
--rw-r--r--   0 edz        (502) staff       (20)      628 2024-05-10 01:39:43.135267 auto-test-common-2.0.5/PKG-INFO
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 01:39:43.073640 auto-test-common-2.0.5/auto_test_common.egg-info/
--rw-r--r--   0 edz        (502) staff       (20)      628 2024-05-10 01:39:42.000000 auto-test-common-2.0.5/auto_test_common.egg-info/PKG-INFO
--rw-r--r--   0 edz        (502) staff       (20)     1821 2024-05-10 01:39:42.000000 auto-test-common-2.0.5/auto_test_common.egg-info/SOURCES.txt
--rw-r--r--   0 edz        (502) staff       (20)        1 2024-05-10 01:39:42.000000 auto-test-common-2.0.5/auto_test_common.egg-info/dependency_links.txt
--rw-r--r--   0 edz        (502) staff       (20)       57 2024-05-10 01:39:42.000000 auto-test-common-2.0.5/auto_test_common.egg-info/entry_points.txt
--rw-r--r--   0 edz        (502) staff       (20)      727 2024-05-10 01:39:42.000000 auto-test-common-2.0.5/auto_test_common.egg-info/requires.txt
--rw-r--r--   0 edz        (502) staff       (20)        7 2024-05-10 01:39:42.000000 auto-test-common-2.0.5/auto_test_common.egg-info/top_level.txt
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 01:39:43.074413 auto-test-common-2.0.5/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-2.0.5/common/__init__.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 01:39:43.077442 auto-test-common-2.0.5/common/autotest/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-2.0.5/common/autotest/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     5450 2024-04-24 07:01:06.000000 auto-test-common-2.0.5/common/autotest/assert_function.py
--rw-r--r--   0 edz        (502) staff       (20)    12818 2024-04-30 05:25:45.000000 auto-test-common-2.0.5/common/autotest/base_requests.py
--rw-r--r--   0 edz        (502) staff       (20)     8348 2024-05-10 01:35:28.000000 auto-test-common-2.0.5/common/autotest/handle_allure.py
--rw-r--r--   0 edz        (502) staff       (20)    14203 2024-04-24 05:16:27.000000 auto-test-common-2.0.5/common/autotest/handle_assert.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 01:39:43.080884 auto-test-common-2.0.5/common/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-2.0.5/common/common/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     8052 2024-05-10 01:20:06.000000 auto-test-common-2.0.5/common/common/api_driver.py
--rw-r--r--   0 edz        (502) staff       (20)     3808 2023-12-19 05:35:52.000000 auto-test-common-2.0.5/common/common/constant.py
--rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-2.0.5/common/common/test.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 01:39:43.085472 auto-test-common-2.0.5/common/config/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.5/common/config/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2808 2023-08-29 05:34:25.000000 auto-test-common-2.0.5/common/config/config.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 01:39:43.092268 auto-test-common-2.0.5/common/data/
--rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-2.0.5/common/data/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    25961 2024-04-24 05:16:27.000000 auto-test-common-2.0.5/common/data/data_process.py
--rw-r--r--   0 edz        (502) staff       (20)      426 2024-04-24 00:46:49.000000 auto-test-common-2.0.5/common/data/eval_data_handle.py
--rw-r--r--   0 edz        (502) staff       (20)     7933 2024-04-24 05:16:27.000000 auto-test-common-2.0.5/common/data/faker_handle.py
--rw-r--r--   0 edz        (502) staff       (20)    12614 2024-04-24 05:16:27.000000 auto-test-common-2.0.5/common/data/handle_common.py
--rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-12 02:50:37.000000 auto-test-common-2.0.5/common/data/template_data.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 01:39:43.097081 auto-test-common-2.0.5/common/db/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.5/common/db/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-2.0.5/common/db/handle_db.py
--rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-2.0.5/common/db/handle_db_batch.py
--rw-r--r--   0 edz        (502) staff       (20)     1991 2024-04-24 00:46:49.000000 auto-test-common-2.0.5/common/db/handle_mongo.py
--rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-2.0.5/common/db/handle_mysqldb.py
--rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-2.0.5/common/db/handle_oracle.py
--rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-2.0.5/common/db/handle_sqlserver.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 01:39:43.098774 auto-test-common-2.0.5/common/driver/
--rw-r--r--   0 edz        (502) staff       (20)        0 2023-06-05 07:58:39.000000 auto-test-common-2.0.5/common/driver/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)      127 2023-06-05 08:02:38.000000 auto-test-common-2.0.5/common/driver/api_page.py
--rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-05 08:02:38.000000 auto-test-common-2.0.5/common/driver/ui_page.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 01:39:43.105893 auto-test-common-2.0.5/common/file/
--rw-r--r--   0 edz        (502) staff       (20)     5030 2024-04-24 05:16:27.000000 auto-test-common-2.0.5/common/file/ReadFile.py
--rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-2.0.5/common/file/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    10873 2024-04-24 00:46:49.000000 auto-test-common-2.0.5/common/file/handle_excel.py
--rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-2.0.5/common/file/handle_file.py
--rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-2.0.5/common/file/handle_reques.py
--rw-r--r--   0 edz        (502) staff       (20)     2360 2024-04-24 00:46:49.000000 auto-test-common-2.0.5/common/file/handle_system.py
--rw-r--r--   0 edz        (502) staff       (20)      955 2023-06-01 02:02:40.000000 auto-test-common-2.0.5/common/file/handle_yaml.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 01:39:43.107092 auto-test-common-2.0.5/common/mq/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.5/common/mq/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-2.0.5/common/mq/handle_rabbit.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 01:39:43.113519 auto-test-common-2.0.5/common/plat/
--rw-r--r--   0 edz        (502) staff       (20)     3385 2024-01-10 05:46:42.000000 auto-test-common-2.0.5/common/plat/ATF_platform.py
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-2.0.5/common/plat/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-2.0.5/common/plat/jenkin_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     7734 2023-11-29 00:51:05.000000 auto-test-common-2.0.5/common/plat/jira_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     7268 2023-11-30 01:02:07.000000 auto-test-common-2.0.5/common/plat/mysql_platform.py
--rw-r--r--   0 edz        (502) staff       (20)    17680 2024-04-24 00:46:49.000000 auto-test-common-2.0.5/common/plat/service_platform.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 01:39:43.133474 auto-test-common-2.0.5/common/plugin/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-2.0.5/common/plugin/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1527 2024-04-24 00:46:49.000000 auto-test-common-2.0.5/common/plugin/allure_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     5156 2024-04-24 00:46:49.000000 auto-test-common-2.0.5/common/plugin/assert_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    10554 2024-04-24 00:46:49.000000 auto-test-common-2.0.5/common/plugin/atf_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     7770 2024-04-24 00:46:49.000000 auto-test-common-2.0.5/common/plugin/data_bus.py
--rw-r--r--   0 edz        (502) staff       (20)     5415 2024-04-24 00:46:49.000000 auto-test-common-2.0.5/common/plugin/data_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13056 2024-04-24 05:10:23.000000 auto-test-common-2.0.5/common/plugin/file_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-2.0.5/common/plugin/hooks_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)       30 2023-06-08 05:24:28.000000 auto-test-common-2.0.5/common/plugin/my_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13130 2023-05-31 08:41:08.000000 auto-test-common-2.0.5/common/plugin/pytest_playwright.py
--rw-r--r--   0 edz        (502) staff       (20)    23509 2024-05-06 01:03:53.000000 auto-test-common-2.0.5/common/plugin/pytest_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     1421 2023-08-23 05:46:04.000000 auto-test-common-2.0.5/common/plugin/template_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     2090 2024-04-24 00:46:49.000000 auto-test-common-2.0.5/common/plugin/yaml_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      443 2024-05-10 01:39:43.137821 auto-test-common-2.0.5/setup.cfg
--rw-r--r--   0 edz        (502) staff       (20)     2101 2024-04-30 05:32:18.000000 auto-test-common-2.0.5/setup.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 08:01:57.780775 auto-test-common-2.0.6/
+-rw-r--r--   0 edz        (502) staff       (20)      628 2024-05-10 08:01:57.781028 auto-test-common-2.0.6/PKG-INFO
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 08:01:57.731320 auto-test-common-2.0.6/auto_test_common.egg-info/
+-rw-r--r--   0 edz        (502) staff       (20)      628 2024-05-10 08:01:57.000000 auto-test-common-2.0.6/auto_test_common.egg-info/PKG-INFO
+-rw-r--r--   0 edz        (502) staff       (20)     1821 2024-05-10 08:01:57.000000 auto-test-common-2.0.6/auto_test_common.egg-info/SOURCES.txt
+-rw-r--r--   0 edz        (502) staff       (20)        1 2024-05-10 08:01:57.000000 auto-test-common-2.0.6/auto_test_common.egg-info/dependency_links.txt
+-rw-r--r--   0 edz        (502) staff       (20)       57 2024-05-10 08:01:57.000000 auto-test-common-2.0.6/auto_test_common.egg-info/entry_points.txt
+-rw-r--r--   0 edz        (502) staff       (20)      727 2024-05-10 08:01:57.000000 auto-test-common-2.0.6/auto_test_common.egg-info/requires.txt
+-rw-r--r--   0 edz        (502) staff       (20)        7 2024-05-10 08:01:57.000000 auto-test-common-2.0.6/auto_test_common.egg-info/top_level.txt
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 08:01:57.731733 auto-test-common-2.0.6/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-2.0.6/common/__init__.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 08:01:57.734995 auto-test-common-2.0.6/common/autotest/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-2.0.6/common/autotest/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     5450 2024-04-24 07:01:06.000000 auto-test-common-2.0.6/common/autotest/assert_function.py
+-rw-r--r--   0 edz        (502) staff       (20)    12837 2024-05-10 02:49:12.000000 auto-test-common-2.0.6/common/autotest/base_requests.py
+-rw-r--r--   0 edz        (502) staff       (20)     8348 2024-05-10 01:35:28.000000 auto-test-common-2.0.6/common/autotest/handle_allure.py
+-rw-r--r--   0 edz        (502) staff       (20)    14203 2024-04-24 05:16:27.000000 auto-test-common-2.0.6/common/autotest/handle_assert.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 08:01:57.738196 auto-test-common-2.0.6/common/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-2.0.6/common/common/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     8622 2024-05-10 05:45:27.000000 auto-test-common-2.0.6/common/common/api_driver.py
+-rw-r--r--   0 edz        (502) staff       (20)     3808 2023-12-19 05:35:52.000000 auto-test-common-2.0.6/common/common/constant.py
+-rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-2.0.6/common/common/test.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 08:01:57.744288 auto-test-common-2.0.6/common/config/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.6/common/config/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2808 2023-08-29 05:34:25.000000 auto-test-common-2.0.6/common/config/config.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 08:01:57.750494 auto-test-common-2.0.6/common/data/
+-rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-2.0.6/common/data/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    25961 2024-04-24 05:16:27.000000 auto-test-common-2.0.6/common/data/data_process.py
+-rw-r--r--   0 edz        (502) staff       (20)      426 2024-04-24 00:46:49.000000 auto-test-common-2.0.6/common/data/eval_data_handle.py
+-rw-r--r--   0 edz        (502) staff       (20)     7933 2024-04-24 05:16:27.000000 auto-test-common-2.0.6/common/data/faker_handle.py
+-rw-r--r--   0 edz        (502) staff       (20)    12614 2024-04-24 05:16:27.000000 auto-test-common-2.0.6/common/data/handle_common.py
+-rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-12 02:50:37.000000 auto-test-common-2.0.6/common/data/template_data.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 08:01:57.755551 auto-test-common-2.0.6/common/db/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.6/common/db/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-2.0.6/common/db/handle_db.py
+-rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-2.0.6/common/db/handle_db_batch.py
+-rw-r--r--   0 edz        (502) staff       (20)     1991 2024-04-24 00:46:49.000000 auto-test-common-2.0.6/common/db/handle_mongo.py
+-rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-2.0.6/common/db/handle_mysqldb.py
+-rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-2.0.6/common/db/handle_oracle.py
+-rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-2.0.6/common/db/handle_sqlserver.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 08:01:57.757938 auto-test-common-2.0.6/common/driver/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2023-06-05 07:58:39.000000 auto-test-common-2.0.6/common/driver/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)      127 2023-06-05 08:02:38.000000 auto-test-common-2.0.6/common/driver/api_page.py
+-rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-05 08:02:38.000000 auto-test-common-2.0.6/common/driver/ui_page.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 08:01:57.764501 auto-test-common-2.0.6/common/file/
+-rw-r--r--   0 edz        (502) staff       (20)     5030 2024-04-24 05:16:27.000000 auto-test-common-2.0.6/common/file/ReadFile.py
+-rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-2.0.6/common/file/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    10873 2024-04-24 00:46:49.000000 auto-test-common-2.0.6/common/file/handle_excel.py
+-rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-2.0.6/common/file/handle_file.py
+-rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-2.0.6/common/file/handle_reques.py
+-rw-r--r--   0 edz        (502) staff       (20)     2360 2024-04-24 00:46:49.000000 auto-test-common-2.0.6/common/file/handle_system.py
+-rw-r--r--   0 edz        (502) staff       (20)      955 2023-06-01 02:02:40.000000 auto-test-common-2.0.6/common/file/handle_yaml.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 08:01:57.765807 auto-test-common-2.0.6/common/mq/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.6/common/mq/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-2.0.6/common/mq/handle_rabbit.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 08:01:57.770464 auto-test-common-2.0.6/common/plat/
+-rw-r--r--   0 edz        (502) staff       (20)     3385 2024-01-10 05:46:42.000000 auto-test-common-2.0.6/common/plat/ATF_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-2.0.6/common/plat/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-2.0.6/common/plat/jenkin_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     7734 2023-11-29 00:51:05.000000 auto-test-common-2.0.6/common/plat/jira_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     7268 2023-11-30 01:02:07.000000 auto-test-common-2.0.6/common/plat/mysql_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)    17680 2024-04-24 00:46:49.000000 auto-test-common-2.0.6/common/plat/service_platform.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 08:01:57.779845 auto-test-common-2.0.6/common/plugin/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-2.0.6/common/plugin/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1527 2024-04-24 00:46:49.000000 auto-test-common-2.0.6/common/plugin/allure_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     5156 2024-04-24 00:46:49.000000 auto-test-common-2.0.6/common/plugin/assert_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    10554 2024-04-24 00:46:49.000000 auto-test-common-2.0.6/common/plugin/atf_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     7770 2024-04-24 00:46:49.000000 auto-test-common-2.0.6/common/plugin/data_bus.py
+-rw-r--r--   0 edz        (502) staff       (20)     5415 2024-04-24 00:46:49.000000 auto-test-common-2.0.6/common/plugin/data_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13056 2024-04-24 05:10:23.000000 auto-test-common-2.0.6/common/plugin/file_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-2.0.6/common/plugin/hooks_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)       30 2023-06-08 05:24:28.000000 auto-test-common-2.0.6/common/plugin/my_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13130 2023-05-31 08:41:08.000000 auto-test-common-2.0.6/common/plugin/pytest_playwright.py
+-rw-r--r--   0 edz        (502) staff       (20)    23509 2024-05-06 01:03:53.000000 auto-test-common-2.0.6/common/plugin/pytest_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     1421 2023-08-23 05:46:04.000000 auto-test-common-2.0.6/common/plugin/template_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     2090 2024-04-24 00:46:49.000000 auto-test-common-2.0.6/common/plugin/yaml_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      443 2024-05-10 08:01:57.781836 auto-test-common-2.0.6/setup.cfg
+-rw-r--r--   0 edz        (502) staff       (20)     2101 2024-04-30 05:32:18.000000 auto-test-common-2.0.6/setup.py
```

### Comparing `auto-test-common-2.0.5/PKG-INFO` & `auto-test-common-2.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-test-common
-Version: 2.0.5
+Version: 2.0.6
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `auto-test-common-2.0.5/auto_test_common.egg-info/PKG-INFO` & `auto-test-common-2.0.6/auto_test_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-test-common
-Version: 2.0.5
+Version: 2.0.6
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `auto-test-common-2.0.5/auto_test_common.egg-info/SOURCES.txt` & `auto-test-common-2.0.6/auto_test_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/auto_test_common.egg-info/requires.txt` & `auto-test-common-2.0.6/auto_test_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/autotest/assert_function.py` & `auto-test-common-2.0.6/common/autotest/assert_function.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/autotest/base_requests.py` & `auto-test-common-2.0.6/common/autotest/base_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
                             from common.plugin.file_plugin import FilePlugin
                             content = FilePlugin.load_data(content['file'])
                     data = req_expr(content=content, data=data, _no_content=0)
             if 'datatype' in schemal_data:
                 datatype = schemal_data['datatype']
             if 'format' in schemal_data:
                 datatype = schemal_data['format']
-            data = BaseRequest.handle_body(data, datatype)
+            data = BaseRequest.handle_body(data, datatype,_replace)
         except Exception as e:
             data = data
         if 'file' in schemal_data and file is None:
             file = schemal_body['file']
         file_obj = DataProcess.handler_files(file)
         if step == '测试接口详情' and DataProcess.isNotNull(schemal_data['desc']):
             step = '测试接口详情:'+schemal_data['desc']
@@ -165,15 +165,15 @@
                 MysqlPlatForm.insert_api_data(url, schemal_data['method'], header, data, res.elapsed.total_seconds(), res.status_code)
         except:
             logger.warning("保存请求数据异常")
         return res
 
 
     @classmethod
-    def handle_body(self, data, format):
+    def handle_body(self, data, format, _replace):
         test_data = data
         try:
             if format == 'text':
                 test_data = DataProcess.handle_data(variable=data, jsonformat=False, _replace=_replace)
             elif format == 'json':
                 test_data = DataProcess.handle_data(variable=data, _replace=_replace)
             elif format == 'None':
```

### Comparing `auto-test-common-2.0.5/common/autotest/handle_allure.py` & `auto-test-common-2.0.6/common/autotest/handle_allure.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/autotest/handle_assert.py` & `auto-test-common-2.0.6/common/autotest/handle_assert.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/common/api_driver.py` & `auto-test-common-2.0.6/common/common/api_driver.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import requests
 from common.autotest.handle_allure import allure_api_step, allure_step
 from requests_toolbelt import MultipartEncoder
 from os import path
 import os
 from common.config.config import TEST_FILE_PATH
 import copy
+from loguru import logger
+import json
 
 
 class APIDriver(object):
 
     session = None
 
     @classmethod
@@ -43,49 +45,49 @@
             header,header_desc = cls.getCommontHeader(header)
             res = session.request(method=method, url=url, params=data, headers=header, cookies=cookie,
                                   auth=_auth,verify=False)
             allure_api_step(desc, url, method, header_desc, data, '', res)
 
         elif parametric_key == 'data':
             header,header_desc = cls.getCommontHeader(header)
-            res = session.request(method=method, url=url, data=cls.dataEncode(data), files=file, headers=header, cookies=cookie,
+            res = session.request(method=method, url=url, data=cls.hand_form_data(data, header), files=file, headers=header, cookies=cookie,
                                   auth=_auth,verify=False)
             allure_api_step(desc, url, method, header_desc, data, file, res)
 
         elif parametric_key == 'text':
             header,header_desc = cls.getCommontHeader(header)
             header['Content-Type'] = 'text/plain'
-            res = session.request(method=method, url=url, data=cls.dataEncode(data), files=file, headers=header, cookies=cookie,
+            res = session.request(method=method, url=url, data=data, files=file, headers=header, cookies=cookie,
                                   auth=_auth, verify=False)
             allure_api_step(desc, url, method, header_desc, data, file, res)
 
         elif parametric_key == 'json':
             header,header_desc = cls.getCommontHeader(header)
             header['Content-Type'] = 'application/json'
             res = session.request(method=method, url=url, json=data, files=file, headers=header, cookies=cookie,
                                   auth=_auth,verify=False)
             allure_api_step(desc, url, method, header_desc, data, file, res)
 
         elif parametric_key == 'xml':
             header,header_desc = cls.getCommontHeader(header)
             header['Content-Type'] = 'application/xml'
-            res = session.request(method=method, url=url, data=cls.dataEncode(data), files=file, headers=header, cookies=cookie,
+            res = session.request(method=method, url=url, data=data, files=file, headers=header, cookies=cookie,
                                   auth=_auth, verify=False)
             allure_api_step(desc, url, method, header_desc, data, file, res)
 
         elif parametric_key == 'form':
             header,header_desc = cls.getCommontHeader(header)
             header['Content-Type'] = 'application/x-www-form-urlencoded'
             try:
                 if isinstance(data, str):
                     from common.data.data_process import DataProcess
                     data = DataProcess.handle_data(data)
             except Exception as e:
                 logger.info(f'测试数据：{data} 转换异常:' + repr(e))
-            res = session.request(method=method, url=url, data=cls.dataEncode(data), files=file, headers=header, cookies=cookie,
+            res = session.request(method=method, url=url, data=cls.hand_form_data(data,header), files=file, headers=header, cookies=cookie,
                                   auth=_auth, verify=False)
             allure_api_step(desc, url, method, header_desc, data, file, res)
 
         elif parametric_key == 'form-data':
             if data is not None:
                 data = cls.handleFile(data)
                 m = MultipartEncoder(data)
@@ -96,14 +98,29 @@
                 allure_api_step(desc, url, method, header_desc, data, file, res)
         else:
             raise ValueError('可选关键字为params, data, xml, json, text, form,form-urlencoded')
         session.close()
         return res
 
     @classmethod
+    def hand_form_data(self, _data, header):
+        _temp = _data
+        try:
+            if header is not None and isinstance(header,dict):
+                if 'Content-Type' in header:
+                    if header['Content-Type'].find('x-www-form-urlencoded') >= 0:
+                        if isinstance(_data, str):
+                            _temp = json.loads(_data)
+        except Exception as e:
+            logger.warning(f'{_data} 转换Json失败')
+        _temp = self.dataEncode(_temp)
+        return _temp
+
+
+    @classmethod
     def getCommontHeader(self, header):
         if header is None:
             header = {'User-Agent':'Mozilla/5.0 (Windows NT 10.0; Win64; x64) Chrome/83.0.4103.116 Safari/537.36',
                       'Connection':'keep-alive',
                       'Accept-Encoding':'gzip, deflate, br',
                       'Accept-Language':'zh-CN,zh;q=0.9',
                       'Accept':'*/*'}
```

### Comparing `auto-test-common-2.0.5/common/common/constant.py` & `auto-test-common-2.0.6/common/common/constant.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/common/test.py` & `auto-test-common-2.0.6/common/common/test.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/config/config.py` & `auto-test-common-2.0.6/common/config/config.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/data/data_process.py` & `auto-test-common-2.0.6/common/data/data_process.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/data/faker_handle.py` & `auto-test-common-2.0.6/common/data/faker_handle.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/data/handle_common.py` & `auto-test-common-2.0.6/common/data/handle_common.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/data/template_data.py` & `auto-test-common-2.0.6/common/data/template_data.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/db/handle_db.py` & `auto-test-common-2.0.6/common/db/handle_db.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/db/handle_db_batch.py` & `auto-test-common-2.0.6/common/db/handle_db_batch.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/db/handle_mongo.py` & `auto-test-common-2.0.6/common/db/handle_mongo.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/db/handle_mysqldb.py` & `auto-test-common-2.0.6/common/db/handle_mysqldb.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/db/handle_oracle.py` & `auto-test-common-2.0.6/common/db/handle_oracle.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/db/handle_sqlserver.py` & `auto-test-common-2.0.6/common/db/handle_sqlserver.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/driver/ui_page.py` & `auto-test-common-2.0.6/common/driver/ui_page.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/file/ReadFile.py` & `auto-test-common-2.0.6/common/file/ReadFile.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/file/handle_excel.py` & `auto-test-common-2.0.6/common/file/handle_excel.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/file/handle_file.py` & `auto-test-common-2.0.6/common/file/handle_file.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/file/handle_reques.py` & `auto-test-common-2.0.6/common/file/handle_reques.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/file/handle_system.py` & `auto-test-common-2.0.6/common/file/handle_system.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/file/handle_yaml.py` & `auto-test-common-2.0.6/common/file/handle_yaml.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/mq/handle_rabbit.py` & `auto-test-common-2.0.6/common/mq/handle_rabbit.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/plat/ATF_platform.py` & `auto-test-common-2.0.6/common/plat/ATF_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/plat/jenkin_platform.py` & `auto-test-common-2.0.6/common/plat/jenkin_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/plat/jira_platform.py` & `auto-test-common-2.0.6/common/plat/jira_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/plat/mysql_platform.py` & `auto-test-common-2.0.6/common/plat/mysql_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/plat/service_platform.py` & `auto-test-common-2.0.6/common/plat/service_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/plugin/allure_plugin.py` & `auto-test-common-2.0.6/common/plugin/allure_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/plugin/assert_plugin.py` & `auto-test-common-2.0.6/common/plugin/assert_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/plugin/atf_plugin.py` & `auto-test-common-2.0.6/common/plugin/atf_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/plugin/data_bus.py` & `auto-test-common-2.0.6/common/plugin/data_bus.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/plugin/data_plugin.py` & `auto-test-common-2.0.6/common/plugin/data_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/plugin/file_plugin.py` & `auto-test-common-2.0.6/common/plugin/file_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/plugin/hooks_plugin.py` & `auto-test-common-2.0.6/common/plugin/hooks_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/plugin/pytest_playwright.py` & `auto-test-common-2.0.6/common/plugin/pytest_playwright.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/plugin/pytest_plugin.py` & `auto-test-common-2.0.6/common/plugin/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/plugin/template_plugin.py` & `auto-test-common-2.0.6/common/plugin/template_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/common/plugin/yaml_plugin.py` & `auto-test-common-2.0.6/common/plugin/yaml_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.5/setup.py` & `auto-test-common-2.0.6/setup.py`

 * *Files identical despite different names*

