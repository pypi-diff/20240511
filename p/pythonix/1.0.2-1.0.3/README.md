# Comparing `tmp/pythonix-1.0.2.tar.gz` & `tmp/pythonix-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonix-1.0.2.tar", max compression
+gzip compressed data, was "pythonix-1.0.3.tar", max compression
```

## Comparing `pythonix-1.0.2.tar` & `pythonix-1.0.3.tar`

### file list

```diff
@@ -1,34 +1,26 @@
--rw-r--r--   0        0        0     3027 2024-05-08 15:06:58.839631 pythonix-1.0.2/README.md
--rw-r--r--   0        0        0      284 2024-05-08 15:07:57.059631 pythonix-1.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-13 01:39:00.350000 pythonix-1.0.2/pythonix/__init__.py
--rw-r--r--   0        0        0       84 2024-05-08 15:00:35.669631 pythonix-1.0.2/pythonix/curry.py
--rw-r--r--   0        0        0     5348 2024-04-25 15:52:31.904118 pythonix-1.0.2/pythonix/internals/__pycache__/op.cpython-312.pyc
--rw-r--r--   0        0        0     2421 2024-04-18 01:37:05.054118 pythonix-1.0.2/pythonix/internals/__pycache__/ops.cpython-312.pyc
--rw-r--r--   0        0        0     4967 2024-04-25 15:54:40.194118 pythonix-1.0.2/pythonix/internals/__pycache__/pair.cpython-312.pyc
--rw-r--r--   0        0        0     7799 2024-04-22 17:28:53.444118 pythonix-1.0.2/pythonix/internals/__pycache__/pipe.cpython-312.pyc
--rw-r--r--   0        0        0     7141 2024-04-18 01:37:05.044118 pythonix-1.0.2/pythonix/internals/__pycache__/pipes.cpython-312.pyc
--rw-r--r--   0        0        0    13646 2024-04-25 15:46:38.174118 pythonix-1.0.2/pythonix/internals/__pycache__/req.cpython-312.pyc
--rw-r--r--   0        0        0    10297 2024-04-23 19:30:10.434118 pythonix-1.0.2/pythonix/internals/__pycache__/request.cpython-312.pyc
--rw-r--r--   0        0        0    22954 2024-04-25 16:07:26.584118 pythonix-1.0.2/pythonix/internals/__pycache__/res.cpython-312.pyc
--rw-r--r--   0        0        0     7175 2024-04-25 16:23:02.564118 pythonix-1.0.2/pythonix/internals/__pycache__/trail.cpython-312.pyc
--rw-r--r--   0        0        0      817 2024-04-25 17:35:02.224118 pythonix-1.0.2/pythonix/internals/__pycache__/types.cpython-312.pyc
--rw-r--r--   0        0        0     8183 2024-05-08 15:01:24.259631 pythonix-1.0.2/pythonix/internals/curry.py
--rw-r--r--   0        0        0     3915 2024-05-08 14:33:57.509631 pythonix-1.0.2/pythonix/internals/mdeq.py
--rw-r--r--   0        0        0     2596 2024-05-08 03:48:32.109631 pythonix-1.0.2/pythonix/internals/op.py
--rw-r--r--   0        0        0     1376 2024-05-08 15:04:34.579631 pythonix-1.0.2/pythonix/internals/pair.py
--rw-r--r--   0        0        0     4169 2024-05-08 14:18:48.939631 pythonix-1.0.2/pythonix/internals/pipe.py
--rw-r--r--   0        0        0     7385 2024-05-08 14:37:25.509631 pythonix-1.0.2/pythonix/internals/req.py
--rw-r--r--   0        0        0    12034 2024-05-08 14:07:35.969631 pythonix-1.0.2/pythonix/internals/res.py
--rw-r--r--   0        0        0     2251 2024-05-08 14:22:48.329631 pythonix-1.0.2/pythonix/internals/trail.py
--rw-r--r--   0        0        0     2697 2024-05-08 14:35:33.779631 pythonix-1.0.2/pythonix/internals/tuple.py
--rw-r--r--   0        0        0      178 2024-05-08 15:06:04.479631 pythonix-1.0.2/pythonix/internals/types.py
--rw-r--r--   0        0        0      206 2024-04-23 18:09:04.734118 pythonix-1.0.2/pythonix/mdeq.py
--rw-r--r--   0        0        0       69 2024-04-22 17:26:16.504118 pythonix-1.0.2/pythonix/op.py
--rw-r--r--   0        0        0      133 2024-04-23 19:02:18.274118 pythonix-1.0.2/pythonix/pair.py
--rw-r--r--   0        0        0      886 2024-04-18 16:47:23.234118 pythonix-1.0.2/pythonix/pipe.py
--rw-r--r--   0        0        0      246 2024-05-08 15:06:15.069631 pythonix-1.0.2/pythonix/prelude.py
--rw-r--r--   0        0        0      644 2024-04-25 15:40:16.334118 pythonix-1.0.2/pythonix/req.py
--rw-r--r--   0        0        0      425 2024-04-22 18:27:24.324118 pythonix-1.0.2/pythonix/res.py
--rw-r--r--   0        0        0      183 2024-04-25 18:08:10.144118 pythonix-1.0.2/pythonix/trail.py
--rw-r--r--   0        0        0      181 2024-04-22 17:55:20.064118 pythonix-1.0.2/pythonix/tuple.py
--rw-r--r--   0        0        0     3402 1970-01-01 00:00:00.000000 pythonix-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3027 2024-05-08 15:21:18.899631 pythonix-1.0.3/README.md
+-rw-r--r--   0        0        0      380 2024-05-11 15:46:30.309631 pythonix-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-13 01:39:00.350000 pythonix-1.0.3/pythonix/__init__.py
+-rw-r--r--   0        0        0       85 2024-05-09 16:54:03.549631 pythonix-1.0.3/pythonix/curry.py
+-rw-r--r--   0        0        0      107 2024-05-11 15:40:12.579631 pythonix-1.0.3/pythonix/dict_utils.py
+-rw-r--r--   0        0        0     8292 2024-05-09 16:54:03.899631 pythonix-1.0.3/pythonix/internals/curry.py
+-rw-r--r--   0        0        0     4186 2024-05-11 15:40:07.379631 pythonix-1.0.3/pythonix/internals/dict_utils.py
+-rw-r--r--   0        0        0     3914 2024-05-09 16:54:03.669631 pythonix-1.0.3/pythonix/internals/mdeq.py
+-rw-r--r--   0        0        0     2877 2024-05-11 15:23:07.359631 pythonix-1.0.3/pythonix/internals/op.py
+-rw-r--r--   0        0        0     1381 2024-05-09 16:54:03.599631 pythonix-1.0.3/pythonix/internals/pair.py
+-rw-r--r--   0        0        0     4518 2024-05-09 21:32:52.849631 pythonix-1.0.3/pythonix/internals/pipe.py
+-rw-r--r--   0        0        0     7290 2024-05-09 16:54:03.759631 pythonix-1.0.3/pythonix/internals/req.py
+-rw-r--r--   0        0        0    12636 2024-05-09 21:54:17.529631 pythonix-1.0.3/pythonix/internals/res.py
+-rw-r--r--   0        0        0     2251 2024-05-09 16:55:17.189631 pythonix-1.0.3/pythonix/internals/trail.py
+-rw-r--r--   0        0        0     2696 2024-05-09 20:50:48.239631 pythonix-1.0.3/pythonix/internals/tup.py
+-rw-r--r--   0        0        0      178 2024-05-09 16:54:03.619631 pythonix-1.0.3/pythonix/internals/types.py
+-rw-r--r--   0        0        0      207 2024-05-09 16:54:03.619631 pythonix-1.0.3/pythonix/mdeq.py
+-rw-r--r--   0        0        0       74 2024-05-11 15:23:19.849631 pythonix-1.0.3/pythonix/op.py
+-rw-r--r--   0        0        0      135 2024-05-09 16:54:03.619631 pythonix-1.0.3/pythonix/pair.py
+-rw-r--r--   0        0        0      886 2024-04-18 16:47:23.234118 pythonix-1.0.3/pythonix/pipe.py
+-rw-r--r--   0        0        0      349 2024-05-11 15:45:04.599631 pythonix-1.0.3/pythonix/prelude.py
+-rw-r--r--   0        0        0      645 2024-05-09 16:54:03.639631 pythonix-1.0.3/pythonix/req.py
+-rw-r--r--   0        0        0      446 2024-05-09 21:54:26.459631 pythonix-1.0.3/pythonix/res.py
+-rw-r--r--   0        0        0      183 2024-04-25 18:08:10.144118 pythonix-1.0.3/pythonix/trail.py
+-rw-r--r--   0        0        0      233 2024-05-09 20:51:19.949631 pythonix-1.0.3/pythonix/tup.py
+-rw-r--r--   0        0        0     3498 1970-01-01 00:00:00.000000 pythonix-1.0.3/PKG-INFO
```

### Comparing `pythonix-1.0.2/README.md` & `pythonix-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # PYTHONIX
 
