# Comparing `tmp/brukeropus-1.0.2.tar.gz` & `tmp/brukeropus-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brukeropus-1.0.2.tar", last modified: Sat May  4 18:07:30 2024, max compression
+gzip compressed data, was "brukeropus-1.0.3.tar", last modified: Sat May 11 02:18:02 2024, max compression
```

## Comparing `brukeropus-1.0.2.tar` & `brukeropus-1.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 18:07:30.440015 brukeropus-1.0.2/
--rw-rw-rw-   0        0        0     1087 2024-02-29 18:02:08.000000 brukeropus-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     5274 2024-05-04 18:07:30.440015 brukeropus-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4523 2024-05-03 14:26:32.000000 brukeropus-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 18:07:30.405367 brukeropus-1.0.2/brukeropus/
--rw-rw-rw-   0        0        0     2581 2024-05-03 13:47:15.000000 brukeropus-1.0.2/brukeropus/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 18:07:30.424361 brukeropus-1.0.2/brukeropus/control/
--rw-rw-rw-   0        0        0     1746 2024-04-24 01:13:04.000000 brukeropus-1.0.2/brukeropus/control/__init__.py
--rw-rw-rw-   0        0        0     9678 2024-04-23 16:48:27.000000 brukeropus-1.0.2/brukeropus/control/dde.py
--rw-rw-rw-   0        0        0    11639 2024-04-24 00:59:48.000000 brukeropus-1.0.2/brukeropus/control/opus.py
-drwxrwxrwx   0        0        0        0 2024-05-04 18:07:30.424361 brukeropus-1.0.2/brukeropus/file/
--rw-rw-rw-   0        0        0    17333 2024-04-23 18:20:14.000000 brukeropus-1.0.2/brukeropus/file/__init__.py
--rw-rw-rw-   0        0        0     9467 2024-03-05 15:18:18.000000 brukeropus-1.0.2/brukeropus/file/constants.py
--rw-rw-rw-   0        0        0    25809 2024-04-23 01:26:07.000000 brukeropus-1.0.2/brukeropus/file/file.py
--rw-rw-rw-   0        0        0    13119 2024-02-29 18:02:08.000000 brukeropus-1.0.2/brukeropus/file/parser.py
--rw-rw-rw-   0        0        0     9949 2024-02-29 18:02:08.000000 brukeropus-1.0.2/brukeropus/file/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-04 18:07:30.440015 brukeropus-1.0.2/brukeropus.egg-info/
--rw-rw-rw-   0        0        0     5274 2024-05-04 18:07:30.000000 brukeropus-1.0.2/brukeropus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      440 2024-05-04 18:07:30.000000 brukeropus-1.0.2/brukeropus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 18:07:30.000000 brukeropus-1.0.2/brukeropus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-04 18:07:30.000000 brukeropus-1.0.2/brukeropus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-04 18:07:30.000000 brukeropus-1.0.2/brukeropus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      816 2024-05-04 18:02:25.000000 brukeropus-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-04 18:07:30.440015 brukeropus-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-11 02:18:02.519623 brukeropus-1.0.3/
+-rw-rw-rw-   0        0        0     1087 2024-02-29 18:02:08.000000 brukeropus-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     5274 2024-05-11 02:18:02.519623 brukeropus-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4523 2024-05-03 14:26:32.000000 brukeropus-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 02:18:02.488390 brukeropus-1.0.3/brukeropus/
+-rw-rw-rw-   0        0        0     2581 2024-05-03 13:47:15.000000 brukeropus-1.0.3/brukeropus/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 02:18:02.504010 brukeropus-1.0.3/brukeropus/control/
+-rw-rw-rw-   0        0        0     1746 2024-04-24 01:13:04.000000 brukeropus-1.0.3/brukeropus/control/__init__.py
+-rw-rw-rw-   0        0        0     9678 2024-04-23 16:48:27.000000 brukeropus-1.0.3/brukeropus/control/dde.py
+-rw-rw-rw-   0        0        0    11639 2024-04-24 00:59:48.000000 brukeropus-1.0.3/brukeropus/control/opus.py
+drwxrwxrwx   0        0        0        0 2024-05-11 02:18:02.519623 brukeropus-1.0.3/brukeropus/file/
+-rw-rw-rw-   0        0        0    17333 2024-04-23 18:20:14.000000 brukeropus-1.0.3/brukeropus/file/__init__.py
+-rw-rw-rw-   0        0        0     9467 2024-03-05 15:18:18.000000 brukeropus-1.0.3/brukeropus/file/constants.py
+-rw-rw-rw-   0        0        0    26208 2024-05-11 02:14:16.000000 brukeropus-1.0.3/brukeropus/file/file.py
+-rw-rw-rw-   0        0        0    13123 2024-05-11 02:12:49.000000 brukeropus-1.0.3/brukeropus/file/parser.py
+-rw-rw-rw-   0        0        0     9949 2024-02-29 18:02:08.000000 brukeropus-1.0.3/brukeropus/file/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-11 02:18:02.519623 brukeropus-1.0.3/brukeropus.egg-info/
+-rw-rw-rw-   0        0        0     5274 2024-05-11 02:18:02.000000 brukeropus-1.0.3/brukeropus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      440 2024-05-11 02:18:02.000000 brukeropus-1.0.3/brukeropus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 02:18:02.000000 brukeropus-1.0.3/brukeropus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-11 02:18:02.000000 brukeropus-1.0.3/brukeropus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-11 02:18:02.000000 brukeropus-1.0.3/brukeropus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      816 2024-05-11 02:16:06.000000 brukeropus-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-11 02:18:02.519623 brukeropus-1.0.3/setup.cfg
```

### Comparing `brukeropus-1.0.2/LICENSE` & `brukeropus-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.2/PKG-INFO` & `brukeropus-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brukeropus
-Version: 1.0.2
+Version: 1.0.3
 Summary: A python package for communicating with Bruker OPUS spectroscopy software and reading its binary file format.
 Author-email: Josh Duran <josh.m.duran@gmail.com>
 Project-URL: Homepage, https://github.com/joshduran/brukeropus
 Project-URL: Issues, https://github.com/joshduran/brukeropus/issues
 Project-URL: Documentation, https://joshduran.github.io/brukeropus/brukeropus.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `brukeropus-1.0.2/README.md` & `brukeropus-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.2/brukeropus/__init__.py` & `brukeropus-1.0.3/brukeropus/__init__.py`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.2/brukeropus/control/__init__.py` & `brukeropus-1.0.3/brukeropus/control/__init__.py`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.2/brukeropus/control/dde.py` & `brukeropus-1.0.3/brukeropus/control/dde.py`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.2/brukeropus/control/opus.py` & `brukeropus-1.0.3/brukeropus/control/opus.py`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.2/brukeropus/file/__init__.py` & `brukeropus-1.0.3/brukeropus/file/__init__.py`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.2/brukeropus/file/constants.py` & `brukeropus-1.0.3/brukeropus/file/constants.py`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.2/brukeropus/file/file.py` & `brukeropus-1.0.3/brukeropus/file/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,20 +404,30 @@
             raise AttributeError(text)
 
     def __getitem__(self, item):
         return self._params.__getitem__(item)
 
     def _set_datetime(self):
         if 'dat' in self.keys() and 'tim' in self.keys():
