# Comparing `tmp/ReadyCellOne-0.1.3.tar.gz` & `tmp/readycellone-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReadyCellOne-0.1.3.tar", last modified: Mon Feb 19 19:44:40 2024, max compression
+gzip compressed data, was "readycellone-0.1.4.tar", last modified: Sat May 11 00:05:54 2024, max compression
```

## Comparing `ReadyCellOne-0.1.3.tar` & `readycellone-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-02-19 19:44:40.259682 ReadyCellOne-0.1.3/
--rw-r--r--   0 alex       (501) staff       (20)      396 2024-02-19 19:44:40.259450 ReadyCellOne-0.1.3/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)       75 2023-09-21 15:55:12.000000 ReadyCellOne-0.1.3/README.md
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-02-19 19:44:40.258229 ReadyCellOne-0.1.3/ReadyCellOne/
--rw-r--r--   0 alex       (501) staff       (20)     8631 2024-02-17 20:25:31.000000 ReadyCellOne-0.1.3/ReadyCellOne/core.py
--rw-r--r--   0 alex       (501) staff       (20)       60 2024-02-17 20:25:31.000000 ReadyCellOne-0.1.3/ReadyCellOne/init.py
--rw-r--r--   0 alex       (501) staff       (20)     9164 2024-02-17 20:25:31.000000 ReadyCellOne-0.1.3/ReadyCellOne/plot.py
--rw-r--r--   0 alex       (501) staff       (20)     3566 2024-02-19 19:43:49.000000 ReadyCellOne-0.1.3/ReadyCellOne/utils.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-02-19 19:44:40.259161 ReadyCellOne-0.1.3/ReadyCellOne.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)      396 2024-02-19 19:44:40.000000 ReadyCellOne-0.1.3/ReadyCellOne.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      317 2024-02-19 19:44:40.000000 ReadyCellOne-0.1.3/ReadyCellOne.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2024-02-19 19:44:40.000000 ReadyCellOne-0.1.3/ReadyCellOne.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2024-02-19 19:20:12.000000 ReadyCellOne-0.1.3/ReadyCellOne.egg-info/not-zip-safe
--rw-r--r--   0 alex       (501) staff       (20)       56 2024-02-19 19:44:40.000000 ReadyCellOne-0.1.3/ReadyCellOne.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)       13 2024-02-19 19:44:40.000000 ReadyCellOne-0.1.3/ReadyCellOne.egg-info/top_level.txt
--rw-r--r--   0 alex       (501) staff       (20)       38 2024-02-19 19:44:40.259719 ReadyCellOne-0.1.3/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)      533 2024-02-19 19:44:33.000000 ReadyCellOne-0.1.3/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-11 00:05:54.056124 readycellone-0.1.4/
+-rw-r--r--   0 alex       (501) staff       (20)      396 2024-05-11 00:05:54.055894 readycellone-0.1.4/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     2378 2024-05-10 22:08:05.000000 readycellone-0.1.4/README.md
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-11 00:05:54.054091 readycellone-0.1.4/ReadyCellOne/
+-rw-r--r--   0 alex       (501) staff       (20)     9170 2024-05-10 23:50:28.000000 readycellone-0.1.4/ReadyCellOne/core.py
+-rw-r--r--   0 alex       (501) staff       (20)       60 2024-02-17 20:25:31.000000 readycellone-0.1.4/ReadyCellOne/init.py
+-rw-r--r--   0 alex       (501) staff       (20)     9164 2024-02-17 20:25:31.000000 readycellone-0.1.4/ReadyCellOne/plot.py
+-rw-r--r--   0 alex       (501) staff       (20)     3566 2024-02-19 19:43:49.000000 readycellone-0.1.4/ReadyCellOne/utils.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-11 00:05:54.055613 readycellone-0.1.4/ReadyCellOne.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)      396 2024-05-11 00:05:54.000000 readycellone-0.1.4/ReadyCellOne.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      317 2024-05-11 00:05:54.000000 readycellone-0.1.4/ReadyCellOne.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2024-05-11 00:05:54.000000 readycellone-0.1.4/ReadyCellOne.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2024-02-19 19:20:12.000000 readycellone-0.1.4/ReadyCellOne.egg-info/not-zip-safe
+-rw-r--r--   0 alex       (501) staff       (20)       56 2024-05-11 00:05:54.000000 readycellone-0.1.4/ReadyCellOne.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)       13 2024-05-11 00:05:54.000000 readycellone-0.1.4/ReadyCellOne.egg-info/top_level.txt
+-rw-r--r--   0 alex       (501) staff       (20)       38 2024-05-11 00:05:54.056172 readycellone-0.1.4/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)      533 2024-05-11 00:05:10.000000 readycellone-0.1.4/setup.py
```

### Comparing `ReadyCellOne-0.1.3/ReadyCellOne/core.py` & `readycellone-0.1.4/ReadyCellOne/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,115 +5,113 @@
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.multiclass import OneVsRestClassifier
 from sklearn.preprocessing import label_binarize
 
 from ReadyCellOne.utils import *
 
 # Core functions
