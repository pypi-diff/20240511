# Comparing `tmp/abses-0.5.8.tar.gz` & `tmp/abses-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abses-0.5.8.tar", max compression
+gzip compressed data, was "abses-0.6.0.tar", max compression
```

## Comparing `abses-0.5.8.tar` & `abses-0.6.0.tar`

### file list

```diff
@@ -1,29 +1,42 @@
--rw-r--r--   0        0        0    10280 2023-02-23 05:59:56.670150 abses-0.5.8/LICENSE
-drwxr-xr-x   0        0        0        0 2023-10-20 02:43:17.702059 abses-0.5.8/LICENSES/
--rw-r--r--   0        0        0     6273 2024-04-10 23:24:41.142521 abses-0.5.8/README.md
--rw-r--r--   0        0        0      978 2024-04-17 20:22:18.052991 abses-0.5.8/abses/__init__.py
--rw-r--r--   0        0        0     9558 2024-04-17 20:09:28.912183 abses-0.5.8/abses/actor.py
--rw-r--r--   0        0        0     2651 2024-04-06 01:06:25.259012 abses-0.5.8/abses/bases.py
--rw-r--r--   0        0        0     4973 2024-04-17 20:10:03.296369 abses-0.5.8/abses/cells.py
--rw-r--r--   0        0        0     2967 2024-04-06 01:06:25.259964 abses-0.5.8/abses/components.py
--rw-r--r--   0        0        0    17519 2024-04-17 20:09:28.912922 abses-0.5.8/abses/container.py
--rw-r--r--   0        0        0     8957 2024-04-06 01:06:25.261273 abses-0.5.8/abses/decision.py
--rw-r--r--   0        0        0     3056 2024-04-17 20:09:28.913290 abses-0.5.8/abses/dynamic.py
--rw-r--r--   0        0        0      298 2024-01-11 09:19:35.315645 abses-0.5.8/abses/errors.py
--rw-r--r--   0        0        0     3956 2024-04-06 01:06:25.261907 abses-0.5.8/abses/human.py
--rw-r--r--   0        0        0    19075 2024-04-17 20:09:28.913742 abses-0.5.8/abses/links.py
--rw-r--r--   0        0        0      347 2024-01-11 09:19:35.316189 abses-0.5.8/abses/logging.py
--rw-r--r--   0        0        0    12160 2024-04-17 20:09:28.914257 abses-0.5.8/abses/main.py
--rw-r--r--   0        0        0     5695 2024-04-17 20:09:28.914551 abses-0.5.8/abses/modules.py
--rw-r--r--   0        0        0     8368 2024-04-17 20:15:11.153437 abses-0.5.8/abses/move.py
--rw-r--r--   0        0        0    30522 2024-04-17 20:09:28.915222 abses-0.5.8/abses/nature.py
--rw-r--r--   0        0        0     3102 2024-04-17 20:09:28.915489 abses-0.5.8/abses/objects.py
--rw-r--r--   0        0        0     6247 2024-04-17 20:15:11.153720 abses-0.5.8/abses/random.py
--rw-r--r--   0        0        0     1611 2024-04-04 10:58:12.168183 abses-0.5.8/abses/selection.py
--rw-r--r--   0        0        0    11588 2024-04-17 20:09:28.916092 abses-0.5.8/abses/sequences.py
--rw-r--r--   0        0        0     1098 2024-04-06 01:06:25.265815 abses-0.5.8/abses/states.py
--rw-r--r--   0        0        0    14591 2024-04-06 01:06:25.266235 abses-0.5.8/abses/time.py
--rw-r--r--   0        0        0     3216 2024-04-12 13:02:22.365090 abses-0.5.8/abses/tools/func.py
--rw-r--r--   0        0        0      723 2024-04-17 19:21:17.693370 abses-0.5.8/abses/tools/regex.py
--rw-r--r--   0        0        0     2469 2024-04-17 20:22:18.047793 abses-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     7241 1970-01-01 00:00:00.000000 abses-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0    10280 2023-02-23 05:59:56.670150 abses-0.6.0/LICENSE
+drwxr-xr-x   0        0        0        0 2023-10-20 02:43:17.702059 abses-0.6.0/LICENSES/
+-rw-r--r--   0        0        0     6273 2024-04-10 23:24:41.142521 abses-0.6.0/README.md
+-rw-r--r--   0        0        0     1076 2024-05-11 09:28:11.067993 abses-0.6.0/abses/__init__.py
+-rw-r--r--   0        0        0     2651 2024-05-11 09:28:11.068165 abses-0.6.0/abses/_bases/bases.py
+-rw-r--r--   0        0        0     3124 2024-05-11 09:28:11.068264 abses-0.6.0/abses/_bases/components.py
+-rw-r--r--   0        0        0     3128 2024-05-11 09:28:11.068727 abses-0.6.0/abses/_bases/dynamic.py
+-rw-r--r--   0        0        0      298 2024-05-11 09:28:11.068876 abses-0.6.0/abses/_bases/errors.py
+-rw-r--r--   0        0        0      347 2024-05-11 09:28:11.068990 abses-0.6.0/abses/_bases/logging.py
+-rw-r--r--   0        0        0     6280 2024-05-11 09:28:11.069510 abses-0.6.0/abses/_bases/modules.py
+-rw-r--r--   0        0        0     3075 2024-05-11 09:28:11.069838 abses-0.6.0/abses/_bases/objects.py
+-rw-r--r--   0        0        0     1098 2024-05-11 09:28:11.069942 abses-0.6.0/abses/_bases/states.py
+-rw-r--r--   0        0        0     9572 2024-05-11 09:28:11.070216 abses-0.6.0/abses/actor.py
+-rw-r--r--   0        0        0     4979 2024-05-11 09:28:11.070565 abses-0.6.0/abses/cells.py
+-rw-r--r--   0        0        0      297 2024-05-11 09:28:11.070733 abses-0.6.0/abses/conf/default.yaml
+-rw-r--r--   0        0        0    17526 2024-05-11 09:28:11.070970 abses-0.6.0/abses/container.py
+-rw-r--r--   0        0        0      969 2024-05-11 09:28:11.071255 abses-0.6.0/abses/data.py
+-rw-r--r--   0        0        0     8957 2024-05-10 03:24:33.872539 abses-0.6.0/abses/decision.py
+-rw-r--r--   0        0        0    14654 2024-05-11 09:28:11.071603 abses-0.6.0/abses/experiment.py
+-rw-r--r--   0        0        0     3930 2024-05-11 09:28:11.071776 abses-0.6.0/abses/human.py
+-rw-r--r--   0        0        0    19386 2024-05-11 09:28:11.072342 abses-0.6.0/abses/links.py
+-rw-r--r--   0        0        0    13666 2024-05-11 09:28:11.072495 abses-0.6.0/abses/main.py
+-rw-r--r--   0        0        0     8375 2024-05-11 09:28:11.072683 abses-0.6.0/abses/move.py
+-rw-r--r--   0        0        0    12421 2024-05-11 09:28:11.073005 abses-0.6.0/abses/nature.py
+-rw-r--r--   0        0        0    28654 2024-05-11 09:28:11.073487 abses-0.6.0/abses/patch.py
+-rw-r--r--   0        0        0     6802 2024-05-11 09:28:11.073646 abses-0.6.0/abses/random.py
+-rw-r--r--   0        0        0     1611 2024-04-04 10:58:12.168183 abses-0.6.0/abses/selection.py
+-rw-r--r--   0        0        0    11768 2024-05-11 09:28:11.073845 abses-0.6.0/abses/sequences.py
+-rw-r--r--   0        0        0    14598 2024-05-11 09:28:11.073992 abses-0.6.0/abses/time.py
+-rw-r--r--   0        0        0     4494 2024-05-11 09:28:11.074135 abses-0.6.0/abses/tools/func.py
+-rw-r--r--   0        0        0      723 2024-04-17 19:21:17.693370 abses-0.6.0/abses/tools/regex.py
+-rw-r--r--   0        0        0      918 2024-05-11 09:28:11.074248 abses-0.6.0/abses/viz/viz_actors.py
+-rw-r--r--   0        0        0     1149 2024-05-11 09:28:11.074327 abses-0.6.0/abses/viz/viz_model.py
+-rw-r--r--   0        0        0     4620 2024-05-11 09:28:11.074600 abses-0.6.0/abses/viz/viz_nature.py
+-rw-r--r--   0        0        0     6148 2024-04-14 20:25:37.202150 abses-0.6.0/data/.DS_Store
+-rw-r--r--   0        0        0  1653872 2023-09-03 00:55:23.536915 abses-0.6.0/data/YR_cities.zip
+-rw-r--r--   0        0        0   395561 2023-11-13 06:23:20.897117 abses-0.6.0/data/farmland.tif
+-rw-r--r--   0        0        0    84033 2023-09-02 23:31:24.485471 abses-0.6.0/data/irr_lands.csv
+-rw-r--r--   0        0        0  6726328 2023-03-03 00:57:27.899017 abses-0.6.0/data/precipitation.nc
+-rw-r--r--   0        0        0   189444 2024-05-11 09:28:11.085808 abses-0.6.0/icons/fa-regular-400.otf
+-rw-r--r--   0        0        0     2714 2024-05-11 09:28:11.086826 abses-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7334 1970-01-01 00:00:00.000000 abses-0.6.0/PKG-INFO
```

### Comparing `abses-0.5.8/LICENSE` & `abses-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `abses-0.5.8/README.md` & `abses-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `abses-0.5.8/abses/__init__.py` & `abses-0.6.0/abses/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,17 +23,21 @@
     "Actor",
     "Decision",
     "ActorsList",
     "PatchCell",
     "perception",
     "alive_required",
     "time_condition",
