# Comparing `tmp/prophetverse-0.0.3rc1.tar.gz` & `tmp/prophetverse-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prophetverse-0.0.3rc1.tar", max compression
+gzip compressed data, was "prophetverse-0.0.4.tar", max compression
```

## Comparing `prophetverse-0.0.3rc1.tar` & `prophetverse-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,22 @@
--rw-r--r--   0        0        0    11357 2024-04-30 13:00:34.998978 prophetverse-0.0.3rc1/LICENSE
--rw-r--r--   0        0        0     3328 2024-04-30 13:00:34.998978 prophetverse-0.0.3rc1/README.md
--rw-r--r--   0        0        0      673 2024-04-30 13:01:41.506610 prophetverse-0.0.3rc1/pyproject.toml
--rw-r--r--   0        0        0       61 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/__init__.py
--rw-r--r--   0        0        0     1797 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/changepoint.py
--rw-r--r--   0        0        0    14517 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/effects.py
--rw-r--r--   0        0        0     6608 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/engine.py
--rw-r--r--   0        0        0       66 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/logger.py
--rw-r--r--   0        0        0      110 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/models/__init__.py
--rw-r--r--   0        0        0       25 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/models/multivariate_model/__init__.py
--rw-r--r--   0        0        0     2528 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/models/multivariate_model/_model.py
--rw-r--r--   0        0        0     1541 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/models/multivariate_model/changepoint.py
--rw-r--r--   0        0        0     4831 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/models/multivariate_model/multiindex.py
--rw-r--r--   0        0        0     1546 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/models/univariate_model.py
--rw-r--r--   0        0        0       77 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/sktime/__init__.py
--rw-r--r--   0        0        0     4364 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/sktime/_expand_column_per_level.py
--rw-r--r--   0        0        0    14328 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/sktime/base.py
--rw-r--r--   0        0        0    25304 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/sktime/multivariate.py
--rw-r--r--   0        0        0     2054 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/sktime/seasonality.py
--rw-r--r--   0        0        0    13915 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/sktime/univariate.py
--rw-r--r--   0        0        0     3813 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/utils/frame_to_array.py
--rw-r--r--   0        0        0     1206 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/utils/logistic.py
--rw-r--r--   0        0        0      756 2024-04-30 13:00:35.018978 prophetverse-0.0.3rc1/src/prophetverse/utils/regex.py
--rw-r--r--   0        0        0     3874 1970-01-01 00:00:00.000000 prophetverse-0.0.3rc1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-10 22:04:44.945565 prophetverse-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3328 2024-05-10 22:04:44.945565 prophetverse-0.0.4/README.md
+-rw-r--r--   0        0        0      668 2024-05-10 22:04:53.769589 prophetverse-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       61 2024-05-10 22:04:44.965565 prophetverse-0.0.4/src/prophetverse/__init__.py
+-rw-r--r--   0        0        0     8336 2024-05-10 22:04:44.965565 prophetverse-0.0.4/src/prophetverse/effects.py
+-rw-r--r--   0        0        0     6688 2024-05-10 22:04:44.965565 prophetverse-0.0.4/src/prophetverse/engine.py
+-rw-r--r--   0        0        0       59 2024-05-10 22:04:44.965565 prophetverse-0.0.4/src/prophetverse/logger.py
+-rw-r--r--   0        0        0     4032 2024-05-10 22:04:44.965565 prophetverse-0.0.4/src/prophetverse/models.py
+-rw-r--r--   0        0        0       77 2024-05-10 22:04:44.965565 prophetverse-0.0.4/src/prophetverse/sktime/__init__.py
+-rw-r--r--   0        0        0     4701 2024-05-10 22:04:44.965565 prophetverse-0.0.4/src/prophetverse/sktime/_expand_column_per_level.py
+-rw-r--r--   0        0        0    14213 2024-05-10 22:04:44.965565 prophetverse-0.0.4/src/prophetverse/sktime/base.py
+-rw-r--r--   0        0        0    15371 2024-05-10 22:04:44.965565 prophetverse-0.0.4/src/prophetverse/sktime/multivariate.py
+-rw-r--r--   0        0        0     2054 2024-05-10 22:04:44.965565 prophetverse-0.0.4/src/prophetverse/sktime/seasonality.py
+-rw-r--r--   0        0        0    10052 2024-05-10 22:04:44.965565 prophetverse-0.0.4/src/prophetverse/sktime/univariate.py
+-rw-r--r--   0        0        0       25 2024-05-10 22:04:44.965565 prophetverse-0.0.4/src/prophetverse/trend/__init__.py
+-rw-r--r--   0        0        0     2836 2024-05-10 22:04:44.965565 prophetverse-0.0.4/src/prophetverse/trend/base.py
+-rw-r--r--   0        0        0    16632 2024-05-10 22:04:44.965565 prophetverse-0.0.4/src/prophetverse/trend/piecewise.py
+-rw-r--r--   0        0        0       77 2024-05-10 22:04:44.965565 prophetverse-0.0.4/src/prophetverse/utils/__init__.py
+-rw-r--r--   0        0        0     4309 2024-05-10 22:04:44.965565 prophetverse-0.0.4/src/prophetverse/utils/frame_to_array.py
+-rw-r--r--   0        0        0      988 2024-05-10 22:04:44.965565 prophetverse-0.0.4/src/prophetverse/utils/multiindex.py
+-rw-r--r--   0        0        0      802 2024-05-10 22:04:44.965565 prophetverse-0.0.4/src/prophetverse/utils/regex.py
+-rw-r--r--   0        0        0     3871 1970-01-01 00:00:00.000000 prophetverse-0.0.4/PKG-INFO
```

### Comparing `prophetverse-0.0.3rc1/LICENSE` & `prophetverse-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.3rc1/README.md` & `prophetverse-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.3rc1/src/prophetverse/engine.py` & `prophetverse-0.0.4/src/prophetverse/engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import Callable
+
+import jax
 import numpyro
