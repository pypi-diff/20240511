# Comparing `tmp/kfslog-2.0.0.tar.gz` & `tmp/kfslog-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfslog-2.0.0.tar", max compression
+gzip compressed data, was "kfslog-2.0.1.tar", max compression
```

## Comparing `kfslog-2.0.0.tar` & `kfslog-2.0.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    25385 2024-05-09 22:13:13.920913 kfslog-2.0.0/KFSlog/KFSlog.py
--rw-r--r--   0        0        0      581 2024-05-09 22:13:13.920913 kfslog-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      631 2024-05-09 22:13:13.920913 kfslog-2.0.0/readme.md
--rw-r--r--   0        0        0     1222 1970-01-01 00:00:00.000000 kfslog-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    25451 2024-05-11 08:18:53.399704 kfslog-2.0.1/KFSlog/KFSlog.py
+-rw-r--r--   0        0        0      581 2024-05-11 08:18:53.399704 kfslog-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      631 2024-05-11 08:18:53.399704 kfslog-2.0.1/readme.md
+-rw-r--r--   0        0        0     1222 1970-01-01 00:00:00.000000 kfslog-2.0.1/PKG-INFO
```

### Comparing `kfslog-2.0.0/KFSlog/KFSlog.py` & `kfslog-2.0.1/KFSlog/KFSlog.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,15 +213,15 @@
         else:
             self.baseFilename=dt.datetime.now(dt.timezone.utc).strftime(self.baseFilename_format)
         return
 
 
 def timeit(executions: int=1) -> typing.Callable:
     """
-    If executions is 1: Decorates function with "Executing function()...", "Executed function().\\nΔt=t" and returns the decorated function's result.
+    If executions is 1: Decorates function with "Executing function()...", "Executed function().\\nΔt = t" and returns the decorated function's result.
     If executions is greater than 1: Executes function respective number of times and displays total, minimum, maximum, and average execution time, standard deviation, and function success rate, meaning the function has returned normally and not raised an exception. The function's results are returned in a list[result.Result] and have to be unwrapped by the caller.
 
     Arguments:
     - executions: number of times to execute function
 
     Returns:
     - decorated function's result, if multiple executions: all function's results wrapped in list[result.Result[...]]
@@ -272,43 +272,43 @@
                     exc_times.append((t1-t0).total_seconds())
                     results.append(result.Ok(function_result))  # append success result
 
             
             if executions==1:               # if only 1 execution: unwraps result
                 if results[0].is_ok():      # if success:
                     r=results[0].unwrap()
-                    logger.info(f"Executed \"{f.__name__}{inspect.signature(f)}\".\nΔt={KFSfstr.notation_tech(exc_times[0], 4)}s")
+                    logger.info(f"Executed \"{f.__name__}{inspect.signature(f)}\".\nΔt = {KFSfstr.notation_tech(exc_times[0], 4)}s")
                     logger.debug(f"Result: {r}")
                     return r
                 else:                       # if crash:
                     e=results[0].unwrap_err()
                     if f.__name__!="main":  # if not main crashed: error
-                        logger.error(f"Executing \"{f.__name__}{inspect.signature(f)}\" failed with {KFSfstr.full_class_name(e)}.\nΔt={KFSfstr.notation_tech(exc_times[0], 4)}s")
+                        logger.error(f"Executing \"{f.__name__}{inspect.signature(f)}\" failed with {KFSfstr.full_class_name(e)}.\nΔt = {KFSfstr.notation_tech(exc_times[0], 4)}s")
                     else:                   # if main crashed: critical
-                        logger.critical(f"Executing \"{f.__name__}{inspect.signature(f)}\" failed with {KFSfstr.full_class_name(e)}.\nΔt={KFSfstr.notation_tech(exc_times[0], 4)}s")
+                        logger.critical(f"Executing \"{f.__name__}{inspect.signature(f)}\" failed with {KFSfstr.full_class_name(e)}.\nΔt = {KFSfstr.notation_tech(exc_times[0], 4)}s")
                     raise e
             
             if 1<executions:    # if multiple executions: return list of results, caller has to unwrap them
                 logger.info(f"Executed \"{f.__name__}{inspect.signature(f)}\" {KFSfstr.notation_abs(executions, 0, round_static=True)} times.\n"+\
-                            f"ΔT={KFSfstr.notation_tech(sum(exc_times), 4)}s\n"+\
-                            f"Δt_min={KFSfstr.notation_tech(min(exc_times), 4)}s\n"+\
-                            f"Δt_max={KFSfstr.notation_tech(max(exc_times), 4)}s\n"+\
-                            f"Δt_avg={KFSfstr.notation_tech(sum(exc_times)/len(exc_times), 4)}s\n"+\
-                            f"σ={KFSfstr.notation_tech(math.sqrt(sum([(exc_time-sum(exc_times)/len(exc_times))**2 for exc_time in exc_times])/len(exc_times)), 4)}s\n"+\
-                            f"ok={KFSfstr.notation_abs(len([r for r in results if r.is_ok()]), 0, round_static=True)}/{KFSfstr.notation_abs(len(results), 0, round_static=True)} ({KFSfstr.notation_abs(len([r for r in results if r.is_ok()])/len(results), 2, round_static=True)})")
+                            f"ΔT     = {KFSfstr.notation_tech(sum(exc_times), 4)}s\n"+\
+                            f"Δt_min = {KFSfstr.notation_tech(min(exc_times), 4)}s\n"+\
+                            f"Δt_max = {KFSfstr.notation_tech(max(exc_times), 4)}s\n"+\
+                            f"Δt_avg = {KFSfstr.notation_tech(sum(exc_times)/len(exc_times), 4)}s\n"+\
+                            f"σ      = {KFSfstr.notation_tech(math.sqrt(sum([(exc_time-sum(exc_times)/len(exc_times))**2 for exc_time in exc_times])/len(exc_times)), 4)}s\n"+\
+                            f"ok     = {KFSfstr.notation_abs(len([r for r in results if r.is_ok()]), 0, round_static=True)}/{KFSfstr.notation_abs(len(results), 0, round_static=True)} ({KFSfstr.notation_abs(len([r for r in results if r.is_ok()])/len(results), 2, round_static=True)})")
                 logger.debug(f"Results: {results}")
                 return results
         
         return function_new # type:ignore
     return decorator
 
 
 def timeit_async(executions: int=1) -> typing.Callable:
     """