-A collection of functional modules in Python 12 inspired by Gleam and Rust.
+A collection of functional modules in Python 11 inspired by Gleam and Rust.
 If you have like functional programming, but have to program in Python, then check this out.
 
 ## Features
 
 1. Exceptions as values support similar to Rust
 2. Emphasis on immutable types
 3. Great support for immutable data structures
```

### Comparing `pythonix-1.0.2/pythonix/internals/curry.py` & `pythonix-1.0.3/pythonix/internals/curry.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,258 +1,318 @@
 from unittest import TestCase
 from typing import TypeVar, Callable
 
-T1 = TypeVar('T1')
-T2 = TypeVar('T2')
-T3 = TypeVar('T3')
-T4 = TypeVar('T4')
-T5 = TypeVar('T5')
-T6 = TypeVar('T6')
-T7 = TypeVar('T7')
-T8 = TypeVar('T8')
-T9 = TypeVar('T9')
-U = TypeVar('U')
+T1 = TypeVar("T1")
+T2 = TypeVar("T2")
+T3 = TypeVar("T3")
+T4 = TypeVar("T4")
+T5 = TypeVar("T5")
+T6 = TypeVar("T6")
+T7 = TypeVar("T7")
+T8 = TypeVar("T8")
+T9 = TypeVar("T9")
+U = TypeVar("U")
 
 
 def two(func: Callable[[T1, T2], U]) -> Callable[[T1], Callable[[T2], U]]:
-
     def in1(t1: T1) -> Callable[[T2], U]:
-
         def in2(t2: T2) -> U:
-
             return func(t1, t2)
-        
+
         return in2
 
     return in1
 
 
-def three(func: Callable[[T1, T2, T3], U]) -> Callable[[T1], Callable[[T2], Callable[[T3], U]]]:
-
+def three(
+    func: Callable[[T1, T2, T3], U]
+) -> Callable[[T1], Callable[[T2], Callable[[T3], U]]]:
     def in1(t1: T1) -> Callable[[T2], Callable[[T3], U]]:
-
         def in2(t2: T2) -> Callable[[T3], U]:
-
             def in3(t3: T3) -> U:
-
                 return func(t1, t2, t3)
-            
+
             return in3
 
         return in2
-    
+
     return in1
 
 
 def four(
     func: Callable[[T1, T2, T3, T4], U]
 ) -> Callable[[T1], Callable[[T2], Callable[[T3], Callable[[T4], U]]]]:
-    
     def in1(t1: T1) -> Callable[[T2], Callable[[T3], Callable[[T4], U]]]:
-
         def in2(t2: T2) -> Callable[[T3], Callable[[T4], U]]:
-
             def in3(t3: T3) -> Callable[[T4], U]:
-
                 def in4(t4: T4) -> U:
-
                     func(t1, t2, t3, t4)
-                
+
                 return in4
-            
+
             return in3
-    
+
         return in2
-    
+
     return in1
 
 
 def five(
     func: Callable[[T1, T2, T3, T4, T5], U]
 ) -> Callable[[T1], Callable[[T2], Callable[[T3], Callable[[T4], Callable[[T5], U]]]]]:
-    
-    def in1(t1: T1) -> Callable[[T2], Callable[[T3], Callable[[T4], Callable[[T5], U]]]]:
-
+    def in1(
+        t1: T1,
+    ) -> Callable[[T2], Callable[[T3], Callable[[T4], Callable[[T5], U]]]]:
         def in2(t2: T2) -> Callable[[T3], Callable[[T4], Callable[[T5], U]]]:
-
             def in3(t3: T3) -> Callable[[T4], Callable[[T5], U]]:
-
                 def in4(t4: T4) -> Callable[[T5], U]:
-                    
                     def in5(t5: T5) -> U:
-                        
                         return func(t1, t2, t3, t4, t5)
-                    
+
                     return in5
-                
+
                 return in4
-            
+
             return in3
-    
+
         return in2
-    
+
     return in1
 
 
 def six(
     func: Callable[[T1, T2, T3, T4, T5, T6], U]
-) -> Callable[[T1], Callable[[T2], Callable[[T3], Callable[[T4], Callable[[T5], Callable[[T6], U]]]]]]:
-    
-    def in1(t1: T1) -> Callable[[T2], Callable[[T3], Callable[[T4], Callable[[T5], Callable[[T6], U]]]]]:
-
-        def in2(t2: T2) -> Callable[[T3], Callable[[T4], Callable[[T5], Callable[[T6], U]]]]:
-
+) -> Callable[
+    [T1],
+    Callable[[T2], Callable[[T3], Callable[[T4], Callable[[T5], Callable[[T6], U]]]]],
+]:
+    def in1(
+        t1: T1,
+    ) -> Callable[
+        [T2], Callable[[T3], Callable[[T4], Callable[[T5], Callable[[T6], U]]]]
+    ]:
+        def in2(
+            t2: T2,
+        ) -> Callable[[T3], Callable[[T4], Callable[[T5], Callable[[T6], U]]]]:
             def in3(t3: T3) -> Callable[[T4], Callable[[T5], Callable[[T6], U]]]:
-
                 def in4(t4: T4) -> Callable[[T5], Callable[[T6], U]]:
-                    
                     def in5(t5: T5) -> Callable[[T6], U]:
-                        
                         def in6(t6: T6) -> U:
-                            
                             return func(t1, t2, t3, t4, t5, t6)
-                        
+
                         return in6
-                    
+
                     return in5
-                
+
                 return in4
-            
+
             return in3
-    
+
         return in2
