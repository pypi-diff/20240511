# Comparing `tmp/linktest-2.7.6.tar.gz` & `tmp/linktest-2.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.7.6.tar", last modified: Fri May 10 09:09:59 2024, max compression
+gzip compressed data, was "linktest-2.7.7.tar", last modified: Sat May 11 14:51:50 2024, max compression
```

## Comparing `linktest-2.7.6.tar` & `linktest-2.7.7.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-10 09:09:59.737899 linktest-2.7.6/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-10 09:09:59.737625 linktest-2.7.6/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-10 09:09:59.735150 linktest-2.7.6/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-05-10 08:22:07.000000 linktest-2.7.6/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/detect_delimiter.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16684 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16093 2024-05-10 06:04:13.000000 linktest-2.7.6/linktest/generate_html_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    32360 2024-05-10 09:07:21.000000 linktest-2.7.6/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8676 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   103040 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/re_func.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1334 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2188 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9534 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-10 08:22:14.000000 linktest-2.7.6/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3445 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14288 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/webdriver_wrapper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14075 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/webdriver_wrapper_chrome.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13707 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/webdriver_wrapper_edge.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13725 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/webdriver_wrapper_firefox.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13695 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/webdriver_wrapper_ie.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14139 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/webdriver_wrapper_safari.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-05-10 05:53:00.000000 linktest-2.7.6/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-10 09:09:59.737239 linktest-2.7.6/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-10 09:09:59.000000 linktest-2.7.6/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1451 2024-05-10 09:09:59.000000 linktest-2.7.6/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-05-10 09:09:59.000000 linktest-2.7.6/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-05-10 09:09:59.000000 linktest-2.7.6/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-05-10 09:09:59.000000 linktest-2.7.6/linktest.egg-info/top_level.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-05-10 09:09:59.737959 linktest-2.7.6/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-10 09:09:54.000000 linktest-2.7.6/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-11 14:51:50.131667 linktest-2.7.7/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-11 14:51:50.131429 linktest-2.7.7/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-11 14:51:50.129233 linktest-2.7.7/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-05-11 14:26:27.000000 linktest-2.7.7/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-05-11 14:27:40.000000 linktest-2.7.7/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/detect_delimiter.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16684 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16243 2024-05-10 09:40:20.000000 linktest-2.7.7/linktest/generate_html_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    37992 2024-05-11 14:45:31.000000 linktest-2.7.7/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8676 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   102849 2024-05-11 08:42:16.000000 linktest-2.7.7/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/re_func.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1334 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2170 2024-05-10 09:36:35.000000 linktest-2.7.7/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9534 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-11 14:26:34.000000 linktest-2.7.7/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3445 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14288 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/webdriver_wrapper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14075 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/webdriver_wrapper_chrome.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13707 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/webdriver_wrapper_edge.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13725 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/webdriver_wrapper_firefox.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13695 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/webdriver_wrapper_ie.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14139 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/webdriver_wrapper_safari.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-11 14:51:50.131032 linktest-2.7.7/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-11 14:51:49.000000 linktest-2.7.7/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1451 2024-05-11 14:51:49.000000 linktest-2.7.7/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-05-11 14:51:49.000000 linktest-2.7.7/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-05-11 14:51:49.000000 linktest-2.7.7/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-05-11 14:51:49.000000 linktest-2.7.7/linktest.egg-info/top_level.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-05-11 14:51:50.131722 linktest-2.7.7/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-11 14:51:43.000000 linktest-2.7.7/setup.py
```

### Comparing `linktest-2.7.6/linktest/appium_utils.py` & `linktest-2.7.7/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.6/linktest/auto_generate_testcase_list.py` & `linktest-2.7.7/linktest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.6/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.7.7/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.6/linktest/base_testcase.py` & `linktest-2.7.7/linktest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.6/linktest/clean_data.py` & `linktest-2.7.7/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.6/linktest/conver_xml_into_db.py` & `linktest-2.7.7/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.6/linktest/database_helper.py` & `linktest-2.7.7/linktest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.6/linktest/date_utilities.py` & `linktest-2.7.7/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.6/linktest/doctor.py` & `linktest-2.7.7/linktest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.6/linktest/framework_log.py` & `linktest-2.7.7/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.6/linktest/generate_html_log.py` & `linktest-2.7.7/linktest/generate_html_log.py`

 * *Files 5% similar despite different names*

```diff
@@ -199,33 +199,33 @@
             line += "<img src='" + line.split(
                 "WebDriver Action:</span> <b style='color:#006600; font-size: 20px;'>'save_screenshot'</b> with <b style='color:#333333'>args</b>:")[
                 1].strip() + "' width='100%'>"
 
         # if "logged_requests.py" in line:
         #     line = line.replace("logged_requests.py", "<span style='color:#0066CC'>logged_requests.py</span>")
 