+    "Experiment",
+    "load_data",
 ]
-__version__ = "v0.5.8"
+__version__ = "v0.6.0"
 
 from .actor import Actor, alive_required, perception
 from .container import ActorsList
+from .data import load_data
 from .decision import Decision
+from .experiment import Experiment
 from .human import BaseHuman
 from .main import MainModel
 from .nature import BaseNature, PatchCell, PatchModule
 from .time import time_condition
```

### Comparing `abses-0.5.8/abses/actor.py` & `abses-0.6.0/abses/actor.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,19 +27,19 @@
 try:
     from typing import TypeAlias
 except ImportError:
     from typing_extensions import TypeAlias
 
 import mesa_geo as mg
 
+from abses._bases.errors import ABSESpyError
+from abses._bases.objects import _BaseObj
 from abses.decision import _DecisionFactory
-from abses.errors import ABSESpyError
 from abses.links import TargetName, _LinkNodeActor, _LinkNodeCell
 from abses.move import _Movements
-from abses.objects import _BaseObj
 from abses.tools.func import make_list
 
 if TYPE_CHECKING:
     from abses.cells import Pos
     from abses.main import MainModel
     from abses.nature import PatchCell, PatchModule
```

### Comparing `abses-0.5.8/abses/bases.py` & `abses-0.6.0/abses/_bases/bases.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.8/abses/cells.py` & `abses-0.6.0/abses/cells.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Callable, Optional, Tuple, Union
 
 from mesa_geo.raster_layers import RasterBase
 
 from abses import ActorsList
+from abses._bases.errors import ABSESpyError
 from abses.container import _CellAgentsContainer
-from abses.errors import ABSESpyError
 from abses.links import TargetName, _LinkNodeCell
 
 if TYPE_CHECKING:
     from abses.main import H, MainModel, N
     from abses.nature import PatchModule
 
 try:
@@ -32,15 +32,15 @@
 Pos: TypeAlias = Tuple[int, int]
 
 
 def raster_attribute(
     func: Callable[[Any], Union[str | int | float]]
 ) -> property:
     """Turn the method into a property that the patch can extract.
-    Examples:
+    Example:
         ```
         class TestCell(Cell):
             @raster_attribute
             def test:
                 return 1
 
         # Using this test cell to create a PatchModule.
```

### Comparing `abses-0.5.8/abses/components.py` & `abses-0.6.0/abses/_bases/components.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 3. TimeDriver 时间驱动器
 4. DataCollector 数据收集器
 """
 
 from __future__ import annotations
 
 import re
+from pathlib import Path
 from typing import TYPE_CHECKING, Any, Iterable, Optional, Set, Union
 
 from omegaconf import DictConfig
 
 from abses.tools.func import make_list
 from abses.tools.regex import MODULE_NAME
 
@@ -46,14 +47,19 @@
         self._model: MainModel[Any, Any] = model
         if name is None:
             name = self.__class__.__name__.lower()
         self.name = name
         self.add_args(self.__args__)
 
     @property
+    def outpath(self) -> Optional[Path]:
+        """Where to save the outputs."""
+        return self._model.outpath
+
+    @property
     def name(self) -> str:
         """Get the name of the component"""
         return self._name
 
     @name.setter
     def name(self, value: str) -> None:
         """Set the name of the component"""
```

### Comparing `abses-0.5.8/abses/container.py` & `abses-0.6.0/abses/container.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 except ImportError:
     from typing_extensions import TypeAlias
 
 import geopandas as gpd
 import mesa_geo as mg
 from loguru import logger
 
+from abses._bases.errors import ABSESpyError
 from abses.actor import Actor, Breeds
-from abses.errors import ABSESpyError
 from abses.sequences import HOW, ActorsList, Selection
 from abses.tools.func import make_list
 
 if TYPE_CHECKING:
     from abses.cells import PatchCell
     from abses.main import MainModel
```

### Comparing `abses-0.5.8/abses/decision.py` & `abses-0.6.0/abses/decision.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.8/abses/dynamic.py` & `abses-0.6.0/abses/_bases/dynamic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 #!/usr/bin/env python 3.11.0
 # -*-coding:utf-8 -*-
 # @Author  : Shuang (Twist) Song
 # @Contact   : SongshGeo@gmail.com
 # GitHub   : https://github.com/SongshGeo
 # Website: https://cv.songshgeo.com/
 
+"""Dynamic variables
+"""
+
 from __future__ import annotations
 
 import inspect
 from typing import TYPE_CHECKING, Any, Callable, List
 
 if TYPE_CHECKING:
+    from ..time import TimeDriver
     from .objects import _BaseObj
-    from .time import TimeDriver
 
 
 class _DynamicVariable:
     """Time dependent variable
 
     A time dependent function will take the model time driver as
     an input and return its value. The function can also take other
     variables as inputs. The function can be defined as a static
     method of a class or a function.
     """
 
     def __init__(
-        self, name: str, obj: _BaseObj, data: Any, function: Callable
+        self, name: str, obj: _BaseObj, data: Any, function: Callable, **kwargs
     ) -> None:
         self._name: str = name
         self._obj: _BaseObj = obj
         self._data: Any = data
         self._function: Callable = function
         self._cached_data: Any = None