-from numpyro.infer.initialization import init_to_mean
-from numpyro.infer import SVI, TraceEnum_ELBO, init_to_value, Trace_ELBO, MCMC, NUTS, Predictive
+from numpyro.infer import (MCMC, NUTS, SVI, Predictive, Trace_ELBO,
+                           TraceEnum_ELBO, init_to_value)
 from numpyro.infer.autoguide import AutoDelta
-import jax
+from numpyro.infer.initialization import init_to_mean
 
 
 class InferenceEngine:
     """Class representing an inference engine for a given model.
 
     Args:
         model (Callable): The model to be used for inference.
@@ -64,37 +66,40 @@
         num_steps (int, optional): The number of optimization steps to perform. Defaults to 10000.
         rng_key (jax.random.PRNGKey, optional): The random number generator key. Defaults to None.
     """
 
     def __init__(
         self,
         model: Callable,
-        optimizer: numpyro.optim._NumPyroOptim = None,
+        optimizer_factory: numpyro.optim._NumPyroOptim = None,
         num_steps=10000,
         rng_key=None,
     ):
-        if optimizer is None:
-            optimizer = numpyro.optim.Adam(step_size=0.001)
-        self.optimizer = optimizer
+        if optimizer_factory is None:
+            optimizer_factory = self.default_optimizer_factory
+        self.optimizer_factory = optimizer_factory
         self.num_steps = num_steps
         super().__init__(model, rng_key)
 
+    def default_optimizer_factory(self):
+        return numpyro.optim.Adam(step_size=0.001)
+
     def infer(self, **kwargs):
         """
         Perform MAP inference.
 
         Args:
             **kwargs: Additional keyword arguments to be passed to the model.
 
         Returns:
             self: The updated MAPInferenceEngine object.
         """
         self.guide_ = AutoDelta(self.model, init_loc_fn=init_to_mean())
