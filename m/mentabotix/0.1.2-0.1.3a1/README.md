# Comparing `tmp/mentabotix-0.1.2.tar.gz` & `tmp/mentabotix-0.1.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentabotix-0.1.2.tar", last modified: Mon May  6 10:37:26 2024, max compression
+gzip compressed data, was "mentabotix-0.1.3a1.tar", last modified: Fri May 10 14:52:46 2024, max compression
```

## Comparing `mentabotix-0.1.2.tar` & `mentabotix-0.1.3a1.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0    19747 2024-05-06 10:37:03.911770 mentabotix-0.1.2/README.md
--rw-r--r--   0        0        0      630 2024-05-06 10:37:26.247763 mentabotix-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      847 2024-05-06 10:37:03.915770 mentabotix-0.1.2/src/mentabotix/__init__.py
--rw-r--r--   0        0        0    63015 2024-05-06 10:37:03.915770 mentabotix-0.1.2/src/mentabotix/modules/botix.py
--rw-r--r--   0        0        0      225 2024-05-06 10:37:03.915770 mentabotix-0.1.2/src/mentabotix/modules/exceptions.py
--rw-r--r--   0        0        0      580 2024-05-06 10:37:03.915770 mentabotix-0.1.2/src/mentabotix/modules/logger.py
--rw-r--r--   0        0        0    19645 2024-05-06 10:37:03.915770 mentabotix-0.1.2/src/mentabotix/modules/menta.py
--rw-r--r--   0        0        0     3363 2024-05-06 10:37:03.915770 mentabotix-0.1.2/src/mentabotix/tools/algrithm_tools.py
--rw-r--r--   0        0        0      229 2024-05-06 10:37:03.915770 mentabotix-0.1.2/src/mentabotix/tools/generators.py
--rw-r--r--   0        0        0     5457 2024-05-06 10:37:03.915770 mentabotix-0.1.2/src/mentabotix/vision/camra.py
--rw-r--r--   0        0        0     8336 2024-05-06 10:37:03.915770 mentabotix-0.1.2/src/mentabotix/vision/tagdetector.py
--rw-r--r--   0        0        0        0 2024-05-06 10:37:03.915770 mentabotix-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0    13373 2024-05-06 10:37:03.915770 mentabotix-0.1.2/tests/test_botix.py
--rw-r--r--   0        0        0     8042 2024-05-06 10:37:03.915770 mentabotix-0.1.2/tests/test_menta.py
--rw-r--r--   0        0        0     6488 2024-05-06 10:37:03.915770 mentabotix-0.1.2/tests/test_moving_state.py
--rw-r--r--   0        0        0     5578 2024-05-06 10:37:03.915770 mentabotix-0.1.2/tests/test_moving_transition.py
--rw-r--r--   0        0        0    20179 1970-01-01 00:00:00.000000 mentabotix-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    23777 2024-05-10 14:52:22.743390 mentabotix-0.1.3a1/README.md
+-rw-r--r--   0        0        0      657 2024-05-10 14:52:46.007509 mentabotix-0.1.3a1/pyproject.toml
+-rw-r--r--   0        0        0      974 2024-05-10 14:52:22.743390 mentabotix-0.1.3a1/src/mentabotix/__init__.py
+-rw-r--r--   0        0        0    68552 2024-05-10 14:52:22.743390 mentabotix-0.1.3a1/src/mentabotix/modules/botix.py
+-rw-r--r--   0        0        0      225 2024-05-10 14:52:22.743390 mentabotix-0.1.3a1/src/mentabotix/modules/exceptions.py
+-rw-r--r--   0        0        0      580 2024-05-10 14:52:22.743390 mentabotix-0.1.3a1/src/mentabotix/modules/logger.py
+-rw-r--r--   0        0        0    19645 2024-05-10 14:52:22.743390 mentabotix-0.1.3a1/src/mentabotix/modules/menta.py
+-rw-r--r--   0        0        0     3363 2024-05-10 14:52:22.743390 mentabotix-0.1.3a1/src/mentabotix/tools/algrithm_tools.py
+-rw-r--r--   0        0        0     7500 2024-05-10 14:52:22.743390 mentabotix-0.1.3a1/src/mentabotix/tools/composers.py
+-rw-r--r--   0        0        0      229 2024-05-10 14:52:22.743390 mentabotix-0.1.3a1/src/mentabotix/tools/generators.py
+-rw-r--r--   0        0        0     5457 2024-05-10 14:52:22.743390 mentabotix-0.1.3a1/src/mentabotix/vision/camra.py
+-rw-r--r--   0        0        0     8336 2024-05-10 14:52:22.743390 mentabotix-0.1.3a1/src/mentabotix/vision/tagdetector.py
+-rw-r--r--   0        0        0        0 2024-05-10 14:52:22.743390 mentabotix-0.1.3a1/tests/__init__.py
+-rw-r--r--   0        0        0    15471 2024-05-10 14:52:22.743390 mentabotix-0.1.3a1/tests/test_botix.py
+-rw-r--r--   0        0        0     8569 2024-05-10 14:52:22.747391 mentabotix-0.1.3a1/tests/test_composer.py
+-rw-r--r--   0        0        0     8042 2024-05-10 14:52:22.747391 mentabotix-0.1.3a1/tests/test_menta.py
+-rw-r--r--   0        0        0     6488 2024-05-10 14:52:22.747391 mentabotix-0.1.3a1/tests/test_moving_state.py
+-rw-r--r--   0        0        0     5578 2024-05-10 14:52:22.747391 mentabotix-0.1.3a1/tests/test_moving_transition.py
+-rw-r--r--   0        0        0    24211 1970-01-01 00:00:00.000000 mentabotix-0.1.3a1/PKG-INFO
```

### Comparing `mentabotix-0.1.2/README.md` & `mentabotix-0.1.3a1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: mentabotix
+Version: 0.1.3a1
+Summary: A Bot control lib
+Author-Email: Whth <88489697+Whth@users.noreply.github.com>
+License: MIT
+Requires-Python: >=3.11
+Requires-Dist: coloredlogs>=15.0.1
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: pyapriltags>=3.3.0.3
+Requires-Dist: terminaltables>=3.1.10
+Requires-Dist: bdmc>=0.1.4
+Requires-Dist: opencv-python-headless>=4.9.0.80
+Description-Content-Type: text/markdown
+
 # mentabotix
 
 > A dedicated lib to control 4-fixed-wheels robot
 ---
 
 ## Installation
 