+        self.attrs = kwargs
         self.now()
 
     @property
-    def name(self):
+    def name(self) -> str:
         """Get the name of the variable
 
         Returns
         -------
         name: str
         """
         return self._name
@@ -105,16 +109,15 @@
             if attr in source_code
         ]
 
     def now(self) -> Any:
         """Return the dynamic variable function's output
 
         Returns:
-            output:
-                Any
+            The dynamic data value now.
         """
         required_attrs = self.get_required_attributes(self.function)
         args = {attr: getattr(self, attr) for attr in required_attrs}
         result = self.function(**args)
         self._cached_data = result
         return result
```

### Comparing `abses-0.5.8/abses/human.py` & `abses-0.6.0/abses/human.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,21 @@
 
 try:
     from typing import TypeAlias
 except ImportError:
     from typing_extensions import TypeAlias
 
 from loguru import logger
-from omegaconf import DictConfig
 
 from abses.actor import Actor
 from abses.links import _LinkContainer
 
+from ._bases.modules import CompositeModule, Module
 from .cells import PatchCell
 from .container import _AgentsContainer
-from .modules import CompositeModule, Module
 from .sequences import ActorsList, Selection
 
 Actors: TypeAlias = Union[ActorsList[Actor], Selection, Actor]
 Trigger: TypeAlias = Union[str, Callable[..., Any]]
 if TYPE_CHECKING:
     from abses import MainModel
```

### Comparing `abses-0.5.8/abses/links.py` & `abses-0.6.0/abses/links.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 with contextlib.suppress(ImportError):
     import networkx as nx
 try:
     from typing import TypeAlias
 except ImportError:
     from typing_extensions import TypeAlias
 
-from abses.errors import ABSESpyError
+from abses._bases.errors import ABSESpyError
 from abses.sequences import ActorsList
 
 if TYPE_CHECKING:
     from abses import MainModel
     from abses.actor import Actor
     from abses.cells import PatchCell
     from abses.container import _CellAgentsContainer
@@ -463,14 +463,23 @@
     unique_id: int = -1
     breed = _BreedDescriptor()
 
     @abstractmethod
     def _default_redirection(self, target: Optional[TargetName]) -> AttrGetter:
         """默认重定向"""
 
+    @classmethod
+    def viz_attrs(cls, **kwargs) -> Dict[str, Any]:
+        """Return the attributes for viz."""
+        return {
+            "marker": getattr(cls, "marker", "o"),
+            "color": getattr(cls, "color", "black"),
+            "alpha": getattr(cls, "alpha", 1.0),
+        } | kwargs
+
     @cached_property
     def link(self) -> _LinkProxy:
         """A proxy which can be used to manipulate the links:
 
         1. `link.to()`: creates a new link from this actor to another.
         2. `link.by()`: creates a new link from another to this actor.
         3. `link.get()`: gets the links of this actor.
```

### Comparing `abses-0.5.8/abses/main.py` & `abses-0.6.0/abses/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,19 @@
 
 """
 The main modelling framework of ABSESpy.
 """
 
 from __future__ import annotations
 
+import functools
+import os
 import sys
+import types
+from pathlib import Path
 from typing import (
     Any,
     Callable,
     Dict,
     Generic,
     List,
     Literal,
@@ -38,21 +42,22 @@
 from mesa import DataCollector, Model
 from mesa.time import BaseScheduler
 from omegaconf import DictConfig, OmegaConf
 
 from abses import __version__
 from abses.actor import Actor
 
-from .bases import _Notice
+from ._bases.bases import _Notice
+from ._bases.states import _States
 from .container import _AgentsContainer
 from .human import BaseHuman
 from .nature import BaseNature
 from .sequences import ActorsList
-from .states import _States
 from .time import TimeDriver
+from .viz.viz_model import _VizModel
 
 # Logging configuration
 logger.remove(0)
 logger.add(
     sys.stderr,
     format="[{time:YYYY-MM-DD HH:mm:ss}][{module:<15}] | {message}",
     level="WARNING",
@@ -107,14 +112,15 @@
 
     def __init__(
         self,
         parameters: DictConfig = DictConfig({}),
         human_class: Optional[Type[H]] = None,
         nature_class: Optional[Type[N]] = None,
         run_id: Optional[int] = None,
+        outpath: Optional[Path] = None,
         **kwargs: Optional[Any],
     ) -> None:
         Model.__init__(self, **kwargs)
         _Notice.__init__(self)
         _States.__init__(self)
 
         self.running: bool = True
@@ -123,16 +129,17 @@
         self._settings = DictConfig(parameters)
         self._version: str = __version__
         self._check_subsystems(h_cls=human_class, n_cls=nature_class)
         self._agents = _AgentsContainer(
             model=self, max_len=kwargs.get("max_agents")
         )
         self._time = TimeDriver(model=self)
-        self._run_id: int | None = run_id
-        self.schedule = BaseScheduler(model=self)
+        self._run_id: Optional[int] = run_id
+        self.outpath = outpath
+        self.schedule: BaseScheduler = BaseScheduler(model=self)
         self.initialize_data_collector()
         self._do_each("initialize", order=("nature", "human"))
         self._do_each("set_state", code=1)  # initial state
 
     def __repr__(self) -> str:
         version = self._version
         return f"<{self.name}-{version}({self.state})>"
@@ -161,14 +168,26 @@
         _obj = {"model": self, "nature": self.nature, "human": self.human}
         for name in order:
             if name not in _obj:
                 raise ValueError(f"{name} is not a valid component.")
             getattr(_obj[name], _func)(**kwargs)
 
     @property
+    def outpath(self) -> Optional[Path]:
+        """Output path where to deposit assets."""
+        return self._outpath
+
+    @outpath.setter
+    def outpath(self, path: Optional[Path]) -> None:
+        if path is None:
+            path = Path(os.getcwd())
+        assert path.is_dir(), f"Invalid path {path}"
+        self._outpath = path
+
+    @property
     def run_id(self) -> int | None:
         """The run id of the current model.
         It's useful in batch run.
         When running a single model, the run id is None.
         """
         return self._run_id
 
@@ -250,14 +269,19 @@
         """Register a new breed of agents in the model."""
         if not issubclass(breed, Actor):
             raise TypeError(f"{breed} is not a subclass of Actor.")
         self._breeds[breed.breed] = breed
         for container in self._containers:
             container[breed.breed] = set()
 
+    @functools.cached_property
+    def plot(self) -> _VizModel:
+        """Plotting the model."""
+        return _VizModel(self)
+
     def run_model(self, steps: Optional[int] = None) -> None:
         """Start running the model.
 
         In order, the model will go through the following steps:
         1. Call `model.setup()` method.
         2. Call `model.step()` method.
         3. Repeating steps, until the end situation is triggered
@@ -290,16 +314,30 @@
         self._do_each("step", order=("model", "nature", "human"))
         self.schedule.step()
         self.datacollector.collect(self)
 
     def _end(self) -> None:
         self._do_each("end", order=("nature", "human", "model"))
         self._do_each("set_state", code=3)
+        self.final_report()
         logger.info(f"Ending {self.name}")
 
