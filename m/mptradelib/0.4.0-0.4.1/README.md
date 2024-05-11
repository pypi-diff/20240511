# Comparing `tmp/mptradelib-0.4.0.tar.gz` & `tmp/mptradelib-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mptradelib-0.4.0.tar", max compression
+gzip compressed data, was "mptradelib-0.4.1.tar", max compression
```

## Comparing `mptradelib-0.4.0.tar` & `mptradelib-0.4.1.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-r--r--   0        0        0     3137 2024-05-03 13:20:41.913077 mptradelib-0.4.0/README.md
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.4.0/mptradelib/__init__.py
--rw-r--r--   0        0        0     4685 2024-05-09 18:07:27.997364 mptradelib-0.4.0/mptradelib/backtest.py
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.4.0/mptradelib/broker/__init__.py
--rw-r--r--   0        0        0    11073 2024-05-09 18:27:16.773912 mptradelib-0.4.0/mptradelib/broker/broker.py
--rw-r--r--   0        0        0     5808 2024-05-09 18:04:15.841857 mptradelib-0.4.0/mptradelib/broker/session.py
--rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.4.0/mptradelib/broker/shoonya.py
--rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.4.0/mptradelib/broker/ticker.py
--rw-r--r--   0        0        0        0 2024-05-03 11:19:20.268249 mptradelib-0.4.0/mptradelib/cli/__init__.py
--rw-r--r--   0        0        0     2342 2024-05-09 18:05:58.447254 mptradelib-0.4.0/mptradelib/cli/new.py
--rw-r--r--   0        0        0      953 2024-05-09 18:11:12.323673 mptradelib-0.4.0/mptradelib/cli/templates/strategy/__init__.py.jinja
--rw-r--r--   0        0        0     2984 2024-05-04 12:28:56.516490 mptradelib-0.4.0/mptradelib/cli/templates/strategy/backtest.ipynb.jinja
--rw-r--r--   0        0        0      614 2024-05-03 12:29:43.201283 mptradelib-0.4.0/mptradelib/cli/templates/strategy/livetrade.py.jinja
--rw-r--r--   0        0        0     5394 2024-05-09 18:03:46.504439 mptradelib-0.4.0/mptradelib/feed.py
--rw-r--r--   0        0        0     2007 2024-05-09 18:25:26.040938 mptradelib-0.4.0/mptradelib/livetrade.py
--rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.4.0/mptradelib/test_renko.py
--rw-r--r--   0        0        0       77 2024-05-06 16:16:12.200968 mptradelib-0.4.0/mptradelib/utils/__init__.py
--rw-r--r--   0        0        0      902 2024-05-06 16:14:19.221626 mptradelib-0.4.0/mptradelib/utils/simulated_trades.py
--rw-r--r--   0        0        0     5502 2024-05-06 16:15:40.095142 mptradelib-0.4.0/mptradelib/utils/tearsheet.py
--rw-r--r--   0        0        0      910 2024-05-06 16:15:09.786235 mptradelib-0.4.0/mptradelib/utils/utils.py
--rw-r--r--   0        0        0      829 2024-05-09 18:31:59.599239 mptradelib-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4003 1970-01-01 00:00:00.000000 mptradelib-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     3137 2024-05-03 13:20:41.913077 mptradelib-0.4.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.4.1/mptradelib/__init__.py
+-rw-r--r--   0        0        0     4662 2024-05-10 19:46:01.019193 mptradelib-0.4.1/mptradelib/backtest.py
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.4.1/mptradelib/broker/__init__.py
+-rw-r--r--   0        0        0    11073 2024-05-09 18:27:16.773912 mptradelib-0.4.1/mptradelib/broker/broker.py
+-rw-r--r--   0        0        0     5808 2024-05-09 18:04:15.841857 mptradelib-0.4.1/mptradelib/broker/session.py
+-rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.4.1/mptradelib/broker/shoonya.py
+-rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.4.1/mptradelib/broker/ticker.py
+-rw-r--r--   0        0        0        0 2024-05-03 11:19:20.268249 mptradelib-0.4.1/mptradelib/cli/__init__.py
+-rw-r--r--   0        0        0     2342 2024-05-09 18:05:58.447254 mptradelib-0.4.1/mptradelib/cli/new.py
+-rw-r--r--   0        0        0      953 2024-05-09 18:11:12.323673 mptradelib-0.4.1/mptradelib/cli/templates/strategy/__init__.py.jinja
+-rw-r--r--   0        0        0     2984 2024-05-04 12:28:56.516490 mptradelib-0.4.1/mptradelib/cli/templates/strategy/backtest.ipynb.jinja
+-rw-r--r--   0        0        0      614 2024-05-03 12:29:43.201283 mptradelib-0.4.1/mptradelib/cli/templates/strategy/livetrade.py.jinja
+-rw-r--r--   0        0        0     5394 2024-05-09 18:03:46.504439 mptradelib-0.4.1/mptradelib/feed.py
+-rw-r--r--   0        0        0     2007 2024-05-09 18:25:26.040938 mptradelib-0.4.1/mptradelib/livetrade.py
+-rw-r--r--   0        0        0       36 2024-05-11 12:09:46.778908 mptradelib-0.4.1/mptradelib/optimizers/__init__.py
+-rw-r--r--   0        0        0     5103 2024-05-11 12:09:34.052370 mptradelib-0.4.1/mptradelib/optimizers/walkforward.py
+-rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.4.1/mptradelib/test_renko.py
+-rw-r--r--   0        0        0       77 2024-05-06 16:16:12.200968 mptradelib-0.4.1/mptradelib/utils/__init__.py
+-rw-r--r--   0        0        0      902 2024-05-06 16:14:19.221626 mptradelib-0.4.1/mptradelib/utils/simulated_trades.py
+-rw-r--r--   0        0        0     6878 2024-05-10 13:29:58.164902 mptradelib-0.4.1/mptradelib/utils/tearsheet.py
+-rw-r--r--   0        0        0      910 2024-05-06 16:15:09.786235 mptradelib-0.4.1/mptradelib/utils/utils.py
+-rw-r--r--   0        0        0      846 2024-05-11 12:09:58.305379 mptradelib-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4041 1970-01-01 00:00:00.000000 mptradelib-0.4.1/PKG-INFO
```

### Comparing `mptradelib-0.4.0/README.md` & `mptradelib-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.0/mptradelib/backtest.py` & `mptradelib-0.4.1/mptradelib/backtest.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,29 @@
 from typing import Callable
 from tqdm import tqdm
 from hyperopt import fmin, tpe, hp, STATUS_OK
 from hyperopt.pyll import scope
 from retry import retry
 import multiprocessing as mp
 from .broker.broker import Order
