# Comparing `tmp/mlpr-0.1.4.tar.gz` & `tmp/mlpr-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpr-0.1.4.tar", max compression
+gzip compressed data, was "mlpr-0.1.5.tar", max compression
```

## Comparing `mlpr-0.1.4.tar` & `mlpr-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      289 2024-05-11 02:18:39.159292 mlpr-0.1.4/CHANGELOG.md
--rw-r--r--   0        0        0     1063 2024-04-27 16:49:57.314542 mlpr-0.1.4/LICENSE
--rw-r--r--   0        0        0    30288 2024-05-11 03:38:08.390692 mlpr-0.1.4/README.md
--rw-r--r--   0        0        0      256 2024-05-11 02:24:23.791737 mlpr-0.1.4/SECURITY.md
--rw-r--r--   0        0        0     2502 2024-05-11 03:43:13.660048 mlpr-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       70 2024-05-11 03:43:17.023960 mlpr-0.1.4/src/mlpr/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 16:52:49.073225 mlpr-0.1.4/src/mlpr/ml/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 18:27:54.717513 mlpr-0.1.4/src/mlpr/ml/supervisioned/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 18:28:38.701333 mlpr-0.1.4/src/mlpr/ml/supervisioned/classification/__init__.py
--rw-r--r--   0        0        0     5103 2024-05-11 02:06:39.037536 mlpr-0.1.4/src/mlpr/ml/supervisioned/classification/uncertainty.py
--rw-r--r--   0        0        0     2242 2024-05-11 01:58:21.065745 mlpr-0.1.4/src/mlpr/ml/supervisioned/classification/utils.py
--rw-r--r--   0        0        0        0 2024-04-27 18:28:52.537279 mlpr-0.1.4/src/mlpr/ml/supervisioned/forecasting/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 23:35:52.450714 mlpr-0.1.4/src/mlpr/ml/supervisioned/regression/__init__.py
--rw-r--r--   0        0        0    18436 2024-05-05 00:35:48.981115 mlpr-0.1.4/src/mlpr/ml/supervisioned/regression/metrics.py
--rw-r--r--   0        0        0    18464 2024-05-05 00:20:45.686332 mlpr-0.1.4/src/mlpr/ml/supervisioned/regression/plots.py
--rw-r--r--   0        0        0        0 2024-04-27 16:52:49.073225 mlpr-0.1.4/src/mlpr/ml/supervisioned/tunning/__init__.py
--rw-r--r--   0        0        0     6314 2024-05-10 23:01:04.220209 mlpr-0.1.4/src/mlpr/ml/supervisioned/tunning/grid_search.py
--rw-r--r--   0        0        0       62 2024-04-27 21:43:09.387068 mlpr-0.1.4/src/mlpr/reports/__init__.py
--rw-r--r--   0        0        0     1742 2024-05-04 23:35:34.703861 mlpr-0.1.4/src/mlpr/reports/create.py
--rw-r--r--   0        0        0    32249 1970-01-01 00:00:00.000000 mlpr-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      289 2024-05-11 02:18:39.159292 mlpr-0.1.5/CHANGELOG.md
+-rw-r--r--   0        0        0     1063 2024-04-27 16:49:57.314542 mlpr-0.1.5/LICENSE
+-rw-r--r--   0        0        0    30231 2024-05-11 03:50:25.744186 mlpr-0.1.5/README.md
+-rw-r--r--   0        0        0      256 2024-05-11 02:24:23.791737 mlpr-0.1.5/SECURITY.md
+-rw-r--r--   0        0        0     2502 2024-05-11 03:50:45.279950 mlpr-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       70 2024-05-11 03:50:41.867990 mlpr-0.1.5/src/mlpr/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 16:52:49.073225 mlpr-0.1.5/src/mlpr/ml/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 18:27:54.717513 mlpr-0.1.5/src/mlpr/ml/supervisioned/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 18:28:38.701333 mlpr-0.1.5/src/mlpr/ml/supervisioned/classification/__init__.py
+-rw-r--r--   0        0        0     5103 2024-05-11 02:06:39.037536 mlpr-0.1.5/src/mlpr/ml/supervisioned/classification/uncertainty.py
+-rw-r--r--   0        0        0     2242 2024-05-11 01:58:21.065745 mlpr-0.1.5/src/mlpr/ml/supervisioned/classification/utils.py
+-rw-r--r--   0        0        0        0 2024-04-27 18:28:52.537279 mlpr-0.1.5/src/mlpr/ml/supervisioned/forecasting/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 23:35:52.450714 mlpr-0.1.5/src/mlpr/ml/supervisioned/regression/__init__.py
+-rw-r--r--   0        0        0    18436 2024-05-05 00:35:48.981115 mlpr-0.1.5/src/mlpr/ml/supervisioned/regression/metrics.py
+-rw-r--r--   0        0        0    18464 2024-05-05 00:20:45.686332 mlpr-0.1.5/src/mlpr/ml/supervisioned/regression/plots.py
+-rw-r--r--   0        0        0        0 2024-04-27 16:52:49.073225 mlpr-0.1.5/src/mlpr/ml/supervisioned/tunning/__init__.py
+-rw-r--r--   0        0        0     6314 2024-05-10 23:01:04.220209 mlpr-0.1.5/src/mlpr/ml/supervisioned/tunning/grid_search.py
+-rw-r--r--   0        0        0       62 2024-04-27 21:43:09.387068 mlpr-0.1.5/src/mlpr/reports/__init__.py
+-rw-r--r--   0        0        0     1742 2024-05-04 23:35:34.703861 mlpr-0.1.5/src/mlpr/reports/create.py
+-rw-r--r--   0        0        0    32192 1970-01-01 00:00:00.000000 mlpr-0.1.5/PKG-INFO
```

### Comparing `mlpr-0.1.4/LICENSE` & `mlpr-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.4/README.md` & `mlpr-0.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -100,17 +100,15 @@
 from sklearn.neighbors import KNeighborsClassifier
 from sklearn.svm import SVC
 from sklearn.tree import DecisionTreeClassifier
 
 from sklearn.datasets import make_blobs
 from sklearn.metrics import accuracy_score, precision_score, recall_score, f1_score, cohen_kappa_score
 