+    def final_report(self) -> Dict[str, Any]:
+        """Report at the end of this model."""
+        result = {}
+        for k, reporter in self._reports["final"].items():
+            if isinstance(reporter, str):
+                value = getattr(self, reporter)
+            elif isinstance(reporter, types.FunctionType):
+                value = reporter(self)
+            else:
+                raise TypeError(f"Invalid final reporter {type(reporter)}.")
+            result[k] = value
+        return result
+
     def summary(self, verbose: bool = False) -> pd.DataFrame:
         """Report the state of the model."""
         print(f"Using ABSESpy version: {self.version}")
         # Basic reports
         to_report = {
             "name": self.name,
             "state": self.state,
@@ -336,25 +374,32 @@
         cfg: DictConfig = self.settings.get("reports", OmegaConf.create({}))
         to_reports = cast(
             Dict[str, Dict[str, Reporter]],
             OmegaConf.to_container(cfg, resolve=True),
         )
         reporting_model: Dict[str, Reporter] = to_reports.get("model", {})
         reporting_agents: Dict[str, Reporter] = to_reports.get("agents", {})
+        reporting_final: Dict[str, Reporter] = to_reports.get("final", {})
         if model_reporters is not None:
             reporting_model |= model_reporters
         if agent_reporters is not None:
             reporting_agents |= agent_reporters
         _convert_to_python_expression(reporting_model)
         _convert_to_python_expression(reporting_agents)
+        _convert_to_python_expression(reporting_final)
         self.datacollector = DataCollector(
             model_reporters=reporting_model,
             agent_reporters=reporting_agents,
             tables=tables,
         )
+        self._reports = {
+            "model": reporting_model,
+            "agent": reporting_agents,
+            "final": reporting_final,
+        }
 
 
 def _convert_to_python_expression(
     expression_dict: Dict[str, Reporter]
 ) -> None:
     """Convert a Python expression string to a Python expression."""
     for key, value in expression_dict.items():
```

### Comparing `abses-0.5.8/abses/modules.py` & `abses-0.6.0/abses/_bases/modules.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,31 +12,39 @@
 
 from __future__ import annotations
 
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
+    Generic,
     Iterator,
     List,
+    Literal,
     Optional,
     Type,
     TypeVar,
 )
 
 from loguru import logger
 
+from abses._bases.bases import _Notice
+from abses._bases.objects import _BaseObj
+from abses._bases.states import _States
 from abses.tools.func import iter_func
 
-from .bases import _Notice
-from .objects import _BaseObj
-from .states import _States
-
 if TYPE_CHECKING:
-    from .main import MainModel
+    from ..main import MainModel
+
+try:
+    from typing import TypeAlias
+except ImportError:
+    from typing_extensions import TypeAlias
+
+HowCreation: TypeAlias = Literal["from_resolution", "from_file", "copy_layer"]
 
 
 class Module(_BaseObj):
     """Basic module for the model."""
 
     def __init__(
         self,
@@ -83,27 +91,36 @@
         Called at the end of the simulation.
         """
 
 
 ModuleType = TypeVar("ModuleType", bound=Module)
 
 
-class _ModuleFactory(object):
+class _ModuleFactory(Generic[ModuleType]):
     """To create a module."""
 
     methods: List[str] = []
     default_cls: type[Module] = Module
 
     def __init__(self, father) -> None:
         self.father: CompositeModule = father
-        self.modules: Dict[str, Module] = {}
+        self.modules: Dict[str, ModuleType] = {}
 
     def __iter__(self) -> Iterator[Module]:
         return iter(self.modules.values())
 
+    def __getitem__(self, name: str) -> Module:
+        return self.modules[name]
+
+    def __contains__(self, name: str | ModuleType) -> bool:
+        return name in self.modules or name in self.modules.values()
+
+    def __len__(self) -> int:
+        return len(self.modules)
+
     def _check_cls(
         self, module_cls: Optional[Type[ModuleType]]
     ) -> Type[Module]:
         """Check if the provided class is a valid module class."""
         if module_cls is None:
             return self.default_cls
         if not issubclass(module_cls, self.default_cls):
@@ -120,15 +137,15 @@
     def _check_name(self, name: str) -> None:
         """Check if the name is valid."""
         if name in self.modules:
             raise ValueError(f"Name '{name}' already exists in the model.")
 
     def new(
         self,
-        how: Optional[str] = None,
+        how: Optional[HowCreation] = None,
         module_class: Optional[Type[ModuleType]] = None,
         **kwargs,
     ) -> ModuleType:
         """Create a module and attach it to the model.
 
         Parameters:
             module_class:
@@ -168,20 +185,22 @@
 
 
 # Composite
 class CompositeModule(Module, _States, _Notice):
     """基本的组合模块，可以创建次级模块"""
 
     def __init__(
-        self, model: MainModel[Any, Any], name: Optional[str] = None
+        self,
+        model: MainModel[Any, Any],
+        name: Optional[str] = None,
     ) -> None:
         Module.__init__(self, model, name=name)
         _States.__init__(self)
         _Notice.__init__(self)
-        self._modules = _ModuleFactory(self)
+        self._modules: _ModuleFactory = _ModuleFactory(self)
 
     @property
     def modules(self) -> _ModuleFactory:
         """All attached sub-modules."""
         return self._modules
 
     @property
@@ -206,10 +225,10 @@
     def step(self):
         return super().step()
 
     @iter_func("modules")
     def end(self):
         return super().end()
 
-    def create_module(self, module_cls, *args, **kwargs):
+    def create_module(self, module_cls, how=None, **kwargs):
         """Create a module."""
-        return self.modules.new(module_class=module_cls, *args, **kwargs)
+        return self.modules.new(how=how, module_class=module_cls, **kwargs)
```

### Comparing `abses-0.5.8/abses/move.py` & `abses-0.6.0/abses/move.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     from typing import TypeAlias
 except ImportError:
     from typing_extensions import TypeAlias
 
 from mesa.space import Coordinate
 from mesa_geo.raster_layers import RasterBase
 
-from abses.errors import ABSESpyError
+from abses._bases.errors import ABSESpyError
 from abses.links import _LinkNodeCell
 
 if TYPE_CHECKING:
     from abses.actor import Actor
     from abses.cells import PatchCell
     from abses.nature import PatchModule
```

### Comparing `abses-0.5.8/abses/nature.py` & `abses-0.6.0/abses/patch.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,83 +1,85 @@
 #!/usr/bin/env python 3.11.0
 # -*-coding:utf-8 -*-
-# @Author  : Shuang Song
+# @Author  : Shuang (Twist) Song
 # @Contact   : SongshGeo@gmail.com
 # GitHub   : https://github.com/SongshGeo
 # Website: https://cv.songshgeo.com/
 
+"""PatchModule class
 """
-The spatial module.
-"""
-
 from __future__ import annotations
 
 import copy
 import functools
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterator,
+    Literal,
     Optional,
     Sequence,
     Set,
     Type,
     Union,
     cast,
     overload,
 )
 
 try:
-    from typing import Self, TypeAlias
+    from typing import TypeAlias
 except ImportError:
-    from typing_extensions import Self, TypeAlias
+    from typing_extensions import TypeAlias
 
 import numpy as np
 import pyproj
 import rasterio
 import rioxarray
 import xarray as xr
 from loguru import logger
 from mesa.space import Coordinate
 from mesa_geo.raster_layers import RasterBase
 from rasterio import mask
 from rasterio.enums import Resampling
 from rasterio.warp import calculate_default_transform, transform_bounds
 from shapely import Geometry
 
-from abses.modules import CompositeModule, Module, _ModuleFactory
+from abses._bases.errors import ABSESpyError
+from abses._bases.modules import Module, _ModuleFactory
+from abses.cells import PatchCell
 from abses.random import ListRandom
+from abses.sequences import ActorsList
 from abses.tools.func import get_buffer
-
-from .cells import PatchCell
-from .errors import ABSESpyError
-from .sequences import ActorsList
+from abses.viz.viz_nature import _VizNature
 
 if TYPE_CHECKING:
     from abses.main import MainModel
 
 CRS = "epsg:4326"
+CellFilter: TypeAlias = Optional[str | np.ndarray | xr.DataArray | Geometry]
 Raster: TypeAlias = Union[
     np.ndarray,
     xr.DataArray,
     xr.Dataset,
 ]
-CellFilter: TypeAlias = Optional[str | np.ndarray | xr.DataArray | Geometry]
 
 
 class _PatchModuleFactory(_ModuleFactory):
     def __init__(self, father) -> None:
         super().__init__(father)
         self.default_cls = PatchModule
 
     def __repr__(self) -> str:
         return repr(self.father)
 
+    def __getitem__(self, name: str) -> PatchModule:
+        return self.modules[name]
+
     def from_resolution(
         self,
         model: MainModel[Any, Any],
         name: Optional[str] = None,
         shape: Coordinate = (10, 10),
         crs: Optional[pyproj.CRS | str] = CRS,
         resolution: Union[int, float] = 1,
@@ -170,14 +172,16 @@
         raster_file: str,
         model: MainModel[Any, Any],
         cell_cls: type[PatchCell] = PatchCell,
         module_cls: Optional[Type[PatchModule]] = None,
         name: str | None = None,
         attr_name: str | None = None,
         apply_raster: bool = False,
+        band: int = 1,
+        nodata: Any = np.nan,
         **kwargs: Any,
     ) -> PatchModule:
         """Create a raster layer module from a file.
 
         Parameters:
             raster_file:
                 File path of a geo-tiff dataset.
@@ -191,16 +195,18 @@
                 E.g., class Module -> module.
             cell_cls:
                 Class type of `PatchCell` to create.
 
         """
         to_create = cast(PatchModule, self._check_cls(module_cls=module_cls))
         with rasterio.open(raster_file, "r") as dataset:
-            values = dataset.read()
-            _, height, width = values.shape
+            values = dataset.read(band)
+            nodata_mask = values == dataset.nodata
+            values[nodata_mask] = nodata
+            height, width = values.shape
             total_bounds = [
                 dataset.bounds.left,
                 dataset.bounds.bottom,
                 dataset.bounds.right,
                 dataset.bounds.top,
             ]
         obj: PatchModule = to_create(
@@ -208,14 +214,15 @@
             name=name,
             width=width,
             height=height,
             crs=dataset.crs,
             total_bounds=total_bounds,
             cell_cls=cell_cls,
         )
+        obj.mask = np.squeeze(~nodata_mask)
         # obj._transform = dataset.transform
         if apply_raster:
             obj.apply_raster(values, attr_name=attr_name, **kwargs)
         return obj
 
 
 class PatchModule(Module, RasterBase):
@@ -265,19 +272,35 @@
         logger.info(f"Using rioxarray version: {rioxarray.__version__}")
 
         func = np.vectorize(lambda row, col: cell_cls(self, (row, col)))
         self._cells: np.ndarray = np.fromfunction(
             func, shape=(self.height, self.width), dtype=object
         )
         self._attributes: Set[str] = set()
+        self.mask: np.ndarray = np.ones(self.shape2d)
 
-    @property
-    def cells(self) -> np.ndarray:
+    @functools.cached_property
+    def cells(self) -> ActorsList[PatchCell]:
         """The cells stored in this layer."""
-        return self._cells
+        return ActorsList(self.model, self.array_cells[self.mask])
+
+    @property
+    def mask(self) -> np.ndarray:
+        """Where is not accessible."""
+        return self._mask
+
+    @mask.setter
+    def mask(self, array: np.ndarray) -> None:
+        """Setting mask."""
+        if array.shape != self.shape2d:
+            raise ABSESpyError(
+                f"Shape mismatching, setting mask {array.shape}."
+                f"but the module is expecting shape {self.shape2d}."
+            )
+        self._mask = array.astype(bool)
 
     def __repr__(self):
         return f"<{self.name}{self.shape2d}: {len(self.attributes)} vars>"
 
     def __getitem__(
         self,
         index: int | Sequence[Coordinate] | tuple[int | slice, int | slice],
@@ -301,21 +324,25 @@
         All `PatchCell` methods decorated by `raster_attribute` should be appeared here.
         """
         return self.cell_cls.__attribute_properties__()
 
     @functools.cached_property
     def xda(self) -> xr.DataArray:
         """Get the xarray raster layer with spatial coordinates."""
-        arr = np.ones(self.shape2d)
-        xda = xr.DataArray(data=arr, coords=self.coords)
+        xda = xr.DataArray(data=self.mask, coords=self.coords)
         xda = xda.rio.write_crs(self.crs)
         xda = xda.rio.set_spatial_dims("x", "y")
         xda = xda.rio.write_transform(self.transform)
         return xda.rio.write_coordinate_system()
 
+    @functools.cached_property
+    def plot(self) -> _VizNature:
+        """Plotting"""
+        return _VizNature(self)
+
     @property
     def attributes(self) -> set[str]:
         """All accessible attributes from this layer."""
         return self._attributes | self.cell_properties
 
     @property
     def shape2d(self) -> Coordinate:
@@ -330,31 +357,31 @@
         This is useful when working with `rasterio` band.
         """
         return 1, self.height, self.width
 
     @functools.cached_property
     def array_cells(self) -> np.ndarray:
         """Array type of the `PatchCell` stored in this module."""
-        # return np.flipud(np.array(self.cells).T)
         return self._cells
 
     @functools.cached_property
     def coords(self) -> Coordinate:
         """Coordinate system of the raster data.
         This is useful when working with `xarray.DataArray`.
         """
         min_x, min_y, max_x, max_y = self.total_bounds
         coords_x = np.linspace(min_x, max_x, self.width, endpoint=False)
-        coords_y = np.linspace(min_y, max_y, self.height, endpoint=False)
+        coords_y = np.linspace(max_y, min_y, self.height, endpoint=False)
         return {
             "y": coords_y,
             "x": coords_x,
         }
 
-    def to_crs(self, crs, inplace=False) -> Self | None:
+    def to_crs(self, crs, inplace=False) -> Optional[PatchModule]:
+        """Converting the raster data to a another CRS."""
         super()._to_crs_check(crs)
         layer = self if inplace else copy.copy(self)
 
         src_crs = rasterio.crs.CRS.from_user_input(layer.crs)
         dst_crs = rasterio.crs.CRS.from_user_input(crs)
         if not layer.crs.is_exact_same(crs):
             transform, _, _ = calculate_default_transform(
@@ -386,47 +413,60 @@
             raise ABSESpyError(
                 f"Shape mismatch: {data.shape} [input] != {self.shape2d} [expected]."
             )
         if isinstance(data, str) and data in self.attributes:
             return self.get_raster(data)
         raise TypeError("Invalid data type or shape.")
 
-    def dynamic_var(self, attr_name: str) -> np.ndarray:
+    def dynamic_var(
+        self,
+        attr_name: str,
+        dtype: Literal["numpy", "xarray", "rasterio"] = "numpy",
+    ) -> np.ndarray:
         """Update and get dynamic variable.
 
         Parameters:
             attr_name:
                 The dynamic variable to retrieve.
 
         Returns:
             2D numpy.ndarray data of the variable.
         """
+        # 获取动态变量，及其附加属性
         array = super().dynamic_var(attr_name)
-        # 判断算出来的是一个符合形状的矩阵
-        self._attr_or_array(array)
+        assert isinstance(array, (np.ndarray, xr.DataArray, xr.Dataset))
+        kwargs = super().dynamic_variables[attr_name].attrs
         # 将矩阵转换为三维，并更新空间数据
-        self.apply_raster(array, attr_name=attr_name)
-        return array
+        self.apply_raster(array, attr_name=attr_name, **kwargs)
+        if dtype == "numpy":
+            return self.get_raster(attr_name, update=False)
+        if dtype == "xarray":
+            return self.get_xarray(attr_name, update=False)
+        if dtype == "rasterio":
+            return self.get_rasterio(attr_name, update=False)
+        raise ValueError(f"Unknown expected dtype {dtype}.")
 
     def get_rasterio(
-        self, attr_name: str | None = None
+        self,
+        attr_name: Optional[str] = None,
+        update: bool = True,
     ) -> rasterio.MemoryFile:
         """Gets the Rasterio raster layer corresponding to the attribute. Save to a temporary rasterio memory file.
 
         Parameters:
             attr_name:
                 The attribute name for creating the rasterio file.
 
         Returns:
             The rasterio tmp memory file of raster.
         """
         if attr_name is None:
             data = np.ones(self.shape2d)
         else:
-            data = self.get_raster(attr_name=attr_name)
+            data = self.get_raster(attr_name=attr_name, update=update)
         # 如果获取到的是2维，重整为3维
         if len(data.shape) != 3:
             data = data.reshape(self.shape3d)
         with rasterio.MemoryFile() as mem_file:
             with mem_file.open(
                 driver="GTiff",
                 height=data.shape[1],
@@ -436,27 +476,31 @@
                 crs=self.crs,
                 transform=self.transform,
             ) as dataset:
                 dataset.write(data)
             # Open the dataset again for reading and return
             return mem_file.open()
 
-    def get_xarray(self, attr_name: Optional[str] = None) -> xr.DataArray:
+    def get_xarray(
+        self,
+        attr_name: Optional[str] = None,
+        update: bool = True,
+    ) -> xr.DataArray:
         """Get the xarray raster layer with spatial coordinates.
 
         Parameters:
             attr_name:
                 The attribute to retrieve. If None (by default),
                 return all available attributes (3D DataArray).
                 Otherwise, 2D DataArray of the chosen attribute.
 
         Returns:
             Xarray.DataArray data with spatial coordinates of the chosen attribute.
         """
-        data = self.get_raster(attr_name=attr_name)
+        data = self.get_raster(attr_name=attr_name, update=update)
         if attr_name:
             name = attr_name
             data = data.reshape(self.shape2d)
             coords = self.coords
         else:
             coords = {"variable": list(self.attributes)}
             coords |= self.coords
@@ -466,15 +510,15 @@
             name=name,
             coords=coords,
         ).rio.write_crs(self.crs)
 
     @property
     def random(self) -> ListRandom:
         """Randomly"""
-        return self.select().random
+        return self.cells.random
 
     def _select_by_geometry(
         self,
         geometry: Geometry,
         refer_layer: Optional[str] = None,
         **kwargs: Dict[str, Any],
     ) -> np.ndarray:
@@ -531,15 +575,15 @@
             isinstance(where, (np.ndarray, str, xr.DataArray)) or where is None
         ):
             mask_ = self._attr_or_array(where).reshape(self.shape2d)
         else:
             raise TypeError(
                 f"{type(where)} is not supported for selecting cells."
             )
-        mask_ = np.nan_to_num(mask_, nan=0.0).astype(bool)
+        mask_ = np.nan_to_num(mask_, nan=0.0).astype(bool) & self.mask
         return ActorsList(self.model, self.array_cells[mask_])
 
     sel = select
 
     def apply(
         self, ufunc: Callable[..., Any], *args: Any, **kwargs: Any
     ) -> np.ndarray:
@@ -636,26 +680,30 @@
             self._add_dataarray(data, attr_name, **kwargs)
         elif isinstance(data, xr.Dataset):
             if attr_name is None:
                 raise ValueError("Attribute name is required for xr.Dataset.")
             dataarray = data[attr_name]
             self._add_dataarray(dataarray, attr_name, **kwargs)
 
-    def get_raster(self, attr_name: Optional[str] = None) -> np.ndarray:
+    def get_raster(
+        self,
+        attr_name: Optional[str] = None,
+        update: bool = True,
+    ) -> np.ndarray:
         """Obtaining the Raster layer by attribute.
 
         Parameters:
             attr_name:
                 The attribute to retrieve.
                 If None (by default), retrieve all attributes as a 3D array.
 
         Returns:
             A 3D array of attribute.
         """
-        if attr_name in self._dynamic_variables:
+        if attr_name in self.dynamic_variables and update:
             return self.dynamic_var(attr_name=attr_name).reshape(self.shape3d)
         if attr_name is not None and attr_name not in self.attributes:
             raise ValueError(
                 f"Attribute {attr_name} does not exist. "
                 f"Choose from {self.attributes}, or set `attr_name` to `None` to retrieve all."
             )
         if attr_name is None:
@@ -773,99 +821,7 @@
 
         Returns:
             True if position is off the grid, False otherwise.
         """
 
         row, col = pos
         return row < 0 or row >= self.height or col < 0 or col >= self.width
-
-
-class BaseNature(CompositeModule):
-    """The Base Nature Module.
-    Note:
-        Look at [this tutorial](../tutorial/beginner/organize_model_structure.ipynb) to understand the model structure.
-        This is NOT a raster layer, but can be seen as a container of different raster layers.
-        Users can create new raster layer (i.e., `PatchModule`) by `new` method.
-        By default, an initialized ABSESpy model will init an instance of this `BaseNature` as `nature` module.
-
-    Attributes:
-        major_layer:
-            The major layer of nature module. By default, it's the first layer that user created.
-        total_bounds:
-            The spatial scope of the model's concern. By default, uses the major layer of this model.
-    """
-
-    def __init__(
-        self, model: MainModel[Any, Any], name: str = "nature"
-    ) -> None:
-        CompositeModule.__init__(self, model, name=name)
-        self._major_layer: Optional[PatchModule] = None
-        self._modules = _PatchModuleFactory(self)
-
-        logger.info("Initializing a new Base Nature module...")
-
-    @property
-    def major_layer(self) -> PatchModule | None:
-        """The major layer of nature module.
-        By default, it's the first created layer.
-        """
-        return self._major_layer
-
-    @major_layer.setter
-    def major_layer(self, layer: PatchModule) -> None:
-        if not isinstance(layer, PatchModule):
-            raise TypeError(f"{layer} is not PatchModule.")
-        self._major_layer = layer
-
-    @property
-    def total_bounds(self) -> np.ndarray:
-        """Total bounds. The spatial scope of the model's concern.
-        If None (by default), uses the major layer of this model.
-        Usually, the major layer is the first layer sub-module you created.
-        """
-        if self.major_layer is None:
-            raise ValueError(f"No major layer in {self.modules}.")
-        return self.major_layer.total_bounds
-
-    @property
-    def crs(self) -> pyproj.CRS:
-        """Geo CRS."""
-        return (
-            pyproj.CRS(CRS)
-            if self.major_layer is None
-            else self.major_layer.crs
-        )
-
-    def create_module(
-        self,
-        *args,
-        module_cls: Optional[Type[PatchModule]] = None,
-        major_layer: bool = False,
-        **kwargs: Any,
-    ) -> PatchModule:
-        """Creates a submodule of the raster layer.
-
-        Parameters:
-            module_class:
-                The custom module class.
-            how:
-                Class method to call when creating the new sub-module (raster layer).
-                So far, there are three options:
-                    `from_resolution`: by selecting shape and resolution.
-                    `from_file`: by input of a geo-tiff dataset.
-                    `copy_layer`: by copying shape, resolution, bounds, crs, and coordinates of an existing submodule.
-                if None (by default), just simply create a sub-module without any custom methods (i.e., use the base class `PatchModule`).
-            **kwargs:
-                Any other arg passed to the creation method.
-                See corresponding method of your how option from `PatchModule` class methods.
-
-        Returns:
-            the created new module.
-        """
-        if self.modules.is_empty:
-            major_layer = True
-        module = self.modules.new(module_class=module_cls, *args, **kwargs)
-        # 如果是第一个创建的模块,则将其作为主要的图层
-        if major_layer:
-            self.major_layer = module
-        setattr(self, module.name, module)
-        return module
```

### Comparing `abses-0.5.8/abses/objects.py` & `abses-0.6.0/abses/_bases/objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,20 +7,19 @@
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional
 
 import mesa
 
+from abses._bases.bases import _Observer
+from abses._bases.components import _Component
+from abses._bases.dynamic import _DynamicVariable
 from abses.time import TimeDriver
 
-from .bases import _Observer
-from .components import _Component
-from .dynamic import _DynamicVariable
-
 if TYPE_CHECKING:
     from abses.main import MainModel
 
 
 class _BaseObj(_Observer, _Component):
     """
     Base class for model's objects.
@@ -69,40 +68,38 @@
                 ABSES model object.
         """
         if not isinstance(model, mesa.Model):
             raise TypeError("Model must be an instance of mesa.Model")
         self._model = model
 
     @property
-    def dynamic_variables(self) -> Dict[str, Any]:
+    def dynamic_variables(self) -> Dict[str, _DynamicVariable]:
         """Returns read-only model's dynamic variables.
 
         Returns:
             Dict[str, Any]:
                 Dictionary of model's dynamic variables.
         """
-        if not self._dynamic_variables:
-            return {}
-        return {k: v.now() for k, v in self._dynamic_variables.items()}
+        return self._dynamic_variables
 
     def add_dynamic_variable(
-        self, name: str, data: Any, function: Callable
+        self, name: str, data: Any, function: Callable, **kwargs
     ) -> None:
         """Adds new dynamic variable.
 
         Parameters:
             name:
                 Name of the variable.
             data:
                 Data source for callable function.
             function:
                 Function to calculate the dynamic variable.
         """
         var = _DynamicVariable(
-            obj=self, name=name, data=data, function=function
+            obj=self, name=name, data=data, function=function, **kwargs
         )
         self._dynamic_variables[name] = var
 
     def dynamic_var(self, attr_name: str) -> Any:
         """Returns output of a dynamic variable.
 
         Parameters:
```

### Comparing `abses-0.5.8/abses/random.py` & `abses-0.6.0/abses/random.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,21 +12,22 @@
     TYPE_CHECKING,
     Any,
     Iterable,
     List,
     Literal,
     Optional,
     Tuple,
+    Type,
     Union,
     overload,
 )
 
 import numpy as np
 
-from abses.errors import ABSESpyError
+from abses._bases.errors import ABSESpyError
 from abses.tools.func import make_list
 
 if TYPE_CHECKING:
     from abses.actor import Actor
     from abses.main import MainModel
     from abses.sequences import ActorsList
 
@@ -160,14 +161,31 @@
         )
         return (
             chosen[0]
             if size == 1 and not as_list
             else self._to_actors_list(chosen)
         )
 
+    def new(
+        self,
+        actor_cls: Type[Actor],
+        num: int = 1,
+        replace: bool = False,
+        prob: np.ndarray | None = None,
+        **kwargs,
+    ) -> ActorsList[Actor]:
+        """Randomly creating new agents for a given actor type."""
+        cells = self.choice(as_list=True, size=num, replace=replace, prob=prob)
+        objs = cells.apply(
+            lambda c: c.agents.new(
+                breed_cls=actor_cls, singleton=True, **kwargs
+            )
+        )
+        return self._to_actors_list(objs)
+
     def link(
         self, link: str, p: float = 1.0, mutual: bool = True
     ) -> List[Tuple[Actor, Actor]]:
         """Random build links between actors.
 
         Parameters:
             link:
```

### Comparing `abses-0.5.8/abses/selection.py` & `abses-0.6.0/abses/selection.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.8/abses/sequences.py` & `abses-0.6.0/abses/sequences.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,19 +35,19 @@
 except ImportError:
     from typing_extensions import TypeAlias
 
 import mesa_geo as mg
 import numpy as np
 from numpy.typing import NDArray
 
-from abses.errors import ABSESpyError
+from abses._bases.errors import ABSESpyError
 from abses.random import ListRandom
 from abses.selection import selecting
-
-from .tools.func import make_list
+from abses.tools.func import make_list
+from abses.viz.viz_actors import _VizNodeList
 
 if TYPE_CHECKING:
     from abses.actor import Actor, TargetName
     from abses.links import _LinkNode
     from abses.main import MainModel
 
 Selection: TypeAlias = Union[str, Iterable[bool], Dict[str, bool]]
@@ -110,17 +110,22 @@
                     f"Length of the input {len(length)} mismatch {len(self)} actors."
                 )
             return False
         return True
 
     @cached_property
     def random(self) -> ListRandom:
-        """随机模块"""
+        """Random module"""
         return ListRandom(actors=self, model=self._model)
 
+    @cached_property
+    def plot(self) -> _VizNodeList:
+        """Plotting module"""
+        return _VizNodeList(self)
+
     def to_dict(self) -> Dict[str, ActorsList[Link]]:
         """Convert all actors in this list to a dictionary like {breed: ActorList}.
 
         Returns:
             key is the breed of actors, and values are corresponding actors.
         """
         dic: Dict[str, ActorsList[Link]] = {}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `abses-0.5.8/abses/states.py` & `abses-0.6.0/abses/_bases/states.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.8/abses/time.py` & `abses-0.6.0/abses/time.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 )
 
 import pendulum
 from omegaconf import DictConfig
 from pendulum.datetime import DateTime
 from pendulum.duration import Duration
 
-from abses.components import _Component
+from abses._bases.components import _Component
 
 if TYPE_CHECKING:
     from .main import MainModel
 
 try:
     from typing import Self
 except ImportError:
```

### Comparing `abses-0.5.8/abses/tools/func.py` & `abses-0.6.0/abses/tools/func.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,23 +6,28 @@
 # Website: https://cv.songshgeo.com/
 
 """
 这个模块储存一些
 """
 
 import logging
-from typing import Any, Callable, List
+from functools import wraps
+from typing import Any, Callable, List, Optional, Tuple, TypeVar, cast
 
 import numpy as np