+from typing import List
 
 class Backtest:
     params: dict = {
         "sl": None,
         "tp": None
     }
 
     def __init__(self, data: pd.DataFrame, compute: Callable[[pd.DataFrame, dict], pd.DataFrame]=None, tp=2, sl=1, intraday=True):
         self.data = data
         self.compute = compute
         self.params['tp'] = tp
         self.params['sl'] = sl
         self.intraday = intraday
-        self.__orders = []
+        self.__orders: List[Order] = []
         self.__position = None
 
     def run(self, **kwargs):
         self.params.update(kwargs)
 
         data = self.data.copy()
         
@@ -44,15 +45,15 @@
         data.loc[data.entries == -1, 'tp'] = data.close * (1 - self.params['tp']/100)
         
         data['exit_price'] = data.open.shift(-1)
         data['trade_time'] = data.datetime.shift(-1)
 
         for row in data.itertuples():
             self._backtest(row)
-        out_df = pd.DataFrame([asdict(o) for o in self.__orders])
+        out_df = pd.DataFrame([o.model_dump() for o in self.__orders])
         self.__orders = []
         self.__position = None
         return out_df, data
 
     def _exit_position(self, row):
         self.__position.exit_price = row.exit_price
         self.__position.exit_time = row.trade_time
@@ -108,16 +109,14 @@
         )
         p = {k: int(v) for k, v in best.items()}
         r = self.run(**p)
         return best, np.sum(r[0].profit)
     
     def optimize(self, runs=5, show_progress=False, **kwargs):
         results = []
