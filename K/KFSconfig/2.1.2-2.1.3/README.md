# Comparing `tmp/kfsconfig-2.1.2.tar.gz` & `tmp/kfsconfig-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfsconfig-2.1.2.tar", max compression
+gzip compressed data, was "kfsconfig-2.1.3.tar", max compression
```

## Comparing `kfsconfig-2.1.2.tar` & `kfsconfig-2.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    15698 2024-05-09 22:29:04.382243 kfsconfig-2.1.2/KFSconfig/KFSconfig.py
--rw-r--r--   0        0        0      514 2024-05-09 22:29:04.382243 kfsconfig-2.1.2/pyproject.toml
--rw-r--r--   0        0        0      668 2024-05-09 22:29:04.382243 kfsconfig-2.1.2/readme.md
--rw-r--r--   0        0        0     1185 1970-01-01 00:00:00.000000 kfsconfig-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0    15612 2024-05-11 21:43:13.411040 kfsconfig-2.1.3/KFSconfig/KFSconfig.py
+-rw-r--r--   0        0        0      514 2024-05-11 21:43:13.411040 kfsconfig-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0      668 2024-05-11 21:43:13.411040 kfsconfig-2.1.3/readme.md
+-rw-r--r--   0        0        0     1185 1970-01-01 00:00:00.000000 kfsconfig-2.1.3/PKG-INFO
```

### Comparing `kfsconfig-2.1.2/KFSconfig/KFSconfig.py` & `kfsconfig-2.1.3/KFSconfig/KFSconfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,14 @@
     logger.debug(config)
 
 
     if any(v==None for v in config.values())==True and setting_None_ok==False:                                                                                  # if any setting is still None and not allowed to be None: error
         logger.error(f"After going through all enabled sources, settings {[k for k, v in config.items() if v==None]} are still None and setting_None_ok is false.")
         
         if config_filepaths!=None and 1<=len(config_filepaths) and all([os.path.exists(config_filepath)==False for config_filepath in config_filepaths])==True: # if a file source is enabled and no files at set filepaths exist: offer creation of default config file at highest priority filepath using config_default's values
-            logger.info(f"None of the following filepaths exist: {config_filepaths}")
             match force_input(f"Would you like to create a default \"{config_filepaths[0]}\"? (y/n)"):
                 case "y":
                     try:
                         _create_default_file(config_filepaths[0], config_default)                                                                               # create default config file at highest priority filepath using config_default's values
                     except OSError:                                                                                                                             # if creating fails: error, if file already exists error because it should have been checked before
                         pass
                 case "n":
```

### Comparing `kfsconfig-2.1.2/pyproject.toml` & `kfsconfig-2.1.3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 authors     = ["9FS <pray4spam@googlemail.com>"]
 description = ""
 license     = "MIT"
 name        = "KFSconfig"
 packages    = [{ include = "KFSconfig" }]
 readme      = "readme.md"
 repository  = "https://github.com/9-FS/2023-09-20-KFSconfig"
-version     = "2.1.2"
+version     = "2.1.3"
 
 [tool.poetry.dependencies]
 kfslog = "^2.0.0"
 python = "^3.12.0"
 
 [tool.poetry.group.dev.dependencies]
 hypothesis = "^6.0.0"
```

### Comparing `kfsconfig-2.1.2/readme.md` & `kfsconfig-2.1.3/readme.md`

 * *Files identical despite different names*

### Comparing `kfsconfig-2.1.2/PKG-INFO` & `kfsconfig-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KFSconfig
-Version: 2.1.2
+Version: 2.1.3
 Summary: 
 Home-page: https://github.com/9-FS/2023-09-20-KFSconfig
 License: MIT
 Author: 9FS
 Author-email: pray4spam@googlemail.com
 Requires-Python: >=3.12.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