+from matplotlib import pyplot as plt
+from matplotlib.axes import Axes
 from scipy import ndimage
 
 from abses.tools.regex import CAMEL_NAME
 
 logger = logging.getLogger(__name__)
 
+F = TypeVar("F", bound=Callable[..., Any])
+
 
 def get_buffer(
     array: np.ndarray,
     radius: int = 1,
     moor: bool = False,
     annular: bool = False,
 ) -> np.ndarray:
@@ -110,7 +115,40 @@
             The name to convert.
 
     Returns:
         The converted name.
     """
     # https://stackoverflow.com/questions/1175208/elegant-python-function-to-convert-camelcase-to-snake-case
     return CAMEL_NAME.sub("_", name).lower()
+
+
+def with_axes(
+    decorated_func: Optional[F] = None, figsize: Tuple[int, int] = (6, 4)
+) -> Callable[..., Any]:
+    """装饰一个函数/方法，如果该方法接受一个参数叫'ax'并且为None，为其增加一个默认的绘图布。
+
+    Parameters:
+        decorated_func:
+            被装饰的函数，检查是否有参数传递给装饰器，若没有则返回装饰器本身。
+        figsize:
+            图片画布的大小，默认宽度为6，高度为4。
+
+    Returns:
+        被装饰的函数
+    """
+
+    def decorator(func):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            ax = kwargs.get("ax", None)
+            if ax is None:
+                _, ax = plt.subplots(figsize=figsize)
+                kwargs["ax"] = cast(Axes, ax)
+                result = func(*args, **kwargs)
+                return result
+            else:
+                return func(*args, **kwargs)
+
+        return wrapper
+
+    # 检查是否有参数传递给装饰器，若没有则返回装饰器本身
+    return decorator(decorated_func) if decorated_func else decorator
```

### Comparing `abses-0.5.8/abses/tools/regex.py` & `abses-0.6.0/abses/tools/regex.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.8/pyproject.toml` & `abses-0.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -27,32 +27,42 @@
 
 [tool.isort]
 profile = "black"
 line_length = 79
 
 [tool.poetry]
 name = "abses"
-version = "0.5.8"
+version = "0.6.0"
 description = "ABSESpy makes it easier to build artificial Social-ecological systems with real GeoSpatial datasets and fully incorporate human behaviour."
 authors = ["Shuang Song <songshgeo@gmail.com>"]
 license = "Apache 2.0 License"
 readme = "README.md"
+include = [
+  "icons/fa-regular-400.otf",
+  "abses/conf/**/*.yaml",
+  "data/*"
+]
+
+[tool.poetry.plugins."hydra.searchpath"]
+abses = "hydra_plugins.abses_searchpath_plugin:ABSESpySearchPathPlugin"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 netcdf4 = ">=1.6"
 hydra-core = "~1.3"
 mesa-geo = "^0.6.0"
 xarray = "~2023"
 fiona = ">1.8"
 loguru = "~0.7"
 rioxarray = "~0.13"
 pendulum = "~2"
 geopandas = "~0"
 typing-extensions = "^4.10.0"
+fontawesome = "^5.10.1.post1"
+seaborn = "^0.13.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest-clarity = "^1.0.1"
 pre-commit = "^3.0.1"
 scriv = "^1.2.0"
 pytest = "^7.2.1"
 sourcery = "^1.0.6"
```

### Comparing `abses-0.5.8/PKG-INFO` & `abses-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: abses
-Version: 0.5.8
+Version: 0.6.0
 Summary: ABSESpy makes it easier to build artificial Social-ecological systems with real GeoSpatial datasets and fully incorporate human behaviour.
 License: Apache 2.0 License
 Author: Shuang Song
 Author-email: songshgeo@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fiona (>1.8)
+Requires-Dist: fontawesome (>=5.10.1.post1,<6.0.0)
 Requires-Dist: geopandas (>=0,<1)
 Requires-Dist: hydra-core (>=1.3,<1.4)
 Requires-Dist: loguru (>=0.7,<0.8)
 Requires-Dist: mesa-geo (>=0.6.0,<0.7.0)
 Requires-Dist: netcdf4 (>=1.6)
 Requires-Dist: pendulum (>=2,<3)
 Requires-Dist: rioxarray (>=0.13,<0.14)
+Requires-Dist: seaborn (>=0.13.2,<0.14.0)
 Requires-Dist: typing-extensions (>=4.10.0,<5.0.0)
 Requires-Dist: xarray (>=2023,<2024)
 Description-Content-Type: text/markdown
 
 # ABSESpy: Agent-Based Modeling Framework for Social-Ecological Systems
 
 ![ABSES_banner](https://songshgeo-picgo-1302043007.cos.ap-beijing.myqcloud.com/uPic/CleanShot%202023-10-19%20at%2019.08.12@2x.png)
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: abses Version: 0.5.8 Summary: ABSESpy makes it
+Metadata-Version: 2.1 Name: abses Version: 0.6.0 Summary: ABSESpy makes it
 easier to build artificial Social-ecological systems with real GeoSpatial
 datasets and fully incorporate human behaviour. License: Apache 2.0 License
 Author: Shuang Song Author-email: songshgeo@gmail.com Requires-Python:
 >=3.9,<3.12 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: fiona (>1.8) Requires-
-Dist: geopandas (>=0,<1) Requires-Dist: hydra-core (>=1.3,<1.4) Requires-Dist:
-loguru (>=0.7,<0.8) Requires-Dist: mesa-geo (>=0.6.0,<0.7.0) Requires-Dist:
-netcdf4 (>=1.6) Requires-Dist: pendulum (>=2,<3) Requires-Dist: rioxarray
-(>=0.13,<0.14) Requires-Dist: typing-extensions (>=4.10.0,<5.0.0) Requires-
-Dist: xarray (>=2023,<2024) Description-Content-Type: text/markdown # ABSESpy:
-Agent-Based Modeling Framework for Social-Ecological Systems ![ABSES_banner]
-(https://songshgeo-picgo-1302043007.cos.ap-beijing.myqcloud.com/uPic/
-CleanShot%202023-10-19%20at%2019.08.12@2x.png)
+Dist: fontawesome (>=5.10.1.post1,<6.0.0) Requires-Dist: geopandas (>=0,<1)
+Requires-Dist: hydra-core (>=1.3,<1.4) Requires-Dist: loguru (>=0.7,<0.8)
+Requires-Dist: mesa-geo (>=0.6.0,<0.7.0) Requires-Dist: netcdf4 (>=1.6)
+Requires-Dist: pendulum (>=2,<3) Requires-Dist: rioxarray (>=0.13,<0.14)
+Requires-Dist: seaborn (>=0.13.2,<0.14.0) Requires-Dist: typing-extensions
+(>=4.10.0,<5.0.0) Requires-Dist: xarray (>=2023,<2024) Description-Content-
+Type: text/markdown # ABSESpy: Agent-Based Modeling Framework for Social-
+Ecological Systems ![ABSES_banner](https://songshgeo-picgo-1302043007.cos.ap-
+beijing.myqcloud.com/uPic/CleanShot%202023-10-19%20at%2019.08.12@2x.png)
   _[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]_[_S_t_a_r_s_]_[_I_s_s_u_e_s_]_[_R_e_p_o
 _S_i_z_e_]_[_f_o_l_l_o_w_ _o_n_ _T_w_i_t_t_e_r_]_[_g_i_t_h_u_b_]--- Language: [English Readme] | [ç®ä½ä¸­æ]
                                     **[â
                                  âInstallâ
                             â][Install]** **[â
                              âGetting startedâ
                         â][Getting Started]** **[â
```