-
-from src.mlpr.ml.supervisioned.tunning.grid_search import GridSearch
-from utils.reader import read_file_yaml
+from mlpr.ml.supervisioned.tunning.grid_search import GridSearch
 ```
 
 ## Methods
 
 Here we have a custom method for accuracy to use in model selection. Thus:
 
 ```python
@@ -362,17 +360,17 @@
 from sklearn.linear_model import LogisticRegression
 from sklearn.metrics import (accuracy_score, cohen_kappa_score, f1_score,
                              precision_score, recall_score)
 from sklearn.naive_bayes import GaussianNB
 from sklearn.svm import SVC
 from sklearn.tree import DecisionTreeClassifier
 
-from src.mlpr.ml.supervisioned.classification.uncertainty import UncertaintyPlots
-from src.mlpr.ml.supervisioned.classification.utils import calculate_probas
-from src.mlpr.ml.supervisioned.tunning.grid_search import GridSearch
+from mlpr.ml.supervisioned.classification.uncertainty import UncertaintyPlots
+from mlpr.ml.supervisioned.classification.utils import calculate_probas
+from mlpr.ml.supervisioned.tunning.grid_search import GridSearch
 
 import warnings
 warnings.filterwarnings("ignore")
 ```
 
 ## Parameters
 Setting parameters for the experiments.
```

#### html2text {}