-    
+
     return in1
 
 
 def seven(
     func: Callable[[T1, T2, T3, T4, T5, T6, T7], U]
-) -> Callable[[T1], Callable[[T2], Callable[[T3], Callable[[T4], Callable[[T5], Callable[[T6], Callable[[T7], U]]]]]]]:
-    
-    def in1(t1: T1) -> Callable[[T2], Callable[[T3], Callable[[T4], Callable[[T5], Callable[[T6], Callable[[T7], U]]]]]]:
-
-        def in2(t2: T2) -> Callable[[T3], Callable[[T4], Callable[[T5], Callable[[T6], Callable[[T7], U]]]]]:
-
-            def in3(t3: T3) -> Callable[[T4], Callable[[T5], Callable[[T6], Callable[[T7], U]]]]:
-
+) -> Callable[
+    [T1],
+    Callable[
+        [T2],
+        Callable[
+            [T3], Callable[[T4], Callable[[T5], Callable[[T6], Callable[[T7], U]]]]
+        ],
+    ],
+]:
+    def in1(
+        t1: T1,
+    ) -> Callable[
+        [T2],
+        Callable[
+            [T3], Callable[[T4], Callable[[T5], Callable[[T6], Callable[[T7], U]]]]
+        ],
+    ]:
+        def in2(
+            t2: T2,
+        ) -> Callable[
+            [T3], Callable[[T4], Callable[[T5], Callable[[T6], Callable[[T7], U]]]]
+        ]:
+            def in3(
+                t3: T3,
+            ) -> Callable[[T4], Callable[[T5], Callable[[T6], Callable[[T7], U]]]]:
                 def in4(t4: T4) -> Callable[[T5], Callable[[T6], Callable[[T7], U]]]:
-                    
                     def in5(t5: T5) -> Callable[[T6], Callable[[T7], U]]:
-                        
                         def in6(t6: T6) -> Callable[[T7], U]:
-                            
                             def in7(t7: T7) -> U:
-                                
                                 return func(t1, t2, t3, t4, t5, t6, t7)
-                            
+
                             return in7
-                        
+
                         return in6
-                    
+
                     return in5
-                
+
                 return in4
-            
+
             return in3
-    
+
         return in2
-    
+
     return in1
 
 
 def eight(
     func: Callable[[T1, T2, T3, T4, T5, T6, T7, T8], U]
-) -> Callable[[T1], Callable[[T2], Callable[[T3], Callable[[T4], Callable[[T5], Callable[[T6], Callable[[T7], Callable[[T8], U]]]]]]]]:
-    
-    def in1(t1: T1) -> Callable[[T2], Callable[[T3], Callable[[T4], Callable[[T5], Callable[[T6], Callable[[T7], Callable[[T8], U]]]]]]]:
-
-        def in2(t2: T2) -> Callable[[T3], Callable[[T4], Callable[[T5], Callable[[T6], Callable[[T7], Callable[[T8], U]]]]]]:
-
-            def in3(t3: T3) -> Callable[[T4], Callable[[T5], Callable[[T6], Callable[[T7], Callable[[T8], U]]]]]:
-
-                def in4(t4: T4) -> Callable[[T5], Callable[[T6], Callable[[T7], Callable[[T8], U]]]]:
-                    
-                    def in5(t5: T5) -> Callable[[T6], Callable[[T7], Callable[[T8], U]]]:
-                        
+) -> Callable[
+    [T1],
+    Callable[
+        [T2],
+        Callable[
+            [T3],
+            Callable[
+                [T4], Callable[[T5], Callable[[T6], Callable[[T7], Callable[[T8], U]]]]
+            ],
+        ],
+    ],
+]:
+    def in1(
+        t1: T1,
+    ) -> Callable[
+        [T2],
+        Callable[
+            [T3],
+            Callable[
+                [T4], Callable[[T5], Callable[[T6], Callable[[T7], Callable[[T8], U]]]]
+            ],
+        ],
+    ]:
+        def in2(
+            t2: T2,
+        ) -> Callable[
+            [T3],
+            Callable[
+                [T4], Callable[[T5], Callable[[T6], Callable[[T7], Callable[[T8], U]]]]
+            ],
+        ]:
+            def in3(
+                t3: T3,
+            ) -> Callable[
+                [T4], Callable[[T5], Callable[[T6], Callable[[T7], Callable[[T8], U]]]]
+            ]:
+                def in4(
+                    t4: T4,
+                ) -> Callable[[T5], Callable[[T6], Callable[[T7], Callable[[T8], U]]]]:
+                    def in5(
+                        t5: T5,
+                    ) -> Callable[[T6], Callable[[T7], Callable[[T8], U]]]:
                         def in6(t6: T6) -> Callable[[T7], Callable[[T8], U]]:
-                            
                             def in7(t7: T7) -> Callable[[T8], U]:
-                                
                                 def in8(t8: T8) -> U:
-                                    
                                     return func(t1, t2, t3, t4, t5, t6, t7, t8)
-                                
+
                                 return in8
-                            
+
                             return in7
-                        
+
                         return in6
-                    
+
                     return in5
-                
+
                 return in4
-            
+
             return in3
-    
+
         return in2
-    
+
     return in1
 
 
 def nine(
     func: Callable[[T1, T2, T3, T4, T5, T6, T7, T8, T9], U]
-) -> Callable[[T1], Callable[[T2], Callable[[T3], Callable[[T4], Callable[[T5], Callable[[T6], Callable[[T7], Callable[[T8], Callable[[T9], U]]]]]]]]]:
-    
-    def in1(t1: T1) -> Callable[[T2], Callable[[T3], Callable[[T4], Callable[[T5], Callable[[T6], Callable[[T7], Callable[[T8], Callable[[T9], U]]]]]]]]:
-
-        def in2(t2: T2) -> Callable[[T3], Callable[[T4], Callable[[T5], Callable[[T6], Callable[[T7], Callable[[T8], Callable[[T9], U]]]]]]]:
-
-            def in3(t3: T3) -> Callable[[T4], Callable[[T5], Callable[[T6], Callable[[T7], Callable[[T8], Callable[[T9], U]]]]]]:
-
-                def in4(t4: T4) -> Callable[[T5], Callable[[T6], Callable[[T7], Callable[[T8], Callable[[T9], U]]]]]:
-                    
-                    def in5(t5: T5) -> Callable[[T6], Callable[[T7], Callable[[T8], Callable[[T9], U]]]]:
-                        
-                        def in6(t6: T6) -> Callable[[T7], Callable[[T8], Callable[[T9], U]]]:
-                            
+) -> Callable[
+    [T1],
+    Callable[
+        [T2],
+        Callable[
+            [T3],
+            Callable[
+                [T4],
+                Callable[
+                    [T5],
+                    Callable[[T6], Callable[[T7], Callable[[T8], Callable[[T9], U]]]],
+                ],
+            ],
+        ],
+    ],
+]:
+    def in1(
+        t1: T1,
+    ) -> Callable[
+        [T2],
+        Callable[
+            [T3],
+            Callable[
+                [T4],
+                Callable[
+                    [T5],
+                    Callable[[T6], Callable[[T7], Callable[[T8], Callable[[T9], U]]]],
+                ],
+            ],
+        ],
+    ]:
+        def in2(
+            t2: T2,
+        ) -> Callable[
+            [T3],
+            Callable[
+                [T4],
+                Callable[
+                    [T5],
+                    Callable[[T6], Callable[[T7], Callable[[T8], Callable[[T9], U]]]],
+                ],
+            ],
+        ]:
+            def in3(
+                t3: T3,
+            ) -> Callable[
+                [T4],
+                Callable[
+                    [T5],
+                    Callable[[T6], Callable[[T7], Callable[[T8], Callable[[T9], U]]]],
+                ],
+            ]:
+                def in4(
+                    t4: T4,
+                ) -> Callable[
+                    [T5],
+                    Callable[[T6], Callable[[T7], Callable[[T8], Callable[[T9], U]]]],
+                ]:
+                    def in5(
+                        t5: T5,
+                    ) -> Callable[
+                        [T6], Callable[[T7], Callable[[T8], Callable[[T9], U]]]
+                    ]:
+                        def in6(
+                            t6: T6,
+                        ) -> Callable[[T7], Callable[[T8], Callable[[T9], U]]]:
                             def in7(t7: T7) -> Callable[[T8], Callable[[T9], U]]:
-                                
                                 def in8(t8: T8) -> Callable[[T9], U]:
-                                    
                                     def in9(t9: T9) -> U:
-
                                         return func(t1, t2, t3, t4, t5, t6, t7, t8, t9)
-                                    
+
                                     return in9
-                                
+
                                 return in8
-                            
+
                             return in7
-                        
+
                         return in6
-                    
-                    return in5
-                
-                return in4
-            
-            return in3
-    
-        return in2
-    
-    return in1
 
+                    return in5
 
+                return in4
 
-class TestCurry(TestCase):
+            return in3
 
-    def test_two(self) -> None:
-        
-        @two
-        def foo(x: int, y: str) -> tuple[int, str]:
-            return x, y
-        
-        x = 5
-        y = 'hello'
-        expected = (x, y)
-        actual = foo(x)(y)
+        return in2
 
-        self.assertSequenceEqual(expected, actual)
+    return in1
```

### Comparing `pythonix-1.0.2/pythonix/internals/mdeq.py` & `pythonix-1.0.3/pythonix/internals/mdeq.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 """
 from collections import deque
 from __future__ import annotations
 from typing import Iterable, Generic, TypeVar
 from pythonix.res import null_and_error_safe, safe, Ok
 from pythonix.curry import two, three
 
-Val = TypeVar('Val')
-NewVal = TypeVar('NewVal')
+Val = TypeVar("Val")
+NewVal = TypeVar("NewVal")
+
 
 class MDeq(Generic[Val], object):
     """
     `MDeq` is a singly-typed mutable linked list. `push` and `pop` operations are thread safe and run in
     `O(1)` time. Insert and get operations run in `O(n)` time. As a mutable data structure there are some
     rules to keep in mind.
 
@@ -114,15 +115,14 @@
 def last(deq: MDeq[Val]) -> Val:
     """
     Returns the last element in an `MDeq` if it exists.
     """
     return deq.inner[-1]
 
 
-
 @two
 @null_and_error_safe(IndexError)
 def at(index: int, deq: MDeq[Val]) -> Val:
     """
     Returns the element at the provided index in an `MDeq` if it exists.
     """
     return deq.inner[index]
@@ -160,11 +160,10 @@
 def index(find: Val, start: int = 1):
     """
     Retrieves the index of the provide dvalue, if it exists.
     """
 
     @null_and_error_safe(ValueError)
     def inner(deq: MDeq[Val]) -> int:
-
         return deq.inner.index(find, start)
 
     return inner
```

### Comparing `pythonix-1.0.2/pythonix/internals/op.py` & `pythonix-1.0.3/pythonix/internals/op.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 """
 Functions used to operate over data structures
 """
-from typing import Callable, Iterable, Iterator, Any, SupportsIndex, TypeVar
+from typing import Callable, Iterable, Iterator, Any, SupportsIndex, TypeVar, Mapping
 from functools import reduce
 from pythonix.internals.res import null_and_error_safe
 
-Val = TypeVar('Val')
-SecondVal = TypeVar('SecondVal')
-NewVal = TypeVar('NewVal')
+Val = TypeVar("Val")
+SecondVal = TypeVar("SecondVal")
+NewVal = TypeVar("NewVal")
+
 
 def filterx(using: Callable[[Val], bool]) -> Callable[[Iterable[Val]], Iterator[Val]]:
     """
     Filter over an `Iterable` with a function that takes each of its elements and returns a True or False.
     True evaluations are kept while False are not kept in the result.
     """
-    def get_data(iterable: Iterable[Val]) -> filter[Val]:
 
+    def get_data(iterable: Iterable[Val]) -> Iterator[Val]:
         return filter(using, iterable)
 
     return get_data
 
 
 def mapx(using: Callable[[Val], NewVal]) -> Callable[[Iterable[Val]], Iterator[NewVal]]:
     """
-    Run the `using` function over an `Iterable` and return an `Iterator` containing the result 
+    Run the `using` function over an `Iterable` and return an `Iterator` containing the result.
     """
-    def get_data(iterable: Iterable[Val]) -> map[NewVal]:
+
+    def get_data(iterable: Iterable[Val]) -> Iterator[NewVal]:
 
         return map(using, iterable)
 
     return get_data
 
 
-def reducex(using: Callable[[Val, SecondVal], NewVal]) -> Callable[[Iterable[Val | SecondVal]], Iterator[NewVal]]:
+def reducex(
+    using: Callable[[Val, SecondVal], NewVal]
+) -> Callable[[Iterable[Val | SecondVal]], Iterator[NewVal]]:
     """
-    Run a function that takes two arguments over an `Iterable` to produce a single result. 
+    Run a function that takes two arguments over an `Iterable` to produce a single result.
     """
-    def get_data(iterable: Iterable[Val | SecondVal]) -> reduce[NewVal]:
 
+    def get_data(iterable: Iterable[Val | SecondVal]) -> NewVal:
         return reduce(using, iterable)
 
     return get_data
 
 
 def attr(name: str, type_hint: type[NewVal] = Any):
     """
@@ -87,7 +91,19 @@
     """
 
     @null_and_error_safe(IndexError, KeyError)
     def inner(iterable: Iterable[Val]) -> Val:
         return iterable[index]
 
     return inner
+
+
+def arg(val: Val):
+    '''
+    Applies a single argument to a function and returns its result.
+    Useful for piping an argument into a function via `Bind` or `Do`
+    '''
+    def get_op(op: Callable[[Val], NewVal]):
+
+        return op(arg)
+    
+    return get_op
```

### Comparing `pythonix-1.0.2/pythonix/internals/pair.py` & `pythonix-1.0.3/pythonix/internals/pair.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,34 +3,39 @@
 """
 
 from typing import NamedTuple, Tuple, TypeVar, Generic, TypeAlias
 from pythonix.internals.types import Fn
 from pythonix.internals.curry import two
 
 
-Val = TypeVar('Val')
-NewVal = TypeVar('NewVal')
+Val = TypeVar("Val")
+NewVal = TypeVar("NewVal")
 KeyStr: TypeAlias = str
 
+
 class Pair(Generic[Val], NamedTuple):
     """
     A typed key value pair whose key is a `str`
     """
+
     key: str
     value: Val
 
+
 Pairs: TypeAlias = Tuple[Pair[Val], ...]
 
+
 @two
 def new(key: KeyStr, value: Val) -> Pair[Val]:
     """
