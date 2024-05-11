# Comparing `tmp/lukasdata-1.2.8.tar.gz` & `tmp/lukasdata-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lukasdata-1.2.8.tar", last modified: Wed May  8 19:00:55 2024, max compression
+gzip compressed data, was "lukasdata-1.2.9.tar", last modified: Sat May 11 10:20:10 2024, max compression
```

## Comparing `lukasdata-1.2.8.tar` & `lukasdata-1.2.9.tar`

### file list

```diff
@@ -1,34 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 19:00:55.129738 lukasdata-1.2.8/
--rw-rw-rw-   0        0        0      128 2024-05-08 19:00:55.126741 lukasdata-1.2.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-08 19:00:55.096759 lukasdata-1.2.8/lukasdata/
--rw-rw-rw-   0        0        0        0 2024-04-22 22:29:19.000000 lukasdata-1.2.8/lukasdata/__init__.py
--rw-rw-rw-   0        0        0      440 2024-05-04 13:56:10.000000 lukasdata-1.2.8/lukasdata/analyze_datasets.py
--rw-rw-rw-   0        0        0      616 2024-04-22 22:29:19.000000 lukasdata-1.2.8/lukasdata/change_directory.py
--rw-rw-rw-   0        0        0      416 2024-05-03 13:24:44.000000 lukasdata-1.2.8/lukasdata/check_for_all_zeroes.py
--rw-rw-rw-   0        0        0      260 2024-04-29 20:51:11.000000 lukasdata-1.2.8/lukasdata/concat_dfs.py
--rw-rw-rw-   0        0        0      351 2024-04-22 22:29:19.000000 lukasdata-1.2.8/lukasdata/count_nans.py
--rw-rw-rw-   0        0        0      332 2024-04-22 22:29:19.000000 lukasdata-1.2.8/lukasdata/create_mask.py
--rw-rw-rw-   0        0        0      178 2024-04-22 22:29:19.000000 lukasdata-1.2.8/lukasdata/del_jpg.py
--rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.2.8/lukasdata/determine_file_type.py
--rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.2.8/lukasdata/dict_to_json.py
--rw-rw-rw-   0        0        0      387 2024-04-26 08:28:12.000000 lukasdata-1.2.8/lukasdata/drop_column_with_na.py
--rw-rw-rw-   0        0        0      322 2024-05-08 17:36:02.000000 lukasdata-1.2.8/lukasdata/drop_columns_permutation_score.py
--rw-rw-rw-   0        0        0      385 2024-04-26 08:43:39.000000 lukasdata-1.2.8/lukasdata/get_list_intersection.py
--rw-rw-rw-   0        0        0      447 2024-04-22 22:29:19.000000 lukasdata-1.2.8/lukasdata/get_number_columns.py
--rw-rw-rw-   0        0        0      255 2024-04-22 22:29:19.000000 lukasdata-1.2.8/lukasdata/json_to_dict.py
--rw-rw-rw-   0        0        0     1738 2024-05-08 18:59:59.000000 lukasdata-1.2.8/lukasdata/keras_input.py
--rw-rw-rw-   0        0        0      144 2024-04-22 22:29:19.000000 lukasdata-1.2.8/lukasdata/list_to_string.py
--rw-rw-rw-   0        0        0      129 2024-04-26 08:32:10.000000 lukasdata-1.2.8/lukasdata/mean_impute.py
--rw-rw-rw-   0        0        0      160 2024-04-26 08:29:44.000000 lukasdata-1.2.8/lukasdata/na_counts.py
--rw-rw-rw-   0        0        0      132 2024-04-30 10:39:24.000000 lukasdata-1.2.8/lukasdata/order_dict.py
--rw-rw-rw-   0        0        0     2400 2024-05-07 10:05:15.000000 lukasdata-1.2.8/lukasdata/permutation_importance.py
--rw-rw-rw-   0        0        0     1182 2024-04-22 22:29:19.000000 lukasdata-1.2.8/lukasdata/plot_metric_history.py
--rw-rw-rw-   0        0        0      160 2024-04-22 22:29:19.000000 lukasdata-1.2.8/lukasdata/string_to_text.py
-drwxrwxrwx   0        0        0        0 2024-05-08 19:00:55.124741 lukasdata-1.2.8/lukasdata.egg-info/
--rw-rw-rw-   0        0        0      128 2024-05-08 19:00:54.000000 lukasdata-1.2.8/lukasdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      833 2024-05-08 19:00:55.000000 lukasdata-1.2.8/lukasdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 19:00:54.000000 lukasdata-1.2.8/lukasdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-08 19:00:54.000000 lukasdata-1.2.8/lukasdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-08 19:00:54.000000 lukasdata-1.2.8/lukasdata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 19:00:55.130737 lukasdata-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0      192 2024-05-08 19:00:39.000000 lukasdata-1.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 10:20:10.207524 lukasdata-1.2.9/
+-rw-rw-rw-   0        0        0      128 2024-05-11 10:20:10.205526 lukasdata-1.2.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-11 10:20:10.133595 lukasdata-1.2.9/cleaning/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.2.9/cleaning/__init__.py
+-rw-rw-rw-   0        0        0      416 2024-05-03 13:24:44.000000 lukasdata-1.2.9/cleaning/check_for_all_zeroes.py
+-rw-rw-rw-   0        0        0      387 2024-04-26 08:28:12.000000 lukasdata-1.2.9/cleaning/drop_column_with_na.py
+-rw-rw-rw-   0        0        0      129 2024-04-26 08:32:10.000000 lukasdata-1.2.9/cleaning/mean_impute.py
+-rw-rw-rw-   0        0        0      160 2024-04-26 08:29:44.000000 lukasdata-1.2.9/cleaning/na_counts.py
+drwxrwxrwx   0        0        0        0 2024-05-11 10:20:10.149588 lukasdata-1.2.9/datahandler/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.2.9/datahandler/__init__.py
+-rw-rw-rw-   0        0        0      616 2024-04-22 22:29:19.000000 lukasdata-1.2.9/datahandler/change_directory.py
+-rw-rw-rw-   0        0        0      178 2024-04-22 22:29:19.000000 lukasdata-1.2.9/datahandler/del_jpg.py
+-rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.2.9/datahandler/determine_file_type.py
+-rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.2.9/datahandler/dict_to_json.py
+-rw-rw-rw-   0        0        0      255 2024-04-22 22:29:19.000000 lukasdata-1.2.9/datahandler/json_to_dict.py
+-rw-rw-rw-   0        0        0      132 2024-04-30 10:39:24.000000 lukasdata-1.2.9/datahandler/order_dict.py
+-rw-rw-rw-   0        0        0      160 2024-04-22 22:29:19.000000 lukasdata-1.2.9/datahandler/string_to_text.py
+drwxrwxrwx   0        0        0        0 2024-05-11 10:20:10.157583 lukasdata-1.2.9/exploration/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.2.9/exploration/__init__.py
+-rw-rw-rw-   0        0        0      440 2024-05-04 13:56:10.000000 lukasdata-1.2.9/exploration/analyze_datasets.py
+-rw-rw-rw-   0        0        0      351 2024-04-22 22:29:19.000000 lukasdata-1.2.9/exploration/count_nans.py
+-rw-rw-rw-   0        0        0      385 2024-04-26 08:43:39.000000 lukasdata-1.2.9/exploration/get_list_intersection.py
+drwxrwxrwx   0        0        0        0 2024-05-11 10:20:10.203534 lukasdata-1.2.9/lukasdata.egg-info/
+-rw-rw-rw-   0        0        0      128 2024-05-11 10:20:10.000000 lukasdata-1.2.9/lukasdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      972 2024-05-11 10:20:10.000000 lukasdata-1.2.9/lukasdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 10:20:10.000000 lukasdata-1.2.9/lukasdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-11 10:20:10.000000 lukasdata-1.2.9/lukasdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       63 2024-05-11 10:20:10.000000 lukasdata-1.2.9/lukasdata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-11 10:20:10.191534 lukasdata-1.2.9/machine_learning/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.2.9/machine_learning/__init__.py
+-rw-rw-rw-   0        0        0      322 2024-05-08 17:36:02.000000 lukasdata-1.2.9/machine_learning/drop_columns_permutation_score.py
+-rw-rw-rw-   0        0        0     2005 2024-05-11 09:53:36.000000 lukasdata-1.2.9/machine_learning/keras_input.py
+-rw-rw-rw-   0        0        0     1166 2024-05-11 09:53:38.000000 lukasdata-1.2.9/machine_learning/ml_model.py
+-rw-rw-rw-   0        0        0     2400 2024-05-09 08:33:54.000000 lukasdata-1.2.9/machine_learning/permutation_importance.py
+drwxrwxrwx   0        0        0        0 2024-05-11 10:20:10.201528 lukasdata-1.2.9/manipulation/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.2.9/manipulation/__init__.py
+-rw-rw-rw-   0        0        0      260 2024-04-29 20:51:11.000000 lukasdata-1.2.9/manipulation/concat_dfs.py
+-rw-rw-rw-   0        0        0      332 2024-04-22 22:29:19.000000 lukasdata-1.2.9/manipulation/create_mask.py
+-rw-rw-rw-   0        0        0      447 2024-04-22 22:29:19.000000 lukasdata-1.2.9/manipulation/int_columns.py
+-rw-rw-rw-   0        0        0      144 2024-04-22 22:29:19.000000 lukasdata-1.2.9/manipulation/list_to_string.py
+-rw-rw-rw-   0        0        0       42 2024-05-11 10:20:10.207524 lukasdata-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      192 2024-05-11 10:20:03.000000 lukasdata-1.2.9/setup.py
```

### Comparing `lukasdata-1.2.8/lukasdata/change_directory.py` & `lukasdata-1.2.9/datahandler/change_directory.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.2.8/lukasdata/keras_input.py` & `lukasdata-1.2.9/machine_learning/keras_input.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import numpy as np
 import tensorflow as tf
 from sklearn.model_selection import train_test_split
 
 class keras_input():
     def __init__(self,df) -> None:
         self.df=df