@@ -195,14 +210,21 @@
 
 Welcome to the guide on using Botix for state-transition control schema creation and compilation. This document will
 walk you through the steps to design a control schema using state and transition concepts, and then how to compile those
 schemas into executable closures using the Botix framework.
 
 ### Understanding State-Transition Control Schema
 
+Let's start with the fundamental schema rules:
+> - A `MovingState` **MUST** connect exactly **ONE** `MovingTransition` as its input state.
+>- A `MovingTransition` **MUST** have at least **ONE** `MovingState` as either input or output.
+>- A State-Transition Control Schema **MUST** have **EXACTLY ONE** `MovingState` as its initial state and **AT LEAST ONE
+   ** `MovingState` as its final state.
+>- A State-Transition Control Schema **MUST NOT** have any loop, a correct control schema should always be a tree graph.
+
 Imagine you're designing an autonomous robot that needs to navigate different environments. Each behavior or action the
 robot can take is represented by a **state**, such as "moving forward," "turning left," or "halt." Transitions between
 these states are triggered by events or conditions, forming a **control schema**.
 
 #### States
 
 - In Botix, a state is represented by the `MovingState` class. Each state might have associated actions like setting
@@ -447,15 +469,15 @@
 transition_bc = MovingTransition(duration=2, from_states=state_b, to_states=state_c)
 
 botix = Botix(controller=con)
 botix.token_pool.append(transition_start_a)
 botix.token_pool.append(transition_ab)
 botix.token_pool.append(transition_bc)
 
-# not compile the code into closure, just return the code lines and context, which is human readable.
+# not compile the code into closure, just return the code lines and context, which is human-readable.
 function_closure: Callable[[], None] = botix.compile(return_median=False)
 
 print(function_closure)
 ```
 
 By printing out the `function_closure` object, you can see the compiled code as a closure that can be called
 
@@ -538,16 +560,155 @@
 # compile to closure
 compiled_closure: Callable[[], None] = botix.compile(return_median=False)
 
 # call the closure, which will execute the compiled code
 compiled_closure()
 
 
+
 ```
 
+### Schema Visualization
+
+Botix support schema visualization with `export_structure` method, which write Puml source code to a file.
+
+```python
+from mentabotix import MovingState, MovingTransition, Botix
+from bdmc import CloseLoopController, MotorInfo
+from typing import List
+import random
+
+# init the state-transition schema
+state_a = MovingState(100)
+state_b = MovingState(200)
+state_c = MovingState(300)
+state_d = MovingState(400)
+state_e = MovingState(500)
+state_f = MovingState(600)
+
+
+def transition_breaker_fac(lst: List[int]):
+    def _inner() -> int:
+        return random.choice(lst)
+
+    return _inner
+
+
+transition_a_bcd = MovingTransition(
+    duration=1,
+    from_states=state_a,
+    to_states={1: state_b, 2: state_c, 3: state_d},
+    breaker=transition_breaker_fac([1, 2, 3]),
+)
+transition_d_ef = MovingTransition(
+    duration=1,
+    from_states=state_d,
+    to_states={1: state_e, 2: state_f},
+    breaker=transition_breaker_fac([1, 2]),
+)
+
+# make the botix object
+botix = Botix(controller=CloseLoopController(motor_infos=[MotorInfo(i) for i in range(4)], port="COM3"))
+
+# add the transition
+botix.token_pool.extend([transition_a_bcd, transition_d_ef])
+
+# export the structure
+botix.export_structure("schema.puml")
+```
+
+The result will be written to `schema.puml` and below is the expected Puml source code.
+
+```plantuml
+@startuml
+state "5-MovingState(600, 600, 600, 600)" as state_6
+state "4-MovingState(500, 500, 500, 500)" as state_5
+state break_2 <<choice>>
+note right of break_2: _inner() -> int
+state "3-MovingState(400, 400, 400, 400)" as state_4
+state "2-MovingState(300, 300, 300, 300)" as state_3
+state "1-MovingState(200, 200, 200, 200)" as state_2
+state break_1 <<choice>>
+note right of break_1: _inner() -> int
+state "0-MovingState(100, 100, 100, 100)" as state_1
+state_1 --> break_1
+break_1 --> state_2: 1
+break_1 --> state_3: 2
+break_1 --> state_4: 3
+state_4 --> break_2
+break_2 --> state_5: 1
+break_2 --> state_6: 2
+
+[*] --> state_1
+
+state_2 --> [*]
+state_3 --> [*]
+state_5 --> [*]
+state_6 --> [*]
+
+@enduml
+
+```
+
+Below is the expected render result:
+
+![image](docs/assets/state.png)
+
+### Use State-Transition Composer
+
+State-Transition Composer is a tool that helps you to design and compile state-transition control schema.
+
+```python
+from mentabotix import MovingChainComposer, MovingState, MovingTransition, Botix
+from bdmc import CloseLoopController, MotorInfo
+
+# init the state-transition composer
+comp = MovingChainComposer()
+
+# add some states and transitions one by one to the composer, the composer will auto-connect the states and transitions
+(comp
+ .add(MovingState(0))
+ .add(MovingTransition(0.2))
+ .add(MovingState(1000))
+ .add(MovingTransition(0.3))
+ .add(MovingState(2000)))
+
+# export the structure
+states, transitions = comp.export_structure()
+
+# let's use botix to make the visualization!
+# first make the botix object
+con = CloseLoopController(motor_infos=[MotorInfo(i) for i in range(4)])
+botix = Botix(controller=con)
+
+# make the visualization
+botix.export_structure("composed.puml", transitions=transitions)
+```
+
+The exported structure will be written to `composed.puml`, and below is the expected Puml source code.
+
+```plantuml
+@startuml
+state "3-MovingState(2000, 2000, 2000, 2000)" as state_3
+state "2-MovingState(1000, 1000, 1000, 1000)" as state_2
+state "1-MovingState(0, 0, 0, 0)" as state_1
+state_1 --> state_2
+state_2 --> state_3
+
+[*] --> state_1
+
+state_3 --> [*]
+
+@enduml
+```
+
+The render result is shown below:
+
+![image](docs/assets/composed.png)
+
 ## Logging
 
 use `set_log_level` to silent the console to improve the performance in high pressure conditions
 
 ```python
 from mentabotix import set_log_level
 
@@ -560,8 +721,8 @@
 """
 
 set_log_level(50)  # set the log-level to 50, which makes logger only print the msg important than the CRITICAL logging
 
 from logging import CRITICAL
 
 set_log_level(CRITICAL)  # this has the same effect as above
-```
+```
```