-    Create a new key value `Pair` safely 
+    Create a new key value `Pair` safely
     """
     return Pair(key, value)
 
+
 @two
 def set_key(key: KeyStr, pair: Pair[Val]) -> Pair[Val]:
     """
     Creates a new `Pair` from a provided one with the provided key.
     """
     return new(key)(pair.value)
 
@@ -45,14 +50,15 @@
 
 def get_value(pair: Pair[Val]) -> Val:
     """
     Retrieves the `value` of a provided `Pair`
     """
     return pair.value
 
+
 def get_key(pair: Pair[Val]) -> KeyStr:
     """
     Retrieves the `key` of a provided `Pair`
     """
     return pair.key
```

### Comparing `pythonix-1.0.2/pythonix/internals/pipe.py` & `pythonix-1.0.3/pythonix/internals/pipe.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from __future__ import annotations
 from typing import Callable, Protocol, Tuple, overload, TypeVar, Generic
 from pythonix.internals import trail
 from pythonix.internals.trail import Trail, Log
 
-Val = TypeVar('Val')
-NewVal = TypeVar('NewVal')
+Val = TypeVar("Val")
+NewVal = TypeVar("NewVal")
 
 
 class HasInner(Generic[Val], Protocol):
-
     inner: Val
 
 
 class Bind(Generic[Val]):
     """
     Container that allows sequential functions calls to change its inner value and type.
     Transformations can be done with with either the `run` or `__call__` methods.
@@ -31,14 +30,21 @@
     - `__call__(Fn(T) -> U) -> Bind<U>`: Identical to the `run` function.
     """
 
     inner: Val
 
     def __init__(self, inner: Val) -> None:
         self.inner = inner
+    
+    @property
+    def do(self) -> Do[Val]:
+        """
+        Converts the `Bind` pipe to a `Do` pipe
+        """
+        return Do(self.inner)
 
     def run(self, using: Callable[[Val], NewVal]) -> Bind[NewVal]:
         """
         Performs a transformation on the contained value using the function provided.
         Returns a new `Bind` object containing the new value. Works only with single arity
         functions.
         """
@@ -81,14 +87,21 @@
     def run(self, using: Callable[[Val], NewVal]) -> Do[Val]:
         """
         Performs the provided function on the `inner` value, but does not return its result.
         Returns itself instead.
         """
         using(self.inner)
         return self
+    
+    @property
+    def bind(self) -> Bind[Val]:
+        """
+        Converts the `Do` pipe to a `Bind` pipe
+        """
+        return Bind(self.inner)
 
     def __call__(self, using: Callable[[Val], NewVal]) -> Do[Val]:
         """
         Performs the provided function on the `inner` value, but does not return its result.
         Returns itself instead.
         """
         return self.run(using)
@@ -111,18 +124,24 @@
                 self.inner = inner
                 self.logs = logs + inner.logs
             case _:
                 self.inner = trail.new()(inner)
                 self.logs = logs
 
     @overload
-    def __call__(self, using: Callable[[Val], trail.Trail[NewVal]], *logs: Log) -> Blaze[NewVal]: ...
+    def __call__(
+        self, using: Callable[[Val], trail.Trail[NewVal]], *logs: Log
+    ) -> Blaze[NewVal]:
+        ...
 
     @overload
-    def __call__(self, using: Callable[[Val], NewVal], *logs: Log) -> Blaze[NewVal]: ...
+    def __call__(self, using: Callable[[Val], NewVal], *logs: Log) -> Blaze[NewVal]:
+        ...
 
-    def __call__(self, using: Callable[[Val], trail.Trail[NewVal] | NewVal], *logs: Log) -> Blaze[NewVal]:
+    def __call__(
+        self, using: Callable[[Val], trail.Trail[NewVal] | NewVal], *logs: Log
+    ) -> Blaze[NewVal]:
         """
         Call the function and attach the logs from the function `Trail` and the optional logs
         to the new instance of `Blaze` containing the result.
         """
         return Blaze(using(self.inner.inner), *(self.logs + logs))
```

### Comparing `pythonix-1.0.2/pythonix/internals/req.py` & `pythonix-1.0.3/pythonix/internals/req.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from typing import NamedTuple, ParamSpec, Callable, Tuple, TypeVar
 from pythonix.op import mapx
 from pythonix.pipe import Bind
 from pythonix.res import Res
 import pythonix.pair as pair
 from functools import singledispatch
 from requests import (
-    get      as _get,
-    post     as _post,
-    put      as _put,
-    delete   as _delete,
+    get as _get,
+    post as _post,
+    put as _put,
+    delete as _delete,
     Response as OGResponse,
-    HTTPError
+    HTTPError,
 )
 from pythonix.internals.pair import Pair, Pairs
 from pythonix.internals.pipe import Bind
 from pythonix import res
 
-P = ParamSpec('P')
+P = ParamSpec("P")
+
 
 class Response(NamedTuple):
     """
     Parsed response from an HTTP request.
     """
+
     url: str
     body: bytes
     status: int
 
 
 def parse_response(response: OGResponse) -> Response:
     """
@@ -43,243 +45,257 @@
     return response
 
 
 class Request(NamedTuple):
     """
     Request type to be sent via an HTTP method
     """
+
     url: str
     headers: Pairs[bytes]
     params: Pairs[bytes]
     data: Pairs[bytes]
 
-RequestType = TypeVar('RequestType', bound='Request')
+
+RequestType = TypeVar("RequestType", bound="Request")
+
 
 class Get(Request):
     """
     An HTTP request set as a `GET`
     """
+
     method: Callable[P, Response] = _get
 
+
 class Post(Request):
     """
     An HTTP request set as a `POST`
     """
+
     method: Callable[P, Response] = _post
 
+
 class Put(Request):
     """
     An HTTP request set as a `PUT`
     """
+
     method: Callable[P, Response] = _put
 
+
 class Delete(Request):
     """
     An HTTP request set as a `DELETE`
     """
+
     method: Callable[P, Response] = _delete
 
 
 @singledispatch
 def to_bytes(value: int) -> bytes:
     return bytes(value)
 
+
 @to_bytes.register(str)
 def _(value: str) -> bytes:
-    return bytes(value, 'utf-8')
+    return bytes(value, "utf-8")
 
 
 def set_value_to_bytes(keyvalue: Pair[str | int]) -> Pair[bytes]:
     Bind(keyvalue)(pair.map(to_bytes)).inner
 
 
 def get(url: str):
     """
     Set the URL for the request type
     """
+
     def get_headers(*headers: Pair[str | int]):
         """
         Add key value pairs to represent headers
         #### Example
         ```python
         new(Get)('https://helloworld.com')(
             pair.new('Authorization')('Bearer asdfasdfads'),
             pair.new('Content-Type')('application/json'),
         )
         ```
         """
+
         def get_params(*params: Pair[str | int]):
             """
             Add key value pairs to represent params. Same methodology as for headers.
             """
             return Get(
                 url,
                 tuple(mapx(set_value_to_bytes)(headers)),
                 tuple(mapx(set_value_to_bytes)(params)),
-                tuple()
+                tuple(),
             )
 
         return get_params
 
     return get_headers
 
 
 def post(url: str):
     """
     Set the URL for the request type
     """