-def train_rco_model(train_adata, train_cell_state_obs_column, test_adata, expression_program, species='human',
+def train_rco_model(train_adata, train_cell_state_obs_column, test_adata, test_cell_state_obs_column, expression_program, species='human',
                     n_trees=1000, max_depth=3, random_state=100, class_weight='balanced',
-                    num_random_samples=0, train_order=None, test_cell_state_obs_column=None, test_order=None):
+                    num_random_samples=0, train_order=None, test_order=None):
   '''
 
   High level function to train a ReadyCellOne model.
 
   @param train_adata: AnnData, training matrix, expects scRNA-seq.
+  @param train_cell_state_obs_column: str, name of the observation column in train_adata for cell state annotations.
+         This is the target variable for classification.
   @param test_adata: AnnData, testing matrix, can be bulk or single-cell.
-  @param cell_state_obs_column: str, name of the observation column in train_adata for cell state annotations. 
-          This is the target variable for classification.
-  @param expression_program: str or list, if str, name of GOBP, BioCarta, KEGG, or Reactome functional gene set from MSigDB. 
+  @param test_cell_state_obs_column: str, name of observation column in test_adata for cell state annotations.
+  @param expression_program: str or list, if str, name of GOBP, BioCarta, KEGG, or Reactome functional gene set from MSigDB.
           If list, custom gene set. The model features will be restricted to these genes during training.
   @param species: 'human' or 'mouse'
   @param n_trees (default:1000): number of estimators in random forest classifier.
   @param max_depth (default:3): max depth for each decision tree in the random forest.
   @param random_state (default:100): seed for the random state.
   @param class_weight (default:'balanced'): whether or not to balance the classes.
-  @param num_random_samples (optional; default: 0): This is to add a negative control class in the training process. 
+  @param num_random_samples (optional; default: 0): This is to add a negative control class in the training process.
           The idea is that any query samples that are dissimilar to the cell states trained on will be predicted as a random expression profile.
-  @param order (optional): 
+  @param train_order (optional): specify ordering of each target class (cell state) in training labels for downstream visualization.
+  @param test_order (optional): specify ordering of each target class (cell state) in test labels for downstream visualization.
 
   @return
           clf: trained classifier
-          train_ranked_expression_reduced: the
-          test_ranked_expression_reduced:
-          y_train
-          cgenes
+          train_ranked_expression_reduced: pd.DataFrame, the rank-transformed training data, reduced to input gene list
+          test_ranked_expression_reduced: pd.DataFrame, the rank-transformed test data, reduced to input gene list
+          y_train: sklearn label-binarized train labels in the order specified by param train_order.
+          y_test: sklearn label-binarized test labels in the order specified by param test_order.
+          cgenes: intersection set of genes between training data and test data
 
   '''
 
   train_adata_common, test_adata_common, cgenes = restrict_to_cgenes(train_adata, test_adata)
 
   train_df = train_adata_common.to_df()
   test_df = test_adata_common.to_df()
 
   train_cell_state_obs = train_adata.obs[train_cell_state_obs_column]
+  test_cell_state_obs = test_adata.obs[test_cell_state_obs_column]
 
-  y_train = None
-  y_test = None
+  y_train = train_cell_state_obs
+  y_test = test_cell_state_obs
 
   train_ranked_expression = pd.DataFrame()
 
   # Rank-based feature transformation
   if num_random_samples > 0:
     train_cell_state_obs = np.concatenate([train_cell_state_obs, np.array(['random'] * num_random_samples)])
