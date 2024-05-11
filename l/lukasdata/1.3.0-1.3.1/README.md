# Comparing `tmp/lukasdata-1.3.0.tar.gz` & `tmp/lukasdata-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lukasdata-1.3.0.tar", last modified: Sat May 11 13:23:08 2024, max compression
+gzip compressed data, was "lukasdata-1.3.1.tar", last modified: Sat May 11 13:26:00 2024, max compression
```

## Comparing `lukasdata-1.3.0.tar` & `lukasdata-1.3.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 13:23:08.717030 lukasdata-1.3.0/
--rw-rw-rw-   0        0        0      128 2024-05-11 13:23:08.715032 lukasdata-1.3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-11 13:23:08.519809 lukasdata-1.3.0/cleaning/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.0/cleaning/__init__.py
--rw-rw-rw-   0        0        0      416 2024-05-03 13:24:44.000000 lukasdata-1.3.0/cleaning/check_for_all_zeroes.py
--rw-rw-rw-   0        0        0      387 2024-04-26 08:28:12.000000 lukasdata-1.3.0/cleaning/drop_column_with_na.py
--rw-rw-rw-   0        0        0      129 2024-04-26 08:32:10.000000 lukasdata-1.3.0/cleaning/mean_impute.py
--rw-rw-rw-   0        0        0      160 2024-04-26 08:29:44.000000 lukasdata-1.3.0/cleaning/na_counts.py
-drwxrwxrwx   0        0        0        0 2024-05-11 13:23:08.583634 lukasdata-1.3.0/datahandler/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.0/datahandler/__init__.py
--rw-rw-rw-   0        0        0      616 2024-04-22 22:29:19.000000 lukasdata-1.3.0/datahandler/change_directory.py
--rw-rw-rw-   0        0        0      178 2024-04-22 22:29:19.000000 lukasdata-1.3.0/datahandler/del_jpg.py
--rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.3.0/datahandler/determine_file_type.py
--rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.3.0/datahandler/dict_to_json.py
--rw-rw-rw-   0        0        0      255 2024-04-22 22:29:19.000000 lukasdata-1.3.0/datahandler/json_to_dict.py
--rw-rw-rw-   0        0        0      132 2024-04-30 10:39:24.000000 lukasdata-1.3.0/datahandler/order_dict.py
--rw-rw-rw-   0        0        0      160 2024-04-22 22:29:19.000000 lukasdata-1.3.0/datahandler/string_to_text.py
-drwxrwxrwx   0        0        0        0 2024-05-11 13:23:08.612734 lukasdata-1.3.0/exploration/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.0/exploration/__init__.py
--rw-rw-rw-   0        0        0      440 2024-05-04 13:56:10.000000 lukasdata-1.3.0/exploration/analyze_datasets.py
--rw-rw-rw-   0        0        0      351 2024-04-22 22:29:19.000000 lukasdata-1.3.0/exploration/count_nans.py
--rw-rw-rw-   0        0        0      385 2024-04-26 08:43:39.000000 lukasdata-1.3.0/exploration/get_list_intersection.py
-drwxrwxrwx   0        0        0        0 2024-05-11 13:23:08.714033 lukasdata-1.3.0/lukasdata.egg-info/
--rw-rw-rw-   0        0        0      128 2024-05-11 13:23:08.000000 lukasdata-1.3.0/lukasdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      972 2024-05-11 13:23:08.000000 lukasdata-1.3.0/lukasdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 13:23:08.000000 lukasdata-1.3.0/lukasdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-11 13:23:08.000000 lukasdata-1.3.0/lukasdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       63 2024-05-11 13:23:08.000000 lukasdata-1.3.0/lukasdata.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-11 13:23:08.675724 lukasdata-1.3.0/machine_learning/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.0/machine_learning/__init__.py
--rw-rw-rw-   0        0        0      322 2024-05-08 17:36:02.000000 lukasdata-1.3.0/machine_learning/drop_columns_permutation_score.py
--rw-rw-rw-   0        0        0     2005 2024-05-11 09:53:36.000000 lukasdata-1.3.0/machine_learning/keras_input.py
--rw-rw-rw-   0        0        0     1166 2024-05-11 09:53:38.000000 lukasdata-1.3.0/machine_learning/ml_model.py
--rw-rw-rw-   0        0        0     2400 2024-05-09 08:33:54.000000 lukasdata-1.3.0/machine_learning/permutation_importance.py
-drwxrwxrwx   0        0        0        0 2024-05-11 13:23:08.711035 lukasdata-1.3.0/manipulation/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.0/manipulation/__init__.py
--rw-rw-rw-   0        0        0      260 2024-04-29 20:51:11.000000 lukasdata-1.3.0/manipulation/concat_dfs.py
--rw-rw-rw-   0        0        0      332 2024-04-22 22:29:19.000000 lukasdata-1.3.0/manipulation/create_mask.py
--rw-rw-rw-   0        0        0      447 2024-04-22 22:29:19.000000 lukasdata-1.3.0/manipulation/int_columns.py
--rw-rw-rw-   0        0        0      144 2024-04-22 22:29:19.000000 lukasdata-1.3.0/manipulation/list_to_string.py
--rw-rw-rw-   0        0        0       42 2024-05-11 13:23:08.718029 lukasdata-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0      192 2024-05-11 13:23:00.000000 lukasdata-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 13:26:00.242993 lukasdata-1.3.1/
+-rw-rw-rw-   0        0        0      128 2024-05-11 13:26:00.239949 lukasdata-1.3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-11 13:26:00.165822 lukasdata-1.3.1/cleaning/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.1/cleaning/__init__.py
+-rw-rw-rw-   0        0        0      416 2024-05-03 13:24:44.000000 lukasdata-1.3.1/cleaning/check_for_all_zeroes.py
+-rw-rw-rw-   0        0        0      387 2024-04-26 08:28:12.000000 lukasdata-1.3.1/cleaning/drop_column_with_na.py
+-rw-rw-rw-   0        0        0      129 2024-04-26 08:32:10.000000 lukasdata-1.3.1/cleaning/mean_impute.py
+-rw-rw-rw-   0        0        0      160 2024-04-26 08:29:44.000000 lukasdata-1.3.1/cleaning/na_counts.py
+drwxrwxrwx   0        0        0        0 2024-05-11 13:26:00.184810 lukasdata-1.3.1/datahandler/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.1/datahandler/__init__.py
+-rw-rw-rw-   0        0        0      616 2024-04-22 22:29:19.000000 lukasdata-1.3.1/datahandler/change_directory.py
+-rw-rw-rw-   0        0        0      178 2024-04-22 22:29:19.000000 lukasdata-1.3.1/datahandler/del_jpg.py
+-rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.3.1/datahandler/determine_file_type.py
+-rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.3.1/datahandler/dict_to_json.py
+-rw-rw-rw-   0        0        0      255 2024-04-22 22:29:19.000000 lukasdata-1.3.1/datahandler/json_to_dict.py
+-rw-rw-rw-   0        0        0      132 2024-04-30 10:39:24.000000 lukasdata-1.3.1/datahandler/order_dict.py
+-rw-rw-rw-   0        0        0      160 2024-04-22 22:29:19.000000 lukasdata-1.3.1/datahandler/string_to_text.py
+drwxrwxrwx   0        0        0        0 2024-05-11 13:26:00.194541 lukasdata-1.3.1/exploration/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.1/exploration/__init__.py
+-rw-rw-rw-   0        0        0      440 2024-05-04 13:56:10.000000 lukasdata-1.3.1/exploration/analyze_datasets.py
+-rw-rw-rw-   0        0        0      351 2024-04-22 22:29:19.000000 lukasdata-1.3.1/exploration/count_nans.py
+-rw-rw-rw-   0        0        0      385 2024-04-26 08:43:39.000000 lukasdata-1.3.1/exploration/get_list_intersection.py
+drwxrwxrwx   0        0        0        0 2024-05-11 13:26:00.238951 lukasdata-1.3.1/lukasdata.egg-info/
+-rw-rw-rw-   0        0        0      128 2024-05-11 13:26:00.000000 lukasdata-1.3.1/lukasdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      972 2024-05-11 13:26:00.000000 lukasdata-1.3.1/lukasdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 13:26:00.000000 lukasdata-1.3.1/lukasdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-11 13:26:00.000000 lukasdata-1.3.1/lukasdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       63 2024-05-11 13:26:00.000000 lukasdata-1.3.1/lukasdata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-11 13:26:00.223481 lukasdata-1.3.1/machine_learning/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.1/machine_learning/__init__.py
+-rw-rw-rw-   0        0        0      322 2024-05-08 17:36:02.000000 lukasdata-1.3.1/machine_learning/drop_columns_permutation_score.py
+-rw-rw-rw-   0        0        0     2005 2024-05-11 09:53:36.000000 lukasdata-1.3.1/machine_learning/keras_input.py
+-rw-rw-rw-   0        0        0     1166 2024-05-11 09:53:38.000000 lukasdata-1.3.1/machine_learning/ml_model.py
+-rw-rw-rw-   0        0        0     2400 2024-05-09 08:33:54.000000 lukasdata-1.3.1/machine_learning/permutation_importance.py
+drwxrwxrwx   0        0        0        0 2024-05-11 13:26:00.235794 lukasdata-1.3.1/manipulation/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.1/manipulation/__init__.py
+-rw-rw-rw-   0        0        0      260 2024-04-29 20:51:11.000000 lukasdata-1.3.1/manipulation/concat_dfs.py
+-rw-rw-rw-   0        0        0      332 2024-04-22 22:29:19.000000 lukasdata-1.3.1/manipulation/create_mask.py
+-rw-rw-rw-   0        0        0      447 2024-04-22 22:29:19.000000 lukasdata-1.3.1/manipulation/int_columns.py
+-rw-rw-rw-   0        0        0      144 2024-04-22 22:29:19.000000 lukasdata-1.3.1/manipulation/list_to_string.py
+-rw-rw-rw-   0        0        0       42 2024-05-11 13:26:00.243993 lukasdata-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      192 2024-05-11 13:25:53.000000 lukasdata-1.3.1/setup.py
```

### Comparing `lukasdata-1.3.0/datahandler/change_directory.py` & `lukasdata-1.3.1/datahandler/change_directory.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.0/lukasdata.egg-info/SOURCES.txt` & `lukasdata-1.3.1/lukasdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.0/machine_learning/keras_input.py` & `lukasdata-1.3.1/machine_learning/keras_input.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.0/machine_learning/ml_model.py` & `lukasdata-1.3.1/machine_learning/ml_model.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.0/machine_learning/permutation_importance.py` & `lukasdata-1.3.1/machine_learning/permutation_importance.py`

 * *Files identical despite different names*