+
     def get_headers(*headers: Pair[str | int]):
         """
         Add key value pairs to represent headers
         #### Example
         ```python
         new(Get)('https://helloworld.com')(
             pair.new('Authorization')('Bearer asdfasdfads'),
             pair.new('Content-Type')('application/json'),
         )
         ```
         """
+
         def get_params(*params: Pair[str | int]):
             """
             Add key value pairs to represent params. Same methodology as for headers.
             """
+
             def get_data(*data: Pair[str | int]):
                 """
                 Add key value pairs to represent data for the request
                 """
                 return Post(
                     url,
                     tuple(mapx(set_value_to_bytes)(headers)),
                     tuple(mapx(set_value_to_bytes)(params)),
-                    tuple(mapx(set_value_to_bytes)(data))
+                    tuple(mapx(set_value_to_bytes)(data)),
                 )
 
             return get_data
 
         return get_params
 
     return get_headers
 
+
 def put(url: str):
     """
     Set the URL for the request type
     """
+
     def get_headers(*headers: Pair[str | int]):
         """
         Add key value pairs to represent headers
         #### Example
         ```python
         new(Get)('https://helloworld.com')(
             pair.new('Authorization')('Bearer asdfasdfads'),
             pair.new('Content-Type')('application/json'),
         )
         ```
         """
+
         def get_params(*params: Pair[str | int]):
             """
             Add key value pairs to represent params. Same methodology as for headers.
             """
+
             def get_data(*data: Pair[str | int]):
                 """
                 Add key value pairs to represent data for the request
                 """
                 return Put(
                     url,
                     tuple(mapx(set_value_to_bytes)(headers)),
                     tuple(mapx(set_value_to_bytes)(params)),
-                    tuple(mapx(set_value_to_bytes)(data))
+                    tuple(mapx(set_value_to_bytes)(data)),
                 )
 
             return get_data
 
         return get_params
 
     return get_headers
 
 
 def delete(url: str):
     """
     Set the URL for the request type
     """
+
     def get_headers(*headers: Pair[str | int]):
         """
         Add key value pairs to represent headers
         #### Example
         ```python
         new(Get)('https://helloworld.com')(
             pair.new('Authorization')('Bearer asdfasdfads'),
             pair.new('Content-Type')('application/json'),
         )
         ```
         """
-        return Post(
-            url,
-            tuple(mapx(set_value_to_bytes)(headers)),
-            tuple(),
-            tuple()
-        )
+        return Post(url, tuple(mapx(set_value_to_bytes)(headers)), tuple(), tuple())
 
     return get_headers
 
 
 def set_url(url: str):
     """
     Recreates the given request type with a new URL
     """
+
     def get_content[R: (Request)](content: R) -> R:
-        
         return content.__class__(url, content.headers, content.params, content.data)
 
     return get_content
 
 
 def set_headers(*headers: Pair[str | int]):
     """
     Recreates the given request types with a new set of headers
     """
+
     def get_content[R: (Request)](content: R) -> R:
         return content.__class__(content.url, headers, content.params, content.data)
 
     return get_content
 
 
 def set_params(*params: Pair[str | int]):
     """
     Recreates the given request type with a new set of headers
     """
-    def get_content[R: (Request)](content: R) -> R:
 
+    def get_content[R: (Request)](content: R) -> R:
         return content.__class__(content.url, content.headers, params, content.data)
 
     return get_content
 
 
 def set_data(*data: Pair[str | int]):
     """
     Recreates the given request type with a new set of data
     """
-    def get_content[R: (Request)](content: R) -> R:
 
+    def get_content[R: (Request)](content: R) -> R:
         return content.__class__(content.url, content.headers, content.params, data)
 
     return get_content
 
 
 def body(content: RequestType) -> Tuple[Pair[bytes], ...]:
     """
     Combines the headers, params, and content of `Request`
     """
     return content.headers + content.params + content.data
 
+
 def send(request: RequestType) -> Res[Response, HTTPError]:
     """
     Sends the provided `Request` and then parses its response, capturing any errors that occur.
     """
-    return (
-        Bind(request)
-        (body)
-        (lambda body: {'url': request.url} | {k: v for k, v in body})
-        (lambda kwargs: request.method(**kwargs))
-        (check_status)
-        (res.map(parse_response))
-        .inner
-    )
+    return Bind(request)(body)(
+        lambda body: {"url": request.url} | {k: v for k, v in body}
+    )(lambda kwargs: request.method(**kwargs))(check_status)(
+        res.map(parse_response)
+    ).inner
```

### Comparing `pythonix-1.0.2/pythonix/internals/res.py` & `pythonix-1.0.3/pythonix/internals/res.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from collections.abc import Iterator
 from typing import TypeVar, Generic, NamedTuple, cast, ParamSpec, Callable
 from pythonix.internals.types import Fn
 
 P = ParamSpec("P")
 
 UnwrapErr = ValueError("Attempted to retrieve an Err from an Ok")