-            date_str = self.dat
-            time_str = self.tim
-            dt_str = date_str + '-' + time_str[:time_str.index(' (')]
-            fmt = '%d/%m/%Y-%H:%M:%S.%f'
-            dt = datetime.datetime.strptime(dt_str, fmt)
-            self.datetime = dt
+            try:
+                date_str = self.dat
+                time_str = self.tim
+                dt_str = date_str + '-' + time_str[:time_str.index(' (')]
+                try:
+                    fmt = '%d/%m/%Y-%H:%M:%S.%f'
+                    dt = datetime.datetime.strptime(dt_str, fmt)
+                except:
+                    try:
+                        fmt = '%Y/%m/%d-%H:%M:%S.%f'
+                        dt = datetime.datetime.strptime(dt_str, fmt)
+                    except:
+                        self.datetime = None
+                self.datetime = dt
+            except:
+                self.datetime = None
         else:
             self.datetime = None
 
     def keys(self):
         '''Returns a `dict_keys` class of all valid keys in the class (i.e. dict.keys())'''
         return self._params.keys()
 
@@ -491,17 +501,17 @@
         data_str = ', '.join(data_keys)
         return 'File Directory: ' + str(self.num_blocks) + ' total blocks; data blocks: (' + data_str + ')'
 
     def _pair_data_and_status_blocks(self):
         for data_block in self.data_blocks:
             status_matches = [block for block in self.data_status_blocks if block.is_data_status_match(data_block)]
             if len(status_matches) == 0:
-                text = 'Warning: No data status block match for data block: ' + str(data_block)
-                + '\n\tdata block will be ignored.'
+                text = 'Warning: No data status block match for data block: ' + str(data_block) \
+                    + '\n\tdata block will be ignored.'
                 warnings.warn(text)
             elif len(status_matches) > 1:
-                text = 'Warning: Multiple data status block matches for data block: ' + str(data_block)
-                + '\n\tMatches:' + '; '.join([str(match) for match in status_matches])
-                + '\n\tdata block will be ignored.'
+                text = 'Warning: Multiple data status block matches for data block: ' + str(data_block) \
+                    + '\n\tMatches:' + '; '.join([str(match) for match in status_matches]) \
+                    + '\n\tdata block will be ignored.'
                 warnings.warn(text)
             else:
                 self.data_and_status_block_pairs.append((data_block, status_matches[0]))
```

### Comparing `brukeropus-1.0.2/brukeropus/file/parser.py` & `brukeropus-1.0.3/brukeropus/file/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,17 +140,17 @@
         else:
             fmt_str = '<'+str(val_size)+'s'
         try:
             val = struct.unpack_from(fmt_str, blockbytes, loc + 8)[0]
             if 's' in fmt_str:
                 x00_pos = val.find(b'\x00')
                 if x00_pos != -1:
-                    val = val[:x00_pos].decode('utf-8')
+                    val = val[:x00_pos].decode('latin-1')
                 else:
-                    val = val.decode('utf-8')
+                    val = val.decode('latin-1')
         except Exception as e:
             val = 'Failed to load: ' + str(e)
         yield key, val
         loc = loc + val_size + 8
 
 
 def get_dpf_dtype_count(dpf: int, size: int):
@@ -267,14 +267,14 @@
     '''
     byte_string = struct.unpack_from('<' + str(size) + 's', filebytes, start)[0]
     byte_strings = byte_string.split(b'\x00')
     strings = []
     for entry in byte_strings:
         if entry != b'':
             try:
-                strings.append(entry.decode('utf-8'))
+                strings.append(entry.decode('latin-1'))
             except Exception:
                 try:
-                    strings.append(entry.decode('latin-1'))
+                    strings.append(entry.decode('utf-8'))
                 except Exception as e:
                     strings.append('<Decode Exception>: ' + str(e))
     return strings
```

### Comparing `brukeropus-1.0.2/brukeropus/file/utils.py` & `brukeropus-1.0.3/brukeropus/file/utils.py`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.2/brukeropus.egg-info/PKG-INFO` & `brukeropus-1.0.3/brukeropus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brukeropus
-Version: 1.0.2
+Version: 1.0.3
 Summary: A python package for communicating with Bruker OPUS spectroscopy software and reading its binary file format.
 Author-email: Josh Duran <josh.m.duran@gmail.com>
 Project-URL: Homepage, https://github.com/joshduran/brukeropus
 Project-URL: Issues, https://github.com/joshduran/brukeropus/issues
 Project-URL: Documentation, https://joshduran.github.io/brukeropus/brukeropus.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `brukeropus-1.0.2/pyproject.toml` & `brukeropus-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "brukeropus"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Josh Duran", email="josh.m.duran@gmail.com" },
 ]
 description = "A python package for communicating with Bruker OPUS spectroscopy software and reading its binary file format."
 readme = "README.md"
 dependencies = ["numpy"]
 requires-python = ">=3.6"
```