-    train_ranked_expression = transcriptome_rank_transform(train_df)
 
-  else:
-    train_ranked_expression = transcriptome_rank_transform(train_df, add_random_samples=False)
+  train_ranked_expression = transcriptome_rank_transform(train_df, num_random_samples=num_random_samples)
 
   train_unique_cell_states = np.unique(train_cell_state_obs)
 
   # Processing of target variable
   if train_order:
     sorted_indices = np.argsort([train_order.index(x) for x in train_unique_cell_states])
     train_unique_cell_states = train_unique_cell_states[sorted_indices]
 
   y_train = label_binarize(train_cell_state_obs, classes=train_unique_cell_states)
 
-  if test_cell_state_obs_column:
-    test_cell_state_obs = test_adata.obs[test_cell_state_obs_column]
+  if test_order:
     test_unique_cell_states = np.unique(test_cell_state_obs)
+    if 'random' in train_unique_cell_states:
+      test_unique_cell_states = np.concatenate([test_unique_cell_states, np.array(['random'])])
+
+    sorted_indices = np.argsort([test_order.index(x) for x in test_unique_cell_states])
+    test_unique_cell_states = test_unique_cell_states[sorted_indices]
 
-    if test_order:
-      if 'random' in train_unique_cell_states:
-        test_unique_cell_states = np.concatenate([test_unique_cell_states, np.array(['random'])])
-
-      sorted_indices = np.argsort([test_order.index(x) for x in test_unique_cell_states])
-      test_unique_cell_states = test_unique_cell_states[sorted_indices]
-
-    if num_random_samples > 0:
-      y_test = label_binarize(test_cell_state_obs, classes=test_unique_cell_states)
-    else:
-      y_test = label_binarize(test_cell_state_obs, classes=test_unique_cell_states)
+  if num_random_samples > 0:
+    y_test = np.concatenate([test_cell_state_obs, np.array(['random'] * num_random_samples)])
 
   # Gene annotation based feature selection
   gene_set = []
 
   if isinstance(expression_program, list):
     gene_set = expression_program
   else:
     gene_set = get_expression_program(expression_program, species=species)
 
   train_ranked_expression_reduced = select_expression_program_genes(train_ranked_expression, gene_set)
 
+  print('train', train_ranked_expression_reduced.shape)
+
   # Process test dataset
-  test_ranked_expression = transcriptome_rank_transform(test_df, add_random_samples=False)
+  test_ranked_expression = transcriptome_rank_transform(test_df, num_random_samples)
   test_ranked_expression_reduced = select_expression_program_genes(test_ranked_expression, gene_set)
 
+  print('test', test_ranked_expression_reduced.shape)
+
   # Train the RCO model
   clf = make_classifier(n_trees=n_trees, max_depth=max_depth, random_state=random_state, class_weight=class_weight)
 
   print('training...')
 
   clf.fit(train_ranked_expression_reduced, y_train)
 
-  if test_cell_state_obs_column:
-    return clf, train_ranked_expression_reduced, test_ranked_expression_reduced, y_train, y_test, cgenes
-
-  return clf, train_ranked_expression_reduced, test_ranked_expression_reduced, y_train, cgenes
+  return clf, train_ranked_expression_reduced, test_ranked_expression_reduced, y_train, y_test, cgenes
 
 
 def restrict_to_cgenes(train_adata, test_adata):
   '''
   Computes the common set of genes for RF classification
 
   '''
```

### Comparing `ReadyCellOne-0.1.3/ReadyCellOne/plot.py` & `readycellone-0.1.4/ReadyCellOne/plot.py`

 * *Files identical despite different names*

### Comparing `ReadyCellOne-0.1.3/ReadyCellOne/utils.py` & `readycellone-0.1.4/ReadyCellOne/utils.py`

 * *Files identical despite different names*

### Comparing `ReadyCellOne-0.1.3/setup.py` & `readycellone-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='ReadyCellOne',
-      version='0.1.3',
+      version='0.1.4',
       description='Computational tools to enable task-centric cell engineering',
       url='http://github.com/CahanLab/ReadyCellOne/',
       author='Patrick Cahan',
       author_email='patrick.cahan@gmail.com',
       license='MIT',
       packages=['ReadyCellOne'],
       install_requires=[
```

