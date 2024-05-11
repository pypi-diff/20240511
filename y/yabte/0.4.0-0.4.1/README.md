# Comparing `tmp/yabte-0.4.0.tar.gz` & `tmp/yabte-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yabte-0.4.0.tar", max compression
+gzip compressed data, was "yabte-0.4.1.tar", max compression
```

## Comparing `yabte-0.4.0.tar` & `yabte-0.4.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1072 2024-03-29 16:22:09.145167 yabte-0.4.0/LICENSE
--rw-r--r--   0        0        0     3306 2024-03-29 16:22:09.145167 yabte-0.4.0/README.md
--rw-r--r--   0        0        0     1344 2024-03-29 16:22:09.153167 yabte-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       30 2024-03-29 16:22:09.157167 yabte-0.4.0/yabte/__init__.py
--rw-r--r--   0        0        0     1191 2024-03-29 16:22:09.157167 yabte-0.4.0/yabte/backtest/__init__.py
--rw-r--r--   0        0        0      722 2024-03-29 16:22:09.157167 yabte-0.4.0/yabte/backtest/_helpers.py
--rw-r--r--   0        0        0     4930 2024-03-29 16:22:09.157167 yabte-0.4.0/yabte/backtest/asset.py
--rw-r--r--   0        0        0     4095 2024-03-29 16:22:09.157167 yabte-0.4.0/yabte/backtest/book.py
--rw-r--r--   0        0        0    14421 2024-03-29 16:22:09.157167 yabte-0.4.0/yabte/backtest/order.py
--rw-r--r--   0        0        0     3568 2024-03-29 16:22:09.157167 yabte-0.4.0/yabte/backtest/strategy.py
--rw-r--r--   0        0        0     7136 2024-03-29 16:22:09.157167 yabte-0.4.0/yabte/backtest/strategyrunner.py
--rw-r--r--   0        0        0     2298 2024-03-29 16:22:09.157167 yabte-0.4.0/yabte/backtest/transaction.py
--rw-r--r--   0        0        0        0 2024-03-29 16:22:09.157167 yabte-0.4.0/yabte/tests/__init__.py
--rw-r--r--   0        0        0      602 2024-03-29 16:22:09.157167 yabte-0.4.0/yabte/tests/_helpers.py
--rw-r--r--   0        0        0     1278 2024-03-29 16:22:09.157167 yabte-0.4.0/yabte/tests/_unittest_numpy_extensions.py
--rw-r--r--   0        0        0   137308 2024-03-29 16:22:09.157167 yabte-0.4.0/yabte/tests/data/nasdaq/AAPL.csv
--rw-r--r--   0        0        0   135665 2024-03-29 16:22:09.157167 yabte-0.4.0/yabte/tests/data/nasdaq/AMZN.csv
--rw-r--r--   0        0        0    90302 2024-03-29 16:22:09.157167 yabte-0.4.0/yabte/tests/data/nasdaq/GOOG.csv
--rw-r--r--   0        0        0   136484 2024-03-29 16:22:09.161167 yabte-0.4.0/yabte/tests/data/nasdaq/INTC.csv
--rw-r--r--   0        0        0   135802 2024-03-29 16:22:09.161167 yabte-0.4.0/yabte/tests/data/nasdaq/META.csv
--rw-r--r--   0        0        0    93835 2024-03-29 16:22:09.161167 yabte-0.4.0/yabte/tests/data/nasdaq/MSFT.csv
--rw-r--r--   0        0        0   130341 2024-03-29 16:22:09.161167 yabte-0.4.0/yabte/tests/data/nasdaq/NFLX.csv
--rw-r--r--   0        0        0   139249 2024-03-29 16:22:09.161167 yabte-0.4.0/yabte/tests/data/nasdaq/TSLA.csv
--rw-r--r--   0        0        0      906 2024-03-29 16:22:09.161167 yabte-0.4.0/yabte/tests/test_notebooks.py
--rw-r--r--   0        0        0     1676 2024-03-29 16:22:09.161167 yabte-0.4.0/yabte/tests/test_portopt.py
--rw-r--r--   0        0        0     4099 2024-03-29 16:22:09.161167 yabte-0.4.0/yabte/tests/test_simulation.py
--rw-r--r--   0        0        0    18863 2024-03-29 16:22:09.161167 yabte-0.4.0/yabte/tests/test_strategy_runner.py
--rw-r--r--   0        0        0     1560 2024-03-29 16:22:09.161167 yabte-0.4.0/yabte/tests/test_utilities.py
--rw-r--r--   0        0        0        0 2024-03-29 16:22:09.161167 yabte-0.4.0/yabte/utilities/__init__.py
--rw-r--r--   0        0        0     1179 2024-03-29 16:22:09.161167 yabte-0.4.0/yabte/utilities/lagrangian.py
--rw-r--r--   0        0        0     2369 2024-03-29 16:22:09.161167 yabte-0.4.0/yabte/utilities/pandas_extension.py
--rw-r--r--   0        0        0        0 2024-03-29 16:22:09.161167 yabte-0.4.0/yabte/utilities/plot/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 16:22:09.161167 yabte-0.4.0/yabte/utilities/plot/matplotlib/__init__.py
--rw-r--r--   0        0        0     3360 2024-03-29 16:22:09.161167 yabte-0.4.0/yabte/utilities/plot/matplotlib/marker_updater.py
--rw-r--r--   0        0        0     5594 2024-03-29 16:22:09.161167 yabte-0.4.0/yabte/utilities/plot/matplotlib/strategy_runner.py
--rw-r--r--   0        0        0        0 2024-03-29 16:22:09.161167 yabte-0.4.0/yabte/utilities/plot/plotly/__init__.py
--rw-r--r--   0        0        0     5703 2024-03-29 16:22:09.161167 yabte-0.4.0/yabte/utilities/plot/plotly/strategy_runner.py
--rw-r--r--   0        0        0        0 2024-03-29 16:22:09.161167 yabte-0.4.0/yabte/utilities/portopt/__init__.py
--rw-r--r--   0        0        0     2334 2024-03-29 16:22:09.161167 yabte-0.4.0/yabte/utilities/portopt/hierarchical_risk_parity.py
--rw-r--r--   0        0        0      396 2024-03-29 16:22:09.161167 yabte-0.4.0/yabte/utilities/portopt/inverse_volatility.py
--rw-r--r--   0        0        0     1973 2024-03-29 16:22:09.161167 yabte-0.4.0/yabte/utilities/portopt/minimum_variance.py
--rw-r--r--   0        0        0        0 2024-03-29 16:22:09.165167 yabte-0.4.0/yabte/utilities/simulation/__init__.py
--rw-r--r--   0        0        0     1475 2024-03-29 16:22:09.165167 yabte-0.4.0/yabte/utilities/simulation/geometric_brownian_motion.py
--rw-r--r--   0        0        0     2098 2024-03-29 16:22:09.165167 yabte-0.4.0/yabte/utilities/simulation/heston.py
--rw-r--r--   0        0        0     1102 2024-03-29 16:22:09.165167 yabte-0.4.0/yabte/utilities/simulation/weiner.py
--rw-r--r--   0        0        0      441 2024-03-29 16:22:09.165167 yabte-0.4.0/yabte/utilities/strategy_helpers.py
--rw-r--r--   0        0        0     4385 1970-01-01 00:00:00.000000 yabte-0.4.0/setup.py
--rw-r--r--   0        0        0     3995 1970-01-01 00:00:00.000000 yabte-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-11 20:01:24.824070 yabte-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3558 2024-05-11 20:01:24.824070 yabte-0.4.1/README.md
+-rw-r--r--   0        0        0     1375 2024-05-11 20:01:24.832070 yabte-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      106 2024-05-11 20:01:24.836070 yabte-0.4.1/yabte/__init__.py
+-rw-r--r--   0        0        0     1191 2024-05-11 20:01:24.836070 yabte-0.4.1/yabte/backtest/__init__.py
+-rw-r--r--   0        0        0      722 2024-05-11 20:01:24.836070 yabte-0.4.1/yabte/backtest/_helpers.py
+-rw-r--r--   0        0        0     4930 2024-05-11 20:01:24.836070 yabte-0.4.1/yabte/backtest/asset.py
+-rw-r--r--   0        0        0     4095 2024-05-11 20:01:24.836070 yabte-0.4.1/yabte/backtest/book.py
+-rw-r--r--   0        0        0    14421 2024-05-11 20:01:24.836070 yabte-0.4.1/yabte/backtest/order.py
+-rw-r--r--   0        0        0     3568 2024-05-11 20:01:24.836070 yabte-0.4.1/yabte/backtest/strategy.py
+-rw-r--r--   0        0        0     7609 2024-05-11 20:01:24.836070 yabte-0.4.1/yabte/backtest/strategyrunner.py
+-rw-r--r--   0        0        0     2298 2024-05-11 20:01:24.836070 yabte-0.4.1/yabte/backtest/transaction.py
+-rw-r--r--   0        0        0        0 2024-05-11 20:01:24.836070 yabte-0.4.1/yabte/tests/__init__.py
+-rw-r--r--   0        0        0      602 2024-05-11 20:01:24.836070 yabte-0.4.1/yabte/tests/_helpers.py
+-rw-r--r--   0        0        0     1278 2024-05-11 20:01:24.836070 yabte-0.4.1/yabte/tests/_unittest_numpy_extensions.py
+-rw-r--r--   0        0        0   137308 2024-05-11 20:01:24.836070 yabte-0.4.1/yabte/tests/data/nasdaq/AAPL.csv
+-rw-r--r--   0        0        0   135665 2024-05-11 20:01:24.836070 yabte-0.4.1/yabte/tests/data/nasdaq/AMZN.csv
+-rw-r--r--   0        0        0    90302 2024-05-11 20:01:24.836070 yabte-0.4.1/yabte/tests/data/nasdaq/GOOG.csv
+-rw-r--r--   0        0        0   136484 2024-05-11 20:01:24.836070 yabte-0.4.1/yabte/tests/data/nasdaq/INTC.csv
+-rw-r--r--   0        0        0   135802 2024-05-11 20:01:24.840070 yabte-0.4.1/yabte/tests/data/nasdaq/META.csv
+-rw-r--r--   0        0        0    93835 2024-05-11 20:01:24.840070 yabte-0.4.1/yabte/tests/data/nasdaq/MSFT.csv
+-rw-r--r--   0        0        0   130341 2024-05-11 20:01:24.840070 yabte-0.4.1/yabte/tests/data/nasdaq/NFLX.csv
+-rw-r--r--   0        0        0   139249 2024-05-11 20:01:24.840070 yabte-0.4.1/yabte/tests/data/nasdaq/TSLA.csv
+-rw-r--r--   0        0        0      906 2024-05-11 20:01:24.840070 yabte-0.4.1/yabte/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1676 2024-05-11 20:01:24.840070 yabte-0.4.1/yabte/tests/test_portopt.py
+-rw-r--r--   0        0        0     4099 2024-05-11 20:01:24.840070 yabte-0.4.1/yabte/tests/test_simulation.py
+-rw-r--r--   0        0        0    19681 2024-05-11 20:01:24.840070 yabte-0.4.1/yabte/tests/test_strategy_runner.py
+-rw-r--r--   0        0        0     1560 2024-05-11 20:01:24.840070 yabte-0.4.1/yabte/tests/test_utilities.py
+-rw-r--r--   0        0        0        0 2024-05-11 20:01:24.840070 yabte-0.4.1/yabte/utilities/__init__.py
+-rw-r--r--   0        0        0     1179 2024-05-11 20:01:24.840070 yabte-0.4.1/yabte/utilities/lagrangian.py
+-rw-r--r--   0        0        0     2743 2024-05-11 20:01:24.840070 yabte-0.4.1/yabte/utilities/pandas_extension.py
+-rw-r--r--   0        0        0        0 2024-05-11 20:01:24.840070 yabte-0.4.1/yabte/utilities/plot/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-11 20:01:24.840070 yabte-0.4.1/yabte/utilities/plot/matplotlib/__init__.py
+-rw-r--r--   0        0        0     3360 2024-05-11 20:01:24.840070 yabte-0.4.1/yabte/utilities/plot/matplotlib/marker_updater.py
+-rw-r--r--   0        0        0     5594 2024-05-11 20:01:24.840070 yabte-0.4.1/yabte/utilities/plot/matplotlib/strategy_runner.py
+-rw-r--r--   0        0        0        0 2024-05-11 20:01:24.840070 yabte-0.4.1/yabte/utilities/plot/plotly/__init__.py
+-rw-r--r--   0        0        0     5703 2024-05-11 20:01:24.840070 yabte-0.4.1/yabte/utilities/plot/plotly/strategy_runner.py
+-rw-r--r--   0        0        0        0 2024-05-11 20:01:24.840070 yabte-0.4.1/yabte/utilities/portopt/__init__.py
+-rw-r--r--   0        0        0     2334 2024-05-11 20:01:24.840070 yabte-0.4.1/yabte/utilities/portopt/hierarchical_risk_parity.py
+-rw-r--r--   0        0        0      396 2024-05-11 20:01:24.840070 yabte-0.4.1/yabte/utilities/portopt/inverse_volatility.py
+-rw-r--r--   0        0        0     1973 2024-05-11 20:01:24.840070 yabte-0.4.1/yabte/utilities/portopt/minimum_variance.py
+-rw-r--r--   0        0        0        0 2024-05-11 20:01:24.840070 yabte-0.4.1/yabte/utilities/simulation/__init__.py
+-rw-r--r--   0        0        0     1475 2024-05-11 20:01:24.840070 yabte-0.4.1/yabte/utilities/simulation/geometric_brownian_motion.py
+-rw-r--r--   0        0        0     2098 2024-05-11 20:01:24.840070 yabte-0.4.1/yabte/utilities/simulation/heston.py
+-rw-r--r--   0        0        0     1246 2024-05-11 20:01:24.840070 yabte-0.4.1/yabte/utilities/simulation/weiner.py
+-rw-r--r--   0        0        0      441 2024-05-11 20:01:24.840070 yabte-0.4.1/yabte/utilities/strategy_helpers.py
+-rw-r--r--   0        0        0     4649 1970-01-01 00:00:00.000000 yabte-0.4.1/setup.py
+-rw-r--r--   0        0        0     4254 1970-01-01 00:00:00.000000 yabte-0.4.1/PKG-INFO
```

### Comparing `yabte-0.4.0/LICENSE` & `yabte-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yabte-0.4.0/README.md` & `yabte-0.4.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 # yabte - Yet Another BackTesting Engine
 
 Python module for backtesting trading strategies.
 