-        self.svi_ = SVI(self.model, self.guide_, self.optimizer, loss=Trace_ELBO())
-        self.run_results_ = self.svi_.run(
+        svi_ = SVI(self.model, self.guide_, self.optimizer_factory(), loss=Trace_ELBO())
+        self.run_results_ = svi_.run(
             rng_key=self.rng_key, num_steps=self.num_steps, **kwargs
         )
         self.posterior_samples_ = self.guide_.sample_posterior(self.rng_key, params=self.run_results_.params, **kwargs)
         return self
 
     def predict(self, **kwargs):
         """
@@ -187,13 +192,13 @@
         Args:
             **kwargs: Additional keyword arguments to be passed to the Predictive method.
 
         Returns:
             Dict[str, np.ndarray]: The predictive samples.
 
         """
-        sites = set(self.posterior_samples_.keys()).union(["obs"])
-        predictive = Predictive(self.model, self.posterior_samples_, return_sites=sites)
+        
+        predictive = Predictive(self.model, self.posterior_samples_)
 
         self.samples_predictive_ = predictive(self.rng_key, **kwargs)
         self.samples_ = self.mcmc_.get_samples()
         return self.samples_predictive_
```

### Comparing `prophetverse-0.0.3rc1/src/prophetverse/models/multivariate_model/multiindex.py` & `prophetverse-0.0.4/src/prophetverse/utils/frame_to_array.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,23 @@
 import numpy as np
 import pandas as pd
 from jax import numpy as jnp
 from sktime.transformations.hierarchical.reconcile import _get_s_matrix
 
 NANOSECONDS_TO_SECONDS = 1000 * 1000 * 1000
 
+__all__ = [
+    "get_bottom_series_idx",
+    "get_multiindex_loc",
+    "loc_bottom_series",
+    "iterate_all_series",
+    "convert_index_to_days_since_epoch",
+    "series_to_tensor",
+    "convert_dataframe_to_tensors",
+]
 
 def get_bottom_series_idx(y):
     """
     Get the index of the bottom series in a hierarchical time series.
 
     Parameters:
     y (pd.DataFrame): The hierarchical time series.
@@ -53,14 +62,17 @@
 
     Parameters:
     y (pd.DataFrame): The hierarchical time series.
 
     Returns:
     pd.DataFrame: The bottom series.
     """
+    
+    if y.index.nlevels == 1:
+        return y
     return get_multiindex_loc(y, get_bottom_series_idx(y))
 
 
 def iterate_all_series(y):
     """
     Iterate over all series in a hierarchical time series.
 
@@ -82,14 +94,19 @@
     Parameters:
     idx (pd.Index): The pandas Index.
 
     Returns:
     np.ndarray: The converted array of days since epoch.
     """
     t = idx
+    
+    if not (isinstance(t, pd.PeriodIndex) or isinstance(t, pd.DatetimeIndex)):
+        return t.values
+    
+    
     if isinstance(t, pd.PeriodIndex):
         t = t.to_timestamp()
 
     return t.to_numpy(dtype=np.int64) // NANOSECONDS_TO_SECONDS / (3600 * 24.0)
 
 
 def series_to_tensor(y):
@@ -101,14 +118,18 @@
 
     Returns:
     jnp.ndarray: The JAX tensor representing all series.
     """
     names = []
     array = []
     series_len = None
+    
+    if y.index.nlevels== 1:
+        return jnp.array(y.values).reshape((1, -1, len(y.columns)))
+    
     for idx, series in iterate_all_series(y):
         if series_len is None:
             series_len = len(series)
         if len(series) != series_len:
             raise ValueError("Series {} has length {}, but expected {}".format(idx, len(series), series_len))
         
         names.append(idx)
@@ -146,36 +167,7 @@
     tuple: A tuple containing the time arrays and the DataFrame arrays as JAX tensors.
     """
     t_arrays = extract_timetensor_from_dataframe(df)
 
     df_as_arrays = series_to_tensor(df)
 
     return t_arrays, df_as_arrays
-
-
-def reindex_time_series(df, new_time_index):
-    """
-    Reindexes the time index level (-1) of a multi-index DataFrame with a new time index.
-
-    Parameters:
-    df (pd.DataFrame): The original DataFrame with a multi-level index.
-    new_time_index (pd.Index or similar): The new time index to apply to the DataFrame.
-
-    Returns:
-    pd.DataFrame: A DataFrame with the updated time index.
-    """
-    # Ensure the input DataFrame has a multi-index
-    if not isinstance(df.index, pd.MultiIndex):
-        raise ValueError("DataFrame must have a multi-level index")
-
-    # Extract the current indices except for the time index
-    levels = df.index.levels[:-1]
-    labels = df.index.codes[:-1]
-    names = df.index.names[:-1]
-
-    # Create a new multi-index combining the existing levels with the new time index
-    new_index = pd.MultiIndex.from_product(
-        levels + [new_time_index], names=names + [df.index.names[-1]]
-    )
-
-    # Reindex the DataFrame using the new index
-    return df.reindex(new_index)
```

### Comparing `prophetverse-0.0.3rc1/src/prophetverse/sktime/_expand_column_per_level.py` & `prophetverse-0.0.4/src/prophetverse/sktime/_expand_column_per_level.py`

 * *Files 13% similar despite different names*

```diff
@@ -36,26 +36,33 @@
         Parameters:
         - X (pd.DataFrame): The input data.
         - y (pd.Series or None): The target variable. Not used in this transformer.
 
         Returns:
         - self (ExpandColumnPerLevel): The fitted transformer object.
         """
-        regex_patterns = [re.compile(pattern) for pattern in self.columns_regex]
+        regex_patterns = [re.compile(str(pattern)) for pattern in self.columns_regex]
         self.matched_columns_ = set(
             [
                 col
                 for col in X.columns
                 for pattern in regex_patterns
-                if pattern.match(col)
+                if pattern.match(str(col))
             ]
         )
 
         self.new_columns_ = {}
         # Ensure identifiers are tuples
+        if X.index.nlevels == 1:
+            self.skip_transform_ = True
+            self.series_identifiers_ = None
+            self.new_columns_ = {col: col for col in self.matched_columns_}
+            return self 
+        
+        self.skip_transform_ = False
         self.series_identifiers_ = [
             idx if isinstance(idx, tuple) else (idx,)
             for idx in X.index.droplevel(-1).unique()
         ]
         for identifier in self.series_identifiers_:
             for col in self.matched_columns_:
                 self.new_columns_[self.get_col_name(col, identifier)] = col
@@ -82,14 +89,17 @@
         Parameters:
         - X (pd.DataFrame): The input data.
         - y (pd.Series or None): The target variable. Not used in this transformer.
 
         Returns:
         - X_transformed (pd.DataFrame): The transformed data with expanded columns.
         """
+        if self.skip_transform_:
+            return X
+        
         if not isinstance(X.index, pd.MultiIndex):
             raise ValueError("Input must have a multi-level index")
         X_original = X.copy()
         X = X.copy()
 
         regex_patterns = [re.compile(pattern) for pattern in self.columns_regex]
         matched_columns = self.matched_columns_
```

### Comparing `prophetverse-0.0.3rc1/src/prophetverse/sktime/base.py` & `prophetverse-0.0.4/src/prophetverse/sktime/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 import itertools
+import logging
+import re
+from collections import OrderedDict
 from typing import Any, Dict, List, Optional, Tuple, Union
 
-import numpy as np
 import jax
 import jax.numpy as jnp
+import numpy as np
 import numpyro
 import numpyro.distributions as dist
 import pandas as pd
 from numpyro import sample
 from numpyro.contrib.control_flow import scan
 from numpyro.infer import MCMC, NUTS, Predictive, init_to_mean
 from sktime.forecasting.base import BaseForecaster, ForecastingHorizon
-from collections import OrderedDict
-from prophetverse.engine import MAPInferenceEngine, MCMCInferenceEngine, InferenceEngine
-from prophetverse.effects import LinearEffect
+
+from prophetverse.effects import AbstractEffect, LinearEffect
+from prophetverse.engine import (InferenceEngine, MAPInferenceEngine,
+                                 MCMCInferenceEngine)
 from prophetverse.utils.frame_to_array import series_to_tensor
-from prophetverse.effects import AbstractEffect
-import re
-import logging
+
 
 class BaseBayesianForecaster(BaseForecaster):
     """
     Base class for Bayesian forecasters in hierarchical-prophet.
 
     Args:
         rng_seed (int): Random number generator seed.
         method (str): Inference method to use. Currently, only "mcmc" is supported.
         num_samples (int): Number of MCMC samples to draw.
         num_warmup (int): Number of warmup steps for MCMC.
         num_chains (int): Number of MCMC chains to run.
-        
+
         *args: Additional positional arguments.
         **kwargs: Additional keyword arguments.
     """
 
     _tags = {
         "capability:pred_int": True,
         "capability:pred_int:insample": True,
+        "enforce_index_type": [pd.Period, pd.DatetimeIndex],
     }
 
     def __init__(
         self,
         rng_key,
         inference_method,
         mcmc_samples,
@@ -59,34 +62,46 @@
         self.mcmc_chains = mcmc_chains
         self.inference_method = inference_method
         self.optimizer_steps = optimizer_steps
         self.optimizer_name = optimizer_name
         self.optimizer_kwargs = optimizer_kwargs
         self._sample_sites = set()
         super().__init__(*args, **kwargs)
-        self.predictive_samples_ = None
-
-    @property
+        
+    
     def optimizer(self):
-        if self.optimizer_name.startswith('optax'):
+        optimizer_kwargs = self.optimizer_kwargs
+        optimizer_name = self.optimizer_name
+        rng_key = self.rng_key
+
+        if rng_key is None:
+            rng_key = jax.random.PRNGKey(24)
+
+        if optimizer_kwargs is None:
+            optimizer_kwargs = {"step_size": 1e-4}
+        if optimizer_name is None:
+            optimizer_name = "Adam"
+
+        if optimizer_name.startswith("optax"):
 
-            from numpyro.optim import optax_to_numpyro
             import optax
-            scheduler = optax.cosine_decay_schedule(**self.optimizer_kwargs)
+            from numpyro.optim import optax_to_numpyro
+
+            scheduler = optax.cosine_decay_schedule(**optimizer_kwargs)
 
             opt = optax_to_numpyro(
                 optax.chain(
-                    
                     optax.scale_by_adam(),
                     optax.scale_by_schedule(scheduler),
-                    optax.scale(-1.0))
+                    optax.scale(-1.0),
+                )
             )
             return opt
 
-        return getattr(numpyro.optim, self.optimizer_name)(**self.optimizer_kwargs)
+        return getattr(numpyro.optim, optimizer_name)(**optimizer_kwargs)
 
     def _get_fit_data(self, y, X, fh) -> Dict[str, Any]:
         """
         Get the data required for the Numpyro model.
 
         This method should be implemented by subclasses.
 
@@ -140,27 +155,38 @@
             fh (ForecastingHorizon): Forecasting horizon.
 
         Returns:
             self: The fitted Bayesian forecaster.
         """
 
         self._set_y_scales(y)
-        y  = self._scale_y(y)
+        y = self._scale_y(y)
 
+        self.internal_y_indexes_ = y.index
         data = self._get_fit_data(y, X, fh)
 
         self.distributions_ = data.get("distributions", {})
 
+        rng_key = self.rng_key
+        if rng_key is None:
+            rng_key = jax.random.PRNGKey(24)
+
         if self.inference_method == "mcmc":
-            self.inference_engine_ = MCMCInferenceEngine(self.model, num_samples=self.mcmc_samples, num_warmup=self.mcmc_warmup, num_chains=self.mcmc_chains, rng_key=self.rng_key)
+            self.inference_engine_ = MCMCInferenceEngine(
+                self.model,
+                num_samples=self.mcmc_samples,
+                num_warmup=self.mcmc_warmup,
+                num_chains=self.mcmc_chains,
+                rng_key=rng_key,
+            )
         elif self.inference_method == "map":
             self.inference_engine_ = MAPInferenceEngine(
                 self.model,
-                rng_key=self.rng_key,
-                optimizer=self.optimizer,
+                rng_key=rng_key,
+                optimizer_factory=self.optimizer,
                 num_steps=self.optimizer_steps,
             )
         else:
             raise ValueError(f"Unknown method {self.inference_method}")
 
         self.inference_engine_.infer(**data)
         self.posterior_samples_ = self.inference_engine_.posterior_samples_
@@ -175,74 +201,71 @@
             fh (ForecastingHorizon): Forecasting horizon.
             X (pd.DataFrame): Exogenous variables.
 
         Returns:
             pd.DataFrame: Point forecasts for the forecasting horizon.
         """
         predictive_samples = self.predict_samples(fh=fh, X=X)
-        self.forecast_samples_ = predictive_samples
         y_pred = predictive_samples.mean(axis=1).to_frame(self._y.columns[0])
 
         return y_pred
 
     def predict_all_sites(self, fh, X=None):
 
         if not isinstance(fh, ForecastingHorizon):
             fh = self._check_fh(fh)
 
         fh_as_index = self.fh_to_index(fh)
 
-        predict_data = self._get_predict_data(X=X,fh= fh)
+        predict_data = self._get_predict_data(X=X, fh=fh)
 
         predictive_samples_ = self.inference_engine_.predict(**predict_data)
         out = pd.DataFrame(
             data={
                 site: data.mean(axis=0).flatten()
                 for site, data in predictive_samples_.items()
             },
             index=self.periodindex_to_multiindex(fh_as_index),
         ).sort_index()
         return self._inv_scale_y(out)
 
-    def predict_samples(
-        self,
-        fh,
-        X=None
-):
+    def predict_samples(self, fh, X=None):
         """
         Generate samples from the posterior predictive distribution.
 
         Args:
             X (pd.DataFrame): Exogenous variables.
             fh (ForecastingHorizon): Forecasting horizon.
 
         Returns:
             pd.DataFrame: Samples from the posterior predictive distribution.
         """
         fh_as_index = self.fh_to_index(fh)
 
         predict_data = self._get_predict_data(X=X, fh=fh)
 
-        self.predictive_samples_ = self.inference_engine_.predict(**predict_data)
+        predictive_samples_ = self.inference_engine_.predict(**predict_data)
 
-        observation_site = self.predictive_samples_["obs"]
-        n_samples = self.predictive_samples_["obs"].shape[0]
+        observation_site = predictive_samples_["obs"]
+        n_samples = predictive_samples_["obs"].shape[0]
         preds = pd.DataFrame(
             data=observation_site.T.reshape((-1, n_samples)),
             columns=list(range(n_samples)),
             index=self.periodindex_to_multiindex(fh_as_index),
         ).sort_index()
 
         return self._inv_scale_y(preds)
 
     def _set_y_scales(self, y):
         if y.index.nlevels == 1:
             self._scale = y.abs().max().values[0]
         else:
-            self._scale = y.groupby(level=list(range(y.index.nlevels - 1))).agg(lambda x: np.abs(x).max())
+            self._scale = y.groupby(level=list(range(y.index.nlevels - 1))).agg(
+                lambda x: np.abs(x).max()
+            )
 
     def _scale_y(self, y):
         if y.index.nlevels == 1:
             return y / self._scale
         scale_for_each_obs = self._scale.loc[y.index.droplevel(-1)].values
         return y / scale_for_each_obs
 
@@ -287,31 +310,33 @@
 
         Returns:
             pd.MultiIndex: Converted MultiIndex.
         """
         if self._y.index.nlevels == 1:
             return periodindex
 
-        base_levels = self._y.index.droplevel(-1).unique().tolist()
-
-        # import Iterable
-        from collections.abc import Iterable
+        series_id_tuples = self.internal_y_indexes_.droplevel(-1).unique().tolist()
 
         # Check if base_levels 0 is a iterable:
-        if not isinstance(base_levels[0], tuple):
-            base_levels = [(x,) for x in base_levels]
+        if not isinstance(series_id_tuples[0], tuple):
+            series_id_tuples = [(x,) for x in series_id_tuples]
+
+        series_id_tuples = self._filter_series_tuples(series_id_tuples)
 
         return pd.Index(
             map(
                 lambda x: (*x[0], x[1]),
-                itertools.product(base_levels, periodindex),
+                itertools.product(series_id_tuples, periodindex),
             ),
-            name=self._y.index.names,
+            name=self.internal_y_indexes_.names,
         )
 
+    def _filter_series_tuples(self, levels: List[Tuple]) -> List[Tuple]:
+        return levels
+
     def fh_to_index(self, fh: ForecastingHorizon, y: pd.DataFrame = None):
         """
         Convert a ForecastingHorizon to an index.
 
         Args:
             fh (ForecastingHorizon): Forecasting horizon.
             y (pd.DataFrame, optional): Target variable. Defaults to None.
@@ -328,17 +353,16 @@
         return fh_dates
 
     @property
     def var_names(self):
 
         return list(self.distributions_.keys())
 
-    def plot_trace(self, *, figsize=(15,25), compact=True, var_names=None, **kwargs):
+    def plot_trace(self, *, figsize=(15, 25), compact=True, var_names=None, **kwargs):
         import arviz as az
-        
 
         if var_names is None:
             var_names = self.var_names
 
         return az.plot_trace(
             az.from_numpyro(self.inference_engine_.mcmc_),
             var_names=var_names,
@@ -348,65 +372,37 @@
         )
 
     @property
     def site_names(self) -> list[Any]:
         return list(self.posterior_samples_.keys())
 
 
-def init_params(distributions) -> dict:
-    """
-    Initializes the model parameters.
-    """
-
-    params = {}
-
-    for coefficient_name, distribution in distributions.items():
-
-        if not isinstance(distribution, OrderedDict):
-            params[coefficient_name] = numpyro.sample(coefficient_name, distribution)
-        else:
-            coefficients = []
-            for (
-                inner_coefficient_name,
-                coefficient_distribution,
-            ) in distribution.items():
-                coefficients.append(
-                    numpyro.sample(inner_coefficient_name, coefficient_distribution)
-                )
-            params[coefficient_name] = jnp.concatenate(coefficients, axis=0)
-
-    return params
-
-
 class ExogenousEffectMixin:
 
-    def __init__(self,
-                 
-                 exogenous_effects: List[AbstractEffect],
-                 default_effect = None,
-                 **kwargs):
+    def __init__(
+        self, exogenous_effects: List[AbstractEffect], default_effect=None, **kwargs
+    ):
 
-        
         self.exogenous_effects = exogenous_effects
         self.default_effect = default_effect
         super().__init__(**kwargs)
-        
-        if self.default_effect is None:
-            self.default_effect = LinearEffect(
-                id="default_exog",
-                prior=(dist.Normal, 0, 1),
-                effect_mode="additive",
-            )
 
     def _set_custom_effects(self, feature_names):
 
         effects_and_columns = {}
         columns_with_effects = set()
         exogenous_effects = self.exogenous_effects or {}
-        
+
+        default_effect = self.default_effect
+        if default_effect is None:
+            default_effect = LinearEffect(
+                id="default_exog",
+                prior=(dist.Normal, 0, 1),
+                effect_mode="additive",
+            )
 
         for effect in exogenous_effects:
 
             columns = effect.match_columns(feature_names)
 
             if columns_with_effects.intersection(columns):
                 raise ValueError(
@@ -433,34 +429,36 @@
 
         if len(features_without_effects):
 
             effects_and_columns.update(
                 {
                     "default": (
                         features_without_effects,
-                        self.default_effect,
+                        default_effect,
                     )
                 }
             )
 
         self._exogenous_effects_and_columns = effects_and_columns
 
     def _get_exogenous_data_array(self, X):
 
         out = {}
         for effect_name, (columns, _) in self._exogenous_effects_and_columns.items():
             # If no columns are found, skip
             if len(columns) == 0:
                 continue
-            
+
             if X.index.nlevels == 1:
                 array = jnp.array(X[columns].values)
             else:
                 array = series_to_tensor(X[columns])
 
-            out[effect_name] = array 
+            out[effect_name] = array
 
         return out
 
     @property
     def exogenous_effect_dict(self):
-        return {k: v[1] for k, v in self._exogenous_effects_and_columns.items() if len(v[0])}
+        return {
+            k: v[1] for k, v in self._exogenous_effects_and_columns.items() if len(v[0])
+        }
```

### Comparing `prophetverse-0.0.3rc1/src/prophetverse/sktime/seasonality.py` & `prophetverse-0.0.4/src/prophetverse/sktime/seasonality.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.3rc1/src/prophetverse/sktime/univariate.py` & `prophetverse-0.0.4/src/prophetverse/sktime/univariate.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,26 @@
 """ Univariate Prophet model
 
 This module implements the Univariate Prophet model, similar to the one implemented in the `prophet` library.
 
 """
-
-from typing import Callable
 from functools import partial
-from sktime.transformations.series.detrend import Detrender
+from typing import Callable
+
 import jax.numpy as jnp
 import pandas as pd
-from numpyro import distributions as dist
 from jax import random
+from numpyro import distributions as dist
 from sktime.forecasting.base import ForecastingHorizon
 
-from prophetverse.utils.frame_to_array import convert_index_to_days_since_epoch
-from prophetverse.sktime.base import (
-    BaseBayesianForecaster,
-    ExogenousEffectMixin, init_params,
-)
-
-
-from sktime.transformations.base import BaseTransformer
-from prophetverse.utils.logistic import suggest_logistic_rate_and_offset
-
-from prophetverse.models.univariate_model import model
-from prophetverse.changepoint import (
-    get_changepoint_matrix,
-    get_changepoint_timeindexes,
-)
-import functools
-
+from prophetverse.models import univariate_model
+from prophetverse.sktime.base import (BaseBayesianForecaster,
+                                      ExogenousEffectMixin)
+from prophetverse.trend.piecewise import (PiecewiseLinearTrend,
+                                          PiecewiseLogisticTrend, TrendModel)
 
 __all__ = ["Prophet"]
 
 
 class Prophet(ExogenousEffectMixin, BaseBayesianForecaster):
     """
 
@@ -96,19 +83,19 @@
         noise_scale=0.05,
         trend="linear",
         mcmc_samples=2000,
         mcmc_warmup=200,
         mcmc_chains=4,
         inference_method="map",
         optimizer_name="Adam",
-        optimizer_kwargs={"step_size" : 1e-4},
-        optimizer_steps=100_000,
+        optimizer_kwargs=None,
+        optimizer_steps=1_000,
         exogenous_effects=None,
         default_effect=None,
-        rng_key=random.PRNGKey(24),
+        rng_key=None,
     ):
         """
         Initializes the Prophet model.
         """
 
         self.changepoint_interval = changepoint_interval
         self.changepoint_range = changepoint_range