-Val = TypeVar('Val')
-NewVal = TypeVar('NewVal')
+Val = TypeVar("Val")
+NewVal = TypeVar("NewVal")
 ErrVal = TypeVar("ErrVal", bound="Exception")
 NewErrVal = TypeVar("NewErrVal", bound="Exception")
 
 
 class Nil(Exception):
     """
     Error class used to represent an unexpected `None` value.
@@ -135,31 +135,31 @@
             return True
 
 
 def is_ok_and(predicate: Fn[Val, bool]) -> Callable[[Res[Val, ErrVal]], bool]:
     """
     Return `True` if the `Res` is `Ok` and the `predicate` evaluates to `True`.
     """
-    def inner(res: Res[Val, ErrVal]) -> bool:
 
+    def inner(res: Res[Val, ErrVal]) -> bool:
         match res:
             case Ok(t):
                 return predicate(t)
             case _:
                 return False
 
     return inner
 
 
 def is_err_and(predicate: Fn[ErrVal, bool]) -> Callable[[Res[Val, ErrVal]], bool]:
     """
     Return `True` if the `Res` is `Err` and the `predicate` evaluates to `True`
     """
-    def inner(res: Res[Val, ErrVal]) -> bool:
 
+    def inner(res: Res[Val, ErrVal]) -> bool:
         match res:
             case Err(e):
                 return predicate(e)
             case _:
                 return False
 
     return inner
@@ -176,31 +176,31 @@
             raise e
 
 
 def unwrap_or(default: Val) -> Fn[Res[Val, ErrVal], Val]:
     """
     Return the `Ok` value if `Ok`, else return the default
     """
-    def inner(res: Res[Val, ErrVal]) -> Val:
 
+    def inner(res: Res[Val, ErrVal]) -> Val:
         match res:
             case Ok(val):
                 return val
             case _:
                 return default
 
     return inner
 
 
 def unwrap_or_else(on_err: Callable[[], Val]) -> Fn[Res[Val, ErrVal], Val]:
     """
     Return the `Ok` value if `Ok`, else run the `on_err` function that returns the same type.
     """
-    def inner(res: Res[Val, ErrVal]) -> Val:
 
+    def inner(res: Res[Val, ErrVal]) -> Val:
         match res:
             case Ok(val):
                 return val
             case _:
                 return on_err()
 
     return inner
@@ -217,102 +217,137 @@
             return e
 
 
 def map(using: Fn[Val, NewVal]) -> Fn[Res[Val, ErrVal], Res[NewVal, ErrVal]]:
     """
     Run the function on the `Ok` if `Ok`, else return the current `Err`
     """
+
     def inner(res: Res[Val, ErrVal]) -> Res[NewVal, ErrVal]:
         match res:
             case Ok(t):
                 return ok(using(t))(ErrVal)
             case _:
                 return cast(Res[NewVal, ErrVal], res)
 
     return inner
 
 
-def map_or(using: Fn[Val, NewVal]) -> Callable[[NewVal], Callable[[Res[Val, ErrVal]], Res[NewVal, ErrVal]]]:
+def map_or(
+    using: Fn[Val, NewVal]
+) -> Callable[[NewVal], Callable[[Res[Val, ErrVal]], Res[NewVal, ErrVal]]]:
     """
     Runs the function on the `Ok` or return the `default` if `Err`
     """
-    def get_default(default: NewVal) -> Callable[[Res[Val, ErrVal]], Res[NewVal, ErrVal]]:
 
+    def get_default(
+        default: NewVal,
+    ) -> Callable[[Res[Val, ErrVal]], Res[NewVal, ErrVal]]:
         def inner(res: Res[Val, ErrVal]) -> Res[NewVal, ErrVal]:
-
             match res:
                 case Ok(t):
                     return ok(using(t))(ErrVal)
                 case _:
                     return ok(default)(ErrVal)
 
         return inner
 
     return get_default
 
 
-def map_catch(using: Callable[[Val], NewVal]) -> Callable[[type[ErrVal]], Callable[[Res[Val, ErrVal]], Res[NewVal, ErrVal]]]:
+def map_err(
+    using: Fn[ErrVal, NewErrVal]
+) -> Callable[[Res[Val, ErrVal]], Res[Val, NewErrVal]]:
+    """
+    Runs the function on the `ErrVal` if in `Err` or returns the current `Ok`
+    """
+
+    def inner(res: Res[Val, ErrVal]) -> Res[Val, ErrVal]:
+        match res:
+            case Err(e):
+                return err(Val)(using(e))
+            case _:
+                return cast(Res[Val, NewErrVal], res)
+
+    return inner
+
+
+def map_catch(
+    using: Callable[[Val], NewVal]
+) -> Callable[[type[ErrVal]], Callable[[Res[Val, ErrVal]], Res[NewVal, ErrVal]]]:
     """
     Runs the function that could fail if `Ok`, else return the current `Err`
     """
-    def get_catch(catch: type[ErrVal]) -> Callable[[Res[Val, ErrVal]], Res[NewVal, ErrVal]]:
 
+    def get_catch(
+        catch: type[ErrVal],
+    ) -> Callable[[Res[Val, ErrVal]], Res[NewVal, ErrVal]]:
         def inner(res: Res[Val, ErrVal]) -> Res[NewVal, ErrVal]:
-
             match res:
                 case Ok(t):
                     try:
                         return ok(using(t))(ErrVal)
                     except catch as e:
                         return err(NewVal)(e)
                 case Err(e):
                     return cast(Res[NewVal, ErrVal], res)
 
         return inner
 
     return get_catch
 
 
-def map_or_else(using: Fn[Val, NewVal]) -> Callable[[Callable[[], NewVal]], Callable[[Res[Val, ErrVal]], Res[NewVal, ErrVal]]]:
+def map_or_else(
+    using: Fn[Val, NewVal]
+) -> Callable[
+    [Callable[[], NewVal]], Callable[[Res[Val, ErrVal]], Res[NewVal, ErrVal]]
+]:
     """
     Runs the provided function if `Ok`, or runs the default function if `Err`
     """
-    def get_default(default: Callable[[], NewVal]) -> Callable[[Res[Val, ErrVal]], Res[NewVal, ErrVal]]:
 
+    def get_default(
+        default: Callable[[], NewVal]
+    ) -> Callable[[Res[Val, ErrVal]], Res[NewVal, ErrVal]]:
         def inner(res: Res[Val, ErrVal]) -> Res[NewVal, ErrVal]:
-
             match res:
                 case Ok(t):
                     return ok(using(t))(ErrVal)
                 case _:
                     return ok(default())(ErrVal)
 
         return inner
 
     return get_default
 
 
-def and_then(using: Fn[Val, Res[NewVal, ErrVal]]) -> Fn[Res[Val, ErrVal], Res[NewVal, ErrVal]]:
+def and_then(
+    using: Fn[Val, Res[NewVal, ErrVal]]
+) -> Fn[Res[Val, ErrVal], Res[NewVal, ErrVal]]:
     """
     Runs the function that returns a new `Res` if `Ok`, else return the current `Err`
     """
+
     def inner(res: Res[Val, ErrVal]) -> Res[NewVal, ErrVal]:
         match res:
             case Ok(t):
                 return cast(Res[NewVal, ErrVal], using(t))
             case _:
                 return cast(Res[NewVal, ErrVal], res)
 
     return inner
 
 
-def or_else(using: Fn[ErrVal, Res[NewVal, NewErrVal]]) -> Fn[Res[Val, ErrVal], Res[Val, NewErrVal]]:
+def or_else(
+    using: Fn[ErrVal, Res[NewVal, NewErrVal]]
+) -> Fn[Res[Val, ErrVal], Res[Val, NewErrVal]]:
     """
     Runs the function that returns a new `Res` if in `Err`, else it will return the current `Ok`
     """
+
     def inner(res: Res[Val, ErrVal]) -> Res[Val, NewErrVal]:
         match res:
             case Err(e):
                 return cast(Res[Val, NewErrVal], using(e))
             case _:
                 return cast(Res[Val, NewErrVal], res)
 
@@ -320,21 +355,25 @@
 
 
 def and_then_catch(using: Fn[Val, NewVal]):
     """
     Runs the function that could fail, catching the specified error and returning a new `Res`.
     Will only be ran if `Ok`, else it will return its current `Err`
     """
-    def get_catch(catch: type[NewErrVal]) -> Fn[Res[Val, ErrVal], Res[NewVal, ErrVal | NewErrVal]]:
 
+    def get_catch(
+        catch: type[NewErrVal],
+    ) -> Fn[Res[Val, ErrVal], Res[NewVal, ErrVal | NewErrVal]]:
         def inner(res: Res[Val, ErrVal]) -> Res[NewVal, ErrVal | NewErrVal]:
             match res:
                 case Ok(t):
                     try:
-                        return cast(Res[NewVal, ErrVal | NewErrVal], ok(using(t))(ErrVal))
+                        return cast(
+                            Res[NewVal, ErrVal | NewErrVal], ok(using(t))(ErrVal)
+                        )
                     except catch as f:
                         return cast(Res[NewVal, ErrVal | NewErrVal], err(NewVal)(f))
                 case Err(f):
                     return cast(Res[NewVal, ErrVal | NewErrVal], err(NewVal)(f))
 
         return inner
 
@@ -342,46 +381,48 @@
 
 
 def map_err(using: Fn[ErrVal, NewErrVal]):
     """
     Changes the internal `Err` using the function if in an `Err` state. Otherwise it returns
     the `Ok`
     """
-    def inner(res: Res[Val, ErrVal]) -> Res[Val, NewErrVal]:
 
+    def inner(res: Res[Val, ErrVal]) -> Res[Val, NewErrVal]:
         match res:
             case Err(e):
                 return err(Val)(using(e))
             case _:
                 return cast(Res[Val, NewErrVal], res)
 
     return inner
 
 
-def and_res(new_res: Res[NewVal, ErrVal]) -> Callable[[Res[Val, ErrVal]], Res[NewVal, ErrVal]]:
+def and_res(
+    new_res: Res[NewVal, ErrVal]
+) -> Callable[[Res[Val, ErrVal]], Res[NewVal, ErrVal]]:
     """
     Returns the provided result if the old one is `Ok`
     """
-    def inner(old_res: Res[Val, ErrVal]) -> Res[NewVal, ErrVal]:
 
+    def inner(old_res: Res[Val, ErrVal]) -> Res[NewVal, ErrVal]:
         match old_res:
             case Ok():
                 return new_res
             case Err():
                 return cast(Res[NewVal, ErrVal], old_res)
 
     return inner
 
 
 def or_res[T, F](new_res: Res[T, F]) -> Callable[[Res[T, ErrVal]], Res[T, F]]:
     """
     Returns the provided result if the current one is an `Err`
     """
-    def inner(old_res: Res[T, ErrVal]) -> Res[T, F]:
 
+    def inner(old_res: Res[T, ErrVal]) -> Res[T, F]:
         match old_res:
             case Ok():
                 return cast(Res[T, F], old_res)
             case Err():
                 return new_res
 
     return inner
@@ -401,17 +442,15 @@
 def safe(err_type: type[ErrVal]):
     """
     Wraps the output `U` of an object or its thrown `Exception` `E` in a
     `Res[U, E]` object. Handles only one `Exception` at a time.
     """
 
     def inner(using: Callable[P, NewVal]) -> Callable[P, Res[NewVal, ErrVal]]:
-
         def wrapper(*args: P.args, **kwargs: P.kwargs) -> Res[NewVal, ErrVal]:
-
             try:
                 return cast(Res[NewVal, ErrVal], ok(using(*args, **kwargs))(err_type))
             except err_type as e:
                 return cast(Res[NewVal, ErrVal], err(NewVal)(e))
 
         return wrapper
 
@@ -420,33 +459,31 @@
 
 def null_safe(using: Callable[P, NewVal | None]):
     """
     Wraps the output of the function in a `Res[T, Nil]` object.
     """
 
     def inner(*args: P.args, **kwargs: P.kwargs) -> Res[NewVal, Nil]:
-
         return some(using(*args, **kwargs))
 
     return inner
 
 
 def null_and_error_safe(*err_types: type[ErrVal]):
     """
     Wraps the output in the `some` function and consumes the error if it is thrown, replacing it with `Nil`
     """
 
     def inner(using: Callable[P, Val]):
-
         def wrapper(*args: P.args, **kwargs: P.kwargs) -> Res[Val, Nil]:
-
             try:
                 return some(using(*args, **kwargs))
             except err_types as e:
                 return map_err(lambda f: Nil(str(f)))(err(Val)(e))
 
         return wrapper
 
     return inner
 
 
-q = unwrap
+q = unwrap
+qe = unwrap_err
```

### Comparing `pythonix-1.0.2/pythonix/internals/trail.py` & `pythonix-1.0.3/pythonix/internals/trail.py`

 * *Files identical despite different names*

### Comparing `pythonix-1.0.2/pythonix/internals/tuple.py` & `pythonix-1.0.3/pythonix/internals/tup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 """
 from typing import Tuple, TypeVar
 from pythonix.op import item
 from pythonix.res import safe, null_and_error_safe
 from pythonix.curry import two, three
 from enum import Enum
 