### Comparing `mentabotix-0.1.2/pyproject.toml` & `mentabotix-0.1.3a1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mentabotix"
-version = "0.1.2"
+version = "0.1.3a1"
 description = "A Bot control lib"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "coloredlogs>=15.0.1",
     "numpy>=1.26.4",
@@ -28,8 +28,9 @@
 [tool.pdm]
 distribution = true
 
 [tool.pdm.dev-dependencies]
 dev = [
     "viztracer>=0.16.2",
     "pytest>=8.1.1",
+    "matplotlib>=3.8.4",
 ]
```

### Comparing `mentabotix-0.1.2/src/mentabotix/__init__.py` & `mentabotix-0.1.3a1/src/mentabotix/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from .modules.botix import MovingState, MovingTransition, Botix
 from .modules.exceptions import BadSignatureError, RequirementError, SamplerTypeError, TokenizeError, StructuralError
 from .modules.logger import set_log_level
 from .modules.menta import Menta, SequenceSampler, IndexedSampler, DirectSampler, SamplerUsage, SamplerType, Sampler
+
+from .tools.composers import MovingChainComposer, straight_chain
 from .vision.camra import Camera
 from .vision.tagdetector import TagDetector
 
 __all__ = [
     "set_log_level",
     # botix
     "MovingState",
@@ -24,8 +26,11 @@
     "TagDetector",
     # exceptions
     "BadSignatureError",
     "RequirementError",
     "SamplerTypeError",
     "TokenizeError",
     "StructuralError",
+    # tools
+    "MovingChainComposer",
+    "straight_chain",
 ]
```

### Comparing `mentabotix-0.1.2/src/mentabotix/modules/botix.py` & `mentabotix-0.1.3a1/src/mentabotix/modules/botix.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import inspect
 from collections import Counter
 from dataclasses import dataclass