@@ -130,15 +117,15 @@
             mcmc_warmup=mcmc_warmup,
             mcmc_chains=mcmc_chains,
             optimizer_name=optimizer_name,
             optimizer_kwargs=optimizer_kwargs,
             optimizer_steps=optimizer_steps,
         )
 
-        self.model = model
+        self.model = univariate_model
         self._validate_hyperparams()
 
     def _validate_hyperparams(self):
         """
         Validate the hyperparameters
         """
         if self.changepoint_interval <= 0:
@@ -151,34 +138,61 @@
         if self.capacity_prior_scale <= 0:
             raise ValueError("capacity_prior_scale must be greater than 0.")
         if self.capacity_prior_loc <= 0:
             raise ValueError("capacity_prior_loc must be greater than 0.")
         if self.trend not in ["linear", "logistic"]:
             raise ValueError('trend must be either "linear" or "logistic".')
 
+    
+
     def _get_fit_data(self, y, X, fh):
         """
         Prepares the data for the Numpyro model.
 
         Args:
             y (pd.DataFrame): Time series data.
             X (pd.DataFrame): Exogenous variables.
             fh (ForecastingHorizon): Forecasting horizon.
 
         Returns:
             dict: Dictionary of data for the Numpyro model.
         """
 
-        self._set_time_scale(y)
+        fh = y.index.get_level_values(-1).unique()
 
         ## Changepoints and trend