-Val = TypeVar('Val')
-NewVal = TypeVar('NewVal')
+Val = TypeVar("Val")
+NewVal = TypeVar("NewVal")
 type IndexInt = int
 
+
 class Side(Enum):
     LEFT: str = "LEFT"
     RIGHT: str = "RIGHT"
 
 
 def new(*elements: Val) -> Tuple[Val, ...]:
     """
@@ -23,18 +24,17 @@
     return elements
 
 
 def push(side: Side = Side.RIGHT):
     """
     Push an element to either side of a `Tuple`
     """
+
     def get_element(element: NewVal):
-        
         def inner(tuples: Tuple[Val, ...]) -> Tuple[Val | NewVal, ...]:
-
             match side:
                 case Side.LEFT:
                     return (element,) + tuples
                 case Side.RIGHT:
                     return tuples + (element,)
 
         return inner
@@ -50,18 +50,17 @@
     return item(index)(tuples)
 
 
 def extend(side: Side = Side.RIGHT):
     """
     Combine two tuple series together
     """
-    def get_left(new: Tuple[Val, ...]):
 
+    def get_left(new: Tuple[Val, ...]):
         def get_right(old: Tuple[NewVal, ...]) -> Tuple[Val | NewVal, ...]:
-
             match side:
                 case Side.LEFT:
                     return new + old
                 case Side.RIGHT:
                     return old + new
 
         return get_right
@@ -83,30 +82,32 @@
     """
     Count the occurrences of the provided value in a `Tuple`
     """
     return tuples.count(value)
 
 
 @three
-def insert(index: IndexInt, insert: NewVal, tuples: Tuple[Val, ...]) -> Tuple[Val | NewVal, ...]:
+def insert(
+    index: IndexInt, insert: NewVal, tuples: Tuple[Val, ...]
+) -> Tuple[Val | NewVal, ...]:
     """
     Recreate the `Tuple` with the provided element at the index
     """
     return tuples[:index] + (insert,) + tuples[index:]
 
 
 @two
 @safe(IndexError)
 def remove(index: IndexInt, tuples: Tuple[Val, ...]) -> Tuple[Val, ...]:
     """
     Recreate the `Tuple` without the element at the provided index
     """
     if index > (length := len(tuples)):
-        raise IndexError(f'Incompatible index {index} is greater than length {length}')
-    return tuples[:index] + tuples[index+1:] 
+        raise IndexError(f"Incompatible index {index} is greater than length {length}")
+    return tuples[:index] + tuples[index + 1 :]
 
 
 push_left = push(Side.LEFT)
 push_right = push(Side.RIGHT)
 extend_left = extend(Side.LEFT)
 extend_right = extend(Side.RIGHT)
 last = get(-1)
```

### Comparing `pythonix-1.0.2/pythonix/pipe.py` & `pythonix-1.0.3/pythonix/pipe.py`

 * *Files identical despite different names*

### Comparing `pythonix-1.0.2/pythonix/req.py` & `pythonix-1.0.3/pythonix/req.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,9 +28,9 @@
     post,
     put,
     set_data,
     set_headers,
     set_params,
     set_url,
     send,
-    Response
+    Response,
 )
```

### Comparing `pythonix-1.0.2/PKG-INFO` & `pythonix-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pythonix
-Version: 1.0.2
-Summary: 
+Version: 1.0.3
+Summary: Rust and Gleam like functional programming in Python, complete with Results, pipes, and currying
 Author: jhok2013
 Author-email: jhok2013@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # PYTHONIX
 
-A collection of functional modules in Python 12 inspired by Gleam and Rust.
+A collection of functional modules in Python 11 inspired by Gleam and Rust.
 If you have like functional programming, but have to program in Python, then check this out.
 
 ## Features
 
 1. Exceptions as values support similar to Rust
 2. Emphasis on immutable types
 3. Great support for immutable data structures
```