-Support event driven backtesting, ie `on_open`, `on_close`, etc. Also supports multiple assets.
+Features
 
-Very basic statistics like book cash, mtm and total value. Currently, everything else needs to be deferred to a 3rd party module like `empyrical`.
+* Event driven, ie `on_open`, `on_close`, etc. 
+* Multiple assets.
+* OHLC Asset. Extendable (e.g support additional fields, e.g. Volatility, or entirely different fields, e.g. Barrels per day).
+* Multiple books.
+* Positional and Basket orders. Extendible (e.g. can support stop loss).
+* Batch runs (for optimization).
+* Captures book history including transactions & daily cash, MtM and total values.
 
-There are some basic tests but use at your own peril. It's not production level code.
+The module provides basic statistics like book cash, mtm and total value. Currently, everything else needs to be deferred to a 3rd party module like `empyrical`.
 
 ## Core dependencies
 
 The core module uses pandas and scipy.
 
 ## Installation
 
 ```bash
 pip install yatbe
 ```
 
 ## Usage
 
-Below is an example usage (the performance of the example strategy won't be good).
+Below is an example usage (the economic performance of the example strategy won't be good).
 
 ```python
 import pandas as pd
 
 from yabte.backtest import Book, SimpleOrder, Strategy, StrategyRunner
 from yabte.tests._helpers import generate_nasdaq_dataset
 from yabte.utilities.plot.plotly.strategy_runner import plot_strategy_runner_result
```

### Comparing `yabte-0.4.0/pyproject.toml` & `yabte-0.4.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "yabte"
-version = "0.4.0"
+version = "0.4.1"
 description = "Yet another backtesting engine"
 authors = ["Blair Azzopardi <blairuk@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bsdz/yabte"
 
 [tool.poetry.build]
-script = "build.py"
+script = "build_mypyc.py"
 generate-setup-file = true
 
 [tool.poetry.dependencies]
 python = "^3.10,<3.13"
-pandas = ">1.5,<3"
+pandas = "^2.2.1"
 scipy = "^1.10.0"
 pandas-stubs = "^2.1.4.231227"
 mypy = "^1.8.0"
 
 [tool.poetry.group.dev]
 optional = true
 
@@ -42,19 +42,20 @@
 [tool.poetry.group.notebooks]
 optional = true
 
 [tool.poetry.group.notebooks.dependencies]
 matplotlib = "^3.6.2"
 plotly = "^5.10.0"
 ipykernel = "^6.20.2"
-pyfeng = "^0.2.5"
 nbconvert = "^7.2.9"
+quantlib = "^1.34"
 
 [tool.isort]
 profile = "black"
+skip_glob = [".venv*/*"]
 
 [[tool.mypy.overrides]]
 module = "plotly.*,scipy.*,matplotlib.*"
 ignore_missing_imports = true
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "setuptools==69.0.2", "mypy==1.8.0", "pandas-stubs==2.1.4.231227"]
```

### Comparing `yabte-0.4.0/yabte/backtest/__init__.py` & `yabte-0.4.1/yabte/backtest/__init__.py`

 * *Files identical despite different names*

### Comparing `yabte-0.4.0/yabte/backtest/_helpers.py` & `yabte-0.4.1/yabte/backtest/_helpers.py`

 * *Files identical despite different names*

### Comparing `yabte-0.4.0/yabte/backtest/asset.py` & `yabte-0.4.1/yabte/backtest/asset.py`

 * *Files identical despite different names*

### Comparing `yabte-0.4.0/yabte/backtest/book.py` & `yabte-0.4.1/yabte/backtest/book.py`

 * *Files identical despite different names*

### Comparing `yabte-0.4.0/yabte/backtest/order.py` & `yabte-0.4.1/yabte/backtest/order.py`

 * *Files identical despite different names*

### Comparing `yabte-0.4.0/yabte/backtest/strategy.py` & `yabte-0.4.1/yabte/backtest/strategy.py`

 * *Files identical despite different names*

### Comparing `yabte-0.4.0/yabte/backtest/strategyrunner.py` & `yabte-0.4.1/yabte/backtest/strategyrunner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import concurrent.futures
 import logging
+from concurrent.futures import ProcessPoolExecutor
 from copy import deepcopy
 from dataclasses import dataclass, field
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, Iterable, List, Optional
 
 import pandas as pd
 
 # TODO: use explicit imports until mypyc fixes attribute lookups in dataclass
 # (https://github.com/mypyc/mypyc/issues/1000)
 from pandas import DataFrame, Series, Timestamp  # type: ignore
 
@@ -215,7 +217,18 @@
                 strat.on_close()
 
             # run book end-of-day tasks
             for book in srr.books:
                 book.eod_tasks(ts, day_data, asset_map)
 
         return srr
+
+    def run_batch(
+        self,
+        params_iterable: Iterable[Dict[str, Any]],
+        executor: ProcessPoolExecutor | None = None,
+    ) -> List[StrategyRunnerResult]:
+        """Run a set of parameter combinations."""
+
+        executor = executor or concurrent.futures.ThreadPoolExecutor()
+        with executor:
+            return list(executor.map(self.run, params_iterable))
```

### Comparing `yabte-0.4.0/yabte/backtest/transaction.py` & `yabte-0.4.1/yabte/backtest/transaction.py`

 * *Files identical despite different names*

### Comparing `yabte-0.4.0/yabte/tests/_helpers.py` & `yabte-0.4.1/yabte/tests/_helpers.py`

 * *Files identical despite different names*

### Comparing `yabte-0.4.0/yabte/tests/_unittest_numpy_extensions.py` & `yabte-0.4.1/yabte/tests/_unittest_numpy_extensions.py`

 * *Files identical despite different names*

### Comparing `yabte-0.4.0/yabte/tests/data/nasdaq/AAPL.csv` & `yabte-0.4.1/yabte/tests/data/nasdaq/AAPL.csv`

 * *Files identical despite different names*

### Comparing `yabte-0.4.0/yabte/tests/data/nasdaq/AMZN.csv` & `yabte-0.4.1/yabte/tests/data/nasdaq/AMZN.csv`

 * *Files identical despite different names*

### Comparing `yabte-0.4.0/yabte/tests/data/nasdaq/GOOG.csv` & `yabte-0.4.1/yabte/tests/data/nasdaq/GOOG.csv`

 * *Files identical despite different names*

### Comparing `yabte-0.4.0/yabte/tests/data/nasdaq/INTC.csv` & `yabte-0.4.1/yabte/tests/data/nasdaq/INTC.csv`

 * *Files identical despite different names*

### Comparing `yabte-0.4.0/yabte/tests/data/nasdaq/META.csv` & `yabte-0.4.1/yabte/tests/data/nasdaq/META.csv`

 * *Files identical despite different names*

### Comparing `yabte-0.4.0/yabte/tests/data/nasdaq/MSFT.csv` & `yabte-0.4.1/yabte/tests/data/nasdaq/MSFT.csv`

 * *Files identical despite different names*

### Comparing `yabte-0.4.0/yabte/tests/data/nasdaq/NFLX.csv` & `yabte-0.4.1/yabte/tests/data/nasdaq/NFLX.csv`

 * *Files identical despite different names*

### Comparing `yabte-0.4.0/yabte/tests/data/nasdaq/TSLA.csv` & `yabte-0.4.1/yabte/tests/data/nasdaq/TSLA.csv`

 * *Files identical despite different names*

### Comparing `yabte-0.4.0/yabte/tests/test_notebooks.py` & `yabte-0.4.1/yabte/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `yabte-0.4.0/yabte/tests/test_portopt.py` & `yabte-0.4.1/yabte/tests/test_portopt.py`

 * *Files identical despite different names*

### Comparing `yabte-0.4.0/yabte/tests/test_simulation.py` & `yabte-0.4.1/yabte/tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `yabte-0.4.0/yabte/tests/test_strategy_runner.py` & `yabte-0.4.1/yabte/tests/test_strategy_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import unittest
 from decimal import Decimal
 
 import numpy as np
 import pandas as pd
 
+import yabte.utilities.pandas_extension
 from yabte.backtest import (
     BasketOrder,
     Book,
     OHLCAsset,
     OrderSizeType,
     OrderStatus,
     PositionalBasketOrder,
@@ -567,10 +568,37 @@
             [
                 (OrderStatus.OPEN, None, Decimal("200")),
                 (OrderStatus.OPEN, "my_key", Decimal("300")),
             ],
             [(o.status, o.key, o.size) for o in srr.orders_unprocessed],
         )
 
+    def test_run_batch(self):
+        book = Book(name="Main", cash=Decimal("100000"))
+
+        sr = StrategyRunner(
+            data=self.df_combined,
+            assets=self.assets,
+            strategies=[TestSMAXOStrat()],
+            books=[book],
+        )
+
+        param_iter = [
+            {"days_long": n, "days_short": m}
+            for n, m in zip([20, 30, 40, 50], [5, 10, 15, 20])
+            if n > m
+        ]
+
+        srrs = sr.run_batch(param_iter)
+
+        self.assertEqual(len(srrs), len(param_iter))
+
+        # check we have distinct sharpe ratios for each param set
+        sharpes = {
+            srr.book_history.loc[:, ("Main", "total")].prc.sharpe_ratio()
+            for srr in srrs
+        }
+        self.assertEqual(len(sharpes), len(param_iter))
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `yabte-0.4.0/yabte/tests/test_utilities.py` & `yabte-0.4.1/yabte/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `yabte-0.4.0/yabte/utilities/lagrangian.py` & `yabte-0.4.1/yabte/utilities/lagrangian.py`

 * *Files identical despite different names*

### Comparing `yabte-0.4.0/yabte/utilities/pandas_extension.py` & `yabte-0.4.1/yabte/utilities/pandas_extension.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,57 +9,65 @@
 
     @property
     def standard(self):
         return (self._obj - self._obj.mean()) / self._obj.std()
 
 
 @pd.api.extensions.register_dataframe_accessor("prc")
+@pd.api.extensions.register_series_accessor("prc")
 class PriceAccessor:
     # TODO: add ledoit cov (via sklearn)
     # http://www.ledoit.net/honey.pdf
-    # TODO: add Sharpe ratio
 
     def __init__(self, pandas_obj):
         self._validate(pandas_obj)
         self._obj = pandas_obj
 
     @staticmethod
     def _validate(obj):
-        if (obj < 0).any(axis=None):
-            raise AttributeError("Prices must be non-negative")
+        pass
 
     @property
     def log_returns(self):
+        if (self._obj < 0).any(axis=None):
+            raise AttributeError("Prices must be non-negative for log returns")
         return np.log((self._obj / self._obj.shift())[1:])
 
     @property
     def returns(self):
         return self._obj.pct_change(fill_method=None)[1:]
 
     @property
     def frequency(self):
         days = pd.Timedelta(np.diff(self._obj.index).min()).days
         if days == 1:
             return 252
         elif days == 7:
             return 52
+        elif 28 <= days <= 31:
+            return 12
 
     def capm_returns(self, risk_free_rate=0):
         returns = self.returns
         returns_mkt = returns.mean(axis=1).rename("MKT")
 
         # concat market retutns & compute sampel covariance matrix
         cov = pd.concat([returns, returns_mkt], axis=1).cov()
         betas = cov.MKT.drop("MKT") / cov.MKT.MKT
 
         return (
             risk_free_rate
             + betas * (returns_mkt.mean() * self.frequency - risk_free_rate)
         ).rename("CAPM")
 
+    def sharpe_ratio(self, risk_free_rate=0, use_log_returns=True):
+        ann_factor = np.sqrt(self.frequency)
+        returns = self.log_returns if use_log_returns else self.returns
+        return ann_factor * (returns.mean() - risk_free_rate) / returns.std()
+
     def null_blips(self, sd=5, sdd=7):
         df = self._obj
         z = df.scl.standard
         zd = z.diff()
         # TODO support blips longer than 1 day?
         for col, series in df[z.abs() > sd].dropna(how="all").dropna(axis=1).items():
             for row, val in series.items():
```

### Comparing `yabte-0.4.0/yabte/utilities/plot/matplotlib/marker_updater.py` & `yabte-0.4.1/yabte/utilities/plot/matplotlib/marker_updater.py`

 * *Files identical despite different names*

### Comparing `yabte-0.4.0/yabte/utilities/plot/matplotlib/strategy_runner.py` & `yabte-0.4.1/yabte/utilities/plot/matplotlib/strategy_runner.py`

 * *Files identical despite different names*

### Comparing `yabte-0.4.0/yabte/utilities/plot/plotly/strategy_runner.py` & `yabte-0.4.1/yabte/utilities/plot/plotly/strategy_runner.py`

 * *Files identical despite different names*

### Comparing `yabte-0.4.0/yabte/utilities/portopt/hierarchical_risk_parity.py` & `yabte-0.4.1/yabte/utilities/portopt/hierarchical_risk_parity.py`

 * *Files identical despite different names*

### Comparing `yabte-0.4.0/yabte/utilities/portopt/minimum_variance.py` & `yabte-0.4.1/yabte/utilities/portopt/minimum_variance.py`

 * *Files identical despite different names*

### Comparing `yabte-0.4.0/yabte/utilities/simulation/geometric_brownian_motion.py` & `yabte-0.4.1/yabte/utilities/simulation/geometric_brownian_motion.py`

 * *Files identical despite different names*

### Comparing `yabte-0.4.0/yabte/utilities/simulation/heston.py` & `yabte-0.4.1/yabte/utilities/simulation/heston.py`

 * *Files identical despite different names*

### Comparing `yabte-0.4.0/yabte/utilities/simulation/weiner.py` & `yabte-0.4.1/yabte/utilities/simulation/weiner.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,26 +10,28 @@
 
 import numpy as np
 
 
 def weiner_simulate_paths(
     n_steps: int,
     n_sims: int = 1,
-    stdev: float = 1,
+    stdev: float | np.ndarray = 1,
     R: np.ndarray = np.array([[1]]),
     rng=None,
 ):
     """Generate simulated Weiner paths.
 
     `stdev` is the increment size, `R` a correlation matrix, `n_steps`
     is how many time steps, `n_sims` the number of simulations and `rng`
-    a numpy random number generator (optional).
+    a numpy random number generator (optional). If `stdev` is a scalar
+    it will be broadcasted to the size of `n_sims`.
     """
 
     R = np.atleast_2d(R)
+    stdev = np.resize(stdev, n_sims).reshape(n_sims, 1)
 
     if rng is None:
         rng = np.random.default_rng()
 
     k = R.shape[0]
 
     # simulate 'n_sims' price paths of `k` sized asset groups with 'n_steps' timesteps
```

### Comparing `yabte-0.4.0/setup.py` & `yabte-0.4.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 
 package_data = \
 {'': ['*'], 'yabte.tests': ['data/nasdaq/*']}
 
 install_requires = \
 ['mypy>=1.8.0,<2.0.0',
  'pandas-stubs>=2.1.4.231227,<3.0.0.0',
- 'pandas>1.5,<3',
+ 'pandas>=2.2.1,<3.0.0',
  'scipy>=1.10.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'yabte',
-    'version': '0.4.0',
+    'version': '0.4.1',
     'description': 'Yet another backtesting engine',
-    'long_description': '# yabte - Yet Another BackTesting Engine\n\nPython module for backtesting trading strategies.\n\nSupport event driven backtesting, ie `on_open`, `on_close`, etc. Also supports multiple assets.\n\nVery basic statistics like book cash, mtm and total value. Currently, everything else needs to be deferred to a 3rd party module like `empyrical`.\n\nThere are some basic tests but use at your own peril. It\'s not production level code.\n\n## Core dependencies\n\nThe core module uses pandas and scipy.\n\n## Installation\n\n```bash\npip install yatbe\n```\n\n## Usage\n\nBelow is an example usage (the performance of the example strategy won\'t be good).\n\n```python\nimport pandas as pd\n\nfrom yabte.backtest import Book, SimpleOrder, Strategy, StrategyRunner\nfrom yabte.tests._helpers import generate_nasdaq_dataset\nfrom yabte.utilities.plot.plotly.strategy_runner import plot_strategy_runner_result\nfrom yabte.utilities.strategy_helpers import crossover\n\n\nclass SMAXO(Strategy):\n    def init(self):\n        # enhance data with simple moving averages\n\n        p = self.params\n        days_short = p.get("days_short", 10)\n        days_long = p.get("days_long", 20)\n\n        close_sma_short = (\n            self.data.loc[:, (slice(None), "Close")]\n            .rolling(days_short)\n            .mean()\n            .rename({"Close": "CloseSMAShort"}, axis=1, level=1)\n        )\n        close_sma_long = (\n            self.data.loc[:, (slice(None), "Close")]\n            .rolling(days_long)\n            .mean()\n            .rename({"Close": "CloseSMALong"}, axis=1, level=1)\n        )\n        self.data = pd.concat(\n            [self.data, close_sma_short, close_sma_long], axis=1\n        ).sort_index(axis=1)\n\n    def on_close(self):\n        # create some orders\n\n        for symbol in ["GOOG", "MSFT"]:\n            df = self.data[symbol]\n            ix_2d = df.index[-2:]\n            data = df.loc[ix_2d, ("CloseSMAShort", "CloseSMALong")].dropna()\n            if len(data) == 2:\n                if crossover(data.CloseSMAShort, data.CloseSMALong):\n                    self.orders.append(SimpleOrder(asset_name=symbol, size=-100))\n                elif crossover(data.CloseSMALong, data.CloseSMAShort):\n                    self.orders.append(SimpleOrder(asset_name=symbol, size=100))\n\n\n# load some data\nassets, df_combined = generate_nasdaq_dataset()\n\n# create a book with 100000 cash\nbook = Book(name="Main", cash="100000")\n\n# run our strategy\nsr = StrategyRunner(\n    data=df_combined,\n    assets=assets,\n    strategies=[SMAXO()],\n    books=[book],\n)\nsrr = sr.run()\n\n# see the trades or book history\nth = srr.transaction_history\nbch = srr.book_history.loc[:, (slice(None), "cash")]\n\n# plot the trades against book value\nplot_strategy_runner_result(srr, sr)\n```\n\n![Output from code](https://raw.githubusercontent.com/bsdz/yabte/main/readme_image.png)\n\n## Examples\n\nJupyter notebook examples can be found under the [notebooks folder](https://github.com/bsdz/yabte/tree/main/notebooks).\n\n## Documentation\n\nDocumentation can be found on [Read the Docs](https://yabte.readthedocs.io/en/latest/).\n\n\n## Development\n\nBefore commit run following format commands in project folder:\n\n```bash\npoetry run black .\npoetry run isort . --profile black\npoetry run docformatter . --recursive --in-place --black --exclude _unittest_numpy_extensions.py\n```\n',
+    'long_description': '# yabte - Yet Another BackTesting Engine\n\nPython module for backtesting trading strategies.\n\nFeatures\n\n* Event driven, ie `on_open`, `on_close`, etc. \n* Multiple assets.\n* OHLC Asset. Extendable (e.g support additional fields, e.g. Volatility, or entirely different fields, e.g. Barrels per day).\n* Multiple books.\n* Positional and Basket orders. Extendible (e.g. can support stop loss).\n* Batch runs (for optimization).\n* Captures book history including transactions & daily cash, MtM and total values.\n\nThe module provides basic statistics like book cash, mtm and total value. Currently, everything else needs to be deferred to a 3rd party module like `empyrical`.\n\n## Core dependencies\n\nThe core module uses pandas and scipy.\n\n## Installation\n\n```bash\npip install yatbe\n```\n\n## Usage\n\nBelow is an example usage (the economic performance of the example strategy won\'t be good).\n\n```python\nimport pandas as pd\n\nfrom yabte.backtest import Book, SimpleOrder, Strategy, StrategyRunner\nfrom yabte.tests._helpers import generate_nasdaq_dataset\nfrom yabte.utilities.plot.plotly.strategy_runner import plot_strategy_runner_result\nfrom yabte.utilities.strategy_helpers import crossover\n\n\nclass SMAXO(Strategy):\n    def init(self):\n        # enhance data with simple moving averages\n\n        p = self.params\n        days_short = p.get("days_short", 10)\n        days_long = p.get("days_long", 20)\n\n        close_sma_short = (\n            self.data.loc[:, (slice(None), "Close")]\n            .rolling(days_short)\n            .mean()\n            .rename({"Close": "CloseSMAShort"}, axis=1, level=1)\n        )\n        close_sma_long = (\n            self.data.loc[:, (slice(None), "Close")]\n            .rolling(days_long)\n            .mean()\n            .rename({"Close": "CloseSMALong"}, axis=1, level=1)\n        )\n        self.data = pd.concat(\n            [self.data, close_sma_short, close_sma_long], axis=1\n        ).sort_index(axis=1)\n\n    def on_close(self):\n        # create some orders\n\n        for symbol in ["GOOG", "MSFT"]:\n            df = self.data[symbol]\n            ix_2d = df.index[-2:]\n            data = df.loc[ix_2d, ("CloseSMAShort", "CloseSMALong")].dropna()\n            if len(data) == 2:\n                if crossover(data.CloseSMAShort, data.CloseSMALong):\n                    self.orders.append(SimpleOrder(asset_name=symbol, size=-100))\n                elif crossover(data.CloseSMALong, data.CloseSMAShort):\n                    self.orders.append(SimpleOrder(asset_name=symbol, size=100))\n\n\n# load some data\nassets, df_combined = generate_nasdaq_dataset()\n\n# create a book with 100000 cash\nbook = Book(name="Main", cash="100000")\n\n# run our strategy\nsr = StrategyRunner(\n    data=df_combined,\n    assets=assets,\n    strategies=[SMAXO()],\n    books=[book],\n)\nsrr = sr.run()\n\n# see the trades or book history\nth = srr.transaction_history\nbch = srr.book_history.loc[:, (slice(None), "cash")]\n\n# plot the trades against book value\nplot_strategy_runner_result(srr, sr)\n```\n\n![Output from code](https://raw.githubusercontent.com/bsdz/yabte/main/readme_image.png)\n\n## Examples\n\nJupyter notebook examples can be found under the [notebooks folder](https://github.com/bsdz/yabte/tree/main/notebooks).\n\n## Documentation\n\nDocumentation can be found on [Read the Docs](https://yabte.readthedocs.io/en/latest/).\n\n\n## Development\n\nBefore commit run following format commands in project folder:\n\n```bash\npoetry run black .\npoetry run isort . --profile black\npoetry run docformatter . --recursive --in-place --black --exclude _unittest_numpy_extensions.py\n```\n',
     'author': 'Blair Azzopardi',
     'author_email': 'blairuk@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bsdz/yabte',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `yabte-0.4.0/PKG-INFO` & `yabte-0.4.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,56 @@
 Metadata-Version: 2.1
 Name: yabte
-Version: 0.4.0
+Version: 0.4.1
 Summary: Yet another backtesting engine
 Home-page: https://github.com/bsdz/yabte
 License: MIT
 Author: Blair Azzopardi
 Author-email: blairuk@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: mypy (>=1.8.0,<2.0.0)
-Requires-Dist: pandas (>1.5,<3)
+Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Requires-Dist: pandas-stubs (>=2.1.4.231227,<3.0.0.0)
 Requires-Dist: scipy (>=1.10.0,<2.0.0)
 Project-URL: Repository, https://github.com/bsdz/yabte
 Description-Content-Type: text/markdown
 
 # yabte - Yet Another BackTesting Engine
 
 Python module for backtesting trading strategies.
 
-Support event driven backtesting, ie `on_open`, `on_close`, etc. Also supports multiple assets.
+Features
 
-Very basic statistics like book cash, mtm and total value. Currently, everything else needs to be deferred to a 3rd party module like `empyrical`.
+* Event driven, ie `on_open`, `on_close`, etc. 
+* Multiple assets.
+* OHLC Asset. Extendable (e.g support additional fields, e.g. Volatility, or entirely different fields, e.g. Barrels per day).
+* Multiple books.
+* Positional and Basket orders. Extendible (e.g. can support stop loss).
+* Batch runs (for optimization).
+* Captures book history including transactions & daily cash, MtM and total values.
 
-There are some basic tests but use at your own peril. It's not production level code.
+The module provides basic statistics like book cash, mtm and total value. Currently, everything else needs to be deferred to a 3rd party module like `empyrical`.
 
 ## Core dependencies
 
 The core module uses pandas and scipy.
 
 ## Installation
 
 ```bash
 pip install yatbe
 ```
 
 ## Usage
 
-Below is an example usage (the performance of the example strategy won't be good).
+Below is an example usage (the economic performance of the example strategy won't be good).
 
 ```python
 import pandas as pd
 
 from yabte.backtest import Book, SimpleOrder, Strategy, StrategyRunner
 from yabte.tests._helpers import generate_nasdaq_dataset
 from yabte.utilities.plot.plotly.strategy_runner import plot_strategy_runner_result
```