-        if "run_test() start" in line:
-            line = line.replace("run_test() start",
-                                "<strong style='color:#0066CC; font-size: 20px;'>run_test() start</strong>")
-
-        if "setup() start" in line:
-            line = line.replace("setup() start",
-                                "<strong style='color:#0066CC; font-size: 20px;'>setup() start</strong>")
-
-        if "setup() end" in line:
-            line = line.replace("setup() end",
-                                "<strong style='color:#0066CC; font-size: 20px;'>setup() end</strong>")
-
-        if "teardown() start" in line:
-            line = line.replace("teardown() start",
-                                "<strong style='color:#0066CC; font-size: 20px;'>teardown() start</strong>")
-
-        if "teardown() end" in line:
-            line = line.replace("teardown() end",
-                                "<strong style='color:#0066CC; font-size: 20px;'>teardown() end</strong>")
+        if "run_test() Start execution" in line:
+            line = line.replace("run_test() Start execution",
+                                "<strong style='color:#0066CC; font-size: 20px;'>run_test() Start execution</strong>")
+
+        if "setup() Start execution" in line:
+            line = line.replace("setup() Start execution",
+                                "<strong style='color:#0066CC; font-size: 20px;'>setup() Start execution</strong>")
+
+        if "setup() End execution" in line:
+            line = line.replace("setup() End execution",
+                                "<strong style='color:#0066CC; font-size: 20px;'>setup() End execution</strong>")
+
+        if "teardown() Start execution" in line:
+            line = line.replace("teardown() Start execution",
+                                "<strong style='color:#0066CC; font-size: 20px;'>teardown() Start execution</strong>")
+
+        if "teardown() End execution" in line:
+            line = line.replace("teardown() End execution",
+                                "<strong style='color:#0066CC; font-size: 20px;'>teardown() End execution</strong>")
 
         if "cURL Start" in line:
             line = line.replace("cURL Start",
                                 "<strong style='color:#0066CC; font-size: 20px;'>cURL Start</strong>")
 
         if "cURL End" in line:
             line = line.replace("cURL End",
```

### Comparing `linktest-2.7.6/linktest/get_adb_devices.py` & `linktest-2.7.7/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.6/linktest/get_ios_devices_list.py` & `linktest-2.7.7/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.6/linktest/get_platform_info.py` & `linktest-2.7.7/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.6/linktest/get_project_info.py` & `linktest-2.7.7/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.6/linktest/html_report.py` & `linktest-2.7.7/linktest/html_report.py`

 * *Files 19% similar despite different names*

```diff
@@ -82,38 +82,51 @@
             # java script code for filter function
             java_script_code_for_filter = """
             <script type="text/javascript">
 
                 function changeTag(){
                     var my_select = document.getElementById("testcase_tag");
                     if (my_select.value == "tests"){
-                        //all_failed_test_cases is  represent for all failed testcases
+                        //all_failed_test_cases is represent for all failed testcases
                         if(document.getElementById("all_failed_test_cases")){
                             all_failed_test_case = document.getElementById("all_failed_test_cases");
                             all_failed_test_case.style.display="none";
                             all_failed_test_case.style.display="block";
 
                             all_failed_case_list = document.getElementsByClassName("all_failed_case");
                             for(var i=0;i<all_failed_case_list.length;i++){
                                 all_failed_case_list[i].style.display="block";
                             }
-                            document.getElementById("num_fail").innerHTML=i;
+                            if (i > 1){
+                                var new_str = i + " Failed Test Cases";
+                                document.getElementById("num_fail").innerHTML=new_str;
+                            } else {
+                                var new_str = i + " Failed Test Case";
+                                document.getElementById("num_fail").innerHTML=new_str;
+                            }
                         }
 
-                        //all_passed_test_cases is  represent for all passed testcases
+                        //all_passed_test_cases is represent for all passed testcases
                         if (document.getElementById("all_passed_test_cases")){
                             all_passed_test_case = document.getElementById("all_passed_test_cases");
                             all_passed_test_case.style.display="none";
                             all_passed_test_case.style.display="block";
                             all_passed_case_list = document.getElementsByClassName("all_passed_case");
 
                             for(var j=0;j<all_passed_case_list.length;j++){
                                 all_passed_case_list[j].style.display="block";
                             }
-                            document.getElementById("num_pass").innerHTML=j;
+                            if (j > 1){
+                                var new_str = j + " Passed Test Cases";
+                                document.getElementById("num_pass").innerHTML=new_str;
+                                } 
+                            else {
+                                var new_str = j + " Passed Test Case";
+                                document.getElementById("num_pass").innerHTML=new_str;
+                            }
                         }
                     }
 
                     var l = new Array()
                     k = 0;
                     all_failed_case_list = document.getElementsByClassName("all_failed_case");
 
@@ -158,37 +171,103 @@
                         }
                         if ("all_passed_case"==l[i].className){
                             num_passed_case = num_passed_case + 1;
                         }
                     }
 
                     if (document.getElementById("num_fail")){
-                        document.getElementById("num_fail").innerHTML=num_failed_case;
+                        var button = document.getElementById("failed_testcase_names");
+                        if (num_failed_case > 1){
+                            var new_str = num_failed_case + " Failed Test Cases";
+                            document.getElementById("num_fail").innerHTML=new_str;
+                            button.style.display = "";
+                        } else {
+                            var new_str = num_failed_case + " Failed Test Case";
+                            document.getElementById("num_fail").innerHTML=new_str;
+                            if (num_failed_case == 0){
+                                button.style.display = "none";
+                            } else if (num_failed_case == 1){
+                                button.style.display = "";
+                            }
+                        }
                     }
                     if (document.getElementById("num_pass")){
-                        document.getElementById("num_pass").innerHTML=num_passed_case;
+                        var new_str = num_passed_case + " Passed Test Cases";
+
+                        if (num_passed_case > 1){
+                            var new_str = num_passed_case + " Passed Test Cases";
+                            document.getElementById("num_pass").innerHTML=new_str;
+                        } else {
+                            var new_str = num_passed_case + " Passed Test Case";
+                            document.getElementById("num_pass").innerHTML=new_str;
+                        }
                     }
                 }
 
             </script>
             """
 
             java_script_code_for_filter
 
             java_script_copy_failed_testcases = """
             <script>
                 function copyFailedTestCase(){
-                    document.getElementById("failed_testcase_names").style.display="none";
-                    
+                    var button = document.getElementById("failed_testcase_names");
+                    button.style.opacity = "0"; // Set opacity to 0 to make the button invisible
                     document.getElementById("copy_status_info").innerHTML = "<font color=#DC3912>Copied</font>";
                     
                     setTimeout(function(){
                         document.getElementById("copy_status_info").innerHTML = "";
-                        document.getElementById("failed_testcase_names").style.display="block";
+                        button.style.opacity = "1"; // Reset opacity to make the button visible again
                     }, 1000);
+                    
+                    // 获取页面中所有 class="all_failed_case" 的 <tr> 元素
+                    var trElements = document.querySelectorAll('tr.all_failed_case');
+                    
+                    // 准备一个数组来存放满足条件的faield test case name
+                    var selectedFailedCaseNames = [];
+                    
+                    // 遍历所有选取的 <tr> 元素
+                    trElements.forEach(function(tr) {
+                        // 检查每个 <tr> 的显示状态是否为 'block'
+                        // 获取实际应用的样式
+                        var computedStyle = window.getComputedStyle(tr);
+                        
+                        // 检查 'display' 属性是否为 'block' 或者没有明确设置
+                        if (computedStyle.display === 'block' || !tr.hasAttribute('style')) {
+                            // 获取第二个 <td> 元素
+                            var secondTd = tr.children[1]; // 假设 <td> 元素是按顺序的
+                            if (secondTd) {
+                                // 获取第一个 <a> 标签
+                                var firstA = secondTd.querySelector('a');
+                                if (firstA) {
+                                    // 获取 <a> 标签的文本
+                                    var fullText = firstA.textContent.trim();
+                                    // 分割字符串并获取斜杠右边的值
+                                    var parts = fullText.split('/');
+                                    var textAfterSlash = parts.length > 1 ? parts[parts.length - 1] : '';
+                                    // 添加到数组中
+                                    selectedFailedCaseNames.push(textAfterSlash);
+                                }
+                            }
+                        }
+                    });
+                    
+                    // Join the array into a single string with commas separating the values
+                    const textToCopy = selectedFailedCaseNames.join(' ');
+                    
+                    // Using the Clipboard API to copy text
+                    navigator.clipboard.writeText(textToCopy).then(function() {
+                        // Success action, e.g., showing a message
+                        document.getElementById('copy_status_info').textContent = 'Copied!';
+                    }, function(err) {
+                        // Error action
+                        document.getElementById('copy_status_info').textContent = 'Failed to copy!';
+                    });
+                    
                 }
             </script>
             """
 
             js_code_str = """
             <html>
                 <head>
@@ -234,63 +313,63 @@
 
             report_file_handler.write(js_code_str)
 
             environment = settings.ENVIRONMENT
 
             str_top_table = """
             <body>
-            <table align='center'>
+            <table align='center' width='1120px;'>
                 <tr>
                     <td>
                         <div id='chart_div' style="min-width: 621px; height: 360px; migin: 10 auto"></div>
                     </td>
                     <td>
                         <table border='0' class="table table-hover">
                             <tr style='background-color: whitesmoke; min-width: 621px;'>
-                                <th>Test Run Start Timestamp</th>
+                                <th>Start Time</th>
                                 <td align="center">%s</td>
                             </tr>
                             <tr>
-                                <th>Test Run Duration (Seconds)</th>
+                                <th>Duration(s)</th>
                                 <td align='center'>%s</td>
                             </tr>
                             <tr>
-                                <th>Total Test Cases Executed</th>
+                                <th>Total Executed</th>
                                 <td align='center'>%s</td>
                             </tr>
                             <tr>
-                                <th>Test Cases Passed</th>
+                                <th>Passed</th>
                                 <td align='center'>%s</td>
                             </tr>
                             <tr>
-                                <th>Test Cases Failed</th>
+                                <th>Failed</th>
                                 <td align='center'>%s</td>
                             </tr>
                             <tr>
-                                <th>Test Execution Environment</th>
+                                <th>Environment</th>
                                 <td align='center'>%s</td>
                             </tr>
                             <tr>
-                                <th>Threads Used</th>
+                                <th>Threads</th>
                                 <td align='center'>%s</td>
                             </tr>
                             <tr>
-                                <th>Test Host Operating System</th>
+                                <th>OS</th>
                                 <td align='center'>%s</td>
                             </tr>
                             <tr>
-                                <th>Test Framework and Version</th>
+                                <th>Framework</th>
                                 <td align='center'><a target="_blank" href="https://plugins.jetbrains.com/plugin/21600-linktest/versions">linktest %s</a></td>
                             </tr>
                         </table>
                     </td>
                 </tr>
             </table>
             """ % (
-                start_time.strftime("%Y-%m-%d %H:%M:%S %p"),
+                start_time.strftime("%Y-%m-%d %H:%M:%S"),
                 execution_time,
                 len(passed_cases) + failed_cases_count,
                 len(passed_cases),
                 failed_cases_count,
                 environment,
                 settings.QUEUE_SIZE,
                 platform_info,
@@ -309,97 +388,112 @@
                 # begin to fetch all the testcase's tags(according to the testcase' package)
                 for testcase in all_testcases:
                     testcase.testcase_filter_tag = "~"
                     testcase_filter_tag = testcase.__module__[0:testcase.__module__.rfind(".")]
                     map_testcases_package(all_testcases_package, tc_map_tag, testcase_filter_tag, testcase)
 
             # generate the drop down list for all the different tags
-            # 判断是不需要显示 'show Global Data List' button
-            if create_global_data_list_flag:
-                html_drop_down_list = """
-                            <table border='0' align='center' width='1050'>
-                                <tr>
-                                    <td width='280'><font style='color: black; font-size: 18; margin-left: -30'><a class="btn btn-success" target='_blank' role='button'
-                                         href='%s'>View Global Data</a></font></td>
-                                    
-                                </tr>
-                            </table>
-                            
-                            <table border='0' align='center' width='1050'>
-                                <tr>
-                                    <td width='285'><font style='color: black; font-size: 18; margin-left: -30'>Filter Cases By Package: </font></td>
-                                    <td>
-                            """ % (output_folder + os.sep + "global_data_list.py")
-            else:
-                html_drop_down_list = """
-            <br>
-            <table border='0' align='center' width='1050'>
+            html_drop_down_list = """
+            <table border='0' align='center' width='1120'>
                 <tr>
-                    <td width='285'><strong style='color: #555555; font-size: 18; margin-left: -30'>Filter Cases By Package: </strong></td>
+                    <td width='285'><strong style='color: #555555; font-size: 18;'>Select Package: </strong></td>
                     <td>
             """
 
             report_file_handler.write(html_drop_down_list)
 
             all_testcases_package_list = []
             for testcase in all_testcases_package:
                 all_testcases_package_list.append(testcase)
 
             all_testcases_package_list.sort()
-            report_file_handler.write("<select class='form-select' style='margin-left: -100px; overflow: hidden; text-overflow: ellipsis; width: 650;' id=\"testcase_tag\" onchange=\"changeTag()\">")
+            report_file_handler.write("<select class='form-select' style='margin-left: -128px; overflow: hidden; text-overflow: ellipsis; width: 780;' id=\"testcase_tag\" onchange=\"changeTag()\">")
             for testcase in all_testcases_package_list:
                 report_file_handler.write("<option value='%s'>" % testcase)
                 report_file_handler.write("%s" % testcase)
                 report_file_handler.write("</option>")
             report_file_handler.write("</select>")
-            report_file_handler.write("</td><td align='left'><p id='copy_status_info'></p></td><td>")
+            report_file_handler.write("</td>")
+
+            if create_global_data_list_flag:
+                view_global_data_str = """<td style="padding-left: 10px; padding-right: 10px;"> <!-- Adjust padding as needed -->
+                                            <a target='_blank' role='button' href='%s' 
+                                            style="background-color: #3366C5;
+                                            color: white; 
+                                            border: none; 
+                                            border-radius: 5px; 
+                                            padding: 5px 8px;
+                                            font-size: 16px; 
+                                            font-weight: 500;
+                                            text-shadow: 0 1px 2px rgba(0, 0, 0, 0.2); 
+                                            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
+                                            transition: background-color 0.3s, box-shadow 0.3s; 
+                                            cursor: pointer;
+                                            outline: none;">View Global Data</a>
+                                        </td>""" % (output_folder + os.sep + "global_data_list.py")
+                report_file_handler.write(view_global_data_str)
 
             if len(failed_cases) > 0:
                 str_failed_testcase_names = ""
 
                 for failed_testcase in failed_cases:
                     str_failed_testcase_names += failed_testcase.__class__.__name__ + " "
 
-                str_failed_testcases = """
-                <button style='background-color: #DC3912; border: none; border-radius: 6px; margin-top: -10px; margin-left: 10%%; width: 125px; height: 39px;' 
-                id="failed_testcase_names" class='failed_testcase_names'
-                 data-clipboard-text="%s" onclick="copyFailedTestCase()">
-                    <font color='white'>Copy Names of Failed Cases</font>
-                </button>
-                <script>
-                    new Clipboard('.failed_testcase_names');
-                </script>
-                """ % str_failed_testcase_names
-
-                report_file_handler.write(str_failed_testcases)
-
-            report_file_handler.write("</td></tr></table>")
+            report_file_handler.write("</tr></table>")
             report_file_handler.write("<br>")
 
             if len(failed_cases) > 0:
+                str_failed_testcases = """
+                                <button style="
+                                    background-color: #DC3912;
+                                    color: white; 
+                                    border: none; 
+                                    border-radius: 5px; 
+                                    padding: 2px 6px;
+                                    font-size: 14px; 
+                                    font-weight: 500;
+                                    text-shadow: 0 1px 2px rgba(0, 0, 0, 0.2); 
+                                    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
+                                    transition: background-color 0.3s, box-shadow 0.3s; 
+                                    cursor: pointer;
+                                    outline: none;
+                                "
+                                id="failed_testcase_names" class='failed_testcase_names'
+                                title="Click to copy the names of all failed test cases to the clipboard"
+                                 data-clipboard-text="%s" onclick="copyFailedTestCase()">
+                                    <font color='white'>Copy Failures</font>
+                                </button>
+                                <font id='copy_status_info' style='margin-left: -100px;'></font>
+                                <script>
+                                    new Clipboard('.failed_testcase_names');
+                                </script>
+                                """ % str_failed_testcase_names
+
                 failed_testcase_table = """
                 <table align='center'>
                 <tr><td>
                 <table class='table table-hover' border='0'>
                     <tr id='all_failed_test_cases' style='color:black; background-color: whitesmoke;'>
                         <th width='100'>
                                CaseID
                         </th>
                     
-                        <th width='800' style='color: #DC3912;'>
-                                <font id='num_fail'>%s</font><font style='margin-left: 8px;'>Failed %s</font>
+                        <th width='860' style='color: #DC3912;'>
+                                <font id='num_fail'>%s &nbsp; Failed %s</font>
+                                <font style='margin-left: 18px;'>%s</font>
                         </th>
                         <th width='160'>
                             Duration(Seconds)
                         </th>
                         
                     </tr>
                 """ % (
                     failed_cases_count,
-                    "Test Cases" if failed_cases_count > 1 else "Test Case"
+                    "Test Cases" if failed_cases_count > 1 else "Test Case",
+                    str_failed_testcases
                 )
 
                 report_file_handler.write(failed_testcase_table)
 
                 sorted_failed_cases = []
 
                 if settings.RERUN_FLAG:
@@ -428,15 +522,15 @@
 
                     report_file_handler.write(
                         "<td width='100' align='center' style='word-break:break-all;no-wrap:no-wrap'>")
                     report_file_handler.write("%s" % ('-' if getattr(failed_testcase, "testcase_id", "None") == None else getattr(failed_testcase, "testcase_id")))
                     report_file_handler.write("</font></td>")
 
                     testcase_information = """
-                        <td width='800' style='word-break:break-all'>
+                        <td width='860' style='word-break:break-all'>
                         <a  href='%s'>
                             <font color='#333'>
                                 %s
                             </font>
                         </a>
                         """ % (
                         module_name,
@@ -491,16 +585,16 @@
 
                 <table class='table table-hover' border='0'>
                     <tr id='all_passed_test_cases' style='color:balck; background-color: whitesmoke;'>
                         <th width='100'>
                             CaseID
                         </th>
                 
-                        <th width='800' style='color: #3366CC;'>
-                            <font id='num_pass'>%s</font><font style='margin-left: 8px;'>Passed %s</font>
+                        <th width='860' style='color: #3366C5;'>
+                            <font id='num_pass'>%s &nbsp;Passed %s</font>
                         </th>
                         
                         <th width='160'>
                             Duration(Seconds)
                         </th>
                         
                     </tr>
@@ -520,15 +614,15 @@
                                                                                       "testcase_filter_tag",
                                                                                       "None"))
 
                     report_file_handler.write("<td width='100' align='center' >")
                     report_file_handler.write("%s" % ('-' if getattr(passed_testcase, "testcase_id", "None") == None else getattr(passed_testcase, "testcase_id")))
                     report_file_handler.write("</font></td>")
 