-        self._set_changepoints_t(y)
-        t = self._index_to_scaled_timearray(y.index)
-        changepoint_matrix = self._get_changepoint_matrix(t)
-        trend_sample_func = self._get_trend_sample_func(y=y, X=X)
+        if self.trend == "linear":
+            self.trend_model_ = PiecewiseLinearTrend(
+                changepoint_interval=self.changepoint_interval,
+                changepoint_range=self.changepoint_range,
+                changepoint_prior_scale=self.changepoint_prior_scale)
+
+        elif self.trend == "logistic":
+            self.trend_model_ = PiecewiseLogisticTrend(
+                changepoint_interval=self.changepoint_interval,
+                changepoint_range=self.changepoint_range,
+                changepoint_prior_scale=self.changepoint_prior_scale,
+                capacity_prior=dist.TransformedDistribution(
+                    dist.HalfNormal(self.capacity_prior_scale),
+                    dist.transforms.AffineTransform(
+                        loc=self.capacity_prior_loc, scale=1
+                    ),
+                )
+            )
+
+        elif isinstance(self.trend, TrendModel):
+            self.trend_model_ = self.trend
+        else:
+            raise ValueError(
+                "trend must be either 'linear', 'logistic' or a TrendModel instance."
+            )
+
+        self.trend_model_.initialize(y)
+
+        trend_data = self.trend_model_.prepare_input_data(fh)
 
         ## Exogenous features
 
         if X is None:
             X = pd.DataFrame(index=y.index)
 
         if self.feature_transformer is not None:
@@ -191,165 +205,31 @@
         self._set_custom_effects(X.columns)
         exogenous_data = self._get_exogenous_data_array(X)
 
         y_array = jnp.array(y.values.flatten()).reshape((-1, 1))
 
         ## Inputs that also are used in predict
         self.fit_and_predict_data_ = {
-            "init_trend_params": trend_sample_func,
-            "trend_mode": self.trend,
-            "exogenous_effects": self.exogenous_effect_dict if self._has_exogenous else None,
-            }
+            
+            "trend_model": self.trend_model_,
+            "noise_scale" : self.noise_scale,
+            "exogenous_effects": (
+                self.exogenous_effect_dict if self._has_exogenous else None
+            ),
+        }
 
         inputs = {
-            "t": self._index_to_scaled_timearray(y.index),
             "y": y_array,
             "data": exogenous_data,
-            "changepoint_matrix": changepoint_matrix,
+            "trend_data": trend_data,
             **self.fit_and_predict_data_,
         }
 
         return inputs
 
-    def _get_trend_sample_func(self, y: pd.DataFrame, X: pd.DataFrame) -> Callable :
-        """
-        
-        Get a function that samples the trend parameters.
-        
-        This function may change in the future. Currently, the model function receives a function to get the changepoint coefficients.
-        This function is passed to the model as a partial function, with the changepoint coefficients as a parameter
-        
-        Args:
-            y (pd.DataFrame): Time series data.
-            X (pd.DataFrame): Exogenous variables.
-            
-        Returns:
-            Callable: Function that samples the trend parameters.
-        
-        """
-        t_scaled = self._index_to_scaled_timearray(y.index)
-        distributions = {}
-
-        changepoints_loc = jnp.zeros(len(self._changepoint_t))
-        detrender = Detrender()
-        trend = y - detrender.fit_transform(y)
-
-        if self.trend == "linear":
-
-            linear_global_rate = (trend.values[-1, 0] - trend.values[0, 0]) / (
-                t_scaled[-1] - t_scaled[0]
-            )
-            changepoints_loc.at[0].set(linear_global_rate)
-
-            distributions["changepoint_coefficients"] = dist.Laplace(
-                changepoints_loc,
-                jnp.ones(len(self._changepoint_t)) * (self.changepoint_prior_scale),
-            )
-
-            distributions["offset"] = dist.Normal(
-                (trend.values[0, 0] - linear_global_rate * t_scaled[0]),
-                0.1,
-            )
-
-        if self.trend == "logistic":
-
-            linear_global_rate, timeoffset = suggest_logistic_rate_and_offset(
-                t_scaled,
-                trend.values.flatten(),
-                capacities=self.capacity_prior_loc,
-            )
-
-            linear_global_rate = linear_global_rate[0]
-            timeoffset = timeoffset[0]
-            changepoints_loc.at[0].set(linear_global_rate)
-
-            changepoint_coefficients_distribution = dist.Laplace(
-                changepoints_loc,
-                jnp.ones(len(self._changepoint_t)) * self.changepoint_prior_scale,
-            )
-
-            distributions["changepoint_coefficients"] = (
-                changepoint_coefficients_distribution
-            )
-
-            distributions["offset"] = dist.Normal(timeoffset, jnp.log(2))
-
-            distributions["capacity"] = dist.TransformedDistribution(
-                dist.HalfNormal(
-                    self.capacity_prior_scale,
-                ),
-                dist.transforms.AffineTransform(loc=self.capacity_prior_loc, scale=1),
-            )
-
-        distributions["std_observation"] = dist.HalfNormal(self.noise_scale)
-
-        def init_trend_params(distributions) -> dict:
-
-            return init_params(distributions)
-
-        return functools.partial(init_trend_params, distributions=distributions)
-
-    def _set_time_scale(self, y: pd.DataFrame):
-        """
-        Sets the scales for the time series data.
-
-        Args:
-            y (pd.DataFrame): Time series data.
-        """
-
-        # Set time scale
-        t_days = convert_index_to_days_since_epoch(y.index)
-
-        self.t_scale = (t_days[1:] - t_days[:-1]).mean()
-        self.t_start = t_days.min() / self.t_scale
-
-    def _index_to_scaled_timearray(self, idx):
-        """
-        Scales the index values.
-
-        Args:
-            idx (pd.Index): Pandas Index object.
-
-        Returns:
-            np.ndarray: Scaled index values.
-        """
-        t_days = convert_index_to_days_since_epoch(idx)
-        return (t_days) / self.t_scale - self.t_start
-
-    def _set_changepoints_t(self, y : pd.DataFrame) -> None:
-        """
-        Sets the array of changepoint times.
-        
-        This function has the colateral effect of setting the attribute `_changepoint_t` in the class.
-
-        Args:
-            y (pd.DataFrame): Time series data.
-        """
-
-        t_scaled = self._index_to_scaled_timearray(y.index)
-
-        self._changepoint_t = get_changepoint_timeindexes(
-            t=t_scaled,
-            changepoint_interval=self.changepoint_interval,
-            changepoint_range=self.changepoint_range,
-        )
-
-    def _get_changepoint_matrix(self, t: jnp.ndarray) -> jnp.ndarray:
-        """
-        Generates the changepoint coefficient matrix.
-
-        Args:
-            t (jnp.ndarray): Array of time values.
-
-        Returns:
-            jnp.ndarray: Changepoint coefficient matrix.
-        """
-
-        return get_changepoint_matrix(t, self._changepoint_t)
-
     def _get_predict_data(
         self, X: pd.DataFrame, fh: ForecastingHorizon
     ) -> dict:
         """
         Prepares the data for making predictions.
 
         Args:
@@ -359,29 +239,25 @@
         Returns:
             dict: Dictionary of data for the Numpyro model.
         """
 
         fh_dates = self.fh_to_index(fh)
         fh_as_index = pd.Index(list(fh_dates.to_numpy()))
 
