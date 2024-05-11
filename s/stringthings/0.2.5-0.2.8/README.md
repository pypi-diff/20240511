# Comparing `tmp/stringthings-0.2.5.tar.gz` & `tmp/stringthings-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stringthings-0.2.5.tar", last modified: Sat Jan 27 16:07:18 2024, max compression
+gzip compressed data, was "stringthings-0.2.8.tar", last modified: Sat May 11 21:00:15 2024, max compression
```

## Comparing `stringthings-0.2.5.tar` & `stringthings-0.2.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-01-27 16:07:18.080000 stringthings-0.2.5/
--rw-rw-rw-   0        0        0     1077 2020-11-01 00:39:44.000000 stringthings-0.2.5/LICENSE
--rw-rw-rw-   0        0        0     3721 2024-01-27 16:07:20.000000 stringthings-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     1641 2024-01-27 12:09:10.000000 stringthings-0.2.5/README.md
--rw-rw-rw-   0        0        0      902 2024-01-27 16:05:56.000000 stringthings-0.2.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-27 16:07:20.000000 stringthings-0.2.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-01-27 16:07:18.090000 stringthings-0.2.5/src/
-drwxrwxrwx   0        0        0        0 2024-01-27 16:07:18.090000 stringthings-0.2.5/src/stringthings/
--rw-rw-rw-   0        0        0      557 2024-01-27 16:05:56.000000 stringthings-0.2.5/src/stringthings/__init__.py
--rw-rw-rw-   0        0        0     2635 2024-01-01 21:01:36.000000 stringthings-0.2.5/src/stringthings/compression.py
--rw-rw-rw-   0        0        0    20209 2024-01-27 12:13:06.000000 stringthings-0.2.5/src/stringthings/dates.py
--rw-rw-rw-   0        0        0      232 2024-01-27 12:09:10.000000 stringthings-0.2.5/src/stringthings/errors.py
--rw-rw-rw-   0        0        0     1592 2024-01-27 16:05:06.000000 stringthings-0.2.5/src/stringthings/filenames.py
--rw-rw-rw-   0        0        0     1659 2024-01-27 12:09:10.000000 stringthings-0.2.5/src/stringthings/numbers.py
--rw-rw-rw-   0        0        0     1944 2024-01-01 21:01:36.000000 stringthings-0.2.5/src/stringthings/splits.py
-drwxrwxrwx   0        0        0        0 2024-01-27 16:07:18.090000 stringthings-0.2.5/src/stringthings.egg-info/
--rw-rw-rw-   0        0        0     3721 2024-01-27 16:07:20.000000 stringthings-0.2.5/src/stringthings.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      474 2024-01-27 16:07:20.000000 stringthings-0.2.5/src/stringthings.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-27 16:07:20.000000 stringthings-0.2.5/src/stringthings.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-01-27 16:07:20.000000 stringthings-0.2.5/src/stringthings.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-01-27 16:07:20.000000 stringthings-0.2.5/src/stringthings.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-01-27 16:07:18.090000 stringthings-0.2.5/test/
--rw-rw-rw-   0        0        0      649 2024-01-01 21:01:36.000000 stringthings-0.2.5/test/test_compression.py
--rw-rw-rw-   0        0        0      123 2024-01-27 12:21:56.000000 stringthings-0.2.5/test/test_dates.py
+drwxrwxrwx   0        0        0        0 2024-05-11 21:00:15.310000 stringthings-0.2.8/
+-rw-rw-rw-   0        0        0     1077 2020-11-01 00:39:44.000000 stringthings-0.2.8/LICENSE
+-rw-rw-rw-   0        0        0     3721 2024-05-11 21:00:16.000000 stringthings-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1641 2024-01-27 12:09:10.000000 stringthings-0.2.8/README.md
+-rw-rw-rw-   0        0        0      902 2024-05-10 09:55:16.000000 stringthings-0.2.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-11 21:00:16.000000 stringthings-0.2.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-11 21:00:15.310000 stringthings-0.2.8/src/
+drwxrwxrwx   0        0        0        0 2024-05-11 21:00:15.320000 stringthings-0.2.8/src/stringthings/
+-rw-rw-rw-   0        0        0      557 2024-05-10 09:55:16.000000 stringthings-0.2.8/src/stringthings/__init__.py
+-rw-rw-rw-   0        0        0     2635 2024-01-01 21:01:36.000000 stringthings-0.2.8/src/stringthings/compression.py
+-rw-rw-rw-   0        0        0    20209 2024-01-27 12:13:06.000000 stringthings-0.2.8/src/stringthings/dates.py
+-rw-rw-rw-   0        0        0      232 2024-01-27 12:09:10.000000 stringthings-0.2.8/src/stringthings/errors.py
+-rw-rw-rw-   0        0        0     1647 2024-01-28 22:59:38.000000 stringthings-0.2.8/src/stringthings/filenames.py
+-rw-rw-rw-   0        0        0     1927 2024-05-10 09:55:16.000000 stringthings-0.2.8/src/stringthings/numbers.py
+-rw-rw-rw-   0        0        0     1944 2024-01-01 21:01:36.000000 stringthings-0.2.8/src/stringthings/splits.py
+drwxrwxrwx   0        0        0        0 2024-05-11 21:00:15.320000 stringthings-0.2.8/src/stringthings.egg-info/
+-rw-rw-rw-   0        0        0     3721 2024-05-11 21:00:16.000000 stringthings-0.2.8/src/stringthings.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      474 2024-05-11 21:00:16.000000 stringthings-0.2.8/src/stringthings.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 21:00:16.000000 stringthings-0.2.8/src/stringthings.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-11 21:00:16.000000 stringthings-0.2.8/src/stringthings.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-11 21:00:16.000000 stringthings-0.2.8/src/stringthings.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-11 21:00:15.320000 stringthings-0.2.8/test/
+-rw-rw-rw-   0        0        0      649 2024-01-01 21:01:36.000000 stringthings-0.2.8/test/test_compression.py
+-rw-rw-rw-   0        0        0      123 2024-01-27 12:21:56.000000 stringthings-0.2.8/test/test_dates.py
```

### Comparing `stringthings-0.2.5/LICENSE` & `stringthings-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `stringthings-0.2.5/PKG-INFO` & `stringthings-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stringthings
-Version: 0.2.5
+Version: 0.2.8
 Summary: some functions to work with strings.
 Author-email: Martin Carlos Araya <martinaraya@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Martín Carlos Araya
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: stringthings Version: 0.2.5 Summary: some functions
+Metadata-Version: 2.1 Name: stringthings Version: 0.2.8 Summary: some functions
 to work with strings. Author-email: Martin Carlos Araya
 gmail.com> License: MIT License Copyright (c) 2020 MartÃ­n Carlos Araya
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
```