-                    report_file_handler.write("<td width='800' style='word-break:break-all'>")
+                    report_file_handler.write("<td width='860' style='word-break:break-all'>")
                     report_file_handler.write("<a title='Click to see the log & screenshot' href='")
                     report_file_handler.write(module_name)
                     report_file_handler.write(
                         "'><font color='%s'>" % (
                             "#333" if passed_testcase.rerun_tag == 0 else "green"))
                     report_file_handler.write(module_name_display)
 
@@ -541,18 +635,18 @@
 
                     report_file_handler.write("</font>")
                     report_file_handler.write("</font></a>")
 
                     try:
                         if passed_testcase.rerun_tag == 0:
                             report_file_handler.write(
-                                "&nbsp; &nbsp; <strong style='color: #555555; '>Log Files: </strong><a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='left' title='View Detailed Log' href='%s'>   <font color='#3366CC'>&nbsp; [TXT </font> </a>" %
+                                "&nbsp; &nbsp; <strong style='color: #555555; '>Log Files: </strong><a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='left' title='View Detailed Log' href='%s'>   <font color='#3366C5'>&nbsp; [TXT </font> </a>" %
                                 passed_testcase.log_file_path)
                             report_file_handler.write(
-                                " |&nbsp; <a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'>   <font color='#3366CC'> HTML]</font> </a>" %
+                                " |&nbsp; <a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'>   <font color='#3366C5'> HTML]</font> </a>" %
                                 passed_testcase.log_file_path.replace("test.log", "test.html"))
                     except BaseException:
                         print(traceback.format_exc())
 
                     try:
                         if passed_testcase.rerun_tag == 1:
                             report_file_handler.write(
@@ -614,15 +708,15 @@
                                 type: 'pie',
                                 radius: '65%%',
                                 data: [
                                     {
                                         value: %s, 
                                         name: 'Passed',
                                         itemStyle: {
-                                            color: "#3366CC"
+                                            color: "#3366C5"
                                         }
                                     },
                                     {
                                         value: %s, 
                                         name: 'Failed', 
                                         itemStyle: {
                                             color: "#DC3912"
```

### Comparing `linktest-2.7.6/linktest/logged_requests.py` & `linktest-2.7.7/linktest/logged_requests.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.6/linktest/main.py` & `linktest-2.7.7/linktest/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 1. settings/__init__.py is used to configure the following items for linktest:
     - Environment (test environment: UAT, QA, PROD, etc.)
     - TESTCASE_TIMEOUT (if a test case's execution is not complete after Testcase_Timeout seconds, a TimeoutException will be thrown)
     - RERUN_FLAG (controls rerunning of failed test cases; default is False)
     - DEBUG_RUN (keeps the browser active after execution is done; default value is False)
     - Show_All_Chrome_Driver_Logs (determines whether to show all webdriver logs; default value is False)
     - QUEUE_SIZE (setting queue_size to 8, for example, means that a maximum of 8 test cases can be executed concurrently)
-    - SAVE_LOG_TO_DB (saves execution logs into testdb; must be used in conjunction with linktest-dashboard)
+    - SAVE_LOG_TO_DB (saves execution logs into testdb; must be used in conjunction with linktest-dashboard, default value is False)
     - generate_xunit_result (saves xunit report; default value is False; used for TestLink integration)
     - AUTO_LOG_HTTP_REQUEST (default value is True; automatically logs request actions)
     - AUTO_DOWNLOAD_CHROMEDRIVER (default value is False; automatically downloads the appropriate Chromedriver based on the Chrome version)
     - AUTO_SCREENSHOT_ON_ACTION (default value is False; automatically generates a screenshot for each WebDriver action)
     - DEFAULT_BROWSER_NAME (default browser name for UI test cases; default value is "chrome")
     - HEAD_LESS (default value is False; runs the browser in headless mode)
     - WEBDRIVER_IMPLICIT_WAIT (default value is 10 seconds; maximum time the WebDriver should wait for an element to be present before throwing an exception)
@@ -916,19 +916,19 @@
                     # 执行 setup() 之前 先 log TestEngineCaseInput(如果是 test-engine 发起的)
                     if BaseTestCase.TestEngineCaseInput:
                         executing_testcase.logger.info("- TestEngineCaseInput:")
                         executing_testcase.logger.info(executing_testcase.TestEngineCaseInput)
 
                     # 先执行 setup()， 再执行 run_test()
                     if hasattr(executing_testcase, "setup"):
-                        executing_testcase.logger.info("- setup() start")
+                        executing_testcase.logger.info(" - setup() Start execution")
                         executing_testcase.setup()
-                        executing_testcase.logger.info("- setup() end")
+                        executing_testcase.logger.info(" - setup() End execution")
 
-                    executing_testcase.logger.info("- run_test() start")
+                    executing_testcase.logger.info(" - run_test() Start execution")
 
                     # For DEBUG_RUN mode,will not set timeout for each testcase
                     executing_testcase.run_test()
 
             except BaseException:
                 executing_testcase.ExecutionStatusSetByFramework = "failed"
                 traceback.print_exc()
@@ -1083,17 +1083,17 @@
                     pass
             finally:
                 # 如果case中 有调用： self.GlobalDataList.append("XXX") 则推荐 settings中设置 ReRun_flag = False
                 executing_testcase.GlobalExecutedCaseList.append(executing_testcase)
 
                 try:
                     if hasattr(executing_testcase, "teardown"):
-                        executing_testcase.logger.info("- teardown() start")
+                        executing_testcase.logger.info(" - teardown() Start execution")
                         executing_testcase.teardown()
-                        executing_testcase.logger.info("- teardown() end")
+                        executing_testcase.logger.info(" - teardown() End execution")
                 except BaseException as e:
                     executing_testcase.logger.error(e)
 
                 try:
                     if hasattr(executing_testcase, "testcase_id"):
                         testcase.testcase_id = executing_testcase.testcase_id
                     elif hasattr(executing_testcase, "test_case_id"):
@@ -2016,29 +2016,26 @@
                 print("generate xml report done...")
         except BaseException:
             traceback.print_exc()
             with open(output_folder + "error_log.txt", "w") as file_obj:
                 file_obj.write(traceback.format_exc())
         finally:
             try:
-                rerun_flag = False
-                if hasattr(settings, "RERUN_FLAG"):
-                    rerun_flag = settings.RERUN_FLAG
-
-                if hasattr(settings, "SAVE_LOG_TO_DB"):
-                    if settings.SAVE_LOG_TO_DB is True:
-                        from . import database_helper
-
-                        database_helper.save_execution_log(passed_testcases=TestCaseExecutor.passed_testcases,
-                                                           failed_testcases=TestCaseExecutor.failed_testcases,
-                                                           output_folder=output_folder,
-                                                           project_name=project_info.project_name,
-                                                           jenkins_job_name=TestCaseExecutor.jenkins_job_name,
-                                                           rerun_flag=rerun_flag
-                                                           )
+                rerun_flag = getattr(settings, "RERUN_FLAG", False)
+
+                if getattr(settings, "SAVE_LOG_TO_DB", False):
+                    from . import database_helper
+
+                    database_helper.save_execution_log(passed_testcases=TestCaseExecutor.passed_testcases,
+                                                       failed_testcases=TestCaseExecutor.failed_testcases,
+                                                       output_folder=output_folder,
+                                                       project_name=project_info.project_name,
+                                                       jenkins_job_name=TestCaseExecutor.jenkins_job_name,
+                                                       rerun_flag=rerun_flag
+                                                       )
             except BaseException:
                 traceback.print_exc()
             finally:
                 try:
                     html_report.Reporter(output_folder,
                                          TestCaseExecutor.passed_testcases,
                                          TestCaseExecutor.failed_testcases,
@@ -2053,32 +2050,32 @@
             print(
                 "=*=*=" * 20 + os.linesep + "Execution has been completed. For further details, please refer to the accompanying HTML report:" + os.linesep + "file:///" + output_folder + os.sep + "report.html")
 
             # save the execution summary into DB (environment, total_execution_time,
             try:
                 import linktest
                 from . import database_helper
-                if hasattr(settings, "SAVE_LOG_TO_DB"):
-                    if settings.SAVE_LOG_TO_DB is True:
-                        end_time = datetime.datetime.now()
-                        execution_time = end_time - begin_time
-
-                        database_helper.insert_execution_summary_log(
-                            execution_id=output_folder.split(os.sep + "output" + os.sep)[1],
-                            environment=settings.ENVIRONMENT,
-                            os=PLATFORM_INFO,
-                            automation_framework_version=linktest.__version__,
-                            total_execution_time=execution_time,
-                            jenkins_job_name=None,
-                            project_name=project_info.project_name,
-                            total_testcases_count=total_testcases_count,
-                            pass_testcases_count=len(TestCaseExecutor.passed_testcases),
-                            fail_testcases_count=total_testcases_count - len(TestCaseExecutor.passed_testcases),
-                            rerun_flag=1 if settings.RERUN_FLAG else 0
-                        )
+
+                if getattr(settings, "SAVE_LOG_TO_DB", False):
+                    end_time = datetime.datetime.now()
+                    execution_time = end_time - begin_time
+
+                    database_helper.insert_execution_summary_log(
+                        execution_id=output_folder.split(os.sep + "output" + os.sep)[1],
+                        environment=settings.ENVIRONMENT,
+                        os=PLATFORM_INFO,
+                        automation_framework_version=linktest.__version__,
+                        total_execution_time=execution_time,
+                        jenkins_job_name=None,
+                        project_name=project_info.project_name,
+                        total_testcases_count=total_testcases_count,
+                        pass_testcases_count=len(TestCaseExecutor.passed_testcases),
+                        fail_testcases_count=total_testcases_count - len(TestCaseExecutor.passed_testcases),
+                        rerun_flag=1 if rerun_flag else 0
+                    )
             except BaseException:
                 traceback.print_exc()
             finally:
                 pass
 
         # 如果最后执行完所有的testcase 并且GlobalDataList 不为空，则自动保存GlobalDataList
         if len(BaseTestCase.GlobalDataList) > 0:
```

### Comparing `linktest-2.7.6/linktest/memory_usage.py` & `linktest-2.7.7/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.6/linktest/re_func.py` & `linktest-2.7.7/linktest/re_func.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.6/linktest/run.py` & `linktest-2.7.7/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.6/linktest/run_testcase_thread.py` & `linktest-2.7.7/linktest/run_testcase_thread.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,24 +25,24 @@
         try:
             # Before executing the setup() method, log TestEngineCaseInput if the action is initiated by the test-engine.
             if BaseTestCase.TestEngineCaseInput:
                 self.executing_testcase.logger.info("------ TestEngineCaseInput:")
                 self.executing_testcase.logger.info(self.executing_testcase.TestEngineCaseInput)
 
             if hasattr(self.executing_testcase, "setup"):
-                self.executing_testcase.logger.info("------ execute setup() Start")
+                self.executing_testcase.logger.info(" - setup() Start execution")
                 self.executing_testcase.setup()
-                self.executing_testcase.logger.info("------ execute setup() End")
+                self.executing_testcase.logger.info(" - setup() End execution")
 
             if hasattr(self.executing_testcase, "runTest"):
                 print("The method runTest() is deprecated. Please rename it to run_test().")
-                self.executing_testcase.logger.info("================== runTest() start:")
+                self.executing_testcase.logger.info(" - runTest() Start execution")
                 self.executing_testcase.runTest()
             else:
-                self.executing_testcase.logger.info("================== run_test() start:")
+                self.executing_testcase.logger.info(" - run_test() Start execution")
                 self.executing_testcase.run_test()
         except BaseException:
             if hasattr(self.executing_testcase, "exception_info"):
                 print("already Timeout, no need to log exception_info again")
             else:
                 traceback.print_exc()
                 self.executing_testcase.exception_info = traceback.format_exc()
```

### Comparing `linktest-2.7.6/linktest/scp_report_to_specified_path.py` & `linktest-2.7.7/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.6/linktest/selenium_helper.py` & `linktest-2.7.7/linktest/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.6/linktest/timeout_thread.py` & `linktest-2.7.7/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.6/linktest/ui_testcase.py` & `linktest-2.7.7/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.6/linktest/update_config.py` & `linktest-2.7.7/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.6/linktest/webdriver_wrapper.py` & `linktest-2.7.7/linktest/webdriver_wrapper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.6/linktest/webdriver_wrapper_chrome.py` & `linktest-2.7.7/linktest/webdriver_wrapper_chrome.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.6/linktest/webdriver_wrapper_edge.py` & `linktest-2.7.7/linktest/webdriver_wrapper_edge.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.6/linktest/webdriver_wrapper_firefox.py` & `linktest-2.7.7/linktest/webdriver_wrapper_firefox.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.6/linktest/webdriver_wrapper_ie.py` & `linktest-2.7.7/linktest/webdriver_wrapper_ie.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.6/linktest/webdriver_wrapper_safari.py` & `linktest-2.7.7/linktest/webdriver_wrapper_safari.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.6/linktest/xml_report.py` & `linktest-2.7.7/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.6/linktest.egg-info/SOURCES.txt` & `linktest-2.7.7/linktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