-        self.array=np.array(df)
-        self.grouped_df=None
+        self.grouped_df=self.create_grouped("idnr")
+        self.array=None
         self.padded_sequences=None
-        self.y=None
         self.x_train=None
         self.x_test=None
         self.y_train=None
         self.y_test=None
     def create_grouped(self,group):
         self.grouped_df=self.df.groupby(group)
     def drop_column(self,dropped_columns):
@@ -37,14 +36,18 @@
             array_list=array.tolist()
             big_array.append(array_list)
         self.array=big_array
     def padding(self,max_len):
         self.padded_sequences = tf.keras.preprocessing.sequence.pad_sequences(self.array, maxlen=max_len, padding='post', truncating='post') 
     def train_test_split(self):
         self.x_train,self.x_test,self.y_train,self.y_test=train_test_split(self.padded_sequences,self.y,test_size=0.33)
-
-        
+    def init_input(self,group_name="idnr",entry_len=10,y_column_name="subsidized"):
+        self.create_grouped(group_name)
+        self.create_array_from_grouped_df()
+        self.create_y(y_column_name,entry_len)
+        self.padding(entry_len)
+        self.train_test_split()
```

### Comparing `lukasdata-1.2.8/lukasdata/permutation_importance.py` & `lukasdata-1.2.9/machine_learning/permutation_importance.py`

 * *Files identical despite different names*