### Comparing `stringthings-0.2.5/README.md` & `stringthings-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `stringthings-0.2.5/pyproject.toml` & `stringthings-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 00000010: 7265 7175 6972 6573 203d 205b 2273 6574  requires = ["set
 00000020: 7570 746f 6f6c 733e 3d36 312e 3022 5d0d  uptools>=61.0"].
 00000030: 0a62 7569 6c64 2d62 6163 6b65 6e64 203d  .build-backend =
 00000040: 2022 7365 7475 7074 6f6f 6c73 2e62 7569   "setuptools.bui
 00000050: 6c64 5f6d 6574 6122 0d0a 0d0a 5b70 726f  ld_meta"....[pro
 00000060: 6a65 6374 5d0d 0a6e 616d 6520 3d20 2273  ject]..name = "s
 00000070: 7472 696e 6774 6869 6e67 7322 0d0a 7665  tringthings"..ve
-00000080: 7273 696f 6e20 3d20 2230 2e32 2e35 220d  rsion = "0.2.5".
+00000080: 7273 696f 6e20 3d20 2230 2e32 2e38 220d  rsion = "0.2.8".
 00000090: 0a61 7574 686f 7273 203d 205b 0d0a 2020  .authors = [..  
 000000a0: 7b20 6e61 6d65 3d22 4d61 7274 696e 2043  { name="Martin C
 000000b0: 6172 6c6f 7320 4172 6179 6122 2c20 656d  arlos Araya", em
 000000c0: 6169 6c3d 226d 6172 7469 6e61 7261 7961  ail="martinaraya
 000000d0: 4067 6d61 696c 2e63 6f6d 2220 7d2c 0d0a  @gmail.com" },..
 000000e0: 5d0d 0a64 6573 6372 6970 7469 6f6e 203d  ]..description =
 000000f0: 2022 736f 6d65 2066 756e 6374 696f 6e73   "some functions
```

### Comparing `stringthings-0.2.5/src/stringthings/__init__.py` & `stringthings-0.2.8/src/stringthings/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*-coding: utf-8 -*-
 """
 Created on Mon Jan 01 13:53:33 2024
 
 @author: Martín Araya
 """
 
-__version__ = "0.2.5"
-__release__ = 20240127
+__version__ = "0.2.8"
+__release__ = 20240510
 
 from .dates import format_date, is_date, format_date as date
 from .numbers import is_numeric, get_number
 from .splits import multisplit, split_dmmmy
 from .compression import expand, compress
 from .filenames import extension
```

### Comparing `stringthings-0.2.5/src/stringthings/compression.py` & `stringthings-0.2.8/src/stringthings/compression.py`

 * *Files identical despite different names*

### Comparing `stringthings-0.2.5/src/stringthings/dates.py` & `stringthings-0.2.8/src/stringthings/dates.py`

 * *Files identical despite different names*

### Comparing `stringthings-0.2.5/src/stringthings/filenames.py` & `stringthings-0.2.8/src/stringthings/filenames.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*-coding: utf-8 -*-
 """
 Created on Mon Jan 01 13:53:33 2024
 
 @author: Martín Araya
 """
-from os.path import isfile, isdir, exists
+from os.path import isfile, isdir
 
 __all__ = ['extension']
 
 
 def extension(file_path: str, backslash_to_slash=True, back_compatibility=False):
     """
     receives a string indicating a FileName.Extension or
@@ -37,14 +37,16 @@
         file_name_ = file_path[len_path:len(file_path) - file_path[::-1].index('.') - 1]
         extension_ = file_path[len(file_path) - file_path[::-1].index('.') - 1:]
     else:
         file_name_ = file_path[len_path:]
         extension_ = ''
 
     fullpath_ = f"{path_}{file_name_}{extension_}".strip()
-    if not isfile(fullpath_) and extension_ == '':
+    if not isfile(fullpath_) and isdir(fullpath_):
         file_name_, extension_, path_= '', '', f"{path_}{file_name_}{extension_}"
+        if not path_.endswith('/'):
+            path_ += '/'
 
     if back_compatibility:
         return file_name_, extension_, path_, fullpath_
     else:
         return extension_, file_name_, path_, fullpath_
```

### Comparing `stringthings-0.2.5/src/stringthings/numbers.py` & `stringthings-0.2.8/src/stringthings/numbers.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 __all__ = ['is_numeric', 'get_number']
 
 
 def is_numeric(string):
     """
     returns True if the string is a number
     """
+    if type(string) in (int, float, complex):
+        return True
+    elif not type(string) is str:
+        string = str(string)
     if 'j' in string.lower():
         try:
             complex(string)
             return True
         except:
             return False
     else:
@@ -25,16 +29,19 @@
             return True
         except:
             return False
 
 
 def get_number(string):
     """
-    returns the number, as integer, float or complex, contained in a numeric string
+    Returns the number, as integer, float or complex, contained in a numeric string.
+    Raise ValueError if the string doesn't represent a number.
     """
+    if type(string) in (int, float, complex):
+        return string
     if is_numeric(string):
         string = string.lower()
         if 'j' in string:
             return complex(string)
         else:
             string = string.replace(' ', '').replace("'", '').replace(',', '.').strip('+')
             if string.endswith('-'):
```

### Comparing `stringthings-0.2.5/src/stringthings/splits.py` & `stringthings-0.2.8/src/stringthings/splits.py`

 * *Files identical despite different names*

### Comparing `stringthings-0.2.5/src/stringthings.egg-info/PKG-INFO` & `stringthings-0.2.8/src/stringthings.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stringthings
-Version: 0.2.5
+Version: 0.2.8
 Summary: some functions to work with strings.
 Author-email: Martin Carlos Araya <martinaraya@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Martín Carlos Araya
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: stringthings Version: 0.2.5 Summary: some functions
+Metadata-Version: 2.1 Name: stringthings Version: 0.2.8 Summary: some functions
 to work with strings. Author-email: Martin Carlos Araya
 gmail.com> License: MIT License Copyright (c) 2020 MartÃ­n Carlos Araya
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
```

### Comparing `stringthings-0.2.5/test/test_compression.py` & `stringthings-0.2.8/test/test_compression.py`

 * *Files identical despite different names*