+from enum import Enum
 from inspect import signature, Signature
 from itertools import zip_longest
 from queue import Queue
 from typing import (
     Tuple,
     TypeAlias,
     Self,
@@ -40,16 +41,28 @@
 IndividualPattern: TypeAlias = Tuple[int, int, int, int]
 FullExpressionPattern: TypeAlias = str
 LRExpressionPattern: TypeAlias = Tuple[Expression, Expression]
 IndividualExpressionPattern: TypeAlias = Tuple[Expression, Expression, Expression, Expression]
 KT = TypeVar("KT", bound=Hashable)
 Context: TypeAlias = Dict[str, Any]
 
-__PLACE_HOLDER__ = "Hello World"
+
+__PLACE_HOLDER__ = 0
 __CONTROLLER_NAME__ = "con"
+__MAGIC_SPLIT_CHAR__ = "$$$"
+
+
+class PatternType(Enum):
+    """
+    Three types of control cmd
+    """
+
+    Full = 1
+    LR = 2
+    Individual = 4
 
 
 def get_function_annotations(func: Callable) -> str:
     """
     Get the function annotations of a given function.
 
     Args:
@@ -134,14 +147,24 @@
         track_width: int = 100
         diagonal_multiplier: float = 1.53
         # TODO: remove the dimensionless feature
 
     __state_id_counter__: ClassVar[int] = 0
 
     @property
+    def pattern_type(self) -> PatternType:
+        """
+        Returns the pattern type of the state.
+
+        Returns:
+            PatternType: The pattern type of the state.
+        """
+        return self._pattern_type
+
+    @property
     def state_id(self) -> int:
         """
         Returns the state identifier.
 
         Returns:
             int: The state identifier.
         """
@@ -164,20 +187,20 @@
 
         :return: An optional list of callables that take no arguments and return None.
         :rtype: Optional[List[Callable[[], None]]]
         """
         return self._after_exiting
 
     @property
-    def used_context_variables(self) -> Set[str]:
+    def used_context_variables(self) -> List[str]:
         """
         Returns the set of context variable names used in the speed expressions.
 
         :return: An optional set of strings representing the context variable names.
-        :rtype: Optional[Set[str]]
+        :rtype: Optional[List[str]]
         """
         return self._used_context_variables
 
     @property
     def speed_expressions(self) -> IndividualExpressionPattern:
         """
         Get the speed expressions of the object.
@@ -187,15 +210,15 @@
         """
         return self._speed_expressions
 
     def __init__(
         self,
         *speeds: Unpack[FullPattern] | Unpack[LRPattern] | Unpack[IndividualPattern],
         speed_expressions: Optional[FullExpressionPattern | LRExpressionPattern | IndividualExpressionPattern] = None,
-        used_context_variables: Optional[Set[str]] = None,
+        used_context_variables: Optional[List[str]] = None,
         before_entering: Optional[List[Callable[[], None]]] = None,
         after_exiting: Optional[List[Callable[[], None]]] = None,
     ) -> None:
         """
         Initialize the MovingState with speeds.
 
         Args:
@@ -203,61 +226,68 @@
                 It should be one of the following types:
                     - FullPattern: A single integer representing full speed for all directions.
                     - LRPattern: A tuple of two integers representing left and right speeds.
                     - IndividualPattern: A tuple of four integers representing individual speeds for each direction.
 
         Keyword Args:
             speed_expressions (Optional[FullExpressionPattern | Unpack[LRExpressionPattern] | Unpack[IndividualExpressionPattern]]): The speed expressions of the wheels.
+            used_context_variables (Optional[List[str]]): The set of context variable names used in the speed expressions.
             before_entering (Optional[List[Callable[[], None]]]): The list of functions to be called before entering the state.
             after_exiting (Optional[List[Callable[[], None]]]): The list of functions to be called after exiting the state.
         Raises:
             ValueError: If the provided speeds do not match any of the above patterns.
         """
         self._speed_expressions: IndividualExpressionPattern
         self._speeds: np.array
-
+        self._pattern_type: PatternType
         match bool(speed_expressions), bool(speeds):
             case True, False:
                 if used_context_variables is None:
                     raise ValueError(
                         "No used_context_variables provided, You must provide a names set that contains all the name of the variables used in the speed_expressions."
                         "If you do not need use context variables, then you should use *speeds argument to create the MovingState."
                     )
                 self._speeds = None
                 match speed_expressions:
                     case str(full_expression):
+                        self._pattern_type = PatternType.Full
                         self._speed_expressions = (full_expression, full_expression, full_expression, full_expression)
                     case (left_expression, right_expression):
                         if all(isinstance(item, int) for item in speed_expressions):
                             raise ValueError(
                                 f"All expressions are integers. You should use *speeds argument to create the MovingState, got {speed_expressions}"
                             )
-
+                        self._pattern_type = PatternType.LR
                         self._speed_expressions = (left_expression, left_expression, right_expression, right_expression)
                     case speed_expressions if len(speed_expressions) == 4:
                         if all(isinstance(item, int) for item in speed_expressions):
                             raise ValueError(
                                 f"All expressions are integers. You should use *speeds argument to create the MovingState, got {speed_expressions}"
                             )
+                        self._pattern_type = PatternType.Individual
                         self._speed_expressions = speed_expressions
                     case _:
                         types = tuple(type(item) for item in speed_expressions)
                         raise ValueError(
                             f"Invalid Speed Expressions. Must be one of [{FullExpressionPattern},{LRExpressionPattern},{IndividualExpressionPattern}], got {types}"
                         )
 
             case False, True:
                 self._speed_expressions = None
                 match speeds:
                     case (int(full_speed),):
+                        self._pattern_type = PatternType.Full
                         self._speeds = np.full((4,), full_speed)
-
                     case (int(left_speed), int(right_speed)):
+                        self._pattern_type = PatternType.LR
+
                         self._speeds = np.array([left_speed, left_speed, right_speed, right_speed])
                     case speeds if len(speeds) == 4 and all(isinstance(item, int) for item in speeds):
+                        self._pattern_type = PatternType.Individual
+
                         self._speeds = np.array(speeds)
                     case _:
                         types = tuple(type(item) for item in speeds)
                         raise ValueError(
                             f"Invalid Speeds. Must be one of [{FullPattern},{LRPattern},{IndividualPattern}], got {types}"
                         )
             case True, True:
@@ -267,27 +297,29 @@
 
             case False, False:
                 raise ValueError(
                     f"Must provide either speeds or speed_expressions, got {speeds} and {speed_expressions}"
                 )
 
         if used_context_variables:
-            self._validate_used_context_variables_presence(used_context_variables, self._speed_expressions)
+            self._validate_used_context_variables(used_context_variables, self._speed_expressions)
         self._before_entering: List[Callable[[], None]] = before_entering
-        self._used_context_variables: Set[str] = used_context_variables
+        self._used_context_variables: List[str] = used_context_variables
         self._after_exiting: List[Callable[[], None]] = after_exiting
         self._identifier: int = MovingState.__state_id_counter__
         MovingState.__state_id_counter__ += 1
 
     @staticmethod
-    def _validate_used_context_variables_presence(
-        used_context_variables: Set[str], speed_expressions: IndividualExpressionPattern
+    def _validate_used_context_variables(
+        used_context_variables: List[str], speed_expressions: IndividualExpressionPattern
     ) -> None:
+        if len(used_context_variables) != len(set(used_context_variables)):
+            raise ValueError(f"used_context_variables can't contain duplicated item!")
         for variable in used_context_variables:
-            if any(variable in expression for expression in speed_expressions):
+            if any(variable in str(expression) for expression in speed_expressions):
                 continue
             raise ValueError(f"Variable {variable} not found in {speed_expressions}.")
 
     @classmethod
     def halt(cls) -> Self:
         """
         Create a new instance of the class with a speed of 0, effectively halting the movement.
@@ -484,37 +516,94 @@
                 if con is None:
                     raise TokenizeError(
                         f"You must parse a CloseLoopController to tokenize a state with expression pattern"
                     )
 
                 getter_function_name_generator = NameGenerator(f"state{self._identifier}_context_getter_")
                 getter_temp_name_generator = NameGenerator(f"state{self._identifier}_context_getter_temp_")
-                input_arg_string = str(tuple(expression)).replace("'", "")
-                for varname in self._used_context_variables:
-                    # Create context retrieval functions using expressions
-                    fn: Callable[[], Any] = con.register_context_getter(varname)
-                    context[(getter_func_var_name := getter_function_name_generator())] = fn
-                    temp_name = getter_temp_name_generator()
-                    if input_arg_string.count(varname) == 1:
-                        input_arg_string = input_arg_string.replace(varname, f"{getter_func_var_name}()", 1)
-                    else:
-                        input_arg_string = input_arg_string.replace(
-                            varname, f"({temp_name}:={getter_func_var_name}())", 1
+                expression_final_value_temp = NameGenerator(f"state{self._identifier}_val_tmp")
+                input_arg_string: str = str(tuple(expression)).replace("'", "")
+
+                match self._pattern_type:
+                    case PatternType.Full:
+                        expression: Tuple[str, str, str, str]
+                        val_temp_name: str = expression_final_value_temp()
+                        full_expression = expression[0]
+                        for varname in self._used_context_variables:
+
+                            # Create context retrieval functions using expressions
+                            fn: Callable[[], Any] = con.register_context_getter(varname)
+                            context[getter_func_var_name := getter_function_name_generator()] = fn
+                            full_expression = self._replace_var(
+                                full_expression, varname, getter_func_var_name, getter_temp_name_generator()
+                            )
+
+                        input_arg_string = (
+                            f"({val_temp_name}:=({full_expression}),{val_temp_name},{val_temp_name},{val_temp_name})"
                         )
-                        input_arg_string = input_arg_string.replace(varname, temp_name)
+                    case PatternType.LR:
+                        expression: IndividualExpressionPattern
+                        l_val_temp_name: str = expression_final_value_temp()
+                        r_val_temp_name: str = expression_final_value_temp()
+                        lr_expression: str = f"{expression[0]}{__MAGIC_SPLIT_CHAR__}{expression[-1]}"
+                        for varname in self._used_context_variables:
+
+                            # Create context retrieval functions using expressions
+                            fn: Callable[[], Any] = con.register_context_getter(varname)
+                            context[getter_func_var_name := getter_function_name_generator()] = fn
+                            lr_expression = self._replace_var(
+                                lr_expression, varname, getter_func_var_name, getter_temp_name_generator()
+                            )
+                        left_expression, right_expression = lr_expression.split(__MAGIC_SPLIT_CHAR__)
+
+                        match isinstance(expression[0], int), isinstance(expression[-1], int):
+                            case True, True:
+                                raise TokenizeError(f"Should never be here!")
+                            case False, False:
+
+                                input_arg_string = f"({l_val_temp_name}:=({left_expression}),{l_val_temp_name},{r_val_temp_name}:=({right_expression}),{r_val_temp_name})"
+                            case False, True:
+                                input_arg_string = f"({l_val_temp_name}:=({left_expression}),{l_val_temp_name},{right_expression},{right_expression})"
+                            case True, False:
+                                input_arg_string = f"({left_expression},{left_expression},{r_val_temp_name}:=({right_expression}),{r_val_temp_name})"
+
+                    case PatternType.Individual:
+                        for varname in self._used_context_variables:
+
+                            # Create context retrieval functions using expressions
+                            fn: Callable[[], Any] = con.register_context_getter(varname)
+                            context[(getter_func_var_name := getter_function_name_generator())] = fn
+                            temp_name = getter_temp_name_generator()
+
+                            if input_arg_string.count(varname) == 1:
+                                input_arg_string = input_arg_string.replace(varname, f"{getter_func_var_name}()", 1)
+                            else:
+                                input_arg_string = input_arg_string.replace(
+                                    varname, f"({temp_name}:={getter_func_var_name}())", 1
+                                )
+                                input_arg_string = input_arg_string.replace(varname, temp_name)
+                    case _:
+                        raise TokenizeError(f"Unknown expression type, got {self._pattern_type}")
                 state_tokens.append(f".set_motors_speed({input_arg_string})")
 
             case None, speeds:
                 state_tokens.append(f".set_motors_speed({tuple(speeds)})")
             case _:
-                raise RuntimeError("should never reach here")
+                raise TokenizeError("should never reach here")
 
         tokens: List[str] = before_enter_tokens + state_tokens + after_exiting_tokens
         return tokens, context
 
+    @staticmethod
+    def _replace_var(source: str, var_name: str, func_name: str, temp_name: str) -> str:
+        if source.count(var_name) == 1:
+            return source.replace(var_name, f"{func_name}()", 1)
+        else:
+            return source.replace(var_name, f"({temp_name}:={func_name}())", 1).replace(var_name, temp_name)
+
     def __hash__(self) -> int:
         return self._identifier
 
     def __eq__(self, other: Self) -> bool:
         return tuple(self._speeds) == tuple(other._speeds) and self._speed_expressions == other._speed_expressions
 
     def __str__(self):
@@ -633,24 +722,31 @@
 
         Returns:
             Tuple[List[str], Context]: A tuple containing a list of tokens and a context dictionary.
         """
         tokens: List[str] = []
         context: Context = {}
         name_generator: NameGenerator = NameGenerator(f"transition{self._transition_id}_breaker_")
-        context[(breaker_name := name_generator())] = self.breaker
         match len(self.to_states):
             case 0:
                 raise TokenizeError(f"Transition must have at least one to_state, got {self.to_states}.")
             case 1 if not callable(self.breaker):
                 tokens.append(f".delay({self.duration})")
             case 1 if callable(self.breaker):
+                context[(breaker_name := name_generator())] = self.breaker
                 tokens.append(f".delay_b({self.duration},{breaker_name},{self.check_interval})")
             case length if length > 1 and callable(self.breaker):
+                context[(breaker_name := name_generator())] = self.breaker
                 tokens.append(f".delay_b_match({self.duration},{breaker_name},{self.check_interval})")
+            case length if length > 1 and not callable(self.breaker):
+                raise TokenizeError(
+                    f"got branching states {self.to_states}, but not give correct breaker, {self.breaker} is not a callable."
+                )
+            case _:
+                raise TokenizeError(f"Undefined Error, got {self.to_states} and {self.breaker}.")
         return tokens, context
 
     def clone(self) -> Self:
         """
         Clones the current `MovingTransition` object and returns a new instance with the same values.
 
         Returns:
@@ -677,16 +773,21 @@
         return self._transition_id
 
 
 TokenPool: TypeAlias = List[MovingTransition]
 
 
 class Botix:
+    """
+    Args:
+        *controller* : A `CloseLoopController` object that represents the bot's controller.
+        *token_pool* : A `TokenPool` object that represents the bot's token pool.
+    """
 
-    def __init__(self, controller: CloseLoopController, token_pool: Optional[List[MovingTransition]] = None):
+    def __init__(self, controller: CloseLoopController, token_pool: Optional[TokenPool] = None):
         self.controller: CloseLoopController = controller
         self.token_pool: TokenPool = token_pool or []
 
     def acquire_unique_start(self, token_pool: TokenPool, none_check: bool = True) -> MovingState | None:
         """
         Retrieves a unique starting state from the given token pool.
 
@@ -1058,30 +1159,31 @@
         self.ensure_structure_validity(self.token_pool)
         start_state = self.acquire_unique_start(self.token_pool)
         end_states = self.acquire_end_states(self.token_pool)
         self.ensure_accessibility(self.token_pool, start_state, end_states)
         if self.acquire_loops():
             raise ValueError("Loops detected! All State-Transition should be implemented using breaker")
 
-    def _assembly_match_cases(self, match_expression: str | List[str], cases: Dict[str, str | List[str]]) -> List[str]:
+    def _assembly_match_cases(self, match_expression: str | List[str], cases: Dict[KT, str | List[str]]) -> List[str]:
         """
         Assembles a list of strings representing match cases based on the given match expression and cases dictionary.
 
         Parameters:
             match_expression (str): The match expression to be used.
             cases (Dict[str, str]): A dictionary containing the cases and their corresponding values.
 
         Returns:
             List[str]: A list of strings representing the match cases.
         """
         match_expression = "".join(match_expression) if isinstance(match_expression, list) else match_expression
 
         lines: List[str] = [f"match {match_expression}:"]
         for key, value in cases.items():
-            lines.append(self._add_indent(f"case {key}:", count=1))
+            case_expr: str = f"'{key}'" if isinstance(key, str) else f"{key}"
+            lines.append(self._add_indent(f"case {case_expr}:", count=1))
             lines.extend(self._add_indent(value.split("\n") if isinstance(value, str) else value, count=2))
         return lines
 
     @staticmethod
     def _add_indent(lines: T_EXPR, indent: str = "    ", count: int = 1) -> T_EXPR:
         """
         Adds an indent to each line in the given list of lines or string.
@@ -1222,17 +1324,17 @@
             case ([*_, last_state], _) if connected_forward_transition := self.acquire_connected_forward_transition(
                 last_state, none_check=False
             ):
 
                 branch_transition, branch_context = connected_forward_transition.tokenize()
                 context.update(branch_context)
                 match_expr = line + "".join(branch_transition)
-                match_branch: Dict[str, List[str]] = {}
+                match_branch: Dict[KT, List[str]] = {}
                 for case, value in connected_forward_transition.to_states.items():
-                    match_branch[str(case)] = self._recursive_compile_tokens(
+                    match_branch[case] = self._recursive_compile_tokens(
                         start=value, context=context, controller_name=controller_name
                     )
                 lines = self._assembly_match_cases(match_expression=match_expr, cases=match_branch)
                 return lines
             case _:
                 compiled_lines.append(line)
                 # If no forward transition is present, return the compiled lines
@@ -1276,14 +1378,17 @@
                         lines.insert(0, f'state "{to_state}" as {to_state_alias}\n')
                     else:
                         to_state_alias = used_state.get(to_state)
                     lines.append(f"{from_state_alias} --> {to_state_alias}\n")
                 else:
                     break_node_name: str = break_gen()
                     lines.insert(0, f"state {break_node_name} <<choice>>\n")
+                    lines.insert(
+                        1, f"note right of {break_node_name}: {get_function_annotations(transition.breaker)}\n"
+                    )
                     lines.append(f"{from_state_alias} --> {break_node_name}\n")
                     for case_name, to_state in transition.to_states.items():
 
                         if to_state not in used_state:
                             to_state_alias: str = name_gen()
                             used_state[to_state] = to_state_alias
                             lines.insert(0, f'state "{to_state}" as {to_state_alias}\n')
```

### Comparing `mentabotix-0.1.2/src/mentabotix/modules/logger.py` & `mentabotix-0.1.3a1/src/mentabotix/modules/logger.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.2/src/mentabotix/modules/menta.py` & `mentabotix-0.1.3a1/src/mentabotix/modules/menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.2/src/mentabotix/tools/algrithm_tools.py` & `mentabotix-0.1.3a1/src/mentabotix/tools/algrithm_tools.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.2/src/mentabotix/vision/camra.py` & `mentabotix-0.1.3a1/src/mentabotix/vision/camra.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.2/src/mentabotix/vision/tagdetector.py` & `mentabotix-0.1.3a1/src/mentabotix/vision/tagdetector.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.2/tests/test_botix.py` & `mentabotix-0.1.3a1/tests/test_botix.py`

 * *Files 22% similar despite different names*

```diff
@@ -217,18 +217,18 @@
         input_string = "line1\nline2"
         expected_output_string = "    line1\n    line2"
         self.assertEqual(test_instance._add_indent(input_string, count=1), expected_output_string)
 
         # Test _assembly_match_cases
         expected_match_cases = [
             "match some_variable:",
-            "    case case1:",
+            "    case 'case1':",
             "        result1",
             "            more_result1",
-            "    case case2:",
+            "    case 'case2':",
             "        result2",
         ]
         self.assertEqual(test_instance._assembly_match_cases(match_expression, cases), expected_match_cases)
 
         # Test _add_indent TypeError
         with self.assertRaises(TypeError):
             test_instance._add_indent(123)  # This should raise a TypeError
@@ -325,10 +325,34 @@
             from_states=state_d,
             to_states={1: state_e, 2: state_f},
             breaker=transition_breaker_fac([1, 2]),
         )
         self.botix_instance.token_pool = [transition_a_bcd, transition_d_ef]
         self.botix_instance.export_structure("test.puml")
 
+    def test_compile_expressions(self):
+        MovingState.__state_id_counter__ = 0
+        MovingTransition.__state_id_counter__ = 0
+
+        state_a = MovingState(speed_expressions="var1", used_context_variables=["var1"])
+        state_b = MovingState(speed_expressions=("var1", "var2"), used_context_variables=["var1", "var2"])
+        state_c = MovingState(
+            speed_expressions=("var1", "var2", "var3", "var4"), used_context_variables=["var1", "var2", "var3", "var4"]
+        )
+        state_d = MovingState(speed_expressions=("var1", 100), used_context_variables=["var1"])
+        state_e = MovingState(
+            speed_expressions=("var1", "var2", "var3", 666), used_context_variables=["var1", "var2", "var3"]
+        )
+        state_f = MovingState(speed_expressions=(500, "var1"), used_context_variables=["var1"])
+
+        state_g = MovingState(speed_expressions=("var1", "var2*var1"), used_context_variables=["var1", "var2"])
+        states = [state_a, state_b, state_c, state_d, state_e, state_f, state_g]
+        std_out = ""
+        for state in states:
+            std_out += str(state.tokenize(self.botix_instance.controller)[0][0])
+
+        correct = ".set_motors_speed((state0_val_tmp1:=(state0_context_getter_1()),state0_val_tmp1,state0_val_tmp1,state0_val_tmp1)).set_motors_speed((state1_val_tmp1:=(state1_context_getter_1()),state1_val_tmp1,state1_val_tmp2:=(state1_context_getter_2()),state1_val_tmp2)).set_motors_speed((state2_context_getter_1(), state2_context_getter_2(), state2_context_getter_3(), state2_context_getter_4())).set_motors_speed((state3_val_tmp1:=(state3_context_getter_1()),state3_val_tmp1,100,100)).set_motors_speed((state4_context_getter_1(), state4_context_getter_2(), state4_context_getter_3(), 666)).set_motors_speed((500,500,state5_val_tmp2:=(state5_context_getter_1()),state5_val_tmp2)).set_motors_speed((state6_val_tmp1:=((state6_context_getter_temp_1:=state6_context_getter_1())),state6_val_tmp1,state6_val_tmp2:=(state6_context_getter_2()*state6_context_getter_temp_1),state6_val_tmp2))"
+        self.assertEqual(correct, std_out)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `mentabotix-0.1.2/tests/test_menta.py` & `mentabotix-0.1.3a1/tests/test_menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.2/tests/test_moving_state.py` & `mentabotix-0.1.3a1/tests/test_moving_state.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self.assertEqual(state_lr.unwrap(), (30, 30, 60, 60))
 
         # Test IndividualPattern
         state_individual = MovingState(10, 20, 30, 40)
         self.assertEqual(state_individual.unwrap(), (10, 20, 30, 40))
 
     def test_init_speed_expressions(self):
-        used_context_variables = {"var1", "var2"}
+        used_context_variables = ["var1", "var2"]
 
         # Test FullExpressionPattern
         state_full_expr = MovingState(speed_expressions="var1+var2", used_context_variables=used_context_variables)
         self.assertEqual(state_full_expr.speed_expressions, ("var1+var2", "var1+var2", "var1+var2", "var1+var2"))
 
         # Test LRExpressionPattern
         state_lr_expr = MovingState(speed_expressions=("var1", "var2"), used_context_variables=used_context_variables)
@@ -46,15 +46,15 @@
         with self.assertRaises(ValueError):
             MovingState()
 
         with self.assertRaises(ValueError):
             MovingState(1, 2, 3, 5, speed_expressions=("expr1", "expr2"))
 
         with self.assertRaises(ValueError):
-            MovingState(speed_expressions=("expr1", "expr2"), used_context_variables={"var1", "var2"})
+            MovingState(speed_expressions=("expr1", "expr2"), used_context_variables=["var1", "var2"])
 
     def test_class_methods(self):
         # Test halt
         state_halt = MovingState.halt()
         self.assertEqual(state_halt.unwrap(), (0, 0, 0, 0))
 
         # Test straight
@@ -98,26 +98,26 @@
         self.assertEqual(cloned_state.unwrap(), (10, 20, 30, 40))
         self.assertIsNot(cloned_state, original_state)  # Ensure a new instance is returned
 
     def test_tokenize(self):
 
         con_mock = Mock(
             spec=CloseLoopController(
-                [MotorInfo(1), MotorInfo(2), MotorInfo(3), MotorInfo(4)], port="COM3", context={"var1": 10, "var2": 20}
+                [MotorInfo(1), MotorInfo(2), MotorInfo(3), MotorInfo(4)], port="COM4", context={"var1": 10, "var2": 20}
             )
         )
 
         state_with_speeds = MovingState(10, 20, 30, 40)
         tokens, context = state_with_speeds.tokenize(con_mock)
         self.assertEqual(tokens, [".set_motors_speed((10, 20, 30, 40))"])
         self.assertEqual(context, {})  # No context needed for states with speeds
 
         state_with_expressions = MovingState(
             speed_expressions=("var1", "var2", "var1+var2", "2*var1-var2"),
-            used_context_variables={"var1", "var2"},
+            used_context_variables=["var1", "var2"],
         )
         tokens, context = state_with_expressions.tokenize(con_mock)
         self.assertCountEqual(
             [
                 ".set_motors_speed(((state1_context_getter_temp_2:=state1_context_getter_2()), "
                 "(state1_context_getter_temp_1:=state1_context_getter_1()), "
                 "state1_context_getter_temp_2+state1_context_getter_temp_1, "
@@ -145,13 +145,13 @@
 
         self.assertEqual(state1, state2)
         self.assertNotEqual(state1, state3)
 
     def test_str(self):
         state = MovingState(10, 20, 30, 40)
         self.assertEqual(str(state), f"{state.state_id}-MovingState(10, 20, 30, 40)")
-        state = MovingState(speed_expressions="var1", used_context_variables={"var1"})
+        state = MovingState(speed_expressions="var1", used_context_variables=["var1"])
         self.assertEqual(str(state), f"{state.state_id}-MovingState('var1', 'var1', 'var1', 'var1')")
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `mentabotix-0.1.2/tests/test_moving_transition.py` & `mentabotix-0.1.3a1/tests/test_moving_transition.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.2/PKG-INFO` & `mentabotix-0.1.3a1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: mentabotix
-Version: 0.1.2
-Summary: A Bot control lib
-Author-Email: Whth <88489697+Whth@users.noreply.github.com>
-License: MIT
-Requires-Python: >=3.11
-Requires-Dist: coloredlogs>=15.0.1
-Requires-Dist: numpy>=1.26.4
-Requires-Dist: pyapriltags>=3.3.0.3
-Requires-Dist: terminaltables>=3.1.10
-Requires-Dist: bdmc>=0.1.4
-Requires-Dist: opencv-python-headless>=4.9.0.80
-Description-Content-Type: text/markdown
-
 # mentabotix
 
 > A dedicated lib to control 4-fixed-wheels robot
 ---
 
 ## Installation
 
@@ -210,14 +195,21 @@
 
 Welcome to the guide on using Botix for state-transition control schema creation and compilation. This document will
 walk you through the steps to design a control schema using state and transition concepts, and then how to compile those
 schemas into executable closures using the Botix framework.
 
 ### Understanding State-Transition Control Schema
 
+Let's start with the fundamental schema rules:
+> - A `MovingState` **MUST** connect exactly **ONE** `MovingTransition` as its input state.
+>- A `MovingTransition` **MUST** have at least **ONE** `MovingState` as either input or output.
+>- A State-Transition Control Schema **MUST** have **EXACTLY ONE** `MovingState` as its initial state and **AT LEAST ONE
+   ** `MovingState` as its final state.
+>- A State-Transition Control Schema **MUST NOT** have any loop, a correct control schema should always be a tree graph.
+
 Imagine you're designing an autonomous robot that needs to navigate different environments. Each behavior or action the
 robot can take is represented by a **state**, such as "moving forward," "turning left," or "halt." Transitions between
 these states are triggered by events or conditions, forming a **control schema**.
 
 #### States
 
 - In Botix, a state is represented by the `MovingState` class. Each state might have associated actions like setting
@@ -462,15 +454,15 @@
 transition_bc = MovingTransition(duration=2, from_states=state_b, to_states=state_c)
 
 botix = Botix(controller=con)
 botix.token_pool.append(transition_start_a)
 botix.token_pool.append(transition_ab)
 botix.token_pool.append(transition_bc)
 
-# not compile the code into closure, just return the code lines and context, which is human readable.
+# not compile the code into closure, just return the code lines and context, which is human-readable.
 function_closure: Callable[[], None] = botix.compile(return_median=False)
 
 print(function_closure)
 ```
 
 By printing out the `function_closure` object, you can see the compiled code as a closure that can be called
 
@@ -553,16 +545,155 @@
 # compile to closure
 compiled_closure: Callable[[], None] = botix.compile(return_median=False)
 
 # call the closure, which will execute the compiled code
 compiled_closure()
 
 
+
 ```
 
+### Schema Visualization
+
+Botix support schema visualization with `export_structure` method, which write Puml source code to a file.
+
+```python
+from mentabotix import MovingState, MovingTransition, Botix
+from bdmc import CloseLoopController, MotorInfo
+from typing import List
+import random
+
+# init the state-transition schema
+state_a = MovingState(100)
+state_b = MovingState(200)
+state_c = MovingState(300)
+state_d = MovingState(400)
+state_e = MovingState(500)
+state_f = MovingState(600)
+
+
+def transition_breaker_fac(lst: List[int]):
+    def _inner() -> int:
+        return random.choice(lst)
+
+    return _inner
+
+
+transition_a_bcd = MovingTransition(
+    duration=1,
+    from_states=state_a,
+    to_states={1: state_b, 2: state_c, 3: state_d},
+    breaker=transition_breaker_fac([1, 2, 3]),
+)
+transition_d_ef = MovingTransition(
+    duration=1,
+    from_states=state_d,
+    to_states={1: state_e, 2: state_f},
+    breaker=transition_breaker_fac([1, 2]),
+)
+
+# make the botix object
+botix = Botix(controller=CloseLoopController(motor_infos=[MotorInfo(i) for i in range(4)], port="COM3"))
+
+# add the transition
+botix.token_pool.extend([transition_a_bcd, transition_d_ef])
+
+# export the structure
+botix.export_structure("schema.puml")
+```
+
+The result will be written to `schema.puml` and below is the expected Puml source code.
+
+```plantuml
+@startuml
+state "5-MovingState(600, 600, 600, 600)" as state_6
+state "4-MovingState(500, 500, 500, 500)" as state_5
+state break_2 <<choice>>
+note right of break_2: _inner() -> int
+state "3-MovingState(400, 400, 400, 400)" as state_4
+state "2-MovingState(300, 300, 300, 300)" as state_3
+state "1-MovingState(200, 200, 200, 200)" as state_2
+state break_1 <<choice>>
+note right of break_1: _inner() -> int
+state "0-MovingState(100, 100, 100, 100)" as state_1
+state_1 --> break_1
+break_1 --> state_2: 1
+break_1 --> state_3: 2
+break_1 --> state_4: 3
+state_4 --> break_2
+break_2 --> state_5: 1
+break_2 --> state_6: 2
+
+[*] --> state_1
+
+state_2 --> [*]
+state_3 --> [*]
+state_5 --> [*]
+state_6 --> [*]
+
+@enduml
+
+```
+
+Below is the expected render result:
+
+![image](docs/assets/state.png)
+
+### Use State-Transition Composer
+
+State-Transition Composer is a tool that helps you to design and compile state-transition control schema.
+
+```python
+from mentabotix import MovingChainComposer, MovingState, MovingTransition, Botix
+from bdmc import CloseLoopController, MotorInfo
+
+# init the state-transition composer
+comp = MovingChainComposer()
+
+# add some states and transitions one by one to the composer, the composer will auto-connect the states and transitions
+(comp
+ .add(MovingState(0))
+ .add(MovingTransition(0.2))
+ .add(MovingState(1000))
+ .add(MovingTransition(0.3))
+ .add(MovingState(2000)))
+
+# export the structure
+states, transitions = comp.export_structure()
+
+# let's use botix to make the visualization!
+# first make the botix object
+con = CloseLoopController(motor_infos=[MotorInfo(i) for i in range(4)])
+botix = Botix(controller=con)
+
+# make the visualization
+botix.export_structure("composed.puml", transitions=transitions)
+```
+
+The exported structure will be written to `composed.puml`, and below is the expected Puml source code.
+
+```plantuml
+@startuml
+state "3-MovingState(2000, 2000, 2000, 2000)" as state_3
+state "2-MovingState(1000, 1000, 1000, 1000)" as state_2
+state "1-MovingState(0, 0, 0, 0)" as state_1
+state_1 --> state_2
+state_2 --> state_3
+
+[*] --> state_1
+
+state_3 --> [*]
+
+@enduml
+```
+
+The render result is shown below:
+
+![image](docs/assets/composed.png)
+
 ## Logging
 
 use `set_log_level` to silent the console to improve the performance in high pressure conditions
 
 ```python
 from mentabotix import set_log_level
 
@@ -575,8 +706,8 @@
 """
 
 set_log_level(50)  # set the log-level to 50, which makes logger only print the msg important than the CRITICAL logging
 
 from logging import CRITICAL
 
 set_log_level(CRITICAL)  # this has the same effect as above
-```
+```
```