-    If executions is 1: Decorates function with "Executing function()...", "Executed function().\\nΔt=t" and returns the decorated function's result.
+    If executions is 1: Decorates function with "Executing function()...", "Executed function().\\nΔt = t" and returns the decorated function's result.
     If executions is greater than 1: Executes function respective number of times and displays total, minimum, maximum, and average execution time, standard deviation, and function success rate, meaning the function has returned normally and not raised an exception. The function's results are returned in a list[result.Result] and have to be unwrapped by the caller.
 
     Arguments:
     - executions: number of times to execute function
 
     Returns:
     - decorated function's result, if multiple executions: all function's results wrapped in list[result.Result[...]]
@@ -359,31 +359,31 @@
                     exc_times.append((t1-t0).total_seconds())
                     results.append(result.Ok(function_result))  # append success result
 
             
             if executions==1:               # if only 1 execution: unwraps result
                 if results[0].is_ok():      # if success:
                     r=results[0].unwrap()
-                    logger.info(f"Executed \"{f.__name__}{inspect.signature(f)}\".\nΔt={KFSfstr.notation_tech(exc_times[0], 4)}s")
+                    logger.info(f"Executed \"{f.__name__}{inspect.signature(f)}\".\nΔt = {KFSfstr.notation_tech(exc_times[0], 4)}s")
                     logger.debug(f"Result: {r}")
                     return r
                 else:                       # if crash:
                     e=results[0].unwrap_err()
                     if f.__name__!="main":  # if not main crashed: error
-                        logger.error(f"Executing \"{f.__name__}{inspect.signature(f)}\" failed with {KFSfstr.full_class_name(e)}.\nΔt={KFSfstr.notation_tech(exc_times[0], 4)}s")
+                        logger.error(f"Executing \"{f.__name__}{inspect.signature(f)}\" failed with {KFSfstr.full_class_name(e)}.\nΔt = {KFSfstr.notation_tech(exc_times[0], 4)}s")
                     else:                   # if main crashed: critical