-        l = tqdm(range(runs)) if show_progress else range(runs)
-
         params = [kwargs] * runs
         if show_progress:
             with tqdm(total=len(params)) as pbar:
                 with mp.Pool(mp.cpu_count()) as p:
                     for r in p.imap(self._optimizer, params):
                         results.append(r)
                         pbar.update()
```

### Comparing `mptradelib-0.4.0/mptradelib/broker/broker.py` & `mptradelib-0.4.1/mptradelib/broker/broker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.0/mptradelib/broker/session.py` & `mptradelib-0.4.1/mptradelib/broker/session.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.0/mptradelib/broker/shoonya.py` & `mptradelib-0.4.1/mptradelib/broker/shoonya.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.0/mptradelib/broker/ticker.py` & `mptradelib-0.4.1/mptradelib/broker/ticker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.0/mptradelib/cli/new.py` & `mptradelib-0.4.1/mptradelib/cli/new.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.0/mptradelib/cli/templates/strategy/__init__.py.jinja` & `mptradelib-0.4.1/mptradelib/cli/templates/strategy/__init__.py.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.0/mptradelib/cli/templates/strategy/backtest.ipynb.jinja` & `mptradelib-0.4.1/mptradelib/cli/templates/strategy/backtest.ipynb.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.0/mptradelib/cli/templates/strategy/livetrade.py.jinja` & `mptradelib-0.4.1/mptradelib/cli/templates/strategy/livetrade.py.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.0/mptradelib/feed.py` & `mptradelib-0.4.1/mptradelib/feed.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.0/mptradelib/livetrade.py` & `mptradelib-0.4.1/mptradelib/livetrade.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.0/mptradelib/test_renko.py` & `mptradelib-0.4.1/mptradelib/test_renko.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.0/mptradelib/utils/simulated_trades.py` & `mptradelib-0.4.1/mptradelib/utils/simulated_trades.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.0/mptradelib/utils/utils.py` & `mptradelib-0.4.1/mptradelib/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.4.0/pyproject.toml` & `mptradelib-0.4.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mptradelib"
-version = "0.4.0"
+version = "0.4.1"
 description = ""
 authors = ["Abhilash Nanda <wishabhilash@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "2.7.1"
@@ -13,14 +13,15 @@
 retry = "0.9.2"
 pyotp = "2.9.0"
 jinja2 = "^3.1.3"
 click = "^8.1.7"
 jinja2-strcase = "^0.0.2"
 redis = "^5.0.4"
 pandas-ta = "^0.3.14b0"
+tqdm = "^4.66.4"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.0"
 
 pandas_ta = { version = "^0.3.14b", optional = true }
 pandas = { version = "^2.1.4", optional = true }
 hyperopt = { version = "^0.2.7", optional = true }
```

### Comparing `mptradelib-0.4.0/PKG-INFO` & `mptradelib-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mptradelib
-Version: 0.4.0
+Version: 0.4.1
 Summary: 
 Author: Abhilash Nanda
 Author-email: wishabhilash@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -18,14 +18,15 @@
 Requires-Dist: jinja2-strcase (>=0.0.2,<0.0.3)
 Requires-Dist: pandas-ta (>=0.3.14b0,<0.4.0) ; extra == "pandasta"
 Requires-Dist: pydantic (==2.7.1)
 Requires-Dist: pyotp (==2.9.0)
 Requires-Dist: redis (>=5.0.4,<6.0.0)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: retry (==0.9.2)
+Requires-Dist: tqdm (>=4.66.4,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Installation
 Create a virtualenv.
 ```
 pip install mptradelib
 ```
```