-        t = self._index_to_scaled_timearray(fh_as_index)
-        changepoint_matrix = self._get_changepoint_matrix(t)
+        trend_data = self.trend_model_.prepare_input_data(fh_as_index)
 
         if X is None:
             X = pd.DataFrame(index=fh_as_index)
 
         if self.feature_transformer is not None:
             X = self.feature_transformer.transform(X)
 
         exogenous_data = (
             self._get_exogenous_data_array(X.loc[fh_as_index]) if self._has_exogenous else None
         )
 
         return dict(
-            t=t.reshape((-1, 1)),
             y=None,
             data=exogenous_data,
-            changepoint_matrix=changepoint_matrix,
+            trend_data=trend_data,
             **self.fit_and_predict_data_,
         )
-
-
```

### Comparing `prophetverse-0.0.3rc1/src/prophetverse/utils/regex.py` & `prophetverse-0.0.4/src/prophetverse/utils/regex.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 
+__all__  = [
+    "starts_with",
+    "exact"
+]
 
 def starts_with(prefixes):
     """
     Returns a regular expression pattern that matches strings starting with any of the given prefixes.
 
     Args:
         prefixes (list): A list of strings representing the prefixes to match.
```

### Comparing `prophetverse-0.0.3rc1/PKG-INFO` & `prophetverse-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prophetverse
-Version: 0.0.3rc1
+Version: 0.0.4
 Summary: 
 Author: Felipe Angelim
 Author-email: felipeangelim@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