-                        logger.critical(f"Executing \"{f.__name__}{inspect.signature(f)}\" failed with {KFSfstr.full_class_name(e)}.\nΔt={KFSfstr.notation_tech(exc_times[0], 4)}s")
+                        logger.critical(f"Executing \"{f.__name__}{inspect.signature(f)}\" failed with {KFSfstr.full_class_name(e)}.\nΔt = {KFSfstr.notation_tech(exc_times[0], 4)}s")
                     raise e
             
             if 1<executions:    # if multiple executions: return list of results, caller has to unwrap them
                 logger.info(f"Executed \"{f.__name__}{inspect.signature(f)}\" {KFSfstr.notation_abs(executions, 0, round_static=True)} times.\n"+\
-                            f"ΔT={KFSfstr.notation_tech(sum(exc_times), 4)}s\n"+\
-                            f"Δt_min={KFSfstr.notation_tech(min(exc_times), 4)}s\n"+\
-                            f"Δt_max={KFSfstr.notation_tech(max(exc_times), 4)}s\n"+\
-                            f"Δt_avg={KFSfstr.notation_tech(sum(exc_times)/len(exc_times), 4)}s\n"+\
-                            f"σ={KFSfstr.notation_tech(math.sqrt(sum([(exc_time-sum(exc_times)/len(exc_times))**2 for exc_time in exc_times])/len(exc_times)), 4)}s\n"+\
-                            f"ok={KFSfstr.notation_abs(len([r for r in results if r.is_ok()]), 0, round_static=True)}/{KFSfstr.notation_abs(len(results), 0, round_static=True)} ({KFSfstr.notation_abs(len([r for r in results if r.is_ok()])/len(results), 2, round_static=True)})")
+                            f"ΔT     = {KFSfstr.notation_tech(sum(exc_times), 4)}s\n"+\
+                            f"Δt_min = {KFSfstr.notation_tech(min(exc_times), 4)}s\n"+\
+                            f"Δt_max = {KFSfstr.notation_tech(max(exc_times), 4)}s\n"+\
+                            f"Δt_avg = {KFSfstr.notation_tech(sum(exc_times)/len(exc_times), 4)}s\n"+\
+                            f"σ      = {KFSfstr.notation_tech(math.sqrt(sum([(exc_time-sum(exc_times)/len(exc_times))**2 for exc_time in exc_times])/len(exc_times)), 4)}s\n"+\
+                            f"ok     = {KFSfstr.notation_abs(len([r for r in results if r.is_ok()]), 0, round_static=True)}/{KFSfstr.notation_abs(len(results), 0, round_static=True)} ({KFSfstr.notation_abs(len([r for r in results if r.is_ok()])/len(results), 2, round_static=True)})")
                 logger.debug(f"Results: {results}")
                 return results
         
         return function_new # type:ignore
     return decorator
```

### Comparing `kfslog-2.0.0/pyproject.toml` & `kfslog-2.0.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 authors     = ["9FS <pray4spam@googlemail.com>"]
 description = ""
 license     = "MIT"
 name        = "KFSlog"
 packages    = [{ include = "KFSlog" }]
 readme      = "readme.md"
 repository  = "https://github.com/9-FS/2023-09-20-KFSlog"
-version     = "2.0.0"
+version     = "2.0.1"
 
 [tool.poetry.dependencies]
 colorama = { version = "^0.4.6", optional = true }
 kfsfstr  = "^1.1.0"
 python   = "^3.12.0"
 result   = "^0.16.0"
```

### Comparing `kfslog-2.0.0/readme.md` & `kfslog-2.0.1/readme.md`

 * *Files identical despite different names*

### Comparing `kfslog-2.0.0/PKG-INFO` & `kfslog-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KFSlog
-Version: 2.0.0
+Version: 2.0.1
 Summary: 
 Home-page: https://github.com/9-FS/2023-09-20-KFSlog
 License: MIT
 Author: 9FS
 Author-email: pray4spam@googlemail.com
 Requires-Python: >=3.12.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