```diff
@@ -27,33 +27,32 @@
 matplotlib.pyplot as plt from sklearn.base import BaseEstimator from
 sklearn.ensemble import RandomForestClassifier, GradientBoostingClassifier from
 sklearn.linear_model import LogisticRegression from sklearn.naive_bayes import
 GaussianNB from sklearn.neighbors import KNeighborsClassifier from sklearn.svm
 import SVC from sklearn.tree import DecisionTreeClassifier from
 sklearn.datasets import make_blobs from sklearn.metrics import accuracy_score,
 precision_score, recall_score, f1_score, cohen_kappa_score from
-src.mlpr.ml.supervisioned.tunning.grid_search import GridSearch from
-utils.reader import read_file_yaml ``` ## Methods Here we have a custom method
-for accuracy to use in model selection. Thus: ```python def
-custom_accuracy_score(y_true: np.ndarray, y_pred: np.ndarray) -> float: return
-accuracy_score(y_true, y_pred, normalize=False) ``` ## Loading the Data Load
-your dataset. In this example, we're generating a dataset for classification
-using sklearn: ```python n_samples = 1000 centers = [(0, 0), (3, 4.5)]
-n_features = 2 cluster_std = 1.3 random_state = 42 ``` ```python np.random.seed
-(random_state) ``` ```python X, y = make_blobs( n_samples=n_samples,
-centers=centers, n_features=n_features, cluster_std=cluster_std,
-random_state=random_state ) ``` ## Plot the dataset ```python fig, ax =
-plt.subplots(1, 1, figsize=(14, 6)) ax.plot(X[:, 0][y == 0], X[:, 1][y == 0],
-"bs") ax.plot(X[:, 0][y == 1], X[:, 1][y == 1], "g^") ax.set_title("Dataset")
-ax.set_frame_on(False) ax.set_xticks([]) ax.set_yticks([]) fig.tight_layout()
-``` [![fig0](https://raw.githack.com/Manuelfjr/mlpr/develop/assets/
-tunning_scatter.png)](https://raw.githack.com/Manuelfjr/mlpr/develop/assets/
-tunning_scatter.png) ## Cross-validtion ```python models: Dict[BaseEstimator,
-Dict] = { RandomForestClassifier: { 'n_estimators': [10, 50, 100, 200],
-'max_depth': [None, 5, 10, 15], 'min_samples_split': [2, 5, 10],
+mlpr.ml.supervisioned.tunning.grid_search import GridSearch ``` ## Methods Here
+we have a custom method for accuracy to use in model selection. Thus: ```python
+def custom_accuracy_score(y_true: np.ndarray, y_pred: np.ndarray) -> float:
+return accuracy_score(y_true, y_pred, normalize=False) ``` ## Loading the Data
+Load your dataset. In this example, we're generating a dataset for
+classification using sklearn: ```python n_samples = 1000 centers = [(0, 0), (3,
+4.5)] n_features = 2 cluster_std = 1.3 random_state = 42 ``` ```python
+np.random.seed(random_state) ``` ```python X, y = make_blobs
+( n_samples=n_samples, centers=centers, n_features=n_features,
+cluster_std=cluster_std, random_state=random_state ) ``` ## Plot the dataset
+```python fig, ax = plt.subplots(1, 1, figsize=(14, 6)) ax.plot(X[:, 0][y ==
+0], X[:, 1][y == 0], "bs") ax.plot(X[:, 0][y == 1], X[:, 1][y == 1], "g^")
+ax.set_title("Dataset") ax.set_frame_on(False) ax.set_xticks([]) ax.set_yticks(
+[]) fig.tight_layout() ``` [![fig0](https://raw.githack.com/Manuelfjr/mlpr/
+develop/assets/tunning_scatter.png)](https://raw.githack.com/Manuelfjr/mlpr/
+develop/assets/tunning_scatter.png) ## Cross-validtion ```python models: Dict
+[BaseEstimator, Dict] = { RandomForestClassifier: { 'n_estimators': [10, 50,
+100, 200], 'max_depth': [None, 5, 10, 15], 'min_samples_split': [2, 5, 10],
 'min_samples_leaf': [1, 2, 4], 'random_state': [random_state] },
 GradientBoostingClassifier: { 'n_estimators': [50, 100, 200], 'learning_rate':
 [0.1, 0.05, 0.01, 0.005], 'subsample': [0.5, 0.8, 1.0], 'random_state':
 [random_state] }, LogisticRegression: { 'C': [0.01, 0.1, 1.0, 10.0], 'penalty':
 ['l1', 'l2'], 'solver': ['liblinear', 'saga'], 'random_state': [random_state]
 }, GaussianNB: { 'var_smoothing': [1e-9, 1e-8, 1e-7, 1e-6, 1e-5] },
 KNeighborsClassifier: { 'n_neighbors': [3, 5, 7, 9], 'weights': ['uniform',
@@ -96,63 +95,63 @@
 matplotlib.pyplot as plt import numpy as np import pandas as pd from
 sklearn.base import BaseEstimator from sklearn.datasets import make_blobs from
 sklearn.ensemble import GradientBoostingClassifier, RandomForestClassifier from
 sklearn.linear_model import LogisticRegression from sklearn.metrics import
 (accuracy_score, cohen_kappa_score, f1_score, precision_score, recall_score)
 from sklearn.naive_bayes import GaussianNB from sklearn.svm import SVC from
 sklearn.tree import DecisionTreeClassifier from
-src.mlpr.ml.supervisioned.classification.uncertainty import UncertaintyPlots
-from src.mlpr.ml.supervisioned.classification.utils import calculate_probas
-from src.mlpr.ml.supervisioned.tunning.grid_search import GridSearch import
-warnings warnings.filterwarnings("ignore") ``` ## Parameters Setting parameters
-for the experiments. ```python random_state: int = 42 n_feats: int = 2 n_size:
-int = 1000 centers: list[tuple] = [ (0, 2), (2, 0), (5, 4.5) ] n_class: int =
-len(centers) cluster_std: list[float] = [1.4, 1.4, 0.8] cv: int = 5
-np.random.seed(random_state) ``` ```python params: dict[str, dict[str, any]] =
-{ "n_samples": n_size, "n_features": n_feats, "centers": centers,
-"cluster_std": cluster_std, "random_state": random_state } ``` ```python
-np.random.seed(random_state) ``` ```python params_split: dict[str, float | int]
-= { 'test_size': 0.25, 'random_state': random_state } params_norm: dict[str,
-bool] = {'with_mean': True, 'with_std': True} model_metrics: dict[str, any] =
-{ 'custom_accuracy': partial(accuracy_score, normalize=False), 'accuracy':
-accuracy_score, 'precision': partial(precision_score, average='macro'),
-'recall': partial(recall_score, average='macro'), 'kappa': cohen_kappa_score,
-'f1': partial(f1_score, average='macro'), } ``` ## Load the dataset Here we are
-generating a dataset for experiments, using blobs from scikit-learn. ```python
-X, y = make_blobs( **params ) ``` ## Plot the dataset Behavior of the dataset
-used in the experiment. ```python markers = ['o', 'v', '^'] fig, ax =
-plt.subplots(1, 1, figsize=(14, 6)) colors = generate_colors("FF4B3E",
-"1C2127", len(np.unique(y))) for i, k in enumerate(np.unique(y)): ax.scatter(X
-[:, 0][y == k], X[:, 1][y == k], marker=markers[i % len(markers)], color=colors
-[i], label=f"c{i}") ax.set_title("Dataset") ax.set_frame_on(False)
-ax.set_xticks([]) ax.set_yticks([]) for center, color in zip(centers, colors):
-ax.scatter( center[0], center[1], color="white", linewidths=3, marker="o",
-edgecolor="black", s=120 ) plt.legend() fig.tight_layout() ``` [![fig1](https:/
-/raw.githack.com/Manuelfjr/mlpr/develop/assets/classification_scatter.png)]
-(https://raw.githack.com/Manuelfjr/mlpr/develop/assets/
-classification_scatter.png) ## Cross-validation ```python models: Dict
-[BaseEstimator, Dict] = { RandomForestClassifier: { 'n_estimators': [10, 50,
-100, 200], 'max_depth': [None, 5, 10, 15], 'min_samples_split': [2, 5, 10],
-'min_samples_leaf': [1, 2, 4], 'random_state': [random_state] },
-GradientBoostingClassifier: { 'n_estimators': [50, 100, 200], 'learning_rate':
-[0.1, 0.05, 0.01, 0.005], 'subsample': [0.5, 0.8, 1.0], 'random_state':
-[random_state] }, LogisticRegression: { 'C': [0.01, 0.1, 1.0, 10.0], 'penalty':
-['l1', 'l2'], 'solver': ['liblinear', 'saga'], 'random_state': [random_state],
-'max_iter': [10000] }, GaussianNB: { 'var_smoothing': [1e-9, 1e-8, 1e-7, 1e-6,
-1e-5] }, SVC: { 'C': [0.01, 0.1, 1.0, 10.0], 'kernel': ['linear', 'poly',
-'rbf', 'sigmoid'], 'degree': [2, 3, 4], 'gamma': ['scale', 'auto'],
-'probability': [True], 'random_state': [random_state] },
-DecisionTreeClassifier: { 'criterion': ['gini', 'entropy'], 'splitter':
-['best', 'random'], 'max_depth': [None, 5, 10, 15], 'min_samples_split': [2, 5,
-10], 'min_samples_leaf': [1, 2, 4], 'random_state': [random_state] } } ```
-```python grid_search = GridSearch( X, y, params_split=params_split,
-models_params=models, normalize=True, params_norm=params_norm,
-scoring='accuracy', metrics=model_metrics ) grid_search.search(cv=cv, n_jobs=-
-1) best_model, best_params = \ grid_search \ .get_best_model() ``` ```python
-results: pd.DataFrame = pd.DataFrame(grid_search._metrics).T results ```
+mlpr.ml.supervisioned.classification.uncertainty import UncertaintyPlots from
+mlpr.ml.supervisioned.classification.utils import calculate_probas from
+mlpr.ml.supervisioned.tunning.grid_search import GridSearch import warnings
+warnings.filterwarnings("ignore") ``` ## Parameters Setting parameters for the
+experiments. ```python random_state: int = 42 n_feats: int = 2 n_size: int =
+1000 centers: list[tuple] = [ (0, 2), (2, 0), (5, 4.5) ] n_class: int = len
+(centers) cluster_std: list[float] = [1.4, 1.4, 0.8] cv: int = 5 np.random.seed
+(random_state) ``` ```python params: dict[str, dict[str, any]] = { "n_samples":
+n_size, "n_features": n_feats, "centers": centers, "cluster_std": cluster_std,
+"random_state": random_state } ``` ```python np.random.seed(random_state) ```
+```python params_split: dict[str, float | int] = { 'test_size': 0.25,
+'random_state': random_state } params_norm: dict[str, bool] = {'with_mean':
+True, 'with_std': True} model_metrics: dict[str, any] = { 'custom_accuracy':
+partial(accuracy_score, normalize=False), 'accuracy': accuracy_score,
+'precision': partial(precision_score, average='macro'), 'recall': partial
+(recall_score, average='macro'), 'kappa': cohen_kappa_score, 'f1': partial
+(f1_score, average='macro'), } ``` ## Load the dataset Here we are generating a
+dataset for experiments, using blobs from scikit-learn. ```python X, y =
+make_blobs( **params ) ``` ## Plot the dataset Behavior of the dataset used in
+the experiment. ```python markers = ['o', 'v', '^'] fig, ax = plt.subplots(1,
+1, figsize=(14, 6)) colors = generate_colors("FF4B3E", "1C2127", len(np.unique
+(y))) for i, k in enumerate(np.unique(y)): ax.scatter(X[:, 0][y == k], X[:, 1]
+[y == k], marker=markers[i % len(markers)], color=colors[i], label=f"c{i}")
+ax.set_title("Dataset") ax.set_frame_on(False) ax.set_xticks([]) ax.set_yticks(
+[]) for center, color in zip(centers, colors): ax.scatter( center[0], center
+[1], color="white", linewidths=3, marker="o", edgecolor="black", s=120 )
+plt.legend() fig.tight_layout() ``` [![fig1](https://raw.githack.com/Manuelfjr/
+mlpr/develop/assets/classification_scatter.png)](https://raw.githack.com/
+Manuelfjr/mlpr/develop/assets/classification_scatter.png) ## Cross-validation
+```python models: Dict[BaseEstimator, Dict] = { RandomForestClassifier:
+{ 'n_estimators': [10, 50, 100, 200], 'max_depth': [None, 5, 10, 15],
+'min_samples_split': [2, 5, 10], 'min_samples_leaf': [1, 2, 4], 'random_state':
+[random_state] }, GradientBoostingClassifier: { 'n_estimators': [50, 100, 200],
+'learning_rate': [0.1, 0.05, 0.01, 0.005], 'subsample': [0.5, 0.8, 1.0],
+'random_state': [random_state] }, LogisticRegression: { 'C': [0.01, 0.1, 1.0,
+10.0], 'penalty': ['l1', 'l2'], 'solver': ['liblinear', 'saga'],
+'random_state': [random_state], 'max_iter': [10000] }, GaussianNB:
+{ 'var_smoothing': [1e-9, 1e-8, 1e-7, 1e-6, 1e-5] }, SVC: { 'C': [0.01, 0.1,
+1.0, 10.0], 'kernel': ['linear', 'poly', 'rbf', 'sigmoid'], 'degree': [2, 3,
+4], 'gamma': ['scale', 'auto'], 'probability': [True], 'random_state':
+[random_state] }, DecisionTreeClassifier: { 'criterion': ['gini', 'entropy'],
+'splitter': ['best', 'random'], 'max_depth': [None, 5, 10, 15],
+'min_samples_split': [2, 5, 10], 'min_samples_leaf': [1, 2, 4], 'random_state':
+[random_state] } } ``` ```python grid_search = GridSearch( X, y,
+params_split=params_split, models_params=models, normalize=True,
+params_norm=params_norm, scoring='accuracy', metrics=model_metrics )
+grid_search.search(cv=cv, n_jobs=-1) best_model, best_params = \ grid_search \
+.get_best_model() ``` ```python results: pd.DataFrame = pd.DataFrame
+(grid_search._metrics).T results ```
                            ccuussttoomm__aaccccuurraaccyy aaccccuurraaccyy pprreecciissiioonn rreeccaallll   kkaappppaa    ff11
 RandomForestClassifier     222.0           0.888    0.883566  0.885902 0.831666 0.882724
 GradientBoostingClassifier 221.0           0.884    0.878830  0.881207 0.825583 0.878421
 LogisticRegression         230.0           0.920    0.915170  0.916987 0.879457 0.915662
 GaussianNB                 231.0           0.924    0.919375  0.921682 0.885539 0.920046
 SVC                        230.0           0.920    0.915170  0.916987 0.879457 0.915662
 DecisionTreeClassifier     214.0           0.856    0.848155  0.845622 0.782325 0.846414
```

### Comparing `mlpr-0.1.4/pyproject.toml` & `mlpr-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlpr"
-version = "0.1.4"
+version = "0.1.5"
 authors = ["Manuel Ferreira Junior <ferreira.jr.ufpb@gmail.com>"]
 description = "A library for machine learning pipeline and creation of reports."
 readme = "README.md"
 maintainers = [
     "Manuel Ferreira Junior <ferreira.jr.ufpb@gmail.com>"
 ]
 classifiers=[
```

### Comparing `mlpr-0.1.4/src/mlpr/ml/supervisioned/classification/uncertainty.py` & `mlpr-0.1.5/src/mlpr/ml/supervisioned/classification/uncertainty.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.4/src/mlpr/ml/supervisioned/classification/utils.py` & `mlpr-0.1.5/src/mlpr/ml/supervisioned/classification/utils.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.4/src/mlpr/ml/supervisioned/regression/metrics.py` & `mlpr-0.1.5/src/mlpr/ml/supervisioned/regression/metrics.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.4/src/mlpr/ml/supervisioned/regression/plots.py` & `mlpr-0.1.5/src/mlpr/ml/supervisioned/regression/plots.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.4/src/mlpr/ml/supervisioned/tunning/grid_search.py` & `mlpr-0.1.5/src/mlpr/ml/supervisioned/tunning/grid_search.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.4/src/mlpr/reports/create.py` & `mlpr-0.1.5/src/mlpr/reports/create.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.4/PKG-INFO` & `mlpr-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpr
-Version: 0.1.4
+Version: 0.1.5
 Summary: A library for machine learning pipeline and creation of reports.
 Author: Manuel Ferreira Junior
 Author-email: ferreira.jr.ufpb@gmail.com
 Maintainer: Manuel Ferreira Junior
 Maintainer-email: ferreira.jr.ufpb@gmail.com
 Requires-Python: >=3.9
 Classifier: Development Status :: 3 - Alpha
@@ -143,17 +143,15 @@
 from sklearn.neighbors import KNeighborsClassifier
 from sklearn.svm import SVC
 from sklearn.tree import DecisionTreeClassifier
 
 from sklearn.datasets import make_blobs
 from sklearn.metrics import accuracy_score, precision_score, recall_score, f1_score, cohen_kappa_score
 
-
-from src.mlpr.ml.supervisioned.tunning.grid_search import GridSearch
-from utils.reader import read_file_yaml
+from mlpr.ml.supervisioned.tunning.grid_search import GridSearch
 ```
 
 ## Methods
 
 Here we have a custom method for accuracy to use in model selection. Thus:
 
 ```python
@@ -405,17 +403,17 @@
 from sklearn.linear_model import LogisticRegression
 from sklearn.metrics import (accuracy_score, cohen_kappa_score, f1_score,
                              precision_score, recall_score)
 from sklearn.naive_bayes import GaussianNB
 from sklearn.svm import SVC
 from sklearn.tree import DecisionTreeClassifier
 
-from src.mlpr.ml.supervisioned.classification.uncertainty import UncertaintyPlots
-from src.mlpr.ml.supervisioned.classification.utils import calculate_probas
-from src.mlpr.ml.supervisioned.tunning.grid_search import GridSearch
+from mlpr.ml.supervisioned.classification.uncertainty import UncertaintyPlots
+from mlpr.ml.supervisioned.classification.utils import calculate_probas
+from mlpr.ml.supervisioned.tunning.grid_search import GridSearch
 
 import warnings
 warnings.filterwarnings("ignore")
 ```
 
 ## Parameters
 Setting parameters for the experiments.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mlpr Version: 0.1.4 Summary: A library for machine
+Metadata-Version: 2.1 Name: mlpr Version: 0.1.5 Summary: A library for machine
 learning pipeline and creation of reports. Author: Manuel Ferreira Junior
 Author-email: ferreira.jr.ufpb@gmail.com Maintainer: Manuel Ferreira Junior
 Maintainer-email: ferreira.jr.ufpb@gmail.com Requires-Python: >=3.9 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: MacOS Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: Unix
@@ -53,33 +53,32 @@
 matplotlib.pyplot as plt from sklearn.base import BaseEstimator from
 sklearn.ensemble import RandomForestClassifier, GradientBoostingClassifier from
 sklearn.linear_model import LogisticRegression from sklearn.naive_bayes import
 GaussianNB from sklearn.neighbors import KNeighborsClassifier from sklearn.svm
 import SVC from sklearn.tree import DecisionTreeClassifier from
 sklearn.datasets import make_blobs from sklearn.metrics import accuracy_score,
 precision_score, recall_score, f1_score, cohen_kappa_score from
-src.mlpr.ml.supervisioned.tunning.grid_search import GridSearch from
-utils.reader import read_file_yaml ``` ## Methods Here we have a custom method
-for accuracy to use in model selection. Thus: ```python def
-custom_accuracy_score(y_true: np.ndarray, y_pred: np.ndarray) -> float: return
-accuracy_score(y_true, y_pred, normalize=False) ``` ## Loading the Data Load
-your dataset. In this example, we're generating a dataset for classification
-using sklearn: ```python n_samples = 1000 centers = [(0, 0), (3, 4.5)]
-n_features = 2 cluster_std = 1.3 random_state = 42 ``` ```python np.random.seed
-(random_state) ``` ```python X, y = make_blobs( n_samples=n_samples,
-centers=centers, n_features=n_features, cluster_std=cluster_std,
-random_state=random_state ) ``` ## Plot the dataset ```python fig, ax =
-plt.subplots(1, 1, figsize=(14, 6)) ax.plot(X[:, 0][y == 0], X[:, 1][y == 0],
-"bs") ax.plot(X[:, 0][y == 1], X[:, 1][y == 1], "g^") ax.set_title("Dataset")
-ax.set_frame_on(False) ax.set_xticks([]) ax.set_yticks([]) fig.tight_layout()
-``` [![fig0](https://raw.githack.com/Manuelfjr/mlpr/develop/assets/
-tunning_scatter.png)](https://raw.githack.com/Manuelfjr/mlpr/develop/assets/
-tunning_scatter.png) ## Cross-validtion ```python models: Dict[BaseEstimator,
-Dict] = { RandomForestClassifier: { 'n_estimators': [10, 50, 100, 200],
-'max_depth': [None, 5, 10, 15], 'min_samples_split': [2, 5, 10],
+mlpr.ml.supervisioned.tunning.grid_search import GridSearch ``` ## Methods Here
+we have a custom method for accuracy to use in model selection. Thus: ```python
+def custom_accuracy_score(y_true: np.ndarray, y_pred: np.ndarray) -> float:
+return accuracy_score(y_true, y_pred, normalize=False) ``` ## Loading the Data
+Load your dataset. In this example, we're generating a dataset for
+classification using sklearn: ```python n_samples = 1000 centers = [(0, 0), (3,
+4.5)] n_features = 2 cluster_std = 1.3 random_state = 42 ``` ```python
+np.random.seed(random_state) ``` ```python X, y = make_blobs
+( n_samples=n_samples, centers=centers, n_features=n_features,
+cluster_std=cluster_std, random_state=random_state ) ``` ## Plot the dataset
+```python fig, ax = plt.subplots(1, 1, figsize=(14, 6)) ax.plot(X[:, 0][y ==
+0], X[:, 1][y == 0], "bs") ax.plot(X[:, 0][y == 1], X[:, 1][y == 1], "g^")
+ax.set_title("Dataset") ax.set_frame_on(False) ax.set_xticks([]) ax.set_yticks(
+[]) fig.tight_layout() ``` [![fig0](https://raw.githack.com/Manuelfjr/mlpr/
+develop/assets/tunning_scatter.png)](https://raw.githack.com/Manuelfjr/mlpr/
+develop/assets/tunning_scatter.png) ## Cross-validtion ```python models: Dict
+[BaseEstimator, Dict] = { RandomForestClassifier: { 'n_estimators': [10, 50,
+100, 200], 'max_depth': [None, 5, 10, 15], 'min_samples_split': [2, 5, 10],
 'min_samples_leaf': [1, 2, 4], 'random_state': [random_state] },
 GradientBoostingClassifier: { 'n_estimators': [50, 100, 200], 'learning_rate':
 [0.1, 0.05, 0.01, 0.005], 'subsample': [0.5, 0.8, 1.0], 'random_state':
 [random_state] }, LogisticRegression: { 'C': [0.01, 0.1, 1.0, 10.0], 'penalty':
 ['l1', 'l2'], 'solver': ['liblinear', 'saga'], 'random_state': [random_state]
 }, GaussianNB: { 'var_smoothing': [1e-9, 1e-8, 1e-7, 1e-6, 1e-5] },
 KNeighborsClassifier: { 'n_neighbors': [3, 5, 7, 9], 'weights': ['uniform',
@@ -122,63 +121,63 @@
 matplotlib.pyplot as plt import numpy as np import pandas as pd from
 sklearn.base import BaseEstimator from sklearn.datasets import make_blobs from
 sklearn.ensemble import GradientBoostingClassifier, RandomForestClassifier from
 sklearn.linear_model import LogisticRegression from sklearn.metrics import
 (accuracy_score, cohen_kappa_score, f1_score, precision_score, recall_score)
 from sklearn.naive_bayes import GaussianNB from sklearn.svm import SVC from
 sklearn.tree import DecisionTreeClassifier from
-src.mlpr.ml.supervisioned.classification.uncertainty import UncertaintyPlots
-from src.mlpr.ml.supervisioned.classification.utils import calculate_probas
-from src.mlpr.ml.supervisioned.tunning.grid_search import GridSearch import
-warnings warnings.filterwarnings("ignore") ``` ## Parameters Setting parameters
-for the experiments. ```python random_state: int = 42 n_feats: int = 2 n_size:
-int = 1000 centers: list[tuple] = [ (0, 2), (2, 0), (5, 4.5) ] n_class: int =
-len(centers) cluster_std: list[float] = [1.4, 1.4, 0.8] cv: int = 5
-np.random.seed(random_state) ``` ```python params: dict[str, dict[str, any]] =
-{ "n_samples": n_size, "n_features": n_feats, "centers": centers,
-"cluster_std": cluster_std, "random_state": random_state } ``` ```python
-np.random.seed(random_state) ``` ```python params_split: dict[str, float | int]
-= { 'test_size': 0.25, 'random_state': random_state } params_norm: dict[str,
-bool] = {'with_mean': True, 'with_std': True} model_metrics: dict[str, any] =
-{ 'custom_accuracy': partial(accuracy_score, normalize=False), 'accuracy':
-accuracy_score, 'precision': partial(precision_score, average='macro'),
-'recall': partial(recall_score, average='macro'), 'kappa': cohen_kappa_score,
-'f1': partial(f1_score, average='macro'), } ``` ## Load the dataset Here we are
-generating a dataset for experiments, using blobs from scikit-learn. ```python
-X, y = make_blobs( **params ) ``` ## Plot the dataset Behavior of the dataset
-used in the experiment. ```python markers = ['o', 'v', '^'] fig, ax =
-plt.subplots(1, 1, figsize=(14, 6)) colors = generate_colors("FF4B3E",
-"1C2127", len(np.unique(y))) for i, k in enumerate(np.unique(y)): ax.scatter(X
-[:, 0][y == k], X[:, 1][y == k], marker=markers[i % len(markers)], color=colors
-[i], label=f"c{i}") ax.set_title("Dataset") ax.set_frame_on(False)
-ax.set_xticks([]) ax.set_yticks([]) for center, color in zip(centers, colors):
-ax.scatter( center[0], center[1], color="white", linewidths=3, marker="o",
-edgecolor="black", s=120 ) plt.legend() fig.tight_layout() ``` [![fig1](https:/
-/raw.githack.com/Manuelfjr/mlpr/develop/assets/classification_scatter.png)]
-(https://raw.githack.com/Manuelfjr/mlpr/develop/assets/
-classification_scatter.png) ## Cross-validation ```python models: Dict
-[BaseEstimator, Dict] = { RandomForestClassifier: { 'n_estimators': [10, 50,
-100, 200], 'max_depth': [None, 5, 10, 15], 'min_samples_split': [2, 5, 10],
-'min_samples_leaf': [1, 2, 4], 'random_state': [random_state] },
-GradientBoostingClassifier: { 'n_estimators': [50, 100, 200], 'learning_rate':
-[0.1, 0.05, 0.01, 0.005], 'subsample': [0.5, 0.8, 1.0], 'random_state':
-[random_state] }, LogisticRegression: { 'C': [0.01, 0.1, 1.0, 10.0], 'penalty':
-['l1', 'l2'], 'solver': ['liblinear', 'saga'], 'random_state': [random_state],
-'max_iter': [10000] }, GaussianNB: { 'var_smoothing': [1e-9, 1e-8, 1e-7, 1e-6,
-1e-5] }, SVC: { 'C': [0.01, 0.1, 1.0, 10.0], 'kernel': ['linear', 'poly',
-'rbf', 'sigmoid'], 'degree': [2, 3, 4], 'gamma': ['scale', 'auto'],
-'probability': [True], 'random_state': [random_state] },
-DecisionTreeClassifier: { 'criterion': ['gini', 'entropy'], 'splitter':
-['best', 'random'], 'max_depth': [None, 5, 10, 15], 'min_samples_split': [2, 5,
-10], 'min_samples_leaf': [1, 2, 4], 'random_state': [random_state] } } ```
-```python grid_search = GridSearch( X, y, params_split=params_split,
-models_params=models, normalize=True, params_norm=params_norm,
-scoring='accuracy', metrics=model_metrics ) grid_search.search(cv=cv, n_jobs=-
-1) best_model, best_params = \ grid_search \ .get_best_model() ``` ```python
-results: pd.DataFrame = pd.DataFrame(grid_search._metrics).T results ```
+mlpr.ml.supervisioned.classification.uncertainty import UncertaintyPlots from
+mlpr.ml.supervisioned.classification.utils import calculate_probas from
+mlpr.ml.supervisioned.tunning.grid_search import GridSearch import warnings
+warnings.filterwarnings("ignore") ``` ## Parameters Setting parameters for the
+experiments. ```python random_state: int = 42 n_feats: int = 2 n_size: int =
+1000 centers: list[tuple] = [ (0, 2), (2, 0), (5, 4.5) ] n_class: int = len
+(centers) cluster_std: list[float] = [1.4, 1.4, 0.8] cv: int = 5 np.random.seed
+(random_state) ``` ```python params: dict[str, dict[str, any]] = { "n_samples":
+n_size, "n_features": n_feats, "centers": centers, "cluster_std": cluster_std,
+"random_state": random_state } ``` ```python np.random.seed(random_state) ```
+```python params_split: dict[str, float | int] = { 'test_size': 0.25,
+'random_state': random_state } params_norm: dict[str, bool] = {'with_mean':
+True, 'with_std': True} model_metrics: dict[str, any] = { 'custom_accuracy':
+partial(accuracy_score, normalize=False), 'accuracy': accuracy_score,
+'precision': partial(precision_score, average='macro'), 'recall': partial
+(recall_score, average='macro'), 'kappa': cohen_kappa_score, 'f1': partial
+(f1_score, average='macro'), } ``` ## Load the dataset Here we are generating a
+dataset for experiments, using blobs from scikit-learn. ```python X, y =
+make_blobs( **params ) ``` ## Plot the dataset Behavior of the dataset used in
+the experiment. ```python markers = ['o', 'v', '^'] fig, ax = plt.subplots(1,
+1, figsize=(14, 6)) colors = generate_colors("FF4B3E", "1C2127", len(np.unique
+(y))) for i, k in enumerate(np.unique(y)): ax.scatter(X[:, 0][y == k], X[:, 1]
+[y == k], marker=markers[i % len(markers)], color=colors[i], label=f"c{i}")
+ax.set_title("Dataset") ax.set_frame_on(False) ax.set_xticks([]) ax.set_yticks(
+[]) for center, color in zip(centers, colors): ax.scatter( center[0], center
+[1], color="white", linewidths=3, marker="o", edgecolor="black", s=120 )
+plt.legend() fig.tight_layout() ``` [![fig1](https://raw.githack.com/Manuelfjr/
+mlpr/develop/assets/classification_scatter.png)](https://raw.githack.com/
+Manuelfjr/mlpr/develop/assets/classification_scatter.png) ## Cross-validation
+```python models: Dict[BaseEstimator, Dict] = { RandomForestClassifier:
+{ 'n_estimators': [10, 50, 100, 200], 'max_depth': [None, 5, 10, 15],
+'min_samples_split': [2, 5, 10], 'min_samples_leaf': [1, 2, 4], 'random_state':
+[random_state] }, GradientBoostingClassifier: { 'n_estimators': [50, 100, 200],
+'learning_rate': [0.1, 0.05, 0.01, 0.005], 'subsample': [0.5, 0.8, 1.0],
+'random_state': [random_state] }, LogisticRegression: { 'C': [0.01, 0.1, 1.0,
+10.0], 'penalty': ['l1', 'l2'], 'solver': ['liblinear', 'saga'],
+'random_state': [random_state], 'max_iter': [10000] }, GaussianNB:
+{ 'var_smoothing': [1e-9, 1e-8, 1e-7, 1e-6, 1e-5] }, SVC: { 'C': [0.01, 0.1,
+1.0, 10.0], 'kernel': ['linear', 'poly', 'rbf', 'sigmoid'], 'degree': [2, 3,
+4], 'gamma': ['scale', 'auto'], 'probability': [True], 'random_state':
+[random_state] }, DecisionTreeClassifier: { 'criterion': ['gini', 'entropy'],
+'splitter': ['best', 'random'], 'max_depth': [None, 5, 10, 15],
+'min_samples_split': [2, 5, 10], 'min_samples_leaf': [1, 2, 4], 'random_state':
+[random_state] } } ``` ```python grid_search = GridSearch( X, y,
+params_split=params_split, models_params=models, normalize=True,
+params_norm=params_norm, scoring='accuracy', metrics=model_metrics )
+grid_search.search(cv=cv, n_jobs=-1) best_model, best_params = \ grid_search \
+.get_best_model() ``` ```python results: pd.DataFrame = pd.DataFrame
+(grid_search._metrics).T results ```
                            ccuussttoomm__aaccccuurraaccyy aaccccuurraaccyy pprreecciissiioonn rreeccaallll   kkaappppaa    ff11
 RandomForestClassifier     222.0           0.888    0.883566  0.885902 0.831666 0.882724
 GradientBoostingClassifier 221.0           0.884    0.878830  0.881207 0.825583 0.878421
 LogisticRegression         230.0           0.920    0.915170  0.916987 0.879457 0.915662
 GaussianNB                 231.0           0.924    0.919375  0.921682 0.885539 0.920046
 SVC                        230.0           0.920    0.915170  0.916987 0.879457 0.915662
 DecisionTreeClassifier     214.0           0.856    0.848155  0.845622 0.782325 0.846414
```

